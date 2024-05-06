# Comparing `tmp/stack_graphs_python_bindings-0.0.1.tar.gz` & `tmp/stack_graphs_python_bindings-0.0.2.tar.gz`

## Comparing `stack_graphs_python_bindings-0.0.1.tar` & `stack_graphs_python_bindings-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,16 @@
--rw-r--r--   0        0        0      491 1970-01-01 00:00:00.000000 stack_graphs_python_bindings-0.0.1/Cargo.toml
--rw-r--r--   0     1001      127     3395 2024-05-06 10:30:49.000000 stack_graphs_python_bindings-0.0.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      730 2024-05-06 10:30:49.000000 stack_graphs_python_bindings-0.0.1/.gitignore
--rw-r--r--   0     1001      127      547 2024-05-06 10:30:49.000000 stack_graphs_python_bindings-0.0.1/README.md
--rw-r--r--   0     1001      127     2837 2024-05-06 10:30:49.000000 stack_graphs_python_bindings-0.0.1/src/lib.rs
--rw-r--r--   0     1001      127     3321 2024-05-06 10:30:49.000000 stack_graphs_python_bindings-0.0.1/src/stack_graphs_wrapper/mod.rs
--rw-r--r--   0     1001      127      268 2024-05-06 10:30:49.000000 stack_graphs_python_bindings-0.0.1/stack_graphs_python.pyi
--rw-r--r--   0     1001      127       66 2024-05-06 10:30:49.000000 stack_graphs_python_bindings-0.0.1/tests/js_sample/index.js
--rw-r--r--   0     1001      127       25 2024-05-06 10:30:49.000000 stack_graphs_python_bindings-0.0.1/tests/js_sample/module.js
--rw-r--r--   0     1001      127      685 2024-05-06 10:30:49.000000 stack_graphs_python_bindings-0.0.1/tests/test.py
--rw-r--r--   0     1001      127    48506 2024-05-06 10:30:49.000000 stack_graphs_python_bindings-0.0.1/Cargo.lock
--rw-r--r--   0     1001      127      404 2024-05-06 10:30:49.000000 stack_graphs_python_bindings-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      894 1970-01-01 00:00:00.000000 stack_graphs_python_bindings-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      577 1970-01-01 00:00:00.000000 stack_graphs_python_bindings-0.0.2/Cargo.toml
+-rw-r--r--   0     1001      127     3486 2024-05-06 12:54:43.000000 stack_graphs_python_bindings-0.0.2/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      730 2024-05-06 12:54:43.000000 stack_graphs_python_bindings-0.0.2/.gitignore
+-rw-r--r--   0     1001      127     1077 2024-05-06 12:54:43.000000 stack_graphs_python_bindings-0.0.2/LICENSE
+-rw-r--r--   0     1001      127      122 2024-05-06 12:54:43.000000 stack_graphs_python_bindings-0.0.2/Makefile
+-rw-r--r--   0     1001      127      909 2024-05-06 12:54:43.000000 stack_graphs_python_bindings-0.0.2/README.md
+-rw-r--r--   0     1001      127     1306 2024-05-06 12:54:43.000000 stack_graphs_python_bindings-0.0.2/src/classes.rs
+-rw-r--r--   0     1001      127     1870 2024-05-06 12:54:43.000000 stack_graphs_python_bindings-0.0.2/src/lib.rs
+-rw-r--r--   0     1001      127     3622 2024-05-06 12:54:43.000000 stack_graphs_python_bindings-0.0.2/src/stack_graphs_wrapper/mod.rs
+-rw-r--r--   0     1001      127      399 2024-05-06 12:54:43.000000 stack_graphs_python_bindings-0.0.2/stack_graphs_python.pyi
+-rw-r--r--   0     1001      127       66 2024-05-06 12:54:43.000000 stack_graphs_python_bindings-0.0.2/tests/js_sample/index.js
+-rw-r--r--   0     1001      127       25 2024-05-06 12:54:43.000000 stack_graphs_python_bindings-0.0.2/tests/js_sample/module.js
+-rw-r--r--   0     1001      127      849 2024-05-06 12:54:43.000000 stack_graphs_python_bindings-0.0.2/tests/test.py
+-rw-r--r--   0     1001      127    50375 2024-05-06 12:54:43.000000 stack_graphs_python_bindings-0.0.2/Cargo.lock
+-rw-r--r--   0     1001      127      405 2024-05-06 12:54:43.000000 stack_graphs_python_bindings-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1279 1970-01-01 00:00:00.000000 stack_graphs_python_bindings-0.0.2/PKG-INFO
```

### Comparing `stack_graphs_python_bindings-0.0.1/.github/workflows/CI.yml` & `stack_graphs_python_bindings-0.0.2/.github/workflows/CI.yml`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,18 @@
       - main
       - master
     tags:
       - '*'
   pull_request:
   workflow_dispatch:
 
+concurrency:
+  group: ${{ github.workflow }}-${{ github.ref }}
+  cancel-in-progress: true
+
 permissions:
   contents: read
 
 jobs:
   linux:
     runs-on: ${{ matrix.platform.runner }}
     strategy:
@@ -27,15 +31,15 @@
           #   target: x86
           # - runner: ubuntu-latest
           #   target: aarch64
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
         with:
-          python-version: '3.10'
+          python-version: '3.11'
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.platform.target }}
           args: --release --out dist --find-interpreter
           sccache: 'true'
           manylinux: auto
@@ -54,15 +58,15 @@
           #   target: x64
           - runner: windows-latest
             target: x86
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
         with:
-          python-version: '3.10'
+          python-version: '3.11'
           architecture: ${{ matrix.platform.target }}
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.platform.target }}
           args: --release --out dist --find-interpreter
           sccache: 'true'
@@ -81,15 +85,15 @@
             target: x86_64
           - runner: macos-14
             target: aarch64
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
         with:
-          python-version: '3.10'
+          python-version: '3.11'
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.platform.target }}
           args: --release --out dist --find-interpreter
           sccache: 'true'
       - name: Upload wheels
```

### Comparing `stack_graphs_python_bindings-0.0.1/.gitignore` & `stack_graphs_python_bindings-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `stack_graphs_python_bindings-0.0.1/src/stack_graphs_wrapper/mod.rs` & `stack_graphs_python_bindings-0.0.2/src/stack_graphs_wrapper/mod.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,53 @@
+use crate::classes::Language;
 use pyo3::exceptions::PyException;
 use pyo3::PyErr;
 use stack_graphs::storage::{SQLiteReader, SQLiteWriter};
 use std::path::PathBuf;
 use tree_sitter_stack_graphs::cli::query::{Querier, QueryResult};
 use tree_sitter_stack_graphs::cli::util::SourcePosition;
 use tree_sitter_stack_graphs::cli::{index::Indexer, util::reporter::ConsoleReporter};
+use tree_sitter_stack_graphs::loader::LanguageConfiguration;
 use tree_sitter_stack_graphs::{loader::Loader, NoCancellation};
 
 // TODO(@nohehf): Better error handling
 #[derive(Debug, Clone)]
 pub struct StackGraphsError {
     message: String,
 }
 
 impl std::convert::From<StackGraphsError> for PyErr {
     fn from(err: StackGraphsError) -> PyErr {
         PyException::new_err(err.message)
     }
 }
 
-pub fn index(paths: Vec<PathBuf>, db_path: &str) -> Result<(), StackGraphsError> {
-    let py_config = tree_sitter_stack_graphs_python::language_configuration(&NoCancellation);
-    let js_config = tree_sitter_stack_graphs_javascript::language_configuration(&NoCancellation);
+fn get_langauge_configuration(lang: Language) -> LanguageConfiguration {
+    match lang {
+        Language::Python => {
+            tree_sitter_stack_graphs_python::language_configuration(&NoCancellation)
+        }
+        Language::JavaScript => {
+            tree_sitter_stack_graphs_javascript::language_configuration(&NoCancellation)
+        }
+        Language::TypeScript => {
+            tree_sitter_stack_graphs_typescript::language_configuration(&NoCancellation)
+        }
+        Language::Java => tree_sitter_stack_graphs_java::language_configuration(&NoCancellation),
+    }
+}
 
-    let configs = vec![js_config, py_config];
+pub fn index(
+    paths: Vec<PathBuf>,
+    db_path: &str,
+    language: Language,
+) -> Result<(), StackGraphsError> {
+    let configurations = vec![get_langauge_configuration(language)];
 
-    let mut loader = match Loader::from_language_configurations(configs, None) {
+    let mut loader = match Loader::from_language_configurations(configurations, None) {
         Ok(ldr) => ldr,
         Err(e) => {
             return Err(StackGraphsError {
                 message: format!("Failed to create loader: {}", e),
             });
         }
     };
@@ -77,24 +95,14 @@
 
     match querier.definitions(reference, &NoCancellation) {
         Ok(results) => Ok(results),
         Err(e) => Err(StackGraphsError {
             message: format!("Failed to query definitions: {}", e),
         }),
     }
-
-    // if results.is_empty() {
-    //     println!("No definitions found");
-    //     return Ok(());
-    // }
-
-    // for res in results {
-    //     println!("Source: {:?}", res.source);
-    //     println!("Targets: {:?}", res.targets);
-    // }
 }
 
 // https://github.com/github/stack-graphs/blob/7db914c01b35ce024f6767e02dd1ad97022a6bc1/tree-sitter-stack-graphs/src/cli/index.rs#L118
 fn canonicalize_paths(paths: Vec<PathBuf>) -> Vec<PathBuf> {
     paths
         .into_iter()
         .map(|p| p.canonicalize())
```

### Comparing `stack_graphs_python_bindings-0.0.1/tests/test.py` & `stack_graphs_python_bindings-0.0.2/tests/test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 import os
-from stack_graphs_python import index, query_definition, Position
+from stack_graphs_python import index, query_definition, Position, Language
 
 # index ./js_sample directory
 
 # convert ./js_sample directory to absolute path
 dir = os.path.abspath("./tests/js_sample")
 db = os.path.abspath("./js_sample.db")
 
 print("Indexing directory: ", dir)
 print("Database path: ", db)
 
-index([dir], db)
+index([dir], db, language=Language.Python)
 
 source_reference: Position = Position(path=dir + "/index.js", line=2, column=12)
 
 print("Querying definition for: ", source_reference.path)
 
 results = query_definition(source_reference, db)
 
 print("Results: ", results)
 
 for result in results:
     print("Path: ", result.path)
     print("Line: ", result.line)
     print("Column: ", result.column)
     print("\n")
+
+assert len(results) == 2
+assert results[0].path.endswith("index.js")
+assert results[0].line == 0
+assert results[0].column == 9
```

### Comparing `stack_graphs_python_bindings-0.0.1/Cargo.lock` & `stack_graphs_python_bindings-0.0.2/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -580,14 +580,20 @@
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
+name = "glob"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
+
+[[package]]
 name = "hashbrown"
 version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d7afe4a420e3fe79967a00898cc1f4db7c8a49a9333a29f8a4bd76a253d5cd04"
 dependencies = [
  "ahash 0.4.8",
 ]
@@ -737,14 +743,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
+name = "json_comments"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9dbbfed4e59ba9750e15ba154fdfd9329cee16ff3df539c2666b70f58cc32105"
+
+[[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
@@ -1222,16 +1234,18 @@
 [[package]]
 name = "stack-graphs-python-bindings"
 version = "0.1.0"
 dependencies = [
  "pyo3",
  "stack-graphs",
  "tree-sitter-stack-graphs",
+ "tree-sitter-stack-graphs-java",
  "tree-sitter-stack-graphs-javascript",
  "tree-sitter-stack-graphs-python",
+ "tree-sitter-stack-graphs-typescript",
 ]
 
 [[package]]
 name = "string-interner"
 version = "0.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "383196d1876517ee6f9f0864d1fc1070331b803335d3c6daaa04bbcccd823c08"
@@ -1405,14 +1419,24 @@
 dependencies = [
  "regex",
  "thiserror",
  "tree-sitter",
 ]
 
 [[package]]
+name = "tree-sitter-java"
+version = "0.20.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f0bf5d3f508cbffcbfe1805834101c0d24297a8b6c2184ad9c595556c46d2420"
+dependencies = [
+ "cc",
+ "tree-sitter",
+]
+
+[[package]]
 name = "tree-sitter-javascript"
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "38d1463af5be7052171161db7cfe45c7621ed959ae533972ab47a09b1ed70ec0"
 dependencies = [
  "cc",
  "tree-sitter",
@@ -1478,14 +1502,24 @@
  "tree-sitter-config",
  "tree-sitter-graph",
  "tree-sitter-loader",
  "walkdir",
 ]
 
 [[package]]
+name = "tree-sitter-stack-graphs-java"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e68fc203c52b91edecbd8e4cf1fbf83d40bee604e33faf32dbae7d1c9bb40c7b"
+dependencies = [
+ "tree-sitter-java",
+ "tree-sitter-stack-graphs",
+]
+
+[[package]]
 name = "tree-sitter-stack-graphs-javascript"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6627c588d44e3af0e85a33d8fdd055e8a1d20f8f37a0cf333c9e624ec0415ee5"
 dependencies = [
  "serde",
  "serde_json",
@@ -1502,26 +1536,64 @@
 checksum = "be8371b7b134ca52e064f2b2e1f2e4bd9cb9e92a07c7f357fa66f5ea111ab15c"
 dependencies = [
  "tree-sitter-python",
  "tree-sitter-stack-graphs",
 ]
 
 [[package]]
+name = "tree-sitter-stack-graphs-typescript"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b9573452aaa69735feebece40a52cca6377482f3988ca48f30fadaad84af980d"
+dependencies = [
+ "glob",
+ "serde",
+ "serde_json",
+ "stack-graphs",
+ "tree-sitter-stack-graphs",
+ "tree-sitter-typescript",
+ "tsconfig",
+]
+
+[[package]]
 name = "tree-sitter-tags"
 version = "0.20.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ccb3f1376219530a37a809751ecf65aa35fd8b9c1c4ab6d4faf5f6a9eeda2c05"
 dependencies = [
  "memchr",
  "regex",
  "thiserror",
  "tree-sitter",
 ]
 
 [[package]]
+name = "tree-sitter-typescript"
+version = "0.20.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "079c695c32d39ad089101c66393aeaca30e967fba3486a91f573d2f0e12d290a"
+dependencies = [
+ "cc",
+ "tree-sitter",
+]
+
+[[package]]
+name = "tsconfig"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8613a6b9775c1e28349947b29fe983d288be5286285aa04e1282207b28be2a48"
+dependencies = [
+ "json_comments",
+ "regex",
+ "serde",
+ "serde_json",
+ "thiserror",
+]
+
+[[package]]
 name = "typenum"
 version = "1.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "42ff0bf0c66b8238c6f3b578df37d0b7848e55df8577b3f74f92a69acceeb825"
 
 [[package]]
 name = "unicode-ident"
```

### Comparing `stack_graphs_python_bindings-0.0.1/PKG-INFO` & `stack_graphs_python_bindings-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,53 @@
 Metadata-Version: 2.3
 Name: stack-graphs-python-bindings
-Version: 0.0.1
+Version: 0.0.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.8
+License-File: LICENSE
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # Stack-Graphs Python bindings
 
 Opinionated Python bindings for the [tree-sitter-stack-graphs](https://github.com/github/stack-graphs) rust library.
 
 It exposes very few, easy to use functions to index files and query references.
 
 This is a proof of concept draft, to test scripting utilities using stack-graphs easily.
 
 It uses pyo3 and maturin to generate the bindings.
 
-## Ressources
+## Installation & Usage
 
-https://pyo3.rs/v0.21.2/getting-started
-
-## Setup
+```bash
+pip install stack-graphs-python-bindings # or poetry, ...
+```
 
-TODO
+```python
+from stack_graphs_python import index, query_definition, Position
 
-```bash
-pipx install maturin
+# ...
 ```
 
+You can refer to the example in [test/test.py](https://github.com/nohehf/stack-graphs-python-bindings/blob/main/tests/test.py) for a concrete usage example.
+
 ## Development
 
-TODO
+### Ressources
+
+https://pyo3.rs/v0.21.2/getting-started
+
+### Setup
 
 ```bash
-maturin develop
+pipx install maturin # or pip, ...
 ```
 
-## Install
+### Testing
 
-TODO
+```bash
+maturin develop
+python tests/test.py
+```
```

