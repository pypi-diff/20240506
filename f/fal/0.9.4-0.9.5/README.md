# Comparing `tmp/fal-0.9.4.tar.gz` & `tmp/fal-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fal-0.9.4.tar", max compression
+gzip compressed data, was "fal-0.9.5.tar", max compression
```

## Comparing `fal-0.9.4.tar` & `fal-0.9.5.tar`

### file list

```diff
@@ -1,90 +1,90 @@
--rw-r--r--   0        0        0    10531 2023-07-17 22:39:33.453927 fal-0.9.4/README.md
--rw-r--r--   0        0        0     2429 2023-07-17 22:39:46.589959 fal-0.9.4/pyproject.toml
--rw-r--r--   0        0        0      639 2023-07-17 22:39:33.465927 fal-0.9.4/src/dbt/adapters/fal/__init__.py
--rw-r--r--   0        0        0       18 2023-07-17 22:39:47.093960 fal-0.9.4/src/dbt/adapters/fal/__version__.py
--rw-r--r--   0        0        0      392 2023-07-17 22:39:33.465927 fal-0.9.4/src/dbt/adapters/fal/connections.py
--rw-r--r--   0        0        0     3369 2023-07-17 22:39:33.465927 fal-0.9.4/src/dbt/adapters/fal/impl.py
--rw-r--r--   0        0        0     2768 2023-07-17 22:39:33.465927 fal-0.9.4/src/dbt/adapters/fal/load_db_profile.py
--rw-r--r--   0        0        0     4091 2023-07-17 22:39:33.465927 fal-0.9.4/src/dbt/adapters/fal/wrappers.py
--rw-r--r--   0        0        0      344 2023-07-17 22:39:33.465927 fal-0.9.4/src/dbt/adapters/fal_experimental/__init__.py
--rw-r--r--   0        0        0       18 2023-07-17 22:39:47.093960 fal-0.9.4/src/dbt/adapters/fal_experimental/__version__.py
--rw-r--r--   0        0        0     4861 2023-07-17 22:39:33.465927 fal-0.9.4/src/dbt/adapters/fal_experimental/adapter.py
--rw-r--r--   0        0        0     8381 2023-07-17 22:39:33.465927 fal-0.9.4/src/dbt/adapters/fal_experimental/adapter_support.py
--rw-r--r--   0        0        0     1627 2023-07-17 22:39:33.465927 fal-0.9.4/src/dbt/adapters/fal_experimental/connections.py
--rw-r--r--   0        0        0     8714 2023-07-17 22:39:33.465927 fal-0.9.4/src/dbt/adapters/fal_experimental/impl.py
--rw-r--r--   0        0        0     3192 2023-07-17 22:39:33.465927 fal-0.9.4/src/dbt/adapters/fal_experimental/support/athena.py
--rw-r--r--   0        0        0     2686 2023-07-17 22:39:33.465927 fal-0.9.4/src/dbt/adapters/fal_experimental/support/bigquery.py
--rw-r--r--   0        0        0      980 2023-07-17 22:39:33.465927 fal-0.9.4/src/dbt/adapters/fal_experimental/support/duckdb.py
--rw-r--r--   0        0        0     2977 2023-07-17 22:39:33.465927 fal-0.9.4/src/dbt/adapters/fal_experimental/support/postgres.py
--rw-r--r--   0        0        0     1633 2023-07-17 22:39:33.465927 fal-0.9.4/src/dbt/adapters/fal_experimental/support/redshift.py
--rw-r--r--   0        0        0     2781 2023-07-17 22:39:33.465927 fal-0.9.4/src/dbt/adapters/fal_experimental/support/snowflake.py
--rw-r--r--   0        0        0      821 2023-07-17 22:39:33.465927 fal-0.9.4/src/dbt/adapters/fal_experimental/support/trino.py
--rw-r--r--   0        0        0       25 2023-07-17 22:39:33.465927 fal-0.9.4/src/dbt/adapters/fal_experimental/telemetry/__init__.py
--rw-r--r--   0        0        0    10767 2023-07-17 22:39:33.469927 fal-0.9.4/src/dbt/adapters/fal_experimental/telemetry/telemetry.py
--rw-r--r--   0        0        0     6572 2023-07-17 22:39:33.469927 fal-0.9.4/src/dbt/adapters/fal_experimental/teleport.py
--rw-r--r--   0        0        0     1153 2023-07-17 22:39:33.469927 fal-0.9.4/src/dbt/adapters/fal_experimental/teleport_adapter_support.py
--rw-r--r--   0        0        0     4719 2023-07-17 22:39:33.469927 fal-0.9.4/src/dbt/adapters/fal_experimental/teleport_support/duckdb.py
--rw-r--r--   0        0        0     2972 2023-07-17 22:39:33.469927 fal-0.9.4/src/dbt/adapters/fal_experimental/teleport_support/snowflake.py
--rw-r--r--   0        0        0     1256 2023-07-17 22:39:33.469927 fal-0.9.4/src/dbt/adapters/fal_experimental/utils/__init__.py
--rw-r--r--   0        0        0     9804 2023-07-17 22:39:33.469927 fal-0.9.4/src/dbt/adapters/fal_experimental/utils/environments.py
--rw-r--r--   0        0        0     1970 2023-07-17 22:39:33.469927 fal-0.9.4/src/dbt/adapters/fal_experimental/utils/yaml_helper.py
--rw-r--r--   0        0        0      208 2023-07-17 22:39:33.469927 fal-0.9.4/src/dbt/fal/adapters/python/__init__.py
--rw-r--r--   0        0        0    11898 2023-07-17 22:39:33.469927 fal-0.9.4/src/dbt/fal/adapters/python/connections.py
--rw-r--r--   0        0        0    10015 2023-07-17 22:39:33.469927 fal-0.9.4/src/dbt/fal/adapters/python/impl.py
--rw-r--r--   0        0        0      181 2023-07-17 22:39:33.469927 fal-0.9.4/src/dbt/fal/adapters/teleport/__init__.py
--rw-r--r--   0        0        0     3498 2023-07-17 22:39:33.469927 fal-0.9.4/src/dbt/fal/adapters/teleport/impl.py
--rw-r--r--   0        0        0     2310 2023-07-17 22:39:33.469927 fal-0.9.4/src/dbt/fal/adapters/teleport/info.py
--rw-r--r--   0        0        0       52 2023-07-17 22:39:33.469927 fal-0.9.4/src/dbt/include/fal/__init__.py
--rw-r--r--   0        0        0       70 2023-07-17 22:39:33.469927 fal-0.9.4/src/dbt/include/fal/dbt_project.yml
--rw-r--r--   0        0        0     1213 2023-07-17 22:39:33.469927 fal-0.9.4/src/dbt/include/fal/macros/materializations/table.sql
--rw-r--r--   0        0        0      265 2023-07-17 22:39:33.469927 fal-0.9.4/src/dbt/include/fal/macros/teleport_duckdb.sql
--rw-r--r--   0        0        0      921 2023-07-17 22:39:33.469927 fal-0.9.4/src/dbt/include/fal/macros/teleport_snowflake.sql
--rw-r--r--   0        0        0       52 2023-07-17 22:39:33.469927 fal-0.9.4/src/dbt/include/fal_experimental/__init__.py
--rw-r--r--   0        0        0       83 2023-07-17 22:39:33.469927 fal-0.9.4/src/dbt/include/fal_experimental/dbt_project.yml
--rw-r--r--   0        0        0      989 2023-07-17 22:39:33.469927 fal-0.9.4/src/dbt/include/fal_experimental/macros/materializations/table.sql
--rw-r--r--   0        0        0     1905 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/__init__.py
--rw-r--r--   0        0        0      238 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/__init__.py
--rw-r--r--   0        0        0       30 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/cli/__init__.py
--rw-r--r--   0        0        0     7650 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/cli/args.py
--rw-r--r--   0        0        0     1550 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/cli/cli.py
--rw-r--r--   0        0        0     5482 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/cli/dbt_runner.py
--rw-r--r--   0        0        0     5857 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/cli/fal_runner.py
--rw-r--r--   0        0        0     4475 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/cli/flow_runner.py
--rw-r--r--   0        0        0       56 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/cli/model_generator/__init__.py
--rw-r--r--   0        0        0     5543 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/cli/model_generator/model_generator.py
--rw-r--r--   0        0        0     3180 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/cli/model_generator/module_check.py
--rw-r--r--   0        0        0     9759 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/cli/selectors.py
--rw-r--r--   0        0        0    12349 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/fal_script.py
--rw-r--r--   0        0        0        0 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/feature_store/__init__.py
--rw-r--r--   0        0        0      401 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/feature_store/feature.py
--rw-r--r--   0        0        0        0 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/integration/__init__.py
--rw-r--r--   0        0        0    24589 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/integration/lib.py
--rw-r--r--   0        0        0     3273 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/integration/logger.py
--rw-r--r--   0        0        0     1867 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/integration/magics.py
--rw-r--r--   0        0        0     9103 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/integration/parse.py
--rw-r--r--   0        0        0    27168 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/integration/project.py
--rw-r--r--   0        0        0        0 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/integration/utils/__init__.py
--rw-r--r--   0        0        0     1970 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/integration/utils/yaml_helper.py
--rw-r--r--   0        0        0      317 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/integration/version.py
--rw-r--r--   0        0        0     1530 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/new/project.py
--rw-r--r--   0        0        0     8411 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/node_graph.py
--rw-r--r--   0        0        0        0 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/packages/__init__.py
--rw-r--r--   0        0        0     1603 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/packages/bridge.py
--rw-r--r--   0        0        0     5562 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/packages/dependency_analysis.py
--rw-r--r--   0        0        0      805 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/packages/environments/__init__.py
--rw-r--r--   0        0        0     9499 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/packages/environments/base.py
--rw-r--r--   0        0        0     4407 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/packages/environments/conda.py
--rw-r--r--   0        0        0     3381 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/packages/environments/virtual_env.py
--rw-r--r--   0        0        0     4823 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/packages/isolated_runner.py
--rw-r--r--   0        0        0        0 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/planner/__init__.py
--rw-r--r--   0        0        0     5669 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/planner/executor.py
--rw-r--r--   0        0        0     6496 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/planner/plan.py
--rw-r--r--   0        0        0     6790 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/planner/schedule.py
--rw-r--r--   0        0        0     9079 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/planner/tasks.py
--rw-r--r--   0        0        0        0 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/telemetry/__init__.py
--rw-r--r--   0        0        0    11441 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/telemetry/telemetry.py
--rw-r--r--   0        0        0     3060 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/typing.py
--rw-r--r--   0        0        0     1728 2023-07-17 22:39:33.469927 fal-0.9.4/src/fal/dbt/utils.py
--rw-r--r--   0        0        0       33 2023-07-17 22:39:33.469927 fal-0.9.4/tests/_fal_testing/__init__.py
--rw-r--r--   0        0        0     1794 2023-07-17 22:39:33.469927 fal-0.9.4/tests/_fal_testing/utils.py
--rw-r--r--   0        0        0    12552 1970-01-01 00:00:00.000000 fal-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0    10531 2023-07-17 22:49:47.483137 fal-0.9.5/README.md
+-rw-r--r--   0        0        0     2429 2023-07-17 22:49:59.455077 fal-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0      639 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal/__init__.py
+-rw-r--r--   0        0        0       18 2023-07-17 22:49:59.947077 fal-0.9.5/src/dbt/adapters/fal/__version__.py
+-rw-r--r--   0        0        0      392 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal/connections.py
+-rw-r--r--   0        0        0     3369 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal/impl.py
+-rw-r--r--   0        0        0     2768 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal/load_db_profile.py
+-rw-r--r--   0        0        0     4091 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal/wrappers.py
+-rw-r--r--   0        0        0      344 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/__init__.py
+-rw-r--r--   0        0        0       18 2023-07-17 22:49:59.947077 fal-0.9.5/src/dbt/adapters/fal_experimental/__version__.py
+-rw-r--r--   0        0        0     4861 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/adapter.py
+-rw-r--r--   0        0        0     8381 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/adapter_support.py
+-rw-r--r--   0        0        0     1627 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/connections.py
+-rw-r--r--   0        0        0     8714 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/impl.py
+-rw-r--r--   0        0        0     3192 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/support/athena.py
+-rw-r--r--   0        0        0     2686 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/support/bigquery.py
+-rw-r--r--   0        0        0      980 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/support/duckdb.py
+-rw-r--r--   0        0        0     2977 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/support/postgres.py
+-rw-r--r--   0        0        0     1633 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/support/redshift.py
+-rw-r--r--   0        0        0     2781 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/support/snowflake.py
+-rw-r--r--   0        0        0      821 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/support/trino.py
+-rw-r--r--   0        0        0       25 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/telemetry/__init__.py
+-rw-r--r--   0        0        0    10813 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/telemetry/telemetry.py
+-rw-r--r--   0        0        0     6572 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/teleport.py
+-rw-r--r--   0        0        0     1153 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/teleport_adapter_support.py
+-rw-r--r--   0        0        0     4719 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/teleport_support/duckdb.py
+-rw-r--r--   0        0        0     2972 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/teleport_support/snowflake.py
+-rw-r--r--   0        0        0     1256 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/utils/__init__.py
+-rw-r--r--   0        0        0     9804 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/utils/environments.py
+-rw-r--r--   0        0        0     1970 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/adapters/fal_experimental/utils/yaml_helper.py
+-rw-r--r--   0        0        0      208 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/fal/adapters/python/__init__.py
+-rw-r--r--   0        0        0    11898 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/fal/adapters/python/connections.py
+-rw-r--r--   0        0        0    10015 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/fal/adapters/python/impl.py
+-rw-r--r--   0        0        0      181 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/fal/adapters/teleport/__init__.py
+-rw-r--r--   0        0        0     3498 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/fal/adapters/teleport/impl.py
+-rw-r--r--   0        0        0     2310 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/fal/adapters/teleport/info.py
+-rw-r--r--   0        0        0       52 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/include/fal/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/include/fal/dbt_project.yml
+-rw-r--r--   0        0        0     1213 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/include/fal/macros/materializations/table.sql
+-rw-r--r--   0        0        0      265 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/include/fal/macros/teleport_duckdb.sql
+-rw-r--r--   0        0        0      921 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/include/fal/macros/teleport_snowflake.sql
+-rw-r--r--   0        0        0       52 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/include/fal_experimental/__init__.py
+-rw-r--r--   0        0        0       83 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/include/fal_experimental/dbt_project.yml
+-rw-r--r--   0        0        0      989 2023-07-17 22:49:47.495137 fal-0.9.5/src/dbt/include/fal_experimental/macros/materializations/table.sql
+-rw-r--r--   0        0        0     1905 2023-07-17 22:49:47.495137 fal-0.9.5/src/fal/__init__.py
+-rw-r--r--   0        0        0      238 2023-07-17 22:49:47.495137 fal-0.9.5/src/fal/dbt/__init__.py
+-rw-r--r--   0        0        0       30 2023-07-17 22:49:47.495137 fal-0.9.5/src/fal/dbt/cli/__init__.py
+-rw-r--r--   0        0        0     7650 2023-07-17 22:49:47.495137 fal-0.9.5/src/fal/dbt/cli/args.py
+-rw-r--r--   0        0        0     1550 2023-07-17 22:49:47.495137 fal-0.9.5/src/fal/dbt/cli/cli.py
+-rw-r--r--   0        0        0     5482 2023-07-17 22:49:47.495137 fal-0.9.5/src/fal/dbt/cli/dbt_runner.py
+-rw-r--r--   0        0        0     5857 2023-07-17 22:49:47.495137 fal-0.9.5/src/fal/dbt/cli/fal_runner.py
+-rw-r--r--   0        0        0     4475 2023-07-17 22:49:47.495137 fal-0.9.5/src/fal/dbt/cli/flow_runner.py
+-rw-r--r--   0        0        0       56 2023-07-17 22:49:47.495137 fal-0.9.5/src/fal/dbt/cli/model_generator/__init__.py
+-rw-r--r--   0        0        0     5543 2023-07-17 22:49:47.495137 fal-0.9.5/src/fal/dbt/cli/model_generator/model_generator.py
+-rw-r--r--   0        0        0     3180 2023-07-17 22:49:47.495137 fal-0.9.5/src/fal/dbt/cli/model_generator/module_check.py
+-rw-r--r--   0        0        0     9759 2023-07-17 22:49:47.495137 fal-0.9.5/src/fal/dbt/cli/selectors.py
+-rw-r--r--   0        0        0    12349 2023-07-17 22:49:47.495137 fal-0.9.5/src/fal/dbt/fal_script.py
+-rw-r--r--   0        0        0        0 2023-07-17 22:49:47.495137 fal-0.9.5/src/fal/dbt/feature_store/__init__.py
+-rw-r--r--   0        0        0      401 2023-07-17 22:49:47.495137 fal-0.9.5/src/fal/dbt/feature_store/feature.py
+-rw-r--r--   0        0        0        0 2023-07-17 22:49:47.495137 fal-0.9.5/src/fal/dbt/integration/__init__.py
+-rw-r--r--   0        0        0    24589 2023-07-17 22:49:47.495137 fal-0.9.5/src/fal/dbt/integration/lib.py
+-rw-r--r--   0        0        0     3273 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/integration/logger.py
+-rw-r--r--   0        0        0     1867 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/integration/magics.py
+-rw-r--r--   0        0        0     9103 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/integration/parse.py
+-rw-r--r--   0        0        0    27168 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/integration/project.py
+-rw-r--r--   0        0        0        0 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/integration/utils/__init__.py
+-rw-r--r--   0        0        0     1970 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/integration/utils/yaml_helper.py
+-rw-r--r--   0        0        0      317 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/integration/version.py
+-rw-r--r--   0        0        0     1530 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/new/project.py
+-rw-r--r--   0        0        0     8411 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/node_graph.py
+-rw-r--r--   0        0        0        0 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/packages/__init__.py
+-rw-r--r--   0        0        0     1603 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/packages/bridge.py
+-rw-r--r--   0        0        0     5562 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/packages/dependency_analysis.py
+-rw-r--r--   0        0        0      805 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/packages/environments/__init__.py
+-rw-r--r--   0        0        0     9499 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/packages/environments/base.py
+-rw-r--r--   0        0        0     4407 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/packages/environments/conda.py
+-rw-r--r--   0        0        0     3381 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/packages/environments/virtual_env.py
+-rw-r--r--   0        0        0     4823 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/packages/isolated_runner.py
+-rw-r--r--   0        0        0        0 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/planner/__init__.py
+-rw-r--r--   0        0        0     5669 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/planner/executor.py
+-rw-r--r--   0        0        0     6496 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/planner/plan.py
+-rw-r--r--   0        0        0     6790 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/planner/schedule.py
+-rw-r--r--   0        0        0     9079 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/planner/tasks.py
+-rw-r--r--   0        0        0        0 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/telemetry/__init__.py
+-rw-r--r--   0        0        0    11487 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/telemetry/telemetry.py
+-rw-r--r--   0        0        0     3060 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/typing.py
+-rw-r--r--   0        0        0     1728 2023-07-17 22:49:47.499137 fal-0.9.5/src/fal/dbt/utils.py
+-rw-r--r--   0        0        0       33 2023-07-17 22:49:47.499137 fal-0.9.5/tests/_fal_testing/__init__.py
+-rw-r--r--   0        0        0     1794 2023-07-17 22:49:47.499137 fal-0.9.5/tests/_fal_testing/utils.py
+-rw-r--r--   0        0        0    12552 1970-01-01 00:00:00.000000 fal-0.9.5/PKG-INFO
```

### Comparing `fal-0.9.4/README.md` & `fal-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/pyproject.toml` & `fal-0.9.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 # name = "dbt-fal"
 # version = "1.5.6a0"
 name = "fal"
-version = "0.9.4"
+version = "0.9.5"
 description = "Run python scripts from any dbt project."
 readme = "README.md"
 homepage = "https://github.com/fal-ai/fal"
 repository = "https://github.com/fal-ai/fal"
 authors = [ "Features & Labels <hello@fal.ai>" ]
 packages = [
     { include = "dbt", from = "src" },
```

### Comparing `fal-0.9.4/src/dbt/adapters/fal/__init__.py` & `fal-0.9.5/src/dbt/adapters/fal/__init__.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/dbt/adapters/fal/impl.py` & `fal-0.9.5/src/dbt/adapters/fal/impl.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/dbt/adapters/fal/load_db_profile.py` & `fal-0.9.5/src/dbt/adapters/fal/load_db_profile.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/dbt/adapters/fal/wrappers.py` & `fal-0.9.5/src/dbt/adapters/fal/wrappers.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/dbt/adapters/fal_experimental/adapter.py` & `fal-0.9.5/src/dbt/adapters/fal_experimental/adapter.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/dbt/adapters/fal_experimental/adapter_support.py` & `fal-0.9.5/src/dbt/adapters/fal_experimental/adapter_support.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/dbt/adapters/fal_experimental/connections.py` & `fal-0.9.5/src/dbt/adapters/fal_experimental/connections.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/dbt/adapters/fal_experimental/impl.py` & `fal-0.9.5/src/dbt/adapters/fal_experimental/impl.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/dbt/adapters/fal_experimental/support/athena.py` & `fal-0.9.5/src/dbt/adapters/fal_experimental/support/athena.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/dbt/adapters/fal_experimental/support/bigquery.py` & `fal-0.9.5/src/dbt/adapters/fal_experimental/support/bigquery.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/dbt/adapters/fal_experimental/support/duckdb.py` & `fal-0.9.5/src/dbt/adapters/fal_experimental/support/duckdb.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/dbt/adapters/fal_experimental/support/postgres.py` & `fal-0.9.5/src/dbt/adapters/fal_experimental/support/postgres.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/dbt/adapters/fal_experimental/support/redshift.py` & `fal-0.9.5/src/dbt/adapters/fal_experimental/support/redshift.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/dbt/adapters/fal_experimental/support/snowflake.py` & `fal-0.9.5/src/dbt/adapters/fal_experimental/support/snowflake.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/dbt/adapters/fal_experimental/support/trino.py` & `fal-0.9.5/src/dbt/adapters/fal_experimental/support/trino.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/dbt/adapters/fal_experimental/telemetry/telemetry.py` & `fal-0.9.5/src/dbt/adapters/fal_experimental/telemetry/telemetry.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,29 +103,29 @@
     return platform.system()
 
 
 def dbt_installed_version():
     """Returns: dbt version"""
     try:
         return pkg_resources.get_distribution("dbt-core").version
-    except ImportError:
+    except pkg_resources.DistributionNotFound:
         return
 
 
 def get_dbt_adapter_type(config: RuntimeConfig) -> str:
     """Returns: the configured actual DBT adapter"""
     target = config.to_target_dict()
     return target["type"]
 
 
 def fal_installed_version():
     """Returns: fal version"""
     try:
         return pkg_resources.get_distribution("dbt-fal").version
-    except ImportError:
+    except pkg_resources.DistributionNotFound:
         return
 
 
 def is_airflow():
     """Returns: True for Airflow env"""
     return "AIRFLOW_CONFIG" in os.environ or "AIRFLOW_HOME" in os.environ
```

### Comparing `fal-0.9.4/src/dbt/adapters/fal_experimental/teleport.py` & `fal-0.9.5/src/dbt/adapters/fal_experimental/teleport.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/dbt/adapters/fal_experimental/teleport_adapter_support.py` & `fal-0.9.5/src/dbt/adapters/fal_experimental/teleport_adapter_support.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/dbt/adapters/fal_experimental/teleport_support/duckdb.py` & `fal-0.9.5/src/dbt/adapters/fal_experimental/teleport_support/duckdb.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/dbt/adapters/fal_experimental/teleport_support/snowflake.py` & `fal-0.9.5/src/dbt/adapters/fal_experimental/teleport_support/snowflake.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/dbt/adapters/fal_experimental/utils/__init__.py` & `fal-0.9.5/src/dbt/adapters/fal_experimental/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/dbt/adapters/fal_experimental/utils/environments.py` & `fal-0.9.5/src/dbt/adapters/fal_experimental/utils/environments.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/dbt/adapters/fal_experimental/utils/yaml_helper.py` & `fal-0.9.5/src/dbt/adapters/fal_experimental/utils/yaml_helper.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/dbt/fal/adapters/python/connections.py` & `fal-0.9.5/src/dbt/fal/adapters/python/connections.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/dbt/fal/adapters/python/impl.py` & `fal-0.9.5/src/dbt/fal/adapters/python/impl.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/dbt/fal/adapters/teleport/impl.py` & `fal-0.9.5/src/dbt/fal/adapters/teleport/impl.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/dbt/fal/adapters/teleport/info.py` & `fal-0.9.5/src/dbt/fal/adapters/teleport/info.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/dbt/include/fal/macros/materializations/table.sql` & `fal-0.9.5/src/dbt/include/fal/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/dbt/include/fal/macros/teleport_snowflake.sql` & `fal-0.9.5/src/dbt/include/fal/macros/teleport_snowflake.sql`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/dbt/include/fal_experimental/macros/materializations/table.sql` & `fal-0.9.5/src/dbt/include/fal_experimental/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/fal/__init__.py` & `fal-0.9.5/src/fal/__init__.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/fal/dbt/cli/args.py` & `fal-0.9.5/src/fal/dbt/cli/args.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/fal/dbt/cli/cli.py` & `fal-0.9.5/src/fal/dbt/cli/cli.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/fal/dbt/cli/dbt_runner.py` & `fal-0.9.5/src/fal/dbt/cli/dbt_runner.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/fal/dbt/cli/fal_runner.py` & `fal-0.9.5/src/fal/dbt/cli/fal_runner.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/fal/dbt/cli/flow_runner.py` & `fal-0.9.5/src/fal/dbt/cli/flow_runner.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/fal/dbt/cli/model_generator/model_generator.py` & `fal-0.9.5/src/fal/dbt/cli/model_generator/model_generator.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/fal/dbt/cli/model_generator/module_check.py` & `fal-0.9.5/src/fal/dbt/cli/model_generator/module_check.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/fal/dbt/cli/selectors.py` & `fal-0.9.5/src/fal/dbt/cli/selectors.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/fal/dbt/fal_script.py` & `fal-0.9.5/src/fal/dbt/fal_script.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/fal/dbt/integration/lib.py` & `fal-0.9.5/src/fal/dbt/integration/lib.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/fal/dbt/integration/logger.py` & `fal-0.9.5/src/fal/dbt/integration/logger.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/fal/dbt/integration/magics.py` & `fal-0.9.5/src/fal/dbt/integration/magics.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/fal/dbt/integration/parse.py` & `fal-0.9.5/src/fal/dbt/integration/parse.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/fal/dbt/integration/project.py` & `fal-0.9.5/src/fal/dbt/integration/project.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/fal/dbt/integration/utils/yaml_helper.py` & `fal-0.9.5/src/fal/dbt/integration/utils/yaml_helper.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/fal/dbt/new/project.py` & `fal-0.9.5/src/fal/dbt/new/project.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/fal/dbt/node_graph.py` & `fal-0.9.5/src/fal/dbt/node_graph.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/fal/dbt/packages/bridge.py` & `fal-0.9.5/src/fal/dbt/packages/bridge.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/fal/dbt/packages/dependency_analysis.py` & `fal-0.9.5/src/fal/dbt/packages/dependency_analysis.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/fal/dbt/packages/environments/__init__.py` & `fal-0.9.5/src/fal/dbt/packages/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/fal/dbt/packages/environments/base.py` & `fal-0.9.5/src/fal/dbt/packages/environments/base.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/fal/dbt/packages/environments/conda.py` & `fal-0.9.5/src/fal/dbt/packages/environments/conda.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/fal/dbt/packages/environments/virtual_env.py` & `fal-0.9.5/src/fal/dbt/packages/environments/virtual_env.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/fal/dbt/packages/isolated_runner.py` & `fal-0.9.5/src/fal/dbt/packages/isolated_runner.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/fal/dbt/planner/executor.py` & `fal-0.9.5/src/fal/dbt/planner/executor.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/fal/dbt/planner/plan.py` & `fal-0.9.5/src/fal/dbt/planner/plan.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/fal/dbt/planner/schedule.py` & `fal-0.9.5/src/fal/dbt/planner/schedule.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/fal/dbt/planner/tasks.py` & `fal-0.9.5/src/fal/dbt/planner/tasks.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/fal/dbt/telemetry/telemetry.py` & `fal-0.9.5/src/fal/dbt/telemetry/telemetry.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     return platform.system()
 
 
 def dbt_installed_version():
     """Returns: dbt version"""
     try:
         return pkg_resources.get_distribution("dbt-core").version
-    except ImportError:
+    except pkg_resources.DistributionNotFound:
         return
 
 
 def get_dbt_adapter_type(config: RuntimeConfig | None) -> str | None:
     """Returns: the configured DBT adapter or None if it's not in a runner context"""
     if config is not None:
         target = config.to_target_dict()
@@ -124,15 +124,15 @@
     return None
 
 
 def fal_installed_version():
     """Returns: fal version"""
     try:
         return pkg_resources.get_distribution("dbt-fal").version
-    except ImportError:
+    except pkg_resources.DistributionNotFound:
         return
 
 
 def is_airflow():
     """Returns: True for Airflow env"""
     return "AIRFLOW_CONFIG" in os.environ or "AIRFLOW_HOME" in os.environ
```

### Comparing `fal-0.9.4/src/fal/dbt/typing.py` & `fal-0.9.5/src/fal/dbt/typing.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/src/fal/dbt/utils.py` & `fal-0.9.5/src/fal/dbt/utils.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/tests/_fal_testing/utils.py` & `fal-0.9.5/tests/_fal_testing/utils.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.4/PKG-INFO` & `fal-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fal
-Version: 0.9.4
+Version: 0.9.5
 Summary: Run python scripts from any dbt project.
 Home-page: https://github.com/fal-ai/fal
 Keywords: dbt,pandas,fal,runtime
 Author: Features & Labels
 Author-email: hello@fal.ai
 Requires-Python: >=3.7.2,<3.12
 Classifier: Development Status :: 4 - Beta
```

