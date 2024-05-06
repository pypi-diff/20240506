# Comparing `tmp/prodsys-0.6.0.tar.gz` & `tmp/prodsys-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodsys-0.6.0.tar", max compression
+gzip compressed data, was "prodsys-0.6.1.tar", max compression
```

## Comparing `prodsys-0.6.0.tar` & `prodsys-0.6.1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0     1096 2023-10-11 11:05:21.946526 prodsys-0.6.0/LICENSE
--rw-r--r--   0        0        0      405 2024-05-04 14:52:14.089697 prodsys-0.6.0/prodsys/__init__.py
--rw-r--r--   0        0        0     1289 2024-05-01 05:54:38.231436 prodsys-0.6.0/prodsys/adapters/__init__.py
--rw-r--r--   0        0        0    56327 2024-05-04 14:52:14.090345 prodsys-0.6.0/prodsys/adapters/adapter.py
--rw-r--r--   0        0        0     8854 2024-05-04 14:52:14.090345 prodsys-0.6.0/prodsys/adapters/json_adapter.py
--rw-r--r--   0        0        0        0 2024-01-07 23:00:16.874004 prodsys-0.6.0/prodsys/conf/__init__.py
--rw-r--r--   0        0        0     2487 2024-01-07 23:00:16.874004 prodsys-0.6.0/prodsys/conf/logging.ini
--rw-r--r--   0        0        0     1155 2024-01-07 23:00:16.874004 prodsys-0.6.0/prodsys/conf/logging_config.py
--rw-r--r--   0        0        0      148 2023-10-11 11:05:22.073479 prodsys-0.6.0/prodsys/control/__init__.py
--rw-r--r--   0        0        0     9030 2024-05-04 14:52:14.094243 prodsys-0.6.0/prodsys/control/routing_control_env.py
--rw-r--r--   0        0        0     8489 2023-10-11 11:05:22.073479 prodsys-0.6.0/prodsys/control/sequencing_control_env.py
--rw-r--r--   0        0        0     2236 2024-05-04 14:52:14.094243 prodsys-0.6.0/prodsys/express/__init__.py
--rw-r--r--   0        0        0      603 2023-10-11 11:05:22.073479 prodsys-0.6.0/prodsys/express/core.py
--rw-r--r--   0        0        0     1589 2024-05-04 14:52:14.094243 prodsys-0.6.0/prodsys/express/node.py
--rw-r--r--   0        0        0    11649 2024-05-04 14:52:14.098787 prodsys-0.6.0/prodsys/express/process.py
--rw-r--r--   0        0        0     2477 2024-05-04 14:52:14.098787 prodsys-0.6.0/prodsys/express/product.py
--rw-r--r--   0        0        0     7129 2024-05-04 14:52:14.101328 prodsys-0.6.0/prodsys/express/production_system.py
--rw-r--r--   0        0        0     8295 2024-05-04 14:52:14.101328 prodsys-0.6.0/prodsys/express/resources.py
--rw-r--r--   0        0        0     2573 2024-05-04 14:52:14.101328 prodsys-0.6.0/prodsys/express/sink.py
--rw-r--r--   0        0        0     3413 2024-05-04 14:52:14.101328 prodsys-0.6.0/prodsys/express/source.py
--rw-r--r--   0        0        0     7554 2024-05-01 07:15:45.742369 prodsys-0.6.0/prodsys/express/state.py
--rw-r--r--   0        0        0     4884 2024-05-04 14:52:14.101328 prodsys-0.6.0/prodsys/express/time_model.py
--rw-r--r--   0        0        0      913 2023-10-11 11:05:22.089564 prodsys-0.6.0/prodsys/factories/__init__.py
--rw-r--r--   0        0        0     3400 2024-05-04 14:52:14.101328 prodsys-0.6.0/prodsys/factories/link_transport_process_updater.py
--rw-r--r--   0        0        0     1745 2024-05-04 14:52:14.101328 prodsys-0.6.0/prodsys/factories/node_factory.py
--rw-r--r--   0        0        0     3752 2024-05-04 14:52:14.109195 prodsys-0.6.0/prodsys/factories/process_factory.py
--rw-r--r--   0        0        0     6358 2024-03-10 14:05:36.923357 prodsys-0.6.0/prodsys/factories/product_factory.py
--rw-r--r--   0        0        0     1992 2024-03-10 14:05:36.923357 prodsys-0.6.0/prodsys/factories/queue_factory.py
--rw-r--r--   0        0        0    11157 2024-05-04 14:52:14.109943 prodsys-0.6.0/prodsys/factories/resource_factory.py
--rw-r--r--   0        0        0     3268 2023-10-11 11:05:22.089564 prodsys-0.6.0/prodsys/factories/sink_factory.py
--rw-r--r--   0        0        0     5089 2024-01-07 23:00:16.890715 prodsys-0.6.0/prodsys/factories/source_factory.py
--rw-r--r--   0        0        0     2856 2023-10-11 11:05:22.089564 prodsys-0.6.0/prodsys/factories/state_factory.py
--rw-r--r--   0        0        0     2045 2023-10-11 11:05:22.089564 prodsys-0.6.0/prodsys/factories/time_model_factory.py
--rw-r--r--   0        0        0     1583 2024-05-04 14:52:14.111436 prodsys-0.6.0/prodsys/models/__init__.py
--rw-r--r--   0        0        0      541 2023-10-11 11:05:22.089564 prodsys-0.6.0/prodsys/models/core_asset.py
--rw-r--r--   0        0        0     1233 2024-05-04 14:52:14.111436 prodsys-0.6.0/prodsys/models/node_data.py
--rw-r--r--   0        0        0     2971 2024-04-26 10:14:01.064800 prodsys-0.6.0/prodsys/models/performance_data.py
--rw-r--r--   0        0        0     9369 2024-04-19 09:06:03.048928 prodsys-0.6.0/prodsys/models/performance_indicators.py
--rw-r--r--   0        0        0    14397 2024-05-04 14:52:14.113445 prodsys-0.6.0/prodsys/models/processes_data.py
--rw-r--r--   0        0        0     6357 2024-05-04 14:20:57.302536 prodsys-0.6.0/prodsys/models/product_data.py
--rw-r--r--   0        0        0     1931 2024-05-04 14:20:57.303890 prodsys-0.6.0/prodsys/models/queue_data.py
--rw-r--r--   0        0        0    12335 2024-05-04 14:52:14.113445 prodsys-0.6.0/prodsys/models/resource_data.py
--rw-r--r--   0        0        0    10745 2024-05-04 14:52:14.115031 prodsys-0.6.0/prodsys/models/scenario_data.py
--rw-r--r--   0        0        0     2846 2024-05-04 14:20:57.305926 prodsys-0.6.0/prodsys/models/sink_data.py
--rw-r--r--   0        0        0     4059 2024-05-04 14:20:57.312957 prodsys-0.6.0/prodsys/models/source_data.py
--rw-r--r--   0        0        0    13852 2024-05-04 14:20:57.312957 prodsys-0.6.0/prodsys/models/state_data.py
--rw-r--r--   0        0        0     6642 2024-05-04 14:20:57.312957 prodsys-0.6.0/prodsys/models/time_model_data.py
--rw-r--r--   0        0        0     2870 2023-10-11 11:05:22.105207 prodsys-0.6.0/prodsys/optimization/__init__.py
--rw-r--r--   0        0        0    12500 2024-05-04 14:52:14.115836 prodsys-0.6.0/prodsys/optimization/evolutionary_algorithm.py
--rw-r--r--   0        0        0    28223 2024-05-04 14:20:57.312957 prodsys-0.6.0/prodsys/optimization/math_opt.py
--rw-r--r--   0        0        0     4642 2024-05-04 14:20:57.321008 prodsys-0.6.0/prodsys/optimization/optimization_analysis.py
--rw-r--r--   0        0        0    46203 2024-05-04 14:52:14.116698 prodsys-0.6.0/prodsys/optimization/optimization_util.py
--rw-r--r--   0        0        0     9601 2024-05-04 14:52:14.118464 prodsys-0.6.0/prodsys/optimization/simulated_annealing.py
--rw-r--r--   0        0        0    11895 2024-05-04 14:52:14.119595 prodsys-0.6.0/prodsys/optimization/tabu_search.py
--rw-r--r--   0        0        0     1704 2023-10-11 11:05:22.105207 prodsys-0.6.0/prodsys/simulation/__init__.py
--rw-r--r--   0        0        0    31006 2024-05-04 14:52:14.120801 prodsys-0.6.0/prodsys/simulation/control.py
--rw-r--r--   0        0        0     6855 2024-05-01 15:14:08.116047 prodsys-0.6.0/prodsys/simulation/logger.py
--rw-r--r--   0        0        0      459 2024-05-04 14:52:14.122204 prodsys-0.6.0/prodsys/simulation/node.py
--rw-r--r--   0        0        0     3765 2024-05-04 14:52:14.123256 prodsys-0.6.0/prodsys/simulation/observer.py
--rw-r--r--   0        0        0     9599 2024-05-04 14:52:14.124428 prodsys-0.6.0/prodsys/simulation/proces_models.py
--rw-r--r--   0        0        0    11900 2024-05-04 14:52:14.125901 prodsys-0.6.0/prodsys/simulation/process.py
--rw-r--r--   0        0        0    10255 2024-05-04 14:52:14.125901 prodsys-0.6.0/prodsys/simulation/product.py
--rw-r--r--   0        0        0     5716 2024-05-04 14:52:14.125901 prodsys-0.6.0/prodsys/simulation/request.py
--rw-r--r--   0        0        0    18086 2024-05-04 14:52:14.125901 prodsys-0.6.0/prodsys/simulation/resources.py
--rw-r--r--   0        0        0    10029 2024-05-04 14:52:14.125901 prodsys-0.6.0/prodsys/simulation/route_finder.py
--rw-r--r--   0        0        0    15942 2024-05-04 14:52:14.132408 prodsys-0.6.0/prodsys/simulation/router.py
--rw-r--r--   0        0        0     3199 2024-04-26 10:14:01.122122 prodsys-0.6.0/prodsys/simulation/sim.py
--rw-r--r--   0        0        0     2260 2024-05-04 14:20:57.328996 prodsys-0.6.0/prodsys/simulation/sink.py
--rw-r--r--   0        0        0     3809 2024-05-04 14:20:57.328996 prodsys-0.6.0/prodsys/simulation/source.py
--rw-r--r--   0        0        0    29728 2024-05-04 14:52:14.132408 prodsys-0.6.0/prodsys/simulation/state.py
--rw-r--r--   0        0        0     2232 2024-01-07 23:00:16.919358 prodsys-0.6.0/prodsys/simulation/store.py
--rw-r--r--   0        0        0     7191 2024-05-04 14:52:14.135356 prodsys-0.6.0/prodsys/simulation/time_model.py
--rw-r--r--   0        0        0       61 2023-10-11 11:05:22.120833 prodsys-0.6.0/prodsys/util/__init__.py
--rw-r--r--   0        0        0     8056 2023-11-06 17:14:55.559034 prodsys-0.6.0/prodsys/util/kpi_visualization.py
--rw-r--r--   0        0        0    30349 2024-05-04 14:20:57.328996 prodsys-0.6.0/prodsys/util/post_processing.py
--rw-r--r--   0        0        0    12893 2024-05-04 14:52:14.136563 prodsys-0.6.0/prodsys/util/runner.py
--rw-r--r--   0        0        0     2657 2023-12-24 16:10:02.245387 prodsys-0.6.0/prodsys/util/statistical_functions.py
--rw-r--r--   0        0        0     4390 2024-05-04 14:52:14.137675 prodsys-0.6.0/prodsys/util/util.py
--rw-r--r--   0        0        0     1605 2024-05-04 14:52:14.138455 prodsys-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     6375 2024-05-04 14:20:57.249746 prodsys-0.6.0/README.md
--rw-r--r--   0        0        0     8405 1970-01-01 00:00:00.000000 prodsys-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-10-11 11:05:21.946526 prodsys-0.6.1/LICENSE
+-rw-r--r--   0        0        0      405 2024-05-05 08:37:15.083348 prodsys-0.6.1/prodsys/__init__.py
+-rw-r--r--   0        0        0     1289 2024-05-01 05:54:38.231436 prodsys-0.6.1/prodsys/adapters/__init__.py
+-rw-r--r--   0        0        0    56359 2024-05-05 08:37:15.084888 prodsys-0.6.1/prodsys/adapters/adapter.py
+-rw-r--r--   0        0        0     8854 2024-05-04 15:39:44.446374 prodsys-0.6.1/prodsys/adapters/json_adapter.py
+-rw-r--r--   0        0        0        0 2024-01-07 23:00:16.874004 prodsys-0.6.1/prodsys/conf/__init__.py
+-rw-r--r--   0        0        0     2487 2024-01-07 23:00:16.874004 prodsys-0.6.1/prodsys/conf/logging.ini
+-rw-r--r--   0        0        0     1155 2024-01-07 23:00:16.874004 prodsys-0.6.1/prodsys/conf/logging_config.py
+-rw-r--r--   0        0        0      148 2023-10-11 11:05:22.073479 prodsys-0.6.1/prodsys/control/__init__.py
+-rw-r--r--   0        0        0     9030 2024-05-04 15:39:44.446374 prodsys-0.6.1/prodsys/control/routing_control_env.py
+-rw-r--r--   0        0        0     8489 2023-10-11 11:05:22.073479 prodsys-0.6.1/prodsys/control/sequencing_control_env.py
+-rw-r--r--   0        0        0     2236 2024-05-04 15:39:44.446374 prodsys-0.6.1/prodsys/express/__init__.py
+-rw-r--r--   0        0        0      603 2023-10-11 11:05:22.073479 prodsys-0.6.1/prodsys/express/core.py
+-rw-r--r--   0        0        0     1589 2024-05-04 15:39:44.446374 prodsys-0.6.1/prodsys/express/node.py
+-rw-r--r--   0        0        0    11649 2024-05-04 15:39:44.446374 prodsys-0.6.1/prodsys/express/process.py
+-rw-r--r--   0        0        0     2477 2024-05-04 15:39:44.457893 prodsys-0.6.1/prodsys/express/product.py
+-rw-r--r--   0        0        0     7129 2024-05-04 15:39:44.457893 prodsys-0.6.1/prodsys/express/production_system.py
+-rw-r--r--   0        0        0     8295 2024-05-04 15:39:44.457893 prodsys-0.6.1/prodsys/express/resources.py
+-rw-r--r--   0        0        0     2573 2024-05-04 15:39:44.464082 prodsys-0.6.1/prodsys/express/sink.py
+-rw-r--r--   0        0        0     3413 2024-05-04 15:39:44.464082 prodsys-0.6.1/prodsys/express/source.py
+-rw-r--r--   0        0        0     7554 2024-05-01 07:15:45.742369 prodsys-0.6.1/prodsys/express/state.py
+-rw-r--r--   0        0        0     4884 2024-05-04 15:39:44.464082 prodsys-0.6.1/prodsys/express/time_model.py
+-rw-r--r--   0        0        0      913 2023-10-11 11:05:22.089564 prodsys-0.6.1/prodsys/factories/__init__.py
+-rw-r--r--   0        0        0     3400 2024-05-04 15:39:44.464082 prodsys-0.6.1/prodsys/factories/link_transport_process_updater.py
+-rw-r--r--   0        0        0     1745 2024-05-04 15:39:44.464082 prodsys-0.6.1/prodsys/factories/node_factory.py
+-rw-r--r--   0        0        0     3752 2024-05-04 15:39:44.464082 prodsys-0.6.1/prodsys/factories/process_factory.py
+-rw-r--r--   0        0        0     6358 2024-03-10 14:05:36.923357 prodsys-0.6.1/prodsys/factories/product_factory.py
+-rw-r--r--   0        0        0     1992 2024-03-10 14:05:36.923357 prodsys-0.6.1/prodsys/factories/queue_factory.py
+-rw-r--r--   0        0        0    11157 2024-05-04 15:39:44.464082 prodsys-0.6.1/prodsys/factories/resource_factory.py
+-rw-r--r--   0        0        0     3268 2023-10-11 11:05:22.089564 prodsys-0.6.1/prodsys/factories/sink_factory.py
+-rw-r--r--   0        0        0     5089 2024-01-07 23:00:16.890715 prodsys-0.6.1/prodsys/factories/source_factory.py
+-rw-r--r--   0        0        0     2856 2023-10-11 11:05:22.089564 prodsys-0.6.1/prodsys/factories/state_factory.py
+-rw-r--r--   0        0        0     2045 2023-10-11 11:05:22.089564 prodsys-0.6.1/prodsys/factories/time_model_factory.py
+-rw-r--r--   0        0        0     1583 2024-05-04 15:39:44.464082 prodsys-0.6.1/prodsys/models/__init__.py
+-rw-r--r--   0        0        0      541 2023-10-11 11:05:22.089564 prodsys-0.6.1/prodsys/models/core_asset.py
+-rw-r--r--   0        0        0     1233 2024-05-04 15:39:44.473598 prodsys-0.6.1/prodsys/models/node_data.py
+-rw-r--r--   0        0        0     3963 2024-05-05 08:37:15.084888 prodsys-0.6.1/prodsys/models/performance_data.py
+-rw-r--r--   0        0        0     9369 2024-04-19 09:06:03.048928 prodsys-0.6.1/prodsys/models/performance_indicators.py
+-rw-r--r--   0        0        0    14397 2024-05-04 15:39:44.476967 prodsys-0.6.1/prodsys/models/processes_data.py
+-rw-r--r--   0        0        0     6357 2024-05-04 14:20:57.302536 prodsys-0.6.1/prodsys/models/product_data.py
+-rw-r--r--   0        0        0     1931 2024-05-04 14:20:57.303890 prodsys-0.6.1/prodsys/models/queue_data.py
+-rw-r--r--   0        0        0    12335 2024-05-04 15:39:44.476967 prodsys-0.6.1/prodsys/models/resource_data.py
+-rw-r--r--   0        0        0    10745 2024-05-05 05:55:40.858758 prodsys-0.6.1/prodsys/models/scenario_data.py
+-rw-r--r--   0        0        0     2846 2024-05-04 14:20:57.305926 prodsys-0.6.1/prodsys/models/sink_data.py
+-rw-r--r--   0        0        0     4059 2024-05-04 14:20:57.312957 prodsys-0.6.1/prodsys/models/source_data.py
+-rw-r--r--   0        0        0    13852 2024-05-04 14:20:57.312957 prodsys-0.6.1/prodsys/models/state_data.py
+-rw-r--r--   0        0        0     6642 2024-05-04 14:20:57.312957 prodsys-0.6.1/prodsys/models/time_model_data.py
+-rw-r--r--   0        0        0     2870 2023-10-11 11:05:22.105207 prodsys-0.6.1/prodsys/optimization/__init__.py
+-rw-r--r--   0        0        0    12423 2024-05-05 08:37:15.084888 prodsys-0.6.1/prodsys/optimization/evolutionary_algorithm.py
+-rw-r--r--   0        0        0    28142 2024-05-05 08:37:15.084888 prodsys-0.6.1/prodsys/optimization/math_opt.py
+-rw-r--r--   0        0        0     4642 2024-05-04 14:20:57.321008 prodsys-0.6.1/prodsys/optimization/optimization_analysis.py
+-rw-r--r--   0        0        0    46203 2024-05-04 15:39:44.483548 prodsys-0.6.1/prodsys/optimization/optimization_util.py
+-rw-r--r--   0        0        0     9523 2024-05-05 08:37:15.091916 prodsys-0.6.1/prodsys/optimization/simulated_annealing.py
+-rw-r--r--   0        0        0    11829 2024-05-05 08:37:15.091916 prodsys-0.6.1/prodsys/optimization/tabu_search.py
+-rw-r--r--   0        0        0     1704 2023-10-11 11:05:22.105207 prodsys-0.6.1/prodsys/simulation/__init__.py
+-rw-r--r--   0        0        0    31006 2024-05-04 15:39:44.489571 prodsys-0.6.1/prodsys/simulation/control.py
+-rw-r--r--   0        0        0     6855 2024-05-01 15:14:08.116047 prodsys-0.6.1/prodsys/simulation/logger.py
+-rw-r--r--   0        0        0      459 2024-05-04 15:39:44.489571 prodsys-0.6.1/prodsys/simulation/node.py
+-rw-r--r--   0        0        0     3765 2024-05-04 15:39:44.489571 prodsys-0.6.1/prodsys/simulation/observer.py
+-rw-r--r--   0        0        0     9599 2024-05-04 15:39:44.489571 prodsys-0.6.1/prodsys/simulation/proces_models.py
+-rw-r--r--   0        0        0    11900 2024-05-04 15:39:44.489571 prodsys-0.6.1/prodsys/simulation/process.py
+-rw-r--r--   0        0        0    10255 2024-05-04 15:39:44.489571 prodsys-0.6.1/prodsys/simulation/product.py
+-rw-r--r--   0        0        0     5716 2024-05-04 15:39:44.489571 prodsys-0.6.1/prodsys/simulation/request.py
+-rw-r--r--   0        0        0    18086 2024-05-04 15:39:44.489571 prodsys-0.6.1/prodsys/simulation/resources.py
+-rw-r--r--   0        0        0    10029 2024-05-04 15:39:44.489571 prodsys-0.6.1/prodsys/simulation/route_finder.py
+-rw-r--r--   0        0        0    15942 2024-05-04 15:39:44.489571 prodsys-0.6.1/prodsys/simulation/router.py
+-rw-r--r--   0        0        0     3202 2024-05-05 08:37:15.091916 prodsys-0.6.1/prodsys/simulation/sim.py
+-rw-r--r--   0        0        0     2260 2024-05-04 14:20:57.328996 prodsys-0.6.1/prodsys/simulation/sink.py
+-rw-r--r--   0        0        0     3809 2024-05-04 14:20:57.328996 prodsys-0.6.1/prodsys/simulation/source.py
+-rw-r--r--   0        0        0    29728 2024-05-04 15:39:44.505331 prodsys-0.6.1/prodsys/simulation/state.py
+-rw-r--r--   0        0        0     2232 2024-01-07 23:00:16.919358 prodsys-0.6.1/prodsys/simulation/store.py
+-rw-r--r--   0        0        0     7191 2024-05-04 15:39:44.505331 prodsys-0.6.1/prodsys/simulation/time_model.py
+-rw-r--r--   0        0        0       61 2023-10-11 11:05:22.120833 prodsys-0.6.1/prodsys/util/__init__.py
+-rw-r--r--   0        0        0     8056 2023-11-06 17:14:55.559034 prodsys-0.6.1/prodsys/util/kpi_visualization.py
+-rw-r--r--   0        0        0    30349 2024-05-04 14:20:57.328996 prodsys-0.6.1/prodsys/util/post_processing.py
+-rw-r--r--   0        0        0    12929 2024-05-05 08:37:15.091916 prodsys-0.6.1/prodsys/util/runner.py
+-rw-r--r--   0        0        0     2657 2023-12-24 16:10:02.245387 prodsys-0.6.1/prodsys/util/statistical_functions.py
+-rw-r--r--   0        0        0     4390 2024-05-04 15:39:44.505331 prodsys-0.6.1/prodsys/util/util.py
+-rw-r--r--   0        0        0     1633 2024-05-05 08:37:15.099883 prodsys-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     7237 2024-05-05 08:37:14.995920 prodsys-0.6.1/README.md
+-rw-r--r--   0        0        0     9296 1970-01-01 00:00:00.000000 prodsys-0.6.1/PKG-INFO
```

### Comparing `prodsys-0.6.0/LICENSE` & `prodsys-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/adapters/__init__.py` & `prodsys-0.6.1/prodsys/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/adapters/adapter.py` & `prodsys-0.6.1/prodsys/adapters/adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -303,16 +303,16 @@
     valid_configuration: bool = True
     reconfiguration_cost: float = 0
 
     class Config:
         validate = True
         validate_assignment = True
         schema_extra = {
-            "example": {
-                "ID": "",
+            "examples": [{
+                "ID": "Example Adapter",
                 "valid_configuration": True,
                 "reconfiguration_cost": 0,
                 "seed": 24,
                 "time_model_data": [
                     {
                         "ID": "function_time_model_1",
                         "description": "normal distribution time model with 20 minutes",
@@ -671,14 +671,15 @@
                         "router": "SimpleRouter",
                         "routing_heuristic": "shortest_queue",
                         "output_queues": ["SourceQueue"],
                     },
                 ],
                 "scenario_data": None,
             }
+            ]
         }
 
     def hash(self) -> str:
         """
         Generates a hash of the adapter based on the hash of all contained entities. Only information describing the physical structure and functionality of the production system is considered. Can be used to compare two production systems of adapters for functional equality.
 
         Returns:
```

### Comparing `prodsys-0.6.0/prodsys/adapters/json_adapter.py` & `prodsys-0.6.1/prodsys/adapters/json_adapter.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/conf/logging.ini` & `prodsys-0.6.1/prodsys/conf/logging.ini`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/conf/logging_config.py` & `prodsys-0.6.1/prodsys/conf/logging_config.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/control/routing_control_env.py` & `prodsys-0.6.1/prodsys/control/routing_control_env.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/control/sequencing_control_env.py` & `prodsys-0.6.1/prodsys/control/sequencing_control_env.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/express/__init__.py` & `prodsys-0.6.1/prodsys/express/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/express/core.py` & `prodsys-0.6.1/prodsys/express/core.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/express/node.py` & `prodsys-0.6.1/prodsys/express/node.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/express/process.py` & `prodsys-0.6.1/prodsys/express/process.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/express/product.py` & `prodsys-0.6.1/prodsys/express/product.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/express/production_system.py` & `prodsys-0.6.1/prodsys/express/production_system.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/express/resources.py` & `prodsys-0.6.1/prodsys/express/resources.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/express/sink.py` & `prodsys-0.6.1/prodsys/express/sink.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/express/source.py` & `prodsys-0.6.1/prodsys/express/source.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/express/state.py` & `prodsys-0.6.1/prodsys/express/state.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/express/time_model.py` & `prodsys-0.6.1/prodsys/express/time_model.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/factories/__init__.py` & `prodsys-0.6.1/prodsys/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/factories/link_transport_process_updater.py` & `prodsys-0.6.1/prodsys/factories/link_transport_process_updater.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/factories/node_factory.py` & `prodsys-0.6.1/prodsys/factories/node_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/factories/process_factory.py` & `prodsys-0.6.1/prodsys/factories/process_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/factories/product_factory.py` & `prodsys-0.6.1/prodsys/factories/product_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/factories/queue_factory.py` & `prodsys-0.6.1/prodsys/factories/queue_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/factories/resource_factory.py` & `prodsys-0.6.1/prodsys/factories/resource_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/factories/sink_factory.py` & `prodsys-0.6.1/prodsys/factories/sink_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/factories/source_factory.py` & `prodsys-0.6.1/prodsys/factories/source_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/factories/state_factory.py` & `prodsys-0.6.1/prodsys/factories/state_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/factories/time_model_factory.py` & `prodsys-0.6.1/prodsys/factories/time_model_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/models/__init__.py` & `prodsys-0.6.1/prodsys/models/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/models/core_asset.py` & `prodsys-0.6.1/prodsys/models/core_asset.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/models/node_data.py` & `prodsys-0.6.1/prodsys/models/node_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/models/performance_data.py` & `prodsys-0.6.1/prodsys/models/performance_data.py`

 * *Files 25% similar despite different names*

```diff
@@ -46,38 +46,64 @@
                     "resource": "R1",
                     "state": "P1",
                     "state_type": "Production",
                     "activity": "start state",
                     "product": "Product_1_12",
                     "expected_end_time": 24.3,
                     "target_location": None,
-                },
+                }, 
                 {
                     "time": 24.3,
                     "resource": "R1",
                     "state": "P1",
                     "state_type": "Production",
                     "activity": "end state",
                     "product": "Product_1_12",
                     "expected_end_time": None,
-                    "target_location": None,
+                    "target_location": "L1",
                 },
             ]
         }
 
 
 class Performance(BaseModel):
     """
     Class that represents the performance of a simulation run.
 
     Args:
         event_log (List[Event]): Event log of the simulation run.
         kpis (List[KPI_UNION]): List of KPIs of the simulation run.
     """
 
+    class Config:
+        schema_extra = {
+            "examples": [{               
+                    "event_log": Event.Config.schema_extra["examples"],
+                    "kpis": [
+                        {
+                            "name": "throughput",
+                            "target": "max",
+                            "weight": 1,
+                            "value": 4.32,
+                            "context": ["system", "product_type"],
+                            "product_type": "ProductType_1",
+                        },
+                        {
+                            "name": "WIP",
+                            "target": "min",
+                            "weight": 1,
+                            "value": 121,
+                            "context": ["system", "product_type"],
+                            "product_type": "ProductType_1",
+                        },
+                    ],
+                }
+            ]
+        }
+
     event_log: List[Event]
     kpis: List[KPI_UNION]
 
     def get_kpi_for_context(self, context: Tuple[KPILevelEnum, ...]) -> List[KPI_UNION]:
         return [kpi for kpi in self.kpis if context == kpi.context]
 
     def get_kpi_for_name(self, name: KPIEnum) -> List[KPI_UNION]:
```

### Comparing `prodsys-0.6.0/prodsys/models/performance_indicators.py` & `prodsys-0.6.1/prodsys/models/performance_indicators.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/models/processes_data.py` & `prodsys-0.6.1/prodsys/models/processes_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/models/product_data.py` & `prodsys-0.6.1/prodsys/models/product_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/models/queue_data.py` & `prodsys-0.6.1/prodsys/models/queue_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/models/resource_data.py` & `prodsys-0.6.1/prodsys/models/resource_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/models/scenario_data.py` & `prodsys-0.6.1/prodsys/models/scenario_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/models/sink_data.py` & `prodsys-0.6.1/prodsys/models/sink_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/models/source_data.py` & `prodsys-0.6.1/prodsys/models/source_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/models/state_data.py` & `prodsys-0.6.1/prodsys/models/state_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/models/time_model_data.py` & `prodsys-0.6.1/prodsys/models/time_model_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/optimization/__init__.py` & `prodsys-0.6.1/prodsys/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/optimization/evolutionary_algorithm.py` & `prodsys-0.6.1/prodsys/optimization/evolutionary_algorithm.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,26 +64,25 @@
     mutation_rate: float = 0.1
     crossover_rate: float = 0.1
     number_of_seeds: int = 1
     number_of_processes: int = 1
 
     class Config:
         schema_extra = {
-            "example": {
-                "summary": "Evolutionary Algorithm Hperparameters",
-                "value": {
+            "examples": [
+                {
                     "seed": 0,
                     "number_of_generations": 10,
                     "population_size": 10,
                     "mutation_rate": 0.1,
                     "crossover_rate": 0.1,
                     "number_of_seeds": 1,
                     "number_of_processes": 1,
                 },
-            }
+            ]
         }
 
 
 
 def register_functions_in_toolbox(
     base_configuration: adapters.JsonProductionSystemAdapter,
     solution_dict: dict,
```

### Comparing `prodsys-0.6.0/prodsys/optimization/math_opt.py` & `prodsys-0.6.1/prodsys/optimization/math_opt.py`

 * *Files 1% similar despite different names*

```diff
@@ -544,23 +544,22 @@
     optimization_time_portion: float = 0.5
     number_of_solutions: int = 1
     adjusted_number_of_transport_resources: int = 1
     number_of_seeds: int = 1
 
     class Config:
         schema_extra = {
-            "example": {
-                "summary": "Mathematical Optimization Hyperparameters",
-                "value": {
+            "examples": [
+                {
                     "optimization_time_portion": 0.5,
                     "number_of_solutions": 1,
                     "adjusted_number_of_transport_resources": 1,
                     "number_of_seeds": 1,
                 },
-            }
+            ]
         }
 
 
 def run_mathematical_optimization(
     save_folder: str,
     base_configuration_file_path: str,
     scenario_file_path: str,
```

### Comparing `prodsys-0.6.0/prodsys/optimization/optimization_analysis.py` & `prodsys-0.6.1/prodsys/optimization/optimization_analysis.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/optimization/optimization_util.py` & `prodsys-0.6.1/prodsys/optimization/optimization_util.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/optimization/simulated_annealing.py` & `prodsys-0.6.1/prodsys/optimization/simulated_annealing.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,25 +100,24 @@
     Tmin: int = 1
     steps: int = 4000
     updates: int = 300
     number_of_seeds: int = 1
 
     class Config:
         schema_extra = {
-            "example": {
-                "summary": "Simulated Annealing Hyperparameters",
-                "value": {
+            "examples": [ 
+            {
                     "seed": 0,
                     "Tmax": 10000,
                     "Tmin": 1,
                     "steps": 4000,
                     "updates": 300,
                     "number_of_seeds": 1,
                 },
-            }
+            ]
         }
 
 
 def run_simulated_annealing(
     save_folder: str,
     base_configuration_file_path: str,
     scenario_file_path: str,
```

### Comparing `prodsys-0.6.0/prodsys/optimization/tabu_search.py` & `prodsys-0.6.1/prodsys/optimization/tabu_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,24 +149,23 @@
     tabu_size: int = 10
     max_steps: int = 300
     max_score: float = 500
     number_of_seeds: int = 1
 
     class Config:
         schema_extra = {
-            "example": {
-                "summary": "Tabu Search Hyperparameters",
-                "value": {
+            "examples": [
+                 {
                     "seed": 0,
                     "tabu_size": 10,
                     "max_steps": 300,
                     "max_score": 500,
                     "number_of_seeds": 1,
                 },
-            }
+            ]
         }
 
 
 def run_tabu_search(
     save_folder: str,
     base_configuration_file_path: str,
     scenario_file_path: str,
```

### Comparing `prodsys-0.6.0/prodsys/simulation/__init__.py` & `prodsys-0.6.1/prodsys/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/simulation/control.py` & `prodsys-0.6.1/prodsys/simulation/control.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/simulation/logger.py` & `prodsys-0.6.1/prodsys/simulation/logger.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/simulation/observer.py` & `prodsys-0.6.1/prodsys/simulation/observer.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/simulation/proces_models.py` & `prodsys-0.6.1/prodsys/simulation/proces_models.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/simulation/process.py` & `prodsys-0.6.1/prodsys/simulation/process.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/simulation/product.py` & `prodsys-0.6.1/prodsys/simulation/product.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/simulation/request.py` & `prodsys-0.6.1/prodsys/simulation/request.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/simulation/resources.py` & `prodsys-0.6.1/prodsys/simulation/resources.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/simulation/route_finder.py` & `prodsys-0.6.1/prodsys/simulation/route_finder.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/simulation/router.py` & `prodsys-0.6.1/prodsys/simulation/router.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/simulation/sim.py` & `prodsys-0.6.1/prodsys/simulation/sim.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     """
     def __init__(self, seed: int=0) -> None:
         super().__init__()
         self.seed: int = seed
         self.pbar: Any = None
         self.last_update = 0
 
-    def run(self, time_range:int):
+    def run(self, time_range: float):
         """
         Runs the simulation for a given time range.
 
         Args:
             time_range (int): The time range to run the simulation for in minutes.
         """
         with temp_seed(self.seed):
```

### Comparing `prodsys-0.6.0/prodsys/simulation/sink.py` & `prodsys-0.6.1/prodsys/simulation/sink.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/simulation/source.py` & `prodsys-0.6.1/prodsys/simulation/source.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/simulation/state.py` & `prodsys-0.6.1/prodsys/simulation/state.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/simulation/store.py` & `prodsys-0.6.1/prodsys/simulation/store.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/simulation/time_model.py` & `prodsys-0.6.1/prodsys/simulation/time_model.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/util/kpi_visualization.py` & `prodsys-0.6.1/prodsys/util/kpi_visualization.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/util/post_processing.py` & `prodsys-0.6.1/prodsys/util/post_processing.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/util/runner.py` & `prodsys-0.6.1/prodsys/util/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,17 +236,17 @@
 
         Returns:
             List[performance_data.Event]: The event data of the simulation.
         """
         p = self.get_post_processor()
         df_raw=self.event_logger.get_data_as_dataframe()
         events = []
-        df_raw["Expected End Time"].fillna(value=-1, inplace=True)
-        df_raw["Target location"].fillna(value="", inplace=True)
-        df_raw["Product"].fillna(value="", inplace=True)
+        df_raw["Expected End Time"] = df_raw["Expected End Time"].fillna(value=-1)
+        df_raw["Target location"] = df_raw["Target location"].fillna(value="")
+        df_raw["Product"] = df_raw["Product"].fillna(value="")
         for index, row in df_raw.iterrows():
             
             events.append(
                 performance_data.Event(
                     time=row["Time"],
                     resource=row["Resource"],
                     state=row["State"],
```

### Comparing `prodsys-0.6.0/prodsys/util/statistical_functions.py` & `prodsys-0.6.1/prodsys/util/statistical_functions.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/prodsys/util/util.py` & `prodsys-0.6.1/prodsys/util/util.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.0/pyproject.toml` & `prodsys-0.6.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prodsys"
-version = "0.6.0"
+version = "0.6.1"
 description = "A useful module for production system simulation and optimization"
 authors = ["Sebastian Behrendt <sebastia.behrendt@kit.edu>"]
 license = "MIT"
 readme = ["README.md", "LICENSE"]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.13"
@@ -17,14 +17,15 @@
 gurobipy = "^10.0.1"
 hydra-core = "^1.3.2"
 pandas = "^2.0.0"
 openpyxl = "^3.1.2"
 plotly = "^5.14.1"
 scipy = "^1.11.1"
 tqdm = "^4.65"
+email-validator = "^2.1.1"
 
 [tool.poetry.extras]
 ai = ["torch", "torchvision", "torchaudio", "tensorboard", "gymnasium", "stable-baselines3"]
 
 
 [tool.poetry.group.ai]
 optional = true
```

### Comparing `prodsys-0.6.0/README.md` & `prodsys-0.6.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 *prodsys - modeling, simulating and optimizing production systems*
 
 ![Build-sucess](https://img.shields.io/badge/build-success-green)
 ![PyPI](https://img.shields.io/pypi/v/prodsys)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/prodsys)
 ![Docu](https://img.shields.io/badge/docu-full-green)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10995273.svg)](https://doi.org/10.5281/zenodo.10995273)
 
 prodsys is a python package for modeling, simulating and optimizing production systems based on the product, process and resource (PPR) modelling principle. For more information, have a look at the [documentation](https://sdm4fzi.github.io/prodsys/).
 
 ## Installation
 
 To install the package, run the following command in the terminal:
 
@@ -98,14 +99,32 @@
 import numpy as np
 wip = np.array(wip_values).mean(axis=0)
 print(wip)
 ```
 
 These examples only cover the most basic functionalities of `prodsys`. For more elaborate guides that guide you through more of the package's features, please see the [tutorials](https://sdm4fzi.github.io/prodsys/Tutorials/tutorial_0_overview). For a complete overview of the package's functionality, please see the [API reference](https://sdm4fzi.github.io/prodsys/API_reference/API_reference_0_overview/).
 
+## Run prodsys as a webserver with REST API
+
+prodsys cannot only be used as a python package, but can also be used as a webserver by interacting with its REST API. All features of prodsys are also available in the API and allow easy integration of prodsys in operative IT architectures. 
+
+The API is based on the [FastAPI](https://fastapi.tiangolo.com/) framework and utilizes the models API of prodsys. To use prodsys as a webserver, you can use the official docker image which can be obtained from dockerhub:
+
+```bash
+docker pull sebbehrendt/prodsys
+```
+
+To start the API, run the following command:
+
+```bash
+docker run -p 8000:8000 sebbehrendt/prodsys
+```
+
+The API documentation is then available at `http://localhost:8000/docs`. 
+
 ## Contributing
 
 `prodsys` is a new project and has therefore much room for improvement. Therefore, it would be a pleasure to get feedback or support! If you want to contribute to the package, either create issues on [prodsys' github page](https://github.com/sdm4fzi/prodsys) for discussing new features or contact me directly via [github](https://github.com/SebBehrendt) or [email](mailto:sebastian.behrendt@kit.edu).
 
 ## License
 
 The package is licensed under the [MIT license](LICENSE).
```

### Comparing `prodsys-0.6.0/PKG-INFO` & `prodsys-0.6.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: prodsys
-Version: 0.6.0
+Version: 0.6.1
 Summary: A useful module for production system simulation and optimization
 License: MIT
 Author: Sebastian Behrendt
 Author-email: sebastia.behrendt@kit.edu
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: ai
 Requires-Dist: deap (>=1.3.3,<2.0.0)
+Requires-Dist: email-validator (>=2.1.1,<3.0.0)
 Requires-Dist: fastapi (==0.99.1)
 Requires-Dist: gurobipy (>=10.0.1,<11.0.0)
 Requires-Dist: hydra-core (>=1.3.2,<2.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: plotly (>=5.14.1,<6.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
@@ -31,14 +32,15 @@
 
 *prodsys - modeling, simulating and optimizing production systems*
 
 ![Build-sucess](https://img.shields.io/badge/build-success-green)
 ![PyPI](https://img.shields.io/pypi/v/prodsys)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/prodsys)
 ![Docu](https://img.shields.io/badge/docu-full-green)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10995273.svg)](https://doi.org/10.5281/zenodo.10995273)
 
 prodsys is a python package for modeling, simulating and optimizing production systems based on the product, process and resource (PPR) modelling principle. For more information, have a look at the [documentation](https://sdm4fzi.github.io/prodsys/).
 
 ## Installation
 
 To install the package, run the following command in the terminal:
 
@@ -127,14 +129,32 @@
 import numpy as np
 wip = np.array(wip_values).mean(axis=0)
 print(wip)
 ```
 
 These examples only cover the most basic functionalities of `prodsys`. For more elaborate guides that guide you through more of the package's features, please see the [tutorials](https://sdm4fzi.github.io/prodsys/Tutorials/tutorial_0_overview). For a complete overview of the package's functionality, please see the [API reference](https://sdm4fzi.github.io/prodsys/API_reference/API_reference_0_overview/).
 
+## Run prodsys as a webserver with REST API
+
+prodsys cannot only be used as a python package, but can also be used as a webserver by interacting with its REST API. All features of prodsys are also available in the API and allow easy integration of prodsys in operative IT architectures. 
+
+The API is based on the [FastAPI](https://fastapi.tiangolo.com/) framework and utilizes the models API of prodsys. To use prodsys as a webserver, you can use the official docker image which can be obtained from dockerhub:
+
+```bash
+docker pull sebbehrendt/prodsys
+```
+
+To start the API, run the following command:
+
+```bash
+docker run -p 8000:8000 sebbehrendt/prodsys
+```
+
+The API documentation is then available at `http://localhost:8000/docs`. 
+
 ## Contributing
 
 `prodsys` is a new project and has therefore much room for improvement. Therefore, it would be a pleasure to get feedback or support! If you want to contribute to the package, either create issues on [prodsys' github page](https://github.com/sdm4fzi/prodsys) for discussing new features or contact me directly via [github](https://github.com/SebBehrendt) or [email](mailto:sebastian.behrendt@kit.edu).
 
 ## License
 
 The package is licensed under the [MIT license](LICENSE).
```

