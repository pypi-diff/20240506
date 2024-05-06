# Comparing `tmp/patiencediff-0.2.8.tar.gz` & `tmp/patiencediff-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patiencediff-0.2.8.tar", last modified: Sun Nov 20 13:08:20 2022, max compression
+gzip compressed data, was "patiencediff-0.2.9.tar", last modified: Tue Nov 29 10:44:42 2022, max compression
```

## Comparing `patiencediff-0.2.8.tar` & `patiencediff-0.2.9.tar`

### file list

```diff
@@ -1,31 +1,21 @@
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2022-11-20 13:08:20.777445 patiencediff-0.2.8/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       37 2022-11-20 13:08:11.000000 patiencediff-0.2.8/.bzrignore
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2022-11-20 13:08:20.773445 patiencediff-0.2.8/.github/
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2022-11-20 13:08:20.777445 patiencediff-0.2.8/.github/workflows/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      535 2022-11-20 13:08:11.000000 patiencediff-0.2.8/.github/workflows/disperse.yml
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      917 2022-11-20 13:08:11.000000 patiencediff-0.2.8/.github/workflows/pythonpackage.yml
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1569 2022-11-20 13:08:11.000000 patiencediff-0.2.8/.github/workflows/pythonpublish.yml
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       59 2022-11-20 13:08:11.000000 patiencediff-0.2.8/.gitignore
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      151 2022-11-20 13:08:11.000000 patiencediff-0.2.8/AUTHORS
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    18092 2022-11-20 13:08:11.000000 patiencediff-0.2.8/COPYING
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       81 2022-11-20 13:08:11.000000 patiencediff-0.2.8/MANIFEST.in
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     2241 2022-11-20 13:08:20.777445 patiencediff-0.2.8/PKG-INFO
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1301 2022-11-20 13:08:11.000000 patiencediff-0.2.8/README.rst
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      833 2022-11-20 13:08:11.000000 patiencediff-0.2.8/build.cmd
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      303 2022-11-20 13:08:11.000000 patiencediff-0.2.8/disperse.conf
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2022-11-20 13:08:20.777445 patiencediff-0.2.8/patiencediff/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     5043 2022-11-20 13:08:14.000000 patiencediff-0.2.8/patiencediff/__init__.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1811 2022-11-20 13:08:11.000000 patiencediff-0.2.8/patiencediff/__main__.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    36249 2022-11-20 13:08:11.000000 patiencediff-0.2.8/patiencediff/_patiencediff_c.c
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      458 2022-11-20 13:08:11.000000 patiencediff-0.2.8/patiencediff/_patiencediff_c.pyi
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     9515 2022-11-20 13:08:11.000000 patiencediff-0.2.8/patiencediff/_patiencediff_py.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)        0 2022-11-20 13:08:11.000000 patiencediff-0.2.8/patiencediff/py.typed
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    22910 2022-11-20 13:08:11.000000 patiencediff-0.2.8/patiencediff/test_patiencediff.py
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2022-11-20 13:08:20.777445 patiencediff-0.2.8/patiencediff.egg-info/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     2241 2022-11-20 13:08:20.000000 patiencediff-0.2.8/patiencediff.egg-info/PKG-INFO
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      568 2022-11-20 13:08:20.000000 patiencediff-0.2.8/patiencediff.egg-info/SOURCES.txt
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)        1 2022-11-20 13:08:20.000000 patiencediff-0.2.8/patiencediff.egg-info/dependency_links.txt
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       13 2022-11-20 13:08:20.000000 patiencediff-0.2.8/patiencediff.egg-info/top_level.txt
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       81 2022-11-20 13:08:11.000000 patiencediff-0.2.8/pyproject.toml
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      967 2022-11-20 13:08:20.777445 patiencediff-0.2.8/setup.cfg
--rwxr-xr-x   0 jelmer    (1000) jelmer    (1000)      304 2022-11-20 13:08:11.000000 patiencediff-0.2.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-29 10:44:42.478248 patiencediff-0.2.9/
+-rw-r--r--   0 root         (0) root         (0)      151 2022-11-29 10:44:40.000000 patiencediff-0.2.9/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)    18092 2022-11-29 10:44:40.000000 patiencediff-0.2.9/COPYING
+-rw-r--r--   0 root         (0) root         (0)       81 2022-11-29 10:44:40.000000 patiencediff-0.2.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2241 2022-11-29 10:44:42.482249 patiencediff-0.2.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1301 2022-11-29 10:44:40.000000 patiencediff-0.2.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-29 10:44:42.478248 patiencediff-0.2.9/patiencediff/
+-rw-r--r--   0 root         (0) root         (0)     5043 2022-11-29 10:44:42.000000 patiencediff-0.2.9/patiencediff/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2022-11-29 10:44:40.000000 patiencediff-0.2.9/patiencediff/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    36249 2022-11-29 10:44:40.000000 patiencediff-0.2.9/patiencediff/_patiencediff_c.c
+-rw-r--r--   0 root         (0) root         (0)     9515 2022-11-29 10:44:40.000000 patiencediff-0.2.9/patiencediff/_patiencediff_py.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-29 10:44:40.000000 patiencediff-0.2.9/patiencediff/py.typed
+-rw-r--r--   0 root         (0) root         (0)    22910 2022-11-29 10:44:40.000000 patiencediff-0.2.9/patiencediff/test_patiencediff.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-29 10:44:42.478248 patiencediff-0.2.9/patiencediff.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2241 2022-11-29 10:44:42.000000 patiencediff-0.2.9/patiencediff.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      386 2022-11-29 10:44:42.000000 patiencediff-0.2.9/patiencediff.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-29 10:44:42.000000 patiencediff-0.2.9/patiencediff.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2022-11-29 10:44:42.000000 patiencediff-0.2.9/patiencediff.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       81 2022-11-29 10:44:40.000000 patiencediff-0.2.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      967 2022-11-29 10:44:42.482249 patiencediff-0.2.9/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)      304 2022-11-29 10:44:40.000000 patiencediff-0.2.9/setup.py
```

### Comparing `patiencediff-0.2.8/COPYING` & `patiencediff-0.2.9/COPYING`

 * *Files identical despite different names*

### Comparing `patiencediff-0.2.8/PKG-INFO` & `patiencediff-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patiencediff
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python implementation of the patiencediff algorithm
 Maintainer: Breezy Developers
 Maintainer-email: team@breezy-vcs.org
 License: GNU GPLv2 or later
 Project-URL: Repository, https://github.com/breezy-team/patiencediff
 Classifier: Development Status :: 6 - Mature
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
```

### Comparing `patiencediff-0.2.8/README.rst` & `patiencediff-0.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `patiencediff-0.2.8/patiencediff/__init__.py` & `patiencediff-0.2.9/patiencediff/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import difflib
 
 from typing import Type
 
 
 __all__ = ['PatienceSequenceMatcher', 'unified_diff', 'unified_diff_files']
 
-__version__ = (0, 2, 8)
+__version__ = (0, 2, 9)
 
 
 # This is a version of unified_diff which only adds a factory parameter
 # so that you can override the default SequenceMatcher
 # this has been submitted as a patch to python
 def unified_diff(a, b, fromfile='', tofile='', fromfiledate='',
                  tofiledate='', n=3, lineterm='\n',
```

### Comparing `patiencediff-0.2.8/patiencediff/__main__.py` & `patiencediff-0.2.9/patiencediff/__main__.py`

 * *Files identical despite different names*

### Comparing `patiencediff-0.2.8/patiencediff/_patiencediff_c.c` & `patiencediff-0.2.9/patiencediff/_patiencediff_c.c`

 * *Files identical despite different names*

### Comparing `patiencediff-0.2.8/patiencediff/_patiencediff_py.py` & `patiencediff-0.2.9/patiencediff/_patiencediff_py.py`

 * *Files identical despite different names*

### Comparing `patiencediff-0.2.8/patiencediff/test_patiencediff.py` & `patiencediff-0.2.9/patiencediff/test_patiencediff.py`

 * *Files identical despite different names*

### Comparing `patiencediff-0.2.8/patiencediff.egg-info/PKG-INFO` & `patiencediff-0.2.9/patiencediff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patiencediff
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python implementation of the patiencediff algorithm
 Maintainer: Breezy Developers
 Maintainer-email: team@breezy-vcs.org
 License: GNU GPLv2 or later
 Project-URL: Repository, https://github.com/breezy-team/patiencediff
 Classifier: Development Status :: 6 - Mature
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
```

### Comparing `patiencediff-0.2.8/setup.cfg` & `patiencediff-0.2.9/setup.cfg`

 * *Files identical despite different names*

