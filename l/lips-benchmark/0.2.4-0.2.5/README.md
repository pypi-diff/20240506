# Comparing `tmp/lips-benchmark-0.2.4.tar.gz` & `tmp/lips-benchmark-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lips-benchmark-0.2.4.tar", last modified: Sat Apr 27 22:11:13 2024, max compression
+gzip compressed data, was "lips-benchmark-0.2.5.tar", last modified: Mon May  6 21:08:22 2024, max compression
```

## Comparing `lips-benchmark-0.2.4.tar` & `lips-benchmark-0.2.5.tar`

### file list

```diff
@@ -1,152 +1,152 @@
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-27 22:11:13.385577 lips-benchmark-0.2.4/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    14980 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/LICENSE
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      252 2023-12-13 18:16:50.000000 lips-benchmark-0.2.4/MANIFEST.in
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    17220 2024-04-27 22:11:13.385577 lips-benchmark-0.2.4/PKG-INFO
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    16185 2024-04-27 22:09:51.000000 lips-benchmark-0.2.4/README.md
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-27 22:11:12.773590 lips-benchmark-0.2.4/configurations/
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-27 22:11:12.773590 lips-benchmark-0.2.4/configurations/airfoil/
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-27 22:11:12.789589 lips-benchmark-0.2.4/configurations/airfoil/benchmarks/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      817 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/configurations/airfoil/benchmarks/confAirfoil.ini
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-27 22:11:12.789589 lips-benchmark-0.2.4/configurations/airfoil/simulators/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      514 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/configurations/airfoil/simulators/tf_fc.ini
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      495 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/configurations/airfoil/simulators/torch_fc.ini
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-27 22:11:12.793589 lips-benchmark-0.2.4/configurations/pneumatic/
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-27 22:11:12.793589 lips-benchmark-0.2.4/configurations/pneumatic/benchmarks/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     5383 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/configurations/pneumatic/benchmarks/confWheel.ini
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)       84 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/configurations/pneumatic/readme.md
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-27 22:11:12.793589 lips-benchmark-0.2.4/configurations/pneumatic/simulators/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1959 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/configurations/pneumatic/simulators/torch_fc.ini
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      385 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/configurations/pneumatic/simulators/torch_unet.ini
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-27 22:11:12.793589 lips-benchmark-0.2.4/configurations/powergrid/
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-27 22:11:12.801589 lips-benchmark-0.2.4/configurations/powergrid/benchmarks/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)  4397595 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/configurations/powergrid/benchmarks/Create_Unitary_Actions_LIPS_Benchmark_L2RPN_Neurips.ipynb
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)   563174 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/configurations/powergrid/benchmarks/Create_Unitary_Actions_LIPS_Benchmark_L2RPN_Sandbox.ipynb
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)   901428 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/configurations/powergrid/benchmarks/Create_Unitary_Actions_LIPS_Benchmark_L2RPN_WCCI_2022.ipynb
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     2168 2024-04-18 13:19:41.000000 lips-benchmark-0.2.4/configurations/powergrid/benchmarks/fine_tuning.ini
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    13713 2024-04-26 09:33:21.000000 lips-benchmark-0.2.4/configurations/powergrid/benchmarks/l2rpn_case14_sandbox.ini
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    15575 2024-04-26 09:33:21.000000 lips-benchmark-0.2.4/configurations/powergrid/benchmarks/l2rpn_idf_2023.ini
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    16794 2024-04-26 09:33:21.000000 lips-benchmark-0.2.4/configurations/powergrid/benchmarks/l2rpn_neurips_2020_track1_small.ini
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    13277 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/configurations/powergrid/benchmarks/l2rpn_wcci_2022.ini
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)       96 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/configurations/powergrid/readme.md
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-27 22:11:12.805589 lips-benchmark-0.2.4/configurations/powergrid/simulators/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      502 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/configurations/powergrid/simulators/tf_fc.ini
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      753 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/configurations/powergrid/simulators/tf_leapnet.ini
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      514 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/configurations/powergrid/simulators/torch_fc.ini
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     4294 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/configurations/powergrid/simulators/torch_gnn.ini
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-27 22:11:12.809589 lips-benchmark-0.2.4/lips/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1099 2024-04-27 22:09:51.000000 lips-benchmark-0.2.4/lips/__init__.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-27 22:11:12.849588 lips-benchmark-0.2.4/lips/augmented_simulators/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      804 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/augmented_simulators/__init__.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     4454 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/augmented_simulators/augmented_simulator.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     4678 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/augmented_simulators/hyperParameterTuner.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-27 22:11:12.861588 lips-benchmark-0.2.4/lips/augmented_simulators/tensorflow_models/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      724 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/augmented_simulators/tensorflow_models/__init__.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-27 22:11:12.873588 lips-benchmark-0.2.4/lips/augmented_simulators/tensorflow_models/airfoil/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      587 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/augmented_simulators/tensorflow_models/airfoil/__init__.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     4149 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/augmented_simulators/tensorflow_models/airfoil/fully_connected.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     7947 2024-04-18 13:19:41.000000 lips-benchmark-0.2.4/lips/augmented_simulators/tensorflow_models/fully_connected.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-27 22:11:12.917587 lips-benchmark-0.2.4/lips/augmented_simulators/tensorflow_models/powergrid/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      705 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/augmented_simulators/tensorflow_models/powergrid/__init__.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     3653 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/augmented_simulators/tensorflow_models/powergrid/fully_connected.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    12493 2024-04-18 13:19:41.000000 lips-benchmark-0.2.4/lips/augmented_simulators/tensorflow_models/powergrid/leap_net.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     5600 2024-04-18 13:19:41.000000 lips-benchmark-0.2.4/lips/augmented_simulators/tensorflow_models/powergrid/resnet.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    11374 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/augmented_simulators/tensorflow_models/powergrid/utils.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    13324 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/augmented_simulators/tensorflow_simulator.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-27 22:11:12.973586 lips-benchmark-0.2.4/lips/augmented_simulators/torch_models/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      188 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/augmented_simulators/torch_models/__init__.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    10903 2024-04-18 13:19:41.000000 lips-benchmark-0.2.4/lips/augmented_simulators/torch_models/fully_connected.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    16278 2024-01-04 10:17:47.000000 lips-benchmark-0.2.4/lips/augmented_simulators/torch_models/gnn.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    14260 2024-01-04 10:17:47.000000 lips-benchmark-0.2.4/lips/augmented_simulators/torch_models/gnn_powergrid_utils.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    15899 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/augmented_simulators/torch_models/u_net.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     5411 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/augmented_simulators/torch_models/utils.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    20434 2024-04-18 13:19:41.000000 lips-benchmark-0.2.4/lips/augmented_simulators/torch_simulator.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-27 22:11:13.017585 lips-benchmark-0.2.4/lips/benchmark/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      516 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/benchmark/__init__.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    14302 2024-04-18 13:19:41.000000 lips-benchmark-0.2.4/lips/benchmark/airfransBenchmark.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     7009 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/benchmark/benchmark.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    24021 2024-04-18 13:19:41.000000 lips-benchmark-0.2.4/lips/benchmark/powergridBenchmark.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    32452 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/benchmark/wheelBenchmark.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-27 22:11:13.033584 lips-benchmark-0.2.4/lips/config/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      579 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/config/__init__.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     5627 2024-01-04 10:17:47.000000 lips-benchmark-0.2.4/lips/config/configmanager.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-27 22:11:13.089583 lips-benchmark-0.2.4/lips/dataset/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      752 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/dataset/__init__.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    13145 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/dataset/airfransDataSet.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     5881 2024-04-18 13:19:41.000000 lips-benchmark-0.2.4/lips/dataset/dataSet.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    39804 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/dataset/pneumaticWheelDataSet.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    29814 2024-04-18 13:19:41.000000 lips-benchmark-0.2.4/lips/dataset/powergridDataSet.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     6342 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/dataset/sampler.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-27 22:11:13.145582 lips-benchmark-0.2.4/lips/dataset/scaler/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      259 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/dataset/scaler/__init__.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    10324 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/dataset/scaler/powergrid_scaler.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     4176 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/dataset/scaler/rolling_scaler.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      419 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/dataset/scaler/scaler.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     3412 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/dataset/scaler/standard_scaler.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     4404 2024-04-18 13:19:41.000000 lips-benchmark-0.2.4/lips/dataset/scaler/standard_scaler_iterative.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     7630 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/dataset/scaler/standard_scaler_per_channel.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-27 22:11:13.161582 lips-benchmark-0.2.4/lips/dataset/utils/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      453 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/dataset/utils/__init__.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    25342 2024-04-18 13:19:41.000000 lips-benchmark-0.2.4/lips/dataset/utils/powergrid_utils.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-27 22:11:13.209581 lips-benchmark-0.2.4/lips/evaluation/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      742 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/evaluation/__init__.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    12403 2024-04-18 13:19:41.000000 lips-benchmark-0.2.4/lips/evaluation/airfrans_evaluation.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     4968 2024-01-04 10:17:47.000000 lips-benchmark-0.2.4/lips/evaluation/evaluation.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     8952 2024-01-04 10:17:47.000000 lips-benchmark-0.2.4/lips/evaluation/pneumatic_evaluation.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    10018 2024-01-04 10:17:47.000000 lips-benchmark-0.2.4/lips/evaluation/powergrid_evaluation.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1713 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/evaluation/utils.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-27 22:11:13.221581 lips-benchmark-0.2.4/lips/logger/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      522 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/logger/__init__.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1497 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/logger/customLogger.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-27 22:11:13.225581 lips-benchmark-0.2.4/lips/metrics/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      443 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/metrics/__init__.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-27 22:11:13.261580 lips-benchmark-0.2.4/lips/metrics/ml_metrics/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/metrics/ml_metrics/__init__.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1661 2024-04-26 09:33:21.000000 lips-benchmark-0.2.4/lips/metrics/ml_metrics/external_metrics.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     2022 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/metrics/ml_metrics/mean_absolute_error.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     2312 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/metrics/ml_metrics/mean_absolute_percentage_error.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     2259 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/metrics/ml_metrics/mean_squared_error.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1737 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/metrics/ml_metrics/metrics.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     3124 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/metrics/ml_metrics/normalized_mean_squared_error.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-27 22:11:13.313579 lips-benchmark-0.2.4/lips/metrics/power_grid/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1231 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/metrics/power_grid/__init__.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     4252 2024-04-18 13:19:41.000000 lips-benchmark-0.2.4/lips/metrics/power_grid/compute_solver_time.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     3736 2024-04-18 13:19:41.000000 lips-benchmark-0.2.4/lips/metrics/power_grid/compute_solver_time_grid2op.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     3512 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/metrics/power_grid/global_conservation.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     5147 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/metrics/power_grid/joule_law.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    12945 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/metrics/power_grid/kirchhoff_law.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     5784 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/metrics/power_grid/local_conservation.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    11086 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/metrics/power_grid/ohm_law.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    13878 2024-04-18 13:19:41.000000 lips-benchmark-0.2.4/lips/metrics/power_grid/physics_compliances.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    10285 2024-04-27 22:09:51.000000 lips-benchmark-0.2.4/lips/metrics/power_grid/verify_voltage_equality.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-27 22:11:13.353578 lips-benchmark-0.2.4/lips/physical_simulator/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1092 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/physical_simulator/__init__.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     7878 2024-04-18 13:19:41.000000 lips-benchmark-0.2.4/lips/physical_simulator/dcApproximationAS.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     8358 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/physical_simulator/getfemSimulator.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    13657 2024-04-18 13:19:41.000000 lips-benchmark-0.2.4/lips/physical_simulator/grid2opSimulator.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1934 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/physical_simulator/physicalSimulator.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1912 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/physical_simulator/physicsSolver.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-27 22:11:13.357578 lips-benchmark-0.2.4/lips/plot/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      453 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/plot/__init__.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-27 22:11:13.373577 lips-benchmark-0.2.4/lips/plot/power_grid/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      604 2024-04-18 13:19:41.000000 lips-benchmark-0.2.4/lips/plot/power_grid/__init__.py
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     6097 2024-04-18 13:19:41.000000 lips-benchmark-0.2.4/lips/plot/power_grid/plotting.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-27 22:11:12.777590 lips-benchmark-0.2.4/lips/tests/
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-27 22:11:12.777590 lips-benchmark-0.2.4/lips/tests/configs/
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-27 22:11:12.777590 lips-benchmark-0.2.4/lips/tests/configs/powergrid/
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-27 22:11:13.373577 lips-benchmark-0.2.4/lips/tests/configs/powergrid/benchmarks/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    11499 2024-01-04 10:17:47.000000 lips-benchmark-0.2.4/lips/tests/configs/powergrid/benchmarks/l2rpn_case14_sandbox.ini
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    15575 2024-01-04 10:17:47.000000 lips-benchmark-0.2.4/lips/tests/configs/powergrid/benchmarks/l2rpn_neurips_2020_track1_small.ini
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-27 22:11:13.377577 lips-benchmark-0.2.4/lips/tests/configs/powergrid/simulators/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      502 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/tests/configs/powergrid/simulators/tf_fc.ini
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      753 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/tests/configs/powergrid/simulators/tf_leapnet.ini
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      514 2023-12-12 21:47:49.000000 lips-benchmark-0.2.4/lips/tests/configs/powergrid/simulators/torch_fc.ini
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1395 2023-12-12 21:47:50.000000 lips-benchmark-0.2.4/lips/utils.py
-drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-04-27 22:11:13.385577 lips-benchmark-0.2.4/lips_benchmark.egg-info/
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    17220 2024-04-27 22:11:11.000000 lips-benchmark-0.2.4/lips_benchmark.egg-info/PKG-INFO
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     4995 2024-04-27 22:11:12.000000 lips-benchmark-0.2.4/lips_benchmark.egg-info/SOURCES.txt
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        1 2024-04-27 22:11:11.000000 lips-benchmark-0.2.4/lips_benchmark.egg-info/dependency_links.txt
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        1 2024-04-26 14:11:45.000000 lips-benchmark-0.2.4/lips_benchmark.egg-info/not-zip-safe
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1134 2024-04-27 22:11:11.000000 lips-benchmark-0.2.4/lips_benchmark.egg-info/requires.txt
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        5 2024-04-27 22:11:11.000000 lips-benchmark-0.2.4/lips_benchmark.egg-info/top_level.txt
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      563 2024-04-27 22:11:13.389577 lips-benchmark-0.2.4/setup.cfg
--rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     4005 2024-04-27 22:09:51.000000 lips-benchmark-0.2.4/setup.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-05-06 21:08:22.038752 lips-benchmark-0.2.5/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    14980 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/LICENSE
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      252 2023-12-13 18:16:50.000000 lips-benchmark-0.2.5/MANIFEST.in
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    21282 2024-05-06 21:08:22.038752 lips-benchmark-0.2.5/PKG-INFO
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    16185 2024-04-27 22:09:51.000000 lips-benchmark-0.2.5/README.md
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-05-06 21:08:21.598761 lips-benchmark-0.2.5/configurations/
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-05-06 21:08:21.598761 lips-benchmark-0.2.5/configurations/airfoil/
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-05-06 21:08:21.606761 lips-benchmark-0.2.5/configurations/airfoil/benchmarks/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      817 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/configurations/airfoil/benchmarks/confAirfoil.ini
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-05-06 21:08:21.610761 lips-benchmark-0.2.5/configurations/airfoil/simulators/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      514 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/configurations/airfoil/simulators/tf_fc.ini
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      495 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/configurations/airfoil/simulators/torch_fc.ini
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-05-06 21:08:21.610761 lips-benchmark-0.2.5/configurations/pneumatic/
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-05-06 21:08:21.610761 lips-benchmark-0.2.5/configurations/pneumatic/benchmarks/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     5383 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/configurations/pneumatic/benchmarks/confWheel.ini
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)       84 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/configurations/pneumatic/readme.md
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-05-06 21:08:21.610761 lips-benchmark-0.2.5/configurations/pneumatic/simulators/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1959 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/configurations/pneumatic/simulators/torch_fc.ini
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      385 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/configurations/pneumatic/simulators/torch_unet.ini
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-05-06 21:08:21.610761 lips-benchmark-0.2.5/configurations/powergrid/
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-05-06 21:08:21.622761 lips-benchmark-0.2.5/configurations/powergrid/benchmarks/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)  4397595 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/configurations/powergrid/benchmarks/Create_Unitary_Actions_LIPS_Benchmark_L2RPN_Neurips.ipynb
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)   563174 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/configurations/powergrid/benchmarks/Create_Unitary_Actions_LIPS_Benchmark_L2RPN_Sandbox.ipynb
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)   901428 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/configurations/powergrid/benchmarks/Create_Unitary_Actions_LIPS_Benchmark_L2RPN_WCCI_2022.ipynb
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     2168 2024-04-18 13:19:41.000000 lips-benchmark-0.2.5/configurations/powergrid/benchmarks/fine_tuning.ini
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    13713 2024-04-26 09:33:21.000000 lips-benchmark-0.2.5/configurations/powergrid/benchmarks/l2rpn_case14_sandbox.ini
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    15575 2024-04-26 09:33:21.000000 lips-benchmark-0.2.5/configurations/powergrid/benchmarks/l2rpn_idf_2023.ini
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    16794 2024-04-26 09:33:21.000000 lips-benchmark-0.2.5/configurations/powergrid/benchmarks/l2rpn_neurips_2020_track1_small.ini
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    13277 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/configurations/powergrid/benchmarks/l2rpn_wcci_2022.ini
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)       96 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/configurations/powergrid/readme.md
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-05-06 21:08:21.622761 lips-benchmark-0.2.5/configurations/powergrid/simulators/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      502 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/configurations/powergrid/simulators/tf_fc.ini
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      753 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/configurations/powergrid/simulators/tf_leapnet.ini
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      514 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/configurations/powergrid/simulators/torch_fc.ini
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     4294 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/configurations/powergrid/simulators/torch_gnn.ini
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-05-06 21:08:21.630760 lips-benchmark-0.2.5/lips/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1099 2024-05-06 21:08:05.000000 lips-benchmark-0.2.5/lips/__init__.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-05-06 21:08:21.658760 lips-benchmark-0.2.5/lips/augmented_simulators/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      804 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/augmented_simulators/__init__.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     4454 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/augmented_simulators/augmented_simulator.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     4678 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/augmented_simulators/hyperParameterTuner.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-05-06 21:08:21.666760 lips-benchmark-0.2.5/lips/augmented_simulators/tensorflow_models/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      724 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/augmented_simulators/tensorflow_models/__init__.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-05-06 21:08:21.674759 lips-benchmark-0.2.5/lips/augmented_simulators/tensorflow_models/airfoil/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      587 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/augmented_simulators/tensorflow_models/airfoil/__init__.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     4149 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/augmented_simulators/tensorflow_models/airfoil/fully_connected.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     7947 2024-04-18 13:19:41.000000 lips-benchmark-0.2.5/lips/augmented_simulators/tensorflow_models/fully_connected.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-05-06 21:08:21.702759 lips-benchmark-0.2.5/lips/augmented_simulators/tensorflow_models/powergrid/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      705 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/augmented_simulators/tensorflow_models/powergrid/__init__.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     3653 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/augmented_simulators/tensorflow_models/powergrid/fully_connected.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    12493 2024-04-18 13:19:41.000000 lips-benchmark-0.2.5/lips/augmented_simulators/tensorflow_models/powergrid/leap_net.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     5600 2024-04-18 13:19:41.000000 lips-benchmark-0.2.5/lips/augmented_simulators/tensorflow_models/powergrid/resnet.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    11374 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/augmented_simulators/tensorflow_models/powergrid/utils.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    13324 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/augmented_simulators/tensorflow_simulator.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-05-06 21:08:21.734758 lips-benchmark-0.2.5/lips/augmented_simulators/torch_models/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      188 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/augmented_simulators/torch_models/__init__.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    10903 2024-04-18 13:19:41.000000 lips-benchmark-0.2.5/lips/augmented_simulators/torch_models/fully_connected.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    16278 2024-01-04 10:17:47.000000 lips-benchmark-0.2.5/lips/augmented_simulators/torch_models/gnn.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    14260 2024-01-04 10:17:47.000000 lips-benchmark-0.2.5/lips/augmented_simulators/torch_models/gnn_powergrid_utils.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    15899 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/augmented_simulators/torch_models/u_net.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     5411 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/augmented_simulators/torch_models/utils.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    20434 2024-04-18 13:19:41.000000 lips-benchmark-0.2.5/lips/augmented_simulators/torch_simulator.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-05-06 21:08:21.762758 lips-benchmark-0.2.5/lips/benchmark/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      516 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/benchmark/__init__.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    14302 2024-04-18 13:19:41.000000 lips-benchmark-0.2.5/lips/benchmark/airfransBenchmark.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     7009 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/benchmark/benchmark.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    24021 2024-04-18 13:19:41.000000 lips-benchmark-0.2.5/lips/benchmark/powergridBenchmark.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    32452 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/benchmark/wheelBenchmark.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-05-06 21:08:21.770758 lips-benchmark-0.2.5/lips/config/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      579 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/config/__init__.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     5627 2024-01-04 10:17:47.000000 lips-benchmark-0.2.5/lips/config/configmanager.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-05-06 21:08:21.802757 lips-benchmark-0.2.5/lips/dataset/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      752 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/dataset/__init__.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    13145 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/dataset/airfransDataSet.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     5881 2024-04-18 13:19:41.000000 lips-benchmark-0.2.5/lips/dataset/dataSet.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    39804 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/dataset/pneumaticWheelDataSet.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    29814 2024-04-18 13:19:41.000000 lips-benchmark-0.2.5/lips/dataset/powergridDataSet.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     6342 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/dataset/sampler.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-05-06 21:08:21.838756 lips-benchmark-0.2.5/lips/dataset/scaler/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      259 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/dataset/scaler/__init__.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    10324 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/dataset/scaler/powergrid_scaler.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     4176 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/dataset/scaler/rolling_scaler.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      419 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/dataset/scaler/scaler.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     3412 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/dataset/scaler/standard_scaler.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     4404 2024-04-18 13:19:41.000000 lips-benchmark-0.2.5/lips/dataset/scaler/standard_scaler_iterative.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     7630 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/dataset/scaler/standard_scaler_per_channel.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-05-06 21:08:21.846756 lips-benchmark-0.2.5/lips/dataset/utils/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      453 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/dataset/utils/__init__.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    25342 2024-04-18 13:19:41.000000 lips-benchmark-0.2.5/lips/dataset/utils/powergrid_utils.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-05-06 21:08:21.874755 lips-benchmark-0.2.5/lips/evaluation/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      742 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/evaluation/__init__.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    12403 2024-04-18 13:19:41.000000 lips-benchmark-0.2.5/lips/evaluation/airfrans_evaluation.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     4968 2024-01-04 10:17:47.000000 lips-benchmark-0.2.5/lips/evaluation/evaluation.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     8952 2024-01-04 10:17:47.000000 lips-benchmark-0.2.5/lips/evaluation/pneumatic_evaluation.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    10018 2024-01-04 10:17:47.000000 lips-benchmark-0.2.5/lips/evaluation/powergrid_evaluation.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1713 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/evaluation/utils.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-05-06 21:08:21.882755 lips-benchmark-0.2.5/lips/logger/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      522 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/logger/__init__.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1497 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/logger/customLogger.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-05-06 21:08:21.882755 lips-benchmark-0.2.5/lips/metrics/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      443 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/metrics/__init__.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-05-06 21:08:21.906755 lips-benchmark-0.2.5/lips/metrics/ml_metrics/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/metrics/ml_metrics/__init__.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1661 2024-04-26 09:33:21.000000 lips-benchmark-0.2.5/lips/metrics/ml_metrics/external_metrics.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     2022 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/metrics/ml_metrics/mean_absolute_error.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     2312 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/metrics/ml_metrics/mean_absolute_percentage_error.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     2259 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/metrics/ml_metrics/mean_squared_error.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1737 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/metrics/ml_metrics/metrics.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     3124 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/metrics/ml_metrics/normalized_mean_squared_error.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-05-06 21:08:21.954754 lips-benchmark-0.2.5/lips/metrics/power_grid/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1231 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/metrics/power_grid/__init__.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     4252 2024-04-18 13:19:41.000000 lips-benchmark-0.2.5/lips/metrics/power_grid/compute_solver_time.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     3736 2024-04-18 13:19:41.000000 lips-benchmark-0.2.5/lips/metrics/power_grid/compute_solver_time_grid2op.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     3512 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/metrics/power_grid/global_conservation.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     5147 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/metrics/power_grid/joule_law.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    12945 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/metrics/power_grid/kirchhoff_law.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     5784 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/metrics/power_grid/local_conservation.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    11086 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/metrics/power_grid/ohm_law.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    13878 2024-04-18 13:19:41.000000 lips-benchmark-0.2.5/lips/metrics/power_grid/physics_compliances.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    10285 2024-04-27 22:09:51.000000 lips-benchmark-0.2.5/lips/metrics/power_grid/verify_voltage_equality.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-05-06 21:08:21.982753 lips-benchmark-0.2.5/lips/physical_simulator/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1092 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/physical_simulator/__init__.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     7878 2024-04-18 13:19:41.000000 lips-benchmark-0.2.5/lips/physical_simulator/dcApproximationAS.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     8358 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/physical_simulator/getfemSimulator.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    13657 2024-04-18 13:19:41.000000 lips-benchmark-0.2.5/lips/physical_simulator/grid2opSimulator.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1934 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/physical_simulator/physicalSimulator.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1912 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/physical_simulator/physicsSolver.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-05-06 21:08:21.986753 lips-benchmark-0.2.5/lips/plot/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      453 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/plot/__init__.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-05-06 21:08:21.998753 lips-benchmark-0.2.5/lips/plot/power_grid/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      604 2024-04-18 13:19:41.000000 lips-benchmark-0.2.5/lips/plot/power_grid/__init__.py
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     6097 2024-04-18 13:19:41.000000 lips-benchmark-0.2.5/lips/plot/power_grid/plotting.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-05-06 21:08:21.598761 lips-benchmark-0.2.5/lips/tests/
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-05-06 21:08:21.598761 lips-benchmark-0.2.5/lips/tests/configs/
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-05-06 21:08:21.602761 lips-benchmark-0.2.5/lips/tests/configs/powergrid/
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-05-06 21:08:22.002753 lips-benchmark-0.2.5/lips/tests/configs/powergrid/benchmarks/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    11499 2024-01-04 10:17:47.000000 lips-benchmark-0.2.5/lips/tests/configs/powergrid/benchmarks/l2rpn_case14_sandbox.ini
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    15575 2024-01-04 10:17:47.000000 lips-benchmark-0.2.5/lips/tests/configs/powergrid/benchmarks/l2rpn_neurips_2020_track1_small.ini
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-05-06 21:08:22.006753 lips-benchmark-0.2.5/lips/tests/configs/powergrid/simulators/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      502 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/tests/configs/powergrid/simulators/tf_fc.ini
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      753 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/tests/configs/powergrid/simulators/tf_leapnet.ini
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      514 2023-12-12 21:47:49.000000 lips-benchmark-0.2.5/lips/tests/configs/powergrid/simulators/torch_fc.ini
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1395 2023-12-12 21:47:50.000000 lips-benchmark-0.2.5/lips/utils.py
+drwxr-xr-x   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        0 2024-05-06 21:08:22.026752 lips-benchmark-0.2.5/lips_benchmark.egg-info/
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)    21282 2024-05-06 21:08:20.000000 lips-benchmark-0.2.5/lips_benchmark.egg-info/PKG-INFO
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     4995 2024-05-06 21:08:21.000000 lips-benchmark-0.2.5/lips_benchmark.egg-info/SOURCES.txt
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        1 2024-05-06 21:08:20.000000 lips-benchmark-0.2.5/lips_benchmark.egg-info/dependency_links.txt
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        1 2024-04-26 14:11:45.000000 lips-benchmark-0.2.5/lips_benchmark.egg-info/not-zip-safe
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     1134 2024-05-06 21:08:20.000000 lips-benchmark-0.2.5/lips_benchmark.egg-info/requires.txt
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)        5 2024-05-06 21:08:20.000000 lips-benchmark-0.2.5/lips_benchmark.egg-info/top_level.txt
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)      563 2024-05-06 21:08:22.046752 lips-benchmark-0.2.5/setup.cfg
+-rw-r--r--   0 milad.leyli-abadi (1658205013) utilisateurs du domaine (1658200513)     3977 2024-05-06 21:08:05.000000 lips-benchmark-0.2.5/setup.py
```

### Comparing `lips-benchmark-0.2.4/LICENSE` & `lips-benchmark-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/PKG-INFO` & `lips-benchmark-0.2.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,7 @@
-Metadata-Version: 2.1
-Name: lips-benchmark
-Version: 0.2.4
-Summary: LIPS : Learning Industrial Physical Simulation benchmark suite
-Home-page: https://github.com/IRT-SystemX/LIPS
-Author: Milad Leyli-abadi
-Author-email: milad.leyli-abadi@irt-systemx.fr
-License: MPL
-Keywords: Physical system solver,augmented simulator,benchmarking
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Natural Language :: English
-Description-Content-Type: text/markdown
-Provides-Extra: recommended
-Provides-Extra: docs
-Provides-Extra: codabench
-Provides-Extra: test
-License-File: LICENSE
-
 # LIPS - Learning Industrial Physical Simulation benchmark suite
 
 This repository implements LIPS benchmarking platform. 
 <!---
 and provides the necessary utilities to reproduce the generated datasets used in research.
 --->
```

### Comparing `lips-benchmark-0.2.4/configurations/airfoil/benchmarks/confAirfoil.ini` & `lips-benchmark-0.2.5/configurations/airfoil/benchmarks/confAirfoil.ini`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/configurations/airfoil/simulators/tf_fc.ini` & `lips-benchmark-0.2.5/configurations/airfoil/simulators/tf_fc.ini`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/configurations/pneumatic/benchmarks/confWheel.ini` & `lips-benchmark-0.2.5/configurations/pneumatic/benchmarks/confWheel.ini`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/configurations/pneumatic/simulators/torch_fc.ini` & `lips-benchmark-0.2.5/configurations/pneumatic/simulators/torch_fc.ini`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/configurations/powergrid/benchmarks/Create_Unitary_Actions_LIPS_Benchmark_L2RPN_Neurips.ipynb` & `lips-benchmark-0.2.5/configurations/powergrid/benchmarks/Create_Unitary_Actions_LIPS_Benchmark_L2RPN_Neurips.ipynb`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/configurations/powergrid/benchmarks/Create_Unitary_Actions_LIPS_Benchmark_L2RPN_Sandbox.ipynb` & `lips-benchmark-0.2.5/configurations/powergrid/benchmarks/Create_Unitary_Actions_LIPS_Benchmark_L2RPN_Sandbox.ipynb`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/configurations/powergrid/benchmarks/Create_Unitary_Actions_LIPS_Benchmark_L2RPN_WCCI_2022.ipynb` & `lips-benchmark-0.2.5/configurations/powergrid/benchmarks/Create_Unitary_Actions_LIPS_Benchmark_L2RPN_WCCI_2022.ipynb`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/configurations/powergrid/benchmarks/fine_tuning.ini` & `lips-benchmark-0.2.5/configurations/powergrid/benchmarks/fine_tuning.ini`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/configurations/powergrid/benchmarks/l2rpn_case14_sandbox.ini` & `lips-benchmark-0.2.5/configurations/powergrid/benchmarks/l2rpn_case14_sandbox.ini`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/configurations/powergrid/benchmarks/l2rpn_idf_2023.ini` & `lips-benchmark-0.2.5/configurations/powergrid/benchmarks/l2rpn_idf_2023.ini`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/configurations/powergrid/benchmarks/l2rpn_neurips_2020_track1_small.ini` & `lips-benchmark-0.2.5/configurations/powergrid/benchmarks/l2rpn_neurips_2020_track1_small.ini`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/configurations/powergrid/benchmarks/l2rpn_wcci_2022.ini` & `lips-benchmark-0.2.5/configurations/powergrid/benchmarks/l2rpn_wcci_2022.ini`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/configurations/powergrid/simulators/tf_leapnet.ini` & `lips-benchmark-0.2.5/configurations/powergrid/simulators/tf_leapnet.ini`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/configurations/powergrid/simulators/torch_fc.ini` & `lips-benchmark-0.2.5/configurations/powergrid/simulators/torch_fc.ini`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/configurations/powergrid/simulators/torch_gnn.ini` & `lips-benchmark-0.2.5/configurations/powergrid/simulators/torch_gnn.ini`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/__init__.py` & `lips-benchmark-0.2.5/lips/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This Source Code Form is subject to the terms of the Mozilla Public License, version 2.0.
 # If a copy of the Mozilla Public License, version 2.0 was not distributed with this file,
 # you can obtain one at http://mozilla.org/MPL/2.0/.
 # SPDX-License-Identifier: MPL-2.0
 # This file is part of LIPS, LIPS is a python platform for power networks benchmarking
 import pathlib
 
-__version__ = "0.2.4"
+__version__ = "0.2.5"
 
 here = pathlib.Path(__file__).parent.resolve()
 
 def get_version(rel_path="__init__.py"):
     init_content = (here / rel_path).read_text(encoding='utf-8')
     for line in init_content.split('\n'):
         if line.startswith('__version__'):
```

### Comparing `lips-benchmark-0.2.4/lips/augmented_simulators/__init__.py` & `lips-benchmark-0.2.5/lips/augmented_simulators/__init__.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/augmented_simulators/augmented_simulator.py` & `lips-benchmark-0.2.5/lips/augmented_simulators/augmented_simulator.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/augmented_simulators/hyperParameterTuner.py` & `lips-benchmark-0.2.5/lips/augmented_simulators/hyperParameterTuner.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/augmented_simulators/tensorflow_models/__init__.py` & `lips-benchmark-0.2.5/lips/augmented_simulators/tensorflow_models/__init__.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/augmented_simulators/tensorflow_models/airfoil/__init__.py` & `lips-benchmark-0.2.5/lips/augmented_simulators/tensorflow_models/airfoil/__init__.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/augmented_simulators/tensorflow_models/airfoil/fully_connected.py` & `lips-benchmark-0.2.5/lips/augmented_simulators/tensorflow_models/airfoil/fully_connected.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/augmented_simulators/tensorflow_models/fully_connected.py` & `lips-benchmark-0.2.5/lips/augmented_simulators/tensorflow_models/fully_connected.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/augmented_simulators/tensorflow_models/powergrid/__init__.py` & `lips-benchmark-0.2.5/lips/augmented_simulators/tensorflow_models/powergrid/__init__.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/augmented_simulators/tensorflow_models/powergrid/fully_connected.py` & `lips-benchmark-0.2.5/lips/augmented_simulators/tensorflow_models/powergrid/fully_connected.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/augmented_simulators/tensorflow_models/powergrid/leap_net.py` & `lips-benchmark-0.2.5/lips/augmented_simulators/tensorflow_models/powergrid/leap_net.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/augmented_simulators/tensorflow_models/powergrid/resnet.py` & `lips-benchmark-0.2.5/lips/augmented_simulators/tensorflow_models/powergrid/resnet.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/augmented_simulators/tensorflow_models/powergrid/utils.py` & `lips-benchmark-0.2.5/lips/augmented_simulators/tensorflow_models/powergrid/utils.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/augmented_simulators/tensorflow_simulator.py` & `lips-benchmark-0.2.5/lips/augmented_simulators/tensorflow_simulator.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/augmented_simulators/torch_models/fully_connected.py` & `lips-benchmark-0.2.5/lips/augmented_simulators/torch_models/fully_connected.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/augmented_simulators/torch_models/gnn.py` & `lips-benchmark-0.2.5/lips/augmented_simulators/torch_models/gnn.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/augmented_simulators/torch_models/gnn_powergrid_utils.py` & `lips-benchmark-0.2.5/lips/augmented_simulators/torch_models/gnn_powergrid_utils.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/augmented_simulators/torch_models/u_net.py` & `lips-benchmark-0.2.5/lips/augmented_simulators/torch_models/u_net.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/augmented_simulators/torch_models/utils.py` & `lips-benchmark-0.2.5/lips/augmented_simulators/torch_models/utils.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/augmented_simulators/torch_simulator.py` & `lips-benchmark-0.2.5/lips/augmented_simulators/torch_simulator.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/benchmark/__init__.py` & `lips-benchmark-0.2.5/lips/benchmark/__init__.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/benchmark/airfransBenchmark.py` & `lips-benchmark-0.2.5/lips/benchmark/airfransBenchmark.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/benchmark/benchmark.py` & `lips-benchmark-0.2.5/lips/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/benchmark/powergridBenchmark.py` & `lips-benchmark-0.2.5/lips/benchmark/powergridBenchmark.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/benchmark/wheelBenchmark.py` & `lips-benchmark-0.2.5/lips/benchmark/wheelBenchmark.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/config/__init__.py` & `lips-benchmark-0.2.5/lips/config/__init__.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/config/configmanager.py` & `lips-benchmark-0.2.5/lips/config/configmanager.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/dataset/__init__.py` & `lips-benchmark-0.2.5/lips/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/dataset/airfransDataSet.py` & `lips-benchmark-0.2.5/lips/dataset/airfransDataSet.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/dataset/dataSet.py` & `lips-benchmark-0.2.5/lips/dataset/dataSet.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/dataset/pneumaticWheelDataSet.py` & `lips-benchmark-0.2.5/lips/dataset/pneumaticWheelDataSet.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/dataset/powergridDataSet.py` & `lips-benchmark-0.2.5/lips/dataset/powergridDataSet.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/dataset/sampler.py` & `lips-benchmark-0.2.5/lips/dataset/sampler.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/dataset/scaler/powergrid_scaler.py` & `lips-benchmark-0.2.5/lips/dataset/scaler/powergrid_scaler.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/dataset/scaler/rolling_scaler.py` & `lips-benchmark-0.2.5/lips/dataset/scaler/rolling_scaler.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/dataset/scaler/standard_scaler.py` & `lips-benchmark-0.2.5/lips/dataset/scaler/standard_scaler.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/dataset/scaler/standard_scaler_iterative.py` & `lips-benchmark-0.2.5/lips/dataset/scaler/standard_scaler_iterative.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/dataset/scaler/standard_scaler_per_channel.py` & `lips-benchmark-0.2.5/lips/dataset/scaler/standard_scaler_per_channel.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/dataset/utils/powergrid_utils.py` & `lips-benchmark-0.2.5/lips/dataset/utils/powergrid_utils.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/evaluation/__init__.py` & `lips-benchmark-0.2.5/lips/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/evaluation/airfrans_evaluation.py` & `lips-benchmark-0.2.5/lips/evaluation/airfrans_evaluation.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/evaluation/evaluation.py` & `lips-benchmark-0.2.5/lips/evaluation/evaluation.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/evaluation/pneumatic_evaluation.py` & `lips-benchmark-0.2.5/lips/evaluation/pneumatic_evaluation.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/evaluation/powergrid_evaluation.py` & `lips-benchmark-0.2.5/lips/evaluation/powergrid_evaluation.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/evaluation/utils.py` & `lips-benchmark-0.2.5/lips/evaluation/utils.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/logger/__init__.py` & `lips-benchmark-0.2.5/lips/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/logger/customLogger.py` & `lips-benchmark-0.2.5/lips/logger/customLogger.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/metrics/ml_metrics/external_metrics.py` & `lips-benchmark-0.2.5/lips/metrics/ml_metrics/external_metrics.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/metrics/ml_metrics/mean_absolute_error.py` & `lips-benchmark-0.2.5/lips/metrics/ml_metrics/mean_absolute_error.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/metrics/ml_metrics/mean_absolute_percentage_error.py` & `lips-benchmark-0.2.5/lips/metrics/ml_metrics/mean_absolute_percentage_error.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/metrics/ml_metrics/mean_squared_error.py` & `lips-benchmark-0.2.5/lips/metrics/ml_metrics/mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/metrics/ml_metrics/metrics.py` & `lips-benchmark-0.2.5/lips/metrics/ml_metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/metrics/ml_metrics/normalized_mean_squared_error.py` & `lips-benchmark-0.2.5/lips/metrics/ml_metrics/normalized_mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/metrics/power_grid/__init__.py` & `lips-benchmark-0.2.5/lips/metrics/power_grid/__init__.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/metrics/power_grid/compute_solver_time.py` & `lips-benchmark-0.2.5/lips/metrics/power_grid/compute_solver_time.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/metrics/power_grid/compute_solver_time_grid2op.py` & `lips-benchmark-0.2.5/lips/metrics/power_grid/compute_solver_time_grid2op.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/metrics/power_grid/global_conservation.py` & `lips-benchmark-0.2.5/lips/metrics/power_grid/global_conservation.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/metrics/power_grid/joule_law.py` & `lips-benchmark-0.2.5/lips/metrics/power_grid/joule_law.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/metrics/power_grid/kirchhoff_law.py` & `lips-benchmark-0.2.5/lips/metrics/power_grid/kirchhoff_law.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/metrics/power_grid/local_conservation.py` & `lips-benchmark-0.2.5/lips/metrics/power_grid/local_conservation.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/metrics/power_grid/ohm_law.py` & `lips-benchmark-0.2.5/lips/metrics/power_grid/ohm_law.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/metrics/power_grid/physics_compliances.py` & `lips-benchmark-0.2.5/lips/metrics/power_grid/physics_compliances.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/metrics/power_grid/verify_voltage_equality.py` & `lips-benchmark-0.2.5/lips/metrics/power_grid/verify_voltage_equality.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/physical_simulator/__init__.py` & `lips-benchmark-0.2.5/lips/physical_simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/physical_simulator/dcApproximationAS.py` & `lips-benchmark-0.2.5/lips/physical_simulator/dcApproximationAS.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/physical_simulator/getfemSimulator.py` & `lips-benchmark-0.2.5/lips/physical_simulator/getfemSimulator.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/physical_simulator/grid2opSimulator.py` & `lips-benchmark-0.2.5/lips/physical_simulator/grid2opSimulator.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/physical_simulator/physicalSimulator.py` & `lips-benchmark-0.2.5/lips/physical_simulator/physicalSimulator.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/physical_simulator/physicsSolver.py` & `lips-benchmark-0.2.5/lips/physical_simulator/physicsSolver.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/plot/power_grid/__init__.py` & `lips-benchmark-0.2.5/lips/plot/power_grid/__init__.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/plot/power_grid/plotting.py` & `lips-benchmark-0.2.5/lips/plot/power_grid/plotting.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/tests/configs/powergrid/benchmarks/l2rpn_case14_sandbox.ini` & `lips-benchmark-0.2.5/lips/tests/configs/powergrid/benchmarks/l2rpn_case14_sandbox.ini`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/tests/configs/powergrid/benchmarks/l2rpn_neurips_2020_track1_small.ini` & `lips-benchmark-0.2.5/lips/tests/configs/powergrid/benchmarks/l2rpn_neurips_2020_track1_small.ini`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/tests/configs/powergrid/simulators/tf_leapnet.ini` & `lips-benchmark-0.2.5/lips/tests/configs/powergrid/simulators/tf_leapnet.ini`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/tests/configs/powergrid/simulators/torch_fc.ini` & `lips-benchmark-0.2.5/lips/tests/configs/powergrid/simulators/torch_fc.ini`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips/utils.py` & `lips-benchmark-0.2.5/lips/utils.py`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips_benchmark.egg-info/SOURCES.txt` & `lips-benchmark-0.2.5/lips_benchmark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/lips_benchmark.egg-info/requires.txt` & `lips-benchmark-0.2.5/lips_benchmark.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 filelock==3.7.1
 json2table==1.1.5
 loguru==0.6.0
 PyYAML==6.0
 tqdm==4.62.3
 grid2op==1.9.8
 pybind11==2.8.1
-lightsim2grid==0.7.5
+lightsim2grid==0.8.1
 leap-net==0.0.5
 protobuf==3.20.2
 pandapower==2.8.0
 pandas==1.5.3
 jupyter
 tensorflow==2.8.1
 torch==2.0.1
@@ -33,15 +33,15 @@
 sphinxcontrib-trio>=1.1.0
 autodocsumm>=0.1.13
 gym>=0.17.2
 
 [recommended]
 grid2op==1.9.8
 pybind11==2.8.1
-lightsim2grid==0.7.5
+lightsim2grid==0.8.1
 leap-net==0.0.5
 protobuf==3.20.2
 pandapower==2.8.0
 pandas==1.5.3
 jupyter
 tensorflow==2.8.1
 torch==2.0.1
@@ -55,15 +55,15 @@
 pytest-metadata
 ipykernel
 pylint
 pylint-exit
 jupytext
 grid2op==1.9.8
 pybind11==2.8.1
-lightsim2grid==0.7.5
+lightsim2grid==0.8.1
 leap-net==0.0.5
 protobuf==3.20.2
 pandapower==2.8.0
 pandas==1.5.3
 jupyter
 tensorflow==2.8.1
 torch==2.0.1
```

### Comparing `lips-benchmark-0.2.4/setup.cfg` & `lips-benchmark-0.2.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `lips-benchmark-0.2.4/setup.py` & `lips-benchmark-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,17 +31,17 @@
         "scipy==1.11.4",
         "six",
         "pathlib",
         "numba",
     ],
     "extras": {
         "recommended": [
-            "grid2op==1.9.8", #>=1.7.2",
+            "grid2op==1.9.8",
             "pybind11==2.8.1",
-            "lightsim2grid==0.7.5", #>=0.7.0.post1",
+            "lightsim2grid==0.8.1",
             "leap-net==0.0.5",
             "protobuf==3.20.2",
             "pandapower==2.8.0",
             "pandas==1.5.3",
             "jupyter",
             "tensorflow==2.8.1",
             "torch==2.0.1",
```

