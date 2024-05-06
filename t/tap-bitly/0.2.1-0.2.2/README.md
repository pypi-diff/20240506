# Comparing `tmp/tap_bitly-0.2.1.tar.gz` & `tmp/tap_bitly-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Fri Mar  1 15:00:42 2024, max compression
+gzip compressed data, last modified: Mon May  6 13:56:30 2024, max compression
```

## Comparing `tap_bitly-0.2.1.tar` & `tap_bitly-0.2.2.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0      620 2024-03-01 15:00:42.000000 tap_bitly-0.2.1/.copier-answers.yml
--rw-r--r--   0        0        0     1011 2024-03-01 15:00:42.000000 tap_bitly-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1013 2024-03-01 15:00:42.000000 tap_bitly-0.2.1/meltano.yml
--rw-r--r--   0        0        0      712 2024-03-01 15:00:42.000000 tap_bitly-0.2.1/.github/FUNDING.yml
--rw-r--r--   0        0        0     1284 2024-03-01 15:00:42.000000 tap_bitly-0.2.1/.github/dependabot.yml
--rw-r--r--   0        0        0       23 2024-03-01 15:00:42.000000 tap_bitly-0.2.1/.github/workflows/constraints.txt
--rw-r--r--   0        0        0      809 2024-03-01 15:00:42.000000 tap_bitly-0.2.1/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1571 2024-03-01 15:00:42.000000 tap_bitly-0.2.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      409 2024-03-01 15:00:42.000000 tap_bitly-0.2.1/.secrets/.gitignore
--rw-r--r--   0        0        0       14 2024-03-01 15:00:42.000000 tap_bitly-0.2.1/output/.gitignore
--rw-r--r--   0        0        0       44 2024-03-01 15:00:42.000000 tap_bitly-0.2.1/tap_bitly/__init__.py
--rw-r--r--   0        0        0     1095 2024-03-01 15:00:42.000000 tap_bitly-0.2.1/tap_bitly/client.py
--rw-r--r--   0        0        0    15293 2024-03-01 15:00:42.000000 tap_bitly-0.2.1/tap_bitly/streams.py
--rw-r--r--   0        0        0     1531 2024-03-01 15:00:42.000000 tap_bitly-0.2.1/tap_bitly/tap.py
--rw-r--r--   0        0        0       39 2024-03-01 15:00:42.000000 tap_bitly-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0       92 2024-03-01 15:00:42.000000 tap_bitly-0.2.1/tests/conftest.py
--rw-r--r--   0        0        0      432 2024-03-01 15:00:42.000000 tap_bitly-0.2.1/tests/test_core.py
--rw-r--r--   0        0        0     2264 2024-03-01 15:00:42.000000 tap_bitly-0.2.1/.gitignore
--rw-r--r--   0        0        0    11337 2024-03-01 15:00:42.000000 tap_bitly-0.2.1/LICENSE
--rw-r--r--   0        0        0     6081 2024-03-01 15:00:42.000000 tap_bitly-0.2.1/README.md
--rw-r--r--   0        0        0     3561 2024-03-01 15:00:42.000000 tap_bitly-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    20499 2024-03-01 15:00:42.000000 tap_bitly-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      620 2024-05-06 13:56:30.000000 tap_bitly-0.2.2/.copier-answers.yml
+-rw-r--r--   0        0        0     1011 2024-05-06 13:56:30.000000 tap_bitly-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1013 2024-05-06 13:56:30.000000 tap_bitly-0.2.2/meltano.yml
+-rw-r--r--   0        0        0     1210 2024-05-06 13:56:30.000000 tap_bitly-0.2.2/.github/dependabot.yml
+-rw-r--r--   0        0        0       23 2024-05-06 13:56:30.000000 tap_bitly-0.2.2/.github/workflows/constraints.txt
+-rw-r--r--   0        0        0      809 2024-05-06 13:56:30.000000 tap_bitly-0.2.2/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1595 2024-05-06 13:56:30.000000 tap_bitly-0.2.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0      409 2024-05-06 13:56:30.000000 tap_bitly-0.2.2/.secrets/.gitignore
+-rw-r--r--   0        0        0       14 2024-05-06 13:56:30.000000 tap_bitly-0.2.2/output/.gitignore
+-rw-r--r--   0        0        0       44 2024-05-06 13:56:30.000000 tap_bitly-0.2.2/tap_bitly/__init__.py
+-rw-r--r--   0        0        0     1095 2024-05-06 13:56:30.000000 tap_bitly-0.2.2/tap_bitly/client.py
+-rw-r--r--   0        0        0    15293 2024-05-06 13:56:30.000000 tap_bitly-0.2.2/tap_bitly/streams.py
+-rw-r--r--   0        0        0     1531 2024-05-06 13:56:30.000000 tap_bitly-0.2.2/tap_bitly/tap.py
+-rw-r--r--   0        0        0       39 2024-05-06 13:56:30.000000 tap_bitly-0.2.2/tests/__init__.py
+-rw-r--r--   0        0        0       92 2024-05-06 13:56:30.000000 tap_bitly-0.2.2/tests/conftest.py
+-rw-r--r--   0        0        0      432 2024-05-06 13:56:30.000000 tap_bitly-0.2.2/tests/test_core.py
+-rw-r--r--   0        0        0     2264 2024-05-06 13:56:30.000000 tap_bitly-0.2.2/.gitignore
+-rw-r--r--   0        0        0    11337 2024-05-06 13:56:30.000000 tap_bitly-0.2.2/LICENSE
+-rw-r--r--   0        0        0     6081 2024-05-06 13:56:30.000000 tap_bitly-0.2.2/README.md
+-rw-r--r--   0        0        0     3597 2024-05-06 13:56:30.000000 tap_bitly-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0    20773 2024-05-06 13:56:30.000000 tap_bitly-0.2.2/PKG-INFO
```

### Comparing `tap_bitly-0.2.1/.copier-answers.yml` & `tap_bitly-0.2.2/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `tap_bitly-0.2.1/.pre-commit-config.yaml` & `tap_bitly-0.2.2/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -19,23 +19,23 @@
 
   - repo: https://github.com/tox-dev/pyproject-fmt
     rev: "1.7.0"
     hooks:
       - id: pyproject-fmt
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.2.0"
+    rev: "v0.3.5"
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix, --show-fixes]
       - id: ruff-format
 
   - repo: https://github.com/pre-commit/pre-commit
-    rev: v3.6.0
+    rev: v3.7.0
     hooks:
       - id: validate_manifest
 
   - repo: https://github.com/python-jsonschema/check-jsonschema
-    rev: 0.27.4
+    rev: 0.28.1
     hooks:
     - id: check-dependabot
     - id: check-github-workflows
```

### Comparing `tap_bitly-0.2.1/meltano.yml` & `tap_bitly-0.2.2/meltano.yml`

 * *Files identical despite different names*

### Comparing `tap_bitly-0.2.1/.github/dependabot.yml` & `tap_bitly-0.2.2/.github/dependabot.yml`

 * *Files 14% similar despite different names*

```diff
@@ -13,18 +13,14 @@
       time: "07:00"
     reviewers:
       - "edgarrmondragon"
     commit-message:
       prefix: "feat(deps): "
       prefix-development: "chore(deps-dev): "
     versioning-strategy: increase-if-necessary
-    groups:
-      singer-sdk:
-        patterns:
-          - "singer-sdk*"
   - package-ecosystem: pip
     directory: "/.github/workflows"
     schedule:
       interval: "monthly"
       timezone: "America/Mexico_City"
       time: "07:00"
     reviewers:
```

### Comparing `tap_bitly-0.2.1/.github/workflows/release.yaml` & `tap_bitly-0.2.2/.github/workflows/release.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -31,8 +31,8 @@
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

### Comparing `tap_bitly-0.2.1/.github/workflows/test.yml` & `tap_bitly-0.2.2/.github/workflows/test.yml`

 * *Files 13% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   workflow_dispatch:
 
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

### Comparing `tap_bitly-0.2.1/tap_bitly/client.py` & `tap_bitly-0.2.2/tap_bitly/client.py`

 * *Files identical despite different names*

### Comparing `tap_bitly-0.2.1/tap_bitly/streams.py` & `tap_bitly-0.2.2/tap_bitly/streams.py`

 * *Files identical despite different names*

### Comparing `tap_bitly-0.2.1/tap_bitly/tap.py` & `tap_bitly-0.2.2/tap_bitly/tap.py`

 * *Files identical despite different names*

### Comparing `tap_bitly-0.2.1/.gitignore` & `tap_bitly-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `tap_bitly-0.2.1/LICENSE` & `tap_bitly-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_bitly-0.2.1/README.md` & `tap_bitly-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `tap_bitly-0.2.1/pyproject.toml` & `tap_bitly-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -27,38 +27,41 @@
   "Programming Language :: Python :: 3.12",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
   "requests>=2",
-  "singer-sdk~=0.35.0",
+  "singer-sdk~=0.37.0",
 ]
 optional-dependencies.dev = [
   "tap-bitly[testing,typing]",
 ]
 optional-dependencies.testing = [
   "deptry>=0.12",
   "pytest>=7.4",
   "pytest-durations",
   "pytest-github-actions-annotate-failures",
-  "singer-sdk[testing]~=0.35.0",
+  "singer-sdk[testing]",
 ]
 optional-dependencies.typing = [
   "mypy",
   "types-requests",
 ]
-urls.documentation = "https://github.com/edgarrmondragon/tap-bitly#readme"
-urls.homepage = "https://github.com/edgarrmondragon/tap-bitly"
-urls.repository = "https://github.com/edgarrmondragon/tap-bitly"
+urls.Documentation = "https://github.com/edgarrmondragon/tap-bitly#readme"
+urls.Homepage = "https://github.com/edgarrmondragon/tap-bitly"
+urls.Repository = "https://github.com/edgarrmondragon/tap-bitly"
 scripts.tap-bitly = "tap_bitly.tap:TapBitly.cli"
 
 [tool.hatch.version]
 source = "vcs"
 
+[tool.hatch.envs.default]
+installer = "uv"
+
 [tool.hatch.envs.sync.scripts]
 console = "tap-bitly {args}"
 jsonl = "tap-bitly {args} > tap-bitly.jsonl"
 
 [tool.hatch.envs.test]
 features = ["testing"]
 [tool.hatch.envs.test.scripts]
```

### Comparing `tap_bitly-0.2.1/PKG-INFO` & `tap_bitly-0.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: tap-bitly
-Version: 0.2.1
+Version: 0.2.2
 Summary: `tap-bitly` is a Singer tap for Bitly, built with the Meltano SDK for Singer Taps.
-Project-URL: documentation, https://github.com/edgarrmondragon/tap-bitly#readme
-Project-URL: homepage, https://github.com/edgarrmondragon/tap-bitly
-Project-URL: repository, https://github.com/edgarrmondragon/tap-bitly
+Project-URL: Documentation, https://github.com/edgarrmondragon/tap-bitly#readme
+Project-URL: Homepage, https://github.com/edgarrmondragon/tap-bitly
+Project-URL: Repository, https://github.com/edgarrmondragon/tap-bitly
 Author-email: Edgar Ramirez-Mondragon <edgarrm358@gmail.com>
 Maintainer-email: Edgar Ramirez-Mondragon <edgarrm358@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -214,23 +214,29 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Requires-Dist: requests>=2
-Requires-Dist: singer-sdk~=0.35.0
+Requires-Dist: singer-sdk~=0.37.0
 Provides-Extra: dev
-Requires-Dist: tap-bitly[testing,typing]; extra == 'dev'
+Requires-Dist: deptry>=0.12; extra == 'dev'
+Requires-Dist: mypy; extra == 'dev'
+Requires-Dist: pytest-durations; extra == 'dev'
+Requires-Dist: pytest-github-actions-annotate-failures; extra == 'dev'
+Requires-Dist: pytest>=7.4; extra == 'dev'
+Requires-Dist: singer-sdk[testing]; extra == 'dev'
+Requires-Dist: types-requests; extra == 'dev'
 Provides-Extra: testing
 Requires-Dist: deptry>=0.12; extra == 'testing'
 Requires-Dist: pytest-durations; extra == 'testing'
 Requires-Dist: pytest-github-actions-annotate-failures; extra == 'testing'
 Requires-Dist: pytest>=7.4; extra == 'testing'
-Requires-Dist: singer-sdk[testing]~=0.35.0; extra == 'testing'
+Requires-Dist: singer-sdk[testing]; extra == 'testing'
 Provides-Extra: typing
 Requires-Dist: mypy; extra == 'typing'
 Requires-Dist: types-requests; extra == 'typing'
 Description-Content-Type: text/markdown
 
 <div align="center">
```

