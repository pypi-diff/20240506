# Comparing `tmp/leap_data_management_utils-0.0.7.tar.gz` & `tmp/leap_data_management_utils-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leap_data_management_utils-0.0.7.tar", last modified: Wed May  1 03:03:23 2024, max compression
+gzip compressed data, was "leap_data_management_utils-0.0.8.tar", last modified: Mon May  6 21:29:17 2024, max compression
```

## Comparing `leap_data_management_utils-0.0.7.tar` & `leap_data_management_utils-0.0.8.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 03:03:23.258377 leap_data_management_utils-0.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 03:03:23.254377 leap_data_management_utils-0.0.7/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-01 03:03:09.000000 leap_data_management_utils-0.0.7/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 03:03:23.254377 leap_data_management_utils-0.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-01 03:03:09.000000 leap_data_management_utils-0.0.7/.github/workflows/catalog-ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-01 03:03:09.000000 leap_data_management_utils-0.0.7/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-01 03:03:09.000000 leap_data_management_utils-0.0.7/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-01 03:03:09.000000 leap_data_management_utils-0.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-01 03:03:09.000000 leap_data_management_utils-0.0.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-01 03:03:09.000000 leap_data_management_utils-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-01 03:03:23.258377 leap_data_management_utils-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-01 03:03:09.000000 leap_data_management_utils-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 03:03:23.254377 leap_data_management_utils-0.0.7/ci/
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-01 03:03:09.000000 leap_data_management_utils-0.0.7/ci/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 03:03:23.258377 leap_data_management_utils-0.0.7/leap_data_management_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-01 03:03:09.000000 leap_data_management_utils-0.0.7/leap_data_management_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-01 03:03:23.000000 leap_data_management_utils-0.0.7/leap_data_management_utils/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8944 2024-05-01 03:03:09.000000 leap_data_management_utils-0.0.7/leap_data_management_utils/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-01 03:03:09.000000 leap_data_management_utils-0.0.7/leap_data_management_utils/cmip_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-01 03:03:09.000000 leap_data_management_utils-0.0.7/leap_data_management_utils/cmip_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9115 2024-05-01 03:03:09.000000 leap_data_management_utils-0.0.7/leap_data_management_utils/cmip_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     9450 2024-05-01 03:03:09.000000 leap_data_management_utils-0.0.7/leap_data_management_utils/data_management_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 03:03:23.258377 leap_data_management_utils-0.0.7/leap_data_management_utils/testing_notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    25238 2024-05-01 03:03:09.000000 leap_data_management_utils-0.0.7/leap_data_management_utils/testing_notebooks/testing_cmip_bigquery.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 03:03:23.258377 leap_data_management_utils-0.0.7/leap_data_management_utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-01 03:03:09.000000 leap_data_management_utils-0.0.7/leap_data_management_utils/tests/test_cmip_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-01 03:03:09.000000 leap_data_management_utils-0.0.7/leap_data_management_utils/tests/test_data_management_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 03:03:23.258377 leap_data_management_utils-0.0.7/leap_data_management_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-01 03:03:23.000000 leap_data_management_utils-0.0.7/leap_data_management_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-01 03:03:23.000000 leap_data_management_utils-0.0.7/leap_data_management_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 03:03:23.000000 leap_data_management_utils-0.0.7/leap_data_management_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-01 03:03:23.000000 leap_data_management_utils-0.0.7/leap_data_management_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-01 03:03:23.000000 leap_data_management_utils-0.0.7/leap_data_management_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-01 03:03:23.000000 leap_data_management_utils-0.0.7/leap_data_management_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-01 03:03:09.000000 leap_data_management_utils-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 03:03:23.258377 leap_data_management_utils-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:29:17.335491 leap_data_management_utils-0.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:29:17.327491 leap_data_management_utils-0.0.8/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-06 21:29:04.000000 leap_data_management_utils-0.0.8/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:29:17.327491 leap_data_management_utils-0.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-06 21:29:04.000000 leap_data_management_utils-0.0.8/.github/workflows/catalog-ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-06 21:29:04.000000 leap_data_management_utils-0.0.8/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-06 21:29:04.000000 leap_data_management_utils-0.0.8/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-06 21:29:04.000000 leap_data_management_utils-0.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-06 21:29:04.000000 leap_data_management_utils-0.0.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-06 21:29:04.000000 leap_data_management_utils-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-06 21:29:17.335491 leap_data_management_utils-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-06 21:29:04.000000 leap_data_management_utils-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:29:17.331491 leap_data_management_utils-0.0.8/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-06 21:29:04.000000 leap_data_management_utils-0.0.8/ci/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:29:17.331491 leap_data_management_utils-0.0.8/leap_data_management_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-06 21:29:04.000000 leap_data_management_utils-0.0.8/leap_data_management_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-06 21:29:17.000000 leap_data_management_utils-0.0.8/leap_data_management_utils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-06 21:29:04.000000 leap_data_management_utils-0.0.8/leap_data_management_utils/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-06 21:29:04.000000 leap_data_management_utils-0.0.8/leap_data_management_utils/cmip_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-06 21:29:04.000000 leap_data_management_utils-0.0.8/leap_data_management_utils/cmip_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9115 2024-05-06 21:29:04.000000 leap_data_management_utils-0.0.8/leap_data_management_utils/cmip_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9450 2024-05-06 21:29:04.000000 leap_data_management_utils-0.0.8/leap_data_management_utils/data_management_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:29:17.331491 leap_data_management_utils-0.0.8/leap_data_management_utils/testing_notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    25238 2024-05-06 21:29:04.000000 leap_data_management_utils-0.0.8/leap_data_management_utils/testing_notebooks/testing_cmip_bigquery.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:29:17.331491 leap_data_management_utils-0.0.8/leap_data_management_utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-06 21:29:04.000000 leap_data_management_utils-0.0.8/leap_data_management_utils/tests/test_cmip_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-06 21:29:04.000000 leap_data_management_utils-0.0.8/leap_data_management_utils/tests/test_data_management_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:29:17.331491 leap_data_management_utils-0.0.8/leap_data_management_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-06 21:29:17.000000 leap_data_management_utils-0.0.8/leap_data_management_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-06 21:29:17.000000 leap_data_management_utils-0.0.8/leap_data_management_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 21:29:17.000000 leap_data_management_utils-0.0.8/leap_data_management_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-06 21:29:17.000000 leap_data_management_utils-0.0.8/leap_data_management_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-06 21:29:17.000000 leap_data_management_utils-0.0.8/leap_data_management_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-06 21:29:17.000000 leap_data_management_utils-0.0.8/leap_data_management_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-06 21:29:04.000000 leap_data_management_utils-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 21:29:17.335491 leap_data_management_utils-0.0.8/setup.cfg
```

### Comparing `leap_data_management_utils-0.0.7/.github/workflows/catalog-ci.yaml` & `leap_data_management_utils-0.0.8/.github/workflows/catalog-ci.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             bash
           cache-environment: true
           cache-downloads: true
           post-cleanup: "all"
 
       - name: Install package
         run: |
-          python -m pip install .
+          python -m pip install ".[catalog]"
 
       - name: Validate Feedstocks and Generate Catalog
         run: |
           leap-catalog --help
           leap-catalog validate --single https://github.com/leap-stc/proto_feedstock/blob/main/feedstock/catalog.yaml
           leap-catalog generate --path https://raw.githubusercontent.com/leap-stc/data-management/staging/catalog/input.yaml --output catalog/
           cat catalog/output/consolidated-web-catalog.json | jq
```

### Comparing `leap_data_management_utils-0.0.7/.github/workflows/ci.yaml` & `leap_data_management_utils-0.0.8/.github/workflows/ci.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,18 @@
       - "main"
   pull_request:
     branches:
       - "*"
   schedule:
     - cron: "0 13 * * 1"
 
+concurrency:
+  group: ${{ github.workflow }}-${{ github.ref }}
+  cancel-in-progress: true
+
 jobs:
   build:
     defaults:
       run:
         shell: bash -l {0}
     strategy:
       fail-fast: false
```

### Comparing `leap_data_management_utils-0.0.7/.github/workflows/release.yaml` & `leap_data_management_utils-0.0.8/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.7/.gitignore` & `leap_data_management_utils-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.7/.pre-commit-config.yaml` & `leap_data_management_utils-0.0.8/.pre-commit-config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -9,15 +9,15 @@
       - id: check-docstring-first
       - id: check-json
       - id: check-yaml
       - id: debug-statements
       - id: mixed-line-ending
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.3.7"
+    rev: "v0.4.3"
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
       - id: ruff-format
 
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: v4.0.0-alpha.8
```

### Comparing `leap_data_management_utils-0.0.7/LICENSE` & `leap_data_management_utils-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.7/PKG-INFO` & `leap_data_management_utils-0.0.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leap-data-management-utils
-Version: 0.0.7
+Version: 0.0.8
 Summary: LEAP / pangeo-forge-recipes extension library for logging data in Google Big Query
 Author-email: LEAP <leap@columbia.edu>
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
@@ -12,31 +12,35 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: apache-beam
 Requires-Dist: cftime
-Requires-Dist: db_dtypes
-Requires-Dist: google-api-core
-Requires-Dist: google-cloud-bigquery
-Requires-Dist: pandas
-Requires-Dist: pangeo-forge-esgf
-Requires-Dist: pangeo-forge-recipes
-Requires-Dist: pydantic-core
-Requires-Dist: pydantic>=2
-Requires-Dist: pyyaml
 Requires-Dist: ruamel.yaml
-Requires-Dist: universal-pathlib
 Requires-Dist: xarray
 Requires-Dist: zarr
+Provides-Extra: pangeo-forge
+Requires-Dist: db_dtypes; extra == "pangeo-forge"
+Requires-Dist: google-api-core; extra == "pangeo-forge"
+Requires-Dist: google-cloud-bigquery; extra == "pangeo-forge"
+Requires-Dist: pandas; extra == "pangeo-forge"
+Requires-Dist: pangeo-forge-esgf; extra == "pangeo-forge"
+Requires-Dist: pangeo-forge-recipes; extra == "pangeo-forge"
+Requires-Dist: apache-beam; extra == "pangeo-forge"
+Provides-Extra: catalog
+Requires-Dist: pydantic>=2; extra == "catalog"
+Requires-Dist: universal-pathlib; extra == "catalog"
+Requires-Dist: pydantic-core; extra == "catalog"
+Provides-Extra: complete
+Requires-Dist: leap-data-management-utils[catalog,pangeo-forge]; extra == "complete"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
+Requires-Dist: leap-data-management-utils[complete]; extra == "test"
 Provides-Extra: dev
-Requires-Dist: leap-data-leap_data_management_utils[test]; extra == "dev"
+Requires-Dist: leap-data-management-utils[test]; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 
 # LEAP Data Management Utils
 
 This Repo is intended to be installed via the `requirements.txt` during recipe execution in `pangeo-forge-recipes`. It currently contains beam transforms to log information into BigQuery tables. Additional shared utilities and checks that are commonly used between LEAP pangeo-forge-feedstocks can live here.
```

### Comparing `leap_data_management_utils-0.0.7/leap_data_management_utils/catalog.py` & `leap_data_management_utils-0.0.8/leap_data_management_utils/catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 import json
 import traceback
 
 import pydantic
 import pydantic_core
 import requests
 import upath
-import yaml
+from ruamel.yaml import YAML
+
+yaml = YAML(typ='safe')
 
 
 def s3_to_https(s3_url: str) -> str:
     # Split the URL into its components
     s3_parts = s3_url.split('/')
 
     # Get the bucket name from the first part of the URL
@@ -76,18 +78,18 @@
     tags: list[str] | None = pydantic.Field(None, description='Tags of the dataset')
     links: list[Link] | None = None
     stores: list[Store] | None = None
     meta_yaml_url: pydantic.HttpUrl | None = pydantic.Field(None, alias='ncviewjs:meta_yaml_url')
 
     @classmethod
     def from_yaml(cls, path: str):
-        content = yaml.safe_load(upath.UPath(path).read_text())
+        content = yaml.load(upath.UPath(path).read_text())
         if 'ncviewjs:meta_yaml_url' in content:
             meta_url = convert_to_raw_github_url(content['ncviewjs:meta_yaml_url'])
-            meta = yaml.safe_load(upath.UPath(meta_url).read_text())
+            meta = yaml.load(upath.UPath(meta_url).read_text())
             content = content | meta
         data = cls.model_validate(content)
         return data
 
 
 def convert_to_raw_github_url(github_url):
     # Check if the URL is already a raw URL
@@ -109,15 +111,15 @@
         super().__init__(self.errors)
 
 
 def collect_feedstocks(path: upath.UPath) -> list[upath.UPath]:
     """Collects all the datasets in the given directory."""
 
     url = convert_to_raw_github_url(path)
-    if not (feedstocks := yaml.safe_load(upath.UPath(url).read_text())['feedstocks']):
+    if not (feedstocks := yaml.load(upath.UPath(url).read_text())['feedstocks']):
         raise FileNotFoundError(f'No YAML files (.yaml or .yml) found in {path}')
     return feedstocks
 
 
 def format_report(title: str, feedstocks: list[dict], include_traceback: bool = False) -> str:
     report = f'{title} ({len(feedstocks)})\n'
     if not feedstocks:
```

### Comparing `leap_data_management_utils-0.0.7/leap_data_management_utils/cmip_catalog.py` & `leap_data_management_utils-0.0.8/leap_data_management_utils/cmip_catalog.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,9 @@
 import pandas as pd
-
-# TODO: This should live in pangeo-forge-esgf?
-# Need to test over there if the changes regarding member_id/varaint_label are correct
-# are breaking anything.
-# from pangeo_forge_esgf.utils import CMIP6_naming_schema_official
-CMIP6_naming_schema_official = 'mip_era.activity_id.institution_id.source_id.experiment_id.member_id.table_id.variable_id.grid_label.version'
+from pangeo_forge_esgf.utils import CMIP6_naming_schema
 
 
 def _maybe_prepend_dummy_dcpp(s: str):
     if '-' not in s:
         return 'none-' + s
     else:
         return s
@@ -22,15 +17,15 @@
         return f'{sub_experiment_id}-{variant_label}'
     else:
         return variant_label
 
 
 def bq_df_to_intake_esm(df: pd.DataFrame) -> pd.DataFrame:
     df = df.copy()
-    iid_facets = CMIP6_naming_schema_official.split('.')
+    iid_facets = CMIP6_naming_schema.split('.')
     # some legit pandas magic here: https://stackoverflow.com/a/39358924
     df_out = df['instance_id'].str.split('.', expand=True)
     df_out = df_out.rename(columns={i: f for i, f in enumerate(iid_facets)})
     df_out['zstore'] = df['store']
     df_out[['sub_experiment_id', 'variant_label']] = (
         df_out['member_id']
         .apply(lambda s: _maybe_prepend_dummy_dcpp(s))
```

### Comparing `leap_data_management_utils-0.0.7/leap_data_management_utils/cmip_testing.py` & `leap_data_management_utils-0.0.8/leap_data_management_utils/cmip_testing.py`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.7/leap_data_management_utils/cmip_transforms.py` & `leap_data_management_utils-0.0.8/leap_data_management_utils/cmip_transforms.py`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.7/leap_data_management_utils/data_management_transforms.py` & `leap_data_management_utils-0.0.8/leap_data_management_utils/data_management_transforms.py`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.7/leap_data_management_utils/testing_notebooks/testing_cmip_bigquery.ipynb` & `leap_data_management_utils-0.0.8/leap_data_management_utils/testing_notebooks/testing_cmip_bigquery.ipynb`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.7/leap_data_management_utils/tests/test_cmip_transforms.py` & `leap_data_management_utils-0.0.8/leap_data_management_utils/tests/test_cmip_transforms.py`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.7/leap_data_management_utils/tests/test_data_management_transforms.py` & `leap_data_management_utils-0.0.8/leap_data_management_utils/tests/test_data_management_transforms.py`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.7/leap_data_management_utils.egg-info/PKG-INFO` & `leap_data_management_utils-0.0.8/leap_data_management_utils.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leap-data-management-utils
-Version: 0.0.7
+Version: 0.0.8
 Summary: LEAP / pangeo-forge-recipes extension library for logging data in Google Big Query
 Author-email: LEAP <leap@columbia.edu>
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
@@ -12,31 +12,35 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: apache-beam
 Requires-Dist: cftime
-Requires-Dist: db_dtypes
-Requires-Dist: google-api-core
-Requires-Dist: google-cloud-bigquery
-Requires-Dist: pandas
-Requires-Dist: pangeo-forge-esgf
-Requires-Dist: pangeo-forge-recipes
-Requires-Dist: pydantic-core
-Requires-Dist: pydantic>=2
-Requires-Dist: pyyaml
 Requires-Dist: ruamel.yaml
-Requires-Dist: universal-pathlib
 Requires-Dist: xarray
 Requires-Dist: zarr
+Provides-Extra: pangeo-forge
+Requires-Dist: db_dtypes; extra == "pangeo-forge"
+Requires-Dist: google-api-core; extra == "pangeo-forge"
+Requires-Dist: google-cloud-bigquery; extra == "pangeo-forge"
+Requires-Dist: pandas; extra == "pangeo-forge"
+Requires-Dist: pangeo-forge-esgf; extra == "pangeo-forge"
+Requires-Dist: pangeo-forge-recipes; extra == "pangeo-forge"
+Requires-Dist: apache-beam; extra == "pangeo-forge"
+Provides-Extra: catalog
+Requires-Dist: pydantic>=2; extra == "catalog"
+Requires-Dist: universal-pathlib; extra == "catalog"
+Requires-Dist: pydantic-core; extra == "catalog"
+Provides-Extra: complete
+Requires-Dist: leap-data-management-utils[catalog,pangeo-forge]; extra == "complete"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
+Requires-Dist: leap-data-management-utils[complete]; extra == "test"
 Provides-Extra: dev
-Requires-Dist: leap-data-leap_data_management_utils[test]; extra == "dev"
+Requires-Dist: leap-data-management-utils[test]; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 
 # LEAP Data Management Utils
 
 This Repo is intended to be installed via the `requirements.txt` during recipe execution in `pangeo-forge-recipes`. It currently contains beam transforms to log information into BigQuery tables. Additional shared utilities and checks that are commonly used between LEAP pangeo-forge-feedstocks can live here.
```

### Comparing `leap_data_management_utils-0.0.7/leap_data_management_utils.egg-info/SOURCES.txt` & `leap_data_management_utils-0.0.8/leap_data_management_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `leap_data_management_utils-0.0.7/pyproject.toml` & `leap_data_management_utils-0.0.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -18,42 +18,51 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
 ]
 dependencies = [
-    "apache-beam",
     "cftime",
+    "ruamel.yaml",
+    "xarray",
+    "zarr",
+]
+
+[project.optional-dependencies]
+
+pangeo-forge=[
     "db_dtypes",
     "google-api-core",
     "google-cloud-bigquery",
     "pandas",
     "pangeo-forge-esgf",
     "pangeo-forge-recipes",
-    "pydantic-core",
+    "apache-beam",
+    ]
+
+catalog = [
     "pydantic>=2",
-    "pyyaml",
-    "ruamel.yaml",
     "universal-pathlib",
-    "xarray",
-    "zarr",
-]
+    "pydantic-core",
+    ]
 
-[project.optional-dependencies]
+
+
+complete = ["leap-data-management-utils[pangeo-forge,catalog]"]
 test = [
-    "pytest"
+    "pytest",
+    "leap-data-management-utils[complete]",
 ]
 
 dev = [
-    "leap-data-leap_data_management_utils[test]",
-    "pre-commit"
+    "leap-data-management-utils[test]",
+    "pre-commit",
 ]
 
-
 [project.scripts]
 leap-catalog = "leap_data_management_utils.catalog:main"
 
 
 [tool.setuptools.packages.find]
 include = ["leap_data_management_utils*"]
```

