# Comparing `tmp/gptk-0.2.11.tar.gz` & `tmp/gptk-0.2.9.tar.gz`

## Comparing `gptk-0.2.11.tar` & `gptk-0.2.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 gptk-0.2.11/.github/workflows/publishing.yml
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 gptk-0.2.11/src/gptk/__init__.py
--rw-r--r--   0        0        0    15130 2020-02-02 00:00:00.000000 gptk-0.2.11/src/gptk/autoprops.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 gptk-0.2.11/src/gptk/constants.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 gptk-0.2.11/src/gptk/encoding.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 gptk-0.2.11/src/gptk/enums.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 gptk-0.2.11/src/gptk/singletons.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 gptk-0.2.11/src/gptk/data/gptk_units.txt
--rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 gptk-0.2.11/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 gptk-0.2.11/LICENSE.md
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 gptk-0.2.11/README.md
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 gptk-0.2.11/pyproject.toml
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 gptk-0.2.11/PKG-INFO
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 gptk-0.2.9/.github/workflows/publishing.yml
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 gptk-0.2.9/src/gptk/__init__.py
+-rw-r--r--   0        0        0    15130 2020-02-02 00:00:00.000000 gptk-0.2.9/src/gptk/autoprops.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 gptk-0.2.9/src/gptk/constants.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 gptk-0.2.9/src/gptk/encoding.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 gptk-0.2.9/src/gptk/enums.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 gptk-0.2.9/src/gptk/singletons.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 gptk-0.2.9/src/gptk/data/gptk_units.txt
+-rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 gptk-0.2.9/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 gptk-0.2.9/LICENSE.md
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 gptk-0.2.9/README.md
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 gptk-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 gptk-0.2.9/PKG-INFO
```

### Comparing `gptk-0.2.11/.github/workflows/publishing.yml` & `gptk-0.2.9/.github/workflows/publishing.yml`

 * *Files 2% similar despite different names*

```diff
@@ -6,27 +6,27 @@
   build:
     name: Build distribution 📦
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python
-      uses: actions/setup-python@v5
+      uses: actions/setup-python@v4
       with:
         python-version: "3.11"
     - name: Install pypa/build
       run: >-
         python3 -m
         pip install
         build
         --user
     - name: Build a binary wheel and a source tarball
       run: python3 -m build
     - name: Store the distribution packages
-      uses: actions/upload-artifact@v4
+      uses: actions/upload-artifact@v3
       with:
         name: python-package-distributions
         path: dist/
 
   publish-to-pypi:
     name: >-
       Publish Python 🐍 distribution 📦 to PyPI
@@ -38,15 +38,15 @@
       name: pypi
       url: https://pypi.org/p/gptk  # Replace <package-name> with your PyPI project name
     permissions:
       id-token: write  # IMPORTANT: mandatory for trusted publishing
 
     steps:
     - name: Download all the dists
-      uses: actions/download-artifact@v4
+      uses: actions/download-artifact@v3
       with:
         name: python-package-distributions
         path: dist/
     - name: Publish distribution 📦 to PyPI
       uses: pypa/gh-action-pypi-publish@release/v1
 
   github-release:
@@ -87,9 +87,7 @@
       # Upload to GitHub Release using the `gh` CLI.
       # `dist/` contains the built packages, and the
       # sigstore-produced signatures and certificates.
       run: >-
         gh release upload
         '${{ github.ref_name }}' dist/**
         --repo '${{ github.repository }}'
-
-
```

### Comparing `gptk-0.2.11/src/gptk/__init__.py` & `gptk-0.2.9/src/gptk/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,14 +17,19 @@
 
 try:
     from .singletons import *
 except ImportError:
     from gptk.singletons import *
 
 try:
+    from .datamodels import *
+except ImportError:
+    from gptk.datamodels import *
+
+try:
     from .enums import *
 except ImportError:
     from gptk.enums import *
 
 try:
     from .autoprops import *
 except ImportError:
```

### Comparing `gptk-0.2.11/src/gptk/autoprops.py` & `gptk-0.2.9/src/gptk/autoprops.py`

 * *Files identical despite different names*

### Comparing `gptk-0.2.11/src/gptk/encoding.py` & `gptk-0.2.9/src/gptk/encoding.py`

 * *Files identical despite different names*

### Comparing `gptk-0.2.11/src/gptk/enums.py` & `gptk-0.2.9/src/gptk/enums.py`

 * *Files identical despite different names*

### Comparing `gptk-0.2.11/src/gptk/singletons.py` & `gptk-0.2.9/src/gptk/singletons.py`

 * *Files identical despite different names*

### Comparing `gptk-0.2.11/src/gptk/data/gptk_units.txt` & `gptk-0.2.9/src/gptk/data/gptk_units.txt`

 * *Files identical despite different names*

### Comparing `gptk-0.2.11/.gitignore` & `gptk-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `gptk-0.2.11/LICENSE.md` & `gptk-0.2.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gptk-0.2.11/pyproject.toml` & `gptk-0.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"] 
 build-backend = "hatchling.build"
 
 [project]
 name = "gptk"
-version = "0.2.11"
+version = "0.2.9"
 authors = [
   { name="J.T. Hartzfeld", email="johnathan.t.hartzfeld@gmail.com" },
 ]
 description = "A General Python Tool Kit, suitable for most projects."
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.11"
```

### Comparing `gptk-0.2.11/PKG-INFO` & `gptk-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gptk
-Version: 0.2.11
+Version: 0.2.9
 Summary: A General Python Tool Kit, suitable for most projects.
 Project-URL: Homepage, https://github.com/JTHartzfeld/gptk
 Project-URL: Bug Tracker, https://github.com/JTHartzfeld/gptk/issues
 Author-email: "J.T. Hartzfeld" <johnathan.t.hartzfeld@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: MIT License
```

