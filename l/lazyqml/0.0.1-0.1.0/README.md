# Comparing `tmp/lazyqml-0.0.1.tar.gz` & `tmp/lazyqml-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazyqml-0.0.1.tar", last modified: Mon Apr 29 07:34:35 2024, max compression
+gzip compressed data, was "lazyqml-0.1.0.tar", last modified: Mon May  6 10:52:00 2024, max compression
```

## Comparing `lazyqml-0.0.1.tar` & `lazyqml-0.1.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:34:35.628805 lazyqml-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-29 07:34:25.000000 lazyqml-0.0.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:34:35.620804 lazyqml-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:34:35.624804 lazyqml-0.0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-29 07:34:25.000000 lazyqml-0.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-29 07:34:25.000000 lazyqml-0.0.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-29 07:34:25.000000 lazyqml-0.0.1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:34:35.624804 lazyqml-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-29 07:34:25.000000 lazyqml-0.0.1/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-29 07:34:25.000000 lazyqml-0.0.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-29 07:34:25.000000 lazyqml-0.0.1/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-29 07:34:25.000000 lazyqml-0.0.1/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-29 07:34:25.000000 lazyqml-0.0.1/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-29 07:34:25.000000 lazyqml-0.0.1/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-29 07:34:25.000000 lazyqml-0.0.1/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-29 07:34:25.000000 lazyqml-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-29 07:34:25.000000 lazyqml-0.0.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-29 07:34:25.000000 lazyqml-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-29 07:34:25.000000 lazyqml-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-29 07:34:35.628805 lazyqml-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-29 07:34:25.000000 lazyqml-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:34:35.624804 lazyqml-0.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-29 07:34:25.000000 lazyqml-0.0.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-29 07:34:25.000000 lazyqml-0.0.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-29 07:34:25.000000 lazyqml-0.0.1/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-04-29 07:34:25.000000 lazyqml-0.0.1/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:34:35.624804 lazyqml-0.0.1/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-29 07:34:25.000000 lazyqml-0.0.1/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-29 07:34:25.000000 lazyqml-0.0.1/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-29 07:34:25.000000 lazyqml-0.0.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-29 07:34:25.000000 lazyqml-0.0.1/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-29 07:34:25.000000 lazyqml-0.0.1/docs/lazyqml.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:34:35.624804 lazyqml-0.0.1/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-29 07:34:25.000000 lazyqml-0.0.1/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-29 07:34:25.000000 lazyqml-0.0.1/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:34:35.628805 lazyqml-0.0.1/lazyqml/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-29 07:34:25.000000 lazyqml-0.0.1/lazyqml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-29 07:34:25.000000 lazyqml-0.0.1/lazyqml/common.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-29 07:34:25.000000 lazyqml-0.0.1/lazyqml/lazyqml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:34:35.628805 lazyqml-0.0.1/lazyqml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-29 07:34:35.000000 lazyqml-0.0.1/lazyqml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-29 07:34:35.000000 lazyqml-0.0.1/lazyqml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 07:34:35.000000 lazyqml-0.0.1/lazyqml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-29 07:34:35.000000 lazyqml-0.0.1/lazyqml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-29 07:34:35.000000 lazyqml-0.0.1/lazyqml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 07:34:35.000000 lazyqml-0.0.1/lazyqml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-29 07:34:25.000000 lazyqml-0.0.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-29 07:34:25.000000 lazyqml-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-29 07:34:25.000000 lazyqml-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-29 07:34:25.000000 lazyqml-0.0.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 07:34:35.628805 lazyqml-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:34:35.628805 lazyqml-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-29 07:34:25.000000 lazyqml-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-29 07:34:25.000000 lazyqml-0.0.1/tests/test_lazyqml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:52:00.628927 lazyqml-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-06 10:51:28.000000 lazyqml-0.1.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:52:00.620927 lazyqml-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:52:00.620927 lazyqml-0.1.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-06 10:51:28.000000 lazyqml-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-06 10:51:28.000000 lazyqml-0.1.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-06 10:51:28.000000 lazyqml-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:52:00.624927 lazyqml-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-06 10:51:28.000000 lazyqml-0.1.0/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-06 10:51:28.000000 lazyqml-0.1.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-06 10:51:28.000000 lazyqml-0.1.0/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-06 10:51:28.000000 lazyqml-0.1.0/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-06 10:51:28.000000 lazyqml-0.1.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-06 10:51:28.000000 lazyqml-0.1.0/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-06 10:51:28.000000 lazyqml-0.1.0/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-06 10:51:28.000000 lazyqml-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-06 10:51:28.000000 lazyqml-0.1.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-06 10:51:28.000000 lazyqml-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-06 10:51:28.000000 lazyqml-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-06 10:52:00.628927 lazyqml-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-06 10:51:28.000000 lazyqml-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:52:00.624927 lazyqml-0.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-06 10:51:28.000000 lazyqml-0.1.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-06 10:51:28.000000 lazyqml-0.1.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-06 10:51:28.000000 lazyqml-0.1.0/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-06 10:51:28.000000 lazyqml-0.1.0/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:52:00.624927 lazyqml-0.1.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-06 10:51:28.000000 lazyqml-0.1.0/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-06 10:51:28.000000 lazyqml-0.1.0/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-06 10:51:28.000000 lazyqml-0.1.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-06 10:51:28.000000 lazyqml-0.1.0/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-06 10:51:28.000000 lazyqml-0.1.0/docs/lazyqml.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:52:00.624927 lazyqml-0.1.0/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-06 10:51:28.000000 lazyqml-0.1.0/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-06 10:51:28.000000 lazyqml-0.1.0/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:52:00.624927 lazyqml-0.1.0/lazyqml/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-06 10:51:28.000000 lazyqml-0.1.0/lazyqml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22448 2024-05-06 10:51:28.000000 lazyqml-0.1.0/lazyqml/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17507 2024-05-06 10:51:28.000000 lazyqml-0.1.0/lazyqml/supervised.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:52:00.624927 lazyqml-0.1.0/lazyqml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-06 10:52:00.000000 lazyqml-0.1.0/lazyqml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-06 10:52:00.000000 lazyqml-0.1.0/lazyqml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 10:52:00.000000 lazyqml-0.1.0/lazyqml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-06 10:52:00.000000 lazyqml-0.1.0/lazyqml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-06 10:52:00.000000 lazyqml-0.1.0/lazyqml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-06 10:52:00.000000 lazyqml-0.1.0/lazyqml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-06 10:51:28.000000 lazyqml-0.1.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-06 10:51:28.000000 lazyqml-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-06 10:51:28.000000 lazyqml-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-06 10:51:28.000000 lazyqml-0.1.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 10:52:00.628927 lazyqml-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:52:00.624927 lazyqml-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-06 10:51:28.000000 lazyqml-0.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-06 10:51:28.000000 lazyqml-0.1.0/tests/test_lazyqml.py
```

### Comparing `lazyqml-0.0.1/.github/workflows/docs-build.yml` & `lazyqml-0.1.0/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.0.1/.github/workflows/docs.yml` & `lazyqml-0.1.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.0.1/.github/workflows/installation.yml` & `lazyqml-0.1.0/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.0.1/.github/workflows/macos.yml` & `lazyqml-0.1.0/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.0.1/.github/workflows/pypi.yml` & `lazyqml-0.1.0/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.0.1/.github/workflows/ubuntu.yml` & `lazyqml-0.1.0/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.0.1/.github/workflows/windows.yml` & `lazyqml-0.1.0/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.0.1/.gitignore` & `lazyqml-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lazyqml-0.0.1/LICENSE` & `lazyqml-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lazyqml-0.0.1/PKG-INFO` & `lazyqml-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: lazyqml
-Version: 0.0.1
+Version: 0.1.0
 Summary: LazyQML benchmarking utility to test quantum machine learning models.
 Author-email: Diego García Vega <garciavdiego@uniovi.es>
 License: MIT License
 Project-URL: Homepage, https://github.com/DiegoGV-Uniovi/lazyqml
 Keywords: lazyqml
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: ==3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.rst
 Requires-Dist: absl-py==1.3.0
 Requires-Dist: appdirs==1.4.4
 Requires-Dist: autograd==1.5
 Requires-Dist: autoray==0.5.3
@@ -26,15 +26,15 @@
 Requires-Dist: contourpy==1.0.6
 Requires-Dist: cycler==0.11.0
 Requires-Dist: dm-tree==0.1.8
 Requires-Dist: fonttools==4.38.0
 Requires-Dist: future==0.18.2
 Requires-Dist: idna==3.4
 Requires-Dist: importlib_metadata==7.1.0
-Requires-Dist: jax==0.4.1
+Requires-Dist: jax==0.4.6
 Requires-Dist: jaxlib==0.4.6
 Requires-Dist: joblib==1.2.0
 Requires-Dist: kiwisolver==1.4.4
 Requires-Dist: ml-dtypes==0.4.0
 Requires-Dist: networkx==2.8.8
 Requires-Dist: ninja==1.11.1
 Requires-Dist: numpy==1.22.3
```

### Comparing `lazyqml-0.0.1/docs/contributing.md` & `lazyqml-0.1.0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `lazyqml-0.0.1/docs/installation.md` & `lazyqml-0.1.0/docs/installation.md`

 * *Files identical despite different names*

### Comparing `lazyqml-0.0.1/lazyqml.egg-info/PKG-INFO` & `lazyqml-0.1.0/lazyqml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: lazyqml
-Version: 0.0.1
+Version: 0.1.0
 Summary: LazyQML benchmarking utility to test quantum machine learning models.
 Author-email: Diego García Vega <garciavdiego@uniovi.es>
 License: MIT License
 Project-URL: Homepage, https://github.com/DiegoGV-Uniovi/lazyqml
 Keywords: lazyqml
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: ==3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.rst
 Requires-Dist: absl-py==1.3.0
 Requires-Dist: appdirs==1.4.4
 Requires-Dist: autograd==1.5
 Requires-Dist: autoray==0.5.3
@@ -26,15 +26,15 @@
 Requires-Dist: contourpy==1.0.6
 Requires-Dist: cycler==0.11.0
 Requires-Dist: dm-tree==0.1.8
 Requires-Dist: fonttools==4.38.0
 Requires-Dist: future==0.18.2
 Requires-Dist: idna==3.4
 Requires-Dist: importlib_metadata==7.1.0
-Requires-Dist: jax==0.4.1
+Requires-Dist: jax==0.4.6
 Requires-Dist: jaxlib==0.4.6
 Requires-Dist: joblib==1.2.0
 Requires-Dist: kiwisolver==1.4.4
 Requires-Dist: ml-dtypes==0.4.0
 Requires-Dist: networkx==2.8.8
 Requires-Dist: ninja==1.11.1
 Requires-Dist: numpy==1.22.3
```

### Comparing `lazyqml-0.0.1/lazyqml.egg-info/SOURCES.txt` & `lazyqml-0.1.0/lazyqml.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 docs/installation.md
 docs/lazyqml.md
 docs/usage.md
 docs/examples/intro.ipynb
 docs/overrides/main.html
 lazyqml/__init__.py
 lazyqml/common.py
-lazyqml/lazyqml.py
+lazyqml/supervised.py
 lazyqml.egg-info/PKG-INFO
 lazyqml.egg-info/SOURCES.txt
 lazyqml.egg-info/dependency_links.txt
 lazyqml.egg-info/entry_points.txt
 lazyqml.egg-info/requires.txt
 lazyqml.egg-info/top_level.txt
 tests/__init__.py
```

### Comparing `lazyqml-0.0.1/lazyqml.egg-info/requires.txt` & `lazyqml-0.1.0/lazyqml.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 contourpy==1.0.6
 cycler==0.11.0
 dm-tree==0.1.8
 fonttools==4.38.0
 future==0.18.2
 idna==3.4
 importlib_metadata==7.1.0
-jax==0.4.1
+jax==0.4.6
 jaxlib==0.4.6
 joblib==1.2.0
 kiwisolver==1.4.4
 ml-dtypes==0.4.0
 networkx==2.8.8
 ninja==1.11.1
 numpy==1.22.3
```

### Comparing `lazyqml-0.0.1/mkdocs.yml` & `lazyqml-0.1.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `lazyqml-0.0.1/pyproject.toml` & `lazyqml-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "lazyqml"
-version = "0.0.1"
+version = "0.1.0"
 dynamic = [
     "dependencies",
 ]
 description = "LazyQML benchmarking utility to test quantum machine learning models."
 readme = "README.md"
-requires-python = "==3.9"
+requires-python = ">=3.8"
 keywords = [
     "lazyqml",
 ]
 license = {text = "MIT License"}
 authors = [
   {name = "Diego García Vega", email = "garciavdiego@uniovi.es"},
 ]
@@ -44,15 +44,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.0.1"
+current_version = "0.1.0"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

### Comparing `lazyqml-0.0.1/requirements.txt` & `lazyqml-0.1.0/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 contourpy==1.0.6
 cycler==0.11.0
 dm-tree==0.1.8
 fonttools==4.38.0
 future==0.18.2
 idna==3.4
 importlib_metadata==7.1.0
-jax==0.4.1
+jax==0.4.6
 jaxlib==0.4.6
 joblib==1.2.0
 kiwisolver==1.4.4
 ml-dtypes==0.4.0
 networkx==2.8.8
 ninja==1.11.1
 numpy==1.22.3
@@ -45,7 +45,8 @@
 toml==0.10.2
 toolz==0.12.0
 typing_extensions==4.4.0
 urllib3==1.26.13
 wheel==0.41.2
 xlrd==2.0.1
 zipp==3.18.1
+
```

