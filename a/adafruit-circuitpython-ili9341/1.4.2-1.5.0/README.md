# Comparing `tmp/adafruit-circuitpython-ili9341-1.4.2.tar.gz` & `tmp/adafruit_circuitpython_ili9341-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ili9341-1.4.2.tar", last modified: Mon Dec 18 17:07:52 2023, max compression
+gzip compressed data, was "adafruit_circuitpython_ili9341-1.5.0.tar", last modified: Mon May  6 21:01:16 2024, max compression
```

## Comparing `adafruit-circuitpython-ili9341-1.4.2.tar` & `adafruit_circuitpython_ili9341-1.5.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 17:07:52.773269 adafruit-circuitpython-ili9341-1.4.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 17:07:52.765269 adafruit-circuitpython-ili9341-1.4.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 17:07:52.769269 adafruit-circuitpython-ili9341-1.4.2/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2023-12-18 17:07:39.000000 adafruit-circuitpython-ili9341-1.4.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 17:07:52.769269 adafruit-circuitpython-ili9341-1.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-12-18 17:07:39.000000 adafruit-circuitpython-ili9341-1.4.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2023-12-18 17:07:39.000000 adafruit-circuitpython-ili9341-1.4.2/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2023-12-18 17:07:39.000000 adafruit-circuitpython-ili9341-1.4.2/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2023-12-18 17:07:39.000000 adafruit-circuitpython-ili9341-1.4.2/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2023-12-18 17:07:39.000000 adafruit-circuitpython-ili9341-1.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2023-12-18 17:07:39.000000 adafruit-circuitpython-ili9341-1.4.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2023-12-18 17:07:39.000000 adafruit-circuitpython-ili9341-1.4.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      388 2023-12-18 17:07:39.000000 adafruit-circuitpython-ili9341-1.4.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2023-12-18 17:07:39.000000 adafruit-circuitpython-ili9341-1.4.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2023-12-18 17:07:39.000000 adafruit-circuitpython-ili9341-1.4.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 17:07:52.769269 adafruit-circuitpython-ili9341-1.4.2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2023-12-18 17:07:39.000000 adafruit-circuitpython-ili9341-1.4.2/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2023-12-18 17:07:39.000000 adafruit-circuitpython-ili9341-1.4.2/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2023-12-18 17:07:39.000000 adafruit-circuitpython-ili9341-1.4.2/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2023-12-18 17:07:52.773269 adafruit-circuitpython-ili9341-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2023-12-18 17:07:39.000000 adafruit-circuitpython-ili9341-1.4.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-18 17:07:39.000000 adafruit-circuitpython-ili9341-1.4.2/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 17:07:52.773269 adafruit-circuitpython-ili9341-1.4.2/adafruit_circuitpython_ili9341.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2023-12-18 17:07:52.000000 adafruit-circuitpython-ili9341-1.4.2/adafruit_circuitpython_ili9341.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2023-12-18 17:07:52.000000 adafruit-circuitpython-ili9341-1.4.2/adafruit_circuitpython_ili9341.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-18 17:07:52.000000 adafruit-circuitpython-ili9341-1.4.2/adafruit_circuitpython_ili9341.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-12-18 17:07:52.000000 adafruit-circuitpython-ili9341-1.4.2/adafruit_circuitpython_ili9341.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-18 17:07:52.000000 adafruit-circuitpython-ili9341-1.4.2/adafruit_circuitpython_ili9341.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2023-12-18 17:07:46.000000 adafruit-circuitpython-ili9341-1.4.2/adafruit_ili9341.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 17:07:52.769269 adafruit-circuitpython-ili9341-1.4.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 17:07:52.773269 adafruit-circuitpython-ili9341-1.4.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2023-12-18 17:07:39.000000 adafruit-circuitpython-ili9341-1.4.2/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-12-18 17:07:39.000000 adafruit-circuitpython-ili9341-1.4.2/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      266 2023-12-18 17:07:39.000000 adafruit-circuitpython-ili9341-1.4.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-18 17:07:39.000000 adafruit-circuitpython-ili9341-1.4.2/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5406 2023-12-18 17:07:39.000000 adafruit-circuitpython-ili9341-1.4.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2023-12-18 17:07:39.000000 adafruit-circuitpython-ili9341-1.4.2/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-18 17:07:39.000000 adafruit-circuitpython-ili9341-1.4.2/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2023-12-18 17:07:39.000000 adafruit-circuitpython-ili9341-1.4.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-18 17:07:39.000000 adafruit-circuitpython-ili9341-1.4.2/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-18 17:07:39.000000 adafruit-circuitpython-ili9341-1.4.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 17:07:52.773269 adafruit-circuitpython-ili9341-1.4.2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2023-12-18 17:07:46.000000 adafruit-circuitpython-ili9341-1.4.2/examples/ili9341_pitft_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2023-12-18 17:07:46.000000 adafruit-circuitpython-ili9341-1.4.2/examples/ili9341_shield_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2023-12-18 17:07:46.000000 adafruit-circuitpython-ili9341-1.4.2/examples/ili9341_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-18 17:07:39.000000 adafruit-circuitpython-ili9341-1.4.2/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2023-12-18 17:07:46.000000 adafruit-circuitpython-ili9341-1.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      151 2023-12-18 17:07:39.000000 adafruit-circuitpython-ili9341-1.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-18 17:07:52.773269 adafruit-circuitpython-ili9341-1.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:01:16.698433 adafruit_circuitpython_ili9341-1.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:01:16.690433 adafruit_circuitpython_ili9341-1.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:01:16.690433 adafruit_circuitpython_ili9341-1.5.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-06 21:01:08.000000 adafruit_circuitpython_ili9341-1.5.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:01:16.694433 adafruit_circuitpython_ili9341-1.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-06 21:01:08.000000 adafruit_circuitpython_ili9341-1.5.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-06 21:01:08.000000 adafruit_circuitpython_ili9341-1.5.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-06 21:01:08.000000 adafruit_circuitpython_ili9341-1.5.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-06 21:01:08.000000 adafruit_circuitpython_ili9341-1.5.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-06 21:01:08.000000 adafruit_circuitpython_ili9341-1.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-06 21:01:08.000000 adafruit_circuitpython_ili9341-1.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-06 21:01:08.000000 adafruit_circuitpython_ili9341-1.5.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-06 21:01:08.000000 adafruit_circuitpython_ili9341-1.5.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-05-06 21:01:08.000000 adafruit_circuitpython_ili9341-1.5.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-06 21:01:08.000000 adafruit_circuitpython_ili9341-1.5.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:01:16.694433 adafruit_circuitpython_ili9341-1.5.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-05-06 21:01:08.000000 adafruit_circuitpython_ili9341-1.5.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-06 21:01:08.000000 adafruit_circuitpython_ili9341-1.5.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-06 21:01:08.000000 adafruit_circuitpython_ili9341-1.5.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-05-06 21:01:16.698433 adafruit_circuitpython_ili9341-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-06 21:01:08.000000 adafruit_circuitpython_ili9341-1.5.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-06 21:01:08.000000 adafruit_circuitpython_ili9341-1.5.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:01:16.698433 adafruit_circuitpython_ili9341-1.5.0/adafruit_circuitpython_ili9341.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-05-06 21:01:16.000000 adafruit_circuitpython_ili9341-1.5.0/adafruit_circuitpython_ili9341.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-06 21:01:16.000000 adafruit_circuitpython_ili9341-1.5.0/adafruit_circuitpython_ili9341.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 21:01:16.000000 adafruit_circuitpython_ili9341-1.5.0/adafruit_circuitpython_ili9341.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-06 21:01:16.000000 adafruit_circuitpython_ili9341-1.5.0/adafruit_circuitpython_ili9341.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-06 21:01:16.000000 adafruit_circuitpython_ili9341-1.5.0/adafruit_circuitpython_ili9341.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-05-06 21:01:14.000000 adafruit_circuitpython_ili9341-1.5.0/adafruit_ili9341.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:01:16.694433 adafruit_circuitpython_ili9341-1.5.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:01:16.694433 adafruit_circuitpython_ili9341-1.5.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-06 21:01:08.000000 adafruit_circuitpython_ili9341-1.5.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-06 21:01:08.000000 adafruit_circuitpython_ili9341-1.5.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-06 21:01:08.000000 adafruit_circuitpython_ili9341-1.5.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-06 21:01:08.000000 adafruit_circuitpython_ili9341-1.5.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-05-06 21:01:08.000000 adafruit_circuitpython_ili9341-1.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-06 21:01:08.000000 adafruit_circuitpython_ili9341-1.5.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-06 21:01:08.000000 adafruit_circuitpython_ili9341-1.5.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-06 21:01:08.000000 adafruit_circuitpython_ili9341-1.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-06 21:01:08.000000 adafruit_circuitpython_ili9341-1.5.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-06 21:01:08.000000 adafruit_circuitpython_ili9341-1.5.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:01:16.698433 adafruit_circuitpython_ili9341-1.5.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-06 21:01:14.000000 adafruit_circuitpython_ili9341-1.5.0/examples/ili9341_pitft_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-06 21:01:14.000000 adafruit_circuitpython_ili9341-1.5.0/examples/ili9341_shield_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-06 21:01:14.000000 adafruit_circuitpython_ili9341-1.5.0/examples/ili9341_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-06 21:01:08.000000 adafruit_circuitpython_ili9341-1.5.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-06 21:01:14.000000 adafruit_circuitpython_ili9341-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-06 21:01:08.000000 adafruit_circuitpython_ili9341-1.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 21:01:16.698433 adafruit_circuitpython_ili9341-1.5.0/setup.cfg
```

### Comparing `adafruit-circuitpython-ili9341-1.4.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit_circuitpython_ili9341-1.5.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ili9341-1.4.2/.gitignore` & `adafruit_circuitpython_ili9341-1.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ili9341-1.4.2/.pre-commit-config.yaml` & `adafruit_circuitpython_ili9341-1.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ili9341-1.4.2/.pylintrc` & `adafruit_circuitpython_ili9341-1.5.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ili9341-1.4.2/CODE_OF_CONDUCT.md` & `adafruit_circuitpython_ili9341-1.5.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ili9341-1.4.2/LICENSE` & `adafruit_circuitpython_ili9341-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ili9341-1.4.2/LICENSES/CC-BY-4.0.txt` & `adafruit_circuitpython_ili9341-1.5.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ili9341-1.4.2/LICENSES/MIT.txt` & `adafruit_circuitpython_ili9341-1.5.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ili9341-1.4.2/LICENSES/Unlicense.txt` & `adafruit_circuitpython_ili9341-1.5.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ili9341-1.4.2/PKG-INFO` & `adafruit_circuitpython_ili9341-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ili9341
-Version: 1.4.2
+Version: 1.5.0
 Summary: displayio driver for ILI9341 and ILI9340 TFT-LCD displays.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ili9341
 Keywords: adafruit,blinka,circuitpython,micropython,ili9341,display,tft,lcd,displayio
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ili9341-1.4.2/README.rst` & `adafruit_circuitpython_ili9341-1.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ili9341-1.4.2/adafruit_circuitpython_ili9341.egg-info/PKG-INFO` & `adafruit_circuitpython_ili9341-1.5.0/adafruit_circuitpython_ili9341.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ili9341
-Version: 1.4.2
+Version: 1.5.0
 Summary: displayio driver for ILI9341 and ILI9340 TFT-LCD displays.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ili9341
 Keywords: adafruit,blinka,circuitpython,micropython,ili9341,display,tft,lcd,displayio
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ili9341-1.4.2/adafruit_circuitpython_ili9341.egg-info/SOURCES.txt` & `adafruit_circuitpython_ili9341-1.5.0/adafruit_circuitpython_ili9341.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ili9341-1.4.2/adafruit_ili9341.py` & `adafruit_circuitpython_ili9341-1.5.0/adafruit_ili9341.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 try:
     from fourwire import FourWire
     from busdisplay import BusDisplay
 except ImportError:
     from displayio import FourWire
     from displayio import Display as BusDisplay
 
-__version__ = "1.4.2"
+__version__ = "1.5.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ILI9341.git"
 
 _INIT_SEQUENCE = (
     b"\x01\x80\x80"  # Software reset then delay 0x80 (128ms)
     b"\xEF\x03\x03\x80\x02"
     b"\xCF\x03\x00\xC1\x30"
     b"\xED\x04\x64\x03\x12\x81"
@@ -72,15 +72,14 @@
     b"\xCB\x05\x39\x2C\x00\x34\x02"
     b"\xF7\x01\x20"
     b"\xEA\x02\x00\x00"
     b"\xc0\x01\x23"  # Power control VRH[5:0]
     b"\xc1\x01\x10"  # Power control SAP[2:0];BT[3:0]
     b"\xc5\x02\x3e\x28"  # VCM control
     b"\xc7\x01\x86"  # VCM control2
-    b"\x36\x01\x38"  # Memory Access Control
     b"\x37\x01\x00"  # Vertical scroll zero
     b"\x3a\x01\x55"  # COLMOD: Pixel Format Set
     b"\xb1\x02\x00\x18"  # Frame Rate Control (In Normal Mode/Full Colors)
     b"\xb6\x03\x08\x82\x27"  # Display Function Control
     b"\xF2\x01\x00"  # 3Gamma Function Disable
     b"\x26\x01\x01"  # Gamma curve selected
     b"\xe0\x0f\x0F\x31\x2B\x0C\x0E\x08\x4E\xF1\x37\x07\x10\x03\x0E\x09\x00"  # Set Gamma
@@ -94,9 +93,23 @@
 class ILI9341(BusDisplay):
     """
     ILI9341 display driver
 
     :param FourWire bus: bus that the display is connected to
     """
 
-    def __init__(self, bus: FourWire, **kwargs: Any):
-        super().__init__(bus, _INIT_SEQUENCE, **kwargs)
+    def __init__(
+        self, bus: FourWire, *, bgr: bool = False, invert: bool = False, **kwargs: Any
+    ):
+        init_sequence = _INIT_SEQUENCE
+        if bgr:
+            init_sequence += (
+                b"\x36\x01\x30"  # _MADCTL Default rotation plus BGR encoding
+            )
+        else:
+            init_sequence += (
+                b"\x36\x01\x38"  # _MADCTL Default rotation plus RGB encoding
+            )
+        if invert:
+            init_sequence += b"\x21\x00"  # _INVON
+
+        super().__init__(bus, init_sequence, **kwargs)
```

### Comparing `adafruit-circuitpython-ili9341-1.4.2/docs/_static/favicon.ico` & `adafruit_circuitpython_ili9341-1.5.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ili9341-1.4.2/docs/conf.py` & `adafruit_circuitpython_ili9341-1.5.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     "sphinx.ext.todo",
 ]
 
 # TODO: Please Read!
 # Uncomment the below if you use native CircuitPython modules such as
 # digitalio, micropython and busio. List the modules you use. Without it, the
 # autodoc module docs will fail to generate with a warning.
-# autodoc_mock_imports = ["digitalio", "busio"]
+autodoc_mock_imports = ["displayio"]
 
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3", None),
     "CircuitPython": ("https://docs.circuitpython.org/en/latest/", None),
 }
 
 # Add any paths that contain templates here, relative to this directory.
```

### Comparing `adafruit-circuitpython-ili9341-1.4.2/docs/index.rst` & `adafruit_circuitpython_ili9341-1.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ili9341-1.4.2/examples/ili9341_pitft_simpletest.py` & `adafruit_circuitpython_ili9341-1.5.0/examples/ili9341_pitft_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ili9341-1.4.2/examples/ili9341_shield_simpletest.py` & `adafruit_circuitpython_ili9341-1.5.0/examples/ili9341_shield_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ili9341-1.4.2/examples/ili9341_simpletest.py` & `adafruit_circuitpython_ili9341-1.5.0/examples/ili9341_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ili9341-1.4.2/pyproject.toml` & `adafruit_circuitpython_ili9341-1.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-ili9341"
 description = "displayio driver for ILI9341 and ILI9340 TFT-LCD displays."
-version = "1.4.2"
+version = "1.5.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_ili9341"}
 keywords = [
     "adafruit",
```

