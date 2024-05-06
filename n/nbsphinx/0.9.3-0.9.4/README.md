# Comparing `tmp/nbsphinx-0.9.3.tar.gz` & `tmp/nbsphinx-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbsphinx-0.9.3.tar", last modified: Sun Aug 27 10:57:29 2023, max compression
+gzip compressed data, was "nbsphinx-0.9.4.tar", last modified: Mon May  6 19:29:13 2024, max compression
```

## Comparing `nbsphinx-0.9.3.tar` & `nbsphinx-0.9.4.tar`

### file list

```diff
@@ -1,63 +1,80 @@
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-08-27 10:57:29.740750 nbsphinx-0.9.3/
--rw-r--r--   0 mg        (1000) mg        (1000)     3700 2022-09-18 14:14:25.000000 nbsphinx-0.9.3/CONTRIBUTING.rst
--rw-r--r--   0 mg        (1000) mg        (1000)     1063 2023-03-14 09:55:02.000000 nbsphinx-0.9.3/LICENSE
--rw-r--r--   0 mg        (1000) mg        (1000)      229 2022-08-28 14:43:55.000000 nbsphinx-0.9.3/MANIFEST.in
--rw-r--r--   0 mg        (1000) mg        (1000)    13809 2023-08-27 10:56:08.000000 nbsphinx-0.9.3/NEWS.rst
--rw-r--r--   0 mg        (1000) mg        (1000)     1929 2023-08-27 10:57:29.736750 nbsphinx-0.9.3/PKG-INFO
--rw-r--r--   0 mg        (1000) mg        (1000)      980 2022-09-18 14:14:25.000000 nbsphinx-0.9.3/README.rst
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-08-27 10:57:29.728750 nbsphinx-0.9.3/doc/
--rw-r--r--   0 mg        (1000) mg        (1000)     9607 2023-06-11 17:18:33.000000 nbsphinx-0.9.3/doc/a-normal-rst-file.rst
--rw-r--r--   0 mg        (1000) mg        (1000)     2297 2022-08-28 14:43:55.000000 nbsphinx-0.9.3/doc/allow-errors-per-cell.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     2578 2022-09-18 14:14:25.000000 nbsphinx-0.9.3/doc/allow-errors.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)    21584 2023-06-11 17:18:33.000000 nbsphinx-0.9.3/doc/code-cells.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     7280 2023-07-07 18:38:14.000000 nbsphinx-0.9.3/doc/conf.py
--rw-r--r--   0 mg        (1000) mg        (1000)    13609 2023-05-06 17:18:22.000000 nbsphinx-0.9.3/doc/configuration.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     3318 2023-03-14 09:55:02.000000 nbsphinx-0.9.3/doc/configuring-kernels.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)       33 2022-08-28 14:43:55.000000 nbsphinx-0.9.3/doc/contributing.rst
--rw-r--r--   0 mg        (1000) mg        (1000)     3642 2022-08-28 14:43:55.000000 nbsphinx-0.9.3/doc/custom-css.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     1556 2022-09-18 16:09:51.000000 nbsphinx-0.9.3/doc/executing-notebooks.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     2113 2022-08-21 14:47:54.000000 nbsphinx-0.9.3/doc/hidden-cells.ipynb
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-08-27 10:57:29.728750 nbsphinx-0.9.3/doc/images/
--rw-r--r--   0 mg        (1000) mg        (1000)     8031 2017-11-28 19:42:46.000000 nbsphinx-0.9.3/doc/images/notebook_icon.png
--rw-r--r--   0 mg        (1000) mg        (1000)    15301 2022-08-28 14:43:55.000000 nbsphinx-0.9.3/doc/images/python_logo.svg
--rw-r--r--   0 mg        (1000) mg        (1000)    39583 2023-03-14 09:55:02.000000 nbsphinx-0.9.3/doc/images/raw_cells_jupyter_notebook.png
--rw-r--r--   0 mg        (1000) mg        (1000)    37656 2023-03-14 09:55:02.000000 nbsphinx-0.9.3/doc/images/raw_cells_jupyterlab.png
--rw-r--r--   0 mg        (1000) mg        (1000)     2405 2023-03-14 09:55:02.000000 nbsphinx-0.9.3/doc/index.rst
--rw-r--r--   0 mg        (1000) mg        (1000)     6987 2023-06-11 17:18:33.000000 nbsphinx-0.9.3/doc/installation.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     7864 2023-03-14 09:55:02.000000 nbsphinx-0.9.3/doc/links.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)    29649 2023-06-11 17:32:19.000000 nbsphinx-0.9.3/doc/markdown-cells.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     1913 2022-08-21 14:47:54.000000 nbsphinx-0.9.3/doc/never-execute.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     2035 2022-08-21 14:47:54.000000 nbsphinx-0.9.3/doc/orphan.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     7234 2022-09-18 14:14:25.000000 nbsphinx-0.9.3/doc/pre-executed.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     5441 2022-09-18 14:14:25.000000 nbsphinx-0.9.3/doc/prolog-and-epilog.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     6746 2023-03-14 09:55:02.000000 nbsphinx-0.9.3/doc/raw-cells.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)      977 2023-06-25 16:50:31.000000 nbsphinx-0.9.3/doc/references.bib
--rw-r--r--   0 mg        (1000) mg        (1000)      775 2023-06-11 17:18:33.000000 nbsphinx-0.9.3/doc/references.rst
--rw-r--r--   0 mg        (1000) mg        (1000)      158 2023-08-26 15:47:11.000000 nbsphinx-0.9.3/doc/requirements.txt
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-08-27 10:57:29.732750 nbsphinx-0.9.3/doc/subdir/
--rw-r--r--   0 mg        (1000) mg        (1000)     2394 2023-03-14 09:55:02.000000 nbsphinx-0.9.3/doc/subdir/a-notebook-in-a-subdir.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     2294 2023-03-14 09:55:02.000000 nbsphinx-0.9.3/doc/subdir/gallery.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     5033 2023-03-14 09:55:02.000000 nbsphinx-0.9.3/doc/subdir/toctree.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     1729 2022-08-28 14:43:55.000000 nbsphinx-0.9.3/doc/timeout.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)    23012 2023-06-11 17:18:33.000000 nbsphinx-0.9.3/doc/usage.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)       58 2022-08-28 14:43:55.000000 nbsphinx-0.9.3/doc/version-history.rst
--rw-r--r--   0 mg        (1000) mg        (1000)      908 2023-03-02 19:46:03.000000 nbsphinx-0.9.3/doc/yet-another.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)       91 2023-03-14 09:55:02.000000 nbsphinx-0.9.3/pyproject.toml
--rw-r--r--   0 mg        (1000) mg        (1000)       38 2023-08-27 10:57:29.740750 nbsphinx-0.9.3/setup.cfg
--rw-r--r--   0 mg        (1000) mg        (1000)     1807 2023-03-14 09:55:02.000000 nbsphinx-0.9.3/setup.py
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-08-27 10:57:29.712750 nbsphinx-0.9.3/src/
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-08-27 10:57:29.732750 nbsphinx-0.9.3/src/nbsphinx/
--rw-r--r--   0 mg        (1000) mg        (1000)    74663 2023-08-27 10:56:06.000000 nbsphinx-0.9.3/src/nbsphinx/__init__.py
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-08-27 10:57:29.736750 nbsphinx-0.9.3/src/nbsphinx/_static/
--rw-r--r--   0 mg        (1000) mg        (1000)     4467 2023-03-14 09:55:02.000000 nbsphinx-0.9.3/src/nbsphinx/_static/nbsphinx-broken-thumbnail.svg
--rw-r--r--   0 mg        (1000) mg        (1000)     7344 2023-06-11 17:18:33.000000 nbsphinx-0.9.3/src/nbsphinx/_static/nbsphinx-code-cells.css_t
--rw-r--r--   0 mg        (1000) mg        (1000)      584 2023-03-14 09:55:02.000000 nbsphinx-0.9.3/src/nbsphinx/_static/nbsphinx-gallery.css
--rw-r--r--   0 mg        (1000) mg        (1000)     2871 2023-03-14 09:55:02.000000 nbsphinx-0.9.3/src/nbsphinx/_static/nbsphinx-no-thumbnail.svg
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-08-27 10:57:29.736750 nbsphinx-0.9.3/src/nbsphinx/_texinputs/
--rw-r--r--   0 mg        (1000) mg        (1000)     8202 2023-03-14 09:55:02.000000 nbsphinx-0.9.3/src/nbsphinx/_texinputs/nbsphinx.sty
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-08-27 10:57:29.736750 nbsphinx-0.9.3/src/nbsphinx.egg-info/
--rw-r--r--   0 mg        (1000) mg        (1000)     1929 2023-08-27 10:57:29.000000 nbsphinx-0.9.3/src/nbsphinx.egg-info/PKG-INFO
--rw-r--r--   0 mg        (1000) mg        (1000)     1324 2023-08-27 10:57:29.000000 nbsphinx-0.9.3/src/nbsphinx.egg-info/SOURCES.txt
--rw-r--r--   0 mg        (1000) mg        (1000)        1 2023-08-27 10:57:29.000000 nbsphinx-0.9.3/src/nbsphinx.egg-info/dependency_links.txt
--rw-r--r--   0 mg        (1000) mg        (1000)       65 2023-08-27 10:57:29.000000 nbsphinx-0.9.3/src/nbsphinx.egg-info/requires.txt
--rw-r--r--   0 mg        (1000) mg        (1000)        9 2023-08-27 10:57:29.000000 nbsphinx-0.9.3/src/nbsphinx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:29:13.959459 nbsphinx-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14048 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-06 19:29:13.959459 nbsphinx-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:29:13.955459 nbsphinx-0.9.4/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/a-markdown-file.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9596 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/a-normal-rst-file.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/allow-errors-per-cell.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/allow-errors.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    22232 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/code-cells.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7280 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13609 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/configuration.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/configuring-kernels.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/custom-css.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/custom-formats.pct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/executing-notebooks.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/fallback_theme.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/favicon.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:29:13.955459 nbsphinx-0.9.4/doc/gallery/
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/gallery/cell-metadata.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/gallery/cell-tag.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/gallery/default-thumbnail.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/gallery/due-rst.pct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/gallery/gallery-with-links.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/gallery/gallery-with-nested-documents.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/gallery/matplotlibrc
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/gallery/multiple-outputs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/gallery/no-thumbnail.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3886 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/gallery/thumbnail-from-conf-py.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/gallery/uno-rst.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/hidden-cells.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:29:13.959459 nbsphinx-0.9.4/doc/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     8031 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/images/notebook_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15301 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/images/python_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    39583 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/images/raw_cells_jupyter_notebook.png
+-rw-r--r--   0 runner    (1001) docker     (127)    37656 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/images/raw_cells_jupyterlab.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6910 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/installation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8108 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/links.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    29649 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/markdown-cells.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/matplotlibrc
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/never-execute.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/orphan.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/pre-executed.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/prolog-and-epilog.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6746 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/raw-cells.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/references.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/references.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:29:13.959459 nbsphinx-0.9.4/doc/subdir/
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/subdir/a-notebook-in-a-subdir.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/subdir/gallery.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/subdir/toctree.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/timeout.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    23012 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/version-history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/doc/yet-another.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 19:29:13.959459 nbsphinx-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:29:13.947459 nbsphinx-0.9.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:29:13.959459 nbsphinx-0.9.4/src/nbsphinx/
+-rw-r--r--   0 runner    (1001) docker     (127)    74617 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/src/nbsphinx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:29:13.959459 nbsphinx-0.9.4/src/nbsphinx/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/src/nbsphinx/_static/nbsphinx-broken-thumbnail.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/src/nbsphinx/_static/nbsphinx-code-cells.css_t
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/src/nbsphinx/_static/nbsphinx-gallery.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/src/nbsphinx/_static/nbsphinx-no-thumbnail.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:29:13.959459 nbsphinx-0.9.4/src/nbsphinx/_texinputs/
+-rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-05-06 19:29:10.000000 nbsphinx-0.9.4/src/nbsphinx/_texinputs/nbsphinx.sty
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:29:13.959459 nbsphinx-0.9.4/src/nbsphinx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-06 19:29:13.000000 nbsphinx-0.9.4/src/nbsphinx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-06 19:29:13.000000 nbsphinx-0.9.4/src/nbsphinx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 19:29:13.000000 nbsphinx-0.9.4/src/nbsphinx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-06 19:29:13.000000 nbsphinx-0.9.4/src/nbsphinx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-06 19:29:13.000000 nbsphinx-0.9.4/src/nbsphinx.egg-info/top_level.txt
```

### Comparing `nbsphinx-0.9.3/CONTRIBUTING.rst` & `nbsphinx-0.9.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.3/LICENSE` & `nbsphinx-0.9.4/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2015-2023 Matthias Geier
+Copyright (c) 2015-2024 Matthias Geier
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `nbsphinx-0.9.3/NEWS.rst` & `nbsphinx-0.9.4/NEWS.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+Version 0.9.4 -- 2024-05-06 -- PyPI__ -- diff__
+ * Require ``docutils >= 0.18.1``
+ * Minor fixes, documentation and CI updates
+
+__ https://pypi.org/project/nbsphinx/0.9.4/
+__ https://github.com/spatialaudio/nbsphinx/compare/0.9.3...0.9.4
+
 Version 0.9.3 -- 2023-08-27 -- PyPI__ -- diff__
  * Fix gallery regression in Sphinx 7.2
 
 __ https://pypi.org/project/nbsphinx/0.9.3/
 __ https://github.com/spatialaudio/nbsphinx/compare/0.9.2...0.9.3
 
 Version 0.9.2 -- 2023-05-24 -- PyPI__ -- diff__
```

### Comparing `nbsphinx-0.9.3/PKG-INFO` & `nbsphinx-0.9.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbsphinx
-Version: 0.9.3
+Version: 0.9.4
 Summary: Jupyter Notebook Tools for Sphinx
 Home-page: https://nbsphinx.readthedocs.io/
 Author: Matthias Geier
 Author-email: Matthias.Geier@gmail.com
 License: MIT
 Project-URL: Documentation, https://nbsphinx.readthedocs.io/
 Project-URL: Source Code, https://github.com/spatialaudio/nbsphinx/
@@ -19,14 +19,20 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Documentation :: Sphinx
 Requires-Python: >=3.6
 License-File: LICENSE
+Requires-Dist: docutils>=0.18.1
+Requires-Dist: jinja2
+Requires-Dist: nbconvert!=5.4,>=5.3
+Requires-Dist: traitlets>=5
+Requires-Dist: nbformat
+Requires-Dist: sphinx>=1.8
 
 Jupyter Notebook Tools for Sphinx
 =================================
 
 ``nbsphinx`` is a Sphinx_ extension that provides a source parser for
 ``*.ipynb`` files.
 Custom Sphinx directives are used to show `Jupyter Notebook`_ code cells (and of
```

### Comparing `nbsphinx-0.9.3/README.rst` & `nbsphinx-0.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.3/doc/a-normal-rst-file.rst` & `nbsphinx-0.9.4/doc/a-normal-rst-file.rst`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
 
 Links to Notebooks, Ye Olde Way
 -------------------------------
 
 In addition to the way shown above, you can also create links to notebooks (and
 other Sphinx source files) with
-`:ref: <https://www.sphinx-doc.org/en/master/usage/restructuredtext/roles.html#role-ref>`_.
+`:ref: <https://www.sphinx-doc.org/en/master/usage/referencing.html#role-ref>`_.
 This has some disadvantages:
 
 * It is arguably a bit more clunky.
 * Because ``:ref:`` is a Sphinx feature, the links don't work on Github and
   other rendered reStructuredText pages that use plain old ``docutils``.
 
 It also has one important advantage:
```

### Comparing `nbsphinx-0.9.3/doc/allow-errors-per-cell.ipynb` & `nbsphinx-0.9.4/doc/allow-errors-per-cell.ipynb`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.3/doc/allow-errors.ipynb` & `nbsphinx-0.9.4/doc/allow-errors.ipynb`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.3/doc/code-cells.ipynb` & `nbsphinx-0.9.4/doc/code-cells.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9948830409356725%*

 * *Differences: {"'cells'": "{70: {'source': {insert: [(0, 'The following code showing the 8 basic ANSI colors is "*

 * *            'based on '*

 * *            "https://web.archive.org/web/20231225185739/https://tldp.org/HOWTO/Bash-Prompt-HOWTO/x329.html.\\n')], "*

 * *            "delete: [0]}}, insert: [(43, OrderedDict([('cell_type', 'markdown'), ('metadata', "*

 * *            "OrderedDict()), ('source', ['Instead of the default `inline` plotting backend,\\n', "*

 * *            "'you can also use the `widget` backend\\n', '(which needs the  […]*

```diff
@@ -419,14 +419,42 @@
                 "fig"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "Instead of the default `inline` plotting backend,\n",
+                "you can also use the `widget` backend\n",
+                "(which needs the `ipympl` package to be installed):"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "%matplotlib widget"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "fig, ax = plt.subplots(figsize=[6, 3])\n",
+                "ax.plot([4, 9, 7, 20, 6, 33, 13, 23, 16, 62, 8]);"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "### Pandas Dataframes\n",
                 "\n",
                 "[Pandas dataframes](https://pandas.pydata.org/pandas-docs/stable/user_guide/dsintro.html#dataframe)\n",
                 "should be displayed as nicely formatted HTML tables (if you are using HTML output)."
             ]
         },
         {
@@ -738,15 +766,15 @@
                 "      'KL\\x1b[49mMN\\x1b[39mOP\\x1b[22mQR\\x1b[24mST\\x1b[27mUV')"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The following code showing the 8 basic ANSI colors is based on https://tldp.org/HOWTO/Bash-Prompt-HOWTO/x329.html.\n",
+                "The following code showing the 8 basic ANSI colors is based on https://web.archive.org/web/20231225185739/https://tldp.org/HOWTO/Bash-Prompt-HOWTO/x329.html.\n",
                 "Each of the 8 colors has an \"intense\" variation, which is used for bold text."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
```

### Comparing `nbsphinx-0.9.3/doc/conf.py` & `nbsphinx-0.9.4/doc/conf.py`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.3/doc/configuration.ipynb` & `nbsphinx-0.9.4/doc/configuration.ipynb`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.3/doc/configuring-kernels.ipynb` & `nbsphinx-0.9.4/doc/configuring-kernels.ipynb`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.3/doc/custom-css.ipynb` & `nbsphinx-0.9.4/doc/custom-css.ipynb`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.3/doc/executing-notebooks.ipynb` & `nbsphinx-0.9.4/doc/executing-notebooks.ipynb`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.3/doc/hidden-cells.ipynb` & `nbsphinx-0.9.4/doc/hidden-cells.ipynb`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.3/doc/images/notebook_icon.png` & `nbsphinx-0.9.4/doc/images/notebook_icon.png`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.3/doc/images/python_logo.svg` & `nbsphinx-0.9.4/doc/images/python_logo.svg`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.3/doc/images/raw_cells_jupyter_notebook.png` & `nbsphinx-0.9.4/doc/images/raw_cells_jupyter_notebook.png`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.3/doc/images/raw_cells_jupyterlab.png` & `nbsphinx-0.9.4/doc/images/raw_cells_jupyterlab.png`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.3/doc/index.rst` & `nbsphinx-0.9.4/doc/index.rst`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.3/doc/installation.ipynb` & `nbsphinx-0.9.4/doc/installation.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988617376775272%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(12, '[Miniforge](https://github.com/conda-forge/miniforge) "*

 * *            "or\\n'), (13, '[Miniconda](https://docs.conda.io/en/latest/miniconda.html)),\\n')], "*

 * *            'delete: [14, 13, 12]}}, 2: {\'source\': {insert: [(8, "If you don\'t know which one '*

 * *            'is best for you, you can try '*

 * *            '[Miniforge](https://github.com/conda-forge/miniforge).\\n")], delete: [8]}}}'}*

```diff
@@ -21,17 +21,16 @@
                 "\n",
                 "## `nbsphinx` Packages\n",
                 "\n",
                 "[![Anaconda Badge](https://anaconda.org/conda-forge/nbsphinx/badges/version.svg)](https://anaconda.org/conda-forge/nbsphinx)\n",
                 "\n",
                 "If you are using the `conda` package manager\n",
                 "(e.g. with\n",
-                "[Miniforge](https://github.com/conda-forge/miniforge),\n",
-                "[Miniconda](https://docs.conda.io/en/latest/miniconda.html) or\n",
-                "[Anaconda](https://www.anaconda.com/download#downloads)),\n",
+                "[Miniforge](https://github.com/conda-forge/miniforge) or\n",
+                "[Miniconda](https://docs.conda.io/en/latest/miniconda.html)),\n",
                 "you can install `nbsphinx` from the [conda-forge](https://conda-forge.org/) channel:\n",
                 "\n",
                 "    conda install -c conda-forge nbsphinx\n",
                 "\n",
                 "[![PyPI version](https://badge.fury.io/py/nbsphinx.png)](https://pypi.org/project/nbsphinx)\n",
                 "\n",
                 "You can of course also install `nbsphinx` with `pip`, Python's own package manager:\n",
@@ -56,15 +55,15 @@
                 "\n",
                 "Some of the aforementioned packages will install some of these prerequisites automatically, some of the things may be already installed on your computer anyway.\n",
                 "\n",
                 "### Python\n",
                 "\n",
                 "Of course you'll need Python, because both Sphinx and `nbsphinx` are implemented in Python.\n",
                 "There are many ways to get Python.\n",
-                "If you don't know which one is best for you, you can try [Miniforge/Mambaforge](https://github.com/conda-forge/miniforge).\n",
+                "If you don't know which one is best for you, you can try [Miniforge](https://github.com/conda-forge/miniforge).\n",
                 "\n",
                 "### Sphinx\n",
                 "\n",
                 "You'll need [Sphinx](https://www.sphinx-doc.org/) as well, because `nbsphinx` is just a Sphinx extension and doesn't do anything on its own.\n",
                 "\n",
                 "If you use `conda`, you can get [Sphinx from the conda-forge channel](https://anaconda.org/conda-forge/sphinx):\n",
                 "\n",
```

### Comparing `nbsphinx-0.9.3/doc/links.ipynb` & `nbsphinx-0.9.4/doc/links.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9947916666666667%*

 * *Differences: {"'cells'": "{insert: [(19, OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), "*

 * *            "('source', ['**Quarto**\\n', '\\n', 'Open-source scientific and technical publishing "*

 * *            "system built on Pandoc.\\n', '\\n', 'https://github.com/quarto-dev/quarto-cli'])]))]}"}*

```diff
@@ -236,14 +236,25 @@
                 "http://hplgit.github.io/doconce/doc/web/index.html"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "**Quarto**\n",
+                "\n",
+                "Open-source scientific and technical publishing system built on Pandoc.\n",
+                "\n",
+                "https://github.com/quarto-dev/quarto-cli"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "**Converting Notebooks to reStructuredText**\n",
                 "\n",
                 "https://github.com/perrette/dimarray/blob/master/docs/scripts/nbconvert_to_rst.py\n",
                 "\n",
                 "`https://gist.github.com/hadim/16e29b5848672e2e497c` (not available anymore)\n",
                 "\n",
                 "https://sphinx-ipynb.readthedocs.io/"
```

### Comparing `nbsphinx-0.9.3/doc/markdown-cells.ipynb` & `nbsphinx-0.9.4/doc/markdown-cells.ipynb`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.3/doc/never-execute.ipynb` & `nbsphinx-0.9.4/doc/never-execute.ipynb`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.3/doc/orphan.ipynb` & `nbsphinx-0.9.4/doc/orphan.ipynb`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.3/doc/pre-executed.ipynb` & `nbsphinx-0.9.4/doc/pre-executed.ipynb`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.3/doc/prolog-and-epilog.ipynb` & `nbsphinx-0.9.4/doc/prolog-and-epilog.ipynb`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.3/doc/raw-cells.ipynb` & `nbsphinx-0.9.4/doc/raw-cells.ipynb`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.3/doc/references.bib` & `nbsphinx-0.9.4/doc/references.bib`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.3/doc/references.rst` & `nbsphinx-0.9.4/doc/references.rst`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.3/doc/subdir/a-notebook-in-a-subdir.ipynb` & `nbsphinx-0.9.4/doc/subdir/a-notebook-in-a-subdir.ipynb`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.3/doc/subdir/gallery.ipynb` & `nbsphinx-0.9.4/doc/subdir/gallery.ipynb`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.3/doc/subdir/toctree.ipynb` & `nbsphinx-0.9.4/doc/subdir/toctree.ipynb`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.3/doc/timeout.ipynb` & `nbsphinx-0.9.4/doc/timeout.ipynb`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.3/doc/usage.ipynb` & `nbsphinx-0.9.4/doc/usage.ipynb`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.3/doc/yet-another.ipynb` & `nbsphinx-0.9.4/doc/yet-another.ipynb`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.3/setup.py` & `nbsphinx-0.9.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,17 +20,17 @@
         '_static/nbsphinx-gallery.css',
         '_static/nbsphinx-no-thumbnail.svg',
         '_static/nbsphinx-broken-thumbnail.svg',
         '_texinputs/nbsphinx.sty',
     ]},
     python_requires='>=3.6',
     install_requires=[
-        'docutils',
+        'docutils>=0.18.1',
         'jinja2',
-        'nbconvert!=5.4',
+        'nbconvert>=5.3,!=5.4',
         'traitlets>=5',
         'nbformat',
         'sphinx>=1.8',
     ],
     author='Matthias Geier',
     author_email='Matthias.Geier@gmail.com',
     description='Jupyter Notebook Tools for Sphinx',
```

### Comparing `nbsphinx-0.9.3/src/nbsphinx/__init__.py` & `nbsphinx-0.9.4/src/nbsphinx/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Jupyter Notebook Tools for Sphinx.
 
 https://nbsphinx.readthedocs.io/
 
 """
-__version__ = '0.9.3'
+__version__ = '0.9.4'
 
 import collections.abc
 import copy
 import html
 from itertools import chain
 import json
 import os
@@ -612,15 +612,15 @@
             allow_errors=env.config.nbsphinx_allow_errors,
             timeout=env.config.nbsphinx_timeout,
             codecell_lexer=env.config.nbsphinx_codecell_lexer,
         )
 
         try:
             rststring, resources = exporter.from_notebook_node(nb, resources)
-        except nbconvert.preprocessors.execute.CellExecutionError as e:
+        except nbconvert.preprocessors.CellExecutionError as e:
             lines = str(e).split('\n')
             lines[0] = 'CellExecutionError in {}:'.format(
                 env.doc2path(env.docname, base=None))
             lines.append("You can ignore this error by setting the following "
                          "in conf.py:\n\n    nbsphinx_allow_errors = True\n")
             raise NotebookError('\n'.join(lines))
         except Exception as e:
@@ -1108,30 +1108,30 @@
             else:
                 lines.append(':{}: {}'.format(option, value))
     except AttributeError:
         raise ValueError(
             'invalid nbsphinx-[link-]gallery/nbsphinx-toctree option: {!r}'
             .format(options))
 
-    text = nbconvert.filters.markdown2rst(cell.source)
+    text = markdown2rst(cell.source)
     settings = docutils.frontend.OptionParser(
         components=(rst.Parser,)).get_default_values()
     node = docutils.utils.new_document('gallery_or_toctree', settings)
     parser = rst.Parser()
     parser.parse(text, node)
 
     if 'caption' not in options:
-        for sec in node.traverse(docutils.nodes.section):
+        for sec in node.findall(docutils.nodes.section):
             assert sec.children
             assert isinstance(sec.children[0], docutils.nodes.title)
             title = sec.children[0].astext()
             lines.append(':caption: ' + title)
             break
     lines.append('')  # empty line
-    for ref in node.traverse(docutils.nodes.reference):
+    for ref in node.findall(docutils.nodes.reference):
         lines.append(ref['name'] + ' <' + unquote(ref.get('refuri')) + '>')
     return '\n    '.join(lines)
 
 
 def _get_empty_lines(text):
     """Get number of empty lines before and after code."""
     before = len(text) - len(text.lstrip('\n'))
@@ -1221,15 +1221,15 @@
 
     """
 
     default_priority = 500  # After AnonymousHyperlinks (440)
 
     def apply(self):
         env = self.document.settings.env
-        for node in self.document.traverse(docutils.nodes.reference):
+        for node in self.document.findall(docutils.nodes.reference):
             filename, fragment = _local_file_from_reference(
                 node, self.document)
             if not filename:
                 if fragment:
                     # This should not be needed if it weren't for
                     # https://github.com/sphinx-doc/sphinx/issues/11336 and
                     # https://github.com/sphinx-doc/sphinx/issues/11335
@@ -1260,15 +1260,15 @@
                 reftarget = '/' + target_docname + target_ext
                 if reftype == 'ref':
                     reftarget = reftarget.lower()
                 linktext = node.astext()
                 xref = sphinx.addnodes.pending_xref(
                     reftype=reftype, reftarget=reftarget, refdomain='std',
                     refwarn=True, refexplicit=True, refdoc=env.docname)
-                xref += docutils.nodes.Text(linktext, linktext)
+                xref += docutils.nodes.Text(linktext)
                 node.replace_self(xref)
             else:
                 # NB: This is a link to an ignored (via exclude_patterns)
                 #     source file.
                 pass
 
 
@@ -1280,15 +1280,15 @@
 
     """
 
     default_priority = 200  # Before CreateSectionLabels (250)
 
     def apply(self):
         all_ids = set()
-        for section in self.document.traverse(docutils.nodes.section):
+        for section in self.document.findall(docutils.nodes.section):
             title = section[0].astext()
             link_id = title.replace(' ', '-').replace('"', '%22')
             if link_id in all_ids:
                 # Avoid duplicated anchors on the same page
                 continue
             all_ids.add(link_id)
             section['ids'] = [link_id]
@@ -1309,15 +1309,15 @@
 
     default_priority = 250  # Before references.PropagateTargets (260)
 
     def apply(self):
         env = self.document.settings.env
         file_ext = env.doc2path(env.docname, base=None)[len(env.docname):]
         i_still_have_to_create_the_document_label = True
-        for section in self.document.traverse(docutils.nodes.section):
+        for section in self.document.findall(docutils.nodes.section):
             assert section.children
             assert isinstance(section.children[0], docutils.nodes.title)
             title = section.children[0].astext()
             link_id = section['ids'][0]
             label = '/' + env.docname + file_ext + '#' + link_id
             label = label.lower()
             env.domaindata['std']['labels'][label] = (
@@ -1339,15 +1339,15 @@
     """Create labels for domain-specific object signatures."""
 
     default_priority = 250  # About the same as CreateSectionLabels
 
     def apply(self):
         env = self.document.settings.env
         file_ext = env.doc2path(env.docname, base=None)[len(env.docname):]
-        for sig in self.document.traverse(sphinx.addnodes.desc_signature):
+        for sig in self.document.findall(sphinx.addnodes.desc_signature):
             try:
                 title = sig['ids'][0]
             except IndexError:
                 # Object has same name as another, so skip it
                 continue
             link_id = title.replace(' ', '-')
             sig['ids'] = [link_id]
@@ -1373,15 +1373,15 @@
         r'\s*<div\s*class\s*=\s*(?P<q>"|\')([a-z\s-]*)(?P=q)\s*>\s*\Z',
         flags=re.IGNORECASE)
     _class_re = re.compile(r'\s*alert\s*alert-(info|warning)\s*\Z')
     _end_re = re.compile(r'\s*</div\s*>\s*\Z', flags=re.IGNORECASE)
 
     def apply(self):
         start_tags = []
-        for node in self.document.traverse(docutils.nodes.raw):
+        for node in self.document.findall(docutils.nodes.raw):
             if node['format'] != 'html':
                 continue
             start_match = self._start_re.match(node.astext())
             if not start_match:
                 continue
             class_match = self._class_re.match(start_match.group(2))
             if not class_match:
@@ -1390,15 +1390,15 @@
             if admonition_class == 'info':
                 admonition_class = 'note'
             start_tags.append((node, admonition_class))
 
         # Reversed order to allow nested <div> elements:
         for node, admonition_class in reversed(start_tags):
             content = []
-            for sibling in node.traverse(include_self=False, descend=False,
+            for sibling in node.findall(include_self=False, descend=False,
                                          siblings=True, ascend=False):
                 end_tag = (isinstance(sibling, docutils.nodes.raw) and
                            sibling['format'] == 'html' and
                            self._end_re.match(sibling.astext()))
                 if end_tag:
                     admonition_node = AdmonitionNode(
                         classes=['admonition', admonition_class])
@@ -1416,15 +1416,15 @@
 class CopyLinkedFiles(docutils.transforms.Transform):
     """Mark linked (local) files to be copied to the HTML output."""
 
     default_priority = 600  # After RewriteLocalLinks
 
     def apply(self):
         env = self.document.settings.env
-        for node in self.document.traverse(docutils.nodes.reference):
+        for node in self.document.findall(docutils.nodes.reference):
             filename, fragment = _local_file_from_reference(
                 node, self.document)
             if not filename:
                 continue  # Not a local link
             relpath = filename + fragment
             file = os.path.normpath(
                 os.path.join(os.path.dirname(env.docname), relpath))
@@ -1716,15 +1716,15 @@
 
 
 def doctree_resolved(app, doctree, fromdocname):
     base = sphinx.util.osutil.relative_uri(
         app.builder.get_target_uri(fromdocname), '')
 
     # Replace GalleryToc with toctree + GalleryNode
-    for node in doctree.traverse(GalleryToc):
+    for node in doctree.findall(GalleryToc):
         toctree_wrapper, = node
         if (len(toctree_wrapper) != 1 or not isinstance(
                 toctree_wrapper[0],
                 (sphinx.addnodes.toctree, DummyTocTree))):
             # This happens for LaTeX output
             node.replace_self(node.children)
             continue
```

### Comparing `nbsphinx-0.9.3/src/nbsphinx/_static/nbsphinx-broken-thumbnail.svg` & `nbsphinx-0.9.4/src/nbsphinx/_static/nbsphinx-broken-thumbnail.svg`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.3/src/nbsphinx/_static/nbsphinx-code-cells.css_t` & `nbsphinx-0.9.4/src/nbsphinx/_static/nbsphinx-code-cells.css_t`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.3/src/nbsphinx/_static/nbsphinx-gallery.css` & `nbsphinx-0.9.4/src/nbsphinx/_static/nbsphinx-gallery.css`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.3/src/nbsphinx/_static/nbsphinx-no-thumbnail.svg` & `nbsphinx-0.9.4/src/nbsphinx/_static/nbsphinx-no-thumbnail.svg`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.3/src/nbsphinx/_texinputs/nbsphinx.sty` & `nbsphinx-0.9.4/src/nbsphinx/_texinputs/nbsphinx.sty`

 * *Files identical despite different names*

### Comparing `nbsphinx-0.9.3/src/nbsphinx.egg-info/PKG-INFO` & `nbsphinx-0.9.4/src/nbsphinx.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbsphinx
-Version: 0.9.3
+Version: 0.9.4
 Summary: Jupyter Notebook Tools for Sphinx
 Home-page: https://nbsphinx.readthedocs.io/
 Author: Matthias Geier
 Author-email: Matthias.Geier@gmail.com
 License: MIT
 Project-URL: Documentation, https://nbsphinx.readthedocs.io/
 Project-URL: Source Code, https://github.com/spatialaudio/nbsphinx/
@@ -19,14 +19,20 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Documentation :: Sphinx
 Requires-Python: >=3.6
 License-File: LICENSE
+Requires-Dist: docutils>=0.18.1
+Requires-Dist: jinja2
+Requires-Dist: nbconvert!=5.4,>=5.3
+Requires-Dist: traitlets>=5
+Requires-Dist: nbformat
+Requires-Dist: sphinx>=1.8
 
 Jupyter Notebook Tools for Sphinx
 =================================
 
 ``nbsphinx`` is a Sphinx_ extension that provides a source parser for
 ``*.ipynb`` files.
 Custom Sphinx directives are used to show `Jupyter Notebook`_ code cells (and of
```

### Comparing `nbsphinx-0.9.3/src/nbsphinx.egg-info/SOURCES.txt` & `nbsphinx-0.9.4/src/nbsphinx.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,57 @@
 CONTRIBUTING.rst
 LICENSE
 MANIFEST.in
 NEWS.rst
 README.rst
 pyproject.toml
 setup.py
+doc/a-markdown-file.md
 doc/a-normal-rst-file.rst
 doc/allow-errors-per-cell.ipynb
 doc/allow-errors.ipynb
 doc/code-cells.ipynb
 doc/conf.py
 doc/configuration.ipynb
 doc/configuring-kernels.ipynb
 doc/contributing.rst
 doc/custom-css.ipynb
+doc/custom-formats.pct.py
 doc/executing-notebooks.ipynb
+doc/fallback_theme.txt
+doc/favicon.svg
 doc/hidden-cells.ipynb
 doc/index.rst
 doc/installation.ipynb
 doc/links.ipynb
 doc/markdown-cells.ipynb
+doc/matplotlibrc
 doc/never-execute.ipynb
 doc/orphan.ipynb
 doc/pre-executed.ipynb
 doc/prolog-and-epilog.ipynb
 doc/raw-cells.ipynb
 doc/references.bib
 doc/references.rst
 doc/requirements.txt
 doc/timeout.ipynb
 doc/usage.ipynb
 doc/version-history.rst
 doc/yet-another.ipynb
+doc/gallery/cell-metadata.ipynb
+doc/gallery/cell-tag.ipynb
+doc/gallery/default-thumbnail.ipynb
+doc/gallery/due-rst.pct.py
+doc/gallery/gallery-with-links.ipynb
+doc/gallery/gallery-with-nested-documents.ipynb
+doc/gallery/matplotlibrc
+doc/gallery/multiple-outputs.ipynb
+doc/gallery/no-thumbnail.ipynb
+doc/gallery/thumbnail-from-conf-py.ipynb
+doc/gallery/uno-rst.ipynb
 doc/images/notebook_icon.png
 doc/images/python_logo.svg
 doc/images/raw_cells_jupyter_notebook.png
 doc/images/raw_cells_jupyterlab.png
 doc/subdir/a-notebook-in-a-subdir.ipynb
 doc/subdir/gallery.ipynb
 doc/subdir/toctree.ipynb
```

