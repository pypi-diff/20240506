# Comparing `tmp/mns_common-1.0.7.9.tar.gz` & `tmp/mns_common-1.0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mns_common-1.0.7.9.tar", last modified: Sat May  4 09:56:12 2024, max compression
+gzip compressed data, was "mns_common-1.0.8.0.tar", last modified: Mon May  6 13:55:27 2024, max compression
```

## Comparing `mns_common-1.0.7.9.tar` & `mns_common-1.0.8.0.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 09:56:12.501230 mns_common-1.0.7.9/
--rw-rw-rw-   0        0        0       59 2024-05-04 09:56:12.500233 mns_common-1.0.7.9/PKG-INFO
--rw-rw-rw-   0        0        0     1354 2023-12-14 15:25:31.000000 mns_common-1.0.7.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 09:56:12.459343 mns_common-1.0.7.9/mns_common/
--rw-rw-rw-   0        0        0      163 2024-01-10 10:52:31.000000 mns_common-1.0.7.9/mns_common/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 09:56:12.462334 mns_common-1.0.7.9/mns_common/api/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.0.7.9/mns_common/api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 09:56:12.465326 mns_common-1.0.7.9/mns_common/api/akshare/
--rw-rw-rw-   0        0        0      165 2023-12-15 04:25:30.000000 mns_common-1.0.7.9/mns_common/api/akshare/__init__.py
--rw-rw-rw-   0        0        0     5057 2023-12-22 09:50:37.000000 mns_common-1.0.7.9/mns_common/api/akshare/k_line_api.py
--rw-rw-rw-   0        0        0     5999 2024-01-05 08:16:46.000000 mns_common-1.0.7.9/mns_common/api/akshare/stock_bid_ask_api.py
--rw-rw-rw-   0        0        0     2245 2023-12-16 12:13:22.000000 mns_common-1.0.7.9/mns_common/api/akshare/stock_dt_pool.py
--rw-rw-rw-   0        0        0     2038 2023-12-16 13:25:10.000000 mns_common-1.0.7.9/mns_common/api/akshare/stock_zb_pool.py
--rw-rw-rw-   0        0        0     1929 2023-12-16 12:13:22.000000 mns_common-1.0.7.9/mns_common/api/akshare/stock_zt_pool_api.py
--rw-rw-rw-   0        0        0     4108 2023-12-16 12:13:22.000000 mns_common-1.0.7.9/mns_common/api/akshare/yjyg_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-04 09:56:12.468318 mns_common-1.0.7.9/mns_common/api/em/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.0.7.9/mns_common/api/em/__init__.py
--rw-rw-rw-   0        0        0     8352 2024-05-04 09:55:55.000000 mns_common-1.0.7.9/mns_common/api/em/east_money_stock_api.py
--rw-rw-rw-   0        0        0     5504 2023-12-22 09:50:37.000000 mns_common-1.0.7.9/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py
--rw-rw-rw-   0        0        0    14960 2024-05-01 15:03:02.000000 mns_common-1.0.7.9/mns_common/api/em/east_money_stock_v2_api.py
--rw-rw-rw-   0        0        0     8285 2023-12-22 09:50:37.000000 mns_common-1.0.7.9/mns_common/api/em/em_concept_index_api.py
-drwxrwxrwx   0        0        0        0 2024-05-04 09:56:12.468318 mns_common-1.0.7.9/mns_common/api/kpl/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.9/mns_common/api/kpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 09:56:12.469316 mns_common-1.0.7.9/mns_common/api/kpl/common/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.7.9/mns_common/api/kpl/common/__init__.py
--rw-rw-rw-   0        0        0     6536 2024-04-24 09:08:22.000000 mns_common-1.0.7.9/mns_common/api/kpl/common/kpl_common_api.py
-drwxrwxrwx   0        0        0        0 2024-05-04 09:56:12.470313 mns_common-1.0.7.9/mns_common/api/kpl/concept/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.7.9/mns_common/api/kpl/concept/__init__.py
--rw-rw-rw-   0        0        0      607 2023-12-16 12:13:22.000000 mns_common-1.0.7.9/mns_common/api/kpl/concept/kpl_concept_api.py
-drwxrwxrwx   0        0        0        0 2024-05-04 09:56:12.471310 mns_common-1.0.7.9/mns_common/api/kpl/constant/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.7.9/mns_common/api/kpl/constant/__init__.py
--rw-rw-rw-   0        0        0      669 2023-12-22 09:50:37.000000 mns_common-1.0.7.9/mns_common/api/kpl/constant/kpl_constant.py
-drwxrwxrwx   0        0        0        0 2024-05-04 09:56:12.472307 mns_common-1.0.7.9/mns_common/api/kpl/industry/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.7.9/mns_common/api/kpl/industry/__init__.py
--rw-rw-rw-   0        0        0      565 2023-12-16 12:13:22.000000 mns_common-1.0.7.9/mns_common/api/kpl/industry/kpl_industry_api.py
-drwxrwxrwx   0        0        0        0 2024-05-04 09:56:12.473305 mns_common-1.0.7.9/mns_common/api/kpl/selection/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.7.9/mns_common/api/kpl/selection/__init__.py
--rw-rw-rw-   0        0        0     1777 2024-01-11 08:08:46.000000 mns_common-1.0.7.9/mns_common/api/kpl/selection/kpl_selection_plate_api.py
-drwxrwxrwx   0        0        0        0 2024-05-04 09:56:12.475299 mns_common-1.0.7.9/mns_common/api/kpl/symbol/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.7.9/mns_common/api/kpl/symbol/__init__.py
--rw-rw-rw-   0        0        0     4792 2024-03-22 08:55:03.000000 mns_common-1.0.7.9/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py
--rw-rw-rw-   0        0        0     1625 2024-03-22 08:56:47.000000 mns_common-1.0.7.9/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py
--rw-rw-rw-   0        0        0     4210 2024-04-21 02:03:32.000000 mns_common-1.0.7.9/mns_common/api/kpl/symbol/symbol_his_quotes_api.py
-drwxrwxrwx   0        0        0        0 2024-05-04 09:56:12.476297 mns_common-1.0.7.9/mns_common/api/msg/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.7.9/mns_common/api/msg/__init__.py
--rw-rw-rw-   0        0        0     1421 2024-02-03 04:57:25.000000 mns_common-1.0.7.9/mns_common/api/msg/push_msg_api.py
-drwxrwxrwx   0        0        0        0 2024-05-04 09:56:12.478292 mns_common-1.0.7.9/mns_common/api/ths/
--rw-rw-rw-   0        0        0      163 2023-12-15 03:59:01.000000 mns_common-1.0.7.9/mns_common/api/ths/__init__.py
--rw-rw-rw-   0        0        0     3614 2023-12-22 09:50:37.000000 mns_common-1.0.7.9/mns_common/api/ths/ths_big_deal_api.py
--rw-rw-rw-   0        0        0    39935 2024-04-12 00:08:48.000000 mns_common-1.0.7.9/mns_common/api/ths/ths_stock_api.py
--rw-rw-rw-   0        0        0     6784 2024-01-12 12:47:02.000000 mns_common-1.0.7.9/mns_common/api/ths/ths_stock_zt_pool_api.py
-drwxrwxrwx   0        0        0        0 2024-05-04 09:56:12.479289 mns_common-1.0.7.9/mns_common/component/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:38:42.000000 mns_common-1.0.7.9/mns_common/component/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 09:56:12.480287 mns_common-1.0.7.9/mns_common/component/cache/
--rw-rw-rw-   0        0        0      163 2024-04-28 07:37:23.000000 mns_common-1.0.7.9/mns_common/component/cache/__init__.py
--rw-rw-rw-   0        0        0      809 2024-04-28 07:38:03.000000 mns_common-1.0.7.9/mns_common/component/cache/cache_service.py
-drwxrwxrwx   0        0        0        0 2024-05-04 09:56:12.481284 mns_common-1.0.7.9/mns_common/component/classify/
--rw-rw-rw-   0        0        0      163 2024-01-09 08:35:24.000000 mns_common-1.0.7.9/mns_common/component/classify/__init__.py
--rw-rw-rw-   0        0        0      522 2024-01-09 09:22:06.000000 mns_common-1.0.7.9/mns_common/component/classify/classify_constant.py
--rw-rw-rw-   0        0        0     3880 2024-01-09 08:35:24.000000 mns_common-1.0.7.9/mns_common/component/classify/symbol_classify_api.py
--rw-rw-rw-   0        0        0     4790 2024-01-13 08:29:24.000000 mns_common-1.0.7.9/mns_common/component/common_service_fun_api.py
-drwxrwxrwx   0        0        0        0 2024-05-04 09:56:12.482282 mns_common-1.0.7.9/mns_common/component/company/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.9/mns_common/component/company/__init__.py
--rw-rw-rw-   0        0        0     6987 2023-12-17 11:37:16.000000 mns_common-1.0.7.9/mns_common/component/company/company_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-04 09:56:12.484275 mns_common-1.0.7.9/mns_common/component/concept/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.9/mns_common/component/concept/__init__.py
--rw-rw-rw-   0        0        0     2626 2024-04-23 08:59:18.000000 mns_common-1.0.7.9/mns_common/component/concept/kpl_concept_common_service_api.py
--rw-rw-rw-   0        0        0     9637 2024-04-30 09:46:26.000000 mns_common-1.0.7.9/mns_common/component/concept/ths_concept_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-04 09:56:12.485273 mns_common-1.0.7.9/mns_common/component/data/
--rw-rw-rw-   0        0        0      163 2024-04-28 07:37:23.000000 mns_common-1.0.7.9/mns_common/component/data/__init__.py
--rw-rw-rw-   0        0        0     4757 2023-12-17 11:40:38.000000 mns_common-1.0.7.9/mns_common/component/data/data_init_api.py
-drwxrwxrwx   0        0        0        0 2024-05-04 09:56:12.486270 mns_common-1.0.7.9/mns_common/component/industry/
--rw-rw-rw-   0        0        0      163 2024-01-13 08:34:39.000000 mns_common-1.0.7.9/mns_common/component/industry/__init__.py
--rw-rw-rw-   0        0        0     3252 2024-01-13 08:57:34.000000 mns_common-1.0.7.9/mns_common/component/industry/ths_industry_index_api.py
-drwxrwxrwx   0        0        0        0 2024-05-04 09:56:12.486270 mns_common-1.0.7.9/mns_common/component/k_line/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.9/mns_common/component/k_line/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 09:56:12.487266 mns_common-1.0.7.9/mns_common/component/k_line/clean/
--rw-rw-rw-   0        0        0      163 2024-01-09 09:22:06.000000 mns_common-1.0.7.9/mns_common/component/k_line/clean/__init__.py
--rw-rw-rw-   0        0        0      248 2024-01-09 09:22:06.000000 mns_common-1.0.7.9/mns_common/component/k_line/clean/k_line_param.py
--rw-rw-rw-   0        0        0    12593 2024-01-09 10:28:47.000000 mns_common-1.0.7.9/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py
-drwxrwxrwx   0        0        0        0 2024-05-04 09:56:12.489261 mns_common-1.0.7.9/mns_common/component/k_line/common/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:41:45.000000 mns_common-1.0.7.9/mns_common/component/k_line/common/__init__.py
--rw-rw-rw-   0        0        0     4449 2023-12-29 04:25:17.000000 mns_common-1.0.7.9/mns_common/component/k_line/common/k_line_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-04 09:56:12.490260 mns_common-1.0.7.9/mns_common/component/k_line/patterns/
--rw-rw-rw-   0        0        0      163 2023-12-22 07:50:10.000000 mns_common-1.0.7.9/mns_common/component/k_line/patterns/__init__.py
--rw-rw-rw-   0        0        0     1809 2023-12-22 08:25:35.000000 mns_common-1.0.7.9/mns_common/component/k_line/patterns/k_line_patterns_service_api.py
--rw-rw-rw-   0        0        0      509 2023-12-22 09:49:23.000000 mns_common-1.0.7.9/mns_common/component/k_line/patterns/pattern_Enum.py
-drwxrwxrwx   0        0        0        0 2024-05-04 09:56:12.491257 mns_common-1.0.7.9/mns_common/component/real_time/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.9/mns_common/component/real_time/__init__.py
--rw-rw-rw-   0        0        0     1378 2023-12-16 12:13:22.000000 mns_common-1.0.7.9/mns_common/component/real_time/real_time_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-04 09:56:12.492254 mns_common-1.0.7.9/mns_common/component/trade/
--rw-rw-rw-   0        0        0      163 2024-04-27 12:44:35.000000 mns_common-1.0.7.9/mns_common/component/trade/__init__.py
--rw-rw-rw-   0        0        0     3084 2024-04-28 13:27:31.000000 mns_common-1.0.7.9/mns_common/component/trade/trade_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-04 09:56:12.493251 mns_common-1.0.7.9/mns_common/component/trade_date/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.9/mns_common/component/trade_date/__init__.py
--rw-rw-rw-   0        0        0     2776 2023-12-28 13:35:59.000000 mns_common-1.0.7.9/mns_common/component/trade_date/trade_date_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-04 09:56:12.494248 mns_common-1.0.7.9/mns_common/component/zt/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.7.9/mns_common/component/zt/__init__.py
--rw-rw-rw-   0        0        0     7794 2024-01-13 09:14:41.000000 mns_common-1.0.7.9/mns_common/component/zt/zt_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-04 09:56:12.496243 mns_common-1.0.7.9/mns_common/constant/
--rw-rw-rw-   0        0        0      163 2023-12-17 08:25:43.000000 mns_common-1.0.7.9/mns_common/constant/__init__.py
--rw-rw-rw-   0        0        0     1567 2024-05-03 14:48:19.000000 mns_common-1.0.7.9/mns_common/constant/db_name_constant.py
--rw-rw-rw-   0        0        0     4507 2024-01-25 14:21:07.000000 mns_common-1.0.7.9/mns_common/constant/kpl_selection_no_choose_constant.py
--rw-rw-rw-   0        0        0      347 2024-05-01 15:03:02.000000 mns_common-1.0.7.9/mns_common/constant/self_choose_constant.py
--rw-rw-rw-   0        0        0    12240 2024-03-11 15:08:57.000000 mns_common-1.0.7.9/mns_common/constant/ths_concept_no_choose_constant.py
-drwxrwxrwx   0        0        0        0 2024-05-04 09:56:12.497240 mns_common-1.0.7.9/mns_common/db/
--rw-rw-rw-   0        0        0    10816 2024-04-24 14:49:25.000000 mns_common-1.0.7.9/mns_common/db/MongodbUtil.py
--rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.0.7.9/mns_common/db/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 09:56:12.499235 mns_common-1.0.7.9/mns_common/utils/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.0.7.9/mns_common/utils/__init__.py
--rw-rw-rw-   0        0        0      352 2023-12-15 04:16:28.000000 mns_common-1.0.7.9/mns_common/utils/async_fun.py
--rw-rw-rw-   0        0        0     1316 2023-12-22 08:25:35.000000 mns_common-1.0.7.9/mns_common/utils/data_frame_util.py
--rw-rw-rw-   0        0        0     7379 2023-12-21 03:38:02.000000 mns_common-1.0.7.9/mns_common/utils/date_handle_util.py
--rw-rw-rw-   0        0        0      451 2023-12-15 04:16:28.000000 mns_common-1.0.7.9/mns_common/utils/ip_util.py
-drwxrwxrwx   0        0        0        0 2024-05-04 09:56:12.500233 mns_common-1.0.7.9/mns_common.egg-info/
--rw-rw-rw-   0        0        0       59 2024-05-04 09:56:12.000000 mns_common-1.0.7.9/mns_common.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3663 2024-05-04 09:56:12.000000 mns_common-1.0.7.9/mns_common.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 09:56:12.000000 mns_common-1.0.7.9/mns_common.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-04 09:56:12.000000 mns_common-1.0.7.9/mns_common.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-04 09:56:12.501230 mns_common-1.0.7.9/setup.cfg
--rw-rw-rw-   0        0        0      466 2024-05-04 09:55:55.000000 mns_common-1.0.7.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:55:27.447262 mns_common-1.0.8.0/
+-rw-rw-rw-   0        0        0       59 2024-05-06 13:55:27.447262 mns_common-1.0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1354 2023-12-14 15:25:31.000000 mns_common-1.0.8.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 13:55:27.401385 mns_common-1.0.8.0/mns_common/
+-rw-rw-rw-   0        0        0      163 2024-01-10 10:52:31.000000 mns_common-1.0.8.0/mns_common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:55:27.403380 mns_common-1.0.8.0/mns_common/api/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.0.8.0/mns_common/api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:55:27.406372 mns_common-1.0.8.0/mns_common/api/akshare/
+-rw-rw-rw-   0        0        0      165 2023-12-15 04:25:30.000000 mns_common-1.0.8.0/mns_common/api/akshare/__init__.py
+-rw-rw-rw-   0        0        0     5057 2023-12-22 09:50:37.000000 mns_common-1.0.8.0/mns_common/api/akshare/k_line_api.py
+-rw-rw-rw-   0        0        0     5999 2024-01-05 08:16:46.000000 mns_common-1.0.8.0/mns_common/api/akshare/stock_bid_ask_api.py
+-rw-rw-rw-   0        0        0     2245 2023-12-16 12:13:22.000000 mns_common-1.0.8.0/mns_common/api/akshare/stock_dt_pool.py
+-rw-rw-rw-   0        0        0     2038 2023-12-16 13:25:10.000000 mns_common-1.0.8.0/mns_common/api/akshare/stock_zb_pool.py
+-rw-rw-rw-   0        0        0     1929 2023-12-16 12:13:22.000000 mns_common-1.0.8.0/mns_common/api/akshare/stock_zt_pool_api.py
+-rw-rw-rw-   0        0        0     4108 2023-12-16 12:13:22.000000 mns_common-1.0.8.0/mns_common/api/akshare/yjyg_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:55:27.409364 mns_common-1.0.8.0/mns_common/api/em/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.0.8.0/mns_common/api/em/__init__.py
+-rw-rw-rw-   0        0        0     8352 2024-05-04 09:55:55.000000 mns_common-1.0.8.0/mns_common/api/em/east_money_stock_api.py
+-rw-rw-rw-   0        0        0     5504 2023-12-22 09:50:37.000000 mns_common-1.0.8.0/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py
+-rw-rw-rw-   0        0        0    14960 2024-05-01 15:03:02.000000 mns_common-1.0.8.0/mns_common/api/em/east_money_stock_v2_api.py
+-rw-rw-rw-   0        0        0     8285 2023-12-22 09:50:37.000000 mns_common-1.0.8.0/mns_common/api/em/em_concept_index_api.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:55:27.410361 mns_common-1.0.8.0/mns_common/api/kpl/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.8.0/mns_common/api/kpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:55:27.410361 mns_common-1.0.8.0/mns_common/api/kpl/common/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.8.0/mns_common/api/kpl/common/__init__.py
+-rw-rw-rw-   0        0        0     6536 2024-04-24 09:08:22.000000 mns_common-1.0.8.0/mns_common/api/kpl/common/kpl_common_api.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:55:27.411358 mns_common-1.0.8.0/mns_common/api/kpl/concept/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.8.0/mns_common/api/kpl/concept/__init__.py
+-rw-rw-rw-   0        0        0      607 2023-12-16 12:13:22.000000 mns_common-1.0.8.0/mns_common/api/kpl/concept/kpl_concept_api.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:55:27.412356 mns_common-1.0.8.0/mns_common/api/kpl/constant/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.8.0/mns_common/api/kpl/constant/__init__.py
+-rw-rw-rw-   0        0        0      669 2023-12-22 09:50:37.000000 mns_common-1.0.8.0/mns_common/api/kpl/constant/kpl_constant.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:55:27.413353 mns_common-1.0.8.0/mns_common/api/kpl/industry/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.8.0/mns_common/api/kpl/industry/__init__.py
+-rw-rw-rw-   0        0        0      565 2023-12-16 12:13:22.000000 mns_common-1.0.8.0/mns_common/api/kpl/industry/kpl_industry_api.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:55:27.414351 mns_common-1.0.8.0/mns_common/api/kpl/selection/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.8.0/mns_common/api/kpl/selection/__init__.py
+-rw-rw-rw-   0        0        0     1926 2024-05-06 13:55:26.000000 mns_common-1.0.8.0/mns_common/api/kpl/selection/kpl_selection_plate_api.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:55:27.416345 mns_common-1.0.8.0/mns_common/api/kpl/symbol/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.8.0/mns_common/api/kpl/symbol/__init__.py
+-rw-rw-rw-   0        0        0     4792 2024-03-22 08:55:03.000000 mns_common-1.0.8.0/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py
+-rw-rw-rw-   0        0        0     1625 2024-03-22 08:56:47.000000 mns_common-1.0.8.0/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py
+-rw-rw-rw-   0        0        0     4210 2024-04-21 02:03:32.000000 mns_common-1.0.8.0/mns_common/api/kpl/symbol/symbol_his_quotes_api.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:55:27.417343 mns_common-1.0.8.0/mns_common/api/msg/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.8.0/mns_common/api/msg/__init__.py
+-rw-rw-rw-   0        0        0     1421 2024-02-03 04:57:25.000000 mns_common-1.0.8.0/mns_common/api/msg/push_msg_api.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:55:27.419337 mns_common-1.0.8.0/mns_common/api/ths/
+-rw-rw-rw-   0        0        0      163 2023-12-15 03:59:01.000000 mns_common-1.0.8.0/mns_common/api/ths/__init__.py
+-rw-rw-rw-   0        0        0     3614 2023-12-22 09:50:37.000000 mns_common-1.0.8.0/mns_common/api/ths/ths_big_deal_api.py
+-rw-rw-rw-   0        0        0    39935 2024-04-12 00:08:48.000000 mns_common-1.0.8.0/mns_common/api/ths/ths_stock_api.py
+-rw-rw-rw-   0        0        0     6784 2024-01-12 12:47:02.000000 mns_common-1.0.8.0/mns_common/api/ths/ths_stock_zt_pool_api.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:55:27.420335 mns_common-1.0.8.0/mns_common/component/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:38:42.000000 mns_common-1.0.8.0/mns_common/component/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:55:27.421332 mns_common-1.0.8.0/mns_common/component/cache/
+-rw-rw-rw-   0        0        0      163 2024-04-28 07:37:23.000000 mns_common-1.0.8.0/mns_common/component/cache/__init__.py
+-rw-rw-rw-   0        0        0      809 2024-04-28 07:38:03.000000 mns_common-1.0.8.0/mns_common/component/cache/cache_service.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:55:27.422329 mns_common-1.0.8.0/mns_common/component/classify/
+-rw-rw-rw-   0        0        0      163 2024-01-09 08:35:24.000000 mns_common-1.0.8.0/mns_common/component/classify/__init__.py
+-rw-rw-rw-   0        0        0      522 2024-01-09 09:22:06.000000 mns_common-1.0.8.0/mns_common/component/classify/classify_constant.py
+-rw-rw-rw-   0        0        0     3880 2024-01-09 08:35:24.000000 mns_common-1.0.8.0/mns_common/component/classify/symbol_classify_api.py
+-rw-rw-rw-   0        0        0     4790 2024-01-13 08:29:24.000000 mns_common-1.0.8.0/mns_common/component/common_service_fun_api.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:55:27.423326 mns_common-1.0.8.0/mns_common/component/company/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.8.0/mns_common/component/company/__init__.py
+-rw-rw-rw-   0        0        0     6987 2023-12-17 11:37:16.000000 mns_common-1.0.8.0/mns_common/component/company/company_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:55:27.424324 mns_common-1.0.8.0/mns_common/component/concept/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.8.0/mns_common/component/concept/__init__.py
+-rw-rw-rw-   0        0        0     2626 2024-05-06 13:49:59.000000 mns_common-1.0.8.0/mns_common/component/concept/kpl_concept_common_service_api.py
+-rw-rw-rw-   0        0        0     9637 2024-04-30 09:46:26.000000 mns_common-1.0.8.0/mns_common/component/concept/ths_concept_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:55:27.425321 mns_common-1.0.8.0/mns_common/component/data/
+-rw-rw-rw-   0        0        0      163 2024-04-28 07:37:23.000000 mns_common-1.0.8.0/mns_common/component/data/__init__.py
+-rw-rw-rw-   0        0        0     4757 2023-12-17 11:40:38.000000 mns_common-1.0.8.0/mns_common/component/data/data_init_api.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:55:27.426318 mns_common-1.0.8.0/mns_common/component/industry/
+-rw-rw-rw-   0        0        0      163 2024-01-13 08:34:39.000000 mns_common-1.0.8.0/mns_common/component/industry/__init__.py
+-rw-rw-rw-   0        0        0     3252 2024-01-13 08:57:34.000000 mns_common-1.0.8.0/mns_common/component/industry/ths_industry_index_api.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:55:27.426318 mns_common-1.0.8.0/mns_common/component/k_line/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.8.0/mns_common/component/k_line/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:55:27.428313 mns_common-1.0.8.0/mns_common/component/k_line/clean/
+-rw-rw-rw-   0        0        0      163 2024-01-09 09:22:06.000000 mns_common-1.0.8.0/mns_common/component/k_line/clean/__init__.py
+-rw-rw-rw-   0        0        0      248 2024-01-09 09:22:06.000000 mns_common-1.0.8.0/mns_common/component/k_line/clean/k_line_param.py
+-rw-rw-rw-   0        0        0    12593 2024-01-09 10:28:47.000000 mns_common-1.0.8.0/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:55:27.429310 mns_common-1.0.8.0/mns_common/component/k_line/common/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:41:45.000000 mns_common-1.0.8.0/mns_common/component/k_line/common/__init__.py
+-rw-rw-rw-   0        0        0     4449 2023-12-29 04:25:17.000000 mns_common-1.0.8.0/mns_common/component/k_line/common/k_line_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:55:27.430308 mns_common-1.0.8.0/mns_common/component/k_line/patterns/
+-rw-rw-rw-   0        0        0      163 2023-12-22 07:50:10.000000 mns_common-1.0.8.0/mns_common/component/k_line/patterns/__init__.py
+-rw-rw-rw-   0        0        0     1809 2023-12-22 08:25:35.000000 mns_common-1.0.8.0/mns_common/component/k_line/patterns/k_line_patterns_service_api.py
+-rw-rw-rw-   0        0        0      509 2023-12-22 09:49:23.000000 mns_common-1.0.8.0/mns_common/component/k_line/patterns/pattern_Enum.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:55:27.431305 mns_common-1.0.8.0/mns_common/component/real_time/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.8.0/mns_common/component/real_time/__init__.py
+-rw-rw-rw-   0        0        0     1378 2023-12-16 12:13:22.000000 mns_common-1.0.8.0/mns_common/component/real_time/real_time_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:55:27.432302 mns_common-1.0.8.0/mns_common/component/trade/
+-rw-rw-rw-   0        0        0      163 2024-04-27 12:44:35.000000 mns_common-1.0.8.0/mns_common/component/trade/__init__.py
+-rw-rw-rw-   0        0        0     3084 2024-04-28 13:27:31.000000 mns_common-1.0.8.0/mns_common/component/trade/trade_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:55:27.439288 mns_common-1.0.8.0/mns_common/component/trade_date/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.8.0/mns_common/component/trade_date/__init__.py
+-rw-rw-rw-   0        0        0     2776 2023-12-28 13:35:59.000000 mns_common-1.0.8.0/mns_common/component/trade_date/trade_date_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:55:27.440281 mns_common-1.0.8.0/mns_common/component/zt/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.8.0/mns_common/component/zt/__init__.py
+-rw-rw-rw-   0        0        0     7794 2024-01-13 09:14:41.000000 mns_common-1.0.8.0/mns_common/component/zt/zt_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:55:27.443273 mns_common-1.0.8.0/mns_common/constant/
+-rw-rw-rw-   0        0        0      163 2023-12-17 08:25:43.000000 mns_common-1.0.8.0/mns_common/constant/__init__.py
+-rw-rw-rw-   0        0        0     1567 2024-05-03 14:48:19.000000 mns_common-1.0.8.0/mns_common/constant/db_name_constant.py
+-rw-rw-rw-   0        0        0     4507 2024-01-25 14:21:07.000000 mns_common-1.0.8.0/mns_common/constant/kpl_selection_no_choose_constant.py
+-rw-rw-rw-   0        0        0      347 2024-05-01 15:03:02.000000 mns_common-1.0.8.0/mns_common/constant/self_choose_constant.py
+-rw-rw-rw-   0        0        0    12240 2024-03-11 15:08:57.000000 mns_common-1.0.8.0/mns_common/constant/ths_concept_no_choose_constant.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:55:27.444270 mns_common-1.0.8.0/mns_common/db/
+-rw-rw-rw-   0        0        0    10816 2024-04-24 14:49:25.000000 mns_common-1.0.8.0/mns_common/db/MongodbUtil.py
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.0.8.0/mns_common/db/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:55:27.446265 mns_common-1.0.8.0/mns_common/utils/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.0.8.0/mns_common/utils/__init__.py
+-rw-rw-rw-   0        0        0      352 2023-12-15 04:16:28.000000 mns_common-1.0.8.0/mns_common/utils/async_fun.py
+-rw-rw-rw-   0        0        0     1316 2023-12-22 08:25:35.000000 mns_common-1.0.8.0/mns_common/utils/data_frame_util.py
+-rw-rw-rw-   0        0        0     7379 2023-12-21 03:38:02.000000 mns_common-1.0.8.0/mns_common/utils/date_handle_util.py
+-rw-rw-rw-   0        0        0      451 2023-12-15 04:16:28.000000 mns_common-1.0.8.0/mns_common/utils/ip_util.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:55:27.447262 mns_common-1.0.8.0/mns_common.egg-info/
+-rw-rw-rw-   0        0        0       59 2024-05-06 13:55:27.000000 mns_common-1.0.8.0/mns_common.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3663 2024-05-06 13:55:27.000000 mns_common-1.0.8.0/mns_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 13:55:27.000000 mns_common-1.0.8.0/mns_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-06 13:55:27.000000 mns_common-1.0.8.0/mns_common.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 13:55:27.447262 mns_common-1.0.8.0/setup.cfg
+-rw-rw-rw-   0        0        0      466 2024-05-06 13:55:26.000000 mns_common-1.0.8.0/setup.py
```

### Comparing `mns_common-1.0.7.9/README.md` & `mns_common-1.0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/api/akshare/k_line_api.py` & `mns_common-1.0.8.0/mns_common/api/akshare/k_line_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/api/akshare/stock_bid_ask_api.py` & `mns_common-1.0.8.0/mns_common/api/akshare/stock_bid_ask_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/api/akshare/stock_dt_pool.py` & `mns_common-1.0.8.0/mns_common/api/akshare/stock_dt_pool.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/api/akshare/stock_zb_pool.py` & `mns_common-1.0.8.0/mns_common/api/akshare/stock_zb_pool.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/api/akshare/stock_zt_pool_api.py` & `mns_common-1.0.8.0/mns_common/api/akshare/stock_zt_pool_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/api/akshare/yjyg_sync_api.py` & `mns_common-1.0.8.0/mns_common/api/akshare/yjyg_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/api/em/east_money_stock_api.py` & `mns_common-1.0.8.0/mns_common/api/em/east_money_stock_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py` & `mns_common-1.0.8.0/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/api/em/east_money_stock_v2_api.py` & `mns_common-1.0.8.0/mns_common/api/em/east_money_stock_v2_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/api/em/em_concept_index_api.py` & `mns_common-1.0.8.0/mns_common/api/em/em_concept_index_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/api/kpl/common/kpl_common_api.py` & `mns_common-1.0.8.0/mns_common/api/kpl/common/kpl_common_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/api/kpl/concept/kpl_concept_api.py` & `mns_common-1.0.8.0/mns_common/api/kpl/concept/kpl_concept_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/api/kpl/constant/kpl_constant.py` & `mns_common-1.0.8.0/mns_common/api/kpl/constant/kpl_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/api/kpl/industry/kpl_industry_api.py` & `mns_common-1.0.8.0/mns_common/api/kpl/industry/kpl_industry_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/api/kpl/selection/kpl_selection_plate_api.py` & `mns_common-1.0.8.0/mns_common/api/kpl/selection/kpl_selection_plate_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 import sys
 import os
 import requests
 import pandas as pd
 import mns_common.utils.data_frame_util as data_frame_util
 import mns_common.api.kpl.common.kpl_common_api as kpl_common_api
+from loguru import logger
 
 file_path = os.path.abspath(__file__)
 end = file_path.index('mns') + 14
 project_path = file_path[0:end]
 sys.path.append(project_path)
 
 
 # 精选板块指数
 def best_choose():
-    return kpl_common_api.get_plate_index(kpl_common_api.BEST_CHOOSE)
+    try:
+        return kpl_common_api.get_plate_index(kpl_common_api.BEST_CHOOSE)
+    except Exception as e:
+        logger.error("获取开盘啦指数异常:{}", e)
+        return None
 
 
 # 精选股票组成
 # Order 排序参数
 # st 分页最大数量
 # index 股票排名index
 def best_choose_stock(plate_code):
```

### Comparing `mns_common-1.0.7.9/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py` & `mns_common-1.0.8.0/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py` & `mns_common-1.0.8.0/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/api/kpl/symbol/symbol_his_quotes_api.py` & `mns_common-1.0.8.0/mns_common/api/kpl/symbol/symbol_his_quotes_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/api/msg/push_msg_api.py` & `mns_common-1.0.8.0/mns_common/api/msg/push_msg_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/api/ths/ths_big_deal_api.py` & `mns_common-1.0.8.0/mns_common/api/ths/ths_big_deal_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/api/ths/ths_stock_api.py` & `mns_common-1.0.8.0/mns_common/api/ths/ths_stock_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/api/ths/ths_stock_zt_pool_api.py` & `mns_common-1.0.8.0/mns_common/api/ths/ths_stock_zt_pool_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/component/cache/cache_service.py` & `mns_common-1.0.8.0/mns_common/component/cache/cache_service.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/component/classify/classify_constant.py` & `mns_common-1.0.8.0/mns_common/component/classify/classify_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/component/classify/symbol_classify_api.py` & `mns_common-1.0.8.0/mns_common/component/classify/symbol_classify_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/component/common_service_fun_api.py` & `mns_common-1.0.8.0/mns_common/component/common_service_fun_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/component/company/company_common_service_api.py` & `mns_common-1.0.8.0/mns_common/component/company/company_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/component/concept/kpl_concept_common_service_api.py` & `mns_common-1.0.8.0/mns_common/component/concept/kpl_concept_common_service_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # 获取单个股票所有概念数据
 @lru_cache(maxsize=None)
 def get_symbol_all_kpl_concept(symbol):
     query = {'symbol': symbol}
     return mongodb_util.find_query_data(db_name_constant.KPL_BEST_CHOOSE_INDEX_DETAIL, query)
 
 
-# 获取有效同花顺概念代码
+# 获取所有开盘啦概念列表
 @lru_cache(maxsize=None)
 def get_kpl_all_concept():
     query = {}
     kpl_best_choose_index = mongodb_util.find_query_data(db_name_constant.KPL_BEST_CHOOSE_INDEX, query)
     return kpl_best_choose_index
```

### Comparing `mns_common-1.0.7.9/mns_common/component/concept/ths_concept_common_service_api.py` & `mns_common-1.0.8.0/mns_common/component/concept/ths_concept_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/component/data/data_init_api.py` & `mns_common-1.0.8.0/mns_common/component/data/data_init_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/component/industry/ths_industry_index_api.py` & `mns_common-1.0.8.0/mns_common/component/industry/ths_industry_index_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py` & `mns_common-1.0.8.0/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/component/k_line/common/k_line_common_service_api.py` & `mns_common-1.0.8.0/mns_common/component/k_line/common/k_line_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/component/k_line/patterns/k_line_patterns_service_api.py` & `mns_common-1.0.8.0/mns_common/component/k_line/patterns/k_line_patterns_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/component/real_time/real_time_common_service_api.py` & `mns_common-1.0.8.0/mns_common/component/real_time/real_time_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/component/trade/trade_service_api.py` & `mns_common-1.0.8.0/mns_common/component/trade/trade_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/component/trade_date/trade_date_common_service_api.py` & `mns_common-1.0.8.0/mns_common/component/trade_date/trade_date_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/component/zt/zt_common_service_api.py` & `mns_common-1.0.8.0/mns_common/component/zt/zt_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/constant/db_name_constant.py` & `mns_common-1.0.8.0/mns_common/constant/db_name_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/constant/kpl_selection_no_choose_constant.py` & `mns_common-1.0.8.0/mns_common/constant/kpl_selection_no_choose_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/constant/ths_concept_no_choose_constant.py` & `mns_common-1.0.8.0/mns_common/constant/ths_concept_no_choose_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/db/MongodbUtil.py` & `mns_common-1.0.8.0/mns_common/db/MongodbUtil.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/utils/data_frame_util.py` & `mns_common-1.0.8.0/mns_common/utils/data_frame_util.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common/utils/date_handle_util.py` & `mns_common-1.0.8.0/mns_common/utils/date_handle_util.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.7.9/mns_common.egg-info/SOURCES.txt` & `mns_common-1.0.8.0/mns_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*
