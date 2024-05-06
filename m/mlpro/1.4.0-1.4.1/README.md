# Comparing `tmp/mlpro-1.4.0.tar.gz` & `tmp/mlpro-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpro-1.4.0.tar", last modified: Wed Apr 17 10:37:58 2024, max compression
+gzip compressed data, was "mlpro-1.4.1.tar", last modified: Mon May  6 12:08:19 2024, max compression
```

## Comparing `mlpro-1.4.0.tar` & `mlpro-1.4.1.tar`

### file list

```diff
@@ -1,249 +1,261 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.051833 mlpro-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-17 10:37:47.000000 mlpro-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-17 10:37:47.000000 mlpro-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-04-17 10:37:58.051833 mlpro-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-17 10:37:47.000000 mlpro-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-17 10:37:49.000000 mlpro-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-17 10:37:58.051833 mlpro-1.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.011834 mlpro-1.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.019834 mlpro-1.4.0/src/mlpro/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.019834 mlpro-1.4.0/src/mlpro/bf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14747 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.019834 mlpro-1.4.0/src/mlpro/bf/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23793 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/datasets/basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.023834 mlpro-1.4.0/src/mlpro/bf/math/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23130 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/math/basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/math/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)    12542 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/math/normalizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.023834 mlpro-1.4.0/src/mlpro/bf/ml/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    55808 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/ml/basics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.023834 mlpro-1.4.0/src/mlpro/bf/ml/systems/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/ml/systems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23245 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/ml/systems/basics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.023834 mlpro-1.4.0/src/mlpro/bf/ml/systems/pool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/ml/systems/pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37878 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/mt.py
--rw-r--r--   0 runner    (1001) docker     (127)    14057 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.023834 mlpro-1.4.0/src/mlpro/bf/physics/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/physics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9959 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/physics/basics.py
--rw-r--r--   0 runner    (1001) docker     (127)    14329 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/physics/unitconverter.py
--rw-r--r--   0 runner    (1001) docker     (127)    32607 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.023834 mlpro-1.4.0/src/mlpro/bf/streams/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    64843 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.023834 mlpro-1.4.0/src/mlpro/bf/streams/samplers/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/samplers/min_wise.py
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/samplers/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/samplers/reservoir_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/samplers/weighted_random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.027834 mlpro-1.4.0/src/mlpro/bf/streams/streams/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16799 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/streams/clouds.py
--rw-r--r--   0 runner    (1001) docker     (127)    11195 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/streams/clouds_with_anomalies.py
--rw-r--r--   0 runner    (1001) docker     (127)     9453 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/streams/csv_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/streams/doublespiral2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/streams/point_outliers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5438 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/streams/provider_mlpro.py
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/streams/rnd10d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.027834 mlpro-1.4.0/src/mlpro/bf/streams/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8445 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/tasks/deriver.py
--rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/tasks/rearranger.py
--rw-r--r--   0 runner    (1001) docker     (127)    19030 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/tasks/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.027834 mlpro-1.4.0/src/mlpro/bf/streams/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/streams/workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.027834 mlpro-1.4.0/src/mlpro/bf/systems/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    83676 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/basics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.027834 mlpro-1.4.0/src/mlpro/bf/systems/pool/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34965 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/doublependulum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/flipflops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.027834 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.011834 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.011834 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.027834 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/
--rw-r--r--   0 runner    (1001) docker     (127)    37884 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Arrow.stl
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/X_letter.stl
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Y_letter.stl
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Z_letter.stl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.027834 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/texture/
--rw-r--r--   0 runner    (1001) docker     (127)   322794 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/texture/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.011834 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/ur5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.031834 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/
--rw-r--r--   0 runner    (1001) docker     (127)    28984 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/base.stl
--rw-r--r--   0 runner    (1001) docker     (127)    52584 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/forearm.stl
--rw-r--r--   0 runner    (1001) docker     (127)    33784 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/shoulder.stl
--rw-r--r--   0 runner    (1001) docker     (127)    58884 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/upperarm.stl
--rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist1.stl
--rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist2.stl
--rw-r--r--   0 runner    (1001) docker     (127)    22384 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist3.stl
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/boxontable.xml
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/cartpole.xml
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/doublependulum.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/mlpro.xml
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/pendulum.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/ur5.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.031834 mlpro-1.4.0/src/mlpro/bf/ui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.031834 mlpro-1.4.0/src/mlpro/bf/ui/sciui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/ui/sciui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33615 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/ui/sciui/framework.py
--rw-r--r--   0 runner    (1001) docker     (127)    10903 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/ui/sciui/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.031834 mlpro-1.4.0/src/mlpro/bf/ui/sciui/pool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/ui/sciui/pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24464 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/ui/sciui/pool/iis.py
--rw-r--r--   0 runner    (1001) docker     (127)    13746 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/ui/sciui/pool/iisbenchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.031834 mlpro-1.4.0/src/mlpro/bf/ui/sciui/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/ui/sciui/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/ui/sciui/templates/scenario_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    31658 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/bf/various.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.031834 mlpro-1.4.0/src/mlpro/gt/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.035834 mlpro-1.4.0/src/mlpro/gt/dynamicgames/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/dynamicgames/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7155 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/dynamicgames/basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/dynamicgames/potential.py
--rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/dynamicgames/stackelberg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.035834 mlpro-1.4.0/src/mlpro/gt/native/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/native/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    66293 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/native/basics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.035834 mlpro-1.4.0/src/mlpro/gt/pool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/pool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.035834 mlpro-1.4.0/src/mlpro/gt/pool/boards/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/pool/boards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/pool/boards/bglp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.035834 mlpro-1.4.0/src/mlpro/gt/pool/native/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/pool/native/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.035834 mlpro-1.4.0/src/mlpro/gt/pool/native/games/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/pool/native/games/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/pool/native/games/prisonersdilemma_2p.py
--rw-r--r--   0 runner    (1001) docker     (127)     7194 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/pool/native/games/prisonersdilemma_3p.py
--rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/pool/native/games/rockpaperscissors.py
--rw-r--r--   0 runner    (1001) docker     (127)    12928 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/pool/native/games/routingproblems_3p.py
--rw-r--r--   0 runner    (1001) docker     (127)    12811 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/pool/native/games/supplydemand_3p.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.035834 mlpro-1.4.0/src/mlpro/gt/pool/native/solvers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/pool/native/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/pool/native/solvers/greedypolicy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/pool/native/solvers/randomsolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.035834 mlpro-1.4.0/src/mlpro/gt/pool/policies/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/gt/pool/policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.035834 mlpro-1.4.0/src/mlpro/oa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.035834 mlpro-1.4.0/src/mlpro/oa/sciui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/sciui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31194 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/sciui/iis.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/sciui/runme.py
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/sciui/scenario_oa1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.035834 mlpro-1.4.0/src/mlpro/oa/streams/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13855 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/basics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.039834 mlpro-1.4.0/src/mlpro/oa/streams/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.039834 mlpro-1.4.0/src/mlpro/oa/streams/tasks/anomalydetectors/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/tasks/anomalydetectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.039834 mlpro-1.4.0/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7951 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/clusterbased.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/contextual.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/drift.py
--rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/tasks/anomalydetectors/basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/tasks/anomalydetectors/cb_detectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/tasks/anomalydetectors/paga_detectors.py
--rw-r--r--   0 runner    (1001) docker     (127)    11878 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/tasks/boundarydetectors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.039834 mlpro-1.4.0/src/mlpro/oa/streams/tasks/clusteranalyzers/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/tasks/clusteranalyzers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11422 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/tasks/clusteranalyzers/basics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.039834 mlpro-1.4.0/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/basics.py
--rw-r--r--   0 runner    (1001) docker     (127)    14437 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/centroid.py
--rw-r--r--   0 runner    (1001) docker     (127)    15142 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/tasks/normalizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.039834 mlpro-1.4.0/src/mlpro/oa/streams/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/streams/workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.039834 mlpro-1.4.0/src/mlpro/oa/systems/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/systems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40080 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/systems/basics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.039834 mlpro-1.4.0/src/mlpro/oa/systems/pool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/systems/pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/oa/systems/pool/doublependulum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.043834 mlpro-1.4.0/src/mlpro/rl/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    36302 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/models_agents.py
--rw-r--r--   0 runner    (1001) docker     (127)    21239 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/models_env.py
--rw-r--r--   0 runner    (1001) docker     (127)    18009 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/models_env_ada.py
--rw-r--r--   0 runner    (1001) docker     (127)    15513 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/models_env_oa.py
--rw-r--r--   0 runner    (1001) docker     (127)    48989 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/models_train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.043834 mlpro-1.4.0/src/mlpro/rl/pool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/pool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.043834 mlpro-1.4.0/src/mlpro/rl/pool/actionplanner/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/pool/actionplanner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9891 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/pool/actionplanner/mpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.043834 mlpro-1.4.0/src/mlpro/rl/pool/envs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/pool/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50258 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/pool/envs/bglp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/pool/envs/cartpole.py
--rw-r--r--   0 runner    (1001) docker     (127)    44837 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/pool/envs/doublependulum.py
--rw-r--r--   0 runner    (1001) docker     (127)    10568 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/pool/envs/gridworld.py
--rw-r--r--   0 runner    (1001) docker     (127)    19097 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/pool/envs/robotinhtm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.043834 mlpro-1.4.0/src/mlpro/rl/pool/policies/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/pool/policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/pool/policies/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/pool/policies/randomgenerator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.043834 mlpro-1.4.0/src/mlpro/rl/pool/sarsbuffer/
--rw-r--r--   0 runner    (1001) docker     (127)    11708 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/pool/sarsbuffer/PrioritizedBuffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/pool/sarsbuffer/RandomSARSBuffer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/pool/sarsbuffer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.043834 mlpro-1.4.0/src/mlpro/rl/pool/scenarios/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/pool/scenarios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    65877 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/rl/sciui_rl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.047834 mlpro-1.4.0/src/mlpro/sl/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13143 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/sl/basics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.047834 mlpro-1.4.0/src/mlpro/sl/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/sl/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/sl/examples/howto_sl_afct_100_train_and_reload_pytorch_mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/sl/fnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    14693 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/sl/models_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)    40710 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/sl/models_train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.047834 mlpro-1.4.0/src/mlpro/sl/pool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/sl/pool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.047834 mlpro-1.4.0/src/mlpro/sl/pool/afct/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/sl/pool/afct/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.047834 mlpro-1.4.0/src/mlpro/sl/pool/afct/fnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/sl/pool/afct/fnn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.047834 mlpro-1.4.0/src/mlpro/sl/pool/afct/fnn/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/sl/pool/afct/fnn/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22451 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/sl/pool/afct/fnn/pytorch/mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)    12154 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/sl/pool/afct/pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.047834 mlpro-1.4.0/src/mlpro/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/wrappers/basics.py
--rw-r--r--   0 runner    (1001) docker     (127)    38971 2024-04-17 10:37:49.000000 mlpro-1.4.0/src/mlpro/wrappers/mujoco.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.047834 mlpro-1.4.0/src/mlpro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-04-17 10:37:57.000000 mlpro-1.4.0/src/mlpro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-17 10:37:58.000000 mlpro-1.4.0/src/mlpro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 10:37:57.000000 mlpro-1.4.0/src/mlpro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-17 10:37:57.000000 mlpro-1.4.0/src/mlpro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-17 10:37:57.000000 mlpro-1.4.0/src/mlpro.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:37:58.047834 mlpro-1.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-17 10:37:49.000000 mlpro-1.4.0/test/test_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-17 10:37:49.000000 mlpro-1.4.0/test/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-04-17 10:37:49.000000 mlpro-1.4.0/test/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-17 10:37:49.000000 mlpro-1.4.0/test/test_math.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-17 10:37:49.000000 mlpro-1.4.0/test/test_pool_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-17 10:37:49.000000 mlpro-1.4.0/test/test_various.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.463511 mlpro-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-06 12:08:14.000000 mlpro-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-06 12:08:14.000000 mlpro-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-05-06 12:08:19.463511 mlpro-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-05-06 12:08:14.000000 mlpro-1.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-06 12:08:15.000000 mlpro-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-06 12:08:19.463511 mlpro-1.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.415511 mlpro-1.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.427511 mlpro-1.4.1/src/mlpro/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.427511 mlpro-1.4.1/src/mlpro/bf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.427511 mlpro-1.4.1/src/mlpro/bf/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/data/buffers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/data/datastoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.431511 mlpro-1.4.1/src/mlpro/bf/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26468 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/datasets/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.431511 mlpro-1.4.1/src/mlpro/bf/math/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23130 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/math/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/math/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.431511 mlpro-1.4.1/src/mlpro/bf/math/normalizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/math/normalizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/math/normalizers/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/math/normalizers/minmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/math/normalizers/ztrans.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10835 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/math/properties.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.431511 mlpro-1.4.1/src/mlpro/bf/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55808 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/ml/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.431511 mlpro-1.4.1/src/mlpro/bf/ml/systems/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/ml/systems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23245 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/ml/systems/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.431511 mlpro-1.4.1/src/mlpro/bf/ml/systems/pool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/ml/systems/pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37878 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/mt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14057 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.431511 mlpro-1.4.1/src/mlpro/bf/physics/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/physics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9959 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/physics/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14329 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/physics/unitconverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32607 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.431511 mlpro-1.4.1/src/mlpro/bf/streams/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64843 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/streams/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.435511 mlpro-1.4.1/src/mlpro/bf/streams/samplers/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/streams/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/streams/samplers/min_wise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/streams/samplers/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/streams/samplers/reservoir_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/streams/samplers/weighted_random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.435511 mlpro-1.4.1/src/mlpro/bf/streams/streams/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/streams/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16799 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/streams/streams/clouds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11195 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/streams/streams/clouds_with_anomalies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9453 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/streams/streams/csv_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/streams/streams/doublespiral2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/streams/streams/point_outliers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5438 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/streams/streams/provider_mlpro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/streams/streams/rnd10d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.435511 mlpro-1.4.1/src/mlpro/bf/streams/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/streams/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8445 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/streams/tasks/deriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/streams/tasks/rearranger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19030 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/streams/tasks/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.435511 mlpro-1.4.1/src/mlpro/bf/streams/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/streams/workflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.435511 mlpro-1.4.1/src/mlpro/bf/systems/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/systems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83676 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/systems/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.435511 mlpro-1.4.1/src/mlpro/bf/systems/pool/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/systems/pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34965 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/systems/pool/doublependulum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/systems/pool/flipflops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.439511 mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.419511 mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.419511 mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.439511 mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/
+-rw-r--r--   0 runner    (1001) docker     (127)    37884 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Arrow.stl
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/X_letter.stl
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Y_letter.stl
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Z_letter.stl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.439511 mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/texture/
+-rw-r--r--   0 runner    (1001) docker     (127)   322794 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/texture/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.419511 mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/assets/ur5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.443511 mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/
+-rw-r--r--   0 runner    (1001) docker     (127)    28984 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/base.stl
+-rw-r--r--   0 runner    (1001) docker     (127)    52584 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/forearm.stl
+-rw-r--r--   0 runner    (1001) docker     (127)    33784 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/shoulder.stl
+-rw-r--r--   0 runner    (1001) docker     (127)    58884 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/upperarm.stl
+-rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist1.stl
+-rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist2.stl
+-rw-r--r--   0 runner    (1001) docker     (127)    22384 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist3.stl
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/boxontable.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/cartpole.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/doublependulum.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/mlpro.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/pendulum.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/ur5.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.443511 mlpro-1.4.1/src/mlpro/bf/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.443511 mlpro-1.4.1/src/mlpro/bf/ui/sciui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/ui/sciui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33615 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/ui/sciui/framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10903 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/ui/sciui/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.443511 mlpro-1.4.1/src/mlpro/bf/ui/sciui/pool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/ui/sciui/pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24464 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/ui/sciui/pool/iis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13746 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/ui/sciui/pool/iisbenchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.443511 mlpro-1.4.1/src/mlpro/bf/ui/sciui/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/ui/sciui/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/ui/sciui/templates/scenario_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31658 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/bf/various.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.443511 mlpro-1.4.1/src/mlpro/gt/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/gt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.443511 mlpro-1.4.1/src/mlpro/gt/dynamicgames/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/gt/dynamicgames/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7155 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/gt/dynamicgames/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/gt/dynamicgames/potential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/gt/dynamicgames/stackelberg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.443511 mlpro-1.4.1/src/mlpro/gt/native/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/gt/native/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66293 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/gt/native/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.443511 mlpro-1.4.1/src/mlpro/gt/pool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/gt/pool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.447511 mlpro-1.4.1/src/mlpro/gt/pool/boards/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/gt/pool/boards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/gt/pool/boards/bglp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.447511 mlpro-1.4.1/src/mlpro/gt/pool/native/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/gt/pool/native/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.447511 mlpro-1.4.1/src/mlpro/gt/pool/native/games/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/gt/pool/native/games/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/gt/pool/native/games/prisonersdilemma_2p.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7194 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/gt/pool/native/games/prisonersdilemma_3p.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/gt/pool/native/games/rockpaperscissors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12928 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/gt/pool/native/games/routingproblems_3p.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12811 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/gt/pool/native/games/supplydemand_3p.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.447511 mlpro-1.4.1/src/mlpro/gt/pool/native/solvers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/gt/pool/native/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/gt/pool/native/solvers/greedypolicy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/gt/pool/native/solvers/randomsolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.447511 mlpro-1.4.1/src/mlpro/gt/pool/policies/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/gt/pool/policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.447511 mlpro-1.4.1/src/mlpro/oa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/oa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.447511 mlpro-1.4.1/src/mlpro/oa/sciui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/oa/sciui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31194 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/oa/sciui/iis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/oa/sciui/runme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/oa/sciui/scenario_oa1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.447511 mlpro-1.4.1/src/mlpro/oa/streams/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/oa/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13855 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/oa/streams/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.447511 mlpro-1.4.1/src/mlpro/oa/streams/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/oa/streams/tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.451511 mlpro-1.4.1/src/mlpro/oa/streams/tasks/anomalydetectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/oa/streams/tasks/anomalydetectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.451511 mlpro-1.4.1/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7951 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/clusterbased.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/contextual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/drift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/oa/streams/tasks/anomalydetectors/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/oa/streams/tasks/anomalydetectors/cb_detectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/oa/streams/tasks/anomalydetectors/paga_detectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11878 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/oa/streams/tasks/boundarydetectors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.451511 mlpro-1.4.1/src/mlpro/oa/streams/tasks/clusteranalyzers/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/oa/streams/tasks/clusteranalyzers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13757 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/oa/streams/tasks/clusteranalyzers/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.451511 mlpro-1.4.1/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/centroid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.451511 mlpro-1.4.1/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/properties/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/properties/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10890 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/properties/centroid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15142 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/oa/streams/tasks/normalizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.451511 mlpro-1.4.1/src/mlpro/oa/streams/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/oa/streams/workflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.451511 mlpro-1.4.1/src/mlpro/oa/systems/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/oa/systems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40080 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/oa/systems/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.455511 mlpro-1.4.1/src/mlpro/oa/systems/pool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/oa/systems/pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/oa/systems/pool/doublependulum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.455511 mlpro-1.4.1/src/mlpro/rl/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/rl/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36302 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/rl/models_agents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21239 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/rl/models_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18009 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/rl/models_env_ada.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15513 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/rl/models_env_oa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48989 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/rl/models_train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.455511 mlpro-1.4.1/src/mlpro/rl/pool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/rl/pool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.455511 mlpro-1.4.1/src/mlpro/rl/pool/actionplanner/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/rl/pool/actionplanner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9891 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/rl/pool/actionplanner/mpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.455511 mlpro-1.4.1/src/mlpro/rl/pool/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/rl/pool/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50258 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/rl/pool/envs/bglp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/rl/pool/envs/cartpole.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44837 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/rl/pool/envs/doublependulum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10568 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/rl/pool/envs/gridworld.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19097 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/rl/pool/envs/robotinhtm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.455511 mlpro-1.4.1/src/mlpro/rl/pool/policies/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/rl/pool/policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/rl/pool/policies/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/rl/pool/policies/randomgenerator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.459511 mlpro-1.4.1/src/mlpro/rl/pool/sarsbuffer/
+-rw-r--r--   0 runner    (1001) docker     (127)    11708 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/rl/pool/sarsbuffer/PrioritizedBuffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/rl/pool/sarsbuffer/RandomSARSBuffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/rl/pool/sarsbuffer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.459511 mlpro-1.4.1/src/mlpro/rl/pool/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/rl/pool/scenarios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65877 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/rl/sciui_rl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.459511 mlpro-1.4.1/src/mlpro/sl/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13144 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/sl/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.459511 mlpro-1.4.1/src/mlpro/sl/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/sl/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/sl/examples/howto_sl_afct_100_train_and_reload_pytorch_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/sl/fnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14693 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/sl/models_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40710 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/sl/models_train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.459511 mlpro-1.4.1/src/mlpro/sl/pool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/sl/pool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.459511 mlpro-1.4.1/src/mlpro/sl/pool/afct/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/sl/pool/afct/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.459511 mlpro-1.4.1/src/mlpro/sl/pool/afct/fnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/sl/pool/afct/fnn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.459511 mlpro-1.4.1/src/mlpro/sl/pool/afct/fnn/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/sl/pool/afct/fnn/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22451 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/sl/pool/afct/fnn/pytorch/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12154 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/sl/pool/afct/pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.459511 mlpro-1.4.1/src/mlpro/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/wrappers/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38971 2024-05-06 12:08:15.000000 mlpro-1.4.1/src/mlpro/wrappers/mujoco.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.463511 mlpro-1.4.1/src/mlpro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-05-06 12:08:19.000000 mlpro-1.4.1/src/mlpro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7670 2024-05-06 12:08:19.000000 mlpro-1.4.1/src/mlpro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 12:08:19.000000 mlpro-1.4.1/src/mlpro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-06 12:08:19.000000 mlpro-1.4.1/src/mlpro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-06 12:08:19.000000 mlpro-1.4.1/src/mlpro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:08:19.463511 mlpro-1.4.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-06 12:08:15.000000 mlpro-1.4.1/test/test_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-05-06 12:08:15.000000 mlpro-1.4.1/test/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-05-06 12:08:15.000000 mlpro-1.4.1/test/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-06 12:08:15.000000 mlpro-1.4.1/test/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-06 12:08:15.000000 mlpro-1.4.1/test/test_pool_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-05-06 12:08:15.000000 mlpro-1.4.1/test/test_various.py
```

### Comparing `mlpro-1.4.0/LICENSE` & `mlpro-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/PKG-INFO` & `mlpro-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpro
-Version: 1.4.0
+Version: 1.4.1
 Summary: MLPro - The Integrative Middleware Framework for Standardized Machine Learning
 Home-page: https://mlpro.readthedocs.io
 Author: MLPro Team
 Author-email: mlpro@listen.fh-swf.de
 Project-URL: Bug Tracker, https://mlpro.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mlpro-1.4.0/README.md` & `mlpro-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/setup.cfg` & `mlpro-1.4.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mlpro
-version = 1.4.0
+version = 1.4.1
 author = MLPro Team
 author_email = mlpro@listen.fh-swf.de
 description = MLPro - The Integrative Middleware Framework for Standardized Machine Learning
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://mlpro.readthedocs.io
 project_urls =
```

### Comparing `mlpro-1.4.0/src/mlpro/bf/data.py` & `mlpro-1.4.1/src/mlpro/oa/streams/tasks/normalizers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,428 +1,404 @@
 ## -------------------------------------------------------------------------------------------------
 ## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
-## -- Package : mlpro.bf
-## -- Module  : data
+## -- Package : mlpro.oa.tasks.normalizers
+## -- Module  : normalizers.py
 ## -------------------------------------------------------------------------------------------------
 ## -- History :
 ## -- yyyy-mm-dd  Ver.      Auth.    Description
-## -- 2021-04-16  0.0.0     DA       Creation
-## -- 2021-05-29  1.0.0     DA       Release of first version
-## -- 2021-06-16  1.1.0     SY       Adding the first version of data storing,
-## --                                data plotting, and data saving classes
-## -- 2021-06-21  1.2.0     SY       Add extensions in classes Loadable,
-## --                                Saveable, DataPlotting & DataStoring.
-## -- 2021-08-28  1.2.1     DA       Added constant C_VAR0 to class DataStoring
-## -- 2021-09-18  1.2.1     MRD      Buffer Class Implementation. Add new parameter buffer
-## --                                to the Adaptive Class
-## -- 2021-09-19  1.2.2     MRD      Improvement on Buffer Class. Implement new base class
-## --                                Buffer Element and BufferRnd
-## -- 2021-09-22  1.3.0     MRD      New classes BufferElement, Buffer, BufferRnd
-## -- 2021-09-25  1.3.1     MRD      Add __len__ functionality for SARBuffer
-## -- 2023-02-09  1.3.2     MRD      Beautify
-## -- 2023-03-02  1.3.3     SY       Update load_data in DataStoring
+## -- 2022-12-07  1.0.0     LSB      Creation/Release
+## -- 2022-12-13  1.0.1     LSB      Refactoring
+## -- 2022-12-20  1.0.2     DA       Refactoring
+## -- 2022-12-20  1.0.3     LSB      Bugfix
+## -- 2022-12-30  1.0.4     LSB      Bugfix
+## -- 2023-01-12  1.1.0     LSB      Renormalizing plot data
+## -- 2023-01-24  1.1.1     LSB      Bugfix
+## -- 2023-02-13  1.1.2     LSB      Bugfix: Setting the default parameter update flag ot false
+## -- 2023-04-09  1.2.0     DA       Class NormalizerZTransform: new methods _adapt(), _adapt_reverse()
+## -- 2023-05-03  1.2.1     DA       Bugfix in NormalizerMinMax._update_plot_2d/3d/nd
+## -- 2023-05-22  1.2.2     SY       Refactoring
 ## -------------------------------------------------------------------------------------------------
 
 """
-Ver. 1.3.3 (2023-03-02)
+Ver. 1.2.2 (2023-05-22)
 
-This module provides various elementary data management classes.
+This module provides implementation for adaptive normalizers for MinMax Normalization and ZTransformation
 """
 
 
-from datetime import datetime, timedelta
-import numpy as np
-import math
-import matplotlib.pyplot as plt
-import pickle as pkl
-import os
-import csv
-import copy
-from mlpro.bf.various import Persistent
-import random
-
+from mlpro.oa.streams.basics import *
+from mlpro.bf.math import normalizers as Norm
 
 
 
 ## -------------------------------------------------------------------------------------------------
 ## -------------------------------------------------------------------------------------------------
-class DataStoring: #(Persistent):
-    """
-    This class provides a functionality to store values of variables during
-    training/simulation.
+class NormalizerMinMax (OATask, Norm.NormalizerMinMax):
     """
+    Class with functionality for adaptive normalization of instances using MinMax Normalization.
 
-    C_VAR0 = 'Frame ID'
+    Parameters
+    ----------
+    p_name: str, optional
+        Name of the task.
+    p_range_max:
+        Processing range of the task, default is a Thread.
+    p_ada:
+        True if the task has adaptivity, default is true.
+    p_duplicate_data : bool
+        If True, instances will be duplicated before processing. Default = False.
+    p_visualize:
+        True for visualization, false by default.
+    p_logging:
+        Logging level of the task. Default is Log.C_LOG_ALL
+    p_kwargs:
+        Additional task parameters
+    """
 
+    C_NAME = 'Normalizer MinMax' 
 
 ## -------------------------------------------------------------------------------------------------
-    def __init__(self, p_variables):
-        """
-        Parameters:
-            p_variable    List of variable names
-        """
-        
-        self.memory_dict = {}
-        self.names = p_variables
-        self.frame_id = {}
-        for name in self.names:
-            self.memory_dict[name] = {}
-            self.frame_id[name] = []
+    def __init__(self,p_name: str = None,
+                  p_range_max = StreamTask.C_RANGE_THREAD,
+                  p_ada : bool = True,
+                  p_duplicate_data : bool = False,
+                  p_visualize:bool = False,
+                  p_logging = Log.C_LOG_ALL,
+                  **p_kwargs):
 
+        OATask.__init__(self,
+                        p_name = p_name,
+                        p_range_max = p_range_max,
+                        p_ada = p_ada,
+                        p_duplicate_data = p_duplicate_data,
+                        p_visualize = p_visualize,
+                        p_logging=p_logging,
+                        **p_kwargs )
 
-## -------------------------------------------------------------------------------------------------
-    def add_frame(self, p_frame_id):
-        """
-        To store unique sections in a variable (e.g episodes in RL, etc.)
-        """
-        
-        for name in self.names:
-            self.memory_dict[name][p_frame_id] = []
-            self.frame_id[name].append(p_frame_id)
 
+        Norm.NormalizerMinMax.__init__(self)
+        self._parameters_updated:bool = None
 
-## -------------------------------------------------------------------------------------------------
-    def memorize(self, p_variable, p_frame_id, p_value):
-        """
-        To store a particular variable into a memory
-        """
-        
-        self.memory_dict[p_variable][p_frame_id].append(p_value)
+        if p_visualize:
+            self._plot_data_2d = None
+            self._plot_data_3d = None
+            self._plot_data_nd = None
 
 
 ## -------------------------------------------------------------------------------------------------
-    def get_values(self, p_variable, p_frame_id=None):
+    def _run(self, p_inst_new:list, p_inst_del:list):
         """
-        To obtain value from the memory
+        Custom method to for run MinMax Normalizer task for normalizing new instances and denormalizing deleted
+        instances.
+
+        Parameters
+        ----------
+        p_inst_new: list
+            List of new instances in the workflow
+        p_inst_del: list
+            List of deleted instances in the workflow
         """
-        
-        if p_frame_id == None:
-            return self.memory_dict[p_variable]
-        else:
-            return self.memory_dict[p_variable][p_frame_id]
 
+        if ((p_inst_new is None) or (len(p_inst_new) == 0)
+                and ((p_inst_del is None) or len(p_inst_del) ==0)) : return
 
-## -------------------------------------------------------------------------------------------------
-    def list_to_chunks(self, p_data, p_chunksize):
-        NumChunks = int(math.ceil(len(p_data) / (p_chunksize * 1.0)))
-        retval = []
-        for chunk in range(NumChunks):
-            retval.append(sum(p_data[chunk * p_chunksize: (chunk + 1) * p_chunksize]) / (1.0 * p_chunksize))
-        return retval
+        for i,inst in enumerate(p_inst_new):
+            if self._param is None:
+                self.update_parameters(inst.get_feature_data().get_related_set())
+            normalized_element = self.normalize(inst.get_feature_data())
+            inst.get_feature_data().set_values(normalized_element.get_values())
 
-
-## -------------------------------------------------------------------------------------------------
-    def compress(self, p_chunksize):
-        for name in self.names:
-            for ep in len(self.memory_dict[name]):
-                self.memory_dict[name][ep] = self.list_to_chunks(self.memory_dict[name][ep], p_chunksize)
+        for j, del_inst in enumerate(p_inst_del):
+            if self._param is None:
+                self.update_parameters(del_inst.get_feature_data().get_related_set())
+            normalized_element = self.normalize(del_inst.get_feature_data())
+            del_inst.get_feature_data().set_values(normalized_element.get_values())
 
 
 ## -------------------------------------------------------------------------------------------------
-    def save_data(self, p_path, p_filename=None, p_delimiter="\t") -> bool:
+    def _adapt_on_event(self, p_event_id:str, p_event_object:Event) -> bool:
         """
-        To save stored data in memory_dict as a readable file format
+        Custom method to adapt the MinMax normalizer parameters based on event raised by Boundary object for changed
+        boundaries.
+
+        Parameters
+        ----------
+        p_event_id: str
+            Event id of the raised event
+
+        p_event_obj: Event
+            Event object that raises the corresponding event
+
+        Returns
+        -------
+        adapted: bool
+            Returns True, if the task has adapted. False otherwise.
         """
 
-        if (p_filename is not None) and (p_filename != ''):
-            self.filename = p_filename
-        else:
-            self.filename = self._generate_filename()
+        set = p_event_object.get_raising_object().get_related_set()
 
-        if self.filename is None:
-            return False
+        self.update_parameters(set)
 
-        try:
-            if not os.path.exists(p_path):
-                os.makedirs(p_path)
-            path_save = p_path + os.sep + self.filename + ".csv"
-            with open(path_save, "w", newline="") as write_file:
-                header = copy.deepcopy(self.names)
-                header.insert(0, self.C_VAR0)
-                writer = csv.writer(write_file, delimiter=p_delimiter, quoting=csv.QUOTE_ALL)
-                writer.writerow(header)
-                writer = csv.writer(write_file, delimiter=p_delimiter)
-                for frame in self.frame_id[self.names[0]]:
-                    for idx in range(len(self.memory_dict[self.names[0]][frame])):
-                        row = []
-                        row.append(frame)
-                        for name in self.names:
-                            row.append(self.memory_dict[name][frame][idx])
-                        writer.writerow(row)
-            return True
-        except:
-            return False
+        self._parameters_updated = True
+
+        return True
 
 
 ## -------------------------------------------------------------------------------------------------
-    def load_data(self,
-                  p_path,
-                  p_filename,
-                  p_delimiter="\t",
-                  p_frame=True,
-                  p_header=True) -> bool:
-        """
-        To load data from a readable file format and store them into the DataStoring class format
+    def _update_plot_2d( self,
+                         p_settings : PlotSettings,
+                         p_inst_new : list,
+                         p_inst_del : list,
+                         **p_kwargs ):
         """
 
-        try:
-            path_load = p_path + os.sep + p_filename
-            with open(path_load, "r") as read_file:
-                reader       = csv.reader(read_file, delimiter=p_delimiter)
-                names        = False
-                str_memorize = False
-                for row in reader:
-                    if names is False:
-                        if p_header:
-                            if p_frame:
-                                del row[0:1]
-                            self.__init__(row)
-                        else:
-                            if p_frame:
-                                del row[0:1]
-                            row_title = []
-                            for i in range(len(row)):
-                                row_title.append('Data_%i'%(i+1))
-                            self.__init__(row_title)
-                            str_memorize = True
-                        names = True
-                    else:
-                        str_memorize = True
-                        
-                    if str_memorize:
-                        if p_frame:
-                            column = 1
-                            for name in self.names:
-                                if row[0] not in self.frame_id[name]:
-                                    self.add_frame(row[0])
-                                try:
-                                    self.memorize(name, row[0], float(row[column]))
-                                except:
-                                    self.memorize(name, row[0],(row[column]))
-                                column += 1
-                        else:
-                            column = 0
-                            for name in self.names:
-                                if 'Frame_0' not in self.frame_id[name]:
-                                    self.add_frame('Frame_0')
-                                try:
-                                    self.memorize(name, 'Frame_0', float(row[column]))
-                                except:
-                                    self.memorize(name, 'Frame_0',(row[column]))
-                                column += 1
-            return True
-        except:
-            return False
+        Method to update the 2d plot for Normalizer. Extended to renormalize the obsolete data on change of parameters.
 
+        Parameters
+        ----------
+        p_settings : PlotSettings
+            Object with further plot settings.
+        p_inst_new : list
+            List of new stream instances to be plotted.
+        p_inst_del : list
+            List of obsolete stream instances to be removed.
+        p_kwargs : dict
+            Further optional plot parameters.
+        """
 
+        if self._parameters_updated and ( len(self._plot_2d_xdata) != 0 ):
 
+            if ( self._plot_data_2d is None ) or ( len(self._plot_2d_xdata) > self._plot_data_2d.shape[0] ):
+                self._plot_data_2d = np.zeros((len(self._plot_2d_xdata),2))
 
+            for i in range(len(self._plot_2d_xdata)):
+                self._plot_data_2d[i][0] = self._plot_2d_xdata[i]
+                self._plot_data_2d[i][1] = self._plot_2d_ydata[i]
 
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class BufferElement:
-    """
-    Base class implementation for buffer element
-    """
+            plot_data_renormalized = self.renormalize(self._plot_data_2d)
 
+            self._plot_2d_xdata = list(j[0] for j in plot_data_renormalized)
+            self._plot_2d_ydata = list(j[1] for j in plot_data_renormalized)
 
-## -------------------------------------------------------------------------------------------------
-    def __init__(self, p_element: dict) -> None:
-        """
-        Parameters:
-            p_element (dict): Buffer element in dictionary
-        """
+            self._parameters_updated = False
 
-        self._element = {}
-        self.add_value_element(p_element)
+        OATask._update_plot_2d(self, p_settings = p_settings,
+                               p_inst_new = p_inst_new,
+                               p_inst_del = p_inst_del,
+                               **p_kwargs)
 
 
 ## -------------------------------------------------------------------------------------------------
-    def add_value_element(self, p_val: dict):
-        """
-        Adding new value to the element container
-
-        Parameters:
-            p_val (dict): Elements in dictionary
+    def _update_plot_3d( self,
+                         p_settings : PlotSettings,
+                         p_inst_new : list,
+                         p_inst_del : list,
+                         **p_kwargs ):
         """
-        
-        self._element = {**self._element, **p_val}
+        Method to update the 3d plot for Normalizer. Extended to renormalize the obsolete data on change of parameters.
 
+        Parameters
+        ----------
+        p_settings : PlotSettings
+            Object with further plot settings.
+        p_inst_new : list
+            List of new stream instances to be plotted.
+        p_inst_del : list
+            List of obsolete stream instances to be removed.
+        p_kwargs : dict
+            Further optional plot parameters.
 
-## -------------------------------------------------------------------------------------------------
-    def get_data(self):
         """
-        Get the buffer element.
 
-        Returns:
-            Returns the buffer element.
-        """
+        if self._parameters_updated and ( len(self._plot_3d_xdata) != 0 ):
 
-        return self._element
+            if ( self._plot_data_3d is None ) or ( len(self._plot_3d_xdata) > self._plot_data_3d.shape[0] ):
+                self._plot_data_3d = np.zeros((len(self._plot_3d_xdata),3))
 
+            for i in range(len(self._plot_3d_xdata)):
+                self._plot_data_3d[i][0] = self._plot_3d_xdata[i]
+                self._plot_data_3d[i][1] = self._plot_3d_ydata[i]
+                self._plot_data_3d[i][2] = self._plot_3d_zdata[i]
 
 
+            plot_data_renormalized = self.renormalize(self._plot_data_3d)
 
+            self._plot_3d_xdata = list(j[0] for j in plot_data_renormalized)
+            self._plot_3d_ydata = list(j[1] for j in plot_data_renormalized)
+            self._plot_3d_zdata = list(j[2] for j in plot_data_renormalized)
 
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class Buffer:
-    """
-    Base class implementation for buffer management.
-    """
+            self._parameters_updated = False
+
+        OATask._update_plot_3d(self, p_settings = p_settings,
+                               p_inst_new = p_inst_new,
+                               p_inst_del = p_inst_del,
+                               **p_kwargs)
 
 
 ## -------------------------------------------------------------------------------------------------
-    def __init__(self, p_size=1):
-        """
-        Parameters:
-            p_size (int, optional): Buffer size. Defaults to 1.
+    def _update_plot_nd( self,
+                         p_settings : PlotSettings,
+                         p_inst_new : list,
+                         p_inst_del : list,
+                         **p_kwargs ):
         """
-        
-        self._size = p_size
-        self._data_buffer = {}
 
+        Method to update the nd plot for Normalizer. Extended to renormalize the obsolete data on change of parameters.
 
-## -------------------------------------------------------------------------------------------------
-    def add_element(self, p_elem: BufferElement):
+        Parameters
+        ----------
+        p_settings : PlotSettings
+            Object with further plot settings.
+        p_inst_new : list
+            List of new stream instances to be plotted.
+        p_inst_del : list
+            List of obsolete stream instances to be removed.
+        p_kwargs : dict
+            Further optional plot parameters.
         """
-        Add element to the buffer.
 
-        Parameters:
-            p_elem (BufferElement): Element of Buffer
-        """
-        
-        self._data_buffer = {**p_elem.get_data(), **self._data_buffer}
-        for key, value in self._data_buffer.items():
-            if key in p_elem.get_data() and key in self._data_buffer:
-                if not isinstance(self._data_buffer[key], list):
-                    self._data_buffer[key] = [p_elem.get_data()[key]]
-                else:
-                    self._data_buffer[key].append(p_elem.get_data()[key])
+        if self._parameters_updated and self._plot_nd_plots:
+            if (len(self._plot_nd_plots[0][0])) != 0:
 
-                if len(self._data_buffer[key]) > self._size:
-                    self._data_buffer[key].pop(-len(self._data_buffer[key]))
+                if ( self._plot_data_nd is None ) or ( len(self._plot_nd_plots[0][0]) > self._plot_data_nd.shape[0] ):
+                    self._plot_data_nd = np.zeros((len(self._plot_nd_plots[0][0]),len(self._plot_nd_plots)))
 
+                for j in range(len(self._plot_nd_plots)):
+                    for i in range(len(self._plot_nd_plots[0][0])):
+                        self._plot_data_nd[i][j] = self._plot_nd_plots[j][0][i]
 
- ## -------------------------------------------------------------------------------------------------
-    def clear(self):
-        """
-        Resets buffer.
-        """
-
-        self._data_buffer.clear()
+                plot_data_renormalized = self.renormalize(self._plot_data_nd)
 
+                for j in range(len(self._plot_nd_plots)):
+                    self._plot_nd_plots[j][0] = list(k[j] for k in plot_data_renormalized)
 
-## -------------------------------------------------------------------------------------------------
-    def get_latest(self):
-        """
-        Returns latest buffered element. 
-        """
 
-        try:
-            return {key: self._data_buffer[key][-1] for key in self._data_buffer}
-        except:
-            return None
+                self._parameters_updated = False
 
+        OATask._update_plot_nd( self, 
+                                p_settings = p_settings,
+                                p_inst_new = p_inst_new,
+                                p_inst_del = p_inst_del,
+                                **p_kwargs )
 
-## -------------------------------------------------------------------------------------------------
-    def get_all(self):
-        """
-        Return all buffered elements.
-        """
-        
-        return self._data_buffer
 
 
-## -------------------------------------------------------------------------------------------------
-    def get_sample(self, p_num: int):
-        """
-        Sample some element from the buffer.
 
-        Parameters:
-            p_num (int): Number of sample
 
-        Returns:
-            Samples in dictionary
-        """
-        
-        return self._extract_rows(self._gen_sample_ind(p_num))
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class NormalizerZTransform (OATask, Norm.NormalizerZTrans):
+    """
+    Class with functionality of adaptive normalization of instances with Z-Transformation
 
+    Parameters
+    ----------
+    p_name: str, optional
+        Name of the task.
+    p_range_max:
+        Processing range of the task, default is a Thread.
+    p_ada:
+        True if the task has adaptivity, default is true.
+    p_duplicate_data : bool
+        If True, instances will be duplicated before processing. Default = False.
+    p_visualize:
+        True for visualization, false by default.
+    p_logging:
+        Logging level of the task. Default is Log.C_LOG_ALL
+    p_kwargs:
+        Additional task parameters
+    """
+    C_NAME = 'Normalizer Z Transform'
 
 ## -------------------------------------------------------------------------------------------------
-    def _gen_sample_ind(self, p_num: int) -> list:
-        """
-        Generate random indices from the buffer.
+    def __init__(self, p_name: str = None,
+                 p_range_max=StreamTask.C_RANGE_THREAD,
+                 p_ada: bool = True,
+                 p_duplicate_data : bool = False,
+                 p_visualize = False,
+                 p_logging=Log.C_LOG_ALL,
+                 **p_kwargs):
 
-        Parameters:
-            p_num (int): Number of sample
+        OATask.__init__(self,
+            p_name=p_name,
+            p_range_max=p_range_max,
+            p_ada=p_ada,
+            p_duplicate_data = p_duplicate_data,
+            p_visualize = p_visualize,
+            p_logging=p_logging,
+            **p_kwargs)
 
-        Returns:
-            List of incides
-        """
-        
-        raise NotImplementedError
+        Norm.NormalizerZTrans.__init__(self)
 
 
 ## -------------------------------------------------------------------------------------------------
-    def _extract_rows(self, p_list_idx: list):
+    def _run(self, p_inst_new:list, p_inst_del:list):
         """
-        Extract the element in the buffer based on a
-        list of indices.
+        Custom method to for run Z-transform task for normalizing new instances and denormalizing deleted instances.
 
-        Parameters:
-            p_list_idx (list): List of indices
+        Parameters
+        ----------
+        p_inst_new: list
+            List of new instances in the workflow
+        p_inst_del: list
+            List of deleted instances in the workflow
 
-        Returns:
-            Samples in dictionary
         """
-        
-        rows = {}
-        for key in self._data_buffer:
-            rows[key] = [self._data_buffer[key][i] for i in p_list_idx]
-        return rows
+        self.adapt(p_inst_new=p_inst_new, p_inst_del=p_inst_del)
 
+        for i, inst in enumerate(p_inst_new):
+            if self._param is None:
+                self.update_parameters(p_data_new=inst.get_feature_data())
+            normalized_element = self.normalize(inst.get_feature_data())
+            inst.get_feature_data().set_values(normalized_element.get_values())
 
-## -------------------------------------------------------------------------------------------------
-    def is_full(self) -> bool:
-        """
-        Check if the buffer is full.
-
-        Returns:
-            True, if the buffer is full
-        """
-        
-        keys = list(self._data_buffer.keys())
-        return len(self._data_buffer[keys[0]]) >= self._size
+        for i,del_inst in enumerate(p_inst_del):
+            if self._param is None:
+                self.update_parameters(p_data_del=del_inst.get_feature_data())
+            normalized_element = self.normalize(del_inst.get_feature_data())
+            del_inst.get_feature_data().set_values(normalized_element.get_values())
 
 
 ## -------------------------------------------------------------------------------------------------
-    def __len__(self):
-        keys = list(self._data_buffer.keys())
-        return len(self._data_buffer[keys[0]])
+    def _adapt(self, p_inst_new:List[Instance]) -> bool:
+        """
+        Custom method to for adapting of Z-transform parameters on new instances.
 
+        Parameters
+        ----------
+        p_inst_new: list
+            List of new instances in the workflow
 
+        Returns
+        -------
+        adapted : bool
+            Returns True, if task has adapted.
 
+        """
 
+        for inst in p_inst_new:
+            self.update_parameters(p_data_new=inst.get_feature_data())
 
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class BufferRnd(Buffer):
-    """
-    Buffer implmentation with random sampling
-    """
+        return True
 
 
 ## -------------------------------------------------------------------------------------------------
-    def _gen_sample_ind(self, p_num: int) -> list:
+    def _adapt_reverse(self, p_inst_del:List[Instance]) -> bool:
         """
-        Generate random indicies
+        Custom method to for adapting of Z-transform parameters on deleted instances.
+
+        Parameters
+        ----------
+        p_inst_del: list
+            List of deleted instances in the workflow
 
-        Parameters:
-            p_num (int): Number of sample
+        Returns
+        -------
+        adapted : bool
+            Returns True, if task has adapted.
 
-        Returns:
-            List of indicies
         """
-        
-        keys = list(self._data_buffer.keys())
-        return random.sample(list(range(0, len(self._data_buffer[keys[0]]))), p_num)
+
+        for del_inst in p_inst_del:
+            self.update_parameters(p_data_del=del_inst.get_feature_data())
+
+        return True
```

### Comparing `mlpro-1.4.0/src/mlpro/bf/datasets/basics.py` & `mlpro-1.4.1/src/mlpro/bf/datasets/basics.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,28 +78,41 @@
 
 
 ## -------------------------------------------------------------------------------------------------
     def __init__(self,
                  p_output_cls = C_CLS_ELEM,
                  p_feature_dataset = None,
                  p_label_dataset = None,
+                 p_features:list[str] = None,
+                 p_labels:list[str] = None,
+                 p_label_indexes:list = None,
                  p_batch_size : int = 1,
                  p_drop_short : bool = False,
                  p_shuffle : bool = False,
                  p_eval_split : float = None,
                  p_test_split : float = None,
                  p_normalize: bool = True,
                  p_settings = None,
                  p_logging = Log.C_LOG_ALL):
 
 
         Log.__init__(self, p_logging = p_logging)
         self._output_cls = p_output_cls
-        self._feature_dataset = p_feature_dataset
-        self._label_dataset = p_label_dataset
+        self._features = p_features
+        self._labels = p_labels
+        self._label_indexes = p_label_indexes
+
+
+        if p_feature_dataset is not None and p_label_dataset is not None:
+            self._feature_dataset = p_feature_dataset
+            self._label_dataset = p_label_dataset
+        elif p_label_dataset:
+            raise ParamError("Please also provide feature dataset as p_dataset.")
+
+
         self._batch_size = p_batch_size
         self._last_batch = False
 
         # 1. Setup the mode of data delivery
         if self._batch_size > 1:
             self._fetch_mode = self.C_FETCH_BATCH
         else:
@@ -218,15 +231,14 @@
         -------
         int
             Length of the dataset.
 
         """
         return len(self._feature_dataset)
 
-
 ## -------------------------------------------------------------------------------------------------
     def set_mode(self, p_mode):
         """
         Sets the mode of the dataset.
 
         Parameters
         ----------
@@ -249,26 +261,43 @@
         if p_mode == self.C_MODE_TEST:
             self.log(Log.C_LOG_TYPE_I, "Dataset mode set to Testing.")
             self._indexes = self._indexes_test.copy()
             self._last_batch = False
 
 
 ## -------------------------------------------------------------------------------------------------
-    @staticmethod
-    def setup_spaces():
+    def setup_spaces(self):
         """
         This is a static custom method to return the feature and label space of the dataset.
 
         Returns
         -------
         Feature Space, Label Space
             A tuple of feature and label space, respectively.
         """
+        feature_space = ESpace()
+        label_space = ESpace()
+        if self._features is not None:
+            for i,feature in enumerate(self._features):
+                feature_space.add_dim(Dimension(p_name_long=feature, p_name_short=f'F{i}_{feature[0:5]}'))
+        else:
+            for i in range(len(self.get_data(0)[0].get_values())):
+                feature_space.add_dim(Dimension(p_name_long=f"Feature {i}", p_name_short=f'F_{i}'))
 
-        return None, None
+        if self._labels is not None:
+            for i,label in enumerate(self._labels):
+               label_space.add_dim(Dimension(p_name_long=label, p_name_short=f'L{i}_{label[0:5]}'))
+        elif self._label_dataset is not None:
+            for i in range(len(self.get_data(0)[1].get_values())):
+                label_space.add_dim(Dimension(p_name_long=f"Label {i}", p_name_short=f'L_{i}'))
+        elif self._label_indexes:
+            for i in range(len(self._label_indexes)):
+                label_space.add_dim(Dimension(p_name_long=f"Label {i}", p_name_short=f'L_{i}'))
+
+        return feature_space, label_space
 
 ## -------------------------------------------------------------------------------------------------
     def _setup_split(self):
 
         """
         The method to split the dataset. This method is called during the instantiation of the class. By defualt the
         dataset is split by dividing the dataset as per the factors given. For custom applications, please rewrite
@@ -297,18 +326,14 @@
         p_shuffle: bool
             Whether the dataset shall be shuffled.
         p_seed: int
             Seed for the purpose of reproducibility.
         p_kwargs: dict
             Additional key worded arguments for custom reset.
 
-        Returns
-        -------
-        Returns the value returned by the custom reset method.
-
         """
         # Shuffle the entire indices
         if not self._split:
             self._indexes.clear()
             self._indexes.extend(self._indexes_train.copy())
             if p_shuffle or self._shuffle:
                 random.shuffle(self._indexes)
@@ -318,18 +343,17 @@
             random.shuffle(self._indexes_train)
             if self._eval_split:
                 random.shuffle(self._indexes_eval)
             if self._test_split:
                 random.shuffle(self._indexes_test)
 
         self._last_batch = False
-        ret_val = self._reset(p_seed=p_seed, p_shuffle=p_shuffle, **p_kwargs)
+        self._reset(p_seed=p_seed, p_shuffle=p_shuffle, **p_kwargs)
         self.log(Log.C_LOG_TYPE_I, "Dataset is reset.")
 
-        return ret_val
 
 ## -------------------------------------------------------------------------------------------------
     def _reset(self, p_seed, p_shuffle = False, **p_kwargs):
         """
         Custom reset method for the dataset.
 
         Parameters
@@ -357,32 +381,37 @@
             Index from which the data shall be fetched.
 
         Returns
         -------
             The data instance at the given instance.
         """
         # 1. Fetch feature and label data and normalize if needed
+        features = self._feature_dataset[p_index]
         if self._normalize:
-            features = self._normalizer_feature_data.normalize(p_data=self._feature_dataset[p_index])
-            labels = self._normalizer_label_data.normalize(p_data=self._label_dataset[p_index])
-        else:
-            features = self._feature_dataset[p_index]
+            features = self._normalizer_feature_data.normalize(p_data=features)
+        if self._label_indexes:
+            labels = []
+            for id in self._label_indexes:
+                labels.append(features.pop(id))
+                label_obj = self._output_cls(self._label_space)
+                label_obj.set_values(labels)
+        elif self._label_dataset is not None:
             labels = self._label_dataset[p_index]
-
-        # 2. Create specific output object, based on the output class
-        if self._output_cls == Element:
-            feature_obj = self._output_cls(self._feature_space)
-            feature_obj.set_values(features)
+            if self._normalize:
+                labels = self._normalizer_label_data.normalize(p_data=labels)
             label_obj = self._output_cls(self._label_space)
             label_obj.set_values(labels)
+        feature_obj = self._output_cls(self._feature_space)
+        feature_obj.set_values(features)
 
-        else:
-            raise ParamError("The output class is not yet supported for this item")
 
-        return feature_obj, label_obj
+        try:
+            return feature_obj, label_obj
+        except:
+            return feature_obj
 
 
 ## -------------------------------------------------------------------------------------------------
     def get_next(self):
 
         """
         Gets the next data instance from the list of indexes prepared for data delivery to a scnenario.
@@ -426,18 +455,21 @@
         del self._indexes[0]
 
         # 4. Get data from that instance, and deliver as BatchElements
         val = self.get_data(index)
 
         feature_element = BatchElement(self._feature_space)
         feature_element.set_values([val[0].get_values()])
-        label_element = BatchElement(self._label_space)
-        label_element.set_values([val[1].get_values()])
+        if self._label_dataset is not None:
+            label_element = BatchElement(self._label_space)
+            label_element.set_values([val[1].get_values()])
 
-        return [(feature_element, label_element)]
+            return [(feature_element, label_element)]
+
+        return feature_element
 
 
 ## -------------------------------------------------------------------------------------------------
     def get_next_batch(self):
         """
         Gets the next batch of data from the dataset for a scenario.
 
@@ -477,26 +509,30 @@
         label_values = []
 
         # 3. Get values and deliver them as BatchElement
         if self._output_cls == Element:
             for index in indexes:
                 vals = self.get_data(index)
                 feature_values.append(vals[0].get_values())
-                label_values.append(vals[1].get_values())
+                if self._label_dataset is not None or self._label_indexes:
+                    label_values.append(vals[1].get_values())
             feature_batch = BatchElement(self._feature_space)
             feature_batch.set_values(feature_values)
-            label_batch = BatchElement(self._label_space)
-            label_batch.set_values(label_values)
+            if self._label_dataset is not None or self._label_indexes:
+                label_batch = BatchElement(self._label_space)
+                label_batch.set_values(label_values)
+                return [(feature_batch, label_batch)]
 
+            return [(feature_batch)]
 
         else:
             raise ParamError("This output class is not yet supported for this dataset")
 
 
-        return [(feature_batch, label_batch)]
+
 
 
 
 
 
 
 ## -------------------------------------------------------------------------------------------------
@@ -543,14 +579,15 @@
     ## -------------------------------------------------------------------------------------------------
     def __init__(self,
                  p_path,
                  p_state_fname,
                  p_action_fname,
                  p_state_space : ESpace,
                  p_action_space : ESpace,
+                 p_op_state_indexes:list[int] = None,
                  p_episode_col = 'Episode ID',
                  p_delimiter = '\t',
                  p_drop_columns = ['Episode ID', 'Cycle', 'Day', 'Second', 'Microsecond'],
                  p_batch_size : int = 1,
                  p_drop_short : bool = False,
                  p_shuffle : bool = False,
                  p_normalize:bool = False,
@@ -567,15 +604,15 @@
                                                             p_drop_columns=p_drop_columns,
                                                             p_episode_col=p_episode_col,
                                                             p_delimiter=p_delimiter)
 
 
         self._state_space = p_state_space.copy(True)
         self._action_space = p_action_space.copy(True)
-
+        self._op_state_indexes = p_op_state_indexes
         # feature_space, label_space = self.setup_spaces()
 
 
         Dataset.__init__(self,
             p_feature_dataset = feature_dataset,
             p_label_dataset = label_dataset,
             p_batch_size=p_batch_size,
@@ -597,20 +634,24 @@
 
         Returns
         -------
         feature_space, label_space: (ESpace, ESpace)
             A tuple of feature and label space of the dataset.
         """
 
-        label_space = self._state_space.copy()
+        if self._op_state_indexes:
+            label_space = self._state_space.spawn(p_id_list=[self._state_space.get_dim_ids()[i] for i in self._op_state_indexes])
+        else:
+            label_space = self._state_space.copy()
+
+        feature_space = self._state_space.copy(p_new_dim_ids=True)
 
         for dim in self._action_space.get_dims():
-            self._state_space.add_dim(dim)
+            feature_space.add_dim(dim)
 
-        feature_space = self._state_space.copy(p_new_dim_ids=True)
 
         return feature_space, label_space
 
 
 ## -------------------------------------------------------------------------------------------------
     def _setup_dataset(self,
                        p_path:str,
@@ -662,7 +703,24 @@
         # Create output df
         output = self._states.iloc[1:].reset_index(drop=True)
         # Drop rows at episode change
         output = output.drop(labels=episode_idx[1:]).values
 
         return input, output
 
+
+## -------------------------------------------------------------------------------------------------
+    def get_data(self, p_index):
+
+        if self._op_state_indexes:
+            features = self._feature_dataset[p_index]
+            labels = [self._label_dataset[p_index][i] for i in self._op_state_indexes]
+
+            feature_obj = BatchElement(self._feature_space)
+            feature_obj.set_values(features)
+            label_obj = BatchElement(self._label_space)
+            label_obj.set_values(labels)
+
+            return feature_obj, label_obj
+
+        else:
+            Dataset.get_data(self, p_index= p_index)
```

### Comparing `mlpro-1.4.0/src/mlpro/bf/events.py` & `mlpro-1.4.1/src/mlpro/bf/events.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/exceptions.py` & `mlpro-1.4.1/src/mlpro/bf/exceptions.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/math/basics.py` & `mlpro-1.4.1/src/mlpro/bf/math/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/ml/basics.py` & `mlpro-1.4.1/src/mlpro/bf/ml/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/ml/systems/basics.py` & `mlpro-1.4.1/src/mlpro/bf/ml/systems/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/mt.py` & `mlpro-1.4.1/src/mlpro/bf/mt.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/ops.py` & `mlpro-1.4.1/src/mlpro/bf/ops.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/physics/basics.py` & `mlpro-1.4.1/src/mlpro/bf/physics/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/physics/unitconverter.py` & `mlpro-1.4.1/src/mlpro/bf/physics/unitconverter.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/plot.py` & `mlpro-1.4.1/src/mlpro/bf/plot.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/streams/models.py` & `mlpro-1.4.1/src/mlpro/bf/streams/models.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/streams/samplers/min_wise.py` & `mlpro-1.4.1/src/mlpro/bf/streams/samplers/min_wise.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/streams/samplers/random.py` & `mlpro-1.4.1/src/mlpro/bf/streams/samplers/random.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/streams/samplers/reservoir_sampling.py` & `mlpro-1.4.1/src/mlpro/bf/streams/samplers/reservoir_sampling.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/streams/samplers/weighted_random.py` & `mlpro-1.4.1/src/mlpro/bf/streams/samplers/weighted_random.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/streams/streams/clouds.py` & `mlpro-1.4.1/src/mlpro/bf/streams/streams/clouds.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/streams/streams/clouds_with_anomalies.py` & `mlpro-1.4.1/src/mlpro/bf/streams/streams/clouds_with_anomalies.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/streams/streams/csv_file.py` & `mlpro-1.4.1/src/mlpro/bf/streams/streams/csv_file.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/streams/streams/doublespiral2d.py` & `mlpro-1.4.1/src/mlpro/bf/streams/streams/doublespiral2d.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/streams/streams/point_outliers.py` & `mlpro-1.4.1/src/mlpro/bf/streams/streams/point_outliers.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 ## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
 ## -- Package : mlpro.bf.streams.streams
 ## -- Module  : point_outliers.py
 ## -------------------------------------------------------------------------------------------------
 ## -- History :
 ## -- yyyy-mm-dd  Ver.      Auth.    Description
 ## -- 2024-02-05  0.0.0     DA       Creation
-## -- 2024-02-06  1.0.0     DA       Creation
+## -- 2024-02-06  1.0.0     DA       First Release
+## -- 2024-04-26  1.1.0     DA       Refactoring: replaced parameter p_outlier_frequency by
+## --                                p_outlier_rate
 ## -------------------------------------------------------------------------------------------------
 
 """
-Ver. 1.0.0 (2024-02-05)
+Ver. 1.1.0 (2024-04-26)
 
 This module provides a multivariate benchmark stream with configurable baselines per feature and
 additional random point outliers.
 
 """
 
 
@@ -34,43 +36,43 @@
 
     p_num_dim : int
         The number of dimensions or features of the data. Default = 3.
     p_num_instances : int
         Total number of instances. The value '0' means indefinite. Default = 1000.
     p_functions : list[str]
         List of mathematical functions per feature. 
-    p_outlier_frequency : int
-        Average frequency of random point outliers.
+    p_outlier_rate : float
+        A value in [0,1] that defines the number of random outliers in % per feature.
     p_seed 
         Seeding value for the random generator. Default = None (no seeding).
     p_logging
         Log level (see constants of class Log). Default: Log.C_LOG_ALL.
     """
 
     C_ID                    = 'PointOutliersND'
     C_NAME                  = 'Point Outliers N-Dim'
     C_TYPE                  = 'Benchmark'
-    C_VERSION               = '1.0.0'
+    C_VERSION               = '1.1.0'
     C_SCIREF_ABSTRACT       = 'This benchmark stream provides multidimensional instances with configurable baselines per feature. Additionally, random point outliers per feature are induced.'
     C_BOUNDARIES            = [0,0]
 
 ## -------------------------------------------------------------------------------------------------
     def __init__( self,
                   p_num_dim : int = 4,
                   p_num_instances : int = 1000,
                   p_functions : list[str] = ['sin', 'cos', 'const', 'lin'],
-                  p_outlier_frequency : int = 50,
+                  p_outlier_rate : float = 0.05,
                   p_seed = None,
                   p_logging = Log.C_LOG_ALL,
                   **p_kwargs ):
         
         self._num_dim            = len(p_functions)
         self.C_NUM_INSTANCES     = p_num_instances
         self._functions          = p_functions
-        self.p_outlier_frequency = p_outlier_frequency
+        self.p_outlier_rate      = p_outlier_rate
         self._fct_methods        = []
 
         for fct in p_functions:
             self._fct_methods.append( getattr(self, '_fct_' + fct) )
 
         self.set_random_seed(p_seed=p_seed)
 
@@ -107,15 +109,15 @@
         if self.C_NUM_INSTANCES== 0: pass
         elif self._index == self.C_NUM_INSTANCES: raise StopIteration
 
         values       = []
         feature_data = Element(self._feature_space)     
 
         for fct_method in self._fct_methods:
-            outlier = random.randint(1,self.p_outlier_frequency) == 1
+            outlier = random.uniform(0,1) <= self.p_outlier_rate
             values.append( fct_method(self._index, outlier) )   
 
         feature_data.set_values(values)
 
         self._index += 1
 
         return Instance( p_feature_data=feature_data )
```

### Comparing `mlpro-1.4.0/src/mlpro/bf/streams/streams/provider_mlpro.py` & `mlpro-1.4.1/src/mlpro/bf/streams/streams/provider_mlpro.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/streams/streams/rnd10d.py` & `mlpro-1.4.1/src/mlpro/bf/streams/streams/rnd10d.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/streams/tasks/deriver.py` & `mlpro-1.4.1/src/mlpro/bf/streams/tasks/deriver.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/streams/tasks/rearranger.py` & `mlpro-1.4.1/src/mlpro/bf/streams/tasks/rearranger.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/streams/tasks/windows.py` & `mlpro-1.4.1/src/mlpro/bf/streams/tasks/windows.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/systems/basics.py` & `mlpro-1.4.1/src/mlpro/bf/systems/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/systems/pool/doublependulum.py` & `mlpro-1.4.1/src/mlpro/bf/systems/pool/doublependulum.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/systems/pool/flipflops.py` & `mlpro-1.4.1/src/mlpro/bf/systems/pool/flipflops.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Arrow.stl` & `mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Arrow.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/X_letter.stl` & `mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/X_letter.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Y_letter.stl` & `mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Y_letter.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Z_letter.stl` & `mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Z_letter.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/texture/logo.png` & `mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/texture/logo.png`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/base.stl` & `mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/base.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/forearm.stl` & `mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/forearm.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/shoulder.stl` & `mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/shoulder.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/upperarm.stl` & `mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/upperarm.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist1.stl` & `mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist1.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist2.stl` & `mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist2.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist3.stl` & `mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist3.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/boxontable.xml` & `mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/boxontable.xml`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/cartpole.xml` & `mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/cartpole.xml`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/doublependulum.xml` & `mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/doublependulum.xml`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/mlpro.xml` & `mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/mlpro.xml`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/pendulum.xml` & `mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/pendulum.xml`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/systems/pool/mujoco/ur5.xml` & `mlpro-1.4.1/src/mlpro/bf/systems/pool/mujoco/ur5.xml`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/ui/sciui/framework.py` & `mlpro-1.4.1/src/mlpro/bf/ui/sciui/framework.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/ui/sciui/main.py` & `mlpro-1.4.1/src/mlpro/bf/ui/sciui/main.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/ui/sciui/pool/iis.py` & `mlpro-1.4.1/src/mlpro/bf/ui/sciui/pool/iis.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/ui/sciui/pool/iisbenchmark.py` & `mlpro-1.4.1/src/mlpro/bf/ui/sciui/pool/iisbenchmark.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/ui/sciui/templates/scenario_test.py` & `mlpro-1.4.1/src/mlpro/bf/ui/sciui/templates/scenario_test.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/bf/various.py` & `mlpro-1.4.1/src/mlpro/bf/various.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/gt/dynamicgames/basics.py` & `mlpro-1.4.1/src/mlpro/gt/dynamicgames/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/gt/dynamicgames/potential.py` & `mlpro-1.4.1/src/mlpro/gt/dynamicgames/potential.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/gt/dynamicgames/stackelberg.py` & `mlpro-1.4.1/src/mlpro/gt/dynamicgames/stackelberg.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/gt/native/basics.py` & `mlpro-1.4.1/src/mlpro/gt/native/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/gt/pool/boards/bglp.py` & `mlpro-1.4.1/src/mlpro/gt/pool/boards/bglp.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/gt/pool/native/games/prisonersdilemma_2p.py` & `mlpro-1.4.1/src/mlpro/gt/pool/native/games/prisonersdilemma_2p.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/gt/pool/native/games/prisonersdilemma_3p.py` & `mlpro-1.4.1/src/mlpro/gt/pool/native/games/prisonersdilemma_3p.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/gt/pool/native/games/rockpaperscissors.py` & `mlpro-1.4.1/src/mlpro/gt/pool/native/games/rockpaperscissors.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/gt/pool/native/games/routingproblems_3p.py` & `mlpro-1.4.1/src/mlpro/gt/pool/native/games/routingproblems_3p.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/gt/pool/native/games/supplydemand_3p.py` & `mlpro-1.4.1/src/mlpro/gt/pool/native/games/supplydemand_3p.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/gt/pool/native/solvers/greedypolicy.py` & `mlpro-1.4.1/src/mlpro/gt/pool/native/solvers/greedypolicy.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/gt/pool/native/solvers/randomsolver.py` & `mlpro-1.4.1/src/mlpro/gt/pool/native/solvers/randomsolver.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/oa/sciui/iis.py` & `mlpro-1.4.1/src/mlpro/oa/sciui/iis.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/oa/sciui/runme.py` & `mlpro-1.4.1/src/mlpro/oa/sciui/runme.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/oa/sciui/scenario_oa1.py` & `mlpro-1.4.1/src/mlpro/oa/sciui/scenario_oa1.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/oa/streams/basics.py` & `mlpro-1.4.1/src/mlpro/oa/streams/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/basics.py` & `mlpro-1.4.1/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/clusterbased.py` & `mlpro-1.4.1/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/clusterbased.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/contextual.py` & `mlpro-1.4.1/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/contextual.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/drift.py` & `mlpro-1.4.1/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/drift.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/group.py` & `mlpro-1.4.1/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/group.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/point.py` & `mlpro-1.4.1/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/point.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/oa/streams/tasks/anomalydetectors/basics.py` & `mlpro-1.4.1/src/mlpro/oa/streams/tasks/anomalydetectors/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/oa/streams/tasks/anomalydetectors/cb_detectors.py` & `mlpro-1.4.1/src/mlpro/oa/streams/tasks/anomalydetectors/cb_detectors.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/oa/streams/tasks/anomalydetectors/paga_detectors.py` & `mlpro-1.4.1/src/mlpro/oa/streams/tasks/anomalydetectors/paga_detectors.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/oa/streams/tasks/boundarydetectors.py` & `mlpro-1.4.1/src/mlpro/oa/streams/tasks/boundarydetectors.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/oa/streams/tasks/clusteranalyzers/basics.py` & `mlpro-1.4.1/src/mlpro/oa/streams/tasks/clusteranalyzers/basics.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,41 +22,50 @@
 ## -- 2023-12-10  0.6.1     DA       Bugfix in method ClusterAnalyzer.get_cluster_membership()
 ## -- 2023-12-20  0.7.0     DA       Renormalization
 ## -- 2024-02-23  0.8.0     DA       Class ClusterCentroid: implementation of methods _remove_plot*
 ## -- 2024-02-24  0.8.1     DA       Method ClusterAnalyzer._remove_cluster() explicitely removes
 ## --                                the plot of a cluster before removal of the cluster itself
 ## -- 2024-02-24  0.8.2     DA       Class ClusterCentroid: redefined method remove_plot()
 ## -- 2024-04-10  0.8.3     DA       Refactoring
+## -- 2024-05-04  0.9.0     DA       Introduction of cluster properties
 ## -------------------------------------------------------------------------------------------------
 
 """
-Ver. 0.8.3 (2024-04-10)
+Ver. 0.9.0 (2024-05-04)
 
 This module provides templates for cluster analysis to be used in the context of online adaptivity.
 """
 
 from matplotlib.figure import Figure
+from mlpro.bf.math.properties import *
 from mlpro.bf.mt import PlotSettings
 from mlpro.bf.streams import Instance
 from mlpro.bf.various import *
 from mlpro.bf.plot import *
 from mlpro.oa.streams import OATask
 from mlpro.bf.math.normalizers import Normalizer
+from mlpro.oa.streams.tasks.clusteranalyzers.clusters import Cluster
 from typing import List, Tuple
 
-from mlpro.oa.streams.tasks.clusteranalyzers.clusters import Cluster
 
 
 
 ## -------------------------------------------------------------------------------------------------
 ## -------------------------------------------------------------------------------------------------
 class ClusterAnalyzer (OATask):
     """
     Base class for online cluster analysis. It raises an event when a cluster was added or removed.
 
+    Steps to implement a new algorithm are:
+    - Create a new class and inherit from this base class
+    - Specify all cluster properties provided/maintained by your algorithm in C_CLUSTER_PROPERTIES.
+    - Implement method self._adapt() to update your cluster list on new instances
+    - Implement method self._adapt_reverse() to update your cluster list on obsolete instances
+    - New cluster: hand over self._cluster_properties on instantiation
+    
     Parameters
     ----------
     p_cls_cluster 
         Cluster class (Class Cluster or a child class).
     p_cluster_limit : int
         Optional limit for clusters to be created. Default = 0 (no limit).
     p_name : str
@@ -78,14 +87,17 @@
     ----------
     C_MS_SCOPE_ALL : int = 0
         Membership scope, that includes all clusters
     C_MS_SCOPE_NONZERO : int = 1
         Membership scope, that includes just clusters with membership values > 0
     C_MS_SCOPE_MAX : int = 2
         Membership scope, that includes just the cluster with the highest membership value.
+    C_CLUSTER_PROPERTIES : PropertyDefinitions
+        List of cluster properties supported/maintained by the algorithm. These properties 
+        are handed over to each new cluster.
     """
 
     C_TYPE                  = 'Cluster Analyzer'
 
     C_EVENT_CLUSTER_ADDED   = 'CLUSTER_ADDED'
     C_EVENT_CLUSTER_REMOVED = 'CLUSTER_REMOVED'
 
@@ -93,17 +105,20 @@
     C_PLOT_STANDALONE       = False
 
     # Possible membership scopes for method get_cluster_memberships
     C_MS_SCOPE_ALL : int    = 0
     C_MS_SCOPE_NONZERO :int = 1
     C_MS_SCOPE_MAX :int     = 2
 
+    # List of cluster properties supported/maintained by the algorithm
+    C_CLUSTER_PROPERTIES : PropertyDefinitions = []
+
 ## -------------------------------------------------------------------------------------------------
     def __init__( self, 
-                  p_cls_cluster,
+                  p_cls_cluster : type = Cluster,
                   p_cluster_limit : int = 0,
                   p_name: str = None, 
                   p_range_max = OATask.C_RANGE_THREAD, 
                   p_ada: bool = True, 
                   p_duplicate_data: bool = False, 
                   p_visualize: bool = False, 
                   p_logging = Log.C_LOG_ALL, 
@@ -117,14 +132,49 @@
                           p_logging = p_logging, 
                           **p_kwargs )
 
         self._cls_cluster   = p_cls_cluster
         self._clusters      = {}
         self._cluster_limit = p_cluster_limit
 
+        self._cluster_properties : PropertyDefinitions = self.C_CLUSTER_PROPERTIES.copy()
+        self._cluster_properties_dict = {}
+        for prop in self._cluster_properties:
+            self._cluster_properties_dict[prop[0]] = prop
+
+
+## -------------------------------------------------------------------------------------------------
+    def align_cluster_properties( self, p_properties : PropertyDefinitions ) -> list:
+        """
+        Aligns list of cluster properties with the given list. In particular, the maximum derivative
+        order of numeric properties is aligned. 
+
+        Parameters
+        ----------
+        p_properties : PropertyDefinitions
+            List of properties to be aligned with.
+
+        Returns
+        list
+            List of unknown properties.
+        """
+
+        unknown_properties = []
+
+        for p_ext in p_properties:
+            try:
+                p_int = self._cluster_properties_dict[p_ext[0]]
+                p_int[1] = p_ext[1]   # alignment of maximum order of derivatives
+                p_int[2] = p_ext[2]   # alignment of property class
+            except:
+                # Property not supported by cluster algorithm
+                unknown_properties.append(p_ext[0])
+
+        return unknown_properties
+
 
 ## -------------------------------------------------------------------------------------------------
     def _run(self, p_inst_new: List[Instance], p_inst_del: List[Instance]):
         self.adapt( p_inst_new=p_inst_new, p_inst_del=p_inst_del )
 
 
 ## -------------------------------------------------------------------------------------------------
@@ -138,14 +188,19 @@
            True, if adding a new cluster allowed. False otherwise.
         """
 
         return ( self._cluster_limit == 0 ) or ( len(self._clusters.key()) < self._cluster_limit )
     
 
 ## -------------------------------------------------------------------------------------------------
+    def get_cluster_cls(self):
+        return self._cls_cluster
+    
+
+## -------------------------------------------------------------------------------------------------
     def get_clusters(self) -> dict[Cluster]:
         """
         This method returns the current list of clusters. 
 
         Returns
         -------
         dict_of_clusters : dict[Cluster]
```

### Comparing `mlpro-1.4.0/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/basics.py` & `mlpro-1.4.1/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/centroid.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ## -------------------------------------------------------------------------------------------------
 ## -- Project : MLPro - The integrative middleware framework for standardized machine learning
 ## -- Package : mlpro.oa.streams.tasks.clusteranalyzers.clusters
-## -- Module  : basics.py
+## -- Module  : centroid.py
 ## -------------------------------------------------------------------------------------------------
 ## -- History :
 ## -- yyyy-mm-dd  Ver.      Auth.    Description
 ## -- 2023-01-24  0.0.0     DA       Creation
 ## -- 2023-04-18  0.1.0     DA       First implementation of classes ClusterMembership, ClusterAnalyzer
 ## -- 2023-05-06  0.2.0     DA       New class ClusterCentroid
 ## -- 2023-05-14  0.3.0     DA       Class ClusterAnalyzer: simplification
@@ -22,96 +22,91 @@
 ## -- 2023-12-10  0.6.1     DA       Bugfix in method ClusterAnalyzer.get_cluster_membership()
 ## -- 2023-12-20  0.7.0     DA       Renormalization
 ## -- 2024-02-23  0.8.0     DA       Class ClusterCentroid: implementation of methods _remove_plot*
 ## -- 2024-02-24  0.8.1     DA       Method ClusterAnalyzer._remove_cluster() explicitely removes
 ## --                                the plot of a cluster before removal of the cluster itself
 ## -- 2024-02-24  0.8.2     DA       Class ClusterCentroid: redefined method remove_plot()
 ## -- 2024-04-10  0.8.3     DA       Refactoring
+## -- 2024-04-29  0.9.0     DA       Refactoring after changes on class Point
+## -- 2024-05-06  1.0.0     DA       Refactoring
 ## -------------------------------------------------------------------------------------------------
 
 """
-Ver. 0.8.3 (2024-04-10)
+Ver. 1.0.0 (2024-05-06)
 
-This module provides templates for clusters to be used in cluster analyzer algorithms.
+This module provides templates for cluster analysis to be used in the context of online adaptivity.
 """
 
-from mlpro.bf.mt import Figure, PlotSettings
+from typing import List, Tuple
+
 from mlpro.bf.various import *
 from mlpro.bf.plot import *
 from mlpro.bf.streams import *
+from mlpro.bf.math.properties import *
 from mlpro.bf.math.normalizers import Normalizer
+from mlpro.oa.streams.tasks.clusteranalyzers.clusters import Cluster
+from mlpro.oa.streams.tasks.clusteranalyzers.clusters.properties import cprop_centroid
 
 
 
 
 ## -------------------------------------------------------------------------------------------------
 ## -------------------------------------------------------------------------------------------------
-class Cluster (Id, Plottable):
+class ClusterCentroid (Cluster):
     """
-    Base class for a cluster. 
+    Extended cluster class with a centroid.
 
     Parameters
     ----------
     p_id
-        Optional external id.
+        Optional external id
     p_visualize : bool
         Boolean switch for visualisation. Default = False.
-    p_color : string
-        Color of the cluster during visualization.
+    p_cls_centroid = Point
+        Name of a point class. Default = Point
     **p_kwargs
         Further optional keyword arguments.
-    """
 
-    C_PLOT_ACTIVE           = True
-    C_PLOT_STANDALONE       = False
-    C_PLOT_VALID_VIEWS      = [ PlotSettings.C_VIEW_2D, 
-                                PlotSettings.C_VIEW_3D, 
-                                PlotSettings.C_VIEW_ND ]
-    C_PLOT_DEFAULT_VIEW     = PlotSettings.C_VIEW_ND
-
-    C_CLUSTER_COLORS        = [ 'blue', 'orange', 'green', 'red', 'purple', 'brown', 'pink', 'gray', 'olive', 'cyan' ]
+    Attributes
+    ----------
+    centroid : Centroid
+        Centroid object.
+    """
 
 ## -------------------------------------------------------------------------------------------------
     def __init__( self, 
                   p_id = None,
-                  p_visualize : bool = False,
-                  p_color = 'red',
-                  **p_kwargs ):
-
-        self._kwargs = p_kwargs.copy()
-        Id.__init__( self, p_id = p_id )
-        Plottable.__init__( self, p_visualize = p_visualize )
+                  p_properties : PropertyDefinitions = [],
+                  p_visualize : bool = False ):
+
+        super().__init__( p_id=p_id, p_properties=p_properties, p_visualize=p_visualize )
+
+        self.add_properties( p_property_definitions = [ cprop_centroid ], p_visualize = p_visualize )
+        self.centroid.set_id( p_id = self.get_id() )
+        self._centroid_elem : Element = None
+
+
+# ## -------------------------------------------------------------------------------------------------
+    def set_id(self, p_id=None):
+        super().set_id( p_id = p_id )
+        try:
+            self.centroid.set_id( p_id = p_id )
+        except:
+            pass
+
+
+## -------------------------------------------------------------------------------------------------
+    def get_membership(self, p_inst: Instance) -> float:
+        feature_data = p_inst.get_feature_data()
+
+        if self._centroid_elem is None:
+            self._centroid_elem = Element( p_set=feature_data.get_related_set() )
+
+        self._centroid_elem.set_values( p_value=self.centroid.value )
+
+        return feature_data.get_related_set().distance( p_e1 = feature_data, p_e2 = self._centroid_elem )
 
 
 ## -------------------------------------------------------------------------------------------------
-    def get_membership(self, p_inst : Instance ) -> float:
-        """
-        Custom method to compute a scalar membership value for the given instance.
-
-        Parameters
-        ----------
-        p_inst : Instance
-            Instance.
-
-        Returns
-        -------
-        float
-            Scalar value >= 0 that determines the membership of the given instance to this cluster. 
-            A value 0 means that the given instance is not a member of the cluster.
-        """
-
-        raise NotImplementedError
-    
-
- ## -------------------------------------------------------------------------------------------------
-    def renormalize(self, p_normalizer:Normalizer):
-        """
-        Custom method to renormalize internally buffered data using the given normalizer object. 
-        This method is called especially by method ClusterAnalyzer._renormalize().
-        
-        Parameters
-        ----------
-        p_normalizer : Normalizer
-            Normalizer object to be applied on task-specific 
-        """
+    def renormalize(self, p_normalizer: Normalizer):
+        self.centroid.renormalize( p_normalizer=p_normalizer)
 
-        pass
```

### Comparing `mlpro-1.4.0/src/mlpro/oa/streams/tasks/normalizers.py` & `mlpro-1.4.1/src/mlpro/rl/models_env_oa.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,404 +1,451 @@
 ## -------------------------------------------------------------------------------------------------
 ## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
-## -- Package : mlpro.oa.tasks.normalizers
-## -- Module  : normalizers.py
+## -- Package : mlpro.rl
+## -- Module  : models_adaptive_environment.py
 ## -------------------------------------------------------------------------------------------------
 ## -- History :
 ## -- yyyy-mm-dd  Ver.      Auth.    Description
-## -- 2022-12-07  1.0.0     LSB      Creation/Release
-## -- 2022-12-13  1.0.1     LSB      Refactoring
-## -- 2022-12-20  1.0.2     DA       Refactoring
-## -- 2022-12-20  1.0.3     LSB      Bugfix
-## -- 2022-12-30  1.0.4     LSB      Bugfix
-## -- 2023-01-12  1.1.0     LSB      Renormalizing plot data
-## -- 2023-01-24  1.1.1     LSB      Bugfix
-## -- 2023-02-13  1.1.2     LSB      Bugfix: Setting the default parameter update flag ot false
-## -- 2023-04-09  1.2.0     DA       Class NormalizerZTransform: new methods _adapt(), _adapt_reverse()
-## -- 2023-05-03  1.2.1     DA       Bugfix in NormalizerMinMax._update_plot_2d/3d/nd
-## -- 2023-05-22  1.2.2     SY       Refactoring
+## -- 2023-05-30  0.0.0     LSB      Creation
+## -- 2023-05-31  0.1.0     LSB      Visulization
+## -- 2023-05-31  0.1.1     LSB      Cleaning
+## -- 2023-05-31  0.1.2     LSB      Visualization fixed
 ## -------------------------------------------------------------------------------------------------
 
 """
-Ver. 1.2.2 (2023-05-22)
+Ver. 0.1.2 (2023-05-31)
 
-This module provides implementation for adaptive normalizers for MinMax Normalization and ZTransformation
+This module provides model classes for adaptive environments
 """
 
 
-from mlpro.oa.streams.basics import *
-from mlpro.bf.math import normalizers as Norm
+from mlpro.oa.streams import *
+from mlpro.oa.systems import *
+from mlpro.rl.models import *
+
+
 
 
 
 ## -------------------------------------------------------------------------------------------------
 ## -------------------------------------------------------------------------------------------------
-class NormalizerMinMax (OATask, Norm.NormalizerMinMax):
+class OAFctReward(FctReward, Model):
     """
-    Class with functionality for adaptive normalization of instances using MinMax Normalization.
+    This is a template class for Online Adaptive Reward Computation function. Please overwrite the
+    _compute_reward() method or provide an adaptive class as a parameter with all the additional
+    required parameters.
 
     Parameters
     ----------
-    p_name: str, optional
-        Name of the task.
-    p_range_max:
-        Processing range of the task, default is a Thread.
-    p_ada:
-        True if the task has adaptivity, default is true.
-    p_duplicate_data : bool
-        If True, instances will be duplicated before processing. Default = False.
-    p_visualize:
-        True for visualization, false by default.
-    p_logging:
-        Logging level of the task. Default is Log.C_LOG_ALL
-    p_kwargs:
-        Additional task parameters
+    p_id
+    p_name
+    p_range_max
+    p_autorun
+    p_class_shared
+    p_ada
+    p_afct_cls
+    p_state_space
+    p_action_space
+    p_input_space_cls
+    p_output_space_cls
+    p_output_elem_cls
+    p_threshold
+    p_buffer_size
+    p_wf_reward
+    p_visualize
+    p_logging
+    p_kwargs
     """
 
-    C_NAME = 'Normalizer MinMax' 
 
 ## -------------------------------------------------------------------------------------------------
-    def __init__(self,p_name: str = None,
-                  p_range_max = StreamTask.C_RANGE_THREAD,
-                  p_ada : bool = True,
-                  p_duplicate_data : bool = False,
-                  p_visualize:bool = False,
-                  p_logging = Log.C_LOG_ALL,
-                  **p_kwargs):
-
-        OATask.__init__(self,
-                        p_name = p_name,
-                        p_range_max = p_range_max,
-                        p_ada = p_ada,
-                        p_duplicate_data = p_duplicate_data,
-                        p_visualize = p_visualize,
-                        p_logging=p_logging,
-                        **p_kwargs )
-
-
-        Norm.NormalizerMinMax.__init__(self)
-        self._parameters_updated:bool = None
+    def __init__(self,
+                 p_id = None,
+                 p_name: str = None,
+                 p_range_max: int = Async.C_RANGE_PROCESS,
+                 p_autorun: int = Task.C_AUTORUN_NONE,
+                 p_class_shared = None,
+                 p_ada:bool=True,
+                 p_afct_cls = None,
+                 p_state_space: MSpace = None,
+                 p_action_space: MSpace = None,
+                 p_input_space_cls=ESpace,
+                 p_output_space_cls=ESpace,
+                 p_output_elem_cls=State,  # Specific output element type
+                 p_threshold=0,
+                 p_buffer_size=0,
+                 p_wf_reward: OAWorkflow = None,
+                 p_visualize:bool=False,
+                 p_logging=Log.C_LOG_ALL,
+                 **p_kwargs):
 
-        if p_visualize:
-            self._plot_data_2d = None
-            self._plot_data_3d = None
-            self._plot_data_nd = None
+        self._afct_reward = None
+        if p_afct_cls is not None:
+            if (p_state_space is None) or (p_action_space is None):
+                raise ParamError("Please provide mandatory parameters state and action space.")
+
+            self._afct_reward = AFctReward(p_afct_cls=p_afct_cls,
+                                             p_state_space=p_state_space,
+                                             p_action_space=p_action_space,
+                                             p_input_space_cls=p_input_space_cls,
+                                             p_output_space_cls=p_output_space_cls,
+                                             p_output_elem_cls=p_output_elem_cls,
+                                             p_threshold=p_threshold,
+                                             p_buffer_size=p_buffer_size,
+                                             p_ada=p_ada,
+                                             p_visualize=p_visualize,
+                                             p_logging=p_logging,
+                                             **p_kwargs)
+
+        FctReward.__init__(self, p_logging = p_logging)
+
+        Model.__init__(self,
+                       p_id= p_id,
+                       p_name=p_name,
+                       p_range_max=p_range_max,
+                       p_autorun=p_autorun,
+                       p_class_shared=p_class_shared,
+                       p_ada=p_ada,
+                       p_visualize=p_visualize,
+                       p_logging=p_logging,
+                       **p_kwargs)
+
+        if p_wf_reward is None:
+            self._wf_reward = OAWorkflow(p_name='Reward Computation',
+                                         p_visualize=p_visualize,
+                                         p_ada=p_ada,
+                                         p_logging=p_logging)
+        else:
+            self._wf_reward = p_wf_reward
+
+
+        self._state_obj_old:State = None
+        self._state_obj_new:State = None
+        self._setup_wf_reward = False
+        self._inst_old:State = None
 
 
 ## -------------------------------------------------------------------------------------------------
-    def _run(self, p_inst_new:list, p_inst_del:list):
+    def compute_reward(self, p_state_old: State = None, p_state_new: State = None) -> Reward:
         """
-        Custom method to for run MinMax Normalizer task for normalizing new instances and denormalizing deleted
-        instances.
 
         Parameters
         ----------
-        p_inst_new: list
-            List of new instances in the workflow
-        p_inst_del: list
-            List of deleted instances in the workflow
-        """
+        p_state
+        p_state_new
+
+        Returns
+        -------
 
-        if ((p_inst_new is None) or (len(p_inst_new) == 0)
-                and ((p_inst_del is None) or len(p_inst_del) ==0)) : return
+        """
 
-        for i,inst in enumerate(p_inst_new):
-            if self._param is None:
-                self.update_parameters(inst.get_feature_data().get_related_set())
-            normalized_element = self.normalize(inst.get_feature_data())
-            inst.get_feature_data().set_values(normalized_element.get_values())
+        # 1. Copy the state parameters for further processing
+        self.log(Log.C_LOG_TYPE_I, 'Start Computing the Reward....')
+        if p_state_old is not None:
+            self._state_obj_old = p_state_old.copy()
+        self._state_obj_new = p_state_new.copy()
+
+        # 2. Check for the first run
+        if not self._setup_wf_reward:
+            self._setup_wf_reward = self._setup_oafct_reward()
+
+        # 2.1 Check if the first instance (old state) is already processed
+        if self._inst_old is None:
+            inst_new = [self._state_obj_old, self._state_obj_new]
+        else:
+            inst_new = [self._state_obj_new]
 
-        for j, del_inst in enumerate(p_inst_del):
-            if self._param is None:
-                self.update_parameters(del_inst.get_feature_data().get_related_set())
-            normalized_element = self.normalize(del_inst.get_feature_data())
-            del_inst.get_feature_data().set_values(normalized_element.get_values())
+        # 3. Run the workflow
+        self._wf_reward.run(p_inst_new=inst_new)
 
+        # 4. Return the results
+        return self._wf_reward.get_so().get_results()[self.get_tid()]
 
 ## -------------------------------------------------------------------------------------------------
-    def _adapt_on_event(self, p_event_id:str, p_event_object:Event) -> bool:
+    def _adapt_on_event(self, p_event_id: str, p_event_object: Event) -> bool:
         """
-        Custom method to adapt the MinMax normalizer parameters based on event raised by Boundary object for changed
-        boundaries.
 
         Parameters
         ----------
-        p_event_id: str
-            Event id of the raised event
-
-        p_event_obj: Event
-            Event object that raises the corresponding event
+        p_event_id
+        p_event_object
 
         Returns
         -------
-        adapted: bool
-            Returns True, if the task has adapted. False otherwise.
-        """
 
-        set = p_event_object.get_raising_object().get_related_set()
+        """
+        pass
 
-        self.update_parameters(set)
+## -------------------------------------------------------------------------------------------------
+    def add_task_reward(self, p_task: StreamTask, p_pred_tasks: list = None):
+        """
+        Adds a task to the workflow.
+        Parameters
+        ----------
+        p_task: OATask, StreamTask
+            The task to be added to the workflow
 
-        self._parameters_updated = True
+        p_pred_task: list[Task]
+            Name of the predecessor tasks for the task to be added
 
-        return True
+        """
 
+        self._wf_reward.add_task(p_task=p_task, p_pred_tasks=p_pred_tasks)
 
 ## -------------------------------------------------------------------------------------------------
-    def _update_plot_2d( self,
-                         p_settings : PlotSettings,
-                         p_inst_new : list,
-                         p_inst_del : list,
-                         **p_kwargs ):
+    def _run_wf_reward(self, p_inst_new, p_inst_del):
         """
-
-        Method to update the 2d plot for Normalizer. Extended to renormalize the obsolete data on change of parameters.
+        Runs the reward computation workflow of the system.
 
         Parameters
         ----------
-        p_settings : PlotSettings
-            Object with further plot settings.
-        p_inst_new : list
-            List of new stream instances to be plotted.
-        p_inst_del : list
-            List of obsolete stream instances to be removed.
-        p_kwargs : dict
-            Further optional plot parameters.
-        """
-
-        if self._parameters_updated and ( len(self._plot_2d_xdata) != 0 ):
+        p_inst_new: list[State]
+            List of new instances to be processed by the workflow.
 
-            if ( self._plot_data_2d is None ) or ( len(self._plot_2d_xdata) > self._plot_data_2d.shape[0] ):
-                self._plot_data_2d = np.zeros((len(self._plot_2d_xdata),2))
+        p_inst_del: list[State]
+            List of old instances to be processed by the workflow.
 
-            for i in range(len(self._plot_2d_xdata)):
-                self._plot_data_2d[i][0] = self._plot_2d_xdata[i]
-                self._plot_data_2d[i][1] = self._plot_2d_ydata[i]
+        """
+        if len(p_inst_new) == 2 :
+            state_new = p_inst_new[1]
+            self._inst_old = p_inst_new[0]
 
-            plot_data_renormalized = self.renormalize(self._plot_data_2d)
+        elif len(p_inst_new) == 1:
+            state_new = p_inst_new[0]
 
-            self._plot_2d_xdata = list(j[0] for j in plot_data_renormalized)
-            self._plot_2d_ydata = list(j[1] for j in plot_data_renormalized)
+        if self._inst_old is not None:
+            state_old = self._inst_old
 
-            self._parameters_updated = False
+        else:
+            state_old = p_inst_new[0]
 
-        OATask._update_plot_2d(self, p_settings = p_settings,
-                               p_inst_new = p_inst_new,
-                               p_inst_del = p_inst_del,
-                               **p_kwargs)
 
+        if self._afct_reward is not None:
+            self._wf_reward.get_so().add_result(self.get_id(), AFctReward.compute_reward(self,
+                                                                              p_state_new=state_new,
+                                                                              p_state_old=state_old))
+        else:
+            self._wf_reward.get_so().add_result(self.get_id(), FctReward.compute_reward(self,
+                                                                             p_state_new=state_new,
+                                                                             p_state_old=state_old))
 
-## -------------------------------------------------------------------------------------------------
-    def _update_plot_3d( self,
-                         p_settings : PlotSettings,
-                         p_inst_new : list,
-                         p_inst_del : list,
-                         **p_kwargs ):
+# -------------------------------------------------------------------------------------------------
+    def _adapt(self, **p_kwargs) -> bool:
         """
-        Method to update the 3d plot for Normalizer. Extended to renormalize the obsolete data on change of parameters.
+        When called, the function and it's components adapt based on the provided parameters.
 
         Parameters
         ----------
-        p_settings : PlotSettings
-            Object with further plot settings.
-        p_inst_new : list
-            List of new stream instances to be plotted.
-        p_inst_del : list
-            List of obsolete stream instances to be removed.
-        p_kwargs : dict
-            Further optional plot parameters.
+        p_kwargs
+            additional parameters for adaptation.
 
+        Returns
+        -------
+        adapted: bool
+            Returns true if the Function has adapted
         """
 
-        if self._parameters_updated and ( len(self._plot_3d_xdata) != 0 ):
-
-            if ( self._plot_data_3d is None ) or ( len(self._plot_3d_xdata) > self._plot_data_3d.shape[0] ):
-                self._plot_data_3d = np.zeros((len(self._plot_3d_xdata),3))
-
-            for i in range(len(self._plot_3d_xdata)):
-                self._plot_data_3d[i][0] = self._plot_3d_xdata[i]
-                self._plot_data_3d[i][1] = self._plot_3d_ydata[i]
-                self._plot_data_3d[i][2] = self._plot_3d_zdata[i]
-
-
-            plot_data_renormalized = self.renormalize(self._plot_data_3d)
-
-            self._plot_3d_xdata = list(j[0] for j in plot_data_renormalized)
-            self._plot_3d_ydata = list(j[1] for j in plot_data_renormalized)
-            self._plot_3d_zdata = list(j[2] for j in plot_data_renormalized)
+        adapted = False
+        try:
+            adapted = self._wf_reward.adapt(**p_kwargs) or adapted
+        except:
+            adapted = False or adapted
 
-            self._parameters_updated = False
+        if self._afct_reward is not None:
+            try:
+                adapted = self._afct_reward.adapt(**p_kwargs) or adapted
+            except:
+                adapted = False or adapted
 
-        OATask._update_plot_3d(self, p_settings = p_settings,
-                               p_inst_new = p_inst_new,
-                               p_inst_del = p_inst_del,
-                               **p_kwargs)
+        return adapted
 
 
 ## -------------------------------------------------------------------------------------------------
-    def _update_plot_nd( self,
-                         p_settings : PlotSettings,
-                         p_inst_new : list,
-                         p_inst_del : list,
-                         **p_kwargs ):
+    def _setup_oafct_reward(self):
         """
+        Adds a pseudo task to the success computation workflow, with the method to be wrapped.
 
-        Method to update the nd plot for Normalizer. Extended to renormalize the obsolete data on change of parameters.
+        Returns
+        -------
+        bool
+            False when successfully setup.
 
-        Parameters
-        ----------
-        p_settings : PlotSettings
-            Object with further plot settings.
-        p_inst_new : list
-            List of new stream instances to be plotted.
-        p_inst_del : list
-            List of obsolete stream instances to be removed.
-        p_kwargs : dict
-            Further optional plot parameters.
         """
+        if len(self._wf_reward._tasks) == 0:
+            p_pred_tasks = None
+        else:
+            p_pred_tasks = [self._wf_reward._tasks[-1]]
 
-        if self._parameters_updated and self._plot_nd_plots:
-            if (len(self._plot_nd_plots[0][0])) != 0:
-
-                if ( self._plot_data_nd is None ) or ( len(self._plot_nd_plots[0][0]) > self._plot_data_nd.shape[0] ):
-                    self._plot_data_nd = np.zeros((len(self._plot_nd_plots[0][0]),len(self._plot_nd_plots)))
-
-                for j in range(len(self._plot_nd_plots)):
-                    for i in range(len(self._plot_nd_plots[0][0])):
-                        self._plot_data_nd[i][j] = self._plot_nd_plots[j][0][i]
-
-                plot_data_renormalized = self.renormalize(self._plot_data_nd)
-
-                for j in range(len(self._plot_nd_plots)):
-                    self._plot_nd_plots[j][0] = list(k[j] for k in plot_data_renormalized)
-
-
-                self._parameters_updated = False
+        self._wf_reward.add_task(p_task=PseudoTask(p_wrap_method=self._run_wf_reward),
+                                  p_pred_tasks=p_pred_tasks)
+        return True
 
-        OATask._update_plot_nd( self, 
-                                p_settings = p_settings,
-                                p_inst_new = p_inst_new,
-                                p_inst_del = p_inst_del,
-                                **p_kwargs )
 
 
 
 
 
 ## -------------------------------------------------------------------------------------------------
 ## -------------------------------------------------------------------------------------------------
-class NormalizerZTransform (OATask, Norm.NormalizerZTrans):
+class OAEnvironment(OAFctReward, OASystem, Environment):
     """
-    Class with functionality of adaptive normalization of instances with Z-Transformation
+    Template class for Online Adaptive Environments, which adds the Online Adaptive Reward Computation functionality
+    over OASystem.
 
     Parameters
     ----------
-    p_name: str, optional
-        Name of the task.
-    p_range_max:
-        Processing range of the task, default is a Thread.
-    p_ada:
-        True if the task has adaptivity, default is true.
-    p_duplicate_data : bool
-        If True, instances will be duplicated before processing. Default = False.
-    p_visualize:
-        True for visualization, false by default.
-    p_logging:
-        Logging level of the task. Default is Log.C_LOG_ALL
-    p_kwargs:
-        Additional task parameters
+    p_id
+    p_name
+    p_buffer_size
+    p_ada
+    p_range_max
+    p_autorun
+    p_class_shared
+    p_mode
+    p_latency
+    p_t_step
+    p_fct_strans
+    p_fct_reward
+    p_fct_success
+    p_fct_broken
+    p_wf
+    p_wf_success
+    p_wf_broken
+    p_wf_reward
+    p_mujoco_file
+    p_frame_skip
+    p_state_mapping
+    p_action_mapping
+    p_camera_conf
+    p_visualize
+    p_logging
+    p_kwargs
     """
-    C_NAME = 'Normalizer Z Transform'
 
-## -------------------------------------------------------------------------------------------------
-    def __init__(self, p_name: str = None,
-                 p_range_max=StreamTask.C_RANGE_THREAD,
+
+    ## -------------------------------------------------------------------------------------------------
+    def __init__(self,
+                 p_id = None,
+                 p_name: str = None,
+                 p_buffer_size: int = 0,
                  p_ada: bool = True,
-                 p_duplicate_data : bool = False,
-                 p_visualize = False,
-                 p_logging=Log.C_LOG_ALL,
+                 p_range_max: int = Range.C_RANGE_NONE,
+                 p_autorun: int = Task.C_AUTORUN_NONE,
+                 p_class_shared: Shared = None,
+                 p_mode=Mode.C_MODE_SIM,
+                 p_latency: timedelta = None,
+                 p_t_step: timedelta = None,
+                 p_fct_strans: FctSTrans = None,
+                 p_fct_reward: FctReward = None,
+                 p_fct_success: FctSuccess = None,
+                 p_fct_broken: FctBroken = None,
+                 p_wf : OAWorkflow = None,
+                 p_wf_success : OAWorkflow = None,
+                 p_wf_broken : OAWorkflow = None,
+                 p_wf_reward : OAWorkflow = None,
+                 p_mujoco_file = None,
+                 p_frame_skip: int = 1,
+                 p_state_mapping = None,
+                 p_action_mapping = None,
+                 p_camera_conf: tuple = (None, None, None),
+                 p_visualize: bool = False,
+                 p_logging: bool = Log.C_LOG_ALL,
                  **p_kwargs):
 
-        OATask.__init__(self,
-            p_name=p_name,
-            p_range_max=p_range_max,
-            p_ada=p_ada,
-            p_duplicate_data = p_duplicate_data,
-            p_visualize = p_visualize,
-            p_logging=p_logging,
-            **p_kwargs)
 
-        Norm.NormalizerZTrans.__init__(self)
+        OAFctReward.__init__(self, p_wf_reward=p_wf_reward, p_visualize=p_visualize)
+
+        Environment.__init__(self,
+                             p_mode = p_mode,
+                             p_latency = p_latency,
+                             p_fct_strans = p_fct_strans,
+                             p_fct_reward = p_fct_reward,
+                             p_fct_success = p_fct_success,
+                             p_fct_broken = p_fct_broken,
+                             p_mujoco_file = p_mujoco_file,
+                             p_frame_skip = p_frame_skip,
+                             p_state_mapping = p_state_mapping,
+                             p_action_mapping = p_action_mapping,
+                             p_camera_conf = p_camera_conf,
+                             p_visualize = p_visualize,
+                             p_logging = p_logging)
+
+        OASystem.__init__(self,
+                            p_id=p_id,
+                            p_name=p_name,
+                            p_range_max=p_range_max,
+                            p_autorun=p_autorun,
+                            p_class_shared=p_class_shared,
+                            p_ada=p_ada,
+                            p_mode=p_mode,
+                            p_latency=p_latency,
+                            p_t_step=p_t_step,
+                            p_fct_strans=p_fct_strans,
+                            p_fct_success=p_fct_success,
+                            p_fct_broken=p_fct_broken,
+                            p_wf=p_wf,
+                            p_wf_success=p_wf_success,
+                            p_wf_broken=p_wf_broken,
+                            p_mujoco_file=p_mujoco_file,
+                            p_frame_skip=p_frame_skip,
+                            p_state_mapping=p_state_mapping,
+                            p_action_mapping=p_action_mapping,
+                            p_camera_conf=p_camera_conf,
+                            p_visualize=p_visualize,
+                            p_logging=p_logging,
+                            **p_kwargs)
+
+
+        self._workflows.append(self._wf_reward)
+        self._fcts.append(self._fct_reward)
 
 
 ## -------------------------------------------------------------------------------------------------
-    def _run(self, p_inst_new:list, p_inst_del:list):
+    def compute_reward(self, p_state_old: State = None, p_state_new: State = None) -> Reward:
         """
-        Custom method to for run Z-transform task for normalizing new instances and denormalizing deleted instances.
+        Simulates a state transition based on a state and action. Custom method _simulate_reaction()
+        is called.
 
         Parameters
         ----------
-        p_inst_new: list
-            List of new instances in the workflow
-        p_inst_del: list
-            List of deleted instances in the workflow
-
-        """
-        self.adapt(p_inst_new=p_inst_new, p_inst_del=p_inst_del)
+        p_state: State
+            State of the System.
 
-        for i, inst in enumerate(p_inst_new):
-            if self._param is None:
-                self.update_parameters(p_data_new=inst.get_feature_data())
-            normalized_element = self.normalize(inst.get_feature_data())
-            inst.get_feature_data().set_values(normalized_element.get_values())
+        p_action: Action
+            External action provided for the action simulation
 
-        for i,del_inst in enumerate(p_inst_del):
-            if self._param is None:
-                self.update_parameters(p_data_del=del_inst.get_feature_data())
-            normalized_element = self.normalize(del_inst.get_feature_data())
-            del_inst.get_feature_data().set_values(normalized_element.get_values())
-
-
-## -------------------------------------------------------------------------------------------------
-    def _adapt(self, p_inst_new:List[Instance]) -> bool:
-        """
-        Custom method to for adapting of Z-transform parameters on new instances.
-
-        Parameters
-        ----------
-        p_inst_new: list
-            List of new instances in the workflow
+        p_t_step: timedelta, optional.
+            The timestep for which the system is to be simulated
 
         Returns
         -------
-        adapted : bool
-            Returns True, if task has adapted.
+        state: State
+            The new state of the System.
 
         """
+        if p_state_old is not None:
+            state_old = p_state_old
+        else:
+            state_old = self._prev_state
 
-        for inst in p_inst_new:
-            self.update_parameters(p_data_new=inst.get_feature_data())
+        if state_old is None:
+            return None
 
-        return True
+        if p_state_new is not None:
+            state_new = p_state_new
 
+        else:
+            state_new = self._state
 
-## -------------------------------------------------------------------------------------------------
-    def _adapt_reverse(self, p_inst_del:List[Instance]) -> bool:
-        """
-        Custom method to for adapting of Z-transform parameters on deleted instances.
+        if self._fct_reward is not None:
+            self._last_reward = self._fct_reward.compute_reward(p_state_new=state_new, p_state_old=state_old)
+        else:
+            self._last_reward = OAFctReward.compute_reward(self, p_state_new=state_new, p_state_old=state_old)
 
-        Parameters
-        ----------
-        p_inst_del: list
-            List of deleted instances in the workflow
+        return self._last_reward
 
-        Returns
-        -------
-        adapted : bool
-            Returns True, if task has adapted.
 
-        """
+## -------------------------------------------------------------------------------------------------
+    def get_workflow_reward(self):
 
-        for del_inst in p_inst_del:
-            self.update_parameters(p_data_del=del_inst.get_feature_data())
+        return self._wf_reward
 
-        return True
```

### Comparing `mlpro-1.4.0/src/mlpro/oa/systems/basics.py` & `mlpro-1.4.1/src/mlpro/oa/systems/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/oa/systems/pool/doublependulum.py` & `mlpro-1.4.1/src/mlpro/oa/systems/pool/doublependulum.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/rl/models.py` & `mlpro-1.4.1/src/mlpro/rl/models.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/rl/models_agents.py` & `mlpro-1.4.1/src/mlpro/rl/models_agents.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/rl/models_env.py` & `mlpro-1.4.1/src/mlpro/rl/models_env.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/rl/models_env_ada.py` & `mlpro-1.4.1/src/mlpro/rl/models_env_ada.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/rl/models_train.py` & `mlpro-1.4.1/src/mlpro/rl/models_train.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/rl/pool/actionplanner/mpc.py` & `mlpro-1.4.1/src/mlpro/rl/pool/actionplanner/mpc.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/rl/pool/envs/bglp.py` & `mlpro-1.4.1/src/mlpro/rl/pool/envs/bglp.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/rl/pool/envs/cartpole.py` & `mlpro-1.4.1/src/mlpro/rl/pool/envs/cartpole.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/rl/pool/envs/doublependulum.py` & `mlpro-1.4.1/src/mlpro/rl/pool/envs/doublependulum.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/rl/pool/envs/gridworld.py` & `mlpro-1.4.1/src/mlpro/rl/pool/envs/gridworld.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/rl/pool/envs/robotinhtm.py` & `mlpro-1.4.1/src/mlpro/rl/pool/envs/robotinhtm.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/rl/pool/policies/dummy.py` & `mlpro-1.4.1/src/mlpro/rl/pool/policies/dummy.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/rl/pool/policies/randomgenerator.py` & `mlpro-1.4.1/src/mlpro/rl/pool/policies/randomgenerator.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/rl/pool/sarsbuffer/PrioritizedBuffer.py` & `mlpro-1.4.1/src/mlpro/rl/pool/sarsbuffer/PrioritizedBuffer.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/rl/pool/sarsbuffer/RandomSARSBuffer.py` & `mlpro-1.4.1/src/mlpro/rl/pool/sarsbuffer/RandomSARSBuffer.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/rl/sciui_rl.py` & `mlpro-1.4.1/src/mlpro/rl/sciui_rl.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/sl/basics.py` & `mlpro-1.4.1/src/mlpro/sl/basics.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 ## --                                - Remove SLNetwork
 ## -- 2023-03-10  0.4.3     DA       Class SLAdaptiveFunction: refactoring of constructor parameters
 ## -- 2023-06-20  0.4.4     LSB      Moved the quality check to the adapt online method
 ## -- 2023-06-20  0.5.0     LSB      New methods: adapt_offline and adapt_online
 ## -- 2023-07-24  0.5.1     LSB      Merged the new methods back to _adapt method
 ## -------------------------------------------------------------------------------------------------
 
+
 """
 Ver. 0.5.1 (2023-06-24)
 
 This module provides model classes for supervised learning tasks. 
 """
```

### Comparing `mlpro-1.4.0/src/mlpro/sl/examples/howto_sl_afct_100_train_and_reload_pytorch_mlp.py` & `mlpro-1.4.1/src/mlpro/sl/examples/howto_sl_afct_100_train_and_reload_pytorch_mlp.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 ## -- Package : mlpro.sl
 ## -- Module  : models_data.py
 ## -------------------------------------------------------------------------------------------------
 ## -- History :
 ## -- yyyy-mm-dd  Ver.      Auth.    Description
 ## -- 2023-06-18  0.0.0     LSB      Creation
 ## -- 2023-07-15  1.0.0     LSB      Release
+## -- 2023-07-30  1.0.1     LSB      Updates regarding selected output variables
 ## -------------------------------------------------------------------------------------------------
 
 """
-Ver. 1.0.0 (2023-07-15)
+Ver. 1.0.1 (2023-07-30)
 
 This module provides dataset classes for supervised learning tasks.
 
 You will learn:
 
 1. How to setup a SLScenario and Training
 
@@ -80,31 +81,32 @@
 
 
         self._dataset = SASDataset(p_path=train_path,
                                     p_state_fname=name_train_states,
                                     p_action_fname=name_train_actions,
                                     p_state_space=state_space,
                                     p_action_space=action_space,
+                                    p_op_state_indexes=[0,2],
                                     p_normalize=True,
                                     p_batch_size=16,
                                     p_eval_split=0.5,
                                     p_shuffle=False,
                                     p_logging=Log.C_LOG_WE)
 
 
         return PyTorchMLP(p_input_space=self._dataset._feature_space,
                                  p_output_space=self._dataset._label_space,
                                  p_output_elem_cls=BatchElement,
-                                 p_num_hidden_layers=3,
+                                 p_num_hidden_layers=5,
                                  p_activation_fct=nn.LeakyReLU(0.5),
                                  p_output_activation_fct=nn.LeakyReLU(1),
                                  p_optimizer=opt.Adam,
                                  p_batch_size=200,
                                  p_metrics=[MSEMetric(p_logging=Log.C_LOG_NOTHING),
-                                            MetricAccuracy(p_threshold=10, p_logging=Log.C_LOG_NOTHING)],
+                                            MetricAccuracy(p_threshold=20, p_logging=Log.C_LOG_NOTHING)],
                                  p_learning_rate=0.0005,
                                  p_hidden_size=256,
                                  p_loss_fct=nn.MSELoss,
                                  p_logging=Log.C_LOG_WE)
 
 
 
@@ -172,14 +174,15 @@
     def _setup(self, p_mode, p_ada:bool, p_visualize:bool, p_logging) -> Model:
 
         self._dataset = SASDataset(p_path = inference_path,
                                    p_state_fname = name_infer_states,
                                    p_action_fname = name_infer_actions,
                                    p_state_space=state_space,
                                    p_action_space=action_space,
+                                   p_op_state_indexes=[0,2],
                                    p_batch_size=1,
                                    p_shuffle=False,
                                    p_normalize = True,
                                    p_logging=Log.C_LOG_NOTHING)
```

### Comparing `mlpro-1.4.0/src/mlpro/sl/fnn.py` & `mlpro-1.4.1/src/mlpro/sl/fnn.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/sl/models_eval.py` & `mlpro-1.4.1/src/mlpro/sl/models_eval.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/sl/models_train.py` & `mlpro-1.4.1/src/mlpro/sl/models_train.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/sl/pool/afct/fnn/pytorch/mlp.py` & `mlpro-1.4.1/src/mlpro/sl/pool/afct/fnn/pytorch/mlp.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/sl/pool/afct/pytorch.py` & `mlpro-1.4.1/src/mlpro/sl/pool/afct/pytorch.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/wrappers/basics.py` & `mlpro-1.4.1/src/mlpro/wrappers/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro/wrappers/mujoco.py` & `mlpro-1.4.1/src/mlpro/wrappers/mujoco.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/src/mlpro.egg-info/PKG-INFO` & `mlpro-1.4.1/src/mlpro.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpro
-Version: 1.4.0
+Version: 1.4.1
 Summary: MLPro - The Integrative Middleware Framework for Standardized Machine Learning
 Home-page: https://mlpro.readthedocs.io
 Author: MLPro Team
 Author-email: mlpro@listen.fh-swf.de
 Project-URL: Bug Tracker, https://mlpro.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mlpro-1.4.0/src/mlpro.egg-info/SOURCES.txt` & `mlpro-1.4.1/src/mlpro.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -6,27 +6,33 @@
 src/mlpro/__init__.py
 src/mlpro.egg-info/PKG-INFO
 src/mlpro.egg-info/SOURCES.txt
 src/mlpro.egg-info/dependency_links.txt
 src/mlpro.egg-info/requires.txt
 src/mlpro.egg-info/top_level.txt
 src/mlpro/bf/__init__.py
-src/mlpro/bf/data.py
 src/mlpro/bf/events.py
 src/mlpro/bf/exceptions.py
 src/mlpro/bf/mt.py
 src/mlpro/bf/ops.py
 src/mlpro/bf/plot.py
 src/mlpro/bf/various.py
+src/mlpro/bf/data/__init__.py
+src/mlpro/bf/data/buffers.py
+src/mlpro/bf/data/datastoring.py
 src/mlpro/bf/datasets/__init__.py
 src/mlpro/bf/datasets/basics.py
 src/mlpro/bf/math/__init__.py
 src/mlpro/bf/math/basics.py
 src/mlpro/bf/math/geometry.py
-src/mlpro/bf/math/normalizers.py
+src/mlpro/bf/math/properties.py
+src/mlpro/bf/math/normalizers/__init__.py
+src/mlpro/bf/math/normalizers/basics.py
+src/mlpro/bf/math/normalizers/minmax.py
+src/mlpro/bf/math/normalizers/ztrans.py
 src/mlpro/bf/ml/__init__.py
 src/mlpro/bf/ml/basics.py
 src/mlpro/bf/ml/systems/__init__.py
 src/mlpro/bf/ml/systems/basics.py
 src/mlpro/bf/ml/systems/pool/__init__.py
 src/mlpro/bf/physics/__init__.py
 src/mlpro/bf/physics/basics.py
@@ -127,14 +133,17 @@
 src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/group.py
 src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/point.py
 src/mlpro/oa/streams/tasks/clusteranalyzers/__init__.py
 src/mlpro/oa/streams/tasks/clusteranalyzers/basics.py
 src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/__init__.py
 src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/basics.py
 src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/centroid.py
+src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/properties/__init__.py
+src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/properties/basics.py
+src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/properties/centroid.py
 src/mlpro/oa/streams/workflows/__init__.py
 src/mlpro/oa/systems/__init__.py
 src/mlpro/oa/systems/basics.py
 src/mlpro/oa/systems/pool/__init__.py
 src/mlpro/oa/systems/pool/doublependulum.py
 src/mlpro/rl/__init__.py
 src/mlpro/rl/models.py
```

### Comparing `mlpro-1.4.0/test/test_buffer.py` & `mlpro-1.4.1/test/test_buffer.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/test/test_environment.py` & `mlpro-1.4.1/test/test_environment.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/test/test_examples.py` & `mlpro-1.4.1/test/test_examples.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/test/test_math.py` & `mlpro-1.4.1/test/test_math.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/test/test_pool_policies.py` & `mlpro-1.4.1/test/test_pool_policies.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.0/test/test_various.py` & `mlpro-1.4.1/test/test_various.py`

 * *Files identical despite different names*

