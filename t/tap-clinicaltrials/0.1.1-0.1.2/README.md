# Comparing `tmp/tap_clinicaltrials-0.1.1.tar.gz` & `tmp/tap_clinicaltrials-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Fri Mar  1 17:17:54 2024, max compression
+gzip compressed data, last modified: Mon May  6 13:36:51 2024, max compression
```

## Comparing `tap_clinicaltrials-0.1.1.tar` & `tap_clinicaltrials-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,26 @@
--rw-r--r--   0        0        0      910 2024-03-01 17:17:54.000000 tap_clinicaltrials-0.1.1/.copier-answers.yml
--rw-r--r--   0        0        0      862 2024-03-01 17:17:54.000000 tap_clinicaltrials-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      345 2024-03-01 17:17:54.000000 tap_clinicaltrials-0.1.1/CITATION.cff
--rw-r--r--   0        0        0     2887 2024-03-01 17:17:54.000000 tap_clinicaltrials-0.1.1/meltano.yml
--rw-r--r--   0        0        0     2359 2024-03-01 17:17:54.000000 tap_clinicaltrials-0.1.1/plugin.yaml
--rw-r--r--   0        0        0       74 2024-03-01 17:17:54.000000 tap_clinicaltrials-0.1.1/.github/FUNDING.yml
--rw-r--r--   0        0        0     1174 2024-03-01 17:17:54.000000 tap_clinicaltrials-0.1.1/.github/dependabot.yml
--rw-r--r--   0        0        0      873 2024-03-01 17:17:54.000000 tap_clinicaltrials-0.1.1/.github/workflows/build.yml
--rw-r--r--   0        0        0       23 2024-03-01 17:17:54.000000 tap_clinicaltrials-0.1.1/.github/workflows/constraints.txt
--rw-r--r--   0        0        0     1814 2024-03-01 17:17:54.000000 tap_clinicaltrials-0.1.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      409 2024-03-01 17:17:54.000000 tap_clinicaltrials-0.1.1/.secrets/.gitignore
--rw-r--r--   0        0        0       14 2024-03-01 17:17:54.000000 tap_clinicaltrials-0.1.1/output/.gitignore
--rw-r--r--   0        0        0     5777 2024-03-01 17:17:54.000000 tap_clinicaltrials-0.1.1/plugins/loaders/target-duckdb--jwills.lock
--rw-r--r--   0        0        0     1709 2024-03-01 17:17:54.000000 tap_clinicaltrials-0.1.1/plugins/loaders/target-jsonl--andyh1203.lock
--rw-r--r--   0        0        0       89 2024-03-01 17:17:54.000000 tap_clinicaltrials-0.1.1/tap_clinicaltrials/__init__.py
--rw-r--r--   0        0        0      137 2024-03-01 17:17:54.000000 tap_clinicaltrials-0.1.1/tap_clinicaltrials/__main__.py
--rw-r--r--   0        0        0     2411 2024-03-01 17:17:54.000000 tap_clinicaltrials-0.1.1/tap_clinicaltrials/discover.py
--rw-r--r--   0        0        0     2953 2024-03-01 17:17:54.000000 tap_clinicaltrials-0.1.1/tap_clinicaltrials/streams.py
--rw-r--r--   0        0        0     1842 2024-03-01 17:17:54.000000 tap_clinicaltrials-0.1.1/tap_clinicaltrials/tap.py
--rw-r--r--   0        0        0       24 2024-03-01 17:17:54.000000 tap_clinicaltrials-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0       92 2024-03-01 17:17:54.000000 tap_clinicaltrials-0.1.1/tests/conftest.py
--rw-r--r--   0        0        0     2138 2024-03-01 17:17:54.000000 tap_clinicaltrials-0.1.1/tests/test_core.py
--rw-r--r--   0        0        0     1899 2024-03-01 17:17:54.000000 tap_clinicaltrials-0.1.1/.gitignore
--rw-r--r--   0        0        0    11355 2024-03-01 17:17:54.000000 tap_clinicaltrials-0.1.1/LICENSE
--rw-r--r--   0        0        0     5956 2024-03-01 17:17:54.000000 tap_clinicaltrials-0.1.1/README.md
--rw-r--r--   0        0        0     3528 2024-03-01 17:17:54.000000 tap_clinicaltrials-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    20386 2024-03-01 17:17:54.000000 tap_clinicaltrials-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      910 2024-05-06 13:36:51.000000 tap_clinicaltrials-0.1.2/.copier-answers.yml
+-rw-r--r--   0        0        0      862 2024-05-06 13:36:51.000000 tap_clinicaltrials-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      345 2024-05-06 13:36:51.000000 tap_clinicaltrials-0.1.2/CITATION.cff
+-rw-r--r--   0        0        0     2887 2024-05-06 13:36:51.000000 tap_clinicaltrials-0.1.2/meltano.yml
+-rw-r--r--   0        0        0     2359 2024-05-06 13:36:51.000000 tap_clinicaltrials-0.1.2/plugin.yaml
+-rw-r--r--   0        0        0     1174 2024-05-06 13:36:51.000000 tap_clinicaltrials-0.1.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      873 2024-05-06 13:36:51.000000 tap_clinicaltrials-0.1.2/.github/workflows/build.yml
+-rw-r--r--   0        0        0       23 2024-05-06 13:36:51.000000 tap_clinicaltrials-0.1.2/.github/workflows/constraints.txt
+-rw-r--r--   0        0        0     1838 2024-05-06 13:36:51.000000 tap_clinicaltrials-0.1.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0      409 2024-05-06 13:36:51.000000 tap_clinicaltrials-0.1.2/.secrets/.gitignore
+-rw-r--r--   0        0        0       14 2024-05-06 13:36:51.000000 tap_clinicaltrials-0.1.2/output/.gitignore
+-rw-r--r--   0        0        0     5777 2024-05-06 13:36:51.000000 tap_clinicaltrials-0.1.2/plugins/loaders/target-duckdb--jwills.lock
+-rw-r--r--   0        0        0     1709 2024-05-06 13:36:51.000000 tap_clinicaltrials-0.1.2/plugins/loaders/target-jsonl--andyh1203.lock
+-rw-r--r--   0        0        0       89 2024-05-06 13:36:51.000000 tap_clinicaltrials-0.1.2/tap_clinicaltrials/__init__.py
+-rw-r--r--   0        0        0      137 2024-05-06 13:36:51.000000 tap_clinicaltrials-0.1.2/tap_clinicaltrials/__main__.py
+-rw-r--r--   0        0        0     2411 2024-05-06 13:36:51.000000 tap_clinicaltrials-0.1.2/tap_clinicaltrials/discover.py
+-rw-r--r--   0        0        0     2953 2024-05-06 13:36:51.000000 tap_clinicaltrials-0.1.2/tap_clinicaltrials/streams.py
+-rw-r--r--   0        0        0     1842 2024-05-06 13:36:51.000000 tap_clinicaltrials-0.1.2/tap_clinicaltrials/tap.py
+-rw-r--r--   0        0        0       24 2024-05-06 13:36:51.000000 tap_clinicaltrials-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0       92 2024-05-06 13:36:51.000000 tap_clinicaltrials-0.1.2/tests/conftest.py
+-rw-r--r--   0        0        0     2138 2024-05-06 13:36:51.000000 tap_clinicaltrials-0.1.2/tests/test_core.py
+-rw-r--r--   0        0        0     1899 2024-05-06 13:36:51.000000 tap_clinicaltrials-0.1.2/.gitignore
+-rw-r--r--   0        0        0    11355 2024-05-06 13:36:51.000000 tap_clinicaltrials-0.1.2/LICENSE
+-rw-r--r--   0        0        0     5956 2024-05-06 13:36:51.000000 tap_clinicaltrials-0.1.2/README.md
+-rw-r--r--   0        0        0     3528 2024-05-06 13:36:51.000000 tap_clinicaltrials-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    20540 2024-05-06 13:36:51.000000 tap_clinicaltrials-0.1.2/PKG-INFO
```

### Comparing `tap_clinicaltrials-0.1.1/.copier-answers.yml` & `tap_clinicaltrials-0.1.2/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `tap_clinicaltrials-0.1.1/.pre-commit-config.yaml` & `tap_clinicaltrials-0.1.2/.pre-commit-config.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-json
         exclude: "\\.vscode/.*.json"
       - id: check-toml
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
 
   - repo: https://github.com/tox-dev/pyproject-fmt
-    rev: "1.7.0"
+    rev: "1.8.0"
     hooks:
       - id: pyproject-fmt
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.2.2"
+    rev: "v0.4.2"
     hooks:
       - id: ruff
         name: Ruff lint
         args: [--fix, --exit-non-zero-on-fix, --show-fixes]
       - id: ruff-format
         name: Ruff format
 
   - repo: https://github.com/pre-commit/pre-commit
-    rev: v3.6.2
+    rev: v3.7.0
     hooks:
       - id: validate_manifest
 
   - repo: https://github.com/python-jsonschema/check-jsonschema
-    rev: 0.28.0
+    rev: 0.28.2
     hooks:
     - id: check-dependabot
     - id: check-github-workflows
```

### Comparing `tap_clinicaltrials-0.1.1/meltano.yml` & `tap_clinicaltrials-0.1.2/meltano.yml`

 * *Files identical despite different names*

### Comparing `tap_clinicaltrials-0.1.1/plugin.yaml` & `tap_clinicaltrials-0.1.2/plugin.yaml`

 * *Files identical despite different names*

### Comparing `tap_clinicaltrials-0.1.1/.github/dependabot.yml` & `tap_clinicaltrials-0.1.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `tap_clinicaltrials-0.1.1/.github/workflows/build.yml` & `tap_clinicaltrials-0.1.2/.github/workflows/build.yml`

 * *Files 1% similar despite different names*

```diff
@@ -33,8 +33,8 @@
         path: dist
     - uses: svenstaro/upload-release-action@v2
       with:
         file: dist/*.whl
         tag: ${{ github.ref }}
         overwrite: true
         file_glob: true
-    - uses: pypa/gh-action-pypi-publish@v1.8.12
+    - uses: pypa/gh-action-pypi-publish@v1.8.14
```

### Comparing `tap_clinicaltrials-0.1.1/.github/workflows/test.yml` & `tap_clinicaltrials-0.1.2/.github/workflows/test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
       - .github/workflows/constraints.txt
 
 jobs:
   test:
     runs-on: ubuntu-latest
     env:
       FORCE_COLOR: "1"
-      PIP_CONSTRAINT: .github/workflows/constraints.txt
+      PIP_CONSTRAINT: ${{ github.workspace }}/.github/workflows/constraints.txt
     strategy:
       fail-fast: false
       matrix:
         script: ["test:integration"]
         python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
         include:
         - { script: "test:dependencies", python-version: "3.12" }
```

### Comparing `tap_clinicaltrials-0.1.1/plugins/loaders/target-duckdb--jwills.lock` & `tap_clinicaltrials-0.1.2/plugins/loaders/target-duckdb--jwills.lock`

 * *Files identical despite different names*

### Comparing `tap_clinicaltrials-0.1.1/plugins/loaders/target-jsonl--andyh1203.lock` & `tap_clinicaltrials-0.1.2/plugins/loaders/target-jsonl--andyh1203.lock`

 * *Files identical despite different names*

### Comparing `tap_clinicaltrials-0.1.1/tap_clinicaltrials/discover.py` & `tap_clinicaltrials-0.1.2/tap_clinicaltrials/discover.py`

 * *Files identical despite different names*

### Comparing `tap_clinicaltrials-0.1.1/tap_clinicaltrials/streams.py` & `tap_clinicaltrials-0.1.2/tap_clinicaltrials/streams.py`

 * *Files identical despite different names*

### Comparing `tap_clinicaltrials-0.1.1/tap_clinicaltrials/tap.py` & `tap_clinicaltrials-0.1.2/tap_clinicaltrials/tap.py`

 * *Files identical despite different names*

### Comparing `tap_clinicaltrials-0.1.1/tests/test_core.py` & `tap_clinicaltrials-0.1.2/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `tap_clinicaltrials-0.1.1/.gitignore` & `tap_clinicaltrials-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `tap_clinicaltrials-0.1.1/LICENSE` & `tap_clinicaltrials-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_clinicaltrials-0.1.1/README.md` & `tap_clinicaltrials-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `tap_clinicaltrials-0.1.1/pyproject.toml` & `tap_clinicaltrials-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -28,31 +28,31 @@
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
   "requests<3,>=2",
   "requests-cache<2,>=1",
-  "singer-sdk~=0.36.0",
+  "singer-sdk~=0.37.0",
 ]
 optional-dependencies.dev = [
   "tap-clinicaltrials[testing,typing]",
 ]
 optional-dependencies.testing = [
   "deptry>=0.12",
   "pytest>=7.4",
   "singer-sdk[testing]",
 ]
 optional-dependencies.typing = [
   "mypy",
   "types-requests",
 ]
-urls.documentation = "https://github.com/edgarrmondragon/tap-clinicaltrials#readme"
-urls.homepage = "https://github.com/edgarrmondragon/tap-clinicaltrials"
-urls.repository = "https://github.com/edgarrmondragon/tap-clinicaltrials"
+urls.Documentation = "https://github.com/edgarrmondragon/tap-clinicaltrials#readme"
+urls.Homepage = "https://github.com/edgarrmondragon/tap-clinicaltrials"
+urls.Repository = "https://github.com/edgarrmondragon/tap-clinicaltrials"
 scripts."tap-clinicaltrials" = "tap_clinicaltrials.tap:TapClinicalTrials.cli"
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.envs.sync.scripts]
 console = "tap-clinicaltrials {args}"
```

### Comparing `tap_clinicaltrials-0.1.1/PKG-INFO` & `tap_clinicaltrials-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: tap-clinicaltrials
-Version: 0.1.1
+Version: 0.1.2
 Summary: `tap-clinicaltrials` is a Singer tap for ClinicalTrials.gov, built with the Meltano SDK for Singer Taps.
-Project-URL: documentation, https://github.com/edgarrmondragon/tap-clinicaltrials#readme
-Project-URL: homepage, https://github.com/edgarrmondragon/tap-clinicaltrials
-Project-URL: repository, https://github.com/edgarrmondragon/tap-clinicaltrials
+Project-URL: Documentation, https://github.com/edgarrmondragon/tap-clinicaltrials#readme
+Project-URL: Homepage, https://github.com/edgarrmondragon/tap-clinicaltrials
+Project-URL: Repository, https://github.com/edgarrmondragon/tap-clinicaltrials
 Author-email: Edgar Ramírez-Mondragón <edgarrmondragon@hey.com>
 Maintainer-email: Edgar Ramírez-Mondragón <edgarrmondragon@hey.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -215,17 +215,21 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Requires-Dist: requests-cache<2,>=1
 Requires-Dist: requests<3,>=2
-Requires-Dist: singer-sdk~=0.36.0
+Requires-Dist: singer-sdk~=0.37.0
 Provides-Extra: dev
-Requires-Dist: tap-clinicaltrials[testing,typing]; extra == 'dev'
+Requires-Dist: deptry>=0.12; extra == 'dev'
+Requires-Dist: mypy; extra == 'dev'
+Requires-Dist: pytest>=7.4; extra == 'dev'
+Requires-Dist: singer-sdk[testing]; extra == 'dev'
+Requires-Dist: types-requests; extra == 'dev'
 Provides-Extra: testing
 Requires-Dist: deptry>=0.12; extra == 'testing'
 Requires-Dist: pytest>=7.4; extra == 'testing'
 Requires-Dist: singer-sdk[testing]; extra == 'testing'
 Provides-Extra: typing
 Requires-Dist: mypy; extra == 'typing'
 Requires-Dist: types-requests; extra == 'typing'
```

