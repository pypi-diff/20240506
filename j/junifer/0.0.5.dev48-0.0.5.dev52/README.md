# Comparing `tmp/junifer-0.0.5.dev48.tar.gz` & `tmp/junifer-0.0.5.dev52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "junifer-0.0.5.dev48.tar", last modified: Tue Apr 30 12:37:41 2024, max compression
+gzip compressed data, was "junifer-0.0.5.dev52.tar", last modified: Mon May  6 10:29:41 2024, max compression
```

## Comparing `junifer-0.0.5.dev48.tar` & `junifer-0.0.5.dev52.tar`

### file list

```diff
@@ -1,454 +1,455 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.409692 junifer-0.0.5.dev48/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.345693 junifer-0.0.5.dev48/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.345693 junifer-0.0.5.dev48/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/.github/ISSUE_TEMPLATE/dataset-request.yml
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/.github/ISSUE_TEMPLATE/documention-request.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/.github/ISSUE_TEMPLATE/marker-request.yml
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.345693 junifer-0.0.5.dev48/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/.github/workflows/ci-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/.github/workflows/docs-preview.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34354 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-04-30 12:37:41.409692 junifer-0.0.5.dev48/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/conda-env.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.349693 junifer-0.0.5.dev48/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.333693 junifer-0.0.5.dev48/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.349693 junifer-0.0.5.dev48/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.349693 junifer-0.0.5.dev48/docs/_static/js/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/_static/js/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.349693 junifer-0.0.5.dev48/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/_templates/versions.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.353693 junifer-0.0.5.dev48/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/api/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/api/configs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/api/data.rst
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/api/datagrabbers.rst
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/api/datareaders.rst
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/api/markers.rst
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/api/nilearn.rst
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/api/onthefly.rst
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/api/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/api/preprocessing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/api/stats.rst
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/api/storage.rst
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/api/testing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/api/utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)    25180 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/builtin.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.353693 junifer-0.0.5.dev48/docs/changes/
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/changes/contributors.inc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.353693 junifer-0.0.5.dev48/docs/changes/newsfragments/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/changes/newsfragments/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/changes/newsfragments/115.doc
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/changes/newsfragments/161.feature
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/changes/newsfragments/273.feature
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/changes/newsfragments/323.feature
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/changes/newsfragments/324.bugfix
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/changes/newsfragments/330.doc
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/changes/newsfragments/332.bugfix
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/changes/newsfragments/336.removal
--rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     8636 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/contribution.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.357693 junifer-0.0.5.dev48/docs/extending/
--rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/extending/coordinates.rst
--rw-r--r--   0 runner    (1001) docker     (127)    18384 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/extending/datagrabber.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/extending/dependencies.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/extending/extension.rst
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/extending/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9693 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/extending/marker.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/extending/masks.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/extending/parcellations.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/extending/preprocessor.rst
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/help.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.357693 junifer-0.0.5.dev48/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    62148 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/images/junifer_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/links.inc
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/maintaining.rst
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/redirect.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.357693 junifer-0.0.5.dev48/docs/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/sphinxext/gh_substitutions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/starting.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.357693 junifer-0.0.5.dev48/docs/understanding/
--rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/understanding/data.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/understanding/datagrabber.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/understanding/datareader.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/understanding/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/understanding/marker.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/understanding/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/understanding/preprocess.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/understanding/storage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.357693 junifer-0.0.5.dev48/docs/using/
--rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/using/codeless.rst
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/using/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/using/masks.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/using/queueing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/using/running.rst
--rw-r--r--   0 runner    (1001) docker     (127)    26282 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/docs/whats_new.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.357693 junifer-0.0.5.dev48/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/examples/norun_hcpfc_pearson.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/examples/norun_ukbvm_gmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/examples/run_compute_parcel_mean.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/examples/run_datagrabber_bids_datalad.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/examples/run_ets_rss_marker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/examples/run_junifer_julearn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/examples/run_run_gmd_mean.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.361693 junifer-0.0.5.dev48/examples/yamls/
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/examples/yamls/gmd_mean.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/examples/yamls/gmd_mean_htcondor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/examples/yamls/partly_cloudy_agg_mean_tian.yml
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/examples/yamls/ukb_gmd_mean.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/ignore_words.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.361693 junifer-0.0.5.dev48/junifer/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-30 12:37:41.000000 junifer-0.0.5.dev48/junifer/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.361693 junifer-0.0.5.dev48/junifer/api/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15329 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/api/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/api/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    13055 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/api/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/api/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.361693 junifer-0.0.5.dev48/junifer/api/queue_context/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/api/queue_context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9561 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/api/queue_context/gnu_parallel_local_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13233 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/api/queue_context/htcondor_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/api/queue_context/queue_context_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.361693 junifer-0.0.5.dev48/junifer/api/queue_context/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/api/queue_context/tests/test_gnu_parallel_local_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8619 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/api/queue_context/tests/test_htcondor_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.365693 junifer-0.0.5.dev48/junifer/api/res/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.365693 junifer-0.0.5.dev48/junifer/api/res/afni/
--rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/api/res/afni/3dAFNItoNIFTI
--rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/api/res/afni/3dRSFC
--rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/api/res/afni/3dReHo
--rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/api/res/afni/afni
--rwxr-xr-x   0 runner    (1001) docker     (127)     1130 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/api/res/afni/run_afni_docker.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.365693 junifer-0.0.5.dev48/junifer/api/res/ants/
--rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/api/res/ants/ResampleImage
--rwxr-xr-x   0 runner    (1001) docker     (127)       57 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/api/res/ants/antsApplyTransforms
--rwxr-xr-x   0 runner    (1001) docker     (127)       65 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/api/res/ants/antsApplyTransformsToPoints
--rwxr-xr-x   0 runner    (1001) docker     (127)     1119 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/api/res/ants/run_ants_docker.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.365693 junifer-0.0.5.dev48/junifer/api/res/fsl/
--rwxr-xr-x   0 runner    (1001) docker     (127)       46 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/api/res/fsl/applywarp
--rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/api/res/fsl/flirt
--rwxr-xr-x   0 runner    (1001) docker     (127)       49 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/api/res/fsl/img2imgcoord
--rwxr-xr-x   0 runner    (1001) docker     (127)     1122 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/api/res/fsl/run_fsl_docker.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       49 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/api/res/fsl/std2imgcoord
--rwxr-xr-x   0 runner    (1001) docker     (127)      517 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/api/res/run_conda.bash
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/api/res/run_conda.zsh
--rwxr-xr-x   0 runner    (1001) docker     (127)      507 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/api/res/run_venv.bash
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/api/res/run_venv.zsh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.365693 junifer-0.0.5.dev48/junifer/api/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.365693 junifer-0.0.5.dev48/junifer/api/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/api/tests/data/gmd_mean.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/api/tests/data/gmd_mean_htcondor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/api/tests/data/partly_cloudy_agg_mean_tian.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/api/tests/test_api_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10969 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/api/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    17753 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/api/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/api/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.365693 junifer-0.0.5.dev48/junifer/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.369693 junifer-0.0.5.dev48/junifer/configs/juseless/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/configs/juseless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.369693 junifer-0.0.5.dev48/junifer/configs/juseless/datagrabbers/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/configs/juseless/datagrabbers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/configs/juseless/datagrabbers/camcan_vbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/configs/juseless/datagrabbers/ixi_vbm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.369693 junifer-0.0.5.dev48/junifer/configs/juseless/datagrabbers/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/configs/juseless/datagrabbers/tests/test_ucla.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/configs/juseless/datagrabbers/ucla.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/configs/juseless/datagrabbers/ukb_vbm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.369693 junifer-0.0.5.dev48/junifer/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.337693 junifer-0.0.5.dev48/junifer/data/VOIs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.373693 junifer-0.0.5.dev48/junifer/data/VOIs/meta/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/data/VOIs/meta/AutobiographicalMemory_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/data/VOIs/meta/CogAC_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/data/VOIs/meta/CogAR_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/data/VOIs/meta/DMNBuckner_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/data/VOIs/meta/Empathy_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/data/VOIs/meta/Motor_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/data/VOIs/meta/MultiTask_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/data/VOIs/meta/PhysioStress_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/data/VOIs/meta/Power2013_MNI_VOIs.tsv
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/data/VOIs/meta/Rew_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/data/VOIs/meta/Somatosensory_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/data/VOIs/meta/ToM_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/data/VOIs/meta/VigAtt_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/data/VOIs/meta/WM_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/data/VOIs/meta/eMDN_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/data/VOIs/meta/eSAD_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/data/VOIs/meta/extDMN_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12381 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/data/coordinates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.337693 junifer-0.0.5.dev48/junifer/data/masks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.373693 junifer-0.0.5.dev48/junifer/data/masks/vickery-patil/
--rw-r--r--   0 runner    (1001) docker     (127)    88270 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)    12862 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)     8700 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)    21427 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/data/masks.py
--rw-r--r--   0 runner    (1001) docker     (127)    65225 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/data/parcellations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/data/template_spaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.377693 junifer-0.0.5.dev48/junifer/data/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/data/tests/test_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/data/tests/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15878 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/data/tests/test_masks.py
--rw-r--r--   0 runner    (1001) docker     (127)    38222 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/data/tests/test_parcellations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/data/tests/test_template_spaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.377693 junifer-0.0.5.dev48/junifer/datagrabber/
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/datagrabber/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.377693 junifer-0.0.5.dev48/junifer/datagrabber/aomic/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/datagrabber/aomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/datagrabber/aomic/id1000.py
--rw-r--r--   0 runner    (1001) docker     (127)     8466 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/datagrabber/aomic/piop1.py
--rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/datagrabber/aomic/piop2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.377693 junifer-0.0.5.dev48/junifer/datagrabber/aomic/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/datagrabber/aomic/tests/test_id1000.py
--rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/datagrabber/aomic/tests/test_piop1.py
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/datagrabber/aomic/tests/test_piop2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/datagrabber/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10659 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/datagrabber/datalad_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12945 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/datagrabber/dmcc13_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.377693 junifer-0.0.5.dev48/junifer/datagrabber/hcp1200/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/datagrabber/hcp1200/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/datagrabber/hcp1200/datalad_hcp1200.py
--rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/datagrabber/hcp1200/hcp1200.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.377693 junifer-0.0.5.dev48/junifer/datagrabber/hcp1200/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10765 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/datagrabber/hcp1200/tests/test_hcp1200.py
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/datagrabber/multiple.py
--rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/datagrabber/pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/datagrabber/pattern_datalad.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.381693 junifer-0.0.5.dev48/junifer/datagrabber/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/datagrabber/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/datagrabber/tests/test_datagrabber_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16285 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/datagrabber/tests/test_datalad_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/datagrabber/tests/test_dmcc13_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     5659 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/datagrabber/tests/test_multiple.py
--rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/datagrabber/tests/test_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     6483 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/datagrabber/tests/test_pattern_datalad.py
--rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/datagrabber/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.381693 junifer-0.0.5.dev48/junifer/datareader/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/datareader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/datareader/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.381693 junifer-0.0.5.dev48/junifer/datareader/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/datareader/tests/test_default_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.381693 junifer-0.0.5.dev48/junifer/external/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.337693 junifer-0.0.5.dev48/junifer/external/h5io/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.381693 junifer-0.0.5.dev48/junifer/external/h5io/h5io/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-30 12:37:37.000000 junifer-0.0.5.dev48/junifer/external/h5io/h5io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28748 2024-04-30 12:37:37.000000 junifer-0.0.5.dev48/junifer/external/h5io/h5io/_h5io.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-30 12:37:37.000000 junifer-0.0.5.dev48/junifer/external/h5io/h5io/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-30 12:37:37.000000 junifer-0.0.5.dev48/junifer/external/h5io/h5io/chunked_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-30 12:37:37.000000 junifer-0.0.5.dev48/junifer/external/h5io/h5io/chunked_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.381693 junifer-0.0.5.dev48/junifer/external/nilearn/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/external/nilearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16274 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/external/nilearn/junifer_nifti_spheres_masker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.381693 junifer-0.0.5.dev48/junifer/external/nilearn/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10370 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.385692 junifer-0.0.5.dev48/junifer/markers/
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/collection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.385692 junifer-0.0.5.dev48/junifer/markers/complexity/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/complexity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/complexity/complexity_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/complexity/hurst_exponent.py
--rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/complexity/multiscale_entropy_auc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/complexity/perm_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/complexity/range_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/complexity/range_entropy_auc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/complexity/sample_entropy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.385692 junifer-0.0.5.dev48/junifer/markers/complexity/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/complexity/tests/test_complexity_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/complexity/tests/test_hurst_exponent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/complexity/tests/test_multiscale_entropy_auc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/complexity/tests/test_perm_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/complexity/tests/test_range_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/complexity/tests/test_range_entropy_auc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/complexity/tests/test_sample_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/complexity/tests/test_weighted_perm_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/complexity/weighted_perm_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/ets_rss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.389692 junifer-0.0.5.dev48/junifer/markers/falff/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/falff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/falff/_afni_falff.py
--rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/falff/_junifer_falff.py
--rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/falff/falff_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/falff/falff_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/falff/falff_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.389692 junifer-0.0.5.dev48/junifer/markers/falff/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/falff/tests/test_falff_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/falff/tests/test_falff_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.389692 junifer-0.0.5.dev48/junifer/markers/functional_connectivity/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/functional_connectivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py
--rw-r--r--   0 runner    (1001) docker     (127)     5179 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/functional_connectivity/functional_connectivity_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/functional_connectivity/functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/functional_connectivity/functional_connectivity_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.389692 junifer-0.0.5.dev48/junifer/markers/functional_connectivity/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py
--rw-r--r--   0 runner    (1001) docker     (127)     8702 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/parcel_aggregation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.393692 junifer-0.0.5.dev48/junifer/markers/reho/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/reho/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/reho/_afni_reho.py
--rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/reho/_junifer_reho.py
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/reho/reho_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/reho/reho_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/reho/reho_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.393692 junifer-0.0.5.dev48/junifer/markers/reho/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/reho/tests/test_reho_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/reho/tests/test_reho_spheres.py
--rw-r--r--   0 runner    (1001) docker     (127)     8275 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/sphere_aggregation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.393692 junifer-0.0.5.dev48/junifer/markers/temporal_snr/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/temporal_snr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/temporal_snr/temporal_snr_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/temporal_snr/temporal_snr_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/temporal_snr/temporal_snr_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.393692 junifer-0.0.5.dev48/junifer/markers/temporal_snr/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/temporal_snr/tests/test_temporal_snr_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.393692 junifer-0.0.5.dev48/junifer/markers/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/tests/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/tests/test_ets_rss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/tests/test_marker_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/tests/test_markers_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    26531 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/tests/test_parcel_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9747 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/tests/test_sphere_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/markers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.393692 junifer-0.0.5.dev48/junifer/onthefly/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/onthefly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/onthefly/read_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.393692 junifer-0.0.5.dev48/junifer/onthefly/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/onthefly/tests/test_read_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.397692 junifer-0.0.5.dev48/junifer/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/pipeline/pipeline_step_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/pipeline/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/pipeline/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.397692 junifer-0.0.5.dev48/junifer/pipeline/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7807 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/pipeline/tests/test_pipeline_step_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/pipeline/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/pipeline/tests/test_update_meta_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/pipeline/tests/test_workdir_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/pipeline/update_meta_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     8039 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/pipeline/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/pipeline/workdir_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.397692 junifer-0.0.5.dev48/junifer/preprocess/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/preprocess/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.397692 junifer-0.0.5.dev48/junifer/preprocess/confounds/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/preprocess/confounds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20841 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/preprocess/confounds/fmriprep_confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.397692 junifer-0.0.5.dev48/junifer/preprocess/confounds/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    20757 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.397692 junifer-0.0.5.dev48/junifer/preprocess/smoothing/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/preprocess/smoothing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/preprocess/smoothing/_afni_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/preprocess/smoothing/_fsl_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/preprocess/smoothing/_nilearn_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/preprocess/smoothing/smoothing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.397692 junifer-0.0.5.dev48/junifer/preprocess/smoothing/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/preprocess/smoothing/tests/test_smoothing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.397692 junifer-0.0.5.dev48/junifer/preprocess/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/preprocess/tests/test_preprocess_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.401692 junifer-0.0.5.dev48/junifer/preprocess/warping/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/preprocess/warping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/preprocess/warping/_ants_warper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/preprocess/warping/_fsl_warper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/preprocess/warping/space_warper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.401692 junifer-0.0.5.dev48/junifer/preprocess/warping/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/preprocess/warping/tests/test_space_warper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.401692 junifer-0.0.5.dev48/junifer/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9654 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/storage/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    35631 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/storage/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/storage/pandas_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    21244 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/storage/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.401692 junifer-0.0.5.dev48/junifer/storage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    29338 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/storage/tests/test_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/storage/tests/test_pandas_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    28318 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/storage/tests/test_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/storage/tests/test_storage_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11854 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/storage/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/storage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.401692 junifer-0.0.5.dev48/junifer/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.401692 junifer-0.0.5.dev48/junifer/testing/data/
--rw-r--r--   0 runner    (1001) docker     (127)   406849 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv
--rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/testing/datagrabbers.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/testing/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.405692 junifer-0.0.5.dev48/junifer/testing/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/testing/tests/test_partlycloudytesting_datagrabber.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/testing/tests/test_spmauditory_datagrabber.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/testing/tests/test_testing_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/testing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.405692 junifer-0.0.5.dev48/junifer/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/tests/test_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.405692 junifer-0.0.5.dev48/junifer/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/utils/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9216 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.405692 junifer-0.0.5.dev48/junifer/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/utils/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/utils/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7754 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/junifer/utils/tests/test_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.409692 junifer-0.0.5.dev48/junifer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-04-30 12:37:41.000000 junifer-0.0.5.dev48/junifer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13943 2024-04-30 12:37:41.000000 junifer-0.0.5.dev48/junifer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 12:37:41.000000 junifer-0.0.5.dev48/junifer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-30 12:37:41.000000 junifer-0.0.5.dev48/junifer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-30 12:37:41.000000 junifer-0.0.5.dev48/junifer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-30 12:37:41.000000 junifer-0.0.5.dev48/junifer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 12:37:41.409692 junifer-0.0.5.dev48/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:37:41.405692 junifer-0.0.5.dev48/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/tools/create_aomic1000_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/tools/create_aomicpiop1_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/tools/create_aomicpiop2_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/tools/create_bids_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/tools/create_bids_example_dataset_sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/tools/create_dmcc13_benchmark_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/tools/create_hcp1200_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-30 12:37:36.000000 junifer-0.0.5.dev48/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.215333 junifer-0.0.5.dev52/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.159333 junifer-0.0.5.dev52/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.159333 junifer-0.0.5.dev52/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/.github/ISSUE_TEMPLATE/dataset-request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/.github/ISSUE_TEMPLATE/documention-request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/.github/ISSUE_TEMPLATE/marker-request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.159333 junifer-0.0.5.dev52/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/.github/workflows/ci-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/.github/workflows/docs-preview.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34354 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-05-06 10:29:41.215333 junifer-0.0.5.dev52/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/conda-env.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.163333 junifer-0.0.5.dev52/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.147333 junifer-0.0.5.dev52/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.163333 junifer-0.0.5.dev52/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.163333 junifer-0.0.5.dev52/docs/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/_static/js/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.163333 junifer-0.0.5.dev52/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/_templates/versions.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.163333 junifer-0.0.5.dev52/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/api/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/api/configs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/api/data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/api/datagrabbers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/api/datareaders.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/api/markers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/api/nilearn.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/api/onthefly.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/api/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/api/preprocessing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/api/stats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/api/storage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/api/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/api/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    25180 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/builtin.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.163333 junifer-0.0.5.dev52/docs/changes/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/changes/contributors.inc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.167333 junifer-0.0.5.dev52/docs/changes/newsfragments/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/changes/newsfragments/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/changes/newsfragments/115.doc
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/changes/newsfragments/161.feature
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/changes/newsfragments/273.feature
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/changes/newsfragments/323.feature
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/changes/newsfragments/324.bugfix
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/changes/newsfragments/330.doc
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/changes/newsfragments/331.bugfix
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/changes/newsfragments/332.bugfix
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/changes/newsfragments/336.removal
+-rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8636 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/contribution.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.167333 junifer-0.0.5.dev52/docs/extending/
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/extending/coordinates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    18384 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/extending/datagrabber.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/extending/dependencies.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/extending/extension.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/extending/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9693 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/extending/marker.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/extending/masks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/extending/parcellations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/extending/preprocessor.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/help.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.167333 junifer-0.0.5.dev52/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    62148 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/images/junifer_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/links.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/maintaining.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/redirect.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.167333 junifer-0.0.5.dev52/docs/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/sphinxext/gh_substitutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/starting.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.171333 junifer-0.0.5.dev52/docs/understanding/
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/understanding/data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/understanding/datagrabber.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/understanding/datareader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/understanding/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/understanding/marker.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/understanding/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/understanding/preprocess.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/understanding/storage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.171333 junifer-0.0.5.dev52/docs/using/
+-rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/using/codeless.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/using/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/using/masks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/using/queueing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/using/running.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    26282 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/docs/whats_new.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.171333 junifer-0.0.5.dev52/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/examples/norun_hcpfc_pearson.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/examples/norun_ukbvm_gmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/examples/run_compute_parcel_mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/examples/run_datagrabber_bids_datalad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/examples/run_ets_rss_marker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/examples/run_junifer_julearn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/examples/run_run_gmd_mean.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.171333 junifer-0.0.5.dev52/examples/yamls/
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/examples/yamls/gmd_mean.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/examples/yamls/gmd_mean_htcondor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/examples/yamls/partly_cloudy_agg_mean_tian.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/examples/yamls/ukb_gmd_mean.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/ignore_words.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.171333 junifer-0.0.5.dev52/junifer/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-06 10:29:41.000000 junifer-0.0.5.dev52/junifer/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.175333 junifer-0.0.5.dev52/junifer/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15329 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/api/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/api/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13055 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/api/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/api/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.175333 junifer-0.0.5.dev52/junifer/api/queue_context/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/api/queue_context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9561 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/api/queue_context/gnu_parallel_local_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13233 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/api/queue_context/htcondor_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/api/queue_context/queue_context_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.175333 junifer-0.0.5.dev52/junifer/api/queue_context/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/api/queue_context/tests/test_gnu_parallel_local_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8619 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/api/queue_context/tests/test_htcondor_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.175333 junifer-0.0.5.dev52/junifer/api/res/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.175333 junifer-0.0.5.dev52/junifer/api/res/afni/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/api/res/afni/3dAFNItoNIFTI
+-rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/api/res/afni/3dRSFC
+-rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/api/res/afni/3dReHo
+-rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/api/res/afni/afni
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1130 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/api/res/afni/run_afni_docker.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.175333 junifer-0.0.5.dev52/junifer/api/res/ants/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/api/res/ants/ResampleImage
+-rwxr-xr-x   0 runner    (1001) docker     (127)       57 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/api/res/ants/antsApplyTransforms
+-rwxr-xr-x   0 runner    (1001) docker     (127)       65 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/api/res/ants/antsApplyTransformsToPoints
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1119 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/api/res/ants/run_ants_docker.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.179333 junifer-0.0.5.dev52/junifer/api/res/fsl/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       46 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/api/res/fsl/applywarp
+-rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/api/res/fsl/flirt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       49 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/api/res/fsl/img2imgcoord
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1122 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/api/res/fsl/run_fsl_docker.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       49 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/api/res/fsl/std2imgcoord
+-rwxr-xr-x   0 runner    (1001) docker     (127)      517 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/api/res/run_conda.bash
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/api/res/run_conda.zsh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      507 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/api/res/run_venv.bash
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/api/res/run_venv.zsh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.179333 junifer-0.0.5.dev52/junifer/api/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.179333 junifer-0.0.5.dev52/junifer/api/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/api/tests/data/gmd_mean.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/api/tests/data/gmd_mean_htcondor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/api/tests/data/partly_cloudy_agg_mean_tian.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/api/tests/test_api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10969 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/api/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17753 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/api/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/api/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.179333 junifer-0.0.5.dev52/junifer/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.179333 junifer-0.0.5.dev52/junifer/configs/juseless/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/configs/juseless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.179333 junifer-0.0.5.dev52/junifer/configs/juseless/datagrabbers/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/configs/juseless/datagrabbers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/configs/juseless/datagrabbers/camcan_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/configs/juseless/datagrabbers/ixi_vbm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.179333 junifer-0.0.5.dev52/junifer/configs/juseless/datagrabbers/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/configs/juseless/datagrabbers/tests/test_ucla.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/configs/juseless/datagrabbers/ucla.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/configs/juseless/datagrabbers/ukb_vbm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.183333 junifer-0.0.5.dev52/junifer/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.151333 junifer-0.0.5.dev52/junifer/data/VOIs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.183333 junifer-0.0.5.dev52/junifer/data/VOIs/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/data/VOIs/meta/AutobiographicalMemory_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/data/VOIs/meta/CogAC_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/data/VOIs/meta/CogAR_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/data/VOIs/meta/DMNBuckner_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/data/VOIs/meta/Empathy_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/data/VOIs/meta/Motor_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/data/VOIs/meta/MultiTask_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/data/VOIs/meta/PhysioStress_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/data/VOIs/meta/Power2013_MNI_VOIs.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/data/VOIs/meta/Rew_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/data/VOIs/meta/Somatosensory_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/data/VOIs/meta/ToM_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/data/VOIs/meta/VigAtt_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/data/VOIs/meta/WM_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/data/VOIs/meta/eMDN_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/data/VOIs/meta/eSAD_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/data/VOIs/meta/extDMN_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12381 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/data/coordinates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.151333 junifer-0.0.5.dev52/junifer/data/masks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.187333 junifer-0.0.5.dev52/junifer/data/masks/vickery-patil/
+-rw-r--r--   0 runner    (1001) docker     (127)    88270 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    12862 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     8700 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    21427 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/data/masks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65345 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/data/parcellations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/data/template_spaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.187333 junifer-0.0.5.dev52/junifer/data/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/data/tests/test_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/data/tests/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15878 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/data/tests/test_masks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38222 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/data/tests/test_parcellations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/data/tests/test_template_spaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.187333 junifer-0.0.5.dev52/junifer/datagrabber/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/datagrabber/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.187333 junifer-0.0.5.dev52/junifer/datagrabber/aomic/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/datagrabber/aomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/datagrabber/aomic/id1000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8466 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/datagrabber/aomic/piop1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/datagrabber/aomic/piop2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.187333 junifer-0.0.5.dev52/junifer/datagrabber/aomic/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/datagrabber/aomic/tests/test_id1000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/datagrabber/aomic/tests/test_piop1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/datagrabber/aomic/tests/test_piop2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/datagrabber/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10659 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/datagrabber/datalad_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12945 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/datagrabber/dmcc13_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.187333 junifer-0.0.5.dev52/junifer/datagrabber/hcp1200/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/datagrabber/hcp1200/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/datagrabber/hcp1200/datalad_hcp1200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/datagrabber/hcp1200/hcp1200.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.187333 junifer-0.0.5.dev52/junifer/datagrabber/hcp1200/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10765 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/datagrabber/hcp1200/tests/test_hcp1200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/datagrabber/multiple.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/datagrabber/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/datagrabber/pattern_datalad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.191333 junifer-0.0.5.dev52/junifer/datagrabber/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/datagrabber/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/datagrabber/tests/test_datagrabber_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16285 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/datagrabber/tests/test_datalad_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/datagrabber/tests/test_dmcc13_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5659 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/datagrabber/tests/test_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/datagrabber/tests/test_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6483 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/datagrabber/tests/test_pattern_datalad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/datagrabber/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.191333 junifer-0.0.5.dev52/junifer/datareader/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/datareader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/datareader/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.191333 junifer-0.0.5.dev52/junifer/datareader/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/datareader/tests/test_default_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.191333 junifer-0.0.5.dev52/junifer/external/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.151333 junifer-0.0.5.dev52/junifer/external/h5io/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.191333 junifer-0.0.5.dev52/junifer/external/h5io/h5io/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-06 10:29:37.000000 junifer-0.0.5.dev52/junifer/external/h5io/h5io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28748 2024-05-06 10:29:37.000000 junifer-0.0.5.dev52/junifer/external/h5io/h5io/_h5io.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-06 10:29:37.000000 junifer-0.0.5.dev52/junifer/external/h5io/h5io/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-06 10:29:37.000000 junifer-0.0.5.dev52/junifer/external/h5io/h5io/chunked_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-06 10:29:37.000000 junifer-0.0.5.dev52/junifer/external/h5io/h5io/chunked_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.191333 junifer-0.0.5.dev52/junifer/external/nilearn/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/external/nilearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16274 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/external/nilearn/junifer_nifti_spheres_masker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.191333 junifer-0.0.5.dev52/junifer/external/nilearn/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10370 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.195333 junifer-0.0.5.dev52/junifer/markers/
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/collection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.195333 junifer-0.0.5.dev52/junifer/markers/complexity/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/complexity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/complexity/complexity_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/complexity/hurst_exponent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/complexity/multiscale_entropy_auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/complexity/perm_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/complexity/range_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/complexity/range_entropy_auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/complexity/sample_entropy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.195333 junifer-0.0.5.dev52/junifer/markers/complexity/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/complexity/tests/test_complexity_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/complexity/tests/test_hurst_exponent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/complexity/tests/test_multiscale_entropy_auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/complexity/tests/test_perm_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/complexity/tests/test_range_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/complexity/tests/test_range_entropy_auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/complexity/tests/test_sample_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/complexity/tests/test_weighted_perm_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/complexity/weighted_perm_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/ets_rss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.195333 junifer-0.0.5.dev52/junifer/markers/falff/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/falff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/falff/_afni_falff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/falff/_junifer_falff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/falff/falff_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/falff/falff_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/falff/falff_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.199333 junifer-0.0.5.dev52/junifer/markers/falff/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/falff/tests/test_falff_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/falff/tests/test_falff_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.199333 junifer-0.0.5.dev52/junifer/markers/functional_connectivity/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/functional_connectivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5179 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/functional_connectivity/functional_connectivity_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/functional_connectivity/functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/functional_connectivity/functional_connectivity_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.199333 junifer-0.0.5.dev52/junifer/markers/functional_connectivity/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8702 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/parcel_aggregation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.199333 junifer-0.0.5.dev52/junifer/markers/reho/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/reho/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/reho/_afni_reho.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/reho/_junifer_reho.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/reho/reho_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/reho/reho_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/reho/reho_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.199333 junifer-0.0.5.dev52/junifer/markers/reho/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/reho/tests/test_reho_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/reho/tests/test_reho_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8275 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/sphere_aggregation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.203333 junifer-0.0.5.dev52/junifer/markers/temporal_snr/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/temporal_snr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/temporal_snr/temporal_snr_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/temporal_snr/temporal_snr_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/temporal_snr/temporal_snr_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.203333 junifer-0.0.5.dev52/junifer/markers/temporal_snr/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/temporal_snr/tests/test_temporal_snr_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.203333 junifer-0.0.5.dev52/junifer/markers/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/tests/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/tests/test_ets_rss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/tests/test_marker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/tests/test_markers_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26531 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/tests/test_parcel_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9747 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/tests/test_sphere_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/markers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.203333 junifer-0.0.5.dev52/junifer/onthefly/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/onthefly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/onthefly/read_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.203333 junifer-0.0.5.dev52/junifer/onthefly/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/onthefly/tests/test_read_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.203333 junifer-0.0.5.dev52/junifer/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/pipeline/pipeline_step_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/pipeline/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/pipeline/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.203333 junifer-0.0.5.dev52/junifer/pipeline/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7807 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/pipeline/tests/test_pipeline_step_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/pipeline/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/pipeline/tests/test_update_meta_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/pipeline/tests/test_workdir_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/pipeline/update_meta_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8039 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/pipeline/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/pipeline/workdir_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.207333 junifer-0.0.5.dev52/junifer/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/preprocess/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.207333 junifer-0.0.5.dev52/junifer/preprocess/confounds/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/preprocess/confounds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20841 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/preprocess/confounds/fmriprep_confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.207333 junifer-0.0.5.dev52/junifer/preprocess/confounds/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    20757 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.207333 junifer-0.0.5.dev52/junifer/preprocess/smoothing/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/preprocess/smoothing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/preprocess/smoothing/_afni_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/preprocess/smoothing/_fsl_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/preprocess/smoothing/_nilearn_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/preprocess/smoothing/smoothing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.207333 junifer-0.0.5.dev52/junifer/preprocess/smoothing/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/preprocess/smoothing/tests/test_smoothing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.207333 junifer-0.0.5.dev52/junifer/preprocess/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/preprocess/tests/test_preprocess_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.207333 junifer-0.0.5.dev52/junifer/preprocess/warping/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/preprocess/warping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/preprocess/warping/_ants_warper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/preprocess/warping/_fsl_warper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/preprocess/warping/space_warper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.207333 junifer-0.0.5.dev52/junifer/preprocess/warping/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/preprocess/warping/tests/test_space_warper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.207333 junifer-0.0.5.dev52/junifer/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9654 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35631 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/storage/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/storage/pandas_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21244 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/storage/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.211333 junifer-0.0.5.dev52/junifer/storage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    29338 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/storage/tests/test_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/storage/tests/test_pandas_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28318 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/storage/tests/test_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/storage/tests/test_storage_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11854 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/storage/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/storage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.211333 junifer-0.0.5.dev52/junifer/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.211333 junifer-0.0.5.dev52/junifer/testing/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   406849 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/testing/datagrabbers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/testing/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.211333 junifer-0.0.5.dev52/junifer/testing/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/testing/tests/test_partlycloudytesting_datagrabber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/testing/tests/test_spmauditory_datagrabber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/testing/tests/test_testing_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.211333 junifer-0.0.5.dev52/junifer/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/tests/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.211333 junifer-0.0.5.dev52/junifer/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/utils/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9216 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.211333 junifer-0.0.5.dev52/junifer/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/utils/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/utils/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7754 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/junifer/utils/tests/test_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.215333 junifer-0.0.5.dev52/junifer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-05-06 10:29:41.000000 junifer-0.0.5.dev52/junifer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13981 2024-05-06 10:29:41.000000 junifer-0.0.5.dev52/junifer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 10:29:41.000000 junifer-0.0.5.dev52/junifer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-06 10:29:41.000000 junifer-0.0.5.dev52/junifer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-06 10:29:41.000000 junifer-0.0.5.dev52/junifer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-06 10:29:41.000000 junifer-0.0.5.dev52/junifer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 10:29:41.215333 junifer-0.0.5.dev52/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:29:41.215333 junifer-0.0.5.dev52/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/tools/create_aomic1000_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/tools/create_aomicpiop1_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/tools/create_aomicpiop2_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/tools/create_bids_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/tools/create_bids_example_dataset_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/tools/create_dmcc13_benchmark_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/tools/create_hcp1200_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-06 10:29:36.000000 junifer-0.0.5.dev52/tox.ini
```

### Comparing `junifer-0.0.5.dev48/.github/ISSUE_TEMPLATE/bug-report.yml` & `junifer-0.0.5.dev52/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/.github/ISSUE_TEMPLATE/dataset-request.yml` & `junifer-0.0.5.dev52/.github/ISSUE_TEMPLATE/dataset-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/.github/ISSUE_TEMPLATE/documention-request.yml` & `junifer-0.0.5.dev52/.github/ISSUE_TEMPLATE/documention-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/.github/ISSUE_TEMPLATE/feature-request.yml` & `junifer-0.0.5.dev52/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/.github/ISSUE_TEMPLATE/marker-request.yml` & `junifer-0.0.5.dev52/.github/ISSUE_TEMPLATE/marker-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/.github/workflows/ci-docs.yml` & `junifer-0.0.5.dev52/.github/workflows/ci-docs.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/.github/workflows/ci.yml` & `junifer-0.0.5.dev52/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/.github/workflows/docs-preview.yml` & `junifer-0.0.5.dev52/.github/workflows/docs-preview.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/.github/workflows/docs.yml` & `junifer-0.0.5.dev52/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/.github/workflows/lint.yml` & `junifer-0.0.5.dev52/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/.github/workflows/pypi.yml` & `junifer-0.0.5.dev52/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/.gitignore` & `junifer-0.0.5.dev52/.gitignore`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/.pre-commit-config.yaml` & `junifer-0.0.5.dev52/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/LICENSE.md` & `junifer-0.0.5.dev52/LICENSE.md`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/PKG-INFO` & `junifer-0.0.5.dev52/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junifer
-Version: 0.0.5.dev48
+Version: 0.0.5.dev52
 Summary: JUelich NeuroImaging FEature extractoR
 Author-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 Maintainer-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 License: AGPL-3.0-only
 Project-URL: Changelog, https://juaml.github.io/junifer/main/whats_new.html
 Project-URL: Documentation, https://juaml.github.io/junifer
 Project-URL: Homepage, https://juaml.github.io/junifer
```

### Comparing `junifer-0.0.5.dev48/README.md` & `junifer-0.0.5.dev52/README.md`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/codecov.yml` & `junifer-0.0.5.dev52/codecov.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/conda-env.yml` & `junifer-0.0.5.dev52/conda-env.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/docs/Makefile` & `junifer-0.0.5.dev52/docs/Makefile`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/docs/_static/css/custom.css` & `junifer-0.0.5.dev52/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/docs/_templates/versions.html` & `junifer-0.0.5.dev52/docs/_templates/versions.html`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/docs/builtin.rst` & `junifer-0.0.5.dev52/docs/builtin.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/docs/changes/contributors.inc` & `junifer-0.0.5.dev52/docs/changes/contributors.inc`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/docs/conf.py` & `junifer-0.0.5.dev52/docs/conf.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/docs/contribution.rst` & `junifer-0.0.5.dev52/docs/contribution.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/docs/extending/coordinates.rst` & `junifer-0.0.5.dev52/docs/extending/coordinates.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/docs/extending/datagrabber.rst` & `junifer-0.0.5.dev52/docs/extending/datagrabber.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/docs/extending/dependencies.rst` & `junifer-0.0.5.dev52/docs/extending/dependencies.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/docs/extending/extension.rst` & `junifer-0.0.5.dev52/docs/extending/extension.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/docs/extending/index.rst` & `junifer-0.0.5.dev52/docs/extending/index.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/docs/extending/marker.rst` & `junifer-0.0.5.dev52/docs/extending/marker.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/docs/extending/masks.rst` & `junifer-0.0.5.dev52/docs/extending/masks.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/docs/extending/parcellations.rst` & `junifer-0.0.5.dev52/docs/extending/parcellations.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/docs/extending/preprocessor.rst` & `junifer-0.0.5.dev52/docs/extending/preprocessor.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/docs/faq.rst` & `junifer-0.0.5.dev52/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/docs/help.rst` & `junifer-0.0.5.dev52/docs/help.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/docs/images/junifer_logo.png` & `junifer-0.0.5.dev52/docs/images/junifer_logo.png`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/docs/index.rst` & `junifer-0.0.5.dev52/docs/index.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/docs/installation.rst` & `junifer-0.0.5.dev52/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/docs/links.inc` & `junifer-0.0.5.dev52/docs/links.inc`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/docs/maintaining.rst` & `junifer-0.0.5.dev52/docs/maintaining.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/docs/sphinxext/gh_substitutions.py` & `junifer-0.0.5.dev52/docs/sphinxext/gh_substitutions.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/docs/starting.rst` & `junifer-0.0.5.dev52/docs/starting.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/docs/understanding/data.rst` & `junifer-0.0.5.dev52/docs/understanding/data.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/docs/understanding/datagrabber.rst` & `junifer-0.0.5.dev52/docs/understanding/datagrabber.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/docs/understanding/datareader.rst` & `junifer-0.0.5.dev52/docs/understanding/datareader.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/docs/understanding/index.rst` & `junifer-0.0.5.dev52/docs/understanding/index.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/docs/understanding/marker.rst` & `junifer-0.0.5.dev52/docs/understanding/marker.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/docs/understanding/pipeline.rst` & `junifer-0.0.5.dev52/docs/understanding/pipeline.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/docs/understanding/preprocess.rst` & `junifer-0.0.5.dev52/docs/understanding/preprocess.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/docs/understanding/storage.rst` & `junifer-0.0.5.dev52/docs/understanding/storage.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/docs/using/codeless.rst` & `junifer-0.0.5.dev52/docs/using/codeless.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/docs/using/index.rst` & `junifer-0.0.5.dev52/docs/using/index.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/docs/using/masks.rst` & `junifer-0.0.5.dev52/docs/using/masks.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/docs/using/queueing.rst` & `junifer-0.0.5.dev52/docs/using/queueing.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/docs/using/running.rst` & `junifer-0.0.5.dev52/docs/using/running.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/docs/whats_new.rst` & `junifer-0.0.5.dev52/docs/whats_new.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/examples/norun_hcpfc_pearson.py` & `junifer-0.0.5.dev52/examples/norun_hcpfc_pearson.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/examples/norun_ukbvm_gmd.py` & `junifer-0.0.5.dev52/examples/norun_ukbvm_gmd.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/examples/run_compute_parcel_mean.py` & `junifer-0.0.5.dev52/examples/run_compute_parcel_mean.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/examples/run_datagrabber_bids_datalad.py` & `junifer-0.0.5.dev52/examples/run_datagrabber_bids_datalad.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/examples/run_ets_rss_marker.py` & `junifer-0.0.5.dev52/examples/run_ets_rss_marker.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/examples/run_junifer_julearn.py` & `junifer-0.0.5.dev52/examples/run_junifer_julearn.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/examples/run_run_gmd_mean.py` & `junifer-0.0.5.dev52/examples/run_run_gmd_mean.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/examples/yamls/gmd_mean.yaml` & `junifer-0.0.5.dev52/examples/yamls/gmd_mean.yaml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/examples/yamls/ukb_gmd_mean.yaml` & `junifer-0.0.5.dev52/examples/yamls/ukb_gmd_mean.yaml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/api/cli.py` & `junifer-0.0.5.dev52/junifer/api/cli.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/api/decorators.py` & `junifer-0.0.5.dev52/junifer/api/decorators.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/api/functions.py` & `junifer-0.0.5.dev52/junifer/api/functions.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/api/parser.py` & `junifer-0.0.5.dev52/junifer/api/parser.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/api/queue_context/gnu_parallel_local_adapter.py` & `junifer-0.0.5.dev52/junifer/api/queue_context/gnu_parallel_local_adapter.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/api/queue_context/htcondor_adapter.py` & `junifer-0.0.5.dev52/junifer/api/queue_context/htcondor_adapter.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/api/queue_context/queue_context_adapter.py` & `junifer-0.0.5.dev52/junifer/api/queue_context/queue_context_adapter.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/api/queue_context/tests/test_gnu_parallel_local_adapter.py` & `junifer-0.0.5.dev52/junifer/api/queue_context/tests/test_gnu_parallel_local_adapter.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/api/queue_context/tests/test_htcondor_adapter.py` & `junifer-0.0.5.dev52/junifer/api/queue_context/tests/test_htcondor_adapter.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/api/res/afni/run_afni_docker.sh` & `junifer-0.0.5.dev52/junifer/api/res/afni/run_afni_docker.sh`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/api/res/ants/run_ants_docker.sh` & `junifer-0.0.5.dev52/junifer/api/res/ants/run_ants_docker.sh`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/api/res/fsl/run_fsl_docker.sh` & `junifer-0.0.5.dev52/junifer/api/res/fsl/run_fsl_docker.sh`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/api/res/run_conda.bash` & `junifer-0.0.5.dev52/junifer/api/res/run_conda.bash`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/api/res/run_conda.zsh` & `junifer-0.0.5.dev52/junifer/api/res/run_conda.zsh`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/api/tests/test_api_utils.py` & `junifer-0.0.5.dev52/junifer/api/tests/test_api_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/api/tests/test_cli.py` & `junifer-0.0.5.dev52/junifer/api/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/api/tests/test_functions.py` & `junifer-0.0.5.dev52/junifer/api/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/api/tests/test_parser.py` & `junifer-0.0.5.dev52/junifer/api/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/api/utils.py` & `junifer-0.0.5.dev52/junifer/api/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py` & `junifer-0.0.5.dev52/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/configs/juseless/datagrabbers/camcan_vbm.py` & `junifer-0.0.5.dev52/junifer/configs/juseless/datagrabbers/camcan_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/configs/juseless/datagrabbers/ixi_vbm.py` & `junifer-0.0.5.dev52/junifer/configs/juseless/datagrabbers/ixi_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py` & `junifer-0.0.5.dev52/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py` & `junifer-0.0.5.dev52/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py` & `junifer-0.0.5.dev52/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/configs/juseless/datagrabbers/tests/test_ucla.py` & `junifer-0.0.5.dev52/junifer/configs/juseless/datagrabbers/tests/test_ucla.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py` & `junifer-0.0.5.dev52/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/configs/juseless/datagrabbers/ucla.py` & `junifer-0.0.5.dev52/junifer/configs/juseless/datagrabbers/ucla.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/configs/juseless/datagrabbers/ukb_vbm.py` & `junifer-0.0.5.dev52/junifer/configs/juseless/datagrabbers/ukb_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/data/VOIs/meta/AutobiographicalMemory_VOIs.txt` & `junifer-0.0.5.dev52/junifer/data/VOIs/meta/AutobiographicalMemory_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt` & `junifer-0.0.5.dev52/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt` & `junifer-0.0.5.dev52/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/data/VOIs/meta/Power2013_MNI_VOIs.tsv` & `junifer-0.0.5.dev52/junifer/data/VOIs/meta/Power2013_MNI_VOIs.tsv`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/data/VOIs/meta/Rew_VOIs.txt` & `junifer-0.0.5.dev52/junifer/data/VOIs/meta/Rew_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/data/VOIs/meta/WM_VOIs.txt` & `junifer-0.0.5.dev52/junifer/data/VOIs/meta/WM_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/data/__init__.py` & `junifer-0.0.5.dev52/junifer/data/__init__.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/data/coordinates.py` & `junifer-0.0.5.dev52/junifer/data/coordinates.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz` & `junifer-0.0.5.dev52/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz` & `junifer-0.0.5.dev52/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz` & `junifer-0.0.5.dev52/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/data/masks.py` & `junifer-0.0.5.dev52/junifer/data/masks.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/data/parcellations.py` & `junifer-0.0.5.dev52/junifer/data/parcellations.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,15 +322,17 @@
                 f"-r {target_std_space_template_path.resolve()}",
                 f"-t {xfm_file_path.resolve()}",
                 f"-o {warped_parcellation_path.resolve()}",
             ]
             # Call antsApplyTransforms
             run_ext_cmd(name="antsApplyTransforms", cmd=apply_transforms_cmd)
 
-            img = nib.load(warped_parcellation_path)
+            raw_img = nib.load(warped_parcellation_path)
+            # Remove extra dimension added by ANTs
+            img = image.math_img("np.squeeze(img)", img=raw_img)
 
         # Resample parcellation to target image
         img_to_merge = image.resample_to_img(
             source_img=img,
             target_img=target_img,
             interpolation="nearest",
             copy=True,
```

### Comparing `junifer-0.0.5.dev48/junifer/data/template_spaces.py` & `junifer-0.0.5.dev52/junifer/data/template_spaces.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/data/tests/test_coordinates.py` & `junifer-0.0.5.dev52/junifer/data/tests/test_coordinates.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/data/tests/test_data_utils.py` & `junifer-0.0.5.dev52/junifer/data/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/data/tests/test_masks.py` & `junifer-0.0.5.dev52/junifer/data/tests/test_masks.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/data/tests/test_parcellations.py` & `junifer-0.0.5.dev52/junifer/data/tests/test_parcellations.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/data/tests/test_template_spaces.py` & `junifer-0.0.5.dev52/junifer/data/tests/test_template_spaces.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/data/utils.py` & `junifer-0.0.5.dev52/junifer/data/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/datagrabber/__init__.py` & `junifer-0.0.5.dev52/junifer/datagrabber/__init__.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/datagrabber/aomic/id1000.py` & `junifer-0.0.5.dev52/junifer/datagrabber/aomic/id1000.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/datagrabber/aomic/piop1.py` & `junifer-0.0.5.dev52/junifer/datagrabber/aomic/piop1.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/datagrabber/aomic/piop2.py` & `junifer-0.0.5.dev52/junifer/datagrabber/aomic/piop2.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/datagrabber/aomic/tests/test_id1000.py` & `junifer-0.0.5.dev52/junifer/datagrabber/aomic/tests/test_id1000.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/datagrabber/aomic/tests/test_piop1.py` & `junifer-0.0.5.dev52/junifer/datagrabber/aomic/tests/test_piop1.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/datagrabber/aomic/tests/test_piop2.py` & `junifer-0.0.5.dev52/junifer/datagrabber/aomic/tests/test_piop2.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/datagrabber/base.py` & `junifer-0.0.5.dev52/junifer/datagrabber/base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/datagrabber/datalad_base.py` & `junifer-0.0.5.dev52/junifer/datagrabber/datalad_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/datagrabber/dmcc13_benchmark.py` & `junifer-0.0.5.dev52/junifer/datagrabber/dmcc13_benchmark.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/datagrabber/hcp1200/datalad_hcp1200.py` & `junifer-0.0.5.dev52/junifer/datagrabber/hcp1200/datalad_hcp1200.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/datagrabber/hcp1200/hcp1200.py` & `junifer-0.0.5.dev52/junifer/datagrabber/hcp1200/hcp1200.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/datagrabber/hcp1200/tests/test_hcp1200.py` & `junifer-0.0.5.dev52/junifer/datagrabber/hcp1200/tests/test_hcp1200.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/datagrabber/multiple.py` & `junifer-0.0.5.dev52/junifer/datagrabber/multiple.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/datagrabber/pattern.py` & `junifer-0.0.5.dev52/junifer/datagrabber/pattern.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/datagrabber/pattern_datalad.py` & `junifer-0.0.5.dev52/junifer/datagrabber/pattern_datalad.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/datagrabber/tests/test_base.py` & `junifer-0.0.5.dev52/junifer/datagrabber/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/datagrabber/tests/test_datagrabber_utils.py` & `junifer-0.0.5.dev52/junifer/datagrabber/tests/test_datagrabber_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/datagrabber/tests/test_datalad_base.py` & `junifer-0.0.5.dev52/junifer/datagrabber/tests/test_datalad_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/datagrabber/tests/test_dmcc13_benchmark.py` & `junifer-0.0.5.dev52/junifer/datagrabber/tests/test_dmcc13_benchmark.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/datagrabber/tests/test_multiple.py` & `junifer-0.0.5.dev52/junifer/datagrabber/tests/test_multiple.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/datagrabber/tests/test_pattern.py` & `junifer-0.0.5.dev52/junifer/datagrabber/tests/test_pattern.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/datagrabber/tests/test_pattern_datalad.py` & `junifer-0.0.5.dev52/junifer/datagrabber/tests/test_pattern_datalad.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/datagrabber/utils.py` & `junifer-0.0.5.dev52/junifer/datagrabber/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/datareader/default.py` & `junifer-0.0.5.dev52/junifer/datareader/default.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/datareader/tests/test_default_reader.py` & `junifer-0.0.5.dev52/junifer/datareader/tests/test_default_reader.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/external/h5io/h5io/_h5io.py` & `junifer-0.0.5.dev52/junifer/external/h5io/h5io/_h5io.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/external/h5io/h5io/chunked_array.py` & `junifer-0.0.5.dev52/junifer/external/h5io/h5io/chunked_array.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/external/h5io/h5io/chunked_list.py` & `junifer-0.0.5.dev52/junifer/external/h5io/h5io/chunked_list.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/external/nilearn/junifer_nifti_spheres_masker.py` & `junifer-0.0.5.dev52/junifer/external/nilearn/junifer_nifti_spheres_masker.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py` & `junifer-0.0.5.dev52/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/__init__.py` & `junifer-0.0.5.dev52/junifer/markers/__init__.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/base.py` & `junifer-0.0.5.dev52/junifer/markers/base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/collection.py` & `junifer-0.0.5.dev52/junifer/markers/collection.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/complexity/__init__.py` & `junifer-0.0.5.dev52/junifer/markers/complexity/__init__.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/complexity/complexity_base.py` & `junifer-0.0.5.dev52/junifer/markers/complexity/complexity_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/complexity/hurst_exponent.py` & `junifer-0.0.5.dev52/junifer/markers/complexity/hurst_exponent.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/complexity/multiscale_entropy_auc.py` & `junifer-0.0.5.dev52/junifer/markers/complexity/multiscale_entropy_auc.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/complexity/perm_entropy.py` & `junifer-0.0.5.dev52/junifer/markers/complexity/perm_entropy.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/complexity/range_entropy.py` & `junifer-0.0.5.dev52/junifer/markers/complexity/range_entropy.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/complexity/range_entropy_auc.py` & `junifer-0.0.5.dev52/junifer/markers/complexity/range_entropy_auc.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/complexity/sample_entropy.py` & `junifer-0.0.5.dev52/junifer/markers/complexity/sample_entropy.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/complexity/tests/test_hurst_exponent.py` & `junifer-0.0.5.dev52/junifer/markers/complexity/tests/test_hurst_exponent.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/complexity/tests/test_multiscale_entropy_auc.py` & `junifer-0.0.5.dev52/junifer/markers/complexity/tests/test_multiscale_entropy_auc.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/complexity/tests/test_perm_entropy.py` & `junifer-0.0.5.dev52/junifer/markers/complexity/tests/test_perm_entropy.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/complexity/tests/test_range_entropy.py` & `junifer-0.0.5.dev52/junifer/markers/complexity/tests/test_range_entropy.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/complexity/tests/test_range_entropy_auc.py` & `junifer-0.0.5.dev52/junifer/markers/complexity/tests/test_range_entropy_auc.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/complexity/tests/test_sample_entropy.py` & `junifer-0.0.5.dev52/junifer/markers/complexity/tests/test_sample_entropy.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/complexity/tests/test_weighted_perm_entropy.py` & `junifer-0.0.5.dev52/junifer/markers/complexity/tests/test_weighted_perm_entropy.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/complexity/weighted_perm_entropy.py` & `junifer-0.0.5.dev52/junifer/markers/complexity/weighted_perm_entropy.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/ets_rss.py` & `junifer-0.0.5.dev52/junifer/markers/ets_rss.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/falff/_afni_falff.py` & `junifer-0.0.5.dev52/junifer/markers/falff/_afni_falff.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/falff/_junifer_falff.py` & `junifer-0.0.5.dev52/junifer/markers/falff/_junifer_falff.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/falff/falff_base.py` & `junifer-0.0.5.dev52/junifer/markers/falff/falff_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/falff/falff_parcels.py` & `junifer-0.0.5.dev52/junifer/markers/falff/falff_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/falff/falff_spheres.py` & `junifer-0.0.5.dev52/junifer/markers/falff/falff_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/falff/tests/test_falff_parcels.py` & `junifer-0.0.5.dev52/junifer/markers/falff/tests/test_falff_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/falff/tests/test_falff_spheres.py` & `junifer-0.0.5.dev52/junifer/markers/falff/tests/test_falff_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py` & `junifer-0.0.5.dev52/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py` & `junifer-0.0.5.dev52/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py` & `junifer-0.0.5.dev52/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/functional_connectivity/functional_connectivity_base.py` & `junifer-0.0.5.dev52/junifer/markers/functional_connectivity/functional_connectivity_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/functional_connectivity/functional_connectivity_parcels.py` & `junifer-0.0.5.dev52/junifer/markers/functional_connectivity/functional_connectivity_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/functional_connectivity/functional_connectivity_spheres.py` & `junifer-0.0.5.dev52/junifer/markers/functional_connectivity/functional_connectivity_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py` & `junifer-0.0.5.dev52/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py` & `junifer-0.0.5.dev52/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py` & `junifer-0.0.5.dev52/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py` & `junifer-0.0.5.dev52/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py` & `junifer-0.0.5.dev52/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py` & `junifer-0.0.5.dev52/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/parcel_aggregation.py` & `junifer-0.0.5.dev52/junifer/markers/parcel_aggregation.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/reho/_afni_reho.py` & `junifer-0.0.5.dev52/junifer/markers/reho/_afni_reho.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/reho/_junifer_reho.py` & `junifer-0.0.5.dev52/junifer/markers/reho/_junifer_reho.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/reho/reho_base.py` & `junifer-0.0.5.dev52/junifer/markers/reho/reho_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/reho/reho_parcels.py` & `junifer-0.0.5.dev52/junifer/markers/reho/reho_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/reho/reho_spheres.py` & `junifer-0.0.5.dev52/junifer/markers/reho/reho_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/reho/tests/test_reho_parcels.py` & `junifer-0.0.5.dev52/junifer/markers/reho/tests/test_reho_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/reho/tests/test_reho_spheres.py` & `junifer-0.0.5.dev52/junifer/markers/reho/tests/test_reho_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/sphere_aggregation.py` & `junifer-0.0.5.dev52/junifer/markers/sphere_aggregation.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/temporal_snr/temporal_snr_base.py` & `junifer-0.0.5.dev52/junifer/markers/temporal_snr/temporal_snr_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/temporal_snr/temporal_snr_parcels.py` & `junifer-0.0.5.dev52/junifer/markers/temporal_snr/temporal_snr_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/temporal_snr/temporal_snr_spheres.py` & `junifer-0.0.5.dev52/junifer/markers/temporal_snr/temporal_snr_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py` & `junifer-0.0.5.dev52/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py` & `junifer-0.0.5.dev52/junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/tests/test_collection.py` & `junifer-0.0.5.dev52/junifer/markers/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/tests/test_ets_rss.py` & `junifer-0.0.5.dev52/junifer/markers/tests/test_ets_rss.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/tests/test_marker_utils.py` & `junifer-0.0.5.dev52/junifer/markers/tests/test_marker_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/tests/test_markers_base.py` & `junifer-0.0.5.dev52/junifer/markers/tests/test_markers_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/tests/test_parcel_aggregation.py` & `junifer-0.0.5.dev52/junifer/markers/tests/test_parcel_aggregation.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/tests/test_sphere_aggregation.py` & `junifer-0.0.5.dev52/junifer/markers/tests/test_sphere_aggregation.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/markers/utils.py` & `junifer-0.0.5.dev52/junifer/markers/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/onthefly/read_transform.py` & `junifer-0.0.5.dev52/junifer/onthefly/read_transform.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/onthefly/tests/test_read_transform.py` & `junifer-0.0.5.dev52/junifer/onthefly/tests/test_read_transform.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/pipeline/pipeline_step_mixin.py` & `junifer-0.0.5.dev52/junifer/pipeline/pipeline_step_mixin.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/pipeline/registry.py` & `junifer-0.0.5.dev52/junifer/pipeline/registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/pipeline/singleton.py` & `junifer-0.0.5.dev52/junifer/pipeline/singleton.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/pipeline/tests/test_pipeline_step_mixin.py` & `junifer-0.0.5.dev52/junifer/pipeline/tests/test_pipeline_step_mixin.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/pipeline/tests/test_registry.py` & `junifer-0.0.5.dev52/junifer/pipeline/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/pipeline/tests/test_update_meta_mixin.py` & `junifer-0.0.5.dev52/junifer/pipeline/tests/test_update_meta_mixin.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/pipeline/tests/test_workdir_manager.py` & `junifer-0.0.5.dev52/junifer/pipeline/tests/test_workdir_manager.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/pipeline/update_meta_mixin.py` & `junifer-0.0.5.dev52/junifer/pipeline/update_meta_mixin.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/pipeline/utils.py` & `junifer-0.0.5.dev52/junifer/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/pipeline/workdir_manager.py` & `junifer-0.0.5.dev52/junifer/pipeline/workdir_manager.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/preprocess/base.py` & `junifer-0.0.5.dev52/junifer/preprocess/base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/preprocess/confounds/fmriprep_confound_remover.py` & `junifer-0.0.5.dev52/junifer/preprocess/confounds/fmriprep_confound_remover.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py` & `junifer-0.0.5.dev52/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/preprocess/smoothing/_afni_smoothing.py` & `junifer-0.0.5.dev52/junifer/preprocess/smoothing/_afni_smoothing.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/preprocess/smoothing/_fsl_smoothing.py` & `junifer-0.0.5.dev52/junifer/preprocess/smoothing/_fsl_smoothing.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/preprocess/smoothing/_nilearn_smoothing.py` & `junifer-0.0.5.dev52/junifer/preprocess/smoothing/_nilearn_smoothing.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/preprocess/smoothing/smoothing.py` & `junifer-0.0.5.dev52/junifer/preprocess/smoothing/smoothing.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/preprocess/smoothing/tests/test_smoothing.py` & `junifer-0.0.5.dev52/junifer/preprocess/smoothing/tests/test_smoothing.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/preprocess/tests/test_preprocess_base.py` & `junifer-0.0.5.dev52/junifer/preprocess/tests/test_preprocess_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/preprocess/warping/_ants_warper.py` & `junifer-0.0.5.dev52/junifer/preprocess/warping/_ants_warper.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/preprocess/warping/_fsl_warper.py` & `junifer-0.0.5.dev52/junifer/preprocess/warping/_fsl_warper.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/preprocess/warping/space_warper.py` & `junifer-0.0.5.dev52/junifer/preprocess/warping/space_warper.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/preprocess/warping/tests/test_space_warper.py` & `junifer-0.0.5.dev52/junifer/preprocess/warping/tests/test_space_warper.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/stats.py` & `junifer-0.0.5.dev52/junifer/stats.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/storage/base.py` & `junifer-0.0.5.dev52/junifer/storage/base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/storage/hdf5.py` & `junifer-0.0.5.dev52/junifer/storage/hdf5.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/storage/pandas_base.py` & `junifer-0.0.5.dev52/junifer/storage/pandas_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/storage/sqlite.py` & `junifer-0.0.5.dev52/junifer/storage/sqlite.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/storage/tests/test_hdf5.py` & `junifer-0.0.5.dev52/junifer/storage/tests/test_hdf5.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/storage/tests/test_pandas_base.py` & `junifer-0.0.5.dev52/junifer/storage/tests/test_pandas_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/storage/tests/test_sqlite.py` & `junifer-0.0.5.dev52/junifer/storage/tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/storage/tests/test_storage_base.py` & `junifer-0.0.5.dev52/junifer/storage/tests/test_storage_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/storage/tests/test_utils.py` & `junifer-0.0.5.dev52/junifer/storage/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/storage/utils.py` & `junifer-0.0.5.dev52/junifer/storage/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv` & `junifer-0.0.5.dev52/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/testing/datagrabbers.py` & `junifer-0.0.5.dev52/junifer/testing/datagrabbers.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/testing/registry.py` & `junifer-0.0.5.dev52/junifer/testing/registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py` & `junifer-0.0.5.dev52/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/testing/tests/test_partlycloudytesting_datagrabber.py` & `junifer-0.0.5.dev52/junifer/testing/tests/test_partlycloudytesting_datagrabber.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/testing/tests/test_spmauditory_datagrabber.py` & `junifer-0.0.5.dev52/junifer/testing/tests/test_spmauditory_datagrabber.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/testing/tests/test_testing_registry.py` & `junifer-0.0.5.dev52/junifer/testing/tests/test_testing_registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/testing/utils.py` & `junifer-0.0.5.dev52/junifer/testing/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/tests/test_stats.py` & `junifer-0.0.5.dev52/junifer/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/utils/helpers.py` & `junifer-0.0.5.dev52/junifer/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/utils/logging.py` & `junifer-0.0.5.dev52/junifer/utils/logging.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/utils/tests/test_fs.py` & `junifer-0.0.5.dev52/junifer/utils/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/utils/tests/test_helpers.py` & `junifer-0.0.5.dev52/junifer/utils/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer/utils/tests/test_logging.py` & `junifer-0.0.5.dev52/junifer/utils/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/junifer.egg-info/PKG-INFO` & `junifer-0.0.5.dev52/junifer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junifer
-Version: 0.0.5.dev48
+Version: 0.0.5.dev52
 Summary: JUelich NeuroImaging FEature extractoR
 Author-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 Maintainer-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 License: AGPL-3.0-only
 Project-URL: Changelog, https://juaml.github.io/junifer/main/whats_new.html
 Project-URL: Documentation, https://juaml.github.io/junifer
 Project-URL: Homepage, https://juaml.github.io/junifer
```

### Comparing `junifer-0.0.5.dev48/junifer.egg-info/SOURCES.txt` & `junifer-0.0.5.dev52/junifer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 docs/changes/newsfragments/.gitignore
 docs/changes/newsfragments/115.doc
 docs/changes/newsfragments/161.feature
 docs/changes/newsfragments/273.feature
 docs/changes/newsfragments/323.feature
 docs/changes/newsfragments/324.bugfix
 docs/changes/newsfragments/330.doc
+docs/changes/newsfragments/331.bugfix
 docs/changes/newsfragments/332.bugfix
 docs/changes/newsfragments/336.removal
 docs/extending/coordinates.rst
 docs/extending/datagrabber.rst
 docs/extending/dependencies.rst
 docs/extending/extension.rst
 docs/extending/index.rst
```

### Comparing `junifer-0.0.5.dev48/junifer.egg-info/requires.txt` & `junifer-0.0.5.dev52/junifer.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/pyproject.toml` & `junifer-0.0.5.dev52/pyproject.toml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/tools/create_aomic1000_example_dataset.py` & `junifer-0.0.5.dev52/tools/create_aomic1000_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/tools/create_aomicpiop1_example_dataset.py` & `junifer-0.0.5.dev52/tools/create_aomicpiop1_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/tools/create_aomicpiop2_example_dataset.py` & `junifer-0.0.5.dev52/tools/create_aomicpiop2_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/tools/create_bids_example_dataset.py` & `junifer-0.0.5.dev52/tools/create_bids_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/tools/create_bids_example_dataset_sessions.py` & `junifer-0.0.5.dev52/tools/create_bids_example_dataset_sessions.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/tools/create_dmcc13_benchmark_example_dataset.py` & `junifer-0.0.5.dev52/tools/create_dmcc13_benchmark_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/tools/create_hcp1200_example_dataset.py` & `junifer-0.0.5.dev52/tools/create_hcp1200_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev48/tox.ini` & `junifer-0.0.5.dev52/tox.ini`

 * *Files identical despite different names*

