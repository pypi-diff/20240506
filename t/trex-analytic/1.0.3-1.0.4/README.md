# Comparing `tmp/trex-analytic-1.0.3.tar.gz` & `tmp/trex-analytic-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/trex-analytic-1.0.3.tar", last modified: Wed Nov  8 01:01:32 2023, max compression
+gzip compressed data, was "trex-analytic-1.0.4.tar", last modified: Mon May  6 09:50:53 2024, max compression
```

## Comparing `trex-analytic-1.0.3.tar` & `trex-analytic-1.0.4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-11-08 01:01:32.000000 trex-analytic-1.0.3/
--rw-r--r--   0 jacklok    (501) staff       (20)      359 2023-11-08 01:01:32.000000 trex-analytic-1.0.3/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)     2622 2021-01-11 01:11:49.000000 trex-analytic-1.0.3/README.md
--rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-11-08 01:01:32.000000 trex-analytic-1.0.3/setup.cfg
--rw-r--r--   0 jacklok    (501) staff       (20)      707 2023-11-08 01:01:01.000000 trex-analytic-1.0.3/setup.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-11-08 01:01:32.000000 trex-analytic-1.0.3/tests/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-11 08:40:47.000000 trex-analytic-1.0.3/tests/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      974 2021-01-18 02:08:03.000000 trex-analytic-1.0.3/tests/test_chart_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      559 2021-01-21 09:11:07.000000 trex-analytic-1.0.3/tests/test_cloud_tasks_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     3063 2021-01-20 07:30:52.000000 trex-analytic-1.0.3/tests/test_create_bigquery_table.py
--rw-r--r--   0 jacklok    (501) staff       (20)      595 2021-01-15 01:14:30.000000 trex-analytic-1.0.3/tests/test_delete_bigquery_dataset.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1325 2021-01-15 06:16:18.000000 trex-analytic-1.0.3/tests/test_import_customer_data.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2343 2021-01-20 01:23:38.000000 trex-analytic-1.0.3/tests/test_import_merchant_customer_data.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1320 2021-01-15 06:16:09.000000 trex-analytic-1.0.3/tests/test_import_merchant_data.py
--rw-r--r--   0 jacklok    (501) staff       (20)      748 2021-01-15 01:23:07.000000 trex-analytic-1.0.3/tests/test_list_table_from_dataset.py
--rw-r--r--   0 jacklok    (501) staff       (20)      380 2021-01-19 07:00:13.000000 trex-analytic-1.0.3/tests/test_main_app.py
--rw-r--r--   0 jacklok    (501) staff       (20)      922 2021-07-01 02:28:22.000000 trex-analytic-1.0.3/tests/test_query_customer.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-11-08 01:01:32.000000 trex-analytic-1.0.3/trex_analytic.egg-info/
--rw-r--r--   0 jacklok    (501) staff       (20)      359 2023-11-08 01:01:32.000000 trex-analytic-1.0.3/trex_analytic.egg-info/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)     1892 2023-11-08 01:01:32.000000 trex-analytic-1.0.3/trex_analytic.egg-info/SOURCES.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-11-08 01:01:32.000000 trex-analytic-1.0.3/trex_analytic.egg-info/dependency_links.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       98 2023-11-08 01:01:32.000000 trex-analytic-1.0.3/trex_analytic.egg-info/requires.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       20 2023-11-08 01:01:32.000000 trex-analytic-1.0.3/trex_analytic.egg-info/top_level.txt
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-11-08 01:01:32.000000 trex-analytic-1.0.3/trexanalytics/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-11 01:25:07.000000 trex-analytic-1.0.3/trexanalytics/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     9229 2023-02-10 11:21:00.000000 trex-analytic-1.0.3/trexanalytics/bigquery_table_template_config.py
--rw-r--r--   0 jacklok    (501) staff       (20)    19208 2023-11-07 12:40:36.000000 trex-analytic-1.0.3/trexanalytics/bigquery_upstream_data_config.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4484 2023-02-23 10:06:43.000000 trex-analytic-1.0.3/trexanalytics/conf.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-11-08 01:01:32.000000 trex-analytic-1.0.3/trexanalytics/controllers/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-11 01:45:04.000000 trex-analytic-1.0.3/trexanalytics/controllers/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-11-08 01:01:32.000000 trex-analytic-1.0.3/trexanalytics/controllers/bigquery/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-18 05:12:38.000000 trex-analytic-1.0.3/trexanalytics/controllers/bigquery/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)    14411 2023-03-07 02:42:00.000000 trex-analytic-1.0.3/trexanalytics/controllers/bigquery/customer_query_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2540 2023-03-07 04:22:38.000000 trex-analytic-1.0.3/trexanalytics/controllers/bigquery/query_base_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     5383 2021-07-01 02:13:45.000000 trex-analytic-1.0.3/trexanalytics/controllers/bigquery/redemption_query_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     5566 2021-07-01 02:13:41.000000 trex-analytic-1.0.3/trexanalytics/controllers/bigquery/rewarding_query_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    14535 2021-08-30 06:35:04.000000 trex-analytic-1.0.3/trexanalytics/controllers/bigquery/transaction_query_routes.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-11-08 01:01:32.000000 trex-analytic-1.0.3/trexanalytics/controllers/importdata/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-12 02:42:37.000000 trex-analytic-1.0.3/trexanalytics/controllers/importdata/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)    19860 2022-09-29 03:34:40.000000 trex-analytic-1.0.3/trexanalytics/controllers/importdata/import_customer_data_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    14404 2023-02-27 08:40:04.000000 trex-analytic-1.0.3/trexanalytics/controllers/importdata/import_data_base_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     6544 2021-08-20 10:27:07.000000 trex-analytic-1.0.3/trexanalytics/controllers/importdata/import_merchant_data_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     8306 2021-08-20 10:27:16.000000 trex-analytic-1.0.3/trexanalytics/controllers/importdata/import_transaction_data_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    17823 2023-02-27 07:41:18.000000 trex-analytic-1.0.3/trexanalytics/controllers/importdata/import_upstream_data_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)       49 2021-01-21 07:31:55.000000 trex-analytic-1.0.3/trexanalytics/controllers/importdata/import_user_data_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2473 2022-09-23 07:30:35.000000 trex-analytic-1.0.3/trexanalytics/controllers/main_routes.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-11-08 01:01:32.000000 trex-analytic-1.0.3/trexanalytics/controllers/template/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-11 06:02:49.000000 trex-analytic-1.0.3/trexanalytics/controllers/template/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      907 2021-01-20 09:34:38.000000 trex-analytic-1.0.3/trexanalytics/controllers/template/table_template_routes.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-11-08 01:01:32.000000 trex-analytic-1.0.3/trexanalytics/controllers/upstreamdata/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-26 10:02:40.000000 trex-analytic-1.0.3/trexanalytics/controllers/upstreamdata/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-11-08 01:01:32.000000 trex-analytic-1.0.3/trexanalytics/helper/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2023-03-27 04:02:29.000000 trex-analytic-1.0.3/trexanalytics/helper/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     3549 2023-03-27 10:56:12.000000 trex-analytic-1.0.3/trexanalytics/helper/bigquery_upstream_helpers.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-11-08 01:01:32.000000 trex-analytic-1.0.3/trexanalytics/util/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-11 06:16:58.000000 trex-analytic-1.0.3/trexanalytics/util/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      537 2021-01-18 02:07:17.000000 trex-analytic-1.0.3/trexanalytics/util/chart_util.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:50:53.669378 trex-analytic-1.0.4/
+-rw-r--r--   0 jacklok    (501) staff       (20)      502 2024-05-06 09:50:53.669199 trex-analytic-1.0.4/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)     2622 2021-01-11 01:11:49.000000 trex-analytic-1.0.4/README.md
+-rw-r--r--   0 jacklok    (501) staff       (20)       75 2024-05-06 09:50:53.670175 trex-analytic-1.0.4/setup.cfg
+-rw-r--r--   0 jacklok    (501) staff       (20)      707 2024-05-06 09:50:26.000000 trex-analytic-1.0.4/setup.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:50:53.643384 trex-analytic-1.0.4/tests/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-11 08:40:47.000000 trex-analytic-1.0.4/tests/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      974 2021-01-18 02:08:03.000000 trex-analytic-1.0.4/tests/test_chart_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      559 2021-01-21 09:11:07.000000 trex-analytic-1.0.4/tests/test_cloud_tasks_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     3063 2021-01-20 07:30:52.000000 trex-analytic-1.0.4/tests/test_create_bigquery_table.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      595 2021-01-15 01:14:30.000000 trex-analytic-1.0.4/tests/test_delete_bigquery_dataset.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1325 2021-01-15 06:16:18.000000 trex-analytic-1.0.4/tests/test_import_customer_data.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2343 2021-01-20 01:23:38.000000 trex-analytic-1.0.4/tests/test_import_merchant_customer_data.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1320 2021-01-15 06:16:09.000000 trex-analytic-1.0.4/tests/test_import_merchant_data.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      748 2021-01-15 01:23:07.000000 trex-analytic-1.0.4/tests/test_list_table_from_dataset.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      380 2021-01-19 07:00:13.000000 trex-analytic-1.0.4/tests/test_main_app.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      922 2021-07-01 02:28:22.000000 trex-analytic-1.0.4/tests/test_query_customer.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:50:53.668410 trex-analytic-1.0.4/trex_analytic.egg-info/
+-rw-r--r--   0 jacklok    (501) staff       (20)      502 2024-05-06 09:50:53.000000 trex-analytic-1.0.4/trex_analytic.egg-info/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)     1892 2024-05-06 09:50:53.000000 trex-analytic-1.0.4/trex_analytic.egg-info/SOURCES.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        1 2024-05-06 09:50:53.000000 trex-analytic-1.0.4/trex_analytic.egg-info/dependency_links.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       98 2024-05-06 09:50:53.000000 trex-analytic-1.0.4/trex_analytic.egg-info/requires.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       20 2024-05-06 09:50:53.000000 trex-analytic-1.0.4/trex_analytic.egg-info/top_level.txt
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:50:53.649386 trex-analytic-1.0.4/trexanalytics/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-11 01:25:07.000000 trex-analytic-1.0.4/trexanalytics/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     9229 2023-02-10 11:21:00.000000 trex-analytic-1.0.4/trexanalytics/bigquery_table_template_config.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    19208 2023-11-10 13:04:48.000000 trex-analytic-1.0.4/trexanalytics/bigquery_upstream_data_config.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4484 2023-02-23 10:06:43.000000 trex-analytic-1.0.4/trexanalytics/conf.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:50:53.650277 trex-analytic-1.0.4/trexanalytics/controllers/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-11 01:45:04.000000 trex-analytic-1.0.4/trexanalytics/controllers/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:50:53.654753 trex-analytic-1.0.4/trexanalytics/controllers/bigquery/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-18 05:12:38.000000 trex-analytic-1.0.4/trexanalytics/controllers/bigquery/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    14411 2023-03-07 02:42:00.000000 trex-analytic-1.0.4/trexanalytics/controllers/bigquery/customer_query_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2540 2023-03-07 04:22:38.000000 trex-analytic-1.0.4/trexanalytics/controllers/bigquery/query_base_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     5383 2021-07-01 02:13:45.000000 trex-analytic-1.0.4/trexanalytics/controllers/bigquery/redemption_query_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     5566 2021-07-01 02:13:41.000000 trex-analytic-1.0.4/trexanalytics/controllers/bigquery/rewarding_query_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    14535 2021-08-30 06:35:04.000000 trex-analytic-1.0.4/trexanalytics/controllers/bigquery/transaction_query_routes.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:50:53.661188 trex-analytic-1.0.4/trexanalytics/controllers/importdata/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-12 02:42:37.000000 trex-analytic-1.0.4/trexanalytics/controllers/importdata/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    19860 2022-09-29 03:34:40.000000 trex-analytic-1.0.4/trexanalytics/controllers/importdata/import_customer_data_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    14401 2024-04-29 06:56:55.000000 trex-analytic-1.0.4/trexanalytics/controllers/importdata/import_data_base_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     6406 2024-05-06 09:50:11.000000 trex-analytic-1.0.4/trexanalytics/controllers/importdata/import_merchant_data_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     8306 2021-08-20 10:27:16.000000 trex-analytic-1.0.4/trexanalytics/controllers/importdata/import_transaction_data_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    18271 2024-05-03 02:23:35.000000 trex-analytic-1.0.4/trexanalytics/controllers/importdata/import_upstream_data_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)       49 2021-01-21 07:31:55.000000 trex-analytic-1.0.4/trexanalytics/controllers/importdata/import_user_data_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2473 2022-09-23 07:30:35.000000 trex-analytic-1.0.4/trexanalytics/controllers/main_routes.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:50:53.662309 trex-analytic-1.0.4/trexanalytics/controllers/template/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-11 06:02:49.000000 trex-analytic-1.0.4/trexanalytics/controllers/template/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      907 2021-01-20 09:34:38.000000 trex-analytic-1.0.4/trexanalytics/controllers/template/table_template_routes.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:50:53.664604 trex-analytic-1.0.4/trexanalytics/controllers/upstreamdata/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-26 10:02:40.000000 trex-analytic-1.0.4/trexanalytics/controllers/upstreamdata/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:50:53.665740 trex-analytic-1.0.4/trexanalytics/helper/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2023-03-27 04:02:29.000000 trex-analytic-1.0.4/trexanalytics/helper/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     3549 2023-03-27 10:56:12.000000 trex-analytic-1.0.4/trexanalytics/helper/bigquery_upstream_helpers.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:50:53.667243 trex-analytic-1.0.4/trexanalytics/util/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-11 06:16:58.000000 trex-analytic-1.0.4/trexanalytics/util/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      537 2021-01-18 02:07:17.000000 trex-analytic-1.0.4/trexanalytics/util/chart_util.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `trex-analytic-1.0.3/README.md` & `trex-analytic-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `trex-analytic-1.0.3/setup.py` & `trex-analytic-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 from pip._vendor.pkg_resources import require
 
 setuptools.setup(
      name='trex-analytic',  
-     version='1.0.3',
+     version='1.0.4',
      author="Jack Lok",
      author_email="sglok77@gmail.com",
      description="TRex analytics package",
      packages=setuptools.find_packages(),
      classifiers=[
          "Programming Language :: Python :: 3",
          "License :: OSI Approved :: MIT License",
```

### Comparing `trex-analytic-1.0.3/tests/test_chart_util.py` & `trex-analytic-1.0.4/tests/test_chart_util.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-1.0.3/tests/test_cloud_tasks_util.py` & `trex-analytic-1.0.4/tests/test_cloud_tasks_util.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-1.0.3/tests/test_create_bigquery_table.py` & `trex-analytic-1.0.4/tests/test_create_bigquery_table.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-1.0.3/tests/test_delete_bigquery_dataset.py` & `trex-analytic-1.0.4/tests/test_delete_bigquery_dataset.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-1.0.3/tests/test_import_customer_data.py` & `trex-analytic-1.0.4/tests/test_import_customer_data.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-1.0.3/tests/test_import_merchant_customer_data.py` & `trex-analytic-1.0.4/tests/test_import_merchant_customer_data.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-1.0.3/tests/test_import_merchant_data.py` & `trex-analytic-1.0.4/tests/test_import_merchant_data.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-1.0.3/tests/test_list_table_from_dataset.py` & `trex-analytic-1.0.4/tests/test_list_table_from_dataset.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-1.0.3/tests/test_query_customer.py` & `trex-analytic-1.0.4/tests/test_query_customer.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-1.0.3/trex_analytic.egg-info/SOURCES.txt` & `trex-analytic-1.0.4/trex_analytic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trex-analytic-1.0.3/trexanalytics/bigquery_table_template_config.py` & `trex-analytic-1.0.4/trexanalytics/bigquery_table_template_config.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-1.0.3/trexanalytics/bigquery_upstream_data_config.py` & `trex-analytic-1.0.4/trexanalytics/bigquery_upstream_data_config.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-1.0.3/trexanalytics/conf.py` & `trex-analytic-1.0.4/trexanalytics/conf.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-1.0.3/trexanalytics/controllers/bigquery/customer_query_routes.py` & `trex-analytic-1.0.4/trexanalytics/controllers/bigquery/customer_query_routes.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-1.0.3/trexanalytics/controllers/bigquery/query_base_routes.py` & `trex-analytic-1.0.4/trexanalytics/controllers/bigquery/query_base_routes.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-1.0.3/trexanalytics/controllers/bigquery/redemption_query_routes.py` & `trex-analytic-1.0.4/trexanalytics/controllers/bigquery/redemption_query_routes.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-1.0.3/trexanalytics/controllers/bigquery/rewarding_query_routes.py` & `trex-analytic-1.0.4/trexanalytics/controllers/bigquery/rewarding_query_routes.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-1.0.3/trexanalytics/controllers/bigquery/transaction_query_routes.py` & `trex-analytic-1.0.4/trexanalytics/controllers/bigquery/transaction_query_routes.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-1.0.3/trexanalytics/controllers/importdata/import_customer_data_routes.py` & `trex-analytic-1.0.4/trexanalytics/controllers/importdata/import_customer_data_routes.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-1.0.3/trexanalytics/controllers/importdata/import_data_base_routes.py` & `trex-analytic-1.0.4/trexanalytics/controllers/importdata/import_data_base_routes.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         logger.info('%s: data_payload=%s', self.__class__.__name__, data_payload)
         
         try:
             
             total_count     = self.get_import_data_count(**data_payload) or 0
             
             
-            logger.debug('%s: total_count=%s', self.__class__.__name__,total_count)
+            logger.debug('InitImportDataBaseResource: total_count=%s',total_count)
             
             if total_count>0:
                 try:
                     page_size   = self.get_import_data_page_size()
                     task_count  = int(total_count/page_size)
                     remaining   = total_count % page_size
                     
@@ -112,16 +112,16 @@
                     
                     
                     task_url    = self.get_task_url()
                     if task_url:
                         task_url    = analytics_conf.UPSTREAM_BASE_URL + task_url
                         queue_name  = self.get_task_queue()
                         
-                        logger.info('%s: task_url=%s', self.__class__.__name__, task_url)
-                        logger.info('%s: queue_name=%s', self.__class__.__name__, queue_name)
+                        logger.info('InitImportDataBaseResource: task_url=%s', task_url)
+                        logger.info('InitImportDataBaseResource: queue_name=%s', queue_name)
                         
                         create_task(task_url, queue_name, 
                                     in_seconds      = self.get_task_delay_in_seconds(),
                                     http_method     = self.get_task_http_method(), 
                                     payload         = payload,
                                     credential_path = lib_conf.SYSTEM_TASK_SERVICE_CREDENTIAL_PATH, 
                                     project_id      = lib_conf.SYSTEM_TASK_GCLOUD_PROJECT_ID,
```

### Comparing `trex-analytic-1.0.3/trexanalytics/controllers/importdata/import_merchant_data_routes.py` & `trex-analytic-1.0.4/trexanalytics/controllers/importdata/import_merchant_data_routes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 '''
 Created on 12 Jan 2021
 
 @author: jacklok
 '''
 
-from flask import Blueprint, render_template, session, abort, redirect, url_for, current_app
-import logging, json, uuid
-from flask.globals import current_app
-from trexlib.utils.google.bigquery_util import create_table_from_template, create_bigquery_client, stream_data_by_datetime_partition
+from flask import Blueprint
+import logging, uuid
+from trexlib.utils.google.bigquery_util import create_bigquery_client, stream_data_by_datetime_partition
 from trexanalytics import conf as analytics_conf
 from trexanalytics.bigquery_table_template_config import REGISTERED_MERCHANT_TEMPLATE
 from trexmodel.models.datastore.merchant_models import MerchantAcct
 
 from trexmodel.utils.model.model_util import create_db_client 
-from trexmodel.conf import MAX_FETCH_RECORD
+from trexconf.conf import MAX_FETCH_RECORD
 from datetime import datetime
 from trexlib.utils.log_util import get_tracelog
 from trexanalytics.controllers.importdata.import_data_base_routes import TriggerImportDataBaseResource, InitImportDataBaseResource, ImportDataBaseResource
 from flask_restful import Api
 from trexanalytics.bigquery_table_template_config import TABLE_SCHEME_TEMPLATE
```

### Comparing `trex-analytic-1.0.3/trexanalytics/controllers/importdata/import_transaction_data_routes.py` & `trex-analytic-1.0.4/trexanalytics/controllers/importdata/import_transaction_data_routes.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-1.0.3/trexanalytics/controllers/importdata/import_upstream_data_routes.py` & `trex-analytic-1.0.4/trexanalytics/controllers/importdata/import_upstream_data_routes.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,19 +38,23 @@
         return resp
     
     def post(self):
         return self.get()
     
     def get(self):
         try:
-            count = count_all_unsend_upstream_data()
+            result = list_all_unsend_upstream_data()
         except:
             logger.debug(get_tracelog())
         
-        return self.output_html("count=%d"% (count))
+        #return self.output_html("count=%d, <br>%s"% (len(result), result))
+        return jsonify({
+                'count': len(result),
+                'result':result,
+                })
     
 class ImportUpstreamDataResource(Resource):
     
     def output_html(self, content, code=200, headers=None):
         resp = Response(content, mimetype='text/html', headers=headers)
         resp.status_code = code
         return resp
@@ -97,14 +101,23 @@
 
 def count_all_unsend_upstream_data():
     db_client = create_db_client(caller_info="count_all_unsend_upstream_data")
     with db_client.context():
         count       = UpstreamData.count_not_sent()
     return count
 
+def list_all_unsend_upstream_data():
+    db_client = create_db_client(caller_info="list_all_unsend_upstream_data")
+    final_result = []
+    with db_client.context():
+        result       = UpstreamData.list_not_send()
+        for r in result:
+            final_result.append(r.to_dict())
+    return final_result
+
 def count_upstream_data_by_date_range(date_start, date_end):
     db_client = create_db_client(caller_info="count_upstream_data_by_date_range")
     with db_client.context():
         count       = UpstreamData.count_by_date_range(date_start, date_end)
     return count
 
 
@@ -114,20 +127,20 @@
         logger.debug('offset=%d limit=%d', offset, limit)
         
         
         try:
             start_cursor    = kwargs.get('start_cursor')
             batch_id        = kwargs.get('batch_id')
             
-            logger.debug('ImportAllUpstreamData: start_cursor=%s', start_cursor)
-            logger.debug('ImportAllUpstreamData: batch_id=%s', batch_id)
+            logger.info('ImportAllUpstreamData: start_cursor=%s', start_cursor)
+            logger.info('ImportAllUpstreamData: batch_id=%s', batch_id)
             
             next_cursor     = import_all_unsend_upstream_data_function(dataset_name='system', limit=limit, start_cursor=start_cursor, batch_id=batch_id)
             
-            logger.debug('ImportAllUpstreamData: next_cursor=%s', next_cursor)
+            logger.info('ImportAllUpstreamData: next_cursor=%s', next_cursor)
             
             return next_cursor
         except:
             logger.debug('Failed due to %s', get_tracelog())
         
     
     def get_task_url(self):
@@ -221,15 +234,15 @@
         stream_content      = u.stream_content
         
         import_upstream_dict = {'': stream_content}
 
 
     
         logger.debug('################################ batch_id= %s ############################################', batch_id)
-        logger.debug(import_upstream_dict)
+        logger.info(import_upstream_dict)
         logger.debug('#####################################################################################################')
         
         __errors = stream_data(bg_client, dataset_name, table_template_name, 
                                                    TABLE_SCHEME_TEMPLATE.get(table_template_name), table_name, stream_content
                                                    )
         
         if len(__errors)>0:
```

### Comparing `trex-analytic-1.0.3/trexanalytics/controllers/main_routes.py` & `trex-analytic-1.0.4/trexanalytics/controllers/main_routes.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-1.0.3/trexanalytics/controllers/template/table_template_routes.py` & `trex-analytic-1.0.4/trexanalytics/controllers/template/table_template_routes.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-1.0.3/trexanalytics/helper/bigquery_upstream_helpers.py` & `trex-analytic-1.0.4/trexanalytics/helper/bigquery_upstream_helpers.py`

 * *Files identical despite different names*

### Comparing `trex-analytic-1.0.3/trexanalytics/util/chart_util.py` & `trex-analytic-1.0.4/trexanalytics/util/chart_util.py`

 * *Files identical despite different names*

