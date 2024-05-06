# Comparing `tmp/pollination-honeybee-energy-0.7.7.tar.gz` & `tmp/pollination-honeybee-energy-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pollination-honeybee-energy-0.7.7.tar", last modified: Tue Mar  5 23:26:11 2024, max compression
+gzip compressed data, was "dist/pollination-honeybee-energy-0.7.8.tar", last modified: Mon May  6 16:56:52 2024, max compression
```

## Comparing `pollination-honeybee-energy-0.7.7.tar` & `pollination-honeybee-energy-0.7.8.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 23:26:11.000000 pollination-honeybee-energy-0.7.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 23:26:11.000000 pollination-honeybee-energy-0.7.7/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-05 23:25:19.000000 pollination-honeybee-energy-0.7.7/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 23:26:11.000000 pollination-honeybee-energy-0.7.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-03-05 23:25:19.000000 pollination-honeybee-energy-0.7.7/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-03-05 23:25:19.000000 pollination-honeybee-energy-0.7.7/.github/workflows/dependency-release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-05 23:25:19.000000 pollination-honeybee-energy-0.7.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-05 23:25:19.000000 pollination-honeybee-energy-0.7.7/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-03-05 23:25:19.000000 pollination-honeybee-energy-0.7.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-03-05 23:26:11.000000 pollination-honeybee-energy-0.7.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-03-05 23:25:19.000000 pollination-honeybee-energy-0.7.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-05 23:25:19.000000 pollination-honeybee-energy-0.7.7/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-05 23:25:19.000000 pollination-honeybee-energy-0.7.7/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 23:26:11.000000 pollination-honeybee-energy-0.7.7/pollination/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 23:26:11.000000 pollination-honeybee-energy-0.7.7/pollination/honeybee_energy/
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-03-05 23:25:19.000000 pollination-honeybee-energy-0.7.7/pollination/honeybee_energy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13029 2024-03-05 23:25:19.000000 pollination-honeybee-energy-0.7.7/pollination/honeybee_energy/baseline.py
--rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-03-05 23:25:19.000000 pollination-honeybee-energy-0.7.7/pollination/honeybee_energy/result.py
--rw-r--r--   0 runner    (1001) docker     (127)    11428 2024-03-05 23:25:19.000000 pollination-honeybee-energy-0.7.7/pollination/honeybee_energy/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    11333 2024-03-05 23:25:19.000000 pollination-honeybee-energy-0.7.7/pollination/honeybee_energy/simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-03-05 23:25:19.000000 pollination-honeybee-energy-0.7.7/pollination/honeybee_energy/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 23:26:11.000000 pollination-honeybee-energy-0.7.7/pollination_honeybee_energy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-03-05 23:26:11.000000 pollination-honeybee-energy-0.7.7/pollination_honeybee_energy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-03-05 23:26:11.000000 pollination-honeybee-energy-0.7.7/pollination_honeybee_energy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 23:26:11.000000 pollination-honeybee-energy-0.7.7/pollination_honeybee_energy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 23:25:38.000000 pollination-honeybee-energy-0.7.7/pollination_honeybee_energy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-05 23:26:11.000000 pollination-honeybee-energy-0.7.7/pollination_honeybee_energy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-05 23:26:11.000000 pollination-honeybee-energy-0.7.7/pollination_honeybee_energy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-05 23:25:19.000000 pollination-honeybee-energy-0.7.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-05 23:26:11.000000 pollination-honeybee-energy-0.7.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-03-05 23:25:19.000000 pollination-honeybee-energy-0.7.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 23:26:11.000000 pollination-honeybee-energy-0.7.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 23:25:19.000000 pollination-honeybee-energy-0.7.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-05 23:25:19.000000 pollination-honeybee-energy-0.7.7/tests/baseline_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-03-05 23:25:19.000000 pollination-honeybee-energy-0.7.7/tests/result_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-03-05 23:25:19.000000 pollination-honeybee-energy-0.7.7/tests/settings_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-05 23:25:19.000000 pollination-honeybee-energy-0.7.7/tests/simulate_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-03-05 23:25:19.000000 pollination-honeybee-energy-0.7.7/tests/translate_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:56:52.000000 pollination-honeybee-energy-0.7.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:56:52.000000 pollination-honeybee-energy-0.7.8/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-06 16:55:59.000000 pollination-honeybee-energy-0.7.8/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:56:52.000000 pollination-honeybee-energy-0.7.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-05-06 16:55:59.000000 pollination-honeybee-energy-0.7.8/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-06 16:55:59.000000 pollination-honeybee-energy-0.7.8/.github/workflows/dependency-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-06 16:55:59.000000 pollination-honeybee-energy-0.7.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-06 16:55:59.000000 pollination-honeybee-energy-0.7.8/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-05-06 16:55:59.000000 pollination-honeybee-energy-0.7.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-06 16:56:52.000000 pollination-honeybee-energy-0.7.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-06 16:55:59.000000 pollination-honeybee-energy-0.7.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-06 16:55:59.000000 pollination-honeybee-energy-0.7.8/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-06 16:55:59.000000 pollination-honeybee-energy-0.7.8/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:56:52.000000 pollination-honeybee-energy-0.7.8/pollination/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:56:52.000000 pollination-honeybee-energy-0.7.8/pollination/honeybee_energy/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-06 16:55:59.000000 pollination-honeybee-energy-0.7.8/pollination/honeybee_energy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13029 2024-05-06 16:55:59.000000 pollination-honeybee-energy-0.7.8/pollination/honeybee_energy/baseline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-05-06 16:55:59.000000 pollination-honeybee-energy-0.7.8/pollination/honeybee_energy/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11428 2024-05-06 16:55:59.000000 pollination-honeybee-energy-0.7.8/pollination/honeybee_energy/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11333 2024-05-06 16:55:59.000000 pollination-honeybee-energy-0.7.8/pollination/honeybee_energy/simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-06 16:55:59.000000 pollination-honeybee-energy-0.7.8/pollination/honeybee_energy/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:56:52.000000 pollination-honeybee-energy-0.7.8/pollination_honeybee_energy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-06 16:56:51.000000 pollination-honeybee-energy-0.7.8/pollination_honeybee_energy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-06 16:56:52.000000 pollination-honeybee-energy-0.7.8/pollination_honeybee_energy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:56:51.000000 pollination-honeybee-energy-0.7.8/pollination_honeybee_energy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:56:15.000000 pollination-honeybee-energy-0.7.8/pollination_honeybee_energy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-06 16:56:51.000000 pollination-honeybee-energy-0.7.8/pollination_honeybee_energy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-06 16:56:51.000000 pollination-honeybee-energy-0.7.8/pollination_honeybee_energy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-06 16:55:59.000000 pollination-honeybee-energy-0.7.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-06 16:56:52.000000 pollination-honeybee-energy-0.7.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-06 16:55:59.000000 pollination-honeybee-energy-0.7.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:56:52.000000 pollination-honeybee-energy-0.7.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:55:59.000000 pollination-honeybee-energy-0.7.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-06 16:55:59.000000 pollination-honeybee-energy-0.7.8/tests/baseline_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-06 16:55:59.000000 pollination-honeybee-energy-0.7.8/tests/result_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-06 16:55:59.000000 pollination-honeybee-energy-0.7.8/tests/settings_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-06 16:55:59.000000 pollination-honeybee-energy-0.7.8/tests/simulate_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-06 16:55:59.000000 pollination-honeybee-energy-0.7.8/tests/translate_test.py
```

### Comparing `pollination-honeybee-energy-0.7.7/.github/workflows/ci.yaml` & `pollination-honeybee-energy-0.7.8/.github/workflows/ci.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     runs-on: ${{ matrix.os }}
     steps:
       - uses: actions/checkout@v2
       - name: set up Python
         uses: actions/setup-python@v2
         with:
-          python-version: 3.7
+          python-version: '3.10'
       - name: install python dependencies
         run: |
           pip install -r dev-requirements.txt
           pip install .
       - name: run tests
         run: python -m pytest tests/
```

### Comparing `pollination-honeybee-energy-0.7.7/.github/workflows/dependency-release.yaml` & `pollination-honeybee-energy-0.7.8/.github/workflows/dependency-release.yaml`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-energy-0.7.7/LICENSE` & `pollination-honeybee-energy-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-energy-0.7.7/PKG-INFO` & `pollination-honeybee-energy-0.7.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-honeybee-energy
-Version: 0.7.7
+Version: 0.7.8
 Summary: Honeybee energy plugin for Pollination.
 Home-page: https://github.com/pollination/honeybee-energy
 Author: ladybug-tools
 Author-email: chris@ladybug.tools
 Maintainer: Chris, ladybug-tools
 Maintainer-email: chris@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-honeybee-energy-0.7.7/README.md` & `pollination-honeybee-energy-0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-energy-0.7.7/pollination/honeybee_energy/baseline.py` & `pollination-honeybee-energy-0.7.8/pollination/honeybee_energy/baseline.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-energy-0.7.7/pollination/honeybee_energy/result.py` & `pollination-honeybee-energy-0.7.8/pollination/honeybee_energy/result.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-energy-0.7.7/pollination/honeybee_energy/settings.py` & `pollination-honeybee-energy-0.7.8/pollination/honeybee_energy/settings.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-energy-0.7.7/pollination/honeybee_energy/simulate.py` & `pollination-honeybee-energy-0.7.8/pollination/honeybee_energy/simulate.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-energy-0.7.7/pollination/honeybee_energy/translate.py` & `pollination-honeybee-energy-0.7.8/pollination/honeybee_energy/translate.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-energy-0.7.7/pollination_honeybee_energy.egg-info/PKG-INFO` & `pollination-honeybee-energy-0.7.8/pollination_honeybee_energy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-honeybee-energy
-Version: 0.7.7
+Version: 0.7.8
 Summary: Honeybee energy plugin for Pollination.
 Home-page: https://github.com/pollination/honeybee-energy
 Author: ladybug-tools
 Author-email: chris@ladybug.tools
 Maintainer: Chris, ladybug-tools
 Maintainer-email: chris@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-honeybee-energy-0.7.7/pollination_honeybee_energy.egg-info/SOURCES.txt` & `pollination-honeybee-energy-0.7.8/pollination_honeybee_energy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-energy-0.7.7/setup.py` & `pollination-honeybee-energy-0.7.8/setup.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-energy-0.7.7/tests/baseline_test.py` & `pollination-honeybee-energy-0.7.8/tests/baseline_test.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-energy-0.7.7/tests/result_test.py` & `pollination-honeybee-energy-0.7.8/tests/result_test.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-energy-0.7.7/tests/settings_test.py` & `pollination-honeybee-energy-0.7.8/tests/settings_test.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-energy-0.7.7/tests/simulate_test.py` & `pollination-honeybee-energy-0.7.8/tests/simulate_test.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-energy-0.7.7/tests/translate_test.py` & `pollination-honeybee-energy-0.7.8/tests/translate_test.py`

 * *Files identical despite different names*

