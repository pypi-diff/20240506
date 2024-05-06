# Comparing `tmp/adata-2.0.1b0.tar.gz` & `tmp/adata-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adata-2.0.1b0.tar", last modified: Wed Apr 17 10:56:33 2024, max compression
+gzip compressed data, was "adata-2.1.0.tar", last modified: Mon May  6 10:07:38 2024, max compression
```

## Comparing `adata-2.0.1b0.tar` & `adata-2.1.0.tar`

### file list

```diff
@@ -1,137 +1,141 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.239185 adata-2.0.1b0/
--rw-rw-rw-   0        0        0    11558 2023-04-07 05:48:39.000000 adata-2.0.1b0/LICENSE
--rw-rw-rw-   0        0        0      126 2023-10-23 06:31:33.000000 adata-2.0.1b0/MANIFEST.in
--rw-rw-rw-   0        0        0    21039 2024-04-17 10:56:33.239185 adata-2.0.1b0/PKG-INFO
--rw-rw-rw-   0        0        0    20328 2024-04-17 10:27:23.000000 adata-2.0.1b0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.129518 adata-2.0.1b0/adata/
--rw-rw-rw-   0        0        0     1189 2023-10-10 02:59:10.000000 adata-2.0.1b0/adata/__init__.py
--rw-rw-rw-   0        0        0      737 2024-04-17 10:56:21.000000 adata-2.0.1b0/adata/__version__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.135520 adata-2.0.1b0/adata/bond/
--rw-rw-rw-   0        0        0      261 2023-06-05 11:07:12.000000 adata-2.0.1b0/adata/bond/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.137521 adata-2.0.1b0/adata/bond/cache/
--rw-rw-rw-   0        0        0      103 2023-08-18 09:30:57.000000 adata-2.0.1b0/adata/bond/cache/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.139521 adata-2.0.1b0/adata/bond/info/
--rw-rw-rw-   0        0        0      261 2023-10-10 02:59:10.000000 adata-2.0.1b0/adata/bond/info/__init__.py
--rw-rw-rw-   0        0        0     2200 2023-05-31 08:21:01.000000 adata-2.0.1b0/adata/bond/info/bond_code.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.141522 adata-2.0.1b0/adata/bond/market/
--rw-rw-rw-   0        0        0      104 2023-05-31 08:12:06.000000 adata-2.0.1b0/adata/bond/market/__init__.py
--rw-rw-rw-   0        0        0      203 2023-04-07 05:48:39.000000 adata-2.0.1b0/adata/bond/market/bond_market.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.142522 adata-2.0.1b0/adata/common/
--rw-rw-rw-   0        0        0      150 2023-04-07 05:48:39.000000 adata-2.0.1b0/adata/common/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.145523 adata-2.0.1b0/adata/common/base/
--rw-rw-rw-   0        0        0      133 2023-06-05 03:44:57.000000 adata-2.0.1b0/adata/common/base/__init__.py
--rw-rw-rw-   0        0        0      195 2023-08-14 05:47:34.000000 adata-2.0.1b0/adata/common/base/base_req.py
--rw-rw-rw-   0        0        0     3015 2023-08-18 09:30:57.000000 adata-2.0.1b0/adata/common/base/base_ths.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.148523 adata-2.0.1b0/adata/common/exception/
--rw-rw-rw-   0        0        0       97 2023-07-10 08:15:13.000000 adata-2.0.1b0/adata/common/exception/__init__.py
--rw-rw-rw-   0        0        0      379 2023-08-01 09:58:42.000000 adata-2.0.1b0/adata/common/exception/exception_msg.py
--rw-rw-rw-   0        0        0      350 2023-08-14 06:04:13.000000 adata-2.0.1b0/adata/common/exception/handler.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.154524 adata-2.0.1b0/adata/common/headers/
--rw-rw-rw-   0        0        0     6407 2023-07-10 08:15:13.000000 adata-2.0.1b0/adata/common/headers/__init__.py
--rw-rw-rw-   0        0        0     5772 2023-04-07 05:48:39.000000 adata-2.0.1b0/adata/common/headers/baidu_headers.py
--rw-rw-rw-   0        0        0      571 2023-08-14 05:47:34.000000 adata-2.0.1b0/adata/common/headers/east_headers.py
--rw-rw-rw-   0        0        0      602 2023-04-18 11:18:06.000000 adata-2.0.1b0/adata/common/headers/sina_headers.py
--rw-rw-rw-   0        0        0     3085 2023-08-08 04:51:00.000000 adata-2.0.1b0/adata/common/headers/ths_headers.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.158525 adata-2.0.1b0/adata/common/js/
--rw-rw-rw-   0        0        0       99 2023-05-05 10:05:38.000000 adata-2.0.1b0/adata/common/js/__init__.py
--rw-rw-rw-   0        0        0    15792 2023-08-01 09:31:40.000000 adata-2.0.1b0/adata/common/js/hexin.js
--rw-rw-rw-   0        0        0    39849 2023-06-28 03:35:45.000000 adata-2.0.1b0/adata/common/js/ths.js
-drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.163526 adata-2.0.1b0/adata/common/utils/
--rw-rw-rw-   0        0        0      190 2023-07-10 08:15:13.000000 adata-2.0.1b0/adata/common/utils/__init__.py
--rw-rw-rw-   0        0        0      501 2023-12-04 11:20:28.000000 adata-2.0.1b0/adata/common/utils/code_utils.py
--rw-rw-rw-   0        0        0      877 2023-10-10 02:59:10.000000 adata-2.0.1b0/adata/common/utils/cookie.py
--rw-rw-rw-   0        0        0     3046 2023-04-07 05:48:39.000000 adata-2.0.1b0/adata/common/utils/snowflake.py
--rw-rw-rw-   0        0        0     2891 2023-08-07 03:04:02.000000 adata-2.0.1b0/adata/common/utils/sunrequests.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.164527 adata-2.0.1b0/adata/fund/
--rw-rw-rw-   0        0        0      327 2024-04-17 10:25:02.000000 adata-2.0.1b0/adata/fund/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.165527 adata-2.0.1b0/adata/fund/cache/
--rw-rw-rw-   0        0        0      103 2023-06-02 06:05:35.000000 adata-2.0.1b0/adata/fund/cache/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.167527 adata-2.0.1b0/adata/fund/info/
--rw-rw-rw-   0        0        0      260 2023-10-10 02:59:10.000000 adata-2.0.1b0/adata/fund/info/__init__.py
--rw-rw-rw-   0        0        0     5247 2023-08-01 10:31:22.000000 adata-2.0.1b0/adata/fund/info/fund_info.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.171529 adata-2.0.1b0/adata/fund/market/
--rw-rw-rw-   0        0        0      379 2024-04-17 10:25:02.000000 adata-2.0.1b0/adata/fund/market/__init__.py
--rw-rw-rw-   0        0        0     2416 2024-04-17 10:44:44.000000 adata-2.0.1b0/adata/fund/market/etf_market.py
--rw-rw-rw-   0        0        0      654 2024-04-17 10:45:50.000000 adata-2.0.1b0/adata/fund/market/etf_market_template.py
--rw-rw-rw-   0        0        0     7990 2024-04-17 10:45:50.000000 adata-2.0.1b0/adata/fund/market/etf_market_ths.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.172528 adata-2.0.1b0/adata/message/
--rw-rw-rw-   0        0        0      103 2023-04-07 05:48:39.000000 adata-2.0.1b0/adata/message/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.176529 adata-2.0.1b0/adata/sentiment/
--rw-rw-rw-   0        0        0      466 2023-08-01 04:36:50.000000 adata-2.0.1b0/adata/sentiment/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.177530 adata-2.0.1b0/adata/sentiment/cache/
--rw-rw-rw-   0        0        0      103 2023-08-18 09:30:57.000000 adata-2.0.1b0/adata/sentiment/cache/__init__.py
--rw-rw-rw-   0        0        0     9633 2023-08-01 04:08:30.000000 adata-2.0.1b0/adata/sentiment/north_flow.py
--rw-rw-rw-   0        0        0     3741 2023-08-18 09:30:57.000000 adata-2.0.1b0/adata/sentiment/securities_margin.py
--rw-rw-rw-   0        0        0     4271 2023-08-08 04:51:00.000000 adata-2.0.1b0/adata/sentiment/stock_lifting.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.178530 adata-2.0.1b0/adata/stock/
--rw-rw-rw-   0        0        0      420 2023-10-10 02:59:10.000000 adata-2.0.1b0/adata/stock/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.181530 adata-2.0.1b0/adata/stock/cache/
--rw-rw-rw-   0        0        0      267 2023-10-18 11:49:59.000000 adata-2.0.1b0/adata/stock/cache/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.207178 adata-2.0.1b0/adata/stock/cache/calendar/
--rw-rw-rw-   0        0        0       34 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2004.csv
--rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2005.csv
--rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2006.csv
--rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2007.csv
--rw-rw-rw-   0        0        0     5890 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2008.csv
--rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2009.csv
--rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2010.csv
--rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2011.csv
--rw-rw-rw-   0        0        0     5890 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2012.csv
--rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2013.csv
--rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2014.csv
--rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2015.csv
--rw-rw-rw-   0        0        0     5890 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2016.csv
--rw-rw-rw-   0        0        0     5858 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2017.csv
--rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2018.csv
--rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2019.csv
--rw-rw-rw-   0        0        0     5890 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2020.csv
--rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2021.csv
--rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2022.csv
--rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2023.csv
--rw-rw-rw-   0        0        0     5888 2023-12-29 03:33:12.000000 adata-2.0.1b0/adata/stock/cache/calendar/2024.csv
--rw-rw-rw-   0        0        0      428 2023-12-11 07:21:42.000000 adata-2.0.1b0/adata/stock/cache/calendar/__init__.py
--rw-rw-rw-   0        0        0   174847 2023-10-18 12:45:02.000000 adata-2.0.1b0/adata/stock/cache/code.csv
--rw-rw-rw-   0        0        0     8752 2023-06-02 06:45:42.000000 adata-2.0.1b0/adata/stock/cache/index_code_rel_ths.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.210179 adata-2.0.1b0/adata/stock/index/
--rw-rw-rw-   0        0        0      267 2023-06-02 03:44:46.000000 adata-2.0.1b0/adata/stock/index/__init__.py
--rw-rw-rw-   0        0        0      207 2023-06-02 03:44:46.000000 adata-2.0.1b0/adata/stock/index/cal_index.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.214180 adata-2.0.1b0/adata/stock/info/
--rw-rw-rw-   0        0        0      501 2023-10-10 02:59:10.000000 adata-2.0.1b0/adata/stock/info/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.220181 adata-2.0.1b0/adata/stock/info/concept/
--rw-rw-rw-   0        0        0       86 2023-08-07 03:04:02.000000 adata-2.0.1b0/adata/stock/info/concept/__init__.py
--rw-rw-rw-   0        0        0      485 2023-08-07 03:04:02.000000 adata-2.0.1b0/adata/stock/info/concept/stock_concept.py
--rw-rw-rw-   0        0        0     5595 2024-02-26 03:31:53.000000 adata-2.0.1b0/adata/stock/info/concept/stock_concept_east.py
--rw-rw-rw-   0        0        0      463 2023-12-04 11:54:33.000000 adata-2.0.1b0/adata/stock/info/concept/stock_concept_template.py
--rw-rw-rw-   0        0        0    15126 2023-12-29 03:33:12.000000 adata-2.0.1b0/adata/stock/info/concept/stock_concept_ths.py
--rw-rw-rw-   0        0        0     5770 2023-10-18 12:46:30.000000 adata-2.0.1b0/adata/stock/info/stock_code.py
--rw-rw-rw-   0        0        0    10715 2023-10-18 04:49:44.000000 adata-2.0.1b0/adata/stock/info/stock_index.py
--rw-rw-rw-   0        0        0     2321 2023-08-08 04:46:57.000000 adata-2.0.1b0/adata/stock/info/trade_calendar.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.222181 adata-2.0.1b0/adata/stock/market/
--rw-rw-rw-   0        0        0      550 2023-10-10 02:59:10.000000 adata-2.0.1b0/adata/stock/market/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.226183 adata-2.0.1b0/adata/stock/market/concepth_market/
--rw-rw-rw-   0        0        0      385 2023-08-07 03:32:53.000000 adata-2.0.1b0/adata/stock/market/concepth_market/__init__.py
--rw-rw-rw-   0        0        0     7028 2023-08-08 11:22:09.000000 adata-2.0.1b0/adata/stock/market/concepth_market/concept_market_east.py
--rw-rw-rw-   0        0        0      695 2023-08-08 11:05:55.000000 adata-2.0.1b0/adata/stock/market/concepth_market/concept_market_template.py
--rw-rw-rw-   0        0        0     9587 2023-08-08 10:57:42.000000 adata-2.0.1b0/adata/stock/market/concepth_market/concept_market_ths.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.230183 adata-2.0.1b0/adata/stock/market/index_market/
--rw-rw-rw-   0        0        0       97 2023-08-07 03:04:02.000000 adata-2.0.1b0/adata/stock/market/index_market/__init__.py
--rw-rw-rw-   0        0        0     2218 2023-12-29 03:56:23.000000 adata-2.0.1b0/adata/stock/market/index_market/market_index.py
--rw-rw-rw-   0        0        0     6865 2023-12-29 03:55:54.000000 adata-2.0.1b0/adata/stock/market/index_market/market_index_east.py
--rw-rw-rw-   0        0        0     1746 2023-08-08 11:47:56.000000 adata-2.0.1b0/adata/stock/market/index_market/market_index_template.py
--rw-rw-rw-   0        0        0     8246 2023-08-08 11:48:17.000000 adata-2.0.1b0/adata/stock/market/index_market/market_index_ths.py
--rw-rw-rw-   0        0        0     3199 2023-10-18 04:50:22.000000 adata-2.0.1b0/adata/stock/market/stock_dividend.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.237185 adata-2.0.1b0/adata/stock/market/stock_market/
--rw-rw-rw-   0        0        0      176 2023-10-10 02:59:10.000000 adata-2.0.1b0/adata/stock/market/stock_market/__init__.py
--rw-rw-rw-   0        0        0     3519 2024-04-17 10:25:01.000000 adata-2.0.1b0/adata/stock/market/stock_market/stock_market.py
--rw-rw-rw-   0        0        0    11398 2023-12-04 12:31:36.000000 adata-2.0.1b0/adata/stock/market/stock_market/stock_market_baidu.py
--rw-rw-rw-   0        0        0     5415 2023-09-18 06:30:43.000000 adata-2.0.1b0/adata/stock/market/stock_market/stock_market_qq.py
--rw-rw-rw-   0        0        0     2666 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/market/stock_market/stock_market_sina.py
--rw-rw-rw-   0        0        0     2658 2023-09-13 12:58:10.000000 adata-2.0.1b0/adata/stock/market/stock_market/stock_market_template.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.134520 adata-2.0.1b0/adata.egg-info/
--rw-rw-rw-   0        0        0    21039 2024-04-17 10:56:33.000000 adata-2.0.1b0/adata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3649 2024-04-17 10:56:33.000000 adata-2.0.1b0/adata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 10:56:33.000000 adata-2.0.1b0/adata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2024-04-17 10:56:33.000000 adata-2.0.1b0/adata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-17 10:56:33.000000 adata-2.0.1b0/adata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 10:56:33.240186 adata-2.0.1b0/setup.cfg
--rw-rw-rw-   0        0        0     1838 2023-12-04 12:31:36.000000 adata-2.0.1b0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 10:07:38.967992 adata-2.1.0/
+-rw-rw-rw-   0        0        0    11558 2023-04-07 05:48:39.000000 adata-2.1.0/LICENSE
+-rw-rw-rw-   0        0        0      126 2023-10-23 06:31:33.000000 adata-2.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    22202 2024-05-06 10:07:38.965992 adata-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    21493 2024-05-06 08:45:08.000000 adata-2.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 10:07:38.846964 adata-2.1.0/adata/
+-rw-rw-rw-   0        0        0     1189 2023-10-10 02:59:10.000000 adata-2.1.0/adata/__init__.py
+-rw-rw-rw-   0        0        0      735 2024-05-06 05:25:06.000000 adata-2.1.0/adata/__version__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 10:07:38.853968 adata-2.1.0/adata/bond/
+-rw-rw-rw-   0        0        0      329 2024-05-06 05:14:27.000000 adata-2.1.0/adata/bond/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 10:07:38.855966 adata-2.1.0/adata/bond/cache/
+-rw-rw-rw-   0        0        0      103 2023-08-18 09:30:57.000000 adata-2.1.0/adata/bond/cache/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 10:07:38.857968 adata-2.1.0/adata/bond/info/
+-rw-rw-rw-   0        0        0      261 2023-10-10 02:59:10.000000 adata-2.1.0/adata/bond/info/__init__.py
+-rw-rw-rw-   0        0        0     2200 2023-05-31 08:21:01.000000 adata-2.1.0/adata/bond/info/bond_code.py
+drwxrwxrwx   0        0        0        0 2024-05-06 10:07:38.861968 adata-2.1.0/adata/bond/market/
+-rw-rw-rw-   0        0        0      275 2024-05-06 05:14:27.000000 adata-2.1.0/adata/bond/market/__init__.py
+-rw-rw-rw-   0        0        0      903 2024-05-06 05:16:30.000000 adata-2.1.0/adata/bond/market/bond_market.py
+-rw-rw-rw-   0        0        0     2339 2024-05-06 06:00:23.000000 adata-2.1.0/adata/bond/market/bond_market_sina.py
+-rw-rw-rw-   0        0        0      641 2024-05-06 05:14:27.000000 adata-2.1.0/adata/bond/market/bond_market_template.py
+drwxrwxrwx   0        0        0        0 2024-05-06 10:07:38.862969 adata-2.1.0/adata/common/
+-rw-rw-rw-   0        0        0      150 2023-04-07 05:48:39.000000 adata-2.1.0/adata/common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 10:07:38.865969 adata-2.1.0/adata/common/base/
+-rw-rw-rw-   0        0        0      133 2023-06-05 03:44:57.000000 adata-2.1.0/adata/common/base/__init__.py
+-rw-rw-rw-   0        0        0      195 2023-08-14 05:47:34.000000 adata-2.1.0/adata/common/base/base_req.py
+-rw-rw-rw-   0        0        0     3015 2023-08-18 09:30:57.000000 adata-2.1.0/adata/common/base/base_ths.py
+drwxrwxrwx   0        0        0        0 2024-05-06 10:07:38.869970 adata-2.1.0/adata/common/exception/
+-rw-rw-rw-   0        0        0       97 2023-07-10 08:15:13.000000 adata-2.1.0/adata/common/exception/__init__.py
+-rw-rw-rw-   0        0        0      379 2023-08-01 09:58:42.000000 adata-2.1.0/adata/common/exception/exception_msg.py
+-rw-rw-rw-   0        0        0      350 2023-08-14 06:04:13.000000 adata-2.1.0/adata/common/exception/handler.py
+drwxrwxrwx   0        0        0        0 2024-05-06 10:07:38.875972 adata-2.1.0/adata/common/headers/
+-rw-rw-rw-   0        0        0     6407 2023-07-10 08:15:13.000000 adata-2.1.0/adata/common/headers/__init__.py
+-rw-rw-rw-   0        0        0     5772 2023-04-07 05:48:39.000000 adata-2.1.0/adata/common/headers/baidu_headers.py
+-rw-rw-rw-   0        0        0      571 2023-08-14 05:47:34.000000 adata-2.1.0/adata/common/headers/east_headers.py
+-rw-rw-rw-   0        0        0      602 2023-04-18 11:18:06.000000 adata-2.1.0/adata/common/headers/sina_headers.py
+-rw-rw-rw-   0        0        0     3085 2023-08-08 04:51:00.000000 adata-2.1.0/adata/common/headers/ths_headers.py
+drwxrwxrwx   0        0        0        0 2024-05-06 10:07:38.878971 adata-2.1.0/adata/common/js/
+-rw-rw-rw-   0        0        0       99 2023-05-05 10:05:38.000000 adata-2.1.0/adata/common/js/__init__.py
+-rw-rw-rw-   0        0        0    15792 2023-08-01 09:31:40.000000 adata-2.1.0/adata/common/js/hexin.js
+-rw-rw-rw-   0        0        0    39849 2023-06-28 03:35:45.000000 adata-2.1.0/adata/common/js/ths.js
+drwxrwxrwx   0        0        0        0 2024-05-06 10:07:38.883973 adata-2.1.0/adata/common/utils/
+-rw-rw-rw-   0        0        0      190 2023-07-10 08:15:13.000000 adata-2.1.0/adata/common/utils/__init__.py
+-rw-rw-rw-   0        0        0      501 2023-12-04 11:20:28.000000 adata-2.1.0/adata/common/utils/code_utils.py
+-rw-rw-rw-   0        0        0      877 2023-10-10 02:59:10.000000 adata-2.1.0/adata/common/utils/cookie.py
+-rw-rw-rw-   0        0        0     3046 2023-04-07 05:48:39.000000 adata-2.1.0/adata/common/utils/snowflake.py
+-rw-rw-rw-   0        0        0     2891 2023-08-07 03:04:02.000000 adata-2.1.0/adata/common/utils/sunrequests.py
+drwxrwxrwx   0        0        0        0 2024-05-06 10:07:38.884973 adata-2.1.0/adata/fund/
+-rw-rw-rw-   0        0        0      327 2024-04-17 10:25:02.000000 adata-2.1.0/adata/fund/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 10:07:38.885973 adata-2.1.0/adata/fund/cache/
+-rw-rw-rw-   0        0        0      103 2023-06-02 06:05:35.000000 adata-2.1.0/adata/fund/cache/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 10:07:38.888974 adata-2.1.0/adata/fund/info/
+-rw-rw-rw-   0        0        0      260 2023-10-10 02:59:10.000000 adata-2.1.0/adata/fund/info/__init__.py
+-rw-rw-rw-   0        0        0     5247 2023-08-01 10:31:22.000000 adata-2.1.0/adata/fund/info/fund_info.py
+drwxrwxrwx   0        0        0        0 2024-05-06 10:07:38.891975 adata-2.1.0/adata/fund/market/
+-rw-rw-rw-   0        0        0      379 2024-04-17 10:25:02.000000 adata-2.1.0/adata/fund/market/__init__.py
+-rw-rw-rw-   0        0        0     2416 2024-04-17 10:44:44.000000 adata-2.1.0/adata/fund/market/etf_market.py
+-rw-rw-rw-   0        0        0      654 2024-04-17 10:45:50.000000 adata-2.1.0/adata/fund/market/etf_market_template.py
+-rw-rw-rw-   0        0        0     7990 2024-04-17 10:45:50.000000 adata-2.1.0/adata/fund/market/etf_market_ths.py
+drwxrwxrwx   0        0        0        0 2024-05-06 10:07:38.893975 adata-2.1.0/adata/message/
+-rw-rw-rw-   0        0        0      103 2023-04-07 05:48:39.000000 adata-2.1.0/adata/message/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 10:07:38.898977 adata-2.1.0/adata/sentiment/
+-rw-rw-rw-   0        0        0      531 2024-05-06 06:08:44.000000 adata-2.1.0/adata/sentiment/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 10:07:38.900977 adata-2.1.0/adata/sentiment/cache/
+-rw-rw-rw-   0        0        0      103 2023-08-18 09:30:57.000000 adata-2.1.0/adata/sentiment/cache/__init__.py
+-rw-rw-rw-   0        0        0     4684 2024-05-06 05:10:37.000000 adata-2.1.0/adata/sentiment/hot.py
+-rw-rw-rw-   0        0        0     9633 2023-08-01 04:08:30.000000 adata-2.1.0/adata/sentiment/north_flow.py
+-rw-rw-rw-   0        0        0     3741 2023-08-18 09:30:57.000000 adata-2.1.0/adata/sentiment/securities_margin.py
+-rw-rw-rw-   0        0        0     4271 2023-08-08 04:51:00.000000 adata-2.1.0/adata/sentiment/stock_lifting.py
+drwxrwxrwx   0        0        0        0 2024-05-06 10:07:38.901978 adata-2.1.0/adata/stock/
+-rw-rw-rw-   0        0        0      420 2023-10-10 02:59:10.000000 adata-2.1.0/adata/stock/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 10:07:38.906978 adata-2.1.0/adata/stock/cache/
+-rw-rw-rw-   0        0        0      267 2023-10-18 11:49:59.000000 adata-2.1.0/adata/stock/cache/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 10:07:38.930984 adata-2.1.0/adata/stock/cache/calendar/
+-rw-rw-rw-   0        0        0       34 2023-07-07 08:19:03.000000 adata-2.1.0/adata/stock/cache/calendar/2004.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.1.0/adata/stock/cache/calendar/2005.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.1.0/adata/stock/cache/calendar/2006.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.1.0/adata/stock/cache/calendar/2007.csv
+-rw-rw-rw-   0        0        0     5890 2023-07-07 08:19:03.000000 adata-2.1.0/adata/stock/cache/calendar/2008.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.1.0/adata/stock/cache/calendar/2009.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.1.0/adata/stock/cache/calendar/2010.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.1.0/adata/stock/cache/calendar/2011.csv
+-rw-rw-rw-   0        0        0     5890 2023-07-07 08:19:03.000000 adata-2.1.0/adata/stock/cache/calendar/2012.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.1.0/adata/stock/cache/calendar/2013.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.1.0/adata/stock/cache/calendar/2014.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.1.0/adata/stock/cache/calendar/2015.csv
+-rw-rw-rw-   0        0        0     5890 2023-07-07 08:19:03.000000 adata-2.1.0/adata/stock/cache/calendar/2016.csv
+-rw-rw-rw-   0        0        0     5858 2023-07-07 08:19:03.000000 adata-2.1.0/adata/stock/cache/calendar/2017.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.1.0/adata/stock/cache/calendar/2018.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.1.0/adata/stock/cache/calendar/2019.csv
+-rw-rw-rw-   0        0        0     5890 2023-07-07 08:19:03.000000 adata-2.1.0/adata/stock/cache/calendar/2020.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.1.0/adata/stock/cache/calendar/2021.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.1.0/adata/stock/cache/calendar/2022.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.1.0/adata/stock/cache/calendar/2023.csv
+-rw-rw-rw-   0        0        0     5888 2023-12-29 03:33:12.000000 adata-2.1.0/adata/stock/cache/calendar/2024.csv
+-rw-rw-rw-   0        0        0      428 2023-12-11 07:21:42.000000 adata-2.1.0/adata/stock/cache/calendar/__init__.py
+-rw-rw-rw-   0        0        0   174847 2023-10-18 12:45:02.000000 adata-2.1.0/adata/stock/cache/code.csv
+-rw-rw-rw-   0        0        0     8752 2023-06-02 06:45:42.000000 adata-2.1.0/adata/stock/cache/index_code_rel_ths.py
+drwxrwxrwx   0        0        0        0 2024-05-06 10:07:38.932985 adata-2.1.0/adata/stock/index/
+-rw-rw-rw-   0        0        0      267 2023-06-02 03:44:46.000000 adata-2.1.0/adata/stock/index/__init__.py
+-rw-rw-rw-   0        0        0      207 2023-06-02 03:44:46.000000 adata-2.1.0/adata/stock/index/cal_index.py
+drwxrwxrwx   0        0        0        0 2024-05-06 10:07:38.938986 adata-2.1.0/adata/stock/info/
+-rw-rw-rw-   0        0        0      563 2024-04-24 02:40:19.000000 adata-2.1.0/adata/stock/info/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 10:07:38.943987 adata-2.1.0/adata/stock/info/concept/
+-rw-rw-rw-   0        0        0       86 2023-08-07 03:04:02.000000 adata-2.1.0/adata/stock/info/concept/__init__.py
+-rw-rw-rw-   0        0        0      485 2023-08-07 03:04:02.000000 adata-2.1.0/adata/stock/info/concept/stock_concept.py
+-rw-rw-rw-   0        0        0     5595 2024-02-26 03:31:53.000000 adata-2.1.0/adata/stock/info/concept/stock_concept_east.py
+-rw-rw-rw-   0        0        0      463 2023-12-04 11:54:33.000000 adata-2.1.0/adata/stock/info/concept/stock_concept_template.py
+-rw-rw-rw-   0        0        0    15126 2023-12-29 03:33:12.000000 adata-2.1.0/adata/stock/info/concept/stock_concept_ths.py
+-rw-rw-rw-   0        0        0     5770 2023-10-18 12:46:30.000000 adata-2.1.0/adata/stock/info/stock_code.py
+-rw-rw-rw-   0        0        0    10715 2023-10-18 04:49:44.000000 adata-2.1.0/adata/stock/info/stock_index.py
+-rw-rw-rw-   0        0        0     3482 2024-04-24 03:14:43.000000 adata-2.1.0/adata/stock/info/stock_info.py
+-rw-rw-rw-   0        0        0     2321 2023-08-08 04:46:57.000000 adata-2.1.0/adata/stock/info/trade_calendar.py
+drwxrwxrwx   0        0        0        0 2024-05-06 10:07:38.945987 adata-2.1.0/adata/stock/market/
+-rw-rw-rw-   0        0        0      550 2023-10-10 02:59:10.000000 adata-2.1.0/adata/stock/market/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 10:07:38.951988 adata-2.1.0/adata/stock/market/concepth_market/
+-rw-rw-rw-   0        0        0      385 2023-08-07 03:32:53.000000 adata-2.1.0/adata/stock/market/concepth_market/__init__.py
+-rw-rw-rw-   0        0        0     7028 2023-08-08 11:22:09.000000 adata-2.1.0/adata/stock/market/concepth_market/concept_market_east.py
+-rw-rw-rw-   0        0        0      695 2023-08-08 11:05:55.000000 adata-2.1.0/adata/stock/market/concepth_market/concept_market_template.py
+-rw-rw-rw-   0        0        0     9587 2023-08-08 10:57:42.000000 adata-2.1.0/adata/stock/market/concepth_market/concept_market_ths.py
+drwxrwxrwx   0        0        0        0 2024-05-06 10:07:38.956989 adata-2.1.0/adata/stock/market/index_market/
+-rw-rw-rw-   0        0        0       97 2023-08-07 03:04:02.000000 adata-2.1.0/adata/stock/market/index_market/__init__.py
+-rw-rw-rw-   0        0        0     2218 2023-12-29 03:56:23.000000 adata-2.1.0/adata/stock/market/index_market/market_index.py
+-rw-rw-rw-   0        0        0     6865 2023-12-29 03:55:54.000000 adata-2.1.0/adata/stock/market/index_market/market_index_east.py
+-rw-rw-rw-   0        0        0     1746 2023-08-08 11:47:56.000000 adata-2.1.0/adata/stock/market/index_market/market_index_template.py
+-rw-rw-rw-   0        0        0     8246 2023-08-08 11:48:17.000000 adata-2.1.0/adata/stock/market/index_market/market_index_ths.py
+-rw-rw-rw-   0        0        0     3199 2023-10-18 04:50:22.000000 adata-2.1.0/adata/stock/market/stock_dividend.py
+drwxrwxrwx   0        0        0        0 2024-05-06 10:07:38.963991 adata-2.1.0/adata/stock/market/stock_market/
+-rw-rw-rw-   0        0        0      176 2023-10-10 02:59:10.000000 adata-2.1.0/adata/stock/market/stock_market/__init__.py
+-rw-rw-rw-   0        0        0     3519 2024-05-06 02:15:08.000000 adata-2.1.0/adata/stock/market/stock_market/stock_market.py
+-rw-rw-rw-   0        0        0    11398 2023-12-04 12:31:36.000000 adata-2.1.0/adata/stock/market/stock_market/stock_market_baidu.py
+-rw-rw-rw-   0        0        0     5415 2023-09-18 06:30:43.000000 adata-2.1.0/adata/stock/market/stock_market/stock_market_qq.py
+-rw-rw-rw-   0        0        0     2666 2023-07-07 08:19:03.000000 adata-2.1.0/adata/stock/market/stock_market/stock_market_sina.py
+-rw-rw-rw-   0        0        0     2658 2023-09-13 12:58:10.000000 adata-2.1.0/adata/stock/market/stock_market/stock_market_template.py
+drwxrwxrwx   0        0        0        0 2024-05-06 10:07:38.851966 adata-2.1.0/adata.egg-info/
+-rw-rw-rw-   0        0        0    22202 2024-05-06 10:07:38.000000 adata-2.1.0/adata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3783 2024-05-06 10:07:38.000000 adata-2.1.0/adata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 10:07:38.000000 adata-2.1.0/adata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2024-05-06 10:07:38.000000 adata-2.1.0/adata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-06 10:07:38.000000 adata-2.1.0/adata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 10:07:38.967992 adata-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1838 2023-12-04 12:31:36.000000 adata-2.1.0/setup.py
```

### Comparing `adata-2.0.1b0/LICENSE` & `adata-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/PKG-INFO` & `adata-2.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adata
-Version: 2.0.1b0
+Version: 2.1.0
 Summary: A Data,A Stock,ETF,Bond,Quant,Stock Market,K Line
 Home-page: https://github.com/1nchaos/adata
 Author: 1nchaos
 Author-email: 9527@1nchaos.com
 License: Apache License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
@@ -151,14 +151,15 @@
 ### （1）股票-Stock
 
 #### 	1. 基本信息
 
 | 数据             | API                                   | 说明                                   | 备注                                                         |
 | ---------------- | ------------------------------------- | -------------------------------------- | ------------------------------------------------------------ |
 | A股代码          | stock.info.all_code()                 | 所有A股代码信息                        |                                                              |
+| 股本信息         | stock.info.get_stock_shares()         | 获取单只股票的股本信息                 | 来源：东方财富                                               |
 | **概念**         |                                       |                                        |                                                              |
 | 来源：同花顺     |                                       |                                        |                                                              |
 | 概念代码         | stock.info.all_concept_code_ths()     | 所有A股概念代码信息（同花顺）          | 来源：同花顺公开数据                                         |
 | 概念成分列表     | stock.info.concept_constituent_ths()  | 获取同花顺概念指数的成分股（同花顺）   | 注意：返回结果只有股票代码和股票简称，可根据概念名称查询     |
 | 股票所属概念     | stock.info.get_concept_ths()          | 获取单只股票所属的概念板块             | [F10](https://basic.10jqka.com.cn/300033/concept.html)       |
 | 来源：东方财富   |                                       |                                        |                                                              |
 | 概念代码         | stock.info.all_concept_code_east()    | 所有A股概念代码信息（东方财富）        | 来源：[东方财富](https://data.eastmoney.com/bkzj/gn.html)    |
@@ -207,29 +208,32 @@
 | ------- | ------------------------------------ | -------------------------------- | ---------------------------------------- |
 | ETF行情 | fund.market.get_market_etf()         | 获取ETF的行情信息-日、周、月 k线 | 来源：[同花顺](https://m.10jqka.com.cn/) |
 |         | fund.market.get_market_etf_min()     | 获取ETF的行情-当日分时           |                                          |
 |         | fund.market.get_market_etf_current() | 获取当前的ETF行情                | 实时行情                                 |
 
 ### （3）债券-Bond
 
-| 数据           | API                          | 说明                                | 备注                                                   |
-| -------------- | ---------------------------- | ----------------------------------- | ------------------------------------------------------ |
-| 可转债代码     | bond.info.all_convert_code() | 获取所有A股市场的可转换债券代码信息 | 来源：1. [同花顺](http://data.10jqka.com.cn/ipo/bond/) |
-| 其它数据排期中 | TODO                         | 若您有相关资源可以一起参与贡献      |                                                        |
+| 数据       | API                               | 说明                                | 备注                                                   |
+| ---------- | --------------------------------- | ----------------------------------- | ------------------------------------------------------ |
+| 可转债代码 | bond.info.all_convert_code()      | 获取所有A股市场的可转换债券代码信息 | 来源：1. [同花顺](http://data.10jqka.com.cn/ipo/bond/) |
+| 可转债行情 | bond.market.list_market_current() | 获取A股市场的可转换债券最新行情     | 来源：新浪                                             |
 
 ### （4）舆情
 
 | 数据                     | API                                  | 说明                                       | 备注                                                         |
 | ------------------------ | ------------------------------------ | ------------------------------------------ | ------------------------------------------------------------ |
 | 最近一个月的股票解禁列表 | sentiment.stock_lifting_last_month() | 查询最近一个月的股票解禁列表               | 来源：1. [同花顺](http://data.10jqka.com.cn/market/xsjj/)    |
 | 全市场融资融券余额列表   | sentiment.securities_margin()        | 查询全市场融资融券余额列表                 | 来源：1. [东方财富](https://data.eastmoney.com/rzrq/)        |
 | **北向资金-行情**        |                                      |                                            |                                                              |
 |                          | sentiment.north.north_flow_current() | 获取北向资金（沪深港通）当前流入资金的行情 | 来源：1.[东方财富](https://data.eastmoney.com/hsgt/index.html) |
 |                          | sentiment.north.north_flow_min()     | 获取北向资金分时行情                       |                                                              |
 |                          | sentiment.north.north_flow()         | 获取北向资金历史流入行情                   |                                                              |
+| **热度榜单**             | sentiment.hot.pop_rank_100_east      | 东方财富人气100榜单                        | 来源：[东方财富](http://guba.eastmoney.com/rank/)            |
+|                          | sentiment.hot.hot_rank_100_ths()     | 同花顺热度100排行榜                        | 来源：[同花顺](https://dq.10jqka.com.cn/fuyao/hot_list_data/out/hot_list/v1/stock?stock_type=a&type=hour&list_type=normal) |
+|                          | sentiment.hot.hot_concept_20_ths()   | 同花顺热门概念板块20排行榜                 | 来源：[同花顺](https://dq.10jqka.com.cn/fuyao/hot_list_data/out/hot_list/v1/stock?stock_type=a&type=hour&list_type=normal) |
 | 其它数据排期中           | TODO                                 | 若您有相关资源可以一起参与贡献             |                                                              |
 
 ## 三、[数据源](https://adata.30006124.xyz/dataSource.html)
 
 | 数据源     | 板块                                                         | 描述             |
 | ---------- | ------------------------------------------------------------ | ---------------- |
 | 同花顺     | [数据中心](http://data.10jqka.com.cn/)，[行情中心](http://q.10jqka.com.cn/)，[问财](http://www.iwencai.com/unifiedwap/home/index) | 让投资变的更简单 |
@@ -277,17 +281,17 @@
 4.  新建 Pull Request
 
 
 ## 特别鸣谢
 
 > 对于项目有支持，包括但不仅限：内容贡献，bug提交，思想交流等等，对项目有影响的个人和机构
 
-| Simon | [bigbigbigfish](https://github.com/bigbigbigfish) | [LuneZ99](https://github.com/LuneZ99) | 匿名用户 | thue | [Triones009](https://github.com/Triones009) | **[adaaaaaa](https://github.com/adaaaaaa)** | **[LeslieWuboy](https://github.com/LeslieWuboy)** |
-| ----- | ------------------------------------------------- | ------------------------------------- | -------- | ---- | ------------------------------------------- | ------------------------------------------- | ------------------------------------------------- |
-|       |                                                   |                                       |          |      |                                             |                                             |                                                   |
+| Simon                                 | [bigbigbigfish](https://github.com/bigbigbigfish) | [LuneZ99](https://github.com/LuneZ99)         | 匿名用户 | thue | [Triones009](https://github.com/Triones009) | **[adaaaaaa](https://github.com/adaaaaaa)** | **[LeslieWuboy](https://github.com/LeslieWuboy)** | [yinzhengxin](https://github.com/yinzhengxin) |
+| ------------------------------------- | ------------------------------------------------- | --------------------------------------------- | -------- | ---- | ------------------------------------------- | ------------------------------------------- | ------------------------------------------------- | --------------------------------------------- |
+| [yxm0513](https://github.com/yxm0513) | [hanxuanliang](https://github.com/hanxuanliang)   | [akihara-sam](https://github.com/akihara-sam) |          |      |                                             |                                             |                                                   |                                               |
 
 ----------------------------------------------------------------------
 
 > 
 ## Star History
 
 [![Star History Chart](https://api.star-history.com/svg?repos=1nchaos/adata&type=Date)](https://star-history.com/#1nchaos/adata&Date)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: adata Version: 2.0.1b0 Summary: A Data,A
+Metadata-Version: 2.1 Name: adata Version: 2.1.0 Summary: A Data,A
 Stock,ETF,Bond,Quant,Stock Market,K Line Home-page: https://github.com/1nchaos/
 adata Author: 1nchaos Author-email: 9527@1nchaos.com License: Apache License
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
@@ -69,16 +69,18 @@
 ## äºã[æ°æ®åè¡¨](https://adata.30006124.xyz/dic/dataList.html)
 æ´çäºææ°çæ¬çæ°æ®åè¡¨åç¸å³ä½¿ç¨Apiï¼è¯¦ç»åå®¹åç¸å³ä½¿ç¨åæ°ï¼è¯·åèæ°æ®å­å¸ææ¡£ã
 - [æ°æ®åè¡¨](https://adata.30006124.xyz/dic/dataList.html) - [æ°æ®å­å¸]
 (https://adata.30006124.xyz/dic/stockInfo.html) ### ï¼1ï¼è¡ç¥¨-Stock #### 1.
 åºæ¬ä¿¡æ¯ | æ°æ® | API | è¯´æ | å¤æ³¨ | | ---------------- | ----------
 --------------------------- | -------------------------------------- | --------
 ---------------------------------------------------- | | Aè¡ä»£ç  |
-stock.info.all_code() | ææAè¡ä»£ç ä¿¡æ¯ | | | **æ¦å¿µ** | | | | |
-æ¥æºï¼åè±é¡º | | | | | æ¦å¿µä»£ç  | stock.info.all_concept_code_ths() |
+stock.info.all_code() | ææAè¡ä»£ç ä¿¡æ¯ | | | è¡æ¬ä¿¡æ¯ |
+stock.info.get_stock_shares() | è·åååªè¡ç¥¨çè¡æ¬ä¿¡æ¯ |
+æ¥æºï¼ä¸æ¹è´¢å¯ | | **æ¦å¿µ** | | | | | æ¥æºï¼åè±é¡º | | | | |
+æ¦å¿µä»£ç  | stock.info.all_concept_code_ths() |
 ææAè¡æ¦å¿µä»£ç ä¿¡æ¯ï¼åè±é¡ºï¼ | æ¥æºï¼åè±é¡ºå¬å¼æ°æ® |
 | æ¦å¿µæååè¡¨ | stock.info.concept_constituent_ths() |
 è·ååè±é¡ºæ¦å¿µææ°çæåè¡ï¼åè±é¡ºï¼ |
 æ³¨æï¼è¿åç»æåªæè¡ç¥¨ä»£ç åè¡ç¥¨ç®ç§°ï¼å¯æ ¹æ®æ¦å¿µåç§°æ¥è¯¢
 | | è¡ç¥¨æå±æ¦å¿µ | stock.info.get_concept_ths() |
 è·åååªè¡ç¥¨æå±çæ¦å¿µæ¿å | [F10](https://basic.10jqka.com.cn/
 300033/concept.html) | | æ¥æºï¼ä¸æ¹è´¢å¯ | | | | | æ¦å¿µä»£ç  |
@@ -141,48 +143,58 @@
 quote.eastmoney.com/center/gridlist.html#fund_etf) | #### 2. è¡æä¿¡æ¯ |
 æ°æ® | API | è¯´æ | å¤æ³¨ | | ------- | ----------------------------------
 -- | -------------------------------- | ---------------------------------------
 - | | ETFè¡æ | fund.market.get_market_etf() | è·åETFçè¡æä¿¡æ¯-
 æ¥ãå¨ãæ kçº¿ | æ¥æºï¼[åè±é¡º](https://m.10jqka.com.cn/) | | |
 fund.market.get_market_etf_min() | è·åETFçè¡æ-å½æ¥åæ¶ | | | |
 fund.market.get_market_etf_current() | è·åå½åçETFè¡æ | å®æ¶è¡æ
-| ### ï¼3ï¼åºå¸-Bond | æ°æ® | API | è¯´æ | å¤æ³¨ | | -------------- |
----------------------------- | ----------------------------------- | ----------
--------------------------------------------- | | å¯è½¬åºä»£ç  |
+| ### ï¼3ï¼åºå¸-Bond | æ°æ® | API | è¯´æ | å¤æ³¨ | | ---------- | ----
+----------------------------- | ----------------------------------- | ---------
+--------------------------------------------- | | å¯è½¬åºä»£ç  |
 bond.info.all_convert_code() |
 è·åææAè¡å¸åºçå¯è½¬æ¢åºå¸ä»£ç ä¿¡æ¯ | æ¥æºï¼1. [åè±é¡º]
-(http://data.10jqka.com.cn/ipo/bond/) | | å¶å®æ°æ®ææä¸­ | TODO |
-è¥æ¨æç¸å³èµæºå¯ä»¥ä¸èµ·åä¸è´¡ç® | | ### ï¼4ï¼èæ | æ°æ® |
-API | è¯´æ | å¤æ³¨ | | ------------------------ | --------------------------
----------- | ------------------------------------------ | ---------------------
---------------------------------------- | |
+(http://data.10jqka.com.cn/ipo/bond/) | | å¯è½¬åºè¡æ |
+bond.market.list_market_current() |
+è·åAè¡å¸åºçå¯è½¬æ¢åºå¸ææ°è¡æ | æ¥æºï¼æ°æµª | ###
+ï¼4ï¼èæ | æ°æ® | API | è¯´æ | å¤æ³¨ | | ------------------------ | -
+----------------------------------- | -----------------------------------------
+- | ------------------------------------------------------------ | |
 æè¿ä¸ä¸ªæçè¡ç¥¨è§£ç¦åè¡¨ | sentiment.stock_lifting_last_month() |
 æ¥è¯¢æè¿ä¸ä¸ªæçè¡ç¥¨è§£ç¦åè¡¨ | æ¥æºï¼1. [åè±é¡º](http://
 data.10jqka.com.cn/market/xsjj/) | | å¨å¸åºèèµèå¸ä½é¢åè¡¨ |
 sentiment.securities_margin() | æ¥è¯¢å¨å¸åºèèµèå¸ä½é¢åè¡¨ |
 æ¥æºï¼1. [ä¸æ¹è´¢å¯](https://data.eastmoney.com/rzrq/) | |
 **ååèµé-è¡æ** | | | | | | sentiment.north.north_flow_current() |
 è·åååèµéï¼æ²ªæ·±æ¸¯éï¼å½åæµå¥èµéçè¡æ | æ¥æºï¼1.
 [ä¸æ¹è´¢å¯](https://data.eastmoney.com/hsgt/index.html) | | |
 sentiment.north.north_flow_min() | è·åååèµéåæ¶è¡æ | | | |
 sentiment.north.north_flow() | è·åååèµéåå²æµå¥è¡æ | | |
-å¶å®æ°æ®ææä¸­ | TODO | è¥æ¨æç¸å³èµæºå¯ä»¥ä¸èµ·åä¸è´¡ç® |
-| ## ä¸ã[æ°æ®æº](https://adata.30006124.xyz/dataSource.html) | æ°æ®æº
-| æ¿å | æè¿° | | ---------- | --------------------------------------------
----------------- | ---------------- | | åè±é¡º | [æ°æ®ä¸­å¿](http://
-data.10jqka.com.cn/)ï¼[è¡æä¸­å¿](http://q.10jqka.com.cn/)ï¼[é®è´¢](http:
-//www.iwencai.com/unifiedwap/home/index) | è®©æèµåçæ´ç®å | |
-ç¾åº¦è¡å¸é | [è¡å¸é](https://gushitong.baidu.com/) |
-ç§æè®©æèµæ´ç®å | | ä¸æ¹è´¢å¯ | [æ°æ®ä¸­å¿](https://
-data.eastmoney.com/center/)ï¼[è¡æä¸­å¿](http://quote.eastmoney.com/center/
-) | è´¢ç»é¨æ· | | è¾è®¯çè´¢ | [è¡æä¸­å¿](https://
-stockapp.finance.qq.com/mstats/#) | | | æ°æµªè´¢ç» | [æ°æµªè´¢ç»](https://
-finance.sina.com.cn/stock/) | é¨æ·ç½ç« | ***-------------------------------
--------------æè°¢åä½å¤§åæä¾çæ°æ®---------------------------------
--------------*** ## åã å¶å®åè
+**ç­åº¦æ¦å** | sentiment.hot.pop_rank_100_east |
+ä¸æ¹è´¢å¯äººæ°100æ¦å | æ¥æºï¼[ä¸æ¹è´¢å¯](http://
+guba.eastmoney.com/rank/) | | | sentiment.hot.hot_rank_100_ths() |
+åè±é¡ºç­åº¦100æè¡æ¦ | æ¥æºï¼[åè±é¡º](https://dq.10jqka.com.cn/
+fuyao/hot_list_data/out/hot_list/v1/
+stock?stock_type=a&type=hour&list_type=normal) | | |
+sentiment.hot.hot_concept_20_ths() | åè±é¡ºç­é¨æ¦å¿µæ¿å20æè¡æ¦ |
+æ¥æºï¼[åè±é¡º](https://dq.10jqka.com.cn/fuyao/hot_list_data/out/hot_list/
+v1/stock?stock_type=a&type=hour&list_type=normal) | | å¶å®æ°æ®ææä¸­ |
+TODO | è¥æ¨æç¸å³èµæºå¯ä»¥ä¸èµ·åä¸è´¡ç® | | ## ä¸ã[æ°æ®æº]
+(https://adata.30006124.xyz/dataSource.html) | æ°æ®æº | æ¿å | æè¿° | |
+---------- | ------------------------------------------------------------ | ---
+------------- | | åè±é¡º | [æ°æ®ä¸­å¿](http://data.10jqka.com.cn/)ï¼
+[è¡æä¸­å¿](http://q.10jqka.com.cn/)ï¼[é®è´¢](http://www.iwencai.com/
+unifiedwap/home/index) | è®©æèµåçæ´ç®å | | ç¾åº¦è¡å¸é |
+[è¡å¸é](https://gushitong.baidu.com/) | ç§æè®©æèµæ´ç®å | |
+ä¸æ¹è´¢å¯ | [æ°æ®ä¸­å¿](https://data.eastmoney.com/center/)ï¼
+[è¡æä¸­å¿](http://quote.eastmoney.com/center/) | è´¢ç»é¨æ· | |
+è¾è®¯çè´¢ | [è¡æä¸­å¿](https://stockapp.finance.qq.com/mstats/#) | | |
+æ°æµªè´¢ç» | [æ°æµªè´¢ç»](https://finance.sina.com.cn/stock/) |
+é¨æ·ç½ç« | ***--------------------------------------------
+æè°¢åä½å¤§åæä¾çæ°æ®----------------------------------------------
+*** ## åã å¶å®åè
 ä¸»è¦è®°å½æ¥éè¿çé¡¹ç®åç¸å³å¹³å°ï¼å¹¶å¯¹æ­¤é¡¹ç®äº§çäºæ·±è¿å°è±¡ï¼ç¹æ­¤é¸£è°¢ã
 | [akshare](https://gitee.com/mirrors/akshare) | [èå®½éå](https://
 www.joinquant.com/) | [baostock](http://baostock.com/baostock/index.php/
 Python%E5%BC%80%E5%8F%91%E8%B5%84%E6%BA%90) | [MyData](http://api.mairui.club/
 hsdata.html) | | -------------------------------------------- | ---------------
 ----------------------- | -----------------------------------------------------
 ------- | -------------------------------------------- | ## äºãåå¸è®¡å
@@ -203,19 +215,22 @@
 1. Fork æ¬ä»åº 2. æ°å»º Feat_xxx åæ¯ 3.
 æäº¤ä»£ç ï¼æ³¨æä»£ç é£æ ¼åæ¬é¡¹ç®ä¸è´å³å¯ï¼ 4. æ°å»º Pull
 Request ## ç¹å«é¸£è°¢ >
 å¯¹äºé¡¹ç®ææ¯æï¼åæ¬ä½ä¸ä»éï¼åå®¹è´¡ç®ï¼bugæäº¤ï¼ææ³äº¤æµç­ç­ï¼å¯¹é¡¹ç®æå½±åçä¸ªäººåæºæ
 | Simon | [bigbigbigfish](https://github.com/bigbigbigfish) | [LuneZ99](https:/
 /github.com/LuneZ99) | å¿åç¨æ· | thue | [Triones009](https://github.com/
 Triones009) | **[adaaaaaa](https://github.com/adaaaaaa)** | **[LeslieWuboy]
-(https://github.com/LeslieWuboy)** | | ----- | --------------------------------
------------------ | ------------------------------------- | -------- | ---- | -
------------------------------------------- | ----------------------------------
---------- | ------------------------------------------------- | | | | | | | | |
-| ---------------------------------------------------------------------- > ##
-Star History [![Star History Chart](https://api.star-history.com/
-svg?repos=1nchaos/adata&type=Date)](https://star-history.com/#1nchaos/
-adata&Date) ## æ¬¢è¿è¿è¡äº¤æµ
+(https://github.com/LeslieWuboy)** | [yinzhengxin](https://github.com/
+yinzhengxin) | | ------------------------------------- | ----------------------
+--------------------------- | --------------------------------------------- | -
+------- | ---- | ------------------------------------------- | ----------------
+--------------------------- | ------------------------------------------------
+- | --------------------------------------------- | | [yxm0513](https://
+github.com/yxm0513) | [hanxuanliang](https://github.com/hanxuanliang) |
+[akihara-sam](https://github.com/akihara-sam) | | | | | | | -------------------
+--------------------------------------------------- > ## Star History [![Star
+History Chart](https://api.star-history.com/svg?repos=1nchaos/adata&type=Date)]
+(https://star-history.com/#1nchaos/adata&Date) ## æ¬¢è¿è¿è¡äº¤æµ
                                     _[_l_o_g_o_]
 - æ·»å wxå¥½åï¼å¤æ³¨ï¼Adataéåè¿äº¤æµç¾¤ï¼ -
 ç¾¤æè¿å»ºç«ï¼æå¨æä¾ä¸ä¸ªäº¤æµçå¹³å°ï¼æ¬¢è¿è®¨è®ºäº¤æµï¼ -
 ä¸èµ·ä¿å«3000ç¹ç´å°çªç ´6124ç¹ã
```

### Comparing `adata-2.0.1b0/README.md` & `adata-2.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -132,14 +132,15 @@
 ### （1）股票-Stock
 
 #### 	1. 基本信息
 
 | 数据             | API                                   | 说明                                   | 备注                                                         |
 | ---------------- | ------------------------------------- | -------------------------------------- | ------------------------------------------------------------ |
 | A股代码          | stock.info.all_code()                 | 所有A股代码信息                        |                                                              |
+| 股本信息         | stock.info.get_stock_shares()         | 获取单只股票的股本信息                 | 来源：东方财富                                               |
 | **概念**         |                                       |                                        |                                                              |
 | 来源：同花顺     |                                       |                                        |                                                              |
 | 概念代码         | stock.info.all_concept_code_ths()     | 所有A股概念代码信息（同花顺）          | 来源：同花顺公开数据                                         |
 | 概念成分列表     | stock.info.concept_constituent_ths()  | 获取同花顺概念指数的成分股（同花顺）   | 注意：返回结果只有股票代码和股票简称，可根据概念名称查询     |
 | 股票所属概念     | stock.info.get_concept_ths()          | 获取单只股票所属的概念板块             | [F10](https://basic.10jqka.com.cn/300033/concept.html)       |
 | 来源：东方财富   |                                       |                                        |                                                              |
 | 概念代码         | stock.info.all_concept_code_east()    | 所有A股概念代码信息（东方财富）        | 来源：[东方财富](https://data.eastmoney.com/bkzj/gn.html)    |
@@ -188,29 +189,32 @@
 | ------- | ------------------------------------ | -------------------------------- | ---------------------------------------- |
 | ETF行情 | fund.market.get_market_etf()         | 获取ETF的行情信息-日、周、月 k线 | 来源：[同花顺](https://m.10jqka.com.cn/) |
 |         | fund.market.get_market_etf_min()     | 获取ETF的行情-当日分时           |                                          |
 |         | fund.market.get_market_etf_current() | 获取当前的ETF行情                | 实时行情                                 |
 
 ### （3）债券-Bond
 
-| 数据           | API                          | 说明                                | 备注                                                   |
-| -------------- | ---------------------------- | ----------------------------------- | ------------------------------------------------------ |
-| 可转债代码     | bond.info.all_convert_code() | 获取所有A股市场的可转换债券代码信息 | 来源：1. [同花顺](http://data.10jqka.com.cn/ipo/bond/) |
-| 其它数据排期中 | TODO                         | 若您有相关资源可以一起参与贡献      |                                                        |
+| 数据       | API                               | 说明                                | 备注                                                   |
+| ---------- | --------------------------------- | ----------------------------------- | ------------------------------------------------------ |
+| 可转债代码 | bond.info.all_convert_code()      | 获取所有A股市场的可转换债券代码信息 | 来源：1. [同花顺](http://data.10jqka.com.cn/ipo/bond/) |
+| 可转债行情 | bond.market.list_market_current() | 获取A股市场的可转换债券最新行情     | 来源：新浪                                             |
 
 ### （4）舆情
 
 | 数据                     | API                                  | 说明                                       | 备注                                                         |
 | ------------------------ | ------------------------------------ | ------------------------------------------ | ------------------------------------------------------------ |
 | 最近一个月的股票解禁列表 | sentiment.stock_lifting_last_month() | 查询最近一个月的股票解禁列表               | 来源：1. [同花顺](http://data.10jqka.com.cn/market/xsjj/)    |
 | 全市场融资融券余额列表   | sentiment.securities_margin()        | 查询全市场融资融券余额列表                 | 来源：1. [东方财富](https://data.eastmoney.com/rzrq/)        |
 | **北向资金-行情**        |                                      |                                            |                                                              |
 |                          | sentiment.north.north_flow_current() | 获取北向资金（沪深港通）当前流入资金的行情 | 来源：1.[东方财富](https://data.eastmoney.com/hsgt/index.html) |
 |                          | sentiment.north.north_flow_min()     | 获取北向资金分时行情                       |                                                              |
 |                          | sentiment.north.north_flow()         | 获取北向资金历史流入行情                   |                                                              |
+| **热度榜单**             | sentiment.hot.pop_rank_100_east      | 东方财富人气100榜单                        | 来源：[东方财富](http://guba.eastmoney.com/rank/)            |
+|                          | sentiment.hot.hot_rank_100_ths()     | 同花顺热度100排行榜                        | 来源：[同花顺](https://dq.10jqka.com.cn/fuyao/hot_list_data/out/hot_list/v1/stock?stock_type=a&type=hour&list_type=normal) |
+|                          | sentiment.hot.hot_concept_20_ths()   | 同花顺热门概念板块20排行榜                 | 来源：[同花顺](https://dq.10jqka.com.cn/fuyao/hot_list_data/out/hot_list/v1/stock?stock_type=a&type=hour&list_type=normal) |
 | 其它数据排期中           | TODO                                 | 若您有相关资源可以一起参与贡献             |                                                              |
 
 ## 三、[数据源](https://adata.30006124.xyz/dataSource.html)
 
 | 数据源     | 板块                                                         | 描述             |
 | ---------- | ------------------------------------------------------------ | ---------------- |
 | 同花顺     | [数据中心](http://data.10jqka.com.cn/)，[行情中心](http://q.10jqka.com.cn/)，[问财](http://www.iwencai.com/unifiedwap/home/index) | 让投资变的更简单 |
@@ -258,17 +262,17 @@
 4.  新建 Pull Request
 
 
 ## 特别鸣谢
 
 > 对于项目有支持，包括但不仅限：内容贡献，bug提交，思想交流等等，对项目有影响的个人和机构
 
-| Simon | [bigbigbigfish](https://github.com/bigbigbigfish) | [LuneZ99](https://github.com/LuneZ99) | 匿名用户 | thue | [Triones009](https://github.com/Triones009) | **[adaaaaaa](https://github.com/adaaaaaa)** | **[LeslieWuboy](https://github.com/LeslieWuboy)** |
-| ----- | ------------------------------------------------- | ------------------------------------- | -------- | ---- | ------------------------------------------- | ------------------------------------------- | ------------------------------------------------- |
-|       |                                                   |                                       |          |      |                                             |                                             |                                                   |
+| Simon                                 | [bigbigbigfish](https://github.com/bigbigbigfish) | [LuneZ99](https://github.com/LuneZ99)         | 匿名用户 | thue | [Triones009](https://github.com/Triones009) | **[adaaaaaa](https://github.com/adaaaaaa)** | **[LeslieWuboy](https://github.com/LeslieWuboy)** | [yinzhengxin](https://github.com/yinzhengxin) |
+| ------------------------------------- | ------------------------------------------------- | --------------------------------------------- | -------- | ---- | ------------------------------------------- | ------------------------------------------- | ------------------------------------------------- | --------------------------------------------- |
+| [yxm0513](https://github.com/yxm0513) | [hanxuanliang](https://github.com/hanxuanliang)   | [akihara-sam](https://github.com/akihara-sam) |          |      |                                             |                                             |                                                   |                                               |
 
 ----------------------------------------------------------------------
 
 > 
 ## Star History
 
 [![Star History Chart](https://api.star-history.com/svg?repos=1nchaos/adata&type=Date)](https://star-history.com/#1nchaos/adata&Date)
```

#### html2text {}

```diff
@@ -60,16 +60,18 @@
 ## äºã[æ°æ®åè¡¨](https://adata.30006124.xyz/dic/dataList.html)
 æ´çäºææ°çæ¬çæ°æ®åè¡¨åç¸å³ä½¿ç¨Apiï¼è¯¦ç»åå®¹åç¸å³ä½¿ç¨åæ°ï¼è¯·åèæ°æ®å­å¸ææ¡£ã
 - [æ°æ®åè¡¨](https://adata.30006124.xyz/dic/dataList.html) - [æ°æ®å­å¸]
 (https://adata.30006124.xyz/dic/stockInfo.html) ### ï¼1ï¼è¡ç¥¨-Stock #### 1.
 åºæ¬ä¿¡æ¯ | æ°æ® | API | è¯´æ | å¤æ³¨ | | ---------------- | ----------
 --------------------------- | -------------------------------------- | --------
 ---------------------------------------------------- | | Aè¡ä»£ç  |
-stock.info.all_code() | ææAè¡ä»£ç ä¿¡æ¯ | | | **æ¦å¿µ** | | | | |
-æ¥æºï¼åè±é¡º | | | | | æ¦å¿µä»£ç  | stock.info.all_concept_code_ths() |
+stock.info.all_code() | ææAè¡ä»£ç ä¿¡æ¯ | | | è¡æ¬ä¿¡æ¯ |
+stock.info.get_stock_shares() | è·åååªè¡ç¥¨çè¡æ¬ä¿¡æ¯ |
+æ¥æºï¼ä¸æ¹è´¢å¯ | | **æ¦å¿µ** | | | | | æ¥æºï¼åè±é¡º | | | | |
+æ¦å¿µä»£ç  | stock.info.all_concept_code_ths() |
 ææAè¡æ¦å¿µä»£ç ä¿¡æ¯ï¼åè±é¡ºï¼ | æ¥æºï¼åè±é¡ºå¬å¼æ°æ® |
 | æ¦å¿µæååè¡¨ | stock.info.concept_constituent_ths() |
 è·ååè±é¡ºæ¦å¿µææ°çæåè¡ï¼åè±é¡ºï¼ |
 æ³¨æï¼è¿åç»æåªæè¡ç¥¨ä»£ç åè¡ç¥¨ç®ç§°ï¼å¯æ ¹æ®æ¦å¿µåç§°æ¥è¯¢
 | | è¡ç¥¨æå±æ¦å¿µ | stock.info.get_concept_ths() |
 è·åååªè¡ç¥¨æå±çæ¦å¿µæ¿å | [F10](https://basic.10jqka.com.cn/
 300033/concept.html) | | æ¥æºï¼ä¸æ¹è´¢å¯ | | | | | æ¦å¿µä»£ç  |
@@ -132,48 +134,58 @@
 quote.eastmoney.com/center/gridlist.html#fund_etf) | #### 2. è¡æä¿¡æ¯ |
 æ°æ® | API | è¯´æ | å¤æ³¨ | | ------- | ----------------------------------
 -- | -------------------------------- | ---------------------------------------
 - | | ETFè¡æ | fund.market.get_market_etf() | è·åETFçè¡æä¿¡æ¯-
 æ¥ãå¨ãæ kçº¿ | æ¥æºï¼[åè±é¡º](https://m.10jqka.com.cn/) | | |
 fund.market.get_market_etf_min() | è·åETFçè¡æ-å½æ¥åæ¶ | | | |
 fund.market.get_market_etf_current() | è·åå½åçETFè¡æ | å®æ¶è¡æ
-| ### ï¼3ï¼åºå¸-Bond | æ°æ® | API | è¯´æ | å¤æ³¨ | | -------------- |
----------------------------- | ----------------------------------- | ----------
--------------------------------------------- | | å¯è½¬åºä»£ç  |
+| ### ï¼3ï¼åºå¸-Bond | æ°æ® | API | è¯´æ | å¤æ³¨ | | ---------- | ----
+----------------------------- | ----------------------------------- | ---------
+--------------------------------------------- | | å¯è½¬åºä»£ç  |
 bond.info.all_convert_code() |
 è·åææAè¡å¸åºçå¯è½¬æ¢åºå¸ä»£ç ä¿¡æ¯ | æ¥æºï¼1. [åè±é¡º]
-(http://data.10jqka.com.cn/ipo/bond/) | | å¶å®æ°æ®ææä¸­ | TODO |
-è¥æ¨æç¸å³èµæºå¯ä»¥ä¸èµ·åä¸è´¡ç® | | ### ï¼4ï¼èæ | æ°æ® |
-API | è¯´æ | å¤æ³¨ | | ------------------------ | --------------------------
----------- | ------------------------------------------ | ---------------------
---------------------------------------- | |
+(http://data.10jqka.com.cn/ipo/bond/) | | å¯è½¬åºè¡æ |
+bond.market.list_market_current() |
+è·åAè¡å¸åºçå¯è½¬æ¢åºå¸ææ°è¡æ | æ¥æºï¼æ°æµª | ###
+ï¼4ï¼èæ | æ°æ® | API | è¯´æ | å¤æ³¨ | | ------------------------ | -
+----------------------------------- | -----------------------------------------
+- | ------------------------------------------------------------ | |
 æè¿ä¸ä¸ªæçè¡ç¥¨è§£ç¦åè¡¨ | sentiment.stock_lifting_last_month() |
 æ¥è¯¢æè¿ä¸ä¸ªæçè¡ç¥¨è§£ç¦åè¡¨ | æ¥æºï¼1. [åè±é¡º](http://
 data.10jqka.com.cn/market/xsjj/) | | å¨å¸åºèèµèå¸ä½é¢åè¡¨ |
 sentiment.securities_margin() | æ¥è¯¢å¨å¸åºèèµèå¸ä½é¢åè¡¨ |
 æ¥æºï¼1. [ä¸æ¹è´¢å¯](https://data.eastmoney.com/rzrq/) | |
 **ååèµé-è¡æ** | | | | | | sentiment.north.north_flow_current() |
 è·åååèµéï¼æ²ªæ·±æ¸¯éï¼å½åæµå¥èµéçè¡æ | æ¥æºï¼1.
 [ä¸æ¹è´¢å¯](https://data.eastmoney.com/hsgt/index.html) | | |
 sentiment.north.north_flow_min() | è·åååèµéåæ¶è¡æ | | | |
 sentiment.north.north_flow() | è·åååèµéåå²æµå¥è¡æ | | |
-å¶å®æ°æ®ææä¸­ | TODO | è¥æ¨æç¸å³èµæºå¯ä»¥ä¸èµ·åä¸è´¡ç® |
-| ## ä¸ã[æ°æ®æº](https://adata.30006124.xyz/dataSource.html) | æ°æ®æº
-| æ¿å | æè¿° | | ---------- | --------------------------------------------
----------------- | ---------------- | | åè±é¡º | [æ°æ®ä¸­å¿](http://
-data.10jqka.com.cn/)ï¼[è¡æä¸­å¿](http://q.10jqka.com.cn/)ï¼[é®è´¢](http:
-//www.iwencai.com/unifiedwap/home/index) | è®©æèµåçæ´ç®å | |
-ç¾åº¦è¡å¸é | [è¡å¸é](https://gushitong.baidu.com/) |
-ç§æè®©æèµæ´ç®å | | ä¸æ¹è´¢å¯ | [æ°æ®ä¸­å¿](https://
-data.eastmoney.com/center/)ï¼[è¡æä¸­å¿](http://quote.eastmoney.com/center/
-) | è´¢ç»é¨æ· | | è¾è®¯çè´¢ | [è¡æä¸­å¿](https://
-stockapp.finance.qq.com/mstats/#) | | | æ°æµªè´¢ç» | [æ°æµªè´¢ç»](https://
-finance.sina.com.cn/stock/) | é¨æ·ç½ç« | ***-------------------------------
--------------æè°¢åä½å¤§åæä¾çæ°æ®---------------------------------
--------------*** ## åã å¶å®åè
+**ç­åº¦æ¦å** | sentiment.hot.pop_rank_100_east |
+ä¸æ¹è´¢å¯äººæ°100æ¦å | æ¥æºï¼[ä¸æ¹è´¢å¯](http://
+guba.eastmoney.com/rank/) | | | sentiment.hot.hot_rank_100_ths() |
+åè±é¡ºç­åº¦100æè¡æ¦ | æ¥æºï¼[åè±é¡º](https://dq.10jqka.com.cn/
+fuyao/hot_list_data/out/hot_list/v1/
+stock?stock_type=a&type=hour&list_type=normal) | | |
+sentiment.hot.hot_concept_20_ths() | åè±é¡ºç­é¨æ¦å¿µæ¿å20æè¡æ¦ |
+æ¥æºï¼[åè±é¡º](https://dq.10jqka.com.cn/fuyao/hot_list_data/out/hot_list/
+v1/stock?stock_type=a&type=hour&list_type=normal) | | å¶å®æ°æ®ææä¸­ |
+TODO | è¥æ¨æç¸å³èµæºå¯ä»¥ä¸èµ·åä¸è´¡ç® | | ## ä¸ã[æ°æ®æº]
+(https://adata.30006124.xyz/dataSource.html) | æ°æ®æº | æ¿å | æè¿° | |
+---------- | ------------------------------------------------------------ | ---
+------------- | | åè±é¡º | [æ°æ®ä¸­å¿](http://data.10jqka.com.cn/)ï¼
+[è¡æä¸­å¿](http://q.10jqka.com.cn/)ï¼[é®è´¢](http://www.iwencai.com/
+unifiedwap/home/index) | è®©æèµåçæ´ç®å | | ç¾åº¦è¡å¸é |
+[è¡å¸é](https://gushitong.baidu.com/) | ç§æè®©æèµæ´ç®å | |
+ä¸æ¹è´¢å¯ | [æ°æ®ä¸­å¿](https://data.eastmoney.com/center/)ï¼
+[è¡æä¸­å¿](http://quote.eastmoney.com/center/) | è´¢ç»é¨æ· | |
+è¾è®¯çè´¢ | [è¡æä¸­å¿](https://stockapp.finance.qq.com/mstats/#) | | |
+æ°æµªè´¢ç» | [æ°æµªè´¢ç»](https://finance.sina.com.cn/stock/) |
+é¨æ·ç½ç« | ***--------------------------------------------
+æè°¢åä½å¤§åæä¾çæ°æ®----------------------------------------------
+*** ## åã å¶å®åè
 ä¸»è¦è®°å½æ¥éè¿çé¡¹ç®åç¸å³å¹³å°ï¼å¹¶å¯¹æ­¤é¡¹ç®äº§çäºæ·±è¿å°è±¡ï¼ç¹æ­¤é¸£è°¢ã
 | [akshare](https://gitee.com/mirrors/akshare) | [èå®½éå](https://
 www.joinquant.com/) | [baostock](http://baostock.com/baostock/index.php/
 Python%E5%BC%80%E5%8F%91%E8%B5%84%E6%BA%90) | [MyData](http://api.mairui.club/
 hsdata.html) | | -------------------------------------------- | ---------------
 ----------------------- | -----------------------------------------------------
 ------- | -------------------------------------------- | ## äºãåå¸è®¡å
@@ -194,19 +206,22 @@
 1. Fork æ¬ä»åº 2. æ°å»º Feat_xxx åæ¯ 3.
 æäº¤ä»£ç ï¼æ³¨æä»£ç é£æ ¼åæ¬é¡¹ç®ä¸è´å³å¯ï¼ 4. æ°å»º Pull
 Request ## ç¹å«é¸£è°¢ >
 å¯¹äºé¡¹ç®ææ¯æï¼åæ¬ä½ä¸ä»éï¼åå®¹è´¡ç®ï¼bugæäº¤ï¼ææ³äº¤æµç­ç­ï¼å¯¹é¡¹ç®æå½±åçä¸ªäººåæºæ
 | Simon | [bigbigbigfish](https://github.com/bigbigbigfish) | [LuneZ99](https:/
 /github.com/LuneZ99) | å¿åç¨æ· | thue | [Triones009](https://github.com/
 Triones009) | **[adaaaaaa](https://github.com/adaaaaaa)** | **[LeslieWuboy]
-(https://github.com/LeslieWuboy)** | | ----- | --------------------------------
------------------ | ------------------------------------- | -------- | ---- | -
------------------------------------------- | ----------------------------------
---------- | ------------------------------------------------- | | | | | | | | |
-| ---------------------------------------------------------------------- > ##
-Star History [![Star History Chart](https://api.star-history.com/
-svg?repos=1nchaos/adata&type=Date)](https://star-history.com/#1nchaos/
-adata&Date) ## æ¬¢è¿è¿è¡äº¤æµ
+(https://github.com/LeslieWuboy)** | [yinzhengxin](https://github.com/
+yinzhengxin) | | ------------------------------------- | ----------------------
+--------------------------- | --------------------------------------------- | -
+------- | ---- | ------------------------------------------- | ----------------
+--------------------------- | ------------------------------------------------
+- | --------------------------------------------- | | [yxm0513](https://
+github.com/yxm0513) | [hanxuanliang](https://github.com/hanxuanliang) |
+[akihara-sam](https://github.com/akihara-sam) | | | | | | | -------------------
+--------------------------------------------------- > ## Star History [![Star
+History Chart](https://api.star-history.com/svg?repos=1nchaos/adata&type=Date)]
+(https://star-history.com/#1nchaos/adata&Date) ## æ¬¢è¿è¿è¡äº¤æµ
                                     _[_l_o_g_o_]
 - æ·»å wxå¥½åï¼å¤æ³¨ï¼Adataéåè¿äº¤æµç¾¤ï¼ -
 ç¾¤æè¿å»ºç«ï¼æå¨æä¾ä¸ä¸ªäº¤æµçå¹³å°ï¼æ¬¢è¿è®¨è®ºäº¤æµï¼ -
 ä¸èµ·ä¿å«3000ç¹ç´å°çªç ´6124ç¹ã
```

### Comparing `adata-2.0.1b0/adata/__init__.py` & `adata-2.1.0/adata/__init__.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/__version__.py` & `adata-2.1.0/adata/__version__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
-VERSION = (2, 0, 1)
-PRERELEASE = 'beta'  # alpha, beta or rc
+VERSION = (2, 1, 0)
+PRERELEASE = None  # alpha, beta or rc
 REVISION = None
 
 
 def generate_version(version, prerelease=None, revision=None):
     version_parts = [".".join(map(str, version))]
     if prerelease is not None:
         version_parts.append(f"-{prerelease}")
```

### Comparing `adata-2.0.1b0/adata/bond/info/bond_code.py` & `adata-2.1.0/adata/bond/info/bond_code.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/common/base/base_ths.py` & `adata-2.1.0/adata/common/base/base_ths.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/common/headers/__init__.py` & `adata-2.1.0/adata/common/headers/__init__.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/common/headers/baidu_headers.py` & `adata-2.1.0/adata/common/headers/baidu_headers.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/common/headers/east_headers.py` & `adata-2.1.0/adata/common/headers/east_headers.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/common/headers/sina_headers.py` & `adata-2.1.0/adata/common/headers/sina_headers.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/common/headers/ths_headers.py` & `adata-2.1.0/adata/common/headers/ths_headers.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/common/js/hexin.js` & `adata-2.1.0/adata/common/js/hexin.js`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/common/js/ths.js` & `adata-2.1.0/adata/common/js/ths.js`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/common/utils/cookie.py` & `adata-2.1.0/adata/common/utils/cookie.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/common/utils/snowflake.py` & `adata-2.1.0/adata/common/utils/snowflake.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/common/utils/sunrequests.py` & `adata-2.1.0/adata/common/utils/sunrequests.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/fund/info/fund_info.py` & `adata-2.1.0/adata/fund/info/fund_info.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/fund/market/etf_market.py` & `adata-2.1.0/adata/fund/market/etf_market.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/fund/market/etf_market_template.py` & `adata-2.1.0/adata/fund/market/etf_market_template.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/fund/market/etf_market_ths.py` & `adata-2.1.0/adata/fund/market/etf_market_ths.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/sentiment/north_flow.py` & `adata-2.1.0/adata/sentiment/north_flow.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/sentiment/securities_margin.py` & `adata-2.1.0/adata/sentiment/securities_margin.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/sentiment/stock_lifting.py` & `adata-2.1.0/adata/sentiment/stock_lifting.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/cache/calendar/2005.csv` & `adata-2.1.0/adata/stock/cache/calendar/2005.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/cache/calendar/2006.csv` & `adata-2.1.0/adata/stock/cache/calendar/2006.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/cache/calendar/2007.csv` & `adata-2.1.0/adata/stock/cache/calendar/2007.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/cache/calendar/2008.csv` & `adata-2.1.0/adata/stock/cache/calendar/2008.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/cache/calendar/2009.csv` & `adata-2.1.0/adata/stock/cache/calendar/2009.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/cache/calendar/2010.csv` & `adata-2.1.0/adata/stock/cache/calendar/2010.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/cache/calendar/2011.csv` & `adata-2.1.0/adata/stock/cache/calendar/2011.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/cache/calendar/2012.csv` & `adata-2.1.0/adata/stock/cache/calendar/2012.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/cache/calendar/2013.csv` & `adata-2.1.0/adata/stock/cache/calendar/2013.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/cache/calendar/2014.csv` & `adata-2.1.0/adata/stock/cache/calendar/2014.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/cache/calendar/2015.csv` & `adata-2.1.0/adata/stock/cache/calendar/2015.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/cache/calendar/2016.csv` & `adata-2.1.0/adata/stock/cache/calendar/2016.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/cache/calendar/2017.csv` & `adata-2.1.0/adata/stock/cache/calendar/2017.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/cache/calendar/2018.csv` & `adata-2.1.0/adata/stock/cache/calendar/2018.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/cache/calendar/2019.csv` & `adata-2.1.0/adata/stock/cache/calendar/2019.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/cache/calendar/2020.csv` & `adata-2.1.0/adata/stock/cache/calendar/2020.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/cache/calendar/2021.csv` & `adata-2.1.0/adata/stock/cache/calendar/2021.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/cache/calendar/2022.csv` & `adata-2.1.0/adata/stock/cache/calendar/2022.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/cache/calendar/2023.csv` & `adata-2.1.0/adata/stock/cache/calendar/2023.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/cache/calendar/2024.csv` & `adata-2.1.0/adata/stock/cache/calendar/2024.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/cache/code.csv` & `adata-2.1.0/adata/stock/cache/code.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/cache/index_code_rel_ths.py` & `adata-2.1.0/adata/stock/cache/index_code_rel_ths.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/info/concept/stock_concept_east.py` & `adata-2.1.0/adata/stock/info/concept/stock_concept_east.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/info/concept/stock_concept_ths.py` & `adata-2.1.0/adata/stock/info/concept/stock_concept_ths.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/info/stock_code.py` & `adata-2.1.0/adata/stock/info/stock_code.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/info/stock_index.py` & `adata-2.1.0/adata/stock/info/stock_index.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/info/trade_calendar.py` & `adata-2.1.0/adata/stock/info/trade_calendar.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/market/__init__.py` & `adata-2.1.0/adata/stock/market/__init__.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/market/concepth_market/concept_market_east.py` & `adata-2.1.0/adata/stock/market/concepth_market/concept_market_east.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/market/concepth_market/concept_market_template.py` & `adata-2.1.0/adata/stock/market/concepth_market/concept_market_template.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/market/concepth_market/concept_market_ths.py` & `adata-2.1.0/adata/stock/market/concepth_market/concept_market_ths.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/market/index_market/market_index.py` & `adata-2.1.0/adata/stock/market/index_market/market_index.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/market/index_market/market_index_east.py` & `adata-2.1.0/adata/stock/market/index_market/market_index_east.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/market/index_market/market_index_template.py` & `adata-2.1.0/adata/stock/market/index_market/market_index_template.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/market/index_market/market_index_ths.py` & `adata-2.1.0/adata/stock/market/index_market/market_index_ths.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/market/stock_dividend.py` & `adata-2.1.0/adata/stock/market/stock_dividend.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/market/stock_market/stock_market.py` & `adata-2.1.0/adata/stock/market/stock_market/stock_market.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,12 +84,12 @@
         :param stock_code: 股票代码
         :return: 最新当天的分时成交
         """
         return self.baidu.get_market_bar(stock_code=stock_code)
 
 
 if __name__ == '__main__':
-    print(StockMarket().get_market(stock_code='000001', start_date='2021-01-01', k_type=1))
+    print(StockMarket().get_market(stock_code='300416', start_date='2021-01-01', k_type=1))
     print(StockMarket().get_market_min(stock_code='000001'))
     print(StockMarket().list_market_current(code_list=['000001', '600001', '000795', '872925']))
     print(StockMarket().get_market_five(stock_code='000001'))
     print(StockMarket().get_market_bar(stock_code='872925'))
```

### Comparing `adata-2.0.1b0/adata/stock/market/stock_market/stock_market_baidu.py` & `adata-2.1.0/adata/stock/market/stock_market/stock_market_baidu.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/market/stock_market/stock_market_qq.py` & `adata-2.1.0/adata/stock/market/stock_market/stock_market_qq.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/market/stock_market/stock_market_sina.py` & `adata-2.1.0/adata/stock/market/stock_market/stock_market_sina.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata/stock/market/stock_market/stock_market_template.py` & `adata-2.1.0/adata/stock/market/stock_market/stock_market_template.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.1b0/adata.egg-info/PKG-INFO` & `adata-2.1.0/adata.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adata
-Version: 2.0.1b0
+Version: 2.1.0
 Summary: A Data,A Stock,ETF,Bond,Quant,Stock Market,K Line
 Home-page: https://github.com/1nchaos/adata
 Author: 1nchaos
 Author-email: 9527@1nchaos.com
 License: Apache License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
@@ -151,14 +151,15 @@
 ### （1）股票-Stock
 
 #### 	1. 基本信息
 
 | 数据             | API                                   | 说明                                   | 备注                                                         |
 | ---------------- | ------------------------------------- | -------------------------------------- | ------------------------------------------------------------ |
 | A股代码          | stock.info.all_code()                 | 所有A股代码信息                        |                                                              |
+| 股本信息         | stock.info.get_stock_shares()         | 获取单只股票的股本信息                 | 来源：东方财富                                               |
 | **概念**         |                                       |                                        |                                                              |
 | 来源：同花顺     |                                       |                                        |                                                              |
 | 概念代码         | stock.info.all_concept_code_ths()     | 所有A股概念代码信息（同花顺）          | 来源：同花顺公开数据                                         |
 | 概念成分列表     | stock.info.concept_constituent_ths()  | 获取同花顺概念指数的成分股（同花顺）   | 注意：返回结果只有股票代码和股票简称，可根据概念名称查询     |
 | 股票所属概念     | stock.info.get_concept_ths()          | 获取单只股票所属的概念板块             | [F10](https://basic.10jqka.com.cn/300033/concept.html)       |
 | 来源：东方财富   |                                       |                                        |                                                              |
 | 概念代码         | stock.info.all_concept_code_east()    | 所有A股概念代码信息（东方财富）        | 来源：[东方财富](https://data.eastmoney.com/bkzj/gn.html)    |
@@ -207,29 +208,32 @@
 | ------- | ------------------------------------ | -------------------------------- | ---------------------------------------- |
 | ETF行情 | fund.market.get_market_etf()         | 获取ETF的行情信息-日、周、月 k线 | 来源：[同花顺](https://m.10jqka.com.cn/) |
 |         | fund.market.get_market_etf_min()     | 获取ETF的行情-当日分时           |                                          |
 |         | fund.market.get_market_etf_current() | 获取当前的ETF行情                | 实时行情                                 |
 
 ### （3）债券-Bond
 
-| 数据           | API                          | 说明                                | 备注                                                   |
-| -------------- | ---------------------------- | ----------------------------------- | ------------------------------------------------------ |
-| 可转债代码     | bond.info.all_convert_code() | 获取所有A股市场的可转换债券代码信息 | 来源：1. [同花顺](http://data.10jqka.com.cn/ipo/bond/) |
-| 其它数据排期中 | TODO                         | 若您有相关资源可以一起参与贡献      |                                                        |
+| 数据       | API                               | 说明                                | 备注                                                   |
+| ---------- | --------------------------------- | ----------------------------------- | ------------------------------------------------------ |
+| 可转债代码 | bond.info.all_convert_code()      | 获取所有A股市场的可转换债券代码信息 | 来源：1. [同花顺](http://data.10jqka.com.cn/ipo/bond/) |
+| 可转债行情 | bond.market.list_market_current() | 获取A股市场的可转换债券最新行情     | 来源：新浪                                             |
 
 ### （4）舆情
 
 | 数据                     | API                                  | 说明                                       | 备注                                                         |
 | ------------------------ | ------------------------------------ | ------------------------------------------ | ------------------------------------------------------------ |
 | 最近一个月的股票解禁列表 | sentiment.stock_lifting_last_month() | 查询最近一个月的股票解禁列表               | 来源：1. [同花顺](http://data.10jqka.com.cn/market/xsjj/)    |
 | 全市场融资融券余额列表   | sentiment.securities_margin()        | 查询全市场融资融券余额列表                 | 来源：1. [东方财富](https://data.eastmoney.com/rzrq/)        |
 | **北向资金-行情**        |                                      |                                            |                                                              |
 |                          | sentiment.north.north_flow_current() | 获取北向资金（沪深港通）当前流入资金的行情 | 来源：1.[东方财富](https://data.eastmoney.com/hsgt/index.html) |
 |                          | sentiment.north.north_flow_min()     | 获取北向资金分时行情                       |                                                              |
 |                          | sentiment.north.north_flow()         | 获取北向资金历史流入行情                   |                                                              |
+| **热度榜单**             | sentiment.hot.pop_rank_100_east      | 东方财富人气100榜单                        | 来源：[东方财富](http://guba.eastmoney.com/rank/)            |
+|                          | sentiment.hot.hot_rank_100_ths()     | 同花顺热度100排行榜                        | 来源：[同花顺](https://dq.10jqka.com.cn/fuyao/hot_list_data/out/hot_list/v1/stock?stock_type=a&type=hour&list_type=normal) |
+|                          | sentiment.hot.hot_concept_20_ths()   | 同花顺热门概念板块20排行榜                 | 来源：[同花顺](https://dq.10jqka.com.cn/fuyao/hot_list_data/out/hot_list/v1/stock?stock_type=a&type=hour&list_type=normal) |
 | 其它数据排期中           | TODO                                 | 若您有相关资源可以一起参与贡献             |                                                              |
 
 ## 三、[数据源](https://adata.30006124.xyz/dataSource.html)
 
 | 数据源     | 板块                                                         | 描述             |
 | ---------- | ------------------------------------------------------------ | ---------------- |
 | 同花顺     | [数据中心](http://data.10jqka.com.cn/)，[行情中心](http://q.10jqka.com.cn/)，[问财](http://www.iwencai.com/unifiedwap/home/index) | 让投资变的更简单 |
@@ -277,17 +281,17 @@
 4.  新建 Pull Request
 
 
 ## 特别鸣谢
 
 > 对于项目有支持，包括但不仅限：内容贡献，bug提交，思想交流等等，对项目有影响的个人和机构
 
-| Simon | [bigbigbigfish](https://github.com/bigbigbigfish) | [LuneZ99](https://github.com/LuneZ99) | 匿名用户 | thue | [Triones009](https://github.com/Triones009) | **[adaaaaaa](https://github.com/adaaaaaa)** | **[LeslieWuboy](https://github.com/LeslieWuboy)** |
-| ----- | ------------------------------------------------- | ------------------------------------- | -------- | ---- | ------------------------------------------- | ------------------------------------------- | ------------------------------------------------- |
-|       |                                                   |                                       |          |      |                                             |                                             |                                                   |
+| Simon                                 | [bigbigbigfish](https://github.com/bigbigbigfish) | [LuneZ99](https://github.com/LuneZ99)         | 匿名用户 | thue | [Triones009](https://github.com/Triones009) | **[adaaaaaa](https://github.com/adaaaaaa)** | **[LeslieWuboy](https://github.com/LeslieWuboy)** | [yinzhengxin](https://github.com/yinzhengxin) |
+| ------------------------------------- | ------------------------------------------------- | --------------------------------------------- | -------- | ---- | ------------------------------------------- | ------------------------------------------- | ------------------------------------------------- | --------------------------------------------- |
+| [yxm0513](https://github.com/yxm0513) | [hanxuanliang](https://github.com/hanxuanliang)   | [akihara-sam](https://github.com/akihara-sam) |          |      |                                             |                                             |                                                   |                                               |
 
 ----------------------------------------------------------------------
 
 > 
 ## Star History
 
 [![Star History Chart](https://api.star-history.com/svg?repos=1nchaos/adata&type=Date)](https://star-history.com/#1nchaos/adata&Date)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: adata Version: 2.0.1b0 Summary: A Data,A
+Metadata-Version: 2.1 Name: adata Version: 2.1.0 Summary: A Data,A
 Stock,ETF,Bond,Quant,Stock Market,K Line Home-page: https://github.com/1nchaos/
 adata Author: 1nchaos Author-email: 9527@1nchaos.com License: Apache License
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
@@ -69,16 +69,18 @@
 ## äºã[æ°æ®åè¡¨](https://adata.30006124.xyz/dic/dataList.html)
 æ´çäºææ°çæ¬çæ°æ®åè¡¨åç¸å³ä½¿ç¨Apiï¼è¯¦ç»åå®¹åç¸å³ä½¿ç¨åæ°ï¼è¯·åèæ°æ®å­å¸ææ¡£ã
 - [æ°æ®åè¡¨](https://adata.30006124.xyz/dic/dataList.html) - [æ°æ®å­å¸]
 (https://adata.30006124.xyz/dic/stockInfo.html) ### ï¼1ï¼è¡ç¥¨-Stock #### 1.
 åºæ¬ä¿¡æ¯ | æ°æ® | API | è¯´æ | å¤æ³¨ | | ---------------- | ----------
 --------------------------- | -------------------------------------- | --------
 ---------------------------------------------------- | | Aè¡ä»£ç  |
-stock.info.all_code() | ææAè¡ä»£ç ä¿¡æ¯ | | | **æ¦å¿µ** | | | | |
-æ¥æºï¼åè±é¡º | | | | | æ¦å¿µä»£ç  | stock.info.all_concept_code_ths() |
+stock.info.all_code() | ææAè¡ä»£ç ä¿¡æ¯ | | | è¡æ¬ä¿¡æ¯ |
+stock.info.get_stock_shares() | è·åååªè¡ç¥¨çè¡æ¬ä¿¡æ¯ |
+æ¥æºï¼ä¸æ¹è´¢å¯ | | **æ¦å¿µ** | | | | | æ¥æºï¼åè±é¡º | | | | |
+æ¦å¿µä»£ç  | stock.info.all_concept_code_ths() |
 ææAè¡æ¦å¿µä»£ç ä¿¡æ¯ï¼åè±é¡ºï¼ | æ¥æºï¼åè±é¡ºå¬å¼æ°æ® |
 | æ¦å¿µæååè¡¨ | stock.info.concept_constituent_ths() |
 è·ååè±é¡ºæ¦å¿µææ°çæåè¡ï¼åè±é¡ºï¼ |
 æ³¨æï¼è¿åç»æåªæè¡ç¥¨ä»£ç åè¡ç¥¨ç®ç§°ï¼å¯æ ¹æ®æ¦å¿µåç§°æ¥è¯¢
 | | è¡ç¥¨æå±æ¦å¿µ | stock.info.get_concept_ths() |
 è·åååªè¡ç¥¨æå±çæ¦å¿µæ¿å | [F10](https://basic.10jqka.com.cn/
 300033/concept.html) | | æ¥æºï¼ä¸æ¹è´¢å¯ | | | | | æ¦å¿µä»£ç  |
@@ -141,48 +143,58 @@
 quote.eastmoney.com/center/gridlist.html#fund_etf) | #### 2. è¡æä¿¡æ¯ |
 æ°æ® | API | è¯´æ | å¤æ³¨ | | ------- | ----------------------------------
 -- | -------------------------------- | ---------------------------------------
 - | | ETFè¡æ | fund.market.get_market_etf() | è·åETFçè¡æä¿¡æ¯-
 æ¥ãå¨ãæ kçº¿ | æ¥æºï¼[åè±é¡º](https://m.10jqka.com.cn/) | | |
 fund.market.get_market_etf_min() | è·åETFçè¡æ-å½æ¥åæ¶ | | | |
 fund.market.get_market_etf_current() | è·åå½åçETFè¡æ | å®æ¶è¡æ
-| ### ï¼3ï¼åºå¸-Bond | æ°æ® | API | è¯´æ | å¤æ³¨ | | -------------- |
----------------------------- | ----------------------------------- | ----------
--------------------------------------------- | | å¯è½¬åºä»£ç  |
+| ### ï¼3ï¼åºå¸-Bond | æ°æ® | API | è¯´æ | å¤æ³¨ | | ---------- | ----
+----------------------------- | ----------------------------------- | ---------
+--------------------------------------------- | | å¯è½¬åºä»£ç  |
 bond.info.all_convert_code() |
 è·åææAè¡å¸åºçå¯è½¬æ¢åºå¸ä»£ç ä¿¡æ¯ | æ¥æºï¼1. [åè±é¡º]
-(http://data.10jqka.com.cn/ipo/bond/) | | å¶å®æ°æ®ææä¸­ | TODO |
-è¥æ¨æç¸å³èµæºå¯ä»¥ä¸èµ·åä¸è´¡ç® | | ### ï¼4ï¼èæ | æ°æ® |
-API | è¯´æ | å¤æ³¨ | | ------------------------ | --------------------------
----------- | ------------------------------------------ | ---------------------
---------------------------------------- | |
+(http://data.10jqka.com.cn/ipo/bond/) | | å¯è½¬åºè¡æ |
+bond.market.list_market_current() |
+è·åAè¡å¸åºçå¯è½¬æ¢åºå¸ææ°è¡æ | æ¥æºï¼æ°æµª | ###
+ï¼4ï¼èæ | æ°æ® | API | è¯´æ | å¤æ³¨ | | ------------------------ | -
+----------------------------------- | -----------------------------------------
+- | ------------------------------------------------------------ | |
 æè¿ä¸ä¸ªæçè¡ç¥¨è§£ç¦åè¡¨ | sentiment.stock_lifting_last_month() |
 æ¥è¯¢æè¿ä¸ä¸ªæçè¡ç¥¨è§£ç¦åè¡¨ | æ¥æºï¼1. [åè±é¡º](http://
 data.10jqka.com.cn/market/xsjj/) | | å¨å¸åºèèµèå¸ä½é¢åè¡¨ |
 sentiment.securities_margin() | æ¥è¯¢å¨å¸åºèèµèå¸ä½é¢åè¡¨ |
 æ¥æºï¼1. [ä¸æ¹è´¢å¯](https://data.eastmoney.com/rzrq/) | |
 **ååèµé-è¡æ** | | | | | | sentiment.north.north_flow_current() |
 è·åååèµéï¼æ²ªæ·±æ¸¯éï¼å½åæµå¥èµéçè¡æ | æ¥æºï¼1.
 [ä¸æ¹è´¢å¯](https://data.eastmoney.com/hsgt/index.html) | | |
 sentiment.north.north_flow_min() | è·åååèµéåæ¶è¡æ | | | |
 sentiment.north.north_flow() | è·åååèµéåå²æµå¥è¡æ | | |
-å¶å®æ°æ®ææä¸­ | TODO | è¥æ¨æç¸å³èµæºå¯ä»¥ä¸èµ·åä¸è´¡ç® |
-| ## ä¸ã[æ°æ®æº](https://adata.30006124.xyz/dataSource.html) | æ°æ®æº
-| æ¿å | æè¿° | | ---------- | --------------------------------------------
----------------- | ---------------- | | åè±é¡º | [æ°æ®ä¸­å¿](http://
-data.10jqka.com.cn/)ï¼[è¡æä¸­å¿](http://q.10jqka.com.cn/)ï¼[é®è´¢](http:
-//www.iwencai.com/unifiedwap/home/index) | è®©æèµåçæ´ç®å | |
-ç¾åº¦è¡å¸é | [è¡å¸é](https://gushitong.baidu.com/) |
-ç§æè®©æèµæ´ç®å | | ä¸æ¹è´¢å¯ | [æ°æ®ä¸­å¿](https://
-data.eastmoney.com/center/)ï¼[è¡æä¸­å¿](http://quote.eastmoney.com/center/
-) | è´¢ç»é¨æ· | | è¾è®¯çè´¢ | [è¡æä¸­å¿](https://
-stockapp.finance.qq.com/mstats/#) | | | æ°æµªè´¢ç» | [æ°æµªè´¢ç»](https://
-finance.sina.com.cn/stock/) | é¨æ·ç½ç« | ***-------------------------------
--------------æè°¢åä½å¤§åæä¾çæ°æ®---------------------------------
--------------*** ## åã å¶å®åè
+**ç­åº¦æ¦å** | sentiment.hot.pop_rank_100_east |
+ä¸æ¹è´¢å¯äººæ°100æ¦å | æ¥æºï¼[ä¸æ¹è´¢å¯](http://
+guba.eastmoney.com/rank/) | | | sentiment.hot.hot_rank_100_ths() |
+åè±é¡ºç­åº¦100æè¡æ¦ | æ¥æºï¼[åè±é¡º](https://dq.10jqka.com.cn/
+fuyao/hot_list_data/out/hot_list/v1/
+stock?stock_type=a&type=hour&list_type=normal) | | |
+sentiment.hot.hot_concept_20_ths() | åè±é¡ºç­é¨æ¦å¿µæ¿å20æè¡æ¦ |
+æ¥æºï¼[åè±é¡º](https://dq.10jqka.com.cn/fuyao/hot_list_data/out/hot_list/
+v1/stock?stock_type=a&type=hour&list_type=normal) | | å¶å®æ°æ®ææä¸­ |
+TODO | è¥æ¨æç¸å³èµæºå¯ä»¥ä¸èµ·åä¸è´¡ç® | | ## ä¸ã[æ°æ®æº]
+(https://adata.30006124.xyz/dataSource.html) | æ°æ®æº | æ¿å | æè¿° | |
+---------- | ------------------------------------------------------------ | ---
+------------- | | åè±é¡º | [æ°æ®ä¸­å¿](http://data.10jqka.com.cn/)ï¼
+[è¡æä¸­å¿](http://q.10jqka.com.cn/)ï¼[é®è´¢](http://www.iwencai.com/
+unifiedwap/home/index) | è®©æèµåçæ´ç®å | | ç¾åº¦è¡å¸é |
+[è¡å¸é](https://gushitong.baidu.com/) | ç§æè®©æèµæ´ç®å | |
+ä¸æ¹è´¢å¯ | [æ°æ®ä¸­å¿](https://data.eastmoney.com/center/)ï¼
+[è¡æä¸­å¿](http://quote.eastmoney.com/center/) | è´¢ç»é¨æ· | |
+è¾è®¯çè´¢ | [è¡æä¸­å¿](https://stockapp.finance.qq.com/mstats/#) | | |
+æ°æµªè´¢ç» | [æ°æµªè´¢ç»](https://finance.sina.com.cn/stock/) |
+é¨æ·ç½ç« | ***--------------------------------------------
+æè°¢åä½å¤§åæä¾çæ°æ®----------------------------------------------
+*** ## åã å¶å®åè
 ä¸»è¦è®°å½æ¥éè¿çé¡¹ç®åç¸å³å¹³å°ï¼å¹¶å¯¹æ­¤é¡¹ç®äº§çäºæ·±è¿å°è±¡ï¼ç¹æ­¤é¸£è°¢ã
 | [akshare](https://gitee.com/mirrors/akshare) | [èå®½éå](https://
 www.joinquant.com/) | [baostock](http://baostock.com/baostock/index.php/
 Python%E5%BC%80%E5%8F%91%E8%B5%84%E6%BA%90) | [MyData](http://api.mairui.club/
 hsdata.html) | | -------------------------------------------- | ---------------
 ----------------------- | -----------------------------------------------------
 ------- | -------------------------------------------- | ## äºãåå¸è®¡å
@@ -203,19 +215,22 @@
 1. Fork æ¬ä»åº 2. æ°å»º Feat_xxx åæ¯ 3.
 æäº¤ä»£ç ï¼æ³¨æä»£ç é£æ ¼åæ¬é¡¹ç®ä¸è´å³å¯ï¼ 4. æ°å»º Pull
 Request ## ç¹å«é¸£è°¢ >
 å¯¹äºé¡¹ç®ææ¯æï¼åæ¬ä½ä¸ä»éï¼åå®¹è´¡ç®ï¼bugæäº¤ï¼ææ³äº¤æµç­ç­ï¼å¯¹é¡¹ç®æå½±åçä¸ªäººåæºæ
 | Simon | [bigbigbigfish](https://github.com/bigbigbigfish) | [LuneZ99](https:/
 /github.com/LuneZ99) | å¿åç¨æ· | thue | [Triones009](https://github.com/
 Triones009) | **[adaaaaaa](https://github.com/adaaaaaa)** | **[LeslieWuboy]
-(https://github.com/LeslieWuboy)** | | ----- | --------------------------------
------------------ | ------------------------------------- | -------- | ---- | -
------------------------------------------- | ----------------------------------
---------- | ------------------------------------------------- | | | | | | | | |
-| ---------------------------------------------------------------------- > ##
-Star History [![Star History Chart](https://api.star-history.com/
-svg?repos=1nchaos/adata&type=Date)](https://star-history.com/#1nchaos/
-adata&Date) ## æ¬¢è¿è¿è¡äº¤æµ
+(https://github.com/LeslieWuboy)** | [yinzhengxin](https://github.com/
+yinzhengxin) | | ------------------------------------- | ----------------------
+--------------------------- | --------------------------------------------- | -
+------- | ---- | ------------------------------------------- | ----------------
+--------------------------- | ------------------------------------------------
+- | --------------------------------------------- | | [yxm0513](https://
+github.com/yxm0513) | [hanxuanliang](https://github.com/hanxuanliang) |
+[akihara-sam](https://github.com/akihara-sam) | | | | | | | -------------------
+--------------------------------------------------- > ## Star History [![Star
+History Chart](https://api.star-history.com/svg?repos=1nchaos/adata&type=Date)]
+(https://star-history.com/#1nchaos/adata&Date) ## æ¬¢è¿è¿è¡äº¤æµ
                                     _[_l_o_g_o_]
 - æ·»å wxå¥½åï¼å¤æ³¨ï¼Adataéåè¿äº¤æµç¾¤ï¼ -
 ç¾¤æè¿å»ºç«ï¼æå¨æä¾ä¸ä¸ªäº¤æµçå¹³å°ï¼æ¬¢è¿è®¨è®ºäº¤æµï¼ -
 ä¸èµ·ä¿å«3000ç¹ç´å°çªç ´6124ç¹ã
```

### Comparing `adata-2.0.1b0/adata.egg-info/SOURCES.txt` & `adata-2.1.0/adata.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 adata.egg-info/top_level.txt
 adata/bond/__init__.py
 adata/bond/cache/__init__.py
 adata/bond/info/__init__.py
 adata/bond/info/bond_code.py
 adata/bond/market/__init__.py
 adata/bond/market/bond_market.py
+adata/bond/market/bond_market_sina.py
+adata/bond/market/bond_market_template.py
 adata/common/__init__.py
 adata/common/base/__init__.py
 adata/common/base/base_req.py
 adata/common/base/base_ths.py
 adata/common/exception/__init__.py
 adata/common/exception/exception_msg.py
 adata/common/exception/handler.py
@@ -41,14 +43,15 @@
 adata/fund/info/fund_info.py
 adata/fund/market/__init__.py
 adata/fund/market/etf_market.py
 adata/fund/market/etf_market_template.py
 adata/fund/market/etf_market_ths.py
 adata/message/__init__.py
 adata/sentiment/__init__.py
+adata/sentiment/hot.py
 adata/sentiment/north_flow.py
 adata/sentiment/securities_margin.py
 adata/sentiment/stock_lifting.py
 adata/sentiment/cache/__init__.py
 adata/stock/__init__.py
 adata/stock/cache/__init__.py
 adata/stock/cache/code.csv
@@ -76,14 +79,15 @@
 adata/stock/cache/calendar/2024.csv
 adata/stock/cache/calendar/__init__.py
 adata/stock/index/__init__.py
 adata/stock/index/cal_index.py
 adata/stock/info/__init__.py
 adata/stock/info/stock_code.py
 adata/stock/info/stock_index.py
+adata/stock/info/stock_info.py
 adata/stock/info/trade_calendar.py
 adata/stock/info/concept/__init__.py
 adata/stock/info/concept/stock_concept.py
 adata/stock/info/concept/stock_concept_east.py
 adata/stock/info/concept/stock_concept_template.py
 adata/stock/info/concept/stock_concept_ths.py
 adata/stock/market/__init__.py
```

### Comparing `adata-2.0.1b0/setup.py` & `adata-2.1.0/setup.py`

 * *Files identical despite different names*

