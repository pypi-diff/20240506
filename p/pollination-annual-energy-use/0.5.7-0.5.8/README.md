# Comparing `tmp/pollination-annual-energy-use-0.5.7.tar.gz` & `tmp/pollination-annual-energy-use-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pollination-annual-energy-use-0.5.7.tar", last modified: Wed Mar  6 00:18:08 2024, max compression
+gzip compressed data, was "dist/pollination-annual-energy-use-0.5.8.tar", last modified: Mon May  6 18:46:38 2024, max compression
```

## Comparing `pollination-annual-energy-use-0.5.7.tar` & `pollination-annual-energy-use-0.5.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 00:18:08.000000 pollination-annual-energy-use-0.5.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 00:18:08.000000 pollination-annual-energy-use-0.5.7/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-06 00:17:13.000000 pollination-annual-energy-use-0.5.7/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 00:18:08.000000 pollination-annual-energy-use-0.5.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-03-06 00:17:13.000000 pollination-annual-energy-use-0.5.7/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-03-06 00:17:13.000000 pollination-annual-energy-use-0.5.7/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-06 00:17:13.000000 pollination-annual-energy-use-0.5.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-06 00:17:13.000000 pollination-annual-energy-use-0.5.7/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-03-06 00:17:13.000000 pollination-annual-energy-use-0.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-03-06 00:18:08.000000 pollination-annual-energy-use-0.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-03-06 00:17:13.000000 pollination-annual-energy-use-0.5.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-06 00:17:13.000000 pollination-annual-energy-use-0.5.7/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-06 00:17:13.000000 pollination-annual-energy-use-0.5.7/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 00:18:08.000000 pollination-annual-energy-use-0.5.7/pollination/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 00:18:08.000000 pollination-annual-energy-use-0.5.7/pollination/annual_energy_use/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-06 00:17:13.000000 pollination-annual-energy-use-0.5.7/pollination/annual_energy_use/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-03-06 00:17:13.000000 pollination-annual-energy-use-0.5.7/pollination/annual_energy_use/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 00:18:08.000000 pollination-annual-energy-use-0.5.7/pollination_annual_energy_use.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-03-06 00:18:08.000000 pollination-annual-energy-use-0.5.7/pollination_annual_energy_use.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-06 00:18:08.000000 pollination-annual-energy-use-0.5.7/pollination_annual_energy_use.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 00:18:08.000000 pollination-annual-energy-use-0.5.7/pollination_annual_energy_use.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 00:17:36.000000 pollination-annual-energy-use-0.5.7/pollination_annual_energy_use.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-06 00:18:08.000000 pollination-annual-energy-use-0.5.7/pollination_annual_energy_use.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-06 00:18:08.000000 pollination-annual-energy-use-0.5.7/pollination_annual_energy_use.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-06 00:17:13.000000 pollination-annual-energy-use-0.5.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-06 00:18:08.000000 pollination-annual-energy-use-0.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-03-06 00:17:13.000000 pollination-annual-energy-use-0.5.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 00:18:08.000000 pollination-annual-energy-use-0.5.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 00:17:13.000000 pollination-annual-energy-use-0.5.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-06 00:17:13.000000 pollination-annual-energy-use-0.5.7/tests/validation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:46:38.000000 pollination-annual-energy-use-0.5.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:46:38.000000 pollination-annual-energy-use-0.5.8/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-06 18:45:41.000000 pollination-annual-energy-use-0.5.8/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:46:38.000000 pollination-annual-energy-use-0.5.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-06 18:45:41.000000 pollination-annual-energy-use-0.5.8/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-06 18:45:41.000000 pollination-annual-energy-use-0.5.8/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-06 18:45:41.000000 pollination-annual-energy-use-0.5.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-06 18:45:41.000000 pollination-annual-energy-use-0.5.8/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-05-06 18:45:41.000000 pollination-annual-energy-use-0.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-06 18:46:38.000000 pollination-annual-energy-use-0.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-06 18:45:41.000000 pollination-annual-energy-use-0.5.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-06 18:45:41.000000 pollination-annual-energy-use-0.5.8/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-06 18:45:41.000000 pollination-annual-energy-use-0.5.8/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:46:38.000000 pollination-annual-energy-use-0.5.8/pollination/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:46:38.000000 pollination-annual-energy-use-0.5.8/pollination/annual_energy_use/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-06 18:45:41.000000 pollination-annual-energy-use-0.5.8/pollination/annual_energy_use/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-05-06 18:45:41.000000 pollination-annual-energy-use-0.5.8/pollination/annual_energy_use/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:46:38.000000 pollination-annual-energy-use-0.5.8/pollination_annual_energy_use.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-06 18:46:38.000000 pollination-annual-energy-use-0.5.8/pollination_annual_energy_use.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-06 18:46:38.000000 pollination-annual-energy-use-0.5.8/pollination_annual_energy_use.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 18:46:38.000000 pollination-annual-energy-use-0.5.8/pollination_annual_energy_use.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 18:46:01.000000 pollination-annual-energy-use-0.5.8/pollination_annual_energy_use.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-06 18:46:38.000000 pollination-annual-energy-use-0.5.8/pollination_annual_energy_use.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-06 18:46:38.000000 pollination-annual-energy-use-0.5.8/pollination_annual_energy_use.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-06 18:45:41.000000 pollination-annual-energy-use-0.5.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-06 18:46:38.000000 pollination-annual-energy-use-0.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-06 18:45:41.000000 pollination-annual-energy-use-0.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:46:38.000000 pollination-annual-energy-use-0.5.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 18:45:41.000000 pollination-annual-energy-use-0.5.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-06 18:45:41.000000 pollination-annual-energy-use-0.5.8/tests/validation_test.py
```

### Comparing `pollination-annual-energy-use-0.5.7/.github/workflows/ci.yaml` & `pollination-annual-energy-use-0.5.8/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pollination-annual-energy-use-0.5.7/.github/workflows/tests.yaml` & `pollination-annual-energy-use-0.5.8/.github/workflows/tests.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,14 @@
 
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

### Comparing `pollination-annual-energy-use-0.5.7/LICENSE` & `pollination-annual-energy-use-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pollination-annual-energy-use-0.5.7/PKG-INFO` & `pollination-annual-energy-use-0.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-annual-energy-use
-Version: 0.5.7
+Version: 0.5.8
 Summary: Run an annual energy simulation and compute energy use intensity.
 Home-page: https://github.com/pollination/annual-energy-use
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: chris, ladybug-tools
 Maintainer-email: chris@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-annual-energy-use-0.5.7/pollination/annual_energy_use/entry.py` & `pollination-annual-energy-use-0.5.8/pollination/annual_energy_use/entry.py`

 * *Files identical despite different names*

### Comparing `pollination-annual-energy-use-0.5.7/pollination_annual_energy_use.egg-info/PKG-INFO` & `pollination-annual-energy-use-0.5.8/pollination_annual_energy_use.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-annual-energy-use
-Version: 0.5.7
+Version: 0.5.8
 Summary: Run an annual energy simulation and compute energy use intensity.
 Home-page: https://github.com/pollination/annual-energy-use
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: chris, ladybug-tools
 Maintainer-email: chris@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-annual-energy-use-0.5.7/pollination_annual_energy_use.egg-info/SOURCES.txt` & `pollination-annual-energy-use-0.5.8/pollination_annual_energy_use.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pollination-annual-energy-use-0.5.7/setup.py` & `pollination-annual-energy-use-0.5.8/setup.py`

 * *Files identical despite different names*

