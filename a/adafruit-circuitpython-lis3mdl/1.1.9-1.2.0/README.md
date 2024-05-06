# Comparing `tmp/adafruit-circuitpython-lis3mdl-1.1.9.tar.gz` & `tmp/adafruit_circuitpython_lis3mdl-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-lis3mdl-1.1.9.tar", last modified: Tue Mar  2 23:50:52 2021, max compression
+gzip compressed data, was "adafruit_circuitpython_lis3mdl-1.2.0.tar", last modified: Mon May  6 21:41:40 2024, max compression
```

## Comparing `adafruit-circuitpython-lis3mdl-1.1.9.tar` & `adafruit_circuitpython_lis3mdl-1.2.0.tar`

### file list

```diff
@@ -1,45 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:50:52.115970 adafruit-circuitpython-lis3mdl-1.1.9/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:50:52.111970 adafruit-circuitpython-lis3mdl-1.1.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:50:52.115970 adafruit-circuitpython-lis3mdl-1.1.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     2329 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (116)     2712 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (116)      205 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)     1020 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (116)    16231 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (116)      162 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (116)     6147 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (116)     1104 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:50:52.115970 adafruit-circuitpython-lis3mdl-1.1.9/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (116)    16814 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1108 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1211 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (116)     4188 2021-03-02 23:50:52.115970 adafruit-circuitpython-lis3mdl-1.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2663 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (116)      108 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:50:52.115970 adafruit-circuitpython-lis3mdl-1.1.9/adafruit_circuitpython_lis3mdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     4188 2021-03-02 23:50:51.000000 adafruit-circuitpython-lis3mdl-1.1.9/adafruit_circuitpython_lis3mdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      898 2021-03-02 23:50:52.000000 adafruit-circuitpython-lis3mdl-1.1.9/adafruit_circuitpython_lis3mdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-03-02 23:50:51.000000 adafruit-circuitpython-lis3mdl-1.1.9/adafruit_circuitpython_lis3mdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       81 2021-03-02 23:50:51.000000 adafruit-circuitpython-lis3mdl-1.1.9/adafruit_circuitpython_lis3mdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       17 2021-03-02 23:50:51.000000 adafruit-circuitpython-lis3mdl-1.1.9/adafruit_circuitpython_lis3mdl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)    10092 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/adafruit_lis3mdl.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:50:52.115970 adafruit-circuitpython-lis3mdl-1.1.9/docs/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:50:52.115970 adafruit-circuitpython-lis3mdl-1.1.9/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (116)     4414 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (116)      105 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (116)      266 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (116)       96 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (116)     5688 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)      382 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (116)       96 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (116)      997 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)       96 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/docs/index.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:50:52.115970 adafruit-circuitpython-lis3mdl-1.1.9/examples/
--rw-r--r--   0 runner    (1001) docker     (116)      665 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/examples/lis3mdl_compass.py
--rw-r--r--   0 runner    (1001) docker     (116)      978 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/examples/lis3mdl_data_rate_test.py
--rw-r--r--   0 runner    (1001) docker     (116)      985 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/examples/lis3mdl_lsm6ds_test.py
--rw-r--r--   0 runner    (1001) docker     (116)      722 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/examples/lis3mdl_range_test.py
--rw-r--r--   0 runner    (1001) docker     (116)      458 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/examples/lis3mdl_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (116)      184 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-03-02 23:50:52.115970 adafruit-circuitpython-lis3mdl-1.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2101 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:41:40.188195 adafruit_circuitpython_lis3mdl-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:41:40.176195 adafruit_circuitpython_lis3mdl-1.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:41:40.180195 adafruit_circuitpython_lis3mdl-1.2.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-06 21:41:31.000000 adafruit_circuitpython_lis3mdl-1.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:41:40.180195 adafruit_circuitpython_lis3mdl-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-06 21:41:31.000000 adafruit_circuitpython_lis3mdl-1.2.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-06 21:41:31.000000 adafruit_circuitpython_lis3mdl-1.2.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-06 21:41:31.000000 adafruit_circuitpython_lis3mdl-1.2.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-06 21:41:31.000000 adafruit_circuitpython_lis3mdl-1.2.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-06 21:41:31.000000 adafruit_circuitpython_lis3mdl-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-06 21:41:31.000000 adafruit_circuitpython_lis3mdl-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-06 21:41:31.000000 adafruit_circuitpython_lis3mdl-1.2.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-06 21:41:31.000000 adafruit_circuitpython_lis3mdl-1.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-05-06 21:41:31.000000 adafruit_circuitpython_lis3mdl-1.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-06 21:41:31.000000 adafruit_circuitpython_lis3mdl-1.2.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:41:40.180195 adafruit_circuitpython_lis3mdl-1.2.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-05-06 21:41:31.000000 adafruit_circuitpython_lis3mdl-1.2.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-06 21:41:31.000000 adafruit_circuitpython_lis3mdl-1.2.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-06 21:41:31.000000 adafruit_circuitpython_lis3mdl-1.2.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-06 21:41:40.184195 adafruit_circuitpython_lis3mdl-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-05-06 21:41:31.000000 adafruit_circuitpython_lis3mdl-1.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-06 21:41:31.000000 adafruit_circuitpython_lis3mdl-1.2.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:41:40.184195 adafruit_circuitpython_lis3mdl-1.2.0/adafruit_circuitpython_lis3mdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-06 21:41:40.000000 adafruit_circuitpython_lis3mdl-1.2.0/adafruit_circuitpython_lis3mdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-06 21:41:40.000000 adafruit_circuitpython_lis3mdl-1.2.0/adafruit_circuitpython_lis3mdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 21:41:40.000000 adafruit_circuitpython_lis3mdl-1.2.0/adafruit_circuitpython_lis3mdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-06 21:41:40.000000 adafruit_circuitpython_lis3mdl-1.2.0/adafruit_circuitpython_lis3mdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-06 21:41:40.000000 adafruit_circuitpython_lis3mdl-1.2.0/adafruit_circuitpython_lis3mdl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10957 2024-05-06 21:41:37.000000 adafruit_circuitpython_lis3mdl-1.2.0/adafruit_lis3mdl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:41:40.184195 adafruit_circuitpython_lis3mdl-1.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:41:40.184195 adafruit_circuitpython_lis3mdl-1.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-06 21:41:31.000000 adafruit_circuitpython_lis3mdl-1.2.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-06 21:41:31.000000 adafruit_circuitpython_lis3mdl-1.2.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-06 21:41:31.000000 adafruit_circuitpython_lis3mdl-1.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-06 21:41:31.000000 adafruit_circuitpython_lis3mdl-1.2.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-05-06 21:41:31.000000 adafruit_circuitpython_lis3mdl-1.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-06 21:41:31.000000 adafruit_circuitpython_lis3mdl-1.2.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-06 21:41:31.000000 adafruit_circuitpython_lis3mdl-1.2.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-06 21:41:31.000000 adafruit_circuitpython_lis3mdl-1.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-06 21:41:31.000000 adafruit_circuitpython_lis3mdl-1.2.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-06 21:41:31.000000 adafruit_circuitpython_lis3mdl-1.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:41:40.184195 adafruit_circuitpython_lis3mdl-1.2.0/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2519 2024-05-06 21:41:37.000000 adafruit_circuitpython_lis3mdl-1.2.0/examples/lis3mdl_calibrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-06 21:41:37.000000 adafruit_circuitpython_lis3mdl-1.2.0/examples/lis3mdl_compass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-06 21:41:37.000000 adafruit_circuitpython_lis3mdl-1.2.0/examples/lis3mdl_data_rate_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-06 21:41:37.000000 adafruit_circuitpython_lis3mdl-1.2.0/examples/lis3mdl_lsm6ds_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-06 21:41:37.000000 adafruit_circuitpython_lis3mdl-1.2.0/examples/lis3mdl_range_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-06 21:41:37.000000 adafruit_circuitpython_lis3mdl-1.2.0/examples/lis3mdl_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-06 21:41:31.000000 adafruit_circuitpython_lis3mdl-1.2.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-06 21:41:37.000000 adafruit_circuitpython_lis3mdl-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-06 21:41:31.000000 adafruit_circuitpython_lis3mdl-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 21:41:40.188195 adafruit_circuitpython_lis3mdl-1.2.0/setup.cfg
```

### Comparing `adafruit-circuitpython-lis3mdl-1.1.9/.pre-commit-config.yaml` & `adafruit_circuitpython_lis3mdl-1.2.0/.pre-commit-config.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
--   repo: https://github.com/python/black
-    rev: 20.8b1
+  - repo: https://github.com/python/black
+    rev: 23.3.0
     hooks:
-    - id: black
--   repo: https://github.com/fsfe/reuse-tool
-    rev: v0.12.1
+      - id: black
+  - repo: https://github.com/fsfe/reuse-tool
+    rev: v1.1.2
     hooks:
-    - id: reuse
--   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v2.3.0
+      - id: reuse
+  - repo: https://github.com/pre-commit/pre-commit-hooks
+    rev: v4.4.0
     hooks:
-    -   id: check-yaml
-    -   id: end-of-file-fixer
-    -   id: trailing-whitespace
--   repo: https://github.com/pycqa/pylint
-    rev: pylint-2.7.1
+      - id: check-yaml
+      - id: end-of-file-fixer
+      - id: trailing-whitespace
+  - repo: https://github.com/pycqa/pylint
+    rev: v2.17.4
     hooks:
-    -   id: pylint
+      - id: pylint
         name: pylint (library code)
         types: [python]
-        exclude: "^(docs/|examples/|setup.py$)"
--   repo: local
-    hooks:
-    -   id: pylint_examples
-        name: pylint (examples code)
+        args:
+          - --disable=consider-using-f-string
+        exclude: "^(docs/|examples/|tests/|setup.py$)"
+      - id: pylint
+        name: pylint (example code)
         description: Run pylint rules on "examples/*.py" files
-        entry: /usr/bin/env bash -c
-        args: ['([[ ! -d "examples" ]] || for example in $(find . -path "./examples/*.py"); do pylint --disable=missing-docstring,invalid-name $example; done)']
-        language: system
+        types: [python]
+        files: "^examples/"
+        args:
+          - --disable=missing-docstring,invalid-name,consider-using-f-string,duplicate-code
+      - id: pylint
+        name: pylint (test code)
+        description: Run pylint rules on "tests/*.py" files
+        types: [python]
+        files: "^tests/"
+        args:
+          - --disable=missing-docstring,consider-using-f-string,duplicate-code
```

### Comparing `adafruit-circuitpython-lis3mdl-1.1.9/.pylintrc` & `adafruit_circuitpython_lis3mdl-1.2.0/.pylintrc`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,36 @@
-# SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
+# SPDX-FileCopyrightText: 2017 Scott Shawcroft, written for Adafruit Industries
 #
 # SPDX-License-Identifier: Unlicense
 
 [MASTER]
 
 # A comma-separated list of package or module names from where C extensions may
 # be loaded. Extensions are loading into the active Python interpreter and may
 # run arbitrary code
 extension-pkg-whitelist=
 
-# Add files or directories to the blacklist. They should be base names, not
+# Add files or directories to the ignore-list. They should be base names, not
 # paths.
 ignore=CVS
 
-# Add files or directories matching the regex patterns to the blacklist. The
+# Add files or directories matching the regex patterns to the ignore-list. The
 # regex matches against base names, not paths.
 ignore-patterns=
 
 # Python code to execute, usually for sys.path manipulation such as
 # pygtk.require().
 #init-hook=
 
 # Use multiple processes to speed up Pylint.
-# jobs=1
-jobs=2
+jobs=1
 
 # List of plugins (as comma separated values of python modules names) to load,
 # usually to register additional checkers.
-load-plugins=
+load-plugins=pylint.extensions.no_self_use
 
 # Pickle collected data for later comparisons.
 persistent=yes
 
 # Specify a configuration file.
 #rcfile=
 
@@ -51,16 +50,16 @@
 # option multiple times (only on the command line, not in the configuration
 # file where it should appear only once).You can also use "--disable=all" to
 # disable everything first and then reenable specific checks. For example, if
 # you want to run only the similarities checker, you can use "--disable=all
 # --enable=similarities". If you want to run only the classes checker, but have
 # no Warning level messages displayed, use"--disable=all --enable=classes
 # --disable=W"
-# disable=import-error,print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call
-disable=print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call,import-error,bad-continuation
+# disable=import-error,raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,deprecated-str-translate-call
+disable=raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,import-error,pointless-string-statement,unspecified-encoding
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
 enable=
 
@@ -222,20 +221,14 @@
 
 # Maximum number of characters on a single line.
 max-line-length=100
 
 # Maximum number of lines in a module
 max-module-lines=1000
 
-# List of optional constructs for which whitespace checking is disabled. `dict-
-# separator` is used to allow tabulation in dicts, etc.: {1  : 1,\n222: 2}.
-# `trailing-comma` allows a space between comma and closing bracket: (a, ).
-# `empty-line` allows space-only lines.
-no-space-check=trailing-comma,dict-separator
-
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
 single-line-class-stmt=no
 
 # Allow the body of an if to be on the same line as the test if there is no
 # else.
 single-line-if-stmt=no
@@ -249,86 +242,58 @@
 # Ignore docstrings when computing similarities.
 ignore-docstrings=yes
 
 # Ignore imports when computing similarities.
 ignore-imports=yes
 
 # Minimum lines number of a similarity.
-min-similarity-lines=4
+min-similarity-lines=12
 
 
 [BASIC]
 
-# Naming hint for argument names
-argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct argument names
 argument-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for attribute names
-attr-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct attribute names
 attr-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Bad variable names which should always be refused, separated by a comma
 bad-names=foo,bar,baz,toto,tutu,tata
 
-# Naming hint for class attribute names
-class-attribute-name-hint=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
-
 # Regular expression matching correct class attribute names
 class-attribute-rgx=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
 
-# Naming hint for class names
-# class-name-hint=[A-Z_][a-zA-Z0-9]+$
-class-name-hint=[A-Z_][a-zA-Z0-9_]+$
-
 # Regular expression matching correct class names
 # class-rgx=[A-Z_][a-zA-Z0-9]+$
 class-rgx=[A-Z_][a-zA-Z0-9_]+$
 
-# Naming hint for constant names
-const-name-hint=(([A-Z_][A-Z0-9_]*)|(__.*__))$
-
 # Regular expression matching correct constant names
 const-rgx=(([A-Z_][A-Z0-9_]*)|(__.*__))$
 
 # Minimum line length for functions/classes that require docstrings, shorter
 # ones are exempt.
 docstring-min-length=-1
 
-# Naming hint for function names
-function-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct function names
 function-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Good variable names which should always be accepted, separated by a comma
 # good-names=i,j,k,ex,Run,_
 good-names=r,g,b,w,i,j,k,n,x,y,z,ex,ok,Run,_
 
 # Include a hint for the correct naming format with invalid-name
 include-naming-hint=no
 
-# Naming hint for inline iteration names
-inlinevar-name-hint=[A-Za-z_][A-Za-z0-9_]*$
-
 # Regular expression matching correct inline iteration names
 inlinevar-rgx=[A-Za-z_][A-Za-z0-9_]*$
 
-# Naming hint for method names
-method-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct method names
 method-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for module names
-module-name-hint=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
-
 # Regular expression matching correct module names
 module-rgx=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
 
 # Colon-delimited sets of names that determine each other's naming style when
 # the name regexes allow several styles.
 name-group=
 
@@ -336,17 +301,14 @@
 # not require a docstring.
 no-docstring-rgx=^_
 
 # List of decorators that produce properties, such as abc.abstractproperty. Add
 # to this list to register other decorators that produce valid properties.
 property-classes=abc.abstractproperty
 
-# Naming hint for variable names
-variable-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct variable names
 variable-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 
 [IMPORTS]
 
 # Allow wildcard imports from modules that define __all__.
@@ -430,8 +392,8 @@
 min-public-methods=1
 
 
 [EXCEPTIONS]
 
 # Exceptions that will emit a warning when being caught. Defaults to
 # "Exception"
-overgeneral-exceptions=Exception
+overgeneral-exceptions=builtins.Exception
```

### Comparing `adafruit-circuitpython-lis3mdl-1.1.9/CODE_OF_CONDUCT.md` & `adafruit_circuitpython_lis3mdl-1.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lis3mdl-1.1.9/LICENSE` & `adafruit_circuitpython_lis3mdl-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lis3mdl-1.1.9/LICENSES/CC-BY-4.0.txt` & `adafruit_circuitpython_lis3mdl-1.2.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lis3mdl-1.1.9/LICENSES/MIT.txt` & `adafruit_circuitpython_lis3mdl-1.2.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lis3mdl-1.1.9/LICENSES/Unlicense.txt` & `adafruit_circuitpython_lis3mdl-1.2.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lis3mdl-1.1.9/PKG-INFO` & `adafruit_circuitpython_lis3mdl-1.2.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,106 +1,112 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-lis3mdl
-Version: 1.1.9
+Version: 1.2.0
 Summary: CircuitPython helper library for the LIS3MDL 3-axis magnetometer
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_LIS3MDL
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
+Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
-Description: Introduction
-        ============
-        
-        .. image:: https://readthedocs.org/projects/adafruit-circuitpython-lis3mdl/badge/?version=latest
-            :target: https://circuitpython.readthedocs.io/projects/lis3mdl/en/latest/
-            :alt: Documentation Status
-        
-        .. image:: https://img.shields.io/discord/327254708534116352.svg
-            :target: https://adafru.it/discord
-            :alt: Discord
-        
-        .. image:: https://github.com/adafruit/Adafruit_CircuitPython_LIS3MDL/workflows/Build%20CI/badge.svg
-            :target: https://github.com/adafruit/Adafruit_CircuitPython_LIS3MDL/actions
-            :alt: Build Status
-        
-        CircuitPython helper library for the LIS3MDL 3-axis magnetometer
-        
-        
-        Dependencies
-        =============
-        This driver depends on:
-        
-        * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
-        * `Bus Device <https://github.com/adafruit/Adafruit_CircuitPython_BusDevice>`_
-        * `Register <https://github.com/adafruit/Adafruit_CircuitPython_Register>`_
-        
-        Please ensure all dependencies are available on the CircuitPython filesystem.
-        This is easily achieved by downloading
-        `the Adafruit library and driver bundle <https://circuitpython.org/libraries>`_.
-        
-        Installing from PyPI
-        =====================
-        
-        On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
-        PyPI <https://pypi.org/project/adafruit-circuitpython-lis3mdl/>`_. To install for current user:
-        
-        .. code-block:: shell
-        
-            pip3 install adafruit-circuitpython-lis3mdl
-        
-        To install system-wide (this may be required in some cases):
-        
-        .. code-block:: shell
-        
-            sudo pip3 install adafruit-circuitpython-lis3mdl
-        
-        To install in a virtual environment in your current project:
-        
-        .. code-block:: shell
-        
-            mkdir project-name && cd project-name
-            python3 -m venv .env
-            source .env/bin/activate
-            pip3 install adafruit-circuitpython-lis3mdl
-        
-        Usage Example
-        =============
-        
-        .. code-block:: python
-        
-            import time
-            import board
-            import busio
-            import adafruit_lis3mdl
-        
-            i2c = busio.I2C(board.SCL, board.SDA)
-            sensor = adafruit_lis3mdl.LIS3MDL(i2c)
-        
-            while True:
-                mag_x, mag_y, mag_z = sensor.magnetic
-        
-                print('X:{0:10.2f}, Y:{1:10.2f}, Z:{2:10.2f} uT'.format(mag_x, mag_y, mag_z))
-                print('')
-                time.sleep(1.0)
-        
-        Contributing
-        ============
-        
-        Contributions are welcome! Please read our `Code of Conduct
-        <https://github.com/adafruit/Adafruit_CircuitPython_LIS3MDL/blob/master/CODE_OF_CONDUCT.md>`_
-        before contributing to help this project stay welcoming.
-        
-        Documentation
-        =============
-        
-        For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-        
-Keywords: adafruit blinka circuitpython micropython lis3mdl magnetometer LSM6DS33 IMU
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_LIS3MDL
+Keywords: adafruit,blinka,circuitpython,micropython,lis3mdl,magnetometer,LSM6DS33,IMU
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: Adafruit-Blinka
+Requires-Dist: adafruit-circuitpython-register
+Requires-Dist: adafruit-circuitpython-busdevice
+Provides-Extra: optional
+
+Introduction
+============
+
+.. image:: https://readthedocs.org/projects/adafruit-circuitpython-lis3mdl/badge/?version=latest
+    :target: https://docs.circuitpython.org/projects/lis3mdl/en/latest/
+    :alt: Documentation Status
+
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
+    :target: https://adafru.it/discord
+    :alt: Discord
+
+.. image:: https://github.com/adafruit/Adafruit_CircuitPython_LIS3MDL/workflows/Build%20CI/badge.svg
+    :target: https://github.com/adafruit/Adafruit_CircuitPython_LIS3MDL/actions
+    :alt: Build Status
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
+CircuitPython helper library for the LIS3MDL 3-axis magnetometer
+
+
+Dependencies
+=============
+This driver depends on:
+
+* `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
+* `Bus Device <https://github.com/adafruit/Adafruit_CircuitPython_BusDevice>`_
+* `Register <https://github.com/adafruit/Adafruit_CircuitPython_Register>`_
+
+Please ensure all dependencies are available on the CircuitPython filesystem.
+This is easily achieved by downloading
+`the Adafruit library and driver bundle <https://circuitpython.org/libraries>`_.
+
+Installing from PyPI
+=====================
+
+On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
+PyPI <https://pypi.org/project/adafruit-circuitpython-lis3mdl/>`_. To install for current user:
+
+.. code-block:: shell
+
+    pip3 install adafruit-circuitpython-lis3mdl
+
+To install system-wide (this may be required in some cases):
+
+.. code-block:: shell
+
+    sudo pip3 install adafruit-circuitpython-lis3mdl
+
+To install in a virtual environment in your current project:
+
+.. code-block:: shell
+
+    mkdir project-name && cd project-name
+    python3 -m venv .venv
+    source .venv/bin/activate
+    pip3 install adafruit-circuitpython-lis3mdl
+
+Usage Example
+=============
+
+.. code-block:: python3
+
+    import time
+    import board
+    import adafruit_lis3mdl
+
+    i2c = board.I2C()  # uses board.SCL and board.SDA
+    sensor = adafruit_lis3mdl.LIS3MDL(i2c)
+
+    while True:
+        mag_x, mag_y, mag_z = sensor.magnetic
+
+        print('X:{0:10.2f}, Y:{1:10.2f}, Z:{2:10.2f} uT'.format(mag_x, mag_y, mag_z))
+        print('')
+        time.sleep(1.0)
+
+Documentation
+=============
+
+API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/lis3mdl/en/latest/>`_.
+
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
+Contributing
+============
+
+Contributions are welcome! Please read our `Code of Conduct
+<https://github.com/adafruit/Adafruit_CircuitPython_LIS3MDL/blob/main/CODE_OF_CONDUCT.md>`_
+before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-lis3mdl-1.1.9/README.rst` & `adafruit_circuitpython_lis3mdl-1.2.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-lis3mdl/badge/?version=latest
-    :target: https://circuitpython.readthedocs.io/projects/lis3mdl/en/latest/
+    :target: https://docs.circuitpython.org/projects/lis3mdl/en/latest/
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_LIS3MDL/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_LIS3MDL/actions
     :alt: Build Status
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
 CircuitPython helper library for the LIS3MDL 3-axis magnetometer
 
 
 Dependencies
 =============
 This driver depends on:
 
@@ -45,42 +49,43 @@
     sudo pip3 install adafruit-circuitpython-lis3mdl
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-lis3mdl
 
 Usage Example
 =============
 
-.. code-block:: python
+.. code-block:: python3
 
     import time
     import board
-    import busio
     import adafruit_lis3mdl
 
-    i2c = busio.I2C(board.SCL, board.SDA)
+    i2c = board.I2C()  # uses board.SCL and board.SDA
     sensor = adafruit_lis3mdl.LIS3MDL(i2c)
 
     while True:
         mag_x, mag_y, mag_z = sensor.magnetic
 
         print('X:{0:10.2f}, Y:{1:10.2f}, Z:{2:10.2f} uT'.format(mag_x, mag_y, mag_z))
         print('')
         time.sleep(1.0)
 
+Documentation
+=============
+
+API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/lis3mdl/en/latest/>`_.
+
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
-<https://github.com/adafruit/Adafruit_CircuitPython_LIS3MDL/blob/master/CODE_OF_CONDUCT.md>`_
+<https://github.com/adafruit/Adafruit_CircuitPython_LIS3MDL/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-Documentation
-=============
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
```

### Comparing `adafruit-circuitpython-lis3mdl-1.1.9/adafruit_circuitpython_lis3mdl.egg-info/PKG-INFO` & `adafruit_circuitpython_lis3mdl-1.2.0/adafruit_circuitpython_lis3mdl.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,106 +1,112 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-lis3mdl
-Version: 1.1.9
+Version: 1.2.0
 Summary: CircuitPython helper library for the LIS3MDL 3-axis magnetometer
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_LIS3MDL
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
+Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
-Description: Introduction
-        ============
-        
-        .. image:: https://readthedocs.org/projects/adafruit-circuitpython-lis3mdl/badge/?version=latest
-            :target: https://circuitpython.readthedocs.io/projects/lis3mdl/en/latest/
-            :alt: Documentation Status
-        
-        .. image:: https://img.shields.io/discord/327254708534116352.svg
-            :target: https://adafru.it/discord
-            :alt: Discord
-        
-        .. image:: https://github.com/adafruit/Adafruit_CircuitPython_LIS3MDL/workflows/Build%20CI/badge.svg
-            :target: https://github.com/adafruit/Adafruit_CircuitPython_LIS3MDL/actions
-            :alt: Build Status
-        
-        CircuitPython helper library for the LIS3MDL 3-axis magnetometer
-        
-        
-        Dependencies
-        =============
-        This driver depends on:
-        
-        * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
-        * `Bus Device <https://github.com/adafruit/Adafruit_CircuitPython_BusDevice>`_
-        * `Register <https://github.com/adafruit/Adafruit_CircuitPython_Register>`_
-        
-        Please ensure all dependencies are available on the CircuitPython filesystem.
-        This is easily achieved by downloading
-        `the Adafruit library and driver bundle <https://circuitpython.org/libraries>`_.
-        
-        Installing from PyPI
-        =====================
-        
-        On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
-        PyPI <https://pypi.org/project/adafruit-circuitpython-lis3mdl/>`_. To install for current user:
-        
-        .. code-block:: shell
-        
-            pip3 install adafruit-circuitpython-lis3mdl
-        
-        To install system-wide (this may be required in some cases):
-        
-        .. code-block:: shell
-        
-            sudo pip3 install adafruit-circuitpython-lis3mdl
-        
-        To install in a virtual environment in your current project:
-        
-        .. code-block:: shell
-        
-            mkdir project-name && cd project-name
-            python3 -m venv .env
-            source .env/bin/activate
-            pip3 install adafruit-circuitpython-lis3mdl
-        
-        Usage Example
-        =============
-        
-        .. code-block:: python
-        
-            import time
-            import board
-            import busio
-            import adafruit_lis3mdl
-        
-            i2c = busio.I2C(board.SCL, board.SDA)
-            sensor = adafruit_lis3mdl.LIS3MDL(i2c)
-        
-            while True:
-                mag_x, mag_y, mag_z = sensor.magnetic
-        
-                print('X:{0:10.2f}, Y:{1:10.2f}, Z:{2:10.2f} uT'.format(mag_x, mag_y, mag_z))
-                print('')
-                time.sleep(1.0)
-        
-        Contributing
-        ============
-        
-        Contributions are welcome! Please read our `Code of Conduct
-        <https://github.com/adafruit/Adafruit_CircuitPython_LIS3MDL/blob/master/CODE_OF_CONDUCT.md>`_
-        before contributing to help this project stay welcoming.
-        
-        Documentation
-        =============
-        
-        For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-        
-Keywords: adafruit blinka circuitpython micropython lis3mdl magnetometer LSM6DS33 IMU
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_LIS3MDL
+Keywords: adafruit,blinka,circuitpython,micropython,lis3mdl,magnetometer,LSM6DS33,IMU
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: Adafruit-Blinka
+Requires-Dist: adafruit-circuitpython-register
+Requires-Dist: adafruit-circuitpython-busdevice
+Provides-Extra: optional
+
+Introduction
+============
+
+.. image:: https://readthedocs.org/projects/adafruit-circuitpython-lis3mdl/badge/?version=latest
+    :target: https://docs.circuitpython.org/projects/lis3mdl/en/latest/
+    :alt: Documentation Status
+
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
+    :target: https://adafru.it/discord
+    :alt: Discord
+
+.. image:: https://github.com/adafruit/Adafruit_CircuitPython_LIS3MDL/workflows/Build%20CI/badge.svg
+    :target: https://github.com/adafruit/Adafruit_CircuitPython_LIS3MDL/actions
+    :alt: Build Status
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
+CircuitPython helper library for the LIS3MDL 3-axis magnetometer
+
+
+Dependencies
+=============
+This driver depends on:
+
+* `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
+* `Bus Device <https://github.com/adafruit/Adafruit_CircuitPython_BusDevice>`_
+* `Register <https://github.com/adafruit/Adafruit_CircuitPython_Register>`_
+
+Please ensure all dependencies are available on the CircuitPython filesystem.
+This is easily achieved by downloading
+`the Adafruit library and driver bundle <https://circuitpython.org/libraries>`_.
+
+Installing from PyPI
+=====================
+
+On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
+PyPI <https://pypi.org/project/adafruit-circuitpython-lis3mdl/>`_. To install for current user:
+
+.. code-block:: shell
+
+    pip3 install adafruit-circuitpython-lis3mdl
+
+To install system-wide (this may be required in some cases):
+
+.. code-block:: shell
+
+    sudo pip3 install adafruit-circuitpython-lis3mdl
+
+To install in a virtual environment in your current project:
+
+.. code-block:: shell
+
+    mkdir project-name && cd project-name
+    python3 -m venv .venv
+    source .venv/bin/activate
+    pip3 install adafruit-circuitpython-lis3mdl
+
+Usage Example
+=============
+
+.. code-block:: python3
+
+    import time
+    import board
+    import adafruit_lis3mdl
+
+    i2c = board.I2C()  # uses board.SCL and board.SDA
+    sensor = adafruit_lis3mdl.LIS3MDL(i2c)
+
+    while True:
+        mag_x, mag_y, mag_z = sensor.magnetic
+
+        print('X:{0:10.2f}, Y:{1:10.2f}, Z:{2:10.2f} uT'.format(mag_x, mag_y, mag_z))
+        print('')
+        time.sleep(1.0)
+
+Documentation
+=============
+
+API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/lis3mdl/en/latest/>`_.
+
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
+Contributing
+============
+
+Contributions are welcome! Please read our `Code of Conduct
+<https://github.com/adafruit/Adafruit_CircuitPython_LIS3MDL/blob/main/CODE_OF_CONDUCT.md>`_
+before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-lis3mdl-1.1.9/adafruit_circuitpython_lis3mdl.egg-info/SOURCES.txt` & `adafruit_circuitpython_lis3mdl-1.2.0/adafruit_circuitpython_lis3mdl.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 .gitignore
 .pre-commit-config.yaml
 .pylintrc
-.readthedocs.yml
+.readthedocs.yaml
 CODE_OF_CONDUCT.md
 LICENSE
 README.rst
 README.rst.license
 adafruit_lis3mdl.py
+optional_requirements.txt
+pyproject.toml
 requirements.txt
-setup.py
+.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
-.github/workflows/release.yml
+.github/workflows/failure-help-text.yml
+.github/workflows/release_gh.yml
+.github/workflows/release_pypi.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 adafruit_circuitpython_lis3mdl.egg-info/PKG-INFO
 adafruit_circuitpython_lis3mdl.egg-info/SOURCES.txt
 adafruit_circuitpython_lis3mdl.egg-info/dependency_links.txt
 adafruit_circuitpython_lis3mdl.egg-info/requires.txt
@@ -22,14 +26,16 @@
 docs/api.rst
 docs/api.rst.license
 docs/conf.py
 docs/examples.rst
 docs/examples.rst.license
 docs/index.rst
 docs/index.rst.license
+docs/requirements.txt
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
+examples/lis3mdl_calibrator.py
 examples/lis3mdl_compass.py
 examples/lis3mdl_data_rate_test.py
 examples/lis3mdl_lsm6ds_test.py
 examples/lis3mdl_range_test.py
 examples/lis3mdl_simpletest.py
```

### Comparing `adafruit-circuitpython-lis3mdl-1.1.9/adafruit_lis3mdl.py` & `adafruit_circuitpython_lis3mdl-1.2.0/adafruit_lis3mdl.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,41 +16,43 @@
 **Hardware:**
 * Adafruit `Adafruit LSM6DS33 + LIS3MDL - 9 DoF IMU
 <https://www.adafruit.com/product/4485>`_ (Product ID: 4485)
 
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
-  https://github.com/adafruit/circuitpython/releases
+  https://circuitpython.org/downloads
 
 
 * Adafruit's Bus Device library: https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 * Adafruit's Register library: https://github.com/adafruit/Adafruit_CircuitPython_Register
 """
 from time import sleep
 from micropython import const
-import adafruit_bus_device.i2c_device as i2c_device
+from adafruit_bus_device import i2c_device
 from adafruit_register.i2c_struct import ROUnaryStruct, Struct
 from adafruit_register.i2c_bits import RWBits
 from adafruit_register.i2c_bit import RWBit
 
-__version__ = "0.0.0-auto.0"
-__repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_LSM6DSOX.git"
+try:
+    from typing import Iterable, Tuple, Union, Optional
+    from busio import I2C
+except ImportError:
+    pass
+
+__version__ = "1.2.0"
+__repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_LIS3MDL.git"
 
 
 _LIS3MDL_DEFAULT_ADDRESS = const(0x1C)
 
 _LIS3MDL_CHIP_ID = const(0x3D)
 
 _LIS3MDL_WHOAMI = const(0xF)
 
-
-__version__ = "0.0.0-auto.0"
-__repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_LIS3MDL.git"
-
 _LIS3MDL_WHO_AM_I = const(0x0F)  # Register that contains the part ID
 _LIS3MDL_CTRL_REG1 = const(0x20)  # Register address for control 1
 _LIS3MDL_CTRL_REG2 = const(0x21)  # Register address for control 2
 _LIS3MDL_CTRL_REG3 = const(0x22)  # Register address for control 3
 _LIS3MDL_CTRL_REG4 = const(0x23)  # Register address for control 3
 _LIS3MDL_OUT_X_L = const(0x28)  # Register address for X axis lower byte
 _LIS3MDL_INT_CFG = const(0x30)  # Interrupt configuration register
@@ -59,51 +61,49 @@
 _GAUSS_TO_UT = 100
 
 
 class CV:
     """struct helper"""
 
     @classmethod
-    def add_values(cls, value_tuples):
+    def add_values(
+        cls, value_tuples: Iterable[Tuple[str, int, Union[int, str], Optional[int]]]
+    ):
         "creates CV entires"
         cls.string = {}
         cls.lsb = {}
 
         for value_tuple in value_tuples:
             name, value, string, lsb = value_tuple
             setattr(cls, name, value)
             cls.string[value] = string
             cls.lsb[value] = lsb
 
     @classmethod
-    def is_valid(cls, value):
+    def is_valid(cls, value: int) -> bool:
         "Returns true if the given value is a member of the CV"
         return value in cls.string
 
 
 class Range(CV):
     """Options for ``accelerometer_range``"""
 
-    pass  # pylint: disable=unnecessary-pass
-
 
 Range.add_values(
     (
         ("RANGE_4_GAUSS", 0, 4, 6842),
         ("RANGE_8_GAUSS", 1, 8, 3421),
         ("RANGE_12_GAUSS", 2, 12, 2281),
         ("RANGE_16_GAUSS", 3, 16, 1711),
     )
 )
 
 
 class PerformanceMode(CV):
-    """Options for `performance_mode` """
-
-    pass  # pylint: disable=unnecessary-pass
+    """Options for `performance_mode`"""
 
 
 PerformanceMode.add_values(
     (
         ("MODE_LOW_POWER", 0, "Low Power", None),
         ("MODE_MEDIUM", 1, "Medium Performance", None),
         ("MODE_HIGH", 2, "High Performance", None),
@@ -130,16 +130,14 @@
     ``RATE_300_HZ``                300 HZ ( Sets ``PerformanceMode`` to ``MODE_HIGH``)
     ``RATE_560_HZ``                560 HZ ( Sets ``PerformanceMode`` to ``MODE_MEDIUM``)
     ``RATE_1000_HZ``               1000 HZ ( Sets ``PerformanceMode`` to ``MODE_LOW_POWER``)
     =============================  ============================================
 
     """
 
-    pass  # pylint: disable=unnecessary-pass
-
 
 # The magnetometer data rate, includes FAST_ODR bit
 Rate.add_values(
     (
         ("RATE_0_625_HZ", 0b0000, 0.625, None),
         ("RATE_1_25_HZ", 0b0010, 1.25, None),
         ("RATE_2_5_HZ", 0b0100, 2.5, None),
@@ -164,16 +162,14 @@
     =============================  ============================================
     ``OperationMode.CONTINUOUS``     Measurements are made continuously at the given `data_rate`
     ``OperationMode.SINGLE``         Setting to ``SINGLE`` takes a single measurement.
     ``OperationMode.POWER_DOWN``     Halts measurements. `magnetic` will return the last measurement
     =============================  ============================================
     """
 
-    pass  # pylint: disable=unnecessary-pass
-
 
 OperationMode.add_values(
     (
         ("CONTINUOUS", 0b00, "Continuous", None),
         ("SINGLE", 0b01, "Single", None),
         ("POWER_DOWN", 0b11, "Power Down", None),
     )
@@ -184,16 +180,42 @@
 #   LIS3MDL_SINGLEMODE = ,     ///< Single-shot conversion
 #   LIS3MDL_POWERDOWNMODE = ,  ///< Powered-down mode
 # } lis3mdl_operationmode_t;
 
 
 class LIS3MDL:
     """Driver for the LIS3MDL 3-axis magnetometer.
+
     :param ~busio.I2C i2c_bus: The I2C bus the LIS3MDL is connected to.
-    :param address: The I2C slave address of the sensor
+    :param int address: The I2C device address. Defaults to :const:`0x1C`
+
+    **Quickstart: Importing and using the device**
+
+        Here is an example of using the :class:`LIS3MDL` class.
+        First you will need to import the libraries to use the sensor
+
+        .. code-block:: python
+
+            import board
+            import adafruit_lis3mdl
+
+        Once this is done you can define your `board.I2C` object and define your sensor object
+
+        .. code-block:: python
+
+            i2c = board.I2C()
+            sensor = adafruit_lis3mdl.LIS3MDL(i2c)
+
+        Now you have access to the :attr:`magnetic` attribute
+
+        .. code-block:: python
+
+            mag_x, mag_y, mag_z = sensor.magnetic
+
+
     """
 
     _chip_id = ROUnaryStruct(_LIS3MDL_WHOAMI, "<b")
 
     _perf_mode = RWBits(2, _LIS3MDL_CTRL_REG1, 5)
     _z_perf_mode = RWBits(2, _LIS3MDL_CTRL_REG4, 2)
 
@@ -202,71 +224,78 @@
     _data_rate = RWBits(4, _LIS3MDL_CTRL_REG1, 1)
 
     _raw_mag_data = Struct(_LIS3MDL_OUT_X_L, "<hhh")
 
     _range = RWBits(2, _LIS3MDL_CTRL_REG2, 5)
     _reset = RWBit(_LIS3MDL_CTRL_REG2, 2)
 
-    def __init__(self, i2c_bus, address=_LIS3MDL_DEFAULT_ADDRESS):
-        # pylint: disable=no-member
+    def __init__(
+        self,
+        i2c_bus: I2C,
+        address: int = _LIS3MDL_DEFAULT_ADDRESS,
+        performance_mode: PerformanceMode = PerformanceMode.MODE_ULTRA,
+        data_rate: Rate = Rate.RATE_155_HZ,
+        range_: Range = Range.RANGE_4_GAUSS,
+        operation_mode: OperationMode = OperationMode.CONTINUOUS,
+    ) -> None:
+        # pylint: disable=no-member,too-many-arguments
         self.i2c_device = i2c_device.I2CDevice(i2c_bus, address)
         if self._chip_id != _LIS3MDL_CHIP_ID:
             raise RuntimeError("Failed to find LIS3MDL - check your wiring!")
 
         self.reset()
-        self.performance_mode = PerformanceMode.MODE_ULTRA
-
-        self.data_rate = Rate.RATE_155_HZ
-        self.range = Range.RANGE_4_GAUSS
-        self.operation_mode = OperationMode.CONTINUOUS
+        self.performance_mode = performance_mode
+        self.data_rate = data_rate
+        self.range = range_
+        self.operation_mode = operation_mode
 
         sleep(0.010)
 
-    def reset(self):  # pylint: disable=no-self-use
+    def reset(self) -> None:
         """Reset the sensor to the default state set by the library"""
         self._reset = True
         sleep(0.010)
 
     @property
-    def magnetic(self):
+    def magnetic(self) -> Tuple[float, float, float]:
         """The processed magnetometer sensor values.
         A 3-tuple of X, Y, Z axis values in microteslas that are signed floats.
         """
 
         raw_mag_data = self._raw_mag_data
         x = self._scale_mag_data(raw_mag_data[0])
         y = self._scale_mag_data(raw_mag_data[1])
         z = self._scale_mag_data(raw_mag_data[2])
 
         return (x, y, z)
 
-    def _scale_mag_data(self, raw_measurement):  # pylint: disable=no-self-use
+    def _scale_mag_data(self, raw_measurement: int) -> float:
         return (raw_measurement / Range.lsb[self.range]) * _GAUSS_TO_UT
 
     @property
-    def range(self):
+    def range(self) -> int:
         """The measurement range for the magnetic sensor. Must be a ``Range``"""
         return self._range
 
     @range.setter
-    def range(self, value):
+    def range(self, value: int) -> None:
         if not Range.is_valid(value):
             raise AttributeError("``range`` must be a ``Range``")
 
         self._range = value
 
         sleep(0.010)
 
     @property
-    def data_rate(self):
+    def data_rate(self) -> int:
         """The rate at which the sensor takes measurements. Must be a ``Rate``"""
         return self._data_rate
 
     @data_rate.setter
-    def data_rate(self, value):
+    def data_rate(self, value: int) -> None:
         # pylint: disable=no-member
         if value is Rate.RATE_155_HZ:
             self.performance_mode = PerformanceMode.MODE_ULTRA
         if value is Rate.RATE_300_HZ:
             self.performance_mode = PerformanceMode.MODE_HIGH
         if value is Rate.RATE_560_HZ:
             self.performance_mode = PerformanceMode.MODE_MEDIUM
@@ -274,33 +303,33 @@
             self.performance_mode = PerformanceMode.MODE_LOW_POWER
         sleep(0.010)
         if not Rate.is_valid(value):
             raise AttributeError("`data_rate` must be a `Rate`")
         self._data_rate = value
 
     @property
-    def performance_mode(self):
-        """Sets the 'performance mode' of the sensor. Must be a `PerformanceMode`.
+    def performance_mode(self) -> int:
+        """Sets the 'performance mode' of the sensor. Must be a ``PerformanceMode``.
         Note that `performance_mode` affects the available data rate and will be
         automatically changed by setting ``data_rate`` to certain values."""
 
         return self._perf_mode
 
     @performance_mode.setter
-    def performance_mode(self, value):
+    def performance_mode(self, value: int) -> None:
         if not PerformanceMode.is_valid(value):
             raise AttributeError("`performance_mode` must be a `PerformanceMode`")
         self._perf_mode = value
         self._z_perf_mode = value
 
     @property
-    def operation_mode(self):
+    def operation_mode(self) -> int:
         """The operating mode for the sensor, controlling how measurements are taken.
         Must be an `OperationMode`. See the the `OperationMode` document for additional details
         """
         return self._operation_mode
 
     @operation_mode.setter
-    def operation_mode(self, value):
+    def operation_mode(self, value: int) -> None:
         if not OperationMode.is_valid(value):
             raise AttributeError("operation mode must be a OperationMode")
         self._operation_mode = value
```

### Comparing `adafruit-circuitpython-lis3mdl-1.1.9/docs/_static/favicon.ico` & `adafruit_circuitpython_lis3mdl-1.2.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lis3mdl-1.1.9/docs/conf.py` & `adafruit_circuitpython_lis3mdl-1.2.0/docs/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,59 +2,68 @@
 
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import sys
+import datetime
 
 sys.path.insert(0, os.path.abspath(".."))
 
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.autodoc",
+    "sphinxcontrib.jquery",
     "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
     "sphinx.ext.todo",
 ]
 
 # Uncomment the below if you use native CircuitPython modules such as
 # digitalio, micropython and busio. List the modules you use. Without it, the
 # autodoc module docs will fail to generate with a warning.
 autodoc_mock_imports = ["micropython", "adafruit_bus_device", "adafruit_register"]
 
 
 intersphinx_mapping = {
-    "python": ("https://docs.python.org/3.4", None),
+    "python": ("https://docs.python.org/3", None),
     "BusDevice": (
-        "https://circuitpython.readthedocs.io/projects/busdevice/en/latest/",
+        "https://docs.circuitpython.org/projects/busdevice/en/latest/",
         None,
     ),
     "Register": (
-        "https://circuitpython.readthedocs.io/projects/register/en/latest/",
+        "https://docs.circuitpython.org/projects/register/en/latest/",
         None,
     ),
-    "CircuitPython": ("https://circuitpython.readthedocs.io/en/latest/", None),
+    "CircuitPython": ("https://docs.circuitpython.org/en/latest/", None),
 }
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "Adafruit LIS3MDL Library"
-copyright = "2020 Bryan Siepert"
+creation_year = "2020"
+current_year = str(datetime.datetime.now().year)
+year_duration = (
+    current_year
+    if current_year == creation_year
+    else creation_year + " - " + current_year
+)
+copyright = year_duration + " Bryan Siepert"
 author = "Bryan Siepert"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
@@ -63,15 +72,15 @@
 release = "1.0"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store", ".env", "CODE_OF_CONDUCT.md"]
 
 # The reST default role (used for this markup: `text`) to use for all
@@ -95,27 +104,18 @@
 napoleon_numpy_docstring = False
 
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-on_rtd = os.environ.get("READTHEDOCS", None) == "True"
+import sphinx_rtd_theme
 
-if not on_rtd:  # only import and set the theme if we're building docs locally
-    try:
-        import sphinx_rtd_theme
-
-        html_theme = "sphinx_rtd_theme"
-        html_theme_path = [sphinx_rtd_theme.get_html_theme_path(), "."]
-    except:
-        html_theme = "default"
-        html_theme_path = ["."]
-else:
-    html_theme_path = ["."]
+html_theme = "sphinx_rtd_theme"
+html_theme_path = [sphinx_rtd_theme.get_html_theme_path(), "."]
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 
 # The name of an image file (relative to this directory) to use as a favicon of
```

### Comparing `adafruit-circuitpython-lis3mdl-1.1.9/docs/index.rst` & `adafruit_circuitpython_lis3mdl-1.2.0/docs/index.rst`

 * *Files 14% similar despite different names*

```diff
@@ -29,16 +29,17 @@
 
     Adafruit `Adafruit LSM6DS33 + LIS3MDL - 9 DoF IMU <https://www.adafruit.com/product/4485>
 
 
 .. toctree::
     :caption: Other Links
 
-    Download <https://github.com/adafruit/adafruit_CircuitPython_LIS3MDL/releases/latest>
-    CircuitPython Reference Documentation <https://circuitpython.readthedocs.io>
+    Download from GitHub <https://github.com/adafruit/adafruit_CircuitPython_LIS3MDL/releases/latest>
+    Download Library Bundle <https://circuitpython.org/libraries>
+    CircuitPython Reference Documentation <https://docs.circuitpython.org>
     CircuitPython Support Forum <https://forums.adafruit.com/viewforum.php?f=60>
     Discord Chat <https://adafru.it/discord>
     Adafruit Learning System <https://learn.adafruit.com>
     Adafruit Blog <https://blog.adafruit.com>
     Adafruit Store <https://www.adafruit.com>
 
 Indices and tables
```

### Comparing `adafruit-circuitpython-lis3mdl-1.1.9/examples/lis3mdl_compass.py` & `adafruit_circuitpython_lis3mdl-1.2.0/examples/lis3mdl_compass.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 # SPDX-License-Identifier: MIT
 
 """ Display compass heading data five times per second """
 import time
 from math import atan2, degrees
 import board
-import busio
 import adafruit_lis3mdl
 
-i2c = busio.I2C(board.SCL, board.SDA)
+i2c = board.I2C()  # uses board.SCL and board.SDA
+# i2c = board.STEMMA_I2C()  # For using the built-in STEMMA QT connector on a microcontroller
 sensor = adafruit_lis3mdl.LIS3MDL(i2c)
 
 
 def vector_2_degrees(x, y):
     angle = degrees(atan2(y, x))
     if angle < 0:
         angle += 360
```

### Comparing `adafruit-circuitpython-lis3mdl-1.1.9/examples/lis3mdl_data_rate_test.py` & `adafruit_circuitpython_lis3mdl-1.2.0/examples/lis3mdl_data_rate_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 # SPDX-License-Identifier: MIT
 
 """ Test Each Data Rate """
 
 # pylint: disable=no-member
 import time
 import board
-import busio
 from adafruit_lis3mdl import LIS3MDL, Rate, PerformanceMode
 
-i2c = busio.I2C(board.SCL, board.SDA)
+i2c = board.I2C()  # uses board.SCL and board.SDA
+# i2c = board.STEMMA_I2C()  # For using the built-in STEMMA QT connector on a microcontroller
 sensor = LIS3MDL(i2c)
 
 current_rate = Rate.RATE_155_HZ
 sensor.data_rate = current_rate
 start_time = time.monotonic()
 print("data_rate is", Rate.string[sensor.data_rate], "HZ")
 print("performance_mode is", PerformanceMode.string[sensor.performance_mode])
```

### Comparing `adafruit-circuitpython-lis3mdl-1.1.9/examples/lis3mdl_range_test.py` & `adafruit_circuitpython_lis3mdl-1.2.0/examples/lis3mdl_range_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 # SPDX-License-Identifier: MIT
 
 """ Test Each range """
 # pylint: disable=no-member
 import time
 import board
-import busio
 from adafruit_lis3mdl import LIS3MDL, Range
 
-i2c = busio.I2C(board.SCL, board.SDA)
+i2c = board.I2C()  # uses board.SCL and board.SDA
+# i2c = board.STEMMA_I2C()  # For using the built-in STEMMA QT connector on a microcontroller
 sensor = LIS3MDL(i2c)
 
 while True:
-
     for mag_range in [
         Range.RANGE_4_GAUSS,
         Range.RANGE_8_GAUSS,
         Range.RANGE_12_GAUSS,
         Range.RANGE_16_GAUSS,
     ]:
         sensor.range = mag_range
```

