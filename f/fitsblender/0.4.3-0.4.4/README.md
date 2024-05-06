# Comparing `tmp/fitsblender-0.4.3.tar.gz` & `tmp/fitsblender-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fitsblender-0.4.3.tar", last modified: Tue Sep  6 20:44:50 2022, max compression
+gzip compressed data, was "fitsblender-0.4.4.tar", last modified: Mon May  6 19:20:33 2024, max compression
```

## Comparing `fitsblender-0.4.3.tar` & `fitsblender-0.4.4.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 20:44:50.347373 fitsblender-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-09-06 20:44:40.000000 fitsblender-0.4.3/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 20:44:50.343373 fitsblender-0.4.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 20:44:50.343373 fitsblender-0.4.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2470 2022-09-06 20:44:40.000000 fitsblender-0.4.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-09-06 20:44:40.000000 fitsblender-0.4.3/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-09-06 20:44:40.000000 fitsblender-0.4.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     3207 2022-09-06 20:44:40.000000 fitsblender-0.4.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1560 2022-09-06 20:44:40.000000 fitsblender-0.4.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1388 2022-09-06 20:44:50.347373 fitsblender-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      748 2022-09-06 20:44:40.000000 fitsblender-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      701 2022-09-06 20:44:40.000000 fitsblender-0.4.3/azure-pipelines.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 20:44:50.343373 fitsblender-0.4.3/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     3140 2022-09-06 20:44:40.000000 fitsblender-0.4.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 20:44:50.343373 fitsblender-0.4.3/docs/source/
--rw-r--r--   0 runner    (1001) docker     (121)     6665 2022-09-06 20:44:40.000000 fitsblender-0.4.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      450 2022-09-06 20:44:40.000000 fitsblender-0.4.3/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 20:44:50.343373 fitsblender-0.4.3/fitsblender/
--rw-r--r--   0 runner    (1001) docker     (121)     2158 2022-09-06 20:44:40.000000 fitsblender-0.4.3/fitsblender/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8764 2022-09-06 20:44:40.000000 fitsblender-0.4.3/fitsblender/acs_header.rules
--rw-r--r--   0 runner    (1001) docker     (121)     9872 2022-09-06 20:44:40.000000 fitsblender-0.4.3/fitsblender/blender.py
--rw-r--r--   0 runner    (1001) docker     (121)    38589 2022-09-06 20:44:40.000000 fitsblender-0.4.3/fitsblender/blendheaders.py
--rw-r--r--   0 runner    (1001) docker     (121)     9018 2022-09-06 20:44:40.000000 fitsblender-0.4.3/fitsblender/hst_header.rules
--rw-r--r--   0 runner    (1001) docker     (121)     8473 2022-09-06 20:44:40.000000 fitsblender-0.4.3/fitsblender/jwst_header.rules
--rw-r--r--   0 runner    (1001) docker     (121)    10623 2022-09-06 20:44:40.000000 fitsblender-0.4.3/fitsblender/nicmos_header.rules
--rw-r--r--   0 runner    (1001) docker     (121)     8476 2022-09-06 20:44:40.000000 fitsblender-0.4.3/fitsblender/nircam_header.rules
--rw-r--r--   0 runner    (1001) docker     (121)     8264 2022-09-06 20:44:40.000000 fitsblender-0.4.3/fitsblender/nirspec_header.rules
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 20:44:50.347373 fitsblender-0.4.3/fitsblender/pars/
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-09-06 20:44:40.000000 fitsblender-0.4.3/fitsblender/pars/blendheaders.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      621 2022-09-06 20:44:40.000000 fitsblender-0.4.3/fitsblender/pars/blendheaders.cfgspc
--rw-r--r--   0 runner    (1001) docker     (121)    10621 2022-09-06 20:44:40.000000 fitsblender-0.4.3/fitsblender/stis_header.rules
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 20:44:50.347373 fitsblender-0.4.3/fitsblender/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     5760 2022-09-06 20:44:40.000000 fitsblender-0.4.3/fitsblender/tests/EUVEngc4151imgx.fits
--rw-r--r--   0 runner    (1001) docker     (121)    20160 2022-09-06 20:44:40.000000 fitsblender-0.4.3/fitsblender/tests/FGSf64y0106m_a1f.fits
--rw-r--r--   0 runner    (1001) docker     (121)    14400 2022-09-06 20:44:40.000000 fitsblender-0.4.3/fitsblender/tests/FOSy19g0309t_c2f.fits
--rw-r--r--   0 runner    (1001) docker     (121)    20160 2022-09-06 20:44:40.000000 fitsblender-0.4.3/fitsblender/tests/HRSz0yd020fm_c2f.fits
--rw-r--r--   0 runner    (1001) docker     (121)    28800 2022-09-06 20:44:40.000000 fitsblender-0.4.3/fitsblender/tests/IUElwp25637mxlo.fits
--rw-r--r--   0 runner    (1001) docker     (121)    20160 2022-09-06 20:44:40.000000 fitsblender-0.4.3/fitsblender/tests/NICMOSn4hk12010_mos.fits
--rw-r--r--   0 runner    (1001) docker     (121)    11520 2022-09-06 20:44:40.000000 fitsblender-0.4.3/fitsblender/tests/UITfuv2582gc.fits
--rw-r--r--   0 runner    (1001) docker     (121)    23040 2022-09-06 20:44:40.000000 fitsblender-0.4.3/fitsblender/tests/WFPC2ASSNu5780205bx.fits
--rw-r--r--   0 runner    (1001) docker     (121)    23040 2022-09-06 20:44:40.000000 fitsblender-0.4.3/fitsblender/tests/WFPC2u5780205r_c0fx.fits
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-06 20:44:40.000000 fitsblender-0.4.3/fitsblender/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4222 2022-09-06 20:44:40.000000 fitsblender-0.4.3/fitsblender/tests/test_fitsblender.py
--rw-r--r--   0 runner    (1001) docker     (121)    10621 2022-09-06 20:44:40.000000 fitsblender-0.4.3/fitsblender/wfc3_header.rules
--rw-r--r--   0 runner    (1001) docker     (121)    10616 2022-09-06 20:44:40.000000 fitsblender-0.4.3/fitsblender/wfpc2_header.rules
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 20:44:50.347373 fitsblender-0.4.3/fitsblender.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1388 2022-09-06 20:44:50.000000 fitsblender-0.4.3/fitsblender.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1271 2022-09-06 20:44:50.000000 fitsblender-0.4.3/fitsblender.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-06 20:44:50.000000 fitsblender-0.4.3/fitsblender.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-09-06 20:44:50.000000 fitsblender-0.4.3/fitsblender.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-09-06 20:44:50.000000 fitsblender-0.4.3/fitsblender.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-09-06 20:44:40.000000 fitsblender-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      998 2022-09-06 20:44:50.347373 fitsblender-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1414 2022-09-06 20:44:40.000000 fitsblender-0.4.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      794 2022-09-06 20:44:40.000000 fitsblender-0.4.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:20:33.658509 fitsblender-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-06 19:20:21.000000 fitsblender-0.4.4/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-06 19:20:21.000000 fitsblender-0.4.4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:20:33.650508 fitsblender-0.4.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-06 19:20:21.000000 fitsblender-0.4.4/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:20:33.650508 fitsblender-0.4.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-06 19:20:21.000000 fitsblender-0.4.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-06 19:20:21.000000 fitsblender-0.4.4/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-06 19:20:21.000000 fitsblender-0.4.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-06 19:20:21.000000 fitsblender-0.4.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-06 19:20:21.000000 fitsblender-0.4.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-06 19:20:33.658509 fitsblender-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-06 19:20:21.000000 fitsblender-0.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-06 19:20:21.000000 fitsblender-0.4.4/azure-pipelines.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:20:33.650508 fitsblender-0.4.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-06 19:20:21.000000 fitsblender-0.4.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:20:33.650508 fitsblender-0.4.4/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-05-06 19:20:21.000000 fitsblender-0.4.4/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-06 19:20:21.000000 fitsblender-0.4.4/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:20:33.654509 fitsblender-0.4.4/fitsblender/
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-06 19:20:21.000000 fitsblender-0.4.4/fitsblender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8798 2024-05-06 19:20:21.000000 fitsblender-0.4.4/fitsblender/acs_header.rules
+-rw-r--r--   0 runner    (1001) docker     (127)     9872 2024-05-06 19:20:21.000000 fitsblender-0.4.4/fitsblender/blender.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38758 2024-05-06 19:20:21.000000 fitsblender-0.4.4/fitsblender/blendheaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9018 2024-05-06 19:20:21.000000 fitsblender-0.4.4/fitsblender/hst_header.rules
+-rw-r--r--   0 runner    (1001) docker     (127)     8473 2024-05-06 19:20:21.000000 fitsblender-0.4.4/fitsblender/jwst_header.rules
+-rw-r--r--   0 runner    (1001) docker     (127)    10623 2024-05-06 19:20:21.000000 fitsblender-0.4.4/fitsblender/nicmos_header.rules
+-rw-r--r--   0 runner    (1001) docker     (127)     8476 2024-05-06 19:20:21.000000 fitsblender-0.4.4/fitsblender/nircam_header.rules
+-rw-r--r--   0 runner    (1001) docker     (127)     8264 2024-05-06 19:20:21.000000 fitsblender-0.4.4/fitsblender/nirspec_header.rules
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:20:33.654509 fitsblender-0.4.4/fitsblender/pars/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-06 19:20:21.000000 fitsblender-0.4.4/fitsblender/pars/blendheaders.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-06 19:20:21.000000 fitsblender-0.4.4/fitsblender/pars/blendheaders.cfgspc
+-rw-r--r--   0 runner    (1001) docker     (127)    10621 2024-05-06 19:20:21.000000 fitsblender-0.4.4/fitsblender/stis_header.rules
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:20:33.658509 fitsblender-0.4.4/fitsblender/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-05-06 19:20:21.000000 fitsblender-0.4.4/fitsblender/tests/EUVEngc4151imgx.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    20160 2024-05-06 19:20:21.000000 fitsblender-0.4.4/fitsblender/tests/FGSf64y0106m_a1f.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    14400 2024-05-06 19:20:21.000000 fitsblender-0.4.4/fitsblender/tests/FOSy19g0309t_c2f.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    20160 2024-05-06 19:20:21.000000 fitsblender-0.4.4/fitsblender/tests/HRSz0yd020fm_c2f.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    28800 2024-05-06 19:20:21.000000 fitsblender-0.4.4/fitsblender/tests/IUElwp25637mxlo.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    20160 2024-05-06 19:20:21.000000 fitsblender-0.4.4/fitsblender/tests/NICMOSn4hk12010_mos.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    11520 2024-05-06 19:20:21.000000 fitsblender-0.4.4/fitsblender/tests/UITfuv2582gc.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    23040 2024-05-06 19:20:21.000000 fitsblender-0.4.4/fitsblender/tests/WFPC2ASSNu5780205bx.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    23040 2024-05-06 19:20:21.000000 fitsblender-0.4.4/fitsblender/tests/WFPC2u5780205r_c0fx.fits
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:20:21.000000 fitsblender-0.4.4/fitsblender/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-05-06 19:20:21.000000 fitsblender-0.4.4/fitsblender/tests/test_fitsblender.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10659 2024-05-06 19:20:21.000000 fitsblender-0.4.4/fitsblender/wfc3_header.rules
+-rw-r--r--   0 runner    (1001) docker     (127)    10616 2024-05-06 19:20:21.000000 fitsblender-0.4.4/fitsblender/wfpc2_header.rules
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:20:33.658509 fitsblender-0.4.4/fitsblender.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-06 19:20:33.000000 fitsblender-0.4.4/fitsblender.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-06 19:20:33.000000 fitsblender-0.4.4/fitsblender.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 19:20:33.000000 fitsblender-0.4.4/fitsblender.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-06 19:20:33.000000 fitsblender-0.4.4/fitsblender.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-06 19:20:33.000000 fitsblender-0.4.4/fitsblender.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-06 19:20:21.000000 fitsblender-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-06 19:20:21.000000 fitsblender-0.4.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 19:20:33.658509 fitsblender-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-06 19:20:21.000000 fitsblender-0.4.4/tox.ini
```

### Comparing `fitsblender-0.4.3/CODE_OF_CONDUCT.md` & `fitsblender-0.4.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `fitsblender-0.4.3/LICENSE.txt` & `fitsblender-0.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fitsblender-0.4.3/README.md` & `fitsblender-0.4.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # fitsblender
 
-[![Build Status](https://dev.azure.com/spacetelescope/fitsblender/_apis/build/status/spacetelescope.fitsblender?branchName=master)](https://dev.azure.com/spacetelescope/fitsblender/_build/latest?definitionId=14&branchName=master)
-[![codecov](https://codecov.io/gh/spacetelescope/fitsblender/branch/master/graph/badge.svg)](https://codecov.io/gh/spacetelescope/fitsblender)
+[![Build Status](https://dev.azure.com/spacetelescope/fitsblender/_apis/build/status/spacetelescope.fitsblender?branchName=main)](https://dev.azure.com/spacetelescope/fitsblender/_build/latest?definitionId=14&branchName=main)
+[![codecov](https://codecov.io/gh/spacetelescope/fitsblender/branch/main/graph/badge.svg)](https://codecov.io/gh/spacetelescope/fitsblender)
 
 FITSBLENDER
 ============
 
 This package supports the creation of a combined header for a FITS file based on the contents of the headers
 of a set of input FITS images.  A rules file defines what keywords will be present in the combined
 output header as well as how the output value will be determined from the set of values from all
```

### Comparing `fitsblender-0.4.3/docs/Makefile` & `fitsblender-0.4.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fitsblender-0.4.3/docs/source/conf.py` & `fitsblender-0.4.4/docs/source/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,20 @@
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
 import os
 import sys
 
+# The version info for the project you're documenting, acts as replacement for
+# |version| and |release|, also used in various other places throughout the
+# built documents.
+
+from fitsblender import __version__ as version
+
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 sys.path.insert(1, os.path.abspath('.'))
 sys.path.insert(1, os.path.abspath('..'))
 sys.path.insert(1, os.path.abspath(os.path.join('..', '..')))
 
@@ -31,173 +37,167 @@
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix of source filenames.
 source_suffix = '.rst'
 
 # The encoding of source files.
-#source_encoding = 'utf-8'
+# source_encoding = 'utf-8'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = u'fitsblender'
 copyright = u'2010, Michael Droettboom'
 
-# The version info for the project you're documenting, acts as replacement for
-# |version| and |release|, also used in various other places throughout the
-# built documents.
-
-from fitsblender import __version__ as VERSION
-# The short X.Y version.
-version = VERSION
+# The short X.Y `version`
 # The full version, including alpha/beta/rc tags.
 release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
-#language = None
+# language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
-#today = ''
+# today = ''
 # Else, today_fmt is used as the format for a strftime call.
-#today_fmt = '%B %d, %Y'
+# today_fmt = '%B %d, %Y'
 
 # List of documents that shouldn't be included in the build.
-#unused_docs = []
+# unused_docs = []
 
 # List of directories, relative to source directory, that shouldn't be searched
 # for source files.
 exclude_trees = []
 
 # The reST default role (used for this markup: `text`) to use for all documents.
-#default_role = None
+# default_role = None
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
-#add_function_parentheses = True
+# add_function_parentheses = True
 
 # If true, the current module name will be prepended to all description
 # unit titles (such as .. function::).
-#add_module_names = True
+# add_module_names = True
 
 # If true, sectionauthor and moduleauthor directives will be shown in the
 # output. They are ignored by default.
-#show_authors = False
+# show_authors = False
 
 # The name of the Pygments (syntax highlighting) style to use.
 pygments_style = 'sphinx'
 
 # A list of ignored prefixes for module index sorting.
-#modindex_common_prefix = []
+# modindex_common_prefix = []
 
 
 # -- Options for HTML output ---------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  Major themes that come with
 # Sphinx are currently 'default' and 'sphinxdoc'.
-#html_theme = 'default'
+# html_theme = 'default'
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
-#html_theme_options = {}
+# html_theme_options = {}
 
 # Add any paths that contain custom themes here, relative to this directory.
-#html_theme_path = []
+# html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
-#html_title = None
+# html_title = None
 
 # A shorter title for the navigation bar.  Default is the same as html_title.
-#html_short_title = None
+# html_short_title = None
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
-#html_logo = None
+# html_logo = None
 
 # The name of an image file (within the static path) to use as favicon of the
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
-#html_favicon = None
+# html_favicon = None
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-#html_static_path = ['_static']
+# html_static_path = ['_static']
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
 # using the given strftime format.
-#html_last_updated_fmt = '%b %d, %Y'
+# html_last_updated_fmt = '%b %d, %Y'
 
 # If true, SmartyPants will be used to convert quotes and dashes to
 # typographically correct entities.
-#html_use_smartypants = True
+# html_use_smartypants = True
 
 # Custom sidebar templates, maps document names to template names.
-#html_sidebars = {}
+# html_sidebars = {}
 
 # Additional templates that should be rendered to pages, maps page names to
 # template names.
-#html_additional_pages = {}
+# html_additional_pages = {}
 
 # If false, no module index is generated.
-#html_use_modindex = True
+# html_use_modindex = True
 
 # If false, no index is generated.
-#html_use_index = True
+# html_use_index = True
 
 # If true, the index is split into individual pages for each letter.
-#html_split_index = False
+# html_split_index = False
 
 # If true, links to the reST sources are added to the pages.
-#html_show_sourcelink = True
+# html_show_sourcelink = True
 
 # If true, an OpenSearch description file will be output, and all pages will
 # contain a <link> tag referring to it.  The value of this option must be the
 # base URL from which the finished HTML is served.
-#html_use_opensearch = ''
+# html_use_opensearch = ''
 
 # If nonempty, this is the file name suffix for HTML files (e.g. ".xhtml").
-#html_file_suffix = ''
+# html_file_suffix = ''
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = 'fitsblenderdoc'
 
 
 # -- Options for LaTeX output --------------------------------------------------
 
 # The paper size ('letter' or 'a4').
-#latex_paper_size = 'letter'
+# latex_paper_size = 'letter'
 
 # The font size ('10pt', '11pt' or '12pt').
-#latex_font_size = '10pt'
+# latex_font_size = '10pt'
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass [howto/manual]).
 latex_documents = [
   ('index', 'fitsblender.tex', u'fitsblender Documentation',
    u'Michael Droettboom', 'manual'),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
-#latex_logo = None
+# latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
 # not chapters.
-#latex_use_parts = False
+# latex_use_parts = False
 
 # Additional stuff for the LaTeX preamble.
-#latex_preamble = ''
+# latex_preamble = ''
 
 # Documents to append as an appendix to all manuals.
-#latex_appendices = []
+# latex_appendices = []
 
 # If false, no module index is generated.
-#latex_use_modindex = True
+# latex_use_modindex = True
 
 
 # Example configuration for intersphinx: refer to the Python standard library.
 # intersphinx_mapping = {'http://docs.python.org/': None}
```

### Comparing `fitsblender-0.4.3/fitsblender/__init__.py` & `fitsblender-0.4.4/fitsblender/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,19 +25,19 @@
 # ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR
 # TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE
 # USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH
 # DAMAGE.
 from __future__ import absolute_import
 import os
 import sys
+import importlib.metadata
 
-from pkg_resources import get_distribution, DistributionNotFound
 try:
-    __version__ = get_distribution(__name__).version
-except DistributionNotFound:
+    __version__ = importlib.metadata.version(__name__)
+except importlib.metadata.PackageNotFoundError:  # pragma: no cover
     # package is not installed
     __version__ = 'UNKNOWN'
 
 
 from . import blender
 from .blender import fitsblender
```

### Comparing `fitsblender-0.4.3/fitsblender/acs_header.rules` & `fitsblender-0.4.4/fitsblender/acs_header.rules`

 * *Files 0% similar despite different names*

```diff
@@ -313,14 +313,15 @@
 SDQFLAGS
 SHADCORR
 SHADFILE
 SHUTRPOS
 SIMPLE
 SIZAXIS1
 SIZAXIS2
+SKYCELL
 SKYSUB
 SKYSUM
 SNRMAX
 SNRMEAN
 SNRMIN
 SOFTERRS
 SPOTTAB
@@ -479,14 +480,15 @@
 READNSED  READNSED  first
 REJ_RATE  REJ_RATE  first
 SCALENSE  SCALENSE  first
 SCLAMP      SCLAMP    multi
 SHADCORR  SHADCORR  multi
 SHADFILE  SHADFILE  multi
 SHUTRPOS  SHUTRPOS  multi
+SKYCELL   SKYCELL   first
 SKYSUB      SKYSUB    multi
 SKYSUM      SKYSUM    sum
 SPOTTAB   SPOTTAB   multi
 SUBARRAY  SUBARRAY  first
 SUNANGLE  SUNANGLE  first
 SUN_ALT   SUN_ALT   first
 WRTERR      WRTERR    multi
```

### Comparing `fitsblender-0.4.3/fitsblender/blender.py` & `fitsblender-0.4.4/fitsblender/blender.py`

 * *Files identical despite different names*

### Comparing `fitsblender-0.4.3/fitsblender/blendheaders.py` & `fitsblender-0.4.4/fitsblender/blendheaders.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,17 @@
 # Version of rules file format supported by this version of the code
 # All changes should be backwards compatible to older rules versions
 # so any rules file with Version >= __rules_version__ should work with this code
 __rules_version__ = 1.1
 
 fits_required_bool_kws = ['SIMPLE', 'EXTEND']
 WCS_KEYWORDS = ['CD1_1', 'CD1_2', 'CD2_1', 'CD2_2', 'CRPIX1',
-              'CRPIX2', 'CRVAL1', 'CRVAL2', 'CTYPE1', 'CTYPE2',
-              'VAFACTOR', 'ORIENTAT', 'BUNIT', 'WCSNAME']
+                'CRPIX2', 'CRVAL1', 'CRVAL2', 'CTYPE1', 'CTYPE2',
+                'VAFACTOR', 'ORIENTAT', 'BUNIT', 'WCSNAME']
+
 
 #
 # Custom blending functions
 #
 def multi(vals):
     """
     This will either return the common value from a list of identical values
@@ -90,54 +91,55 @@
                  'sum': np.sum,
                  'max': np.max,
                  'min': np.min,
                  'stddev': np.std}
 
 delete_command = '<delete>'
 
+
 #
 #  TEAL Interfaces to run this task
 #
 def getHelpAsString(docstring=False):
     """
     return useful help from a file in the script directory called __taskname__.help
     """
     install_dir = os.path.dirname(__file__)
     htmlfile = os.path.join(install_dir, 'htmlhelp', __taskname__+'.html')
     helpfile = os.path.join(install_dir, __taskname__+'.help')
     if docstring or (not docstring and not os.path.exists(htmlfile)):
-        helpString = __taskname__+' Version '+__version__+' updated on '+__vdate__+'\n\n'
+        help_string = __taskname__+' Version '+__version__+' updated on '+__vdate__+'\n\n'
         if os.path.exists(helpfile):
-            helpString += teal.getHelpFileAsString(__taskname__, __file__)
+            help_string += teal.getHelpFileAsString(__taskname__, __file__)
         else:
-            helpString += blendheaders.__doc__
+            help_string += blendheaders.__doc__
     else:
-        helpString = 'file://'+htmlfile
+        help_string = 'file://'+htmlfile
 
-    return helpString
+    return help_string
 
 
 def run(configobj):
     # Interpret user-input from TEAL GUI and call function
     blendheaders(configobj['drzfile'],
-                inputs=configobj['inputs'],
-                output=configobj['output'],
-                sciext=configobj['sciext'],
-                errext=configobj['errext'],
-                dqext=configobj['dqext'],
-                verbose=configobj['verbose'])
+                 inputs=configobj['inputs'],
+                 output=configobj['output'],
+                 sciext=configobj['sciext'],
+                 errext=configobj['errext'],
+                 dqext=configobj['dqext'],
+                 verbose=configobj['verbose'])
 
 
 #
 #  Primary functional interface for the code
 #
 def blendheaders(drzfile, inputs=None, output=None,
-                extensions={'SCI':'SCI', 'ERR':'WHT', 'DQ':'CON'},
-                sciext='SCI', errext='ERR', dqext='DQ',
-                rules_file=None, verbose=False):
+                 extensions={'SCI': 'SCI', 'ERR': 'WHT', 'DQ': 'CON'},
+                 sciext='SCI', errext='ERR', dqext='DQ',
+                 rules_file=None, verbose=False):
     """ Blend headers that went into creating the original drzfile into a
     new header with table that contains keyword values from all input images.
 
     The drzfile will be used to determine the names of the input files, should
     no filenames be provided in the 'inputs' parameter.
 
     The drzfile will be updated 'in-place' with the new headers and table if
@@ -195,34 +197,37 @@
         Print out additional messages during processing when specified.
 
     """
     # interpret input
     drzfiles = parseinput.parseinput(drzfile)[0]
 
     ext_list = []
-    for e in extensions: ext_list.append(e)
+    for e in extensions:
+        ext_list.append(e)
 
     # operate on each drzfile specified
     for drzfile in drzfiles:
         if inputs in [None, '', ' ', 'INDEF', 'None']:
             inputs = extract_filenames_from_drz(drzfile)
 
         if verbose:
             print('Creating blended headers from: ')
-            for i in inputs: print('    ', i)
+            for i in inputs:
+                print('    ', i)
 
         newhdrs, newtab = get_blended_headers(inputs, verbose=verbose,
-                        extlist=ext_list, rules_file=rules_file)
+                                              extlist=ext_list,
+                                              rules_file=rules_file)
 
         # Remove distortion related keywords not included in rules
         for hdr in newhdrs:
             remove_distortion_keywords(hdr)
 
         # open drizzle product to update headers with new headers
-        open_mode='update'
+        open_mode = 'update'
         if output not in [None, '', ' ', 'INDEF', 'None']:
             open_mode = 'readonly'
         drzimg = fits.open(drzfile, mode=open_mode)
 
         # Determine whether we are working with a simple DRZ FITS file or
         # a full multi-extension DRZ FITS file.
         if len(drzimg) < 3:
@@ -292,20 +297,21 @@
 
         if 'nextend' in drzimg[0].header:
             drzimg[0].header['nextend'] = len(drzimg)-1
 
         # Write out the updated product
         if open_mode == 'update':
             drzimg.close()
-            print('Updated ',drzfile,' with blended headers.')
+            print('Updated ', drzfile, ' with blended headers.')
         else:
-            if os.path.exists(output): os.remove(output)
+            if os.path.exists(output):
+                os.remove(output)
             drzimg.writeto(output)
             drzimg.close()
-            print('Created new file ',output,' with blended headers.')
+            print('Created new file ', output, ' with blended headers.')
 
         # Clean up for the next run
         del drzimg, newhdrs, newtab
 
 
 def get_blended_headers(inputs, verbose=False, extlist=['SCI', 'ERR', 'DQ'], rules_file=None):
     """
@@ -366,15 +372,16 @@
             rname_kw = 'filename'
         rootname = inputs[0][rname_kw].strip()
         phdrdict[rootname] = inputs[0]
         hdrlist = inputs
 
     # create a list of unique PRIMARY headers for use later
     phdrlist = []
-    for name in phdrdict: phdrlist.append(phdrdict[name])
+    for name in phdrdict:
+        phdrlist.append(phdrdict[name])
 
     num_files = len(phdrlist)
 
     # Determine what blending rules need to be merged to create the final
     # blended headers. There will be a separate set of rules for each
     # instrument, and all rules get merged into a composite set of rules that
     # get applied to all input headers regardless of instrument.
@@ -383,21 +390,21 @@
     # the PRIMARY header of each input
     #
     icache = {}
     for i in range(num_files):
         ph = hdrlist[0][i]
         inst = ph['instrume'].lower()
         tel = ph['telescop'].lower()
-        hlist = [hdrlist[0][i],hdrlist[1][i],hdrlist[2][i],hdrlist[3][i]]
+        hlist = [hdrlist[0][i], hdrlist[1][i], hdrlist[2][i], hdrlist[3][i]]
         if inst not in icache:
             # initialize the appropriate class for this data's instrument
             inst_class = KeywordRules(inst, telescope=tel, rules_file=rules_file)
             if verbose:
                 print("Found RULEFILE for {}/{} of: {}".format(tel, inst,
-                    inst_class.rules_file))
+                      inst_class.rules_file))
             # Interpret rules for this class based on image that
             # initialized this instrument's rules
             inst_class.interpret_rules(hlist)
 
             # Now add this interpreted class to the cache
             icache[inst] = inst_class
 
@@ -440,27 +447,27 @@
 #
 # Classes for managing keyword rules
 #
 class KeywordRules(object):
 
     rules_name_suffix = '_header.rules'
 
-    def __init__(self,instrument, telescope='HST', rules_file=None): 
+    def __init__(self, instrument, telescope='HST', rules_file=None):
         """ Read in the rules used to interpret the keywords from the specified
             instrument image header.
         """
         self.instrument = instrument
         self.telescope = telescope
         self.new_header = None
         self.rules_version = None
 
         # Add support for user-specified rules file...
         self.rules_file = rules_file
         if self.rules_file is None:
-            self.get_filename() # define rules file
+            self.get_filename()  # define rules file
 
         self.rules_version, i = self.get_rules_header(self.rules_file)
         rfile = open(self.rules_file)
         self.rule_specs = rfile.readlines()
         rfile.close()
 
         self.rule_objects = []
@@ -481,42 +488,42 @@
         rfiles = glob.glob('*.rules')
         rfiles.sort()
 
         # Sort through list and find only applicable rules files
         # This would include picking up any rules files using the default
         # naming convention; namely, <instrument>_header.rules
         for r in rfiles:
-            v,i = self.get_rules_header(r)
+            v, i = self.get_rules_header(r)
             if v is None or i is None:
                 continue
             if v <= __rules_version__ and i == self.instrument.lower():
                 rules_file = r
                 break
 
         if rules_file is None:
             # define default rules name installed with the software
             rules_name = self.instrument.lower()+self.rules_name_suffix
-            rules_file = os.path.join(os.path.dirname(__file__),rules_name)
+            rules_file = os.path.join(os.path.dirname(__file__), rules_name)
             if not os.path.exists(rules_file):
                 rules_name = self.telescope+self.rules_name_suffix
-                rules_file = os.path.join(os.path.dirname(__file__),rules_name)
+                rules_file = os.path.join(os.path.dirname(__file__), rules_name)
                 if not os.path.exists(rules_file):
                     rules_file = None
 
         if rules_file is None:
             errmsg = 'ERROR:\n'+'    No valid rules file found for:\n'
             errmsg += f'    INSTRUMENT = {self.instrument}\n'
             errmsg += f'    RULES Version <= {__rules_version__}\n'
             print(textutil.textbox(errmsg))
             raise ValueError
 
         self.rules_file = rules_file
         return rules_file
 
-    def get_rules_header(self,filename):
+    def get_rules_header(self, filename):
         """
         Open a potential rules file and return the recognized
         version and instrument types provided in the file's first 2 lines
         """
         version = None
         instrument = None
         f = open(filename)  # open file in read-only mode
@@ -599,15 +606,15 @@
             Primary, SCI, WHT, CTX,...
 
             This method returns the new header and summary table
             as `astropy.io.fits.Header` and numpy.ndarray masked array or
             fits.binTableHDU objects
         """
         # Apply rules to headers
-        fbdict,fbtab = blender.fitsblender(headers, self.rules)
+        fbdict, fbtab = blender.fitsblender(headers, self.rules)
 
         # Determine which keywords are included in the table but not
         # the new dict(header). These will be removed from the output
         # header altogether
         tabcols = fbtab.dtype.names
         hdrkws = list(fbdict.keys())
         del_kws = list(set(tabcols) - set(hdrkws))
@@ -720,15 +727,15 @@
         self.section_name = []
 
     def interpret(self, hdr):
         if self.rules:
             # If self.rules has already been defined for this rule, do not try
             # to interpret it any further with additional headers
             return
-        irules,sname,delkws = interpret_line(self.rule_spec, hdr)
+        irules, sname, delkws = interpret_line(self.rule_spec, hdr)
         # keep track of any section name identified for this rule
         if sname:
             self.section_name.append(sname)
 
         # also keep track of what keywords should be deleted based on this rule
         if delkws:
             self.delete_kws = delkws
@@ -746,15 +753,15 @@
     """
     # Initialize output values
     rules = []
     section_name = None
     delete_kws = []
     # Ignore comment lines in rules file
     if line[0] == '#' or len(line.strip()) == 0 or line[0] == '!':
-        return rules,section_name,delete_kws
+        return rules, section_name, delete_kws
     # clean up input lines
     line = line.strip('\n')
 
     # strip off any comment from the line before parsing the line
     if '#' in line:
         line = line[:line.rfind('#')].strip()
 
@@ -872,21 +879,21 @@
             try:
                 del hdr[kw]
             except KeyError:
                 pass
 
     # Remove '-SIP' from CTYPE for output product
     if 'ctype1' in hdr and hdr['ctype1'].find('SIP') > -1:
-            hdr['ctype1'] = hdr['ctype1'][:-4]
-            hdr['ctype2'] = hdr['ctype2'][:-4]
+        hdr['ctype1'] = hdr['ctype1'][:-4]
+        hdr['ctype2'] = hdr['ctype2'][:-4]
 
     # Remove SIP coefficients from DRZ product
     for k in list(hdr.items()):
-        if (k[0][:2] in ['A_','B_']) or (k[0][:3] in ['IDC','SCD'] and k[0] != 'IDCTAB') or \
-        k[0][:6] in ['SCTYPE','SCRVAL','SNAXIS','SCRPIX']:
+        if (k[0][:2] in ['A_', 'B_']) or (k[0][:3] in ['IDC', 'SCD'] and k[0] != 'IDCTAB') or \
+           k[0][:6] in ['SCTYPE', 'SCRVAL', 'SNAXIS', 'SCRPIX']:
             try:
                 del hdr[k[0]]
             except KeyError:
                 pass
 
     # Remove paper IV related keywords related to the
     #   DGEO correction here
@@ -947,15 +954,15 @@
         _extkey = 'EXTNAME'
 
         #
         # Now, extract the headers necessary for output (as copies)
         # 1. Find the SCI extension in the template image
         # 2. Make a COPY of the extension header for use in new output file
         if fextn is None:
-            extnum = fileutil.findKeywordExtn(ftemplate,_extkey,extlist[0])
+            extnum = fileutil.findKeywordExtn(ftemplate, _extkey, extlist[0])
         else:
             extnum = (extlist[0], fnum)
         scihdr = fits.Header(ftemplate[extnum].header.copy())
         extnum_sci = extnum
 
         # Extract the header for additional extensions
         if len(extlist) > 1 and extlist[1] not in [None, '', ' ', 'INDEF', 'None']:
@@ -964,38 +971,38 @@
             else:
                 # there may or may not be a second type of extension in the template
                 count = 0
                 for f in ftemplate:
                     if 'extname' in f.header and f.header['extname'] == extlist[1]:
                         count += 1
                 if count > 0:
-                    extnum = (extlist[1],fnum)
+                    extnum = (extlist[1], fnum)
                 else:
                     # Use science header for remaining headers
-                    extnum = (extlist[0],fnum)
+                    extnum = (extlist[0], fnum)
         else:
             extnum = extnum_sci
 
         errhdr = fits.Header(ftemplate[extnum].header.copy())
         errhdr['bunit'] = 'UNITLESS'
 
         if len(extlist) > 2 and extlist[2] not in [None, '', ' ', 'INDEF', 'None']:
 
             if fextn is None:
-                extnum = fileutil.findKeywordExtn(ftemplate,_extkey,extlist[2])
+                extnum = fileutil.findKeywordExtn(ftemplate, _extkey, extlist[2])
             else:
                 count = 0
                 for f in ftemplate:
                     if 'extname' in f.header and f.header['extname'] == extlist[2]:
                         count += 1
                 if count > 0:
-                    extnum = (extlist[2],fnum)
+                    extnum = (extlist[2], fnum)
                 else:
                     # Use science header for remaining headers
-                    extnum = (extlist[0],fnum)
+                    extnum = (extlist[0], fnum)
         else:
             extnum = extnum_sci
 
         dqhdr = fits.Header(ftemplate[extnum].header.copy())
         dqhdr['bunit'] = 'UNITLESS'
 
     else:
@@ -1042,15 +1049,15 @@
         for cname in t.dtype.names:
             print('CNAME: ', cname, ' with dtype: ', t[cname].dtype, new_table[cname].dtype)
             new_table[cname] = t[cname]
 
     return new_table
 
 
-def cat_headers(hdr1,hdr2):
+def cat_headers(hdr1, hdr2):
     """
     Create new `astropy.io.fits.Header` object from concatenating 2 input Headers
     """
     nhdr = hdr1.copy()
     for c in hdr2.cards:
         nhdr.append(c)
```

### Comparing `fitsblender-0.4.3/fitsblender/hst_header.rules` & `fitsblender-0.4.4/fitsblender/hst_header.rules`

 * *Files identical despite different names*

### Comparing `fitsblender-0.4.3/fitsblender/jwst_header.rules` & `fitsblender-0.4.4/fitsblender/jwst_header.rules`

 * *Files identical despite different names*

### Comparing `fitsblender-0.4.3/fitsblender/nicmos_header.rules` & `fitsblender-0.4.4/fitsblender/nicmos_header.rules`

 * *Files identical despite different names*

### Comparing `fitsblender-0.4.3/fitsblender/nircam_header.rules` & `fitsblender-0.4.4/fitsblender/nircam_header.rules`

 * *Files identical despite different names*

### Comparing `fitsblender-0.4.3/fitsblender/nirspec_header.rules` & `fitsblender-0.4.4/fitsblender/nirspec_header.rules`

 * *Files identical despite different names*

### Comparing `fitsblender-0.4.3/fitsblender/pars/blendheaders.cfgspc` & `fitsblender-0.4.4/fitsblender/pars/blendheaders.cfgspc`

 * *Files identical despite different names*

### Comparing `fitsblender-0.4.3/fitsblender/stis_header.rules` & `fitsblender-0.4.4/fitsblender/stis_header.rules`

 * *Files identical despite different names*

### Comparing `fitsblender-0.4.3/fitsblender/tests/EUVEngc4151imgx.fits` & `fitsblender-0.4.4/fitsblender/tests/EUVEngc4151imgx.fits`

 * *Files identical despite different names*

### Comparing `fitsblender-0.4.3/fitsblender/tests/FGSf64y0106m_a1f.fits` & `fitsblender-0.4.4/fitsblender/tests/FGSf64y0106m_a1f.fits`

 * *Files identical despite different names*

### Comparing `fitsblender-0.4.3/fitsblender/tests/FOSy19g0309t_c2f.fits` & `fitsblender-0.4.4/fitsblender/tests/FOSy19g0309t_c2f.fits`

 * *Files identical despite different names*

### Comparing `fitsblender-0.4.3/fitsblender/tests/HRSz0yd020fm_c2f.fits` & `fitsblender-0.4.4/fitsblender/tests/HRSz0yd020fm_c2f.fits`

 * *Files identical despite different names*

### Comparing `fitsblender-0.4.3/fitsblender/tests/IUElwp25637mxlo.fits` & `fitsblender-0.4.4/fitsblender/tests/IUElwp25637mxlo.fits`

 * *Files identical despite different names*

### Comparing `fitsblender-0.4.3/fitsblender/tests/NICMOSn4hk12010_mos.fits` & `fitsblender-0.4.4/fitsblender/tests/NICMOSn4hk12010_mos.fits`

 * *Files identical despite different names*

### Comparing `fitsblender-0.4.3/fitsblender/tests/UITfuv2582gc.fits` & `fitsblender-0.4.4/fitsblender/tests/UITfuv2582gc.fits`

 * *Files identical despite different names*

### Comparing `fitsblender-0.4.3/fitsblender/tests/WFPC2ASSNu5780205bx.fits` & `fitsblender-0.4.4/fitsblender/tests/WFPC2ASSNu5780205bx.fits`

 * *Files identical despite different names*

### Comparing `fitsblender-0.4.3/fitsblender/tests/WFPC2u5780205r_c0fx.fits` & `fitsblender-0.4.4/fitsblender/tests/WFPC2u5780205r_c0fx.fits`

 * *Files identical despite different names*

### Comparing `fitsblender-0.4.3/fitsblender/tests/test_fitsblender.py` & `fitsblender-0.4.4/fitsblender/tests/test_fitsblender.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,30 +23,24 @@
 # BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS
 # OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
 # ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR
 # TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE
 # USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH
 # DAMAGE.
 from __future__ import print_function
-import glob
-import os
+from pathlib import Path
 
 import numpy as np
 from astropy.io import fits as pyfits
 from numpy.testing import \
     assert_equal, assert_almost_equal, assert_array_almost_equal, assert_raises
 
 import fitsblender
 
-ROOT_DIR = None
-
-
-def setup():
-    global ROOT_DIR
-    ROOT_DIR = os.path.dirname(__file__)
+ROOT_DIR = Path(__file__).parent
 
 
 def _test_fitsblender(files):
     spec = [
         ('CRPIX1', 'crpix', np.average),
         ('crpix1', 'crpix_lower', np.average),
         ('CRPIX1', 'crpix_constant', np.average, 'constant', 0),
@@ -74,23 +68,22 @@
     assert t['observer'][0] == 'A. A. Zdziarski'
     assert_almost_equal(d['crpix_sum'], 466.0)
     assert_almost_equal(d['crpix_last'], 420.0)
     assert_almost_equal(d['crpix_stddev'], 204.77012857239592)
 
 
 def test_filenames():
-    files = [
-        (x, 0) for x in glob.glob(os.path.join(ROOT_DIR, "*.fits"))]
+    files = [(str(x), 0) for x in ROOT_DIR.glob("*.fits")]
     files.sort()
 
     _test_fitsblender(files)
 
 
 def test_header_objects():
-    files = glob.glob(os.path.join(ROOT_DIR, "*.fits"))
+    files = list(ROOT_DIR.glob("*.fits"))
     files.sort()
     headers = [pyfits.open(x)[0].header for x in files]
 
     _test_fitsblender(headers)
 
 
 def test_nospec():
@@ -106,27 +99,25 @@
     def raises():
         d, t = fitsblender.fitsblender(files, spec)
 
     spec = [
         ('CRPIX1', 'crpix_raise', np.average, 'raises')
         ]
 
-    files = [
-        (x, 0) for x in glob.glob(os.path.join(ROOT_DIR, "*.fits"))]
+    files = [(str(x), 0) for x in ROOT_DIR.glob("*.fits")]
     files.sort()
 
     assert_raises(ValueError, raises)
 
 
 def test_raise_table():
     def raises():
         d, t = fitsblender.fitsblender(files, spec)
 
     spec = [
         ('CRPIX1', 'crpix_raise', None, 'raises')
         ]
 
-    files = [
-        (x, 0) for x in glob.glob(os.path.join(ROOT_DIR, "*.fits"))]
+    files = [(str(x), 0) for x in ROOT_DIR.glob("*.fits")]
     files.sort()
 
     assert_raises(ValueError, raises)
```

### Comparing `fitsblender-0.4.3/fitsblender/wfc3_header.rules` & `fitsblender-0.4.4/fitsblender/wfc3_header.rules`

 * *Files 0% similar despite different names*

```diff
@@ -298,14 +298,15 @@
 SDQFLAGS
 SHADCORR
 SHADFILE
 SHUTRPOS
 SIMPLE
 SIZAXIS1
 SIZAXIS2
+SKYCELL
 SKYSUB
 SKYSUM
 SNRMAX
 SNRMEAN
 SNRMIN
 SOFTERRS
 STDCFFF
@@ -505,14 +506,15 @@
 SCALENSE    SCALENSE    first
 SCLAMP    SCLAMP    multi
 SDQFLAGS    SDQFLAGS    first
 SHADCORR    SHADCORR    multi
 SHADFILE    SHADFILE    multi
 SIZAXIS1    SIZAXIS1    first
 SIZAXIS2    SIZAXIS2    first
+SKYCELL     SKYCELL     first
 SOFTERRS    SOFTERRS    sum
 STDCFFF    STDCFFF    multi
 STDCFFP    STDCFFP    multi
 SUBARRAY    SUBARRAY    first
 SUBTYPE    SUBTYPE    multi
 SUNANGLE   SUNANGLE   first
 T_SGSTAR    T_SGSTAR    multi
```

### Comparing `fitsblender-0.4.3/fitsblender/wfpc2_header.rules` & `fitsblender-0.4.4/fitsblender/wfpc2_header.rules`

 * *Files identical despite different names*

### Comparing `fitsblender-0.4.3/fitsblender.egg-info/SOURCES.txt` & `fitsblender-0.4.4/fitsblender.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 .coveragerc
+.flake8
 .gitignore
 CODE_OF_CONDUCT.md
 LICENSE.txt
 README.md
 azure-pipelines.yml
 pyproject.toml
-setup.cfg
-setup.py
+requirements-dev.txt
 tox.ini
+.github/CODEOWNERS
 .github/workflows/ci.yml
 .github/workflows/publish-to-pypi.yml
 docs/Makefile
 docs/source/conf.py
 docs/source/index.rst
 fitsblender/__init__.py
 fitsblender/acs_header.rules
```

