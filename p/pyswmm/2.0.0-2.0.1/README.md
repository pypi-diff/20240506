# Comparing `tmp/pyswmm-2.0.0.tar.gz` & `tmp/pyswmm-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyswmm-2.0.0.tar", last modified: Wed Feb  7 03:05:56 2024, max compression
+gzip compressed data, was "pyswmm-2.0.1.tar", last modified: Mon May  6 03:38:28 2024, max compression
```

## Comparing `pyswmm-2.0.0.tar` & `pyswmm-2.0.1.tar`

### file list

```diff
@@ -1,69 +1,67 @@
-drwxr-xr-x   0 bryant     (501) staff       (20)        0 2024-02-07 03:05:56.347708 pyswmm-2.0.0/
--rw-r--r--   0 bryant     (501) staff       (20)      625 2023-11-28 00:00:14.000000 pyswmm-2.0.0/AUTHORS
--rw-r--r--   0 bryant     (501) staff       (20)    17432 2024-02-07 02:58:13.000000 pyswmm-2.0.0/CHANGELOG.md
--rw-r--r--   0 bryant     (501) staff       (20)     1343 2024-02-07 02:58:13.000000 pyswmm-2.0.0/LICENSE.txt
--rw-r--r--   0 bryant     (501) staff       (20)       60 2022-04-01 19:49:46.000000 pyswmm-2.0.0/MANIFEST.in
--rw-r--r--   0 bryant     (501) staff       (20)     7972 2024-02-07 03:05:56.346885 pyswmm-2.0.0/PKG-INFO
--rw-r--r--   0 bryant     (501) staff       (20)     6250 2024-02-07 02:58:13.000000 pyswmm-2.0.0/README.md
-drwxr-xr-x   0 bryant     (501) staff       (20)        0 2024-02-07 03:05:56.304858 pyswmm-2.0.0/pyswmm/
--rw-r--r--   0 bryant     (501) staff       (20)     1440 2024-02-07 02:58:13.000000 pyswmm-2.0.0/pyswmm/__init__.py
--rw-r--r--   0 bryant     (501) staff       (20)     5162 2024-02-07 02:58:13.000000 pyswmm-2.0.0/pyswmm/_monkey_patch.py
--rw-r--r--   0 bryant     (501) staff       (20)      882 2024-01-24 15:54:28.000000 pyswmm-2.0.0/pyswmm/config.py
--rw-r--r--   0 bryant     (501) staff       (20)     1083 2024-02-07 02:58:13.000000 pyswmm-2.0.0/pyswmm/errors.py
--rw-r--r--   0 bryant     (501) staff       (20)     6650 2024-02-07 02:58:13.000000 pyswmm-2.0.0/pyswmm/lidcontrols.py
--rw-r--r--   0 bryant     (501) staff       (20)    22142 2024-02-07 02:58:13.000000 pyswmm-2.0.0/pyswmm/lidgroups.py
--rw-r--r--   0 bryant     (501) staff       (20)    37395 2024-02-07 02:58:13.000000 pyswmm-2.0.0/pyswmm/lidlayers.py
--rw-r--r--   0 bryant     (501) staff       (20)    11439 2022-04-01 19:49:46.000000 pyswmm-2.0.0/pyswmm/lidunits.py
--rw-r--r--   0 bryant     (501) staff       (20)    31707 2023-11-28 00:00:14.000000 pyswmm-2.0.0/pyswmm/links.py
--rw-r--r--   0 bryant     (501) staff       (20)    26165 2023-11-28 00:00:14.000000 pyswmm-2.0.0/pyswmm/nodes.py
--rw-r--r--   0 bryant     (501) staff       (20)    45787 2024-02-07 02:58:13.000000 pyswmm-2.0.0/pyswmm/output.py
--rw-r--r--   0 bryant     (501) staff       (20)     6615 2023-11-28 00:00:14.000000 pyswmm-2.0.0/pyswmm/raingages.py
--rw-r--r--   0 bryant     (501) staff       (20)    29182 2022-04-01 19:49:46.000000 pyswmm-2.0.0/pyswmm/reader.py
--rw-r--r--   0 bryant     (501) staff       (20)    31514 2024-02-07 02:58:13.000000 pyswmm-2.0.0/pyswmm/simulation.py
--rw-r--r--   0 bryant     (501) staff       (20)    20644 2023-11-28 00:00:14.000000 pyswmm-2.0.0/pyswmm/subcatchments.py
--rw-r--r--   0 bryant     (501) staff       (20)    52074 2024-02-07 02:58:13.000000 pyswmm-2.0.0/pyswmm/swmm5.py
--rw-r--r--   0 bryant     (501) staff       (20)     3222 2023-11-28 00:00:14.000000 pyswmm-2.0.0/pyswmm/system.py
-drwxr-xr-x   0 bryant     (501) staff       (20)        0 2024-02-07 03:05:56.322897 pyswmm-2.0.0/pyswmm/tests/
--rw-r--r--   0 bryant     (501) staff       (20)      346 2022-04-01 19:49:46.000000 pyswmm-2.0.0/pyswmm/tests/__init__.py
-drwxr-xr-x   0 bryant     (501) staff       (20)        0 2024-02-07 03:05:56.341356 pyswmm-2.0.0/pyswmm/tests/data/
--rw-r--r--   0 bryant     (501) staff       (20)     1982 2023-11-28 00:00:14.000000 pyswmm-2.0.0/pyswmm/tests/data/__init__.py
--rw-r--r--   0 bryant     (501) staff       (20)    13531 2022-04-01 19:49:46.000000 pyswmm-2.0.0/pyswmm/tests/data/model_bad_input_1.inp
--rw-r--r--   0 bryant     (501) staff       (20)     4829 2023-11-28 00:00:14.000000 pyswmm-2.0.0/pyswmm/tests/data/model_constantinflow_constanteffluent.inp
--rw-r--r--   0 bryant     (501) staff       (20)    13531 2022-04-01 19:49:46.000000 pyswmm-2.0.0/pyswmm/tests/data/model_full_features.inp
--rw-r--r--   0 bryant     (501) staff       (20)    19277 2022-04-01 19:49:46.000000 pyswmm-2.0.0/pyswmm/tests/data/model_lids.inp
--rw-r--r--   0 bryant     (501) staff       (20)     9264 2022-04-01 19:49:46.000000 pyswmm-2.0.0/pyswmm/tests/data/model_node_inflows.inp
--rw-r--r--   0 bryant     (501) staff       (20)    14013 2022-04-01 19:49:46.000000 pyswmm-2.0.0/pyswmm/tests/data/model_pollutants.inp
--rw-r--r--   0 bryant     (501) staff       (20)    14013 2023-11-28 00:00:14.000000 pyswmm-2.0.0/pyswmm/tests/data/model_pollutants_2.inp
--rw-r--r--   0 bryant     (501) staff       (20)     3606 2023-11-28 00:00:14.000000 pyswmm-2.0.0/pyswmm/tests/data/model_pollutants_setters.inp
--rw-r--r--   0 bryant     (501) staff       (20)    13019 2022-04-01 19:49:46.000000 pyswmm-2.0.0/pyswmm/tests/data/model_pump_setting.inp
--rwxr-xr-x   0 bryant     (501) staff       (20)     6079 2022-04-01 19:49:46.000000 pyswmm-2.0.0/pyswmm/tests/data/model_rain.inp
--rw-r--r--   0 bryant     (501) staff       (20)    12675 2022-04-01 19:49:46.000000 pyswmm-2.0.0/pyswmm/tests/data/model_storage_pump.inp
--rw-r--r--   0 bryant     (501) staff       (20)    12675 2022-04-01 19:49:46.000000 pyswmm-2.0.0/pyswmm/tests/data/model_storage_pump_MGD.inp
--rw-r--r--   0 bryant     (501) staff       (20)     9009 2022-04-01 19:49:46.000000 pyswmm-2.0.0/pyswmm/tests/data/model_subcatch_stats.inp
--rw-r--r--   0 bryant     (501) staff       (20)     9264 2022-04-01 19:49:46.000000 pyswmm-2.0.0/pyswmm/tests/data/model_toolkit_units.inp
--rw-r--r--   0 bryant     (501) staff       (20)    13325 2022-04-01 19:49:46.000000 pyswmm-2.0.0/pyswmm/tests/data/model_weir_setting.inp
--rw-r--r--   0 bryant     (501) staff       (20)    12773 2024-02-06 21:20:37.000000 pyswmm-2.0.0/pyswmm/tests/data/model_weir_setting_a.inp
--rw-r--r--   0 bryant     (501) staff       (20)      967 2022-04-01 19:49:46.000000 pyswmm-2.0.0/pyswmm/tests/test_current_time.py
--rw-r--r--   0 bryant     (501) staff       (20)     1884 2022-04-01 19:49:46.000000 pyswmm-2.0.0/pyswmm/tests/test_errors.py
--rw-r--r--   0 bryant     (501) staff       (20)     1736 2024-02-07 02:58:13.000000 pyswmm-2.0.0/pyswmm/tests/test_general_engine.py
--rw-r--r--   0 bryant     (501) staff       (20)     9793 2022-04-01 19:49:46.000000 pyswmm-2.0.0/pyswmm/tests/test_lid.py
--rw-r--r--   0 bryant     (501) staff       (20)     7303 2022-04-01 19:49:46.000000 pyswmm-2.0.0/pyswmm/tests/test_links.py
--rw-r--r--   0 bryant     (501) staff       (20)    10762 2022-04-01 19:49:46.000000 pyswmm-2.0.0/pyswmm/tests/test_nodes.py
--rw-r--r--   0 bryant     (501) staff       (20)     4987 2024-02-07 02:58:13.000000 pyswmm-2.0.0/pyswmm/tests/test_output.py
--rw-r--r--   0 bryant     (501) staff       (20)     4722 2023-11-28 01:24:25.000000 pyswmm-2.0.0/pyswmm/tests/test_pollutants.py
--rw-r--r--   0 bryant     (501) staff       (20)     1233 2022-04-01 19:49:46.000000 pyswmm-2.0.0/pyswmm/tests/test_rainfallAPI.py
--rw-r--r--   0 bryant     (501) staff       (20)     6940 2024-02-07 02:58:13.000000 pyswmm-2.0.0/pyswmm/tests/test_simulation.py
--rw-r--r--   0 bryant     (501) staff       (20)     2783 2022-04-01 19:49:46.000000 pyswmm-2.0.0/pyswmm/tests/test_subcatchments.py
--rw-r--r--   0 bryant     (501) staff       (20)     1174 2022-04-01 19:49:46.000000 pyswmm-2.0.0/pyswmm/tests/test_system.py
--rw-r--r--   0 bryant     (501) staff       (20)    16277 2023-11-28 01:24:25.000000 pyswmm-2.0.0/pyswmm/toolkitapi.py
-drwxr-xr-x   0 bryant     (501) staff       (20)        0 2024-02-07 03:05:56.343340 pyswmm-2.0.0/pyswmm/utils/
--rw-r--r--   0 bryant     (501) staff       (20)      325 2022-04-01 19:49:46.000000 pyswmm-2.0.0/pyswmm/utils/__init__.py
--rw-r--r--   0 bryant     (501) staff       (20)      598 2022-04-01 19:49:46.000000 pyswmm-2.0.0/pyswmm/utils/fixtures.py
-drwxr-xr-x   0 bryant     (501) staff       (20)        0 2024-02-07 03:05:56.344285 pyswmm-2.0.0/pyswmm.egg-info/
--rw-r--r--   0 bryant     (501) staff       (20)     7972 2024-02-07 03:05:56.000000 pyswmm-2.0.0/pyswmm.egg-info/PKG-INFO
--rw-r--r--   0 bryant     (501) staff       (20)     1697 2024-02-07 03:05:56.000000 pyswmm-2.0.0/pyswmm.egg-info/SOURCES.txt
--rw-r--r--   0 bryant     (501) staff       (20)        1 2024-02-07 03:05:56.000000 pyswmm-2.0.0/pyswmm.egg-info/dependency_links.txt
--rw-r--r--   0 bryant     (501) staff       (20)      296 2024-02-07 03:05:56.000000 pyswmm-2.0.0/pyswmm.egg-info/requires.txt
--rw-r--r--   0 bryant     (501) staff       (20)        7 2024-02-07 03:05:56.000000 pyswmm-2.0.0/pyswmm.egg-info/top_level.txt
--rw-r--r--   0 bryant     (501) staff       (20)       38 2024-02-07 03:05:56.347894 pyswmm-2.0.0/setup.cfg
--rw-r--r--   0 bryant     (501) staff       (20)     2871 2023-12-01 20:38:48.000000 pyswmm-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:38:28.421544 pyswmm-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-06 03:38:21.000000 pyswmm-2.0.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    17432 2024-05-06 03:38:21.000000 pyswmm-2.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-06 03:38:21.000000 pyswmm-2.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-06 03:38:21.000000 pyswmm-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7972 2024-05-06 03:38:28.421544 pyswmm-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-05-06 03:38:21.000000 pyswmm-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:38:28.413544 pyswmm-2.0.1/pyswmm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5162 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/_monkey_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/lidcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22142 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/lidgroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37395 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/lidlayers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11439 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/lidunits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31707 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26165 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45787 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/raingages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29182 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31514 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20644 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/subcatchments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52641 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/swmm5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:38:28.417544 pyswmm-2.0.1/pyswmm/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:38:28.417544 pyswmm-2.0.1/pyswmm/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13531 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/tests/data/model_bad_input_1.inp
+-rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/tests/data/model_constantinflow_constanteffluent.inp
+-rw-r--r--   0 runner    (1001) docker     (127)    13531 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/tests/data/model_full_features.inp
+-rw-r--r--   0 runner    (1001) docker     (127)    19277 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/tests/data/model_lids.inp
+-rw-r--r--   0 runner    (1001) docker     (127)     9264 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/tests/data/model_node_inflows.inp
+-rw-r--r--   0 runner    (1001) docker     (127)    14013 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/tests/data/model_pollutants.inp
+-rw-r--r--   0 runner    (1001) docker     (127)    14013 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/tests/data/model_pollutants_2.inp
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/tests/data/model_pollutants_setters.inp
+-rw-r--r--   0 runner    (1001) docker     (127)    13019 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/tests/data/model_pump_setting.inp
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6079 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/tests/data/model_rain.inp
+-rw-r--r--   0 runner    (1001) docker     (127)    12675 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/tests/data/model_storage_pump.inp
+-rw-r--r--   0 runner    (1001) docker     (127)    12675 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/tests/data/model_storage_pump_MGD.inp
+-rw-r--r--   0 runner    (1001) docker     (127)     9009 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/tests/data/model_subcatch_stats.inp
+-rw-r--r--   0 runner    (1001) docker     (127)     9264 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/tests/data/model_toolkit_units.inp
+-rw-r--r--   0 runner    (1001) docker     (127)    13325 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/tests/data/model_weir_setting.inp
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/tests/test_current_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/tests/test_general_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9900 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/tests/test_lid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/tests/test_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10808 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/tests/test_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4987 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/tests/test_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/tests/test_pollutants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/tests/test_rainfallAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6940 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/tests/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/tests/test_subcatchments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/tests/test_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16277 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/toolkitapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:38:28.421544 pyswmm-2.0.1/pyswmm/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-06 03:38:21.000000 pyswmm-2.0.1/pyswmm/utils/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:38:28.421544 pyswmm-2.0.1/pyswmm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7972 2024-05-06 03:38:28.000000 pyswmm-2.0.1/pyswmm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-06 03:38:28.000000 pyswmm-2.0.1/pyswmm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 03:38:28.000000 pyswmm-2.0.1/pyswmm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-06 03:38:28.000000 pyswmm-2.0.1/pyswmm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-06 03:38:28.000000 pyswmm-2.0.1/pyswmm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 03:38:28.421544 pyswmm-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-06 03:38:21.000000 pyswmm-2.0.1/setup.py
```

### Comparing `pyswmm-2.0.0/AUTHORS` & `pyswmm-2.0.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/CHANGELOG.md` & `pyswmm-2.0.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/LICENSE.txt` & `pyswmm-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/PKG-INFO` & `pyswmm-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyswmm
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python Wrapper for SWMM5 API
 Home-page: https://www.pyswmm.org
 Author: Bryant E. McDonnell (See AUTHORS)
 License: BSD2 License
 Keywords: swmm5,swmm,hydraulics,hydrology,modeling,collection system
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Documentation :: Sphinx
```

### Comparing `pyswmm-2.0.0/README.md` & `pyswmm-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm/__init__.py` & `pyswmm-2.0.1/pyswmm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from pyswmm.nodes import Node, Nodes
 from pyswmm.simulation import Simulation, SimulationPreConfig
 from pyswmm.output import Output, SubcatchSeries, NodeSeries, LinkSeries, SystemSeries
 from pyswmm.subcatchments import Subcatchment, Subcatchments
 from pyswmm.system import SystemStats
 from pyswmm.raingages import RainGages, RainGage
 
-VERSION_INFO = (2, 0, 0)
+VERSION_INFO = (2, 0, 1)
 
 __version__ = '.'.join(map(str, VERSION_INFO))
 __author__ = 'Bryant E. McDonnell (Hydroinformatics, LLC) - bemcdonnell@gmail.com'
 __copyright__ = 'Copyright (c) 2024 Bryant E. McDonnell (See AUTHORS)'
 __licence__ = 'BSD2'
 __all__ = [
     Link, Links, LidControls, LidGroups, Node, Nodes, Subcatchment,
```

### Comparing `pyswmm-2.0.0/pyswmm/_monkey_patch.py` & `pyswmm-2.0.1/pyswmm/_monkey_patch.py`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm/errors.py` & `pyswmm-2.0.1/pyswmm/errors.py`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm/lidcontrols.py` & `pyswmm-2.0.1/pyswmm/lidcontrols.py`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm/lidgroups.py` & `pyswmm-2.0.1/pyswmm/lidgroups.py`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm/lidlayers.py` & `pyswmm-2.0.1/pyswmm/lidlayers.py`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm/lidunits.py` & `pyswmm-2.0.1/pyswmm/lidunits.py`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm/links.py` & `pyswmm-2.0.1/pyswmm/links.py`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm/nodes.py` & `pyswmm-2.0.1/pyswmm/nodes.py`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm/output.py` & `pyswmm-2.0.1/pyswmm/output.py`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm/raingages.py` & `pyswmm-2.0.1/pyswmm/raingages.py`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm/reader.py` & `pyswmm-2.0.1/pyswmm/reader.py`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm/simulation.py` & `pyswmm-2.0.1/pyswmm/simulation.py`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm/subcatchments.py` & `pyswmm-2.0.1/pyswmm/subcatchments.py`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm/swmm5.py` & `pyswmm-2.0.1/pyswmm/swmm5.py`

 * *Files 0% similar despite different names*

```diff
@@ -554,15 +554,23 @@
 
     def getObjectIDIndex(self, objecttype, ID):
         """Get Object ID Index. Mostly used as an internal function."""
         return solver.project_get_index(objecttype, ID)
 
     def ObjectIDexist(self, objecttype, ID):
         """Check if Object ID Exists. Mostly used as an internal function."""
-        index = solver.project_get_index(objecttype, ID)
+        # Incurred some micro-tech debt. This updated implementation will cover the before and after
+        # case of removing this line in SWMM.  Currently the SWMM function throws a non-zero error code. As
+        # a result, when it hit swmm-python(swmm-toolkit), it throws an exception.
+        # https://github.com/pyswmm/Stormwater-Management-Model/blob/459db1d4dfc61ff994ae01f92eae64e378e08915/src/solver/toolkit.c#L170
+        try:
+            # eventually this function will return -1 if the index does not exist.
+            index = solver.project_get_index(objecttype, ID)
+        except:
+            index = -1
 
         if index != -1:
             return True
         else:
             return False
 
     def getNodeType(self, ID):
```

### Comparing `pyswmm-2.0.0/pyswmm/system.py` & `pyswmm-2.0.1/pyswmm/system.py`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm/tests/data/__init__.py` & `pyswmm-2.0.1/pyswmm/tests/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm/tests/data/model_bad_input_1.inp` & `pyswmm-2.0.1/pyswmm/tests/data/model_bad_input_1.inp`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm/tests/data/model_constantinflow_constanteffluent.inp` & `pyswmm-2.0.1/pyswmm/tests/data/model_constantinflow_constanteffluent.inp`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm/tests/data/model_full_features.inp` & `pyswmm-2.0.1/pyswmm/tests/data/model_full_features.inp`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm/tests/data/model_lids.inp` & `pyswmm-2.0.1/pyswmm/tests/data/model_lids.inp`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm/tests/data/model_node_inflows.inp` & `pyswmm-2.0.1/pyswmm/tests/data/model_node_inflows.inp`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm/tests/data/model_pollutants.inp` & `pyswmm-2.0.1/pyswmm/tests/data/model_pollutants.inp`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm/tests/data/model_pollutants_2.inp` & `pyswmm-2.0.1/pyswmm/tests/data/model_pollutants_2.inp`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm/tests/data/model_pollutants_setters.inp` & `pyswmm-2.0.1/pyswmm/tests/data/model_pollutants_setters.inp`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm/tests/data/model_pump_setting.inp` & `pyswmm-2.0.1/pyswmm/tests/data/model_pump_setting.inp`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm/tests/data/model_rain.inp` & `pyswmm-2.0.1/pyswmm/tests/data/model_rain.inp`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm/tests/data/model_storage_pump.inp` & `pyswmm-2.0.1/pyswmm/tests/data/model_storage_pump.inp`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm/tests/data/model_storage_pump_MGD.inp` & `pyswmm-2.0.1/pyswmm/tests/data/model_storage_pump_MGD.inp`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm/tests/data/model_subcatch_stats.inp` & `pyswmm-2.0.1/pyswmm/tests/data/model_subcatch_stats.inp`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm/tests/data/model_toolkit_units.inp` & `pyswmm-2.0.1/pyswmm/tests/data/model_toolkit_units.inp`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm/tests/data/model_weir_setting.inp` & `pyswmm-2.0.1/pyswmm/tests/data/model_weir_setting.inp`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm/tests/test_current_time.py` & `pyswmm-2.0.1/pyswmm/tests/test_current_time.py`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm/tests/test_errors.py` & `pyswmm-2.0.1/pyswmm/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm/tests/test_general_engine.py` & `pyswmm-2.0.1/pyswmm/tests/test_general_engine.py`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm/tests/test_lid.py` & `pyswmm-2.0.1/pyswmm/tests/test_lid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Local imports
+from swmm.toolkit.solver import lid_usage_get_flux_rate
 from pyswmm import Simulation
 from pyswmm import LidControls, LidGroups
 from pyswmm.tests.data import MODEL_LIDS_PATH
 from pytest import approx
 UT_PRECISION = 1  # %
 
 
@@ -13,14 +14,15 @@
                 assert(str(control) == 'LID')
             if i == 1:
                 assert(str(control) == 'Green_LID')
 
 
 def test_list_lid_groups():
     with Simulation(MODEL_LIDS_PATH) as sim:
+        assert "DUMMY_GROUP" not in LidGroups(sim)
         for i, group in enumerate(LidGroups(sim)):
             if i == 0:
                 assert('subcatchment {} has {} lid units'.format(group,
                                                                  len(group)) == 'subcatchment 1 has 0 lid units')
             if i == 1:
                 assert('subcatchment {} has {} lid units'.format(group,
                                                                  len(group)) == 'subcatchment 2 has 3 lid units')
```

### Comparing `pyswmm-2.0.0/pyswmm/tests/test_links.py` & `pyswmm-2.0.1/pyswmm/tests/test_links.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         assert (c1c2.inlet_node == "J1")
         assert (c1c2.outlet_node == "J2")
 
 
 def test_links_2():
     with Simulation(MODEL_WEIR_SETTING_PATH) as sim:
         link_names = ["C1", "C1:C2", "C2", "C3"]
+        assert "DUMMY_LINK" not in Links(sim)
         for link in Links(sim):
             assert (link.linkid in link_names)
             link.flow_limit = 10
             assert (link.flow_limit == 10)
 
 
 def test_links_3():
```

### Comparing `pyswmm-2.0.0/pyswmm/tests/test_nodes.py` & `pyswmm-2.0.1/pyswmm/tests/test_nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     assert(node.invert_elevation == 20.728)
 
 
 def test_nodes_2():
     ''' pytest pyswmm/tests/test_nodes.py -k `test_nodes_2` '''
     with Simulation(MODEL_WEIR_SETTING_PATH) as sim:
         print("\n\n\nNODES\n")
+        assert "DUMMY_LINK" not in Nodes(sim)
         for node in Nodes(sim):
             assert ('J' in node.nodeid)
             node.invert_elevation = 10
             assert (node.invert_elevation == 10)
 
 
 def test_nodes_3():
```

### Comparing `pyswmm-2.0.0/pyswmm/tests/test_output.py` & `pyswmm-2.0.1/pyswmm/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm/tests/test_pollutants.py` & `pyswmm-2.0.1/pyswmm/tests/test_pollutants.py`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm/tests/test_rainfallAPI.py` & `pyswmm-2.0.1/pyswmm/tests/test_rainfallAPI.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
             if round(x, 2) == 10.0:
                 check += 1
     assert(check == 718)
 
 
 def test_rainfall():
     with Simulation(MODEL_RAIN) as sim:
+        assert "DUMMY_RG" not in RainGages(sim)
         rg = RainGages(sim)["Gage1"]
         assert(rg.raingageid == "Gage1")
 
         sim.step_advance(3600)
         for ind, step in enumerate(sim):
             if 0 < ind < 5:
                 assert(rg.total_precip == 1)
```

### Comparing `pyswmm-2.0.0/pyswmm/tests/test_simulation.py` & `pyswmm-2.0.1/pyswmm/tests/test_simulation.py`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm/tests/test_subcatchments.py` & `pyswmm-2.0.1/pyswmm/tests/test_subcatchments.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         sim.step_advance(300)
         for ind, step in enumerate(sim):
             print(S3.runoff)
 
 
 def test_subcatchments_2():
     with Simulation(MODEL_WEIR_SETTING_PATH) as sim:
+        assert "DUMMY_SUBC" not in Subcatchments(sim)
         for subcatchment in Subcatchments(sim):
             print(subcatchment)
             print(subcatchment.subcatchmentid)
             print(subcatchment.curb_length)
             subcatchment.curb_length = 10
             print(subcatchment.curb_length)
```

### Comparing `pyswmm-2.0.0/pyswmm/tests/test_system.py` & `pyswmm-2.0.1/pyswmm/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm/toolkitapi.py` & `pyswmm-2.0.1/pyswmm/toolkitapi.py`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm/utils/fixtures.py` & `pyswmm-2.0.1/pyswmm/utils/fixtures.py`

 * *Files identical despite different names*

### Comparing `pyswmm-2.0.0/pyswmm.egg-info/PKG-INFO` & `pyswmm-2.0.1/pyswmm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyswmm
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python Wrapper for SWMM5 API
 Home-page: https://www.pyswmm.org
 Author: Bryant E. McDonnell (See AUTHORS)
 License: BSD2 License
 Keywords: swmm5,swmm,hydraulics,hydrology,modeling,collection system
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Documentation :: Sphinx
```

### Comparing `pyswmm-2.0.0/pyswmm.egg-info/SOURCES.txt` & `pyswmm-2.0.1/pyswmm.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 CHANGELOG.md
 LICENSE.txt
 MANIFEST.in
 README.md
 setup.py
 pyswmm/__init__.py
 pyswmm/_monkey_patch.py
-pyswmm/config.py
 pyswmm/errors.py
 pyswmm/lidcontrols.py
 pyswmm/lidgroups.py
 pyswmm/lidlayers.py
 pyswmm/lidunits.py
 pyswmm/links.py
 pyswmm/nodes.py
@@ -52,10 +51,9 @@
 pyswmm/tests/data/model_pump_setting.inp
 pyswmm/tests/data/model_rain.inp
 pyswmm/tests/data/model_storage_pump.inp
 pyswmm/tests/data/model_storage_pump_MGD.inp
 pyswmm/tests/data/model_subcatch_stats.inp
 pyswmm/tests/data/model_toolkit_units.inp
 pyswmm/tests/data/model_weir_setting.inp
-pyswmm/tests/data/model_weir_setting_a.inp
 pyswmm/utils/__init__.py
 pyswmm/utils/fixtures.py
```

### Comparing `pyswmm-2.0.0/setup.py` & `pyswmm-2.0.1/setup.py`

 * *Files identical despite different names*

