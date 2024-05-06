# Comparing `tmp/dbt-materialize-1.7.7.tar.gz` & `tmp/dbt-materialize-1.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-materialize-1.7.7.tar", last modified: Sat Apr 20 00:25:53 2024, max compression
+gzip compressed data, was "dbt-materialize-1.7.8.tar", last modified: Mon May  6 17:47:50 2024, max compression
```

## Comparing `dbt-materialize-1.7.7.tar` & `dbt-materialize-1.7.8.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-20 00:25:53.288179 dbt-materialize-1.7.7/
--rw-r--r--   0 materialize  (2000) materialize   (993)      424 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/MANIFEST.in
--rw-r--r--   0 materialize  (2000) materialize   (993)     6613 2024-04-20 00:25:53.288179 dbt-materialize-1.7.7/PKG-INFO
--rw-r--r--   0 materialize  (2000) materialize   (993)     6292 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/README.md
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-20 00:25:53.278179 dbt-materialize-1.7.7/dbt/
--rw-r--r--   0 materialize  (2000) materialize   (993)      729 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/__init__.py
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-20 00:25:53.278179 dbt-materialize-1.7.7/dbt/adapters/
--rw-r--r--   0 materialize  (2000) materialize   (993)      729 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/adapters/__init__.py
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-20 00:25:53.278179 dbt-materialize-1.7.7/dbt/adapters/materialize/
--rw-r--r--   0 materialize  (2000) materialize   (993)     1125 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/adapters/materialize/__init__.py
--rw-r--r--   0 materialize  (2000) materialize   (993)      801 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/adapters/materialize/__version__.py
--rw-r--r--   0 materialize  (2000) materialize   (993)     5553 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/adapters/materialize/connections.py
--rw-r--r--   0 materialize  (2000) materialize   (993)     1598 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/adapters/materialize/exceptions.py
--rw-r--r--   0 materialize  (2000) materialize   (993)    11918 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/adapters/materialize/impl.py
--rw-r--r--   0 materialize  (2000) materialize   (993)     2284 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/adapters/materialize/relation.py
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-20 00:25:53.278179 dbt-materialize-1.7.7/dbt/include/
--rw-r--r--   0 materialize  (2000) materialize   (993)      729 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/__init__.py
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-20 00:25:53.278179 dbt-materialize-1.7.7/dbt/include/materialize/
--rw-r--r--   0 materialize  (2000) materialize   (993)      782 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/__init__.py
--rw-r--r--   0 materialize  (2000) materialize   (993)      808 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/dbt_project.yml
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-20 00:25:53.278179 dbt-materialize-1.7.7/dbt/include/materialize/macros/
--rw-r--r--   0 materialize  (2000) materialize   (993)     9472 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/adapters.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     2592 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/catalog.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)      979 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/columns.sql
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-20 00:25:53.278179 dbt-materialize-1.7.7/dbt/include/materialize/macros/deploy/
--rw-r--r--   0 materialize  (2000) materialize   (993)     1711 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/deploy/deploy_await.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1981 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/deploy/deploy_cleanup.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)    12165 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/deploy/deploy_init.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     6053 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/deploy/deploy_permission_validation.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     5361 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/deploy/deploy_promote.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)      989 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/freshness.sql
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-20 00:25:53.278179 dbt-materialize-1.7.7/dbt/include/materialize/macros/materializations/
--rw-r--r--   0 materialize  (2000) materialize   (993)     1911 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/materializations/incremental.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1922 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/materializations/materialized_view.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1224 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/materializations/materializedview.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1970 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/materializations/sink.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1835 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/materializations/source.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1974 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/materializations/table.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     2828 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/materializations/test.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1883 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/materializations/view.sql
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-20 00:25:53.278179 dbt-materialize-1.7.7/dbt/include/materialize/macros/tests/
--rw-r--r--   0 materialize  (2000) materialize   (993)     1033 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/tests/helpers.sql
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-20 00:25:53.278179 dbt-materialize-1.7.7/dbt/include/materialize/macros/utils/
--rw-r--r--   0 materialize  (2000) materialize   (993)     1151 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/utils/await_cluster_ready.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     3245 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/utils/ci_utils.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1986 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/utils/exists.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)      887 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/utils/generate_cluster_name.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1285 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/utils/generate_schema_name.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     5211 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/utils/is_cluster_ready.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1016 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/macros/utils/listagg.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1257 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/profile_template.yml
--rw-r--r--   0 materialize  (2000) materialize   (993)     1277 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/materialize/sample_profiles.yml
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-20 00:25:53.278179 dbt-materialize-1.7.7/dbt/include/starter_project/
--rw-r--r--   0 materialize  (2000) materialize   (993)      917 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/starter_project/dbt_project.yml
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-20 00:25:53.278179 dbt-materialize-1.7.7/dbt/include/starter_project/models/
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-20 00:25:53.288179 dbt-materialize-1.7.7/dbt/include/starter_project/models/example/
--rw-r--r--   0 materialize  (2000) materialize   (993)      972 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/starter_project/models/example/fraud_activity.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)      999 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/starter_project/models/example/funds_movement.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)      936 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/starter_project/models/example/my_first_dbt_model.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)      753 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/starter_project/models/example/my_second_dbt_model.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     2822 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/starter_project/models/example/schema.yml
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-20 00:25:53.288179 dbt-materialize-1.7.7/dbt/include/starter_project/models/example/sources/
--rw-r--r--   0 materialize  (2000) materialize   (993)      774 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/starter_project/models/example/sources/auction.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)      866 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/starter_project/models/example/sources/sources.yml
--rw-r--r--   0 materialize  (2000) materialize   (993)     1068 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/dbt/include/starter_project/models/example/winning_bids.sql
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-04-20 00:25:53.288179 dbt-materialize-1.7.7/dbt_materialize.egg-info/
--rw-r--r--   0 materialize  (2000) materialize   (993)     6613 2024-04-20 00:25:53.000000 dbt-materialize-1.7.7/dbt_materialize.egg-info/PKG-INFO
--rw-r--r--   0 materialize  (2000) materialize   (993)     2636 2024-04-20 00:25:53.000000 dbt-materialize-1.7.7/dbt_materialize.egg-info/SOURCES.txt
--rw-r--r--   0 materialize  (2000) materialize   (993)        1 2024-04-20 00:25:53.000000 dbt-materialize-1.7.7/dbt_materialize.egg-info/dependency_links.txt
--rw-r--r--   0 materialize  (2000) materialize   (993)       52 2024-04-20 00:25:53.000000 dbt-materialize-1.7.7/dbt_materialize.egg-info/requires.txt
--rw-r--r--   0 materialize  (2000) materialize   (993)        4 2024-04-20 00:25:53.000000 dbt-materialize-1.7.7/dbt_materialize.egg-info/top_level.txt
--rw-r--r--   0 materialize  (2000) materialize   (993)      464 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/pyproject.toml
--rw-r--r--   0 materialize  (2000) materialize   (993)       38 2024-04-20 00:25:53.288179 dbt-materialize-1.7.7/setup.cfg
--rw-r--r--   0 materialize  (2000) materialize   (993)     1814 2024-04-20 00:23:38.000000 dbt-materialize-1.7.7/setup.py
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-06 17:47:50.728657 dbt-materialize-1.7.8/
+-rw-r--r--   0 materialize  (2000) materialize   (993)      424 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/MANIFEST.in
+-rw-r--r--   0 materialize  (2000) materialize   (993)     6613 2024-05-06 17:47:50.728657 dbt-materialize-1.7.8/PKG-INFO
+-rw-r--r--   0 materialize  (2000) materialize   (993)     6292 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/README.md
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-06 17:47:50.728657 dbt-materialize-1.7.8/dbt/
+-rw-r--r--   0 materialize  (2000) materialize   (993)      729 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/__init__.py
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-06 17:47:50.728657 dbt-materialize-1.7.8/dbt/adapters/
+-rw-r--r--   0 materialize  (2000) materialize   (993)      729 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/adapters/__init__.py
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-06 17:47:50.728657 dbt-materialize-1.7.8/dbt/adapters/materialize/
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1125 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/adapters/materialize/__init__.py
+-rw-r--r--   0 materialize  (2000) materialize   (993)      801 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/adapters/materialize/__version__.py
+-rw-r--r--   0 materialize  (2000) materialize   (993)     5553 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/adapters/materialize/connections.py
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1598 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/adapters/materialize/exceptions.py
+-rw-r--r--   0 materialize  (2000) materialize   (993)    11918 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/adapters/materialize/impl.py
+-rw-r--r--   0 materialize  (2000) materialize   (993)     2284 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/adapters/materialize/relation.py
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-06 17:47:50.728657 dbt-materialize-1.7.8/dbt/include/
+-rw-r--r--   0 materialize  (2000) materialize   (993)      729 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/__init__.py
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-06 17:47:50.728657 dbt-materialize-1.7.8/dbt/include/materialize/
+-rw-r--r--   0 materialize  (2000) materialize   (993)      782 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/__init__.py
+-rw-r--r--   0 materialize  (2000) materialize   (993)      808 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/dbt_project.yml
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-06 17:47:50.728657 dbt-materialize-1.7.8/dbt/include/materialize/macros/
+-rw-r--r--   0 materialize  (2000) materialize   (993)     9472 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/adapters.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     2592 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/catalog.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)      979 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/columns.sql
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-06 17:47:50.728657 dbt-materialize-1.7.8/dbt/include/materialize/macros/deploy/
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1711 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/deploy/deploy_await.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1981 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/deploy/deploy_cleanup.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)    12199 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/deploy/deploy_init.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     6053 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/deploy/deploy_permission_validation.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     5361 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/deploy/deploy_promote.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)      989 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/freshness.sql
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-06 17:47:50.728657 dbt-materialize-1.7.8/dbt/include/materialize/macros/materializations/
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1911 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/materializations/incremental.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1922 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/materializations/materialized_view.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1224 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/materializations/materializedview.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1970 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/materializations/sink.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1835 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/materializations/source.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1974 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/materializations/table.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     2828 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/materializations/test.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1883 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/materializations/view.sql
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-06 17:47:50.728657 dbt-materialize-1.7.8/dbt/include/materialize/macros/tests/
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1033 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/tests/helpers.sql
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-06 17:47:50.728657 dbt-materialize-1.7.8/dbt/include/materialize/macros/utils/
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1151 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/utils/await_cluster_ready.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     3245 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/utils/ci_utils.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1986 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/utils/exists.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)      887 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/utils/generate_cluster_name.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1285 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/utils/generate_schema_name.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     5211 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/utils/is_cluster_ready.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1016 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/utils/listagg.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1257 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/profile_template.yml
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1277 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/sample_profiles.yml
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-06 17:47:50.728657 dbt-materialize-1.7.8/dbt/include/starter_project/
+-rw-r--r--   0 materialize  (2000) materialize   (993)      917 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/starter_project/dbt_project.yml
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-06 17:47:50.728657 dbt-materialize-1.7.8/dbt/include/starter_project/models/
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-06 17:47:50.728657 dbt-materialize-1.7.8/dbt/include/starter_project/models/example/
+-rw-r--r--   0 materialize  (2000) materialize   (993)      972 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/starter_project/models/example/fraud_activity.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)      999 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/starter_project/models/example/funds_movement.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)      936 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/starter_project/models/example/my_first_dbt_model.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)      753 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/starter_project/models/example/my_second_dbt_model.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     2822 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/starter_project/models/example/schema.yml
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-06 17:47:50.728657 dbt-materialize-1.7.8/dbt/include/starter_project/models/example/sources/
+-rw-r--r--   0 materialize  (2000) materialize   (993)      774 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/starter_project/models/example/sources/auction.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)      866 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/starter_project/models/example/sources/sources.yml
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1068 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/starter_project/models/example/winning_bids.sql
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-06 17:47:50.728657 dbt-materialize-1.7.8/dbt_materialize.egg-info/
+-rw-r--r--   0 materialize  (2000) materialize   (993)     6613 2024-05-06 17:47:50.000000 dbt-materialize-1.7.8/dbt_materialize.egg-info/PKG-INFO
+-rw-r--r--   0 materialize  (2000) materialize   (993)     2636 2024-05-06 17:47:50.000000 dbt-materialize-1.7.8/dbt_materialize.egg-info/SOURCES.txt
+-rw-r--r--   0 materialize  (2000) materialize   (993)        1 2024-05-06 17:47:50.000000 dbt-materialize-1.7.8/dbt_materialize.egg-info/dependency_links.txt
+-rw-r--r--   0 materialize  (2000) materialize   (993)       52 2024-05-06 17:47:50.000000 dbt-materialize-1.7.8/dbt_materialize.egg-info/requires.txt
+-rw-r--r--   0 materialize  (2000) materialize   (993)        4 2024-05-06 17:47:50.000000 dbt-materialize-1.7.8/dbt_materialize.egg-info/top_level.txt
+-rw-r--r--   0 materialize  (2000) materialize   (993)      464 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/pyproject.toml
+-rw-r--r--   0 materialize  (2000) materialize   (993)       38 2024-05-06 17:47:50.728657 dbt-materialize-1.7.8/setup.cfg
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1814 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/setup.py
```

### Comparing `dbt-materialize-1.7.7/PKG-INFO` & `dbt-materialize-1.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-materialize
-Version: 1.7.7
+Version: 1.7.8
 Summary: The Materialize adapter plugin for dbt.
 Home-page: https://github.com/MaterializeInc/materialize/blob/main/misc/dbt-materialize
 Author: Materialize, Inc.
 Author-email: support@materialize.com
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `dbt-materialize-1.7.7/README.md` & `dbt-materialize-1.7.8/README.md`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/__init__.py` & `dbt-materialize-1.7.8/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/adapters/__init__.py` & `dbt-materialize-1.7.8/dbt/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/adapters/materialize/__init__.py` & `dbt-materialize-1.7.8/dbt/adapters/materialize/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/adapters/materialize/__version__.py` & `dbt-materialize-1.7.8/dbt/adapters/materialize/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # If you bump this version, bump it in setup.py too.
-version = "1.7.7"
+version = "1.7.8"
```

### Comparing `dbt-materialize-1.7.7/dbt/adapters/materialize/connections.py` & `dbt-materialize-1.7.8/dbt/adapters/materialize/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/adapters/materialize/exceptions.py` & `dbt-materialize-1.7.8/dbt/adapters/materialize/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/adapters/materialize/impl.py` & `dbt-materialize-1.7.8/dbt/adapters/materialize/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/adapters/materialize/relation.py` & `dbt-materialize-1.7.8/dbt/adapters/materialize/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/include/__init__.py` & `dbt-materialize-1.7.8/dbt/include/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/include/materialize/__init__.py` & `dbt-materialize-1.7.8/dbt/include/materialize/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/include/materialize/dbt_project.yml` & `dbt-materialize-1.7.8/dbt/include/materialize/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/include/materialize/macros/adapters.sql` & `dbt-materialize-1.7.8/dbt/include/materialize/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/include/materialize/macros/catalog.sql` & `dbt-materialize-1.7.8/dbt/include/materialize/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/include/materialize/macros/columns.sql` & `dbt-materialize-1.7.8/dbt/include/materialize/macros/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/include/materialize/macros/deploy/deploy_await.sql` & `dbt-materialize-1.7.8/dbt/include/materialize/macros/deploy/deploy_await.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/include/materialize/macros/deploy/deploy_cleanup.sql` & `dbt-materialize-1.7.8/dbt/include/materialize/macros/deploy/deploy_cleanup.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/include/materialize/macros/deploy/deploy_init.sql` & `dbt-materialize-1.7.8/dbt/include/materialize/macros/deploy/deploy_init.sql`

 * *Files 2% similar despite different names*

```diff
@@ -194,29 +194,29 @@
 {% macro internal_copy_schema_default_privs(from, to) %}
 
 {% set find_default_privs %}
 SELECT
   'ALTER DEFAULT PRIVILEGES ' ||
   CASE
     WHEN object_owner = 'PUBLIC' THEN 'FOR ALL ROLES '
-    ELSE 'FOR ROLE ' || object_owner
+    ELSE 'FOR ROLE ' || quote_ident(object_owner) || ' '
   END ||
   'IN SCHEMA {{ to }} '         ||
   'GRANT '  || privilege_type   || ' ' ||
   'ON '     || object_type      || 's ' ||
-  'TO '     || grantee
+  'TO '     || quote_ident(grantee)
 FROM mz_internal.mz_show_default_privileges
 WHERE database = current_database() AND schema = {{ dbt.string_literal(from) }}
     AND object_owner <> 'none' AND grantee <> 'none'
 {% endset %}
 
 {% set alter_defaults = run_query(find_default_privs) %}
 {% if execute %}
     {% for alter in alter_defaults.rows %}
-        {{ run_query(alter) }}
+        {{ run_query(alter[0]) }}
     {% endfor %}
 {% endif %}
 {% endmacro %}
 
 {% macro internal_copy_schema_grants(from, to) %}
 {% set find_revokes %}
 WITH schema_privilege AS (
@@ -269,15 +269,15 @@
 {% endmacro %}
 
 {% macro internal_copy_cluster_grants(from, to) %}
 {% set find_revokes %}
 WITH cluster_privilege AS (
     SELECT mz_internal.mz_aclexplode(privileges).*
     FROM mz_clusters
-    WHERE name = {{ dbt.string_literal(from) }}
+    WHERE name = {{ dbt.string_literal(to) }}
 )
 
 SELECT 'REVOKE '     || c.privilege_type || ' ' ||
        'ON CLUSTER ' || quote_ident({{ dbt.string_literal(to) }}) || ' ' ||
        'FROM '       || quote_ident(grantee.name)
 FROM cluster_privilege AS c
 JOIN mz_roles AS grantee ON c.grantee = grantee.id
```

### Comparing `dbt-materialize-1.7.7/dbt/include/materialize/macros/deploy/deploy_permission_validation.sql` & `dbt-materialize-1.7.8/dbt/include/materialize/macros/deploy/deploy_permission_validation.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/include/materialize/macros/deploy/deploy_promote.sql` & `dbt-materialize-1.7.8/dbt/include/materialize/macros/deploy/deploy_promote.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/include/materialize/macros/freshness.sql` & `dbt-materialize-1.7.8/dbt/include/materialize/macros/freshness.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/include/materialize/macros/materializations/incremental.sql` & `dbt-materialize-1.7.8/dbt/include/materialize/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/include/materialize/macros/materializations/materialized_view.sql` & `dbt-materialize-1.7.8/dbt/include/materialize/macros/materializations/materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/include/materialize/macros/materializations/materializedview.sql` & `dbt-materialize-1.7.8/dbt/include/materialize/macros/materializations/materializedview.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/include/materialize/macros/materializations/sink.sql` & `dbt-materialize-1.7.8/dbt/include/materialize/macros/materializations/sink.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/include/materialize/macros/materializations/source.sql` & `dbt-materialize-1.7.8/dbt/include/materialize/macros/materializations/source.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/include/materialize/macros/materializations/table.sql` & `dbt-materialize-1.7.8/dbt/include/materialize/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/include/materialize/macros/materializations/test.sql` & `dbt-materialize-1.7.8/dbt/include/materialize/macros/materializations/test.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/include/materialize/macros/materializations/view.sql` & `dbt-materialize-1.7.8/dbt/include/materialize/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/include/materialize/macros/tests/helpers.sql` & `dbt-materialize-1.7.8/dbt/include/materialize/macros/tests/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/include/materialize/macros/utils/await_cluster_ready.sql` & `dbt-materialize-1.7.8/dbt/include/materialize/macros/utils/await_cluster_ready.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/include/materialize/macros/utils/ci_utils.sql` & `dbt-materialize-1.7.8/dbt/include/materialize/macros/utils/ci_utils.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/include/materialize/macros/utils/exists.sql` & `dbt-materialize-1.7.8/dbt/include/materialize/macros/utils/exists.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/include/materialize/macros/utils/generate_cluster_name.sql` & `dbt-materialize-1.7.8/dbt/include/materialize/macros/utils/generate_cluster_name.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/include/materialize/macros/utils/generate_schema_name.sql` & `dbt-materialize-1.7.8/dbt/include/materialize/macros/utils/generate_schema_name.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/include/materialize/macros/utils/is_cluster_ready.sql` & `dbt-materialize-1.7.8/dbt/include/materialize/macros/utils/is_cluster_ready.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/include/materialize/macros/utils/listagg.sql` & `dbt-materialize-1.7.8/dbt/include/materialize/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/include/materialize/profile_template.yml` & `dbt-materialize-1.7.8/dbt/include/materialize/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/include/materialize/sample_profiles.yml` & `dbt-materialize-1.7.8/dbt/include/materialize/sample_profiles.yml`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/include/starter_project/dbt_project.yml` & `dbt-materialize-1.7.8/dbt/include/starter_project/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/include/starter_project/models/example/fraud_activity.sql` & `dbt-materialize-1.7.8/dbt/include/starter_project/models/example/fraud_activity.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/include/starter_project/models/example/funds_movement.sql` & `dbt-materialize-1.7.8/dbt/include/starter_project/models/example/funds_movement.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/include/starter_project/models/example/my_first_dbt_model.sql` & `dbt-materialize-1.7.8/dbt/include/starter_project/models/example/my_first_dbt_model.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/include/starter_project/models/example/my_second_dbt_model.sql` & `dbt-materialize-1.7.8/dbt/include/starter_project/models/example/my_second_dbt_model.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/include/starter_project/models/example/schema.yml` & `dbt-materialize-1.7.8/dbt/include/starter_project/models/example/schema.yml`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/include/starter_project/models/example/sources/auction.sql` & `dbt-materialize-1.7.8/dbt/include/starter_project/models/example/sources/auction.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/include/starter_project/models/example/sources/sources.yml` & `dbt-materialize-1.7.8/dbt/include/starter_project/models/example/sources/sources.yml`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt/include/starter_project/models/example/winning_bids.sql` & `dbt-materialize-1.7.8/dbt/include/starter_project/models/example/winning_bids.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/dbt_materialize.egg-info/PKG-INFO` & `dbt-materialize-1.7.8/dbt_materialize.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-materialize
-Version: 1.7.7
+Version: 1.7.8
 Summary: The Materialize adapter plugin for dbt.
 Home-page: https://github.com/MaterializeInc/materialize/blob/main/misc/dbt-materialize
 Author: Materialize, Inc.
 Author-email: support@materialize.com
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `dbt-materialize-1.7.7/dbt_materialize.egg-info/SOURCES.txt` & `dbt-materialize-1.7.8/dbt_materialize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.7/setup.py` & `dbt-materialize-1.7.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 README = Path(__file__).parent / "README.md"
 
 setup(
     name="dbt-materialize",
     # This adapter's minor version should match the required dbt-postgres version,
     # but patch versions may differ.
     # If you bump this version, bump it in __version__.py too.
-    version="1.7.7",
+    version="1.7.8",
     description="The Materialize adapter plugin for dbt.",
     long_description=(Path(__file__).parent / "README.md").open().read(),
     long_description_content_type="text/markdown",
     author="Materialize, Inc.",
     author_email="support@materialize.com",
     url="https://github.com/MaterializeInc/materialize/blob/main/misc/dbt-materialize",
     packages=find_packages(),
```

