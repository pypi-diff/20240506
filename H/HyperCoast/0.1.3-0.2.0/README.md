# Comparing `tmp/hypercoast-0.1.3.tar.gz` & `tmp/hypercoast-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypercoast-0.1.3.tar", last modified: Tue Apr 30 15:26:03 2024, max compression
+gzip compressed data, was "hypercoast-0.2.0.tar", last modified: Sun May  5 22:18:22 2024, max compression
```

## Comparing `hypercoast-0.1.3.tar` & `hypercoast-0.2.0.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:26:03.636089 hypercoast-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-30 15:25:53.000000 hypercoast-0.1.3/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:26:03.624090 hypercoast-0.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:26:03.628090 hypercoast-0.1.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-30 15:25:53.000000 hypercoast-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-30 15:25:53.000000 hypercoast-0.1.3/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-30 15:25:53.000000 hypercoast-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:26:03.628090 hypercoast-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-30 15:25:53.000000 hypercoast-0.1.3/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-30 15:25:53.000000 hypercoast-0.1.3/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-30 15:25:53.000000 hypercoast-0.1.3/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-30 15:25:53.000000 hypercoast-0.1.3/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-30 15:25:53.000000 hypercoast-0.1.3/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-30 15:25:53.000000 hypercoast-0.1.3/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-30 15:25:53.000000 hypercoast-0.1.3/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-30 15:25:53.000000 hypercoast-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-30 15:25:53.000000 hypercoast-0.1.3/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:26:03.636089 hypercoast-0.1.3/HyperCoast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-30 15:26:03.000000 hypercoast-0.1.3/HyperCoast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-30 15:26:03.000000 hypercoast-0.1.3/HyperCoast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:26:03.000000 hypercoast-0.1.3/HyperCoast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-30 15:26:03.000000 hypercoast-0.1.3/HyperCoast.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-30 15:26:03.000000 hypercoast-0.1.3/HyperCoast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-30 15:26:03.000000 hypercoast-0.1.3/HyperCoast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-30 15:25:53.000000 hypercoast-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-30 15:25:53.000000 hypercoast-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-30 15:26:03.636089 hypercoast-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-30 15:25:53.000000 hypercoast-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:26:03.632089 hypercoast-0.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-30 15:25:53.000000 hypercoast-0.1.3/docs/CNAME
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-30 15:25:53.000000 hypercoast-0.1.3/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 15:25:53.000000 hypercoast-0.1.3/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-30 15:25:53.000000 hypercoast-0.1.3/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-30 15:25:53.000000 hypercoast-0.1.3/docs/emit.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:26:03.632089 hypercoast-0.1.3/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-30 15:25:53.000000 hypercoast-0.1.3/docs/examples/emit.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-30 15:25:53.000000 hypercoast-0.1.3/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-30 15:25:53.000000 hypercoast-0.1.3/docs/hypercoast.md
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-30 15:25:53.000000 hypercoast-0.1.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-30 15:25:53.000000 hypercoast-0.1.3/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:26:03.632089 hypercoast-0.1.3/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-30 15:25:53.000000 hypercoast-0.1.3/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-30 15:25:53.000000 hypercoast-0.1.3/docs/pace.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-30 15:25:53.000000 hypercoast-0.1.3/docs/ui.md
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-30 15:25:53.000000 hypercoast-0.1.3/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:26:03.632089 hypercoast-0.1.3/hypercoast/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-30 15:25:53.000000 hypercoast-0.1.3/hypercoast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-30 15:25:53.000000 hypercoast-0.1.3/hypercoast/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    37765 2024-04-30 15:25:53.000000 hypercoast-0.1.3/hypercoast/emit.py
--rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-04-30 15:25:53.000000 hypercoast-0.1.3/hypercoast/hypercoast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-30 15:25:53.000000 hypercoast-0.1.3/hypercoast/pace.py
--rw-r--r--   0 runner    (1001) docker     (127)     8206 2024-04-30 15:25:53.000000 hypercoast-0.1.3/hypercoast/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-30 15:25:53.000000 hypercoast-0.1.3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-30 15:25:53.000000 hypercoast-0.1.3/pyproject-codespell.precommit-toml
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-30 15:25:53.000000 hypercoast-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-30 15:25:53.000000 hypercoast-0.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-30 15:25:53.000000 hypercoast-0.1.3/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 15:26:03.636089 hypercoast-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:26:03.636089 hypercoast-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-30 15:25:53.000000 hypercoast-0.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-30 15:25:53.000000 hypercoast-0.1.3/tests/test_hypercoast.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:18:22.763610 hypercoast-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-05 22:18:11.000000 hypercoast-0.2.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:18:22.755610 hypercoast-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:18:22.755610 hypercoast-0.2.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-05 22:18:11.000000 hypercoast-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-05 22:18:11.000000 hypercoast-0.2.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-05 22:18:11.000000 hypercoast-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:18:22.759610 hypercoast-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-05 22:18:11.000000 hypercoast-0.2.0/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-05 22:18:11.000000 hypercoast-0.2.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-05 22:18:11.000000 hypercoast-0.2.0/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-05 22:18:11.000000 hypercoast-0.2.0/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-05 22:18:11.000000 hypercoast-0.2.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-05 22:18:11.000000 hypercoast-0.2.0/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-05 22:18:11.000000 hypercoast-0.2.0/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-05 22:18:11.000000 hypercoast-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-05 22:18:11.000000 hypercoast-0.2.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:18:22.763610 hypercoast-0.2.0/HyperCoast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-05 22:18:22.000000 hypercoast-0.2.0/HyperCoast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-05 22:18:22.000000 hypercoast-0.2.0/HyperCoast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 22:18:22.000000 hypercoast-0.2.0/HyperCoast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-05 22:18:22.000000 hypercoast-0.2.0/HyperCoast.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-05 22:18:22.000000 hypercoast-0.2.0/HyperCoast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-05 22:18:22.000000 hypercoast-0.2.0/HyperCoast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-05 22:18:11.000000 hypercoast-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-05 22:18:11.000000 hypercoast-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-05 22:18:22.763610 hypercoast-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-05 22:18:11.000000 hypercoast-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:18:22.759610 hypercoast-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-05 22:18:11.000000 hypercoast-0.2.0/docs/CNAME
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-05 22:18:11.000000 hypercoast-0.2.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 22:18:11.000000 hypercoast-0.2.0/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-05 22:18:11.000000 hypercoast-0.2.0/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-05 22:18:11.000000 hypercoast-0.2.0/docs/emit.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:18:22.759610 hypercoast-0.2.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-05 22:18:11.000000 hypercoast-0.2.0/docs/examples/emit.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-05 22:18:11.000000 hypercoast-0.2.0/docs/examples/pace.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-05 22:18:11.000000 hypercoast-0.2.0/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-05 22:18:11.000000 hypercoast-0.2.0/docs/hypercoast.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-05 22:18:11.000000 hypercoast-0.2.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-05 22:18:11.000000 hypercoast-0.2.0/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:18:22.759610 hypercoast-0.2.0/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-05 22:18:11.000000 hypercoast-0.2.0/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-05 22:18:11.000000 hypercoast-0.2.0/docs/pace.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-05 22:18:11.000000 hypercoast-0.2.0/docs/ui.md
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-05 22:18:11.000000 hypercoast-0.2.0/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:18:22.763610 hypercoast-0.2.0/hypercoast/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-05 22:18:11.000000 hypercoast-0.2.0/hypercoast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-05-05 22:18:11.000000 hypercoast-0.2.0/hypercoast/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37765 2024-05-05 22:18:11.000000 hypercoast-0.2.0/hypercoast/emit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10790 2024-05-05 22:18:11.000000 hypercoast-0.2.0/hypercoast/hypercoast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-05-05 22:18:11.000000 hypercoast-0.2.0/hypercoast/pace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8206 2024-05-05 22:18:11.000000 hypercoast-0.2.0/hypercoast/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-05 22:18:11.000000 hypercoast-0.2.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-05 22:18:11.000000 hypercoast-0.2.0/pyproject-codespell.precommit-toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-05 22:18:11.000000 hypercoast-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-05 22:18:11.000000 hypercoast-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-05 22:18:11.000000 hypercoast-0.2.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 22:18:22.763610 hypercoast-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:18:22.763610 hypercoast-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-05 22:18:11.000000 hypercoast-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-05 22:18:11.000000 hypercoast-0.2.0/tests/test_hypercoast.py
```

### Comparing `hypercoast-0.1.3/.github/workflows/docs-build.yml` & `hypercoast-0.2.0/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.3/.github/workflows/docs.yml` & `hypercoast-0.2.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.3/.github/workflows/installation.yml` & `hypercoast-0.2.0/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.3/.github/workflows/macos.yml` & `hypercoast-0.2.0/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.3/.github/workflows/pypi.yml` & `hypercoast-0.2.0/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.3/.github/workflows/ubuntu.yml` & `hypercoast-0.2.0/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.3/.github/workflows/windows.yml` & `hypercoast-0.2.0/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.3/.gitignore` & `hypercoast-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.3/.pre-commit-config.yaml` & `hypercoast-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.3/HyperCoast.egg-info/PKG-INFO` & `hypercoast-0.2.0/HyperCoast.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HyperCoast
-Version: 0.1.3
+Version: 0.2.0
 Summary: A Python package for processing hyperspectral data in coastal regions
 Author-email: Qiusheng Wu <giswqs@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/opengeos/HyperCoast
 Keywords: HyperCoast
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -26,15 +26,15 @@
 Requires-Dist: numpy
 Requires-Dist: rioxarray
 Requires-Dist: s3fs
 Requires-Dist: xarray
 Provides-Extra: all
 Requires-Dist: HyperCoast[extra]; extra == "all"
 Provides-Extra: extra
-Requires-Dist: pandas; extra == "extra"
+Requires-Dist: cartopy; extra == "extra"
 
 # HyperCoast
 
 [![image](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/opengeos/HyperCoast/blob/main)
 [![image](https://img.shields.io/pypi/v/HyperCoast.svg)](https://pypi.python.org/pypi/HyperCoast)
 [![image](https://static.pepy.tech/badge/hypercoast)](https://pepy.tech/project/hypercoast)
 [![image](https://img.shields.io/conda/vn/conda-forge/hypercoast.svg)](https://anaconda.org/conda-forge/hypercoast)
```

### Comparing `hypercoast-0.1.3/HyperCoast.egg-info/SOURCES.txt` & `hypercoast-0.2.0/HyperCoast.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 docs/hypercoast.md
 docs/index.md
 docs/installation.md
 docs/pace.md
 docs/ui.md
 docs/usage.md
 docs/examples/emit.ipynb
+docs/examples/pace.ipynb
 docs/overrides/main.html
 hypercoast/__init__.py
 hypercoast/common.py
 hypercoast/emit.py
 hypercoast/hypercoast.py
 hypercoast/pace.py
 hypercoast/ui.py
```

### Comparing `hypercoast-0.1.3/LICENSE` & `hypercoast-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.3/PKG-INFO` & `hypercoast-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HyperCoast
-Version: 0.1.3
+Version: 0.2.0
 Summary: A Python package for processing hyperspectral data in coastal regions
 Author-email: Qiusheng Wu <giswqs@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/opengeos/HyperCoast
 Keywords: HyperCoast
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -26,15 +26,15 @@
 Requires-Dist: numpy
 Requires-Dist: rioxarray
 Requires-Dist: s3fs
 Requires-Dist: xarray
 Provides-Extra: all
 Requires-Dist: HyperCoast[extra]; extra == "all"
 Provides-Extra: extra
-Requires-Dist: pandas; extra == "extra"
+Requires-Dist: cartopy; extra == "extra"
 
 # HyperCoast
 
 [![image](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/opengeos/HyperCoast/blob/main)
 [![image](https://img.shields.io/pypi/v/HyperCoast.svg)](https://pypi.python.org/pypi/HyperCoast)
 [![image](https://static.pepy.tech/badge/hypercoast)](https://pepy.tech/project/hypercoast)
 [![image](https://img.shields.io/conda/vn/conda-forge/hypercoast.svg)](https://anaconda.org/conda-forge/hypercoast)
```

### Comparing `hypercoast-0.1.3/README.md` & `hypercoast-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.3/docs/contributing.md` & `hypercoast-0.2.0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.3/docs/examples/emit.ipynb` & `hypercoast-0.2.0/docs/examples/emit.ipynb`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.3/docs/index.md` & `hypercoast-0.2.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.3/docs/installation.md` & `hypercoast-0.2.0/docs/installation.md`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.3/hypercoast/common.py` & `hypercoast-0.2.0/hypercoast/common.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """The common module contains common functions and classes used by the other modules.
 """
 
 import os
+from typing import List
 
 
 def github_raw_url(url):
     """Get the raw URL for a GitHub file.
 
     Args:
         url (str): The GitHub URL.
@@ -112,7 +113,28 @@
                     if not os.path.exists(output):
                         os.makedirs(output)
                     tar_ref.extractall(output)
                 else:
                     tar_ref.extractall(os.path.dirname(output))
 
     return os.path.abspath(output)
+
+
+def netcdf_groups(filepath: str) -> List[str]:
+    """
+    Get the list of groups in a NetCDF file.
+
+    Args:
+        filepath (str): The path to the NetCDF file.
+
+    Returns:
+        list: A list of group names in the NetCDF file.
+
+    Example:
+        >>> netcdf_groups('path/to/netcdf/file')
+        ['group1', 'group2', 'group3']
+    """
+    import h5netcdf
+
+    with h5netcdf.File(filepath) as file:
+        groups = list(file)
+    return groups
```

### Comparing `hypercoast-0.1.3/hypercoast/emit.py` & `hypercoast-0.2.0/hypercoast/emit.py`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.3/hypercoast/hypercoast.py` & `hypercoast-0.2.0/hypercoast/hypercoast.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Main module."""
 
 import ipyleaflet
 import leafmap
 import xarray as xr
-from .common import download_file
+from .common import download_file, netcdf_groups
 from .emit import read_emit, plot_emit, viz_emit, emit_to_netcdf, emit_to_image
 from .pace import *
 
 
 class Map(leafmap.Map):
     """
     A class that extends leafmap.Map to provide additional functionality for hypercoast.
```

### Comparing `hypercoast-0.1.3/hypercoast/ui.py` & `hypercoast-0.2.0/hypercoast/ui.py`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.3/mkdocs.yml` & `hypercoast-0.2.0/mkdocs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -77,13 +77,14 @@
     - Usage: usage.md
     - Contributing: contributing.md
     - FAQ: faq.md
     - Changelog: changelog.md
     - Report Issues: https://github.com/opengeos/HyperCoast/issues
     - Examples:
           - examples/emit.ipynb
+          - examples/pace.ipynb
     - API Reference:
           - common module: common.md
           - emit module: emit.md
           - hypercoast module: hypercoast.md
           - pace module: pace.md
           - ui module: ui.md
```

### Comparing `hypercoast-0.1.3/pyproject.toml` & `hypercoast-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "HyperCoast"
-version = "0.1.3"
+version = "0.2.0"
 dynamic = [
     "dependencies",
 ]
 description = "A Python package for processing hyperspectral data in coastal regions"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -30,15 +30,15 @@
 
 [project.optional-dependencies]
 all = [
     "HyperCoast[extra]",
 ]
 
 extra = [
-    "pandas",
+    "cartopy",
 ]
 
 
 [tool]
 [tool.setuptools.packages.find]
 include = ["hypercoast*"]
 exclude = ["docs*"]
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.1.3"
+current_version = "0.2.0"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

