# Comparing `tmp/encyclopedia_vae-0.1.1.tar.gz` & `tmp/encyclopedia_vae-0.1.2.tar.gz`

## Comparing `encyclopedia_vae-0.1.1.tar` & `encyclopedia_vae-0.1.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.1/.python-version
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.1/Changelog.md
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.1/ruff.toml
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.1/.github/workflows/lint.yml
--rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.1/configs/bbvae.yaml
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.1/configs/betatc_vae.yaml
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.1/configs/cvae.yaml
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.1/configs/vae.yaml
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.1/encyclopedia_vae/__init__.py
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.1/encyclopedia_vae/cli.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.1/encyclopedia_vae/types_helpers.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.1/encyclopedia_vae/data/lit_celeba.py
--rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.1/encyclopedia_vae/lit_models/lit_vae.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.1/encyclopedia_vae/losses/__init__.py
--rw-r--r--   0        0        0     4736 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.1/encyclopedia_vae/losses/losses.py
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.1/encyclopedia_vae/models/__init__.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.1/encyclopedia_vae/models/base.py
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.1/encyclopedia_vae/models/beta_vae.py
--rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.1/encyclopedia_vae/models/betatc_vae.py
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.1/encyclopedia_vae/models/cvae.py
--rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.1/encyclopedia_vae/models/vanilla_vae.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.1/encyclopedia_vae/modules/__init__.py
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.1/encyclopedia_vae/modules/decoder.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.1/encyclopedia_vae/modules/encoder.py
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.1/encyclopedia_vae/modules/residual.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.1/encyclopedia_vae/modules/vectorquantizer.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.1/tests/test_betatcvae.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.1/tests/test_betavae.py
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.1/tests/test_cvae.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.1/tests/test_vae.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.1/.gitignore
--rw-r--r--   0        0        0    11455 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.1/LICENSE.md
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.1/README.md
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/.python-version
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/Changelog.md
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/ruff.toml
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/configs/bbvae.yaml
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/configs/betatc_vae.yaml
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/configs/cvae.yaml
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/configs/vae.yaml
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/encyclopedia_vae/__init__.py
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/encyclopedia_vae/cli.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/encyclopedia_vae/types_helpers.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/encyclopedia_vae/data/lit_celeba.py
+-rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/encyclopedia_vae/lit_models/lit_vae.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/encyclopedia_vae/losses/__init__.py
+-rw-r--r--   0        0        0     4736 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/encyclopedia_vae/losses/losses.py
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/encyclopedia_vae/models/__init__.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/encyclopedia_vae/models/base.py
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/encyclopedia_vae/models/beta_vae.py
+-rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/encyclopedia_vae/models/betatc_vae.py
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/encyclopedia_vae/models/cvae.py
+-rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/encyclopedia_vae/models/vanilla_vae.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/encyclopedia_vae/modules/__init__.py
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/encyclopedia_vae/modules/decoder.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/encyclopedia_vae/modules/encoder.py
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/encyclopedia_vae/modules/residual.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/encyclopedia_vae/modules/vectorquantizer.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/tests/test_betatcvae.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/tests/test_betavae.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/tests/test_cvae.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/tests/test_vae.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/.gitignore
+-rw-r--r--   0        0        0    11455 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/LICENSE.md
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/README.md
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 encyclopedia_vae-0.1.2/PKG-INFO
```

### Comparing `encyclopedia_vae-0.1.1/.pre-commit-config.yaml` & `encyclopedia_vae-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `encyclopedia_vae-0.1.1/.github/workflows/lint.yml` & `encyclopedia_vae-0.1.2/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `encyclopedia_vae-0.1.1/.github/workflows/publish.yml` & `encyclopedia_vae-0.1.2/.github/workflows/publish.yml`

 * *Files 1% similar despite different names*

```diff
@@ -64,20 +64,20 @@
 
     steps:
     - name: Download all the dists
       uses: actions/download-artifact@v3
       with:
         name: python-package-distributions
         path: dist/
-    - name: Sign the dists with Sigstore
-      uses: sigstore/gh-action-sigstore-python@v1.2.3
-      with:
-        inputs: >-
-          ./dist/*.tar.gz
-          ./dist/*.whl
+    # - name: Sign the dists with Sigstore
+    #   uses: sigstore/gh-action-sigstore-python@v1.2.3
+    #   with:
+    #     inputs: >-
+    #       ./dist/*.tar.gz
+    #       ./dist/*.whl
     - name: Create GitHub Release
       env:
         GITHUB_TOKEN: ${{ github.token }}
       run: >-
         gh release create
         '${{ github.ref_name }}'
         --repo '${{ github.repository }}'
```

### Comparing `encyclopedia_vae-0.1.1/.github/workflows/test.yml` & `encyclopedia_vae-0.1.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `encyclopedia_vae-0.1.1/encyclopedia_vae/types_helpers.py` & `encyclopedia_vae-0.1.2/encyclopedia_vae/types_helpers.py`

 * *Files identical despite different names*

### Comparing `encyclopedia_vae-0.1.1/encyclopedia_vae/data/lit_celeba.py` & `encyclopedia_vae-0.1.2/encyclopedia_vae/data/lit_celeba.py`

 * *Files identical despite different names*

### Comparing `encyclopedia_vae-0.1.1/encyclopedia_vae/lit_models/lit_vae.py` & `encyclopedia_vae-0.1.2/encyclopedia_vae/lit_models/lit_vae.py`

 * *Files identical despite different names*

### Comparing `encyclopedia_vae-0.1.1/encyclopedia_vae/losses/losses.py` & `encyclopedia_vae-0.1.2/encyclopedia_vae/losses/losses.py`

 * *Files identical despite different names*

### Comparing `encyclopedia_vae-0.1.1/encyclopedia_vae/models/__init__.py` & `encyclopedia_vae-0.1.2/encyclopedia_vae/models/__init__.py`

 * *Files identical despite different names*

### Comparing `encyclopedia_vae-0.1.1/encyclopedia_vae/models/base.py` & `encyclopedia_vae-0.1.2/encyclopedia_vae/models/base.py`

 * *Files identical despite different names*

### Comparing `encyclopedia_vae-0.1.1/encyclopedia_vae/models/beta_vae.py` & `encyclopedia_vae-0.1.2/encyclopedia_vae/models/beta_vae.py`

 * *Files identical despite different names*

### Comparing `encyclopedia_vae-0.1.1/encyclopedia_vae/models/betatc_vae.py` & `encyclopedia_vae-0.1.2/encyclopedia_vae/models/betatc_vae.py`

 * *Files identical despite different names*

### Comparing `encyclopedia_vae-0.1.1/encyclopedia_vae/models/cvae.py` & `encyclopedia_vae-0.1.2/encyclopedia_vae/models/cvae.py`

 * *Files identical despite different names*

### Comparing `encyclopedia_vae-0.1.1/encyclopedia_vae/models/vanilla_vae.py` & `encyclopedia_vae-0.1.2/encyclopedia_vae/models/vanilla_vae.py`

 * *Files identical despite different names*

### Comparing `encyclopedia_vae-0.1.1/encyclopedia_vae/modules/decoder.py` & `encyclopedia_vae-0.1.2/encyclopedia_vae/modules/decoder.py`

 * *Files identical despite different names*

### Comparing `encyclopedia_vae-0.1.1/encyclopedia_vae/modules/encoder.py` & `encyclopedia_vae-0.1.2/encyclopedia_vae/modules/encoder.py`

 * *Files identical despite different names*

### Comparing `encyclopedia_vae-0.1.1/encyclopedia_vae/modules/vectorquantizer.py` & `encyclopedia_vae-0.1.2/encyclopedia_vae/modules/vectorquantizer.py`

 * *Files identical despite different names*

### Comparing `encyclopedia_vae-0.1.1/tests/test_betatcvae.py` & `encyclopedia_vae-0.1.2/tests/test_betatcvae.py`

 * *Files identical despite different names*

### Comparing `encyclopedia_vae-0.1.1/tests/test_betavae.py` & `encyclopedia_vae-0.1.2/tests/test_betavae.py`

 * *Files identical despite different names*

### Comparing `encyclopedia_vae-0.1.1/tests/test_cvae.py` & `encyclopedia_vae-0.1.2/tests/test_cvae.py`

 * *Files identical despite different names*

### Comparing `encyclopedia_vae-0.1.1/tests/test_vae.py` & `encyclopedia_vae-0.1.2/tests/test_vae.py`

 * *Files identical despite different names*

### Comparing `encyclopedia_vae-0.1.1/LICENSE.md` & `encyclopedia_vae-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `encyclopedia_vae-0.1.1/README.md` & `encyclopedia_vae-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `encyclopedia_vae-0.1.1/pyproject.toml` & `encyclopedia_vae-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "encyclopedia-vae"
-version = "0.1.1"
+version = "0.1.2"
 description = "Add your description here"
 authors = [
     { name = "BaptisteMorisse", email = "bmorisse.pro@proton.me" }
 ]
 dependencies = [
     "torch>=2.3.0",
     "lightning[pytorch-extra]>=2.2.4",
```

### Comparing `encyclopedia_vae-0.1.1/PKG-INFO` & `encyclopedia_vae-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: encyclopedia-vae
-Version: 0.1.1
+Version: 0.1.2
 Summary: Add your description here
 Author-email: BaptisteMorisse <bmorisse.pro@proton.me>
 License-File: LICENSE.md
 Requires-Python: >=3.9
 Requires-Dist: einops>=0.8.0
 Requires-Dist: lightning[pytorch-extra]>=2.2.4
 Requires-Dist: torch>=2.3.0
```

