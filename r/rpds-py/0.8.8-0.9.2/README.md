# Comparing `tmp/rpds_py-0.8.8.tar.gz` & `tmp/rpds_py-0.9.2.tar.gz`

## Comparing `rpds_py-0.8.8.tar` & `rpds_py-0.9.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      245 1970-01-01 00:00:00.000000 rpds_py-0.8.8/Cargo.toml
--rw-r--r--   0        0        0      219 2023-07-06 14:59:52.000000 rpds_py-0.8.8/.github/dependabot.yml
--rw-r--r--   0        0        0       81 2023-07-06 14:59:52.000000 rpds_py-0.8.8/.github/release.yml
--rw-r--r--   0        0        0     5106 2023-07-06 14:59:52.000000 rpds_py-0.8.8/.github/workflows/CI.yml
--rw-r--r--   0        0        0      758 2023-07-06 14:59:52.000000 rpds_py-0.8.8/.gitignore
--rw-r--r--   0        0        0     1050 2023-07-06 14:59:52.000000 rpds_py-0.8.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1076 2023-07-06 14:59:52.000000 rpds_py-0.8.8/LICENSE
--rw-r--r--   0        0        0     2522 2023-07-06 14:59:52.000000 rpds_py-0.8.8/README.rst
--rw-r--r--   0        0        0     1043 2023-07-06 14:59:52.000000 rpds_py-0.8.8/noxfile.py
--rw-r--r--   0        0        0     1406 2023-07-06 14:59:52.000000 rpds_py-0.8.8/pyproject.toml
--rw-r--r--   0        0        0     1697 2023-07-06 14:59:52.000000 rpds_py-0.8.8/rpds.pyi
--rw-r--r--   0        0        0    17578 2023-07-06 14:59:52.000000 rpds_py-0.8.8/src/lib.rs
--rw-r--r--   0        0        0       20 2023-07-06 14:59:52.000000 rpds_py-0.8.8/tests/requirements.in
--rw-r--r--   0        0        0      484 2023-07-06 14:59:52.000000 rpds_py-0.8.8/tests/requirements.txt
--rw-r--r--   0        0        0     8653 2023-07-06 14:59:52.000000 rpds_py-0.8.8/tests/test_hash_trie_map.py
--rw-r--r--   0        0        0     5098 2023-07-06 14:59:52.000000 rpds_py-0.8.8/tests/test_hash_trie_set.py
--rw-r--r--   0        0        0     3533 2023-07-06 14:59:52.000000 rpds_py-0.8.8/tests/test_list.py
--rw-r--r--   0        0        0     8633 2023-07-06 14:59:52.000000 rpds_py-0.8.8/Cargo.lock
--rw-r--r--   0        0        0     3705 1970-01-01 00:00:00.000000 rpds_py-0.8.8/PKG-INFO
+-rw-r--r--   0        0        0      245 1970-01-01 00:00:00.000000 rpds_py-0.9.2/Cargo.toml
+-rw-r--r--   0        0        0      219 2023-07-18 14:07:14.000000 rpds_py-0.9.2/.github/dependabot.yml
+-rw-r--r--   0        0        0       81 2023-07-18 14:07:14.000000 rpds_py-0.9.2/.github/release.yml
+-rw-r--r--   0        0        0     5289 2023-07-18 14:07:14.000000 rpds_py-0.9.2/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      758 2023-07-18 14:07:14.000000 rpds_py-0.9.2/.gitignore
+-rw-r--r--   0        0        0     1050 2023-07-18 14:07:14.000000 rpds_py-0.9.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1076 2023-07-18 14:07:14.000000 rpds_py-0.9.2/LICENSE
+-rw-r--r--   0        0        0     2576 2023-07-18 14:07:14.000000 rpds_py-0.9.2/README.rst
+-rw-r--r--   0        0        0     1051 2023-07-18 14:07:14.000000 rpds_py-0.9.2/noxfile.py
+-rw-r--r--   0        0        0     1451 2023-07-18 14:07:14.000000 rpds_py-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     1697 2023-07-18 14:07:14.000000 rpds_py-0.9.2/rpds.pyi
+-rw-r--r--   0        0        0    17578 2023-07-18 14:07:14.000000 rpds_py-0.9.2/src/lib.rs
+-rw-r--r--   0        0        0       20 2023-07-18 14:07:14.000000 rpds_py-0.9.2/tests/requirements.in
+-rw-r--r--   0        0        0      484 2023-07-18 14:07:14.000000 rpds_py-0.9.2/tests/requirements.txt
+-rw-r--r--   0        0        0     8653 2023-07-18 14:07:14.000000 rpds_py-0.9.2/tests/test_hash_trie_map.py
+-rw-r--r--   0        0        0     5098 2023-07-18 14:07:14.000000 rpds_py-0.9.2/tests/test_hash_trie_set.py
+-rw-r--r--   0        0        0     3533 2023-07-18 14:07:14.000000 rpds_py-0.9.2/tests/test_list.py
+-rw-r--r--   0        0        0     8394 2023-07-18 14:07:14.000000 rpds_py-0.9.2/Cargo.lock
+-rw-r--r--   0        0        0     3810 1970-01-01 00:00:00.000000 rpds_py-0.9.2/PKG-INFO
```

### Comparing `rpds_py-0.8.8/.github/workflows/CI.yml` & `rpds_py-0.9.2/.github/workflows/CI.yml`

 * *Files 12% similar despite different names*

```diff
@@ -59,15 +59,22 @@
         if: runner.os == 'Linux' && startsWith(matrix.noxenv, 'docs')
       - name: Install dependencies
         run: brew install enchant
         if: runner.os == 'macOS' && startsWith(matrix.noxenv, 'docs')
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
-          python-version: "3.x"
+          python-version: |
+            3.8
+            3.9
+            3.10
+            3.11
+            3.12
+            pypy3.10
+          allow-prereleases: true
       - name: Set up nox
         uses: wntrblm/nox@2023.04.22
       - name: Run nox
         run: nox -s "${{ matrix.noxenv }}"
 
   manylinux:
     needs: test
@@ -80,15 +87,15 @@
       - uses: actions/setup-python@v4
         with:
           python-version: "3.x"
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
-          args: --release --out dist --interpreter '3.8 3.9 3.10 3.11 pypy3.8 pypy3.9'
+          args: --release --out dist --interpreter '3.8 3.9 3.10 3.11 3.12 pypy3.8 pypy3.9 pypy3.10'
           manylinux: auto
       - name: Upload wheels
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
 
@@ -106,15 +113,15 @@
       - uses: actions/setup-python@v4
         with:
           python-version: "3.x"
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
-          args: --release --out dist --interpreter '3.8 3.9 3.10 3.11 pypy3.8 pypy3.9'
+          args: --release --out dist --interpreter '3.8 3.9 3.10 3.11 3.12 pypy3.8 pypy3.9 pypy3.10'
           manylinux: musllinux_1_2
       - name: Upload wheels
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
 
@@ -152,15 +159,15 @@
       - uses: actions/setup-python@v4
         with:
           python-version: "3.x"
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
-          args: --release --out dist --interpreter '3.8 3.9 3.10 3.11 pypy3.8 pypy3.9'
+          args: --release --out dist --interpreter '3.8 3.9 3.10 3.11 3.12 pypy3.8 pypy3.9 pypy3.10'
       - name: Upload wheels
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
 
   release:
```

### Comparing `rpds_py-0.8.8/.gitignore` & `rpds_py-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.8/.pre-commit-config.yaml` & `rpds_py-0.9.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.8/LICENSE` & `rpds_py-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.8/README.rst` & `rpds_py-0.9.2/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
   :target: https://pypi.org/project/rpds-py/
 
 .. |CI| image:: https://github.com/crate-py/rpds/workflows/CI/badge.svg
   :alt: Build status
   :target: https://github.com/crate-py/rpds/actions?query=workflow%3ACI
 
 
-Python bindings to the Rust ``rpds`` crate.
+Python bindings to the `Rust rpds crate <https://docs.rs/rpds/>`_ for persistent data structures.
 
 What's here is quite minimal (in transparency, it was written initially to support replacing ``pyrsistent`` in the `referencing library <https://github.com/python-jsonschema/referencing>`_).
 If you see something missing (which is very likely), a PR is definitely welcome to add it.
 
 Installation
 ------------
```

### Comparing `rpds_py-0.8.8/noxfile.py` & `rpds_py-0.9.2/noxfile.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         if default:
             nox.options.sessions.append(kwargs.get("name", fn.__name__))
         return nox.session(**kwargs)(fn)
 
     return _session
 
 
-@session(python=["3.8", "3.9", "3.10", "3.11", "pypy3"])
+@session(python=["3.8", "3.9", "3.10", "3.11", "3.12", "pypy3"])
 def tests(session):
     session.install(ROOT, "-r", TESTS / "requirements.txt")
     if session.posargs == ["coverage"]:
         session.install("coverage[toml]")
         session.run("coverage", "run", "-m", "pytest")
         session.run("coverage", "report")
     else:
```

### Comparing `rpds_py-0.8.8/pyproject.toml` & `rpds_py-0.9.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Rust",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 
 ]
 dynamic = ["version"]
```

### Comparing `rpds_py-0.8.8/rpds.pyi` & `rpds_py-0.9.2/rpds.pyi`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.8/src/lib.rs` & `rpds_py-0.9.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.8/tests/test_hash_trie_map.py` & `rpds_py-0.9.2/tests/test_hash_trie_map.py`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.8/tests/test_hash_trie_set.py` & `rpds_py-0.9.2/tests/test_hash_trie_set.py`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.8/tests/test_list.py` & `rpds_py-0.9.2/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `rpds_py-0.8.8/Cargo.lock` & `rpds_py-0.9.2/Cargo.lock`

 * *Files 10% similar despite different names*

```diff
@@ -33,23 +33,23 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "libc"
-version = "0.2.139"
+version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "201de327520df007757c1f0adce6e827fe8562fbc28bfd9c15571c66ca1f5f79"
+checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "memoffset"
@@ -58,46 +58,46 @@
 checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.7"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "windows-targets",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.51"
+version = "1.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d727cae5b39d21da60fa540906919ad737832fe0b1c165da3a34d6548c849d6"
+checksum = "18fb31db3f9bddb2ea821cde30a9f70117e3f119938b5ee630b7403aa6e2ead9"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.19.1"
@@ -156,26 +156,26 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.23"
+version = "1.0.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8856d8364d252a14d474036ea1358d63c9e6965c8e5c1885c18f73d70bff9c7b"
+checksum = "5fe8a65d69dd0808184ebb5f836ab526bb259db23c657efa38711b1072ee47f0"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "rpds"
 version = "0.13.0"
@@ -183,32 +183,32 @@
 checksum = "9bd6ce569b15c331b1e5fd8cf6adb0bf240678b5f0cdc4d0f41e11683f6feba9"
 dependencies = [
  "archery",
 ]
 
 [[package]]
 name = "rpds-py"
-version = "0.8.8"
+version = "0.9.2"
 dependencies = [
  "archery",
  "pyo3",
  "rpds",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
 
 [[package]]
 name = "static_assertions"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
 
@@ -221,88 +221,79 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.6"
+version = "0.12.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
+checksum = "df8e77cb757a61f51b947ec4a7e3646efd825b73561db1c232a8ccb639e611a0"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.6"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84a22b9f218b40614adcb3f4ff08b703773ad44fa9423e4e0d346d5db86e4ebc"
+checksum = "301abaae475aa91687eb82514b328ab47a211a533026cb25fc3e519b86adfc3c"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
-name = "windows-sys"
-version = "0.45.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
-dependencies = [
- "windows-targets",
-]
-
-[[package]]
 name = "windows-targets"
-version = "0.42.1"
+version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e2522491fbfcd58cc84d47aeb2958948c4b8982e9a2d8a2a35bbaed431390e7"
+checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c9864e83243fdec7fc9c5444389dcbbfd258f745e7853198f365e3c4968a608"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c8b1b673ffc16c47a9ff48570a9d85e25d265735c503681332589af6253c6c7"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "de3887528ad530ba7bdbb1faa8275ec7a1155a45ffa57c37993960277145d640"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf4d1122317eddd6ff351aa852118a2418ad4214e6613a50e0191f7004372605"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1040f221285e17ebccbc2591ffdc2d44ee1f9186324dd3e84e99ac68d699c45"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "628bfdf232daa22b0d64fdb62b09fcc36bb01f05a3939e20ab73aaf9470d0463"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "447660ad36a13288b1db4d4248e857b510e8c3a225c822ba4fb748c0aafecffd"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
```

### Comparing `rpds_py-0.8.8/PKG-INFO` & `rpds_py-0.9.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: rpds-py
-Version: 0.8.8
+Version: 0.9.2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Python bindings to Rust's persistent data structures (rpds)
 Keywords: data structures,rust,persistent
 Author: Julian Berman
@@ -41,15 +42,15 @@
   :target: https://pypi.org/project/rpds-py/
 
 .. |CI| image:: https://github.com/crate-py/rpds/workflows/CI/badge.svg
   :alt: Build status
   :target: https://github.com/crate-py/rpds/actions?query=workflow%3ACI
 
 
-Python bindings to the Rust ``rpds`` crate.
+Python bindings to the `Rust rpds crate <https://docs.rs/rpds/>`_ for persistent data structures.
 
 What's here is quite minimal (in transparency, it was written initially to support replacing ``pyrsistent`` in the `referencing library <https://github.com/python-jsonschema/referencing>`_).
 If you see something missing (which is very likely), a PR is definitely welcome to add it.
 
 Installation
 ------------
```

