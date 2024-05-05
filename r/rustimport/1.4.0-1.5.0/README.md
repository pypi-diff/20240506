# Comparing `tmp/rustimport-1.4.0.tar.gz` & `tmp/rustimport-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rustimport-1.4.0.tar", last modified: Tue Jan  2 09:59:59 2024, max compression
+gzip compressed data, was "rustimport-1.5.0.tar", last modified: Sun May  5 22:43:37 2024, max compression
```

## Comparing `rustimport-1.4.0.tar` & `rustimport-1.5.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 09:59:59.637978 rustimport-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-01-02 09:59:46.000000 rustimport-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-02 09:59:46.000000 rustimport-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14217 2024-01-02 09:59:59.637978 rustimport-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13566 2024-01-02 09:59:46.000000 rustimport-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-02 09:59:46.000000 rustimport-1.4.0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 09:59:59.633978 rustimport-1.4.0/rustimport/
--rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-01-02 09:59:46.000000 rustimport-1.4.0/rustimport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-01-02 09:59:46.000000 rustimport-1.4.0/rustimport/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-01-02 09:59:46.000000 rustimport-1.4.0/rustimport/checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-01-02 09:59:46.000000 rustimport-1.4.0/rustimport/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-01-02 09:59:46.000000 rustimport-1.4.0/rustimport/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-01-02 09:59:46.000000 rustimport-1.4.0/rustimport/find.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-01-02 09:59:46.000000 rustimport-1.4.0/rustimport/import_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)    13460 2024-01-02 09:59:46.000000 rustimport-1.4.0/rustimport/importable.py
--rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-01-02 09:59:46.000000 rustimport-1.4.0/rustimport/ipython_magic.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-01-02 09:59:46.000000 rustimport-1.4.0/rustimport/load.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 09:59:59.633978 rustimport-1.4.0/rustimport/pre_processing/
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-01-02 09:59:46.000000 rustimport-1.4.0/rustimport/pre_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-01-02 09:59:46.000000 rustimport-1.4.0/rustimport/pre_processing/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-01-02 09:59:46.000000 rustimport-1.4.0/rustimport/pre_processing/pyo3_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-01-02 09:59:46.000000 rustimport-1.4.0/rustimport/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 09:59:59.633978 rustimport-1.4.0/rustimport.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14217 2024-01-02 09:59:59.000000 rustimport-1.4.0/rustimport.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-01-02 09:59:59.000000 rustimport-1.4.0/rustimport.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-02 09:59:59.000000 rustimport-1.4.0/rustimport.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-02 09:59:59.000000 rustimport-1.4.0/rustimport.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-02 09:59:59.000000 rustimport-1.4.0/rustimport.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-02 09:59:59.000000 rustimport-1.4.0/rustimport.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-02 09:59:59.637978 rustimport-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-01-02 09:59:46.000000 rustimport-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 09:59:59.633978 rustimport-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-01-02 09:59:46.000000 rustimport-1.4.0/tests/run_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-01-02 09:59:46.000000 rustimport-1.4.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-01-02 09:59:46.000000 rustimport-1.4.0/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-01-02 09:59:46.000000 rustimport-1.4.0/tests/test_ipython_magic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:43:37.978914 rustimport-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-05 22:43:30.000000 rustimport-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-05 22:43:30.000000 rustimport-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14228 2024-05-05 22:43:37.978914 rustimport-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13577 2024-05-05 22:43:30.000000 rustimport-1.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-05 22:43:30.000000 rustimport-1.5.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:43:37.974913 rustimport-1.5.0/rustimport/
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-05-05 22:43:30.000000 rustimport-1.5.0/rustimport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7155 2024-05-05 22:43:30.000000 rustimport-1.5.0/rustimport/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-05-05 22:43:30.000000 rustimport-1.5.0/rustimport/checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-05-05 22:43:30.000000 rustimport-1.5.0/rustimport/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-05 22:43:30.000000 rustimport-1.5.0/rustimport/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-05 22:43:30.000000 rustimport-1.5.0/rustimport/find.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-05 22:43:30.000000 rustimport-1.5.0/rustimport/import_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13460 2024-05-05 22:43:30.000000 rustimport-1.5.0/rustimport/importable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-05-05 22:43:30.000000 rustimport-1.5.0/rustimport/ipython_magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-05 22:43:30.000000 rustimport-1.5.0/rustimport/load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:43:37.974913 rustimport-1.5.0/rustimport/pre_processing/
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-05-05 22:43:30.000000 rustimport-1.5.0/rustimport/pre_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-05 22:43:30.000000 rustimport-1.5.0/rustimport/pre_processing/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-05 22:43:30.000000 rustimport-1.5.0/rustimport/pre_processing/pyo3_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-05 22:43:30.000000 rustimport-1.5.0/rustimport/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:43:37.978914 rustimport-1.5.0/rustimport.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14228 2024-05-05 22:43:37.000000 rustimport-1.5.0/rustimport.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-05 22:43:37.000000 rustimport-1.5.0/rustimport.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 22:43:37.000000 rustimport-1.5.0/rustimport.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 22:43:37.000000 rustimport-1.5.0/rustimport.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-05 22:43:37.000000 rustimport-1.5.0/rustimport.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-05 22:43:37.000000 rustimport-1.5.0/rustimport.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 22:43:37.978914 rustimport-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-05 22:43:30.000000 rustimport-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:43:37.978914 rustimport-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-05 22:43:30.000000 rustimport-1.5.0/tests/run_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-05-05 22:43:30.000000 rustimport-1.5.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-05 22:43:30.000000 rustimport-1.5.0/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-05 22:43:30.000000 rustimport-1.5.0/tests/test_ipython_magic.py
```

### Comparing `rustimport-1.4.0/LICENSE` & `rustimport-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rustimport-1.4.0/PKG-INFO` & `rustimport-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rustimport
-Version: 1.4.0
+Version: 1.5.0
 Summary: Import Rust files directly from Python!
 Home-page: https://github.com/mityax/rustimport
 Author: mityax
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -17,15 +17,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: toml>=0.10.2
 
 # rustimport - Import Rust directly from Python! 
 
 <p align=center>
-    <a target="_blank" href="https://www.python.org/downloads/" title="Python version"><img src="https://img.shields.io/badge/python-%3E=_3.6-green.svg"></a>
+    <a target="_blank" href="https://www.python.org/downloads/" title="Python version"><img src="https://img.shields.io/badge/python-%3E=_3.8-green.svg"></a>
     <a target="_blank" href="https://pypi.org/project/rustimport/" title="PyPI version"><img src="https://img.shields.io/pypi/v/rustimport?logo=pypi"></a>
     <a target="_blank" href="LICENSE" title="License: MIT"><img src="https://img.shields.io/badge/License-MIT-blue.svg"></a></a>
 </p>
 
 rustimport was heavily inspired by and is partly based upon [cppimport](https://github.com/tbenthompson/cppimport). Check it out if you're interested in the same functionality for C and C++!
 
 ## Installation
@@ -109,15 +109,15 @@
 [dependencies.pyo3]
 version = "0.16.2"
 features = [ "extension-module",]
 ```
 3. It generated a code block exporting your method and appended it to the end of your file:
 ```rust
 #[pymodule]
-fn somecode(_py: Python, m: &PyModule) -> PyResult<()> {
+fn somecode(_py: Python, m: &Bound<'_, PyModule>) -> PyResult<()> {
   m.add_function(wrap_pyfunction!(square, m)?)?;
   Ok(())
 }
 ```
 
 ### Customizing an extension
 You can do all the above yourself. rustimport will detect that and only fill in the missing parts to make your extension work.
```

### Comparing `rustimport-1.4.0/README.md` & `rustimport-1.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # rustimport - Import Rust directly from Python! 
 
 <p align=center>
-    <a target="_blank" href="https://www.python.org/downloads/" title="Python version"><img src="https://img.shields.io/badge/python-%3E=_3.6-green.svg"></a>
+    <a target="_blank" href="https://www.python.org/downloads/" title="Python version"><img src="https://img.shields.io/badge/python-%3E=_3.8-green.svg"></a>
     <a target="_blank" href="https://pypi.org/project/rustimport/" title="PyPI version"><img src="https://img.shields.io/pypi/v/rustimport?logo=pypi"></a>
     <a target="_blank" href="LICENSE" title="License: MIT"><img src="https://img.shields.io/badge/License-MIT-blue.svg"></a></a>
 </p>
 
 rustimport was heavily inspired by and is partly based upon [cppimport](https://github.com/tbenthompson/cppimport). Check it out if you're interested in the same functionality for C and C++!
 
 ## Installation
@@ -89,15 +89,15 @@
 [dependencies.pyo3]
 version = "0.16.2"
 features = [ "extension-module",]
 ```
 3. It generated a code block exporting your method and appended it to the end of your file:
 ```rust
 #[pymodule]
-fn somecode(_py: Python, m: &PyModule) -> PyResult<()> {
+fn somecode(_py: Python, m: &Bound<'_, PyModule>) -> PyResult<()> {
   m.add_function(wrap_pyfunction!(square, m)?)?;
   Ok(())
 }
 ```
 
 ### Customizing an extension
 You can do all the above yourself. rustimport will detect that and only fill in the missing parts to make your extension work.
```

### Comparing `rustimport-1.4.0/rustimport/__init__.py` & `rustimport-1.5.0/rustimport/__init__.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.4.0/rustimport/__main__.py` & `rustimport-1.5.0/rustimport/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging
 import os
 import re
 import sys
 from typing import List
 
 from rustimport import build_all, build_filepath, settings
+from rustimport.pre_processing import PyO3Template
 
 rust_lib_template = """// rustimport:pyo3
 
 use pyo3::prelude::*;
 
 #[pyfunction]
 fn say_hello() {
@@ -17,15 +18,15 @@
 }
 
 // Uncomment the below to implement custom pyo3 binding code. Otherwise, 
 // rustimport will generate it for you for all functions annotated with
 // #[pyfunction] and all structs annotated with #[pyclass].
 //
 //#[pymodule]
-//fn {{EXTENSION_NAME}}(_py: Python, m: &PyModule) -> PyResult<()> {
+//fn {{EXTENSION_NAME}}(_py: Python, m: &Bound<'_, PyModule>) -> PyResult<()> {
 //    m.add_function(wrap_pyfunction!(say_hello, m)?)?;
 //    Ok(())
 //}
 """
 
 cargo_toml_template = """[package]
 name = "{{EXTENSION_NAME}}"
@@ -50,15 +51,15 @@
 # "cdylib" is necessary to produce a shared library for Python to import from.
 # Downstream Rust code (including code in `bin/`, `examples/`, and `examples/`) will not be able
 # to `use {{EXTENSION_NAME}};` unless the "rlib" or "lib" crate type is also included, e.g.:
 # crate-type = ["cdylib", "rlib"]
 crate-type = ["cdylib"]
 
 [dependencies]
-pyo3 = { version = "0.18.3", features = ["extension-module"] }
+pyo3 = { version = "{{PYO3_VERSION}}", features = ["extension-module"] }
 """
 
 
 def create_extension(name: str, cwd: str = '.'):
     if not re.match(r'^[a-zA-Z]\w*(\.rs)?$', name):
         raise ValueError(f"Invalid extension name: {name}. The name may only contain letters (preferably lowercase), "
                          f"numbers and underscores and should start with a letter.")
@@ -71,15 +72,17 @@
             f.write(rust_lib_template.replace('{{EXTENSION_NAME}}', name))
     else:
         src_dir = os.path.join(path, 'src')
         os.makedirs(src_dir)
         with open(os.path.join(src_dir, 'lib.rs'), 'w+') as f:
             f.write(rust_lib_template.replace('{{EXTENSION_NAME}}', name))
         with open(os.path.join(path, 'Cargo.toml'), 'w+') as f:
-            f.write(cargo_toml_template.replace('{{EXTENSION_NAME}}', name))
+            f.write(cargo_toml_template
+                    .replace('{{EXTENSION_NAME}}', name)
+                    .replace('{{PYO3_VERSION}}', PyO3Template.PYO3_VERSION))
         with open(os.path.join(path, '.rustimport'), 'w+') as f:
             f.write("This is a marker-file to make this crate importable by rustimport.")
 
 
 def _run_from_commandline(raw_args: List[str]):
     parser = argparse.ArgumentParser("rustimport")
```

### Comparing `rustimport-1.4.0/rustimport/checksum.py` & `rustimport-1.5.0/rustimport/checksum.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.4.0/rustimport/compiler.py` & `rustimport-1.5.0/rustimport/compiler.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.4.0/rustimport/error_handling.py` & `rustimport-1.5.0/rustimport/error_handling.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.4.0/rustimport/find.py` & `rustimport-1.5.0/rustimport/find.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.4.0/rustimport/import_hook.py` & `rustimport-1.5.0/rustimport/import_hook.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.4.0/rustimport/importable.py` & `rustimport-1.5.0/rustimport/importable.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.4.0/rustimport/ipython_magic.py` & `rustimport-1.5.0/rustimport/ipython_magic.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.4.0/rustimport/load.py` & `rustimport-1.5.0/rustimport/load.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.4.0/rustimport/pre_processing/__init__.py` & `rustimport-1.5.0/rustimport/pre_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.4.0/rustimport/pre_processing/base.py` & `rustimport-1.5.0/rustimport/pre_processing/base.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.4.0/rustimport/pre_processing/pyo3_template.py` & `rustimport-1.5.0/rustimport/pre_processing/pyo3_template.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import sys
 from typing import List
 
 from rustimport.pre_processing.base import Template
 
 
 class PyO3Template(Template):
+    PYO3_VERSION = "0.21.2"
+
     def process(self) -> Template.TemplatingResult:
         return Template.TemplatingResult(
             cargo_manifest=self.__generate_manifest(),
             contents=self.__process_content(),
             additional_cargo_args=self.__get_cargo_args(),
         )
 
@@ -21,15 +23,15 @@
                 'edition': '2021',
             },
             'lib': {
                 'name': self.lib_name,
                 'crate-type': ['cdylib'],
             },
             'dependencies': {
-                'pyo3': {'version': '0.18.3', 'features': ['extension-module']}
+                'pyo3': {'version': PyO3Template.PYO3_VERSION, 'features': ['extension-module']}
             }
         })
 
     def __process_content(self) -> bytes:
         if not re.search(rb'#\[pymodule]\s*(?:\w\s+)*?fn\s+([\w0-9]+)', self.contents):
             # If the file doesn't contain the "pymodule" macro, we generate it automatically
             return self.contents + b"\n\n" + self.__generate_pymodule()
@@ -39,15 +41,15 @@
         functions = re.finditer(
             rb'#\[pyfunction.*\s*(?:\w+\s+)*?(?:#\[pyo3.*)?\s*(?:\w+\s+)*?fn\s+([\w0-9]+)', self.contents, re.MULTILINE
         )
         structs = re.finditer(rb'#\[pyclass]\s*(?:\w+\s+)*?(?:struct|enum)\s+([\w0-9]+)', self.contents, re.MULTILINE)
 
         res = [
             b'#[pymodule]',
-            b'fn ' + self.lib_name.encode() + b'(_py: Python, m: &PyModule) -> PyResult<()> {',
+            b'fn ' + self.lib_name.encode() + b"(_py: Python, m: &Bound<'_, PyModule>) -> PyResult<()> {",
             *[
                 b'  m.add_function(wrap_pyfunction!(' + func.group(1) + b', m)?)?;'
                 for func in functions
             ],
             *[
                 b'  m.add_class::<' + struct.group(1) + b'>()?;'
                 for struct in structs
```

### Comparing `rustimport-1.4.0/rustimport/settings.py` & `rustimport-1.5.0/rustimport/settings.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.4.0/rustimport.egg-info/PKG-INFO` & `rustimport-1.5.0/rustimport.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rustimport
-Version: 1.4.0
+Version: 1.5.0
 Summary: Import Rust files directly from Python!
 Home-page: https://github.com/mityax/rustimport
 Author: mityax
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -17,15 +17,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: toml>=0.10.2
 
 # rustimport - Import Rust directly from Python! 
 
 <p align=center>
-    <a target="_blank" href="https://www.python.org/downloads/" title="Python version"><img src="https://img.shields.io/badge/python-%3E=_3.6-green.svg"></a>
+    <a target="_blank" href="https://www.python.org/downloads/" title="Python version"><img src="https://img.shields.io/badge/python-%3E=_3.8-green.svg"></a>
     <a target="_blank" href="https://pypi.org/project/rustimport/" title="PyPI version"><img src="https://img.shields.io/pypi/v/rustimport?logo=pypi"></a>
     <a target="_blank" href="LICENSE" title="License: MIT"><img src="https://img.shields.io/badge/License-MIT-blue.svg"></a></a>
 </p>
 
 rustimport was heavily inspired by and is partly based upon [cppimport](https://github.com/tbenthompson/cppimport). Check it out if you're interested in the same functionality for C and C++!
 
 ## Installation
@@ -109,15 +109,15 @@
 [dependencies.pyo3]
 version = "0.16.2"
 features = [ "extension-module",]
 ```
 3. It generated a code block exporting your method and appended it to the end of your file:
 ```rust
 #[pymodule]
-fn somecode(_py: Python, m: &PyModule) -> PyResult<()> {
+fn somecode(_py: Python, m: &Bound<'_, PyModule>) -> PyResult<()> {
   m.add_function(wrap_pyfunction!(square, m)?)?;
   Ok(())
 }
 ```
 
 ### Customizing an extension
 You can do all the above yourself. rustimport will detect that and only fill in the missing parts to make your extension work.
```

### Comparing `rustimport-1.4.0/rustimport.egg-info/SOURCES.txt` & `rustimport-1.5.0/rustimport.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rustimport-1.4.0/setup.py` & `rustimport-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.4.0/tests/test_cli.py` & `rustimport-1.5.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.4.0/tests/test_examples.py` & `rustimport-1.5.0/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.4.0/tests/test_ipython_magic.py` & `rustimport-1.5.0/tests/test_ipython_magic.py`

 * *Files identical despite different names*

