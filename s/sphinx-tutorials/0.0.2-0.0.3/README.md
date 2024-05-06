# Comparing `tmp/sphinx_tutorials-0.0.2.tar.gz` & `tmp/sphinx_tutorials-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_tutorials-0.0.2.tar", last modified: Mon Feb 19 22:48:37 2024, max compression
+gzip compressed data, was "sphinx_tutorials-0.0.3.tar", last modified: Mon May  6 15:33:36 2024, max compression
```

## Comparing `sphinx_tutorials-0.0.2.tar` & `sphinx_tutorials-0.0.3.tar`

### file list

```diff
@@ -1,74 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 22:48:36.994433 sphinx_tutorials-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 22:48:36.986433 sphinx_tutorials-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 22:48:36.990433 sphinx_tutorials-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/.github/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5627 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-02-19 22:48:36.994433 sphinx_tutorials-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 22:48:36.990433 sphinx_tutorials-0.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 22:48:36.990433 sphinx_tutorials-0.0.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/docs/_static/extra.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 22:48:36.990433 sphinx_tutorials-0.0.2/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/docs/_templates/base.html
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/docs/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 22:48:36.990433 sphinx_tutorials-0.0.2/docs/basic-usage/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/docs/basic-usage/basic-usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 22:48:36.990433 sphinx_tutorials-0.0.2/docs/basic-usage/include_folder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/docs/basic-usage/include_folder/example_script.rst
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/docs/basic-usage/include_this.rst
--rw-r--r--   0 runner    (1001) docker     (127)    16491 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 22:48:36.994433 sphinx_tutorials-0.0.2/docs/development/
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/docs/development/documentation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/docs/development/formatting.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/docs/development/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/docs/development/unit-tests.rst
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/docs/genindex.rst
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/docs/getting-started.rst
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 22:48:36.994433 sphinx_tutorials-0.0.2/docs/logo/
--rw-r--r--   0 runner    (1001) docker     (127)    60623 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/docs/logo/favicon-white.png
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/docs/logo/home-icon-white.svg
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 22:48:36.994433 sphinx_tutorials-0.0.2/docs/release-notes/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/docs/release-notes/v0.0.md
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/docs/release-notes/versioning.rst
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 22:48:36.994433 sphinx_tutorials-0.0.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 22:48:36.994433 sphinx_tutorials-0.0.2/examples/_skip_folder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/examples/_skip_folder/example_script.py
--rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/examples/_skip_this.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 22:48:36.994433 sphinx_tutorials-0.0.2/examples/include_folder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/examples/include_folder/example_script.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/examples/include_this.py
--rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 22:48:36.994433 sphinx_tutorials-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 22:48:36.990433 sphinx_tutorials-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 22:48:36.994433 sphinx_tutorials-0.0.2/src/sphinx_tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/src/sphinx_tutorials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-19 22:48:36.000000 sphinx_tutorials-0.0.2/src/sphinx_tutorials/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/src/sphinx_tutorials/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 22:48:36.994433 sphinx_tutorials-0.0.2/src/sphinx_tutorials/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/src/sphinx_tutorials/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/src/sphinx_tutorials/utils/conversion_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/src/sphinx_tutorials/utils/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 22:48:36.994433 sphinx_tutorials-0.0.2/src/sphinx_tutorials.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-02-19 22:48:36.000000 sphinx_tutorials-0.0.2/src/sphinx_tutorials.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-02-19 22:48:36.000000 sphinx_tutorials-0.0.2/src/sphinx_tutorials.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 22:48:36.000000 sphinx_tutorials-0.0.2/src/sphinx_tutorials.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-19 22:48:36.000000 sphinx_tutorials-0.0.2/src/sphinx_tutorials.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-19 22:48:36.000000 sphinx_tutorials-0.0.2/src/sphinx_tutorials.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-19 22:48:36.000000 sphinx_tutorials-0.0.2/src/sphinx_tutorials.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 22:48:36.994433 sphinx_tutorials-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-19 22:48:19.000000 sphinx_tutorials-0.0.2/tests/test_sphinx_tutorials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:36.488855 sphinx_tutorials-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:36.468855 sphinx_tutorials-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:36.476855 sphinx_tutorials-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5627 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-06 15:33:36.488855 sphinx_tutorials-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:36.476855 sphinx_tutorials-0.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/docs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:36.476855 sphinx_tutorials-0.0.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/docs/_static/st-api.css
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/docs/_static/st-api.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/docs/_static/st-base.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8977 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/docs/_static/st-highlight-copy_code.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/docs/_static/st-highlight.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/docs/_static/st-highlight.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/docs/_static/st-notebooks.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/docs/_static/st-notebooks.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:36.476855 sphinx_tutorials-0.0.3/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/docs/_templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)    18166 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:36.480855 sphinx_tutorials-0.0.3/docs/logo/
+-rw-r--r--   0 runner    (1001) docker     (127)    60623 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/docs/logo/favicon-white.png
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/docs/logo/home-icon-white.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   266651 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/docs/logo/logo-sphinx-tutorials-sphinx.png
+-rw-r--r--   0 runner    (1001) docker     (127)   286032 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/docs/logo/logo-sphinx-tutorials-sphinx2.png
+-rw-r--r--   0 runner    (1001) docker     (127)   830845 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/docs/logo/logo-sphinx-tutorials.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:36.480855 sphinx_tutorials-0.0.3/docs/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/docs/pages/_tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/docs/pages/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:36.484855 sphinx_tutorials-0.0.3/docs/pages/development/
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/docs/pages/development/documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/docs/pages/development/formatting.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/docs/pages/development/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/docs/pages/development/unit-tests.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/docs/pages/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:36.484855 sphinx_tutorials-0.0.3/docs/pages/release-notes/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/docs/pages/release-notes/v0.0.md
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/docs/pages/release-notes/versioning.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:36.484855 sphinx_tutorials-0.0.3/docs/pages/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:36.484855 sphinx_tutorials-0.0.3/docs/pages/tutorials/included/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/docs/pages/tutorials/included/gets_included.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/docs/pages/tutorials/included.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/docs/pages/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 15:33:36.488855 sphinx_tutorials-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:36.472855 sphinx_tutorials-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:36.484855 sphinx_tutorials-0.0.3/src/sphinx_tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/src/sphinx_tutorials/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:36.472855 sphinx_tutorials-0.0.3/src/sphinx_tutorials/_docs_files/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:36.488855 sphinx_tutorials-0.0.3/src/sphinx_tutorials/_docs_files/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/src/sphinx_tutorials/_docs_files/_static/st-api.css
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/src/sphinx_tutorials/_docs_files/_static/st-api.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/src/sphinx_tutorials/_docs_files/_static/st-base.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8977 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/src/sphinx_tutorials/_docs_files/_static/st-highlight-copy_code.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/src/sphinx_tutorials/_docs_files/_static/st-highlight.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/src/sphinx_tutorials/_docs_files/_static/st-highlight.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/src/sphinx_tutorials/_docs_files/_static/st-notebooks.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/src/sphinx_tutorials/_docs_files/_static/st-notebooks.js
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-06 15:33:36.000000 sphinx_tutorials-0.0.3/src/sphinx_tutorials/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/src/sphinx_tutorials/sphinx_tutorials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:36.488855 sphinx_tutorials-0.0.3/src/sphinx_tutorials/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/src/sphinx_tutorials/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/src/sphinx_tutorials/utils/_converter_OLD.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7162 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/src/sphinx_tutorials/utils/copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/src/sphinx_tutorials/utils/py_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/src/sphinx_tutorials/utils/toc_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:36.488855 sphinx_tutorials-0.0.3/src/sphinx_tutorials.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-06 15:33:36.000000 sphinx_tutorials-0.0.3/src/sphinx_tutorials.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-06 15:33:36.000000 sphinx_tutorials-0.0.3/src/sphinx_tutorials.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 15:33:36.000000 sphinx_tutorials-0.0.3/src/sphinx_tutorials.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-06 15:33:36.000000 sphinx_tutorials-0.0.3/src/sphinx_tutorials.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-06 15:33:36.000000 sphinx_tutorials-0.0.3/src/sphinx_tutorials.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-06 15:33:36.000000 sphinx_tutorials-0.0.3/src/sphinx_tutorials.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:36.488855 sphinx_tutorials-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/tests/test_sphinx_tutorials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:36.488855 sphinx_tutorials-0.0.3/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:36.488855 sphinx_tutorials-0.0.3/tutorials/_skip/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/tutorials/_skip/gets_skipped.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/tutorials/_skip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:36.488855 sphinx_tutorials-0.0.3/tutorials/included/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/tutorials/included/gets_included.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-06 15:33:23.000000 sphinx_tutorials-0.0.3/tutorials/included.py
```

### Comparing `sphinx_tutorials-0.0.2/.github/workflows/build.yaml` & `sphinx_tutorials-0.0.3/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `sphinx_tutorials-0.0.2/.github/workflows/docs.yaml` & `sphinx_tutorials-0.0.3/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `sphinx_tutorials-0.0.2/.github/workflows/lint.yaml` & `sphinx_tutorials-0.0.3/.github/workflows/lint.yaml`

 * *Files identical despite different names*

### Comparing `sphinx_tutorials-0.0.2/.github/workflows/release.yaml` & `sphinx_tutorials-0.0.3/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `sphinx_tutorials-0.0.2/.github/workflows/test.yaml` & `sphinx_tutorials-0.0.3/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `sphinx_tutorials-0.0.2/.gitignore` & `sphinx_tutorials-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `sphinx_tutorials-0.0.2/LICENSE` & `sphinx_tutorials-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_tutorials-0.0.2/PKG-INFO` & `sphinx_tutorials-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx_tutorials
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tools for docs in Python
 Author-email: Bernardo Dionisi <bernardo.dionisi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bernardodionisi/sphinx_tutorials
 Project-URL: Source, https://github.com/bernardodionisi/sphinx_tutorials
 Project-URL: Issues, https://github.com/bernardodionisi/sphinx_tutorials/issues
 Project-URL: Documentation, https://bernardodionisi.github.io/sphinx_tutorials/latest/
@@ -18,16 +18,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: click
-Requires-Dist: polars
-Requires-Dist: matplotlib
+Requires-Dist: sphinx<7.3
+Requires-Dist: sphinx-immaterial==0.11.11
+Requires-Dist: myst-parser==0.18.1
+Requires-Dist: sphinx-design==0.5.0
+Requires-Dist: sphinx-last-updated-by-git==0.3.6
+Requires-Dist: sphinx-math-dollar==1.2.1
+Requires-Dist: ipykernel==6.26.0
+Requires-Dist: myst-nb==0.17.2
+Requires-Dist: pickleshare==0.7.5
 Requires-Dist: typing_extensions>=4.0.0
 Provides-Extra: dev
 
 # `sphinx_tutorials`
-
-functionality coming soon !
```

### Comparing `sphinx_tutorials-0.0.2/docs/conf.py` & `sphinx_tutorials-0.0.3/docs/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,64 +18,82 @@
 sys.path.insert(0, os.path.abspath("."))
 sys.path.insert(0, os.path.abspath(".."))
 
 # Need to build docs with Python 3.8 or higher for proper typing annotations, including from __future__ import annotations
 assert sys.version_info.major == 3 and sys.version_info.minor >= 8
 
 # Assign a build variable to the builtin module that inerts the @set_module decorator. This is done because set_module
-# confuses Sphinx when parsing overloaded functions. When not building the documentation, the @set_module("sphinx_tutorials")
+# confuses Sphinx when parsing overloaded functions. When not building the documentation, the @set_module("sphinx-tutorials")
 # decorator works as intended.
 import builtins
 
 setattr(builtins, "__sphinx_build__", True)
 
 import sphinx
 
+from pathlib import Path
 import sphinx_tutorials
 
+# import sphinx_autosummary_accessors
+
 # -- Project information -----------------------------------------------------
 
-project = "sphinx_tutorials"
-copyright = "2023, Bernardo Dionisi"
+project = "sphinx-tutorials"
+copyright = "2022-2023, Bernardo Dionisi"
 author = "Bernardo Dionisi"
 version = sphinx_tutorials.__version__
 
 # -- General configuration ---------------------------------------------------
 
+
+sphinx_tutorials.generate(
+    docs_path=Path(__file__).parent.absolute(),
+    tutorials_source_path=Path(__file__).parent.parent.absolute() / "tutorials",
+    tutorials_dest_path=Path(__file__).parent.absolute() / "pages",
+    style=True,
+    overwrite_style=True,
+    overwrite_tutorials=True,
+    include_suffixes=[".ipynb", ".py"],
+    exclude_prefixes=[".", "_"]
+)
+
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named "sphinx.ext.*") or your custom
 # ones.
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.napoleon",
     "sphinx.ext.mathjax",
     "sphinx.ext.intersphinx",
     # ---
-    # "sphinx_copybutton",
 
     "sphinx_last_updated_by_git",
     "sphinx_immaterial",
     "sphinx_immaterial.apidoc.python.apigen",
     "sphinx_math_dollar",
-    "myst_parser",
+
     "sphinx_design",
+    # "sphinx_autosummary_accessors",
+
+    "myst_nb",  # for notebooks
+    # "myst_parser", # Write source in markdown, not rst. a dependency of myst_nb
 
     "IPython.sphinxext.ipython_console_highlighting",
     "IPython.sphinxext.ipython_directive",
-
-    # "sphinx_tutorials.ipython_with_reprs",
 ]
 
+jupyter_execute_notebooks = "off"
+
 # # --- exclude In [x]: and Out[x]: when copying ---
 # # Configuration for sphinx_copybutton
 # copybutton_prompt_text = r"^In \[\d+\]:.*?|Out\[\d+\]:.*?$"
 # copybutton_prompt_is_regexp = True
 # ------------------------------------------------
-
 # Add any paths that contain templates here, relative to this directory.
+# templates_path = ["_templates", sphinx_autosummary_accessors.templates_path]
 templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 source_suffix = [".rst", ".md", ".ipynb"]
 
 # Tell sphinx that ReadTheDocs will create an index.rst file as the main file,
@@ -100,59 +118,72 @@
 # a list of builtin themes.
 #
 html_theme = "sphinx_immaterial"
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
+
+# ----------------------------------------------------------------------
+
 html_static_path = ["_static"]
 
-html_css_files = [
-    "extra.css",
-]
+html_js_files = [str(file.name) for file in Path("_static").glob("*.js")]
+html_css_files = [str(file.name) for file in Path("_static").glob("*.css")]
+
+html_css_files.extend([
+    # # is built in sphinx-immaterial but star not showing properly
+    "https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css",
+    # "https://cdn.jsdelivr.net/npm/bootstrap-icons@1.7.2/font/bootstrap-icons.css"
+])
+
+# ----------------------------------------------------------------------
 
 # Define a custom inline Python syntax highlighting literal
 rst_prolog = """
 .. role:: python(code)
    :language: python
    :class: highlight
 """
 
 # Sets the default role of `content` to :python:`content`, which uses the custom Python syntax highlighting inline literal
 default_role = "python"
 
-html_title = "sphinx_tutorials"
-# html_favicon = "../logo/sphinx_tutorials-favicon-color.png"
-# html_logo = "../logo/sphinx_tutorials-favicon-white.png"
-
-html_logo = "logo/favicon-white.png"
+html_title = "sphinx-tutorials"
+# html_favicon = "../logo/sphinx-tutorials-favicon-color.png"
+# html_logo = "../logo/sphinx-tutorials-favicon-white.png"
+
+# html_logo = "logo/favicon-white.png"
+html_favicon = "logo/logo-sphinx-tutorials-sphinx.png"
+html_logo = "logo/logo-sphinx-tutorials-sphinx.png"
 
 # Sphinx Immaterial theme options
 html_theme_options = {
     "icon": {
         "repo": "fontawesome/brands/github",
     },
-    "site_url": "https://sphinx_tutorials.readthedocs.io/",  # todo: <---- no read the docs?
-    "repo_url": "https://github.com/bernardodionisi/sphinx_tutorials",
-    "repo_name": "bernardodionisi/sphinx_tutorials",
+    "site_url": "https://sphinx-tutorials.readthedocs.io/",  # todo: <---- no read the docs?
+    "repo_url": "https://github.com/bernardodionisi/sphinx-tutorials",
+    "repo_name": "bernardodionisi/sphinx-tutorials",
     "social": [
         {
             "icon": "fontawesome/brands/github",
-            "link": "https://github.com/bernardodionisi/sphinx_tutorials",
+            "link": "https://github.com/bernardodionisi/sphinx-tutorials",
         },
         {
             "icon": "fontawesome/brands/python",
-            "link": "https://pypi.org/project/sphinx_tutorials/",
+            "link": "https://pypi.org/project/sphinx-tutorials/",
         },
     ],
     "edit_uri": "",
     "globaltoc_collapse": False,
     "features": [
         # "navigation.expand",
         "navigation.tabs",
+        "navigation.tabs.sticky",
         # "toc.integrate",
         # "navigation.sections",
         # "navigation.instant",
         # "header.autohide",
         "navigation.top",
         "navigation.tracking",
         "toc.follow",
@@ -174,51 +205,54 @@
             "scheme": "slate",
             "toggle": {
                 "icon": "material/weather-sunny",
                 "name": "Switch to light mode",
             },
         },
     ],
+
     "analytics": {
         "provider": "google",
         "property": "G-4FW9NCNFZH",
     },
+
     "version_dropdown": True,
     "version_json": "../versions.json",
 }
 
 html_last_updated_fmt = ""
 html_use_index = True
 html_domain_indices = True
 
 # -- Extension configuration -------------------------------------------------
 
 # Create hyperlinks to other documentation
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3", None),
-    "polars": ("https://pola-rs.github.io/polars/py-polars/html", None),
+    "polars": ("https://docs.pola.rs/py-polars/html", None),
 }
 
 autodoc_default_options = {
     "imported-members": True,
     "members": True,
     # "special-members": True,
     # "inherited-members": "ndarray",
     # "member-order": "groupwise",
 }
 autodoc_typehints = "signature"
 autodoc_typehints_description_target = "documented"
 autodoc_typehints_format = "short"
 
 autodoc_type_aliases = {
+    # "": "",
     "pl.DataFrame": "polars.DataFrame",
     "pl.LazyFrame": "polars.LazyFrame",
 }
 
-ipython_execlines = ["import sphinx_tutorials"]
+ipython_execlines = ["import sphinx-tutorials"]
 
 myst_enable_extensions = ["dollarmath"]
 
 mathjax_config = {
     "tex2jax": {
         "inlineMath": [["\\(", "\\)"]],
         "displayMath": [["\\[", "\\]"]],
@@ -248,32 +282,37 @@
     (r"method:.*\.[A-Z][A-Za-z,_]*", "Constructors"),
     (r"method:.*\.__[A-Za-z,_]*__", "Special methods"),
     (r"method:.*\.__(init|new)__", "Constructors"),
     (r"method:.*\.__(str|repr)__", "String representation"),
     ("property:.*", "Properties"),
     (r".*:.*\.info_[a-z,_]*", "Metadata"),
     (r".*:.*\.to_[a-z,_]*", "Export"),
+    (r".*:.*\.set_[a-z,_]*", "Config"),
     # (r".*:.*\.is_[a-z,_]*", "Attributes"),
 ]
 python_apigen_default_order = [
     ("class:.*", 10),
     ("data:.*", 11),
     ("function:.*", 12),
     ("classmethod:.*", 40),
+    ("property:.*", 45),
     ("method:.*", 50),
     (r"method:.*\.[A-Z][A-Za-z,_]*", 20),
     (r"method:.*\.__[A-Za-z,_]*__", 28),
     (r"method:.*\.__(init|new)__", 20),
     (r"method:.*\.__(str|repr)__", 30),
-    ("property:.*", 60),
     (r".*:.*\.info_[a-z,_]*", 70),
     (r".*:.*\.to_[a-z,_]*", 80),
+    (r".*:.*\.set_[a-z,_]*", 40),
+
     # (r".*:.*\.is_[a-z,_]*", 70),
 ]
-python_apigen_order_tiebreaker = "alphabetical"
+# python_apigen_order_tiebreaker = "alphabetical"
+python_apigen_order_tiebreaker = "definition_order"
+
 python_apigen_case_insensitive_filesystem = False
 python_apigen_show_base_classes = True
 
 # Python domain directive configuration
 python_type_aliases = autodoc_type_aliases
 python_module_names_to_strip_from_xrefs = ["collections.abc"]
 
@@ -296,14 +335,22 @@
         "color": (95, 132, 142),
         "title": "Code Example",
         "icon": "material/code-tags",
         "override": True,
     },
 
     {
+        "name": "optional-dependencies",
+        "color": (54, 69, 79),
+        "title": "Optional Dependencies",
+        "icon": "octicons/download-16",
+        "override": True,
+    },
+
+    {
         "name": "sources-description",
         "color": (54, 69, 79),
         "title": "Sources Information (click to expand)",
         "icon": "material/database",
         "override": True,
     },
 
@@ -343,22 +390,39 @@
     "__len__",
     "__eq__",
 ]
 
 
 def autodoc_skip_member(app, what, name, obj, skip, options):
     """
-    Instruct autodoc to skip members that are inherited from np.ndarray.
+    Instruct autodoc to skip members
     """
+
     if skip:
         # Continue skipping things Sphinx already wants to skip
         return skip
 
+    namespaces = [
+        "PanelAggsMeta",
+        "PanelAggsList",
+        "InfoList",
+        "Summary",
+    ]
+    if name in "__init__" and obj.__qualname__ in [
+        f"{i}.__init__" for i in namespaces
+    ]:
+        return True
+
     if name == "__init__":
         return False
+
+    # if name in SPECIAL_MEMBERS:
+    #     # Don't skip members in "special-members"
+    #     return False
+
     # elif hasattr(obj, "__objclass__"):
     #     # This is a NumPy method, don't include docs
     #     return True
     # elif getattr(obj, "__qualname__", None) in ["FunctionMixin.dot", "Array.astype"]:
     #     # NumPy methods that were overridden, don't include docs
     #     return True
     # elif (
@@ -370,18 +434,14 @@
     #         # Specifically allow these methods to be documented
     #         return False
     #     else:
     #         # This is a NumPy method that was overridden in one of our ndarray subclasses. Also don't include
     #         # these docs.
     #         return True
 
-    if name in SPECIAL_MEMBERS:
-        # Don't skip members in "special-members"
-        return False
-
     if name[0] == "_":
         # For some reason we need to tell Sphinx to hide private members
         return True
 
     return skip
 
 
@@ -409,53 +469,53 @@
 # def classproperty(obj):
 #     ret = classmethod(obj)
 #     ret.__doc__ = obj.__doc__
 #     return ret
 # 
 # 
 # ArrayMeta_properties = [
-#     member for member in dir(sphinx_tutorials.Array) if inspect.isdatadescriptor(getattr(type(sphinx_tutorials.Array), member, None))
+#     member for member in dir(galois.Array) if inspect.isdatadescriptor(getattr(type(galois.Array), member, None))
 # ]
 # for p in ArrayMeta_properties:
 #     # Fetch the class properties from the private metaclasses
-#     ArrayMeta_property = getattr(sphinx_tutorials._domains._meta.ArrayMeta, p)
+#     ArrayMeta_property = getattr(galois._domains._meta.ArrayMeta, p)
 # 
 #     # Temporarily delete the class properties from the private metaclasses
-#     delattr(sphinx_tutorials._domains._meta.ArrayMeta, p)
+#     delattr(galois._domains._meta.ArrayMeta, p)
 # 
 #     # Add a Python 3.9 style class property to the public class
-#     setattr(sphinx_tutorials.Array, p, classproperty(ArrayMeta_property))
+#     setattr(galois.Array, p, classproperty(ArrayMeta_property))
 # 
 #     # Add back the class properties to the private metaclasses
-#     setattr(sphinx_tutorials._domains._meta.ArrayMeta, p, ArrayMeta_property)
+#     setattr(galois._domains._meta.ArrayMeta, p, ArrayMeta_property)
 # 
 # 
 # FieldArrayMeta_properties = [
 #     member
-#     for member in dir(sphinx_tutorials.FieldArray)
-#     if inspect.isdatadescriptor(getattr(type(sphinx_tutorials.FieldArray), member, None))
+#     for member in dir(galois.FieldArray)
+#     if inspect.isdatadescriptor(getattr(type(galois.FieldArray), member, None))
 # ]
 # for p in FieldArrayMeta_properties:
 #     # Fetch the class properties from the private metaclasses
 #     if p in ArrayMeta_properties:
-#         ArrayMeta_property = getattr(sphinx_tutorials._domains._meta.ArrayMeta, p)
-#     FieldArrayMeta_property = getattr(sphinx_tutorials._fields._meta.FieldArrayMeta, p)
+#         ArrayMeta_property = getattr(galois._domains._meta.ArrayMeta, p)
+#     FieldArrayMeta_property = getattr(galois._fields._meta.FieldArrayMeta, p)
 # 
 #     # Temporarily delete the class properties from the private metaclasses
 #     if p in ArrayMeta_properties:
-#         delattr(sphinx_tutorials._domains._meta.ArrayMeta, p)
-#     delattr(sphinx_tutorials._fields._meta.FieldArrayMeta, p)
+#         delattr(galois._domains._meta.ArrayMeta, p)
+#     delattr(galois._fields._meta.FieldArrayMeta, p)
 # 
 #     # Add a Python 3.9 style class property to the public class
-#     setattr(sphinx_tutorials.FieldArray, p, classproperty(FieldArrayMeta_property))
+#     setattr(galois.FieldArray, p, classproperty(FieldArrayMeta_property))
 # 
 #     # Add back the class properties to the private metaclasses
 #     if p in ArrayMeta_properties:
-#         setattr(sphinx_tutorials._domains._meta.ArrayMeta, p, ArrayMeta_property)
-#     setattr(sphinx_tutorials._fields._meta.FieldArrayMeta, p, FieldArrayMeta_property)
+#         setattr(galois._domains._meta.ArrayMeta, p, ArrayMeta_property)
+#     setattr(galois._fields._meta.FieldArrayMeta, p, FieldArrayMeta_property)
 
 
 def autodoc_process_signature(app, what, name, obj, options, signature, return_annotation):
     signature = modify_type_hints(signature)
     return_annotation = modify_type_hints(return_annotation)
     return signature, return_annotation
```

### Comparing `sphinx_tutorials-0.0.2/docs/development/documentation.rst` & `sphinx_tutorials-0.0.3/docs/pages/development/documentation.rst`

 * *Files identical despite different names*

### Comparing `sphinx_tutorials-0.0.2/docs/development/formatting.rst` & `sphinx_tutorials-0.0.3/docs/pages/development/formatting.rst`

 * *Files identical despite different names*

### Comparing `sphinx_tutorials-0.0.2/docs/development/installation.rst` & `sphinx_tutorials-0.0.3/docs/pages/development/installation.rst`

 * *Files identical despite different names*

### Comparing `sphinx_tutorials-0.0.2/docs/development/unit-tests.rst` & `sphinx_tutorials-0.0.3/docs/pages/development/unit-tests.rst`

 * *Files identical despite different names*

### Comparing `sphinx_tutorials-0.0.2/docs/getting-started.rst` & `sphinx_tutorials-0.0.3/docs/pages/installation.rst`

 * *Files identical despite different names*

### Comparing `sphinx_tutorials-0.0.2/docs/logo/favicon-white.png` & `sphinx_tutorials-0.0.3/docs/logo/favicon-white.png`

 * *Files identical despite different names*

### Comparing `sphinx_tutorials-0.0.2/docs/logo/home-icon-white.svg` & `sphinx_tutorials-0.0.3/docs/logo/home-icon-white.svg`

 * *Files identical despite different names*

### Comparing `sphinx_tutorials-0.0.2/examples/_skip_this.py` & `sphinx_tutorials-0.0.3/tutorials/_skip.py`

 * *Files identical despite different names*

### Comparing `sphinx_tutorials-0.0.2/pyproject.toml` & `sphinx_tutorials-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -21,17 +21,23 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
 ]
 requires-python = ">=3.9"
 dependencies = [
-    "click",
-    "polars",
-    "matplotlib",
+    "sphinx < 7.3",
+    "sphinx-immaterial == 0.11.11",
+    "myst-parser == 0.18.1",
+    "sphinx-design  == 0.5.0",
+    "sphinx-last-updated-by-git == 0.3.6",
+    "sphinx-math-dollar == 1.2.1",
+    "ipykernel == 6.26.0",
+    "myst-nb == 0.17.2",
+    "pickleshare == 0.7.5",
     "typing_extensions >= 4.0.0", # v4.0.0 needed for: Self (Python 3.11+) and Literal (Python 3.8+)
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
 ]
```

### Comparing `sphinx_tutorials-0.0.2/src/sphinx_tutorials/utils/converter.py` & `sphinx_tutorials-0.0.3/src/sphinx_tutorials/utils/_converter_OLD.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from __future__ import annotations
 
 from pathlib import Path
 
-from sphinx_tutorials.utils.conversion_rules import parse_py_and_write_rst
+from sphinx_tutorials.utils.py_rules import py_to_rst
 
 
 def generate_rst(
         origin_path: Path,
         target_path: Path,
-        force_overwrite: bool = False
+        force_overwrite: bool = False,
+        pkg_name: str = None,
 ) -> None:
     _convert_py_files(
         origin_path=origin_path,
         target_path=target_path,
         force_overwrite=force_overwrite
     )
 
-    _create_basic_usage_rst(target_path)
+    _create_basic_usage_rst(target_path, pkg_name=pkg_name)
 
 
 def _convert_py_files(
         origin_path: Path,
         target_path: Path,
         force_overwrite: bool = False
 ) -> None:
@@ -42,15 +43,15 @@
     )
 
     if existing_rst_files and not force_overwrite:
         raise FileExistsError("\n\t" + "\n\t".join(map(str, existing_rst_files)))
 
     for f in py_files:
         rst_file = target_path / f.relative_to(origin_path).with_suffix('.rst')
-        parse_py_and_write_rst(origin_file_path=f, target_file_path=rst_file)
+        py_to_rst(origin_file_path=f, target_file_path=rst_file)
 
 
 def _find_existing_rst_files(
         py_files: list[Path],  # where the .py files are
         target_path: Path  # where the .rst should go
 ) -> list[str | Path]:
     out = []
@@ -66,56 +67,84 @@
 
 
 # ----------------------------------------------------------------------
 
 def _create_basic_usage_rst(
         target_path: Path,
         *,
-        title: str = "Tutorials",
         pkg_name: str = None,
-        show_versions: bool = False
 ) -> None:
-    basic_usage_rst_path = target_path / 'basic-usage.rst'
+    tutorials_rst_path = target_path / 'tutorials.rst'
 
     # get a list of all the available RST files
-    rst_files = [
-        file.relative_to(target_path)
-        for file in target_path.glob('**/*.rst')
-        if file.name != 'basic-usage.rst'
-    ]
+    rsts = _create_folder_files_dict(target_path=target_path)
 
-    # Create the content for 'basic-usage.rst'
-    rst_content = f"{title}\n{'=' * len(title)}\n\n"
+    rst_content = ""
+    for title, files in rsts.items():
+        # Add a toctree directive for all generated RST files
+        rst_content += add_toc_tree(title=title, rst_files=files)
 
-    if pkg_name is not None:
-        rst_content += f"""
-Tutorials to get you started using {pkg_name}.
-        """
+    if pkg_name:
+        rst_content = add_show_dependencies(rst_content, pkg_name)
 
-    # Add a toctree directive for all generated RST files
-    rst_content += """
-.. toctree::
-   :maxdepth: 2
-    """
+    # Write the content to 'tutorials.rst'
+    with tutorials_rst_path.open('w') as rst_file:
+        rst_file.write(rst_content)
 
-    for rst_file in rst_files:
-        rst_content += f"""
-   {rst_file}
-        """
 
-    if show_versions:
-        rst_content += f"""
-    
+def add_show_dependencies(rst_content: str, pkg_name: str) -> str:
+    rst_content += f"""
+
 .. code-example:: Dependencies Versions in Tutorials
     :collapsible:
 
     .. ipython:: python
-    
+
         import {pkg_name}
-        
+
         {pkg_name}.show_versions()
-    
-    """
 
-    # Write the content to 'basic-usage.rst'
-    with basic_usage_rst_path.open('w') as rst_file:
-        rst_file.write(rst_content)
+        """
+    return rst_content
+
+
+def add_toc_tree(title: str | None, rst_files: list) -> str:
+    if title is None:
+        title = 'Tutorials'
+
+    title = title.replace("_", " ").title().strip()
+
+    toc_str = f"\n{title}\n{'=' * len(title)}\n\n"
+
+    # Add a toctree directive for all generated RST files
+    toc_str += """
+.. toctree::
+   :maxdepth: 1
+        """
+
+    for rst_file in rst_files:
+        toc_str += f"""
+   {rst_file}
+            """
+
+    return toc_str
+
+
+def _create_folder_files_dict(
+        target_path: Path,
+        exclude_file: str = 'tutorials.rst') -> dict[str | None, list[Path]]:
+    rst_files = [
+        file.relative_to(target_path)
+        for file in target_path.glob('**/*.rst')
+        if file.name != exclude_file
+    ]
+
+    folder_files_dict = {}
+
+    # todo: instead of separating with - make the subfolders subtitles
+    for file in rst_files:
+        # Generate the key by joining folder names with " - ",
+        # or use 'root' for files at the root level
+        folder = " - ".join(file.parts[:-1]) if len(file.parts) > 1 else 'root'
+        folder_files_dict.setdefault(folder, []).append(file)
+
+    return folder_files_dict
```

### Comparing `sphinx_tutorials-0.0.2/src/sphinx_tutorials.egg-info/PKG-INFO` & `sphinx_tutorials-0.0.3/src/sphinx_tutorials.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx_tutorials
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tools for docs in Python
 Author-email: Bernardo Dionisi <bernardo.dionisi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bernardodionisi/sphinx_tutorials
 Project-URL: Source, https://github.com/bernardodionisi/sphinx_tutorials
 Project-URL: Issues, https://github.com/bernardodionisi/sphinx_tutorials/issues
 Project-URL: Documentation, https://bernardodionisi.github.io/sphinx_tutorials/latest/
@@ -18,16 +18,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: click
-Requires-Dist: polars
-Requires-Dist: matplotlib
+Requires-Dist: sphinx<7.3
+Requires-Dist: sphinx-immaterial==0.11.11
+Requires-Dist: myst-parser==0.18.1
+Requires-Dist: sphinx-design==0.5.0
+Requires-Dist: sphinx-last-updated-by-git==0.3.6
+Requires-Dist: sphinx-math-dollar==1.2.1
+Requires-Dist: ipykernel==6.26.0
+Requires-Dist: myst-nb==0.17.2
+Requires-Dist: pickleshare==0.7.5
 Requires-Dist: typing_extensions>=4.0.0
 Provides-Extra: dev
 
 # `sphinx_tutorials`
-
-functionality coming soon !
```

