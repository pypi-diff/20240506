# Comparing `tmp/stsci.skypac-1.0.8.tar.gz` & `tmp/stsci.skypac-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/stsci.skypac-1.0.8.tar", last modified: Thu Aug 12 16:58:00 2021, max compression
+gzip compressed data, was "stsci.skypac-1.0.9.tar", last modified: Fri Apr 22 23:33:58 2022, max compression
```

## Comparing `stsci.skypac-1.0.8.tar` & `stsci.skypac-1.0.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-12 16:58:00.000000 stsci.skypac-1.0.8/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-12 16:58:00.000000 stsci.skypac-1.0.8/stsci.skypac.egg-info/
--rw-r--r--   0 root         (0) root         (0)        6 2021-08-12 16:58:00.000000 stsci.skypac-1.0.8/stsci.skypac.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      359 2021-08-12 16:58:00.000000 stsci.skypac-1.0.8/stsci.skypac.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1490 2021-08-12 16:58:00.000000 stsci.skypac-1.0.8/stsci.skypac.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2021-08-12 16:58:00.000000 stsci.skypac-1.0.8/stsci.skypac.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1040 2021-08-12 16:58:00.000000 stsci.skypac-1.0.8/stsci.skypac.egg-info/SOURCES.txt
--rwxr-xr-x   0 root         (0) root         (0)     3172 2021-08-12 16:57:15.000000 stsci.skypac-1.0.8/setup.py
--rw-r--r--   0 root         (0) root         (0)      496 2021-08-12 16:57:15.000000 stsci.skypac-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)     3207 2021-08-12 16:57:15.000000 stsci.skypac-1.0.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)      176 2021-08-12 16:57:15.000000 stsci.skypac-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1490 2021-08-12 16:58:00.000000 stsci.skypac-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1557 2021-08-12 16:57:15.000000 stsci.skypac-1.0.8/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      522 2021-08-12 16:57:15.000000 stsci.skypac-1.0.8/.gitignore
--rw-r--r--   0 root         (0) root         (0)       82 2021-08-12 16:57:15.000000 stsci.skypac-1.0.8/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-12 16:58:00.000000 stsci.skypac-1.0.8/stsci/
--rw-r--r--   0 root         (0) root         (0)      476 2021-08-12 16:57:15.000000 stsci.skypac-1.0.8/stsci/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-12 16:58:00.000000 stsci.skypac-1.0.8/stsci/skypac/
--rw-r--r--   0 root         (0) root         (0)    77162 2021-08-12 16:57:15.000000 stsci.skypac-1.0.8/stsci/skypac/parseat.py
--rw-r--r--   0 root         (0) root         (0)     2999 2021-08-12 16:57:15.000000 stsci.skypac-1.0.8/stsci/skypac/skystatistics.py
--rw-r--r--   0 root         (0) root         (0)    72994 2021-08-12 16:57:15.000000 stsci.skypac-1.0.8/stsci/skypac/skymatch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-12 16:58:00.000000 stsci.skypac-1.0.8/stsci/skypac/pars/
--rw-r--r--   0 root         (0) root         (0)     2363 2021-08-12 16:57:15.000000 stsci.skypac-1.0.8/stsci/skypac/pars/skymatch.cfgspc
--rw-r--r--   0 root         (0) root         (0)      397 2021-08-12 16:57:15.000000 stsci.skypac-1.0.8/stsci/skypac/pars/skymatch.cfg
--rw-r--r--   0 root         (0) root         (0)      997 2021-08-12 16:57:15.000000 stsci.skypac-1.0.8/stsci/skypac/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26755 2021-08-12 16:57:15.000000 stsci.skypac-1.0.8/stsci/skypac/skymatch.help
--rwxr-xr-x   0 root         (0) root         (0)    82337 2021-08-12 16:57:15.000000 stsci.skypac-1.0.8/stsci/skypac/utils.py
--rwxr-xr-x   0 root         (0) root         (0)    10798 2021-08-12 16:57:15.000000 stsci.skypac-1.0.8/stsci/skypac/pamutils.py
--rwxr-xr-x   0 root         (0) root         (0)    47144 2021-08-12 16:57:15.000000 stsci.skypac-1.0.8/stsci/skypac/skyline.py
--rwxr-xr-x   0 root         (0) root         (0)    13595 2021-08-12 16:57:15.000000 stsci.skypac-1.0.8/stsci/skypac/region.py
--rw-r--r--   0 root         (0) root         (0)      777 2021-08-12 16:57:15.000000 stsci.skypac-1.0.8/stsci/skypac/hstinfo.py
--rw-r--r--   0 root         (0) root         (0)       79 2021-08-12 16:57:15.000000 stsci.skypac-1.0.8/.readthedocs.yml
--rw-r--r--   0 root         (0) root         (0)     3135 2021-08-12 16:57:15.000000 stsci.skypac-1.0.8/Jenkinsfile
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-12 16:58:00.000000 stsci.skypac-1.0.8/docs/
--rw-r--r--   0 root         (0) root         (0)     5694 2021-08-12 16:57:15.000000 stsci.skypac-1.0.8/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-12 16:58:00.000000 stsci.skypac-1.0.8/docs/_static/
--rw-r--r--   0 root         (0) root         (0)    65413 2021-08-12 16:57:15.000000 stsci.skypac-1.0.8/docs/_static/stsci_pri_combo_mark_white.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-12 16:58:00.000000 stsci.skypac-1.0.8/docs/_static/css/
--rw-r--r--   0 root         (0) root         (0)   122264 2021-08-12 16:57:15.000000 stsci.skypac-1.0.8/docs/_static/css/custom.css
--rw-r--r--   0 root         (0) root         (0)      364 2021-08-12 16:57:15.000000 stsci.skypac-1.0.8/docs/.rtd-environment.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-12 16:58:00.000000 stsci.skypac-1.0.8/docs/source/
--rw-r--r--   0 root         (0) root         (0)       56 2021-08-12 16:57:15.000000 stsci.skypac-1.0.8/docs/source/LICENSE.rst
--rwxr-xr-x   0 root         (0) root         (0)      443 2021-08-12 16:57:15.000000 stsci.skypac-1.0.8/docs/source/skyline.rst
--rw-r--r--   0 root         (0) root         (0)      309 2021-08-12 16:57:15.000000 stsci.skypac-1.0.8/docs/source/index.rst
--rw-r--r--   0 root         (0) root         (0)      255 2021-08-12 16:57:15.000000 stsci.skypac-1.0.8/docs/source/pamutils.rst
--rwxr-xr-x   0 root         (0) root         (0)      234 2021-08-12 16:57:15.000000 stsci.skypac-1.0.8/docs/source/region.rst
--rwxr-xr-x   0 root         (0) root         (0)      319 2021-08-12 16:57:15.000000 stsci.skypac-1.0.8/docs/source/parseat.rst
--rw-r--r--   0 root         (0) root         (0)    13910 2021-08-12 16:57:15.000000 stsci.skypac-1.0.8/docs/source/conf.py
--rwxr-xr-x   0 root         (0) root         (0)      222 2021-08-12 16:57:15.000000 stsci.skypac-1.0.8/docs/source/utils.rst
--rw-r--r--   0 root         (0) root         (0)      349 2021-08-12 16:57:15.000000 stsci.skypac-1.0.8/docs/source/skymatch.rst
--rwxr-xr-x   0 root         (0) root         (0)      297 2021-08-12 16:57:15.000000 stsci.skypac-1.0.8/docs/source/skystatistics.rst
--rw-r--r--   0 root         (0) root         (0)     3165 2021-08-12 16:57:15.000000 stsci.skypac-1.0.8/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-12 16:58:00.000000 stsci.skypac-1.0.8/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-12 16:58:00.000000 stsci.skypac-1.0.8/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      855 2021-08-12 16:57:15.000000 stsci.skypac-1.0.8/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 root         (0) root         (0)     1068 2021-08-12 16:58:00.000000 stsci.skypac-1.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-22 23:33:58.140139 stsci.skypac-1.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-22 23:33:58.136139 stsci.skypac-1.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-22 23:33:58.140139 stsci.skypac-1.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)      681 2022-04-22 23:33:44.000000 stsci.skypac-1.0.9/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      522 2022-04-22 23:33:44.000000 stsci.skypac-1.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-04-22 23:33:44.000000 stsci.skypac-1.0.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     3207 2022-04-22 23:33:44.000000 stsci.skypac-1.0.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     3135 2022-04-22 23:33:44.000000 stsci.skypac-1.0.9/Jenkinsfile
+-rw-r--r--   0 runner    (1001) docker     (121)     1557 2022-04-22 23:33:44.000000 stsci.skypac-1.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      176 2022-04-22 23:33:44.000000 stsci.skypac-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-04-22 23:33:58.140139 stsci.skypac-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      496 2022-04-22 23:33:44.000000 stsci.skypac-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-22 23:33:58.140139 stsci.skypac-1.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      364 2022-04-22 23:33:44.000000 stsci.skypac-1.0.9/docs/.rtd-environment.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     5694 2022-04-22 23:33:44.000000 stsci.skypac-1.0.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-22 23:33:58.140139 stsci.skypac-1.0.9/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-22 23:33:58.140139 stsci.skypac-1.0.9/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (121)   122264 2022-04-22 23:33:44.000000 stsci.skypac-1.0.9/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (121)    65413 2022-04-22 23:33:44.000000 stsci.skypac-1.0.9/docs/_static/stsci_pri_combo_mark_white.png
+-rw-r--r--   0 runner    (1001) docker     (121)     3165 2022-04-22 23:33:44.000000 stsci.skypac-1.0.9/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-22 23:33:58.140139 stsci.skypac-1.0.9/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (121)       56 2022-04-22 23:33:44.000000 stsci.skypac-1.0.9/docs/source/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    13910 2022-04-22 23:33:44.000000 stsci.skypac-1.0.9/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      309 2022-04-22 23:33:44.000000 stsci.skypac-1.0.9/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      255 2022-04-22 23:33:44.000000 stsci.skypac-1.0.9/docs/source/pamutils.rst
+-rwxr-xr-x   0 runner    (1001) docker     (121)      319 2022-04-22 23:33:44.000000 stsci.skypac-1.0.9/docs/source/parseat.rst
+-rwxr-xr-x   0 runner    (1001) docker     (121)      234 2022-04-22 23:33:44.000000 stsci.skypac-1.0.9/docs/source/region.rst
+-rwxr-xr-x   0 runner    (1001) docker     (121)      443 2022-04-22 23:33:44.000000 stsci.skypac-1.0.9/docs/source/skyline.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      349 2022-04-22 23:33:44.000000 stsci.skypac-1.0.9/docs/source/skymatch.rst
+-rwxr-xr-x   0 runner    (1001) docker     (121)      297 2022-04-22 23:33:44.000000 stsci.skypac-1.0.9/docs/source/skystatistics.rst
+-rwxr-xr-x   0 runner    (1001) docker     (121)      222 2022-04-22 23:33:44.000000 stsci.skypac-1.0.9/docs/source/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       82 2022-04-22 23:33:44.000000 stsci.skypac-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-04-22 23:33:58.144140 stsci.skypac-1.0.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3172 2022-04-22 23:33:44.000000 stsci.skypac-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-22 23:33:58.140139 stsci.skypac-1.0.9/stsci/
+-rw-r--r--   0 runner    (1001) docker     (121)      476 2022-04-22 23:33:44.000000 stsci.skypac-1.0.9/stsci/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-22 23:33:58.140139 stsci.skypac-1.0.9/stsci/skypac/
+-rw-r--r--   0 runner    (1001) docker     (121)      997 2022-04-22 23:33:44.000000 stsci.skypac-1.0.9/stsci/skypac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      777 2022-04-22 23:33:44.000000 stsci.skypac-1.0.9/stsci/skypac/hstinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    10798 2022-04-22 23:33:44.000000 stsci.skypac-1.0.9/stsci/skypac/pamutils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-22 23:33:58.140139 stsci.skypac-1.0.9/stsci/skypac/pars/
+-rw-r--r--   0 runner    (1001) docker     (121)      397 2022-04-22 23:33:44.000000 stsci.skypac-1.0.9/stsci/skypac/pars/skymatch.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2363 2022-04-22 23:33:44.000000 stsci.skypac-1.0.9/stsci/skypac/pars/skymatch.cfgspc
+-rw-r--r--   0 runner    (1001) docker     (121)    77162 2022-04-22 23:33:44.000000 stsci.skypac-1.0.9/stsci/skypac/parseat.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    13595 2022-04-22 23:33:44.000000 stsci.skypac-1.0.9/stsci/skypac/region.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    47144 2022-04-22 23:33:44.000000 stsci.skypac-1.0.9/stsci/skypac/skyline.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26755 2022-04-22 23:33:44.000000 stsci.skypac-1.0.9/stsci/skypac/skymatch.help
+-rw-r--r--   0 runner    (1001) docker     (121)    72994 2022-04-22 23:33:44.000000 stsci.skypac-1.0.9/stsci/skypac/skymatch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2999 2022-04-22 23:33:44.000000 stsci.skypac-1.0.9/stsci/skypac/skystatistics.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    82337 2022-04-22 23:33:44.000000 stsci.skypac-1.0.9/stsci/skypac/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-22 23:33:58.140139 stsci.skypac-1.0.9/stsci.skypac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-04-22 23:33:57.000000 stsci.skypac-1.0.9/stsci.skypac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1040 2022-04-22 23:33:58.000000 stsci.skypac-1.0.9/stsci.skypac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-22 23:33:57.000000 stsci.skypac-1.0.9/stsci.skypac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      359 2022-04-22 23:33:57.000000 stsci.skypac-1.0.9/stsci.skypac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-04-22 23:33:58.000000 stsci.skypac-1.0.9/stsci.skypac.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `stsci.skypac-1.0.8/stsci.skypac.egg-info/PKG-INFO` & `stsci.skypac-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stsci.skypac
-Version: 1.0.8
+Version: 1.0.9
 Summary: Sky matching on image mosaic
 Home-page: https://github.com/spacetelescope/stsci.skypac
 Author: Mihai Cara, Warren Hack, Pey Lian Lim
 Author-email: help@stsci.edu
 License: BSD-3-Clause
 Project-URL: Bug Reports, https://github.com/spacetelescope/stsci.skypac/issues/
 Project-URL: Source, https://github.com/spacetelescope/stsci.skypac/
```

### Comparing `stsci.skypac-1.0.8/stsci.skypac.egg-info/SOURCES.txt` & `stsci.skypac-1.0.9/stsci.skypac.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stsci.skypac-1.0.8/setup.py` & `stsci.skypac-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `stsci.skypac-1.0.8/CODE_OF_CONDUCT.md` & `stsci.skypac-1.0.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `stsci.skypac-1.0.8/PKG-INFO` & `stsci.skypac-1.0.9/stsci.skypac.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stsci.skypac
-Version: 1.0.8
+Version: 1.0.9
 Summary: Sky matching on image mosaic
 Home-page: https://github.com/spacetelescope/stsci.skypac
 Author: Mihai Cara, Warren Hack, Pey Lian Lim
 Author-email: help@stsci.edu
 License: BSD-3-Clause
 Project-URL: Bug Reports, https://github.com/spacetelescope/stsci.skypac/issues/
 Project-URL: Source, https://github.com/spacetelescope/stsci.skypac/
```

### Comparing `stsci.skypac-1.0.8/LICENSE.txt` & `stsci.skypac-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stsci.skypac-1.0.8/.gitignore` & `stsci.skypac-1.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `stsci.skypac-1.0.8/stsci/skypac/parseat.py` & `stsci.skypac-1.0.9/stsci/skypac/parseat.py`

 * *Files identical despite different names*

### Comparing `stsci.skypac-1.0.8/stsci/skypac/skystatistics.py` & `stsci.skypac-1.0.9/stsci/skypac/skystatistics.py`

 * *Files identical despite different names*

### Comparing `stsci.skypac-1.0.8/stsci/skypac/skymatch.py` & `stsci.skypac-1.0.9/stsci/skypac/skymatch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1317,15 +1317,15 @@
     t_wght2 = 0
     area = 0.0
 
     for m1 in s1.members:
         for m2 in s2.members:
             pts1 = np.sort(list(m1.polygon.points)[0], axis=0)
             pts2 = np.sort(list(m2.polygon.points)[0], axis=0)
-            if np.allclose(pts1, pts2, rtol=0, atol=5e-9):
+            if np.allclose(pts1, pts2, rtol=0, atol=1e-8):
                 intersect_poly = m1.polygon.copy()
             else:
                 intersect_poly = m1.polygon.intersection(m2.polygon)
 
             # Check if we even have regions that potentially may have an area.
             # This is done mostly to make sure tha code that follows does
             # not crash when no "good" polygons are available.
```

### Comparing `stsci.skypac-1.0.8/stsci/skypac/pars/skymatch.cfgspc` & `stsci.skypac-1.0.9/stsci/skypac/pars/skymatch.cfgspc`

 * *Files identical despite different names*

### Comparing `stsci.skypac-1.0.8/stsci/skypac/__init__.py` & `stsci.skypac-1.0.9/stsci/skypac/__init__.py`

 * *Files identical despite different names*

### Comparing `stsci.skypac-1.0.8/stsci/skypac/skymatch.help` & `stsci.skypac-1.0.9/stsci/skypac/skymatch.help`

 * *Files identical despite different names*

### Comparing `stsci.skypac-1.0.8/stsci/skypac/utils.py` & `stsci.skypac-1.0.9/stsci/skypac/utils.py`

 * *Files identical despite different names*

### Comparing `stsci.skypac-1.0.8/stsci/skypac/pamutils.py` & `stsci.skypac-1.0.9/stsci/skypac/pamutils.py`

 * *Files identical despite different names*

### Comparing `stsci.skypac-1.0.8/stsci/skypac/skyline.py` & `stsci.skypac-1.0.9/stsci/skypac/skyline.py`

 * *Files identical despite different names*

### Comparing `stsci.skypac-1.0.8/stsci/skypac/region.py` & `stsci.skypac-1.0.9/stsci/skypac/region.py`

 * *Files identical despite different names*

### Comparing `stsci.skypac-1.0.8/stsci/skypac/hstinfo.py` & `stsci.skypac-1.0.9/stsci/skypac/hstinfo.py`

 * *Files identical despite different names*

### Comparing `stsci.skypac-1.0.8/Jenkinsfile` & `stsci.skypac-1.0.9/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `stsci.skypac-1.0.8/docs/Makefile` & `stsci.skypac-1.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `stsci.skypac-1.0.8/docs/_static/stsci_pri_combo_mark_white.png` & `stsci.skypac-1.0.9/docs/_static/stsci_pri_combo_mark_white.png`

 * *Files identical despite different names*

### Comparing `stsci.skypac-1.0.8/docs/_static/css/custom.css` & `stsci.skypac-1.0.9/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `stsci.skypac-1.0.8/docs/source/conf.py` & `stsci.skypac-1.0.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `stsci.skypac-1.0.8/docs/make.bat` & `stsci.skypac-1.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `stsci.skypac-1.0.8/setup.cfg` & `stsci.skypac-1.0.9/setup.cfg`

 * *Files identical despite different names*

