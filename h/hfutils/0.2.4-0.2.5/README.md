# Comparing `tmp/hfutils-0.2.4.tar.gz` & `tmp/hfutils-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hfutils-0.2.4.tar", last modified: Sat May  4 18:52:47 2024, max compression
+gzip compressed data, was "hfutils-0.2.5.tar", last modified: Mon May  6 15:38:51 2024, max compression
```

## Comparing `hfutils-0.2.4.tar` & `hfutils-0.2.5.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:52:47.085215 hfutils-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-04 18:52:24.000000 hfutils-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-04 18:52:24.000000 hfutils-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10149 2024-05-04 18:52:47.085215 hfutils-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-05-04 18:52:24.000000 hfutils-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:52:47.077216 hfutils-0.2.4/hfutils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:52:47.077216 hfutils-0.2.4/hfutils/archive/
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/archive/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/archive/rar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/archive/sevenz.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/archive/tar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/archive/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:52:47.077216 hfutils-0.2.4/hfutils/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:52:47.081215 hfutils-0.2.4/hfutils/entry/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/entry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/entry/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/entry/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/entry/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/entry/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/entry/ls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/entry/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/entry/whoami.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:52:47.081215 hfutils-0.2.4/hfutils/index/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11377 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/index/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/index/hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/index/make.py
--rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/index/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:52:47.081215 hfutils-0.2.4/hfutils/operate/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/operate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/operate/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7528 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/operate/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/operate/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/operate/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:52:47.081215 hfutils-0.2.4/hfutils/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/utils/binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/utils/temp.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/utils/tqdm_.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/utils/walk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:52:47.081215 hfutils-0.2.4/hfutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10149 2024-05-04 18:52:47.000000 hfutils-0.2.4/hfutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-04 18:52:47.000000 hfutils-0.2.4/hfutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 18:52:47.000000 hfutils-0.2.4/hfutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-04 18:52:47.000000 hfutils-0.2.4/hfutils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-04 18:52:47.000000 hfutils-0.2.4/hfutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-04 18:52:47.000000 hfutils-0.2.4/hfutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-04 18:52:24.000000 hfutils-0.2.4/requirements-7z.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-04 18:52:24.000000 hfutils-0.2.4/requirements-build.txt
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-04 18:52:24.000000 hfutils-0.2.4/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-04 18:52:24.000000 hfutils-0.2.4/requirements-rar.txt
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-04 18:52:24.000000 hfutils-0.2.4/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 18:52:24.000000 hfutils-0.2.4/requirements-transfer.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-04 18:52:24.000000 hfutils-0.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 18:52:47.089216 hfutils-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-04 18:52:24.000000 hfutils-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:38:51.514883 hfutils-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-06 15:38:32.000000 hfutils-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-06 15:38:32.000000 hfutils-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-05-06 15:38:51.514883 hfutils-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-05-06 15:38:32.000000 hfutils-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:38:51.506883 hfutils-0.2.5/hfutils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:38:51.506883 hfutils-0.2.5/hfutils/archive/
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/archive/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/archive/rar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/archive/sevenz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/archive/tar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/archive/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:38:51.506883 hfutils-0.2.5/hfutils/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:38:51.506883 hfutils-0.2.5/hfutils/entry/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/entry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/entry/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/entry/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/entry/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/entry/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/entry/ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/entry/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/entry/whoami.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:38:51.510883 hfutils-0.2.5/hfutils/index/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11377 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/index/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/index/hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/index/make.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/index/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:38:51.510883 hfutils-0.2.5/hfutils/operate/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/operate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/operate/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7528 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/operate/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/operate/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/operate/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:38:51.510883 hfutils-0.2.5/hfutils/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/utils/binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15309 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/utils/irregular_repo.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/utils/temp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/utils/tqdm_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-06 15:38:32.000000 hfutils-0.2.5/hfutils/utils/walk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:38:51.510883 hfutils-0.2.5/hfutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-05-06 15:38:51.000000 hfutils-0.2.5/hfutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-06 15:38:51.000000 hfutils-0.2.5/hfutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 15:38:51.000000 hfutils-0.2.5/hfutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-06 15:38:51.000000 hfutils-0.2.5/hfutils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-06 15:38:51.000000 hfutils-0.2.5/hfutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-06 15:38:51.000000 hfutils-0.2.5/hfutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-06 15:38:32.000000 hfutils-0.2.5/requirements-7z.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-06 15:38:32.000000 hfutils-0.2.5/requirements-build.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-06 15:38:32.000000 hfutils-0.2.5/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-06 15:38:32.000000 hfutils-0.2.5/requirements-rar.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-06 15:38:32.000000 hfutils-0.2.5/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-06 15:38:32.000000 hfutils-0.2.5/requirements-transfer.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-06 15:38:32.000000 hfutils-0.2.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 15:38:51.514883 hfutils-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-06 15:38:32.000000 hfutils-0.2.5/setup.py
```

### Comparing `hfutils-0.2.4/LICENSE` & `hfutils-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.4/PKG-INFO` & `hfutils-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hfutils
-Version: 0.2.4
+Version: 0.2.5
 Summary: Useful utilities for huggingface
 Home-page: https://github.com/deepghs/hfutils
 Author: narugo1992
 Author-email: narugo992@gmail.com
 License: Apache License, Version 2.0
 Keywords: Utilities of images.
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,14 +22,15 @@
 License-File: LICENSE
 Requires-Dist: hbutils>=0.9.0
 Requires-Dist: huggingface_hub>=0.22
 Requires-Dist: tqdm
 Requires-Dist: requests
 Requires-Dist: click>=7
 Requires-Dist: tzlocal
+Requires-Dist: natsort
 Provides-Extra: rar
 Requires-Dist: rarfile; extra == "rar"
 Provides-Extra: test
 Requires-Dist: coverage>=5; extra == "test"
 Requires-Dist: mock>=4.0.3; extra == "test"
 Requires-Dist: flake8~=3.5; extra == "test"
 Requires-Dist: testfixtures>=6.18.5; extra == "test"
```

### Comparing `hfutils-0.2.4/README.md` & `hfutils-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.4/hfutils/archive/__init__.py` & `hfutils-0.2.5/hfutils/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.4/hfutils/archive/base.py` & `hfutils-0.2.5/hfutils/archive/base.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.4/hfutils/archive/rar.py` & `hfutils-0.2.5/hfutils/archive/rar.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.4/hfutils/archive/sevenz.py` & `hfutils-0.2.5/hfutils/archive/sevenz.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.4/hfutils/archive/tar.py` & `hfutils-0.2.5/hfutils/archive/tar.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.4/hfutils/archive/zip.py` & `hfutils-0.2.5/hfutils/archive/zip.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.4/hfutils/entry/base.py` & `hfutils-0.2.5/hfutils/entry/base.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.4/hfutils/entry/dispatch.py` & `hfutils-0.2.5/hfutils/entry/dispatch.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.4/hfutils/entry/download.py` & `hfutils-0.2.5/hfutils/entry/download.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.4/hfutils/entry/ls.py` & `hfutils-0.2.5/hfutils/entry/ls.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.4/hfutils/entry/upload.py` & `hfutils-0.2.5/hfutils/entry/upload.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.4/hfutils/entry/whoami.py` & `hfutils-0.2.5/hfutils/entry/whoami.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.4/hfutils/index/fetch.py` & `hfutils-0.2.5/hfutils/index/fetch.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.4/hfutils/index/hash.py` & `hfutils-0.2.5/hfutils/index/hash.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.4/hfutils/index/make.py` & `hfutils-0.2.5/hfutils/index/make.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.4/hfutils/index/validate.py` & `hfutils-0.2.5/hfutils/index/validate.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.4/hfutils/operate/base.py` & `hfutils-0.2.5/hfutils/operate/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import fnmatch
 import os
 from functools import lru_cache
 from typing import Literal, List, Optional
 
 from huggingface_hub import HfApi, HfFileSystem
 
+from hfutils.utils import parse_hf_fs_path
+
 RepoTypeTyping = Literal['dataset', 'model', 'space']
 REPO_TYPES = ['dataset', 'model', 'space']
 
 
 @lru_cache()
 def _get_hf_token() -> Optional[str]:
     """
@@ -109,20 +111,23 @@
     else:
         raise ValueError(f'Invalid repo_type - {repo_type!r}.')
     if subdir and subdir != '.':
         repo_root_path = f'{repo_root_path}/{subdir}'
 
     try:
         _exist_files = [
-            os.path.relpath(file, repo_root_path)
+            parse_hf_fs_path(file).filename
             for file in hf_fs.glob(f'{repo_root_path}/**', revision=revision)
         ]
     except FileNotFoundError:
         return []
-    _exist_ps = sorted([(file, file.split(os.sep)) for file in _exist_files], key=lambda x: x[1])
+    if subdir and subdir != '.':
+        _exist_files = [os.path.relpath(file, subdir) for file in _exist_files]
+
+    _exist_ps = sorted([(file, file.split('/')) for file in _exist_files], key=lambda x: x[1])
     retval = []
     for i, (file, segments) in enumerate(_exist_ps):
         if i < len(_exist_ps) - 1 and segments == _exist_ps[i + 1][1][:len(segments)]:
             continue
         if file != '.':
             if not _is_file_ignored(segments, ignore_patterns):
                 retval.append('/'.join(segments))
```

### Comparing `hfutils-0.2.4/hfutils/operate/download.py` & `hfutils-0.2.5/hfutils/operate/download.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.4/hfutils/operate/upload.py` & `hfutils-0.2.5/hfutils/operate/upload.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.4/hfutils/operate/validate.py` & `hfutils-0.2.5/hfutils/operate/validate.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.4/hfutils/utils/binary.py` & `hfutils-0.2.5/hfutils/utils/binary.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.4/hfutils/utils/download.py` & `hfutils-0.2.5/hfutils/utils/download.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.4/hfutils/utils/temp.py` & `hfutils-0.2.5/hfutils/utils/temp.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.4/hfutils/utils/tqdm_.py` & `hfutils-0.2.5/hfutils/utils/tqdm_.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.4/hfutils/utils/walk.py` & `hfutils-0.2.5/hfutils/utils/walk.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.4/hfutils.egg-info/PKG-INFO` & `hfutils-0.2.5/hfutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hfutils
-Version: 0.2.4
+Version: 0.2.5
 Summary: Useful utilities for huggingface
 Home-page: https://github.com/deepghs/hfutils
 Author: narugo1992
 Author-email: narugo992@gmail.com
 License: Apache License, Version 2.0
 Keywords: Utilities of images.
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,14 +22,15 @@
 License-File: LICENSE
 Requires-Dist: hbutils>=0.9.0
 Requires-Dist: huggingface_hub>=0.22
 Requires-Dist: tqdm
 Requires-Dist: requests
 Requires-Dist: click>=7
 Requires-Dist: tzlocal
+Requires-Dist: natsort
 Provides-Extra: rar
 Requires-Dist: rarfile; extra == "rar"
 Provides-Extra: test
 Requires-Dist: coverage>=5; extra == "test"
 Requires-Dist: mock>=4.0.3; extra == "test"
 Requires-Dist: flake8~=3.5; extra == "test"
 Requires-Dist: testfixtures>=6.18.5; extra == "test"
```

### Comparing `hfutils-0.2.4/hfutils.egg-info/SOURCES.txt` & `hfutils-0.2.5/hfutils.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -41,11 +41,12 @@
 hfutils/operate/base.py
 hfutils/operate/download.py
 hfutils/operate/upload.py
 hfutils/operate/validate.py
 hfutils/utils/__init__.py
 hfutils/utils/binary.py
 hfutils/utils/download.py
+hfutils/utils/irregular_repo.json
 hfutils/utils/path.py
 hfutils/utils/temp.py
 hfutils/utils/tqdm_.py
 hfutils/utils/walk.py
```

### Comparing `hfutils-0.2.4/hfutils.egg-info/requires.txt` & `hfutils-0.2.5/hfutils.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 hbutils>=0.9.0
 huggingface_hub>=0.22
 tqdm
 requests
 click>=7
 tzlocal
+natsort
 
 [7z]
 py7zr
 
 [build]
 pyinstaller<5,>=4.7
```

### Comparing `hfutils-0.2.4/setup.py` & `hfutils-0.2.5/setup.py`

 * *Files identical despite different names*

