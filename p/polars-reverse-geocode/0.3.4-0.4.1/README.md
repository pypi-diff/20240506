# Comparing `tmp/polars_reverse_geocode-0.3.4.tar.gz` & `tmp/polars_reverse_geocode-0.4.1.tar.gz`

## Comparing `polars_reverse_geocode-0.3.4.tar` & `polars_reverse_geocode-0.4.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 polars_reverse_geocode-0.3.4/Cargo.toml
--rw-r--r--   0     1001      127     3464 2024-03-26 13:00:31.000000 polars_reverse_geocode-0.3.4/.github/workflows/CI.yml
--rw-r--r--   0     1001      127       17 2024-03-26 13:00:31.000000 polars_reverse_geocode-0.3.4/.gitignore
--rw-r--r--   0     1001      127     5243 2024-03-26 13:00:31.000000 polars_reverse_geocode-0.3.4/CODE_OF_CONDUCT.md
--rw-r--r--   0     1001      127     1077 2024-03-26 13:00:31.000000 polars_reverse_geocode-0.3.4/LICENSE
--rw-r--r--   0     1001      127      701 2024-03-26 13:00:31.000000 polars_reverse_geocode-0.3.4/Makefile
--rw-r--r--   0     1001      127     1542 2024-03-26 13:00:31.000000 polars_reverse_geocode-0.3.4/README.md
--rw-r--r--   0     1001      127     1052 2024-03-26 13:00:31.000000 polars_reverse_geocode-0.3.4/polars_reverse_geocode/__init__.py
--rw-r--r--   0     1001      127        0 2024-03-26 13:00:31.000000 polars_reverse_geocode-0.3.4/polars_reverse_geocode/py.typed
--rw-r--r--   0     1001      127     2336 2024-03-26 13:00:31.000000 polars_reverse_geocode-0.3.4/polars_reverse_geocode/utils.py
--rw-r--r--   0     1001      127       32 2024-03-26 13:00:31.000000 polars_reverse_geocode-0.3.4/requirements.txt
--rw-r--r--   0     1001      127     3506 2024-03-26 13:00:31.000000 polars_reverse_geocode-0.3.4/src/expressions.rs
--rw-r--r--   0     1001      127      169 2024-03-26 13:00:31.000000 polars_reverse_geocode-0.3.4/src/lib.rs
--rw-r--r--   0     1001      127      713 2024-03-26 13:00:31.000000 polars_reverse_geocode-0.3.4/src/utils.rs
--rw-r--r--   0     1001      127      197 2024-03-26 13:00:31.000000 polars_reverse_geocode-0.3.4/t.py
--rw-r--r--   0     1001      127        0 2024-03-26 13:00:31.000000 polars_reverse_geocode-0.3.4/tests/__init__.py
--rw-r--r--   0     1001      127     1400 2024-03-26 13:00:31.000000 polars_reverse_geocode-0.3.4/tests/test_main.py
--rw-r--r--   0     1001      127    41107 2024-03-26 13:00:37.000000 polars_reverse_geocode-0.3.4/Cargo.lock
--rw-r--r--   0     1001      127      340 2024-03-26 13:00:31.000000 polars_reverse_geocode-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     1905 1970-01-01 00:00:00.000000 polars_reverse_geocode-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0      615 1970-01-01 00:00:00.000000 polars_reverse_geocode-0.4.1/Cargo.toml
+-rw-r--r--   0     1001      127     3463 2024-05-06 11:43:02.000000 polars_reverse_geocode-0.4.1/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127       17 2024-05-06 11:43:02.000000 polars_reverse_geocode-0.4.1/.gitignore
+-rw-r--r--   0     1001      127     5243 2024-05-06 11:43:02.000000 polars_reverse_geocode-0.4.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0     1001      127     1077 2024-05-06 11:43:02.000000 polars_reverse_geocode-0.4.1/LICENSE
+-rw-r--r--   0     1001      127      701 2024-05-06 11:43:02.000000 polars_reverse_geocode-0.4.1/Makefile
+-rw-r--r--   0     1001      127     1546 2024-05-06 11:43:02.000000 polars_reverse_geocode-0.4.1/README.md
+-rw-r--r--   0     1001      127     1210 2024-05-06 11:43:02.000000 polars_reverse_geocode-0.4.1/bump_version.py
+-rw-r--r--   0     1001      127     1068 2024-05-06 11:43:02.000000 polars_reverse_geocode-0.4.1/polars_reverse_geocode/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-06 11:43:02.000000 polars_reverse_geocode-0.4.1/polars_reverse_geocode/py.typed
+-rw-r--r--   0     1001      127     2336 2024-05-06 11:43:02.000000 polars_reverse_geocode-0.4.1/polars_reverse_geocode/utils.py
+-rw-r--r--   0     1001      127       32 2024-05-06 11:43:02.000000 polars_reverse_geocode-0.4.1/requirements.txt
+-rw-r--r--   0     1001      127     2636 2024-05-06 11:43:02.000000 polars_reverse_geocode-0.4.1/src/expressions.rs
+-rw-r--r--   0     1001      127      169 2024-05-06 11:43:02.000000 polars_reverse_geocode-0.4.1/src/lib.rs
+-rw-r--r--   0     1001      127      713 2024-05-06 11:43:02.000000 polars_reverse_geocode-0.4.1/src/utils.rs
+-rw-r--r--   0     1001      127      197 2024-05-06 11:43:02.000000 polars_reverse_geocode-0.4.1/t.py
+-rw-r--r--   0     1001      127        0 2024-05-06 11:43:02.000000 polars_reverse_geocode-0.4.1/tests/__init__.py
+-rw-r--r--   0     1001      127     1017 2024-05-06 11:43:02.000000 polars_reverse_geocode-0.4.1/tests/test_main.py
+-rw-r--r--   0     1001      127    43501 2024-05-06 11:43:10.000000 polars_reverse_geocode-0.4.1/Cargo.lock
+-rw-r--r--   0     1001      127      340 2024-05-06 11:43:02.000000 polars_reverse_geocode-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1909 1970-01-01 00:00:00.000000 polars_reverse_geocode-0.4.1/PKG-INFO
```

### Comparing `polars_reverse_geocode-0.3.4/.github/workflows/CI.yml` & `polars_reverse_geocode-0.4.1/.github/workflows/CI.yml`

 * *Files 5% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Set up Rust
         run: rustup show
       - uses: mozilla-actions/sccache-action@v0.0.3
       - run: make venv
-      - run: .venv/bin/python -m pip install polars==0.20.6  # min version
+      - run: venv/bin/python -m pip install polars==0.20.6  # min version
       - run: make install
       - run: make test
 
   linux:
     runs-on: ubuntu-latest
     strategy:
       matrix:
```

### Comparing `polars_reverse_geocode-0.3.4/CODE_OF_CONDUCT.md` & `polars_reverse_geocode-0.4.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `polars_reverse_geocode-0.3.4/LICENSE` & `polars_reverse_geocode-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_reverse_geocode-0.3.4/Makefile` & `polars_reverse_geocode-0.4.1/Makefile`

 * *Files identical despite different names*

### Comparing `polars_reverse_geocode-0.3.4/README.md` & `polars_reverse_geocode-0.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 ```
 
 ## Usage example
 
 ```python
 import polars as pl
 
-from polars_reverse_geocode import reverse_geocode
+from polars_reverse_geocode import find_closest_city
 
 df = pl.DataFrame({
     'lat': [37.7749, 51.01, 52.5],
     'lon': [-122.4194, -3.9, -.91]
 })
-print(df.with_columns(city=reverse_geocode('lat', 'lon')))
+print(df.with_columns(city=find_closest_city('lat', 'lon')))
 ```
 
 ```
 shape: (3, 3)
 ┌─────────┬───────────┬───────────────────┐
 │ lat     ┆ lon       ┆ city              │
 │ ---     ┆ ---       ┆ ---               │
```

### Comparing `polars_reverse_geocode-0.3.4/polars_reverse_geocode/utils.py` & `polars_reverse_geocode-0.4.1/polars_reverse_geocode/utils.py`

 * *Files identical despite different names*

### Comparing `polars_reverse_geocode-0.3.4/src/expressions.rs` & `polars_reverse_geocode-0.4.1/src/expressions.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 #![allow(clippy::unused_unit)]
-use h3o::{LatLng, Resolution};
 use polars::prelude::*;
 use polars_arrow::array::MutablePlString;
 use polars_core::utils::align_chunks_binary;
 use pyo3_polars::derive::polars_expr;
-use serde::Deserialize;
 use std::fmt::Write;
 
 use reverse_geocoder::ReverseGeocoder;
 
 #[polars_expr(output_type=String)]
 fn reverse_geocode(inputs: &[Series]) -> PolarsResult<Series> {
     let lhs = inputs[0].f64()?;
@@ -38,59 +36,32 @@
             mutarr.freeze().boxed()
         })
         .collect();
     let out: StringChunked = unsafe { ChunkedArray::from_chunks("placeholder", chunks) };
     Ok(out.into_series())
 }
 
-#[derive(Deserialize)]
-struct H3Kwargs {
-    resolution: u8,
-}
-
 #[polars_expr(output_type=String)]
-fn h3(inputs: &[Series], kwargs: H3Kwargs) -> PolarsResult<Series> {
+fn find_closest_state(inputs: &[Series]) -> PolarsResult<Series> {
     let lhs = inputs[0].f64()?;
     let rhs = inputs[1].f64()?;
-
-    let resolution = match kwargs.resolution {
-        1 => Resolution::One,
-        2 => Resolution::Two,
-        3 => Resolution::Three,
-        4 => Resolution::Four,
-        5 => Resolution::Five,
-        6 => Resolution::Six,
-        7 => Resolution::Seven,
-        8 => Resolution::Eight,
-        9 => Resolution::Nine,
-        10 => Resolution::Ten,
-        11 => Resolution::Eleven,
-        12 => Resolution::Twelve,
-        13 => Resolution::Thirteen,
-        14 => Resolution::Fourteen,
-        15 => Resolution::Fifteen,
-        _ => {
-            polars_bail!(InvalidOperation: "expected resolution between 1 and 15, got {}", kwargs.resolution)
-        }
-    };
+    let geocoder = ReverseGeocoder::new();
 
     let (lhs, rhs) = align_chunks_binary(lhs, rhs);
     let chunks = lhs
         .downcast_iter()
         .zip(rhs.downcast_iter())
         .map(|(lhs_arr, rhs_arr)| {
             let mut buf = String::new();
             let mut mutarr = MutablePlString::with_capacity(lhs_arr.len());
 
             for (lhs_opt_val, rhs_opt_val) in lhs_arr.iter().zip(rhs_arr.iter()) {
                 match (lhs_opt_val, rhs_opt_val) {
                     (Some(lhs_val), Some(rhs_val)) => {
-                        let coord = LatLng::new(*lhs_val, *rhs_val).expect("valid coord");
-                        let cell = coord.to_cell(resolution);
-                        let res = cell.to_string();
+                        let res = &geocoder.search((*lhs_val, *rhs_val)).record.admin1;
                         buf.clear();
                         write!(buf, "{res}").unwrap();
                         mutarr.push(Some(&buf))
                     }
                     _ => mutarr.push_null(),
                 }
             }
```

### Comparing `polars_reverse_geocode-0.3.4/src/utils.rs` & `polars_reverse_geocode-0.4.1/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_reverse_geocode-0.3.4/tests/test_main.py` & `polars_reverse_geocode-0.4.1/tests/test_main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import polars as pl
 from polars.testing import assert_frame_equal
 
-from polars_reverse_geocode import reverse_geocode, h3
+from polars_reverse_geocode import reverse_geocode, find_closest_state
 
 
 def test_main() -> None:
     df = pl.DataFrame({"lat": [37.7749, 51.01, 52.5], "lon": [-122.4194, -3.9, -0.91]})
     result = df.with_columns(city=reverse_geocode("lat", "lon"))
     expected = pl.DataFrame(
         {
@@ -13,29 +13,18 @@
             "lon": [-122.4194, -3.9, -0.91],
             "city": ["San Francisco", "South Molton", "Market Harborough"],
         }
     )
     assert_frame_equal(result, expected)
 
 
-def test_h3() -> None:
+def test_find_closest_state() -> None:
     df = pl.DataFrame({"lat": [37.7749, 51.01, 52.5], "lon": [-122.4194, -3.9, -0.91]})
-    result = df.with_columns(h3=h3("lat", "lon"))
+    result = df.with_columns(city=find_closest_state("lat", "lon"))
     expected = pl.DataFrame(
         {
             "lat": [37.7749, 51.01, 52.5],
             "lon": [-122.4194, -3.9, -0.91],
-            "h3": ["89283082803ffff", "89195b5b04fffff", "8919436a5d7ffff"],
-        }
-    )
-    assert_frame_equal(result, expected)
-
-    df = pl.DataFrame({"lat": [37.7749, 51.01, 52.5], "lon": [-122.4194, -3.9, -0.91]})
-    result = df.with_columns(h3=h3("lat", "lon", resolution=6))
-    expected = pl.DataFrame(
-        {
-            "lat": [37.7749, 51.01, 52.5],
-            "lon": [-122.4194, -3.9, -0.91],
-            "h3": ["86283082fffffff", "86195b5b7ffffff", "8619436a7ffffff"],
+            "city": ["California", "England", "England"],
         }
     )
     assert_frame_equal(result, expected)
```

### Comparing `polars_reverse_geocode-0.3.4/Cargo.lock` & `polars_reverse_geocode-0.4.1/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 [[package]]
 name = "ahash"
 version = "0.8.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d713b3834d76b85304d4d525563c1276e2e30dc97cc67bfb4585a4a29fc2c89f"
 dependencies = [
  "cfg-if",
- "const-random",
  "getrandom",
  "once_cell",
  "version_check",
  "zerocopy",
 ]
 
 [[package]]
@@ -29,22 +28,28 @@
 name = "allocator-api2"
 version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0942ffc6dcaadf03badf6e6a2d0228460359d5e34b57ccdc720b7382dfbd5ec5"
 
 [[package]]
 name = "argminmax"
-version = "0.6.1"
+version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "202108b46429b765ef483f8a24d5c46f48c14acfdacc086dd4ab6dddf6bcdbd2"
+checksum = "52424b59d69d69d5056d508b260553afd91c57e21849579cd1f50ee8b8b88eaa"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
+name = "array-init-cursor"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bf7d0a018de4f6aa429b9d33d69edf69072b1c5b1cb8d3e4a5f7ef898fc3eb76"
+
+[[package]]
 name = "atoi_simd"
 version = "0.15.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ae037714f313c1353189ead58ef9eec30a8e8dc101b2622d461418fd59e28a9"
 
 [[package]]
 name = "autocfg"
@@ -55,14 +60,20 @@
 [[package]]
 name = "az"
 version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b7e4c2464d97fe331d41de9d5db0def0a96f4d823b8b32a2efd503578988973"
 
 [[package]]
+name = "base64"
+version = "0.21.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
+
+[[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
@@ -129,34 +140,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5bc015644b92d5890fab7489e49d21f879d5c990186827d42ec511919404f38b"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
-name = "const-random"
-version = "0.1.18"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "87e00182fe74b066627d63b85fd550ac2998d4b0bd86bfed477a0ae4c7c71359"
-dependencies = [
- "const-random-macro",
-]
-
-[[package]]
-name = "const-random-macro"
-version = "0.1.16"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9d839f2a20b0aee515dc581a6172f2321f96cab76c1a38a4c584a194955390e"
-dependencies = [
- "getrandom",
- "once_cell",
- "tiny-keccak",
-]
-
-[[package]]
 name = "crossbeam-deque"
 version = "0.8.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "613f8cc01fe9cf1a3eb3d7f488fd2fa8388403e97039e2f73692932e291a770d"
 dependencies = [
  "crossbeam-epoch",
  "crossbeam-utils",
@@ -243,14 +234,20 @@
 [[package]]
 name = "ethnum"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b90ca2580b73ab6a1f724b76ca11ab632df820fd6040c336200d2c1df7b3c82c"
 
 [[package]]
+name = "fallible-streaming-iterator"
+version = "0.1.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7360491ce676a36bf9bb3c56c1aa791658183a54d2744120f27285738d90465a"
+
+[[package]]
 name = "fast-float"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95765f67b4b18863968b4a1bd5bb576f732b29a4a28c7cd84c09fa3e2875f33c"
 
 [[package]]
 name = "fixed"
@@ -262,20 +259,14 @@
  "bytemuck",
  "half",
  "num-traits",
  "typenum",
 ]
 
 [[package]]
-name = "float_eq"
-version = "1.0.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "28a80e3145d8ad11ba0995949bbcf48b9df2be62772b3d351ef017dff6ecb853"
-
-[[package]]
 name = "foreign_vec"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ee1b05cbd864bcaecbd3455d6d967862d446e4ebfc3c2e5e5b9841e53cba6673"
 
 [[package]]
 name = "generator"
@@ -300,33 +291,14 @@
  "js-sys",
  "libc",
  "wasi",
  "wasm-bindgen",
 ]
 
 [[package]]
-name = "h3o"
-version = "0.6.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "732921589aa26ebc91ba314ccbccc284d25a85b24a3bcd98dfa476fd8100bd85"
-dependencies = [
- "ahash",
- "either",
- "float_eq",
- "h3o-bit",
- "libm",
-]
-
-[[package]]
-name = "h3o-bit"
-version = "0.1.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6fb45e8060378c0353781abf67e1917b545a6b710d0342d85b70c125af7ef320"
-
-[[package]]
 name = "half"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bc52e53916c08643f1b56ec082790d1e86a32e58dc5268f897f313fbae7b4872"
 dependencies = [
  "cfg-if",
  "crunchy",
@@ -617,41 +589,60 @@
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-targets 0.48.5",
 ]
 
 [[package]]
+name = "parquet-format-safe"
+version = "0.2.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1131c54b167dd4e4799ce762e1ab01549ebb94d5bdd13e6ec1b467491c378e1f"
+
+[[package]]
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
 
 [[package]]
 name = "pin-project-lite"
 version = "0.2.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
 
 [[package]]
+name = "planus"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fc1691dd09e82f428ce8d6310bd6d5da2557c82ff17694d2a32cad7242aea89f"
+dependencies = [
+ "array-init-cursor",
+]
+
+[[package]]
 name = "polars"
-version = "0.37.0"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e43795c49010cb851d45227caa17769e83760e21d260ba6285c563b754e1652f"
+checksum = "0ea21b858b16b9c0e17a12db2800d11aa5b4bd182be6b3022eb537bbfc1f2db5"
 dependencies = [
  "getrandom",
+ "polars-arrow",
  "polars-core",
+ "polars-error",
+ "polars-parquet",
+ "polars-utils",
  "version_check",
 ]
 
 [[package]]
 name = "polars-arrow"
-version = "0.37.0"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "faacd21a2548fa6d50c72d6b8d4649a8e029a0f3c6c5545b7f436f0610e49b0f"
+checksum = "725b09f2b5ef31279b66e27bbab63c58d49d8f6696b66b1f46c7eaab95e80f75"
 dependencies = [
  "ahash",
  "atoi_simd",
  "bytemuck",
  "chrono",
  "dyn-clone",
  "either",
@@ -659,42 +650,55 @@
  "fast-float",
  "foreign_vec",
  "getrandom",
  "hashbrown",
  "itoa",
  "multiversion",
  "num-traits",
+ "polars-arrow-format",
  "polars-error",
  "polars-utils",
  "ryu",
  "simdutf8",
  "streaming-iterator",
  "strength_reduce",
  "version_check",
 ]
 
 [[package]]
+name = "polars-arrow-format"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "19b0ef2474af9396b19025b189d96e992311e6a47f90c53cd998b36c4c64b84c"
+dependencies = [
+ "planus",
+ "serde",
+]
+
+[[package]]
 name = "polars-compute"
-version = "0.37.0"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32d9dc87f8003ae0edeef5ad9ac92b2a345480bbe17adad64496113ae84706dd"
+checksum = "a796945b14b14fbb79b91ef0406e6fddca2be636e889f81ea5d6ee7d36efb4fe"
 dependencies = [
  "bytemuck",
+ "either",
  "num-traits",
  "polars-arrow",
  "polars-error",
  "polars-utils",
+ "strength_reduce",
  "version_check",
 ]
 
 [[package]]
 name = "polars-core"
-version = "0.37.0"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "befd4d280a82219a01035c4f901319ceba65998c594d0c64f9a439cdee1d7777"
+checksum = "465f70d3e96b6d0b1a43c358ba451286b8c8bd56696feff020d65702aa33e35c"
 dependencies = [
  "ahash",
  "bitflags 2.4.2",
  "bytemuck",
  "either",
  "hashbrown",
  "indexmap",
@@ -712,37 +716,38 @@
  "thiserror",
  "version_check",
  "xxhash-rust",
 ]
 
 [[package]]
 name = "polars-error"
-version = "0.37.0"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "50f2435b02d1ba36d8c1f6a722cad04e4c0b2705a3112c5706e6960d405d7798"
+checksum = "5224d5d05e6b8a6f78b75951ae1b5f82c8ab1979e11ffaf5fd41941e3d5b0757"
 dependencies = [
+ "polars-arrow-format",
  "simdutf8",
  "thiserror",
 ]
 
 [[package]]
 name = "polars-ffi"
-version = "0.37.0"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f02331289626c8894e7b68467cd2de84d010f90def9bdd479e00e4fbafced7a9"
+checksum = "dcdd5a0b45dea8df72db9dfca694a1acc753bd868f3a751903b83cacdb896d2b"
 dependencies = [
  "polars-arrow",
  "polars-core",
 ]
 
 [[package]]
 name = "polars-io"
-version = "0.37.0"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b51fba2cf014cb39c2b38353d601540fb9db643be65abb9ca8ff44b9c4c4a88e"
+checksum = "b2c8589e418cbe4a48228d64b2a8a40284a82ec3c98817c0c2bcc0267701338b"
 dependencies = [
  "ahash",
  "bytes",
  "home",
  "memchr",
  "memmap2",
  "num-traits",
@@ -755,17 +760,17 @@
  "rayon",
  "regex",
  "smartstring",
 ]
 
 [[package]]
 name = "polars-ops"
-version = "0.37.0"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6395f5fd5e1adf016fd6403c0a493181c1a349a7a145b2687cdf50a0d630310a"
+checksum = "efdbdb4d9a92109bc2e0ce8e17af5ae8ab643bb5b7ee9d1d74f0aeffd1fbc95f"
 dependencies = [
  "ahash",
  "argminmax",
  "bytemuck",
  "either",
  "hashbrown",
  "indexmap",
@@ -779,78 +784,107 @@
  "rayon",
  "regex",
  "smartstring",
  "version_check",
 ]
 
 [[package]]
+name = "polars-parquet"
+version = "0.39.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b421d2196f786fdfe162db614c8485f8308fe41575d4de634a39bbe460d1eb6a"
+dependencies = [
+ "ahash",
+ "base64",
+ "ethnum",
+ "num-traits",
+ "parquet-format-safe",
+ "polars-arrow",
+ "polars-error",
+ "polars-utils",
+ "seq-macro",
+ "simdutf8",
+ "streaming-decompression",
+]
+
+[[package]]
 name = "polars-plan"
-version = "0.37.0"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7fb7d7527be2aa33baace9000f6772eb9df7cd57ec010a4b273435d2dc1349e8"
+checksum = "2fb8e2302e20c44defd5be8cad9c96e75face63c3a5f609aced8c4ec3b3ac97d"
 dependencies = [
  "ahash",
  "bytemuck",
+ "hashbrown",
  "once_cell",
  "percent-encoding",
  "polars-arrow",
  "polars-core",
  "polars-io",
  "polars-ops",
  "polars-utils",
  "rayon",
+ "recursive",
  "smartstring",
  "strum_macros",
  "version_check",
 ]
 
 [[package]]
 name = "polars-reverse-geocode"
-version = "0.3.4"
+version = "0.4.1"
 dependencies = [
- "h3o",
  "jemallocator",
  "polars",
  "polars-arrow",
  "pyo3",
  "pyo3-polars",
  "reverse_geocoder",
  "serde",
 ]
 
 [[package]]
 name = "polars-row"
-version = "0.37.0"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f4984d97aad3d0db92afe76ebcab10b5e37a1216618b5703ae0d2917ccd6168c"
+checksum = "a515bdc68c2ae3702e3de70d89601f3b71ca8137e282a226dddb53ee4bacfa2e"
 dependencies = [
+ "bytemuck",
  "polars-arrow",
  "polars-error",
  "polars-utils",
 ]
 
 [[package]]
 name = "polars-utils"
-version = "0.37.0"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "38f9c955bb1e9b55d835aeb7fe4e4e8826e01abe5f0ada979ceb7d2b9af7b569"
+checksum = "c760b6c698cfe2fbbbd93d6cfb408db14ececfe1d92445dae2229ce1b5b21ae8"
 dependencies = [
  "ahash",
  "bytemuck",
  "hashbrown",
  "indexmap",
  "num-traits",
  "once_cell",
  "polars-error",
+ "raw-cpuid",
  "rayon",
  "smartstring",
+ "stacker",
  "version_check",
 ]
 
 [[package]]
+name = "portable-atomic"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
+
+[[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
@@ -858,96 +892,107 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2422ad645d89c99f8f3e6b88a9fdeca7fabeac836b1002371c4367c8f984aae"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
+name = "psm"
+version = "0.1.21"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5787f7cda34e3033a72192c018bc5883100330f362ef279a8cbccfce8bb4e874"
+dependencies = [
+ "cc",
+]
+
+[[package]]
 name = "pyo3"
-version = "0.20.2"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a89dc7a5850d0e983be1ec2a463a171d20990487c3cfcd68b5363f1ee3d6fe0"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
+ "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.20.2"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "07426f0d8fe5a601f26293f300afd1a7b1ed5e78b2a705870c5f30893c5163be"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.20.2"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dbb7dec17e17766b46bca4f1a4215a85006b4c2ecde122076c562dd058da6cf1"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.20.2"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05f738b4e40d50b5711957f142878cfa0f28e054aa0ebdfc3fd137a843f74ed3"
+checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 2.0.50",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.20.2"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fc910d4851847827daf9d6cdd4a823fbdaab5b8818325c5e97a86da79e8881f"
+checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
  "heck",
  "proc-macro2",
+ "pyo3-build-config",
  "quote",
  "syn 2.0.50",
 ]
 
 [[package]]
 name = "pyo3-polars"
-version = "0.11.3"
+version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7fa311764163c831c75f9ca49499abacbf7ece676cad0b059d962a384aa18224"
+checksum = "469bd1d378fb3a34c1b182383e84741d9e7c5451a5d29a3f9c557aac161876cd"
 dependencies = [
  "polars",
  "polars-core",
  "polars-ffi",
  "polars-plan",
  "pyo3",
  "pyo3-polars-derive",
  "serde",
  "serde-pickle",
  "thiserror",
 ]
 
 [[package]]
 name = "pyo3-polars-derive"
-version = "0.5.0"
+version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e654e869ba1b0b440dde8e11890fb3578fccd75a4b007672e44eed70071517b4"
+checksum = "3ba3d428667917efd2c233534db5779f55b398e123aea75243da8491856e1131"
 dependencies = [
  "polars-core",
  "polars-ffi",
  "polars-plan",
  "proc-macro2",
  "quote",
  "syn 2.0.50",
@@ -999,18 +1044,27 @@
 checksum = "32cb0b9bc82b0a0876c2dd994a7e7a2683d3e7390ca40e6886785ef0c7e3ee31"
 dependencies = [
  "num-traits",
  "rand",
 ]
 
 [[package]]
+name = "raw-cpuid"
+version = "11.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e29830cbb1290e404f24c73af91c5d8d631ce7e128691e9477556b540cd01ecd"
+dependencies = [
+ "bitflags 2.4.2",
+]
+
+[[package]]
 name = "rayon"
-version = "1.8.1"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa7237101a77a10773db45d62004a272517633fbcc3df19d96455ede1122e051"
+checksum = "b418a60154510ca1a002a752ca9714984e21e4241e804d32555251faf8b78ffa"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
@@ -1019,14 +1073,34 @@
 checksum = "1465873a3dfdaa8ae7cb14b4383657caab0b3e8a0aa9ae8e04b044854c8dfce2"
 dependencies = [
  "crossbeam-deque",
  "crossbeam-utils",
 ]
 
 [[package]]
+name = "recursive"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0786a43debb760f491b1bc0269fe5e84155353c67482b9e60d0cfb596054b43e"
+dependencies = [
+ "recursive-proc-macro-impl",
+ "stacker",
+]
+
+[[package]]
+name = "recursive-proc-macro-impl"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "76009fbe0614077fc1a2ce255e3a1881a2e3a3527097d5dc6d8212c585e7e38b"
+dependencies = [
+ "quote",
+ "syn 2.0.50",
+]
+
+[[package]]
 name = "redox_syscall"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags 1.3.2",
 ]
@@ -1087,14 +1161,20 @@
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
+name = "seq-macro"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a3f0bf26fd526d2a95683cd0f87bf103b8539e2ca1ef48ce002d67aad59aa0b4"
+
+[[package]]
 name = "serde"
 version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
 dependencies = [
  "serde_derive",
 ]
@@ -1158,20 +1238,42 @@
 [[package]]
 name = "sorted-vec"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c6734caf0b6f51addd5eeacca12fb39b2c6c14e8d4f3ac42f3a78955c0467458"
 
 [[package]]
+name = "stacker"
+version = "0.1.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c886bd4480155fd3ef527d45e9ac8dd7118a898a46530b7b94c3e21866259fce"
+dependencies = [
+ "cc",
+ "cfg-if",
+ "libc",
+ "psm",
+ "winapi",
+]
+
+[[package]]
 name = "static_assertions"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
 
 [[package]]
+name = "streaming-decompression"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bf6cc3b19bfb128a8ad11026086e31d3ce9ad23f8ea37354b31383a187c44cf3"
+dependencies = [
+ "fallible-streaming-iterator",
+]
+
+[[package]]
 name = "streaming-iterator"
 version = "0.1.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b2231b7c3057d5e4ad0156fb3dc807d900806020c5ffa3ee6ff2c8c76fb8520"
 
 [[package]]
 name = "strength_reduce"
@@ -1253,23 +1355,14 @@
 checksum = "3fdd6f064ccff2d6567adcb3873ca630700f00b5ad3f060c25b5dcfd9a4ce152"
 dependencies = [
  "cfg-if",
  "once_cell",
 ]
 
 [[package]]
-name = "tiny-keccak"
-version = "2.0.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2c9d3793400a45f954c52e73d068316d76b6f4e36977e3fcebb13a2721e80237"
-dependencies = [
- "crunchy",
-]
-
-[[package]]
 name = "tracing"
 version = "0.1.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c3523ab5a71916ccf420eebdf5521fcef02141234bbc0b8a49f2fdc4544364ef"
 dependencies = [
  "pin-project-lite",
  "tracing-attributes",
```

### Comparing `polars_reverse_geocode-0.3.4/PKG-INFO` & `polars_reverse_geocode-0.4.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: polars-reverse-geocode
-Version: 0.3.4
+Version: 0.4.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
@@ -21,21 +21,21 @@
 ```
 
 ## Usage example
 
 ```python
 import polars as pl
 
-from polars_reverse_geocode import reverse_geocode
+from polars_reverse_geocode import find_closest_city
 
 df = pl.DataFrame({
     'lat': [37.7749, 51.01, 52.5],
     'lon': [-122.4194, -3.9, -.91]
 })
-print(df.with_columns(city=reverse_geocode('lat', 'lon')))
+print(df.with_columns(city=find_closest_city('lat', 'lon')))
 ```
 
 ```
 shape: (3, 3)
 ┌─────────┬───────────┬───────────────────┐
 │ lat     ┆ lon       ┆ city              │
 │ ---     ┆ ---       ┆ ---               │
```

