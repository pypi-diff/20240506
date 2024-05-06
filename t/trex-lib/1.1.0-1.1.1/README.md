# Comparing `tmp/trex-lib-1.1.0.tar.gz` & `tmp/trex-lib-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trex-lib-1.1.0.tar", last modified: Mon May  6 07:59:53 2024, max compression
+gzip compressed data, was "trex-lib-1.1.1.tar", last modified: Mon May  6 09:15:57 2024, max compression
```

## Comparing `trex-lib-1.1.0.tar` & `trex-lib-1.1.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:59:53.188233 trex-lib-1.1.0/
--rw-r--r--   0 jacklok    (501) staff       (20)     1052 2020-09-03 05:31:42.000000 trex-lib-1.1.0/LICENSE
--rw-r--r--   0 jacklok    (501) staff       (20)       58 2020-09-03 00:38:04.000000 trex-lib-1.1.0/MANIFEST.in
--rw-r--r--   0 jacklok    (501) staff       (20)      622 2024-05-06 07:59:53.187954 trex-lib-1.1.0/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)       34 2020-09-03 04:20:20.000000 trex-lib-1.1.0/README.md
--rw-r--r--   0 jacklok    (501) staff       (20)      172 2021-08-13 04:29:57.000000 trex-lib-1.1.0/pyproject.toml
--rw-r--r--   0 jacklok    (501) staff       (20)       75 2024-05-06 07:59:53.189523 trex-lib-1.1.0/setup.cfg
--rw-r--r--   0 jacklok    (501) staff       (20)     1213 2024-05-06 07:59:30.000000 trex-lib-1.1.0/setup.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:59:53.186845 trex-lib-1.1.0/trex_lib.egg-info/
--rw-r--r--   0 jacklok    (501) staff       (20)      622 2024-05-06 07:59:53.000000 trex-lib-1.1.0/trex_lib.egg-info/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)     1482 2024-05-06 07:59:53.000000 trex-lib-1.1.0/trex_lib.egg-info/SOURCES.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        1 2024-05-06 07:59:53.000000 trex-lib-1.1.0/trex_lib.egg-info/dependency_links.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       89 2024-05-06 07:59:53.000000 trex-lib-1.1.0/trex_lib.egg-info/requires.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       14 2024-05-06 07:59:53.000000 trex-lib-1.1.0/trex_lib.egg-info/top_level.txt
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:59:53.149501 trex-lib-1.1.0/trexlib/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-04 07:13:04.000000 trex-lib-1.1.0/trexlib/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     5426 2024-04-05 01:57:54.000000 trex-lib-1.1.0/trexlib/conf_to_remove.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:59:53.150637 trex-lib-1.1.0/trexlib/libs/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-22 09:26:13.000000 trex-lib-1.1.0/trexlib/libs/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:59:53.151292 trex-lib-1.1.0/trexlib/libs/controllers/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2023-02-13 02:03:08.000000 trex-lib-1.1.0/trexlib/libs/controllers/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     9783 2024-04-29 04:45:24.000000 trex-lib-1.1.0/trexlib/libs/controllers/task_base_routes.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:59:53.152578 trex-lib-1.1.0/trexlib/libs/facebook/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2024-04-04 09:51:48.000000 trex-lib-1.1.0/trexlib/libs/facebook/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:59:53.153207 trex-lib-1.1.0/trexlib/libs/facebook/util/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2024-04-04 09:52:59.000000 trex-lib-1.1.0/trexlib/libs/facebook/util/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2726 2024-04-08 02:49:39.000000 trex-lib-1.1.0/trexlib/libs/facebook/util/whatsapp_util.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:59:53.154519 trex-lib-1.1.0/trexlib/libs/firebase/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2022-06-09 04:14:24.000000 trex-lib-1.1.0/trexlib/libs/firebase/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      378 2022-06-09 06:38:00.000000 trex-lib-1.1.0/trexlib/libs/firebase/firebase_helper.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:59:53.156548 trex-lib-1.1.0/trexlib/libs/flask_wtf/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-22 09:26:46.000000 trex-lib-1.1.0/trexlib/libs/flask_wtf/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      133 2021-01-22 09:30:44.000000 trex-lib-1.1.0/trexlib/libs/flask_wtf/crsf_ext.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1918 2024-05-01 14:52:30.000000 trex-lib-1.1.0/trexlib/libs/flask_wtf/request_wrapper.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:59:53.165453 trex-lib-1.1.0/trexlib/utils/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-01 09:38:27.000000 trex-lib-1.1.0/trexlib/utils/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:59:53.181199 trex-lib-1.1.0/trexlib/utils/common/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-lib-1.1.0/trexlib/utils/common/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4514 2022-09-26 14:54:31.000000 trex-lib-1.1.0/trexlib/utils/common/common_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      926 2023-08-30 15:08:13.000000 trex-lib-1.1.0/trexlib/utils/common/config_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      488 2020-09-01 10:21:00.000000 trex-lib-1.1.0/trexlib/utils/common/conftest.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1194 2020-09-04 02:28:26.000000 trex-lib-1.1.0/trexlib/utils/common/crm_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1573 2021-04-21 02:37:36.000000 trex-lib-1.1.0/trexlib/utils/common/currency_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     3707 2024-04-29 04:45:34.000000 trex-lib-1.1.0/trexlib/utils/common/date_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      290 2020-09-01 10:20:46.000000 trex-lib-1.1.0/trexlib/utils/common/float_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4201 2021-03-04 08:12:18.000000 trex-lib-1.1.0/trexlib/utils/common/format_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1087 2024-04-29 04:45:42.000000 trex-lib-1.1.0/trexlib/utils/common/pagination_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1087 2021-06-24 07:11:43.000000 trex-lib-1.1.0/trexlib/utils/common/phone_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      825 2021-08-13 09:35:21.000000 trex-lib-1.1.0/trexlib/utils/common/user_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      933 2024-01-27 15:50:32.000000 trex-lib-1.1.0/trexlib/utils/crypto_util.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:59:53.185002 trex-lib-1.1.0/trexlib/utils/google/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-20 04:05:45.000000 trex-lib-1.1.0/trexlib/utils/google/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)    12870 2024-04-29 04:38:39.000000 trex-lib-1.1.0/trexlib/utils/google/bigquery_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4295 2024-04-29 04:46:45.000000 trex-lib-1.1.0/trexlib/utils/google/cloud_tasks_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1365 2024-04-29 04:44:56.000000 trex-lib-1.1.0/trexlib/utils/google/gcloud_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      159 2020-09-04 07:30:52.000000 trex-lib-1.1.0/trexlib/utils/log_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      766 2024-03-21 04:18:42.000000 trex-lib-1.1.0/trexlib/utils/member_card_generator.py
--rw-r--r--   0 jacklok    (501) staff       (20)     3216 2024-04-29 04:46:01.000000 trex-lib-1.1.0/trexlib/utils/security_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     8213 2024-04-29 04:46:10.000000 trex-lib-1.1.0/trexlib/utils/sms_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     5170 2024-04-22 11:10:51.000000 trex-lib-1.1.0/trexlib/utils/string_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1277 2020-09-04 07:38:09.000000 trex-lib-1.1.0/trexlib/utils/url_util.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:15:57.740449 trex-lib-1.1.1/
+-rw-r--r--   0 jacklok    (501) staff       (20)     1052 2020-09-03 05:31:42.000000 trex-lib-1.1.1/LICENSE
+-rw-r--r--   0 jacklok    (501) staff       (20)       58 2020-09-03 00:38:04.000000 trex-lib-1.1.1/MANIFEST.in
+-rw-r--r--   0 jacklok    (501) staff       (20)      622 2024-05-06 09:15:57.740260 trex-lib-1.1.1/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)       34 2020-09-03 04:20:20.000000 trex-lib-1.1.1/README.md
+-rw-r--r--   0 jacklok    (501) staff       (20)      172 2021-08-13 04:29:57.000000 trex-lib-1.1.1/pyproject.toml
+-rw-r--r--   0 jacklok    (501) staff       (20)       75 2024-05-06 09:15:57.741258 trex-lib-1.1.1/setup.cfg
+-rw-r--r--   0 jacklok    (501) staff       (20)     1213 2024-05-06 09:15:33.000000 trex-lib-1.1.1/setup.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:15:57.739617 trex-lib-1.1.1/trex_lib.egg-info/
+-rw-r--r--   0 jacklok    (501) staff       (20)      622 2024-05-06 09:15:57.000000 trex-lib-1.1.1/trex_lib.egg-info/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)     1482 2024-05-06 09:15:57.000000 trex-lib-1.1.1/trex_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        1 2024-05-06 09:15:57.000000 trex-lib-1.1.1/trex_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       89 2024-05-06 09:15:57.000000 trex-lib-1.1.1/trex_lib.egg-info/requires.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       14 2024-05-06 09:15:57.000000 trex-lib-1.1.1/trex_lib.egg-info/top_level.txt
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:15:57.719586 trex-lib-1.1.1/trexlib/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-04 07:13:04.000000 trex-lib-1.1.1/trexlib/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     5426 2024-04-05 01:57:54.000000 trex-lib-1.1.1/trexlib/conf_to_remove.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:15:57.720392 trex-lib-1.1.1/trexlib/libs/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-22 09:26:13.000000 trex-lib-1.1.1/trexlib/libs/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:15:57.721143 trex-lib-1.1.1/trexlib/libs/controllers/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2023-02-13 02:03:08.000000 trex-lib-1.1.1/trexlib/libs/controllers/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     9783 2024-04-29 04:45:24.000000 trex-lib-1.1.1/trexlib/libs/controllers/task_base_routes.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:15:57.722010 trex-lib-1.1.1/trexlib/libs/facebook/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2024-04-04 09:51:48.000000 trex-lib-1.1.1/trexlib/libs/facebook/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:15:57.722666 trex-lib-1.1.1/trexlib/libs/facebook/util/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2024-04-04 09:52:59.000000 trex-lib-1.1.1/trexlib/libs/facebook/util/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2727 2024-05-06 09:13:17.000000 trex-lib-1.1.1/trexlib/libs/facebook/util/whatsapp_util.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:15:57.723469 trex-lib-1.1.1/trexlib/libs/firebase/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2022-06-09 04:14:24.000000 trex-lib-1.1.1/trexlib/libs/firebase/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      378 2022-06-09 06:38:00.000000 trex-lib-1.1.1/trexlib/libs/firebase/firebase_helper.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:15:57.724656 trex-lib-1.1.1/trexlib/libs/flask_wtf/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-22 09:26:46.000000 trex-lib-1.1.1/trexlib/libs/flask_wtf/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      133 2021-01-22 09:30:44.000000 trex-lib-1.1.1/trexlib/libs/flask_wtf/crsf_ext.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1918 2024-05-01 14:52:30.000000 trex-lib-1.1.1/trexlib/libs/flask_wtf/request_wrapper.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:15:57.730071 trex-lib-1.1.1/trexlib/utils/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-01 09:38:27.000000 trex-lib-1.1.1/trexlib/utils/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:15:57.736565 trex-lib-1.1.1/trexlib/utils/common/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-lib-1.1.1/trexlib/utils/common/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4514 2022-09-26 14:54:31.000000 trex-lib-1.1.1/trexlib/utils/common/common_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      926 2023-08-30 15:08:13.000000 trex-lib-1.1.1/trexlib/utils/common/config_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      488 2020-09-01 10:21:00.000000 trex-lib-1.1.1/trexlib/utils/common/conftest.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1194 2020-09-04 02:28:26.000000 trex-lib-1.1.1/trexlib/utils/common/crm_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1573 2021-04-21 02:37:36.000000 trex-lib-1.1.1/trexlib/utils/common/currency_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     3707 2024-04-29 04:45:34.000000 trex-lib-1.1.1/trexlib/utils/common/date_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      290 2020-09-01 10:20:46.000000 trex-lib-1.1.1/trexlib/utils/common/float_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4201 2021-03-04 08:12:18.000000 trex-lib-1.1.1/trexlib/utils/common/format_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1087 2024-04-29 04:45:42.000000 trex-lib-1.1.1/trexlib/utils/common/pagination_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1087 2021-06-24 07:11:43.000000 trex-lib-1.1.1/trexlib/utils/common/phone_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      825 2021-08-13 09:35:21.000000 trex-lib-1.1.1/trexlib/utils/common/user_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      933 2024-01-27 15:50:32.000000 trex-lib-1.1.1/trexlib/utils/crypto_util.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:15:57.738944 trex-lib-1.1.1/trexlib/utils/google/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-20 04:05:45.000000 trex-lib-1.1.1/trexlib/utils/google/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    12870 2024-04-29 04:38:39.000000 trex-lib-1.1.1/trexlib/utils/google/bigquery_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4132 2024-05-06 09:13:26.000000 trex-lib-1.1.1/trexlib/utils/google/cloud_tasks_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1365 2024-04-29 04:44:56.000000 trex-lib-1.1.1/trexlib/utils/google/gcloud_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      159 2020-09-04 07:30:52.000000 trex-lib-1.1.1/trexlib/utils/log_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      766 2024-03-21 04:18:42.000000 trex-lib-1.1.1/trexlib/utils/member_card_generator.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     3216 2024-04-29 04:46:01.000000 trex-lib-1.1.1/trexlib/utils/security_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     8213 2024-04-29 04:46:10.000000 trex-lib-1.1.1/trexlib/utils/sms_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     5170 2024-04-22 11:10:51.000000 trex-lib-1.1.1/trexlib/utils/string_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1277 2020-09-04 07:38:09.000000 trex-lib-1.1.1/trexlib/utils/url_util.py
```

### Comparing `trex-lib-1.1.0/LICENSE` & `trex-lib-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.0/PKG-INFO` & `trex-lib-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trex-lib
-Version: 1.1.0
+Version: 1.1.1
 Summary: TRex Core library package
 Home-page: https://bitbucket.org/lokjac/trex-lib
 Author: Jack Lok
 Author-email: sglok77@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `trex-lib-1.1.0/setup.py` & `trex-lib-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
      name='trex-lib',  
-     version='1.1.0',
+     version='1.1.1',
      author="Jack Lok",
      author_email="sglok77@gmail.com",
      description="TRex Core library package",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://bitbucket.org/lokjac/trex-lib",
      packages=setuptools.find_packages(),
```

### Comparing `trex-lib-1.1.0/trex_lib.egg-info/PKG-INFO` & `trex-lib-1.1.1/trex_lib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trex-lib
-Version: 1.1.0
+Version: 1.1.1
 Summary: TRex Core library package
 Home-page: https://bitbucket.org/lokjac/trex-lib
 Author: Jack Lok
 Author-email: sglok77@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `trex-lib-1.1.0/trex_lib.egg-info/SOURCES.txt` & `trex-lib-1.1.1/trex_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.0/trexlib/conf_to_remove.py` & `trex-lib-1.1.1/trexlib/conf_to_remove.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.0/trexlib/libs/controllers/task_base_routes.py` & `trex-lib-1.1.1/trexlib/libs/controllers/task_base_routes.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.0/trexlib/libs/facebook/util/whatsapp_util.py` & `trex-lib-1.1.1/trexlib/libs/facebook/util/whatsapp_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 '''
 Created on 4 Apr 2024
 
 @author: jacklok
 '''
 import requests, logging
-from trexlib.conf import WHATSAPP_TOKEN, WHATSAPP_PHONE_NUMBER_ID,FACEBOOK_API_VERSION
+from trexconf.conf import WHATSAPP_TOKEN, WHATSAPP_PHONE_NUMBER_ID,FACEBOOK_API_VERSION
 
 logger = logging.getLogger('utils')
     
 def _construct_whatasapp_message_header():
     return {
                 "Authorization": f"Bearer %s" % WHATSAPP_TOKEN,
                 "Content-Type": "application/json",
```

### Comparing `trex-lib-1.1.0/trexlib/libs/flask_wtf/request_wrapper.py` & `trex-lib-1.1.1/trexlib/libs/flask_wtf/request_wrapper.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.0/trexlib/utils/common/common_util.py` & `trex-lib-1.1.1/trexlib/utils/common/common_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.0/trexlib/utils/common/config_util.py` & `trex-lib-1.1.1/trexlib/utils/common/config_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.0/trexlib/utils/common/crm_util.py` & `trex-lib-1.1.1/trexlib/utils/common/crm_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.0/trexlib/utils/common/currency_util.py` & `trex-lib-1.1.1/trexlib/utils/common/currency_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.0/trexlib/utils/common/date_util.py` & `trex-lib-1.1.1/trexlib/utils/common/date_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.0/trexlib/utils/common/format_util.py` & `trex-lib-1.1.1/trexlib/utils/common/format_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.0/trexlib/utils/common/pagination_util.py` & `trex-lib-1.1.1/trexlib/utils/common/pagination_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.0/trexlib/utils/common/phone_util.py` & `trex-lib-1.1.1/trexlib/utils/common/phone_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.0/trexlib/utils/common/user_util.py` & `trex-lib-1.1.1/trexlib/utils/common/user_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.0/trexlib/utils/crypto_util.py` & `trex-lib-1.1.1/trexlib/utils/crypto_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.0/trexlib/utils/google/bigquery_util.py` & `trex-lib-1.1.1/trexlib/utils/google/bigquery_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.0/trexlib/utils/google/cloud_tasks_util.py` & `trex-lib-1.1.1/trexlib/utils/google/cloud_tasks_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from trexconf import conf as lib_conf 
 import logging, json
 from datetime import datetime, timedelta
 from google.oauth2 import service_account 
 from google.protobuf import timestamp_pb2
 from trexlib.utils.security_util import create_basic_authentication, verfiy_basic_authentication
 from trexlib.utils.string_util import random_string
-#from trexlib.conf_to_remove import SYSTEM_TASK_SERVICE_ACCOUNT_KEY, SYSTEM_TASK_GCLOUD_PROJECT_ID, SYSTEM_TASK_GCLOUD_LOCATION, SYSTEM_TASK_SERVICE_ACCOUNT_EMAIL
 
 logger = logging.getLogger('utils-debug')
 
 def create_task(task_url, queue_name, payload=None, in_seconds=None, http_method='get', headers=None, 
                 credential_path=None, 
                 project_id=None, 
                 location=None,
```

### Comparing `trex-lib-1.1.0/trexlib/utils/google/gcloud_util.py` & `trex-lib-1.1.1/trexlib/utils/google/gcloud_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.0/trexlib/utils/member_card_generator.py` & `trex-lib-1.1.1/trexlib/utils/member_card_generator.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.0/trexlib/utils/security_util.py` & `trex-lib-1.1.1/trexlib/utils/security_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.0/trexlib/utils/sms_util.py` & `trex-lib-1.1.1/trexlib/utils/sms_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.0/trexlib/utils/string_util.py` & `trex-lib-1.1.1/trexlib/utils/string_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.0/trexlib/utils/url_util.py` & `trex-lib-1.1.1/trexlib/utils/url_util.py`

 * *Files identical despite different names*

