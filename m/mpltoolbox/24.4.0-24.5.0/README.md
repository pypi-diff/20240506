# Comparing `tmp/mpltoolbox-24.4.0.tar.gz` & `tmp/mpltoolbox-24.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpltoolbox-24.4.0.tar", last modified: Mon Apr 29 09:33:32 2024, max compression
+gzip compressed data, was "mpltoolbox-24.5.0.tar", last modified: Mon May  6 10:51:30 2024, max compression
```

## Comparing `mpltoolbox-24.4.0.tar` & `mpltoolbox-24.5.0.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:33:32.309115 mpltoolbox-24.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:33:32.301115 mpltoolbox-24.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:33:32.305115 mpltoolbox-24.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-29 09:33:32.309115 mpltoolbox-24.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:33:32.305115 mpltoolbox-24.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9422 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/docs/callbacks.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/docs/demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/docs/ellipses.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:33:32.305115 mpltoolbox-24.4.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)   137750 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/docs/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    75876 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    95767 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/docs/lines.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/docs/points.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/docs/polygons.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/docs/programmatic-control.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/docs/rectangles.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/docs/spans.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-29 09:33:32.309115 mpltoolbox-24.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:33:32.305115 mpltoolbox-24.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:33:32.309115 mpltoolbox-24.4.0/src/mpltoolbox/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/src/mpltoolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/src/mpltoolbox/ellipses.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/src/mpltoolbox/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/src/mpltoolbox/hspans.py
--rw-r--r--   0 runner    (1001) docker     (127)     5700 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/src/mpltoolbox/lines.py
--rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/src/mpltoolbox/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/src/mpltoolbox/points.py
--rw-r--r--   0 runner    (1001) docker     (127)     8111 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/src/mpltoolbox/polygons.py
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/src/mpltoolbox/rectangles.py
--rw-r--r--   0 runner    (1001) docker     (127)    12565 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/src/mpltoolbox/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/src/mpltoolbox/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/src/mpltoolbox/vspans.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:33:32.309115 mpltoolbox-24.4.0/src/mpltoolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-29 09:33:32.000000 mpltoolbox-24.4.0/src/mpltoolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-29 09:33:32.000000 mpltoolbox-24.4.0/src/mpltoolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 09:33:32.000000 mpltoolbox-24.4.0/src/mpltoolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-29 09:33:32.000000 mpltoolbox-24.4.0/src/mpltoolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-29 09:33:32.000000 mpltoolbox-24.4.0/src/mpltoolbox.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:33:32.309115 mpltoolbox-24.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/tests/lines_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-29 09:32:13.000000 mpltoolbox-24.4.0/tests/points_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:51:30.893834 mpltoolbox-24.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:51:30.885834 mpltoolbox-24.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:51:30.885834 mpltoolbox-24.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-06 10:51:30.893834 mpltoolbox-24.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:51:30.889834 mpltoolbox-24.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9422 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/docs/callbacks.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/docs/demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/docs/ellipses.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:51:30.889834 mpltoolbox-24.5.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   137750 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/docs/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    75876 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    95767 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/docs/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/docs/lines.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/docs/points.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/docs/polygons.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/docs/programmatic-control.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/docs/rectangles.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/docs/spans.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-06 10:51:30.893834 mpltoolbox-24.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:51:30.885834 mpltoolbox-24.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:51:30.889834 mpltoolbox-24.5.0/src/mpltoolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/src/mpltoolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/src/mpltoolbox/ellipses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/src/mpltoolbox/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/src/mpltoolbox/hspans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5700 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/src/mpltoolbox/lines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/src/mpltoolbox/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/src/mpltoolbox/points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8111 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/src/mpltoolbox/polygons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/src/mpltoolbox/rectangles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13493 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/src/mpltoolbox/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/src/mpltoolbox/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/src/mpltoolbox/vspans.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:51:30.893834 mpltoolbox-24.5.0/src/mpltoolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-06 10:51:30.000000 mpltoolbox-24.5.0/src/mpltoolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-06 10:51:30.000000 mpltoolbox-24.5.0/src/mpltoolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 10:51:30.000000 mpltoolbox-24.5.0/src/mpltoolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-06 10:51:30.000000 mpltoolbox-24.5.0/src/mpltoolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-06 10:51:30.000000 mpltoolbox-24.5.0/src/mpltoolbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:51:30.893834 mpltoolbox-24.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/tests/lines_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-06 10:51:24.000000 mpltoolbox-24.5.0/tests/points_test.py
```

### Comparing `mpltoolbox-24.4.0/LICENSE` & `mpltoolbox-24.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.4.0/PKG-INFO` & `mpltoolbox-24.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpltoolbox
-Version: 24.4.0
+Version: 24.5.0
 Summary: Interactive tools for matplotlib
 Home-page: https://github.com/scipp/mpltoolbox
 Author: Neil Vaytet
 Author-email: neil.vaytet@esss.se
 License: BSD
 Project-URL: Bug Tracker, https://github.com/scipp/mpltoolbox/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mpltoolbox-24.4.0/README.md` & `mpltoolbox-24.5.0/README.md`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.4.0/docs/callbacks.ipynb` & `mpltoolbox-24.5.0/docs/callbacks.ipynb`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.4.0/docs/conf.py` & `mpltoolbox-24.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.4.0/docs/demo.ipynb` & `mpltoolbox-24.5.0/docs/demo.ipynb`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.4.0/docs/ellipses.ipynb` & `mpltoolbox-24.5.0/docs/ellipses.ipynb`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.4.0/docs/images/favicon.ico` & `mpltoolbox-24.5.0/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.4.0/docs/images/logo.png` & `mpltoolbox-24.5.0/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.4.0/docs/images/logo.svg` & `mpltoolbox-24.5.0/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.4.0/docs/index.rst` & `mpltoolbox-24.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.4.0/docs/lines.ipynb` & `mpltoolbox-24.5.0/docs/lines.ipynb`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.4.0/docs/points.ipynb` & `mpltoolbox-24.5.0/docs/points.ipynb`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.4.0/docs/polygons.ipynb` & `mpltoolbox-24.5.0/docs/polygons.ipynb`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.4.0/docs/programmatic-control.ipynb` & `mpltoolbox-24.5.0/docs/programmatic-control.ipynb`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.4.0/docs/rectangles.ipynb` & `mpltoolbox-24.5.0/docs/rectangles.ipynb`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.4.0/docs/spans.ipynb` & `mpltoolbox-24.5.0/docs/spans.ipynb`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.4.0/setup.cfg` & `mpltoolbox-24.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.4.0/src/mpltoolbox/ellipses.py` & `mpltoolbox-24.5.0/src/mpltoolbox/ellipses.py`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.4.0/src/mpltoolbox/hspans.py` & `mpltoolbox-24.5.0/src/mpltoolbox/hspans.py`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.4.0/src/mpltoolbox/lines.py` & `mpltoolbox-24.5.0/src/mpltoolbox/lines.py`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.4.0/src/mpltoolbox/patch.py` & `mpltoolbox-24.5.0/src/mpltoolbox/patch.py`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.4.0/src/mpltoolbox/points.py` & `mpltoolbox-24.5.0/src/mpltoolbox/points.py`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.4.0/src/mpltoolbox/polygons.py` & `mpltoolbox-24.5.0/src/mpltoolbox/polygons.py`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.4.0/src/mpltoolbox/rectangles.py` & `mpltoolbox-24.5.0/src/mpltoolbox/rectangles.py`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.4.0/src/mpltoolbox/tool.py` & `mpltoolbox-24.5.0/src/mpltoolbox/tool.py`

 * *Files 3% similar despite different names*

```diff
@@ -157,38 +157,62 @@
     def start(self):
         """
         Activate the tool.
         """
         self._connections["button_press_event"] = self._fig.canvas.mpl_connect(
             "button_press_event", self._on_button_press
         )
-        self._connections["pick_event"] = self._fig.canvas.mpl_connect(
-            "pick_event", self._on_pick
-        )
+        if "pick_event" not in self._connections:
+            self._connections["pick_event"] = self._fig.canvas.mpl_connect(
+                "pick_event", self._on_pick
+            )
+        for child in self.children:
+            child._vertices.set_visible(True)
 
     def stop(self):
         """
-        Dectivate the tool.
+        Dectivate adding new children, but resizing and moving existing children is
+        still possible.
+        """
+        self._disconnect(
+            [key for key in self._connections.keys() if key != "pick_event"]
+        )
+
+    def freeze(self):
+        """
+        Deactivate the tool but keep the children. No new children can be added and
+        existing children cannot be moved or resized.
         """
         self._disconnect(list(self._connections.keys()))
+        for child in self.children:
+            child._vertices.set_visible(False)
 
-    def shutdown(self):
+    def clear(self):
         """
-        Deactivate the tool and remove all children from the axes.
+        Remove all children from the axes.
         """
-        self.stop()
         for a in self.children:
             a.remove()
         self.children.clear()
-        self._connections.clear()
         self._draw()
 
+    def shutdown(self):
+        """
+        Deactivate the tool and remove all children from the axes.
+        """
+        self.stop()
+        self._connections.clear()
+        self.clear()
+
     def _get_active_tool(self) -> str:
         return self._fig.canvas.toolbar.mode
 
+    def _locked_by_other_tool(self) -> bool:
+        return getattr(self._ax, "_mpltoolbox_lock", False)
+
     def _disconnect(self, keys: List[str]):
         for key in keys:
             if key in self._connections:
                 self._fig.canvas.mpl_disconnect(self._connections[key])
                 del self._connections[key]
 
     def _connect(self, connections: dict):
@@ -196,19 +220,19 @@
             self._connections[key] = self._fig.canvas.mpl_connect(key, func)
 
     def _on_button_press(self, event: Event):
         if (
             event.button != 1
             or self._pick_lock
             or self._get_active_tool()
+            or self._locked_by_other_tool()
             or event.modifiers
+            or event.inaxes != self._ax
         ):
             return
-        if event.inaxes != self._ax:
-            return
         if "motion_notify_event" not in self._connections:
             self._nclicks = 0
             self._spawn_new_owner(x=event.xdata, y=event.ydata)
             self._connect({"motion_notify_event": self._on_motion_notify})
         self._nclicks += 1
         self._persist_vertex(event=event, owner=self.children[-1])
 
@@ -240,26 +264,27 @@
     def _finalize_owner(self):
         child = self.children[-1]
         child.set_picker(5.0)
         if self.on_create is not None:
             self.call_on_create(child)
 
     def _on_pick(self, event: Event):
-        if self._get_active_tool():
-            return
-        if event.artist.parent not in self.children:
-            return
         mev = event.mouseevent
-        if mev.inaxes != self._ax:
+        if (
+            self._get_active_tool()
+            or event.artist.parent not in self.children
+            or mev.inaxes != self._ax
+        ):
             return
         art = event.artist
         if (mev.button == 1) and ("ctrl" not in mev.modifiers):
             if not art.parent.is_moveable(art):
                 return
             self._pick_lock = True
+            self._ax._mpltoolbox_lock = True
             self._grab_vertex(event)
         if mev.button == 3:
             if not art.parent.is_draggable(art):
                 return
             self._pick_lock = True
             self._grab_owner(event)
         if (mev.button == 2) or ((mev.button == 1) and ("ctrl" in mev.modifiers)):
@@ -322,14 +347,15 @@
             self.call_on_drag_move(self._grabbed_owner)
         if self.on_change is not None:
             self.call_on_change(self._grabbed_owner)
 
     def _release_owner(self, event: Event, kind: str):
         self._disconnect(["motion_notify_event", "button_release_event"])
         self._pick_lock = False
+        self._ax._mpltoolbox_lock = False
         if (kind == "vertex") and (self.on_vertex_release is not None):
             self.call_on_vertex_release(self._moving_vertex_owner)
         elif (kind == "drag") and (self.on_drag_release is not None):
             self.call_on_drag_release(self._grabbed_owner)
 
     def click(
         self,
```

### Comparing `mpltoolbox-24.4.0/src/mpltoolbox/vspans.py` & `mpltoolbox-24.5.0/src/mpltoolbox/vspans.py`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.4.0/src/mpltoolbox.egg-info/PKG-INFO` & `mpltoolbox-24.5.0/src/mpltoolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpltoolbox
-Version: 24.4.0
+Version: 24.5.0
 Summary: Interactive tools for matplotlib
 Home-page: https://github.com/scipp/mpltoolbox
 Author: Neil Vaytet
 Author-email: neil.vaytet@esss.se
 License: BSD
 Project-URL: Bug Tracker, https://github.com/scipp/mpltoolbox/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mpltoolbox-24.4.0/src/mpltoolbox.egg-info/SOURCES.txt` & `mpltoolbox-24.5.0/src/mpltoolbox.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+.readthedocs.yaml
 LICENSE
 README.md
 environment.yml
 pyproject.toml
 setup.cfg
 .github/workflows/ci.yml
 docs/api.rst
```

### Comparing `mpltoolbox-24.4.0/tests/conftest.py` & `mpltoolbox-24.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.4.0/tests/lines_test.py` & `mpltoolbox-24.5.0/tests/lines_test.py`

 * *Files identical despite different names*

### Comparing `mpltoolbox-24.4.0/tests/points_test.py` & `mpltoolbox-24.5.0/tests/points_test.py`

 * *Files identical despite different names*

