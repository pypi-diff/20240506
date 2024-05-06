# Comparing `tmp/endec-0.1.1.tar.gz` & `tmp/endec-0.1.2.tar.gz`

## Comparing `endec-0.1.1.tar` & `endec-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      164 1970-01-01 00:00:00.000000 endec-0.1.1/Cargo.toml
--rw-r--r--   0     1001      127     4333 2024-04-18 05:44:53.000000 endec-0.1.1/.github/workflows/build.yml
--rw-r--r--   0     1001      127      994 2024-04-18 05:44:53.000000 endec-0.1.1/.github/workflows/test.yml
--rw-r--r--   0     1001      127      685 2024-04-18 05:44:53.000000 endec-0.1.1/.gitignore
--rw-r--r--   0     1001      127     1064 2024-04-18 05:44:53.000000 endec-0.1.1/LICENSE
--rw-r--r--   0     1001      127     2304 2024-04-18 05:44:53.000000 endec-0.1.1/README.md
--rw-r--r--   0     1001      127      113 2024-04-18 05:44:53.000000 endec-0.1.1/python/endec/__init__.py
--rw-r--r--   0     1001      127      515 2024-04-18 05:44:53.000000 endec-0.1.1/python/endec/_endec.pyi
--rw-r--r--   0     1001      127     1060 2024-04-18 05:44:53.000000 endec-0.1.1/python/endec/exceptions.py
--rw-r--r--   0     1001      127        0 2024-04-18 05:44:53.000000 endec-0.1.1/python/endec/py.typed
--rw-r--r--   0     1001      127      745 2024-04-18 05:44:53.000000 endec-0.1.1/renovate.json
--rw-r--r--   0     1001      127       86 2024-04-18 05:44:53.000000 endec-0.1.1/rust-toolchain.toml
--rw-r--r--   0     1001      127     4306 2024-04-18 05:44:53.000000 endec-0.1.1/src/decode.rs
--rw-r--r--   0     1001      127      865 2024-04-18 05:44:53.000000 endec-0.1.1/src/encode.rs
--rw-r--r--   0     1001      127     1083 2024-04-18 05:44:53.000000 endec-0.1.1/src/ffi/exceptions.rs
--rw-r--r--   0     1001      127     3080 2024-04-18 05:44:53.000000 endec-0.1.1/src/ffi/mod.rs
--rw-r--r--   0     1001      127       33 2024-04-18 05:44:53.000000 endec-0.1.1/src/lib.rs
--rw-r--r--   0     1001      127     6158 2024-04-18 05:44:53.000000 endec-0.1.1/tests/test_decode.py
--rw-r--r--   0     1001      127     1965 2024-04-18 05:44:53.000000 endec-0.1.1/tests/test_encode.py
--rw-r--r--   0     1001      127      294 2024-04-18 05:44:53.000000 endec-0.1.1/tests/test_iso2022jp.py
--rw-r--r--   0     1001      127      193 2024-04-18 05:44:53.000000 endec-0.1.1/tox.ini
--rw-r--r--   0     1001      127     8098 2024-04-18 05:44:53.000000 endec-0.1.1/Cargo.lock
--rw-r--r--   0     1001      127     1201 2024-04-18 05:44:53.000000 endec-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3301 1970-01-01 00:00:00.000000 endec-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      164 1970-01-01 00:00:00.000000 endec-0.1.2/Cargo.toml
+-rw-r--r--   0     1001      127     4333 2024-05-06 08:56:15.000000 endec-0.1.2/.github/workflows/build.yml
+-rw-r--r--   0     1001      127      994 2024-05-06 08:56:15.000000 endec-0.1.2/.github/workflows/test.yml
+-rw-r--r--   0     1001      127      685 2024-05-06 08:56:15.000000 endec-0.1.2/.gitignore
+-rw-r--r--   0     1001      127     1064 2024-05-06 08:56:15.000000 endec-0.1.2/LICENSE
+-rw-r--r--   0     1001      127     2304 2024-05-06 08:56:15.000000 endec-0.1.2/README.md
+-rw-r--r--   0     1001      127      113 2024-05-06 08:56:15.000000 endec-0.1.2/python/endec/__init__.py
+-rw-r--r--   0     1001      127      515 2024-05-06 08:56:15.000000 endec-0.1.2/python/endec/_endec.pyi
+-rw-r--r--   0     1001      127     1060 2024-05-06 08:56:15.000000 endec-0.1.2/python/endec/exceptions.py
+-rw-r--r--   0     1001      127        0 2024-05-06 08:56:15.000000 endec-0.1.2/python/endec/py.typed
+-rw-r--r--   0     1001      127      745 2024-05-06 08:56:15.000000 endec-0.1.2/renovate.json
+-rw-r--r--   0     1001      127       86 2024-05-06 08:56:15.000000 endec-0.1.2/rust-toolchain.toml
+-rw-r--r--   0     1001      127     4306 2024-05-06 08:56:15.000000 endec-0.1.2/src/decode.rs
+-rw-r--r--   0     1001      127      865 2024-05-06 08:56:15.000000 endec-0.1.2/src/encode.rs
+-rw-r--r--   0     1001      127     1083 2024-05-06 08:56:15.000000 endec-0.1.2/src/ffi/exceptions.rs
+-rw-r--r--   0     1001      127     3080 2024-05-06 08:56:15.000000 endec-0.1.2/src/ffi/mod.rs
+-rw-r--r--   0     1001      127       33 2024-05-06 08:56:15.000000 endec-0.1.2/src/lib.rs
+-rw-r--r--   0     1001      127     6158 2024-05-06 08:56:15.000000 endec-0.1.2/tests/test_decode.py
+-rw-r--r--   0     1001      127     1965 2024-05-06 08:56:15.000000 endec-0.1.2/tests/test_encode.py
+-rw-r--r--   0     1001      127      294 2024-05-06 08:56:15.000000 endec-0.1.2/tests/test_iso2022jp.py
+-rw-r--r--   0     1001      127      193 2024-05-06 08:56:15.000000 endec-0.1.2/tox.ini
+-rw-r--r--   0     1001      127     8329 2024-05-06 08:56:15.000000 endec-0.1.2/Cargo.lock
+-rw-r--r--   0     1001      127     1201 2024-05-06 08:56:15.000000 endec-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3301 1970-01-01 00:00:00.000000 endec-0.1.2/PKG-INFO
```

### Comparing `endec-0.1.1/.github/workflows/build.yml` & `endec-0.1.2/.github/workflows/build.yml`

 * *Files 19% similar despite different names*

```diff
@@ -33,106 +33,106 @@
           - runner: ubuntu-latest
             target: armv7
           - runner: ubuntu-latest
             target: s390x
           - runner: ubuntu-latest
             target: ppc64le
     steps:
-      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # v4.1.1
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b # v4.1.4
       - uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d # v5.1.0
         with:
           python-version: '3.10'
       - name: Build wheels
-        uses: PyO3/maturin-action@bf468cfccfe9a3fec2554b0eebf2e9276cf066aa # v1.42.1
+        uses: PyO3/maturin-action@52b28abb0c6729beb388babfc348bf6ff5aaff31 # v1.42.2
         with:
           target: ${{ matrix.platform.target }}
           args: --release --out dist --find-interpreter
           sccache: 'true'
           manylinux: auto
       - name: Upload wheels
-        uses: actions/upload-artifact@5d5d22a31266ced268874388b861e4b58bb5c2f3 # v4.3.1
+        uses: actions/upload-artifact@65462800fd760344b1a7b4382951275a0abb4808 # v4.3.3
         with:
           name: wheels-linux-${{ matrix.platform.target }}
           path: dist
 
   windows:
     runs-on: ${{ matrix.platform.runner }}
     strategy:
       matrix:
         platform:
           - runner: windows-latest
             target: x64
           - runner: windows-latest
             target: x86
     steps:
-      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # v4.1.1
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b # v4.1.4
       - uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d # v5.1.0
         with:
           python-version: '3.10'
           architecture: ${{ matrix.platform.target }}
       - name: Build wheels
-        uses: PyO3/maturin-action@bf468cfccfe9a3fec2554b0eebf2e9276cf066aa # v1.42.1
+        uses: PyO3/maturin-action@52b28abb0c6729beb388babfc348bf6ff5aaff31 # v1.42.2
         with:
           target: ${{ matrix.platform.target }}
           args: --release --out dist --find-interpreter
           sccache: 'true'
       - name: Upload wheels
-        uses: actions/upload-artifact@5d5d22a31266ced268874388b861e4b58bb5c2f3 # v4.3.1
+        uses: actions/upload-artifact@65462800fd760344b1a7b4382951275a0abb4808 # v4.3.3
         with:
           name: wheels-windows-${{ matrix.platform.target }}
           path: dist
 
   macos:
     runs-on: ${{ matrix.platform.runner }}
     strategy:
       matrix:
         platform:
           - runner: macos-latest
             target: x86_64
           - runner: macos-14
             target: aarch64
     steps:
-      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # v4.1.1
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b # v4.1.4
       - uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d # v5.1.0
         with:
           python-version: '3.10'
       - name: Build wheels
-        uses: PyO3/maturin-action@bf468cfccfe9a3fec2554b0eebf2e9276cf066aa # v1.42.1
+        uses: PyO3/maturin-action@52b28abb0c6729beb388babfc348bf6ff5aaff31 # v1.42.2
         with:
           target: ${{ matrix.platform.target }}
           args: --release --out dist --find-interpreter
           sccache: 'true'
       - name: Upload wheels
-        uses: actions/upload-artifact@5d5d22a31266ced268874388b861e4b58bb5c2f3 # v4.3.1
+        uses: actions/upload-artifact@65462800fd760344b1a7b4382951275a0abb4808 # v4.3.3
         with:
           name: wheels-macos-${{ matrix.platform.target }}
           path: dist
 
   sdist:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # v4.1.1
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b # v4.1.4
       - name: Build sdist
-        uses: PyO3/maturin-action@bf468cfccfe9a3fec2554b0eebf2e9276cf066aa # v1.42.1
+        uses: PyO3/maturin-action@52b28abb0c6729beb388babfc348bf6ff5aaff31 # v1.42.2
         with:
           command: sdist
           args: --out dist
       - name: Upload sdist
-        uses: actions/upload-artifact@5d5d22a31266ced268874388b861e4b58bb5c2f3 # v4.3.1
+        uses: actions/upload-artifact@65462800fd760344b1a7b4382951275a0abb4808 # v4.3.3
         with:
           name: wheels-sdist
           path: dist
 
   release:
     name: Release
     runs-on: ubuntu-latest
     if: "startsWith(github.ref, 'refs/tags/')"
     needs: [linux, windows, macos, sdist]
     steps:
-      - uses: actions/download-artifact@c850b930e6ba138125429b7e5c93fc707a7f8427 # v4.1.4
+      - uses: actions/download-artifact@65a9edc5881444af0b9093a5e628f2fe47ea3b2e # v4.1.7
       - name: Publish to PyPI
-        uses: PyO3/maturin-action@bf468cfccfe9a3fec2554b0eebf2e9276cf066aa # v1.42.1
+        uses: PyO3/maturin-action@52b28abb0c6729beb388babfc348bf6ff5aaff31 # v1.42.2
         env:
           MATURIN_PYPI_TOKEN: ${{ secrets.PYPI_API_TOKEN }}
         with:
           command: upload
           args: --non-interactive --skip-existing wheels-*/*
```

### Comparing `endec-0.1.1/.github/workflows/test.yml` & `endec-0.1.2/.github/workflows/test.yml`

 * *Files 17% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     runs-on: "${{ matrix.platform }}"
     strategy:
       matrix:
         platform: ["ubuntu-latest", "windows-latest"]
         python-version: ["3.12", "3.11", "3.10", "3.9", "3.8"]
 
     steps:
-      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # v4.1.1
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b # v4.1.4
       - uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d # v5.1.0
         with:
           python-version: "${{ matrix.python-version }}"
           allow-prereleases: true
 
       - name: Install dependencies
         run: |
```

### Comparing `endec-0.1.1/.gitignore` & `endec-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `endec-0.1.1/LICENSE` & `endec-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `endec-0.1.1/README.md` & `endec-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `endec-0.1.1/python/endec/_endec.pyi` & `endec-0.1.2/python/endec/_endec.pyi`

 * *Files identical despite different names*

### Comparing `endec-0.1.1/python/endec/exceptions.py` & `endec-0.1.2/python/endec/exceptions.py`

 * *Files identical despite different names*

### Comparing `endec-0.1.1/renovate.json` & `endec-0.1.2/renovate.json`

 * *Files identical despite different names*

### Comparing `endec-0.1.1/src/decode.rs` & `endec-0.1.2/src/decode.rs`

 * *Files identical despite different names*

### Comparing `endec-0.1.1/src/encode.rs` & `endec-0.1.2/src/encode.rs`

 * *Files identical despite different names*

### Comparing `endec-0.1.1/src/ffi/exceptions.rs` & `endec-0.1.2/src/ffi/exceptions.rs`

 * *Files identical despite different names*

### Comparing `endec-0.1.1/src/ffi/mod.rs` & `endec-0.1.2/src/ffi/mod.rs`

 * *Files identical despite different names*

### Comparing `endec-0.1.1/tests/test_decode.py` & `endec-0.1.2/tests/test_decode.py`

 * *Files identical despite different names*

### Comparing `endec-0.1.1/tests/test_encode.py` & `endec-0.1.2/tests/test_encode.py`

 * *Files identical despite different names*

### Comparing `endec-0.1.1/Cargo.lock` & `endec-0.1.2/Cargo.lock`

 * *Files 4% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 name = "autocfg"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "bitflags"
-version = "1.3.2"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
@@ -27,15 +27,15 @@
 checksum = "b45de904aa0b010bce2ab45264d0631681847fa7b6f2eaa7dab7619943bc4f59"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "endec"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "encoding_rs",
  "pyo3",
 ]
 
 [[package]]
 name = "heck"
@@ -47,23 +47,23 @@
 name = "indoc"
 version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.154"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "ae743338b92ff9146ce83992f766a31066a91a8c84a45e0e9f21e7cf6de6d346"
 
 [[package]]
 name = "lock_api"
-version = "0.4.11"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "memoffset"
@@ -78,27 +78,27 @@
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.9"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-targets",
 ]
@@ -107,17 +107,17 @@
 name = "portable-atomic"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.79"
+version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
+checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.21.2"
@@ -179,26 +179,26 @@
  "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.4.1"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
@@ -209,17 +209,17 @@
 name = "smallvec"
 version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "syn"
-version = "2.0.57"
+version = "2.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11a6ae1e52eb25aab8f3fb9fca13be982a373b8f1157ca14b897a825ba4a2d35"
+checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -238,61 +238,68 @@
 name = "unindent"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
 name = "windows-targets"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
+ "windows_i686_gnullvm",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.48.5"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
```

### Comparing `endec-0.1.1/pyproject.toml` & `endec-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=1.5,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "endec"
-version = "0.1.1"
+version = "0.1.2"
 description = "Web-compatible encoding and decoding library"
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [{ name = "Thitat Auareesuksakul", email = "flux@thitat.net" }]
 keywords = ["encoding_rs", "web", "codec"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `endec-0.1.1/PKG-INFO` & `endec-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: endec
-Version: 0.1.1
+Version: 0.1.2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
```

