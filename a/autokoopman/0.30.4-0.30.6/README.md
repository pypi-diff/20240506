# Comparing `tmp/autokoopman-0.30.4.tar.gz` & `tmp/autokoopman-0.30.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autokoopman-0.30.4.tar", last modified: Tue Oct 24 23:37:22 2023, max compression
+gzip compressed data, was "autokoopman-0.30.6.tar", last modified: Mon May  6 17:02:43 2024, max compression
```

## Comparing `autokoopman-0.30.4.tar` & `autokoopman-0.30.6.tar`

### file list

```diff
@@ -1,59 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 23:37:22.906989 autokoopman-0.30.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-10-24 23:37:09.000000 autokoopman-0.30.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7604 2023-10-24 23:37:22.906989 autokoopman-0.30.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6773 2023-10-24 23:37:09.000000 autokoopman-0.30.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 23:37:22.910989 autokoopman-0.30.4/autokoopman/
--rw-r--r--   0 runner    (1001) docker     (127)      895 2023-10-24 23:37:09.000000 autokoopman-0.30.4/autokoopman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-24 23:37:09.000000 autokoopman-0.30.4/autokoopman/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2023-10-24 23:37:22.910989 autokoopman-0.30.4/autokoopman/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    15389 2023-10-24 23:37:09.000000 autokoopman-0.30.4/autokoopman/autokoopman.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 23:37:22.906989 autokoopman-0.30.4/autokoopman/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-24 23:37:09.000000 autokoopman-0.30.4/autokoopman/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2023-10-24 23:37:09.000000 autokoopman-0.30.4/autokoopman/benchmark/bio2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2023-10-24 23:37:09.000000 autokoopman-0.30.4/autokoopman/benchmark/fhn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2023-10-24 23:37:09.000000 autokoopman-0.30.4/autokoopman/benchmark/lalo20.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2023-10-24 23:37:09.000000 autokoopman-0.30.4/autokoopman/benchmark/pendulum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2023-10-24 23:37:09.000000 autokoopman-0.30.4/autokoopman/benchmark/prde20.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2023-10-24 23:37:09.000000 autokoopman-0.30.4/autokoopman/benchmark/robe21.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2023-10-24 23:37:09.000000 autokoopman-0.30.4/autokoopman/benchmark/spring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 23:37:22.906989 autokoopman-0.30.4/autokoopman/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-24 23:37:09.000000 autokoopman-0.30.4/autokoopman/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2023-10-24 23:37:09.000000 autokoopman-0.30.4/autokoopman/core/estimator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2023-10-24 23:37:09.000000 autokoopman-0.30.4/autokoopman/core/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     7321 2023-10-24 23:37:09.000000 autokoopman-0.30.4/autokoopman/core/observables.py
--rw-r--r--   0 runner    (1001) docker     (127)    15679 2023-10-24 23:37:09.000000 autokoopman-0.30.4/autokoopman/core/system.py
--rw-r--r--   0 runner    (1001) docker     (127)    21196 2023-10-24 23:37:09.000000 autokoopman-0.30.4/autokoopman/core/trajectory.py
--rw-r--r--   0 runner    (1001) docker     (127)    10610 2023-10-24 23:37:09.000000 autokoopman-0.30.4/autokoopman/core/tuner.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-24 23:37:09.000000 autokoopman-0.30.4/autokoopman/core/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 23:37:22.906989 autokoopman-0.30.4/autokoopman/estimator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-24 23:37:09.000000 autokoopman-0.30.4/autokoopman/estimator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14241 2023-10-24 23:37:09.000000 autokoopman-0.30.4/autokoopman/estimator/deepkoopman.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2023-10-24 23:37:09.000000 autokoopman-0.30.4/autokoopman/estimator/dmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4270 2023-10-24 23:37:09.000000 autokoopman-0.30.4/autokoopman/estimator/koopman.py
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2023-10-24 23:37:09.000000 autokoopman-0.30.4/autokoopman/estimator/sindy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 23:37:22.906989 autokoopman-0.30.4/autokoopman/tuner/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-24 23:37:09.000000 autokoopman-0.30.4/autokoopman/tuner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4621 2023-10-24 23:37:09.000000 autokoopman-0.30.4/autokoopman/tuner/bayesianopt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2023-10-24 23:37:09.000000 autokoopman-0.30.4/autokoopman/tuner/gridsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2023-10-24 23:37:09.000000 autokoopman-0.30.4/autokoopman/tuner/montecarlo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 23:37:22.906989 autokoopman-0.30.4/autokoopman.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7604 2023-10-24 23:37:22.000000 autokoopman-0.30.4/autokoopman.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2023-10-24 23:37:22.000000 autokoopman-0.30.4/autokoopman.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-24 23:37:22.000000 autokoopman-0.30.4/autokoopman.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2023-10-24 23:37:22.000000 autokoopman-0.30.4/autokoopman.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-10-24 23:37:22.000000 autokoopman-0.30.4/autokoopman.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-10-24 23:37:09.000000 autokoopman-0.30.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      200 2023-10-24 23:37:22.910989 autokoopman-0.30.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2023-10-24 23:37:09.000000 autokoopman-0.30.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 23:37:22.902989 autokoopman-0.30.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-24 23:37:09.000000 autokoopman-0.30.4/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 23:37:22.906989 autokoopman-0.30.4/test/unit_test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-24 23:37:09.000000 autokoopman-0.30.4/test/unit_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2023-10-24 23:37:09.000000 autokoopman-0.30.4/test/unit_test/test_autokoopman.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2023-10-24 23:37:09.000000 autokoopman-0.30.4/test/unit_test/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2023-10-24 23:37:09.000000 autokoopman-0.30.4/test/unit_test/test_deepk.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-10-24 23:37:09.000000 autokoopman-0.30.4/test/unit_test/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2023-10-24 23:37:09.000000 autokoopman-0.30.4/test/unit_test/test_koopman.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2023-10-24 23:37:09.000000 autokoopman-0.30.4/test/unit_test/test_sindy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2023-10-24 23:37:09.000000 autokoopman-0.30.4/test/unit_test/test_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2023-10-24 23:37:09.000000 autokoopman-0.30.4/test/unit_test/test_trajectory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:02:43.307475 autokoopman-0.30.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-06 17:02:36.000000 autokoopman-0.30.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8849 2024-05-06 17:02:43.307475 autokoopman-0.30.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8018 2024-05-06 17:02:36.000000 autokoopman-0.30.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:02:43.307475 autokoopman-0.30.6/autokoopman/
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-06 17:02:36.000000 autokoopman-0.30.6/autokoopman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 17:02:36.000000 autokoopman-0.30.6/autokoopman/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-06 17:02:43.307475 autokoopman-0.30.6/autokoopman/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18851 2024-05-06 17:02:36.000000 autokoopman-0.30.6/autokoopman/autokoopman.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:02:43.303475 autokoopman-0.30.6/autokoopman/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 17:02:36.000000 autokoopman-0.30.6/autokoopman/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-06 17:02:36.000000 autokoopman-0.30.6/autokoopman/benchmark/bio2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-06 17:02:36.000000 autokoopman-0.30.6/autokoopman/benchmark/fhn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-06 17:02:36.000000 autokoopman-0.30.6/autokoopman/benchmark/lalo20.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-06 17:02:36.000000 autokoopman-0.30.6/autokoopman/benchmark/pendulum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-06 17:02:36.000000 autokoopman-0.30.6/autokoopman/benchmark/prde20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-05-06 17:02:36.000000 autokoopman-0.30.6/autokoopman/benchmark/robe21.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-06 17:02:36.000000 autokoopman-0.30.6/autokoopman/benchmark/spring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:02:43.303475 autokoopman-0.30.6/autokoopman/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 17:02:36.000000 autokoopman-0.30.6/autokoopman/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-05-06 17:02:36.000000 autokoopman-0.30.6/autokoopman/core/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-06 17:02:36.000000 autokoopman-0.30.6/autokoopman/core/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-06 17:02:36.000000 autokoopman-0.30.6/autokoopman/core/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15679 2024-05-06 17:02:36.000000 autokoopman-0.30.6/autokoopman/core/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22687 2024-05-06 17:02:36.000000 autokoopman-0.30.6/autokoopman/core/trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9582 2024-05-06 17:02:36.000000 autokoopman-0.30.6/autokoopman/core/tuner.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 17:02:36.000000 autokoopman-0.30.6/autokoopman/core/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:02:43.303475 autokoopman-0.30.6/autokoopman/estimator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 17:02:36.000000 autokoopman-0.30.6/autokoopman/estimator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14244 2024-05-06 17:02:36.000000 autokoopman-0.30.6/autokoopman/estimator/deepkoopman.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-06 17:02:36.000000 autokoopman-0.30.6/autokoopman/estimator/dmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-05-06 17:02:36.000000 autokoopman-0.30.6/autokoopman/estimator/koopman.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-05-06 17:02:36.000000 autokoopman-0.30.6/autokoopman/estimator/sindy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:02:43.303475 autokoopman-0.30.6/autokoopman/observable/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-06 17:02:36.000000 autokoopman-0.30.6/autokoopman/observable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-05-06 17:02:36.000000 autokoopman-0.30.6/autokoopman/observable/observables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-05-06 17:02:36.000000 autokoopman-0.30.6/autokoopman/observable/reweighted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-06 17:02:36.000000 autokoopman-0.30.6/autokoopman/observable/rff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:02:43.307475 autokoopman-0.30.6/autokoopman/tuner/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 17:02:36.000000 autokoopman-0.30.6/autokoopman/tuner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4621 2024-05-06 17:02:36.000000 autokoopman-0.30.6/autokoopman/tuner/bayesianopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-05-06 17:02:36.000000 autokoopman-0.30.6/autokoopman/tuner/gridsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-06 17:02:36.000000 autokoopman-0.30.6/autokoopman/tuner/montecarlo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:02:43.307475 autokoopman-0.30.6/autokoopman.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8849 2024-05-06 17:02:43.000000 autokoopman-0.30.6/autokoopman.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-06 17:02:43.000000 autokoopman-0.30.6/autokoopman.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 17:02:43.000000 autokoopman-0.30.6/autokoopman.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-06 17:02:43.000000 autokoopman-0.30.6/autokoopman.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-06 17:02:43.000000 autokoopman-0.30.6/autokoopman.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-06 17:02:36.000000 autokoopman-0.30.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-06 17:02:43.307475 autokoopman-0.30.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-06 17:02:36.000000 autokoopman-0.30.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:02:43.299475 autokoopman-0.30.6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 17:02:36.000000 autokoopman-0.30.6/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:02:43.299475 autokoopman-0.30.6/test/unit_test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 17:02:36.000000 autokoopman-0.30.6/test/unit_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-06 17:02:36.000000 autokoopman-0.30.6/test/unit_test/test_autokoopman.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-06 17:02:36.000000 autokoopman-0.30.6/test/unit_test/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-06 17:02:36.000000 autokoopman-0.30.6/test/unit_test/test_deepk.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-06 17:02:36.000000 autokoopman-0.30.6/test/unit_test/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-06 17:02:36.000000 autokoopman-0.30.6/test/unit_test/test_koopman.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-06 17:02:36.000000 autokoopman-0.30.6/test/unit_test/test_sindy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-06 17:02:36.000000 autokoopman-0.30.6/test/unit_test/test_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-05-06 17:02:36.000000 autokoopman-0.30.6/test/unit_test/test_trajectory.py
```

### Comparing `autokoopman-0.30.4/LICENSE` & `autokoopman-0.30.6/LICENSE`

 * *Files identical despite different names*

### Comparing `autokoopman-0.30.4/PKG-INFO` & `autokoopman-0.30.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autokoopman
-Version: 0.30.4
+Version: 0.30.6
 Summary: Automated Koopman Operator Linearization Library
 Home-page: https://github.com/EthanJamesLew/AutoKoopman
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Intended Audience :: Science/Research
@@ -139,14 +139,34 @@
 *AutoKoopman Class Structure in the Training Pipeline*. A user can implement any of the classes to extend AutoKoopman (e.g., custom observables, a custom tuner, a new system id estimator).
 
 ## Documentation
 
 See the
 [AutoKoopman Documentation](https://ethanjameslew.github.io/AutoKoopman/).
 
+## Citing AutoKoopman
+
+AutoKoopman has been published as a tool paper at ATVA 2023. The preprint can be found [here](https://www.researchgate.net/profile/Ethan-Lew/publication/374805680_AutoKoopman_A_Toolbox_for_Automated_System_Identification_via_Koopman_Operator_Linearization/links/6537cf9f1d6e8a70704c7f31/AutoKoopman-A-Toolbox-for-Automated-System-Identification-via-Koopman-Operator-Linearization.pdf).
+
+If you cite AutoKoopman, please cite
+
+Lew, E., Hekal, A., Potomkin, K., Kochdumper, N., Hencey, B., Bak, S., & Bogomolov, S. (2023, October). Autokoopman: A toolbox for automated system identification via koopman operator linearization. In International Symposium on Automated Technology for Verification and Analysis (pp. 237-250). Cham: Springer Nature Switzerland.
+
+Bibtex:
+```
+@inproceedings{lew2023autokoopman,
+  title={Autokoopman: A toolbox for automated system identification via koopman operator linearization},
+  author={Lew, Ethan and Hekal, Abdelrahman and Potomkin, Kostiantyn and Kochdumper, Niklas and Hencey, Brandon and Bak, Stanley and Bogomolov, Sergiy},
+  booktitle={International Symposium on Automated Technology for Verification and Analysis},
+  pages={237--250},
+  year={2023},
+  organization={Springer}
+}
+```
+
 ## References  
 
 <a id="1">[1]</a> Williams, M. O., Kevrekidis, I. G., & Rowley, C. W. (2015). A data–driven approximation of the koopman operator: Extending dynamic mode decomposition. Journal of Nonlinear Science, 25, 1307-1346.
 
  <a id="2">[2]</a> Li, Y., He, H., Wu, J., Katabi, D., & Torralba, A. (2019). Learning compositional koopman operators for model-based control. arXiv preprint arXiv:1910.08264.
 
   <a id="3">[3]</a> Brunton, S. L., Proctor, J. L., & Kutz, J. N. (2016). Discovering governing equations from data by sparse identification of nonlinear dynamical systems. Proceedings of the national academy of sciences, 113(15), 3932-3937.
```

### Comparing `autokoopman-0.30.4/README.md` & `autokoopman-0.30.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -116,14 +116,34 @@
 *AutoKoopman Class Structure in the Training Pipeline*. A user can implement any of the classes to extend AutoKoopman (e.g., custom observables, a custom tuner, a new system id estimator).
 
 ## Documentation
 
 See the
 [AutoKoopman Documentation](https://ethanjameslew.github.io/AutoKoopman/).
 
+## Citing AutoKoopman
+
+AutoKoopman has been published as a tool paper at ATVA 2023. The preprint can be found [here](https://www.researchgate.net/profile/Ethan-Lew/publication/374805680_AutoKoopman_A_Toolbox_for_Automated_System_Identification_via_Koopman_Operator_Linearization/links/6537cf9f1d6e8a70704c7f31/AutoKoopman-A-Toolbox-for-Automated-System-Identification-via-Koopman-Operator-Linearization.pdf).
+
+If you cite AutoKoopman, please cite
+
+Lew, E., Hekal, A., Potomkin, K., Kochdumper, N., Hencey, B., Bak, S., & Bogomolov, S. (2023, October). Autokoopman: A toolbox for automated system identification via koopman operator linearization. In International Symposium on Automated Technology for Verification and Analysis (pp. 237-250). Cham: Springer Nature Switzerland.
+
+Bibtex:
+```
+@inproceedings{lew2023autokoopman,
+  title={Autokoopman: A toolbox for automated system identification via koopman operator linearization},
+  author={Lew, Ethan and Hekal, Abdelrahman and Potomkin, Kostiantyn and Kochdumper, Niklas and Hencey, Brandon and Bak, Stanley and Bogomolov, Sergiy},
+  booktitle={International Symposium on Automated Technology for Verification and Analysis},
+  pages={237--250},
+  year={2023},
+  organization={Springer}
+}
+```
+
 ## References  
 
 <a id="1">[1]</a> Williams, M. O., Kevrekidis, I. G., & Rowley, C. W. (2015). A data–driven approximation of the koopman operator: Extending dynamic mode decomposition. Journal of Nonlinear Science, 25, 1307-1346.
 
  <a id="2">[2]</a> Li, Y., He, H., Wu, J., Katabi, D., & Torralba, A. (2019). Learning compositional koopman operators for model-based control. arXiv preprint arXiv:1910.08264.
 
   <a id="3">[3]</a> Brunton, S. L., Proctor, J. L., & Kutz, J. N. (2016). Discovering governing equations from data by sparse identification of nonlinear dynamical systems. Proceedings of the national academy of sciences, 113(15), 3932-3937.
```

### Comparing `autokoopman-0.30.4/autokoopman/__init__.py` & `autokoopman-0.30.6/autokoopman/__init__.py`

 * *Files identical despite different names*

### Comparing `autokoopman-0.30.4/autokoopman/autokoopman.py` & `autokoopman-0.30.6/autokoopman/autokoopman.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,55 +1,60 @@
 """
 Main AutoKoopman Function (Convenience Function)
 """
-from typing import Callable, Union, Sequence, Optional, Tuple
+from typing import Callable, Dict, Hashable, Union, Sequence, Optional, Tuple
 
 import numpy as np
 
-import autokoopman.core.observables as kobs
+import autokoopman.observable as kobs
 from autokoopman.core.trajectory import (
     TrajectoriesData,
     UniformTimeTrajectoriesData,
     UniformTimeTrajectory,
 )
 from autokoopman.core.tuner import (
     HyperparameterTuner,
     HyperparameterMap,
     ParameterSpace,
     ContinuousParameter,
     DiscreteParameter,
     TrajectoryScoring,
 )
 from autokoopman.estimator.koopman import KoopmanDiscEstimator
+from autokoopman.estimator.koopman import KoopmanContinuousEstimator
 from autokoopman.tuner.gridsearch import GridSearchTuner
 from autokoopman.tuner.montecarlo import MonteCarloTuner
 from autokoopman.tuner.bayesianopt import BayesianOptTuner
-from autokoopman.core.observables import KoopmanObservable
+from autokoopman.observable.observables import KoopmanObservable
 from autokoopman.core.format import hide_prints
 
 __all__ = ["auto_koopman"]
 
 
 # valid string identifiers for the autokoopman magic
 obs_types = {"rff", "poly", "quadratic", "id", "deep"}
 opt_types = {"grid", "monte-carlo", "bopt"}
-scoring_func_types = {"total", "end", "relative"}
+scoring_func_types = {"total", "end", "relative", "weighted"}
 
 
-def get_scoring_func(score_name):
+def get_scoring_func(score_name, scoring_weights):
     """resolve scoring function from name or callable type"""
     # if callable, just return it
     if callable(score_name):
         return score_name
     if score_name == "total":
         return TrajectoryScoring.total_score
     elif score_name == "end":
         return TrajectoryScoring.end_point_score
     elif score_name == "relative":
         return TrajectoryScoring.relative_score
+    elif score_name == "weighted":
+        return lambda true, pred: TrajectoryScoring.weighted_score(
+            true, pred, scoring_weights
+        )
     else:
         raise ValueError(
             f"Scoring function name {score_name} is not in available list (names are {scoring_func_types})"
         )
 
 
 def get_parameter_space(obs_type, threshold_range, rank):
@@ -93,59 +98,84 @@
             "koopman-id",
             [
                 DiscreteParameter("rank", *rank),
             ],
         )
 
 
-def get_estimator(obs_type, sampling_period, dim, obs, hyperparams, normalize):
+def get_estimator(
+    obs_type,
+    learn_continuous,
+    sampling_period,
+    dim,
+    obs,
+    hyperparams,
+    normalize,
+    weights,
+):
     """from the myriad of user suppled switches, select the right estimator"""
+
+    def inst_estimator(*args, **kwargs):
+        if learn_continuous:
+            return KoopmanContinuousEstimator(
+                args[0], *args[2:], weights=weights, **kwargs
+            )
+        else:
+            return KoopmanDiscEstimator(*args, weights=weights, **kwargs)
+
     if obs_type == "rff":
         observables = kobs.IdentityObservable() | kobs.RFFObservable(
             dim, obs, hyperparams[0]
         )
-        return KoopmanDiscEstimator(
+        return inst_estimator(
             observables, sampling_period, dim, rank=hyperparams[1], normalize=normalize
         )
     elif obs_type == "quadratic":
         observables = kobs.IdentityObservable() | kobs.QuadraticObservable(dim)
-        return KoopmanDiscEstimator(
+        return inst_estimator(
             observables, sampling_period, dim, rank=hyperparams[0], normalize=normalize
         )
     elif obs_type == "poly":
         observables = kobs.PolynomialObservable(dim, hyperparams[0])
-        return KoopmanDiscEstimator(
+        return inst_estimator(
             observables, sampling_period, dim, rank=hyperparams[1], normalize=normalize
         )
     elif obs_type == "id":
         observables = kobs.IdentityObservable()
-        return KoopmanDiscEstimator(
+        return inst_estimator(
             observables, sampling_period, dim, rank=hyperparams[0], normalize=normalize
         )
     elif isinstance(obs_type, KoopmanObservable):
-        return KoopmanDiscEstimator(
+        return inst_estimator(
             obs_type, sampling_period, dim, rank=hyperparams[0], normalize=normalize
         )
     else:
         raise ValueError(f"unknown observables type {obs_type}")
 
 
 def auto_koopman(
     training_data: Union[TrajectoriesData, Sequence[np.ndarray]],
     inputs_training_data: Optional[Sequence[np.ndarray]] = None,
+    learn_continuous: bool = False,
     sampling_period: Optional[float] = None,
     normalize: bool = False,
     opt: Union[str, HyperparameterTuner] = "monte-carlo",
     max_opt_iter: int = 100,
     max_epochs: int = 500,
     n_splits: Optional[int] = None,
     obs_type: Union[str, KoopmanObservable] = "rff",
     cost_func: Union[
         str, Callable[[TrajectoriesData, TrajectoriesData], float]
     ] = "total",
+    scoring_weights: Optional[
+        Union[Sequence[np.ndarray], Dict[Hashable, np.ndarray]]
+    ] = None,
+    learning_weights: Optional[
+        Union[Sequence[np.ndarray], Dict[Hashable, np.ndarray]]
+    ] = None,
     n_obs: int = 100,
     rank: Optional[Union[Tuple[int, int], Tuple[int, int, int]]] = None,
     grid_param_slices: int = 10,
     lengthscale: Tuple[float, float] = (1e-4, 1e1),
     enc_dim: Tuple[int, int, int] = (2, 64, 16),
     n_layers: Tuple[int, int, int] = (1, 8, 2),
     torch_device: Optional[str] = None,
@@ -154,22 +184,23 @@
     """
     AutoKoopman Convenience Function
         This is an interface to the dynamical systems learning functionality of the AutoKoopman library. The user can select
         estimators classes at a high level. A tuner can be chosen to find the best hyperparameter values.
 
     :param training_data: training trajectories data from which to learn the system
     :param inputs_training_data: optional input trajectories data from which to learn the system (this isn't needed if the training data has inputs already)
+    :param learn_continuous: whether to learn a continuous time or discrete time Koopman estimator
     :param sampling_period: (for discrete time system) sampling period of training data
     :param normalize: normalize the states of the training trajectories
     :param opt: hyperparameter optimizer {"grid", "monte-carlo", "bopt"}
     :param max_opt_iter: maximum iterations for the tuner to use
     :param max_epochs: maximum number of training epochs
     :param n_splits: (for optimizers) if set, switches to k-folds bootstrap validation for the hyperparameter tuning. This is useful for things like RFF tuning where the results have noise.
     :param obs_type: (for koopman) koopman observables to use {"rff", "quadratic", "poly", "id", "deep"}
-    :param cost_func: cost function to use for hyperparameter optimization
+    :param cost_func: cost function to use for hyperparameter optimization {"total", "end", "relative"}
     :param  n_obs: (for koopman) number of observables to use (if applicable)
     :param rank: (for koopman) rank range (start, stop) or (start, stop, step)
     :param grid_param_slices: (for grid tuner) resolution to slice continuous valued parameters into
     :param lengthscale: (for RFF observables) RFF kernel lengthscale
     :param enc_dim: (for deep learning) number of dimensions in the latent space
     :param n_layers: (for deep learning) number of hidden layers in the encoder / decoder
     :param torch_device: (for deep learning) specify torch compute device
@@ -206,39 +237,59 @@
             # 'hyperparameters': ['gamma', 'rank'],
             # 'hyperparameter_values': (0.004641588833612782, 21),
             # 'tuner_score': 0.14723275426562,
             # 'tuner': <autokoopman.tuner.gridsearch.GridSearchTuner at 0x7f0f92f95580>,
             # 'estimator': <autokoopman.estimator.koopman.KoopmanDiscEstimator at 0x7f0f92ff0610>}
     """
 
-    training_data, sampling_period = _sanitize_training_data(
-        training_data, inputs_training_data, sampling_period, opt, obs_type
+    if cost_func == "weighted":
+        assert (
+            scoring_weights is not None
+        ), f"weighted scoring requires scoring weights (currently None)"
+
+    (
+        training_data,
+        sampling_period,
+        scoring_weights,
+        learning_weights,
+    ) = _sanitize_training_data(
+        training_data,
+        inputs_training_data,
+        sampling_period,
+        opt,
+        obs_type,
+        scoring_weights,
+        learning_weights,
     )
 
     # get the hyperparameter map
     if obs_type in {"deep"}:
+        if learn_continuous:
+            raise ValueError("deep learning is only for discrete systems")
         modelmap = _deep_model_map(
             training_data,
             max_epochs,
             n_obs,
             enc_dim,
             n_layers,
             torch_device,
             verbose,
             normalize,
         )
     else:
         modelmap = _edmd_model_map(
             training_data,
+            learn_continuous,
             rank,
             obs_type,
             n_obs,
             lengthscale,
             sampling_period,
             normalize,
+            learning_weights,
         )
 
     # setup the tuner
     if opt == "grid":
         gt = GridSearchTuner(
             modelmap,
             training_data,
@@ -251,16 +302,25 @@
             modelmap, training_data, n_splits=n_splits, verbose=verbose
         )
     elif opt == "bopt":
         gt = BayesianOptTuner(modelmap, training_data, verbose=verbose)
     else:
         raise ValueError(f"could not match a tuner to the string {opt}")
 
-    with hide_prints():
-        res = gt.tune(nattempts=max_opt_iter, scoring_func=get_scoring_func(cost_func))
+    if verbose:
+        res = gt.tune(
+            nattempts=max_opt_iter,
+            scoring_func=get_scoring_func(cost_func, scoring_weights),
+        )
+    else:
+        with hide_prints():
+            res = gt.tune(
+                nattempts=max_opt_iter,
+                scoring_func=get_scoring_func(cost_func, scoring_weights),
+            )
 
     # pack results into out custom output
     result = {
         "tuned_model": res["model"].model,
         "model_class": modelmap.parameter_space.name,
         "hyperparameters": [param.name for param in modelmap.parameter_space],
         "hyperparameter_values": res["param"],
@@ -323,19 +383,28 @@
             )
 
     # get the hyperparameter map
     return _ModelMap()
 
 
 def _edmd_model_map(
-    training_data, rank, obs_type, n_obs, lengthscale, sampling_period, normalize
+    training_data,
+    learn_continuous,
+    rank,
+    obs_type,
+    n_obs,
+    lengthscale,
+    sampling_period,
+    normalize,
+    weights,
 ) -> HyperparameterMap:
     """model map for eDMD based methods
 
-    :param training_data:
+    :param training_data: trajectories training dataset
+    :param learn_continuous: whether to learn continuous time or discrete time Koopman estimator
     :param rank: set of ranks to try (of DMD rank parameter)
     :param obs_type:
     :param n_obs: some obs type require a number of observables
     :sampling_period:
 
     :returns: hyperparameter map
     """
@@ -359,23 +428,36 @@
 
         def __init__(self):
             self.names = training_data.state_names
             super(_ModelMap, self).__init__(pspace)
 
         def get_model(self, hyperparams: Sequence):
             return get_estimator(
-                obs_type, sampling_period, dim, n_obs, hyperparams, normalize
+                obs_type,
+                learn_continuous,
+                sampling_period,
+                dim,
+                n_obs,
+                hyperparams,
+                normalize,
+                weights,
             )
 
     # get the hyperparameter map
     return _ModelMap()
 
 
 def _sanitize_training_data(
-    training_data, inputs_training_data, sampling_period, opt, obs_type
+    training_data,
+    inputs_training_data,
+    sampling_period,
+    opt,
+    obs_type,
+    scoring_weights,
+    learning_weights,
 ):
     """auto_koopman input sanitization"""
 
     # if sampling period is None AND discrete system is wanted
     if sampling_period is None:
         sampling_period = np.infty
         for t in training_data:
@@ -391,28 +473,56 @@
         assert (
             opt in opt_types
         ), f"tuner name {opt} is unknown (valid ones are {opt_types})"
 
     # convert the data to autokoopman trajectories
     if isinstance(training_data, TrajectoriesData):
         if not isinstance(training_data, UniformTimeTrajectoriesData):
+            assert (
+                scoring_weights is None and learning_weights is None
+            ), f"weights must be None as interpolation is occuring"
             print(
                 f"resampling trajectories as they need to be uniform time (sampling period {sampling_period})"
             )
             training_data = training_data.interp_uniform_time(sampling_period)
         else:
             if not np.isclose(training_data.sampling_period, sampling_period):
+                assert (
+                    scoring_weights is None and learning_weights is None
+                ), f"weights must be None as interpolation is occuring"
                 print(
                     f"resampling trajectories because the sampling periods differ (original {training_data.sampling_period}, new {sampling_period})"
                 )
                 training_data = training_data.interp_uniform_time(sampling_period)
     else:
+        if isinstance(training_data, dict) and scoring_weights is not None:
+            assert isinstance(
+                scoring_weights, dict
+            ), "training data has unordered keys, so scoring weights must be a dictionary with matching keys"
+        else:
+            if scoring_weights is not None and not isinstance(scoring_weights, dict):
+                scoring_weights = {
+                    idx: weights for idx, weights in enumerate(scoring_weights)
+                }
+
+        if isinstance(training_data, dict) and learning_weights is not None:
+            assert isinstance(
+                learning_weights, dict
+            ), "training data has unordered keys, so learning weights must be a dictionary with matching keys"
+        else:
+            if learning_weights is not None and not isinstance(learning_weights, dict):
+                learning_weights = {
+                    idx: weights for idx, weights in enumerate(learning_weights)
+                }
+
         # figure out how to add inputs
         training_iter = (
-            training_data.items() if isinstance(training_data, dict) else training_data
+            training_data.items()
+            if isinstance(training_data, dict)
+            else enumerate(training_data)
         )
         if inputs_training_data is not None:
             training_iter = [(n, x, inputs_training_data[n]) for n, x in training_iter]
         else:
             training_iter = [(n, x, None) for n, x in training_iter]
         if isinstance(training_data, dict):
             training_data = UniformTimeTrajectoriesData(
@@ -425,8 +535,8 @@
             training_data = UniformTimeTrajectoriesData(
                 {
                     idx: UniformTimeTrajectory(di, u, sampling_period=sampling_period)
                     for idx, di, u in training_iter
                 }
             )
 
-    return training_data, sampling_period
+    return training_data, sampling_period, scoring_weights, learning_weights
```

### Comparing `autokoopman-0.30.4/autokoopman/benchmark/bio2.py` & `autokoopman-0.30.6/autokoopman/benchmark/bio2.py`

 * *Files identical despite different names*

### Comparing `autokoopman-0.30.4/autokoopman/benchmark/fhn.py` & `autokoopman-0.30.6/autokoopman/benchmark/fhn.py`

 * *Files identical despite different names*

### Comparing `autokoopman-0.30.4/autokoopman/benchmark/lalo20.py` & `autokoopman-0.30.6/autokoopman/benchmark/lalo20.py`

 * *Files identical despite different names*

### Comparing `autokoopman-0.30.4/autokoopman/benchmark/pendulum.py` & `autokoopman-0.30.6/autokoopman/benchmark/pendulum.py`

 * *Files identical despite different names*

### Comparing `autokoopman-0.30.4/autokoopman/benchmark/prde20.py` & `autokoopman-0.30.6/autokoopman/benchmark/prde20.py`

 * *Files identical despite different names*

### Comparing `autokoopman-0.30.4/autokoopman/benchmark/robe21.py` & `autokoopman-0.30.6/autokoopman/benchmark/robe21.py`

 * *Files identical despite different names*

### Comparing `autokoopman-0.30.4/autokoopman/benchmark/spring.py` & `autokoopman-0.30.6/autokoopman/benchmark/spring.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import sympy as sp  # type: ignore
-from numpy import cos, sin
+from sympy import cos, sin
 
 import autokoopman.core.system as asys
 
 
 class Spring(asys.SymbolicContinuousSystem):
     r"""
     Spring pendulum
```

### Comparing `autokoopman-0.30.4/autokoopman/core/format.py` & `autokoopman-0.30.6/autokoopman/core/format.py`

 * *Files identical despite different names*

### Comparing `autokoopman-0.30.4/autokoopman/core/observables.py` & `autokoopman-0.30.6/autokoopman/observable/observables.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import abc
 from typing import Sequence
 
 import numpy as np
 import sympy as sp  # type: ignore
 
-from scipy.stats import cauchy, laplace
-
 
 class KoopmanObservable(abc.ABC):
     """
     Koopman Observables Functions
        These objects implement the mapping of the system state to the Koopman invariant space (explicitly).
 
     References
@@ -159,55 +157,7 @@
         self.degree = degree
         self.dimension = dimension
         self.poly = PolynomialFeatures(int(self.degree), include_bias=False)
         self.poly.fit_transform(np.zeros((1, self.dimension)))
 
     def obs_fcn(self, X: np.ndarray) -> np.ndarray:
         return self.poly.transform(np.atleast_2d(X)).T
-
-
-class RFFObservable(KoopmanObservable):
-    def __init__(self, dimension, num_features, gamma, metric="rbf"):
-        super(RFFObservable, self).__init__()
-        self.gamma = gamma
-        self.dimension = dimension
-        self.metric = metric
-        self.D = num_features
-        # Generate D iid samples from p(w)
-        if self.metric == "rbf":
-            self.w = np.sqrt(2 * self.gamma) * np.random.normal(
-                size=(self.D, self.dimension)
-            )
-        elif self.metric == "laplace":
-            self.w = cauchy.rvs(scale=self.gamma, size=(self.D, self.dimension))
-        # Generate D iid samples from Uniform(0,2*pi)
-        self.u = 2 * np.pi * np.random.rand(self.D)
-
-    def obs_fcn(self, X: np.ndarray) -> np.ndarray:
-        # modification...
-        if len(X.shape) == 1:
-            x = np.atleast_2d(X.flatten()).T
-        else:
-            x = X.T
-        w = self.w.T
-        u = self.u[np.newaxis, :].T
-        s = np.sqrt(2 / self.D)
-        Z = s * np.cos(x.T @ w + u.T)
-        return Z.T
-
-    def obs_grad(self, X: np.ndarray) -> np.ndarray:
-        if len(X.shape) == 1:
-            x = np.atleast_2d(X.flatten()).T
-        else:
-            x = X.T
-        x = np.atleast_2d(X.flatten()).T
-        w = self.w.T
-        u = self.u[np.newaxis, :].T
-        s = np.sqrt(2 / self.D)
-        # TODO: make this sparse?
-        Z = -s * np.diag(np.sin(u + w.T @ x).flatten()) @ w.T
-        return Z
-
-    def compute_kernel(self, X: np.ndarray) -> np.ndarray:
-        Z = self.transform(X)
-        K = Z.dot(Z.T)
-        return K
```

### Comparing `autokoopman-0.30.4/autokoopman/core/system.py` & `autokoopman-0.30.6/autokoopman/core/system.py`

 * *Files identical despite different names*

### Comparing `autokoopman-0.30.4/autokoopman/core/trajectory.py` & `autokoopman-0.30.6/autokoopman/core/trajectory.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,14 +206,24 @@
             norm(self.states, axis=axis)[:, np.newaxis],
             None,
             state_names=["<norm>"],
             input_names=None,
             threshold=self._threshold,
         )
 
+    def abs(self) -> "Trajectory":
+        return Trajectory(
+            self.times,
+            np.abs(self.states),
+            None,
+            state_names=self.names,
+            input_names=None,
+            threshold=self._threshold,
+        )
+
 
 class UniformTimeTrajectory(Trajectory):
     """uniform time is a trajectory advanced by a sampling period"""
 
     def __init__(
         self,
         states: np.ndarray,
@@ -487,14 +497,17 @@
     def __add__(self, other: "TrajectoriesData"):
         otheri = self._prepare_other(other)
         return TrajectoriesData({k: v + otheri[k] for k, v in self._trajs.items()})
 
     def norm(self):
         return TrajectoriesData({k: v.norm() for k, v in self._trajs.items()})
 
+    def abs(self):
+        return TrajectoriesData({k: v.abs() for k, v in self._trajs.items()})
+
 
 class UniformTimeTrajectoriesData(TrajectoriesData):
     """a dataset of uniform time trajectories"""
 
     def __init__(self, trajs: Dict[Hashable, Union[UniformTimeTrajectory, Trajectory]]):
         super(UniformTimeTrajectoriesData, self).__init__(trajs)
 
@@ -556,17 +569,15 @@
             data_df, threshold=threshold, time_id=time_id, traj_id=traj_id
         )
         for k, v in traj_data._trajs.items():
             assert v.is_uniform_time, f"{k} is not uniform time"
         return cls({k: v.to_uniform_time_traj() for k, v in traj_data._trajs.items()})
 
     @property
-    def next_step_matrices(
-        self, nstep=1
-    ) -> Tuple[np.ndarray, np.ndarray, Optional[np.ndarray]]:
+    def next_step_matrices(self) -> Tuple[np.ndarray, np.ndarray, Optional[np.ndarray]]:
         r"""
         Next Step Snapshot Matrices
             Return the two "snapshot matrices" :math:`\mathbf X, \mathbf X'` of observations :math:`\{x_1, x_2, ..., x_n \}`,
 
             .. math::
 
                 \mathbf X = \begin{bmatrix} x_1 && x_2 && ... && x_{n-1}  \end{bmatrix}, \quad \mathbf X = \begin{bmatrix} x_2 && x_3 && ... && x_{n}  \end{bmatrix}
@@ -584,31 +595,44 @@
 
         :returns: tuple of (:math:`\mathbf X, \mathbf X'`).
 
         References
             Brunton, S. L., & Kutz, J. N. (2022). Data-driven science and engineering: Machine learning,
             dynamical systems, and control. Cambridge University Press. pp 236-7
         """
-        return self.n_step_matrices(1)
+        return self.n_step_matrices(1, None)[:-1]
+
+    def next_step_matrices_weights(
+        self, weights, nstep=1
+    ) -> Tuple[np.ndarray, np.ndarray, Optional[np.ndarray]]:
+        r"""
+        Weighted Next Step Snapshot Matrices
+        """
+        return self.n_step_matrices(1, weights)
 
     def n_step_matrices(
-        self, nstep
+        self, nstep, weights=None
     ) -> Tuple[np.ndarray, np.ndarray, Optional[np.ndarray]]:
-        X = np.vstack([x.states[:-nstep:nstep, :] for _, x in self._trajs.items()]).T
+        items = self._trajs.items()
+        X = np.vstack([x.states[:-nstep:nstep, :] for _, x in items]).T
 
-        Xp = np.vstack([x.states[nstep::nstep, :] for _, x in self._trajs.items()]).T
+        Xp = np.vstack([x.states[nstep::nstep, :] for _, x in items]).T
 
         if self.input_names is not None:
-            U = np.vstack(
-                [u.inputs[:-nstep:nstep, :] for _, u in self._trajs.items()]
-            ).T
+            U = np.vstack([u.inputs[:-nstep:nstep, :] for _, u in items]).T
         else:
             U = None
 
-        return X, Xp, U
+        # collect weights
+        if weights is None:
+            W = None
+        else:
+            W = np.vstack([weights[idx][:-nstep:nstep, :] for idx, _ in items])
+
+        return X, Xp, U, W
 
     @property
     def differentiate(self) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
         r"""
         Numerical Differentiation -- Current State, Gradient State Estimate, Input
         """
         X = np.vstack([x.states[:-1, :] for _, x in self._trajs.items()]).T
@@ -620,7 +644,32 @@
 
         if self.input_names is not None:
             U = np.vstack([u.inputs[:-1, :] for _, u in self._trajs.items()]).T
         else:
             U = None
 
         return X, Xp, U
+
+    def differentiate_weights(
+        self, weights
+    ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
+        r"""
+        Numerical Differentiation with Weights -- Current State, Gradient State Estimate, Input, weight
+        """
+        items = list(self._trajs.items())
+
+        X = np.vstack([x.states[:-1, :] for _, x in items]).T
+
+        # finite difference
+        Xp = np.vstack([x.states[1:, :] for _, x in items]).T
+        Xp -= X
+        Xp /= self.sampling_period
+
+        if self.input_names is not None:
+            U = np.vstack([u.inputs[:-1, :] for _, u in items]).T
+        else:
+            U = None
+
+        # collect weights
+        W = np.hstack([weights[idx].flatten()[:-1] for idx, _ in items])
+
+        return X, Xp, U, W
```

### Comparing `autokoopman-0.30.4/autokoopman/core/tuner.py` & `autokoopman-0.30.6/autokoopman/core/tuner.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+"""Model Tuning
+"""
 import abc
 import random
 from typing import Sequence, Callable, TypedDict, Any
 import numpy as np
 
 from autokoopman.core.estimator import TrajectoryEstimator
 from autokoopman.core.trajectory import (
     TrajectoriesData,
     UniformTimeTrajectory,
     UniformTimeTrajectoriesData,
 )
+from autokoopman.core.scoring import TrajectoryScoring
 from autokoopman.core.format import _clip_list
 from sklearn.model_selection import KFold
 
 
 class Parameter:
     def __init__(self, name):
         self._name = name
@@ -132,41 +135,14 @@
 
 class TuneResults(TypedDict):
     model: TrajectoryEstimator
     param: Sequence[Any]
     score: float
 
 
-class TrajectoryScoring:
-    @staticmethod
-    def end_point_score(true_data: TrajectoriesData, prediction_data: TrajectoriesData):
-        errors = (prediction_data - true_data).norm()
-        end_errors = np.array([s.states[-1] for s in errors])
-        return np.mean(end_errors)
-
-    @staticmethod
-    def total_score(true_data: TrajectoriesData, prediction_data: TrajectoriesData):
-        errors = (prediction_data - true_data).norm()
-        end_errors = np.array([s.states.flatten() for s in errors])
-
-        return np.mean(np.concatenate(end_errors, axis=0))
-
-    @staticmethod
-    def relative_score(true_data: TrajectoriesData, prediction_data: TrajectoriesData):
-        # TODO: implement this
-        err_term = []
-        for k in prediction_data.traj_names:
-            pred_t = prediction_data[k]
-            true_t = true_data[k]
-            abs_error = np.linalg.norm(pred_t.states - true_t.states)
-            mean_error = np.linalg.norm(pred_t.states - np.mean(pred_t.states, axis=0))
-            err_term.append(abs_error / mean_error)
-        return np.mean(np.array(err_term))
-
-
 class HyperparameterTuner(abc.ABC):
     """
     Tune a HyperparameterMap Object
         The tuner implements a model learning pipeline that can take a mapping from hyperparameters to a model and
         training data and learn an optimized model. For example, given a SINDy estimator, hyperparameter tuner can
         implement gridsearch to find the best sparsity threshold and library type.
     """
```

### Comparing `autokoopman-0.30.4/autokoopman/estimator/deepkoopman.py` & `autokoopman-0.30.6/autokoopman/estimator/deepkoopman.py`

 * *Files 0% similar despite different names*

```diff
@@ -325,15 +325,15 @@
             else range(self.max_iter)
         ):
             risk = None
             # roll out over several steps
             for step_size in range(1, self.rollout_steps + 1):
                 # upload to GPU and normalize the data
                 # NOTE: this is expensive :(
-                X, Xn, U = trajs.n_step_matrices(step_size)
+                X, Xn, U, _ = trajs.n_step_matrices(step_size)
                 X = torch.tensor(X.T, dtype=torch.float32).to(self.device)
                 Xn = torch.tensor(Xn.T, dtype=torch.float32).to(self.device)
                 U = (
                     torch.tensor(U.T, dtype=torch.float32).to(self.device)
                     if self.has_input
                     else None
                 )
```

### Comparing `autokoopman-0.30.4/autokoopman/estimator/dmd.py` & `autokoopman-0.30.6/autokoopman/estimator/dmd.py`

 * *Files identical despite different names*

### Comparing `autokoopman-0.30.4/autokoopman/estimator/sindy.py` & `autokoopman-0.30.6/autokoopman/estimator/sindy.py`

 * *Files identical despite different names*

### Comparing `autokoopman-0.30.4/autokoopman/tuner/bayesianopt.py` & `autokoopman-0.30.6/autokoopman/tuner/bayesianopt.py`

 * *Files identical despite different names*

### Comparing `autokoopman-0.30.4/autokoopman/tuner/gridsearch.py` & `autokoopman-0.30.6/autokoopman/tuner/gridsearch.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,9 +62,10 @@
             try:
                 sampling.send(param)
                 next(sampling)
             except StopIteration:
                 break
             except Exception as exc:
                 print(f"Error: {exc}")
+                raise exc
                 self.error_messages.append((param, exc))
         return self.best_result
```

### Comparing `autokoopman-0.30.4/autokoopman/tuner/montecarlo.py` & `autokoopman-0.30.6/autokoopman/tuner/montecarlo.py`

 * *Files identical despite different names*

### Comparing `autokoopman-0.30.4/autokoopman.egg-info/PKG-INFO` & `autokoopman-0.30.6/autokoopman.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autokoopman
-Version: 0.30.4
+Version: 0.30.6
 Summary: Automated Koopman Operator Linearization Library
 Home-page: https://github.com/EthanJamesLew/AutoKoopman
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Intended Audience :: Science/Research
@@ -139,14 +139,34 @@
 *AutoKoopman Class Structure in the Training Pipeline*. A user can implement any of the classes to extend AutoKoopman (e.g., custom observables, a custom tuner, a new system id estimator).
 
 ## Documentation
 
 See the
 [AutoKoopman Documentation](https://ethanjameslew.github.io/AutoKoopman/).
 
+## Citing AutoKoopman
+
+AutoKoopman has been published as a tool paper at ATVA 2023. The preprint can be found [here](https://www.researchgate.net/profile/Ethan-Lew/publication/374805680_AutoKoopman_A_Toolbox_for_Automated_System_Identification_via_Koopman_Operator_Linearization/links/6537cf9f1d6e8a70704c7f31/AutoKoopman-A-Toolbox-for-Automated-System-Identification-via-Koopman-Operator-Linearization.pdf).
+
+If you cite AutoKoopman, please cite
+
+Lew, E., Hekal, A., Potomkin, K., Kochdumper, N., Hencey, B., Bak, S., & Bogomolov, S. (2023, October). Autokoopman: A toolbox for automated system identification via koopman operator linearization. In International Symposium on Automated Technology for Verification and Analysis (pp. 237-250). Cham: Springer Nature Switzerland.
+
+Bibtex:
+```
+@inproceedings{lew2023autokoopman,
+  title={Autokoopman: A toolbox for automated system identification via koopman operator linearization},
+  author={Lew, Ethan and Hekal, Abdelrahman and Potomkin, Kostiantyn and Kochdumper, Niklas and Hencey, Brandon and Bak, Stanley and Bogomolov, Sergiy},
+  booktitle={International Symposium on Automated Technology for Verification and Analysis},
+  pages={237--250},
+  year={2023},
+  organization={Springer}
+}
+```
+
 ## References  
 
 <a id="1">[1]</a> Williams, M. O., Kevrekidis, I. G., & Rowley, C. W. (2015). A data–driven approximation of the koopman operator: Extending dynamic mode decomposition. Journal of Nonlinear Science, 25, 1307-1346.
 
  <a id="2">[2]</a> Li, Y., He, H., Wu, J., Katabi, D., & Torralba, A. (2019). Learning compositional koopman operators for model-based control. arXiv preprint arXiv:1910.08264.
 
   <a id="3">[3]</a> Brunton, S. L., Proctor, J. L., & Kutz, J. N. (2016). Discovering governing equations from data by sparse identification of nonlinear dynamical systems. Proceedings of the national academy of sciences, 113(15), 3932-3937.
```

### Comparing `autokoopman-0.30.4/autokoopman.egg-info/SOURCES.txt` & `autokoopman-0.30.6/autokoopman.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -29,21 +29,25 @@
 autokoopman/benchmark/pendulum.py
 autokoopman/benchmark/prde20.py
 autokoopman/benchmark/robe21.py
 autokoopman/benchmark/spring.py
 autokoopman/core/__init__.py
 autokoopman/core/estimator.py
 autokoopman/core/format.py
-autokoopman/core/observables.py
+autokoopman/core/scoring.py
 autokoopman/core/system.py
 autokoopman/core/trajectory.py
 autokoopman/core/tuner.py
 autokoopman/core/visualizer.py
 autokoopman/estimator/__init__.py
 autokoopman/estimator/deepkoopman.py
 autokoopman/estimator/dmd.py
 autokoopman/estimator/koopman.py
 autokoopman/estimator/sindy.py
+autokoopman/observable/__init__.py
+autokoopman/observable/observables.py
+autokoopman/observable/reweighted.py
+autokoopman/observable/rff.py
 autokoopman/tuner/__init__.py
 autokoopman/tuner/bayesianopt.py
 autokoopman/tuner/gridsearch.py
 autokoopman/tuner/montecarlo.py
```

### Comparing `autokoopman-0.30.4/setup.py` & `autokoopman-0.30.6/setup.py`

 * *Files identical despite different names*

### Comparing `autokoopman-0.30.4/test/unit_test/test_deepk.py` & `autokoopman-0.30.6/test/unit_test/test_deepk.py`

 * *Files identical despite different names*

### Comparing `autokoopman-0.30.4/test/unit_test/test_koopman.py` & `autokoopman-0.30.6/test/unit_test/test_koopman.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,16 @@
     "normalize",
     koop_config,
 )
 def test_discrete_koopman(normalize):
     """tests the discrete time Koopman estimator"""
     from autokoopman.benchmark.pendulum import PendulumWithInput
     from autokoopman.core.trajectory import TrajectoriesData
-    from autokoopman.core.observables import IdentityObservable, RFFObservable
+    from autokoopman.observable.observables import IdentityObservable
+    from autokoopman.observable.rff import RFFObservable
     from autokoopman.estimator.koopman import KoopmanDiscEstimator
     import random
 
     pend = PendulumWithInput(l=0.6, beta=0.1)
     n_trajs = 40
     training_ivs = np.random.random((n_trajs, 2))
     trajs = {}
@@ -58,15 +59,16 @@
     "normalize",
     koop_config,
 )
 def test_cont_koopman(normalize):
     """tests the continuous time Koopman estimator"""
     from autokoopman.benchmark.pendulum import PendulumWithInput
     from autokoopman.core.trajectory import TrajectoriesData
-    from autokoopman.core.observables import IdentityObservable, RFFObservable
+    from autokoopman.observable.observables import IdentityObservable
+    from autokoopman.observable.rff import RFFObservable
     from autokoopman.estimator.koopman import KoopmanContinuousEstimator
     import random
 
     pend = PendulumWithInput(l=0.6, beta=0.1)
     n_trajs = 40
     training_ivs = np.random.random((n_trajs, 2))
     trajs = {}
```

### Comparing `autokoopman-0.30.4/test/unit_test/test_system.py` & `autokoopman-0.30.6/test/unit_test/test_system.py`

 * *Files identical despite different names*

### Comparing `autokoopman-0.30.4/test/unit_test/test_trajectory.py` & `autokoopman-0.30.6/test/unit_test/test_trajectory.py`

 * *Files identical despite different names*

