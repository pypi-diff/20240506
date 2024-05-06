# Comparing `tmp/trex-model-1.3.9.tar.gz` & `tmp/trex-model-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/trex-model-1.3.9.tar", last modified: Fri Apr 19 01:40:19 2024, max compression
+gzip compressed data, was "trex-model-1.4.0.tar", last modified: Mon May  6 08:02:52 2024, max compression
```

## Comparing `trex-model-1.3.9.tar` & `trex-model-1.4.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-19 01:40:19.000000 trex-model-1.3.9/
--rw-r--r--   0 jacklok    (501) staff       (20)      492 2024-04-19 01:40:19.000000 trex-model-1.3.9/PKG-INFO
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-19 01:40:18.000000 trex-model-1.3.9/trexmodel/
--rw-r--r--   0 jacklok    (501) staff       (20)    32565 2024-04-17 15:19:03.000000 trex-model-1.3.9/trexmodel/program_conf.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2287 2024-01-25 03:42:44.000000 trex-model-1.3.9/trexmodel/conf.py
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-06 08:58:46.000000 trex-model-1.3.9/trexmodel/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-19 01:40:19.000000 trex-model-1.3.9/trexmodel/utils/
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-19 01:40:19.000000 trex-model-1.3.9/trexmodel/utils/gcloud/
--rw-r--r--   0 jacklok    (501) staff       (20)      291 2020-08-31 07:47:30.000000 trex-model-1.3.9/trexmodel/utils/gcloud/datastore_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.3.9/trexmodel/utils/gcloud/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.3.9/trexmodel/utils/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-19 01:40:19.000000 trex-model-1.3.9/trexmodel/utils/model/
--rw-r--r--   0 jacklok    (501) staff       (20)     2453 2022-09-09 14:29:07.000000 trex-model-1.3.9/trexmodel/utils/model/model_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.3.9/trexmodel/utils/model/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-19 01:40:18.000000 trex-model-1.3.9/trexmodel/models/
--rw-r--r--   0 jacklok    (501) staff       (20)     9261 2023-08-24 06:48:34.000000 trex-model-1.3.9/trexmodel/models/merchant_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-03 01:59:33.000000 trex-model-1.3.9/trexmodel/models/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      331 2021-09-02 08:53:31.000000 trex-model-1.3.9/trexmodel/models/prepaid_helpers.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-19 01:40:19.000000 trex-model-1.3.9/trexmodel/models/datastore/
--rw-r--r--   0 jacklok    (501) staff       (20)     8552 2024-03-01 08:11:33.000000 trex-model-1.3.9/trexmodel/models/datastore/loyalty_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     8329 2023-12-27 03:18:38.000000 trex-model-1.3.9/trexmodel/models/datastore/import_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    14671 2024-02-07 03:32:09.000000 trex-model-1.3.9/trexmodel/models/datastore/membership_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4099 2024-01-25 06:53:38.000000 trex-model-1.3.9/trexmodel/models/datastore/message_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1348 2020-09-09 01:17:56.000000 trex-model-1.3.9/trexmodel/models/datastore/task_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    34842 2023-11-07 09:43:31.000000 trex-model-1.3.9/trexmodel/models/datastore/reward_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)      602 2021-02-19 08:54:31.000000 trex-model-1.3.9/trexmodel/models/datastore/spending_base_program_model.py
--rw-r--r--   0 jacklok    (501) staff       (20)    55190 2024-04-17 09:40:14.000000 trex-model-1.3.9/trexmodel/models/datastore/customer_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    22092 2024-01-30 05:47:01.000000 trex-model-1.3.9/trexmodel/models/datastore/message_model_helper.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2155 2021-02-19 08:24:29.000000 trex-model-1.3.9/trexmodel/models/datastore/coporate_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-01 04:46:11.000000 trex-model-1.3.9/trexmodel/models/datastore/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7135 2023-09-21 07:48:57.000000 trex-model-1.3.9/trexmodel/models/datastore/reward_model_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)    32185 2023-12-22 02:46:56.000000 trex-model-1.3.9/trexmodel/models/datastore/pos_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2076 2024-03-28 07:14:43.000000 trex-model-1.3.9/trexmodel/models/datastore/recruit_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    22417 2024-01-19 04:31:41.000000 trex-model-1.3.9/trexmodel/models/datastore/user_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    39078 2023-12-14 09:37:29.000000 trex-model-1.3.9/trexmodel/models/datastore/product_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    17001 2024-04-13 08:31:55.000000 trex-model-1.3.9/trexmodel/models/datastore/redemption_catalogue_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1662 2023-08-16 15:50:05.000000 trex-model-1.3.9/trexmodel/models/datastore/fb_subsriber_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    39811 2024-01-30 09:18:08.000000 trex-model-1.3.9/trexmodel/models/datastore/redeem_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    16394 2024-04-18 02:51:01.000000 trex-model-1.3.9/trexmodel/models/datastore/referral_program_model.py
--rw-r--r--   0 jacklok    (501) staff       (20)     8555 2024-02-15 08:43:33.000000 trex-model-1.3.9/trexmodel/models/datastore/system_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    19218 2024-01-01 16:01:07.000000 trex-model-1.3.9/trexmodel/models/datastore/voucher_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    20632 2023-12-01 03:25:17.000000 trex-model-1.3.9/trexmodel/models/datastore/rating_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1319 2022-09-09 14:28:48.000000 trex-model-1.3.9/trexmodel/models/datastore/test_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    49184 2024-04-17 11:58:10.000000 trex-model-1.3.9/trexmodel/models/datastore/program_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1785 2021-05-17 10:44:34.000000 trex-model-1.3.9/trexmodel/models/datastore/model_decorators.py
--rw-r--r--   0 jacklok    (501) staff       (20)    19899 2024-01-18 06:33:46.000000 trex-model-1.3.9/trexmodel/models/datastore/ndb_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     3223 2023-04-11 07:48:46.000000 trex-model-1.3.9/trexmodel/models/datastore/analytic_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    41297 2023-12-17 08:11:57.000000 trex-model-1.3.9/trexmodel/models/datastore/transaction_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    12170 2024-03-06 03:28:38.000000 trex-model-1.3.9/trexmodel/models/datastore/marketing_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2397 2023-05-24 02:56:50.000000 trex-model-1.3.9/trexmodel/models/datastore/app_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    15032 2024-03-14 09:02:34.000000 trex-model-1.3.9/trexmodel/models/datastore/customer_model_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)    83773 2024-04-18 09:25:49.000000 trex-model-1.3.9/trexmodel/models/datastore/merchant_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    28234 2024-01-30 09:33:33.000000 trex-model-1.3.9/trexmodel/models/datastore/prepaid_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    41800 2024-04-17 14:45:19.000000 trex-model-1.3.9/trexmodel/models/datastore/lucky_draw_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1351 2021-08-19 08:33:56.000000 trex-model-1.3.9/trexmodel/models/datastore/inventory_model.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4892 2022-11-14 06:42:31.000000 trex-model-1.3.9/trexmodel/models/datastore/admin_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-05-16 04:55:29.000000 trex-model-1.3.9/trexmodel/models/model_decorator.py
--rw-r--r--   0 jacklok    (501) staff       (20)      172 2022-03-04 03:54:52.000000 trex-model-1.3.9/trexmodel/pos_conf.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1074 2020-09-06 08:34:15.000000 trex-model-1.3.9/LICENSE
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-19 01:40:18.000000 trex-model-1.3.9/trex_model.egg-info/
--rw-r--r--   0 jacklok    (501) staff       (20)      492 2024-04-19 01:40:18.000000 trex-model-1.3.9/trex_model.egg-info/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)     2326 2024-04-19 01:40:18.000000 trex-model-1.3.9/trex_model.egg-info/SOURCES.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       95 2024-04-19 01:40:18.000000 trex-model-1.3.9/trex_model.egg-info/requires.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       16 2024-04-19 01:40:18.000000 trex-model-1.3.9/trex_model.egg-info/top_level.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        1 2024-04-19 01:40:18.000000 trex-model-1.3.9/trex_model.egg-info/dependency_links.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       60 2020-09-10 05:51:48.000000 trex-model-1.3.9/MANIFEST.in
--rw-r--r--   0 jacklok    (501) staff       (20)       57 2020-09-06 08:43:45.000000 trex-model-1.3.9/README.md
--rw-r--r--   0 jacklok    (501) staff       (20)      922 2024-04-19 01:39:39.000000 trex-model-1.3.9/setup.py
--rw-r--r--   0 jacklok    (501) staff       (20)       75 2024-04-19 01:40:19.000000 trex-model-1.3.9/setup.cfg
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 08:02:52.397532 trex-model-1.4.0/
+-rw-r--r--   0 jacklok    (501) staff       (20)     1074 2020-09-06 08:34:15.000000 trex-model-1.4.0/LICENSE
+-rw-r--r--   0 jacklok    (501) staff       (20)       60 2020-09-10 05:51:48.000000 trex-model-1.4.0/MANIFEST.in
+-rw-r--r--   0 jacklok    (501) staff       (20)      643 2024-05-06 08:02:52.396187 trex-model-1.4.0/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)       57 2020-09-06 08:43:45.000000 trex-model-1.4.0/README.md
+-rw-r--r--   0 jacklok    (501) staff       (20)       75 2024-05-06 08:02:52.398800 trex-model-1.4.0/setup.cfg
+-rw-r--r--   0 jacklok    (501) staff       (20)      922 2024-05-06 07:40:26.000000 trex-model-1.4.0/setup.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 08:02:52.393637 trex-model-1.4.0/trex_model.egg-info/
+-rw-r--r--   0 jacklok    (501) staff       (20)      643 2024-05-06 08:02:52.000000 trex-model-1.4.0/trex_model.egg-info/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)     2326 2024-05-06 08:02:52.000000 trex-model-1.4.0/trex_model.egg-info/SOURCES.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        1 2024-05-06 08:02:52.000000 trex-model-1.4.0/trex_model.egg-info/dependency_links.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       95 2024-05-06 08:02:52.000000 trex-model-1.4.0/trex_model.egg-info/requires.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       16 2024-05-06 08:02:52.000000 trex-model-1.4.0/trex_model.egg-info/top_level.txt
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 08:02:52.316514 trex-model-1.4.0/trexmodel/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-06 08:58:46.000000 trex-model-1.4.0/trexmodel/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2287 2024-04-22 08:11:53.000000 trex-model-1.4.0/trexmodel/conf.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 08:02:52.320343 trex-model-1.4.0/trexmodel/models/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-03 01:59:33.000000 trex-model-1.4.0/trexmodel/models/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 08:02:52.382896 trex-model-1.4.0/trexmodel/models/datastore/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-01 04:46:11.000000 trex-model-1.4.0/trexmodel/models/datastore/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4893 2024-04-29 06:17:32.000000 trex-model-1.4.0/trexmodel/models/datastore/admin_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     3222 2024-05-02 05:47:34.000000 trex-model-1.4.0/trexmodel/models/datastore/analytic_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2397 2023-05-24 02:56:50.000000 trex-model-1.4.0/trexmodel/models/datastore/app_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1645 2024-05-02 05:47:57.000000 trex-model-1.4.0/trexmodel/models/datastore/coporate_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    15032 2024-04-25 01:46:35.000000 trex-model-1.4.0/trexmodel/models/datastore/customer_model_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    55452 2024-05-02 05:48:07.000000 trex-model-1.4.0/trexmodel/models/datastore/customer_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1453 2024-04-29 06:18:03.000000 trex-model-1.4.0/trexmodel/models/datastore/fb_subsriber_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     8120 2024-05-02 05:34:16.000000 trex-model-1.4.0/trexmodel/models/datastore/import_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      876 2024-05-02 05:48:32.000000 trex-model-1.4.0/trexmodel/models/datastore/inventory_model.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     8532 2024-05-02 05:48:57.000000 trex-model-1.4.0/trexmodel/models/datastore/loyalty_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    41799 2024-05-02 05:34:22.000000 trex-model-1.4.0/trexmodel/models/datastore/lucky_draw_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    12155 2024-05-02 05:34:31.000000 trex-model-1.4.0/trexmodel/models/datastore/marketing_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    14631 2024-05-02 05:34:41.000000 trex-model-1.4.0/trexmodel/models/datastore/membership_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    84856 2024-05-02 05:49:13.000000 trex-model-1.4.0/trexmodel/models/datastore/merchant_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    22091 2024-05-02 05:34:47.000000 trex-model-1.4.0/trexmodel/models/datastore/message_model_helper.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     3892 2024-05-02 05:50:04.000000 trex-model-1.4.0/trexmodel/models/datastore/message_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1785 2021-05-17 10:44:34.000000 trex-model-1.4.0/trexmodel/models/datastore/model_decorators.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    19868 2024-05-02 05:50:11.000000 trex-model-1.4.0/trexmodel/models/datastore/ndb_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    32178 2024-05-02 05:50:22.000000 trex-model-1.4.0/trexmodel/models/datastore/pos_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    29746 2024-05-02 05:50:40.000000 trex-model-1.4.0/trexmodel/models/datastore/prepaid_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    38896 2024-05-02 05:50:57.000000 trex-model-1.4.0/trexmodel/models/datastore/product_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    49100 2024-05-02 05:51:10.000000 trex-model-1.4.0/trexmodel/models/datastore/program_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    20631 2024-05-02 05:51:18.000000 trex-model-1.4.0/trexmodel/models/datastore/rating_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1876 2024-05-02 05:51:30.000000 trex-model-1.4.0/trexmodel/models/datastore/recruit_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    39734 2024-05-02 05:51:40.000000 trex-model-1.4.0/trexmodel/models/datastore/redeem_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    16984 2024-05-02 05:35:09.000000 trex-model-1.4.0/trexmodel/models/datastore/redemption_catalogue_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    16215 2024-05-02 05:51:58.000000 trex-model-1.4.0/trexmodel/models/datastore/referral_program_model.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7134 2024-05-02 05:35:18.000000 trex-model-1.4.0/trexmodel/models/datastore/reward_model_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    34841 2024-05-02 05:52:06.000000 trex-model-1.4.0/trexmodel/models/datastore/reward_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      602 2021-02-19 08:54:31.000000 trex-model-1.4.0/trexmodel/models/datastore/spending_base_program_model.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     8548 2024-05-02 05:52:23.000000 trex-model-1.4.0/trexmodel/models/datastore/system_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1332 2024-05-02 05:53:10.000000 trex-model-1.4.0/trexmodel/models/datastore/task_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      789 2024-05-02 05:52:53.000000 trex-model-1.4.0/trexmodel/models/datastore/test_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    41773 2024-05-02 02:32:39.000000 trex-model-1.4.0/trexmodel/models/datastore/transaction_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    23255 2024-05-02 05:53:27.000000 trex-model-1.4.0/trexmodel/models/datastore/user_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    19217 2024-05-02 05:35:25.000000 trex-model-1.4.0/trexmodel/models/datastore/voucher_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    10559 2024-05-02 05:53:36.000000 trex-model-1.4.0/trexmodel/models/merchant_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-05-16 04:55:29.000000 trex-model-1.4.0/trexmodel/models/model_decorator.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      331 2021-09-02 08:53:31.000000 trex-model-1.4.0/trexmodel/models/prepaid_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      172 2022-03-04 03:54:52.000000 trex-model-1.4.0/trexmodel/pos_conf.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    32618 2024-05-02 02:19:46.000000 trex-model-1.4.0/trexmodel/program_conf.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 08:02:52.387352 trex-model-1.4.0/trexmodel/utils/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.4.0/trexmodel/utils/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 08:02:52.388409 trex-model-1.4.0/trexmodel/utils/gcloud/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.4.0/trexmodel/utils/gcloud/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      291 2020-08-31 07:47:30.000000 trex-model-1.4.0/trexmodel/utils/gcloud/datastore_util.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 08:02:52.392132 trex-model-1.4.0/trexmodel/utils/model/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.4.0/trexmodel/utils/model/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2452 2024-05-02 05:53:44.000000 trex-model-1.4.0/trexmodel/utils/model/model_util.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `trex-model-1.3.9/trexmodel/program_conf.py` & `trex-model-1.4.0/trexmodel/program_conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,14 +215,15 @@
 
 
 PROGRAM_REWARD_GIVEAWAY_METHOD_AUTO     = 'auto'
 PROGRAM_REWARD_GIVEAWAY_METHOD_MANUAL   = 'manual'
 PROGRAM_REWARD_GIVEAWAY_METHOD_SYSTEM   = 'system'
 PROGRAM_REWARD_GIVEAWAY_METHOD_TIER     = 'tier'
 PROGRAM_REWARD_GIVEAWAY_METHOD_REDEEM   = 'redeem'
+PROGRAM_REWARD_GIVEAWAY_METHOD_REFERRAL = 'referral'
 
 GIVEAWAY_SYSTEM_CONDITION_NEW_MEMBERSHIP        = 'new_membership'
 GIVEAWAY_SYSTEM_CONDITION_RENEW_MEMBERSHIP      = 'renew_membership'
 GIVEAWAY_SYSTEM_CONDITION_MEMBERSHIP_YEAR       = 'membership_year'
 GIVEAWAY_SYSTEM_CONDITION_DATA_IMPORT           = 'data_import'
 
 GIVEAWAY_SYSTEM_CONDITION_FOR_MEMBERSHIP        = (GIVEAWAY_SYSTEM_CONDITION_NEW_MEMBERSHIP, GIVEAWAY_SYSTEM_CONDITION_RENEW_MEMBERSHIP)
```

### Comparing `trex-model-1.3.9/trexmodel/conf.py` & `trex-model-1.4.0/trexmodel/conf.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.9/trexmodel/utils/model/model_util.py` & `trex-model-1.4.0/trexmodel/utils/model/model_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 @author: jacklok
 '''
 from google.cloud import ndb
 from google.oauth2 import service_account
 from google.auth import crypt
 import io, json, logging
-from trexmodel import conf as model_conf
+from trexconf import conf as model_conf
 import six
 from datetime import datetime
 from trexlib.utils.string_util import random_number
 
 logger = logging.getLogger('model')
 
 def create_db_client(info=None, credential_filepath=None, namespace=None, caller_info=None):
```

### Comparing `trex-model-1.3.9/trexmodel/models/merchant_helpers.py` & `trex-model-1.4.0/trexmodel/models/merchant_helpers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from trexmodel.models.datastore.pos_models import InvoiceNoGeneration,\
     RoundingSetup, DinningOption, PosPaymentMethod
 from trexmodel.models.datastore.merchant_models import ReceiptSetup, Outlet,\
     BannerFile
+from trexlib.utils.string_util import is_not_empty
 
 def construct_merchant_acct_info(merchant_acct):
     account_settings        = {
                                 'account_code'  : merchant_acct.account_code,
                                 'currency'      : merchant_acct.currency_code,
                                 'locale'        : merchant_acct.locale,    
                                 }
@@ -27,27 +28,43 @@
     
     if invoice_no_generation:
         account_settings['invoice_settings']    = {
                                                      'invoice_no_generators'    : invoice_no_generation.generators_list,
                                                                      
                                                     }
     
+    referral_program_settings = merchant_acct.program_settings.get('referral_program', {})
+    
     info =  {
                 'key'                               : merchant_acct.key_in_str,
                 'company_name'                      : merchant_acct.company_name,
                 'brand_name'                        : merchant_acct.brand_name,
                 'website'                           : merchant_acct.website,
                 'account_id'                        : merchant_acct.key_in_str,
                 'api_key'                           : merchant_acct.api_key,
                 'logo_image_url'                    : merchant_acct.logo_public_url,
                 'image_default_base_url'            : merchant_acct.image_default_base_url,
                 'account_settings'                  : account_settings,
                 'outlets'                           : outlet_json_list,
                 'banners'                           : banner_listing,
+                
                 } 
+    if is_not_empty(referral_program_settings):
+        
+        info['referral_program_settings'] = {
+                                                'program_count'             : merchant_acct.effective_referral_program_count,
+                                                'referrer_promote_title'    : referral_program_settings.get('referrer_promote_title'),
+                                                'referrer_promote_desc'     : referral_program_settings.get('referrer_promote_desc'),
+                                                'referrer_promote_image'    : referral_program_settings.get('referrer_promote_image'),
+                                                'referee_promote_title'     : referral_program_settings.get('referee_promote_title'),
+                                                'referee_promote_desc'      : referral_program_settings.get('referee_promote_desc'),
+                                                'referee_promote_image'     : referral_program_settings.get('referee_promote_image'),
+                                                
+                                            }
+    
     return info
 
 def construct_outlet_info(outlet):
     geo_location = None
     if outlet.geo_location:
         geo_location = '%s,%s' % (outlet.geo_location.latitude, outlet.geo_location.longitude)
     return {
```

### Comparing `trex-model-1.3.9/trexmodel/models/datastore/loyalty_models.py` & `trex-model-1.4.0/trexmodel/models/datastore/loyalty_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 @author: jacklok
 '''
 
 from google.cloud import ndb
 from trexmodel.models.datastore.ndb_models import BaseNModel, DictModel
 from trexmodel.models.datastore.merchant_models import Outlet
 from trexlib.utils.string_util import random_number
-import logging, json
-from trexmodel import conf, program_conf
+import logging
+from trexconf import conf
 from datetime import datetime
-from google.api_core.operations_v1.operations_client_config import config
+#from google.api_core.operations_v1.operations_client_config import config
 
 logger = logging.getLogger('debug')
 
 
 class LoyaltyDeviceSetting(BaseNModel,DictModel):
     '''
     merchant_acct as ancestor
```

### Comparing `trex-model-1.3.9/trexmodel/models/datastore/import_models.py` & `trex-model-1.4.0/trexmodel/models/datastore/import_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 '''
 Created on 26 Sep 2023
 
 @author: jacklok
 '''
 
 from google.cloud import ndb
-from trexmodel.models.datastore.user_models import UserMin
-from trexlib.utils.security_util import generate_user_id, hash_password
 from trexmodel.models.datastore.ndb_models import BaseNModel, DictModel
 from trexlib.utils.string_util import random_string
-from trexlib.utils.common.common_util import logger
-from trexlib import conf
 from trexmodel.models.datastore.merchant_models import MerchantAcct
 import logging
 import csv, io
 
-from trexmodel import program_conf
+from trexconf import program_conf
 
 logger = logging.getLogger('model')
 
 class ImportCustomerFile(BaseNModel, DictModel):
     merchant_acct               = ndb.KeyProperty(name="merchant_acct", kind=MerchantAcct)
     file_public_url             = ndb.StringProperty(required=True)
     file_storage_filename       = ndb.StringProperty(required=True)
```

### Comparing `trex-model-1.3.9/trexmodel/models/datastore/membership_models.py` & `trex-model-1.4.0/trexmodel/models/datastore/membership_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,21 +5,20 @@
 '''
 
 from google.cloud import ndb
 from trexmodel.models.datastore.ndb_models import BaseNModel, DictModel
 import trexmodel.conf as model_conf
 from trexlib.utils.string_util import is_not_empty, random_string
 from trexmodel.models.datastore.merchant_models import MerchantAcct, \
-    MerchantUser, Outlet
+    MerchantUser
 import logging
 from dateutil.relativedelta import relativedelta
-from datetime import timedelta
 
 from datetime import datetime
-from trexmodel import program_conf
+from trexconf import program_conf
 
 logger = logging.getLogger('model')
 
 class MembershipBase(BaseNModel, DictModel):
     '''
     Merchant Acct as ancestor
```

### Comparing `trex-model-1.3.9/trexmodel/models/datastore/message_models.py` & `trex-model-1.4.0/trexmodel/models/datastore/message_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,21 +3,17 @@
 
 @author: jacklok
 '''
 
 from google.cloud import ndb
 from trexmodel.models.datastore.ndb_models import BaseNModel, DictModel
 from trexmodel.models.datastore.user_models import User
-import trexmodel.conf as model_conf
+from datetime import datetime
 import logging
-from datetime import datetime, timedelta
-from trexlib.utils.common.date_util import parse_datetime
 from trexmodel import conf
-from google.auth._default import default
-from trexmodel.models.datastore.system_models import Tagging
 from trexmodel.conf import MESSAGE_STATUS_SET, MESSAGE_STATUS_NEW, MESSAGE_CATEGORY_SYSTEM,\
     MESSAGE_STATUS_READ, MESSAGE_CATEGORIES, MESSAGE_CATEGORY_ANNOUNCEMENT
 from trexmodel.models.datastore.transaction_models import CustomerTransaction
 
 
 logger = logging.getLogger('model')
```

### Comparing `trex-model-1.3.9/trexmodel/models/datastore/task_models.py` & `trex-model-1.4.0/trexmodel/models/datastore/task_models.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 '''
 Created on 13 Apr 2020
 
 @author: jacklok
 '''
 from google.cloud import ndb
-import logging
-from trexmodel import conf as model_conf
+from trexconf import conf as model_conf
 from trexmodel.models.datastore.ndb_models import BaseNModel
 
  
 class Todo(BaseNModel):
     
     name                    = ndb.StringProperty(required=True)
     desc                    = ndb.TextProperty(required=False, indexed=False)
```

### Comparing `trex-model-1.3.9/trexmodel/models/datastore/reward_models.py` & `trex-model-1.4.0/trexmodel/models/datastore/reward_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from trexmodel.models.datastore.user_models import User
 from trexmodel.models.datastore.merchant_models import MerchantAcct, Outlet, MerchantUser
 from trexmodel.models.datastore.program_models import MerchantProgram,\
     MerchantTierRewardProgram
 from trexmodel.models.datastore.voucher_models import MerchantVoucher
 from trexlib.utils.string_util import is_empty, is_not_empty
 import logging
-from trexmodel import conf, program_conf
+from trexconf import conf, program_conf
 from trexlib.utils.string_util import random_string
 from datetime import datetime, timedelta
 from trexmodel.utils.model.model_util import generate_transaction_id,\
     string_to_key_property 
 from six import string_types
 from flask_babel import gettext
 from trexmodel.models.datastore.customer_models import Customer
```

### Comparing `trex-model-1.3.9/trexmodel/models/datastore/spending_base_program_model.py` & `trex-model-1.4.0/trexmodel/models/datastore/spending_base_program_model.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.9/trexmodel/models/datastore/customer_models.py` & `trex-model-1.4.0/trexmodel/models/datastore/customer_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from trexmodel.models.datastore.merchant_models import MerchantAcct, Outlet,\
     MerchantUser
 import trexmodel.conf as model_conf
 from trexlib.utils.string_util import is_not_empty, is_empty
 import logging
 from trexlib.utils.common.date_util import convert_date_to_datetime,\
     to_day_of_year
-from trexmodel import conf, program_conf
+from trexconf import conf, program_conf
 from six import string_types
 from datetime import datetime, timedelta
 from trexmodel.models.datastore.membership_models import MerchantTierMembership,\
     MerchantMembership
 from trexmodel.models.datastore.customer_model_helpers import update_customer_entiteld_voucher_summary_after_removed_voucher,\
     update_customer_entiteld_voucher_summary_with_customer_new_voucher
     
@@ -42,14 +42,15 @@
     email                       = ndb.StringProperty(required=False)
     
     birth_date                  = ndb.DateProperty(required=False, indexed=False)
     birth_date_date_str         = ndb.StringProperty(required=False) 
     birth_day_in_year           = ndb.IntegerProperty(required=False)
     gender                      = ndb.StringProperty(required=False)
     reference_code              = ndb.StringProperty(required=True)
+    referral_code               = ndb.StringProperty(required=False)
     
     mobile_app_installed        = ndb.BooleanProperty(required=False, default=False)
     
     tags_list                   = ndb.StringProperty(repeated=True, write_empty_list=True)
     
     memberships_list            = ndb.StringProperty(repeated=True, write_empty_list=True)
     
@@ -64,26 +65,28 @@
     reward_summary                              = ndb.JsonProperty()
     prepaid_summary                             = ndb.JsonProperty()
     entitled_voucher_summary                    = ndb.JsonProperty()
     entitled_birthday_reward_summary            = ndb.JsonProperty()
     entitled_membership_reward_summary          = ndb.JsonProperty()
     entitled_lucky_draw_ticket_summary          = ndb.JsonProperty(required=False)
     
+    referrer_code                               = ndb.StringProperty(required=False)
+    
     kpi_summary                                 = ndb.JsonProperty()
     
     device_details                              = ndb.JsonProperty()
     
     fulltextsearch_field_name           = 'name'
     
     dict_properties     = ['name', 'mobile_phone', 'email', 'gender', 'birth_date', 'reference_code', 'merchant_reference_code',  
                            'tags_list', 'memberships_list', 'registered_merchant_acct', 'entitled_membership_reward_summary',
                            'reward_summary', 'entitled_voucher_summary', 'prepaid_summary', 'kpi_summary', 'entitled_lucky_draw_ticket_summary',
                            'entitled_birthday_reward_summary', 'tier_membership_key',
                            'registered_outlet_key', 'registered_merchant_acct_key', 'registered_datetime', 'modified_datetime',
-                           'registered_user_acct',
+                           'registered_user_acct','referral_code',
                            
                            ]
     
     @property
     def is_any_entitled_voucher_active(self):
         
         today = datetime.utcnow().date()
@@ -263,14 +266,15 @@
         customer_acct.put()    
         
     @staticmethod
     def update_tickets_list_into_lucky_draw_ticket_summary(customer_acct, tickets_list):
         for ticket in tickets_list:
             ticket.patch_prize_image_base_url()
             Customer.update_ticket_into_lucky_draw_ticket_summary(customer_acct, ticket.to_configuration())
+    
     @classmethod
     def get_by_reference_code(cls, reference_code, merchant_acct):
         return cls.query(ndb.AND(cls.reference_code==reference_code, cls.merchant_acct==merchant_acct.create_ndb_key())).get()
     
     @classmethod
     def get_by_merchant_reference_code(cls, merchant_reference_code, merchant_acct):
         return cls.query(ndb.AND(cls.merchant_reference_code==merchant_reference_code, cls.merchant_acct==merchant_acct.create_ndb_key())).get()
@@ -349,14 +353,15 @@
                                #user_acct                = user_acct.create_ndb_key(),  
                                outlet                   = outlet.create_ndb_key(), 
                                name                     = user_acct.name, 
                                email                    = user_acct.email, 
                                mobile_phone             = user_acct.mobile_phone, 
                                gender                   = user_acct.gender, 
                                reference_code           = user_acct.reference_code, 
+                               referral_code            = user_acct.referral_code,
                                birth_date               = user_acct.birth_date, 
                                birth_date_date_str      = user_acct.birth_date_date_str, 
                                birth_day_in_year        = user_acct.birth_day_in_year,
                                merchant_reference_code  = merchant_reference_code,
                                merchant_acct            = merchant_acct.create_ndb_key()
                            )
```

### Comparing `trex-model-1.3.9/trexmodel/models/datastore/message_model_helper.py` & `trex-model-1.4.0/trexmodel/models/datastore/message_model_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 @author: jacklok
 '''
 from trexmodel.program_conf import REWARD_FORMAT_MAP, REWARD_FORMAT_PREPAID
 from trexmodel.models.datastore.message_models import Message
 from trexmodel.conf import MESSAGE_CATEGORY_REWARD, MESSAGE_STATUS_NEW,\
     MESSAGE_CATEGORY_REDEEM
-from trexmodel import program_conf
+from trexconf import program_conf
 from babel.numbers import format_currency
 import logging
 
 
 logger = logging.getLogger('helper')
 
 entitled_reward_message_template = '''{amount} {reward_format}'''
```

### Comparing `trex-model-1.3.9/trexmodel/models/datastore/reward_model_helpers.py` & `trex-model-1.4.0/trexmodel/models/datastore/reward_model_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 '''
 from datetime import datetime
 
 from dateutil.relativedelta import relativedelta
 from trexlib.utils.string_util import is_not_empty
 
 import logging
-from trexmodel import program_conf
+from trexconf import program_conf
 from trexmodel.models.datastore.reward_models import CustomerEntitledVoucher
 from trexmodel.models.datastore.voucher_models import MerchantVoucher
 
 
 logger = logging.getLogger('debug')
 
 def is_customer_entitled_voucher_within_limit(customer, merchant_voucher, redeem_count):
```

### Comparing `trex-model-1.3.9/trexmodel/models/datastore/pos_models.py` & `trex-model-1.4.0/trexmodel/models/datastore/pos_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 from google.cloud import ndb
 from trexmodel.models.datastore.ndb_models import BaseNModel, DictModel
 from trexmodel.models.datastore.merchant_models import Outlet
 from trexlib.utils.string_util import random_number, is_not_empty
-import logging, json
-from trexmodel import conf
+import logging
+from trexconf import conf
 from datetime import datetime
 from trexmodel.models.datastore.product_models import ProductCatalogue
 from trexmodel.models.datastore.model_decorators import model_transactional
 from google.api_core.operations_v1.operations_client_config import config
 
 logger = logging.getLogger('debug')
```

### Comparing `trex-model-1.3.9/trexmodel/models/datastore/recruit_models.py` & `trex-model-1.4.0/trexmodel/models/datastore/recruit_models.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,18 +2,14 @@
 Created on 27 Mar 2024
 
 @author: jacklok
 '''
 
 from trexmodel.models.datastore.ndb_models import BaseNModel, DictModel
 from google.cloud import ndb
-from trexmodel.models.datastore.merchant_models import MerchantAcct, Outlet
-from trexmodel.models.datastore.user_models import User
-from trexmodel import conf
-from datetime import datetime, timedelta
 import logging
 from builtins import staticmethod
 
 logger = logging.getLogger('model')
 
 class RecruitBase(BaseNModel, DictModel):
     name                        = ndb.StringProperty(required=True)
```

### Comparing `trex-model-1.3.9/trexmodel/models/datastore/user_models.py` & `trex-model-1.4.0/trexmodel/models/datastore/user_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 '''
 Created on 10 Apr 2020
 
 @author: jacklok
 '''
 from google.cloud import ndb
 from trexmodel.models.datastore.ndb_models import BaseNModel, DictModel
-from trexlib.utils.string_util import random_number, is_not_empty, random_string,\
+from trexlib.utils.string_util import random_number, random_string,\
     is_empty
 from flask_login import UserMixin
 import logging  
 from trexlib.utils.security_util import generate_user_id, hash_password
 
-from trexlib import conf as lib_conf
-from trexmodel import conf as model_conf, conf
-import json
-from json import JSONEncoder
+from trexconf import conf as lib_conf
+from trexconf import conf as model_conf, conf
 from trexlib.utils.common.date_util import to_day_of_year
 from datetime import datetime, timedelta
-from flask_babel import gettext
 from trexmodel.conf import USER_STATUS_ANONYMOUS, ACCOUNT_LOCKED_IN_MINUTES
 
 logger = logging.getLogger("model")
 
 class UserMin(BaseNModel, DictModel, UserMixin):
     
     #system internal usage
@@ -123,14 +120,15 @@
 
 
 class UserBase(UserMin):
     #---------------------------------------------------------------------------
     # User System Generated fields
     #---------------------------------------------------------------------------
     reference_code              = ndb.StringProperty(required=True)
+    referral_code               = ndb.StringProperty(required=True)
     
     #---------------------------------------------------------------------------
     # User Mutual Mandatory fields
     #---------------------------------------------------------------------------
     email                       = ndb.StringProperty(required=False)
     mobile_phone                = ndb.StringProperty(required=False)
     
@@ -198,25 +196,42 @@
     
     @classmethod
     def get_by_email(cls, email):
         return User.query(ndb.AND(User.email==email, User.deleted==False)).get()
     
     @classmethod
     def list_by_email(cls, email):
-        return User.query(ndb.AND(User.email==email)).fetch(limit=conf.MAX_FETCH_RECORD)
-        
+        return cls.query(ndb.AND(User.email==email)).fetch(limit=conf.MAX_FETCH_RECORD)
+    
     @classmethod
     def get_by_mobile_phone(cls, mobile_phone):
         return User.query(ndb.AND(User.mobile_phone==mobile_phone, User.deleted==False)).get()
     
     @classmethod
+    def get_by_referral_code(cls, referral_code):
+        return User.query(ndb.AND(User.referral_code==referral_code)).get()
+    
+    @classmethod
     def get_by_reset_password_token(cls, request_reset_password_token):
         return User.query(ndb.AND(User.request_reset_password_token==request_reset_password_token)).get()
     
     @classmethod
+    def count_all(cls):
+        return cls.count(limit=conf.MAX_FETCH_RECORD)
+    
+    @classmethod
+    def _generate_referral_code(cls):
+        referral_code = random_string(8, is_human_mistake_safe=True)
+        checking_user = cls.get_by_referral_code(referral_code)
+        while checking_user is not None:
+            referral_code = random_string(8, is_human_mistake_safe=True)
+            checking_user = cls.get_by_referral_code(referral_code)
+        return referral_code
+    
+    @classmethod
     def create(cls, name=None, email=None, mobile_phone=None, 
                gender=None, birth_date=None, 
                password=None, is_email_verified=True, 
                is_mobile_phone_verified=False, 
                reference_code=None, status=None
                ):
         
@@ -237,16 +252,17 @@
             mobile_phone = mobile_phone.replace(" ", "")    
         
         created_user = cls(user_id=user_id, name=name, email=email, mobile_phone=mobile_phone, 
                            gender=gender, birth_date=birth_date, birth_date_date_str=birth_date_date_str,  birth_day_in_year=birth_day_in_year,
                            reference_code=reference_code, status=status,
                            )
         
-        hashed_password = hash_password(user_id, password)
-        created_user.password = hashed_password
+        hashed_password             = hash_password(user_id, password)
+        created_user.password       = hashed_password
+        created_user.referral_code  = cls._generate_referral_code()
         
         
         created_user.is_email_verified          = is_email_verified
         created_user.is_mobile_phone_verified   = is_mobile_phone_verified
         
         if is_email_verified==False:
             created_user.email_vc                               = random_number(6)
@@ -262,19 +278,22 @@
     
     @classmethod
     def update(cls, user_acct=None, **kwargs):
         logger.debug('**kwargs=%s', kwargs)
         
         mobile_phone    = kwargs.get('mobile_phone')
         password        = kwargs.get('password')
-        status          = kwargs.get('status')
+        #status          = kwargs.get('status')
         
         if mobile_phone:
             mobile_phone = mobile_phone.replace(" ", "")
         
+        if is_empty(user_acct.referral_code):
+            user_acct.referral_code = cls._generate_referral_code()
+        
         kwargs['mobile_phone'] = mobile_phone
         
         for key, value in kwargs.items():
             setattr(user_acct, key, value)
         
         if password:
             hashed_password = hash_password(user_acct.user_id, password)
```

### Comparing `trex-model-1.3.9/trexmodel/models/datastore/product_models.py` & `trex-model-1.4.0/trexmodel/models/datastore/product_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 '''
 Created on 23 Jul 2021
 
 @author: jacklok
 '''
 from google.cloud import ndb
 from trexmodel.models.datastore.ndb_models import BaseNModel, DictModel, FullTextSearchable
-from trexmodel.models.datastore.user_models import User
 from trexmodel.models.datastore.merchant_models import MerchantAcct, MerchantUser
 from trexlib.utils.string_util import is_empty, is_not_empty
-import logging, json
-from trexmodel import conf, program_conf
+import logging
+from trexconf import conf
 from trexlib.utils.string_util import random_string
-from datetime import datetime, timedelta
-from trexmodel.models.datastore.customer_models import Customer
 import trexmodel.conf as model_conf
 from trexmodel.models.datastore.model_decorators import model_transactional
 from flask_babel import gettext
 
 
 #logger = logging.getLogger('model')
 logger = logging.getLogger('debug')
```

### Comparing `trex-model-1.3.9/trexmodel/models/datastore/redemption_catalogue_models.py` & `trex-model-1.4.0/trexmodel/models/datastore/redemption_catalogue_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 
 @author: jacklok
 '''
 import logging
 from trexmodel.models.datastore.ndb_models import BaseNModel, DictModel
 from google.cloud import ndb
 from datetime import datetime
-import trexmodel.conf as model_conf
-from trexmodel import program_conf
+from trexconf import program_conf, conf as model_conf
 from trexmodel.models.datastore.merchant_models import MerchantUser,\
     MerchantAcct
 from trexlib.utils.string_util import is_not_empty, is_empty
 from trexmodel.models.datastore.model_decorators import model_transactional
 
 logger = logging.getLogger('model')
```

### Comparing `trex-model-1.3.9/trexmodel/models/datastore/redeem_models.py` & `trex-model-1.4.0/trexmodel/models/datastore/redeem_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,20 +6,19 @@
 
 from google.cloud import ndb
 from trexmodel.models.datastore.ndb_models import BaseNModel, DictModel
 from trexmodel.models.datastore.user_models import User
 from trexmodel.models.datastore.merchant_models import MerchantAcct, Outlet, MerchantUser
 from trexlib.utils.string_util import is_empty, is_not_empty
 import logging, json
-from trexmodel import conf, program_conf
+from trexconf import conf, program_conf
 from datetime import datetime, timedelta
 from trexmodel.utils.model.model_util import generate_transaction_id
 from trexmodel.models.datastore.reward_models import CustomerPointReward,\
     CustomerStampReward, CustomerEntitledVoucher
-from trexmodel.models.datastore.model_decorators import model_transactional
 from trexmodel.models.datastore.customer_models import Customer
 from trexmodel.models.datastore.transaction_models import CustomerTransaction
 from trexmodel.models.datastore.prepaid_models import CustomerPrepaidReward
 from trexmodel.models.datastore.redemption_catalogue_models import RedemptionCatalogue
 from trexmodel.models.datastore import user_models
```

### Comparing `trex-model-1.3.9/trexmodel/models/datastore/referral_program_model.py` & `trex-model-1.4.0/trexmodel/models/datastore/referral_program_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,20 @@
 
 @author: jacklok
 '''
 
 from google.cloud import ndb
 from trexmodel.models.datastore.ndb_models import BaseNModel, DictModel
 import trexmodel.conf as model_conf
-from trexlib.utils.string_util import is_not_empty, random_string, is_empty
-from trexmodel.models.datastore.merchant_models import MerchantAcct, Outlet,\
-    MerchantUser
-from trexmodel.models.datastore.coporate_models import CorporateAcct
+from trexlib.utils.string_util import is_not_empty
+from trexmodel.models.datastore.merchant_models import MerchantAcct, MerchantUser
 import logging
-from trexmodel import conf, program_conf
+from trexconf import conf, program_conf
 from datetime import datetime
 from trexmodel.models.datastore.model_decorators import model_transactional
-from trexlib.utils.common.common_util import sort_list, sort_dict_list
 from builtins import staticmethod
     
 
 
 #logger = logging.getLogger('model')
 logger = logging.getLogger('debug')
```

### Comparing `trex-model-1.3.9/trexmodel/models/datastore/system_models.py` & `trex-model-1.4.0/trexmodel/models/datastore/system_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 Created on 20 Apr 2020
 
 @author: jacklok
 '''
-from trexmodel import conf as model_conf, conf
+from trexconf import conf as model_conf
 from google.cloud import ndb
 from trexmodel.models.datastore.ndb_models import BaseNModel, DictModel
 
 class Country(BaseNModel, DictModel):
     cnty_id                 = ndb.IntegerProperty(required=True)
     cnty_code               = ndb.StringProperty(required=True)
     cnty_name               = ndb.StringProperty(required=True)
```

### Comparing `trex-model-1.3.9/trexmodel/models/datastore/voucher_models.py` & `trex-model-1.4.0/trexmodel/models/datastore/voucher_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from google.cloud import ndb
 from trexmodel.models.datastore.ndb_models import BaseNModel, DictModel
 import trexmodel.conf as model_conf
 from trexlib.utils.string_util import is_not_empty
 from trexmodel.models.datastore.merchant_models import MerchantAcct, \
     MerchantUser
 import logging
-from trexmodel import program_conf
+from trexconf import program_conf
 from datetime import datetime
 from trexmodel.program_conf import VOUCHER_REWARD_TYPE,\
     VOUCHER_REWARD_MAX_QUANTITY,\
     VOUCHER_REWARD_PRICE, VOUCHER_REWARD_BRAND,\
     VOUCHER_REWARD_MIN_SALES_AMOUNT,\
     VOUCHER_REWARD_DISCOUNT_RATE,\
     VOUCHER_REWARD_TYPE_DISCOUNT,\
```

### Comparing `trex-model-1.3.9/trexmodel/models/datastore/rating_models.py` & `trex-model-1.4.0/trexmodel/models/datastore/rating_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 @author: jacklok
 '''
 from trexmodel.models.datastore.ndb_models import BaseNModel, DictModel
 from google.cloud import ndb
 from trexmodel.models.datastore.merchant_models import MerchantAcct, Outlet
 from trexmodel.models.datastore.user_models import User
-from trexmodel import conf
+from trexconf import conf
 from datetime import datetime, timedelta
 import logging
 
 logger = logging.getLogger('model')
 
 class RatingBase(BaseNModel, DictModel):
     user_acct                           = ndb.KeyProperty(name="user_acct", kind=User)
```

### Comparing `trex-model-1.3.9/trexmodel/models/datastore/program_models.py` & `trex-model-1.4.0/trexmodel/models/datastore/program_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,19 +3,17 @@
 
 @author: jacklok
 '''
 from google.cloud import ndb
 from trexmodel.models.datastore.ndb_models import BaseNModel, DictModel
 import trexmodel.conf as model_conf
 from trexlib.utils.string_util import is_not_empty, random_string
-from trexmodel.models.datastore.merchant_models import MerchantAcct, Outlet,\
-    MerchantUser
-from trexmodel.models.datastore.coporate_models import CorporateAcct
+from trexmodel.models.datastore.merchant_models import MerchantAcct,MerchantUser
 import logging
-from trexmodel import conf, program_conf
+from trexconf import conf, program_conf
 from datetime import datetime
 from trexmodel.models.datastore.model_decorators import model_transactional
 from trexlib.utils.common.common_util import sort_list, sort_dict_list
     
 
 
 #logger = logging.getLogger('model')
```

### Comparing `trex-model-1.3.9/trexmodel/models/datastore/model_decorators.py` & `trex-model-1.4.0/trexmodel/models/datastore/model_decorators.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.9/trexmodel/models/datastore/ndb_models.py` & `trex-model-1.4.0/trexmodel/models/datastore/ndb_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 from datetime import datetime, date, time
 from trexlib.utils.string_util import is_not_empty 
 from trexlib.utils.log_util import get_tracelog
 from six import string_types 
 from trexlib.utils.common.date_util import increase_date 
 import logging
 #from google.cloud.ndb._datastore_query import Cursor
-from google.cloud.ndb import Cursor
-from trexlib import conf as lib_conf 
-from trexmodel import conf as model_conf
+#from google.cloud.ndb import Cursor
+from trexconf import conf as lib_conf 
+from trexconf import conf as model_conf
 from google.cloud.datastore.helpers import GeoPoint
  
 logger = logging.getLogger('model') 
 
 def convert_to_serializable_value(val, none_as_empty_string=False, gmt=0, 
                                   datetime_format=lib_conf.DEFAULT_DATETIME_FORMAT, 
                                   date_format=lib_conf.DEFAULT_DATE_FORMAT, 
@@ -284,15 +284,15 @@
         
         return cls.count_with_condition_query(query, limit=limit)
     
     @classmethod
     def count_with_condition_query(cls, query, limit=model_conf.MAX_FETCH_RECORD):    
         
         
-        return query.count(limit=limit, keys_only=True)
+        return query.count(limit=limit)
     
     @classmethod
     def list_all(cls, offset=0,  start_cursor=None, return_with_cursor=False, keys_only=False, 
                  limit=model_conf.MAX_FETCH_RECORD):
         
         query = cls.query()
         
@@ -407,15 +407,15 @@
             
         
         for word in lowercase_words_list:
             query = query.filter(cls.full_text_search_field == word)
             
         logger.debug('query=%s', query)
         
-        return query.count(limit=limit, keys_only=True)
+        return query.count(limit=limit)
             
            
         
     @classmethod
     def full_text_search(cls, text_search = None, query=None, offset=0,  start_cursor=None, return_with_cursor=False, keys_only=False, 
                          limit=model_conf.MAX_FETCH_RECORD_FULL_TEXT_SEARCH_PER_PAGE, to_lowercase=True):
         if query is None:
```

### Comparing `trex-model-1.3.9/trexmodel/models/datastore/analytic_models.py` & `trex-model-1.4.0/trexmodel/models/datastore/analytic_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 Created on 25 Jan 2021
 
 @author: jacklok
 '''
-from trexmodel import conf as model_conf
+from trexconf import conf as model_conf
 from google.cloud import ndb
 from trexmodel.models.datastore.ndb_models import BaseNModel, DictModel
 from datetime import timedelta
 from trexmodel.models.datastore.merchant_models import MerchantAcct
 
 class UpstreamData(BaseNModel, DictModel):
     merchant_acct           = ndb.KeyProperty(name="merchant_acct", kind=MerchantAcct)
```

### Comparing `trex-model-1.3.9/trexmodel/models/datastore/transaction_models.py` & `trex-model-1.4.0/trexmodel/models/datastore/transaction_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from trexmodel.models.datastore.user_models import User
 from trexmodel.models.datastore.customer_models import Customer,\
     CustomerMembership
 from trexlib.utils.string_util import is_not_empty
 from trexmodel.models.datastore.merchant_models import MerchantAcct, Outlet,\
     MerchantUser
 import logging
-from trexmodel import conf, program_conf
+from trexconf import conf, program_conf 
 from datetime import datetime, timedelta
 from trexmodel.utils.model.model_util import generate_transaction_id
 from trexmodel.models.datastore.membership_models import MerchantMembership,\
     MerchantTierMembership
 
 logger = logging.getLogger('model')
 
@@ -323,15 +323,22 @@
     @staticmethod
     def create_manual_transaction(customer, remarks=None, system_remarks=None, transact_outlet=None, transact_by=None, transact_datetime=None, is_sales_transaction=False, 
                                   allow_to_revert=True, is_membership_purchase=False, is_membership_renew=False): 
         return CustomerTransaction.create_system_transaction(customer, remarks=remarks, system_remarks=system_remarks, transact_outlet=transact_outlet, transact_by=transact_by, 
                                    transact_datetime=transact_datetime, reward_giveaway_method=program_conf.PROGRAM_REWARD_GIVEAWAY_METHOD_MANUAL,
                                    is_sales_transaction = is_sales_transaction, allow_to_revert=allow_to_revert, 
                                    is_membership_purchase=is_membership_purchase, is_membership_renew=is_membership_renew,
-                                   )    
+                                   )
+        
+    @staticmethod
+    def create_referral_transaction(customer, transact_outlet=None, transact_datetime=None, ): 
+        return CustomerTransaction.create_system_transaction(customer, transact_outlet=transact_outlet, 
+                                   transact_datetime=transact_datetime, reward_giveaway_method=program_conf.PROGRAM_REWARD_GIVEAWAY_METHOD_REFERRAL,
+                                   allow_to_revert=False,
+                                   )        
     
     @staticmethod
     def create_from_sales_transaction(customer, sales_transaction):
         if sales_transaction:
             customer_transaction = CustomerTransaction(
                                                         parent                          = customer.create_ndb_key(),
```

### Comparing `trex-model-1.3.9/trexmodel/models/datastore/marketing_models.py` & `trex-model-1.4.0/trexmodel/models/datastore/marketing_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 '''
 from trexmodel.models.datastore.ndb_models import BaseNModel, DictModel
 from google.cloud import ndb
 from trexmodel.models.datastore.merchant_models import MerchantUser,\
     MerchantAcct
 from trexlib.utils.string_util import is_not_empty, random_string
 from datetime import datetime
-from trexmodel import program_conf, conf
+from trexconf import conf
 import trexmodel.conf as model_conf
 import logging
 
 logger = logging.getLogger('model')
 
 class PushNotificationSetup(BaseNModel, DictModel):
     '''
```

### Comparing `trex-model-1.3.9/trexmodel/models/datastore/app_models.py` & `trex-model-1.4.0/trexmodel/models/datastore/app_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.9/trexmodel/models/datastore/customer_model_helpers.py` & `trex-model-1.4.0/trexmodel/models/datastore/customer_model_helpers.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.9/trexmodel/models/datastore/merchant_models.py` & `trex-model-1.4.0/trexmodel/models/datastore/merchant_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,17 @@
 from trexmodel.models.datastore.user_models import UserMin
 import trexmodel.conf as model_conf
 from trexlib.utils.security_util import generate_user_id, hash_password
 from trexlib.utils.string_util import random_number, is_empty, is_not_empty,\
     split_by_length, random_string
 import logging
 from datetime import datetime, timedelta
-from trexmodel import conf, program_conf
+from trexconf import conf, program_conf
 from trexmodel.models.datastore.system_models import Tagging
 from trexmodel.models.datastore.model_decorators import model_transactional
-from trexlib.utils.common.common_util import sort_dict_list
 from trexmodel.program_conf import LOYALTY_PACKAGE_LITE, LOYALTY_PRODUCT
 
 logger = logging.getLogger('model')
 #logger = logging.getLogger('debug')
 
 class BusinessEntity(BaseNModel, DictModel):
     company_name                = ndb.StringProperty(required=False)
@@ -86,15 +85,15 @@
     
     stat_figure_update_interval_in_minutes          = conf.MERCHANT_STAT_FIGURE_UPDATE_INTERVAL_IN_MINUTES
     stat_figure_update_datetime_format              = '%d-%m-%Y %H:%M:%S'
     
     dict_properties = ['company_name', 'brand_name', 'contact_name', 'business_reg_no', 'mobile_phone', 
                        'office_phone', 'fax_phone', 'email', 'account_code', 'country',
                        'registered_datetime', 'modified_datetime', 'plan_start_date', 'plan_end_date', 'currency_code', 
-                       'timezone',
+                       'timezone', 'effective_referral_program_count',
                        'published_program_configuration', 'published_referral_program_configuration', 
                        'published_voucher_configuration', 'membership_configuration', 
                        'tier_membership_configuration', 'prepaid_configuration', 'lucky_draw_configuration', 'product_modifier_configuration',
                        'dashboard_stat_figure', 'program_settings', 'is_tier_membership_configured', 'website', 
                        'product_package', 'loyalty_package','account_plan','outlet_count', 'outlet_limit',
                        'published_redemption_catalogue_configuration',
                        ]
@@ -122,14 +121,39 @@
         if self.account_plan:
             if self.account_plan.get('loyalty_package'):
                 return self.account_plan.get('loyalty_package')
         
         return LOYALTY_PACKAGE_LITE
     
     @property
+    def effective_referral_program_count(self):
+        if self.published_referral_program_configuration:
+            program_count = self.published_referral_program_configuration.get('count',0)
+            if program_count>0:
+                check_effective_count = 0
+                program_list = self.published_referral_program_configuration.get('programs');
+                today_date = datetime.today()
+                for program_details in program_list:
+                    start_date_str = program_details.get('start_date')
+                    start_date = datetime.strptime(start_date_str, '%d-%m-%Y')
+                    
+                    end_date_str = program_details.get('end_date')
+                    end_date = datetime.strptime(end_date_str, '%d-%m-%Y')
+                    
+                    if start_date<=today_date and today_date<=end_date:
+                        check_effective_count+=1
+                
+                return check_effective_count
+                    
+            else:
+                return program_count
+                
+        return 0
+    
+    @property
     def outlet_limit(self):
         if self.account_plan:
             if self.account_plan.get('outlet_limit'):
                 return self.account_plan.get('outlet_limit')
         
         return 1
```

### Comparing `trex-model-1.3.9/trexmodel/models/datastore/prepaid_models.py` & `trex-model-1.4.0/trexmodel/models/datastore/prepaid_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,19 +5,17 @@
 '''
 from google.cloud import ndb
 from trexmodel.models.datastore.ndb_models import BaseNModel, DictModel
 from trexmodel.models.datastore.user_models import User
 from trexmodel.models.datastore.merchant_models import MerchantAcct, Outlet, MerchantUser
 import logging, json
 from trexmodel import conf, program_conf
-from trexlib.utils.string_util import random_string, random_number, is_not_empty
-from datetime import datetime, timedelta
-import trexmodel.conf as model_conf
+from trexlib.utils.string_util import random_number, is_not_empty
+from datetime import datetime
 from trexlib.utils.common.common_util import sort_dict_list
-from trexmodel.utils.model.model_util import generate_transaction_id
 from dateutil.relativedelta import relativedelta
 from trexmodel.program_conf import PRODUCT_TYPES, LOYALTY_PRODUCT
 from trexlib.utils.crypto_util import encrypt
 
 logger = logging.getLogger('model')
 
 class PrepaidSettings(BaseNModel,DictModel):
@@ -564,17 +562,19 @@
         logger.debug('prepaid_scheme_details=%s', prepaid_scheme_details)
             
         topup_unit          = CustomerPrepaidReward.__calculate_topup_unit(topup_amount, prepaid_scheme_details)
         prepaid_amount      = CustomerPrepaidReward.__calculate_prepaid_amount(topup_unit, prepaid_scheme_details)
         topup_prepaid_rate  = CustomerPrepaidReward.__calculate_topup_prepaid_rate(prepaid_scheme_details)
         
         topup_by_key = None
+        topup_by_username = None
         
         if topup_by:
             topup_by_key = topup_by.create_ndb_key()
+            topup_by_username = topup_by.username
             
         if topup_datetime is None:
             topup_datetime = datetime.utcnow()
             
         merchant_acct               = customer_acct.registered_merchant_acct
         prepaid_topup_reward        = CustomerPrepaidReward(
                                                             parent                  = customer_acct.create_ndb_key(),
@@ -587,21 +587,57 @@
                                                             used_prepaid_amount     = .0,
                                                             prepaid_scheme_details  = prepaid_scheme_details,
                                                             
                                                             transaction_id          = transaction_id,
                                                             invoice_id              = invoice_id,
                                                             
                                                             topup_by                = topup_by_key,
-                                                            
+                                                            topup_by_username       = topup_by_username, 
                                                             topup_datetime          = topup_datetime,    
                                                             )
         
         prepaid_topup_reward.put()
         
         return prepaid_topup_reward
     
+    @staticmethod
+    def create(customer_acct, topup_outlet, 
+               topup_amount=0, topup_unit=0, topup_prepaid_rate = 1, 
+               prepaid_amount=.0, prepaid_scheme_details={}, 
+               topup_datetime=None, topup_by=None,
+               transaction_id=None, invoice_id=None,
+               ):
+        
+        merchant_acct  = customer_acct.registered_merchant_acct
+        
+        topup_by_key = None
+        topup_by_username = None
+        
+        if topup_by:
+            topup_by_key = topup_by.create_ndb_key()
+            topup_by_username = topup_by.username
+            
+        CustomerPrepaidReward(
+            parent                  = customer_acct.create_ndb_key(),
+            merchant_acct           = merchant_acct.create_ndb_key(),
+            topup_outlet            = topup_outlet.create_ndb_key() if topup_outlet else None,
+            topup_amount            = topup_amount,
+            topup_unit              = topup_unit,
+            prepaid_amount          = prepaid_amount,
+            topup_prepaid_rate      = topup_prepaid_rate,
+            used_prepaid_amount     = .0,
+            prepaid_scheme_details  = prepaid_scheme_details,
+            
+            transaction_id          = transaction_id,
+            invoice_id              = invoice_id,
+            
+            topup_by                = topup_by_key,
+            topup_by_username       = topup_by_username, 
+            topup_datetime          = topup_datetime,   
+             
+            )
     
     @staticmethod
     def delete_all_by_customer(customer):
         query = CustomerPrepaidReward.query(ancestor=customer.create_ndb_key())
         CustomerPrepaidReward.delete_multiples(query)
```

### Comparing `trex-model-1.3.9/trexmodel/models/datastore/lucky_draw_models.py` & `trex-model-1.4.0/trexmodel/models/datastore/lucky_draw_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 '''
 Created on 12 May 2023
 
 @author: jacklok
 '''
 import logging
-from trexmodel import program_conf
+from trexconf import program_conf
 import trexmodel.conf as model_conf
 from trexmodel.models.datastore.ndb_models import BaseNModel, DictModel
 from google.cloud import ndb
 from trexmodel.models.datastore.merchant_models import MerchantUser,\
     MerchantAcct, Outlet
 from trexlib.utils.string_util import is_not_empty, random_string, is_empty
 from datetime import datetime, timedelta
```

### Comparing `trex-model-1.3.9/trexmodel/models/datastore/admin_models.py` & `trex-model-1.4.0/trexmodel/models/datastore/admin_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 '''
 from google.cloud import ndb
 from trexmodel.models.datastore.user_models import UserMin
 from trexlib.utils.security_util import generate_user_id, hash_password
 from trexmodel.models.datastore.ndb_models import BaseNModel, DictModel
 from trexlib.utils.string_util import random_string
 from trexlib.utils.common.common_util import logger
-from trexlib import conf
+from trexconf import conf
 
 
 class SuperUser(UserMin):
     email                           = ndb.StringProperty(required=False)
     created_datetime                = ndb.DateTimeProperty(required=False, auto_now_add=True)
     
     dict_properties         = ['user_id', 'name', 'email', 'gravatar_url', 'active', 'locked',
```

### Comparing `trex-model-1.3.9/LICENSE` & `trex-model-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.9/trex_model.egg-info/SOURCES.txt` & `trex-model-1.4.0/trex_model.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.9/setup.py` & `trex-model-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
      name='trex-model',  
-     version='1.3.9',
+     version='1.4.0',
      author="Jack Lok",
      author_email="sglok77@gmail.com",
      description="TRex database module package",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://bitbucket.org/lokjac/trex-model",
      packages=setuptools.find_packages(),
```

