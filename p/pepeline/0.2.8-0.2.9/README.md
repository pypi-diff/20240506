# Comparing `tmp/pepeline-0.2.8.tar.gz` & `tmp/pepeline-0.2.9.tar.gz`

## Comparing `pepeline-0.2.8.tar` & `pepeline-0.2.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      568 1970-01-01 00:00:00.000000 pepeline-0.2.8/Cargo.toml
--rw-r--r--   0     1001      127     2162 2024-04-29 11:08:29.000000 pepeline-0.2.8/.github/workflows/CI.yml
--rw-r--r--   0     1001      127     2844 2024-04-29 11:08:29.000000 pepeline-0.2.8/.github/workflows/pipl.yml
--rw-r--r--   0     1001      127      686 2024-04-29 11:08:29.000000 pepeline-0.2.8/.gitignore
--rw-r--r--   0     1001      127     1065 2024-04-29 11:08:29.000000 pepeline-0.2.8/LICENSE
--rw-r--r--   0     1001      127      781 2024-04-29 11:08:29.000000 pepeline-0.2.8/README.md
--rw-r--r--   0     1001      127     1827 2024-04-29 11:08:29.000000 pepeline-0.2.8/pepeline.pyi
--rw-r--r--   0     1001      127      629 2024-04-29 11:08:29.000000 pepeline-0.2.8/src/lib.rs
--rw-r--r--   0     1001      127      977 2024-04-29 11:08:29.000000 pepeline-0.2.8/src/utils/core/color_levels.rs
--rw-r--r--   0     1001      127     2195 2024-04-29 11:08:29.000000 pepeline-0.2.8/src/utils/core/convert.rs
--rw-r--r--   0     1001      127     1274 2024-04-29 11:08:29.000000 pepeline-0.2.8/src/utils/core/noise.rs
--rw-r--r--   0     1001      127     3295 2024-04-29 11:08:29.000000 pepeline-0.2.8/src/utils/functions/core_funcion.rs
--rw-r--r--   0     1001      127     2463 2024-04-29 11:08:29.000000 pepeline-0.2.8/src/utils/functions/img_function.rs
--rw-r--r--   0     1001      127      878 2024-04-29 11:08:29.000000 pepeline-0.2.8/src/utils/functions/screentone_function.rs
--rw-r--r--   0     1001      127    10344 2024-04-29 11:08:29.000000 pepeline-0.2.8/src/utils/image/decode.rs
--rw-r--r--   0     1001      127     1254 2024-04-29 11:08:29.000000 pepeline-0.2.8/src/utils/image/save.rs
--rw-r--r--   0     1001      127      341 2024-04-29 11:08:29.000000 pepeline-0.2.8/src/utils/mod.rs
--rw-r--r--   0     1001      127     1353 2024-04-29 11:08:29.000000 pepeline-0.2.8/src/utils/screentone/dot.rs
--rw-r--r--   0     1001      127      986 2024-04-29 11:08:29.000000 pepeline-0.2.8/src/utils/screentone/screentone_add.rs
--rw-r--r--   0     1001      127    34652 2024-04-29 11:08:42.000000 pepeline-0.2.8/Cargo.lock
--rw-r--r--   0     1001      127      428 2024-04-29 11:08:29.000000 pepeline-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     1160 1970-01-01 00:00:00.000000 pepeline-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      568 1970-01-01 00:00:00.000000 pepeline-0.2.9/Cargo.toml
+-rw-r--r--   0     1001      127     2162 2024-05-04 23:21:51.000000 pepeline-0.2.9/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127     2844 2024-05-04 23:21:51.000000 pepeline-0.2.9/.github/workflows/pipl.yml
+-rw-r--r--   0     1001      127      686 2024-05-04 23:21:51.000000 pepeline-0.2.9/.gitignore
+-rw-r--r--   0     1001      127     1065 2024-05-04 23:21:51.000000 pepeline-0.2.9/LICENSE
+-rw-r--r--   0     1001      127      781 2024-05-04 23:21:51.000000 pepeline-0.2.9/README.md
+-rw-r--r--   0     1001      127     1977 2024-05-04 23:21:51.000000 pepeline-0.2.9/pepeline.pyi
+-rw-r--r--   0     1001      127      697 2024-05-04 23:21:51.000000 pepeline-0.2.9/src/lib.rs
+-rw-r--r--   0     1001      127     1035 2024-05-04 23:21:51.000000 pepeline-0.2.9/src/utils/core/color_levels.rs
+-rw-r--r--   0     1001      127     2758 2024-05-04 23:21:51.000000 pepeline-0.2.9/src/utils/core/convert.rs
+-rw-r--r--   0     1001      127     1258 2024-05-04 23:21:51.000000 pepeline-0.2.9/src/utils/core/noise.rs
+-rw-r--r--   0     1001      127     4776 2024-05-04 23:21:51.000000 pepeline-0.2.9/src/utils/functions/core_funcion.rs
+-rw-r--r--   0     1001      127     2463 2024-05-04 23:21:51.000000 pepeline-0.2.9/src/utils/functions/img_function.rs
+-rw-r--r--   0     1001      127      878 2024-05-04 23:21:51.000000 pepeline-0.2.9/src/utils/functions/screentone_function.rs
+-rw-r--r--   0     1001      127    10953 2024-05-04 23:21:51.000000 pepeline-0.2.9/src/utils/image/decode.rs
+-rw-r--r--   0     1001      127     1254 2024-05-04 23:21:51.000000 pepeline-0.2.9/src/utils/image/save.rs
+-rw-r--r--   0     1001      127      341 2024-05-04 23:21:51.000000 pepeline-0.2.9/src/utils/mod.rs
+-rw-r--r--   0     1001      127     1353 2024-05-04 23:21:51.000000 pepeline-0.2.9/src/utils/screentone/dot.rs
+-rw-r--r--   0     1001      127      986 2024-05-04 23:21:51.000000 pepeline-0.2.9/src/utils/screentone/screentone_add.rs
+-rw-r--r--   0     1001      127    34652 2024-05-04 23:21:56.000000 pepeline-0.2.9/Cargo.lock
+-rw-r--r--   0     1001      127      428 2024-05-04 23:21:51.000000 pepeline-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     1160 1970-01-01 00:00:00.000000 pepeline-0.2.9/PKG-INFO
```

### Comparing `pepeline-0.2.8/Cargo.toml` & `pepeline-0.2.9/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pepeline"
-version = "0.2.8"
+version = "0.2.9"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "pepeline"
 crate-type = ["cdylib"]
```

### Comparing `pepeline-0.2.8/.github/workflows/CI.yml` & `pepeline-0.2.9/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pepeline-0.2.8/.github/workflows/pipl.yml` & `pepeline-0.2.9/.github/workflows/pipl.yml`

 * *Files identical despite different names*

### Comparing `pepeline-0.2.8/.gitignore` & `pepeline-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pepeline-0.2.8/LICENSE` & `pepeline-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pepeline-0.2.8/README.md` & `pepeline-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `pepeline-0.2.8/pepeline.pyi` & `pepeline-0.2.9/pepeline.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -30,14 +30,18 @@
     PERLIN = 0,
     SIMPLEX = 1,
     OPENSIMPLEX = 2,
     SUPERSIMPLEX = 3,
     PERLINSURFLET = 4
 
 
+def crop_cord(array: np.ndarray) -> (
+int, int, int, int): "returns image coordinates not equal to 0, made for cropping using the Laplace operator"
+
+
 def fast_color_level(
         array: np.ndarray,
         in_low: None | int,
         in_high: None | int,
         out_low: None | int,
         out_high: None | int,
         gamma: None | float,
```

### Comparing `pepeline-0.2.8/src/lib.rs` & `pepeline-0.2.9/src/lib.rs`

 * *Files 9% similar despite different names*

```diff
@@ -8,10 +8,11 @@
 #[pymodule]
 fn pepeline(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(img_function::read, m)?)?;
     m.add_function(wrap_pyfunction!(screentone_function::screentone, m)?)?;
     m.add_function(wrap_pyfunction!(core_funcion::fast_color_level, m)?)?;
     m.add_function(wrap_pyfunction!(core_funcion::noise_generate, m)?)?;
     m.add_function(wrap_pyfunction!(img_function::save, m)?)?;
+    m.add_function(wrap_pyfunction!(core_funcion::crop_cord, m)?)?;
     m.add_class::<core_funcion::TypeNoise>()?;
     Ok(())
 }
```

### Comparing `pepeline-0.2.8/src/utils/core/color_levels.rs` & `pepeline-0.2.9/src/utils/core/color_levels.rs`

 * *Files 10% similar despite different names*

```diff
@@ -20,12 +20,16 @@
                 .max(0.0)
                 .min(1.0)
                 .powf(gamma)
         })
     } else if gamma != 1.0 {
         array.mapv(|x| ((x - in_low) / (in_range)).max(0.0).min(1.0).powf(gamma))
     } else if gamma == 1.0 && out_range != 1.0 {
-        array.mapv(|x| ((x - in_low) / (in_range) * (out_range) + out_low).max(0.0).min(1.0))
+        array.mapv(|x| {
+            ((x - in_low) / (in_range) * (out_range) + out_low)
+                .max(0.0)
+                .min(1.0)
+        })
     } else {
         array.mapv(|x| ((x - in_low) / (in_range)).max(0.0).min(1.0))
     }
 }
```

### Comparing `pepeline-0.2.8/src/utils/core/convert.rs` & `pepeline-0.2.9/src/utils/core/convert.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+use std::cmp::min;
+
 use image::{GrayImage, RgbImage};
 use ndarray::{Array2, Array3};
 
 pub(crate) fn rgb8_to_gray8(rgb: &[u8]) -> Vec<u8> {
     let mut gray_float: Vec<u8> = Vec::with_capacity(rgb.len() / 3);
     for chunk in rgb.chunks(3) {
         gray_float.push(
@@ -30,14 +32,30 @@
             b as f32 * 0.00392156862745f32
         }
     });
 
     floats
 }
 
+pub(crate) fn u16_to_f32(bytes: &[u8]) -> Vec<f32> {
+    let mut img_float: Vec<f32> = Vec::with_capacity(bytes.len() / 2);
+    for chunk in bytes.chunks(2) {
+        img_float.push(min(255, (chunk[0] as u16 + chunk[1] as u16 * 255) / 255) as f32 / 255.0)
+    }
+    img_float
+}
+
+pub(crate) fn u16_to_u8(bytes: &[u8]) -> Vec<u8> {
+    let mut img_uint: Vec<u8> = Vec::with_capacity(bytes.len() / 2);
+    for chunk in bytes.chunks(2) {
+        img_uint.push(min(255, (chunk[0] as u16 + chunk[1] as u16 * 255) / 255) as u8)
+    }
+    img_uint
+}
+
 pub(crate) fn f32_to_u8(bytes: &[f32]) -> Vec<u8> {
     let mut floats = vec![0; bytes.len()];
     floats
         .iter_mut()
         .zip(bytes.iter())
         .for_each(|(f, &b)| *f = if b == 0.0 { b as u8 } else { (b * 255.0) as u8 });
     floats
```

### Comparing `pepeline-0.2.8/src/utils/core/noise.rs` & `pepeline-0.2.9/src/utils/core/noise.rs`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
     noise_fn: &T,
     x: usize,
     y: usize,
     octaves: u8,
     frequency: f64,
     lacunarity: f64,
 ) -> f32
-    where
-        T: NoiseFn<f64, 2>,
+where
+    T: NoiseFn<f64, 2>,
 {
     let mut total = 0.0;
     let mut frequency = frequency;
     let mut amplitude = 1.0;
     let mut max_amplitude = 0.0;
 
     for _ in 0..octaves {
@@ -35,16 +35,16 @@
     x: usize,
     y: usize,
     z: usize,
     octaves: u8,
     frequency: f64,
     lacunarity: f64,
 ) -> f32
-    where
-        T: NoiseFn<f64, 3>,
+where
+    T: NoiseFn<f64, 3>,
 {
     let mut total = 0.0;
     let mut frequency = frequency;
     let mut amplitude = 1.0;
     let mut max_amplitude = 0.0;
 
     for _ in 0..octaves {
```

### Comparing `pepeline-0.2.8/src/utils/functions/img_function.rs` & `pepeline-0.2.9/src/utils/functions/img_function.rs`

 * *Files identical despite different names*

### Comparing `pepeline-0.2.8/src/utils/functions/screentone_function.rs` & `pepeline-0.2.9/src/utils/functions/screentone_function.rs`

 * *Files identical despite different names*

### Comparing `pepeline-0.2.8/src/utils/image/decode.rs` & `pepeline-0.2.9/src/utils/image/decode.rs`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 use ndarray::{Array2, Array3, ArrayD};
 use zune_jpeg::JpegDecoder;
 use zune_jpeg::zune_core::colorspace::ColorSpace;
 use zune_jpeg::zune_core::options::DecoderOptions;
 use zune_psd::PSDDecoder;
 
 use crate::utils::core::convert::{
-    luma2array, luma2arrayf32, rgb2array, rgb2arrayf32, rgb8_to_gray32, rgb8_to_gray8, u8_to_f32,
+    luma2array, luma2arrayf32, rgb2array, rgb2arrayf32, rgb8_to_gray32, rgb8_to_gray8, u16_to_f32,
+    u16_to_u8, u8_to_f32,
 };
 
 pub(crate) fn gray_img_open(bytes: &[u8]) -> Result<Array2<u8>, Box<dyn Error>> {
     let img = image::io::Reader::new(Cursor::new(bytes))
         .with_guessed_format()?
         .decode()?;
     let img_luma = img.to_luma8();
@@ -129,15 +130,18 @@
     (height, width)
 }
 
 pub(crate) fn psd_gray_decode(img: &[u8]) -> Result<Array2<u8>, Box<dyn Error>> {
     let size_bites: &[u8] = &img[14..22];
     let color_mode = img[25];
     let mut decoder = PSDDecoder::new(img);
-    let px = decoder.decode_raw().unwrap();
+    let mut px = decoder.decode_raw().unwrap();
+    if &img[23] == &16 {
+        px = u16_to_u8(&px);
+    }
     let (height, width) = decode_size_psd(size_bites);
     if color_mode == 1 {
         Ok(Array2::from_shape_vec(
             (height as usize, width as usize),
             px,
         )?)
     } else {
@@ -149,15 +153,18 @@
     }
 }
 
 pub(crate) fn psd_rgb_decode(img: &[u8]) -> Result<Array3<u8>, Box<dyn Error>> {
     let size_bites: &[u8] = &img[14..22];
     let color_mode = img[25];
     let mut decoder = PSDDecoder::new(img);
-    let px = decoder.decode_raw().unwrap();
+    let mut px = decoder.decode_raw().unwrap();
+    if &img[23] == &16 {
+        px = u16_to_u8(&px);
+    }
     let (height, width) = decode_size_psd(size_bites);
     if color_mode == 1 {
         let mut rgb_values = Vec::with_capacity(px.len() * 3);
 
         for gray in &px {
             rgb_values.extend([*gray, *gray, *gray].iter().copied());
         }
@@ -173,15 +180,18 @@
     }
 }
 
 pub(crate) fn psd_gray32_decode(img: &[u8]) -> Result<Array2<f32>, Box<dyn Error>> {
     let size_bites: &[u8] = &img[14..22];
     let color_mode = img[25];
     let mut decoder = PSDDecoder::new(img);
-    let px = decoder.decode_raw().unwrap();
+    let mut px = decoder.decode_raw().unwrap();
+    if &img[23] == &16 {
+        px = u16_to_u8(&px);
+    }
     let (height, width) = decode_size_psd(size_bites);
     if color_mode == 1 {
         let px = u8_to_f32(&px);
         Ok(Array2::from_shape_vec(
             (height as usize, width as usize),
             px,
         )?)
@@ -194,16 +204,19 @@
     }
 }
 
 pub(crate) fn psd_rgb32_decode(img: &[u8]) -> Result<Array3<f32>, Box<dyn Error>> {
     let size_bites: &[u8] = &img[14..22];
     let color_mode = img[25];
     let mut decoder = PSDDecoder::new(img);
-    let px = decoder.decode_raw().unwrap();
+    let mut px = decoder.decode_raw().unwrap();
     let (height, width) = decode_size_psd(size_bites);
+    if &img[23] == &16 {
+        px = u16_to_u8(&px);
+    }
     if color_mode == 1 {
         let mut rgb_values: Vec<f32> = Vec::with_capacity(px.len() * 3);
 
         for gray in &px {
             let gray_f32 = *gray as f32 * 0.00392156862745f32;
             rgb_values.extend([gray_f32, gray_f32, gray_f32].iter().copied());
         }
@@ -220,34 +233,44 @@
     }
 }
 
 pub(crate) fn psd_din_decode(img: &[u8]) -> Result<ArrayD<u8>, Box<dyn Error>> {
     let size_bites: &[u8] = &img[14..22];
     let channels = img[13] as usize;
     let mut decoder = PSDDecoder::new(img);
-    let px = decoder.decode_raw().unwrap();
+    let mut px = decoder.decode_raw().unwrap();
     let (height, width) = decode_size_psd(size_bites);
+    if &img[23] == &16 {
+        px = u16_to_u8(&px);
+    }
     if channels == 1 {
         Ok(Array2::from_shape_vec((height as usize, width as usize), px)?.into_dyn())
     } else {
         Ok(Array3::from_shape_vec((height as usize, width as usize, channels), px)?.into_dyn())
     }
 }
 
 pub(crate) fn psd_din32_decode(img: &[u8]) -> Result<ArrayD<f32>, Box<dyn Error>> {
     let size_bites: &[u8] = &img[14..22];
     let channels = img[13] as usize;
     let mut decoder = PSDDecoder::new(img);
     let px = decoder.decode_raw().unwrap();
     let (height, width) = decode_size_psd(size_bites);
-    let px = u8_to_f32(&px);
+    let px_float = match &img[23] {
+        16 => { u16_to_f32(&px) }
+        8 => { u8_to_f32(&px) }
+        _ => { return Err(Box::new(std::io::Error::new(std::io::ErrorKind::Other, format!("Unsupported bits: {}", &img[23])))); }
+    };
     if channels == 1 {
-        Ok(Array2::from_shape_vec((height as usize, width as usize), px)?.into_dyn())
+        Ok(Array2::from_shape_vec((height as usize, width as usize), px_float)?.into_dyn())
     } else {
-        Ok(Array3::from_shape_vec((height as usize, width as usize, channels), px)?.into_dyn())
+        Ok(
+            Array3::from_shape_vec((height as usize, width as usize, channels), px_float)?
+                .into_dyn(),
+        )
     }
 }
 
 pub fn all_read_u8(path: &Path, mode: u8) -> Result<ArrayD<u8>, Box<dyn Error>> {
     let img = FileBuffer::open(path).map_err(|err| Box::new(err) as Box<dyn Error>)?;
     let img_magic_byte = &img[..4];
     match img_magic_byte {
```

### Comparing `pepeline-0.2.8/src/utils/image/save.rs` & `pepeline-0.2.9/src/utils/image/save.rs`

 * *Files identical despite different names*

### Comparing `pepeline-0.2.8/src/utils/screentone/dot.rs` & `pepeline-0.2.9/src/utils/screentone/dot.rs`

 * *Files identical despite different names*

### Comparing `pepeline-0.2.8/src/utils/screentone/screentone_add.rs` & `pepeline-0.2.9/src/utils/screentone/screentone_add.rs`

 * *Files identical despite different names*

### Comparing `pepeline-0.2.8/Cargo.lock` & `pepeline-0.2.9/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -41,17 +41,17 @@
 name = "arrayvec"
 version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "96d30a06541fbafbc7f82ed10c06164cfbd2c401138f6addd8404629c4b16711"
 
 [[package]]
 name = "autocfg"
-version = "1.2.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "av1-grain"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6678909d8c5d46a42abcf571271e15fdbc0a225e3646cf23762cd415046c78bf"
 dependencies = [
@@ -124,17 +124,17 @@
 name = "byteorder-lite"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f1fe948ff07f4bd06c30984e69f5b4899c516a3ef74f34df92a2df2ab535495"
 
 [[package]]
 name = "cc"
-version = "1.0.95"
+version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d32a725bc159af97c3e629873bb9f88fb8cf8a4867175f76dc987815ea07c83b"
+checksum = "065a29261d53ba54260972629f9ca6bffa69bac13cd1fed61420f7fa68b9f8bd"
 dependencies = [
  "jobserver",
  "libc",
  "once_cell",
 ]
 
 [[package]]
@@ -244,17 +244,17 @@
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "flate2"
-version = "1.0.29"
+version = "1.0.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4556222738635b7a3417ae6130d8f52201e45a0c4d1a907f0826383adb5f85e7"
+checksum = "5f54427cfd1c7829e2a139fcefea601bf088ebca651d2bf53ebc600eac295dae"
 dependencies = [
  "crc32fast",
  "miniz_oxide",
 ]
 
 [[package]]
 name = "flume"
@@ -408,17 +408,17 @@
 name = "lebe"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "03087c2bad5e1034e8cace5926dec053fb3790248370865f5117a7d0213354c8"
 
 [[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.154"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "ae743338b92ff9146ce83992f766a31066a91a8c84a45e0e9f21e7cf6de6d346"
 
 [[package]]
 name = "libfuzzer-sys"
 version = "0.4.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a96cfd5557eb82f2b83fed4955246c988d331975a002961b07c81584d107e7f7"
 dependencies = [
@@ -599,17 +599,17 @@
  "num-bigint",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.18"
+version = "0.2.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
+checksum = "071dfc062690e90b734c0b2273ce72ad0ffa95f0c74596bc250dcfd960262841"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "numpy"
 version = "0.20.0"
@@ -658,15 +658,15 @@
 name = "paste"
 version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "de3145af08024dea9fa9914f381a17b8fc6034dfb00f3a84013f7ff43f29ed4c"
 
 [[package]]
 name = "pepeline"
-version = "0.2.8"
+version = "0.2.9"
 dependencies = [
  "filebuffer",
  "image",
  "ndarray",
  "noise",
  "numpy",
  "pyo3",
@@ -964,26 +964,26 @@
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "serde"
-version = "1.0.199"
+version = "1.0.200"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0c9f6e76df036c77cd94996771fb40db98187f096dd0b9af39c6c6e452ba966a"
+checksum = "ddc6f9cc94d67c0e21aaf7eda3a010fd3af78ebf6e096aa6e2e13c79749cce4f"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.199"
+version = "1.0.200"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11bd257a6541e141e42ca6d24ae26f7714887b47e89aa739099104c7e4d3b7fc"
+checksum = "856f046b9400cee3c8c94ed572ecdb752444c24528c035cd35882aad6f492bcb"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
```

### Comparing `pepeline-0.2.8/PKG-INFO` & `pepeline-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pepeline
-Version: 0.2.8
+Version: 0.2.9
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: numpy >=1.16.0
 License-File: LICENSE
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

