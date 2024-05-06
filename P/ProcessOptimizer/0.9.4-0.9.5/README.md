# Comparing `tmp/ProcessOptimizer-0.9.4.tar.gz` & `tmp/ProcessOptimizer-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProcessOptimizer-0.9.4.tar", last modified: Wed Feb 28 08:36:40 2024, max compression
+gzip compressed data, was "ProcessOptimizer-0.9.5.tar", last modified: Mon May  6 07:56:20 2024, max compression
```

## Comparing `ProcessOptimizer-0.9.4.tar` & `ProcessOptimizer-0.9.5.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxrwx   0        0        0        0 2024-02-28 08:36:40.785859 ProcessOptimizer-0.9.4/
--rw-rw-rw-   0        0        0     1238 2022-01-13 12:11:20.000000 ProcessOptimizer-0.9.4/AUTHORS_scikit_optimize.md
--rw-rw-rw-   0        0        0     1598 2024-02-22 15:02:59.000000 ProcessOptimizer-0.9.4/LICENSE.md
--rw-rw-rw-   0        0        0       61 2024-02-23 12:16:04.000000 ProcessOptimizer-0.9.4/MANIFEST.in
--rw-rw-rw-   0        0        0    10799 2024-02-28 08:36:40.785859 ProcessOptimizer-0.9.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-02-28 08:36:39.535332 ProcessOptimizer-0.9.4/ProcessOptimizer/
--rw-rw-rw-   0        0        0     1978 2024-02-28 08:34:59.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/__init__.py
--rw-rw-rw-   0        0        0    11574 2024-02-20 09:33:34.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/acquisition.py
--rw-rw-rw-   0        0        0    29136 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/bokeh_plot.py
--rw-rw-rw-   0        0        0     8781 2022-01-13 12:11:20.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/callbacks.py
-drwxrwxrwx   0        0        0        0 2024-02-28 08:36:39.746841 ProcessOptimizer-0.9.4/ProcessOptimizer/learning/
--rw-rw-rw-   0        0        0      609 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/learning/__init__.py
--rw-rw-rw-   0        0        0     4461 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/learning/cook_estimator.py
--rw-rw-rw-   0        0        0    18829 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/learning/forest.py
-drwxrwxrwx   0        0        0        0 2024-02-28 08:36:39.807767 ProcessOptimizer-0.9.4/ProcessOptimizer/learning/gaussian_process/
--rw-rw-rw-   0        0        0       85 2021-03-19 12:03:36.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/learning/gaussian_process/__init__.py
--rw-rw-rw-   0        0        0    17518 2023-06-07 11:59:09.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/learning/gaussian_process/gpr.py
--rw-rw-rw-   0        0        0    15220 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/learning/gaussian_process/kernels.py
--rw-rw-rw-   0        0        0     4809 2021-09-23 13:20:36.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/learning/gbrt.py
--rw-rw-rw-   0        0        0     1018 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/learning/has_gradients.py
--rw-rw-rw-   0        0        0     5785 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/learning/use_named_args.py
-drwxrwxrwx   0        0        0        0 2024-02-28 08:36:40.166017 ProcessOptimizer-0.9.4/ProcessOptimizer/model_systems/
--rw-rw-rw-   0        0        0     1007 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/model_systems/__init__.py
--rw-rw-rw-   0        0        0     1579 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/model_systems/benchmarks.py
--rw-rw-rw-   0        0        0     1625 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/model_systems/branin_hoo.py
--rw-rw-rw-   0        0        0    12690 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/model_systems/color_pH.py
-drwxrwxrwx   0        0        0        0 2024-02-28 08:36:40.206639 ProcessOptimizer-0.9.4/ProcessOptimizer/model_systems/data/
--rw-rw-rw-   0        0        0        0 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/model_systems/data/__init__.py
--rw-rw-rw-   0        0        0     6528 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/model_systems/data/color_pH_data.csv
--rw-rw-rw-   0        0        0      815 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/model_systems/gold_map.py
--rw-rw-rw-   0        0        0      897 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/model_systems/gold_map_with_wells.py
--rw-rw-rw-   0        0        0     1650 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/model_systems/hart3.py
--rw-rw-rw-   0        0        0     2021 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/model_systems/hart6.py
--rw-rw-rw-   0        0        0     5149 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/model_systems/model_system.py
--rw-rw-rw-   0        0        0     8658 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/model_systems/noise_models.py
--rw-rw-rw-   0        0        0     1322 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/model_systems/peaks.py
--rw-rw-rw-   0        0        0     1186 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/model_systems/poly2.py
--rw-rw-rw-   0        0        0     1356 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/model_systems/second_order_polynomial_2d.py
-drwxrwxrwx   0        0        0        0 2024-02-28 08:36:40.400583 ProcessOptimizer-0.9.4/ProcessOptimizer/optimizer/
--rw-rw-rw-   0        0        0     3562 2022-01-13 12:11:20.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/optimizer/_NSGA2.py
--rw-rw-rw-   0        0        0      334 2021-03-19 12:03:36.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/optimizer/__init__.py
--rw-rw-rw-   0        0        0    11223 2022-01-13 12:11:20.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/optimizer/base.py
--rw-rw-rw-   0        0        0     4335 2022-01-13 12:11:20.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/optimizer/dummy.py
--rw-rw-rw-   0        0        0     7101 2022-01-13 12:11:20.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/optimizer/forest.py
--rw-rw-rw-   0        0        0     6798 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/optimizer/gbrt.py
--rw-rw-rw-   0        0        0    10870 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/optimizer/gp.py
--rw-rw-rw-   0        0        0    50429 2024-02-28 08:34:59.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/optimizer/optimizer.py
--rw-rw-rw-   0        0        0    89768 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/plots.py
--rw-rw-rw-   0        0        0    28599 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/searchcv.py
-drwxrwxrwx   0        0        0        0 2024-02-28 08:36:40.613359 ProcessOptimizer-0.9.4/ProcessOptimizer/space/
--rw-rw-rw-   0        0        0      127 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/space/__init__.py
--rw-rw-rw-   0        0        0    42212 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/space/constraints.py
--rw-rw-rw-   0        0        0     2582 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/space/normalize_dimensions.py
--rw-rw-rw-   0        0        0    30914 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/space/space.py
--rw-rw-rw-   0        0        0     5265 2023-05-02 07:34:39.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/space/transformers.py
-drwxrwxrwx   0        0        0        0 2024-02-28 08:36:40.775639 ProcessOptimizer-0.9.4/ProcessOptimizer/utils/
--rw-rw-rw-   0        0        0      671 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/utils/__init__.py
--rw-rw-rw-   0        0        0     1183 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/utils/get_rng.py
--rw-rw-rw-   0        0        0    20624 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.4/ProcessOptimizer/utils/utils.py
-drwxrwxrwx   0        0        0        0 2024-02-28 08:36:39.573905 ProcessOptimizer-0.9.4/ProcessOptimizer.egg-info/
--rw-rw-rw-   0        0        0    10799 2024-02-28 08:36:36.000000 ProcessOptimizer-0.9.4/ProcessOptimizer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2116 2024-02-28 08:36:37.000000 ProcessOptimizer-0.9.4/ProcessOptimizer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-28 08:36:36.000000 ProcessOptimizer-0.9.4/ProcessOptimizer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      261 2024-02-28 08:36:36.000000 ProcessOptimizer-0.9.4/ProcessOptimizer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-02-28 08:36:36.000000 ProcessOptimizer-0.9.4/ProcessOptimizer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10374 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.4/README.md
--rw-rw-rw-   0        0        0       42 2024-02-28 08:36:40.785859 ProcessOptimizer-0.9.4/setup.cfg
--rw-rw-rw-   0        0        0     1655 2024-02-28 08:34:59.000000 ProcessOptimizer-0.9.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 07:56:20.533451 ProcessOptimizer-0.9.5/
+-rw-rw-rw-   0        0        0     1238 2022-01-13 12:11:20.000000 ProcessOptimizer-0.9.5/AUTHORS_scikit_optimize.md
+-rw-rw-rw-   0        0        0     1598 2024-02-22 15:02:59.000000 ProcessOptimizer-0.9.5/LICENSE.md
+-rw-rw-rw-   0        0        0       61 2024-02-23 12:16:04.000000 ProcessOptimizer-0.9.5/MANIFEST.in
+-rw-rw-rw-   0        0        0    11011 2024-05-06 07:56:20.532452 ProcessOptimizer-0.9.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-06 07:56:20.083729 ProcessOptimizer-0.9.5/ProcessOptimizer/
+-rw-rw-rw-   0        0        0     1978 2024-05-06 07:52:55.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/__init__.py
+-rw-rw-rw-   0        0        0    11574 2024-03-08 11:21:22.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/acquisition.py
+-rw-rw-rw-   0        0        0    29144 2024-05-06 07:46:36.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/bokeh_plot.py
+-rw-rw-rw-   0        0        0     8781 2022-01-13 12:11:20.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/callbacks.py
+drwxrwxrwx   0        0        0        0 2024-05-06 07:56:20.165724 ProcessOptimizer-0.9.5/ProcessOptimizer/learning/
+-rw-rw-rw-   0        0        0      609 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/learning/__init__.py
+-rw-rw-rw-   0        0        0     4461 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/learning/cook_estimator.py
+-rw-rw-rw-   0        0        0    18829 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/learning/forest.py
+drwxrwxrwx   0        0        0        0 2024-05-06 07:56:20.196723 ProcessOptimizer-0.9.5/ProcessOptimizer/learning/gaussian_process/
+-rw-rw-rw-   0        0        0       85 2021-03-19 12:03:36.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/learning/gaussian_process/__init__.py
+-rw-rw-rw-   0        0        0    17518 2023-06-07 11:59:09.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/learning/gaussian_process/gpr.py
+-rw-rw-rw-   0        0        0    15220 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/learning/gaussian_process/kernels.py
+-rw-rw-rw-   0        0        0     4809 2021-09-23 13:20:36.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/learning/gbrt.py
+-rw-rw-rw-   0        0        0     1018 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/learning/has_gradients.py
+-rw-rw-rw-   0        0        0     5785 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/learning/use_named_args.py
+drwxrwxrwx   0        0        0        0 2024-05-06 07:56:20.334785 ProcessOptimizer-0.9.5/ProcessOptimizer/model_systems/
+-rw-rw-rw-   0        0        0     1007 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/model_systems/__init__.py
+-rw-rw-rw-   0        0        0     1579 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/model_systems/benchmarks.py
+-rw-rw-rw-   0        0        0     1625 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/model_systems/branin_hoo.py
+-rw-rw-rw-   0        0        0    12690 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/model_systems/color_pH.py
+drwxrwxrwx   0        0        0        0 2024-05-06 07:56:20.355795 ProcessOptimizer-0.9.5/ProcessOptimizer/model_systems/data/
+-rw-rw-rw-   0        0        0        0 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/model_systems/data/__init__.py
+-rw-rw-rw-   0        0        0     6528 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/model_systems/data/color_pH_data.csv
+-rw-rw-rw-   0        0        0      815 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/model_systems/gold_map.py
+-rw-rw-rw-   0        0        0      897 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/model_systems/gold_map_with_wells.py
+-rw-rw-rw-   0        0        0     1650 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/model_systems/hart3.py
+-rw-rw-rw-   0        0        0     2021 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/model_systems/hart6.py
+-rw-rw-rw-   0        0        0     5149 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/model_systems/model_system.py
+-rw-rw-rw-   0        0        0     8658 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/model_systems/noise_models.py
+-rw-rw-rw-   0        0        0     1322 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/model_systems/peaks.py
+-rw-rw-rw-   0        0        0     1186 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/model_systems/poly2.py
+-rw-rw-rw-   0        0        0     1356 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/model_systems/second_order_polynomial_2d.py
+drwxrwxrwx   0        0        0        0 2024-05-06 07:56:20.438468 ProcessOptimizer-0.9.5/ProcessOptimizer/optimizer/
+-rw-rw-rw-   0        0        0     3562 2022-01-13 12:11:20.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/optimizer/_NSGA2.py
+-rw-rw-rw-   0        0        0      334 2021-03-19 12:03:36.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/optimizer/__init__.py
+-rw-rw-rw-   0        0        0    11223 2022-01-13 12:11:20.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/optimizer/base.py
+-rw-rw-rw-   0        0        0     4335 2022-01-13 12:11:20.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/optimizer/dummy.py
+-rw-rw-rw-   0        0        0     7101 2022-01-13 12:11:20.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/optimizer/forest.py
+-rw-rw-rw-   0        0        0     6798 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/optimizer/gbrt.py
+-rw-rw-rw-   0        0        0    10870 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/optimizer/gp.py
+-rw-rw-rw-   0        0        0    56587 2024-04-08 08:00:30.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/optimizer/optimizer.py
+-rw-rw-rw-   0        0        0    89770 2024-05-06 07:46:36.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/plots.py
+-rw-rw-rw-   0        0        0    28599 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/searchcv.py
+drwxrwxrwx   0        0        0        0 2024-05-06 07:56:20.497453 ProcessOptimizer-0.9.5/ProcessOptimizer/space/
+-rw-rw-rw-   0        0        0      127 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/space/__init__.py
+-rw-rw-rw-   0        0        0    42212 2024-03-08 11:21:22.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/space/constraints.py
+-rw-rw-rw-   0        0        0     2582 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/space/normalize_dimensions.py
+-rw-rw-rw-   0        0        0    30914 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/space/space.py
+-rw-rw-rw-   0        0        0     5265 2023-05-02 07:34:39.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/space/transformers.py
+drwxrwxrwx   0        0        0        0 2024-05-06 07:56:20.527451 ProcessOptimizer-0.9.5/ProcessOptimizer/utils/
+-rw-rw-rw-   0        0        0      671 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/utils/__init__.py
+-rw-rw-rw-   0        0        0     1183 2024-02-23 12:16:05.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/utils/get_rng.py
+-rw-rw-rw-   0        0        0    20636 2024-05-06 07:46:36.000000 ProcessOptimizer-0.9.5/ProcessOptimizer/utils/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-06 07:56:20.104728 ProcessOptimizer-0.9.5/ProcessOptimizer.egg-info/
+-rw-rw-rw-   0        0        0    11011 2024-05-06 07:56:16.000000 ProcessOptimizer-0.9.5/ProcessOptimizer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2116 2024-05-06 07:56:18.000000 ProcessOptimizer-0.9.5/ProcessOptimizer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 07:56:16.000000 ProcessOptimizer-0.9.5/ProcessOptimizer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      197 2024-05-06 07:56:16.000000 ProcessOptimizer-0.9.5/ProcessOptimizer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-06 07:56:16.000000 ProcessOptimizer-0.9.5/ProcessOptimizer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10586 2024-04-08 08:00:30.000000 ProcessOptimizer-0.9.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-06 07:56:20.534453 ProcessOptimizer-0.9.5/setup.cfg
+-rw-rw-rw-   0        0        0     1575 2024-05-06 07:52:55.000000 ProcessOptimizer-0.9.5/setup.py
```

### Comparing `ProcessOptimizer-0.9.4/AUTHORS_scikit_optimize.md` & `ProcessOptimizer-0.9.5/AUTHORS_scikit_optimize.md`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/LICENSE.md` & `ProcessOptimizer-0.9.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/PKG-INFO` & `ProcessOptimizer-0.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProcessOptimizer
-Version: 0.9.4
+Version: 0.9.5
 Summary: Sequential model-based optimization toolbox     (forked from scikit-optimize)
 Home-page: https://github.com/novonordisk-research/ProcessOptimizer
 Author: Novo Nordisk, Research & Early Development
 License: BSD
 Description-Content-Type: text/markdown
 Provides-Extra: browniebee
 License-File: LICENSE.md
@@ -17,16 +17,16 @@
  | |__) | __ ___   ___ ___  ___ ___| |  | |_ __ | |_ _ _ __ ___  _ _______ _ __ 
  |  ___/ '__/ _ \ / __/ _ \/ __/ __| |  | | '_ \| __| | '_ ` _ \| |_  / _ \ '__|
  | |   | | | (_) | (_|  __/\__ \__ \ |__| | |_) | |_| | | | | | | |/ /  __/ |   
  |_|   |_|  \___/ \___\___||___/___/\____/| .__/ \__|_|_| |_| |_|_/___\___|_|   
                                           | |                                   
                                           |_|                                   
 </pre>
-<a href="https://badge.fury.io/py/ProcessOptimizer"><img src="https://badge.fury.io/py/ProcessOptimizer.svg" alt="PyPI version" height="18"></a>
-<a href="https://github.com/novonordisk-research/ProcessOptimizer/actions"><img src="https://github.com/novonordisk-research/ProcessOptimizer/workflows/Python%20package/badge.svg" alt="Tests" height="18"></a>
+<a href="https://badge.fury.io/py/ProcessOptimizer"><img src="https://badge.fury.io/py/ProcessOptimizer.svg" alt="PyPI version"></a>
+<a href="https://github.com/novonordisk-research/ProcessOptimizer/actions"><img src="https://github.com/novonordisk-research/ProcessOptimizer/actions/workflows/python-package-tests.yml/badge.svg" alt="Tests"></a>
 <a href="https://www.python.org/"><img src="https://img.shields.io/badge/built%20with-Python3-green.svg" alt="built with Python3" /></a>
 <a href="https://www.python.org/"><img src="https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue" alt="Runs on" /></a>
 <a href="https://github.com/novonordisk-research/ProcessOptimizer/blob/develop/LICENSE.md"><img src="https://img.shields.io/pypi/l/ProcessOptimizer" alt="PyPI - License" /></a>
 <a href="https://scikit-optimize.github.io/stable/"><img src="https://img.shields.io/badge/BuildOn-Scikit--Optimize-brightgreen" alt="Scikit-Optimize" /></a>
 <a href="https://doi.org/10.5281/zenodo.5155295"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.5155295.svg" alt="DOI"></a>
 
 [![Downloads](https://static.pepy.tech/personalized-badge/processoptimizer?period=total&units=international_system&left_color=brightgreen&right_color=orange&left_text=Downloads)](https://pepy.tech/project/processoptimizer)
@@ -138,7 +138,8 @@
 
 - In terminal run the command "pytest" and make sure there are no errors
 - Change version number in setup.py
 - Change version number in ProcessOptimizer/\_\_init\_\_.py
 - Remember to `pip install twine` if running in a new virtual env. (You might also have to `pip install wheel`)
 - Run `python setup.py sdist bdist_wheel`
 - Run `python -m twine upload dist/*` (make sure that /dist only contains relevant version)
+- (Remember that pypi has changed the way it handles credentials, you might have to state username: __token__ and then use your token value (incl pypi-prefix) as password. As stated here https://pypi.org/help/#apitoken
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ProcessOptimizer Version: 0.9.4 Summary: Sequential
+Metadata-Version: 2.1 Name: ProcessOptimizer Version: 0.9.5 Summary: Sequential
 model-based optimization toolbox (forked from scikit-optimize) Home-page:
 https://github.com/novonordisk-research/ProcessOptimizer Author: Novo Nordisk,
 Research & Early Development License: BSD Description-Content-Type: text/
 markdown Provides-Extra: browniebee License-File: LICENSE.md License-File:
 AUTHORS_scikit_optimize.md
         _____                              ____        _   _           _
 
@@ -134,8 +134,11 @@
 https://packaging.python.org/tutorials/packaging-projects/ To upload a new
 version to PyPi do the following in the root folder of the project: - In
 terminal run the command "pytest" and make sure there are no errors - Change
 version number in setup.py - Change version number in ProcessOptimizer/
 \_\_init\_\_.py - Remember to `pip install twine` if running in a new virtual
 env. (You might also have to `pip install wheel`) - Run `python setup.py sdist
 bdist_wheel` - Run `python -m twine upload dist/*` (make sure that /dist only
-contains relevant version)
+contains relevant version) - (Remember that pypi has changed the way it handles
+credentials, you might have to state username: __token__ and then use your
+token value (incl pypi-prefix) as password. As stated here https://pypi.org/
+help/#apitoken
```

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/__init__.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from .utils import expected_minimum_random_sampling
 from .utils import load
 from .utils import create_result, y_coverage
 from .plots import plot_objective, plot_objectives
 from .plots import plot_evaluations, plot_convergence
 from .plots import plot_Pareto, plot_expected_minimum_convergence
 
-__version__ = "0.9.4"
+__version__ = "0.9.5"
 
 
 __all__ = (
     "acquisition",
     "benchmarks",
     "ModelSystem",
     "callbacks",
```

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/acquisition.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/acquisition.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/bokeh_plot.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/bokeh_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -421,17 +421,17 @@
                 source_samples = ColumnDataSource(
                     data=dict(x=x_samples, y=y_samples))
                 source_red = ColumnDataSource(
                     data=dict(x=[red_vals[j]], y=[red_vals[i]]))
                 # We plot samples as black circles and the evaluation marker
                 # as a red circle.
                 plot.circle(x='x', y='y', source=source_samples,
-                            size=2, color="black", alpha=0.5)
+                            radius=0.2, color="black", alpha=0.5)
                 plot.circle(x='x', y='y', source=source_red,
-                            size=5, color="red", alpha=1)
+                            radius=0.5, color="red", alpha=1)
 
             # We rotate the categorical labels slighty
             # so they take up less space
             if iscat[j]:
                 plot.xaxis.major_label_orientation = 0.3
             if iscat[i] and i != j:
                 # In case of diagonal, the y-labels are numbers
```

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/callbacks.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/callbacks.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/learning/__init__.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/learning/__init__.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/learning/cook_estimator.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/learning/cook_estimator.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/learning/forest.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/learning/forest.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/learning/gaussian_process/gpr.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/learning/gaussian_process/gpr.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/learning/gaussian_process/kernels.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/learning/gaussian_process/kernels.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/learning/gbrt.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/learning/gbrt.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/learning/has_gradients.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/learning/has_gradients.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/learning/use_named_args.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/learning/use_named_args.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/model_systems/__init__.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/model_systems/__init__.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/model_systems/benchmarks.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/model_systems/benchmarks.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/model_systems/branin_hoo.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/model_systems/branin_hoo.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/model_systems/color_pH.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/model_systems/color_pH.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/model_systems/data/color_pH_data.csv` & `ProcessOptimizer-0.9.5/ProcessOptimizer/model_systems/data/color_pH_data.csv`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/model_systems/gold_map.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/model_systems/gold_map.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/model_systems/gold_map_with_wells.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/model_systems/gold_map_with_wells.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/model_systems/hart3.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/model_systems/hart3.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/model_systems/hart6.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/model_systems/hart6.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/model_systems/model_system.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/model_systems/model_system.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/model_systems/noise_models.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/model_systems/noise_models.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/model_systems/peaks.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/model_systems/peaks.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/model_systems/poly2.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/model_systems/poly2.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/model_systems/second_order_polynomial_2d.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/model_systems/second_order_polynomial_2d.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/optimizer/_NSGA2.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/optimizer/_NSGA2.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/optimizer/base.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/optimizer/base.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/optimizer/dummy.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/optimizer/dummy.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/optimizer/forest.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/optimizer/forest.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/optimizer/gbrt.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/optimizer/gbrt.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/optimizer/gp.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/optimizer/gp.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/optimizer/optimizer.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/optimizer/optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import sys
 import warnings
+from collections import namedtuple
 from math import log
 from numbers import Number
+from typing import Collection, List
 
 import numpy as np
 
 from joblib import Parallel, delayed
 
 from scipy.optimize import fmin_l_bfgs_b
 
@@ -39,17 +41,17 @@
     Use this class directly if you want to control the iterations of your
     bayesian optimisation loop.
 
     In default behavior, the optimizer will reset the modelled experimental
     noise between each refitting (read: while adding new data). This is
     described in Rasmussen and Williams chapter 2.
     Some users might want to plot, predict or sample from a model that includes
-    the modelling of the experimental noise: in that case, two helper methods
-    can "switch" the noise "on/off". Functions are called 'add_modelled_noise'
-    and 'remove_modelled_noise'.
+    the modelling of the observational noise: in that case, two helper methods
+    can "switch" the noise "on/off". Functions are called 'add_observational_noise'
+    and 'remove_observational_noise'.
 
     Parameters
     ----------
     * `dimensions` [list, shape=(n_dims,)]:
         List of search space dimensions.
         Each search dimension can be defined either as
 
@@ -139,15 +141,16 @@
         - "n_restarts_optimizer" [int]
         - "n_jobs" [int]
 
     * `n_objectives` [int, default=1]:
         Number of objectives to be optimized.
         When n_objectives>1 the optimizer will fit models for each objective and the Pareto front can be approximated using NSGA2
 
-
+    * `objective_name_list` [list[str], default ["Y"] or ["Y1","Y2",...]]:
+        The names of the objetive(s).
 
     Attributes
     ----------
     * `Xi` [list]:
         Points at which objective has been evaluated.
     * `yi` [scalar]:
         Values of objective at corresponding points in `Xi`.
@@ -169,14 +172,15 @@
         lhs=True,
         acq_func="EI",
         acq_optimizer="auto",
         random_state=None,
         acq_func_kwargs=None,
         acq_optimizer_kwargs=None,
         n_objectives=1,
+        objective_name_list: List[str] = None,
     ):
         self.rng = check_random_state(random_state)
 
         # Set the number of objectives
         self.n_objectives = n_objectives
 
         # Configure acquisition function
@@ -308,14 +312,30 @@
         self._non_cat_inds = []
         for ind, dim in enumerate(self.space.dimensions):
             if isinstance(dim, Categorical):
                 self._cat_inds.append(ind)
             else:
                 self._non_cat_inds.append(ind)
 
+        # Setting the objective name list
+        if objective_name_list is None:
+            if n_objectives == 1:
+                objective_name_list = ["Y"]
+            else:
+                objective_name_list = [
+                    f"Y{num+1}" for num in range(n_objectives)
+                ]
+        if len(objective_name_list) != n_objectives:
+            raise ValueError(
+                "Objective name list must have length n_objectives "
+                f"({n_objectives}), but has length {len(objective_name_list)} "
+                f"(content {objective_name_list})"
+            )
+        self.objective_name_list = objective_name_list
+
         # Initialize storage for optimization
 
         self.models = []
         self.Xi = []
         self.yi = []
 
         # Initialize cache for `ask` method responses
@@ -820,14 +840,108 @@
             self.yi,
             self.space,
             self.rng,
             models=self.models,
             constraints=self._constraints,
         )
 
+    def estimate(self, x: Collection) -> List[namedtuple]:
+        """
+        Estimates the objective function value(s) for the point(s) `x`.
+
+        Parameters
+        ----------
+        * `x` [list or list-of-lists]:
+            Point(s) at which to estimate the objective function value(s).
+
+        Returns
+        -------
+        * `y` [list[namedtuple]]:
+            List of estimations with the same length as `x`. Each element has
+            a field per objective of the optimizer named after the objectives
+            ("Y" or "Y1", "Y2",... by default). Each objective field contains
+            a single objective estimation with field names "mean" and "std".
+            For single objective optimizers, the estimation has the fields
+            "mean" and "std", and a field with the same name as the objective
+            ("Y" by default), which in turn has the fields "mean" and "std".
+        """
+        self_with_observation_noise = self.copy()
+        self_with_observation_noise.add_observational_noise()
+        self_without_observation_noise = self.copy()
+        self_without_observation_noise.remove_observational_noise()
+        single_objective_estimation = namedtuple(
+            "single_objective_estimation", ["mean", "std", "std_model"]
+        )
+        check_x_in_space(x, self.space)
+        if not is_2Dlistlike(x):
+            x = np.asarray(x).reshape(1, -1).tolist()
+            # If only one point is given, make it an array
+        transformed_x = self.space.transform(x)
+        if self.n_objectives == 1:
+            estimation = namedtuple(
+                "estimation",
+                self.objective_name_list
+                + list(single_objective_estimation._fields),
+            )  # For single objective optimizers, the returned list's elements
+            # are namedtuples, with a field named after the objective ("Y" by
+            # default), which in turn has the fields "mean" and "std", for
+            # consistency with multiobjective. They also have the fields "mean"
+            # and "std", for ease of use.
+            prediction = self_with_observation_noise.models[-1].predict(
+                transformed_x, return_std=True
+            )
+            (_, noiseless_predicted_std) = self_without_observation_noise.models[-1].predict(
+                transformed_x, return_std=True
+            )
+            # The estimate is "packed" different than sci-kit learn predictions
+            # are. The predictions are a tuple of two arrays, one for the mean
+            # and one for the standard deviation; each array has one element
+            # per parameter combination. The estimate is a list of namedtuples,
+            # each with two fields, one for the mean and one for the standard
+            # deviation; each list element corresponds to one parameter
+            # combination.
+            estimate_list = [
+                estimation(
+                    single_objective_estimation(mean, std, std_model),
+                    mean,
+                    std,
+                    std_model
+                ) for
+                mean, std, std_model in zip(
+                    prediction[0], prediction[1], noiseless_predicted_std
+                )
+            ]
+        else:
+            estimation = namedtuple("estimation", self.objective_name_list)
+            # Make a list of predictions, one for each objective. This is a
+            # list of tuples, each tuple containing two arrays, one for the
+            # mean and one for the standard deviation; each array has one
+            # element per x.
+            predict_list = [
+                model.predict(transformed_x, return_std=True) for
+                model in self_with_observation_noise.models[-1]
+            ]
+            noiseless_predict_list = [
+                model.predict(transformed_x, return_std=True) for
+                model in self_without_observation_noise.models[-1]
+            ]
+            estimate_list = []
+            for i in range(len(x)):
+                # For each x and objective, create the
+                # single_objective_estimation and append it to the list of
+                # estimations for that x
+                estimate_list.append([single_objective_estimation(
+                            predict_list[j][0][i],
+                            predict_list[j][1][i],
+                            noiseless_predict_list[j][1][i]
+                        ) for j in range(self.n_objectives)])
+            # Packing the list of estimations for each x into a namedtuple.
+            estimate_list = [estimation(*result) for result in estimate_list]
+        return estimate_list
+
     def _check_y_is_valid(self, x, y):
         """Check if the shape and types of x and y are consistent."""
 
         if "ps" in self.acq_func:
             if is_2Dlistlike(x):
                 if not (np.ndim(y) == 2 and np.shape(y)[1] == 2):
                     raise TypeError("expected y to be a list of (func_val, t)")
@@ -1155,51 +1269,65 @@
             self.__ObjectiveGP,
             np.array(self.space.transformed_bounds),
             MU=MU,
         )
 
         return pop, logbook, front
 
-    # This function adds the modelled white noise to the regressor to allow predictions including noise
-    def add_modelled_noise(self):
+    def add_observational_noise(self):
         """
-        This method will add the noise that has been modelled to fit the data. (The noise is disabled
-        by default to reflect description in book on gaussian processes for Machine Learning
-        This has been described in Eq 2.24 of
-        http://www.gaussianprocess.org/gpml/chapters/RW2.pdf)
+        This method will add the noise that has been modelled to fit the data.
+        (The noise is disabled by default to reflect description in book on
+        gaussian processes for Machine Learning. This has been described in
+        Eq 2.24 of http://www.gaussianprocess.org/gpml/chapters/RW2.pdf)
         """
+        if self.n_objectives > 1:
+            for model in self.models[-1]:
+                self.add_observational_noise_single_model(model)
+        else:
+            self.add_observational_noise_single_model(self.models[-1])
+
+    # This function adds the modelled white noise to the regressor to allow predictions including noise
+    def add_observational_noise_single_model(self, model):
         if (
-            isinstance(self.models[-1].noise, str)
-            and self.models[-1].noise != "gaussian"
+            isinstance(model.noise, str)
+            and model.noise != "gaussian"
         ):
             raise ValueError(
-                "Expected noise to be 'gaussian', got %s" % self.models[-1].noise
+                "Expected noise to be 'gaussian', got %s" % model.noise
             )
-        noise_estimate = self.models[-1].noise_
+        noise_estimate = model.noise_
         white_present, white_param = _param_for_white_kernel_in_Sum(
-            self.models[-1].kernel_
+            model.kernel_
         )
         if white_present:
-            self.models[-1].kernel_.set_params(
+            model.kernel_.set_params(
                 **{white_param: WhiteKernel(noise_level=noise_estimate)}
             )
 
-    def remove_modelled_noise(self):
+    def remove_observational_noise(self):
         """
-        This method resets the noise levels to only include the "true" uncertaincy of the main kernel
-        used for fitting and predicting. This method can be used in conjunction with the
-        'add_modelled_noise()'
+        This method resets the noise levels to only include the "true"
+        uncertaincy of the main kernel used for fitting and predicting. This
+        method can be used in conjunction with the 'add_modelled_noise()'
         """
+        if self.n_objectives > 1:
+            for model in self.models[-1]:
+                self.remove_observational_noise_single_model(model)
+        else:
+            self.remove_observational_noise_single_model(self.models[-1])
+
+    def remove_observational_noise_single_model(self, model):
         if (
-            isinstance(self.models[-1].noise, str)
-            and self.models[-1].noise != "gaussian"
+            isinstance(model.noise, str)
+            and model.noise != "gaussian"
         ):
             raise ValueError(
-                "expected noise to be 'gaussian', got %s" % self.models[-1].noise
+                "expected noise to be 'gaussian', got %s" % model.noise
             )
         white_present, white_param = _param_for_white_kernel_in_Sum(
-            self.models[-1].kernel_
+            model.kernel_
         )
         if white_present:
-            self.models[-1].kernel_.set_params(
+            model.kernel_.set_params(
                 **{white_param: WhiteKernel(noise_level=0.0)}
             )
```

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/plots.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -2295,15 +2295,15 @@
             height_policy = 'max',
             )
 
     # Plot observed data and create Tooltip
     r1 = p.circle(
             list(data_observed_dict.keys())[0],
             list(data_observed_dict.keys())[1],
-            size=10,
+            radius=1,
             source=source_observed,
             legend_label="Observed datapoints",
             fill_alpha=0.4,
             )
     p.add_tools(
             bh_models.HoverTool(
                 renderers=[r1],
@@ -2313,15 +2313,15 @@
                 )
             )
 
     # Plot Pareto-front and create Tooltip
     r2 = p.circle(
             list(data_calculated_dict.keys())[0],
             list(data_calculated_dict.keys())[1],
-            size=10,
+            radius=1,
             source=source_calculated,
             color="red",
             legend_label="Estimated Pareto front",
             )
     p.add_tools(
             bh_models.HoverTool(
                 renderers=[r2],
```

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/searchcv.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/searchcv.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/space/constraints.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/space/constraints.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/space/normalize_dimensions.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/space/normalize_dimensions.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/space/space.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/space/space.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/space/transformers.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/space/transformers.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/utils/__init__.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/utils/get_rng.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/utils/get_rng.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer/utils/utils.py` & `ProcessOptimizer-0.9.5/ProcessOptimizer/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -290,15 +290,15 @@
     best_x = None
     best_fun = np.inf
     
     
     cons = None
     # Prepare a linear constraint, if applicable
     if hasattr(res.constraints, "sum_equals"):
-        A = np.zeros((1, res.space.n_dims))
+        A = np.zeros((1, res.space.transformed_n_dims))
         value = res.constraints.sum_equals[0].value
         for dim in res.constraints.sum_equals[0].dimensions:
             # Normalization rescales the ratio that the constrained dimensions 
             # need to be added together, by an amount that depends on the length
             # of each dimension
             dim_length = res.space.bounds[dim][1] - res.space.bounds[dim][0]
             A[0, dim] = dim_length/value
```

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer.egg-info/PKG-INFO` & `ProcessOptimizer-0.9.5/ProcessOptimizer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProcessOptimizer
-Version: 0.9.4
+Version: 0.9.5
 Summary: Sequential model-based optimization toolbox     (forked from scikit-optimize)
 Home-page: https://github.com/novonordisk-research/ProcessOptimizer
 Author: Novo Nordisk, Research & Early Development
 License: BSD
 Description-Content-Type: text/markdown
 Provides-Extra: browniebee
 License-File: LICENSE.md
@@ -17,16 +17,16 @@
  | |__) | __ ___   ___ ___  ___ ___| |  | |_ __ | |_ _ _ __ ___  _ _______ _ __ 
  |  ___/ '__/ _ \ / __/ _ \/ __/ __| |  | | '_ \| __| | '_ ` _ \| |_  / _ \ '__|
  | |   | | | (_) | (_|  __/\__ \__ \ |__| | |_) | |_| | | | | | | |/ /  __/ |   
  |_|   |_|  \___/ \___\___||___/___/\____/| .__/ \__|_|_| |_| |_|_/___\___|_|   
                                           | |                                   
                                           |_|                                   
 </pre>
-<a href="https://badge.fury.io/py/ProcessOptimizer"><img src="https://badge.fury.io/py/ProcessOptimizer.svg" alt="PyPI version" height="18"></a>
-<a href="https://github.com/novonordisk-research/ProcessOptimizer/actions"><img src="https://github.com/novonordisk-research/ProcessOptimizer/workflows/Python%20package/badge.svg" alt="Tests" height="18"></a>
+<a href="https://badge.fury.io/py/ProcessOptimizer"><img src="https://badge.fury.io/py/ProcessOptimizer.svg" alt="PyPI version"></a>
+<a href="https://github.com/novonordisk-research/ProcessOptimizer/actions"><img src="https://github.com/novonordisk-research/ProcessOptimizer/actions/workflows/python-package-tests.yml/badge.svg" alt="Tests"></a>
 <a href="https://www.python.org/"><img src="https://img.shields.io/badge/built%20with-Python3-green.svg" alt="built with Python3" /></a>
 <a href="https://www.python.org/"><img src="https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue" alt="Runs on" /></a>
 <a href="https://github.com/novonordisk-research/ProcessOptimizer/blob/develop/LICENSE.md"><img src="https://img.shields.io/pypi/l/ProcessOptimizer" alt="PyPI - License" /></a>
 <a href="https://scikit-optimize.github.io/stable/"><img src="https://img.shields.io/badge/BuildOn-Scikit--Optimize-brightgreen" alt="Scikit-Optimize" /></a>
 <a href="https://doi.org/10.5281/zenodo.5155295"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.5155295.svg" alt="DOI"></a>
 
 [![Downloads](https://static.pepy.tech/personalized-badge/processoptimizer?period=total&units=international_system&left_color=brightgreen&right_color=orange&left_text=Downloads)](https://pepy.tech/project/processoptimizer)
@@ -138,7 +138,8 @@
 
 - In terminal run the command "pytest" and make sure there are no errors
 - Change version number in setup.py
 - Change version number in ProcessOptimizer/\_\_init\_\_.py
 - Remember to `pip install twine` if running in a new virtual env. (You might also have to `pip install wheel`)
 - Run `python setup.py sdist bdist_wheel`
 - Run `python -m twine upload dist/*` (make sure that /dist only contains relevant version)
+- (Remember that pypi has changed the way it handles credentials, you might have to state username: __token__ and then use your token value (incl pypi-prefix) as password. As stated here https://pypi.org/help/#apitoken
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ProcessOptimizer Version: 0.9.4 Summary: Sequential
+Metadata-Version: 2.1 Name: ProcessOptimizer Version: 0.9.5 Summary: Sequential
 model-based optimization toolbox (forked from scikit-optimize) Home-page:
 https://github.com/novonordisk-research/ProcessOptimizer Author: Novo Nordisk,
 Research & Early Development License: BSD Description-Content-Type: text/
 markdown Provides-Extra: browniebee License-File: LICENSE.md License-File:
 AUTHORS_scikit_optimize.md
         _____                              ____        _   _           _
 
@@ -134,8 +134,11 @@
 https://packaging.python.org/tutorials/packaging-projects/ To upload a new
 version to PyPi do the following in the root folder of the project: - In
 terminal run the command "pytest" and make sure there are no errors - Change
 version number in setup.py - Change version number in ProcessOptimizer/
 \_\_init\_\_.py - Remember to `pip install twine` if running in a new virtual
 env. (You might also have to `pip install wheel`) - Run `python setup.py sdist
 bdist_wheel` - Run `python -m twine upload dist/*` (make sure that /dist only
-contains relevant version)
+contains relevant version) - (Remember that pypi has changed the way it handles
+credentials, you might have to state username: __token__ and then use your
+token value (incl pypi-prefix) as password. As stated here https://pypi.org/
+help/#apitoken
```

### Comparing `ProcessOptimizer-0.9.4/ProcessOptimizer.egg-info/SOURCES.txt` & `ProcessOptimizer-0.9.5/ProcessOptimizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.9.4/README.md` & `ProcessOptimizer-0.9.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
  | |__) | __ ___   ___ ___  ___ ___| |  | |_ __ | |_ _ _ __ ___  _ _______ _ __ 
  |  ___/ '__/ _ \ / __/ _ \/ __/ __| |  | | '_ \| __| | '_ ` _ \| |_  / _ \ '__|
  | |   | | | (_) | (_|  __/\__ \__ \ |__| | |_) | |_| | | | | | | |/ /  __/ |   
  |_|   |_|  \___/ \___\___||___/___/\____/| .__/ \__|_|_| |_| |_|_/___\___|_|   
                                           | |                                   
                                           |_|                                   
 </pre>
-<a href="https://badge.fury.io/py/ProcessOptimizer"><img src="https://badge.fury.io/py/ProcessOptimizer.svg" alt="PyPI version" height="18"></a>
-<a href="https://github.com/novonordisk-research/ProcessOptimizer/actions"><img src="https://github.com/novonordisk-research/ProcessOptimizer/workflows/Python%20package/badge.svg" alt="Tests" height="18"></a>
+<a href="https://badge.fury.io/py/ProcessOptimizer"><img src="https://badge.fury.io/py/ProcessOptimizer.svg" alt="PyPI version"></a>
+<a href="https://github.com/novonordisk-research/ProcessOptimizer/actions"><img src="https://github.com/novonordisk-research/ProcessOptimizer/actions/workflows/python-package-tests.yml/badge.svg" alt="Tests"></a>
 <a href="https://www.python.org/"><img src="https://img.shields.io/badge/built%20with-Python3-green.svg" alt="built with Python3" /></a>
 <a href="https://www.python.org/"><img src="https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue" alt="Runs on" /></a>
 <a href="https://github.com/novonordisk-research/ProcessOptimizer/blob/develop/LICENSE.md"><img src="https://img.shields.io/pypi/l/ProcessOptimizer" alt="PyPI - License" /></a>
 <a href="https://scikit-optimize.github.io/stable/"><img src="https://img.shields.io/badge/BuildOn-Scikit--Optimize-brightgreen" alt="Scikit-Optimize" /></a>
 <a href="https://doi.org/10.5281/zenodo.5155295"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.5155295.svg" alt="DOI"></a>
 
 [![Downloads](https://static.pepy.tech/personalized-badge/processoptimizer?period=total&units=international_system&left_color=brightgreen&right_color=orange&left_text=Downloads)](https://pepy.tech/project/processoptimizer)
@@ -126,7 +126,8 @@
 
 - In terminal run the command "pytest" and make sure there are no errors
 - Change version number in setup.py
 - Change version number in ProcessOptimizer/\_\_init\_\_.py
 - Remember to `pip install twine` if running in a new virtual env. (You might also have to `pip install wheel`)
 - Run `python setup.py sdist bdist_wheel`
 - Run `python -m twine upload dist/*` (make sure that /dist only contains relevant version)
+- (Remember that pypi has changed the way it handles credentials, you might have to state username: __token__ and then use your token value (incl pypi-prefix) as password. As stated here https://pypi.org/help/#apitoken
```

#### html2text {}

```diff
@@ -128,8 +128,11 @@
 https://packaging.python.org/tutorials/packaging-projects/ To upload a new
 version to PyPi do the following in the root folder of the project: - In
 terminal run the command "pytest" and make sure there are no errors - Change
 version number in setup.py - Change version number in ProcessOptimizer/
 \_\_init\_\_.py - Remember to `pip install twine` if running in a new virtual
 env. (You might also have to `pip install wheel`) - Run `python setup.py sdist
 bdist_wheel` - Run `python -m twine upload dist/*` (make sure that /dist only
-contains relevant version)
+contains relevant version) - (Remember that pypi has changed the way it handles
+credentials, you might have to state username: __token__ and then use your
+token value (incl pypi-prefix) as password. As stated here https://pypi.org/
+help/#apitoken
```

### Comparing `ProcessOptimizer-0.9.4/setup.py` & `ProcessOptimizer-0.9.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="ProcessOptimizer",
-    version="0.9.4",
+    version="0.9.5",
     description="Sequential model-based optimization toolbox \
     (forked from scikit-optimize)",
     url="https://github.com/novonordisk-research/ProcessOptimizer",
     license="BSD",
     author="Novo Nordisk, Research & Early Development",
     packages=[
         "ProcessOptimizer",
@@ -24,33 +24,32 @@
         "ProcessOptimizer.model_systems.data",
         "ProcessOptimizer.optimizer",
         "ProcessOptimizer.space",
         "ProcessOptimizer.utils",
         "ProcessOptimizer.learning.gaussian_process",
     ],
     install_requires=[
-        "numpy>=1.0.0",
-        "matplotlib>=1.0.0",
-        "scipy>=1.0.0",
-        "bokeh>=1.0.0",
+        "numpy",
+        "matplotlib",
+        "scipy",
+        "bokeh",
         "scikit-learn>=0.24.2",
-        "six>=1.0.0",
-        "deap>=1.0.0",
-        "pyYAML>=1.0.0",
+        "six",
+        "deap",
+        "pyYAML",
     ],
     extras_require={
         "browniebee": [
-            "bokeh==3.1.1",
+            "bokeh==3.4.1",
             "deap==1.4.1",
-            "matplotlib==3.7.2",
-            "numpy==1.24.4",
+            "matplotlib==3.8.4",
+            "numpy==1.26.4",
             "pyYAML==6.0.1",
-            "scikit-learn==1.3.0",
-            "scipy==1.10.1",
+            "scikit-learn==1.4.2",
+            "scipy==1.13.0",
             "six==1.16.0",
-            "tornado==6.3.3",
         ]
     },
     long_description=long_description,
     long_description_content_type="text/markdown",
     include_package_data=True,
 )
```

