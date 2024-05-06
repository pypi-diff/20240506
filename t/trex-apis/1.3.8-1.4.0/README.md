# Comparing `tmp/trex-apis-1.3.8.tar.gz` & `tmp/trex-apis-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trex-apis-1.3.8.tar", last modified: Mon Apr  8 02:59:47 2024, max compression
+gzip compressed data, was "trex-apis-1.4.0.tar", last modified: Mon May  6 07:51:15 2024, max compression
```

## Comparing `trex-apis-1.3.8.tar` & `trex-apis-1.4.0.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-08 02:59:47.335711 trex-apis-1.3.8/
--rw-r--r--   0 jacklok    (501) staff       (20)      444 2024-04-08 02:59:47.335597 trex-apis-1.3.8/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)       25 2021-06-30 02:28:26.000000 trex-apis-1.3.8/README.md
--rw-r--r--   0 jacklok    (501) staff       (20)       75 2024-04-08 02:59:47.336624 trex-apis-1.3.8/setup.cfg
--rw-r--r--   0 jacklok    (501) staff       (20)      713 2024-04-08 02:58:47.000000 trex-apis-1.3.8/setup.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-08 02:59:47.334947 trex-apis-1.3.8/trex_apis.egg-info/
--rw-r--r--   0 jacklok    (501) staff       (20)      444 2024-04-08 02:59:47.000000 trex-apis-1.3.8/trex_apis.egg-info/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)     1628 2024-04-08 02:59:47.000000 trex-apis-1.3.8/trex_apis.egg-info/SOURCES.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        1 2024-04-08 02:59:47.000000 trex-apis-1.3.8/trex_apis.egg-info/dependency_links.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       23 2024-04-08 02:59:47.000000 trex-apis-1.3.8/trex_apis.egg-info/requires.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        8 2024-04-08 02:59:47.000000 trex-apis-1.3.8/trex_apis.egg-info/top_level.txt
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-08 02:59:47.297321 trex-apis-1.3.8/trexapi/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:30:07.000000 trex-apis-1.3.8/trexapi/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1372 2024-04-05 03:13:41.000000 trex-apis-1.3.8/trexapi/conf.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-08 02:59:47.321554 trex-apis-1.3.8/trexapi/controllers/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:45:28.000000 trex-apis-1.3.8/trexapi/controllers/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4523 2023-05-23 05:00:09.000000 trex-apis-1.3.8/trexapi/controllers/api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7080 2023-12-04 14:21:25.000000 trex-apis-1.3.8/trexapi/controllers/app_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    44555 2023-12-13 09:05:54.000000 trex-apis-1.3.8/trexapi/controllers/customer_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     6945 2023-04-13 05:36:42.000000 trex-apis-1.3.8/trexapi/controllers/customer_membership_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4750 2023-01-30 07:03:11.000000 trex-apis-1.3.8/trexapi/controllers/customer_reward_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    14912 2024-01-26 08:21:50.000000 trex-apis-1.3.8/trexapi/controllers/loyalty_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    14268 2024-02-05 07:27:46.000000 trex-apis-1.3.8/trexapi/controllers/lucky_draw_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    22414 2024-02-07 06:33:19.000000 trex-apis-1.3.8/trexapi/controllers/merchant_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7436 2024-01-30 09:36:58.000000 trex-apis-1.3.8/trexapi/controllers/message_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    11609 2024-01-30 15:20:28.000000 trex-apis-1.3.8/trexapi/controllers/outlet_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1430 2022-09-26 04:18:01.000000 trex-apis-1.3.8/trexapi/controllers/payment_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    24944 2023-05-23 09:32:47.000000 trex-apis-1.3.8/trexapi/controllers/pos_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     8448 2024-02-01 01:40:55.000000 trex-apis-1.3.8/trexapi/controllers/prepaid_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     5450 2024-01-24 14:48:05.000000 trex-apis-1.3.8/trexapi/controllers/rating_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    10501 2024-02-05 02:35:34.000000 trex-apis-1.3.8/trexapi/controllers/redemption_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    27474 2024-01-29 10:13:52.000000 trex-apis-1.3.8/trexapi/controllers/reward_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    13578 2024-01-25 03:26:42.000000 trex-apis-1.3.8/trexapi/controllers/sales_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)      998 2023-04-18 06:08:18.000000 trex-apis-1.3.8/trexapi/controllers/transaction_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    87341 2024-04-08 02:59:37.000000 trex-apis-1.3.8/trexapi/controllers/user_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2996 2024-01-19 04:06:09.000000 trex-apis-1.3.8/trexapi/controllers/user_reward_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    16728 2024-01-19 03:44:19.000000 trex-apis-1.3.8/trexapi/controllers/voucher_api_routes.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-08 02:59:47.323184 trex-apis-1.3.8/trexapi/decorators/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-01 08:42:13.000000 trex-apis-1.3.8/trexapi/decorators/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)    11971 2024-03-01 01:12:37.000000 trex-apis-1.3.8/trexapi/decorators/api_decorators.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-08 02:59:47.328264 trex-apis-1.3.8/trexapi/forms/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-12 06:42:53.000000 trex-apis-1.3.8/trexapi/forms/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7539 2023-12-13 05:36:24.000000 trex-apis-1.3.8/trexapi/forms/customer_api_forms.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7285 2023-04-18 02:42:03.000000 trex-apis-1.3.8/trexapi/forms/reward_api_forms.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1547 2023-04-18 02:41:54.000000 trex-apis-1.3.8/trexapi/forms/sales_api_forms.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4548 2023-11-22 08:18:38.000000 trex-apis-1.3.8/trexapi/forms/user_api_forms.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-08 02:59:47.329522 trex-apis-1.3.8/trexapi/libs/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-05 10:17:19.000000 trex-apis-1.3.8/trexapi/libs/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1143 2021-07-05 10:57:23.000000 trex-apis-1.3.8/trexapi/libs/flask_auth_wrapper.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-08 02:59:47.333021 trex-apis-1.3.8/trexapi/utils/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-08 10:01:06.000000 trex-apis-1.3.8/trexapi/utils/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2983 2024-01-03 03:38:30.000000 trex-apis-1.3.8/trexapi/utils/api_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)      501 2024-01-30 09:47:06.000000 trex-apis-1.3.8/trexapi/utils/push_notification_helper.py
--rw-r--r--   0 jacklok    (501) staff       (20)     9242 2024-03-14 09:07:57.000000 trex-apis-1.3.8/trexapi/utils/redemption_catalogue_helper.py
--rw-r--r--   0 jacklok    (501) staff       (20)    79248 2024-01-29 13:58:07.000000 trex-apis-1.3.8/trexapi/utils/reward_transaction_helper.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:51:15.126019 trex-apis-1.4.0/
+-rw-r--r--   0 jacklok    (501) staff       (20)      547 2024-05-06 07:51:15.125821 trex-apis-1.4.0/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)       25 2021-06-30 02:28:26.000000 trex-apis-1.4.0/README.md
+-rw-r--r--   0 jacklok    (501) staff       (20)       75 2024-05-06 07:51:15.126945 trex-apis-1.4.0/setup.cfg
+-rw-r--r--   0 jacklok    (501) staff       (20)      808 2024-05-06 07:51:03.000000 trex-apis-1.4.0/setup.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:51:15.125123 trex-apis-1.4.0/trex_apis.egg-info/
+-rw-r--r--   0 jacklok    (501) staff       (20)      547 2024-05-06 07:51:14.000000 trex-apis-1.4.0/trex_apis.egg-info/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)     1658 2024-05-06 07:51:14.000000 trex-apis-1.4.0/trex_apis.egg-info/SOURCES.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        1 2024-05-06 07:51:14.000000 trex-apis-1.4.0/trex_apis.egg-info/dependency_links.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       66 2024-05-06 07:51:14.000000 trex-apis-1.4.0/trex_apis.egg-info/requires.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        8 2024-05-06 07:51:14.000000 trex-apis-1.4.0/trex_apis.egg-info/top_level.txt
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:51:15.074362 trex-apis-1.4.0/trexapi/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:30:07.000000 trex-apis-1.4.0/trexapi/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1474 2024-05-04 13:45:53.000000 trex-apis-1.4.0/trexapi/conf.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:51:15.106435 trex-apis-1.4.0/trexapi/controllers/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:45:28.000000 trex-apis-1.4.0/trexapi/controllers/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4562 2024-05-05 09:45:58.000000 trex-apis-1.4.0/trexapi/controllers/api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     6424 2024-04-30 09:04:02.000000 trex-apis-1.4.0/trexapi/controllers/app_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    44879 2024-04-30 09:15:08.000000 trex-apis-1.4.0/trexapi/controllers/customer_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     6945 2023-04-13 05:36:42.000000 trex-apis-1.4.0/trexapi/controllers/customer_membership_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4750 2023-01-30 07:03:11.000000 trex-apis-1.4.0/trexapi/controllers/customer_reward_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    14687 2024-04-29 08:25:29.000000 trex-apis-1.4.0/trexapi/controllers/loyalty_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    14233 2024-04-29 09:09:32.000000 trex-apis-1.4.0/trexapi/controllers/lucky_draw_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    29768 2024-05-04 14:17:59.000000 trex-apis-1.4.0/trexapi/controllers/merchant_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7522 2024-05-05 09:48:00.000000 trex-apis-1.4.0/trexapi/controllers/message_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    11609 2024-01-30 15:20:28.000000 trex-apis-1.4.0/trexapi/controllers/outlet_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1430 2022-09-26 04:18:01.000000 trex-apis-1.4.0/trexapi/controllers/payment_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    24944 2023-05-23 09:32:47.000000 trex-apis-1.4.0/trexapi/controllers/pos_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     8448 2024-02-01 01:40:55.000000 trex-apis-1.4.0/trexapi/controllers/prepaid_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     5450 2024-01-24 14:48:05.000000 trex-apis-1.4.0/trexapi/controllers/rating_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    10026 2024-04-29 08:25:02.000000 trex-apis-1.4.0/trexapi/controllers/redemption_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    27186 2024-05-05 10:03:43.000000 trex-apis-1.4.0/trexapi/controllers/reward_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    13578 2024-05-05 10:07:29.000000 trex-apis-1.4.0/trexapi/controllers/sales_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      998 2023-04-18 06:08:18.000000 trex-apis-1.4.0/trexapi/controllers/transaction_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    97589 2024-05-05 10:43:46.000000 trex-apis-1.4.0/trexapi/controllers/user_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2996 2024-01-19 04:06:09.000000 trex-apis-1.4.0/trexapi/controllers/user_reward_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    16927 2024-05-05 10:11:04.000000 trex-apis-1.4.0/trexapi/controllers/voucher_api_routes.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:51:15.108282 trex-apis-1.4.0/trexapi/decorators/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-01 08:42:13.000000 trex-apis-1.4.0/trexapi/decorators/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    11971 2024-03-01 01:12:37.000000 trex-apis-1.4.0/trexapi/decorators/api_decorators.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:51:15.113437 trex-apis-1.4.0/trexapi/forms/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-12 06:42:53.000000 trex-apis-1.4.0/trexapi/forms/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7539 2024-04-24 10:25:39.000000 trex-apis-1.4.0/trexapi/forms/customer_api_forms.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7285 2023-04-18 02:42:03.000000 trex-apis-1.4.0/trexapi/forms/reward_api_forms.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1547 2023-04-18 02:41:54.000000 trex-apis-1.4.0/trexapi/forms/sales_api_forms.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4548 2023-11-22 08:18:38.000000 trex-apis-1.4.0/trexapi/forms/user_api_forms.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:51:15.116417 trex-apis-1.4.0/trexapi/libs/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-05 10:17:19.000000 trex-apis-1.4.0/trexapi/libs/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      913 2024-04-22 02:25:05.000000 trex-apis-1.4.0/trexapi/libs/api_decorator.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1143 2021-07-05 10:57:23.000000 trex-apis-1.4.0/trexapi/libs/flask_auth_wrapper.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:51:15.122428 trex-apis-1.4.0/trexapi/utils/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-08 10:01:06.000000 trex-apis-1.4.0/trexapi/utils/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2984 2024-05-05 10:11:27.000000 trex-apis-1.4.0/trexapi/utils/api_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      501 2024-01-30 09:47:06.000000 trex-apis-1.4.0/trexapi/utils/push_notification_helper.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7293 2024-05-02 06:28:02.000000 trex-apis-1.4.0/trexapi/utils/redemption_catalogue_helper.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    79101 2024-04-29 07:53:19.000000 trex-apis-1.4.0/trexapi/utils/reward_transaction_helper.py
```

### Comparing `trex-apis-1.3.8/trex_apis.egg-info/SOURCES.txt` & `trex-apis-1.4.0/trex_apis.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -34,13 +34,14 @@
 trexapi/decorators/api_decorators.py
 trexapi/forms/__init__.py
 trexapi/forms/customer_api_forms.py
 trexapi/forms/reward_api_forms.py
 trexapi/forms/sales_api_forms.py
 trexapi/forms/user_api_forms.py
 trexapi/libs/__init__.py
+trexapi/libs/api_decorator.py
 trexapi/libs/flask_auth_wrapper.py
 trexapi/utils/__init__.py
 trexapi/utils/api_helpers.py
 trexapi/utils/push_notification_helper.py
 trexapi/utils/redemption_catalogue_helper.py
 trexapi/utils/reward_transaction_helper.py
```

### Comparing `trex-apis-1.3.8/trexapi/conf.py` & `trex-apis-1.4.0/trexapi/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,7 +20,11 @@
 LUCKY_DRAW_URL                                                  = os.environ.get('LUCKY_DRAW_URL')
 
 FIREBASE_SERVICE_ACCOUNT_KEY_PATH                               = os.environ.get('FIREBASE_SERVICE_ACCOUNT_KEY_PATH')
 
 USE_VERIFICATION_REQUEST_ID                                     = os.environ.get('USE_VERIFICATION_REQUEST_ID')
 
 SEND_REAL_MESSAGE                                               = os.environ.get('SEND_REAL_MESSAGE')
+
+REFER_BASE_URL                                                  = os.environ.get('REFER_BASE_URL')
+
+
```

### Comparing `trex-apis-1.3.8/trexapi/controllers/api_routes.py` & `trex-apis-1.4.0/trexapi/controllers/api_routes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 '''
 Created on 30 Jun 2021
 
 @author: jacklok
 '''
 
-from flask import Blueprint, request, Response, session 
+from flask import Blueprint, session 
 from flask_restful import Resource, abort
 import logging
 from flask_httpauth import HTTPBasicAuth
-from trexapi import conf
 from flask_restful import Api
 from trexmodel.utils.model.model_util import create_db_client
 from trexmodel.models.datastore.merchant_models import MerchantUser
 import hashlib
-from random import random
-from trexlib.utils.string_util import random_string, is_not_empty
-from flask.json import jsonify
+from trexlib.utils.string_util import random_string
 from datetime import datetime, timedelta
-from trexapi import conf as api_conf
+from trexconf import conf as api_conf
 from trexlib.utils.crypto_util import encrypt_json
+from trexlib.libs.flask_wtf.request_wrapper import session_value
 
-#logger = logging.getLogger('api')
-logger = logging.getLogger('debug')
+logger = logging.getLogger('api')
+#logger = logging.getLogger('debug')
 
 auth = HTTPBasicAuth()
 #auth = HTTPBasicAuthWrapper()
 
 
 api_bp = Blueprint('api_base_bp', __name__,
                                  template_folder='templates',
@@ -71,23 +69,25 @@
 def __generate_random():
     return hashlib.md5(str(random_string(6)).encode('utf-8')).hexdigest()
 
 def default_generate_nonce():
     session["auth_nonce"] = __generate_random()
     return session["auth_nonce"]
  
-def default_verify_nonce(nonce):
-    return nonce == session.get("auth_nonce")
+@session_value
+def default_verify_nonce(session_value, nonce):
+    return nonce == session_value.get("auth_nonce")
 
 def default_generate_opaque():
     session["auth_opaque"] = __generate_random()
     return session["auth_opaque"]
 
-def default_verify_opaque(opaque):
-    return opaque == session.get("auth_opaque")
+@session_value
+def default_verify_opaque(session_value, opaque):
+    return opaque == session_value.get("auth_opaque")
     
 class APIBaseResource(Resource):
     @property
     def realm(self):
         return 'base'
     
     def generate_ha1(self, username, password):
@@ -114,24 +114,24 @@
     
     
 class APIVersionResource(APIBaseResource):
     
     @auth.login_required
     def get(self):
         output_json =  {
-                        'version'   :   conf.VERSION,
+                        'version'   :   api_conf.API_VERSION,
                         'username'  :   auth.current_user()
                         }
         
         return output_json
     
 class APIResource(APIBaseResource):
     
     def get(self):
-        return conf.VERSION    
+        return api_conf.API_VERSION    
 
 '''
 class SecureAPIResource(AuthenticateAPIResource):  
     
     def __init__(self):
         super(SecureAPIResource, self).__init__()
```

### Comparing `trex-apis-1.3.8/trexapi/controllers/app_api_routes.py` & `trex-apis-1.4.0/trexapi/controllers/app_api_routes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,12 @@
-from flask import Blueprint, request
+from flask import Blueprint
 import logging
-from trexlib.utils.log_util import get_tracelog
 from trexmodel.utils.model.model_util import create_db_client
-from datetime import datetime
-from trexlib.utils.string_util import is_not_empty
-from trexmodel.models.datastore.user_models import User
-from trexadmin.libs.http import create_rest_message
-from trexadmin.libs.http import StatusCode
-from werkzeug.datastructures import ImmutableMultiDict
-from trexapi.forms.user_api_forms import UserRegistrationForm
-from trexapi.conf import APPLICATION_NAME, APPLICATION_BASE_URL
-from trexmail.email_helper import trigger_send_email
-from trexmodel.models.datastore.app_models import AppPromotion, AppMessage
 from trexmodel.models.datastore.admin_models import AppBannerFile
  
-from trexlib.utils.common.common_util import sort_dict_list
 from flask.json import jsonify
 
 app_api_bp = Blueprint('app_api_bp', __name__,
                                  template_folder='templates',
                                  static_folder='static',
                                  url_prefix='/api/v1/app')
 
@@ -188,7 +176,9 @@
         logger.debug('result_listing=%s', result_listing)
     '''
     
         
     return jsonify({
             'messages': result_listing,
             })    
+
+
```

### Comparing `trex-apis-1.3.8/trexapi/controllers/customer_api_routes.py` & `trex-apis-1.4.0/trexapi/controllers/customer_api_routes.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 '''
 Created on 7 Jul 2021
 
 @author: jacklok
 '''
 
-from flask import Blueprint, request, session 
-from flask_restful import abort
+from flask import Blueprint, request 
 import logging
 from trexlib.utils.log_util import get_tracelog
 from flask_restful import Api
 from trexmodel.utils.model.model_util import create_db_client
 from flask.json import jsonify
 from datetime import datetime
 from trexapi.decorators.api_decorators import auth_token_required,\
-    outlet_key_required, test_session_expired, device_is_activated
+    outlet_key_required, device_is_activated
 from trexlib.utils.string_util import is_not_empty
 from trexmodel.models.datastore.customer_models import Customer,\
     CustomerMembership, CustomerTierMembership
 from trexmodel.models.datastore.user_models import User
-from trexadmin.libs.http import create_rest_message
-from trexadmin.libs.http import StatusCode
+from trexapi.utils.api_helpers import StatusCode, create_api_message
 from trexmodel.models.datastore.merchant_models import Outlet,\
     MerchantAcct, MerchantUser
 from trexapi.forms.customer_api_forms import CustomerDetailsNewForm, CustomerDetailsUpdateForm,\
     CustomerSearchForm
 from werkzeug.datastructures import ImmutableMultiDict
 from trexapi.controllers.user_api_routes import user_details_dict
 from trexmodel.models.datastore.transaction_models import CustomerTransaction
 from trexapi.utils.api_helpers import get_logged_in_api_username
 from trexmodel.models.datastore.redeem_models import CustomerRedemption
 from trexmodel.models.datastore.model_decorators import model_transactional
 from trexapi.utils.reward_transaction_helper import revert_redemption,\
     revert_transaction
 from trexanalytics.bigquery_upstream_data_config import create_merchant_registered_customer_upstream_for_merchant,\
     create_registered_customer_upstream_for_system
-from trexmodel.models.datastore.membership_models import MerchantMembership,\
-    MerchantTierMembership
+from trexmodel.models.datastore.membership_models import MerchantMembership
 from flask_babel import gettext
+from trexlib.libs.flask_wtf.request_wrapper import request_json, request_headers
 
 logger = logging.getLogger('api')
 
 
 customer_api_bp = Blueprint('customer_api_base_bp', __name__,
                                  template_folder='templates',
                                  static_folder='static',
@@ -52,16 +50,17 @@
 
 
 
 @customer_api_bp.route('/register', methods=['POST'])
 @auth_token_required
 @outlet_key_required
 @device_is_activated
-def create_customer():
-    customer_data_in_json   = request.get_json()
+@request_json
+@request_headers
+def create_customer(customer_data_in_json, request_headers):
     register_customer_form  = CustomerDetailsNewForm(ImmutableMultiDict(customer_data_in_json))
     
     logger.debug('create_customer: customer_data_in_json=%s', customer_data_in_json)
     
     try:
         if register_customer_form.validate():
             logger.debug('customer registration input is valid')
@@ -69,16 +68,16 @@
             
             is_email_used           = False
             is_mobile_phone_used    = False
             customer_is_exist       = False
             created_customer        = None
             created_user_acct       = None
             
-            outlet_key  = request.headers.get('x-outlet-key')
-            acct_id     = request.headers.get('x-acct-id')
+            outlet_key  = request_headers.get('x-outlet-key')
+            acct_id     = request_headers.get('x-acct-id')
             
             logger.debug('outlet_key=%s', outlet_key)
             logger.debug('acct_id=%s', acct_id)
             
             with db_client.context():
                 merchant_acct   = MerchantAcct.fetch(acct_id)
                 outlet          = Outlet.fetch(outlet_key)
@@ -168,18 +167,18 @@
                     else:
                         logger.warn('Invalid granted outlet key')
                 else:
                     logger.warn('Invalid granted outlet key')
             
                 if customer_is_exist:
                     if is_email_used==True:
-                        return create_rest_message('Email have been taken', status_code=StatusCode.BAD_REQUEST)
+                        return create_api_message('Email have been taken', status_code=StatusCode.BAD_REQUEST)
                     
                     elif is_mobile_phone_used==True:
-                        return create_rest_message('Mobile phone have been taken', status_code=StatusCode.BAD_REQUEST)
+                        return create_api_message('Mobile phone have been taken', status_code=StatusCode.BAD_REQUEST)
                     
                 
                 if created_customer:
                     created_user_acct = created_customer.registered_user_acct
                     response_data = {
                                 'customer_key'              : created_customer.key_in_str,
                                 'registered_datetime'       : created_customer.registered_datetime.strftime("%d-%m-%Y %H:%M:%S"),
@@ -191,41 +190,42 @@
                                 
                                 }
                 
                     logger.debug('response_data=%s', response_data)
                     
                     response_data.update(user_details_dict(created_user_acct))
                     
-                    return create_rest_message(status_code=StatusCode.OK, **response_data)
+                    return create_api_message(status_code=StatusCode.OK, **response_data)
                     
                 else:
-                    return create_rest_message(status_code=StatusCode.BAD_REQUEST)
+                    return create_api_message(status_code=StatusCode.BAD_REQUEST)
             
         else:
             logger.warn('customer registration input is invalid')
             error_message = register_customer_form.create_rest_return_error_message()
             
-            return create_rest_message(error_message, status_code=StatusCode.BAD_REQUEST)
+            return create_api_message(error_message, status_code=StatusCode.BAD_REQUEST)
     except:
         logger.error('Fail to register customer due to %s', get_tracelog())
         
-        return create_rest_message(status_code=StatusCode.BAD_REQUEST)
+        return create_api_message(status_code=StatusCode.BAD_REQUEST)
 
 
 @customer_api_bp.route('/reference-code/<ref_code>', methods=['GET'])
 @auth_token_required
 @device_is_activated
-def read_customer(ref_code):
+@request_headers
+def read_customer(ref_code, request_headers):
     
     logger.debug('ref_code=%s', ref_code)
     
     if is_not_empty(ref_code):
         db_client = create_db_client(caller_info="read_customer")
         
-        acct_id     = request.headers.get('x-acct-id')
+        acct_id     = request_headers.get('x-acct-id')
         
         with db_client.context():
             merchant_acct = MerchantAcct.fetch(acct_id)
             customer = Customer.get_by_reference_code(ref_code, merchant_acct)
             
         
         if customer:
@@ -246,18 +246,18 @@
             
             logger.debug('customer_details_json=%s', customer_details_json)
             
             return customer_details_json
             
         else:
             logger.warn('Customer with reference code (%s) is not found', ref_code)
-            return create_rest_message(status_code=StatusCode.BAD_REQUEST)
+            return create_api_message(status_code=StatusCode.BAD_REQUEST)
             
     else:
-        return create_rest_message(status_code=StatusCode.BAD_REQUEST)
+        return create_api_message(status_code=StatusCode.BAD_REQUEST)
     
 @customer_api_bp.route('/customer-key/<customer_key>', methods=['GET'])
 #@auth_token_required
 #@device_is_activated
 def read_customer_by_customer_key(customer_key):
     
     logger.debug('customer_key=%s', customer_key)
@@ -301,25 +301,25 @@
             
         if customer_details_dict:
             return jsonify(customer_details_dict)
             
             
         else:
             logger.warn('Customer with customer_key (%s) is not found', customer_key)
-            return create_rest_message(status_code=StatusCode.BAD_REQUEST)
+            return create_api_message(status_code=StatusCode.BAD_REQUEST)
             
     else:
-        return create_rest_message(status_code=StatusCode.BAD_REQUEST)    
+        return create_api_message(status_code=StatusCode.BAD_REQUEST)    
 
 
 @customer_api_bp.route('/customer-key/<customer_key>', methods=['PUT'])
 @auth_token_required
 @device_is_activated
-def update_customer(customer_key):
-    customer_data_in_json   = request.get_json()
+@request_json
+def update_customer(customer_data_in_json, customer_key):
     updating_customer_form  = CustomerDetailsUpdateForm(ImmutableMultiDict(customer_data_in_json))
     
     logger.debug('update_customer: customer_data_in_json=%s', customer_data_in_json)
     
     try:
         if updating_customer_form.validate():
             logger.debug('customer update input is valid')
@@ -390,32 +390,32 @@
                                     mobile_phone            = mobile_phone, 
                                     password                = customer_data_in_json.get('password'),
                                     )
                 
                 
                 if customer_is_exist:
                     if is_email_used==True:
-                        return create_rest_message('Email have been taken', status_code=StatusCode.BAD_REQUEST)
+                        return create_api_message('Email have been taken', status_code=StatusCode.BAD_REQUEST)
                     
                     elif is_mobile_phone_used==True:
-                        return create_rest_message('Mobile phone have been taken', status_code=StatusCode.BAD_REQUEST)
+                        return create_api_message('Mobile phone have been taken', status_code=StatusCode.BAD_REQUEST)
                     else:
-                        return create_rest_message(status_code=StatusCode.OK)
+                        return create_api_message(status_code=StatusCode.OK)
                 else:
-                    return create_rest_message(gettext('Customer is not exist'), status_code=StatusCode.BAD_REQUEST)
+                    return create_api_message(gettext('Customer is not exist'), status_code=StatusCode.BAD_REQUEST)
             
         else:
             logger.warn('customer registration input is invalid')
             error_message = updating_customer_form.create_rest_return_error_message()
             
-            return create_rest_message(error_message, status_code=StatusCode.BAD_REQUEST)
+            return create_api_message(error_message, status_code=StatusCode.BAD_REQUEST)
     except:
         logger.error('Fail to register customer due to %s', get_tracelog())
         
-        return create_rest_message(status_code=StatusCode.BAD_REQUEST)
+        return create_api_message(status_code=StatusCode.BAD_REQUEST)
         
 @customer_api_bp.route('/<ref_code>', methods=['DELETE'])
 @auth_token_required 
 @device_is_activated
 def delete_customer(ref_code):
     if is_not_empty(ref_code):
         is_found = False
@@ -423,26 +423,27 @@
         with db_client.context():
             customer = Customer.get_by_reference_code(ref_code) 
             if customer:
                 customer.delete()
                 is_found = True
         
         if is_found:
-            return create_rest_message(status_code=StatusCode.NO_CONTENT)
+            return create_api_message(status_code=StatusCode.NO_CONTENT)
         else:
-            return create_rest_message(gettext('Customer is not exist'), status_code=StatusCode.BAD_REQUEST)
+            return create_api_message(gettext('Customer is not exist'), status_code=StatusCode.BAD_REQUEST)
     else:
-        return create_rest_message(status_code=StatusCode.BAD_REQUEST)        
+        return create_api_message(status_code=StatusCode.BAD_REQUEST)        
 
 
 @customer_api_bp.route('/register-as-customer', methods=['POST'])
 @auth_token_required
 @device_is_activated
-def register_user_as_customer():
-    user_data_in_json           = request.get_json()
+@request_json
+@request_headers
+def register_user_as_customer(user_data_in_json, request_headers):
     reference_code              = user_data_in_json.get('reference_code')
     
     logger.debug('register_user_as_customer: user_data_in_json=%s', user_data_in_json)
     
     try:
         if is_not_empty(reference_code):
             logger.debug('customer registration input is valid')
@@ -452,16 +453,16 @@
             existing_user_acct      = None
             is_email_used           = False
             is_mobile_phone_used    = False
             merchant_act_key        = None
             
             merchant_acct           = None
             
-            outlet_key  = request.headers.get('x-outlet-key')
-            acct_id     = request.headers.get('x-acct-id')
+            outlet_key  = request_headers.get('x-outlet-key')
+            acct_id     = request_headers.get('x-acct-id')
             
             logger.debug('register_user_as_customer: outlet_key=%s', outlet_key)
             logger.debug('register_user_as_customer: acct_id=%s', acct_id)
             logger.debug('register_user_as_customer: reference_code=%s', reference_code)
             
             with db_client.context():
                 existing_user_acct  = User.get_by_reference_code(reference_code)
@@ -530,57 +531,59 @@
                                     #'user_details'              : user_details_dict(existing_user_acct),
                                     }
                     
                     response_data.update(user_details_dict(existing_user_acct))
                     
                     logger.debug('register_user_as_customer debug: response_data=%s', response_data)
                     
-                    return create_rest_message(status_code=StatusCode.OK, **response_data)
+                    return create_api_message(status_code=StatusCode.OK, **response_data)
                     
                 else:
                     if is_email_used==True:
-                        return create_rest_message('Email have been taken', status_code=StatusCode.BAD_REQUEST)
+                        return create_api_message('Email have been taken', status_code=StatusCode.BAD_REQUEST)
                     
                     elif is_mobile_phone_used==True:
-                        return create_rest_message('Mobile phone have been taken', status_code=StatusCode.BAD_REQUEST)
+                        return create_api_message('Mobile phone have been taken', status_code=StatusCode.BAD_REQUEST)
                     else:
-                        return create_rest_message('Failed to register customer', status_code=StatusCode.BAD_REQUEST)
+                        return create_api_message('Failed to register customer', status_code=StatusCode.BAD_REQUEST)
             
         else:
             logger.warn('customer registration input is invalid')
             
-            return create_rest_message("Missing register customer input data", status_code=StatusCode.BAD_REQUEST)
+            return create_api_message("Missing register customer input data", status_code=StatusCode.BAD_REQUEST)
     except:
         logger.error('Fail to register customer due to %s', get_tracelog())
         
-        return create_rest_message(status_code=StatusCode.BAD_REQUEST)
+        return create_api_message(status_code=StatusCode.BAD_REQUEST)
 
 @customer_api_bp.route('/search/<limit>', methods=['POST'])
 @auth_token_required
 @device_is_activated
+@request_json
+@request_headers
 #@test_session_expired
-def search_customer(limit):
+def search_customer(search_member_data_in_json, request_headers, limit):
     
-    search_member_data_in_json   = request.get_json()
+    #search_member_data_in_json   = request.get_json()
     search_customer_form         = CustomerSearchForm(ImmutableMultiDict(search_member_data_in_json))
     
     logger.debug('search_member_data_in_json=%s', search_member_data_in_json)
     
     db_client = create_db_client(caller_info="search_customer")
     customer_list = []
     
     if search_customer_form.validate():
         name                        = search_customer_form.name.data
         mobile_phone                = search_customer_form.mobile_phone.data
         email                       = search_customer_form.email.data
         reference_code              = search_customer_form.reference_code.data
         merchant_reference_code     = search_customer_form.merchant_reference_code.data
-        customer_data               = search_customer_form.customer_data.data
+        #customer_data               = search_customer_form.customer_data.data
     
-        acct_id     = request.headers.get('x-acct-id')
+        acct_id     = request_headers.get('x-acct-id')
         
         logger.debug('acct_id=%s', acct_id)
         logger.debug('name=%s', name)
         logger.debug('email=%s', email)
         logger.debug('mobile_phone=%s', mobile_phone)
         logger.debug('reference_code=%s', reference_code)
         logger.debug('merchant_reference_code=%s', merchant_reference_code)
@@ -593,15 +596,18 @@
                                                                                             name                    = name, 
                                                                                             email                   = email, 
                                                                                             mobile_phone            = mobile_phone, 
                                                                                             reference_code          = reference_code,
                                                                                             merchant_reference_code = merchant_reference_code,
                                                                                             limit                   = limit_int,
                                                                                             )
-        
+            
+            logger.debug('total_count=%s', total_count)
+            logger.debug('next_cursor=%s', next_cursor)
+            
             for c in search_results:
                 user_details = c.registered_user_acct
                 customer_details_dict = c.to_dict(
                                             date_format="%d-%m-%Y", 
                                             datetime_format="%d-%m-%Y %H:%M:%S",
                                             excluded_dict_properties=['registered_merchant_acct'],
                                             )
@@ -625,26 +631,26 @@
                 
                 tier_membership_data = _get_tier_membership(c)
                 if tier_membership_data:
                     customer_details_dict['tier_membership'] = tier_membership_data
                 
                 customer_list.append(customer_details_dict)
     
-        #return create_rest_message(status_code=customer_list.OK, customer_list=customer_list)
+        #return create_api_message(status_code=customer_list.OK, customer_list=customer_list)
         customer_details_list_json =  jsonify(customer_list)
             
             
         logger.debug('customer_details_list_json=%s', customer_details_list_json)
             
         return customer_details_list_json
     else:
         error_message = search_customer_form.create_rest_return_error_message()
-        return create_rest_message(error_message, status_code=StatusCode.BAD_REQUEST)
-        #return create_rest_message(gettext('Invalid input'), status_code=StatusCode.BAD_REQUEST)
-        #return create_rest_message('Invalid input', status_code=StatusCode.BAD_REQUEST)
+        return create_api_message(error_message, status_code=StatusCode.BAD_REQUEST)
+        #return create_api_message(gettext('Invalid input'), status_code=StatusCode.BAD_REQUEST)
+        #return create_api_message('Invalid input', status_code=StatusCode.BAD_REQUEST)
 
 
 def _list_customer_basic_memberships(customer):
     customer_membership_final_list = []
     
     if is_not_empty(customer.memberships_list):
         customer_memberships_list = CustomerMembership.list_all_by_customer(customer)
@@ -687,18 +693,19 @@
         
         return membership_data
         
     
 
 @customer_api_bp.route('/reference-code/<reference_code>/list-membership', methods=['GET'])
 @auth_token_required
+@request_headers
 #@test_session_expired
-def list_customer_membership(reference_code):
+def list_customer_membership(request_headers, reference_code):
     if is_not_empty(reference_code):
-        acct_id   = request.headers.get('x-acct-id')
+        acct_id   = request_headers.get('x-acct-id')
         db_client = create_db_client(caller_info="list_customer_membership")
         customer_membershis_list = []
         
         logger.debug('reference_code=%s', reference_code)
         
         with db_client.context():
             merchant_acct   = MerchantAcct.fetch(acct_id)
@@ -707,28 +714,29 @@
             customer_membershis_list = _list_customer_basic_memberships(customer)
             tier_membership_data = _get_tier_membership(customer)
             if tier_membership_data:
                 customer_membershis_list.append(tier_membership_data)
     
         return jsonify(customer_membershis_list)
     else:
-        return create_rest_message(status_code=StatusCode.BAD_REQUEST)    
+        return create_api_message(status_code=StatusCode.BAD_REQUEST)    
                 
 
 
 @customer_api_bp.route('/reference-code/<reference_code>/transaction/limit/<limit>', methods=['GET'])
 @auth_token_required
+@request_headers
 #@test_session_expired
-def list_customer_transaction(reference_code, limit):
+def list_customer_transaction(request_headers, reference_code, limit):
     
     logger.debug('reference_code=%s', reference_code)
     
     if is_not_empty(reference_code):
         limit_int = int(limit, 10)
-        acct_id   = request.headers.get('x-acct-id')
+        acct_id   = request_headers.get('x-acct-id')
         db_client = create_db_client(caller_info="read_customer_sales_transaction")
         transactions_list = []
         with db_client.context():
             merchant_acct = MerchantAcct.fetch(acct_id)
             customer = Customer.get_by_reference_code(reference_code, merchant_acct)
             
         
@@ -745,64 +753,65 @@
                 for r in result:
                     transactions_list.append(r.to_dict(dict_properties=dict_properties,  date_format="%d-%m-%Y", datetime_format="%d-%m-%Y %H:%M:%S"))
             
             return jsonify(transactions_list)
             
         else:
             logger.warn('Customer transaction with reference code (%s) is not found', reference_code)
-            return create_rest_message(status_code=StatusCode.BAD_REQUEST)
+            return create_api_message(status_code=StatusCode.BAD_REQUEST)
             
     else:
-        return create_rest_message(status_code=StatusCode.BAD_REQUEST)
+        return create_api_message(status_code=StatusCode.BAD_REQUEST)
     
 @customer_api_bp.route('/reference-code/<reference_code>/transaction/transaction_id/<transaction_id>/revert', methods=['POST'])
 @auth_token_required
 def revert_customer_transaction(reference_code, transaction_id):
     
     logger.debug('transaction_id=%s', transaction_id)
     
     if is_not_empty(reference_code) and is_not_empty(transaction_id):
-        acct_id   = request.headers.get('x-acct-id')
+        #acct_id   = request_headers.get('x-acct-id')
         db_client = create_db_client(caller_info="revert_customer_sales_transaction")
         
         with db_client.context():
             customer_transactionn       = CustomerTransaction.get_by_transaction_id(transaction_id);
         
         if customer_transactionn:
             with db_client.context():
                 merchant_username       = get_logged_in_api_username()
                 reverted_by             = MerchantUser.get_by_username(merchant_username)
                 
                 reverted_datetime_utc   = datetime.utcnow()
                 __revert_customer_transaction(customer_transactionn, reverted_by, reverted_datetime=reverted_datetime_utc)
             
-            return create_rest_message(status_code=StatusCode.OK, reverted_datetime = customer_transactionn.reverted_datetime.strftime('%d-%m-%Y %H:%M:%S'))
+            return create_api_message(status_code=StatusCode.OK, reverted_datetime = customer_transactionn.reverted_datetime.strftime('%d-%m-%Y %H:%M:%S'))
         else:    
-            return create_rest_message(gettext('Failed to find transaction'), status_code=StatusCode.BAD_REQUEST)
+            return create_api_message(gettext('Failed to find transaction'), status_code=StatusCode.BAD_REQUEST)
         
         
             
     else:
-        return create_rest_message(gettext('Missing reference code or transaction id'), status_code=StatusCode.BAD_REQUEST)    
+        return create_api_message(gettext('Missing reference code or transaction id'), status_code=StatusCode.BAD_REQUEST)    
 
 @model_transactional(desc="revert_customer_transaction")
 def __revert_customer_transaction(customer_transction, reverted_by, reverted_datetime):     
     return revert_transaction(customer_transction, reverted_by, reverted_datetime=reverted_datetime)
 
     
 @customer_api_bp.route('/reference-code/<reference_code>/redemption/limit/<limit>', methods=['GET'])
 @auth_token_required
+@request_headers
 #@test_session_expired
-def list_customer_redemption(reference_code, limit):
+def list_customer_redemption(request_headers, reference_code, limit):
     
     logger.debug('reference_code=%s', reference_code)
     
     if is_not_empty(reference_code):
         limit_int = int(limit, 10)
-        acct_id   = request.headers.get('x-acct-id')
+        acct_id   = request_headers.get('x-acct-id')
         db_client = create_db_client(caller_info="read_customer_sales_transaction")
         redemptions_list = []
         with db_client.context():
             merchant_acct = MerchantAcct.fetch(acct_id)
             customer = Customer.get_by_reference_code(reference_code, merchant_acct)
             
         
@@ -816,47 +825,50 @@
                 for r in result:
                     redemptions_list.append(r.to_dict(dict_properties=dict_properties,  date_format="%d-%m-%Y", datetime_format="%d-%m-%Y %H:%M:%S"))
             
             return jsonify(redemptions_list)
             
         else:
             logger.warn('Customer transaction with reference code (%s) is not found', reference_code)
-            return create_rest_message(status_code=StatusCode.BAD_REQUEST)
+            return create_api_message(status_code=StatusCode.BAD_REQUEST)
             
     else:
-        return create_rest_message(status_code=StatusCode.BAD_REQUEST)    
+        return create_api_message(status_code=StatusCode.BAD_REQUEST)    
     
 @customer_api_bp.route('/reference-code/<reference_code>/redemption/transaction_id/<transaction_id>/revert', methods=['POST'])
 @auth_token_required
-def revert_customer_redemption(reference_code, transaction_id):
+@request_headers
+def revert_customer_redemption(request_headers, reference_code, transaction_id):
     
     logger.debug('transaction_id=%s', transaction_id)
     
     if is_not_empty(reference_code) and is_not_empty(transaction_id):
-        acct_id   = request.headers.get('x-acct-id')
+        #acct_id   = request_headers.get('x-acct-id')
         db_client = create_db_client(caller_info="revert_customer_sales_transaction")
         
         with db_client.context():
             customer_redemption    = CustomerRedemption.get_by_transaction_id(transaction_id);
         
         if customer_redemption:
             with db_client.context():
                 merchant_username       = get_logged_in_api_username()
                 reverted_by             = MerchantUser.get_by_username(merchant_username)
                 
                 reverted_datetime_utc   = datetime.utcnow()
                 __revert_customer_redemption(customer_redemption, reverted_by, reverted_datetime=reverted_datetime_utc)
             
-            return create_rest_message(status_code=StatusCode.OK, reverted_datetime = customer_redemption.reverted_datetime.strftime('%d-%m-%Y %H:%M:%S'))
+            return create_api_message(status_code=StatusCode.OK, reverted_datetime = customer_redemption.reverted_datetime.strftime('%d-%m-%Y %H:%M:%S'))
         else:    
-            return create_rest_message(gettext('Failed to find transaction'), status_code=StatusCode.BAD_REQUEST)
+            return create_api_message(gettext('Failed to find transaction'), status_code=StatusCode.BAD_REQUEST)
         
         
             
     else:
-        return create_rest_message(gettext('Missing reference code or transaction id'), status_code=StatusCode.BAD_REQUEST)
+        return create_api_message(gettext('Missing reference code or transaction id'), status_code=StatusCode.BAD_REQUEST)
     
 @model_transactional(desc="revert_customer_redemption")
 def __revert_customer_redemption(customer_redemption, reverted_by, reverted_datetime=None):     
        
     return revert_redemption(customer_redemption, reverted_by, reverted_datetime=reverted_datetime)
+
+
```

### Comparing `trex-apis-1.3.8/trexapi/controllers/customer_membership_api_routes.py` & `trex-apis-1.4.0/trexapi/controllers/customer_membership_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.8/trexapi/controllers/customer_reward_api_routes.py` & `trex-apis-1.4.0/trexapi/controllers/customer_reward_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.8/trexapi/controllers/loyalty_api_routes.py` & `trex-apis-1.4.0/trexapi/controllers/loyalty_api_routes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 '''
 Created on 28 Oct 2021
 
 @author: jacklok
 '''
 
-from flask import Blueprint, request, url_for, jsonify
-import logging, json
-from trexapi.decorators.api_decorators import auth_token_required,\
-    device_activated_is_required
-from trexlib.utils.string_util import is_not_empty, is_empty
-from trexadmin.libs.http import create_rest_message
-from trexadmin.libs.http import StatusCode
+from flask import Blueprint, request, url_for
+import logging
+from trexapi.decorators.api_decorators import device_activated_is_required
+from trexlib.utils.string_util import is_not_empty
+from trexapi.utils.api_helpers import StatusCode, create_api_message
 from trexmodel.models.datastore.loyalty_models import LoyaltyDeviceSetting
 from trexmodel.utils.model.model_util import create_db_client
 from trexmodel.models import merchant_helpers
-from trexlib.utils.common.common_util import sort_list
-from firebase_admin import firestore
-from datetime import datetime
 from trexapi.conf import API_ERR_CODE_INVALID_ACTIVATION_CODE
-from trexadmin import conf
+from trexconf import conf
 
 
 logger = logging.getLogger('api')
 #logger = logging.getLogger('debug')
 
 loyalty_api_bp = Blueprint('loyalty_api_bp', __name__,
                                  template_folder='templates',
@@ -38,21 +33,21 @@
     if is_not_empty(activation_code):
         db_client = create_db_client(caller_info="check_activation")
         with db_client.context():
             device_setting = LoyaltyDeviceSetting.get_by_activation_code(activation_code)
         
         if device_setting:
             if device_setting.activated==False:
-                return create_rest_message(status_code=StatusCode.OK)
+                return create_api_message(status_code=StatusCode.OK)
             else:
-                return create_rest_message('The code have been used to activate before', status_code=StatusCode.BAD_REQUEST)
+                return create_api_message('The code have been used to activate before', status_code=StatusCode.BAD_REQUEST)
         else:
-            return create_rest_message('Invalid activate code', status_code=StatusCode.BAD_REQUEST)
+            return create_api_message('Invalid activate code', status_code=StatusCode.BAD_REQUEST)
     else:
-        return create_rest_message('Activation code is required', status_code=StatusCode.BAD_REQUEST)
+        return create_api_message('Activation code is required', status_code=StatusCode.BAD_REQUEST)
 
 def get_device_setting(activation_code, device_id=None):
     if is_not_empty(activation_code):
         db_client = create_db_client(caller_info="get_device_setting")
         with db_client.context():
             device_setting = LoyaltyDeviceSetting.get_by_activation_code(activation_code)
         
@@ -66,40 +61,40 @@
                     if device_setting.is_test_setting==False:
                         device_setting.activate(device_id)
                     
                     device_setting_details                              = merchant_helpers.construct_setting_by_outlet(device_setting.assigned_outlet_entity, device_setting=device_setting) 
                     
                     device_setting_details['logo_image_url']            = url_for('system_bp.merchant_logo_image_url', merchant_act_key=device_setting_details.get('account_id'))
                 
-                return create_rest_message(status_code=StatusCode.OK,
+                return create_api_message(status_code=StatusCode.OK,
                                                **device_setting_details
                                                )
             else:
                 if device_id == device_setting.device_id: 
                     with db_client.context():
                         device_setting_details                              = merchant_helpers.construct_setting_by_outlet(device_setting.assigned_outlet_entity, device_setting=device_setting) 
                         
                         device_setting_details['logo_image_url']            = url_for('system_bp.merchant_logo_image_url', merchant_act_key=device_setting_details.get('account_id'))
                     
-                    return create_rest_message(status_code=StatusCode.OK,
+                    return create_api_message(status_code=StatusCode.OK,
                                                **device_setting_details
                                                )
                 else:
-                    return create_rest_message('The code have been used in other device', status_code=StatusCode.BAD_REQUEST)
+                    return create_api_message('The code have been used in other device', status_code=StatusCode.BAD_REQUEST)
             '''
             else:
                 logger.info('Device activation code have been used');
-                return create_rest_message('The code have been used to activate before', status_code=StatusCode.BAD_REQUEST)
+                return create_api_message('The code have been used to activate before', status_code=StatusCode.BAD_REQUEST)
             '''
         else:
             logger.info('Device setting record is not found');
-            return create_rest_message('Invalid activate code', status_code=StatusCode.BAD_REQUEST, error_code=API_ERR_CODE_INVALID_ACTIVATION_CODE)
+            return create_api_message('Invalid activate code', status_code=StatusCode.BAD_REQUEST, error_code=API_ERR_CODE_INVALID_ACTIVATION_CODE)
     else:
         logger.info('activation_code is empty');
-        return create_rest_message('Activation code is required', status_code=StatusCode.BAD_REQUEST)
+        return create_api_message('Activation code is required', status_code=StatusCode.BAD_REQUEST)
     
     
 def reset_deviceSetting(activation_code, device_id):
     if is_not_empty(activation_code):
         db_client = create_db_client(caller_info="reset_deviceSetting")
         with db_client.context():
             device_setting = LoyaltyDeviceSetting.get_by_activation_code(activation_code)
@@ -111,25 +106,25 @@
             if device_setting.activated==True:
             
                 if device_id == device_setting.device_id: 
                     
                     with db_client.context():
                         device_setting.reset()
                     
-                    return create_rest_message(status_code=StatusCode.OK,
+                    return create_api_message(status_code=StatusCode.OK,
                                                )
                 else:
-                    return create_rest_message('The code have been used in other device', status_code=StatusCode.BAD_REQUEST)
+                    return create_api_message('The code have been used in other device', status_code=StatusCode.BAD_REQUEST)
             
         else:
             logger.info('Device setting record is not found, thus the activation code should be invalid');
-            return create_rest_message('Invalid activate code', status_code=StatusCode.BAD_REQUEST, error_code=API_ERR_CODE_INVALID_ACTIVATION_CODE)
+            return create_api_message('Invalid activate code', status_code=StatusCode.BAD_REQUEST, error_code=API_ERR_CODE_INVALID_ACTIVATION_CODE)
     else:
         logger.info('activation_code is empty');
-        return create_rest_message('Activation code is required', status_code=StatusCode.BAD_REQUEST)    
+        return create_api_message('Activation code is required', status_code=StatusCode.BAD_REQUEST)    
     
     
 def updateActivationAndGetDeviceSetting(activation_code, device_id):
     if is_not_empty(activation_code) and is_not_empty(device_id):
         db_client = create_db_client(caller_info="updateActivationAndGetDeviceSetting")
         with db_client.context():
             device_setting = LoyaltyDeviceSetting.get_by_activation_code(activation_code)
@@ -161,29 +156,29 @@
                     device_setting_details  = merchant_helpers.construct_setting_by_outlet(device_setting.assigned_outlet_entity, device_setting=device_setting)
                     #pos_setting_details['logo_image_url']               = url_for('system_bp.merchant_logo_image_url', merchant_act_key=pos_setting_details.get('account_id'))
                 
             if is_valid:
                 
                 logger.debug('device_setting_details=%s', device_setting_details);
                 
-                return create_rest_message(status_code=StatusCode.OK,
+                return create_api_message(status_code=StatusCode.OK,
                                            **device_setting_details
                                            )
             else:
                 if device_setting.activated and device_setting.device_id != device_id:
-                    return create_rest_message('The code have been used in other device', status_code=StatusCode.BAD_REQUEST)
+                    return create_api_message('The code have been used in other device', status_code=StatusCode.BAD_REQUEST)
                 else:
-                    return create_rest_message('Failed to activate', status_code=StatusCode.BAD_REQUEST)
+                    return create_api_message('Failed to activate', status_code=StatusCode.BAD_REQUEST)
             
         else:
             logger.info('Setting record is not found');
-            return create_rest_message('Invalid activate code', status_code=StatusCode.BAD_REQUEST)
+            return create_api_message('Invalid activate code', status_code=StatusCode.BAD_REQUEST)
     else:
         logger.info('activation_code is empty or device id is empty');
-        return create_rest_message('Activation code and device id are required', status_code=StatusCode.BAD_REQUEST)
+        return create_api_message('Activation code and device id are required', status_code=StatusCode.BAD_REQUEST)
 
 @loyalty_api_bp.route('/read-settings/activation-code/<activation_code>', methods=['POST'])
 def read_device_setting(activation_code):
     
     logger.info('activation_code=%s', activation_code)
     device_id       = request.args.get('device_id') or request.form.get('device_id') or request.json.get('device_id')
     
@@ -201,26 +196,26 @@
                 with db_client.context():
                     device_setting_details                              = merchant_helpers.construct_setting_by_outlet(device_setting.assigned_outlet_entity, device_setting=device_setting) 
                     device_setting_details['logo_image_url']            = url_for('system_bp.merchant_logo_image_url', merchant_act_key=device_setting_details.get('account_id'))
                     device_setting_details['device_id']                 = device_id
                     
                 logger.debug('device_setting_details=%s', device_setting_details)
                 
-                return create_rest_message(status_code=StatusCode.OK,
+                return create_api_message(status_code=StatusCode.OK,
                                                **device_setting_details
                                                )
             else:
-                return create_rest_message('The code have been used in other device', status_code=StatusCode.BAD_REQUEST)
+                return create_api_message('The code have been used in other device', status_code=StatusCode.BAD_REQUEST)
             
         else:
             logger.info('Device setting record is not found');
-            return create_rest_message('Invalid activate code', status_code=StatusCode.BAD_REQUEST, error_code=API_ERR_CODE_INVALID_ACTIVATION_CODE)
+            return create_api_message('Invalid activate code', status_code=StatusCode.BAD_REQUEST, error_code=API_ERR_CODE_INVALID_ACTIVATION_CODE)
     else:
         logger.info('activation_code is empty');
-        return create_rest_message('Activation code is required', status_code=StatusCode.BAD_REQUEST)
+        return create_api_message('Activation code is required', status_code=StatusCode.BAD_REQUEST)
         
     
 @loyalty_api_bp.route('/account-sync', methods=['GET'])
 def account_sync():
     activation_code = request.args.get('activation_code') or request.form.get('activation_code') or request.json.get('activation_code')
     
     logger.info('activation_code=%s', activation_code)
@@ -271,17 +266,17 @@
         
         with db_client.context():
             device_setting = LoyaltyDeviceSetting.get_by_activation_code(activation_code)
             
             device_setting.update_device_details(platform, device_token)
             
         
-        return create_rest_message(status_code=StatusCode.ACCEPTED)
+        return create_api_message(status_code=StatusCode.ACCEPTED)
     else:
-        return create_rest_message('Missing required data', status_code=StatusCode.BAD_REQUEST)       
+        return create_api_message('Missing required data', status_code=StatusCode.BAD_REQUEST)       
     
 @loyalty_api_bp.route('/version-sync', methods=['get'])
 def version_sync():
     db_client       = create_db_client(caller_info="version_sync")
     
     with db_client.context():
         version =  {
```

### Comparing `trex-apis-1.3.8/trexapi/controllers/lucky_draw_api_routes.py` & `trex-apis-1.4.0/trexapi/controllers/lucky_draw_api_routes.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,23 +4,22 @@
 from flask import request
 from flask.blueprints import Blueprint
 from trexmodel.models.datastore.lucky_draw_models import LuckyDrawTicket
 from trexmodel.utils.model.model_util import create_db_client
 from flask.json import jsonify
 from trexlib.utils.log_util import get_tracelog
 from trexmodel.models.datastore.merchant_models import MerchantAcct
-from trexapi.decorators.api_decorators import auth_token_required,\
-    merchant_key_required, user_auth_token_required
+from trexapi.decorators.api_decorators import auth_token_required, user_auth_token_required
 from trexlib.utils.string_util import is_not_empty
 from trexmodel.models.datastore.customer_models import Customer
 from trexmodel.models.datastore.model_decorators import model_transactional
 from trexmodel.models.datastore.transaction_models import CustomerTransaction
 from datetime import datetime
 from trexmodel import program_conf
-from trexadmin.libs.app.reward_program.lucky_draw_program import LuckyDrawRewardProgram
+from trexprogram.reward_program.lucky_draw_program import LuckyDrawRewardProgram
 from trexapi.utils.api_helpers import create_api_message, StatusCode
 
 lucky_draw_api_bp = Blueprint('lucky_draw_api_bp', __name__,
                                  template_folder='templates',
                                  static_folder='static',
                                  url_prefix='/api/v1/lucky-draw')
```

### Comparing `trex-apis-1.3.8/trexapi/controllers/merchant_api_routes.py` & `trex-apis-1.4.0/trexapi/controllers/merchant_api_routes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 '''
 Created on 30 Jun 2021
 
 @author: jacklok
 '''
 
-from flask import Blueprint, request, Response, session 
+from flask import Blueprint, request
+import flask 
 from flask_restful import Resource, abort
 import logging
 from trexlib.utils.log_util import get_tracelog
 from flask_httpauth import HTTPBasicAuth
-from trexapi import conf
+from trexconf import conf
 from flask_restful import Api
 from trexmodel.utils.model.model_util import create_db_client
 from trexmodel.models.datastore.merchant_models import MerchantUser,\
     MerchantAcct, Outlet
 import hashlib
-from random import random
 from trexlib.utils.string_util import is_not_empty
 from flask.json import jsonify
 from trexapi import conf as api_conf
 from trexapi.decorators.api_decorators import auth_token_required
 from trexmodel.models.datastore.loyalty_models import LoyaltyDeviceSetting
 from trexmodel.models.datastore.pos_models import POSSetting
 from trexapi.controllers.api_routes import APIBaseResource
 from trexmodel.models import merchant_helpers
-from trexadmin.libs.http import create_rest_message, StatusCode
 from trexmodel.models.datastore.customer_models import Customer,\
     CustomerMembership, CustomerTierMembership
 from trexmodel.models.datastore.rating_models import MerchantRatingResult
 from trexmodel.models.datastore.membership_models import MerchantMembership
+from trexapi.utils.api_helpers import StatusCode, create_api_message
+from trexapi.libs.api_decorator import elapsed_time_trace
+from trexmodel.models.datastore.user_models import User
 
 #logger = logging.getLogger('api')
 logger = logging.getLogger('debug')
 
 auth = HTTPBasicAuth()
 #auth = HTTPBasicAuthWrapper()
 
@@ -88,71 +90,194 @@
     if is_not_empty(merchant_acct_code):
         db_client = create_db_client(caller_info="read_merchant_acct")
         with db_client.context():
             merchant_acct   = MerchantAcct.get_by_account_code(merchant_acct_code)
             
             logger.debug('website=%s', merchant_acct.website)
             merchant_info = merchant_helpers.construct_merchant_acct_info(merchant_acct) 
+            
             merchant_rating_result  = MerchantRatingResult.get_by_merchant_acct(merchant_acct)
             
             
             
             if merchant_rating_result:
                 logger.debug('rating_result=%s', merchant_rating_result.rating_result)
                 merchant_info['rating_reviews'] = merchant_rating_result.rating_result
             
                 
         logger.debug('merchant_info=%s', merchant_info)
             
-        return create_rest_message(status_code=StatusCode.OK,
+        return create_api_message(status_code=StatusCode.OK,
                                                **merchant_info
                                                )
     else:
-        return create_rest_message("Missing merchant account key", status_code=StatusCode.BAD_REQUEST)
+        return create_api_message("Missing merchant account key", status_code=StatusCode.BAD_REQUEST)
+    
+@merchant_api_bp.route('/<merchant_acct_code>/referred-code/<referrer_code>/read-details', methods=['GET'])
+def read_customer_brief_and_merchant_acct_and_referred_code(merchant_acct_code, referrer_code):
+    
+    reference_code = request.args.get('reference_code') or request.form.get('reference_code')
+    
+    logger.debug('merchant_acct_code=%s', merchant_acct_code)
+    logger.debug('referrer_code=%s', referrer_code)
+    logger.debug('reference_code=%s', reference_code)
+    
+    db_client = create_db_client(caller_info="read_customer_brief_and_merchant_acct_from_referred_code")
+    customer_acct = None
+    
+    with db_client.context():
+        merchant_acct   = MerchantAcct.get_by_account_code(merchant_acct_code)
+        
+    if is_not_empty(reference_code):
+        with db_client.context():
+            customer_acct   = Customer.get_by_reference_code(reference_code, merchant_acct)
+            
+    
+    if is_not_empty(merchant_acct_code):
+        
+        with db_client.context():
+            merchant_info   = merchant_helpers.construct_merchant_acct_info(merchant_acct) 
+            referrer_user   = User.get_by_referral_code(referrer_code)
+            
+            if merchant_info and referrer_user:
+                
+                if merchant_info.get('referral_program_settings'):
+                    
+                    refer_a_friend_url      = '{base_url}/referral/program/merchant-code/{merchant_code}/referrer-code/{referrer_code}/join'
+                    refer_a_friend_message  = 'Hi, \n\n{referee_promote_desc}. Please join {brand_name} via below link:\n\n{refer_a_friend_url}'
+                    referee_promote_desc    = merchant_info.get('referral_program_settings').get('referee_promote_desc')
+                        
+                    refer_a_friend_url = refer_a_friend_url.format(
+                                                base_url        = conf.REFER_BASE_URL,
+                                                merchant_code   = merchant_acct.account_code,
+                                                referrer_code   = referrer_code,
+                                                )
+                    
+                    refer_a_friend_deep_link = conf.REFER_A_FRIEND_DEEP_LINK.format(
+                                                merchant_acct_code  = merchant_acct.account_code,
+                                                referrer_code       = referrer_code,
+                                                )
+                    
+                    
+                    refer_a_friend_message = refer_a_friend_message.format(
+                                                referee_promote_desc    = referee_promote_desc,
+                                                brand_name              = merchant_acct.brand_name,
+                                                refer_a_friend_url      = refer_a_friend_url,
+                                                )
+                    
+                    merchant_info['referral_program_settings']['refer_a_friend_url']        = refer_a_friend_url
+                    merchant_info['referral_program_settings']['refer_a_friend_message']    = refer_a_friend_message
+                    merchant_info['referral_program_settings']['refer_a_friend_deep_link']  = refer_a_friend_deep_link
+                    
+                merchant_rating_result  = MerchantRatingResult.get_by_merchant_acct(merchant_acct)
+                
+                
+                
+                if merchant_rating_result:
+                    logger.debug('rating_result=%s', merchant_rating_result.rating_result)
+                    merchant_info['rating_reviews'] = merchant_rating_result.rating_result
+        
+        if referrer_user is None or merchant_info is None:  
+            
+            return create_api_message(status_code=StatusCode.BAD_REQUEST)
+        else:   
+                
+            logger.debug('merchant_info=%s', merchant_info)
+            
+            data = {
+                        'merchant_info' : merchant_info,
+                        'referrer_name' : referrer_user.name,
+                        }
+            
+            if customer_acct is not None:
+                data['customer_brief'] = {
+                                        'name'              : customer_acct.name,
+                                        'reference_code'    : reference_code,
+                                        }
+                
+            return create_api_message(status_code=StatusCode.OK,
+                                                   **data
+                                                   )
+    else:
+        return create_api_message("Missing merchant account key", status_code=StatusCode.BAD_REQUEST)    
     
 @merchant_api_bp.route('/<merchant_acct_code>/joined-brand-details/reference-code/<reference_code>', methods=['GET'])
+@elapsed_time_trace(trace_key='read_joined_brand_details')
 def read_joined_brand_details(merchant_acct_code, reference_code):
     
     merchant_acct           = None
     
     if is_not_empty(merchant_acct_code) and is_not_empty(reference_code):    
         db_client = create_db_client(caller_info="read_merchant_acct")
         with db_client.context():
             merchant_acct           = MerchantAcct.get_by_account_code(merchant_acct_code)
-            customer                = Customer.get_by_reference_code(reference_code, merchant_acct)
             
-            merchant_info           = merchant_helpers.construct_merchant_acct_info(merchant_acct) 
-            merchant_rating_result  = MerchantRatingResult.get_by_merchant_acct(merchant_acct)
-            
-            if merchant_rating_result:
-                logger.debug('rating_result=%s', merchant_rating_result.rating_result)
-                merchant_info['rating_reviews'] = merchant_rating_result.rating_result
-            
-            user_details                                        = customer.registered_user_acct
-            customer_details = customer.to_dict(date_format="%d-%m-%Y", datetime_format="%d-%m-%Y %H:%M:%S")
-            customer_details['customer_key']               = customer.key_in_str
-            customer_details['is_email_verified']          = user_details.is_email_verified
-            customer_details['is_mobile_phone_verified']   = user_details.is_mobile_phone_verified
-            
-            customer_basic_memberships_list = _list_customer_basic_memberships(customer)
-            if customer_basic_memberships_list:
-                customer_details['basic_memberships'] = customer_basic_memberships_list
-            
-            tier_membership_data = _get_tier_membership(customer)
-            if tier_membership_data:
-                customer_details['tier_membership'] = tier_membership_data
+            customer                = Customer.get_by_reference_code(reference_code, merchant_acct)
+            if customer:
+                user_acct               = customer.registered_user_acct
+                merchant_info           = merchant_helpers.construct_merchant_acct_info(merchant_acct) 
+                merchant_rating_result  = MerchantRatingResult.get_by_merchant_acct(merchant_acct)
+                
+                if merchant_info.get('referral_program_settings'):
+                    
+                    refer_a_friend_url      = '{base_url}/referral/program/merchant-acct-code/{merchant_acct_code}/referrer-code/{referrer_code}/join'
+                    refer_a_friend_message  = 'Hi, \n\n{referee_promote_desc}. Please join {brand_name} via below link:\n\n{refer_a_friend_url}'
+                    referee_promote_desc    = merchant_info.get('referral_program_settings').get('referee_promote_desc')
+                        
+                    refer_a_friend_url = refer_a_friend_url.format(
+                                                base_url            = conf.REFER_BASE_URL,
+                                                merchant_acct_code  = merchant_acct.account_code,
+                                                referrer_code       = user_acct.referral_code,
+                                                )
+                    
+                    refer_a_friend_deep_link = conf.REFER_A_FRIEND_DEEP_LINK.format(
+                                                merchant_acct_code   = merchant_acct.account_code,
+                                                referrer_code   = user_acct.referral_code,
+                                                )
+                    
+                    
+                    refer_a_friend_message = refer_a_friend_message.format(
+                                                referee_promote_desc    = referee_promote_desc,
+                                                brand_name              = merchant_acct.brand_name,
+                                                refer_a_friend_url      = refer_a_friend_url,
+                                                )
+                    
+                    merchant_info['referral_program_settings']['refer_a_friend_url']        = refer_a_friend_url
+                    merchant_info['referral_program_settings']['refer_a_friend_message']    = refer_a_friend_message
+                    merchant_info['referral_program_settings']['refer_a_friend_deep_link']  = refer_a_friend_deep_link
+                
+                if merchant_rating_result:
+                    logger.debug('rating_result=%s', merchant_rating_result.rating_result)
+                    merchant_info['rating_reviews'] = merchant_rating_result.rating_result
+                
+                user_details                                        = customer.registered_user_acct
+                customer_details = customer.to_dict(date_format="%d-%m-%Y", datetime_format="%d-%m-%Y %H:%M:%S")
+                customer_details['customer_key']               = customer.key_in_str
+                customer_details['is_email_verified']          = user_details.is_email_verified
+                customer_details['is_mobile_phone_verified']   = user_details.is_mobile_phone_verified
+                
+                customer_basic_memberships_list = _list_customer_basic_memberships(customer)
+                if customer_basic_memberships_list:
+                    customer_details['basic_memberships'] = customer_basic_memberships_list
+                
+                tier_membership_data = _get_tier_membership(customer)
+                if tier_membership_data:
+                    customer_details['tier_membership'] = tier_membership_data
                 
         logger.debug('merchant_info=%s', merchant_info)
-            
-        return create_rest_message(status_code=StatusCode.OK,
+        
+        if customer:    
+            return create_api_message(status_code=StatusCode.OK,
                                                merchant_info    = merchant_info,
                                                customer_details = customer_details,
                                                )
+        else:
+            return create_api_message(status_code=StatusCode.BAD_REQUEST)                                       
     else:
-        return create_rest_message("Missing merchant account key", status_code=StatusCode.BAD_REQUEST)    
+        return create_api_message("Missing merchant account key", status_code=StatusCode.BAD_REQUEST)    
 
 def _list_customer_basic_memberships(customer):
     customer_membership_final_list = []
     
     if is_not_empty(customer.memberships_list):
         customer_memberships_list = CustomerMembership.list_all_by_customer(customer)
         if is_not_empty(customer_memberships_list):
@@ -233,15 +358,15 @@
                     customer_details_dict['voucher_summary']            = customer.entitled_voucher_summary
                     del customer_details_dict['entitled_voucher_summary']
                 '''
         return jsonify(customer_details_dict)
             
     
     else:
-        return create_rest_message("Missing merchant account key or user reference code", status_code=StatusCode.BAD_REQUEST)
+        return create_api_message("Missing merchant account key or user reference code", status_code=StatusCode.BAD_REQUEST)
 
 
 class AccountActivatedAPIResource(APIBaseResource):  
     
     @auth.login_required
     def post(self):
         username    = auth.current_user()
```

### Comparing `trex-apis-1.3.8/trexapi/controllers/message_api_routes.py` & `trex-apis-1.4.0/trexapi/controllers/message_api_routes.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 '''
 Created on 3 Jan 2024
 
 @author: jacklok
 '''
 
-from flask import Blueprint, request
+from flask import Blueprint
 import logging
-from trexlib.utils.log_util import get_tracelog
-from firebase_admin import credentials, messaging
+from firebase_admin import messaging
 
-from trexapi import conf
-from flask.json import jsonify
 from trexapi.utils.api_helpers import create_api_message, StatusCode
-from trexlib.utils.string_util import random_number
+from trexlib.libs.flask_wtf.request_wrapper import request_json
 
 message_api_bp = Blueprint('message_api_bp', __name__,
                                  template_folder='templates',
                                  static_folder='static',
                                  url_prefix='/api/v1/message')
 
 #cred = credentials.Certificate(conf.FIREBASE_SERVICE_ACCOUNT_KEY_PATH)
 #firebase_admin.initialize_app(cred)
 
 
 logger = logging.getLogger('api')
 
 @message_api_bp.route('/private/create', methods=['POST'])
-def create_private_message():
-    notification_data_in_json   = request.get_json()
+@request_json
+def create_private_message(notification_data_in_json):
+    #notification_data_in_json   = request.get_json()
     title_data                  = notification_data_in_json.get('title')
     message_data                = notification_data_in_json.get('message')
     analytics_label             = notification_data_in_json.get('analytics_label')
     device_token                = notification_data_in_json.get('device_token')
     speech                      = notification_data_in_json.get('speech')
     
     logger.info('title_data=%s', title_data)
@@ -54,16 +52,17 @@
     response = messaging.send(message)
     
     logger.debug('response=%s', response)
     
     return create_api_message(status_code=StatusCode.OK,)
 
 @message_api_bp.route('/private/notification/create', methods=['POST'])
-def create_private_notification():
-    notification_data_in_json   = request.get_json()
+@request_json
+def create_private_notification(notification_data_in_json):
+    #notification_data_in_json   = request.get_json()
     title_data                  = notification_data_in_json.get('title')
     message_data                = notification_data_in_json.get('message')
     analytics_label             = notification_data_in_json.get('analytics_label')
     image                       = notification_data_in_json.get('image')
     device_token                = notification_data_in_json.get('device_token')
     speech                      = notification_data_in_json.get('speech')
     
@@ -115,16 +114,17 @@
     response = messaging.send(message)
     
     logger.debug('response=%s', response)
     
     return create_api_message(status_code=StatusCode.OK,)
                               
 @message_api_bp.route('/topic/create', methods=['POST'])
-def create_topic_message():
-    notification_data_in_json   = request.get_json()
+@request_json
+def create_topic_message(notification_data_in_json):
+    #notification_data_in_json   = request.get_json()
     title_data                  = notification_data_in_json.get('title')
     message_data                = notification_data_in_json.get('message')
     analytics_label             = notification_data_in_json.get('analytics_label')
     image                       = notification_data_in_json.get('image')
     topic                       = notification_data_in_json.get('topic')
     speech                      = notification_data_in_json.get('speech')
     
@@ -152,16 +152,17 @@
     response = messaging.send(message)
     
     logger.debug('response=%s', response)
     
     return create_api_message(status_code=StatusCode.OK,)
 
 @message_api_bp.route('/topic/notification/create', methods=['POST'])
-def create_topic_notification():
-    notification_data_in_json   = request.get_json()
+@request_json
+def create_topic_notification(notification_data_in_json):
+    #notification_data_in_json   = request.get_json()
     title_data                  = notification_data_in_json.get('title')
     message_data                = notification_data_in_json.get('message')
     analytics_label             = notification_data_in_json.get('analytics_label')
     image                       = notification_data_in_json.get('image')
     topic                       = notification_data_in_json.get('topic')
     
     logger.info('title_data=%s', title_data)
@@ -186,16 +187,17 @@
     response = messaging.send(message)
     
     logger.debug('response=%s', response)
     
     return create_api_message(status_code=StatusCode.OK,)
 
 @message_api_bp.route('/topic/notification/unsubscribe', methods=['POST'])
-def unsubscribe_topic_notification():
-    notification_data_in_json   = request.get_json()
+@request_json
+def unsubscribe_topic_notification(notification_data_in_json):
+    #notification_data_in_json   = request.get_json()
     device_token                = notification_data_in_json.get('device_token')
     topic                       = notification_data_in_json.get('topic')
     
     logger.info('topic=%s', topic)
     logger.info('device_token=%s', device_token)
     
     messaging.unsubscribe_from_topic(device_token, topic)
```

### Comparing `trex-apis-1.3.8/trexapi/controllers/outlet_api_routes.py` & `trex-apis-1.4.0/trexapi/controllers/outlet_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.8/trexapi/controllers/payment_api_routes.py` & `trex-apis-1.4.0/trexapi/controllers/payment_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.8/trexapi/controllers/pos_api_routes.py` & `trex-apis-1.4.0/trexapi/controllers/pos_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.8/trexapi/controllers/prepaid_api_routes.py` & `trex-apis-1.4.0/trexapi/controllers/prepaid_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.8/trexapi/controllers/rating_api_routes.py` & `trex-apis-1.4.0/trexapi/controllers/rating_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.8/trexapi/controllers/redemption_api_routes.py` & `trex-apis-1.4.0/trexapi/controllers/redemption_api_routes.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,30 +3,20 @@
 
 @author: jacklok
 '''
 from flask import Blueprint, request
 import logging
 from trexlib.utils.log_util import get_tracelog
 from trexmodel.utils.model.model_util import create_db_client
-from trexadmin.libs.http import create_rest_message
-from trexadmin.libs.http import StatusCode
+from trexapi.utils.api_helpers import StatusCode, create_api_message
 from trexmodel.models.datastore.customer_models import Customer
 from trexapi.decorators.api_decorators import customer_key_required
-from trexadmin.libs.decorators import elapsed_time_trace
-from flask.json import jsonify
 from flask_babel import gettext
-from trexadmin import conf
-from trexmodel import conf as model_conf, program_conf
-import os
 from datetime import datetime
-from trexmodel.models.datastore.model_decorators import model_transactional
-from trexmodel.models.datastore.transaction_models import CustomerTransaction
 from trexmodel.models.datastore.redemption_catalogue_models import RedemptionCatalogue
-from trexmodel.models.datastore.redeem_models import RedemptionCatalogueTransaction,\
-    CustomerRedemption
     
 from trexapi.utils.redemption_catalogue_helper import giveaway_redeem_catalogue_item
 
 redemption_api_bp = Blueprint('redemption_api_bp', __name__,
                                  template_folder='templates',
                                  static_folder='static',
                                  url_prefix='/api/v1/redemption')
@@ -55,15 +45,15 @@
                     if __check_is_still_active(catalogue):
                         if __check_is_eligible(customer, catalogue.get('exclusivity')):
                             catalogue['items'] = __resolve_catalogue_items_details(catalogue.get('items'), merchant_acct.published_voucher_configuration.get('vouchers'))
                             filtered_catalogues_list.append(catalogue)
     
     logger.debug('filtered_catalogues_list=%s', filtered_catalogues_list)
                 
-    return create_rest_message(status_code=StatusCode.OK, catalogues_list=filtered_catalogues_list) 
+    return create_api_message(status_code=StatusCode.OK, catalogues_list=filtered_catalogues_list) 
 
 @redemption_api_bp.route('/list-redemption-catalogue/reward-type/<reward_type>', methods=['GET'])
 @customer_key_required
 def list_redemption_catalogue_by_reward_type(customer_key, reward_type):
     logger.info('customer_key=%s', customer_key)
     logger.info('reward_type=%s', reward_type)
     db_client = create_db_client(caller_info="list_redemption_catalogue_by_reward_type")
@@ -84,15 +74,15 @@
                         if __check_is_still_active(catalogue):
                             if __check_is_eligible(customer, catalogue.get('exclusivity')):
                                 catalogue['items'] = __resolve_catalogue_items_details(catalogue.get('items'), merchant_acct.published_voucher_configuration.get('vouchers'))
                                 filtered_catalogues_list.append(catalogue)
     
     logger.debug('filtered_catalogues_list=%s', filtered_catalogues_list)
                 
-    return create_rest_message(status_code=StatusCode.OK, catalogues_list=filtered_catalogues_list)    
+    return create_api_message(status_code=StatusCode.OK, catalogues_list=filtered_catalogues_list)    
 
 def __resolve_catalogue_items_details(catalogue_items_list, vouchers_list):
     resolved_items_list = []
     voucher_dict = __convert_vouchers_list_to_dict(vouchers_list)
     for item in catalogue_items_list:
         voucher = voucher_dict.get(item.get('voucher_key'))
         if voucher:
@@ -206,21 +196,21 @@
                         giveaway_redeem_catalogue_item(customer, redemption_catalogue, voucher_key)
                         reward_summary_after      = customer.reward_summary
                         logger.debug('reward_summary_after=%s', reward_summary_after)
                         
                     
     except:
         logger.error('Failed to redeem due to %s', get_tracelog())
-        return create_rest_message(gettext('Failed to redeem'), status_code=StatusCode.BAD_REQUEST)            
+        return create_api_message(gettext('Failed to redeem'), status_code=StatusCode.BAD_REQUEST)            
             
     if redeem_item_details is None:
-        return create_rest_message(gettext('Invalid redeem item'), status_code=StatusCode.BAD_REQUEST)    
+        return create_api_message(gettext('Invalid redeem item'), status_code=StatusCode.BAD_REQUEST)    
     elif customer is None:    
-        return create_rest_message(gettext('Invalid customer profile'), status_code=StatusCode.BAD_REQUEST)
+        return create_api_message(gettext('Invalid customer profile'), status_code=StatusCode.BAD_REQUEST)
     
     with db_client.context():
         customer_details_dict = customer.to_dict(date_format="%d-%m-%Y", datetime_format="%d-%m-%Y %H:%M:%S")
             
     #customer_details_json =  jsonify(customer_details_dict)
     
-    return create_rest_message(customer_latest_reward=customer_details_dict, status_code=StatusCode.OK)
+    return create_api_message(customer_latest_reward=customer_details_dict, status_code=StatusCode.OK)
```

### Comparing `trex-apis-1.3.8/trexapi/controllers/reward_api_routes.py` & `trex-apis-1.4.0/trexapi/controllers/reward_api_routes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,36 @@
 '''
 Created on 14 Jul 2021
 
 @author: jacklok
 '''
 
-from flask import Blueprint, request, session, jsonify 
-from flask_restful import abort
+from flask import Blueprint 
 import logging
 from trexlib.utils.log_util import get_tracelog
-from flask_restful import Api
 from trexmodel.utils.model.model_util import create_db_client
 #from flask.json import jsonify
 from datetime import datetime, timedelta
 from trexapi.decorators.api_decorators import auth_token_required,\
     outlet_key_required, device_is_activated
 from trexlib.utils.string_util import is_not_empty
 from trexmodel.models.datastore.customer_models import Customer
-from trexmodel.models.datastore.user_models import User
-from trexadmin.libs.http import create_rest_message
-from trexadmin.libs.http import StatusCode
-from trexmodel.models.datastore.merchant_models import Outlet,\
-    MerchantAcct, MerchantUser
+from trexapi.utils.api_helpers import create_api_message, StatusCode
+from trexmodel.models.datastore.merchant_models import Outlet,MerchantUser
 from trexapi.forms.reward_api_forms import GiveRewardTransactionForm, RedeemRewardTransactionForm,\
     PrepaidTopupForm, PrepaidRedeemForm, PointRedeemForm
 from werkzeug.datastructures import ImmutableMultiDict
 from trexmodel.models.datastore.transaction_models import CustomerTransaction
 from trexapi.utils.reward_transaction_helper import create_reward_transaction,\
     redeem_reward_transaction, create_topup_prepaid_transaction
 from trexapi.utils.api_helpers import get_logged_in_api_username
 from trexmodel.models.datastore.voucher_models import MerchantVoucher
-from trexapi import conf
 from trexmodel.models.datastore.prepaid_models import PrepaidSettings
-from trexadmin.libs.jinja.common_filters import format_currency_with_currency_label_filter
-from trexadmin.libs.flask.utils.flask_helper import get_merchant_configured_currency_details
-from trexmodel import program_conf
-
+from trexconf import program_conf
+from trexlib.libs.flask_wtf.request_wrapper import request_json, request_headers
 
 reward_api_bp = Blueprint('reward_api_bp', __name__,
                                  template_folder='templates',
                                  static_folder='static',
                                  url_prefix='/api/v1/reward')
 
 logger = logging.getLogger('api')
@@ -75,37 +67,39 @@
                                             'expiry_date'   : redeem_info.get('expiry_date'),
                                             })
                 '''
                 if all_voucher_list:        
                     all_reward_summary['vouchers'] = all_voucher_list        
                 '''
                         
-                return create_rest_message(
+                return create_api_message(
                                             entitled_reward_summary  = all_reward_summary, 
                                             status_code=StatusCode.OK
                                             )
             
         if customer is None:
-            return create_rest_message('Reference code is invalid', status_code=StatusCode.BAD_REQUEST)
+            return create_api_message('Reference code is invalid', status_code=StatusCode.BAD_REQUEST)
             
     else:
-        return create_rest_message('Reference code is required', status_code=StatusCode.BAD_REQUEST)
+        return create_api_message('Reference code is required', status_code=StatusCode.BAD_REQUEST)
     
 
 @reward_api_bp.route('/reference-code/<reference_code>/give', methods=['POST'])
 @auth_token_required
 @outlet_key_required
 @device_is_activated
-def give_reward(reference_code):
+@request_json
+@request_headers
+def give_reward(transaction_data_in_json, request_headers, reference_code):
     
     logger.debug('reference_code=%s', reference_code)
     
     if is_not_empty(reference_code):
     
-        transaction_data_in_json   = request.get_json()
+        #transaction_data_in_json   = request.get_json()
         
         logger.debug('transaction_data_in_json=%s', transaction_data_in_json)
         
         reward_transaction_form = GiveRewardTransactionForm(ImmutableMultiDict(transaction_data_in_json))
         
         if reward_transaction_form.validate():
             logger.debug('reward transaction data is valid')
@@ -135,35 +129,35 @@
             check_transaction_by_invoice_id = None
             
             if is_not_empty(invoice_id):
                 with db_client.context():
                     check_transaction_by_invoice_id = CustomerTransaction.get_by_invoice_id(invoice_id)
             
             if check_transaction_by_invoice_id:
-                return create_rest_message("The invoice id have been taken", status_code=StatusCode.BAD_REQUEST)
+                return create_api_message("The invoice id have been taken", status_code=StatusCode.BAD_REQUEST)
             else:
                 transact_datetime_in_gmt    = reward_transaction_form.transact_datetime.data
                 merchant_username           = get_logged_in_api_username()
                 
                 logger.debug('transact_datetime_in_gmt=%s', transact_datetime_in_gmt)
                 
                 if merchant_username:
                     try:
                         with db_client.context():
-                            transact_outlet         = Outlet.fetch(request.headers.get('x-outlet-key'))
+                            transact_outlet         = Outlet.fetch(request_headers.get('x-outlet-key'))
                             merchant_acct           = transact_outlet.merchant_acct_entity
                             customer                = Customer.get_by_reference_code(reference_code, merchant_acct)
                             
                                 
                             if transact_datetime_in_gmt:
                                 transact_datetime    =  transact_datetime_in_gmt - timedelta(hours=merchant_acct.gmt_hour)
                                 
                                 now                  = datetime.utcnow()
                                 if transact_datetime > now:
-                                    return create_rest_message('Transact datetime cannot be future', status_code=StatusCode.BAD_REQUEST)
+                                    return create_api_message('Transact datetime cannot be future', status_code=StatusCode.BAD_REQUEST)
                             
                             
                             
                             transact_merchant_user = MerchantUser.get_by_username(merchant_username)
                             
                             logger.debug('going to call give_reward_transaction')
                             
@@ -202,37 +196,39 @@
                                                     'entitled_reward_summary'   : customer_transaction.entitled_reward_summary,
                                                     'entitled_voucher_summary'  : customer_entitled_voucher_list,
                                                     }
                                 
                         return (transaction_details, StatusCode.OK)
                     except:
                         logger.error('Failed to proceed transaction due to %s', get_tracelog())
-                        return create_rest_message('Failed to proceed transaction', status_code=StatusCode.BAD_REQUEST)
+                        return create_api_message('Failed to proceed transaction', status_code=StatusCode.BAD_REQUEST)
                                 
                 else:
-                    return create_rest_message('Missing transact user account', status_code=StatusCode.BAD_REQUEST)
+                    return create_api_message('Missing transact user account', status_code=StatusCode.BAD_REQUEST)
         else:
             logger.warn('reward transaction data input is invalid')
             error_message = reward_transaction_form.create_rest_return_error_message()
             
-            return create_rest_message(error_message, status_code=StatusCode.BAD_REQUEST)
+            return create_api_message(error_message, status_code=StatusCode.BAD_REQUEST)
     else:
-        return create_rest_message('Reference code is required', status_code=StatusCode.BAD_REQUEST)
+        return create_api_message('Reference code is required', status_code=StatusCode.BAD_REQUEST)
     
 @reward_api_bp.route('/reference-code/<reference_code>/redeem', methods=['POST'])
 @auth_token_required
 @outlet_key_required
 @device_is_activated
-def redeem_reward(reference_code):
+@request_json
+@request_headers
+def redeem_reward(transaction_data_in_json, request_headers, reference_code):
     
     logger.debug('reference_code=%s', reference_code)
     
     if is_not_empty(reference_code):
     
-        transaction_data_in_json   = request.get_json()
+        #transaction_data_in_json   = request.get_json()
         
         logger.debug('transaction_data_in_json=%s', transaction_data_in_json)
         
         redeem_reward_transaction_form = RedeemRewardTransactionForm(ImmutableMultiDict(transaction_data_in_json))
         
         if redeem_reward_transaction_form.validate():
             logger.debug('reward transaction data is valid')
@@ -253,33 +249,33 @@
             logger.debug('reward_amount=%s', reward_amount)
             logger.debug('invoice_id=%s', invoice_id)
             logger.debug('remarks=%s', remarks)
             logger.debug('redeem_datetime_in_gmt=%s', redeem_datetime_in_gmt)
             
             db_client = create_db_client(caller_info="redeem_reward")
             with db_client.context():
-                redeemed_by_outlet      = Outlet.fetch(request.headers.get('x-outlet-key'))
+                redeemed_by_outlet      = Outlet.fetch(request_headers.get('x-outlet-key'))
                 merchant_acct           = redeemed_by_outlet.merchant_acct_entity
             
             if redeem_datetime_in_gmt:
                 redeem_datetime    =  redeem_datetime_in_gmt - timedelta(hours=merchant_acct.gmt_hour)
                 
                 now                  = datetime.utcnow()
                 if redeem_datetime > now:
-                    return create_rest_message('Redeem datetime cannot be future', status_code=StatusCode.BAD_REQUEST)
+                    return create_api_message('Redeem datetime cannot be future', status_code=StatusCode.BAD_REQUEST)
                 
                 
                 
             if merchant_username:
                 try:
                     with db_client.context():
                         customer = Customer.get_by_reference_code(reference_code)
                         if customer:
                             merchant_acct   = customer.registered_merchant_acct
-                            redeem_outlet = Outlet.fetch(request.headers.get('x-outlet-key'))
+                            redeem_outlet = Outlet.fetch(request_headers.get('x-outlet-key'))
                             
                         redeem_by_merchant_user = MerchantUser.get_by_username(merchant_username)
                         
                         logger.debug('going to call redeem_reward_transaction')
                         
                         customer_redemption = redeem_reward_transaction(customer, 
                                                                         redeem_outlet       = redeem_outlet, 
@@ -302,37 +298,39 @@
                 
                 except Exception as e:
                     logger.error('Failed to proceed transaction due to %s', get_tracelog())
                     error_message = e.message
                     
                     logger.error('Failed to proceeed transaction due to %s'. error_message)
                     
-                    return create_rest_message('Failed to proceed transaction', status_code=StatusCode.BAD_REQUEST)
+                    return create_api_message('Failed to proceed transaction', status_code=StatusCode.BAD_REQUEST)
                             
             else:
-                return create_rest_message('Missing redeem user account', status_code=StatusCode.BAD_REQUEST)
+                return create_api_message('Missing redeem user account', status_code=StatusCode.BAD_REQUEST)
         
         else:
             error_message = redeem_reward_transaction_form.create_rest_return_error_message()
         
-            return create_rest_message(error_message, status_code=StatusCode.BAD_REQUEST)
+            return create_api_message(error_message, status_code=StatusCode.BAD_REQUEST)
         
     else:
-        return create_rest_message('Reference code is required', status_code=StatusCode.BAD_REQUEST)   
+        return create_api_message('Reference code is required', status_code=StatusCode.BAD_REQUEST)   
     
 @reward_api_bp.route('/reference-code/<reference_code>/prepaid-topup', methods=['POST'])
 @auth_token_required
 @outlet_key_required
 @device_is_activated
-def prepaid_topup(reference_code):
+@request_json
+@request_headers
+def prepaid_topup(prepaid_topup_data_in_json, request_headers, reference_code):
     
     logger.debug('reference_code=%s', reference_code)
     
     if is_not_empty(reference_code):  
-        prepaid_topup_data_in_json   = request.get_json()
+        #prepaid_topup_data_in_json   = request.get_json()
           
         logger.debug('prepaid_topup_data_in_json=%s', prepaid_topup_data_in_json)
         
         prepaid_topup_form      = PrepaidTopupForm(ImmutableMultiDict(prepaid_topup_data_in_json))
         
         
         
@@ -345,15 +343,15 @@
             remarks                 = prepaid_topup_form.remarks.data
             merchant_username       = get_logged_in_api_username()
             customer_transaction    = None    
             prepaid_summary         = {}
             
             db_client = create_db_client(caller_info="prepaid_topup")
             with db_client.context():
-                topup_outlet            = Outlet.fetch(request.headers.get('x-outlet-key'))
+                topup_outlet            = Outlet.fetch(request_headers.get('x-outlet-key'))
                 merchant_acct           = topup_outlet.merchant_acct_entity
                 customer_acct           = Customer.get_by_reference_code(reference_code, merchant_acct)
                 prepaid_program         = PrepaidSettings.fetch(prepaid_program_key)
                 topup_by_merchant_user  = MerchantUser.get_by_username(merchant_username)
                 
                 if customer_acct and prepaid_program:
                     
@@ -364,40 +362,38 @@
                                                                                                 invoice_id=invoice_id, 
                                                                                                 remarks = remarks,
                                                                                                 system_remarks = 'Topup Prepaid',
                                                                                                 )
                     
                     
             if customer_transaction is not None:
-                #prepaid_amount              = prepaid_summary.get('amount')
-                #currency_details            = get_merchant_configured_currency_details()
-                #formatted_prepaid_amount    = format_currency_with_currency_label_filter(prepaid_amount, currency_details=currency_details)
-                
                 
-                return create_rest_message('Prepaid have been topup successfully',
+                return create_api_message('Prepaid have been topup successfully',
                                             status_code=StatusCode.OK
                                             )
             else:
-                return create_rest_message('Failed to topup prepaid', status_code=StatusCode.BAD_REQUEST)
+                return create_api_message('Failed to topup prepaid', status_code=StatusCode.BAD_REQUEST)
                 
         else:
             error_message = prepaid_topup_form.create_rest_return_error_message()
             
-            return create_rest_message(error_message, status_code=StatusCode.BAD_REQUEST)
+            return create_api_message(error_message, status_code=StatusCode.BAD_REQUEST)
         
 @reward_api_bp.route('/reference-code/<reference_code>/prepaid-redeem', methods=['POST'])
 @auth_token_required
 @outlet_key_required
 @device_is_activated
-def prepaid_redeem(reference_code):
+@request_json
+@request_headers
+def prepaid_redeem(prepaid_redeem_data_in_json, request_headers, reference_code):
     
     logger.debug('reference_code=%s', reference_code)
     
     if is_not_empty(reference_code):  
-        prepaid_redeem_data_in_json   = request.get_json()
+        #prepaid_redeem_data_in_json   = request.get_json()
           
         logger.debug('prepaid_redeem_data_in_json=%s', prepaid_redeem_data_in_json)
         
         prepaid_redeem_form      = PrepaidRedeemForm(ImmutableMultiDict(prepaid_redeem_data_in_json))
         
         
         
@@ -409,15 +405,15 @@
             remarks                 = prepaid_redeem_form.remarks.data
             merchant_username       = get_logged_in_api_username()
             
             redemption_details      = None
             
             db_client = create_db_client(caller_info="prepaid_redeem")
             with db_client.context():
-                redeemed_outlet         = Outlet.fetch(request.headers.get('x-outlet-key'))
+                redeemed_outlet         = Outlet.fetch(request_headers.get('x-outlet-key'))
                 merchant_acct           = redeemed_outlet.merchant_acct_entity
                 customer_acct           = Customer.get_by_reference_code(reference_code, merchant_acct)
                 redeem_by_merchant_user = MerchantUser.get_by_username(merchant_username)
                 
                 if customer_acct:
                     redemption_details  = redeem_reward_transaction(customer_acct,  
                                                                 redeem_outlet               = redeemed_outlet,
@@ -431,35 +427,37 @@
                     
                     logger.debug('redemption_details=%s', redemption_details)
                     
                     
             if redemption_details is not None:
                 
                 
-                return create_rest_message('Prepaid have been redeemed successfully',
+                return create_api_message('Prepaid have been redeemed successfully',
                                             status_code=StatusCode.OK
                                             )
             else:
-                return create_rest_message('Failed to redeem prepaid', status_code=StatusCode.BAD_REQUEST)
+                return create_api_message('Failed to redeem prepaid', status_code=StatusCode.BAD_REQUEST)
                 
         else:
             error_message = prepaid_redeem_form.create_rest_return_error_message()
             
-            return create_rest_message(error_message, status_code=StatusCode.BAD_REQUEST)
+            return create_api_message(error_message, status_code=StatusCode.BAD_REQUEST)
         
 @reward_api_bp.route('/reference-code/<reference_code>/point-redeem', methods=['POST'])
 @auth_token_required
 @outlet_key_required
 @device_is_activated
-def point_redeem(reference_code):
+@request_json
+@request_headers
+def point_redeem(point_redeem_data_in_json, request_headers, reference_code):
     
     logger.debug('reference_code=%s', reference_code)
     
     if is_not_empty(reference_code):  
-        point_redeem_data_in_json   = request.get_json()
+        #point_redeem_data_in_json   = request.get_json()
           
         logger.debug('point_redeem_data_in_json=%s', point_redeem_data_in_json)
         
         point_redeem_form      = PointRedeemForm(ImmutableMultiDict(point_redeem_data_in_json))
         
         
         
@@ -471,15 +469,15 @@
             remarks                 = point_redeem_form.remarks.data
             merchant_username       = get_logged_in_api_username()
             
             redemption_details      = None
             
             db_client = create_db_client(caller_info="prepaid_redeem")
             with db_client.context():
-                redeemed_outlet         = Outlet.fetch(request.headers.get('x-outlet-key'))
+                redeemed_outlet         = Outlet.fetch(request_headers.get('x-outlet-key'))
                 merchant_acct           = redeemed_outlet.merchant_acct_entity
                 customer_acct           = Customer.get_by_reference_code(reference_code, merchant_acct)
                 redeem_by_merchant_user = MerchantUser.get_by_username(merchant_username)
                 
                 if customer_acct:
                     redemption_details  = redeem_reward_transaction(customer_acct,  
                                                                 redeem_outlet               = redeemed_outlet,
@@ -493,18 +491,18 @@
                     
                     logger.debug('redemption_details=%s', redemption_details)
                     
                     
             if redemption_details is not None:
                 
                 
-                return create_rest_message('Point have been redeemed successfully',
+                return create_api_message('Point have been redeemed successfully',
                                             status_code=StatusCode.OK
                                             )
             else:
-                return create_rest_message('Failed to redeem point', status_code=StatusCode.BAD_REQUEST)
+                return create_api_message('Failed to redeem point', status_code=StatusCode.BAD_REQUEST)
                 
         else:
             error_message = point_redeem_form.create_rest_return_error_message()
             
-            return create_rest_message(error_message, status_code=StatusCode.BAD_REQUEST)        
+            return create_api_message(error_message, status_code=StatusCode.BAD_REQUEST)
```

### Comparing `trex-apis-1.3.8/trexapi/controllers/sales_api_routes.py` & `trex-apis-1.4.0/trexapi/controllers/sales_api_routes.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,22 +17,20 @@
 from trexmodel.models.datastore.transaction_models import SalesTransaction,\
     CustomerTransaction
 
 from trexapi.utils.reward_transaction_helper import create_sales_transaction,\
     give_reward_from_sales_transaction
 from trexapi.utils.api_helpers import get_logged_in_api_username,\
     create_api_message, StatusCode
-from trexmodel.models.datastore.voucher_models import MerchantVoucher
-from trexapi import conf
-from trexmodel.models.datastore.prepaid_models import PrepaidSettings
-from trexmodel import program_conf
+from trexconf import conf
 from trexapi.forms.sales_api_forms import SalesTransactionForm
-from trexlib.utils.crypto_util import encrypt, decrypt, decrypt_json
+from trexlib.utils.crypto_util import encrypt, decrypt
 from trexapi.conf import EARN_INSTANT_REWARD_URL
 from flask_babel import gettext
+from trexlib.libs.flask_wtf.request_wrapper import request_json, request_headers
 
 
 
 sales_api_bp = Blueprint('sales_api_bp', __name__,
                                  template_folder='templates',
                                  static_folder='static',
                                  url_prefix='/api/v1/sales')
@@ -43,19 +41,21 @@
 @sales_api_bp.route('/ping', methods=['GET'])
 def ping():
     return 'pong', 200
 
 @sales_api_bp.route('/create-sales-transaction', methods=['PUT'])
 @auth_token_required
 @outlet_key_required
-def post_sales_transaction():
+@request_json
+@request_headers
+def post_sales_transaction(transaction_data_in_json, request_headers):
     
     logger.info('---post_sales_transaction---')
     
-    transaction_data_in_json   = request.get_json()
+    #transaction_data_in_json   = request.get_json()
         
     logger.info('transaction_data_in_json=%s', transaction_data_in_json)
     
     transaction_form = SalesTransactionForm(ImmutableMultiDict(transaction_data_in_json))
     
     if transaction_form.validate():
         logger.debug('reward transaction data is valid')
@@ -94,15 +94,15 @@
             transact_datetime_in_gmt    = transaction_form.transact_datetime.data
             merchant_username           = get_logged_in_api_username()
             
             
             if merchant_username:
                 try:
                     with db_client.context():
-                        transact_outlet         = Outlet.fetch(request.headers.get('x-outlet-key'))
+                        transact_outlet         = Outlet.fetch(request_headers.get('x-outlet-key'))
                         merchant_acct           = transact_outlet.merchant_acct_entity
                         
                             
                         if transact_datetime_in_gmt:
                             transact_datetime    =  transact_datetime_in_gmt - timedelta(hours=merchant_acct.gmt_hour)
                             
                             now                  = datetime.utcnow()
@@ -205,15 +205,16 @@
     else:
         return create_api_message(encrypted_transaction_id=encrypted_transaction_id, status_code=StatusCode.OK)     
         
     
     
 @sales_api_bp.route('/reference-code/<reference_code>/transaction/<encrypted_transaction_id>/customer-earn-instant-reward', methods=['POST'])
 @user_auth_token_required
-def customer_earn_instant_reward(reference_code, encrypted_transaction_id): 
+@request_headers
+def customer_earn_instant_reward(request_headers, reference_code, encrypted_transaction_id): 
     
     db_client = create_db_client(caller_info="customer_earn_instant_reward")
         
     logger.info('encrypted_transaction_id=%s', encrypted_transaction_id)
     
     transaction_id = decrypt(encrypted_transaction_id)
     
@@ -240,15 +241,15 @@
                         merchant_acct = sales_transaction.transact_merchant_acct
                         customer = Customer.get_by_reference_code(reference_code, merchant_acct)
                         
                         if customer is None:
                             logger.info('Customer is not found, thus going to create new customer account')
                             instant_reward_issued_outlet = sales_transaction.transact_outlet_entity
                             
-                            reference_code  = request.headers.get('x-reference-code')
+                            reference_code  = request_headers.get('x-reference-code')
                             
                             existing_user_acct = User.get_by_reference_code(reference_code)
                             
                             customer = Customer.create_from_user(instant_reward_issued_outlet, existing_user_acct)
                         
                         if customer:
                             customer_transaction = give_reward_from_sales_transaction(customer, sales_transaction)
```

### Comparing `trex-apis-1.3.8/trexapi/controllers/transaction_api_routes.py` & `trex-apis-1.4.0/trexapi/controllers/transaction_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.8/trexapi/controllers/user_api_routes.py` & `trex-apis-1.4.0/trexapi/controllers/user_api_routes.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,58 +8,61 @@
 import logging
 from trexlib.utils.log_util import get_tracelog
 from trexmodel.utils.model.model_util import create_db_client
 from datetime import datetime, timedelta
 from trexlib.utils.string_util import is_not_empty, random_number, random_string,\
     is_empty, boolify
 from trexmodel.models.datastore.user_models import User
-from trexadmin.libs.http import create_rest_message
-from trexadmin.libs.http import StatusCode
+from trexapi.utils.api_helpers import StatusCode, create_api_message
 from werkzeug.datastructures import ImmutableMultiDict
 from trexapi.forms.user_api_forms import UserRegistrationForm, UserUpdateForm,\
-    OutletReviewsForm
+    OutletReviewsForm, UserStatusForm
 from trexapi.conf import APPLICATION_NAME, APPLICATION_BASE_URL, MOBILE_APP_NAME,\
     USE_VERIFICATION_REQUEST_ID, SEND_REAL_MESSAGE
 from trexmail.email_helper import trigger_send_email
 from trexmodel.models.datastore.merchant_models import MerchantAcct, Outlet
 from trexmodel.models.datastore.customer_models import Customer
 from trexmodel.models.datastore.reward_models import CustomerEntitledVoucher,\
     CustomerPointReward, CustomerEntitledTierRewardSummary
 from trexapi.utils.api_helpers import generate_user_auth_token
 from trexapi.decorators.api_decorators import user_auth_token_required,\
     show_request_info
-from trexadmin.libs.decorators import elapsed_time_trace
 from flask.json import jsonify
-from trexlib.conf import PRODUCTION_MODE, DEPLOYMENT_MODE, DEMO_MODE, LOCAL_MODE
+from trexlib.conf import PRODUCTION_MODE, DEPLOYMENT_MODE, DEMO_MODE
 from flask_babel import gettext
-#from trexadmin import conf
-from trexmodel import conf as model_conf
+from trexconf import conf as model_conf
 import os
 from trexlib.utils.sms_util import send_sms
 from trexmodel.models.datastore.message_models import Message
-from time import strftime
 from trexlib.utils.common.date_util import from_utc_datetime_to_local_datetime
 from trexmodel.conf import USER_STATUS_REGISTERED, GENDER_UNKNOWN_CODE
 from trexmodel.models.datastore.model_decorators import model_transactional
 from trexlib.libs.facebook.util.whatsapp_util import send_whatsapp_verification_message
+from trexanalytics.bigquery_upstream_data_config import create_merchant_registered_customer_upstream_for_merchant,\
+    create_registered_customer_upstream_for_system
+from trexlib.libs.flask_wtf.request_wrapper import request_json, request_headers,\
+    request_values, request_args
+from trexprogram.referral.referral_program import ReferralProgram,\
+    giveaway_referral_program_reward
 
 user_api_bp = Blueprint('user_api_bp', __name__,
                                  template_folder='templates',
                                  static_folder='static',
                                  url_prefix='/api/v1/users')
 
 logger = logging.getLogger('api')
 
 
 @user_api_bp.route('/guest-register', methods=['POST'])
-def guest_register():
+@request_json
+def guest_register(user_data_in_json):
     logger.debug('---guest_register---')
     
     try:
-        user_data_in_json   = request.get_json()
+        #user_data_in_json   = request.get_json()
         logger.debug('guest_register: user_data_in_json=%s', user_data_in_json)
         
         register_user_form  = UserRegistrationForm(ImmutableMultiDict(user_data_in_json))
         if register_user_form.validate():
             logger.debug('guest_register:  registration input is valid')
             db_client = create_db_client(caller_info="guest_register")
             
@@ -74,38 +77,39 @@
                         
                 
                                 
             if registered_user_acct is not None:
                 
                 (expiry_datetime, token)    = generate_user_auth_token(registered_user_acct.user_id, registered_user_acct.reference_code)
                 
-                return create_rest_message(status_code=StatusCode.OK, 
+                return create_api_message(status_code=StatusCode.OK, 
                                            auth_token                           = token,
                                            reference_code                       = registered_user_acct.reference_code,
                                            )
             else:
-                return create_rest_message(status_code=StatusCode.BAD_REQUEST)
+                return create_api_message(status_code=StatusCode.BAD_REQUEST)
             
         else:
             logger.warn('user_register: user registration input is invalid')
             error_message = register_user_form.create_rest_return_error_message()
             
-            return create_rest_message(error_message, status_code=StatusCode.BAD_REQUEST)
+            return create_api_message(error_message, status_code=StatusCode.BAD_REQUEST)
             
     except:
         logger.error('user_register: Fail to register user due to %s', get_tracelog())
         
-        return create_rest_message(status_code=StatusCode.BAD_REQUEST)
+        return create_api_message(status_code=StatusCode.BAD_REQUEST)
     
 @user_api_bp.route('/register', methods=['POST'])
-def user_register():
+@request_json
+def user_register(user_data_in_json):
     logger.debug('user_register: ---user_register---')
     
     try:
-        user_data_in_json   = request.get_json()
+        #user_data_in_json   = request.get_json()
         logger.debug('user_register: user_data_in_json=%s', user_data_in_json)
         
         register_user_form  = UserRegistrationForm(ImmutableMultiDict(user_data_in_json))
         if register_user_form.validate():
             logger.debug('user_register:  registration input is valid')
             db_client = create_db_client(caller_info="user_register")
             
@@ -151,63 +155,64 @@
                                                                 is_email_verified           = True, 
                                                                 is_mobile_phone_verified    = True,
                                                                 status                      = USER_STATUS_REGISTERED,
                                                                )
                             logger.debug('new registered_user_acct=%s', registered_user_acct)
                         else:
                             if checking_registered_user_acct.is_mobile_phone_verified==True:
-                                return create_rest_message('Mobile Phone have been taken', status_code=StatusCode.BAD_REQUEST)
+                                return create_api_message('Mobile Phone have been taken', status_code=StatusCode.BAD_REQUEST)
                     else:
                         registered_user_acct = User.create(
                                                                 name                = name, 
                                                                 email               = email, 
                                                                 birth_date          = birth_date,
                                                                 gender              = gender,
                                                                 password            = password, 
                                                                 is_email_verified   = True,
                                                                 status              = USER_STATUS_REGISTERED,
                                                                )
                         
                         logger.debug('new registered_user_acct=%s', registered_user_acct)
                         
                 else:
-                    return create_rest_message('Email have been taken', status_code=StatusCode.BAD_REQUEST)
+                    return create_api_message('Email have been taken', status_code=StatusCode.BAD_REQUEST)
                 
                                 
             if registered_user_acct is not None:
                 
                 (expiry_datetime, token)    = generate_user_auth_token(registered_user_acct.user_id, registered_user_acct.reference_code)
                 
-                return create_rest_message(status_code=StatusCode.OK, 
+                return create_api_message(status_code=StatusCode.OK, 
                                            auth_token                           = token,
                                            reference_code                       = registered_user_acct.reference_code,
                                            email_vc_expiry_datetime             = registered_user_acct.email_vc_expiry_datetime.strftime('%d-%m-%Y %H:%M:%S') if registered_user_acct.email_vc_expiry_datetime is not None else None,
                                            mobile_phone_vc_expiry_datetime      = registered_user_acct.mobile_phone_vc_expiry_datetime.strftime('%d-%m-%Y %H:%M:%S') if registered_user_acct.mobile_phone_vc_expiry_datetime is not None else None,
                                            status                               = registered_user_acct.status,
                                            )
             else:
-                return create_rest_message(status_code=StatusCode.BAD_REQUEST)
+                return create_api_message(status_code=StatusCode.BAD_REQUEST)
             
         else:
             logger.warn('user_register: user registration input is invalid')
             error_message = register_user_form.create_rest_return_error_message()
             
-            return create_rest_message(error_message, status_code=StatusCode.BAD_REQUEST)
+            return create_api_message(error_message, status_code=StatusCode.BAD_REQUEST)
             
     except:
         logger.error('user_register: Fail to register user due to %s', get_tracelog())
         
-        return create_rest_message(status_code=StatusCode.BAD_REQUEST)    
+        return create_api_message(status_code=StatusCode.BAD_REQUEST)    
 
 @user_api_bp.route('/update', methods=['POST'])
-def user_update():
+@request_json
+def user_update(user_data_in_json):
     logger.debug('user_update: ---user_register---')
     
     try:
-        user_data_in_json   = request.get_json()
+        #user_data_in_json   = request.get_json()
         logger.debug('user_update: user_data_in_json=%s', user_data_in_json)
         
         update_user_form  = UserUpdateForm(ImmutableMultiDict(user_data_in_json))
         if update_user_form.validate():
             logger.debug('update_user_form:  update input is valid')
             db_client = create_db_client(caller_info="user_update")
             
@@ -233,118 +238,152 @@
                 logger.debug('mobile_phone=%s', mobile_phone)
                 logger.debug('birth_date=%s', birth_date)
                 logger.debug('gender=%s', gender)
                 logger.debug('status=%s', status)
                 
                 user_acct = User.get_by_reference_code(reference_code)
                 if user_acct:
+                    
+                    
+                    
                     original_mobile_phone   = user_acct.mobile_phone
                     
+                    is_gender_changed       = user_acct.gender!=gender
+                    is_dob_changed          = user_acct.birth_date!=birth_date
+                    is_name_changed         = user_acct.name!=name
+                    is_mobile_phone_changed = original_mobile_phone!=mobile_phone
+                    
+                    update_upstream = is_gender_changed or is_dob_changed
+                    
+                    update_user_data        =  is_gender_changed or is_dob_changed or is_name_changed or is_mobile_phone_changed
+                    
                     
                     if is_not_empty(mobile_phone):
                         logger.debug('going to update user details with mobile phone=%s', mobile_phone)
-                        if original_mobile_phone!=mobile_phone:
+                        if is_mobile_phone_changed:
                             logger.debug('mobile phone have been changed thus going to check whether new mobile phone is taken or not')
                             checking_mobile_phone_user_acct = User.get_by_mobile_phone(mobile_phone)
                             
                             if checking_mobile_phone_user_acct is None:
                                 logger.debug('mobile phone is not taken')
                                 
                                 _update_user_acct(user_acct, 
                                             mobile_phone    = mobile_phone,
                                             name            = name,
                                             birth_date      = birth_date,
                                             gender          = gender,
                                             status          = status,
+                                            update_upstream = update_upstream,
                                             ) 
                                 
                             else:
-                                return create_rest_message('Mobile Phone have been taken', status_code=StatusCode.BAD_REQUEST)
+                                return create_api_message('Mobile Phone have been taken', status_code=StatusCode.BAD_REQUEST)
                         else:
                             logger.debug('mobile phone is not change')
-                            
-                            _update_user_acct(user_acct, 
+                            if update_user_data:
+                                _update_user_acct(user_acct, 
                                             mobile_phone    = mobile_phone,
                                             name            = name,
                                             birth_date      = birth_date,
                                             gender          = gender,
                                             status          = status,
+                                            update_upstream = update_upstream,
                                             ) 
+                            else:
+                                logger.debug('Ignore to update user details')
                     
                     else:
-                        logger.debug('going to update user details without mobile phone')
-                        
-                        _update_user_acct(user_acct, 
-                                            mobile_phone    = mobile_phone,
-                                            name            = name,
-                                            birth_date      = birth_date,
-                                            gender          = gender,
-                                            status          = status,
-                                            )         
+                        if update_user_data:
+                            logger.debug('going to update user details without mobile phone')
+                            
+                            _update_user_acct(user_acct, 
+                                                mobile_phone    = mobile_phone,
+                                                name            = name,
+                                                birth_date      = birth_date,
+                                                gender          = gender,
+                                                status          = status,
+                                                update_upstream = update_upstream,
+                                                )       
+                        else:
+                            logger.debug('Ignore to update user details')  
                     
                 else:
-                    return create_rest_message('User account is not found', status_code=StatusCode.BAD_REQUEST)
+                    return create_api_message('User account is not found', status_code=StatusCode.BAD_REQUEST)
                 
                                 
-            return create_rest_message(status_code=StatusCode.OK)
+            return create_api_message(status_code=StatusCode.OK)
             
         else:
             logger.warn('user_register: user registration input is invalid')
             error_message = update_user_form.create_rest_return_error_message()
             
-            return create_rest_message(error_message, status_code=StatusCode.BAD_REQUEST)
+            return create_api_message(error_message, status_code=StatusCode.BAD_REQUEST)
             
     except:
         logger.error('user_register: Fail to update user due to %s', get_tracelog())
         
-        return create_rest_message(status_code=StatusCode.BAD_REQUEST)
+        return create_api_message(status_code=StatusCode.BAD_REQUEST)
 
 @model_transactional(desc="_update_user_account")
-def _update_user_acct(user_acct, mobile_phone=None, name=None, birth_date=None, gender=None, status=None):
+def _update_user_acct(user_acct, mobile_phone=None, name=None, birth_date=None, gender=None, status=None, update_upstream=True):
     User.update(user_acct, 
                         mobile_phone    = mobile_phone,
                         name            = name,
                         birth_date      = birth_date,
                         gender          = gender,
                         status          = status,
                         )  
-    Customer.update_all_from_user_acct(user_acct)  
+    __update_customer_data(user_acct)
     
+
+def __update_customer_data(user_acct, update_upstream=True):
+    
+    customer_acct_list = Customer.list_by_user_account(user_acct)
+    if customer_acct_list:
+        for c in customer_acct_list:
+            c.update_from_user_acct(user_acct)
+            
+            if update_upstream:
+                create_merchant_registered_customer_upstream_for_merchant(c)
+                create_registered_customer_upstream_for_system(c)    
     
 @user_api_bp.route('/update-status', methods=['PUT'])
-def user_update_status():
+@request_headers
+@request_json
+def user_update_status(request_headers, user_data_in_json):
     logger.debug('---user_update_status---')
     
-    reference_code      = request.headers.get('x-reference-code')
+    reference_code      = request_headers.get('x-reference-code')
     
     try:
-        user_data_in_json   = request.get_json()
+        #user_data_in_json   = request.get_json()
         logger.debug('user_update_status: user_data_in_json=%s', user_data_in_json)
         
         update_user_status_form  = UserStatusForm(ImmutableMultiDict(user_data_in_json))
         if update_user_status_form.validate():
             logger.debug('update_user_status_form:  update input is valid')
             db_client = create_db_client(caller_info="user_update_status")
             
             with db_client.context():
                 user = User.get_by_reference_code(reference_code)
                 user.status = update_user_status_form.status.data
                 user.put()
                 
-            return create_rest_message(status_code=StatusCode.ACCEPTED)
+            return create_api_message(status_code=StatusCode.ACCEPTED)
 
     except:
         logger.error('Fail to update user status due to %s', get_tracelog())
         
-        return create_rest_message(status_code=StatusCode.BAD_REQUEST)
+        return create_api_message(status_code=StatusCode.BAD_REQUEST)
         
 @user_api_bp.route('/email-auth', methods=['POST'])
-def auth_user_thru_email():
+@request_json
+def auth_user_thru_email(user_data_in_json):
     
-    user_data_in_json   = request.get_json()
+    #user_data_in_json   = request.get_json()
     email               = user_data_in_json.get('email')
     password            = user_data_in_json.get('password')
     
     logger.debug('email=%s', email)
     logger.debug('password=%s', password)
     
     if is_not_empty(email) and is_not_empty(password):
@@ -355,54 +394,55 @@
         
         if user_acct:
             
             logger.debug('auth_user: found user account by email=%s', email)    
             logger.debug('auth_user: found user account by password=%s', password)
             
             if user_acct.is_still_lock:
-                return create_rest_message('User account is locked after many trials for security purpose. Please try after an hour', status_code=StatusCode.BAD_REQUEST)
+                return create_api_message('User account is locked after many trials for security purpose. Please try after an hour', status_code=StatusCode.BAD_REQUEST)
             else:
                 if user_acct.deleted:
-                    return create_rest_message('User email or password is invalid', status_code=StatusCode.BAD_REQUEST)
+                    return create_api_message('User email or password is invalid', status_code=StatusCode.BAD_REQUEST)
                 else:
                     if user_acct.is_valid_password(password):
                     
                         (expiry_datetime, token)    = generate_user_auth_token(user_acct.user_id, user_acct.reference_code)
                         
                         response_data = {
                                             'auth_token'              : token,
                                             }
                             
                         response_data.update(user_details_dict(user_acct))
                         
                         logger.debug('auth_user debug: response_data=%s', response_data)
                         
-                        return create_rest_message(status_code=StatusCode.OK, 
+                        return create_api_message(status_code=StatusCode.OK, 
                                                    **response_data
                                                    
                                                    )
                     else:
                         
                         logger.warn('auth_user: user password is invalid')
                         with db_client.context():
                             user_acct.add_try_count()
                         
-                        return create_rest_message('User email or password is not match', status_code=StatusCode.BAD_REQUEST)
+                        return create_api_message('User email or password is not match', status_code=StatusCode.BAD_REQUEST)
             
         else:
-            return create_rest_message('User email or password is not match', status_code=StatusCode.BAD_REQUEST)
+            return create_api_message('User email or password is not match', status_code=StatusCode.BAD_REQUEST)
             
     else:
         logger.warn('auth_user: user verify input is invalid')
-        return create_rest_message('Missing email or password', status_code=StatusCode.BAD_REQUEST)
+        return create_api_message('Missing email or password', status_code=StatusCode.BAD_REQUEST)
     
 @user_api_bp.route('/mobile-phone-auth', methods=['POST'])
-def auth_user_thru_mobile_phone():
+@request_json
+def auth_user_thru_mobile_phone(user_data_in_json):
     
-    user_data_in_json   = request.get_json()
+    #user_data_in_json   = request.get_json()
     mobile_phone        = user_data_in_json.get('mobile_phone')
     password            = user_data_in_json.get('password')
     
     logger.debug('mobile_phone=%s', mobile_phone)
     logger.debug('password=%s', password)
     
     if is_not_empty(mobile_phone) and is_not_empty(password):
@@ -413,49 +453,49 @@
         
         if user_acct:
             
             logger.debug('auth_user: found user account by mobile_phone=%s', mobile_phone)    
             logger.debug('auth_user: found user account by password=%s', password)
             
             if user_acct.is_still_lock:
-                return create_rest_message('User account is locked after many trials for security purpose. Please try after an hour', status_code=StatusCode.BAD_REQUEST)
+                return create_api_message('User account is locked after many trials for security purpose. Please try after an hour', status_code=StatusCode.BAD_REQUEST)
             else:
                 if user_acct.deleted:
-                    return create_rest_message('User mobile phone or password is invalid', status_code=StatusCode.BAD_REQUEST)
+                    return create_api_message('User mobile phone or password is invalid', status_code=StatusCode.BAD_REQUEST)
                 else:
                     if user_acct.is_valid_password(password):
                     
                         (expiry_datetime, token)    = generate_user_auth_token(user_acct.user_id, user_acct.reference_code)
                         
                         response_data = {
                                             'auth_token'              : token,
                                             }
                             
                         response_data.update(user_details_dict(user_acct))
                         
                         logger.debug('auth_user debug: response_data=%s', response_data)
                         
-                        return create_rest_message(status_code=StatusCode.OK, 
+                        return create_api_message(status_code=StatusCode.OK, 
                                                    **response_data
                                                    
                                                    )
                     else:
                         
                         logger.warn('auth_user: user password is invalid')
                         with db_client.context():
                             user_acct.add_try_count()
                         
-                        return create_rest_message('User mobile phone or password is not match', status_code=StatusCode.BAD_REQUEST)
+                        return create_api_message('User mobile phone or password is not match', status_code=StatusCode.BAD_REQUEST)
             
         else:
-            return create_rest_message('User mobile phone or password is not match', status_code=StatusCode.BAD_REQUEST)
+            return create_api_message('User mobile phone or password is not match', status_code=StatusCode.BAD_REQUEST)
             
     else:
         logger.warn('auth_user: user verify input is invalid')
-        return create_rest_message('Missing mobile phone or password', status_code=StatusCode.BAD_REQUEST)    
+        return create_api_message('Missing mobile phone or password', status_code=StatusCode.BAD_REQUEST)    
 
 
 
 @user_api_bp.route('/set-email-verified', methods=['POST'])
 @user_auth_token_required
 def set_email_verified(reference_code):
     
@@ -466,18 +506,18 @@
     with db_client.context():
         user_acct   = User.get_by_reference_code(reference_code)
     
     if user_acct:
         with db_client.context():
             user_acct.mark_email_verified()
         
-        return create_rest_message(status_code=StatusCode.OK)
+        return create_api_message(status_code=StatusCode.OK)
     
     else:
-        return create_rest_message(status_code=StatusCode.BAD_REQUEST)
+        return create_api_message(status_code=StatusCode.BAD_REQUEST)
     
 @user_api_bp.route('/set-mobile-phone-verified', methods=['POST'])
 @user_auth_token_required
 def set_mobile_phone_verified(reference_code):
     
     db_client = create_db_client(caller_info="set_mobile_phone_verified")
     
@@ -486,24 +526,25 @@
     with db_client.context():
         user_acct   = User.get_by_reference_code(reference_code)
     
     if user_acct:
         with db_client.context():
             user_acct.mark_mobile_phone_verified()
         
-        return create_rest_message(status_code=StatusCode.OK)
+        return create_api_message(status_code=StatusCode.OK)
     
     else:
-        return create_rest_message(status_code=StatusCode.BAD_REQUEST)    
+        return create_api_message(status_code=StatusCode.BAD_REQUEST)    
             
       
 @user_api_bp.route('/verify-email', methods=['POST'])
-def verify_email_account():
+@request_json
+def verify_email_account(user_data_in_json):
     
-    user_data_in_json   = request.get_json()
+    #user_data_in_json   = request.get_json()
     email               = user_data_in_json.get('email')
     verification_code   = user_data_in_json.get('verification_code')
     
     
     if is_not_empty(email) and is_not_empty(verification_code):
         db_client = create_db_client(caller_info="verify_email_account")
         user_acct = None
@@ -516,36 +557,38 @@
         if user_acct:
             logger.debug('verify_email_account: found user account by email=%s', email)    
             if user_acct.email_vc==verification_code:
                 is_within_seconds = (user_acct.email_vc_expiry_datetime - datetime.now()).seconds
                 if is_within_seconds>0:
                     with db_client.context():
                         user_acct.mark_email_verified()
-                    return create_rest_message(status_code=StatusCode.OK)
+                    return create_api_message(status_code=StatusCode.OK)
                 else:
-                    return create_rest_message("Verification Code is expired already", status_code=StatusCode.BAD_REQUEST)
+                    return create_api_message("Verification Code is expired already", status_code=StatusCode.BAD_REQUEST)
             
             else:
                 logger.warn('verify_email_account: verification code is invalid')
-                return create_rest_message("Invalid verification code", status_code=StatusCode.BAD_REQUEST)
+                return create_api_message("Invalid verification code", status_code=StatusCode.BAD_REQUEST)
             
         else:
-            return create_rest_message(status_code=StatusCode.BAD_REQUEST)
+            return create_api_message(status_code=StatusCode.BAD_REQUEST)
             
     else:
         logger.warn('verify_email_account: user verify input is invalid')
-        return create_rest_message(status_code=StatusCode.BAD_REQUEST)    
+        return create_api_message(status_code=StatusCode.BAD_REQUEST)    
     
 @user_api_bp.route('/verify-mobile-phone', methods=['POST'])
-def verify_mobile_phone_account():
+@request_headers
+@request_json
+def verify_mobile_phone_account(request_headers, user_data_in_json):
     
-    user_data_in_json   = request.get_json()
+    #user_data_in_json   = request.get_json()
     mobile_phone        = user_data_in_json.get('mobile_phone')
     verification_code   = user_data_in_json.get('verification_code')
-    reference_code      = request.headers.get('x-reference-code')
+    reference_code      = request_headers.get('x-reference-code')
     
     if is_not_empty(mobile_phone) and is_not_empty(verification_code):
         db_client = create_db_client(caller_info="verify_mobile_phone_account")
         user_acct = None
         with db_client.context():
             user_acct_by_mobile_phone   = User.get_by_mobile_phone(mobile_phone)
             user_acct                   = User.get_by_reference_code(reference_code)
@@ -554,36 +597,37 @@
             if user_acct:
                 logger.debug('verify_mobile_phone_account: found user account by mobile_phone=%s', mobile_phone)    
                 if user_acct.mobile_phone_vc==verification_code:
                     is_within_seconds = (user_acct.mobile_phone_vc_expiry_datetime - datetime.now()).seconds
                     if is_within_seconds>0:
                         with db_client.context():
                             user_acct.mark_email_verified()
-                        return create_rest_message(status_code=StatusCode.OK)
+                        return create_api_message(status_code=StatusCode.OK)
                     else:
-                        return create_rest_message("Verification Code is expired already", status_code=StatusCode.BAD_REQUEST)
+                        return create_api_message("Verification Code is expired already", status_code=StatusCode.BAD_REQUEST)
                 
                 else:
                     logger.warn('verify_mobile_phone_account: verification code is invalid')
-                    return create_rest_message("Invalid verification code", status_code=StatusCode.BAD_REQUEST)
+                    return create_api_message("Invalid verification code", status_code=StatusCode.BAD_REQUEST)
                 
             else:
                 
-                return create_rest_message(gettext('Invalid user account'), status_code=StatusCode.BAD_REQUEST)
+                return create_api_message(gettext('Invalid user account'), status_code=StatusCode.BAD_REQUEST)
         else:
-            return create_rest_message(gettext('Mobile phone have been taken'), status_code=StatusCode.BAD_REQUEST)
+            return create_api_message(gettext('Mobile phone have been taken'), status_code=StatusCode.BAD_REQUEST)
             
     else:
         logger.warn('verify_mobile_phone_account: user verify input is invalid')
-        return create_rest_message(status_code=StatusCode.BAD_REQUEST)        
+        return create_api_message(status_code=StatusCode.BAD_REQUEST)        
 
 @user_api_bp.route('/register-as-customer', methods=['POST'])
+@request_json
 #@user_auth_token_required
-def register_user_as_customer():
-    user_data_in_json           = request.get_json()
+def register_user_as_customer(user_data_in_json):
+    #user_data_in_json           = request.get_json()
     reference_code              = user_data_in_json.get('reference_code')
     merchant_reference_code     = user_data_in_json.get('merchant_reference_code')
     outlet_key                  = user_data_in_json.get('outlet_key')
     
     logger.debug('register_user_as_customer: user_data_in_json=%s', user_data_in_json)
     
     try:
@@ -658,33 +702,165 @@
                                     #'user_details'              : user_details_dict(existing_user_acct),
                                     }
                     
                     response_data.update(user_details_dict(existing_user_acct))
                     
                     logger.debug('register_user_as_customer debug: response_data=%s', response_data)
                     
-                    return create_rest_message(status_code=StatusCode.OK, **response_data)
+                    return create_api_message(status_code=StatusCode.OK, **response_data)
+                    
+                else:
+                    if is_email_used==True:
+                        return create_api_message('Email have been taken', status_code=StatusCode.BAD_REQUEST)
+                    
+                    elif is_mobile_phone_used==True:
+                        return create_api_message('Mobile phone have been taken', status_code=StatusCode.BAD_REQUEST)
+                    else:
+                        return create_api_message('Failed to register customer', status_code=StatusCode.BAD_REQUEST)
+            
+        else:
+            logger.warn('customer registration input is invalid')
+            
+            return create_api_message("Missing register customer input data", status_code=StatusCode.BAD_REQUEST)
+    except:
+        logger.error('Fail to register customer due to %s', get_tracelog())
+        
+        return create_api_message(status_code=StatusCode.BAD_REQUEST)
+
+
+@user_api_bp.route('/register-referred-user-as-customer', methods=['POST'])
+@user_auth_token_required
+@request_json
+def register_referred_user_as_customer(reference_code, user_data_in_json):
+    #user_data_in_json           = request.get_json()
+    #reference_code              = user_data_in_json.get('reference_code')
+    referred_code               = user_data_in_json.get('referred_code')
+    merchant_acct_code          = user_data_in_json.get('merchant_acct_code')
+    
+    logger.debug('register_referred_user_as_customer: user_data_in_json=%s', user_data_in_json)
+    
+    try:
+        if is_not_empty(reference_code):
+            logger.debug('customer registration input is valid')
+            db_client = create_db_client(caller_info="register_referred_user_as_customer")
+            
+            created_customer        = None
+            existing_user_acct      = None
+            is_email_used           = False
+            is_mobile_phone_used    = False
+            merchant_act_key        = None
+            
+            with db_client.context():
+                existing_user_acct  = User.get_by_reference_code(reference_code)
+                if existing_user_acct:
+                    referrer_user_acct      = User.get_by_referral_code(referred_code)
+                    merchant_acct           = MerchantAcct.get_by_account_code(merchant_acct_code)
+                    
+                    referrer_customer_acct  = Customer.get_by_reference_code(referrer_user_acct.reference_code, merchant_acct)
+                    
+                    logger.debug('register_referred_user_as_customer: referrer_customer_acct=%s', referrer_customer_acct)
+                    
+                    if referrer_customer_acct:
+                        outlet                  = referrer_customer_acct.registered_outlet
+                        merchant_act_key        = merchant_acct.key_in_str
+                        outlet_key              = outlet.key_in_str    
+                        
+                        created_customer        = Customer.get_by_reference_code(reference_code, merchant_acct)
+                         
+                        if created_customer is None:
+                            
+                            email           = existing_user_acct.email
+                            mobile_phone    = existing_user_acct.mobile_phone
+                            
+                            logger.debug('email=%s', email)
+                            logger.debug('mobile_phone=%s', mobile_phone)
+                            
+                            checking_customer = Customer.get_by_email(email, merchant_acct=merchant_acct) 
+                            
+                            if checking_customer:
+                                is_email_used = True
+                            else:
+                                if is_not_empty(mobile_phone):
+                                    checking_customer = Customer.get_by_mobile_phone(mobile_phone, merchant_acct=merchant_acct)
+                                    if checking_customer:
+                                        is_mobile_phone_used = True
+                            
+                            logger.debug('is_email_used=%s', is_email_used)
+                            logger.debug('is_mobile_phone_used=%s', is_mobile_phone_used)
+                            
+                            if is_email_used == False and is_mobile_phone_used == False:
+                            
+                                created_customer = __create_referred_user_as_customer(existing_user_acct, merchant_acct, outlet, referrer_customer_acct, referred_code)
+                            
+                                
+                            logger.debug('created_customer=%s', created_customer)
+                        
+                    else:
+                        logger.warn('Customer account not found for referral code=%s', referred_code)
+                
+                if created_customer:
+                    
+                    response_data = {
+                                    'customer_key'              : created_customer.key_in_str,
+                                    'registered_datetime'       : created_customer.registered_datetime.strftime("%d-%m-%Y %H:%M:%S"),
+                                    'merchant_reference_code'   : created_customer.merchant_reference_code,
+                                    'reference_code'            : created_customer.reference_code,
+                                    'merchant_account_key'      : merchant_act_key,
+                                    'company_name'              : merchant_acct.company_name,
+                                    'outlet_key'                : outlet_key,  
+                                    #'user_details'              : user_details_dict(existing_user_acct),
+                                    }
+                    
+                    response_data.update(user_details_dict(existing_user_acct))
+                    
+                    logger.debug('register_user_as_customer debug: response_data=%s', response_data)
+                    
+                    return create_api_message(status_code=StatusCode.OK, **response_data)
                     
                 else:
                     if is_email_used==True:
-                        return create_rest_message('Email have been taken', status_code=StatusCode.BAD_REQUEST)
+                        return create_api_message('Email have been taken', status_code=StatusCode.BAD_REQUEST)
                     
                     elif is_mobile_phone_used==True:
-                        return create_rest_message('Mobile phone have been taken', status_code=StatusCode.BAD_REQUEST)
+                        return create_api_message('Mobile phone have been taken', status_code=StatusCode.BAD_REQUEST)
                     else:
-                        return create_rest_message('Failed to register customer', status_code=StatusCode.BAD_REQUEST)
+                        return create_api_message('Failed to register customer', status_code=StatusCode.BAD_REQUEST)
             
         else:
             logger.warn('customer registration input is invalid')
             
-            return create_rest_message("Missing register customer input data", status_code=StatusCode.BAD_REQUEST)
+            return create_api_message("Missing register customer input data", status_code=StatusCode.BAD_REQUEST)
     except:
         logger.error('Fail to register customer due to %s', get_tracelog())
         
-        return create_rest_message(status_code=StatusCode.BAD_REQUEST)
+        return create_api_message(status_code=StatusCode.BAD_REQUEST)    
+
+@model_transactional(desc="__create_referred_user_as_customer")
+def __create_referred_user_as_customer(user_acct, merchant_acct, referred_outlet, referrer_customer_acct, referrer_code):
+    
+    created_referee_customer = Customer.create_from_user(referred_outlet, user_acct)
+    created_referee_customer.referrer_code = referrer_code
+    created_referee_customer.put()
+    
+    #create_upstream = False
+    create_upstream = True
+    
+    if create_upstream:
+        create_merchant_registered_customer_upstream_for_merchant(created_referee_customer)
+        create_registered_customer_upstream_for_system(created_referee_customer)
+    
+    #trigger referral program reward here
+    giveaway_referral_program_reward(merchant_acct, 
+                                     created_referee_customer, 
+                                     referrer_customer_acct, 
+                                     referred_outlet, 
+                                     create_upstream=create_upstream
+                                     )
+    return created_referee_customer
+    
 
 def user_details_dict(user_acct):
     is_email_verified           = user_acct.is_email_verified
     is_mobile_phone_verified    = user_acct.is_mobile_phone_verified
     
     logger.debug('user_details_dict debug: is_email_verified=%s', is_email_verified)
     logger.debug('user_details_dict debug: is_mobile_phone_verified=%s', is_mobile_phone_verified)
@@ -746,24 +922,25 @@
         
     if is_not_empty(mobile_phone_verified_datetime):
         user_details['mobile_phone_verified_datetime'] = mobile_phone_verified_datetime        
     
     return user_details
     
 @user_api_bp.route('/customer/<reference_code>', methods=['GET'])
-def read_user_customer_acct(reference_code):
+@request_headers
+def read_user_customer_acct(request_headers, reference_code):
     logger.debug('read_user_customer_acct: reference_code=%s', reference_code)
     
     try:
         if is_not_empty(reference_code):
             logger.debug('customer registration input is valid')
             db_client = create_db_client(caller_info="register_user_as_customer")
             
             customer                = None
-            outlet_key              = request.headers.get('x-outlet-key')
+            outlet_key              = request_headers.get('x-outlet-key')
             merchant_acct           = None
             existing_user_acct      = None
             
             logger.debug('outlet_key=%s', outlet_key)
             
             with db_client.context():
                 outlet          = Outlet.fetch(outlet_key)
@@ -791,31 +968,30 @@
                                     #'user_details'              : user_details_dict(existing_user_acct), 
                                     }
                     
                     response_data.update(user_details_dict(existing_user_acct))
                     
                     logger.debug('read_user_customer_acct debug: response_data=%s', response_data)
                     
-                    return create_rest_message(status_code=StatusCode.OK, **response_data)
+                    return create_api_message(status_code=StatusCode.OK, **response_data)
                     
                 else:
-                    return create_rest_message('Customer account not found', status_code=StatusCode.BAD_REQUEST)
+                    return create_api_message('Customer account not found', status_code=StatusCode.BAD_REQUEST)
             
         else:
             logger.warn('customer registration input is invalid')
             
-            return create_rest_message("Missing register customer input data", status_code=StatusCode.BAD_REQUEST)
+            return create_api_message("Missing register customer input data", status_code=StatusCode.BAD_REQUEST)
     except:
         logger.error('Fail to read customer details due to %s', get_tracelog())
         
-        return create_rest_message(status_code=StatusCode.BAD_REQUEST)    
+        return create_api_message(status_code=StatusCode.BAD_REQUEST)    
 
 @user_api_bp.route('/customer/<customer_key>/reward/summary', methods=['GET'])
 @user_auth_token_required
-@elapsed_time_trace(trace_key="read_customer_reward_summary")
 def read_customer_reward_summary(reference_code, customer_key):
     logger.debug('reference_code=%s', reference_code)
     #vouchers_list   = []
     tier_rewards    = []
     
     db_client = create_db_client(caller_info="read_customer_reward_summary")
     with db_client.context():
@@ -845,29 +1021,37 @@
             'entitled_lucky_draw_ticket_summary'    : customer.entitled_lucky_draw_ticket_summary,
             }
     
     return jsonify(result)
     
 @user_api_bp.route('/check-auth-token', methods=['POST'])
 @user_auth_token_required
-def check_auth_token(reference_code):
+@request_headers
+def check_auth_token(reference_code, request_headers):
     
     db_client = create_db_client(caller_info="check_auth_token")
     
+    logger.debug('check_auth_token debug: reference_code=%s', reference_code)
+    logger.debug('check_auth_token debug: request_headers=%s', request_headers)
+    
+    
     with db_client.context():
         user_acct = User.get_by_reference_code(reference_code)
-        user_auth_token     = request.headers.get('x-auth-token')
+        user_auth_token     = request_headers.get('x-auth-token')
+        
+        logger.debug('check_auth_token debug: user_auth_token=%s', user_auth_token)
+        
         
         response_data = {
                         'auth_token'              : user_auth_token,
                         }
         
         response_data.update(user_details_dict(user_acct))
     
-    return create_rest_message(status_code=StatusCode.OK, **response_data)
+    return create_api_message(status_code=StatusCode.OK, **response_data)
 
 
     
 @user_api_bp.route('/<reference_code>', methods=['GET'])
 @user_auth_token_required
 def read_user_acct(reference_code):
     
@@ -890,98 +1074,101 @@
                 #email_vc_expiry_datetime = str(user_acct.email_vc_expiry_datetime)
                 email_vc_expiry_datetime = user_acct.email_vc_expiry_datetime.strftime('%d-%m-%Y %H:%M:%S'),
                 
             if is_mobile_phone_verified == False:
                 #vg_generated_datetime = user_acct.vg_generated_datetime.strftime(user_acct.vg_generated_datetime, '%d/%m/%Y, %H:%M:%S')
                 mobile_phone_vc_expiry_datetime = str(user_acct.mobile_phone_vc_expiry_datetime)    
                 
-            return create_rest_message(status_code=StatusCode.OK, 
+            return create_api_message(status_code=StatusCode.OK, 
                                        reference_code                       = user_acct.reference_code, 
                                        name                                 = user_acct.name, 
                                        email                                = user_acct.email, 
                                        is_email_verified                    = is_email_verified,
                                        is_mobile_phone_verified             = is_mobile_phone_verified,
                                        email_vc_expiry_datetime             = email_vc_expiry_datetime,
                                        mobile_phone_vc_expiry_datetime      = mobile_phone_vc_expiry_datetime,
                                        status                               = user_acct.status,
                                        )
         else:
             logger.debug('user account is not found')
-            return create_rest_message(status_code=StatusCode.BAD_REQUEST)
+            return create_api_message(status_code=StatusCode.BAD_REQUEST)
             
     else:
         logger.warn('verify_user: user verify input is invalid')
-        return create_rest_message(status_code=StatusCode.BAD_REQUEST) 
+        return create_api_message(status_code=StatusCode.BAD_REQUEST) 
     
 @user_api_bp.route('/delete-account-request', methods=['DELETE'])
 @user_auth_token_required
-def delete_user_acct(reference_code):
+@request_values
+def delete_user_acct(reference_code, request_values):
     
     
     db_client = create_db_client(caller_info="delete_user_acct")
     
-    password   = request.args.get('password') or request.form.get('password') or request.json.get('password')
+    #password   = request.args.get('password') or request.form.get('password') or request.json.get('password')
+    password = request_values.get('password')
     
     with db_client.context():
         user_acct = User.get_by_reference_code(reference_code)
     
     if user_acct:
         if user_acct.is_still_lock:
-            return create_rest_message('User account is locked after many trials for security purpose. Please try after an hour.', status_code=StatusCode.BAD_REQUEST)
+            return create_api_message('User account is locked after many trials for security purpose. Please try after an hour.', status_code=StatusCode.BAD_REQUEST)
         else:
             if user_acct.is_valid_password(password):
                 logger.debug('delete_user_acct: found user account by reference_code=%s', reference_code)
                 if user_acct.demo_account==True:
-                    return create_rest_message('Demo account is not allow to delete', status_code=StatusCode.BAD_REQUEST)
+                    return create_api_message('Demo account is not allow to delete', status_code=StatusCode.BAD_REQUEST)
                 else:
                     with db_client.context():
                         user_acct.request_to_delete() 
                     
-                    return create_rest_message(status_code=StatusCode.ACCEPTED,)
+                    return create_api_message(status_code=StatusCode.ACCEPTED,)
             else:
                 with db_client.context():
                     user_acct.add_try_count()
                 
-                return create_rest_message('Password is not match', status_code=StatusCode.BAD_REQUEST)
+                return create_api_message('Password is not match', status_code=StatusCode.BAD_REQUEST)
     
     else:
         logger.debug('user account is not found')
-        return create_rest_message(status_code=StatusCode.BAD_REQUEST)
+        return create_api_message(status_code=StatusCode.BAD_REQUEST)
             
           
     
 @user_api_bp.route('/read-user-new-message-count', methods=['GET'])
 @user_auth_token_required
 def read_user_new_message_count(reference_code):
     logger.info('reference_code=%s', reference_code)
     if is_not_empty(reference_code):
         db_client = create_db_client(caller_info="read_user_new_message_count")
         user_acct = None
         with db_client.context():
             user_acct = User.get_by_reference_code(reference_code)
         
         if user_acct:
-            return create_rest_message(status_code=StatusCode.OK, 
+            return create_api_message(status_code=StatusCode.OK, 
                                        new_message_count = user_acct.new_message_count
                                        )
         else:
             logger.debug('user account is not found')
-            return create_rest_message(status_code=StatusCode.BAD_REQUEST)
+            return create_api_message(status_code=StatusCode.BAD_REQUEST)
             
     else:
         logger.warn('verify_user: user verify input is invalid')
-        return create_rest_message(status_code=StatusCode.BAD_REQUEST)        
+        return create_api_message(status_code=StatusCode.BAD_REQUEST)        
 
 @user_api_bp.route('/joined-brands-list', methods=['GET'])
 @show_request_info
 @user_auth_token_required
-def list_joined_brands(reference_code):
+@request_args
+def list_joined_brands(reference_code, request_args):
     
-    limit           = request.args.get('limit')
-    start_cursor    = request.args.get('start_cursor')
+    limit           = request_args.get('limit')
+    start_cursor    = request_args.get('start_cursor')
     
     logger.debug('limit=%s', limit)
     logger.debug('start_cursor=%s', start_cursor)
     
     if is_not_empty(reference_code):
         db_client = create_db_client(caller_info="list_joined_brands")
         brands_list     = []
@@ -1044,19 +1231,19 @@
                                 }
                   
                 if is_not_empty(next_cursor):
                     result_data['next_cursor'] = next_cursor  
         
         
         
-        return create_rest_message(status_code=StatusCode.OK,
+        return create_api_message(status_code=StatusCode.OK,
                                    **result_data, 
                                    )
     else:
-        return create_rest_message(status_code=StatusCode.BAD_REQUEST) 
+        return create_api_message(status_code=StatusCode.BAD_REQUEST) 
     
 @user_api_bp.route('/all-joined-brands-list', methods=['GET'])
 @user_auth_token_required
 def list_all_joined_brands(reference_code):
     
     
     if is_not_empty(reference_code):
@@ -1088,23 +1275,27 @@
                                      
                 result_data= {
                                 'result'        : brands_list,
                                 'count'         : len(brands_list),
                                 }
                   
         
-        return create_rest_message(status_code=StatusCode.OK,
+        return create_api_message(status_code=StatusCode.OK,
                                    **result_data, 
                                    )
     else:
-        return create_rest_message(status_code=StatusCode.BAD_REQUEST)       
+        return create_api_message(status_code=StatusCode.BAD_REQUEST)       
     
 @user_api_bp.route('/reset-email-vc', methods=['PUT'])
-def reset_email_verification_code():
-    email = request.args.get('email') or request.form.get('email') or request.json.get('email')
+@request_values
+@request_headers
+def reset_email_verification_code(request_values, request_headers):
+    #email = request.args.get('email') or request.form.get('email') or request.json.get('email')
+    email = request_values.get('email')
+    
     
     logger.info('reset_email_verification_code: going to reset email verification code by email=%s', email)
     
     if is_not_empty(email):
         db_client = create_db_client(caller_info="reset_email_verification_code")
         user_acct = None
         
@@ -1135,58 +1326,61 @@
             email_vc_prefix             = random_string(4, is_human_mistake_safe=True)
             
             send_email_verification_code_email(email, email_vc, email_vc_prefix)
             
             logger.info('reset_email_verification_code: email_vc_expiry_datetime=%s', email_vc_expiry_datetime)
             logger.info('reset_email_verification_code: verification code=%s', email_vc)
                 
-            return create_rest_message(status_code=StatusCode.OK, 
+            return create_api_message(status_code=StatusCode.OK, 
                                        #email_vc_expiry_datetime          = str(email_vc_expiry_datetime),
                                        expiry_datetime     = email_vc_expiry_datetime.strftime('%d-%m-%Y %H:%M:%S'),
                                        prefix              = email_vc_prefix, 
                                        code                = email_vc,
                                        
                                        )
         else:
-            reference_code = request.headers.get('x-reference-code')
+            reference_code = request_headers.get('x-reference-code')
             logger.debug('reference_code from header=%s', reference_code)
             logger.debug('reference_code from database=%s', user_acct.reference_code)
             
             if reference_code == user_acct.reference_code:
                 email_vc_expiry_datetime    = _generate_email_expiry_datetime()
                 email_vc                    = random_number(6)
                 
                 if USE_VERIFICATION_REQUEST_ID:
                     email_vc_prefix             = random_string(4, is_human_mistake_safe=True)
                 else:
                     email_vc_prefix             = ''
                 
                 send_email_verification_code_email(email, email_vc, email_vc_prefix)
                 
-                return create_rest_message(status_code=StatusCode.OK, 
+                return create_api_message(status_code=StatusCode.OK, 
                                        #email_vc_expiry_datetime          = str(email_vc_expiry_datetime),
                                        expiry_datetime      = email_vc_expiry_datetime.strftime('%d-%m-%Y %H:%M:%S'),
                                        prefix               = email_vc_prefix,
                                        code                 = email_vc,
                                        )
             else:
-                return create_rest_message('The email have been taken %s' % email, status_code=StatusCode.BAD_REQUEST)
+                return create_api_message('The email have been taken %s' % email, status_code=StatusCode.BAD_REQUEST)
             
     else:
         logger.warn('reset_email_verification_code: reference code is invalid')
-        return create_rest_message(status_code=StatusCode.BAD_REQUEST) 
+        return create_api_message(status_code=StatusCode.BAD_REQUEST) 
 
 def _generate_email_expiry_datetime():
     return datetime.utcnow() + timedelta(minutes=int(os.environ.get('EMAIL_EXPIRY_LENGTH_IN_MINUTE')))
     
 @user_api_bp.route('/reset-mobile-phone-vc', methods=['PUT'])
 @user_auth_token_required
-def reset_mobile_phone_verification_code(reference_code):
-    mobile_phone    = request.args.get('mobile_phone') or request.form.get('mobile_phone') or request.json.get('mobile_phone')
-    send_method     = request.args.get('send_method') or request.form.get('send_method') or request.json.get('send_method')
+@request_values
+def reset_mobile_phone_verification_code(request_values, reference_code):
+    #mobile_phone    = request.args.get('mobile_phone') or request.form.get('mobile_phone') or request.json.get('mobile_phone')
+    #send_method     = request.args.get('send_method') or request.form.get('send_method') or request.json.get('send_method')
+    mobile_phone    = request_values.get('mobile_phone')
+    send_method     = request_values.get('send_method')
 
     logger.debug('mobile_phone=%s', mobile_phone)
     logger.debug('send_method=%s', send_method)
     logger.debug('reference_code=%s', reference_code)
     
     if is_not_empty(mobile_phone):
         db_client                           = create_db_client(caller_info="reset_mobile_phone_verification_code")
@@ -1212,27 +1406,27 @@
                     mobile_phone_vc_prefix             = random_string(4, is_human_mistake_safe=True)
                 else:
                     mobile_phone_vc_prefix = ''
                 
                 try:
                     send_mobile_phone_verification_code(mobile_phone, user_by_mobile_phone.mobile_phone_vc, mobile_phone_vc_prefix, send_method=send_method)
                     
-                    return create_rest_message(status_code=StatusCode.OK, 
+                    return create_api_message(status_code=StatusCode.OK, 
                                                expiry_datetime      = user_by_mobile_phone.mobile_phone_vc_expiry_datetime.strftime('%d-%m-%Y %H:%M:%S'),
                                                code                 = user_by_mobile_phone.mobile_phone_vc,
                                                prefix               = mobile_phone_vc_prefix,
                                                )
                 except:
-                    return create_rest_message(
+                    return create_api_message(
                                                 'Could not send verification code at the moment',
                                                 status_code=StatusCode.BAD_REQUEST,
                                                
                                                )
             else:
-                return create_rest_message(gettext('Mobile phone have been taken'), status_code=StatusCode.BAD_REQUEST)
+                return create_api_message(gettext('Mobile phone have been taken'), status_code=StatusCode.BAD_REQUEST)
         else:
             with db_client.context():
                 user_acct    = User.get_by_reference_code(reference_code)
             
             if user_acct is not None:
                 with db_client.context():
                     user_acct.reset_mobile_phone_vc()
@@ -1245,41 +1439,44 @@
                 logger.debug('reset_mobile_phone_verification_code: mobile_phone_vc_expiry_datetime=%s', user_acct.mobile_phone_vc_expiry_datetime)
                 logger.debug('reset_mobile_phone_verification_code: verification code=%s', user_acct.mobile_phone_vc)    
                 logger.debug('reset_mobile_phone_verification_code: USE_VERIFICATION_REQUEST_ID=%s', USE_VERIFICATION_REQUEST_ID)
                 
                 try:
                     send_mobile_phone_verification_code(mobile_phone, user_acct.mobile_phone_vc, mobile_phone_vc_prefix, send_method=send_method)
                     
-                    return create_rest_message(status_code=StatusCode.OK, 
+                    return create_api_message(status_code=StatusCode.OK, 
                                                expiry_datetime      = user_acct.mobile_phone_vc_expiry_datetime.strftime('%d-%m-%Y %H:%M:%S'),
                                                code                 = user_acct.mobile_phone_vc,
                                                prefix               = mobile_phone_vc_prefix,
                                                
                                                )
                 except:
-                    return create_rest_message(
+                    return create_api_message(
                                                 'Could not send verification code at the moment',
                                                 status_code=StatusCode.BAD_REQUEST,
                                                
                                                )
                     
             else:
-                return create_rest_message(gettext('Invalid input'), status_code=StatusCode.BAD_REQUEST)
+                return create_api_message(gettext('Invalid input'), status_code=StatusCode.BAD_REQUEST)
                 
                 
     else:
         logger.warn('reset_mobile_phone_verification_code: mobile phone is invalid')
-        return create_rest_message(gettext('Missing mobile phone'), status_code=StatusCode.BAD_REQUEST)  
+        return create_api_message(gettext('Missing mobile phone'), status_code=StatusCode.BAD_REQUEST)  
     
 @user_api_bp.route('/change-password', methods=['PUT'])
 @user_auth_token_required
-def change_password(reference_code):
+@request_values
+def change_password(reference_code, request_values):
     
-    existing_password   = request.args.get('existing_password') or request.form.get('existing_password') or request.json.get('existing_password')
-    new_password        = request.args.get('new_password') or request.form.get('new_password') or request.json.get('new_password')
+    #existing_password   = request.args.get('existing_password') or request.form.get('existing_password') or request.json.get('existing_password')
+    #new_password        = request.args.get('new_password') or request.form.get('new_password') or request.json.get('new_password')
+    existing_password   = request_values.get('existing_password')
+    new_password        = request_values.get('new_password')
     
     if is_not_empty(existing_password) and is_not_empty(new_password):
         db_client = create_db_client(caller_info="change_password")
         user_acct = None
         is_existing_password_valid = False
         with db_client.context():
             user_acct = User.get_by_reference_code(reference_code)
@@ -1291,23 +1488,23 @@
             
             with db_client.context():
                 if user_acct.is_valid_password(existing_password):
                     is_existing_password_valid = True
                     user_acct.change_password(new_password)
                 
         if is_existing_password_valid:    
-            return create_rest_message(
+            return create_api_message(
                                     status_code=StatusCode.OK
                                        
                                        )
         else:
-            return create_rest_message('existing password is not valid', status_code=StatusCode.BAD_REQUEST)
+            return create_api_message('existing password is not valid', status_code=StatusCode.BAD_REQUEST)
             
     else:
-        return create_rest_message('Missing password input', status_code=StatusCode.BAD_REQUEST)  
+        return create_api_message('Missing password input', status_code=StatusCode.BAD_REQUEST)  
     
 @user_api_bp.route('/set-password', methods=['PUT'])
 def set_password():
     
     new_password        = request.args.get('new_password') or request.form.get('new_password') or request.json.get('new_password')
     reset_password_token = request.args.get('reset_password_token') or request.form.get('reset_password_token') or request.json.get('reset_password_token')
     
@@ -1326,23 +1523,23 @@
             logger.debug('set_password: found user account by reset_password_token=%s', user_acct)    
             
             
             with db_client.context():
                 user_acct.change_password(new_password)
                 
             
-            return create_rest_message(
+            return create_api_message(
                                     status_code=StatusCode.OK
                                        
                                        )
         else:
-            return create_rest_message('Invalid request to set password', status_code=StatusCode.BAD_REQUEST)
+            return create_api_message('Invalid request to set password', status_code=StatusCode.BAD_REQUEST)
             
     else:
-        return create_rest_message('Missing password input', status_code=StatusCode.BAD_REQUEST)          
+        return create_api_message('Missing password input', status_code=StatusCode.BAD_REQUEST)          
     
 @user_api_bp.route('/request-reset-password-via-email', methods=['POST'])
 def request_reset_password_via_email_post():
     email = request.args.get('email') or request.form.get('email') or request.json.get('email')
     
     logger.debug('reset_password_request_post: going to reset email verification code by email=%s', email)
     
@@ -1363,43 +1560,41 @@
             
             #if is_email_verified:
             with db_client.context():
                 user_acct.reset_password_request()
             
             send_reset_password_request_email(user_acct)
                 
-            return create_rest_message(status_code=StatusCode.OK
+            return create_api_message(status_code=StatusCode.OK
                                        
                                        )
         else:
-            return create_rest_message('Cannot find user by email %s' % email, status_code=StatusCode.BAD_REQUEST)
+            return create_api_message('Cannot find user by email %s' % email, status_code=StatusCode.BAD_REQUEST)
             
     else:
         logger.warn('reset_password_post: email is invalid')
-        return create_rest_message(status_code=StatusCode.BAD_REQUEST) 
+        return create_api_message(status_code=StatusCode.BAD_REQUEST) 
     
 @user_api_bp.route('/request-reset-password-via-mobile-phone', methods=['POST'])
 def request_reset_password_via_mobile_phone_post():
     mobile_phone = request.args.get('mobile_phone') or request.form.get('mobile_phone') or request.json.get('mobile_phone')
     send_method = request.args.get('send_method') or request.form.get('send_method') or request.json.get('send_method')
     
-    logger.debug('request_reset_password_via_mobile_phone_post: going to reset mobile_phone verification code by mobile phone=%s', mobile_phone)
-
-    logger.debug('mobile_phone=%s', mobile_phone)
-    logger.debug('send_method=%s', send_method)
+    logger.info('mobile_phone=%s', mobile_phone)
+    logger.info('send_method=%s', send_method)
     
     if is_not_empty(mobile_phone):
-        db_client                           = create_db_client(caller_info="request_reset_password_via_mobile_phone_post")
+        db_client                   = create_db_client(caller_info="request_reset_password_via_mobile_phone_post")
         
         with db_client.context():
             user_by_mobile_phone    = User.get_by_mobile_phone(mobile_phone)
         
             logger.debug('user_by_mobile_phone=%s', user_by_mobile_phone)
         
-        if user_by_mobile_phone is not None:
+        if user_by_mobile_phone:
             with db_client.context():
                 user_by_mobile_phone.reset_mobile_phone_vc()
                 
                 
                 
             logger.debug('request_reset_password_via_mobile_phone_post debug: mobile_phone_vc_expiry_datetime=%s', user_by_mobile_phone.mobile_phone_vc_expiry_datetime)
             logger.debug('request_reset_password_via_mobile_phone_post debug: verification code=%s', user_by_mobile_phone.mobile_phone_vc)   
@@ -1408,38 +1603,43 @@
                 mobile_phone_vc_prefix             = random_string(4, is_human_mistake_safe=True)
             else:
                 mobile_phone_vc_prefix = ''
             
             try:
                 send_mobile_phone_verification_code(mobile_phone, user_by_mobile_phone.mobile_phone_vc, mobile_phone_vc_prefix, send_method=send_method)
             except:
-                    return create_rest_message(
+                return create_api_message(
                                                 'Could not send verification code at the moment',
                                                 status_code=StatusCode.BAD_REQUEST,
                                                
                                                )
             
             with db_client.context():
                 reset_password_token = '%s-%s' % (mobile_phone_vc_prefix, user_by_mobile_phone.mobile_phone_vc)
                 logger.debug('request_reset_password_via_mobile_phone_post debug: reset_password_token=%s', reset_password_token)
                 user_by_mobile_phone.set_reset_password_token(reset_password_token)
             
-            return create_rest_message(status_code=StatusCode.OK, 
+            return create_api_message(status_code=StatusCode.OK, 
                                        expiry_datetime      = user_by_mobile_phone.mobile_phone_vc_expiry_datetime.strftime('%d-%m-%Y %H:%M:%S'),
                                        code                 = user_by_mobile_phone.mobile_phone_vc,
                                        prefix               = mobile_phone_vc_prefix,
                                        is_invalid_account   = False,
                                        )
         else:
-            return create_rest_message(status_code=StatusCode.OK, is_invalid_account=True,)
+            #return create_api_message(status_code=StatusCode.OK, is_invalid_account=True,)
+            return create_api_message(
+                                    'Could not send verification code at the moment',
+                                    status_code=StatusCode.BAD_REQUEST,
+                                   
+                                   )
                 
                 
     else:
         logger.warn('request_reset_password_via_mobile_phone_post: mobile phone is invalid')
-        return create_rest_message(gettext('Missing mobile phone'), status_code=StatusCode.BAD_REQUEST) 
+        return create_api_message(gettext('Missing mobile phone'), status_code=StatusCode.BAD_REQUEST) 
     
 
 @user_api_bp.route('/outlet-reviews', methods=['POST'])
 @user_auth_token_required
 def outlet_reviews(reference_code):
     logger.debug('---outlet_reviews---')
     logger.debug('outlet_reviews: reference_code=%s', reference_code)
@@ -1456,23 +1656,23 @@
             value_for_money_score   = reviews_data_form.value_for_money_score.data
             
             logger.debug('outlet_reviews: food_score=%s', food_score)
             logger.debug('outlet_reviews: service_score=%s', service_score)
             logger.debug('outlet_reviews: ambience_score=%s', ambience_score)
             logger.debug('outlet_reviews: value_for_money_score=%s', value_for_money_score)
             
-            return create_rest_message(status_code=StatusCode.OK)
+            return create_api_message(status_code=StatusCode.OK)
         
         else:
             logger.warn('outlet_reviews: outlet reviews input is invalid')
             error_message = reviews_data_form.create_rest_return_error_message()
             
-            return create_rest_message(error_message, status_code=StatusCode.BAD_REQUEST)
+            return create_api_message(error_message, status_code=StatusCode.BAD_REQUEST)
     except:
-        return create_rest_message('Failed to process outlet reviews', status_code=StatusCode.BAD_REQUEST)   
+        return create_api_message('Failed to process outlet reviews', status_code=StatusCode.BAD_REQUEST)   
         
 @user_api_bp.route('/voucher/<redeem_code>/remove', methods=['DELETE'])
 @user_auth_token_required
 def remove_user_voucher(reference_code, redeem_code):
     logger.info('reference_code=%s', reference_code)
     logger.info('redeem_code=%s', redeem_code)
         
@@ -1488,21 +1688,21 @@
                 customer_voucher.remove()  
                 customer = customer_voucher.entitled_customer_acct
                 customer.update_after_removed_voucher(customer_voucher)
             else:
                 logger.info('voucher is not found')    
 
         if customer_voucher and customer_voucher.is_removed:        
-            return create_rest_message(status_code=StatusCode.OK)
+            return create_api_message(status_code=StatusCode.OK)
         else:
             logger.info('Invalid voucher redeem code')
-            return create_rest_message('Invalid voucher redeem code', status_code=StatusCode.BAD_REQUEST)
+            return create_api_message('Invalid voucher redeem code', status_code=StatusCode.BAD_REQUEST)
     else:
         logger.info('Missing voucher redeem code')
-        return create_rest_message('Missing voucher redeem code', status_code=StatusCode.BAD_REQUEST)
+        return create_api_message('Missing voucher redeem code', status_code=StatusCode.BAD_REQUEST)
 
 def send_email_verification_code_email(email, verification_code, request_id):
     
     final_verification_code = verification_code
     if is_not_empty(request_id):
         final_verification_code = '%s-%s' % (request_id, verification_code)
         
@@ -1705,52 +1905,52 @@
                 logger.debug('result_data=%s', result_data)
                   
                 if is_not_empty(next_cursor):
                     result_data['next_cursor'] = next_cursor  
         
         
         
-        return create_rest_message(status_code=StatusCode.OK,
+        return create_api_message(status_code=StatusCode.OK,
                                    **result_data, 
                                    )
     else:
-        return create_rest_message(status_code=StatusCode.BAD_REQUEST)          
+        return create_api_message(status_code=StatusCode.BAD_REQUEST)          
     
 
 @user_api_bp.route('/read-user-message', methods=['POST'])
 @user_auth_token_required
 def read_user_message(reference_code):
     logger.info('reference_code=%s', reference_code)
     message_key = request.args.get('message_key') or request.form.get('message_key') or request.json.get('message_key')
     
     if is_not_empty(message_key):
         db_client = create_db_client(caller_info="update_user_message_as_read")
         
         with db_client.context():
             Message.update_read(message_key)
 
-        return create_rest_message(status_code=StatusCode.ACCEPTED,)
+        return create_api_message(status_code=StatusCode.ACCEPTED,)
     else:
-        return create_rest_message(status_code=StatusCode.BAD_REQUEST)
+        return create_api_message(status_code=StatusCode.BAD_REQUEST)
  
 @user_api_bp.route('/delete-user-message', methods=['DELETE'])
 @user_auth_token_required
 def delete_user_message_as_read(reference_code):
     logger.info('reference_code=%s', reference_code)
     message_key = request.args.get('message_key') or request.form.get('message_key') or request.json.get('message_key')
     
     if is_not_empty(message_key):
         db_client = create_db_client(caller_info="delete_user_message_as_read")
         
         with db_client.context():
             Message.update_delete(message_key)
             
-        return create_rest_message(status_code=StatusCode.ACCEPTED,)
+        return create_api_message(status_code=StatusCode.ACCEPTED,)
     else:
-        return create_rest_message(status_code=StatusCode.BAD_REQUEST)
+        return create_api_message(status_code=StatusCode.BAD_REQUEST)
     
 @user_api_bp.route('/update-device-details', methods=['PUT'])
 @user_auth_token_required
 def update_device_details(reference_code):
     platform        = request.args.get('platform') or request.form.get('platform') or request.json.get('platform')
     device_token    = request.args.get('device_token') or request.form.get('device_token') or request.json.get('device_token')
 
@@ -1765,14 +1965,14 @@
             user_acct = User.get_by_reference_code(reference_code)
             
             user_acct.update_device_details(platform, device_token)
             
         
         if user_acct:
             logger.debug('update_device_details: found user account by reference_code=%s', reference_code)
-            return create_rest_message(status_code=StatusCode.ACCEPTED)
+            return create_api_message(status_code=StatusCode.ACCEPTED)
         
         else:
-            return create_rest_message('Invalid user data', status_code=StatusCode.BAD_REQUEST)
+            return create_api_message('Invalid user data', status_code=StatusCode.BAD_REQUEST)
     else:
-        return create_rest_message('Missing required data', status_code=StatusCode.BAD_REQUEST)
+        return create_api_message('Missing required data', status_code=StatusCode.BAD_REQUEST)
```

### Comparing `trex-apis-1.3.8/trexapi/controllers/user_reward_api_routes.py` & `trex-apis-1.4.0/trexapi/controllers/user_reward_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.8/trexapi/controllers/voucher_api_routes.py` & `trex-apis-1.4.0/trexapi/controllers/voucher_api_routes.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,48 +9,47 @@
 from trexlib.utils.log_util import get_tracelog
 from trexmodel.utils.model.model_util import create_db_client
 from datetime import datetime, timedelta
 from trexapi.decorators.api_decorators import auth_token_required,\
     user_auth_token_required, device_is_activated
 from trexlib.utils.string_util import is_not_empty, is_empty
 from trexmodel.models.datastore.customer_models import Customer
-from trexadmin.libs.http import create_rest_message
-from trexadmin.libs.http import StatusCode
+from trexapi.utils.api_helpers import create_api_message, StatusCode
 from trexmodel.models.datastore.merchant_models import Outlet,\
     MerchantUser, MerchantAcct
 from trexapi.forms.reward_api_forms import VoucherRedeemForm, VoucherRemoveForm
 from werkzeug.datastructures import ImmutableMultiDict
 import json
 from trexapi.utils.api_helpers import get_logged_in_api_username
 from trexmodel.models.datastore.voucher_models import MerchantVoucher
 from trexmodel.models.datastore.reward_models import CustomerEntitledVoucher
 
 from trexmodel.models.datastore.redeem_models import CustomerRedemption
 from trexanalytics.bigquery_upstream_data_config import create_merchant_customer_redemption_upstream_for_merchant
 from trexmodel import program_conf
-from trexapi import conf
 from trexmodel.models.datastore.user_models import User
 from flask.json import jsonify
 from trexmodel.models.datastore.model_decorators import model_transactional
 from trexmodel.models.datastore.reward_model_helpers import check_redeem_voucher_is_valid
 from flask_babel import gettext
+from trexlib.libs.flask_wtf.request_wrapper import request_json, request_headers
 
 logger = logging.getLogger('api')
 
 
 voucher_api_bp = Blueprint('voucher_api_bp', __name__,
                                  template_folder='templates',
                                  static_folder='static',
                                  url_prefix='/api/v1/vouchers')
 
 logger = logging.getLogger('api')
 
 @voucher_api_bp.route('/ping', methods=['GET'])
 def ping():
-    return create_rest_message('Pong', status_code=StatusCode.OK)
+    return create_api_message('Pong', status_code=StatusCode.OK)
 
 @voucher_api_bp.route('/voucher/<redeem_code>/details', methods=['POST','GET'])
 @auth_token_required
 @device_is_activated
 def read_voucher(redeem_code):
     if is_not_empty(redeem_code):
         voucher_details = None
@@ -81,30 +80,32 @@
                                                                     'is_revert'         : customer_voucher.is_reverted,
                                                                 }
                                                             ],
                                     }
                 
         
         if voucher_details is None:
-            return create_rest_message('Invalid voucher code', status_code=StatusCode.BAD_REQUEST)
+            return create_api_message('Invalid voucher code', status_code=StatusCode.BAD_REQUEST)
         else:
-            #return create_rest_message(voucher_details=voucher_details, status_code=StatusCode.OK)
+            #return create_api_message(voucher_details=voucher_details, status_code=StatusCode.OK)
             
             logging.debug('voucher_details=%s', voucher_details)
             
             return jsonify(voucher_details)
     else:
-        return create_rest_message('Voucher code is required', status_code=StatusCode.BAD_REQUEST) 
+        return create_api_message('Voucher code is required', status_code=StatusCode.BAD_REQUEST) 
     
 @voucher_api_bp.route('/voucher/redeem', methods=['post'])
 @auth_token_required
 @device_is_activated
-def redeem_voucher():
+@request_json
+@request_headers
+def redeem_voucher(redeem_voucher_data_in_json, request_headers):
     
-    redeem_voucher_data_in_json   = request.get_json()
+    #redeem_voucher_data_in_json   = request.get_json()
     
     redeem_voucher_form = VoucherRedeemForm(ImmutableMultiDict(redeem_voucher_data_in_json))
     
     if redeem_voucher_form.validate():
     
         redeem_code         = redeem_voucher_data_in_json.get('redeem_code')
         invoice_id          = redeem_voucher_form.invoice_id.data
@@ -119,26 +120,26 @@
         
         if redeem_code:
             redeem_code_list = redeem_code.split(',')
             
             
             db_client = create_db_client(caller_info="redeem_voucher")
             with db_client.context():
-                redeemed_by_outlet      = Outlet.fetch(request.headers.get('x-outlet-key'))
-                merchant_acct           = MerchantAcct.fetch(request.headers.get('x-acct-id'))
+                redeemed_by_outlet      = Outlet.fetch(request_headers.get('x-outlet-key'))
+                merchant_acct           = MerchantAcct.fetch(request_headers.get('x-acct-id'))
             
             redeem_datetime             = redeem_voucher_form.redeem_datetime.data
             merchant_username           = get_logged_in_api_username()
             
             
             if redeem_datetime:
                 redeem_datetime_in_gmt      = redeem_datetime - timedelta(hours=merchant_acct.gmt_hour)
                 now                         = datetime.utcnow()
                 if redeem_datetime_in_gmt > now:
-                    return create_rest_message('Redeem datetime cannot be future', status_code=StatusCode.BAD_REQUEST)
+                    return create_api_message('Redeem datetime cannot be future', status_code=StatusCode.BAD_REQUEST)
             
             
             
             to_redeem_voucher_keys_list                             = []
             customer                                                = None
             customer_vouchers_list                                  = []
             
@@ -151,23 +152,23 @@
                     customer_vouchers_list.append(customer_voucher)
                     to_redeem_voucher_keys_list.append(customer_voucher.key_in_str)
                     if customer is None:
                         customer = customer_voucher.entitled_customer_entity
                     else:
                         checking_customer = customer_voucher.entitled_customer_entity
                         if checking_customer.key_in_str!=customer.key_in_str:
-                            return create_rest_message(gettext('Voucher must from same customer'), status_code=StatusCode.BAD_REQUEST)
+                            return create_api_message(gettext('Voucher must from same customer'), status_code=StatusCode.BAD_REQUEST)
                             
                 
             try:
                 with db_client.context():
                     check_redeem_voucher_is_valid(customer, customer_vouchers_list, redeem_datetime=redeem_datetime)
             except Exception as error:
                 logger.error('Failed due to %s', get_tracelog())
-                return create_rest_message(str(error), status_code=StatusCode.BAD_REQUEST)
+                return create_api_message(str(error), status_code=StatusCode.BAD_REQUEST)
             
             @model_transactional(desc='redeem_voucher')
             def __start_transaction_for_redeem_voucher():
                 
                 customer_redemption = CustomerRedemption.create(customer, program_conf.REWARD_FORMAT_VOUCHER , 
                                                           redeemed_outlet               = redeemed_by_outlet,
                                                           redeemed_amount               = 1,            
@@ -188,32 +189,34 @@
                         logger.debug('customer_redemption=%s', customer_redemption)
                         
         
                     if customer_redemption:
                         create_merchant_customer_redemption_upstream_for_merchant(customer_redemption, streamed_datetime=redeemed_datetime)
                 
                 if customer_redemption:        
-                    return create_rest_message(transaction_id = customer_redemption.transaction_id, status_code=StatusCode.OK)
+                    return create_api_message(transaction_id = customer_redemption.transaction_id, status_code=StatusCode.OK)
                 else:
-                    return create_rest_message("Failed to redeem voucher", status_code=StatusCode.BAD_REQUEST)
+                    return create_api_message("Failed to redeem voucher", status_code=StatusCode.BAD_REQUEST)
             else:
-                return create_rest_message('Voucher redeem code is required', status_code=StatusCode.BAD_REQUEST)
+                return create_api_message('Voucher redeem code is required', status_code=StatusCode.BAD_REQUEST)
                 
     else:
         logger.warn('redeem voucher data input is invalid')
         error_message = redeem_voucher_form.create_rest_return_error_message()
             
-        return create_rest_message(error_message, status_code=StatusCode.BAD_REQUEST)
+        return create_api_message(error_message, status_code=StatusCode.BAD_REQUEST)
         
 @voucher_api_bp.route('/voucher/<redeem_code>/remove', methods=['DELETE'])
 @auth_token_required
 @device_is_activated
-def remove_voucher(redeem_code):
+@request_json
+@request_headers
+def remove_voucher(remove_voucher_data_in_json, request_headers, redeem_code):
     
-    remove_voucher_data_in_json   = request.get_json()
+    #remove_voucher_data_in_json   = request.get_json()
     
     remove_voucher_form = VoucherRemoveForm(ImmutableMultiDict(remove_voucher_data_in_json))
     if remove_voucher_form.validate():
     
         #redeem_code         = remove_voucher_data_in_json.get('redeem_code')
         remarks             = remove_voucher_form.remarks.data
         remove_datetime     = remove_voucher_form.remove_datetime.data
@@ -235,47 +238,47 @@
             remove_datetime_in_gmt      = remove_voucher_form.remove_datetime.data
             
             to_remove_voucher_keys_list                         = []
             found_not_valid_redeem_code_list                    = []
             removed_by                                          = None    
             
             with db_client.context():
-                merchant_acct           = MerchantAcct.fetch(request.headers.get('x-acct-id'))
+                merchant_acct           = MerchantAcct.fetch(request_headers.get('x-acct-id'))
                 merchant_username       = get_logged_in_api_username()
                 removed_by              = MerchantUser.get_by_username(merchant_username)
                 
                 
                 for redeem_code in redeem_code_list:
                     customer_voucher    = CustomerEntitledVoucher.get_by_redeem_code(redeem_code)
                     if customer_voucher:
                         to_remove_voucher_keys_list.append(customer_voucher.key_in_str)
                     else:
                         found_not_valid_redeem_code_list.append(redeem_code)
             
             if found_not_valid_redeem_code_list:
-                return create_rest_message("Voucher ({redeem_codes_list}) is not valid".format(redeem_codes_list=",".join(found_not_valid_redeem_code_list)), 
+                return create_api_message("Voucher ({redeem_codes_list}) is not valid".format(redeem_codes_list=",".join(found_not_valid_redeem_code_list)), 
                                            status_code=StatusCode.BAD_REQUEST)            
             else:
                 if to_remove_voucher_keys_list:
                     with db_client.context():
                         if to_remove_voucher_keys_list:
                             for voucher_key in to_remove_voucher_keys_list:
                                 customer_voucher = CustomerEntitledVoucher.fetch(voucher_key)
                                 customer_voucher.remove(removed_by, removed_datetime=remove_datetime_in_gmt)
                             
-                    return create_rest_message(status_code=StatusCode.OK)
+                    return create_api_message(status_code=StatusCode.OK)
                     
                 else:
-                    return create_rest_message('Voucher redeem code is required', status_code=StatusCode.BAD_REQUEST)
+                    return create_api_message('Voucher redeem code is required', status_code=StatusCode.BAD_REQUEST)
     
     else:
         logger.warn('redeem voucher data input is invalid')
         error_message = remove_voucher_form.create_rest_return_error_message()
             
-        return create_rest_message(error_message, status_code=StatusCode.BAD_REQUEST)        
+        return create_api_message(error_message, status_code=StatusCode.BAD_REQUEST)        
              
 
 @voucher_api_bp.route('/entitled/<reference_code>', methods=['GET'])
 def list_entitled_voucher(reference_code):
     
     logger.debug('list_entitled_voucher: going to list entitled voucher by reference code=%s', reference_code)
     
@@ -299,24 +302,25 @@
                                        
         return {
                 'vouchers': voucher_list,
             }
             
     else:
         logger.warn('reset_password_post: email is invalid')
-        return create_rest_message(status_code=StatusCode.BAD_REQUEST)       
+        return create_api_message(status_code=StatusCode.BAD_REQUEST)       
     
 @voucher_api_bp.route('/voucher/<redeem_code>/remove-by-user', methods=['DELETE'])
 @user_auth_token_required
-def remove_user_voucher(reference_code, redeem_code):
+@request_headers
+def remove_user_voucher(reference_code, request_headers, redeem_code):
     logger.info('reference_code=%s', reference_code)
     logger.info('redeem_code=%s', redeem_code)
     
     if is_not_empty(redeem_code):
-        reference_code = request.headers.get('x-reference-code')
+        reference_code = request_headers.get('x-reference-code')
         logger.debug('reference_code=%s', reference_code)
         db_client = create_db_client(caller_info="remove_user_voucher")
         with db_client.context():
             customer_voucher    = CustomerEntitledVoucher.get_by_redeem_code(redeem_code)
             
             if customer_voucher: 
                 
@@ -324,13 +328,13 @@
                 customer = customer_voucher.entitled_customer_acct
                 customer.update_after_removed_voucher(customer_voucher)
             else:
                 logger.info('voucher is not found')    
                
         if customer_voucher and customer_voucher.is_removed:        
         
-            return create_rest_message(status_code=StatusCode.OK)
+            return create_api_message(status_code=StatusCode.OK)
         else:
             logger.info('Invalid voucher redeem code')
-            return create_rest_message('Invalid voucher redeem code', status_code=StatusCode.BAD_REQUEST)
+            return create_api_message('Invalid voucher redeem code', status_code=StatusCode.BAD_REQUEST)
     else:
-        return create_rest_message('Missing voucher redeem code', status_code=StatusCode.BAD_REQUEST)
+        return create_api_message('Missing voucher redeem code', status_code=StatusCode.BAD_REQUEST)
```

### Comparing `trex-apis-1.3.8/trexapi/decorators/api_decorators.py` & `trex-apis-1.4.0/trexapi/decorators/api_decorators.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.8/trexapi/forms/customer_api_forms.py` & `trex-apis-1.4.0/trexapi/forms/customer_api_forms.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,16 +63,16 @@
 class CustomerDetailsNewForm(CustomerDetailsBaseForm):
     
     
     password                      = StringField(gettext('Password'), validators=[
                                         validators.InputRequired(gettext('Password is required')),
                                         
                                         ]
-                                        )    
-
+                                        )
+    
 class CustomerDetailsUpdateForm(CustomerDetailsBaseForm):
     
     password                      = StringField(gettext('Password'), validators=[
                                         validators.Optional(),
                                         ]
                                         )
```

### Comparing `trex-apis-1.3.8/trexapi/forms/reward_api_forms.py` & `trex-apis-1.4.0/trexapi/forms/reward_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.8/trexapi/forms/sales_api_forms.py` & `trex-apis-1.4.0/trexapi/forms/sales_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.8/trexapi/forms/user_api_forms.py` & `trex-apis-1.4.0/trexapi/forms/user_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.8/trexapi/libs/flask_auth_wrapper.py` & `trex-apis-1.4.0/trexapi/libs/flask_auth_wrapper.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.8/trexapi/utils/api_helpers.py` & `trex-apis-1.4.0/trexapi/utils/api_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 @author: jacklok
 '''
 from flask import request
 import logging
 from trexlib.utils.crypto_util import decrypt_json
 from datetime import datetime, timedelta
-from trexapi import conf as api_conf
+from trexconf import conf as api_conf
 from trexlib.utils.crypto_util import encrypt_json
 import six
 from six import string_types
 
 logger = logging.getLogger('helper')
```

### Comparing `trex-apis-1.3.8/trexapi/utils/reward_transaction_helper.py` & `trex-apis-1.4.0/trexapi/utils/reward_transaction_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 '''
 Created on 20 Apr 2021
 
 @author: jacklok
 '''
 from trexlib.utils.google.cloud_tasks_util import create_task
-from trexadmin import conf
+from trexconf import conf
 from trexlib.conf import CHECK_CUSTOMER_ENTITLE_REWARD_TASK_URL, SYSTEM_TASK_SERVICE_CREDENTIAL_PATH, SYSTEM_TASK_GCLOUD_PROJECT_ID, SYSTEM_TASK_GCLOUD_LOCATION, SYSTEM_TASK_SERVICE_ACCOUNT_EMAIL  
 import logging
-from trexadmin.libs.app.reward_program.reward_program_factory import RewardProgramFactory
+from trexprogram.reward_program.reward_program_factory import RewardProgramFactory
 from trexadmin.controllers.system.system_routes import get_currency_config
 from trexmodel.models.datastore.reward_models import CustomerPointReward,\
     CustomerStampReward, CustomerEntitledVoucher, VoucherRewardDetailsForUpstreamData,\
     CustomerEntitledTierRewardSummary
 from datetime import datetime
 from trexmodel import program_conf
 from trexmodel.models.datastore.customer_model_helpers import update_customer_entiteld_voucher_summary_after_reverted_voucher,\
@@ -20,23 +20,21 @@
     update_customer_entiteld_voucher_summary_with_customer_new_voucher,\
     update_prepaid_summary_with_reverted_prepaid,\
     update_reward_summary_with_reverted_reward
 from trexanalytics.bigquery_upstream_data_config import create_merchant_customer_reward_reverted_upstream_for_merchant,\
     create_merchant_customer_transaction_upstream_for_merchant,\
     create_merchant_customer_redemption_upstream_for_merchant,\
     create_merchant_customer_prepaid_upstream_for_merchant,\
-    create_merchant_customer_prepaid_reverted_upstream_for_merchant,\
-    create_merchant_customer_redemption_reverted_upstream_for_merchant,\
-    create_merchant_sales_transaction_upstream_for_merchant
+    create_merchant_customer_redemption_reverted_upstream_for_merchant
 from trexmodel.models.datastore.membership_models import MerchantTierMembership
 from trexmodel.models.datastore.transaction_models import CustomerTransaction,\
     SalesTransaction
 from trexmodel.models.datastore.model_decorators import model_transactional
 from trexmodel.models.datastore.prepaid_models import CustomerPrepaidReward
-from trexadmin.libs.app.reward_program.reward_program_base import EntitledVoucherSummary
+from trexprogram.reward_program.reward_program_base import EntitledVoucherSummary
 from trexmodel.models.datastore.customer_models import Customer,\
     CustomerMembership, CustomerTierMembership
 from trexmodel.models.datastore.redeem_models import CustomerRedemption
 from trexlib.utils.string_util import is_not_empty
 from trexlib.utils.log_util import get_tracelog
 from trexmodel.models.datastore.lucky_draw_models import LuckyDrawTicket
 from trexmodel.models.datastore.message_model_helper import create_transaction_message,\
```

