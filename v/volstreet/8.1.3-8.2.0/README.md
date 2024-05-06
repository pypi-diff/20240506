# Comparing `tmp/volstreet-8.1.3.tar.gz` & `tmp/volstreet-8.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volstreet-8.1.3.tar", last modified: Mon Apr 29 10:20:18 2024, max compression
+gzip compressed data, was "volstreet-8.2.0.tar", last modified: Mon May  6 03:10:02 2024, max compression
```

## Comparing `volstreet-8.1.3.tar` & `volstreet-8.2.0.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 10:20:18.330154 volstreet-8.1.3/
--rw-rw-rw-   0        0        0     1293 2024-04-29 10:20:18.330154 volstreet-8.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      124 2024-03-14 04:36:05.000000 volstreet-8.1.3/README.md
--rw-rw-rw-   0        0        0       91 2024-03-14 04:36:05.000000 volstreet-8.1.3/pyproject.toml
--rw-rw-rw-   0        0        0     1155 2024-04-29 10:20:18.330154 volstreet-8.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-29 10:20:18.157699 volstreet-8.1.3/volstreet/
--rw-rw-rw-   0        0        0      442 2024-03-14 09:55:16.000000 volstreet-8.1.3/volstreet/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 10:20:18.188961 volstreet-8.1.3/volstreet/angel_interface/
--rw-rw-rw-   0        0        0      247 2024-04-26 02:47:59.000000 volstreet-8.1.3/volstreet/angel_interface/__init__.py
--rw-rw-rw-   0        0        0     3726 2024-04-26 02:48:50.000000 volstreet-8.1.3/volstreet/angel_interface/access_rate_handler.py
--rw-rw-rw-   0        0        0      274 2024-04-23 04:22:25.000000 volstreet-8.1.3/volstreet/angel_interface/active_session.py
--rw-rw-rw-   0        0        0     2843 2024-04-28 03:29:15.000000 volstreet-8.1.3/volstreet/angel_interface/async_interface.py
--rw-rw-rw-   0        0        0     7280 2024-03-14 04:36:05.000000 volstreet-8.1.3/volstreet/angel_interface/base_websocket.py
--rw-rw-rw-   0        0        0    18658 2024-04-26 03:17:20.000000 volstreet-8.1.3/volstreet/angel_interface/interface.py
--rw-rw-rw-   0        0        0     2501 2024-04-06 10:22:09.000000 volstreet-8.1.3/volstreet/angel_interface/login.py
--rw-rw-rw-   0        0        0     1988 2024-03-14 04:36:05.000000 volstreet-8.1.3/volstreet/angel_interface/order_websocket.py
--rw-rw-rw-   0        0        0    30773 2024-04-29 09:17:58.000000 volstreet-8.1.3/volstreet/angel_interface/price_websocket.py
--rw-rw-rw-   0        0        0     6687 2024-04-26 02:56:08.000000 volstreet-8.1.3/volstreet/angel_interface/smart_connect.py
-drwxrwxrwx   0        0        0        0 2024-04-29 10:20:18.235928 volstreet-8.1.3/volstreet/backtests/
--rw-rw-rw-   0        0        0      290 2024-04-28 14:01:14.000000 volstreet-8.1.3/volstreet/backtests/__init__.py
--rw-rw-rw-   0        0        0     4064 2024-04-23 04:22:25.000000 volstreet-8.1.3/volstreet/backtests/analysis.py
--rw-rw-rw-   0        0        0     4101 2024-04-28 03:48:57.000000 volstreet-8.1.3/volstreet/backtests/data_updation.py
--rw-rw-rw-   0        0        0    11857 2024-04-25 10:13:39.000000 volstreet-8.1.3/volstreet/backtests/database.py
--rw-rw-rw-   0        0        0    38400 2024-04-03 08:06:51.000000 volstreet-8.1.3/volstreet/backtests/delta_hedging.py
--rw-rw-rw-   0        0        0     5695 2024-03-14 04:36:05.000000 volstreet-8.1.3/volstreet/backtests/delta_optimizer.py
--rw-rw-rw-   0        0        0    48672 2024-04-24 06:53:53.000000 volstreet-8.1.3/volstreet/backtests/framework.py
--rw-rw-rw-   0        0        0     5410 2024-04-13 06:57:57.000000 volstreet-8.1.3/volstreet/backtests/intraday_backtest_abc.py
--rw-rw-rw-   0        0        0     5926 2024-04-26 13:19:27.000000 volstreet-8.1.3/volstreet/backtests/proxy_functions.py
--rw-rw-rw-   0        0        0     2707 2024-04-24 14:17:18.000000 volstreet-8.1.3/volstreet/backtests/result_processing.py
--rw-rw-rw-   0        0        0     6051 2024-04-26 10:25:05.000000 volstreet-8.1.3/volstreet/backtests/runner.py
--rw-rw-rw-   0        0        0     6446 2024-03-26 10:23:44.000000 volstreet-8.1.3/volstreet/backtests/tools.py
--rw-rw-rw-   0        0        0    15734 2024-04-13 06:57:57.000000 volstreet-8.1.3/volstreet/backtests/trend.py
--rw-rw-rw-   0        0        0     1689 2024-04-25 14:52:32.000000 volstreet-8.1.3/volstreet/backtests/underlying_info.py
--rw-rw-rw-   0        0        0    20854 2024-04-24 06:53:53.000000 volstreet-8.1.3/volstreet/blackscholes.py
--rw-rw-rw-   0        0        0     5574 2024-04-24 06:53:53.000000 volstreet-8.1.3/volstreet/config.py
--rw-rw-rw-   0        0        0     2162 2024-03-14 04:36:05.000000 volstreet-8.1.3/volstreet/database_connection.py
-drwxrwxrwx   0        0        0        0 2024-04-29 10:20:18.252017 volstreet-8.1.3/volstreet/datamodule/
--rw-rw-rw-   0        0        0      163 2024-04-13 05:46:57.000000 volstreet-8.1.3/volstreet/datamodule/__init__.py
--rw-rw-rw-   0        0        0     7358 2024-03-14 04:36:05.000000 volstreet-8.1.3/volstreet/datamodule/analysis.py
--rw-rw-rw-   0        0        0    21130 2024-03-14 04:36:05.000000 volstreet-8.1.3/volstreet/datamodule/archive.py
--rw-rw-rw-   0        0        0     9035 2024-04-26 13:37:15.000000 volstreet-8.1.3/volstreet/datamodule/data_handling.py
--rw-rw-rw-   0        0        0     4534 2024-03-14 04:36:05.000000 volstreet-8.1.3/volstreet/datamodule/eod_client.py
--rw-rw-rw-   0        0        0     5639 2024-03-14 04:36:05.000000 volstreet-8.1.3/volstreet/datamodule/gambling.py
--rw-rw-rw-   0        0        0     8098 2024-03-14 04:36:05.000000 volstreet-8.1.3/volstreet/datamodule/intraday_data.py
--rw-rw-rw-   0        0        0    15754 2024-03-26 10:23:44.000000 volstreet-8.1.3/volstreet/datamodule/stockmock.py
--rw-rw-rw-   0        0        0     1219 2024-03-14 04:36:05.000000 volstreet-8.1.3/volstreet/datamodule/trading_assistance.py
--rw-rw-rw-   0        0        0    27286 2024-03-26 10:23:44.000000 volstreet-8.1.3/volstreet/dealingroom.py
--rw-rw-rw-   0        0        0     2573 2024-04-03 08:06:51.000000 volstreet-8.1.3/volstreet/decorators.py
--rw-rw-rw-   0        0        0     1683 2024-03-14 04:36:05.000000 volstreet-8.1.3/volstreet/discord_bot.py
--rw-rw-rw-   0        0        0     1698 2024-03-14 04:36:05.000000 volstreet-8.1.3/volstreet/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-29 10:20:18.267680 volstreet-8.1.3/volstreet/historical_info/
--rw-rw-rw-   0        0        0      975 2024-04-24 06:53:53.000000 volstreet-8.1.3/volstreet/historical_info/__init__.py
--rw-rw-rw-   0        0        0    18590 2024-04-29 02:56:24.000000 volstreet-8.1.3/volstreet/historical_info/index_expiries.pkl
--rw-rw-rw-   0        0        0    16858 2024-04-26 13:32:31.000000 volstreet-8.1.3/volstreet/historical_info/market_days.pkl
-drwxrwxrwx   0        0        0        0 2024-04-29 10:20:18.267680 volstreet-8.1.3/volstreet/models/
--rw-rw-rw-   0        0        0      565 2024-04-24 06:53:53.000000 volstreet-8.1.3/volstreet/models/__init__.py
--rw-rw-rw-   0        0        0      772 2024-03-14 04:36:05.000000 volstreet-8.1.3/volstreet/parallelization.py
--rw-rw-rw-   0        0        0     1659 2024-04-06 06:31:33.000000 volstreet-8.1.3/volstreet/performance_tracking.py
-drwxrwxrwx   0        0        0        0 2024-04-29 10:20:18.267680 volstreet-8.1.3/volstreet/position_dashboard/
--rw-rw-rw-   0        0        0        0 2024-04-17 11:41:53.000000 volstreet-8.1.3/volstreet/position_dashboard/__init__.py
--rw-rw-rw-   0        0        0     1972 2024-04-17 11:41:53.000000 volstreet-8.1.3/volstreet/position_dashboard/app.py
--rw-rw-rw-   0        0        0      572 2024-04-17 11:41:53.000000 volstreet-8.1.3/volstreet/position_dashboard/formatting.py
-drwxrwxrwx   0        0        0        0 2024-04-29 10:20:18.283371 volstreet-8.1.3/volstreet/strategies/
--rw-rw-rw-   0        0        0      156 2024-04-17 11:41:53.000000 volstreet-8.1.3/volstreet/strategies/__init__.py
--rw-rw-rw-   0        0        0    29925 2024-04-29 10:16:57.000000 volstreet-8.1.3/volstreet/strategies/deployment.py
--rw-rw-rw-   0        0        0     5194 2024-04-17 11:41:53.000000 volstreet-8.1.3/volstreet/strategies/error_handling.py
--rw-rw-rw-   0        0        0    51697 2024-04-29 03:38:31.000000 volstreet-8.1.3/volstreet/strategies/helpers.py
--rw-rw-rw-   0        0        0     2949 2024-04-17 11:41:53.000000 volstreet-8.1.3/volstreet/strategies/monitoring.py
--rw-rw-rw-   0        0        0    17179 2024-04-10 07:52:35.000000 volstreet-8.1.3/volstreet/strategies/optimization.py
--rw-rw-rw-   0        0        0    98011 2024-04-29 10:19:25.000000 volstreet-8.1.3/volstreet/strategies/strats.py
--rw-rw-rw-   0        0        0      349 2024-04-12 11:13:05.000000 volstreet-8.1.3/volstreet/strategies/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-29 10:20:18.298905 volstreet-8.1.3/volstreet/trade_interface/
--rw-rw-rw-   0        0        0      224 2024-04-17 11:41:53.000000 volstreet-8.1.3/volstreet/trade_interface/__init__.py
--rw-rw-rw-   0        0        0    26799 2024-04-23 04:22:25.000000 volstreet-8.1.3/volstreet/trade_interface/instruments.py
--rw-rw-rw-   0        0        0    19389 2024-04-29 10:19:25.000000 volstreet-8.1.3/volstreet/trade_interface/order_execution.py
--rw-rw-rw-   0        0        0    20598 2024-04-28 16:45:33.000000 volstreet-8.1.3/volstreet/trade_interface/underlyings.py
-drwxrwxrwx   0        0        0        0 2024-04-29 10:20:18.314612 volstreet-8.1.3/volstreet/utils/
--rw-rw-rw-   0        0        0      138 2024-03-14 04:36:05.000000 volstreet-8.1.3/volstreet/utils/__init__.py
--rw-rw-rw-   0        0        0      757 2024-03-14 04:36:05.000000 volstreet-8.1.3/volstreet/utils/change_config.py
--rw-rw-rw-   0        0        0     3052 2024-04-09 12:38:37.000000 volstreet-8.1.3/volstreet/utils/communication.py
--rw-rw-rw-   0        0        0    13115 2024-04-23 04:22:25.000000 volstreet-8.1.3/volstreet/utils/core.py
--rw-rw-rw-   0        0        0     4419 2024-03-14 04:36:05.000000 volstreet-8.1.3/volstreet/utils/data_io.py
--rw-rw-rw-   0        0        0     9915 2024-04-26 13:19:30.000000 volstreet-8.1.3/volstreet/utils/scrip_processing.py
--rw-rw-rw-   0        0        0     6488 2024-04-23 04:22:25.000000 volstreet-8.1.3/volstreet/vectorized_blackscholes.py
--rw-rw-rw-   0        0        0       16 2024-04-29 03:37:37.000000 volstreet-8.1.3/volstreet/volstreet_mode.json
-drwxrwxrwx   0        0        0        0 2024-04-29 10:20:18.330154 volstreet-8.1.3/volstreet/vslogging/
--rw-rw-rw-   0        0        0       81 2024-03-15 09:40:04.000000 volstreet-8.1.3/volstreet/vslogging/__init__.py
--rw-rw-rw-   0        0        0     2023 2024-03-26 10:23:44.000000 volstreet-8.1.3/volstreet/vslogging/formatters.py
--rw-rw-rw-   0        0        0     1492 2024-03-27 04:16:21.000000 volstreet-8.1.3/volstreet/vslogging/logging_config.json
--rw-rw-rw-   0        0        0      842 2024-03-26 10:23:44.000000 volstreet-8.1.3/volstreet/vslogging/logging_setup.py
--rw-rw-rw-   0        0        0     1390 2024-04-17 11:41:53.000000 volstreet-8.1.3/volstreet/vslogging/parsing.py
-drwxrwxrwx   0        0        0        0 2024-04-29 10:20:18.330154 volstreet-8.1.3/volstreet.egg-info/
--rw-rw-rw-   0        0        0     1293 2024-04-29 10:20:18.000000 volstreet-8.1.3/volstreet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2833 2024-04-29 10:20:18.000000 volstreet-8.1.3/volstreet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 10:20:18.000000 volstreet-8.1.3/volstreet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      460 2024-04-29 10:20:18.000000 volstreet-8.1.3/volstreet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-29 10:20:18.000000 volstreet-8.1.3/volstreet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 03:10:02.170958 volstreet-8.2.0/
+-rw-rw-rw-   0        0        0     1293 2024-05-06 03:10:02.169957 volstreet-8.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2024-03-14 04:36:05.000000 volstreet-8.2.0/README.md
+-rw-rw-rw-   0        0        0       91 2024-03-14 04:36:05.000000 volstreet-8.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1155 2024-05-06 03:10:02.171957 volstreet-8.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-06 03:10:02.079141 volstreet-8.2.0/volstreet/
+-rw-rw-rw-   0        0        0      442 2024-03-14 09:55:16.000000 volstreet-8.2.0/volstreet/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:10:02.098231 volstreet-8.2.0/volstreet/angel_interface/
+-rw-rw-rw-   0        0        0      247 2024-04-26 02:47:59.000000 volstreet-8.2.0/volstreet/angel_interface/__init__.py
+-rw-rw-rw-   0        0        0     3726 2024-04-26 02:48:50.000000 volstreet-8.2.0/volstreet/angel_interface/access_rate_handler.py
+-rw-rw-rw-   0        0        0      274 2024-04-23 04:22:25.000000 volstreet-8.2.0/volstreet/angel_interface/active_session.py
+-rw-rw-rw-   0        0        0     2843 2024-04-28 03:29:15.000000 volstreet-8.2.0/volstreet/angel_interface/async_interface.py
+-rw-rw-rw-   0        0        0     7280 2024-03-14 04:36:05.000000 volstreet-8.2.0/volstreet/angel_interface/base_websocket.py
+-rw-rw-rw-   0        0        0    18658 2024-04-26 03:17:20.000000 volstreet-8.2.0/volstreet/angel_interface/interface.py
+-rw-rw-rw-   0        0        0     2501 2024-04-06 10:22:09.000000 volstreet-8.2.0/volstreet/angel_interface/login.py
+-rw-rw-rw-   0        0        0     1988 2024-03-14 04:36:05.000000 volstreet-8.2.0/volstreet/angel_interface/order_websocket.py
+-rw-rw-rw-   0        0        0    30773 2024-04-29 09:17:58.000000 volstreet-8.2.0/volstreet/angel_interface/price_websocket.py
+-rw-rw-rw-   0        0        0     6687 2024-04-26 02:56:08.000000 volstreet-8.2.0/volstreet/angel_interface/smart_connect.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:10:02.116512 volstreet-8.2.0/volstreet/backtests/
+-rw-rw-rw-   0        0        0      290 2024-04-28 14:01:14.000000 volstreet-8.2.0/volstreet/backtests/__init__.py
+-rw-rw-rw-   0        0        0     4064 2024-04-23 04:22:25.000000 volstreet-8.2.0/volstreet/backtests/analysis.py
+-rw-rw-rw-   0        0        0     4181 2024-05-04 08:33:34.000000 volstreet-8.2.0/volstreet/backtests/data_updation.py
+-rw-rw-rw-   0        0        0    11857 2024-04-25 10:13:39.000000 volstreet-8.2.0/volstreet/backtests/database.py
+-rw-rw-rw-   0        0        0    38400 2024-04-03 08:06:51.000000 volstreet-8.2.0/volstreet/backtests/delta_hedging.py
+-rw-rw-rw-   0        0        0     5695 2024-03-14 04:36:05.000000 volstreet-8.2.0/volstreet/backtests/delta_optimizer.py
+-rw-rw-rw-   0        0        0    48672 2024-05-02 12:46:20.000000 volstreet-8.2.0/volstreet/backtests/framework.py
+-rw-rw-rw-   0        0        0     5410 2024-04-13 06:57:57.000000 volstreet-8.2.0/volstreet/backtests/intraday_backtest_abc.py
+-rw-rw-rw-   0        0        0     7201 2024-05-05 08:31:29.000000 volstreet-8.2.0/volstreet/backtests/proxy_functions.py
+-rw-rw-rw-   0        0        0     2707 2024-04-24 14:17:18.000000 volstreet-8.2.0/volstreet/backtests/result_processing.py
+-rw-rw-rw-   0        0        0     6149 2024-05-04 09:19:15.000000 volstreet-8.2.0/volstreet/backtests/runner.py
+-rw-rw-rw-   0        0        0     6446 2024-03-26 10:23:44.000000 volstreet-8.2.0/volstreet/backtests/tools.py
+-rw-rw-rw-   0        0        0    15734 2024-04-13 06:57:57.000000 volstreet-8.2.0/volstreet/backtests/trend.py
+-rw-rw-rw-   0        0        0     1923 2024-05-05 08:57:06.000000 volstreet-8.2.0/volstreet/backtests/underlying_info.py
+-rw-rw-rw-   0        0        0    20882 2024-05-02 08:25:42.000000 volstreet-8.2.0/volstreet/blackscholes.py
+-rw-rw-rw-   0        0        0     5574 2024-04-24 06:53:53.000000 volstreet-8.2.0/volstreet/config.py
+-rw-rw-rw-   0        0        0     2162 2024-03-14 04:36:05.000000 volstreet-8.2.0/volstreet/database_connection.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:10:02.128637 volstreet-8.2.0/volstreet/datamodule/
+-rw-rw-rw-   0        0        0      163 2024-04-13 05:46:57.000000 volstreet-8.2.0/volstreet/datamodule/__init__.py
+-rw-rw-rw-   0        0        0     7358 2024-03-14 04:36:05.000000 volstreet-8.2.0/volstreet/datamodule/analysis.py
+-rw-rw-rw-   0        0        0    21130 2024-03-14 04:36:05.000000 volstreet-8.2.0/volstreet/datamodule/archive.py
+-rw-rw-rw-   0        0        0     9685 2024-05-04 09:32:35.000000 volstreet-8.2.0/volstreet/datamodule/data_handling.py
+-rw-rw-rw-   0        0        0     4534 2024-03-14 04:36:05.000000 volstreet-8.2.0/volstreet/datamodule/eod_client.py
+-rw-rw-rw-   0        0        0     5639 2024-03-14 04:36:05.000000 volstreet-8.2.0/volstreet/datamodule/gambling.py
+-rw-rw-rw-   0        0        0     8098 2024-03-14 04:36:05.000000 volstreet-8.2.0/volstreet/datamodule/intraday_data.py
+-rw-rw-rw-   0        0        0    15754 2024-03-26 10:23:44.000000 volstreet-8.2.0/volstreet/datamodule/stockmock.py
+-rw-rw-rw-   0        0        0     1219 2024-03-14 04:36:05.000000 volstreet-8.2.0/volstreet/datamodule/trading_assistance.py
+-rw-rw-rw-   0        0        0    25622 2024-05-06 02:53:39.000000 volstreet-8.2.0/volstreet/dealingroom.py
+-rw-rw-rw-   0        0        0     2573 2024-04-03 08:06:51.000000 volstreet-8.2.0/volstreet/decorators.py
+-rw-rw-rw-   0        0        0     1683 2024-03-14 04:36:05.000000 volstreet-8.2.0/volstreet/discord_bot.py
+-rw-rw-rw-   0        0        0     1698 2024-03-14 04:36:05.000000 volstreet-8.2.0/volstreet/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:10:02.133434 volstreet-8.2.0/volstreet/historical_info/
+-rw-rw-rw-   0        0        0      975 2024-04-24 06:53:53.000000 volstreet-8.2.0/volstreet/historical_info/__init__.py
+-rw-rw-rw-   0        0        0    21031 2024-05-04 08:38:02.000000 volstreet-8.2.0/volstreet/historical_info/index_expiries.pkl
+-rw-rw-rw-   0        0        0    16910 2024-05-04 09:35:37.000000 volstreet-8.2.0/volstreet/historical_info/market_days.pkl
+drwxrwxrwx   0        0        0        0 2024-05-06 03:10:02.134439 volstreet-8.2.0/volstreet/models/
+-rw-rw-rw-   0        0        0      568 2024-04-29 10:45:14.000000 volstreet-8.2.0/volstreet/models/__init__.py
+-rw-rw-rw-   0        0        0      772 2024-03-14 04:36:05.000000 volstreet-8.2.0/volstreet/parallelization.py
+-rw-rw-rw-   0        0        0     1659 2024-04-06 06:31:33.000000 volstreet-8.2.0/volstreet/performance_tracking.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:10:02.137550 volstreet-8.2.0/volstreet/position_dashboard/
+-rw-rw-rw-   0        0        0        0 2024-04-17 11:41:53.000000 volstreet-8.2.0/volstreet/position_dashboard/__init__.py
+-rw-rw-rw-   0        0        0     1972 2024-04-17 11:41:53.000000 volstreet-8.2.0/volstreet/position_dashboard/app.py
+-rw-rw-rw-   0        0        0      572 2024-04-17 11:41:53.000000 volstreet-8.2.0/volstreet/position_dashboard/formatting.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:10:02.148640 volstreet-8.2.0/volstreet/strategies/
+-rw-rw-rw-   0        0        0      183 2024-05-03 07:00:07.000000 volstreet-8.2.0/volstreet/strategies/__init__.py
+-rw-rw-rw-   0        0        0    32426 2024-05-06 02:53:39.000000 volstreet-8.2.0/volstreet/strategies/deployment.py
+-rw-rw-rw-   0        0        0     1925 2024-05-03 06:56:48.000000 volstreet-8.2.0/volstreet/strategies/error_handling.py
+-rw-rw-rw-   0        0        0    54994 2024-05-03 11:29:24.000000 volstreet-8.2.0/volstreet/strategies/helpers.py
+-rw-rw-rw-   0        0        0     6352 2024-05-03 06:56:48.000000 volstreet-8.2.0/volstreet/strategies/monitoring.py
+-rw-rw-rw-   0        0        0    18535 2024-05-02 10:20:37.000000 volstreet-8.2.0/volstreet/strategies/optimization.py
+-rw-rw-rw-   0        0        0   106431 2024-05-06 02:59:53.000000 volstreet-8.2.0/volstreet/strategies/strats.py
+-rw-rw-rw-   0        0        0      349 2024-04-12 11:13:05.000000 volstreet-8.2.0/volstreet/strategies/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:10:02.153640 volstreet-8.2.0/volstreet/trade_interface/
+-rw-rw-rw-   0        0        0      224 2024-04-17 11:41:53.000000 volstreet-8.2.0/volstreet/trade_interface/__init__.py
+-rw-rw-rw-   0        0        0    26799 2024-04-23 04:22:25.000000 volstreet-8.2.0/volstreet/trade_interface/instruments.py
+-rw-rw-rw-   0        0        0    19389 2024-04-29 10:19:25.000000 volstreet-8.2.0/volstreet/trade_interface/order_execution.py
+-rw-rw-rw-   0        0        0    20204 2024-05-05 08:31:29.000000 volstreet-8.2.0/volstreet/trade_interface/underlyings.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:10:02.161809 volstreet-8.2.0/volstreet/utils/
+-rw-rw-rw-   0        0        0      138 2024-03-14 04:36:05.000000 volstreet-8.2.0/volstreet/utils/__init__.py
+-rw-rw-rw-   0        0        0      757 2024-03-14 04:36:05.000000 volstreet-8.2.0/volstreet/utils/change_config.py
+-rw-rw-rw-   0        0        0     3052 2024-04-09 12:38:37.000000 volstreet-8.2.0/volstreet/utils/communication.py
+-rw-rw-rw-   0        0        0    14475 2024-05-03 08:15:05.000000 volstreet-8.2.0/volstreet/utils/core.py
+-rw-rw-rw-   0        0        0     4419 2024-03-14 04:36:05.000000 volstreet-8.2.0/volstreet/utils/data_io.py
+-rw-rw-rw-   0        0        0     9915 2024-04-26 13:19:30.000000 volstreet-8.2.0/volstreet/utils/scrip_processing.py
+-rw-rw-rw-   0        0        0     6488 2024-04-23 04:22:25.000000 volstreet-8.2.0/volstreet/vectorized_blackscholes.py
+-rw-rw-rw-   0        0        0       20 2024-05-04 09:32:55.000000 volstreet-8.2.0/volstreet/volstreet_mode.json
+drwxrwxrwx   0        0        0        0 2024-05-06 03:10:02.167957 volstreet-8.2.0/volstreet/vslogging/
+-rw-rw-rw-   0        0        0       81 2024-03-15 09:40:04.000000 volstreet-8.2.0/volstreet/vslogging/__init__.py
+-rw-rw-rw-   0        0        0     2023 2024-03-26 10:23:44.000000 volstreet-8.2.0/volstreet/vslogging/formatters.py
+-rw-rw-rw-   0        0        0     1492 2024-03-27 04:16:21.000000 volstreet-8.2.0/volstreet/vslogging/logging_config.json
+-rw-rw-rw-   0        0        0      842 2024-03-26 10:23:44.000000 volstreet-8.2.0/volstreet/vslogging/logging_setup.py
+-rw-rw-rw-   0        0        0     1390 2024-04-17 11:41:53.000000 volstreet-8.2.0/volstreet/vslogging/parsing.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:10:02.168970 volstreet-8.2.0/volstreet.egg-info/
+-rw-rw-rw-   0        0        0     1293 2024-05-06 03:10:02.000000 volstreet-8.2.0/volstreet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2833 2024-05-06 03:10:02.000000 volstreet-8.2.0/volstreet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 03:10:02.000000 volstreet-8.2.0/volstreet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      460 2024-05-06 03:10:02.000000 volstreet-8.2.0/volstreet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-06 03:10:02.000000 volstreet-8.2.0/volstreet.egg-info/top_level.txt
```

### Comparing `volstreet-8.1.3/PKG-INFO` & `volstreet-8.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volstreet
-Version: 8.1.3
+Version: 8.2.0
 Summary: VolStreet is a Python library for automated trading
 Home-page: https://github.com/rahulthakkr/volstreet
 Author: Rahul Thakkar
 Author-email: r.thakkar15@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `volstreet-8.1.3/setup.cfg` & `volstreet-8.2.0/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6f6c 7374 7265 6574 0d0a 7665   = volstreet..ve
-00000020: 7273 696f 6e20 3d20 382e 312e 330d 0a61  rsion = 8.1.3..a
+00000020: 7273 696f 6e20 3d20 382e 322e 300d 0a61  rsion = 8.2.0..a
 00000030: 7574 686f 7220 3d20 5261 6875 6c20 5468  uthor = Rahul Th
 00000040: 616b 6b61 720d 0a61 7574 686f 725f 656d  akkar..author_em
 00000050: 6169 6c20 3d20 722e 7468 616b 6b61 7231  ail = r.thakkar1
 00000060: 3540 676d 6169 6c2e 636f 6d0d 0a64 6573  5@gmail.com..des
 00000070: 6372 6970 7469 6f6e 203d 2056 6f6c 5374  cription = VolSt
 00000080: 7265 6574 2069 7320 6120 5079 7468 6f6e  reet is a Python
 00000090: 206c 6962 7261 7279 2066 6f72 2061 7574   library for aut
```

### Comparing `volstreet-8.1.3/volstreet/angel_interface/access_rate_handler.py` & `volstreet-8.2.0/volstreet/angel_interface/access_rate_handler.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/angel_interface/async_interface.py` & `volstreet-8.2.0/volstreet/angel_interface/async_interface.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/angel_interface/base_websocket.py` & `volstreet-8.2.0/volstreet/angel_interface/base_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/angel_interface/interface.py` & `volstreet-8.2.0/volstreet/angel_interface/interface.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/angel_interface/login.py` & `volstreet-8.2.0/volstreet/angel_interface/login.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/angel_interface/order_websocket.py` & `volstreet-8.2.0/volstreet/angel_interface/order_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/angel_interface/price_websocket.py` & `volstreet-8.2.0/volstreet/angel_interface/price_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/angel_interface/smart_connect.py` & `volstreet-8.2.0/volstreet/angel_interface/smart_connect.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/backtests/analysis.py` & `volstreet-8.2.0/volstreet/backtests/analysis.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/backtests/data_updation.py` & `volstreet-8.2.0/volstreet/backtests/data_updation.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,16 +19,23 @@
     directory = files("volstreet").joinpath("historical_info")
     # noinspection PyTypeChecker
     file_path = Path(directory.joinpath("index_expiries.pkl"))
 
     with open(file_path, "rb") as file:
         all_expiry_dates = pickle.load(file)
 
-    for underlying in ["NIFTY", "BANKNIFTY", "FINNIFTY", "MIDCPNIFTY"]:
-        index_expiry_dates = all_expiry_dates[underlying]
+    for underlying in [
+        "NIFTY",
+        "BANKNIFTY",
+        "FINNIFTY",
+        "MIDCPNIFTY",
+        "SENSEX",
+        "BANKEX",
+    ]:
+        index_expiry_dates = all_expiry_dates.get(underlying, [])
         new_list = dbc.fetch_historical_expiries(underlying)
         combined_list = [*set(index_expiry_dates + new_list)]
         all_expiry_dates[underlying] = combined_list
         logger.info(f"Extended expiry dates for {underlying}")
 
     with open(file_path, "wb") as file:
         pickle.dump(all_expiry_dates, file)
@@ -52,15 +59,15 @@
         pickle.dump(new_market_days, file)
         logger.info(
             f"Updated market days. New number of market days: {len(new_market_days)}"
         )
 
 
 def update_price_stream_for_index(
-    index: str, earliest_allowed_date: datetime = None, days_to_expiry: int = 2
+    index: str, earliest_allowed_date: "datetime.date" = None, days_to_expiry: int = 2
 ) -> None:
     backtester = BackTester()
     index = UnderlyingInfo(index)
     engine = create_engine(backtester._alchemy_engine_url)
     market_dts = [datetime.combine(day, datetime.min.time()) for day in market_days]
     target_days = [
         day.date()
@@ -74,15 +81,15 @@
         """
     )[0][0]
     filter_date = latest_date or earliest_allowed_date
     assert (
         filter_date
     ), "Atleast one of latest_date or earliest_allowed_date must be provided"
     dates_to_update = [
-        day for day in target_days if day > earliest_allowed_date.date()
+        day for day in target_days if day > filter_date
     ]  # Only update the days which are not already present in the database
     if not dates_to_update:
         logger.info(f"No days to update for {index.name}")
         return
     logger.info(f"Updating price stream for {index.name} for days: {dates_to_update}")
     for day in dates_to_update:
         logger.info(f"Updating price stream for {index.name} on {day}")
```

### Comparing `volstreet-8.1.3/volstreet/backtests/database.py` & `volstreet-8.2.0/volstreet/backtests/database.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/backtests/delta_hedging.py` & `volstreet-8.2.0/volstreet/backtests/delta_hedging.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/backtests/delta_optimizer.py` & `volstreet-8.2.0/volstreet/backtests/delta_optimizer.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/backtests/framework.py` & `volstreet-8.2.0/volstreet/backtests/framework.py`

 * *Files 0% similar despite different names*

```diff
@@ -265,15 +265,15 @@
 
         return merged
 
     def get_prices_for_day(
         self,
         underlying_info: UnderlyingInfo,
         day: str | datetime,
-        num_strikes: int = 25,
+        num_strikes: int = 50,
         num_exp: int = 2,
         start_time: tuple[int, int] = (9, 16),
         end_time: tuple[int, int] = (15, 30),
     ) -> pd.DataFrame:
         """This also fills in missing option prices."""
         day = day.date() if isinstance(day, datetime) else day
         option_chain = self.build_option_chain(
```

### Comparing `volstreet-8.1.3/volstreet/backtests/intraday_backtest_abc.py` & `volstreet-8.2.0/volstreet/backtests/intraday_backtest_abc.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/backtests/proxy_functions.py` & `volstreet-8.2.0/volstreet/backtests/proxy_functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,68 @@
 from datetime import datetime, timedelta, time
+import pandas as pd
+import re
 from volstreet.config import EXPIRY_FREQUENCIES
 from volstreet import config
-from volstreet.utils import current_time, parse_symbol
+from volstreet.utils import current_time
 from volstreet.backtests.underlying_info import UnderlyingInfo, fetch_historical_expiry
 from volstreet.backtests.framework import BackTester
 
 
 class ProxyPriceFeed:
     data_bank = {}
     backtester = BackTester()
     _current_group = None
 
     @classmethod
     def request_grouped_prices_for_day(
-        cls, underlying: UnderlyingInfo, day: datetime, **kwargs
+        cls, underlying: UnderlyingInfo, day: datetime, include_vix_data=False, **kwargs
     ):
+        start_time = time(*kwargs.get("start_time", (9, 16)))
+        end_time = time(*kwargs.get("end_time", (15, 30)))
         day_prices = cls.backtester.fetch_streaming_prices(underlying.name, day)
         if day_prices.empty:
             config.logger.warning(
                 f"No prices found for {underlying.name} on {day} in price_stream. "
                 f"Running process to fetch prices from historical data."
             )
             day_prices = cls.backtester.get_prices_for_day(underlying, day, **kwargs)
         else:
-            start_time = time(*kwargs.get("start_time", (9, 16)))
-            end_time = time(*kwargs.get("end_time", (15, 30)))
             day_prices = day_prices[
                 (day_prices.timestamp.dt.time >= start_time)
                 & (day_prices.timestamp.dt.time <= end_time)
             ]
 
+        if include_vix_data:
+            vix_data = cls.backtester.fetch_index_prices(
+                "India Vix",
+                from_timestamp=f"{day} {start_time}",
+                to_timestamp=f"{day} {end_time}",
+            )
+            vix_data = vix_data.rename(
+                columns={
+                    "timestamp": "timestamp",
+                    "open": "price",
+                    "underlying": "symboltoken",
+                }
+            )
+            vix_data = vix_data[["timestamp", "price", "symboltoken"]]
+            # To ensure that vix prices are available for all timestamps
+            new_index = pd.date_range(
+                start=f"{day} {start_time}", end=f"{day} {end_time}", freq="1min"
+            )
+            new_index.name = "timestamp"
+            vix_data = (
+                vix_data.set_index("timestamp")
+                .reindex(new_index, method="nearest")
+                .reset_index()
+            )
+            day_prices = pd.concat([day_prices, vix_data])
+            day_prices = day_prices.sort_values("timestamp")
+
         day_prices_grouped = day_prices.groupby(day_prices.timestamp.dt.time)
         return day_prices_grouped
 
     @classmethod
     def update_prices(cls):
         prices_at_time = cls._current_group.get_group(config.backtest_state.time())
         price_dict = prices_at_time.to_dict(orient="records")
@@ -66,15 +95,15 @@
     else:
         symbol = f"{name.upper()}{expiry.upper()}{int(strike)}{option_type.upper()}"
         return symbol, symbol
 
 
 def get_expiry_dates(underlying: str):
     expiries = fetch_historical_expiry(
-        underlying, current_time(), threshold_days=0, n_exp=4
+        underlying, current_time(), threshold_days=0, n_exp=3
     )
     return expiries
 
 
 def get_base(name, expiry):
     return UnderlyingInfo(name).base
 
@@ -95,14 +124,19 @@
             )
         else:
             average_price_dict[instr] = avg_prices[instr.symbol]
 
     return average_price_dict
 
 
+def parse_symbol(symbol):
+    match = re.match(r"([A-Za-z]+)(\d{2}[A-Za-z]{3}\d{2})(\d+)(\w+)", symbol)
+    return match.groups()
+
+
 def simulate_execution(order: dict):
 
     price = order["price"]
     index, expiry, strike, option_type = parse_symbol(order["symboltoken"])
     value = order["quantity"] * price * (1 if order["transactiontype"] == "BUY" else -1)
     order_details = {
         "timestamp": current_time(),
```

### Comparing `volstreet-8.1.3/volstreet/backtests/result_processing.py` & `volstreet-8.2.0/volstreet/backtests/result_processing.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/backtests/runner.py` & `volstreet-8.2.0/volstreet/backtests/runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,31 +33,32 @@
         self.price_feed = ProxyPriceFeed
         self.Index = __import__("volstreet.trade_interface").Index
         self.end_directory = self.make_result_directory(end_directory)
 
     def make_result_directory(self, end_directory):
         # Making a directory to store the results
         strategy = self.strategy.__name__
-        index_strategy_directory = f"backtester\\{self.underlying.name}_{strategy}\\"
+        index_strategy_directory = f"backtester\\{self.underlying.name}\\{strategy}\\"
         if end_directory is None:
             make_directory_if_needed(index_strategy_directory)
             folder_number = len(os.listdir(index_strategy_directory)) + 1
             end_directory = f"test_{folder_number}\\"
 
         end_directory = os.path.join(index_strategy_directory, f"{end_directory}\\")
         make_directory_if_needed(end_directory)
         return end_directory
 
     def run(
         self,
         only_expiry: bool = False,
-        num_strikes: int = 30,
+        num_strikes: int = 50,
         num_exp: int = 2,
         start_time: tuple[int, int] = (9, 16),
         end_time: tuple[int, int] = (15, 30),
+        include_vix_data: bool = False,
     ) -> None:
         valid_range = pd.date_range(self.start_date, self.end_date)
         valid_range = [day.date() for day in valid_range if day.date() in market_days]
 
         if only_expiry:
             target_days = map(lambda x: x.date(), self.underlying.expiry_dates)
             target_days = [day for day in target_days if day in valid_range]
@@ -70,14 +71,15 @@
 
         with ThreadPoolExecutor(max_workers=4) as executor:
             daily_prices = [
                 executor.submit(
                     self.price_feed.request_grouped_prices_for_day,
                     self.underlying,
                     day,
+                    include_vix_data=include_vix_data,
                     num_strikes=num_strikes,
                     num_exp=num_exp,
                     start_time=start_time,
                     end_time=end_time,
                 )
                 for day in target_days
             ]
```

### Comparing `volstreet-8.1.3/volstreet/backtests/tools.py` & `volstreet-8.2.0/volstreet/backtests/tools.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/backtests/trend.py` & `volstreet-8.2.0/volstreet/backtests/trend.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/backtests/underlying_info.py` & `volstreet-8.2.0/volstreet/backtests/underlying_info.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         self.name = name.upper()
         self.base = self._get_base()
         self.expiry_dates = filter_expiry_dates_for_index(self.name)
 
     def _get_base(self):
         if self.name in ["NIFTY", "FINNIFTY"]:
             return 50
-        elif self.name == "BANKNIFTY":
+        elif self.name in ["BANKNIFTY", "SENSEX", "BANKEX"]:
             return 100
         elif self.name == "MIDCPNIFTY":
             return 25
         else:
             raise ValueError("Invalid index name")
 
 
@@ -35,18 +35,18 @@
     threshold_days: int = 0,
     n_exp: int = 1,
 ) -> pd.DatetimeIndex | pd.Timestamp | None:
     if isinstance(date_time, str):
         date_time = pd.to_datetime(date_time)
 
     filtered_dates = filter_expiry_dates_for_index(underlying)
+    filtered_dates = filtered_dates.sort_values()
     delta_days = (filtered_dates - date_time.replace(hour=00, minute=00)).days
-    valid_indices = np.where(delta_days < threshold_days, np.inf, delta_days).argsort()[
-        :n_exp
-    ]
-
-    nearest_exp_dates = filtered_dates[valid_indices].sort_values()
-
+    filtered_dates = filtered_dates[delta_days >= threshold_days]
+    nearest_exp_dates = sorted(filtered_dates)
     if n_exp == 1:
         return nearest_exp_dates[0] if len(nearest_exp_dates) != 0 else None
-    else:
-        return nearest_exp_dates
+    if len(nearest_exp_dates) < n_exp:
+        logger.warning(f"Insufficient expiry dates for {underlying} on {date_time}")
+        while len(nearest_exp_dates) < n_exp:
+            nearest_exp_dates = nearest_exp_dates.append(np.nan)
+    return nearest_exp_dates[:n_exp]
```

### Comparing `volstreet-8.1.3/volstreet/blackscholes.py` & `volstreet-8.2.0/volstreet/blackscholes.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,14 +205,15 @@
 
     price_original = (
         call(S, K, t, r, sigma)
         if flag.upper().startswith("C")
         else put(S, K, t, r, sigma)
     )
 
+    # Setting the new time
     new_time = t - time_jump
     new_time = max(new_time, five_minutes_in_years)
 
     # New spot
     actual_time_jump = max(t - new_time, 1e-5)
     S1 = S * np.exp(r * actual_time_jump)
```

### Comparing `volstreet-8.1.3/volstreet/config.py` & `volstreet-8.2.0/volstreet/config.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/database_connection.py` & `volstreet-8.2.0/volstreet/database_connection.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/datamodule/analysis.py` & `volstreet-8.2.0/volstreet/datamodule/analysis.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/datamodule/archive.py` & `volstreet-8.2.0/volstreet/datamodule/archive.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/datamodule/data_handling.py` & `volstreet-8.2.0/volstreet/datamodule/data_handling.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     finally:
         ftp.cwd(original_directory)
 
     return zip_files
 
 
 # Cleaning the csv files
-def parse_option_string_with_digits(option_string: str) -> dict[str, str]:
+def parse_option_string_with_digits(option_string: str) -> dict:
     """
     Parse the given option string to identify the underlying asset, expiry date, strike price, and option type.
     This version accommodates underlying symbols that may contain digits.
 
     Parameters:
         option_string (str): The option string to be parsed.
 
@@ -72,16 +72,21 @@
         return {
             "underlying": groups[0],
             "expiry": groups[1],
             "strike": groups[2],
             "option_type": groups[3].upper(),
         }
     else:
-        print(f"ERROR IN OPTION STRING {option_string}")
-        return {"error": "Invalid option string format"}
+        logger.error(f"Error in parsing option string: {option_string}")
+        return {
+            "underlying": None,
+            "expiry": None,
+            "strike": None,
+            "option_type": None,
+        }
 
 
 def round_to_next_minute(time_str):
     """
     Round a time string (HH:MM:SS) to the next minute.
     """
     time_obj = datetime.strptime(time_str, "%H:%M:%S")
@@ -91,23 +96,32 @@
     return rounded_time_str
 
 
 def process_daily_prices(df):
     # Suppress the specific UserWarning
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", category=UserWarning)
-        # Filtering out tickers that end in either -I.NFO or -II.NFO
-        df = df[~df.Ticker.str.contains(r"(I|II|III|FUT).NFO$")]
-
         # Filtering for only indices
-        df = df[df.Ticker.str.contains(r"^(.*?)NIFTY")]
+
+        # Identify the exchange from the tickers
+        if any(".BFO" in ticker for ticker in df.Ticker):
+            # Filtering out tickers that end in either -I.BFO -II.BFO -III.BFO -FUT.BFO
+            df = df[~df.Ticker.str.contains(r"(I|II|III|FUT).BFO$")]
+            df = df[df.Ticker.str.contains(r"^(SENSEX|BANKEX)")]
+        else:
+            # Filtering out tickers that end in either -I.NFO or -II.NFO
+            df = df[~df.Ticker.str.contains(r"(I|II|III|FUT).NFO$")]
+            df = df[df.Ticker.str.contains(r"^(.*?)NIFTY")]
 
     df[["underlying", "expiry", "strike", "option_type"]] = (
         df.Ticker.apply(parse_option_string_with_digits).apply(pd.Series).values
     )
+    logger.info(f"Length of df before dropping NA rows: {len(df)}")
+    df.dropna(subset=["underlying", "expiry", "strike", "option_type"], inplace=True)
+    logger.info(f"Length of df after dropping NA rows: {len(df)}")
     df.strike = df.strike.apply(int)
     df["Time"] = df["Time"].apply(round_to_next_minute)
     df["Date"] = pd.to_datetime(df.Date, dayfirst=True)
     df["Time"] = pd.to_timedelta(df.Time)
     df["timestamp"] = df["Date"] + df["Time"]
     df = df.drop(columns=["Ticker", "Date", "Time"])
     df = df[
@@ -117,19 +131,16 @@
             "expiry",
             "strike",
             "option_type",
             "Open",
             "High",
             "Low",
             "Close",
-            "Volume",
-            "Open Interest",
         ]
     ]
-    df.drop(columns=["Volume", "Open Interest"], inplace=True)
 
     df.columns = [name.lower() for name in df.columns]
 
     df["expiry"] = pd.to_datetime(df["expiry"], format="%d%b%y")
     df["expiry"] = df["expiry"] + timedelta(hours=15, minutes=30)
 
     return df
@@ -147,21 +158,23 @@
 
             if remove:
                 # Remove the ZIP file
                 os.remove(zip_path)
 
 
 def process_file(file_path):
-    file_name = os.path.basename(file_path).split("_")[2]
+    exchange = os.path.basename(file_path).split("_")[0]
+    file_name = f"{exchange}_{os.path.basename(file_path).split('_')[2]}"
     existing_files = os.listdir(os.path.join("option_prices", "all"))
     if f"{file_name}" in map(
         lambda x: os.path.basename(x), existing_files
     ):  # If the file already exists, skip it
         return
     destination = os.path.join("option_prices", "all", file_name)
+    logger.info(f"Processing {file_path}")
     df = pd.read_csv(file_path)
     df = process_daily_prices(df)
     df.to_csv(destination, index=False)
 
 
 def process_folder(folder_path):
     for day in os.listdir(folder_path):
@@ -183,34 +196,32 @@
 
 
 def insert_csv_to_db(csv_file: str, engine_url: str) -> None:
     engine = create_engine(engine_url)
 
     # Read the CSV file
     df = pd.read_csv(csv_file)
-    df.drop(columns=["volume", "open_interest"], inplace=True)
     df["timestamp"] = pd.to_datetime(df["timestamp"])
-    df["expiry"] = pd.to_datetime(df["expiry"], format="%d%b%y")
-    df["expiry"] = df["expiry"] + timedelta(hours=15, minutes=30)
+    df["expiry"] = pd.to_datetime(df["expiry"])
 
     df.to_sql("index_options", con=engine, if_exists="append", index=False)
 
     logger.info(f"Inserted {csv_file} into the database")
 
 
 def get_new_daily_data(
     database_connection, remote_base_directory, local_base_directory
 ):
     host = os.getenv("GDFL_FTP_HOST")
     username = os.getenv("GDFL_FTP_USER")
     password = os.getenv("GDFL_FTP_PASS")
 
     dates_present = database_connection.execute_query(
-        "SELECT DISTINCT DATE(timestamp) FROM index_options"
-    )
+        "SELECT DISTINCT DATE(timestamp) FROM index_options WHERE underlying = 'NIFTY'"
+    )  # Nifty as a proxy to get the max date of NSE data (DB contains NSE and BSE data)
     dates_present = [date[0] for date in dates_present]
 
     new_files = []  # List to keep track of new files
     for attempt in range(3):
         try:
             with FTPConnection(host, username, password) as ftp:
                 zip_files = find_zip_files(ftp, remote_base_directory)
```

### Comparing `volstreet-8.1.3/volstreet/datamodule/eod_client.py` & `volstreet-8.2.0/volstreet/datamodule/eod_client.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/datamodule/gambling.py` & `volstreet-8.2.0/volstreet/datamodule/gambling.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/datamodule/intraday_data.py` & `volstreet-8.2.0/volstreet/datamodule/intraday_data.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/datamodule/stockmock.py` & `volstreet-8.2.0/volstreet/datamodule/stockmock.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/datamodule/trading_assistance.py` & `volstreet-8.2.0/volstreet/datamodule/trading_assistance.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/dealingroom.py` & `volstreet-8.2.0/volstreet/dealingroom.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,19 @@
 from volstreet.utils import (
     notifier,
     current_time,
     time_to_expiry,
     round_to_nearest,
     parse_symbol,
     find_strike,
-    check_for_weekend,
 )
 from volstreet.angel_interface.interface import lookup_and_return
 from volstreet.angel_interface.price_websocket import PriceWebsocket
 from volstreet.trade_interface import (
     Option,
-    Index,
 )
 from volstreet import blackscholes as bs
 
 
 class OptionChains(defaultdict):
     """An object for having option chains for multiple expiries.
     Each expiry is a dictionary with integer default values"""
@@ -557,60 +555,14 @@
                 "qty": qty_in_lots,
                 "order_type": "MARKET",
                 "time": current_time(),
             }
         )
 
 
-def get_strangle_indices_to_trade(*indices: Index) -> list[Index] | list[None]:
-    safe_indices = ["NIFTY", "BANKNIFTY", "FINNIFTY"]
-
-    times_to_expiries = [
-        time_to_expiry(index.current_expiry, effective_time=True, in_days=True)
-        for index in indices
-    ]
-
-    # Check if any index has less than 1 day to expiry
-    indices_less_than_1_day = [
-        index
-        for index, time_left_to_expiry in zip(indices, times_to_expiries)
-        if time_left_to_expiry < 1
-    ]
-
-    if indices_less_than_1_day:
-        return indices_less_than_1_day
-
-    # If no index has less than 1 day to expiry
-    min_expiry_time = min(times_to_expiries)
-    indices_with_closest_expiries = [
-        index
-        for index, time_left_to_expiry in zip(indices, times_to_expiries)
-        if time_left_to_expiry == min_expiry_time
-    ]
-    weekend_in_range = check_for_weekend(
-        indices_with_closest_expiries[0].current_expiry
-    )
-
-    if weekend_in_range:
-        # Checking if the closest indices are safe indices
-        safe_and_close = [
-            index
-            for index in indices_with_closest_expiries
-            if index.name in safe_indices
-        ]
-        if (
-            safe_and_close
-        ):  # If the indices with the closest expiry are safe indices then return the closest indices
-            return safe_and_close
-        else:  # If the indices with the closest expiry are not safe indices then return safe indices
-            return [index for index in indices if index.name in safe_indices]
-
-    return indices_with_closest_expiries
-
-
 def calc_combined_premium(
     spot,
     time_left,
     strike=None,
     call_strike=None,
     put_strike=None,
     iv=None,
```

### Comparing `volstreet-8.1.3/volstreet/decorators.py` & `volstreet-8.2.0/volstreet/decorators.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/discord_bot.py` & `volstreet-8.2.0/volstreet/discord_bot.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/exceptions.py` & `volstreet-8.2.0/volstreet/exceptions.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/historical_info/__init__.py` & `volstreet-8.2.0/volstreet/historical_info/__init__.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/historical_info/index_expiries.pkl` & `volstreet-8.2.0/volstreet/historical_info/index_expiries.pkl`

 * *Files 11% similar despite different names*

```diff
@@ -1,1162 +1,1315 @@
-00000000: 8004 9593 4800 0000 0000 007d 9428 8c05  ....H......}.(..
+00000000: 8004 951c 5200 0000 0000 007d 9428 8c05  ....R......}.(..
 00000010: 4e49 4654 5994 5d94 288c 1e70 616e 6461  NIFTY.].(..panda
 00000020: 732e 5f6c 6962 732e 7473 6c69 6273 2e74  s._libs.tslibs.t
 00000030: 696d 6573 7461 6d70 7394 8c13 5f75 6e70  imestamps..._unp
 00000040: 6963 6b6c 655f 7469 6d65 7374 616d 7094  ickle_timestamp.
-00000050: 9394 288a 0800 b0a8 78ab 4483 154e 4e4b  ..(.....x.D..NNK
-00000060: 0a74 9452 9468 0528 8a08 00b0 d171 bb6a  .t.R.h.(.....q.j
-00000070: 8515 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00000080: b0fa 6acb 9087 154e 4e4b 0a74 9452 9468  ..j....NNK.t.R.h
-00000090: 0528 8a08 00b0 2364 dbb6 8915 4e4e 4b0a  .(....#d....NNK.
-000000a0: 7494 5294 6805 288a 0800 b04c 5deb dc8b  t.R.h.(....L]...
+00000050: 9394 288a 0800 b0d4 7069 9126 164e 4e4b  ..(.....pi.&.NNK
+00000060: 0a74 9452 9468 0528 8a08 00b0 ec16 e7a6  .t.R.h.(........
+00000070: e316 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00000080: b024 b96a 6ebf 154e 4e4b 0a74 9452 9468  .$.jn..NNK.t.R.h
+00000090: 0528 8a08 00b0 6e2c 090e 3c16 4e4e 4b0a  .(....n,..<.NNK.
+000000a0: 7494 5294 6805 288a 0800 b0f1 96ba 2cca  t.R.h.(.......,.
 000000b0: 154e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-000000c0: 26c5 66b4 8d15 4e4e 4b0a 7494 5294 6805  &.f...NNK.t.R.h.
-000000d0: 288a 0800 b09e 4f0b 2990 154e 4e4b 0a74  (.....O.)..NNK.t
-000000e0: 9452 9468 0528 8a08 00b0 c748 1b4f 9215  .R.h.(.....H.O..
-000000f0: 4e4e 4b0a 7494 5294 6805 288a 0800 b0f0  NNK.t.R.h.(.....
-00000100: 412b 7594 154e 4e4b 0a74 9452 9468 0528  A+u..NNK.t.R.h.(
-00000110: 8a08 00b0 193b 3b9b 9615 4e4e 4b0a 7494  .....;;...NNK.t.
-00000120: 5294 6805 288a 0800 b042 344b c198 154e  R.h.(....B4K...N
-00000130: 4e4b 0a74 9452 9468 0528 8a08 00b0 6b2d  NK.t.R.h.(....k-
-00000140: 5be7 9a15 4e4e 4b0a 7494 5294 6805 288a  [...NNK.t.R.h.(.
-00000150: 0800 b094 266b 0d9d 154e 4e4b 0a74 9452  ....&k...NNK.t.R
-00000160: 9468 0528 8a08 00b0 bd1f 7b33 9f15 4e4e  .h.(......{3..NN
-00000170: 4b0a 7494 5294 6805 288a 0800 b0e6 188b  K.t.R.h.(.......
-00000180: 59a1 154e 4e4b 0a74 9452 9468 0528 8a08  Y..NNK.t.R.h.(..
-00000190: 00b0 0f12 9b7f a315 4e4e 4b0a 7494 5294  ........NNK.t.R.
-000001a0: 6805 288a 0800 b038 0bab a5a5 154e 4e4b  h.(....8.....NNK
-000001b0: 0a74 9452 9468 0528 8a08 00b0 6104 bbcb  .t.R.h.(....a...
-000001c0: a715 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-000001d0: b08a fdca f1a9 154e 4e4b 0a74 9452 9468  .......NNK.t.R.h
-000001e0: 0528 8a08 00b0 b3f6 da17 ac15 4e4e 4b0a  .(..........NNK.
-000001f0: 7494 5294 6805 288a 0800 b0dc efea 3dae  t.R.h.(.......=.
+000000c0: cff0 950b 4017 4e4e 4b0a 7494 5294 6805  ....@.NNK.t.R.h.
+000000d0: 288a 0800 b0f5 eaf7 0aa1 164e 4e4b 0a74  (..........NNK.t
+000000e0: 9452 9468 0528 8a08 00b0 9e78 0439 b617  .R.h.(.....x.9..
+000000f0: 4e4e 4b0a 7494 5294 6805 288a 0800 b0f9  NNK.t.R.h.(.....
+00000100: 672e f99d 194e 4e4b 0a74 9452 9468 0528  g....NNK.t.R.h.(
+00000110: 8a08 00b0 b74a 18f6 8216 4e4e 4b0a 7494  .....J....NNK.t.
+00000120: 5294 6805 288a 0800 b053 b0d6 e103 174e  R.h.(....S.....N
+00000130: 4e4b 0a74 9452 9468 0528 8a08 00b0 957b  NK.t.R.h.(.....{
+00000140: fac4 d215 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
+00000150: 0800 b080 d42a d6b6 154e 4e4b 0a74 9452  .....*...NNK.t.R
+00000160: 9468 0528 8a08 00b0 6c82 ea9e d015 4e4e  .h.(....l.....NN
+00000170: 4b0a 7494 5294 6805 288a 0800 b0dd 447a  K.t.R.h.(.....Dz
+00000180: f5e3 154e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+00000190: 00b0 11bc b9ee 0e16 4e4e 4b0a 7494 5294  ........NNK.t.R.
+000001a0: 6805 288a 0800 b0a4 4d67 76d2 164e 4e4b  h.(.....Mgv..NNK
+000001b0: 0a74 9452 9468 0528 8a08 00b0 7ca9 e607  .t.R.h.(....|...
+000001c0: 0617 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+000001d0: b0a8 78ab 4483 154e 4e4b 0a74 9452 9468  ..x.D..NNK.t.R.h
+000001e0: 0528 8a08 00b0 208e 26a0 0e17 4e4e 4b0a  .(.... .&...NNK.
+000001f0: 7494 5294 6805 288a 0800 b0a0 f929 98fb  t.R.h.(......)..
 00000200: 154e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00000210: 05e9 fa63 b015 4e4e 4b0a 7494 5294 6805  ...c..NNK.t.R.h.
-00000220: 288a 0800 b02e e20a 8ab2 154e 4e4b 0a74  (..........NNK.t
-00000230: 9452 9468 0528 8a08 00b0 57db 1ab0 b415  .R.h.(....W.....
-00000240: 4e4e 4b0a 7494 5294 6805 288a 0800 b080  NNK.t.R.h.(.....
-00000250: d42a d6b6 154e 4e4b 0a74 9452 9468 0528  .*...NNK.t.R.h.(
-00000260: 8a08 00b0 a9cd 3afc b815 4e4e 4b0a 7494  ......:...NNK.t.
-00000270: 5294 6805 288a 0800 b083 35b6 d3ba 154e  R.h.(.....5....N
-00000280: 4e4b 0a74 9452 9468 0528 8a08 00b0 fbbf  NK.t.R.h.(......
-00000290: 5a48 bd15 4e4e 4b0a 7494 5294 6805 288a  ZH..NNK.t.R.h.(.
-000002a0: 0800 b024 b96a 6ebf 154e 4e4b 0a74 9452  ...$.jn..NNK.t.R
-000002b0: 9468 0528 8a08 00b0 4db2 7a94 c115 4e4e  .h.(....M.z...NN
-000002c0: 4b0a 7494 5294 6805 288a 0800 b076 ab8a  K.t.R.h.(....v..
-000002d0: bac3 154e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-000002e0: 00b0 9fa4 9ae0 c515 4e4e 4b0a 7494 5294  ........NNK.t.R.
-000002f0: 6805 288a 0800 b0c8 9daa 06c8 154e 4e4b  h.(..........NNK
-00000300: 0a74 9452 9468 0528 8a08 00b0 f196 ba2c  .t.R.h.(.......,
-00000310: ca15 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00000320: b01a 90ca 52cc 154e 4e4b 0a74 9452 9468  ....R..NNK.t.R.h
-00000330: 0528 8a08 00b0 4389 da78 ce15 4e4e 4b0a  .(....C..x..NNK.
-00000340: 7494 5294 6805 288a 0800 b06c 82ea 9ed0  t.R.h.(....l....
+00000210: 238d d4c6 af17 4e4e 4b0a 7494 5294 6805  #.....NNK.t.R.h.
+00000220: 288a 0800 b0c4 7266 3817 174e 4e4b 0a74  (.....rf8..NNK.t
+00000230: 9452 9468 0528 8a08 00b0 14bb 6715 b016  .R.h.(......g...
+00000240: 4e4e 4b0a 7494 5294 6805 288a 0800 b044  NNK.t.R.h.(....D
+00000250: de69 3004 164e 4e4b 0a74 9452 9468 0528  .i0..NNK.t.R.h.(
+00000260: 8a08 00b0 8e51 08d0 8016 4e4e 4b0a 7494  .....Q....NNK.t.
+00000270: 5294 6805 288a 0800 b025 0efa 25f5 154e  R.h.(....%..%..N
+00000280: 4e4b 0a74 9452 9468 0528 8a08 00b0 c748  NK.t.R.h.(.....H
+00000290: 1b4f 9215 4e4e 4b0a 7494 5294 6805 288a  .O..NNK.t.R.h.(.
+000002a0: 0800 b0cd 4677 9cd4 164e 4e4b 0a74 9452  ....Fw...NNK.t.R
+000002b0: 9468 0528 8a08 00b0 1366 d85d 7a16 4e4e  .h.(.....f.]z.NN
+000002c0: 4b0a 7494 5294 6805 288a 0800 b046 8888  K.t.R.h.(....F..
+000002d0: 9f6f 164e 4e4b 0a74 9452 9468 0528 8a08  .o.NNK.t.R.h.(..
+000002e0: 00b0 b89f a7ad b816 4e4e 4b0a 7494 5294  ........NNK.t.R.
+000002f0: 6805 288a 0800 b0af cb96 49fb 164e 4e4b  h.(.......I..NNK
+00000300: 0a74 9452 9468 0528 8a08 00b0 4f5c 9903  .t.R.h.(....O\..
+00000310: 2d16 4e4e 4b0a 7494 5294 6805 288a 0800  -.NNK.t.R.h.(...
+00000320: b07d fe75 bf3b 174e 4e4b 0a74 9452 9468  .}.u.;.NNK.t.R.h
+00000330: 0528 8a08 00b0 6b2d 5be7 9a15 4e4e 4b0a  .(....k-[...NNK.
+00000340: 7494 5294 6805 288a 0800 b006 3e8a 1be6  t.R.h.(.....>...
 00000350: 154e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00000360: 957b fac4 d215 4e4e 4b0a 7494 5294 6805  .{....NNK.t.R.h.
-00000370: 288a 0800 b0be 740a ebd4 154e 4e4b 0a74  (.....t....NNK.t
-00000380: 9452 9468 0528 8a08 00b0 e76d 1a11 d715  .R.h.(.....m....
-00000390: 4e4e 4b0a 7494 5294 6805 288a 0800 b010  NNK.t.R.h.(.....
-000003a0: 672a 37d9 154e 4e4b 0a74 9452 9468 0528  g*7..NNK.t.R.h.(
-000003b0: 8a08 00b0 3960 3a5d db15 4e4e 4b0a 7494  ....9`:]..NNK.t.
-000003c0: 5294 6805 288a 0800 b062 594a 83dd 154e  R.h.(....bYJ...N
-000003d0: 4e4b 0a74 9452 9468 0528 8a08 00b0 8b52  NK.t.R.h.(.....R
-000003e0: 5aa9 df15 4e4e 4b0a 7494 5294 6805 288a  Z...NNK.t.R.h.(.
-000003f0: 0800 b0b4 4b6a cfe1 154e 4e4b 0a74 9452  ....Kj...NNK.t.R
-00000400: 9468 0528 8a08 00b0 dd44 7af5 e315 4e4e  .h.(.....Dz...NN
-00000410: 4b0a 7494 5294 6805 288a 0800 b006 3e8a  K.t.R.h.(.....>.
-00000420: 1be6 154e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00000430: 00b0 2f37 9a41 e815 4e4e 4b0a 7494 5294  ../7.A..NNK.t.R.
-00000440: 6805 288a 0800 b058 30aa 67ea 154e 4e4b  h.(....X0.g..NNK
-00000450: 0a74 9452 9468 0528 8a08 00b0 8129 ba8d  .t.R.h.(.....)..
-00000460: ec15 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00000470: b0aa 22ca b3ee 154e 4e4b 0a74 9452 9468  .."....NNK.t.R.h
-00000480: 0528 8a08 00b0 d31b dad9 f015 4e4e 4b0a  .(..........NNK.
-00000490: 7494 5294 6805 288a 0800 b0fc 14ea fff2  t.R.h.(.........
-000004a0: 154e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-000004b0: 250e fa25 f515 4e4e 4b0a 7494 5294 6805  %..%..NNK.t.R.h.
-000004c0: 288a 0800 b04e 070a 4cf7 154e 4e4b 0a74  (....N..L..NNK.t
-000004d0: 9452 9468 0528 8a08 00b0 7700 1a72 f915  .R.h.(....w..r..
-000004e0: 4e4e 4b0a 7494 5294 6805 288a 0800 b0a0  NNK.t.R.h.(.....
-000004f0: f929 98fb 154e 4e4b 0a74 9452 9468 0528  .)...NNK.t.R.h.(
-00000500: 8a08 00b0 c9f2 39be fd15 4e4e 4b0a 7494  ......9...NNK.t.
-00000510: 5294 6805 288a 0800 b0f2 eb49 e4ff 154e  R.h.(......I...N
-00000520: 4e4b 0a74 9452 9468 0528 8a08 00b0 cc53  NK.t.R.h.(.....S
-00000530: c5bb 0116 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
-00000540: 0800 b044 de69 3004 164e 4e4b 0a74 9452  ...D.i0..NNK.t.R
-00000550: 9468 0528 8a08 00b0 6dd7 7956 0616 4e4e  .h.(....m.yV..NN
-00000560: 4b0a 7494 5294 6805 288a 0800 b096 d089  K.t.R.h.(.......
-00000570: 7c08 164e 4e4b 0a74 9452 9468 0528 8a08  |..NNK.t.R.h.(..
-00000580: 00b0 bfc9 99a2 0a16 4e4e 4b0a 7494 5294  ........NNK.t.R.
-00000590: 6805 288a 0800 b0e8 c2a9 c80c 164e 4e4b  h.(..........NNK
-000005a0: 0a74 9452 9468 0528 8a08 00b0 11bc b9ee  .t.R.h.(........
-000005b0: 0e16 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-000005c0: b03a b5c9 1411 164e 4e4b 0a74 9452 9468  .:.....NNK.t.R.h
-000005d0: 0528 8a08 00b0 63ae d93a 1316 4e4e 4b0a  .(....c..:..NNK.
-000005e0: 7494 5294 6805 288a 0800 b08c a7e9 6015  t.R.h.(.......`.
-000005f0: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00000600: b5a0 f986 1716 4e4e 4b0a 7494 5294 6805  ......NNK.t.R.h.
-00000610: 288a 0800 b0de 9909 ad19 164e 4e4b 0a74  (..........NNK.t
-00000620: 9452 9468 0528 8a08 00b0 0793 19d3 1b16  .R.h.(..........
-00000630: 4e4e 4b0a 7494 5294 6805 288a 0800 b030  NNK.t.R.h.(....0
-00000640: 8c29 f91d 164e 4e4b 0a74 9452 9468 0528  .)...NNK.t.R.h.(
-00000650: 8a08 00b0 5985 391f 2016 4e4e 4b0a 7494  ....Y.9. .NNK.t.
-00000660: 5294 6805 288a 0800 b082 7e49 4522 164e  R.h.(.....~IE".N
-00000670: 4e4b 0a74 9452 9468 0528 8a08 00b0 ab77  NK.t.R.h.(.....w
-00000680: 596b 2416 4e4e 4b0a 7494 5294 6805 288a  Yk$.NNK.t.R.h.(.
-00000690: 0800 b0d4 7069 9126 164e 4e4b 0a74 9452  ....pi.&.NNK.t.R
-000006a0: 9468 0528 8a08 00b0 fd69 79b7 2816 4e4e  .h.(.....iy.(.NN
-000006b0: 4b0a 7494 5294 6805 288a 0800 b026 6389  K.t.R.h.(....&c.
-000006c0: dd2a 164e 4e4b 0a74 9452 9468 0528 8a08  .*.NNK.t.R.h.(..
-000006d0: 00b0 4f5c 9903 2d16 4e4e 4b0a 7494 5294  ..O\..-.NNK.t.R.
-000006e0: 6805 288a 0800 b078 55a9 292f 164e 4e4b  h.(....xU.)/.NNK
-000006f0: 0a74 9452 9468 0528 8a08 00b0 a14e b94f  .t.R.h.(.....N.O
-00000700: 3116 4e4e 4b0a 7494 5294 6805 288a 0800  1.NNK.t.R.h.(...
-00000710: b0ca 47c9 7533 164e 4e4b 0a74 9452 9468  ..G.u3.NNK.t.R.h
-00000720: 0528 8a08 00b0 f340 d99b 3516 4e4e 4b0a  .(.....@..5.NNK.
-00000730: 7494 5294 6805 288a 0800 b01c 3ae9 c137  t.R.h.(.....:..7
-00000740: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00000750: 4533 f9e7 3916 4e4e 4b0a 7494 5294 6805  E3..9.NNK.t.R.h.
-00000760: 288a 0800 b06e 2c09 0e3c 164e 4e4b 0a74  (....n,..<.NNK.t
-00000770: 9452 9468 0528 8a08 00b0 9725 1934 3e16  .R.h.(.....%.4>.
-00000780: 4e4e 4b0a 7494 5294 6805 288a 0800 b0c0  NNK.t.R.h.(.....
-00000790: 1e29 5a40 164e 4e4b 0a74 9452 9468 0528  .)Z@.NNK.t.R.h.(
-000007a0: 8a08 00b0 e917 3980 4216 4e4e 4b0a 7494  ......9.B.NNK.t.
-000007b0: 5294 6805 288a 0800 b012 1149 a644 164e  R.h.(......I.D.N
-000007c0: 4e4b 0a74 9452 9468 0528 8a08 00b0 3b0a  NK.t.R.h.(....;.
-000007d0: 59cc 4616 4e4e 4b0a 7494 5294 6805 288a  Y.F.NNK.t.R.h.(.
-000007e0: 0800 b064 0369 f248 164e 4e4b 0a74 9452  ...d.i.H.NNK.t.R
-000007f0: 9468 0528 8a08 00b0 8dfc 7818 4b16 4e4e  .h.(......x.K.NN
-00000800: 4b0a 7494 5294 6805 288a 0800 b0b6 f588  K.t.R.h.(.......
-00000810: 3e4d 164e 4e4b 0a74 9452 9468 0528 8a08  >M.NNK.t.R.h.(..
+00000360: 5405 6699 3917 4e4e 4b0a 7494 5294 6805  T.f.9.NNK.t.R.h.
+00000370: 288a 0800 b057 db1a b0b4 154e 4e4b 0a74  (....W.....NNK.t
+00000380: 9452 9468 0528 8a08 00b0 21e3 b557 4417  .R.h.(....!..WD.
+00000390: 4e4e 4b0a 7494 5294 6805 288a 0800 b083  NNK.t.R.h.(.....
+000003a0: 35b6 d3ba 154e 4e4b 0a74 9452 9468 0528  5....NNK.t.R.h.(
+000003b0: 8a08 00b0 b020 2601 3117 4e4e 4b0a 7494  ..... &.1.NNK.t.
+000003c0: 5294 6805 288a 0800 b000 6927 dec9 164e  R.h.(.....i'...N
+000003d0: 4e4b 0a74 9452 9468 0528 8a08 00b0 fa6a  NK.t.R.h.(.....j
+000003e0: cb90 8715 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
+000003f0: 0800 b0a8 a1a4 54a9 174e 4e4b 0a74 9452  ......T..NNK.t.R
+00000400: 9468 0528 8a08 00b0 16c7 635b 7e16 4e4e  .h.(......c[~.NN
+00000410: 4b0a 7494 5294 6805 288a 0800 b054 6743  K.t.R.h.(....TgC
+00000420: 709c 164e 4e4b 0a74 9452 9468 0528 8a08  p..NNK.t.R.h.(..
+00000430: 00b0 944f 641d c317 4e4e 4b0a 7494 5294  ...Od...NNK.t.R.
+00000440: 6805 288a 0800 b059 8539 1f20 164e 4e4b  h.(....Y.9. .NNK
+00000450: 0a74 9452 9468 0528 8a08 00b0 180f a5f3  .t.R.h.(........
+00000460: 8617 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00000470: b023 b6cd d6d5 194e 4e4b 0a74 9452 9468  .#.....NNK.t.R.h
+00000480: 0528 8a08 00b0 5ada c8d6 5516 4e4e 4b0a  .(....Z...U.NNK.
+00000490: 7494 5294 6805 288a 0800 b033 8bd7 1fbf  t.R.h.(....3....
+000004a0: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+000004b0: 3e09 07f3 e716 4e4e 4b0a 7494 5294 6805  >.....NNK.t.R.h.
+000004c0: 288a 0800 b093 fad4 658d 174e 4e4b 0a74  (.......e..NNK.t
+000004d0: 9452 9468 0528 8a08 00b0 60d8 2424 9817  .R.h.(....`.$$..
+000004e0: 4e4e 4b0a 7494 5294 6805 288a 0800 b00e  NNK.t.R.h.(.....
+000004f0: e604 d893 174e 4e4b 0a74 9452 9468 0528  .....NNK.t.R.h.(
+00000500: 8a08 00b0 37df 14fe 9517 4e4e 4b0a 7494  ....7.....NNK.t.
+00000510: 5294 6805 288a 0800 b003 68d5 046b 174e  R.h.(.....h..k.N
+00000520: 4e4b 0a74 9452 9468 0528 8a08 00b0 c771  NK.t.R.h.(.....q
+00000530: 145f b817 4e4e 4b0a 7494 5294 6805 288a  ._..NNK.t.R.h.(.
+00000540: 0800 b097 2519 343e 164e 4e4b 0a74 9452  ....%.4>.NNK.t.R
+00000550: 9468 0528 8a08 00b0 c828 81ed 5017 4e4e  .h.(.....(..P.NN
+00000560: 4b0a 7494 5294 6805 288a 0800 b09d 2375  K.t.R.h.(.....#u
+00000570: 8180 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+00000580: 00b0 95a4 f3d4 f817 4e4e 4b0a 7494 5294  ........NNK.t.R.
+00000590: 6805 288a 0800 b0b4 4b6a cfe1 154e 4e4b  h.(.....Kj...NNK
+000005a0: 0a74 9452 9468 0528 8a08 00b0 da6e c5de  .t.R.h.(.....n..
+000005b0: 6817 4e4e 4b0a 7494 5294 6805 288a 0800  h.NNK.t.R.h.(...
+000005c0: b028 36a1 5cbc 184e 4e4b 0a74 9452 9468  .(6.\..NNK.t.R.h
+000005d0: 0528 8a08 00b0 e8c2 a9c8 0c16 4e4e 4b0a  .(..........NNK.
+000005e0: 7494 5294 6805 288a 0800 b09c cee5 c94a  t.R.h.(........J
+000005f0: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00000600: 1ee4 0731 a316 4e4e 4b0a 7494 5294 6805  ...1..NNK.t.R.h.
+00000610: 288a 0800 b067 0217 19ea 164e 4e4b 0a74  (....g.....NNK.t
+00000620: 9452 9468 0528 8a08 00b0 8b52 5aa9 df15  .R.h.(.....RZ...
+00000630: 4e4e 4b0a 7494 5294 6805 288a 0800 b0fd  NNK.t.R.h.(.....
+00000640: 6979 b728 164e 4e4b 0a74 9452 9468 0528  iy.(.NNK.t.R.h.(
+00000650: 8a08 00b0 2663 89dd 2a16 4e4e 4b0a 7494  ....&c..*.NNK.t.
+00000660: 5294 6805 288a 0800 b096 d089 7c08 164e  R.h.(.......|..N
+00000670: 4e4b 0a74 9452 9468 0528 8a08 00b0 f2eb  NK.t.R.h.(......
+00000680: 49e4 ff15 4e4e 4b0a 7494 5294 6805 288a  I...NNK.t.R.h.(.
+00000690: 0800 b0ca 47c9 7533 164e 4e4b 0a74 9452  ....G.u3.NNK.t.R
+000006a0: 9468 0528 8a08 00b0 cc53 c5bb 0116 4e4e  .h.(.....S....NN
+000006b0: 4b0a 7494 5294 6805 288a 0800 b0e0 4328  K.t.R.h.(.....C(
+000006c0: 1c85 164e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+000006d0: 00b0 c2c8 47c9 ab16 4e4e 4b0a 7494 5294  ....G...NNK.t.R.
+000006e0: 6805 288a 0800 b024 e263 7ee5 174e 4e4b  h.(....$.c~..NNK
+000006f0: 0a74 9452 9468 0528 8a08 00b0 3834 a4b5  .t.R.h.(....84..
+00000700: cb17 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00000710: b0ea 6cc8 3778 164e 4e4b 0a74 9452 9468  ..l.7x.NNK.t.R.h
+00000720: 0528 8a08 00b0 08e8 a88a 5116 4e4e 4b0a  .(........Q.NNK.
+00000730: 7494 5294 6805 288a 0800 b0d1 71bb 6a85  t.R.h.(.....q.j.
+00000740: 154e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00000750: 712b b734 dd16 4e4e 4b0a 7494 5294 6805  q+.4..NNK.t.R.h.
+00000760: 288a 0800 b01a 90ca 52cc 154e 4e4b 0a74  (.......R..NNK.t
+00000770: 9452 9468 0528 8a08 00b0 4832 a70e db16  .R.h.(....H2....
+00000780: 4e4e 4b0a 7494 5294 6805 288a 0800 b0e9  NNK.t.R.h.(.....
+00000790: 1739 8042 164e 4e4b 0a74 9452 9468 0528  .9.B.NNK.t.R.h.(
+000007a0: 8a08 00b0 bcf3 e48b 8f17 4e4e 4b0a 7494  ..........NNK.t.
+000007b0: 5294 6805 288a 0800 b0bd 1f7b 339f 154e  R.h.(......{3..N
+000007c0: 4e4b 0a74 9452 9468 0528 8a08 00b0 4e07  NK.t.R.h.(....N.
+000007d0: 0a4c f715 4e4e 4b0a 7494 5294 6805 288a  .L..NNK.t.R.h.(.
+000007e0: 0800 b06d d779 5606 164e 4e4b 0a74 9452  ...m.yV..NNK.t.R
+000007f0: 9468 0528 8a08 00b0 a14e b94f 3116 4e4e  .h.(.....N.O1.NN
+00000800: 4b0a 7494 5294 6805 288a 0800 b064 0369  K.t.R.h.(....d.i
+00000810: f248 164e 4e4b 0a74 9452 9468 0528 8a08  .H.NNK.t.R.h.(..
 00000820: 00b0 dfee 9864 4f16 4e4e 4b0a 7494 5294  .....dO.NNK.t.R.
-00000830: 6805 288a 0800 b008 e8a8 8a51 164e 4e4b  h.(........Q.NNK
-00000840: 0a74 9452 9468 0528 8a08 00b0 31e1 b8b0  .t.R.h.(....1...
-00000850: 5316 4e4e 4b0a 7494 5294 6805 288a 0800  S.NNK.t.R.h.(...
-00000860: b05a dac8 d655 164e 4e4b 0a74 9452 9468  .Z...U.NNK.t.R.h
-00000870: 0528 8a08 00b0 83d3 d8fc 5716 4e4e 4b0a  .(........W.NNK.
-00000880: 7494 5294 6805 288a 0800 b0ac cce8 225a  t.R.h.(......."Z
-00000890: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-000008a0: d5c5 f848 5c16 4e4e 4b0a 7494 5294 6805  ...H\.NNK.t.R.h.
-000008b0: 288a 0800 b0fe be08 6f5e 164e 4e4b 0a74  (.......o^.NNK.t
-000008c0: 9452 9468 0528 8a08 00b0 27b8 1895 6016  .R.h.(....'...`.
-000008d0: 4e4e 4b0a 7494 5294 6805 288a 0800 b050  NNK.t.R.h.(....P
-000008e0: b128 bb62 164e 4e4b 0a74 9452 9468 0528  .(.b.NNK.t.R.h.(
-000008f0: 8a08 00b0 79aa 38e1 6416 4e4e 4b0a 7494  ....y.8.d.NNK.t.
-00000900: 5294 6805 288a 0800 b0a2 a348 0767 164e  R.h.(......H.g.N
-00000910: 4e4b 0a74 9452 9468 0528 8a08 00b0 cb9c  NK.t.R.h.(......
-00000920: 582d 6916 4e4e 4b0a 7494 5294 6805 288a  X-i.NNK.t.R.h.(.
-00000930: 0800 b0a5 04d4 046b 164e 4e4b 0a74 9452  .......k.NNK.t.R
-00000940: 9468 0528 8a08 00b0 1d8f 7879 6d16 4e4e  .h.(......xym.NN
-00000950: 4b0a 7494 5294 6805 288a 0800 b046 8888  K.t.R.h.(....F..
-00000960: 9f6f 164e 4e4b 0a74 9452 9468 0528 8a08  .o.NNK.t.R.h.(..
-00000970: 00b0 6f81 98c5 7116 4e4e 4b0a 7494 5294  ..o...q.NNK.t.R.
-00000980: 6805 288a 0800 b098 7aa8 eb73 164e 4e4b  h.(.....z..s.NNK
-00000990: 0a74 9452 9468 0528 8a08 00b0 c173 b811  .t.R.h.(.....s..
-000009a0: 7616 4e4e 4b0a 7494 5294 6805 288a 0800  v.NNK.t.R.h.(...
-000009b0: b0ea 6cc8 3778 164e 4e4b 0a74 9452 9468  ..l.7x.NNK.t.R.h
-000009c0: 0528 8a08 00b0 1366 d85d 7a16 4e4e 4b0a  .(.....f.]z.NNK.
-000009d0: 7494 5294 6805 288a 0800 b03c 5fe8 837c  t.R.h.(....<_..|
-000009e0: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-000009f0: 16c7 635b 7e16 4e4e 4b0a 7494 5294 6805  ..c[~.NNK.t.R.h.
-00000a00: 288a 0800 b08e 5108 d080 164e 4e4b 0a74  (.....Q....NNK.t
-00000a10: 9452 9468 0528 8a08 00b0 b74a 18f6 8216  .R.h.(.....J....
-00000a20: 4e4e 4b0a 7494 5294 6805 288a 0800 b0e0  NNK.t.R.h.(.....
-00000a30: 4328 1c85 164e 4e4b 0a74 9452 9468 0528  C(...NNK.t.R.h.(
-00000a40: 8a08 00b0 093d 3842 8716 4e4e 4b0a 7494  .....=8B..NNK.t.
-00000a50: 5294 6805 288a 0800 b032 3648 6889 164e  R.h.(....26Hh..N
-00000a60: 4e4b 0a74 9452 9468 0528 8a08 00b0 5b2f  NK.t.R.h.(....[/
-00000a70: 588e 8b16 4e4e 4b0a 7494 5294 6805 288a  X...NNK.t.R.h.(.
-00000a80: 0800 b084 2868 b48d 164e 4e4b 0a74 9452  ....(h...NNK.t.R
-00000a90: 9468 0528 8a08 00b0 ad21 78da 8f16 4e4e  .h.(.....!x...NN
-00000aa0: 4b0a 7494 5294 6805 288a 0800 b0d6 1a88  K.t.R.h.(.......
-00000ab0: 0092 164e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00000ac0: 00b0 ff13 9826 9416 4e4e 4b0a 7494 5294  .....&..NNK.t.R.
-00000ad0: 6805 288a 0800 b028 0da8 4c96 164e 4e4b  h.(....(..L..NNK
-00000ae0: 0a74 9452 9468 0528 8a08 00b0 5106 b872  .t.R.h.(....Q..r
-00000af0: 9816 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00000b00: b07a ffc7 989a 164e 4e4b 0a74 9452 9468  .z.....NNK.t.R.h
-00000b10: 0528 8a08 00b0 5467 4370 9c16 4e4e 4b0a  .(....TgCp..NNK.
-00000b20: 7494 5294 6805 288a 0800 b0cc f1e7 e49e  t.R.h.(.........
+00000830: 6805 288a 0800 b07c d2df 172c 194e 4e4b  h.(....|...,.NNK
+00000840: 0a74 9452 9468 0528 8a08 00b0 4db2 7a94  .t.R.h.(....M.z.
+00000850: c115 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00000860: b0a2 a348 0767 164e 4e4b 0a74 9452 9468  ...H.g.NNK.t.R.h
+00000870: 0528 8a08 00b0 f8e9 a531 4217 4e4e 4b0a  .(.......1B.NNK.
+00000880: 7494 5294 6805 288a 0800 b0dc 18e4 4dd4  t.R.h.(.......M.
+00000890: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+000008a0: 0a92 c7f9 bc16 4e4e 4b0a 7494 5294 6805  ......NNK.t.R.h.
+000008b0: 288a 0800 b0d5 c5f8 485c 164e 4e4b 0a74  (.......H\.NNK.t
+000008c0: 9452 9468 0528 8a08 00b0 ebc1 57ef ad16  .R.h.(......W...
+000008d0: 4e4e 4b0a 7494 5294 6805 288a 0800 b036  NNK.t.R.h.(....6
+000008e0: 8a85 4660 174e 4e4b 0a74 9452 9468 0528  ..F`.NNK.t.R.h.(
+000008f0: 8a08 00b0 50b1 28bb 6216 4e4e 4b0a 7494  ....P.(.b.NNK.t.
+00000900: 5294 6805 288a 0800 b04c 86e4 ecb1 174e  R.h.(....L.....N
+00000910: 4e4b 0a74 9452 9468 0528 8a08 00b0 2ee2  NK.t.R.h.(......
+00000920: 0a8a b215 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
+00000930: 0800 b02b 0c56 7337 174e 4e4b 0a74 9452  ...+.Vs7.NNK.t.R
+00000940: 9468 0528 8a08 00b0 0793 19d3 1b16 4e4e  .h.(..........NN
+00000950: 4b0a 7494 5294 6805 288a 0800 b03d b477  K.t.R.h.(....=.w
+00000960: 3bb2 164e 4e4b 0a74 9452 9468 0528 8a08  ;..NNK.t.R.h.(..
+00000970: 00b0 4c5d ebdc 8b15 4e4e 4b0a 7494 5294  ..L]....NNK.t.R.
+00000980: 6805 288a 0800 b0c6 7e62 7ee5 164e 4e4b  h.(.....~b~..NNK
+00000990: 0a74 9452 9468 0528 8a08 00b0 6b56 54f7  .t.R.h.(....kVT.
+000009a0: c017 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+000009b0: b016 6586 841b 174e 4e4b 0a74 9452 9468  ..e....NNK.t.R.h
+000009c0: 0528 8a08 00b0 8a26 c401 d017 4e4e 4b0a  .(.....&....NNK.
+000009d0: 7494 5294 6805 288a 0800 b0a9 cd3a fcb8  t.R.h.(......:..
+000009e0: 154e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+000009f0: a5a2 f62d 0817 4e4e 4b0a 7494 5294 6805  ...-..NNK.t.R.h.
+00000a00: 288a 0800 b069 ac35 8855 174e 4e4b 0a74  (....i.5.U.NNK.t
+00000a10: 9452 9468 0528 8a08 00b0 5b2f 588e 8b16  .R.h.(....[/X...
+00000a20: 4e4e 4b0a 7494 5294 6805 288a 0800 b009  NNK.t.R.h.(.....
+00000a30: 3d38 4287 164e 4e4b 0a74 9452 9468 0528  =8B..NNK.t.R.h.(
+00000a40: 8a08 00b0 9fa4 9ae0 c515 4e4e 4b0a 7494  ..........NNK.t.
+00000a50: 5294 6805 288a 0800 b081 29ba 8dec 154e  R.h.(.....)....N
+00000a60: 4e4b 0a74 9452 9468 0528 8a08 00b0 8727  NK.t.R.h.(.....'
+00000a70: 16db 2e17 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
+00000a80: 0800 b062 594a 83dd 154e 4e4b 0a74 9452  ...bYJ...NNK.t.R
+00000a90: 9468 0528 8a08 00b0 63ae d93a 1316 4e4e  .h.(....c..:..NN
+00000aa0: 4b0a 7494 5294 6805 288a 0800 b0c1 73b8  K.t.R.h.(.....s.
+00000ab0: 1176 164e 4e4b 0a74 9452 9468 0528 8a08  .v.NNK.t.R.h.(..
+00000ac0: 00b0 c9f2 39be fd15 4e4e 4b0a 7494 5294  ....9...NNK.t.R.
+00000ad0: 6805 288a 0800 b072 8046 ec12 174e 4e4b  h.(....r.F...NNK
+00000ae0: 0a74 9452 9468 0528 8a08 00b0 4adc c57d  .t.R.h.(....J..}
+00000af0: 4617 4e4e 4b0a 7494 5294 6805 288a 0800  F.NNK.t.R.h.(...
+00000b00: b0d0 4525 c375 174e 4e4b 0a74 9452 9468  ..E%.u.NNK.t.R.h
+00000b10: 0528 8a08 00b0 2db6 74e2 a217 4e4e 4b0a  .(....-.t...NNK.
+00000b20: 7494 5294 6805 288a 0800 b0ad 2178 da8f  t.R.h.(.....!x..
 00000b30: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00000b40: f5ea f70a a116 4e4e 4b0a 7494 5294 6805  ......NNK.t.R.h.
-00000b50: 288a 0800 b01e e407 31a3 164e 4e4b 0a74  (.......1..NNK.t
-00000b60: 9452 9468 0528 8a08 00b0 47dd 1757 a516  .R.h.(....G..W..
-00000b70: 4e4e 4b0a 7494 5294 6805 288a 0800 b070  NNK.t.R.h.(....p
-00000b80: d627 7da7 164e 4e4b 0a74 9452 9468 0528  .'}..NNK.t.R.h.(
-00000b90: 8a08 00b0 99cf 37a3 a916 4e4e 4b0a 7494  ......7...NNK.t.
-00000ba0: 5294 6805 288a 0800 b0c2 c847 c9ab 164e  R.h.(......G...N
-00000bb0: 4e4b 0a74 9452 9468 0528 8a08 00b0 ebc1  NK.t.R.h.(......
-00000bc0: 57ef ad16 4e4e 4b0a 7494 5294 6805 288a  W...NNK.t.R.h.(.
-00000bd0: 0800 b014 bb67 15b0 164e 4e4b 0a74 9452  .....g...NNK.t.R
-00000be0: 9468 0528 8a08 00b0 3db4 773b b216 4e4e  .h.(....=.w;..NN
-00000bf0: 4b0a 7494 5294 6805 288a 0800 b017 1cf3  K.t.R.h.(.......
-00000c00: 12b4 164e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00000c10: 00b0 8fa6 9787 b616 4e4e 4b0a 7494 5294  ........NNK.t.R.
-00000c20: 6805 288a 0800 b0b8 9fa7 adb8 164e 4e4b  h.(..........NNK
-00000c30: 0a74 9452 9468 0528 8a08 00b0 e198 b7d3  .t.R.h.(........
-00000c40: ba16 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00000c50: b00a 92c7 f9bc 164e 4e4b 0a74 9452 9468  .......NNK.t.R.h
-00000c60: 0528 8a08 00b0 338b d71f bf16 4e4e 4b0a  .(....3.....NNK.
-00000c70: 7494 5294 6805 288a 0800 b05c 84e7 45c1  t.R.h.(....\..E.
+00000b40: ae76 0792 c516 4e4e 4b0a 7494 5294 6805  .v....NNK.t.R.h.
+00000b50: 288a 0800 b080 fd23 e6dc 174e 4e4b 0a74  (......#...NNK.t
+00000b60: 9452 9468 0528 8a08 00b0 5c84 e745 c116  .R.h.(....\..E..
+00000b70: 4e4e 4b0a 7494 5294 6805 288a 0800 b052  NNK.t.R.h.(....R
+00000b80: 5b47 2ace 164e 4e4b 0a74 9452 9468 0528  [G*..NNK.t.R.h.(
+00000b90: 8a08 00b0 cb9c 582d 6916 4e4e 4b0a 7494  ......X-i.NNK.t.
+00000ba0: 5294 6805 288a 0800 b028 0da8 4c96 164e  R.h.(....(..L..N
+00000bb0: 4e4b 0a74 9452 9468 0528 8a08 00b0 2962  NK.t.R.h.(....)b
+00000bc0: 3704 cc16 4e4e 4b0a 7494 5294 6805 288a  7...NNK.t.R.h.(.
+00000bd0: 0800 b040 b325 6253 174e 4e4b 0a74 9452  ...@.%bS.NNK.t.R
+00000be0: 9468 0528 8a08 00b0 89d1 344a 9a17 4e4e  .h.(......4J..NN
+00000bf0: 4b0a 7494 5294 6805 288a 0800 b00b e756  K.t.R.h.(......V
+00000c00: b1f2 164e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+00000c10: 00b0 76ab 8aba c315 4e4e 4b0a 7494 5294  ..v.....NNK.t.R.
+00000c20: 6805 288a 0800 b027 b818 9560 164e 4e4b  h.(....'...`.NNK
+00000c30: 0a74 9452 9468 0528 8a08 00b0 7700 1a72  .t.R.h.(....w..r
+00000c40: f915 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00000c50: b0ab 7759 6b24 164e 4e4b 0a74 9452 9468  ..wYk$.NNK.t.R.h
+00000c60: 0528 8a08 00b0 555a f550 6f17 4e4e 4b0a  .(....UZ.Po.NNK.
+00000c70: 7494 5294 6805 288a 0800 b0a5 04d4 046b  t.R.h.(........k
 00000c80: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00000c90: 857d f76b c316 4e4e 4b0a 7494 5294 6805  .}.k..NNK.t.R.h.
-00000ca0: 288a 0800 b0ae 7607 92c5 164e 4e4b 0a74  (.....v....NNK.t
-00000cb0: 9452 9468 0528 8a08 00b0 d76f 17b8 c716  .R.h.(.....o....
-00000cc0: 4e4e 4b0a 7494 5294 6805 288a 0800 b000  NNK.t.R.h.(.....
-00000cd0: 6927 dec9 164e 4e4b 0a74 9452 9468 0528  i'...NNK.t.R.h.(
-00000ce0: 8a08 00b0 2962 3704 cc16 4e4e 4b0a 7494  ....)b7...NNK.t.
-00000cf0: 5294 6805 288a 0800 b052 5b47 2ace 164e  R.h.(....R[G*..N
-00000d00: 4e4b 0a74 9452 9468 0528 8a08 00b0 7b54  NK.t.R.h.(....{T
-00000d10: 5750 d016 4e4e 4b0a 7494 5294 6805 288a  WP..NNK.t.R.h.(.
-00000d20: 0800 b0a4 4d67 76d2 164e 4e4b 0a74 9452  ....Mgv..NNK.t.R
-00000d30: 9468 0528 8a08 00b0 cd46 779c d416 4e4e  .h.(.....Fw...NN
-00000d40: 4b0a 7494 5294 6805 288a 0800 b0f6 3f87  K.t.R.h.(.....?.
-00000d50: c2d6 164e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00000d60: 00b0 1f39 97e8 d816 4e4e 4b0a 7494 5294  ...9....NNK.t.R.
-00000d70: 6805 288a 0800 b048 32a7 0edb 164e 4e4b  h.(....H2....NNK
-00000d80: 0a74 9452 9468 0528 8a08 00b0 712b b734  .t.R.h.(....q+.4
-00000d90: dd16 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00000da0: b09a 24c7 5adf 164e 4e4b 0a74 9452 9468  ..$.Z..NNK.t.R.h
-00000db0: 0528 8a08 00b0 c31d d780 e116 4e4e 4b0a  .(..........NNK.
-00000dc0: 7494 5294 6805 288a 0800 b0ec 16e7 a6e3  t.R.h.(.........
-00000dd0: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00000de0: c67e 627e e516 4e4e 4b0a 7494 5294 6805  .~b~..NNK.t.R.h.
-00000df0: 288a 0800 b03e 0907 f3e7 164e 4e4b 0a74  (....>.....NNK.t
-00000e00: 9452 9468 0528 8a08 00b0 6702 1719 ea16  .R.h.(....g.....
-00000e10: 4e4e 4b0a 7494 5294 6805 288a 0800 b090  NNK.t.R.h.(.....
-00000e20: fb26 3fec 164e 4e4b 0a74 9452 9468 0528  .&?..NNK.t.R.h.(
-00000e30: 8a08 00b0 b9f4 3665 ee16 4e4e 4b0a 7494  ......6e..NNK.t.
-00000e40: 5294 6805 288a 0800 b0e2 ed46 8bf0 164e  R.h.(......F...N
-00000e50: 4e4b 0a74 9452 9468 0528 8a08 00b0 0be7  NK.t.R.h.(......
-00000e60: 56b1 f216 4e4e 4b0a 7494 5294 6805 288a  V...NNK.t.R.h.(.
-00000e70: 0800 b034 e066 d7f4 164e 4e4b 0a74 9452  ...4.f...NNK.t.R
-00000e80: 9468 0528 8a08 00b0 5dd9 76fd f616 4e4e  .h.(....].v...NN
-00000e90: 4b0a 7494 5294 6805 288a 0800 b086 d286  K.t.R.h.(.......
-00000ea0: 23f9 164e 4e4b 0a74 9452 9468 0528 8a08  #..NNK.t.R.h.(..
-00000eb0: 00b0 afcb 9649 fb16 4e4e 4b0a 7494 5294  .....I..NNK.t.R.
-00000ec0: 6805 288a 0800 b0d8 c4a6 6ffd 164e 4e4b  h.(.......o..NNK
-00000ed0: 0a74 9452 9468 0528 8a08 00b0 01be b695  .t.R.h.(........
-00000ee0: ff16 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00000ef0: b02a b7c6 bb01 174e 4e4b 0a74 9452 9468  .*.....NNK.t.R.h
-00000f00: 0528 8a08 00b0 53b0 d6e1 0317 4e4e 4b0a  .(....S.....NNK.
-00000f10: 7494 5294 6805 288a 0800 b07c a9e6 0706  t.R.h.(....|....
+00000c90: f93e 35e9 7717 4e4e 4b0a 7494 5294 6805  .>5.w.NNK.t.R.h.
+00000ca0: 288a 0800 b06e b7df f4c4 174e 4e4b 0a74  (....n.....NNK.t
+00000cb0: 9452 9468 0528 8a08 00b0 2f37 9a41 e815  .R.h.(..../7.A..
+00000cc0: 4e4e 4b0a 7494 5294 6805 288a 0800 b045  NNK.t.R.h.(....E
+00000cd0: 33f9 e739 164e 4e4b 0a74 9452 9468 0528  3..9.NNK.t.R.h.(
+00000ce0: 8a08 00b0 83d3 d8fc 5716 4e4e 4b0a 7494  ........W.NNK.t.
+00000cf0: 5294 6805 288a 0800 b04b 3155 357c 174e  R.h.(....K1U5|.N
+00000d00: 4e4b 0a74 9452 9468 0528 8a08 00b0 3960  NK.t.R.h.(....9`
+00000d10: 3a5d db15 4e4e 4b0a 7494 5294 6805 288a  :]..NNK.t.R.h.(.
+00000d20: 0800 b08c a7e9 6015 164e 4e4b 0a74 9452  ......`..NNK.t.R
+00000d30: 9468 0528 8a08 00b0 ed6b 765e 1917 4e4e  .h.(.....kv^..NN
+00000d40: 4b0a 7494 5294 6805 288a 0800 b05e 2e06  K.t.R.h.(....^..
+00000d50: b52c 174e 4e4b 0a74 9452 9468 0528 8a08  .,.NNK.t.R.h.(..
+00000d60: 00b0 b9f4 3665 ee16 4e4e 4b0a 7494 5294  ....6e..NNK.t.R.
+00000d70: 6805 288a 0800 b0ce 9b06 540a 174e 4e4b  h.(.......T..NNK
+00000d80: 0a74 9452 9468 0528 8a08 00b0 d19a b47a  .t.R.h.(.......z
+00000d90: ab17 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00000da0: b042 344b c198 154e 4e4b 0a74 9452 9468  .B4K...NNK.t.R.h
+00000db0: 0528 8a08 00b0 d31b dad9 f015 4e4e 4b0a  .(..........NNK.
+00000dc0: 7494 5294 6805 288a 0800 b049 8736 c610  t.R.h.(....I.6..
+00000dd0: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00000de0: 9150 b6f6 2117 4e4e 4b0a 7494 5294 6805  .P..!.NNK.t.R.h.
+00000df0: 288a 0800 b0ba 49c6 1c24 174e 4e4b 0a74  (.....I..$.NNK.t
+00000e00: 9452 9468 0528 8a08 00b0 425d 44d1 be17  .R.h.(....B]D...
+00000e10: 4e4e 4b0a 7494 5294 6805 288a 0800 b058  NNK.t.R.h.(....X
+00000e20: 30aa 67ea 154e 4e4b 0a74 9452 9468 0528  0.g..NNK.t.R.h.(
+00000e30: 8a08 00b0 bfc9 99a2 0a16 4e4e 4b0a 7494  ..........NNK.t.
+00000e40: 5294 6805 288a 0800 b0b3 1fd4 27d2 174e  R.h.(.......'..N
+00000e50: 4e4b 0a74 9452 9468 0528 8a08 00b0 accc  NK.t.R.h.(......
+00000e60: e822 5a16 4e4e 4b0a 7494 5294 6805 288a  ."Z.NNK.t.R.h.(.
+00000e70: 0800 b00f 129b 7fa3 154e 4e4b 0a74 9452  .........NNK.t.R
+00000e80: 9468 0528 8a08 00b0 7aff c798 9a16 4e4e  .h.(....z.....NN
+00000e90: 4b0a 7494 5294 6805 288a 0800 b047 dd17  K.t.R.h.(....G..
+00000ea0: 57a5 164e 4e4b 0a74 9452 9468 0528 8a08  W..NNK.t.R.h.(..
+00000eb0: 00b0 1d8f 7879 6d16 4e4e 4b0a 7494 5294  ....xym.NNK.t.R.
+00000ec0: 6805 288a 0800 b0b2 ca44 709c 174e 4e4b  h.(......Dp..NNK
+00000ed0: 0a74 9452 9468 0528 8a08 00b0 e198 b7d3  .t.R.h.(........
+00000ee0: ba16 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00000ef0: b073 d5d5 a348 174e 4e4b 0a74 9452 9468  .s...H.NNK.t.R.h
+00000f00: 0528 8a08 00b0 6a01 c53f 8b17 4e4e 4b0a  .(....j..?..NNK.
+00000f10: 7494 5294 6805 288a 0800 b07f a894 2ea7  t.R.h.(.........
 00000f20: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00000f30: a5a2 f62d 0817 4e4e 4b0a 7494 5294 6805  ...-..NNK.t.R.h.
-00000f40: 288a 0800 b0ce 9b06 540a 174e 4e4b 0a74  (.......T..NNK.t
-00000f50: 9452 9468 0528 8a08 00b0 f794 167a 0c17  .R.h.(.......z..
-00000f60: 4e4e 4b0a 7494 5294 6805 288a 0800 b020  NNK.t.R.h.(.... 
-00000f70: 8e26 a00e 174e 4e4b 0a74 9452 9468 0528  .&...NNK.t.R.h.(
-00000f80: 8a08 00b0 4987 36c6 1017 4e4e 4b0a 7494  ....I.6...NNK.t.
-00000f90: 5294 6805 288a 0800 b072 8046 ec12 174e  R.h.(....r.F...N
-00000fa0: 4e4b 0a74 9452 9468 0528 8a08 00b0 9b79  NK.t.R.h.(.....y
-00000fb0: 5612 1517 4e4e 4b0a 7494 5294 6805 288a  V...NNK.t.R.h.(.
-00000fc0: 0800 b0c4 7266 3817 174e 4e4b 0a74 9452  ....rf8..NNK.t.R
-00000fd0: 9468 0528 8a08 00b0 ed6b 765e 1917 4e4e  .h.(.....kv^..NN
-00000fe0: 4b0a 7494 5294 6805 288a 0800 b016 6586  K.t.R.h.(.....e.
-00000ff0: 841b 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00001000: 00b0 3f5e 96aa 1d17 4e4e 4b0a 7494 5294  ..?^....NNK.t.R.
-00001010: 6805 288a 0800 b068 57a6 d01f 174e 4e4b  h.(....hW....NNK
-00001020: 0a74 9452 9468 0528 8a08 00b0 9150 b6f6  .t.R.h.(.....P..
-00001030: 2117 4e4e 4b0a 7494 5294 6805 288a 0800  !.NNK.t.R.h.(...
-00001040: b0ba 49c6 1c24 174e 4e4b 0a74 9452 9468  ..I..$.NNK.t.R.h
-00001050: 0528 8a08 00b0 e342 d642 2617 4e4e 4b0a  .(.....B.B&.NNK.
-00001060: 7494 5294 6805 288a 0800 b00c 3ce6 6828  t.R.h.(.....<.h(
-00001070: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00001080: 3535 f68e 2a17 4e4e 4b0a 7494 5294 6805  55..*.NNK.t.R.h.
-00001090: 288a 0800 b05e 2e06 b52c 174e 4e4b 0a74  (....^...,.NNK.t
-000010a0: 9452 9468 0528 8a08 00b0 8727 16db 2e17  .R.h.(.....'....
-000010b0: 4e4e 4b0a 7494 5294 6805 288a 0800 b0b0  NNK.t.R.h.(.....
-000010c0: 2026 0131 174e 4e4b 0a74 9452 9468 0528   &.1.NNK.t.R.h.(
-000010d0: 8a08 00b0 d919 3627 3317 4e4e 4b0a 7494  ......6'3.NNK.t.
-000010e0: 5294 6805 288a 0800 b002 1346 4d35 174e  R.h.(......FM5.N
-000010f0: 4e4b 0a74 9452 9468 0528 8a08 00b0 2b0c  NK.t.R.h.(....+.
-00001100: 5673 3717 4e4e 4b0a 7494 5294 6805 288a  Vs7.NNK.t.R.h.(.
-00001110: 0800 b054 0566 9939 174e 4e4b 0a74 9452  ...T.f.9.NNK.t.R
-00001120: 9468 0528 8a08 00b0 7dfe 75bf 3b17 4e4e  .h.(....}.u.;.NN
-00001130: 4b0a 7494 5294 6805 288a 0800 b057 66f1  K.t.R.h.(....Wf.
-00001140: 963d 174e 4e4b 0a74 9452 9468 0528 8a08  .=.NNK.t.R.h.(..
-00001150: 00b0 cff0 950b 4017 4e4e 4b0a 7494 5294  ......@.NNK.t.R.
-00001160: 6805 288a 0800 b0f8 e9a5 3142 174e 4e4b  h.(.......1B.NNK
-00001170: 0a74 9452 9468 0528 8a08 00b0 21e3 b557  .t.R.h.(....!..W
-00001180: 4417 4e4e 4b0a 7494 5294 6805 288a 0800  D.NNK.t.R.h.(...
-00001190: b04a dcc5 7d46 174e 4e4b 0a74 9452 9468  .J..}F.NNK.t.R.h
-000011a0: 0528 8a08 00b0 73d5 d5a3 4817 4e4e 4b0a  .(....s...H.NNK.
-000011b0: 7494 5294 6805 288a 0800 b09c cee5 c94a  t.R.h.(........J
-000011c0: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-000011d0: c5c7 f5ef 4c17 4e4e 4b0a 7494 5294 6805  ....L.NNK.t.R.h.
-000011e0: 288a 0800 b0ee c005 164f 174e 4e4b 0a74  (........O.NNK.t
-000011f0: 9452 9468 0528 8a08 00b0 c828 81ed 5017  .R.h.(.....(..P.
-00001200: 4e4e 4b0a 7494 5294 6805 288a 0800 b040  NNK.t.R.h.(....@
-00001210: b325 6253 174e 4e4b 0a74 9452 9468 0528  .%bS.NNK.t.R.h.(
-00001220: 8a08 00b0 69ac 3588 5517 4e4e 4b0a 7494  ....i.5.U.NNK.t.
-00001230: 5294 6805 288a 0800 b092 a545 ae57 174e  R.h.(......E.W.N
-00001240: 4e4b 0a74 9452 9468 0528 8a08 00b0 bb9e  NK.t.R.h.(......
-00001250: 55d4 5917 4e4e 4b0a 7494 5294 6805 288a  U.Y.NNK.t.R.h.(.
-00001260: 0800 b0e4 9765 fa5b 174e 4e4b 0a74 9452  .....e.[.NNK.t.R
-00001270: 9468 0528 8a08 00b0 0d91 7520 5e17 4e4e  .h.(......u ^.NN
-00001280: 4b0a 7494 5294 6805 288a 0800 b036 8a85  K.t.R.h.(....6..
-00001290: 4660 174e 4e4b 0a74 9452 9468 0528 8a08  F`.NNK.t.R.h.(..
-000012a0: 00b0 5f83 956c 6217 4e4e 4b0a 7494 5294  .._..lb.NNK.t.R.
-000012b0: 6805 288a 0800 b088 7ca5 9264 174e 4e4b  h.(.....|..d.NNK
-000012c0: 0a74 9452 9468 0528 8a08 00b0 b175 b5b8  .t.R.h.(.....u..
-000012d0: 6617 4e4e 4b0a 7494 5294 6805 288a 0800  f.NNK.t.R.h.(...
-000012e0: b0da 6ec5 de68 174e 4e4b 0a74 9452 9468  ..n..h.NNK.t.R.h
-000012f0: 0528 8a08 00b0 0368 d504 6b17 4e4e 4b0a  .(.....h..k.NNK.
-00001300: 7494 5294 6805 288a 0800 b0dd cf50 dc6c  t.R.h.(......P.l
-00001310: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00001320: 555a f550 6f17 4e4e 4b0a 7494 5294 6805  UZ.Po.NNK.t.R.h.
-00001330: 288a 0800 b07e 5305 7771 174e 4e4b 0a74  (....~S.wq.NNK.t
-00001340: 9452 9468 0528 8a08 00b0 a74c 159d 7317  .R.h.(.....L..s.
-00001350: 4e4e 4b0a 7494 5294 6805 288a 0800 b0d0  NNK.t.R.h.(.....
-00001360: 4525 c375 174e 4e4b 0a74 9452 9468 0528  E%.u.NNK.t.R.h.(
-00001370: 8a08 00b0 f93e 35e9 7717 4e4e 4b0a 7494  .....>5.w.NNK.t.
-00001380: 5294 6805 288a 0800 b022 3845 0f7a 174e  R.h.(...."8E.z.N
-00001390: 4e4b 0a74 9452 9468 0528 8a08 00b0 4b31  NK.t.R.h.(....K1
-000013a0: 5535 7c17 4e4e 4b0a 7494 5294 6805 288a  U5|.NNK.t.R.h.(.
-000013b0: 0800 b074 2a65 5b7e 174e 4e4b 0a74 9452  ...t*e[~.NNK.t.R
-000013c0: 9468 0528 8a08 00b0 9d23 7581 8017 4e4e  .h.(.....#u...NN
-000013d0: 4b0a 7494 5294 6805 288a 0800 b0c6 1c85  K.t.R.h.(.......
-000013e0: a782 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-000013f0: 00b0 ef15 95cd 8417 4e4e 4b0a 7494 5294  ........NNK.t.R.
-00001400: 6805 288a 0800 b018 0fa5 f386 174e 4e4b  h.(..........NNK
-00001410: 0a74 9452 9468 0528 8a08 00b0 4108 b519  .t.R.h.(....A...
-00001420: 8917 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00001430: b06a 01c5 3f8b 174e 4e4b 0a74 9452 9468  .j..?..NNK.t.R.h
-00001440: 0528 8a08 00b0 93fa d465 8d17 4e4e 4b0a  .(.......e..NNK.
-00001450: 7494 5294 6805 288a 0800 b0bc f3e4 8b8f  t.R.h.(.........
+00000f30: c31d d780 e116 4e4e 4b0a 7494 5294 6805  ......NNK.t.R.h.
+00000f40: 288a 0800 b06f 8198 c571 164e 4e4b 0a74  (....o...q.NNK.t
+00000f50: 9452 9468 0528 8a08 00b0 92a5 45ae 5717  .R.h.(......E.W.
+00000f60: 4e4e 4b0a 7494 5294 6805 288a 0800 b0f0  NNK.t.R.h.(.....
+00000f70: 412b 7594 154e 4e4b 0a74 9452 9468 0528  A+u..NNK.t.R.h.(
+00000f80: 8a08 00b0 e342 d642 2617 4e4e 4b0a 7494  .....B.B&.NNK.t.
+00000f90: 5294 6805 288a 0800 b03b 0a59 cc46 164e  R.h.(....;.Y.F.N
+00000fa0: 4e4b 0a74 9452 9468 0528 8a08 00b0 f63f  NK.t.R.h.(.....?
+00000fb0: 87c2 d616 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
+00000fc0: 0800 b0d8 c4a6 6ffd 164e 4e4b 0a74 9452  ......o..NNK.t.R
+00000fd0: 9468 0528 8a08 00b0 8dfc 7818 4b16 4e4e  .h.(......x.K.NN
+00000fe0: 4b0a 7494 5294 6805 288a 0800 b078 55a9  K.t.R.h.(....xU.
+00000ff0: 292f 164e 4e4b 0a74 9452 9468 0528 8a08  )/.NNK.t.R.h.(..
+00001000: 00b0 ddcf 50dc 6c17 4e4e 4b0a 7494 5294  ....P.l.NNK.t.R.
+00001010: 6805 288a 0800 b0ee c005 164f 174e 4e4b  h.(........O.NNK
+00001020: 0a74 9452 9468 0528 8a08 00b0 e5ec f4b1  .t.R.h.(........
+00001030: 9117 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00001040: b0e6 188b 59a1 154e 4e4b 0a74 9452 9468  ....Y..NNK.t.R.h
+00001050: 0528 8a08 00b0 de99 09ad 1916 4e4e 4b0a  .(..........NNK.
+00001060: 7494 5294 6805 288a 0800 b01f 3997 e8d8  t.R.h.(.....9...
+00001070: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00001080: c61c 85a7 8217 4e4e 4b0a 7494 5294 6805  ......NNK.t.R.h.
+00001090: 288a 0800 b0aa 22ca b3ee 154e 4e4b 0a74  (....."....NNK.t
+000010a0: 9452 9468 0528 8a08 00b0 dcef ea3d ae15  .R.h.(.......=..
+000010b0: 4e4e 4b0a 7494 5294 6805 288a 0800 b00f  NNK.t.R.h.(.....
+000010c0: 3b94 8fc9 174e 4e4b 0a74 9452 9468 0528  ;....NNK.t.R.h.(
+000010d0: 8a08 00b0 1c3a e9c1 3716 4e4e 4b0a 7494  .....:..7.NNK.t.
+000010e0: 5294 6805 288a 0800 b030 8c29 f91d 164e  R.h.(....0.)...N
+000010f0: 4e4b 0a74 9452 9468 0528 8a08 00b0 6104  NK.t.R.h.(....a.
+00001100: bbcb a715 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
+00001110: 0800 b019 3b3b 9b96 154e 4e4b 0a74 9452  ....;;...NNK.t.R
+00001120: 9468 0528 8a08 00b0 8428 68b4 8d16 4e4e  .h.(.....(h...NN
+00001130: 4b0a 7494 5294 6805 288a 0800 b0e4 9765  K.t.R.h.(......e
+00001140: fa5b 174e 4e4b 0a74 9452 9468 0528 8a08  .[.NNK.t.R.h.(..
+00001150: 00b0 b3f6 da17 ac15 4e4e 4b0a 7494 5294  ........NNK.t.R.
+00001160: 6805 288a 0800 b0fb bf5a 48bd 154e 4e4b  h.(......ZH..NNK
+00001170: 0a74 9452 9468 0528 8a08 00b0 887c a592  .t.R.h.(.....|..
+00001180: 6417 4e4e 4b0a 7494 5294 6805 288a 0800  d.NNK.t.R.h.(...
+00001190: b005 e9fa 63b0 154e 4e4b 0a74 9452 9468  ....c..NNK.t.R.h
+000011a0: 0528 8a08 00b0 e76d 1a11 d715 4e4e 4b0a  .(.....m....NNK.
+000011b0: 7494 5294 6805 288a 0800 b0af 566d 3084  t.R.h.(.....Vm0.
+000011c0: 184e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+000011d0: 9b79 5612 1517 4e4e 4b0a 7494 5294 6805  .yV...NNK.t.R.h.
+000011e0: 288a 0800 b05d d976 fdf6 164e 4e4b 0a74  (....].v...NNK.t
+000011f0: 9452 9468 0528 8a08 00b0 5106 b872 9816  .R.h.(....Q..r..
+00001200: 4e4e 4b0a 7494 5294 6805 288a 0800 b0f3  NNK.t.R.h.(.....
+00001210: 40d9 9b35 164e 4e4b 0a74 9452 9468 0528  @..5.NNK.t.R.h.(
+00001220: 8a08 00b0 9a24 c75a df16 4e4e 4b0a 7494  .....$.Z..NNK.t.
+00001230: 5294 6805 288a 0800 b0bb 9e55 d459 174e  R.h.(......U.Y.N
+00001240: 4e4b 0a74 9452 9468 0528 8a08 00b0 d499  NK.t.R.h.(......
+00001250: 62a1 4c18 4e4e 4b0a 7494 5294 6805 288a  b.L.NNK.t.R.h.(.
+00001260: 0800 b09e 4f0b 2990 154e 4e4b 0a74 9452  ....O.)..NNK.t.R
+00001270: 9468 0528 8a08 00b0 9426 6b0d 9d15 4e4e  .h.(.....&k...NN
+00001280: 4b0a 7494 5294 6805 288a 0800 b074 2a65  K.t.R.h.(....t*e
+00001290: 5b7e 174e 4e4b 0a74 9452 9468 0528 8a08  [~.NNK.t.R.h.(..
+000012a0: 00b0 56af 8408 a517 4e4e 4b0a 7494 5294  ..V.....NNK.t.R.
+000012b0: 6805 288a 0800 b0ef 1595 cd84 174e 4e4b  h.(..........NNK
+000012c0: 0a74 9452 9468 0528 8a08 00b0 31e1 b8b0  .t.R.h.(....1...
+000012d0: 5316 4e4e 4b0a 7494 5294 6805 288a 0800  S.NNK.t.R.h.(...
+000012e0: b08a fdca f1a9 154e 4e4b 0a74 9452 9468  .......NNK.t.R.h
+000012f0: 0528 8a08 00b0 5f83 956c 6217 4e4e 4b0a  .(...._..lb.NNK.
+00001300: 7494 5294 6805 288a 0800 b0e2 ed46 8bf0  t.R.h.(......F..
+00001310: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00001320: 70d6 277d a716 4e4e 4b0a 7494 5294 6805  p.'}..NNK.t.R.h.
+00001330: 288a 0800 b010 672a 37d9 154e 4e4b 0a74  (.....g*7..NNK.t
+00001340: 9452 9468 0528 8a08 00b0 987a a8eb 7316  .R.h.(.....z..s.
+00001350: 4e4e 4b0a 7494 5294 6805 288a 0800 b0d6  NNK.t.R.h.(.....
+00001360: 1a88 0092 164e 4e4b 0a74 9452 9468 0528  .....NNK.t.R.h.(
+00001370: 8a08 00b0 857d f76b c316 4e4e 4b0a 7494  .....}.k..NNK.t.
+00001380: 5294 6805 288a 0800 b082 7e49 4522 164e  R.h.(.....~IE".N
+00001390: 4e4b 0a74 9452 9468 0528 8a08 00b0 8fa6  NK.t.R.h.(......
+000013a0: 9787 b616 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
+000013b0: 0800 b0fe be08 6f5e 164e 4e4b 0a74 9452  ......o^.NNK.t.R
+000013c0: 9468 0528 8a08 00b0 c5c7 f5ef 4c17 4e4e  .h.(........L.NN
+000013d0: 4b0a 7494 5294 6805 288a 0800 b079 aa38  K.t.R.h.(....y.8
+000013e0: e164 164e 4e4b 0a74 9452 9468 0528 8a08  .d.NNK.t.R.h.(..
+000013f0: 00b0 3535 f68e 2a17 4e4e 4b0a 7494 5294  ..55..*.NNK.t.R.
+00001400: 6805 288a 0800 b0c8 9daa 06c8 154e 4e4b  h.(..........NNK
+00001410: 0a74 9452 9468 0528 8a08 00b0 34e0 66d7  .t.R.h.(....4.f.
+00001420: f416 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00001430: b001 beb6 95ff 164e 4e4b 0a74 9452 9468  .......NNK.t.R.h
+00001440: 0528 8a08 00b0 fc14 eaff f215 4e4e 4b0a  .(..........NNK.
+00001450: 7494 5294 6805 288a 0800 b061 2db4 dbcd  t.R.h.(....a-...
 00001460: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00001470: e5ec f4b1 9117 4e4e 4b0a 7494 5294 6805  ......NNK.t.R.h.
-00001480: 288a 0800 b00e e604 d893 174e 4e4b 0a74  (..........NNK.t
-00001490: 9452 9468 0528 8a08 00b0 37df 14fe 9517  .R.h.(....7.....
-000014a0: 4e4e 4b0a 7494 5294 6805 288a 0800 b060  NNK.t.R.h.(....`
-000014b0: d824 2498 174e 4e4b 0a74 9452 9468 0528  .$$..NNK.t.R.h.(
-000014c0: 8a08 00b0 89d1 344a 9a17 4e4e 4b0a 7494  ......4J..NNK.t.
-000014d0: 5294 6805 288a 0800 b0b2 ca44 709c 174e  R.h.(......Dp..N
-000014e0: 4e4b 0a74 9452 9468 0528 8a08 00b0 dbc3  NK.t.R.h.(......
-000014f0: 5496 9e17 4e4e 4b0a 7494 5294 6805 288a  T...NNK.t.R.h.(.
-00001500: 0800 b004 bd64 bca0 174e 4e4b 0a74 9452  .....d...NNK.t.R
-00001510: 9468 0528 8a08 00b0 2db6 74e2 a217 4e4e  .h.(....-.t...NN
-00001520: 4b0a 7494 5294 6805 288a 0800 b056 af84  K.t.R.h.(....V..
-00001530: 08a5 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00001540: 00b0 7fa8 942e a717 4e4e 4b0a 7494 5294  ........NNK.t.R.
-00001550: 6805 288a 0800 b0a8 a1a4 54a9 174e 4e4b  h.(.......T..NNK
-00001560: 0a74 9452 9468 0528 8a08 00b0 d19a b47a  .t.R.h.(.......z
-00001570: ab17 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00001580: b0fa 93c4 a0ad 174e 4e4b 0a74 9452 9468  .......NNK.t.R.h
-00001590: 0528 8a08 00b0 238d d4c6 af17 4e4e 4b0a  .(....#.....NNK.
-000015a0: 7494 5294 6805 288a 0800 b04c 86e4 ecb1  t.R.h.(....L....
-000015b0: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-000015c0: 757f f412 b417 4e4e 4b0a 7494 5294 6805  u.....NNK.t.R.h.
-000015d0: 288a 0800 b09e 7804 39b6 174e 4e4b 0a74  (.....x.9..NNK.t
-000015e0: 9452 9468 0528 8a08 00b0 c771 145f b817  .R.h.(.....q._..
-000015f0: 4e4e 4b0a 7494 5294 6805 288a 0800 b0f0  NNK.t.R.h.(.....
-00001600: 6a24 85ba 174e 4e4b 0a74 9452 9468 0528  j$...NNK.t.R.h.(
-00001610: 8a08 00b0 1964 34ab bc17 4e4e 4b0a 7494  .....d4...NNK.t.
-00001620: 5294 6805 288a 0800 b042 5d44 d1be 174e  R.h.(....B]D...N
-00001630: 4e4b 0a74 9452 9468 0528 8a08 00b0 6b56  NK.t.R.h.(....kV
-00001640: 54f7 c017 4e4e 4b0a 7494 5294 6805 288a  T...NNK.t.R.h.(.
-00001650: 0800 b094 4f64 1dc3 174e 4e4b 0a74 9452  ....Od...NNK.t.R
-00001660: 9468 0528 8a08 00b0 6eb7 dff4 c417 4e4e  .h.(....n.....NN
-00001670: 4b0a 7494 5294 6805 288a 0800 b0e6 4184  K.t.R.h.(.....A.
-00001680: 69c7 174e 4e4b 0a74 9452 9468 0528 8a08  i..NNK.t.R.h.(..
-00001690: 00b0 0f3b 948f c917 4e4e 4b0a 7494 5294  ...;....NNK.t.R.
-000016a0: 6805 288a 0800 b038 34a4 b5cb 174e 4e4b  h.(....84....NNK
-000016b0: 0a74 9452 9468 0528 8a08 00b0 612d b4db  .t.R.h.(....a-..
-000016c0: cd17 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-000016d0: b08a 26c4 01d0 174e 4e4b 0a74 9452 9468  ..&....NNK.t.R.h
-000016e0: 0528 8a08 00b0 b31f d427 d217 4e4e 4b0a  .(.......'..NNK.
-000016f0: 7494 5294 6805 288a 0800 b0dc 18e4 4dd4  t.R.h.(.......M.
-00001700: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00001710: 80fd 23e6 dc17 4e4e 4b0a 7494 5294 6805  ..#...NNK.t.R.h.
-00001720: 288a 0800 b095 a4f3 d4f8 174e 4e4b 0a74  (..........NNK.t
-00001730: 9452 9468 0528 8a08 00b0 aa4b c3c3 1418  .R.h.(.....K....
-00001740: 4e4e 4b0a 7494 5294 6805 288a 0800 b0d4  NNK.t.R.h.(.....
-00001750: 9962 a14c 184e 4e4b 0a74 9452 9468 0528  .b.L.NNK.t.R.h.(
-00001760: 8a08 00b0 af56 6d30 8418 4e4e 4b0a 7494  .....Vm0..NNK.t.
-00001770: 5294 6805 288a 0800 b028 36a1 5cbc 184e  R.h.(....(6.\..N
-00001780: 4e4b 0a74 9452 9468 0528 8a08 00b0 7b7d  NK.t.R.h.(....{}
-00001790: 5060 f618 4e4e 4b0a 7494 5294 6805 288a  P`..NNK.t.R.h.(.
-000017a0: 0800 b07c d2df 172c 194e 4e4b 0a74 9452  ...|...,.NNK.t.R
-000017b0: 9468 0528 8a08 00b0 cf19 8f1b 6619 4e4e  .h.(........f.NN
-000017c0: 4b0a 7494 5294 6805 288a 0800 b023 b6cd  K.t.R.h.(....#..
-000017d0: d6d5 194e 4e4b 0a74 9452 9465 8c09 4241  ...NNK.t.R.e..BA
-000017e0: 4e4b 4e49 4654 5994 5d94 2868 0528 8a08  NKNIFTY.].(h.(..
-000017f0: 00b0 7f7f 9b1e 8115 4e4e 4b0a 7494 5294  ........NNK.t.R.
-00001800: 6805 288a 0800 b0a8 78ab 4483 154e 4e4b  h.(.....x.D..NNK
-00001810: 0a74 9452 9468 0528 8a08 00b0 d171 bb6a  .t.R.h.(.....q.j
-00001820: 8515 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00001830: b0fa 6acb 9087 154e 4e4b 0a74 9452 9468  ..j....NNK.t.R.h
-00001840: 0528 8a08 00b0 2364 dbb6 8915 4e4e 4b0a  .(....#d....NNK.
-00001850: 7494 5294 6805 288a 0800 b04c 5deb dc8b  t.R.h.(....L]...
+00001470: 1964 34ab bc17 4e4e 4b0a 7494 5294 6805  .d4...NNK.t.R.h.
+00001480: 288a 0800 b026 c566 b48d 154e 4e4b 0a74  (....&.f...NNK.t
+00001490: 9452 9468 0528 8a08 00b0 aa4b c3c3 1418  .R.h.(.....K....
+000014a0: 4e4e 4b0a 7494 5294 6805 288a 0800 b03c  NNK.t.R.h.(....<
+000014b0: 5fe8 837c 164e 4e4b 0a74 9452 9468 0528  _..|.NNK.t.R.h.(
+000014c0: 8a08 00b0 90fb 263f ec16 4e4e 4b0a 7494  ......&?..NNK.t.
+000014d0: 5294 6805 288a 0800 b023 64db b689 154e  R.h.(....#d....N
+000014e0: 4e4b 0a74 9452 9468 0528 8a08 00b0 7b7d  NK.t.R.h.(....{}
+000014f0: 5060 f618 4e4e 4b0a 7494 5294 6805 288a  P`..NNK.t.R.h.(.
+00001500: 0800 b0fa 93c4 a0ad 174e 4e4b 0a74 9452  .........NNK.t.R
+00001510: 9468 0528 8a08 00b0 86d2 8623 f916 4e4e  .h.(.......#..NN
+00001520: 4b0a 7494 5294 6805 288a 0800 b0c0 1e29  K.t.R.h.(......)
+00001530: 5a40 164e 4e4b 0a74 9452 9468 0528 8a08  Z@.NNK.t.R.h.(..
+00001540: 00b0 757f f412 b417 4e4e 4b0a 7494 5294  ..u.....NNK.t.R.
+00001550: 6805 288a 0800 b0bf f292 b230 184e 4e4b  h.(........0.NNK
+00001560: 0a74 9452 9468 0528 8a08 00b0 f06a 2485  .t.R.h.(.....j$.
+00001570: ba17 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00001580: b03a b5c9 1411 164e 4e4b 0a74 9452 9468  .:.....NNK.t.R.h
+00001590: 0528 8a08 00b0 d919 3627 3317 4e4e 4b0a  .(......6'3.NNK.
+000015a0: 7494 5294 6805 288a 0800 b0be 740a ebd4  t.R.h.(.....t...
+000015b0: 154e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+000015c0: ccf1 e7e4 9e16 4e4e 4b0a 7494 5294 6805  ......NNK.t.R.h.
+000015d0: 288a 0800 b03f 5e96 aa1d 174e 4e4b 0a74  (....?^....NNK.t
+000015e0: 9452 9468 0528 8a08 00b0 0c3c e668 2817  .R.h.(.....<.h(.
+000015f0: 4e4e 4b0a 7494 5294 6805 288a 0800 b041  NNK.t.R.h.(....A
+00001600: 08b5 1989 174e 4e4b 0a74 9452 9468 0528  .....NNK.t.R.h.(
+00001610: 8a08 00b0 04bd 64bc a017 4e4e 4b0a 7494  ......d...NNK.t.
+00001620: 5294 6805 288a 0800 b0e6 4184 69c7 174e  R.h.(.....A.i..N
+00001630: 4e4b 0a74 9452 9468 0528 8a08 00b0 cf19  NK.t.R.h.(......
+00001640: 8f1b 6619 4e4e 4b0a 7494 5294 6805 288a  ..f.NNK.t.R.h.(.
+00001650: 0800 b012 1149 a644 164e 4e4b 0a74 9452  .....I.D.NNK.t.R
+00001660: 9468 0528 8a08 00b0 b6f5 883e 4d16 4e4e  .h.(.......>M.NN
+00001670: 4b0a 7494 5294 6805 288a 0800 b099 cf37  K.t.R.h.(......7
+00001680: a3a9 164e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+00001690: 00b0 7b54 5750 d016 4e4e 4b0a 7494 5294  ..{TWP..NNK.t.R.
+000016a0: 6805 288a 0800 b0f7 9416 7a0c 174e 4e4b  h.(.......z..NNK
+000016b0: 0a74 9452 9468 0528 8a08 00b0 171c f312  .t.R.h.(........
+000016c0: b416 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+000016d0: b0b1 75b5 b866 174e 4e4b 0a74 9452 9468  ..u..f.NNK.t.R.h
+000016e0: 0528 8a08 00b0 dbc3 5496 9e17 4e4e 4b0a  .(......T...NNK.
+000016f0: 7494 5294 6805 288a 0800 b0b5 a0f9 8617  t.R.h.(.........
+00001700: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00001710: 2ab7 c6bb 0117 4e4e 4b0a 7494 5294 6805  *.....NNK.t.R.h.
+00001720: 288a 0800 b068 57a6 d01f 174e 4e4b 0a74  (....hW....NNK.t
+00001730: 9452 9468 0528 8a08 00b0 0d91 7520 5e17  .R.h.(......u ^.
+00001740: 4e4e 4b0a 7494 5294 6805 288a 0800 b07e  NNK.t.R.h.(....~
+00001750: 5305 7771 174e 4e4b 0a74 9452 9468 0528  S.wq.NNK.t.R.h.(
+00001760: 8a08 00b0 380b aba5 a515 4e4e 4b0a 7494  ....8.....NNK.t.
+00001770: 5294 6805 288a 0800 b022 3845 0f7a 174e  R.h.(...."8E.z.N
+00001780: 4e4b 0a74 9452 9468 0528 8a08 00b0 0213  NK.t.R.h.(......
+00001790: 464d 3517 4e4e 4b0a 7494 5294 6805 288a  FM5.NNK.t.R.h.(.
+000017a0: 0800 b057 66f1 963d 174e 4e4b 0a74 9452  ...Wf..=.NNK.t.R
+000017b0: 9468 0528 8a08 00b0 a74c 159d 7317 4e4e  .h.(.....L..s.NN
+000017c0: 4b0a 7494 5294 6805 288a 0800 b0ff 1398  K.t.R.h.(.......
+000017d0: 2694 164e 4e4b 0a74 9452 9468 0528 8a08  &..NNK.t.R.h.(..
+000017e0: 00b0 4389 da78 ce15 4e4e 4b0a 7494 5294  ..C..x..NNK.t.R.
+000017f0: 6805 288a 0800 b0d7 6f17 b8c7 164e 4e4b  h.(.....o....NNK
+00001800: 0a74 9452 9468 0528 8a08 00b0 3236 4868  .t.R.h.(....26Hh
+00001810: 8916 4e4e 4b0a 7494 5294 658c 0942 414e  ..NNK.t.R.e..BAN
+00001820: 4b4e 4946 5459 945d 9428 6805 288a 0800  KNIFTY.].(h.(...
+00001830: b0d4 7069 9126 164e 4e4b 0a74 9452 9468  ..pi.&.NNK.t.R.h
+00001840: 0528 8a08 00b0 ec16 e7a6 e316 4e4e 4b0a  .(..........NNK.
+00001850: 7494 5294 6805 288a 0800 b024 b96a 6ebf  t.R.h.(....$.jn.
 00001860: 154e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00001870: 26c5 66b4 8d15 4e4e 4b0a 7494 5294 6805  &.f...NNK.t.R.h.
-00001880: 288a 0800 b09e 4f0b 2990 154e 4e4b 0a74  (.....O.)..NNK.t
-00001890: 9452 9468 0528 8a08 00b0 c748 1b4f 9215  .R.h.(.....H.O..
-000018a0: 4e4e 4b0a 7494 5294 6805 288a 0800 b0f0  NNK.t.R.h.(.....
-000018b0: 412b 7594 154e 4e4b 0a74 9452 9468 0528  A+u..NNK.t.R.h.(
-000018c0: 8a08 00b0 193b 3b9b 9615 4e4e 4b0a 7494  .....;;...NNK.t.
-000018d0: 5294 6805 288a 0800 b042 344b c198 154e  R.h.(....B4K...N
-000018e0: 4e4b 0a74 9452 9468 0528 8a08 00b0 6b2d  NK.t.R.h.(....k-
-000018f0: 5be7 9a15 4e4e 4b0a 7494 5294 6805 288a  [...NNK.t.R.h.(.
-00001900: 0800 b094 266b 0d9d 154e 4e4b 0a74 9452  ....&k...NNK.t.R
-00001910: 9468 0528 8a08 00b0 bd1f 7b33 9f15 4e4e  .h.(......{3..NN
-00001920: 4b0a 7494 5294 6805 288a 0800 b0e6 188b  K.t.R.h.(.......
-00001930: 59a1 154e 4e4b 0a74 9452 9468 0528 8a08  Y..NNK.t.R.h.(..
-00001940: 00b0 0f12 9b7f a315 4e4e 4b0a 7494 5294  ........NNK.t.R.
-00001950: 6805 288a 0800 b038 0bab a5a5 154e 4e4b  h.(....8.....NNK
-00001960: 0a74 9452 9468 0528 8a08 00b0 6104 bbcb  .t.R.h.(....a...
-00001970: a715 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00001980: b08a fdca f1a9 154e 4e4b 0a74 9452 9468  .......NNK.t.R.h
-00001990: 0528 8a08 00b0 b3f6 da17 ac15 4e4e 4b0a  .(..........NNK.
-000019a0: 7494 5294 6805 288a 0800 b0dc efea 3dae  t.R.h.(.......=.
-000019b0: 154e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-000019c0: 05e9 fa63 b015 4e4e 4b0a 7494 5294 6805  ...c..NNK.t.R.h.
-000019d0: 288a 0800 b02e e20a 8ab2 154e 4e4b 0a74  (..........NNK.t
-000019e0: 9452 9468 0528 8a08 00b0 57db 1ab0 b415  .R.h.(....W.....
-000019f0: 4e4e 4b0a 7494 5294 6805 288a 0800 b080  NNK.t.R.h.(.....
-00001a00: d42a d6b6 154e 4e4b 0a74 9452 9468 0528  .*...NNK.t.R.h.(
-00001a10: 8a08 00b0 a9cd 3afc b815 4e4e 4b0a 7494  ......:...NNK.t.
-00001a20: 5294 6805 288a 0800 b083 35b6 d3ba 154e  R.h.(.....5....N
-00001a30: 4e4b 0a74 9452 9468 0528 8a08 00b0 fbbf  NK.t.R.h.(......
-00001a40: 5a48 bd15 4e4e 4b0a 7494 5294 6805 288a  ZH..NNK.t.R.h.(.
-00001a50: 0800 b024 b96a 6ebf 154e 4e4b 0a74 9452  ...$.jn..NNK.t.R
-00001a60: 9468 0528 8a08 00b0 4db2 7a94 c115 4e4e  .h.(....M.z...NN
-00001a70: 4b0a 7494 5294 6805 288a 0800 b076 ab8a  K.t.R.h.(....v..
-00001a80: bac3 154e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00001a90: 00b0 9fa4 9ae0 c515 4e4e 4b0a 7494 5294  ........NNK.t.R.
-00001aa0: 6805 288a 0800 b0c8 9daa 06c8 154e 4e4b  h.(..........NNK
-00001ab0: 0a74 9452 9468 0528 8a08 00b0 f196 ba2c  .t.R.h.(.......,
-00001ac0: ca15 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00001ad0: b01a 90ca 52cc 154e 4e4b 0a74 9452 9468  ....R..NNK.t.R.h
-00001ae0: 0528 8a08 00b0 4389 da78 ce15 4e4e 4b0a  .(....C..x..NNK.
-00001af0: 7494 5294 6805 288a 0800 b06c 82ea 9ed0  t.R.h.(....l....
+00001870: 6e2c 090e 3c16 4e4e 4b0a 7494 5294 6805  n,..<.NNK.t.R.h.
+00001880: 288a 0800 b0f1 96ba 2cca 154e 4e4b 0a74  (.......,..NNK.t
+00001890: 9452 9468 0528 8a08 00b0 cff0 950b 4017  .R.h.(........@.
+000018a0: 4e4e 4b0a 7494 5294 6805 288a 0800 b0f5  NNK.t.R.h.(.....
+000018b0: eaf7 0aa1 164e 4e4b 0a74 9452 9468 0528  .....NNK.t.R.h.(
+000018c0: 8a08 00b0 c97d 10a5 8617 4e4e 4b0a 7494  .....}....NNK.t.
+000018d0: 5294 6805 288a 0800 b0b7 4a18 f682 164e  R.h.(.....J....N
+000018e0: 4e4b 0a74 9452 9468 0528 8a08 00b0 53b0  NK.t.R.h.(....S.
+000018f0: d6e1 0317 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
+00001900: 0800 b095 7bfa c4d2 154e 4e4b 0a74 9452  ....{....NNK.t.R
+00001910: 9468 0528 8a08 00b0 80d4 2ad6 b615 4e4e  .h.(......*...NN
+00001920: 4b0a 7494 5294 6805 288a 0800 b06c 82ea  K.t.R.h.(....l..
+00001930: 9ed0 154e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+00001940: 00b0 dd44 7af5 e315 4e4e 4b0a 7494 5294  ...Dz...NNK.t.R.
+00001950: 6805 288a 0800 b011 bcb9 ee0e 164e 4e4b  h.(..........NNK
+00001960: 0a74 9452 9468 0528 8a08 00b0 a44d 6776  .t.R.h.(.....Mgv
+00001970: d216 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00001980: b07c a9e6 0706 174e 4e4b 0a74 9452 9468  .|.....NNK.t.R.h
+00001990: 0528 8a08 00b0 a878 ab44 8315 4e4e 4b0a  .(.....x.D..NNK.
+000019a0: 7494 5294 6805 288a 0800 b020 8e26 a00e  t.R.h.(.... .&..
+000019b0: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+000019c0: a0f9 2998 fb15 4e4e 4b0a 7494 5294 6805  ..)...NNK.t.R.h.
+000019d0: 288a 0800 b0c4 7266 3817 174e 4e4b 0a74  (.....rf8..NNK.t
+000019e0: 9452 9468 0528 8a08 00b0 14bb 6715 b016  .R.h.(......g...
+000019f0: 4e4e 4b0a 7494 5294 6805 288a 0800 b044  NNK.t.R.h.(....D
+00001a00: de69 3004 164e 4e4b 0a74 9452 9468 0528  .i0..NNK.t.R.h.(
+00001a10: 8a08 00b0 8e51 08d0 8016 4e4e 4b0a 7494  .....Q....NNK.t.
+00001a20: 5294 6805 288a 0800 b025 0efa 25f5 154e  R.h.(....%..%..N
+00001a30: 4e4b 0a74 9452 9468 0528 8a08 00b0 c748  NK.t.R.h.(.....H
+00001a40: 1b4f 9215 4e4e 4b0a 7494 5294 6805 288a  .O..NNK.t.R.h.(.
+00001a50: 0800 b0cd 4677 9cd4 164e 4e4b 0a74 9452  ....Fw...NNK.t.R
+00001a60: 9468 0528 8a08 00b0 1366 d85d 7a16 4e4e  .h.(.....f.]z.NN
+00001a70: 4b0a 7494 5294 6805 288a 0800 b046 8888  K.t.R.h.(....F..
+00001a80: 9f6f 164e 4e4b 0a74 9452 9468 0528 8a08  .o.NNK.t.R.h.(..
+00001a90: 00b0 b89f a7ad b816 4e4e 4b0a 7494 5294  ........NNK.t.R.
+00001aa0: 6805 288a 0800 b0af cb96 49fb 164e 4e4b  h.(.......I..NNK
+00001ab0: 0a74 9452 9468 0528 8a08 00b0 4f5c 9903  .t.R.h.(....O\..
+00001ac0: 2d16 4e4e 4b0a 7494 5294 6805 288a 0800  -.NNK.t.R.h.(...
+00001ad0: b0a1 d98f 36ba 174e 4e4b 0a74 9452 9468  ....6..NNK.t.R.h
+00001ae0: 0528 8a08 00b0 7dfe 75bf 3b17 4e4e 4b0a  .(....}.u.;.NNK.
+00001af0: 7494 5294 6805 288a 0800 b06b 2d5b e79a  t.R.h.(....k-[..
 00001b00: 154e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00001b10: 957b fac4 d215 4e4e 4b0a 7494 5294 6805  .{....NNK.t.R.h.
-00001b20: 288a 0800 b0be 740a ebd4 154e 4e4b 0a74  (.....t....NNK.t
-00001b30: 9452 9468 0528 8a08 00b0 e76d 1a11 d715  .R.h.(.....m....
-00001b40: 4e4e 4b0a 7494 5294 6805 288a 0800 b010  NNK.t.R.h.(.....
-00001b50: 672a 37d9 154e 4e4b 0a74 9452 9468 0528  g*7..NNK.t.R.h.(
-00001b60: 8a08 00b0 3960 3a5d db15 4e4e 4b0a 7494  ....9`:]..NNK.t.
-00001b70: 5294 6805 288a 0800 b062 594a 83dd 154e  R.h.(....bYJ...N
-00001b80: 4e4b 0a74 9452 9468 0528 8a08 00b0 8b52  NK.t.R.h.(.....R
-00001b90: 5aa9 df15 4e4e 4b0a 7494 5294 6805 288a  Z...NNK.t.R.h.(.
-00001ba0: 0800 b0b4 4b6a cfe1 154e 4e4b 0a74 9452  ....Kj...NNK.t.R
-00001bb0: 9468 0528 8a08 00b0 dd44 7af5 e315 4e4e  .h.(.....Dz...NN
-00001bc0: 4b0a 7494 5294 6805 288a 0800 b006 3e8a  K.t.R.h.(.....>.
-00001bd0: 1be6 154e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00001be0: 00b0 2f37 9a41 e815 4e4e 4b0a 7494 5294  ../7.A..NNK.t.R.
-00001bf0: 6805 288a 0800 b058 30aa 67ea 154e 4e4b  h.(....X0.g..NNK
-00001c00: 0a74 9452 9468 0528 8a08 00b0 8129 ba8d  .t.R.h.(.....)..
-00001c10: ec15 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00001c20: b0aa 22ca b3ee 154e 4e4b 0a74 9452 9468  .."....NNK.t.R.h
-00001c30: 0528 8a08 00b0 d31b dad9 f015 4e4e 4b0a  .(..........NNK.
-00001c40: 7494 5294 6805 288a 0800 b0fc 14ea fff2  t.R.h.(.........
-00001c50: 154e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00001c60: 250e fa25 f515 4e4e 4b0a 7494 5294 6805  %..%..NNK.t.R.h.
-00001c70: 288a 0800 b04e 070a 4cf7 154e 4e4b 0a74  (....N..L..NNK.t
-00001c80: 9452 9468 0528 8a08 00b0 7700 1a72 f915  .R.h.(....w..r..
-00001c90: 4e4e 4b0a 7494 5294 6805 288a 0800 b0a0  NNK.t.R.h.(.....
-00001ca0: f929 98fb 154e 4e4b 0a74 9452 9468 0528  .)...NNK.t.R.h.(
-00001cb0: 8a08 00b0 c9f2 39be fd15 4e4e 4b0a 7494  ......9...NNK.t.
-00001cc0: 5294 6805 288a 0800 b0f2 eb49 e4ff 154e  R.h.(......I...N
-00001cd0: 4e4b 0a74 9452 9468 0528 8a08 00b0 cc53  NK.t.R.h.(.....S
-00001ce0: c5bb 0116 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
-00001cf0: 0800 b044 de69 3004 164e 4e4b 0a74 9452  ...D.i0..NNK.t.R
-00001d00: 9468 0528 8a08 00b0 6dd7 7956 0616 4e4e  .h.(....m.yV..NN
-00001d10: 4b0a 7494 5294 6805 288a 0800 b096 d089  K.t.R.h.(.......
-00001d20: 7c08 164e 4e4b 0a74 9452 9468 0528 8a08  |..NNK.t.R.h.(..
-00001d30: 00b0 bfc9 99a2 0a16 4e4e 4b0a 7494 5294  ........NNK.t.R.
-00001d40: 6805 288a 0800 b0e8 c2a9 c80c 164e 4e4b  h.(..........NNK
-00001d50: 0a74 9452 9468 0528 8a08 00b0 11bc b9ee  .t.R.h.(........
-00001d60: 0e16 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00001d70: b03a b5c9 1411 164e 4e4b 0a74 9452 9468  .:.....NNK.t.R.h
-00001d80: 0528 8a08 00b0 63ae d93a 1316 4e4e 4b0a  .(....c..:..NNK.
-00001d90: 7494 5294 6805 288a 0800 b08c a7e9 6015  t.R.h.(.......`.
+00001b10: 063e 8a1b e615 4e4e 4b0a 7494 5294 6805  .>....NNK.t.R.h.
+00001b20: 288a 0800 b0fe 49df 55e7 174e 4e4b 0a74  (.....I.U..NNK.t
+00001b30: 9452 9468 0528 8a08 00b0 5405 6699 3917  .R.h.(....T.f.9.
+00001b40: 4e4e 4b0a 7494 5294 6805 288a 0800 b057  NNK.t.R.h.(....W
+00001b50: db1a b0b4 154e 4e4b 0a74 9452 9468 0528  .....NNK.t.R.h.(
+00001b60: 8a08 00b0 21e3 b557 4417 4e4e 4b0a 7494  ....!..WD.NNK.t.
+00001b70: 5294 6805 288a 0800 b083 35b6 d3ba 154e  R.h.(.....5....N
+00001b80: 4e4b 0a74 9452 9468 0528 8a08 00b0 b020  NK.t.R.h.(..... 
+00001b90: 2601 3117 4e4e 4b0a 7494 5294 6805 288a  &.1.NNK.t.R.h.(.
+00001ba0: 0800 b000 6927 dec9 164e 4e4b 0a74 9452  ....i'...NNK.t.R
+00001bb0: 9468 0528 8a08 00b0 fdf4 4f9e b117 4e4e  .h.(......O...NN
+00001bc0: 4b0a 7494 5294 6805 288a 0800 b0fa 6acb  K.t.R.h.(.....j.
+00001bd0: 9087 154e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+00001be0: 00b0 16c7 635b 7e16 4e4e 4b0a 7494 5294  ....c[~.NNK.t.R.
+00001bf0: 6805 288a 0800 b054 6743 709c 164e 4e4b  h.(....TgCp..NNK
+00001c00: 0a74 9452 9468 0528 8a08 00b0 5985 391f  .t.R.h.(....Y.9.
+00001c10: 2016 4e4e 4b0a 7494 5294 6805 288a 0800   .NNK.t.R.h.(...
+00001c20: b05a dac8 d655 164e 4e4b 0a74 9452 9468  .Z...U.NNK.t.R.h
+00001c30: 0528 8a08 00b0 338b d71f bf16 4e4e 4b0a  .(....3.....NNK.
+00001c40: 7494 5294 6805 288a 0800 b03e 0907 f3e7  t.R.h.(....>....
+00001c50: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00001c60: 7f7f 9b1e 8115 4e4e 4b0a 7494 5294 6805  ......NNK.t.R.h.
+00001c70: 288a 0800 b003 68d5 046b 174e 4e4b 0a74  (.....h..k.NNK.t
+00001c80: 9452 9468 0528 8a08 00b0 c771 145f b817  .R.h.(.....q._..
+00001c90: 4e4e 4b0a 7494 5294 6805 288a 0800 b097  NNK.t.R.h.(.....
+00001ca0: 2519 343e 164e 4e4b 0a74 9452 9468 0528  %.4>.NNK.t.R.h.(
+00001cb0: 8a08 00b0 c828 81ed 5017 4e4e 4b0a 7494  .....(..P.NNK.t.
+00001cc0: 5294 6805 288a 0800 b09d 2375 8180 174e  R.h.(.....#u...N
+00001cd0: 4e4b 0a74 9452 9468 0528 8a08 00b0 f3cb  NK.t.R.h.(......
+00001ce0: af82 be17 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
+00001cf0: 0800 b0b4 4b6a cfe1 154e 4e4b 0a74 9452  ....Kj...NNK.t.R
+00001d00: 9468 0528 8a08 00b0 bf54 7089 9317 4e4e  .h.(.....Tp...NN
+00001d10: 4b0a 7494 5294 6805 288a 0800 b0da 6ec5  K.t.R.h.(.....n.
+00001d20: de68 174e 4e4b 0a74 9452 9468 0528 8a08  .h.NNK.t.R.h.(..
+00001d30: 00b0 e8c2 a9c8 0c16 4e4e 4b0a 7494 5294  ........NNK.t.R.
+00001d40: 6805 288a 0800 b09c cee5 c94a 174e 4e4b  h.(........J.NNK
+00001d50: 0a74 9452 9468 0528 8a08 00b0 1ee4 0731  .t.R.h.(.......1
+00001d60: a316 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00001d70: b067 0217 19ea 164e 4e4b 0a74 9452 9468  .g.....NNK.t.R.h
+00001d80: 0528 8a08 00b0 8b52 5aa9 df15 4e4e 4b0a  .(.....RZ...NNK.
+00001d90: 7494 5294 6805 288a 0800 b0fd 6979 b728  t.R.h.(.....iy.(
 00001da0: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00001db0: b5a0 f986 1716 4e4e 4b0a 7494 5294 6805  ......NNK.t.R.h.
-00001dc0: 288a 0800 b0de 9909 ad19 164e 4e4b 0a74  (..........NNK.t
-00001dd0: 9452 9468 0528 8a08 00b0 0793 19d3 1b16  .R.h.(..........
-00001de0: 4e4e 4b0a 7494 5294 6805 288a 0800 b030  NNK.t.R.h.(....0
-00001df0: 8c29 f91d 164e 4e4b 0a74 9452 9468 0528  .)...NNK.t.R.h.(
-00001e00: 8a08 00b0 5985 391f 2016 4e4e 4b0a 7494  ....Y.9. .NNK.t.
-00001e10: 5294 6805 288a 0800 b082 7e49 4522 164e  R.h.(.....~IE".N
-00001e20: 4e4b 0a74 9452 9468 0528 8a08 00b0 ab77  NK.t.R.h.(.....w
-00001e30: 596b 2416 4e4e 4b0a 7494 5294 6805 288a  Yk$.NNK.t.R.h.(.
-00001e40: 0800 b0d4 7069 9126 164e 4e4b 0a74 9452  ....pi.&.NNK.t.R
-00001e50: 9468 0528 8a08 00b0 fd69 79b7 2816 4e4e  .h.(.....iy.(.NN
-00001e60: 4b0a 7494 5294 6805 288a 0800 b026 6389  K.t.R.h.(....&c.
-00001e70: dd2a 164e 4e4b 0a74 9452 9468 0528 8a08  .*.NNK.t.R.h.(..
-00001e80: 00b0 4f5c 9903 2d16 4e4e 4b0a 7494 5294  ..O\..-.NNK.t.R.
-00001e90: 6805 288a 0800 b078 55a9 292f 164e 4e4b  h.(....xU.)/.NNK
-00001ea0: 0a74 9452 9468 0528 8a08 00b0 a14e b94f  .t.R.h.(.....N.O
-00001eb0: 3116 4e4e 4b0a 7494 5294 6805 288a 0800  1.NNK.t.R.h.(...
-00001ec0: b0ca 47c9 7533 164e 4e4b 0a74 9452 9468  ..G.u3.NNK.t.R.h
-00001ed0: 0528 8a08 00b0 f340 d99b 3516 4e4e 4b0a  .(.....@..5.NNK.
-00001ee0: 7494 5294 6805 288a 0800 b01c 3ae9 c137  t.R.h.(.....:..7
-00001ef0: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00001f00: 4533 f9e7 3916 4e4e 4b0a 7494 5294 6805  E3..9.NNK.t.R.h.
-00001f10: 288a 0800 b06e 2c09 0e3c 164e 4e4b 0a74  (....n,..<.NNK.t
-00001f20: 9452 9468 0528 8a08 00b0 9725 1934 3e16  .R.h.(.....%.4>.
-00001f30: 4e4e 4b0a 7494 5294 6805 288a 0800 b0c0  NNK.t.R.h.(.....
-00001f40: 1e29 5a40 164e 4e4b 0a74 9452 9468 0528  .)Z@.NNK.t.R.h.(
-00001f50: 8a08 00b0 e917 3980 4216 4e4e 4b0a 7494  ......9.B.NNK.t.
-00001f60: 5294 6805 288a 0800 b012 1149 a644 164e  R.h.(......I.D.N
-00001f70: 4e4b 0a74 9452 9468 0528 8a08 00b0 3b0a  NK.t.R.h.(....;.
-00001f80: 59cc 4616 4e4e 4b0a 7494 5294 6805 288a  Y.F.NNK.t.R.h.(.
-00001f90: 0800 b064 0369 f248 164e 4e4b 0a74 9452  ...d.i.H.NNK.t.R
-00001fa0: 9468 0528 8a08 00b0 8dfc 7818 4b16 4e4e  .h.(......x.K.NN
-00001fb0: 4b0a 7494 5294 6805 288a 0800 b0b6 f588  K.t.R.h.(.......
-00001fc0: 3e4d 164e 4e4b 0a74 9452 9468 0528 8a08  >M.NNK.t.R.h.(..
-00001fd0: 00b0 dfee 9864 4f16 4e4e 4b0a 7494 5294  .....dO.NNK.t.R.
-00001fe0: 6805 288a 0800 b008 e8a8 8a51 164e 4e4b  h.(........Q.NNK
-00001ff0: 0a74 9452 9468 0528 8a08 00b0 31e1 b8b0  .t.R.h.(....1...
-00002000: 5316 4e4e 4b0a 7494 5294 6805 288a 0800  S.NNK.t.R.h.(...
-00002010: b05a dac8 d655 164e 4e4b 0a74 9452 9468  .Z...U.NNK.t.R.h
-00002020: 0528 8a08 00b0 83d3 d8fc 5716 4e4e 4b0a  .(........W.NNK.
-00002030: 7494 5294 6805 288a 0800 b0ac cce8 225a  t.R.h.(......."Z
+00001db0: 2663 89dd 2a16 4e4e 4b0a 7494 5294 6805  &c..*.NNK.t.R.h.
+00001dc0: 288a 0800 b096 d089 7c08 164e 4e4b 0a74  (.......|..NNK.t
+00001dd0: 9452 9468 0528 8a08 00b0 f2eb 49e4 ff15  .R.h.(......I...
+00001de0: 4e4e 4b0a 7494 5294 6805 288a 0800 b0ca  NNK.t.R.h.(.....
+00001df0: 47c9 7533 164e 4e4b 0a74 9452 9468 0528  G.u3.NNK.t.R.h.(
+00001e00: 8a08 00b0 cc53 c5bb 0116 4e4e 4b0a 7494  .....S....NNK.t.
+00001e10: 5294 6805 288a 0800 b0e0 4328 1c85 164e  R.h.(.....C(...N
+00001e20: 4e4b 0a74 9452 9468 0528 8a08 00b0 c2c8  NK.t.R.h.(......
+00001e30: 47c9 ab16 4e4e 4b0a 7494 5294 6805 288a  G...NNK.t.R.h.(.
+00001e40: 0800 b03a 40a0 fb99 174e 4e4b 0a74 9452  ...:@....NNK.t.R
+00001e50: 9468 0528 8a08 00b0 de24 e093 a217 4e4e  .h.(.....$....NN
+00001e60: 4b0a 7494 5294 6805 288a 0800 b0ea 6cc8  K.t.R.h.(.....l.
+00001e70: 3778 164e 4e4b 0a74 9452 9468 0528 8a08  7x.NNK.t.R.h.(..
+00001e80: 00b0 08e8 a88a 5116 4e4e 4b0a 7494 5294  ......Q.NNK.t.R.
+00001e90: 6805 288a 0800 b0d1 71bb 6a85 154e 4e4b  h.(.....q.j..NNK
+00001ea0: 0a74 9452 9468 0528 8a08 00b0 8d87 4fff  .t.R.h.(......O.
+00001eb0: d317 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00001ec0: b071 2bb7 34dd 164e 4e4b 0a74 9452 9468  .q+.4..NNK.t.R.h
+00001ed0: 0528 8a08 00b0 1a90 ca52 cc15 4e4e 4b0a  .(.......R..NNK.
+00001ee0: 7494 5294 6805 288a 0800 b06d 6250 3d8f  t.R.h.(....mbP=.
+00001ef0: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00001f00: 4832 a70e db16 4e4e 4b0a 7494 5294 6805  H2....NNK.t.R.h.
+00001f10: 288a 0800 b0e9 1739 8042 164e 4e4b 0a74  (......9.B.NNK.t
+00001f20: 9452 9468 0528 8a08 00b0 1147 90d5 9717  .R.h.(.....G....
+00001f30: 4e4e 4b0a 7494 5294 6805 288a 0800 b0bd  NNK.t.R.h.(.....
+00001f40: 1f7b 339f 154e 4e4b 0a74 9452 9468 0528  .{3..NNK.t.R.h.(
+00001f50: 8a08 00b0 8c32 c047 9e17 4e4e 4b0a 7494  .....2.G..NNK.t.
+00001f60: 5294 6805 288a 0800 b04e 070a 4cf7 154e  R.h.(....N..L..N
+00001f70: 4e4b 0a74 9452 9468 0528 8a08 00b0 6dd7  NK.t.R.h.(....m.
+00001f80: 7956 0616 4e4e 4b0a 7494 5294 6805 288a  yV..NNK.t.R.h.(.
+00001f90: 0800 b0a1 4eb9 4f31 164e 4e4b 0a74 9452  ....N.O1.NNK.t.R
+00001fa0: 9468 0528 8a08 00b0 6403 69f2 4816 4e4e  .h.(....d.i.H.NN
+00001fb0: 4b0a 7494 5294 6805 288a 0800 b0df ee98  K.t.R.h.(.......
+00001fc0: 644f 164e 4e4b 0a74 9452 9468 0528 8a08  dO.NNK.t.R.h.(..
+00001fd0: 00b0 4db2 7a94 c115 4e4e 4b0a 7494 5294  ..M.z...NNK.t.R.
+00001fe0: 6805 288a 0800 b0a2 a348 0767 164e 4e4b  h.(......H.g.NNK
+00001ff0: 0a74 9452 9468 0528 8a08 00b0 f8e9 a531  .t.R.h.(.......1
+00002000: 4217 4e4e 4b0a 7494 5294 6805 288a 0800  B.NNK.t.R.h.(...
+00002010: b00a 92c7 f9bc 164e 4e4b 0a74 9452 9468  .......NNK.t.R.h
+00002020: 0528 8a08 00b0 d5c5 f848 5c16 4e4e 4b0a  .(.......H\.NNK.
+00002030: 7494 5294 6805 288a 0800 b0eb c157 efad  t.R.h.(......W..
 00002040: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00002050: d5c5 f848 5c16 4e4e 4b0a 7494 5294 6805  ...H\.NNK.t.R.h.
-00002060: 288a 0800 b0fe be08 6f5e 164e 4e4b 0a74  (.......o^.NNK.t
-00002070: 9452 9468 0528 8a08 00b0 27b8 1895 6016  .R.h.(....'...`.
-00002080: 4e4e 4b0a 7494 5294 6805 288a 0800 b050  NNK.t.R.h.(....P
-00002090: b128 bb62 164e 4e4b 0a74 9452 9468 0528  .(.b.NNK.t.R.h.(
-000020a0: 8a08 00b0 79aa 38e1 6416 4e4e 4b0a 7494  ....y.8.d.NNK.t.
-000020b0: 5294 6805 288a 0800 b0a2 a348 0767 164e  R.h.(......H.g.N
-000020c0: 4e4b 0a74 9452 9468 0528 8a08 00b0 cb9c  NK.t.R.h.(......
-000020d0: 582d 6916 4e4e 4b0a 7494 5294 6805 288a  X-i.NNK.t.R.h.(.
-000020e0: 0800 b0a5 04d4 046b 164e 4e4b 0a74 9452  .......k.NNK.t.R
-000020f0: 9468 0528 8a08 00b0 1d8f 7879 6d16 4e4e  .h.(......xym.NN
-00002100: 4b0a 7494 5294 6805 288a 0800 b046 8888  K.t.R.h.(....F..
-00002110: 9f6f 164e 4e4b 0a74 9452 9468 0528 8a08  .o.NNK.t.R.h.(..
-00002120: 00b0 6f81 98c5 7116 4e4e 4b0a 7494 5294  ..o...q.NNK.t.R.
-00002130: 6805 288a 0800 b098 7aa8 eb73 164e 4e4b  h.(.....z..s.NNK
-00002140: 0a74 9452 9468 0528 8a08 00b0 c173 b811  .t.R.h.(.....s..
-00002150: 7616 4e4e 4b0a 7494 5294 6805 288a 0800  v.NNK.t.R.h.(...
-00002160: b0ea 6cc8 3778 164e 4e4b 0a74 9452 9468  ..l.7x.NNK.t.R.h
-00002170: 0528 8a08 00b0 1366 d85d 7a16 4e4e 4b0a  .(.....f.]z.NNK.
-00002180: 7494 5294 6805 288a 0800 b03c 5fe8 837c  t.R.h.(....<_..|
-00002190: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-000021a0: 16c7 635b 7e16 4e4e 4b0a 7494 5294 6805  ..c[~.NNK.t.R.h.
-000021b0: 288a 0800 b08e 5108 d080 164e 4e4b 0a74  (.....Q....NNK.t
-000021c0: 9452 9468 0528 8a08 00b0 b74a 18f6 8216  .R.h.(.....J....
-000021d0: 4e4e 4b0a 7494 5294 6805 288a 0800 b0e0  NNK.t.R.h.(.....
-000021e0: 4328 1c85 164e 4e4b 0a74 9452 9468 0528  C(...NNK.t.R.h.(
-000021f0: 8a08 00b0 093d 3842 8716 4e4e 4b0a 7494  .....=8B..NNK.t.
-00002200: 5294 6805 288a 0800 b032 3648 6889 164e  R.h.(....26Hh..N
-00002210: 4e4b 0a74 9452 9468 0528 8a08 00b0 5b2f  NK.t.R.h.(....[/
-00002220: 588e 8b16 4e4e 4b0a 7494 5294 6805 288a  X...NNK.t.R.h.(.
-00002230: 0800 b084 2868 b48d 164e 4e4b 0a74 9452  ....(h...NNK.t.R
-00002240: 9468 0528 8a08 00b0 ad21 78da 8f16 4e4e  .h.(.....!x...NN
-00002250: 4b0a 7494 5294 6805 288a 0800 b0d6 1a88  K.t.R.h.(.......
-00002260: 0092 164e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00002270: 00b0 ff13 9826 9416 4e4e 4b0a 7494 5294  .....&..NNK.t.R.
-00002280: 6805 288a 0800 b028 0da8 4c96 164e 4e4b  h.(....(..L..NNK
-00002290: 0a74 9452 9468 0528 8a08 00b0 5106 b872  .t.R.h.(....Q..r
-000022a0: 9816 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-000022b0: b07a ffc7 989a 164e 4e4b 0a74 9452 9468  .z.....NNK.t.R.h
-000022c0: 0528 8a08 00b0 5467 4370 9c16 4e4e 4b0a  .(....TgCp..NNK.
-000022d0: 7494 5294 6805 288a 0800 b0cc f1e7 e49e  t.R.h.(.........
-000022e0: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-000022f0: f5ea f70a a116 4e4e 4b0a 7494 5294 6805  ......NNK.t.R.h.
-00002300: 288a 0800 b01e e407 31a3 164e 4e4b 0a74  (.......1..NNK.t
-00002310: 9452 9468 0528 8a08 00b0 47dd 1757 a516  .R.h.(....G..W..
-00002320: 4e4e 4b0a 7494 5294 6805 288a 0800 b070  NNK.t.R.h.(....p
-00002330: d627 7da7 164e 4e4b 0a74 9452 9468 0528  .'}..NNK.t.R.h.(
-00002340: 8a08 00b0 99cf 37a3 a916 4e4e 4b0a 7494  ......7...NNK.t.
-00002350: 5294 6805 288a 0800 b0c2 c847 c9ab 164e  R.h.(......G...N
-00002360: 4e4b 0a74 9452 9468 0528 8a08 00b0 ebc1  NK.t.R.h.(......
-00002370: 57ef ad16 4e4e 4b0a 7494 5294 6805 288a  W...NNK.t.R.h.(.
-00002380: 0800 b014 bb67 15b0 164e 4e4b 0a74 9452  .....g...NNK.t.R
-00002390: 9468 0528 8a08 00b0 3db4 773b b216 4e4e  .h.(....=.w;..NN
-000023a0: 4b0a 7494 5294 6805 288a 0800 b017 1cf3  K.t.R.h.(.......
-000023b0: 12b4 164e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-000023c0: 00b0 8fa6 9787 b616 4e4e 4b0a 7494 5294  ........NNK.t.R.
-000023d0: 6805 288a 0800 b0b8 9fa7 adb8 164e 4e4b  h.(..........NNK
-000023e0: 0a74 9452 9468 0528 8a08 00b0 e198 b7d3  .t.R.h.(........
-000023f0: ba16 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00002400: b00a 92c7 f9bc 164e 4e4b 0a74 9452 9468  .......NNK.t.R.h
-00002410: 0528 8a08 00b0 338b d71f bf16 4e4e 4b0a  .(....3.....NNK.
-00002420: 7494 5294 6805 288a 0800 b05c 84e7 45c1  t.R.h.(....\..E.
+00002050: 368a 8546 6017 4e4e 4b0a 7494 5294 6805  6..F`.NNK.t.R.h.
+00002060: 288a 0800 b050 b128 bb62 164e 4e4b 0a74  (....P.(.b.NNK.t
+00002070: 9452 9468 0528 8a08 00b0 b52b d06d a017  .R.h.(.....+.m..
+00002080: 4e4e 4b0a 7494 5294 6805 288a 0800 b02e  NNK.t.R.h.(.....
+00002090: e20a 8ab2 154e 4e4b 0a74 9452 9468 0528  .....NNK.t.R.h.(
+000020a0: 8a08 00b0 2b0c 5673 3717 4e4e 4b0a 7494  ....+.Vs7.NNK.t.
+000020b0: 5294 6805 288a 0800 b044 6940 178d 174e  R.h.(....Di@...N
+000020c0: 4e4b 0a74 9452 9468 0528 8a08 00b0 0793  NK.t.R.h.(......
+000020d0: 19d3 1b16 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
+000020e0: 0800 b03d b477 3bb2 164e 4e4b 0a74 9452  ...=.w;..NNK.t.R
+000020f0: 9468 0528 8a08 00b0 45be cfce c217 4e4e  .h.(....E.....NN
+00002100: 4b0a 7494 5294 6805 288a 0800 b04c 5deb  K.t.R.h.(....L].
+00002110: dc8b 154e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+00002120: 00b0 c67e 627e e516 4e4e 4b0a 7494 5294  ...~b~..NNK.t.R.
+00002130: 6805 288a 0800 b016 6586 841b 174e 4e4b  h.(.....e....NNK
+00002140: 0a74 9452 9468 0528 8a08 00b0 1cc5 bfa8  .t.R.h.(........
+00002150: c017 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00002160: b0a9 cd3a fcb8 154e 4e4b 0a74 9452 9468  ...:...NNK.t.R.h
+00002170: 0528 8a08 00b0 a5a2 f62d 0817 4e4e 4b0a  .(.......-..NNK.
+00002180: 7494 5294 6805 288a 0800 b069 ac35 8855  t.R.h.(....i.5.U
+00002190: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+000021a0: 5b2f 588e 8b16 4e4e 4b0a 7494 5294 6805  [/X...NNK.t.R.h.
+000021b0: 288a 0800 b046 135f 86f8 174e 4e4b 0a74  (....F._...NNK.t
+000021c0: 9452 9468 0528 8a08 00b0 093d 3842 8716  .R.h.(.....=8B..
+000021d0: 4e4e 4b0a 7494 5294 6805 288a 0800 b09f  NNK.t.R.h.(.....
+000021e0: a49a e0c5 154e 4e4b 0a74 9452 9468 0528  .....NNK.t.R.h.(
+000021f0: 8a08 00b0 8129 ba8d ec15 4e4e 4b0a 7494  .....)....NNK.t.
+00002200: 5294 6805 288a 0800 b087 2716 db2e 174e  R.h.(.....'....N
+00002210: 4e4b 0a74 9452 9468 0528 8a08 00b0 6259  NK.t.R.h.(....bY
+00002220: 4a83 dd15 4e4e 4b0a 7494 5294 6805 288a  J...NNK.t.R.h.(.
+00002230: 0800 b063 aed9 3a13 164e 4e4b 0a74 9452  ...c..:..NNK.t.R
+00002240: 9468 0528 8a08 00b0 c173 b811 7616 4e4e  .h.(.....s..v.NN
+00002250: 4b0a 7494 5294 6805 288a 0800 b0c9 f239  K.t.R.h.(......9
+00002260: befd 154e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+00002270: 00b0 7280 46ec 1217 4e4e 4b0a 7494 5294  ..r.F...NNK.t.R.
+00002280: 6805 288a 0800 b04a dcc5 7d46 174e 4e4b  h.(....J..}F.NNK
+00002290: 0a74 9452 9468 0528 8a08 00b0 d045 25c3  .t.R.h.(.....E%.
+000022a0: 7517 4e4e 4b0a 7494 5294 6805 288a 0800  u.NNK.t.R.h.(...
+000022b0: b00c 299a 2614 184e 4e4b 0a74 9452 9468  ..).&..NNK.t.R.h
+000022c0: 0528 8a08 00b0 ad21 78da 8f16 4e4e 4b0a  .(.....!x...NNK.
+000022d0: 7494 5294 6805 288a 0800 b012 9c1f 8dcd  t.R.h.(.........
+000022e0: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+000022f0: ae76 0792 c516 4e4e 4b0a 7494 5294 6805  .v....NNK.t.R.h.
+00002300: 288a 0800 b05c 84e7 45c1 164e 4e4b 0a74  (....\..E..NNK.t
+00002310: 9452 9468 0528 8a08 00b0 525b 472a ce16  .R.h.(....R[G*..
+00002320: 4e4e 4b0a 7494 5294 6805 288a 0800 b030  NNK.t.R.h.(....0
+00002330: 1700 e0a6 174e 4e4b 0a74 9452 9468 0528  .....NNK.t.R.h.(
+00002340: 8a08 00b0 cb9c 582d 6916 4e4e 4b0a 7494  ......X-i.NNK.t.
+00002350: 5294 6805 288a 0800 b028 0da8 4c96 164e  R.h.(....(..L..N
+00002360: 4e4b 0a74 9452 9468 0528 8a08 00b0 2962  NK.t.R.h.(....)b
+00002370: 3704 cc16 4e4e 4b0a 7494 5294 6805 288a  7...NNK.t.R.h.(.
+00002380: 0800 b040 b325 6253 174e 4e4b 0a74 9452  ...@.%bS.NNK.t.R
+00002390: 9468 0528 8a08 00b0 0be7 56b1 f216 4e4e  .h.(......V...NN
+000023a0: 4b0a 7494 5294 6805 288a 0800 b076 ab8a  K.t.R.h.(....v..
+000023b0: bac3 154e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+000023c0: 00b0 cad2 9f5c bc17 4e4e 4b0a 7494 5294  .....\..NNK.t.R.
+000023d0: 6805 288a 0800 b027 b818 9560 164e 4e4b  h.(....'...`.NNK
+000023e0: 0a74 9452 9468 0528 8a08 00b0 7700 1a72  .t.R.h.(....w..r
+000023f0: f915 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00002400: b0ab 7759 6b24 164e 4e4b 0a74 9452 9468  ..wYk$.NNK.t.R.h
+00002410: 0528 8a08 00b0 555a f550 6f17 4e4e 4b0a  .(....UZ.Po.NNK.
+00002420: 7494 5294 6805 288a 0800 b0a5 04d4 046b  t.R.h.(........k
 00002430: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00002440: 857d f76b c316 4e4e 4b0a 7494 5294 6805  .}.k..NNK.t.R.h.
-00002450: 288a 0800 b0ae 7607 92c5 164e 4e4b 0a74  (.....v....NNK.t
-00002460: 9452 9468 0528 8a08 00b0 d76f 17b8 c716  .R.h.(.....o....
-00002470: 4e4e 4b0a 7494 5294 6805 288a 0800 b000  NNK.t.R.h.(.....
-00002480: 6927 dec9 164e 4e4b 0a74 9452 9468 0528  i'...NNK.t.R.h.(
-00002490: 8a08 00b0 2962 3704 cc16 4e4e 4b0a 7494  ....)b7...NNK.t.
-000024a0: 5294 6805 288a 0800 b052 5b47 2ace 164e  R.h.(....R[G*..N
-000024b0: 4e4b 0a74 9452 9468 0528 8a08 00b0 7b54  NK.t.R.h.(....{T
-000024c0: 5750 d016 4e4e 4b0a 7494 5294 6805 288a  WP..NNK.t.R.h.(.
-000024d0: 0800 b0a4 4d67 76d2 164e 4e4b 0a74 9452  ....Mgv..NNK.t.R
-000024e0: 9468 0528 8a08 00b0 cd46 779c d416 4e4e  .h.(.....Fw...NN
-000024f0: 4b0a 7494 5294 6805 288a 0800 b0f6 3f87  K.t.R.h.(.....?.
-00002500: c2d6 164e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00002510: 00b0 1f39 97e8 d816 4e4e 4b0a 7494 5294  ...9....NNK.t.R.
-00002520: 6805 288a 0800 b048 32a7 0edb 164e 4e4b  h.(....H2....NNK
-00002530: 0a74 9452 9468 0528 8a08 00b0 712b b734  .t.R.h.(....q+.4
-00002540: dd16 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00002550: b09a 24c7 5adf 164e 4e4b 0a74 9452 9468  ..$.Z..NNK.t.R.h
-00002560: 0528 8a08 00b0 c31d d780 e116 4e4e 4b0a  .(..........NNK.
-00002570: 7494 5294 6805 288a 0800 b0ec 16e7 a6e3  t.R.h.(.........
-00002580: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00002590: c67e 627e e516 4e4e 4b0a 7494 5294 6805  .~b~..NNK.t.R.h.
-000025a0: 288a 0800 b03e 0907 f3e7 164e 4e4b 0a74  (....>.....NNK.t
-000025b0: 9452 9468 0528 8a08 00b0 6702 1719 ea16  .R.h.(....g.....
-000025c0: 4e4e 4b0a 7494 5294 6805 288a 0800 b090  NNK.t.R.h.(.....
-000025d0: fb26 3fec 164e 4e4b 0a74 9452 9468 0528  .&?..NNK.t.R.h.(
-000025e0: 8a08 00b0 b9f4 3665 ee16 4e4e 4b0a 7494  ......6e..NNK.t.
-000025f0: 5294 6805 288a 0800 b0e2 ed46 8bf0 164e  R.h.(......F...N
-00002600: 4e4b 0a74 9452 9468 0528 8a08 00b0 0be7  NK.t.R.h.(......
-00002610: 56b1 f216 4e4e 4b0a 7494 5294 6805 288a  V...NNK.t.R.h.(.
-00002620: 0800 b034 e066 d7f4 164e 4e4b 0a74 9452  ...4.f...NNK.t.R
-00002630: 9468 0528 8a08 00b0 5dd9 76fd f616 4e4e  .h.(....].v...NN
-00002640: 4b0a 7494 5294 6805 288a 0800 b086 d286  K.t.R.h.(.......
-00002650: 23f9 164e 4e4b 0a74 9452 9468 0528 8a08  #..NNK.t.R.h.(..
-00002660: 00b0 afcb 9649 fb16 4e4e 4b0a 7494 5294  .....I..NNK.t.R.
-00002670: 6805 288a 0800 b0d8 c4a6 6ffd 164e 4e4b  h.(.......o..NNK
-00002680: 0a74 9452 9468 0528 8a08 00b0 01be b695  .t.R.h.(........
-00002690: ff16 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-000026a0: b02a b7c6 bb01 174e 4e4b 0a74 9452 9468  .*.....NNK.t.R.h
-000026b0: 0528 8a08 00b0 53b0 d6e1 0317 4e4e 4b0a  .(....S.....NNK.
-000026c0: 7494 5294 6805 288a 0800 b07c a9e6 0706  t.R.h.(....|....
-000026d0: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-000026e0: a5a2 f62d 0817 4e4e 4b0a 7494 5294 6805  ...-..NNK.t.R.h.
-000026f0: 288a 0800 b0ce 9b06 540a 174e 4e4b 0a74  (.......T..NNK.t
-00002700: 9452 9468 0528 8a08 00b0 f794 167a 0c17  .R.h.(.......z..
-00002710: 4e4e 4b0a 7494 5294 6805 288a 0800 b020  NNK.t.R.h.(.... 
-00002720: 8e26 a00e 174e 4e4b 0a74 9452 9468 0528  .&...NNK.t.R.h.(
-00002730: 8a08 00b0 4987 36c6 1017 4e4e 4b0a 7494  ....I.6...NNK.t.
-00002740: 5294 6805 288a 0800 b072 8046 ec12 174e  R.h.(....r.F...N
-00002750: 4e4b 0a74 9452 9468 0528 8a08 00b0 9b79  NK.t.R.h.(.....y
-00002760: 5612 1517 4e4e 4b0a 7494 5294 6805 288a  V...NNK.t.R.h.(.
-00002770: 0800 b0c4 7266 3817 174e 4e4b 0a74 9452  ....rf8..NNK.t.R
-00002780: 9468 0528 8a08 00b0 ed6b 765e 1917 4e4e  .h.(.....kv^..NN
-00002790: 4b0a 7494 5294 6805 288a 0800 b016 6586  K.t.R.h.(.....e.
-000027a0: 841b 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-000027b0: 00b0 3f5e 96aa 1d17 4e4e 4b0a 7494 5294  ..?^....NNK.t.R.
-000027c0: 6805 288a 0800 b068 57a6 d01f 174e 4e4b  h.(....hW....NNK
-000027d0: 0a74 9452 9468 0528 8a08 00b0 9150 b6f6  .t.R.h.(.....P..
-000027e0: 2117 4e4e 4b0a 7494 5294 6805 288a 0800  !.NNK.t.R.h.(...
-000027f0: b0ba 49c6 1c24 174e 4e4b 0a74 9452 9468  ..I..$.NNK.t.R.h
-00002800: 0528 8a08 00b0 e342 d642 2617 4e4e 4b0a  .(.....B.B&.NNK.
-00002810: 7494 5294 6805 288a 0800 b00c 3ce6 6828  t.R.h.(.....<.h(
-00002820: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00002830: 3535 f68e 2a17 4e4e 4b0a 7494 5294 6805  55..*.NNK.t.R.h.
-00002840: 288a 0800 b05e 2e06 b52c 174e 4e4b 0a74  (....^...,.NNK.t
-00002850: 9452 9468 0528 8a08 00b0 8727 16db 2e17  .R.h.(.....'....
-00002860: 4e4e 4b0a 7494 5294 6805 288a 0800 b0b0  NNK.t.R.h.(.....
-00002870: 2026 0131 174e 4e4b 0a74 9452 9468 0528   &.1.NNK.t.R.h.(
-00002880: 8a08 00b0 d919 3627 3317 4e4e 4b0a 7494  ......6'3.NNK.t.
-00002890: 5294 6805 288a 0800 b002 1346 4d35 174e  R.h.(......FM5.N
-000028a0: 4e4b 0a74 9452 9468 0528 8a08 00b0 2b0c  NK.t.R.h.(....+.
-000028b0: 5673 3717 4e4e 4b0a 7494 5294 6805 288a  Vs7.NNK.t.R.h.(.
-000028c0: 0800 b054 0566 9939 174e 4e4b 0a74 9452  ...T.f.9.NNK.t.R
-000028d0: 9468 0528 8a08 00b0 7dfe 75bf 3b17 4e4e  .h.(....}.u.;.NN
-000028e0: 4b0a 7494 5294 6805 288a 0800 b057 66f1  K.t.R.h.(....Wf.
-000028f0: 963d 174e 4e4b 0a74 9452 9468 0528 8a08  .=.NNK.t.R.h.(..
-00002900: 00b0 cff0 950b 4017 4e4e 4b0a 7494 5294  ......@.NNK.t.R.
-00002910: 6805 288a 0800 b0f8 e9a5 3142 174e 4e4b  h.(.......1B.NNK
-00002920: 0a74 9452 9468 0528 8a08 00b0 21e3 b557  .t.R.h.(....!..W
-00002930: 4417 4e4e 4b0a 7494 5294 6805 288a 0800  D.NNK.t.R.h.(...
-00002940: b04a dcc5 7d46 174e 4e4b 0a74 9452 9468  .J..}F.NNK.t.R.h
-00002950: 0528 8a08 00b0 73d5 d5a3 4817 4e4e 4b0a  .(....s...H.NNK.
-00002960: 7494 5294 6805 288a 0800 b09c cee5 c94a  t.R.h.(........J
-00002970: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00002980: c5c7 f5ef 4c17 4e4e 4b0a 7494 5294 6805  ....L.NNK.t.R.h.
-00002990: 288a 0800 b0ee c005 164f 174e 4e4b 0a74  (........O.NNK.t
-000029a0: 9452 9468 0528 8a08 00b0 c828 81ed 5017  .R.h.(.....(..P.
-000029b0: 4e4e 4b0a 7494 5294 6805 288a 0800 b040  NNK.t.R.h.(....@
-000029c0: b325 6253 174e 4e4b 0a74 9452 9468 0528  .%bS.NNK.t.R.h.(
-000029d0: 8a08 00b0 69ac 3588 5517 4e4e 4b0a 7494  ....i.5.U.NNK.t.
-000029e0: 5294 6805 288a 0800 b092 a545 ae57 174e  R.h.(......E.W.N
-000029f0: 4e4b 0a74 9452 9468 0528 8a08 00b0 bb9e  NK.t.R.h.(......
-00002a00: 55d4 5917 4e4e 4b0a 7494 5294 6805 288a  U.Y.NNK.t.R.h.(.
-00002a10: 0800 b0e4 9765 fa5b 174e 4e4b 0a74 9452  .....e.[.NNK.t.R
-00002a20: 9468 0528 8a08 00b0 0d91 7520 5e17 4e4e  .h.(......u ^.NN
-00002a30: 4b0a 7494 5294 6805 288a 0800 b036 8a85  K.t.R.h.(....6..
-00002a40: 4660 174e 4e4b 0a74 9452 9468 0528 8a08  F`.NNK.t.R.h.(..
+00002440: f93e 35e9 7717 4e4e 4b0a 7494 5294 6805  .>5.w.NNK.t.R.h.
+00002450: 288a 0800 b06e b7df f4c4 174e 4e4b 0a74  (....n.....NNK.t
+00002460: 9452 9468 0528 8a08 00b0 316c 8f97 dc17  .R.h.(....1l....
+00002470: 4e4e 4b0a 7494 5294 6805 288a 0800 b02f  NNK.t.R.h.(..../
+00002480: 379a 41e8 154e 4e4b 0a74 9452 9468 0528  7.A..NNK.t.R.h.(
+00002490: 8a08 00b0 4533 f9e7 3916 4e4e 4b0a 7494  ....E3..9.NNK.t.
+000024a0: 5294 6805 288a 0800 b083 d3d8 fc57 164e  R.h.(........W.N
+000024b0: 4e4b 0a74 9452 9468 0528 8a08 00b0 4b31  NK.t.R.h.(....K1
+000024c0: 5535 7c17 4e4e 4b0a 7494 5294 6805 288a  U5|.NNK.t.R.h.(.
+000024d0: 0800 b039 603a 5ddb 154e 4e4b 0a74 9452  ...9`:]..NNK.t.R
+000024e0: 9468 0528 8a08 00b0 8ca7 e960 1516 4e4e  .h.(.......`..NN
+000024f0: 4b0a 7494 5294 6805 288a 0800 b0ed 6b76  K.t.R.h.(.....kv
+00002500: 5e19 174e 4e4b 0a74 9452 9468 0528 8a08  ^..NNK.t.R.h.(..
+00002510: 00b0 5e2e 06b5 2c17 4e4e 4b0a 7494 5294  ..^...,.NNK.t.R.
+00002520: 6805 288a 0800 b0b9 f436 65ee 164e 4e4b  h.(......6e..NNK
+00002530: 0a74 9452 9468 0528 8a08 00b0 ce9b 0654  .t.R.h.(.......T
+00002540: 0a17 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00002550: b042 344b c198 154e 4e4b 0a74 9452 9468  .B4K...NNK.t.R.h
+00002560: 0528 8a08 00b0 d31b dad9 f015 4e4e 4b0a  .(..........NNK.
+00002570: 7494 5294 6805 288a 0800 b049 8736 c610  t.R.h.(....I.6..
+00002580: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00002590: 9150 b6f6 2117 4e4e 4b0a 7494 5294 6805  .P..!.NNK.t.R.h.
+000025a0: 288a 0800 b0ba 49c6 1c24 174e 4e4b 0a74  (.....I..$.NNK.t
+000025b0: 9452 9468 0528 8a08 00b0 9a11 7b18 cb17  .R.h.(......{...
+000025c0: 4e4e 4b0a 7494 5294 6805 288a 0800 b058  NNK.t.R.h.(....X
+000025d0: 30aa 67ea 154e 4e4b 0a74 9452 9468 0528  0.g..NNK.t.R.h.(
+000025e0: 8a08 00b0 bfc9 99a2 0a16 4e4e 4b0a 7494  ..........NNK.t.
+000025f0: 5294 6805 288a 0800 b0ac cce8 225a 164e  R.h.(......."Z.N
+00002600: 4e4b 0a74 9452 9468 0528 8a08 00b0 0f12  NK.t.R.h.(......
+00002610: 9b7f a315 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
+00002620: 0800 b07a ffc7 989a 164e 4e4b 0a74 9452  ...z.....NNK.t.R
+00002630: 9468 0528 8a08 00b0 47dd 1757 a516 4e4e  .h.(....G..W..NN
+00002640: 4b0a 7494 5294 6805 288a 0800 b01d 8f78  K.t.R.h.(......x
+00002650: 796d 164e 4e4b 0a74 9452 9468 0528 8a08  ym.NNK.t.R.h.(..
+00002660: 00b0 b2ca 4470 9c17 4e4e 4b0a 7494 5294  ....Dp..NNK.t.R.
+00002670: 6805 288a 0800 b082 0920 2cab 174e 4e4b  h.(...... ,..NNK
+00002680: 0a74 9452 9468 0528 8a08 00b0 e198 b7d3  .t.R.h.(........
+00002690: ba16 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+000026a0: b073 d5d5 a348 174e 4e4b 0a74 9452 9468  .s...H.NNK.t.R.h
+000026b0: 0528 8a08 00b0 c31d d780 e116 4e4e 4b0a  .(..........NNK.
+000026c0: 7494 5294 6805 288a 0800 b06f 8198 c571  t.R.h.(....o...q
+000026d0: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+000026e0: 92a5 45ae 5717 4e4e 4b0a 7494 5294 6805  ..E.W.NNK.t.R.h.
+000026f0: 288a 0800 b0f0 412b 7594 154e 4e4b 0a74  (.....A+u..NNK.t
+00002700: 9452 9468 0528 8a08 00b0 e342 d642 2617  .R.h.(.....B.B&.
+00002710: 4e4e 4b0a 7494 5294 6805 288a 0800 b01b  NNK.t.R.h.(.....
+00002720: 7030 f18a 174e 4e4b 0a74 9452 9468 0528  p0...NNK.t.R.h.(
+00002730: 8a08 00b0 b680 5f25 d617 4e4e 4b0a 7494  ......_%..NNK.t.
+00002740: 5294 6805 288a 0800 b03b 0a59 cc46 164e  R.h.(....;.Y.F.N
+00002750: 4e4b 0a74 9452 9468 0528 8a08 00b0 f63f  NK.t.R.h.(.....?
+00002760: 87c2 d616 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
+00002770: 0800 b0d8 c4a6 6ffd 164e 4e4b 0a74 9452  ......o..NNK.t.R
+00002780: 9468 0528 8a08 00b0 8dfc 7818 4b16 4e4e  .h.(......x.K.NN
+00002790: 4b0a 7494 5294 6805 288a 0800 b078 55a9  K.t.R.h.(....xU.
+000027a0: 292f 164e 4e4b 0a74 9452 9468 0528 8a08  )/.NNK.t.R.h.(..
+000027b0: 00b0 ddcf 50dc 6c17 4e4e 4b0a 7494 5294  ....P.l.NNK.t.R.
+000027c0: 6805 288a 0800 b0ee c005 164f 174e 4e4b  h.(........O.NNK
+000027d0: 0a74 9452 9468 0528 8a08 00b0 e5ec f4b1  .t.R.h.(........
+000027e0: 9117 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+000027f0: b0e6 188b 59a1 154e 4e4b 0a74 9452 9468  ....Y..NNK.t.R.h
+00002800: 0528 8a08 00b0 de99 09ad 1916 4e4e 4b0a  .(..........NNK.
+00002810: 7494 5294 6805 288a 0800 b01f 3997 e8d8  t.R.h.(.....9...
+00002820: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00002830: aa22 cab3 ee15 4e4e 4b0a 7494 5294 6805  ."....NNK.t.R.h.
+00002840: 288a 0800 b0dc efea 3dae 154e 4e4b 0a74  (.......=..NNK.t
+00002850: 9452 9468 0528 8a08 00b0 1c3a e9c1 3716  .R.h.(.....:..7.
+00002860: 4e4e 4b0a 7494 5294 6805 288a 0800 b030  NNK.t.R.h.(....0
+00002870: 8c29 f91d 164e 4e4b 0a74 9452 9468 0528  .)...NNK.t.R.h.(
+00002880: 8a08 00b0 6104 bbcb a715 4e4e 4b0a 7494  ....a.....NNK.t.
+00002890: 5294 6805 288a 0800 b019 3b3b 9b96 154e  R.h.(.....;;...N
+000028a0: 4e4b 0a74 9452 9468 0528 8a08 00b0 8428  NK.t.R.h.(.....(
+000028b0: 68b4 8d16 4e4e 4b0a 7494 5294 6805 288a  h...NNK.t.R.h.(.
+000028c0: 0800 b0e4 9765 fa5b 174e 4e4b 0a74 9452  .....e.[.NNK.t.R
+000028d0: 9468 0528 8a08 00b0 b3f6 da17 ac15 4e4e  .h.(..........NN
+000028e0: 4b0a 7494 5294 6805 288a 0800 b0fb bf5a  K.t.R.h.(......Z
+000028f0: 48bd 154e 4e4b 0a74 9452 9468 0528 8a08  H..NNK.t.R.h.(..
+00002900: 00b0 887c a592 6417 4e4e 4b0a 7494 5294  ...|..d.NNK.t.R.
+00002910: 6805 288a 0800 b005 e9fa 63b0 154e 4e4b  h.(.......c..NNK
+00002920: 0a74 9452 9468 0528 8a08 00b0 e76d 1a11  .t.R.h.(.....m..
+00002930: d715 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00002940: b077 8bf0 5882 174e 4e4b 0a74 9452 9468  .w..X..NNK.t.R.h
+00002950: 0528 8a08 00b0 9b79 5612 1517 4e4e 4b0a  .(.....yV...NNK.
+00002960: 7494 5294 6805 288a 0800 b05d d976 fdf6  t.R.h.(....].v..
+00002970: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00002980: 5106 b872 9816 4e4e 4b0a 7494 5294 6805  Q..r..NNK.t.R.h.
+00002990: 288a 0800 b0f3 40d9 9b35 164e 4e4b 0a74  (.....@..5.NNK.t
+000029a0: 9452 9468 0528 8a08 00b0 9a24 c75a df16  .R.h.(.....$.Z..
+000029b0: 4e4e 4b0a 7494 5294 6805 288a 0800 b0bb  NNK.t.R.h.(.....
+000029c0: 9e55 d459 174e 4e4b 0a74 9452 9468 0528  .U.Y.NNK.t.R.h.(
+000029d0: 8a08 00b0 9e4f 0b29 9015 4e4e 4b0a 7494  .....O.)..NNK.t.
+000029e0: 5294 6805 288a 0800 b094 266b 0d9d 154e  R.h.(.....&k...N
+000029f0: 4e4b 0a74 9452 9468 0528 8a08 00b0 742a  NK.t.R.h.(....t*
+00002a00: 655b 7e17 4e4e 4b0a 7494 5294 6805 288a  e[~.NNK.t.R.h.(.
+00002a10: 0800 b056 af84 08a5 174e 4e4b 0a74 9452  ...V.....NNK.t.R
+00002a20: 9468 0528 8a08 00b0 31e1 b8b0 5316 4e4e  .h.(....1...S.NN
+00002a30: 4b0a 7494 5294 6805 288a 0800 b08a fdca  K.t.R.h.(.......
+00002a40: f1a9 154e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
 00002a50: 00b0 5f83 956c 6217 4e4e 4b0a 7494 5294  .._..lb.NNK.t.R.
-00002a60: 6805 288a 0800 b088 7ca5 9264 174e 4e4b  h.(.....|..d.NNK
-00002a70: 0a74 9452 9468 0528 8a08 00b0 b175 b5b8  .t.R.h.(.....u..
-00002a80: 6617 4e4e 4b0a 7494 5294 6805 288a 0800  f.NNK.t.R.h.(...
-00002a90: b0da 6ec5 de68 174e 4e4b 0a74 9452 9468  ..n..h.NNK.t.R.h
-00002aa0: 0528 8a08 00b0 0368 d504 6b17 4e4e 4b0a  .(.....h..k.NNK.
-00002ab0: 7494 5294 6805 288a 0800 b0dd cf50 dc6c  t.R.h.(......P.l
-00002ac0: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00002ad0: 555a f550 6f17 4e4e 4b0a 7494 5294 6805  UZ.Po.NNK.t.R.h.
-00002ae0: 288a 0800 b07e 5305 7771 174e 4e4b 0a74  (....~S.wq.NNK.t
-00002af0: 9452 9468 0528 8a08 00b0 a74c 159d 7317  .R.h.(.....L..s.
-00002b00: 4e4e 4b0a 7494 5294 6805 288a 0800 b0d0  NNK.t.R.h.(.....
-00002b10: 4525 c375 174e 4e4b 0a74 9452 9468 0528  E%.u.NNK.t.R.h.(
-00002b20: 8a08 00b0 f93e 35e9 7717 4e4e 4b0a 7494  .....>5.w.NNK.t.
-00002b30: 5294 6805 288a 0800 b022 3845 0f7a 174e  R.h.(...."8E.z.N
-00002b40: 4e4b 0a74 9452 9468 0528 8a08 00b0 4b31  NK.t.R.h.(....K1
-00002b50: 5535 7c17 4e4e 4b0a 7494 5294 6805 288a  U5|.NNK.t.R.h.(.
-00002b60: 0800 b074 2a65 5b7e 174e 4e4b 0a74 9452  ...t*e[~.NNK.t.R
-00002b70: 9468 0528 8a08 00b0 9d23 7581 8017 4e4e  .h.(.....#u...NN
-00002b80: 4b0a 7494 5294 6805 288a 0800 b077 8bf0  K.t.R.h.(....w..
-00002b90: 5882 174e 4e4b 0a74 9452 9468 0528 8a08  X..NNK.t.R.h.(..
-00002ba0: 00b0 a084 007f 8417 4e4e 4b0a 7494 5294  ........NNK.t.R.
-00002bb0: 6805 288a 0800 b0c9 7d10 a586 174e 4e4b  h.(.....}....NNK
-00002bc0: 0a74 9452 9468 0528 8a08 00b0 4108 b519  .t.R.h.(....A...
-00002bd0: 8917 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00002be0: b01b 7030 f18a 174e 4e4b 0a74 9452 9468  ..p0...NNK.t.R.h
-00002bf0: 0528 8a08 00b0 4469 4017 8d17 4e4e 4b0a  .(....Di@...NNK.
-00002c00: 7494 5294 6805 288a 0800 b06d 6250 3d8f  t.R.h.(....mbP=.
+00002a60: 6805 288a 0800 b059 1010 06a9 174e 4e4b  h.(....Y.....NNK
+00002a70: 0a74 9452 9468 0528 8a08 00b0 e2ed 468b  .t.R.h.(......F.
+00002a80: f016 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00002a90: b070 d627 7da7 164e 4e4b 0a74 9452 9468  .p.'}..NNK.t.R.h
+00002aa0: 0528 8a08 00b0 1067 2a37 d915 4e4e 4b0a  .(.....g*7..NNK.
+00002ab0: 7494 5294 6805 288a 0800 b098 7aa8 eb73  t.R.h.(.....z..s
+00002ac0: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00002ad0: d61a 8800 9216 4e4e 4b0a 7494 5294 6805  ......NNK.t.R.h.
+00002ae0: 288a 0800 b085 7df7 6bc3 164e 4e4b 0a74  (.....}.k..NNK.t
+00002af0: 9452 9468 0528 8a08 00b0 827e 4945 2216  .R.h.(.....~IE".
+00002b00: 4e4e 4b0a 7494 5294 6805 288a 0800 b08f  NNK.t.R.h.(.....
+00002b10: a697 87b6 164e 4e4b 0a74 9452 9468 0528  .....NNK.t.R.h.(
+00002b20: 8a08 00b0 febe 086f 5e16 4e4e 4b0a 7494  .......o^.NNK.t.
+00002b30: 5294 6805 288a 0800 b0c5 c7f5 ef4c 174e  R.h.(........L.N
+00002b40: 4e4b 0a74 9452 9468 0528 8a08 00b0 79aa  NK.t.R.h.(....y.
+00002b50: 38e1 6416 4e4e 4b0a 7494 5294 6805 288a  8.d.NNK.t.R.h.(.
+00002b60: 0800 b035 35f6 8e2a 174e 4e4b 0a74 9452  ...55..*.NNK.t.R
+00002b70: 9468 0528 8a08 00b0 c89d aa06 c815 4e4e  .h.(..........NN
+00002b80: 4b0a 7494 5294 6805 288a 0800 b034 e066  K.t.R.h.(....4.f
+00002b90: d7f4 164e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+00002ba0: 00b0 01be b695 ff16 4e4e 4b0a 7494 5294  ........NNK.t.R.
+00002bb0: 6805 288a 0800 b0fc 14ea fff2 154e 4e4b  h.(..........NNK
+00002bc0: 0a74 9452 9468 0528 8a08 00b0 4fe7 6fea  .t.R.h.(....O.o.
+00002bd0: b517 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00002be0: b03b 952f b3cf 174e 4e4b 0a74 9452 9468  .;./...NNK.t.R.h
+00002bf0: 0528 8a08 00b0 26c5 66b4 8d15 4e4e 4b0a  .(....&.f...NNK.
+00002c00: 7494 5294 6805 288a 0800 b0d4 fb3f 78af  t.R.h.(......?x.
 00002c10: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00002c20: e5ec f4b1 9117 4e4e 4b0a 7494 5294 6805  ......NNK.t.R.h.
-00002c30: 288a 0800 b0bf 5470 8993 174e 4e4b 0a74  (.....Tp...NNK.t
+00002c20: 3c5f e883 7c16 4e4e 4b0a 7494 5294 6805  <_..|.NNK.t.R.h.
+00002c30: 288a 0800 b090 fb26 3fec 164e 4e4b 0a74  (......&?..NNK.t
 00002c40: 9452 9468 0528 8a08 00b0 e84d 80af 9517  .R.h.(.....M....
-00002c50: 4e4e 4b0a 7494 5294 6805 288a 0800 b011  NNK.t.R.h.(.....
-00002c60: 4790 d597 174e 4e4b 0a74 9452 9468 0528  G....NNK.t.R.h.(
-00002c70: 8a08 00b0 3a40 a0fb 9917 4e4e 4b0a 7494  ....:@....NNK.t.
-00002c80: 5294 6805 288a 0800 b0b2 ca44 709c 174e  R.h.(......Dp..N
-00002c90: 4e4b 0a74 9452 9468 0528 8a08 00b0 8c32  NK.t.R.h.(.....2
-00002ca0: c047 9e17 4e4e 4b0a 7494 5294 6805 288a  .G..NNK.t.R.h.(.
-00002cb0: 0800 b0b5 2bd0 6da0 174e 4e4b 0a74 9452  ....+.m..NNK.t.R
-00002cc0: 9468 0528 8a08 00b0 de24 e093 a217 4e4e  .h.(.....$....NN
-00002cd0: 4b0a 7494 5294 6805 288a 0800 b056 af84  K.t.R.h.(....V..
-00002ce0: 08a5 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00002cf0: 00b0 3017 00e0 a617 4e4e 4b0a 7494 5294  ..0.....NNK.t.R.
-00002d00: 6805 288a 0800 b059 1010 06a9 174e 4e4b  h.(....Y.....NNK
-00002d10: 0a74 9452 9468 0528 8a08 00b0 8209 202c  .t.R.h.(...... ,
-00002d20: ab17 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00002d30: b0fa 93c4 a0ad 174e 4e4b 0a74 9452 9468  .......NNK.t.R.h
-00002d40: 0528 8a08 00b0 d4fb 3f78 af17 4e4e 4b0a  .(......?x..NNK.
-00002d50: 7494 5294 6805 288a 0800 b0fd f44f 9eb1  t.R.h.(......O..
+00002c50: 4e4e 4b0a 7494 5294 6805 288a 0800 b023  NNK.t.R.h.(....#
+00002c60: 64db b689 154e 4e4b 0a74 9452 9468 0528  d....NNK.t.R.h.(
+00002c70: 8a08 00b0 fa93 c4a0 ad17 4e4e 4b0a 7494  ..........NNK.t.
+00002c80: 5294 6805 288a 0800 b086 d286 23f9 164e  R.h.(.......#..N
+00002c90: 4e4b 0a74 9452 9468 0528 8a08 00b0 c01e  NK.t.R.h.(......
+00002ca0: 295a 4016 4e4e 4b0a 7494 5294 6805 288a  )Z@.NNK.t.R.h.(.
+00002cb0: 0800 b0c0 a9ff 40c9 174e 4e4b 0a74 9452  ......@..NNK.t.R
+00002cc0: 9468 0528 8a08 00b0 481f 5bcc c617 4e4e  .h.(....H.[...NN
+00002cd0: 4b0a 7494 5294 6805 288a 0800 b03a b5c9  K.t.R.h.(....:..
+00002ce0: 1411 164e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+00002cf0: 00b0 d919 3627 3317 4e4e 4b0a 7494 5294  ....6'3.NNK.t.R.
+00002d00: 6805 288a 0800 b0be 740a ebd4 154e 4e4b  h.(.....t....NNK
+00002d10: 0a74 9452 9468 0528 8a08 00b0 ccf1 e7e4  .t.R.h.(........
+00002d20: 9e16 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00002d30: b03f 5e96 aa1d 174e 4e4b 0a74 9452 9468  .?^....NNK.t.R.h
+00002d40: 0528 8a08 00b0 0c3c e668 2817 4e4e 4b0a  .(.....<.h(.NNK.
+00002d50: 7494 5294 6805 288a 0800 b041 08b5 1989  t.R.h.(....A....
 00002d60: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00002d70: 26ee 5fc4 b317 4e4e 4b0a 7494 5294 6805  &._...NNK.t.R.h.
-00002d80: 288a 0800 b04f e76f eab5 174e 4e4b 0a74  (....O.o...NNK.t
-00002d90: 9452 9468 0528 8a08 00b0 c771 145f b817  .R.h.(.....q._..
-00002da0: 4e4e 4b0a 7494 5294 6805 288a 0800 b0a1  NNK.t.R.h.(.....
-00002db0: d98f 36ba 174e 4e4b 0a74 9452 9468 0528  ..6..NNK.t.R.h.(
-00002dc0: 8a08 00b0 cad2 9f5c bc17 4e4e 4b0a 7494  .......\..NNK.t.
-00002dd0: 5294 6805 288a 0800 b0f3 cbaf 82be 174e  R.h.(..........N
-00002de0: 4e4b 0a74 9452 9468 0528 8a08 00b0 1cc5  NK.t.R.h.(......
-00002df0: bfa8 c017 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
-00002e00: 0800 b045 becf cec2 174e 4e4b 0a74 9452  ...E.....NNK.t.R
-00002e10: 9468 0528 8a08 00b0 6eb7 dff4 c417 4e4e  .h.(....n.....NN
-00002e20: 4b0a 7494 5294 6805 288a 0800 b048 1f5b  K.t.R.h.(....H.[
-00002e30: ccc6 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00002e40: 00b0 c0a9 ff40 c917 4e4e 4b0a 7494 5294  .....@..NNK.t.R.
-00002e50: 6805 288a 0800 b09a 117b 18cb 174e 4e4b  h.(......{...NNK
-00002e60: 0a74 9452 9468 0528 8a08 00b0 129c 1f8d  .t.R.h.(........
-00002e70: cd17 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00002e80: b03b 952f b3cf 174e 4e4b 0a74 9452 9468  .;./...NNK.t.R.h
-00002e90: 0528 8a08 00b0 648e 3fd9 d117 4e4e 4b0a  .(....d.?...NNK.
-00002ea0: 7494 5294 6805 288a 0800 b08d 874f ffd3  t.R.h.(......O..
+00002d70: 1211 49a6 4416 4e4e 4b0a 7494 5294 6805  ..I.D.NNK.t.R.h.
+00002d80: 288a 0800 b0b6 f588 3e4d 164e 4e4b 0a74  (.......>M.NNK.t
+00002d90: 9452 9468 0528 8a08 00b0 99cf 37a3 a916  .R.h.(......7...
+00002da0: 4e4e 4b0a 7494 5294 6805 288a 0800 b07b  NNK.t.R.h.(....{
+00002db0: 5457 50d0 164e 4e4b 0a74 9452 9468 0528  TWP..NNK.t.R.h.(
+00002dc0: 8a08 00b0 f794 167a 0c17 4e4e 4b0a 7494  .......z..NNK.t.
+00002dd0: 5294 6805 288a 0800 b017 1cf3 12b4 164e  R.h.(..........N
+00002de0: 4e4b 0a74 9452 9468 0528 8a08 00b0 b175  NK.t.R.h.(.....u
+00002df0: b5b8 6617 4e4e 4b0a 7494 5294 6805 288a  ..f.NNK.t.R.h.(.
+00002e00: 0800 b026 ee5f c4b3 174e 4e4b 0a74 9452  ...&._...NNK.t.R
+00002e10: 9468 0528 8a08 00b0 b5a0 f986 1716 4e4e  .h.(..........NN
+00002e20: 4b0a 7494 5294 6805 288a 0800 b02a b7c6  K.t.R.h.(....*..
+00002e30: bb01 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+00002e40: 00b0 6857 a6d0 1f17 4e4e 4b0a 7494 5294  ..hW....NNK.t.R.
+00002e50: 6805 288a 0800 b00d 9175 205e 174e 4e4b  h.(......u ^.NNK
+00002e60: 0a74 9452 9468 0528 8a08 00b0 7e53 0577  .t.R.h.(....~S.w
+00002e70: 7117 4e4e 4b0a 7494 5294 6805 288a 0800  q.NNK.t.R.h.(...
+00002e80: b038 0bab a5a5 154e 4e4b 0a74 9452 9468  .8.....NNK.t.R.h
+00002e90: 0528 8a08 00b0 2238 450f 7a17 4e4e 4b0a  .(...."8E.z.NNK.
+00002ea0: 7494 5294 6805 288a 0800 b002 1346 4d35  t.R.h.(......FM5
 00002eb0: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00002ec0: 316c 8f97 dc17 4e4e 4b0a 7494 5294 6805  1l....NNK.t.R.h.
-00002ed0: 288a 0800 b0fe 49df 55e7 174e 4e4b 0a74  (.....I.U..NNK.t
-00002ee0: 9452 9468 0528 8a08 00b0 4613 5f86 f817  .R.h.(....F._...
-00002ef0: 4e4e 4b0a 7494 5294 6805 288a 0800 b00c  NNK.t.R.h.(.....
-00002f00: 299a 2614 184e 4e4b 0a74 9452 9468 0528  ).&..NNK.t.R.h.(
-00002f10: 8a08 00b0 7061 fe63 3018 4e4e 4b0a 7494  ....pa.c0.NNK.t.
-00002f20: 5294 658c 0846 494e 4e49 4654 5994 5d94  R.e..FINNIFTY.].
-00002f30: 2868 0528 8a08 00b0 accc e822 5a16 4e4e  (h.(......."Z.NN
-00002f40: 4b0a 7494 5294 6805 288a 0800 b0d5 c5f8  K.t.R.h.(.......
-00002f50: 485c 164e 4e4b 0a74 9452 9468 0528 8a08  H\.NNK.t.R.h.(..
-00002f60: 00b0 febe 086f 5e16 4e4e 4b0a 7494 5294  .....o^.NNK.t.R.
-00002f70: 6805 288a 0800 b027 b818 9560 164e 4e4b  h.(....'...`.NNK
-00002f80: 0a74 9452 9468 0528 8a08 00b0 50b1 28bb  .t.R.h.(....P.(.
-00002f90: 6216 4e4e 4b0a 7494 5294 6805 288a 0800  b.NNK.t.R.h.(...
-00002fa0: b079 aa38 e164 164e 4e4b 0a74 9452 9468  .y.8.d.NNK.t.R.h
-00002fb0: 0528 8a08 00b0 a2a3 4807 6716 4e4e 4b0a  .(......H.g.NNK.
-00002fc0: 7494 5294 6805 288a 0800 b0cb 9c58 2d69  t.R.h.(......X-i
-00002fd0: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00002fe0: a504 d404 6b16 4e4e 4b0a 7494 5294 6805  ....k.NNK.t.R.h.
-00002ff0: 288a 0800 b01d 8f78 796d 164e 4e4b 0a74  (......xym.NNK.t
-00003000: 9452 9468 0528 8a08 00b0 4688 889f 6f16  .R.h.(....F...o.
-00003010: 4e4e 4b0a 7494 5294 6805 288a 0800 b06f  NNK.t.R.h.(....o
-00003020: 8198 c571 164e 4e4b 0a74 9452 9468 0528  ...q.NNK.t.R.h.(
-00003030: 8a08 00b0 987a a8eb 7316 4e4e 4b0a 7494  .....z..s.NNK.t.
-00003040: 5294 6805 288a 0800 b0c1 73b8 1176 164e  R.h.(.....s..v.N
-00003050: 4e4b 0a74 9452 9468 0528 8a08 00b0 ea6c  NK.t.R.h.(.....l
-00003060: c837 7816 4e4e 4b0a 7494 5294 6805 288a  .7x.NNK.t.R.h.(.
-00003070: 0800 b013 66d8 5d7a 164e 4e4b 0a74 9452  ....f.]z.NNK.t.R
-00003080: 9468 0528 8a08 00b0 3c5f e883 7c16 4e4e  .h.(....<_..|.NN
-00003090: 4b0a 7494 5294 6805 288a 0800 b016 c763  K.t.R.h.(......c
-000030a0: 5b7e 164e 4e4b 0a74 9452 9468 0528 8a08  [~.NNK.t.R.h.(..
-000030b0: 00b0 8e51 08d0 8016 4e4e 4b0a 7494 5294  ...Q....NNK.t.R.
-000030c0: 6805 288a 0800 b0b7 4a18 f682 164e 4e4b  h.(.....J....NNK
-000030d0: 0a74 9452 9468 0528 8a08 00b0 e043 281c  .t.R.h.(.....C(.
-000030e0: 8516 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-000030f0: b009 3d38 4287 164e 4e4b 0a74 9452 9468  ..=8B..NNK.t.R.h
-00003100: 0528 8a08 00b0 3236 4868 8916 4e4e 4b0a  .(....26Hh..NNK.
-00003110: 7494 5294 6805 288a 0800 b05b 2f58 8e8b  t.R.h.(....[/X..
-00003120: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00003130: 8428 68b4 8d16 4e4e 4b0a 7494 5294 6805  .(h...NNK.t.R.h.
-00003140: 288a 0800 b0ad 2178 da8f 164e 4e4b 0a74  (.....!x...NNK.t
-00003150: 9452 9468 0528 8a08 00b0 d61a 8800 9216  .R.h.(..........
-00003160: 4e4e 4b0a 7494 5294 6805 288a 0800 b0ff  NNK.t.R.h.(.....
-00003170: 1398 2694 164e 4e4b 0a74 9452 9468 0528  ..&..NNK.t.R.h.(
-00003180: 8a08 00b0 280d a84c 9616 4e4e 4b0a 7494  ....(..L..NNK.t.
-00003190: 5294 6805 288a 0800 b051 06b8 7298 164e  R.h.(....Q..r..N
-000031a0: 4e4b 0a74 9452 9468 0528 8a08 00b0 7aff  NK.t.R.h.(....z.
-000031b0: c798 9a16 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
-000031c0: 0800 b054 6743 709c 164e 4e4b 0a74 9452  ...TgCp..NNK.t.R
-000031d0: 9468 0528 8a08 00b0 ccf1 e7e4 9e16 4e4e  .h.(..........NN
-000031e0: 4b0a 7494 5294 6805 288a 0800 b0f5 eaf7  K.t.R.h.(.......
-000031f0: 0aa1 164e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00003200: 00b0 1ee4 0731 a316 4e4e 4b0a 7494 5294  .....1..NNK.t.R.
-00003210: 6805 288a 0800 b047 dd17 57a5 164e 4e4b  h.(....G..W..NNK
-00003220: 0a74 9452 9468 0528 8a08 00b0 70d6 277d  .t.R.h.(....p.'}
-00003230: a716 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00003240: b099 cf37 a3a9 164e 4e4b 0a74 9452 9468  ...7...NNK.t.R.h
-00003250: 0528 8a08 00b0 c2c8 47c9 ab16 4e4e 4b0a  .(......G...NNK.
-00003260: 7494 5294 6805 288a 0800 b0eb c157 efad  t.R.h.(......W..
+00002ec0: 5766 f196 3d17 4e4e 4b0a 7494 5294 6805  Wf..=.NNK.t.R.h.
+00002ed0: 288a 0800 b0a0 8400 7f84 174e 4e4b 0a74  (..........NNK.t
+00002ee0: 9452 9468 0528 8a08 00b0 a74c 159d 7317  .R.h.(.....L..s.
+00002ef0: 4e4e 4b0a 7494 5294 6805 288a 0800 b064  NNK.t.R.h.(....d
+00002f00: 8e3f d9d1 174e 4e4b 0a74 9452 9468 0528  .?...NNK.t.R.h.(
+00002f10: 8a08 00b0 ff13 9826 9416 4e4e 4b0a 7494  .......&..NNK.t.
+00002f20: 5294 6805 288a 0800 b043 89da 78ce 154e  R.h.(....C..x..N
+00002f30: 4e4b 0a74 9452 9468 0528 8a08 00b0 d76f  NK.t.R.h.(.....o
+00002f40: 17b8 c716 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
+00002f50: 0800 b032 3648 6889 164e 4e4b 0a74 9452  ...26Hh..NNK.t.R
+00002f60: 9468 0528 8a08 00b0 7061 fe63 3018 4e4e  .h.(....pa.c0.NN
+00002f70: 4b0a 7494 5294 658c 0846 494e 4e49 4654  K.t.R.e..FINNIFT
+00002f80: 5994 5d94 2868 0528 8a08 00b0 70c3 db3a  Y.].(h.(....p..:
+00002f90: 9317 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00002fa0: b0c8 8a5e c4b3 164e 4e4b 0a74 9452 9468  ...^...NNK.t.R.h
+00002fb0: 0528 8a08 00b0 3285 d9fc d716 4e4e 4b0a  .(....2.....NNK.
+00002fc0: 7494 5294 6805 288a 0800 b0de 86bd 6a05  t.R.h.(.......j.
+00002fd0: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00002fe0: f5ea f70a a116 4e4e 4b0a 7494 5294 6805  ......NNK.t.R.h.
+00002ff0: 288a 0800 b0b7 4a18 f682 164e 4e4b 0a74  (.....J....NNK.t
+00003000: 9452 9468 0528 8a08 00b0 ff00 4ce4 7f17  .R.h.(......L...
+00003010: 4e4e 4b0a 7494 5294 6805 288a 0800 b0b4  NNK.t.R.h.(.....
+00003020: 381e 8dcd 164e 4e4b 0a74 9452 9468 0528  8....NNK.t.R.h.(
+00003030: 8a08 00b0 f68e 1857 2517 4e4e 4b0a 7494  .......W%.NNK.t.
+00003040: 5294 6805 288a 0800 b014 a81b d39b 174e  R.h.(..........N
+00003050: 4e4b 0a74 9452 9468 0528 8a08 00b0 14bb  NK.t.R.h.(......
+00003060: 6715 b016 4e4e 4b0a 7494 5294 6805 288a  g...NNK.t.R.h.(.
+00003070: 0800 b08e 5108 d080 164e 4e4b 0a74 9452  ....Q....NNK.t.R
+00003080: 9468 0528 8a08 00b0 856a ab29 af17 4e4e  .h.(.....j.)..NN
+00003090: 4b0a 7494 5294 6805 288a 0800 b013 66d8  K.t.R.h.(.....f.
+000030a0: 5d7a 164e 4e4b 0a74 9452 9468 0528 8a08  ]z.NNK.t.R.h.(..
+000030b0: 00b0 a347 6953 eb16 4e4e 4b0a 7494 5294  ...GiS..NNK.t.R.
+000030c0: 6805 288a 0800 b046 8888 9f6f 164e 4e4b  h.(....F...o.NNK
+000030d0: 0a74 9452 9468 0528 8a08 00b0 b89f a7ad  .t.R.h.(........
+000030e0: b816 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+000030f0: b053 ff67 7652 174e 4e4b 0a74 9452 9468  .S.gvR.NNK.t.R.h
+00003100: 0528 8a08 00b0 2650 3d9b 1617 4e4e 4b0a  .(....&P=...NNK.
+00003110: 7494 5294 6805 288a 0800 b083 c08c ba43  t.R.h.(........C
+00003120: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00003130: 77ed cd2f e516 4e4e 4b0a 7494 5294 6805  w../..NNK.t.R.h.
+00003140: 288a 0800 b027 a5cc 524c 174e 4e4b 0a74  (....'..RL.NNK.t
+00003150: 9452 9468 0528 8a08 00b0 7698 3e78 af16  .R.h.(....v.>x..
+00003160: 4e4e 4b0a 7494 5294 6805 288a 0800 b008  NNK.t.R.h.(.....
+00003170: d55c 483d 174e 4e4b 0a74 9452 9468 0528  .\H=.NNK.t.R.h.(
+00003180: 8a08 00b0 31ce 6c6e 3f17 4e4e 4b0a 7494  ....1.ln?.NNK.t.
+00003190: 5294 6805 288a 0800 b06d c42d 14f2 164e  R.h.(....m.-...N
+000031a0: 4e4b 0a74 9452 9468 0528 8a08 00b0 5972  NK.t.R.h.(....Yr
+000031b0: eddc 0b17 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
+000031c0: 0800 b0cb 890c eb54 174e 4e4b 0a74 9452  .......T.NNK.t.R
+000031d0: 9468 0528 8a08 00b0 af1a 28de 4917 4e4e  .h.(......(.I.NN
+000031e0: 4b0a 7494 5294 6805 288a 0800 b009 2aec  K.t.R.h.(.....*.
+000031f0: ff72 174e 4e4b 0a74 9452 9468 0528 8a08  .r.NNK.t.R.h.(..
+00003200: 00b0 581d 5e25 d616 4e4e 4b0a 7494 5294  ..X.^%..NNK.t.R.
+00003210: 6805 288a 0800 b039 4dee 1ac7 164e 4e4b  h.(....9M....NNK
+00003220: 0a74 9452 9468 0528 8a08 00b0 ec03 9b64  .t.R.h.(.......d
+00003230: cf17 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00003240: b01b d20d c8ed 164e 4e4b 0a74 9452 9468  .......NNK.t.R.h
+00003250: 0528 8a08 00b0 16c7 635b 7e16 4e4e 4b0a  .(......c[~.NNK.
+00003260: 7494 5294 6805 288a 0800 b054 6743 709c  t.R.h.(....TgCp.
 00003270: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00003280: 7698 3e78 af16 4e4e 4b0a 7494 5294 6805  v.>x..NNK.t.R.h.
-00003290: 288a 0800 b014 bb67 15b0 164e 4e4b 0a74  (......g...NNK.t
-000032a0: 9452 9468 0528 8a08 00b0 9f91 4e9e b116  .R.h.(......N...
-000032b0: 4e4e 4b0a 7494 5294 6805 288a 0800 b03d  NNK.t.R.h.(....=
-000032c0: b477 3bb2 164e 4e4b 0a74 9452 9468 0528  .w;..NNK.t.R.h.(
-000032d0: 8a08 00b0 c88a 5ec4 b316 4e4e 4b0a 7494  ......^...NNK.t.
-000032e0: 5294 6805 288a 0800 b017 1cf3 12b4 164e  R.h.(..........N
-000032f0: 4e4b 0a74 9452 9468 0528 8a08 00b0 f183  NK.t.R.h.(......
-00003300: 6eea b516 4e4e 4b0a 7494 5294 6805 288a  n...NNK.t.R.h.(.
-00003310: 0800 b08f a697 87b6 164e 4e4b 0a74 9452  .........NNK.t.R
-00003320: 9468 0528 8a08 00b0 1a7d 7e10 b816 4e4e  .h.(.....}~...NN
-00003330: 4b0a 7494 5294 6805 288a 0800 b0b8 9fa7  K.t.R.h.(.......
-00003340: adb8 164e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00003350: 00b0 4376 8e36 ba16 4e4e 4b0a 7494 5294  ..Cv.6..NNK.t.R.
-00003360: 6805 288a 0800 b06c 6f9e 5cbc 164e 4e4b  h.(....lo.\..NNK
-00003370: 0a74 9452 9468 0528 8a08 00b0 9568 ae82  .t.R.h.(.....h..
-00003380: be16 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00003390: b0be 61be a8c0 164e 4e4b 0a74 9452 9468  ..a....NNK.t.R.h
-000033a0: 0528 8a08 00b0 e75a cece c216 4e4e 4b0a  .(.....Z....NNK.
-000033b0: 7494 5294 6805 288a 0800 b010 54de f4c4  t.R.h.(.....T...
-000033c0: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-000033d0: ae76 0792 c516 4e4e 4b0a 7494 5294 6805  .v....NNK.t.R.h.
-000033e0: 288a 0800 b039 4dee 1ac7 164e 4e4b 0a74  (....9M....NNK.t
-000033f0: 9452 9468 0528 8a08 00b0 6246 fe40 c916  .R.h.(....bF.@..
-00003400: 4e4e 4b0a 7494 5294 6805 288a 0800 b08b  NNK.t.R.h.(.....
-00003410: 3f0e 67cb 164e 4e4b 0a74 9452 9468 0528  ?.g..NNK.t.R.h.(
-00003420: 8a08 00b0 b438 1e8d cd16 4e4e 4b0a 7494  .....8....NNK.t.
-00003430: 5294 6805 288a 0800 b0dd 312e b3cf 164e  R.h.(.....1....N
-00003440: 4e4b 0a74 9452 9468 0528 8a08 00b0 062b  NK.t.R.h.(.....+
-00003450: 3ed9 d116 4e4e 4b0a 7494 5294 6805 288a  >...NNK.t.R.h.(.
-00003460: 0800 b02f 244e ffd3 164e 4e4b 0a74 9452  .../$N...NNK.t.R
-00003470: 9468 0528 8a08 00b0 581d 5e25 d616 4e4e  .h.(....X.^%..NN
-00003480: 4b0a 7494 5294 6805 288a 0800 b032 85d9  K.t.R.h.(....2..
-00003490: fcd7 164e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-000034a0: 00b0 aa0f 7e71 da16 4e4e 4b0a 7494 5294  ....~q..NNK.t.R.
-000034b0: 6805 288a 0800 b0d3 088e 97dc 164e 4e4b  h.(..........NNK
-000034c0: 0a74 9452 9468 0528 8a08 00b0 fc01 9ebd  .t.R.h.(........
-000034d0: de16 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-000034e0: b025 fbad e3e0 164e 4e4b 0a74 9452 9468  .%.....NNK.t.R.h
-000034f0: 0528 8a08 00b0 4ef4 bd09 e316 4e4e 4b0a  .(....N.....NNK.
-00003500: 7494 5294 6805 288a 0800 b077 edcd 2fe5  t.R.h.(....w../.
+00003280: b58d ad44 0317 4e4e 4b0a 7494 5294 6805  ...D..NNK.t.R.h.
+00003290: 288a 0800 b051 f36b 3084 174e 4e4b 0a74  (....Q.k0..NNK.t
+000032a0: 9452 9468 0528 8a08 00b0 4675 3c5d 5b17  .R.h.(....Fu<][.
+000032b0: 4e4e 4b0a 7494 5294 6805 288a 0800 b007  NNK.t.R.h.(.....
+000032c0: 80cd 9007 174e 4e4b 0a74 9452 9468 0528  .....NNK.t.R.h.(
+000032d0: 8a08 00b0 d607 3cbe 7d17 4e4e 4b0a 7494  ......<.}.NNK.t.
+000032e0: 5294 6805 288a 0800 b01e d1bb ee8e 174e  R.h.(..........N
+000032f0: 4e4b 0a74 9452 9468 0528 8a08 00b0 c160  NK.t.R.h.(.....`
+00003300: 6ccf 6117 4e4e 4b0a 7494 5294 6805 288a  l.a.NNK.t.R.h.(.
+00003310: 0800 b015 fdaa 8ad1 174e 4e4b 0a74 9452  .........NNK.t.R
+00003320: 9468 0528 8a08 00b0 7842 5de7 1a17 4e4e  .h.(....xB]...NN
+00003330: 4b0a 7494 5294 6805 288a 0800 b012 fefc  K.t.R.h.(.......
+00003340: 6330 174e 4e4b 0a74 9452 9468 0528 8a08  c0.NNK.t.R.h.(..
+00003350: 00b0 b6e2 3cfc 3817 4e4e 4b0a 7494 5294  ....<.8.NNK.t.R.
+00003360: 6805 288a 0800 b01e e407 31a3 164e 4e4b  h.(.......1..NNK
+00003370: 0a74 9452 9468 0528 8a08 00b0 c2c8 47c9  .t.R.h.(......G.
+00003380: ab16 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00003390: b0e0 4328 1c85 164e 4e4b 0a74 9452 9468  ..C(...NNK.t.R.h
+000033a0: 0528 8a08 00b0 4376 8e36 ba16 4e4e 4b0a  .(....Cv.6..NNK.
+000033b0: 7494 5294 6805 288a 0800 b0f3 2d8d 5921  t.R.h.(.....-.Y!
+000033c0: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+000033d0: ea6c c837 7816 4e4e 4b0a 7494 5294 6805  .l.7x.NNK.t.R.h.
+000033e0: 288a 0800 b0d4 5d1d 4f12 174e 4e4b 0a74  (.....].O..NNK.t
+000033f0: 9452 9468 0528 8a08 00b0 7324 6738 9717  .R.h.(....s$g8..
+00003400: 4e4e 4b0a 7494 5294 6805 288a 0800 b064  NNK.t.R.h.(....d
+00003410: f01c b034 174e 4e4b 0a74 9452 9468 0528  ...4.NNK.t.R.h.(
+00003420: 8a08 00b0 3c4c 9c41 6817 4e4e 4b0a 7494  ....<L.Ah.NNK.t.
+00003430: 5294 6805 288a 0800 b0ea 597c f563 174e  R.h.(.....Y|.c.N
+00003440: 4e4b 0a74 9452 9468 0528 8a08 00b0 a2a3  NK.t.R.h.(......
+00003450: 4807 6716 4e4e 4b0a 7494 5294 6805 288a  H.g.NNK.t.R.h.(.
+00003460: 0800 b011 a96d acfa 164e 4e4b 0a74 9452  .....m...NNK.t.R
+00003470: 9468 0528 8a08 00b0 fc01 9ebd de16 4e4e  .h.(..........NN
+00003480: 4b0a 7494 5294 6805 288a 0800 b0d5 c5f8  K.t.R.h.(.......
+00003490: 485c 164e 4e4b 0a74 9452 9468 0528 8a08  H\.NNK.t.R.h.(..
+000034a0: 00b0 ebc1 57ef ad16 4e4e 4b0a 7494 5294  ....W...NNK.t.R.
+000034b0: 6805 288a 0800 b0f4 821c 1157 174e 4e4b  h.(........W.NNK
+000034c0: 0a74 9452 9468 0528 8a08 00b0 7997 ec9e  .t.R.h.(....y...
+000034d0: 5017 4e4e 4b0a 7494 5294 6805 288a 0800  P.NNK.t.R.h.(...
+000034e0: b050 b128 bb62 164e 4e4b 0a74 9452 9468  .P.(.b.NNK.t.R.h
+000034f0: 0528 8a08 00b0 f183 6eea b516 4e4e 4b0a  .(......n...NNK.
+00003500: 7494 5294 6805 288a 0800 b0bf b64d 60f6  t.R.h.(......M`.
 00003510: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00003520: a0e6 dd55 e716 4e4e 4b0a 7494 5294 6805  ...U..NNK.t.R.h.
-00003530: 288a 0800 b0c9 dfed 7be9 164e 4e4b 0a74  (.......{..NNK.t
-00003540: 9452 9468 0528 8a08 00b0 a347 6953 eb16  .R.h.(.....GiS..
-00003550: 4e4e 4b0a 7494 5294 6805 288a 0800 b01b  NNK.t.R.h.(.....
-00003560: d20d c8ed 164e 4e4b 0a74 9452 9468 0528  .....NNK.t.R.h.(
-00003570: 8a08 00b0 44cb 1dee ef16 4e4e 4b0a 7494  ....D.....NNK.t.
-00003580: 5294 6805 288a 0800 b06d c42d 14f2 164e  R.h.(....m.-...N
-00003590: 4e4b 0a74 9452 9468 0528 8a08 00b0 96bd  NK.t.R.h.(......
-000035a0: 3d3a f416 4e4e 4b0a 7494 5294 6805 288a  =:..NNK.t.R.h.(.
-000035b0: 0800 b0bf b64d 60f6 164e 4e4b 0a74 9452  .....M`..NNK.t.R
-000035c0: 9468 0528 8a08 00b0 e8af 5d86 f816 4e4e  .h.(......]...NN
-000035d0: 4b0a 7494 5294 6805 288a 0800 b011 a96d  K.t.R.h.(......m
-000035e0: acfa 164e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-000035f0: 00b0 3aa2 7dd2 fc16 4e4e 4b0a 7494 5294  ..:.}...NNK.t.R.
-00003600: 6805 288a 0800 b063 9b8d f8fe 164e 4e4b  h.(....c.....NNK
-00003610: 0a74 9452 9468 0528 8a08 00b0 8c94 9d1e  .t.R.h.(........
-00003620: 0117 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00003630: b0b5 8dad 4403 174e 4e4b 0a74 9452 9468  ....D..NNK.t.R.h
-00003640: 0528 8a08 00b0 de86 bd6a 0517 4e4e 4b0a  .(.......j..NNK.
-00003650: 7494 5294 6805 288a 0800 b007 80cd 9007  t.R.h.(.........
-00003660: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00003670: e1e7 4868 0917 4e4e 4b0a 7494 5294 6805  ..Hh..NNK.t.R.h.
-00003680: 288a 0800 b059 72ed dc0b 174e 4e4b 0a74  (....Yr....NNK.t
-00003690: 9452 9468 0528 8a08 00b0 826b fd02 0e17  .R.h.(.....k....
-000036a0: 4e4e 4b0a 7494 5294 6805 288a 0800 b0ab  NNK.t.R.h.(.....
-000036b0: 640d 2910 174e 4e4b 0a74 9452 9468 0528  d.)..NNK.t.R.h.(
-000036c0: 8a08 00b0 d45d 1d4f 1217 4e4e 4b0a 7494  .....].O..NNK.t.
-000036d0: 5294 6805 288a 0800 b0fd 562d 7514 174e  R.h.(.....V-u..N
-000036e0: 4e4b 0a74 9452 9468 0528 8a08 00b0 2650  NK.t.R.h.(....&P
-000036f0: 3d9b 1617 4e4e 4b0a 7494 5294 6805 288a  =...NNK.t.R.h.(.
-00003700: 0800 b04f 494d c118 174e 4e4b 0a74 9452  ...OIM...NNK.t.R
-00003710: 9468 0528 8a08 00b0 7842 5de7 1a17 4e4e  .h.(....xB]...NN
-00003720: 4b0a 7494 5294 6805 288a 0800 b0a1 3b6d  K.t.R.h.(.....;m
-00003730: 0d1d 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00003740: 00b0 ca34 7d33 1f17 4e4e 4b0a 7494 5294  ...4}3..NNK.t.R.
-00003750: 6805 288a 0800 b0f3 2d8d 5921 174e 4e4b  h.(.....-.Y!.NNK
-00003760: 0a74 9452 9468 0528 8a08 00b0 1c27 9d7f  .t.R.h.(.....'..
-00003770: 2317 4e4e 4b0a 7494 5294 6805 288a 0800  #.NNK.t.R.h.(...
-00003780: b0f6 8e18 5725 174e 4e4b 0a74 9452 9468  ....W%.NNK.t.R.h
-00003790: 0528 8a08 00b0 6e19 bdcb 2717 4e4e 4b0a  .(....n...'.NNK.
-000037a0: 7494 5294 6805 288a 0800 b097 12cd f129  t.R.h.(........)
+00003520: 3db4 773b b216 4e4e 4b0a 7494 5294 6805  =.w;..NNK.t.R.h.
+00003530: 288a 0800 b0a4 3a1b 34be 174e 4e4b 0a74  (.....:.4..NNK.t
+00003540: 9452 9468 0528 8a08 00b0 3da1 2bf9 9d17  .R.h.(....=.+...
+00003550: 4e4e 4b0a 7494 5294 6805 288a 0800 b0b7  NNK.t.R.h.(.....
+00003560: 37cc b36e 174e 4e4b 0a74 9452 9468 0528  7..n.NNK.t.R.h.(
+00003570: 8a08 00b0 5b2f 588e 8b16 4e4e 4b0a 7494  ....[/X...NNK.t.
+00003580: 5294 6805 288a 0800 b009 3d38 4287 164e  R.h.(.....=8B..N
+00003590: 4e4b 0a74 9452 9468 0528 8a08 00b0 5c71  NK.t.R.h.(....\q
+000035a0: 9b03 ad17 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
+000035b0: 0800 b0f6 2c3b 80c2 174e 4e4b 0a74 9452  ....,;...NNK.t.R
+000035c0: 9468 0528 8a08 00b0 c173 b811 7616 4e4e  .h.(.....s..v.NN
+000035d0: 4b0a 7494 5294 6805 288a 0800 b09f 914e  K.t.R.h.(......N
+000035e0: 9eb1 164e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+000035f0: 00b0 ad21 78da 8f16 4e4e 4b0a 7494 5294  ...!x...NNK.t.R.
+00003600: 6805 288a 0800 b0ae 7607 92c5 164e 4e4b  h.(.....v....NNK
+00003610: 0a74 9452 9468 0528 8a08 00b0 062b 3ed9  .t.R.h.(.....+>.
+00003620: d116 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00003630: b08e 3ebc 8d6c 174e 4e4b 0a74 9452 9468  ..>..l.NNK.t.R.h
+00003640: 0528 8a08 00b0 7118 6bf2 c817 4e4e 4b0a  .(....q.k...NNK.
+00003650: 7494 5294 6805 288a 0800 b0cb 9c58 2d69  t.R.h.(......X-i
+00003660: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00003670: 3ef6 bab0 d317 4e4e 4b0a 7494 5294 6805  >.....NNK.t.R.h.
+00003680: 288a 0800 b028 0da8 4c96 164e 4e4b 0a74  (....(..L..NNK.t
+00003690: 9452 9468 0528 8a08 00b0 8c94 9d1e 0117  .R.h.(..........
+000036a0: 4e4e 4b0a 7494 5294 6805 288a 0800 b0c3  NNK.t.R.h.(.....
+000036b0: 0a8b 3ecd 174e 4e4b 0a74 9452 9468 0528  ..>..NNK.t.R.h.(
+000036c0: 8a08 00b0 27b8 1895 6016 4e4e 4b0a 7494  ....'...`.NNK.t.
+000036d0: 5294 6805 288a 0800 b044 cb1d eeef 164e  R.h.(....D.....N
+000036e0: 4e4b 0a74 9452 9468 0528 8a08 00b0 509e  NK.t.R.h.(....P.
+000036f0: dc78 4e17 4e4e 4b0a 7494 5294 6805 288a  .xN.NNK.t.R.h.(.
+00003700: 0800 b0a5 04d4 046b 164e 4e4b 0a74 9452  .......k.NNK.t.R
+00003710: 9468 0528 8a08 00b0 ca34 7d33 1f17 4e4e  .h.(.....4}3..NN
+00003720: 4b0a 7494 5294 6805 288a 0800 b0e9 04ed  K.t.R.h.(.......
+00003730: 3d2e 174e 4e4b 0a74 9452 9468 0528 8a08  =..NNK.t.R.h.(..
+00003740: 00b0 25fb ade3 e016 4e4e 4b0a 7494 5294  ..%.....NNK.t.R.
+00003750: 6805 288a 0800 b032 23fc 2575 174e 4e4b  h.(....2#.%u.NNK
+00003760: 0a74 9452 9468 0528 8a08 00b0 669a 3b1f  .t.R.h.(....f.;.
+00003770: a017 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00003780: b06e 19bd cb27 174e 4e4b 0a74 9452 9468  .n...'.NNK.t.R.h
+00003790: 0528 8a08 00b0 acb9 9ce0 4517 4e4e 4b0a  .(........E.NNK.
+000037a0: 7494 5294 6805 288a 0800 b0cc de9b a28a  t.R.h.(.........
 000037b0: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-000037c0: c00b dd17 2c17 4e4e 4b0a 7494 5294 6805  ....,.NNK.t.R.h.
-000037d0: 288a 0800 b0e9 04ed 3d2e 174e 4e4b 0a74  (.......=..NNK.t
-000037e0: 9452 9468 0528 8a08 00b0 12fe fc63 3017  .R.h.(.......c0.
-000037f0: 4e4e 4b0a 7494 5294 6805 288a 0800 b03b  NNK.t.R.h.(....;
-00003800: f70c 8a32 174e 4e4b 0a74 9452 9468 0528  ...2.NNK.t.R.h.(
-00003810: 8a08 00b0 64f0 1cb0 3417 4e4e 4b0a 7494  ....d...4.NNK.t.
-00003820: 5294 6805 288a 0800 b08d e92c d636 174e  R.h.(......,.6.N
-00003830: 4e4b 0a74 9452 9468 0528 8a08 00b0 b6e2  NK.t.R.h.(......
-00003840: 3cfc 3817 4e4e 4b0a 7494 5294 6805 288a  <.8.NNK.t.R.h.(.
-00003850: 0800 b0df db4c 223b 174e 4e4b 0a74 9452  .....L";.NNK.t.R
-00003860: 9468 0528 8a08 00b0 08d5 5c48 3d17 4e4e  .h.(......\H=.NN
-00003870: 4b0a 7494 5294 6805 288a 0800 b031 ce6c  K.t.R.h.(....1.l
-00003880: 6e3f 174e 4e4b 0a74 9452 9468 0528 8a08  n?.NNK.t.R.h.(..
-00003890: 00b0 5ac7 7c94 4117 4e4e 4b0a 7494 5294  ..Z.|.A.NNK.t.R.
-000038a0: 6805 288a 0800 b083 c08c ba43 174e 4e4b  h.(........C.NNK
-000038b0: 0a74 9452 9468 0528 8a08 00b0 acb9 9ce0  .t.R.h.(........
-000038c0: 4517 4e4e 4b0a 7494 5294 6805 288a 0800  E.NNK.t.R.h.(...
-000038d0: b0d5 b2ac 0648 174e 4e4b 0a74 9452 9468  .....H.NNK.t.R.h
-000038e0: 0528 8a08 00b0 af1a 28de 4917 4e4e 4b0a  .(......(.I.NNK.
-000038f0: 7494 5294 6805 288a 0800 b027 a5cc 524c  t.R.h.(....'..RL
+000037c0: 9712 cdf1 2917 4e4e 4b0a 7494 5294 6805  ....).NNK.t.R.h.
+000037d0: 288a 0800 b0dd 312e b3cf 164e 4e4b 0a74  (.....1....NNK.t
+000037e0: 9452 9468 0528 8a08 00b0 9a11 7b18 cb17  .R.h.(......{...
+000037f0: 4e4e 4b0a 7494 5294 6805 288a 0800 b0d3  NNK.t.R.h.(.....
+00003800: 088e 97dc 164e 4e4b 0a74 9452 9468 0528  .....NNK.t.R.h.(
+00003810: 8a08 00b0 accc e822 5a16 4e4e 4b0a 7494  ......."Z.NNK.t.
+00003820: 5294 6805 288a 0800 b07a ffc7 989a 164e  R.h.(....z.....N
+00003830: 4e4b 0a74 9452 9468 0528 8a08 00b0 7b41  NK.t.R.h.(....{A
+00003840: 0b0e bc17 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
+00003850: 0800 b047 dd17 57a5 164e 4e4b 0a74 9452  ...G..W..NNK.t.R
+00003860: 9468 0528 8a08 00b0 1d8f 7879 6d16 4e4e  .h.(......xym.NN
+00003870: 4b0a 7494 5294 6805 288a 0800 b0a1 3b6d  K.t.R.h.(.....;m
+00003880: 0d1d 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+00003890: 00b0 9568 ae82 be16 4e4e 4b0a 7494 5294  ...h....NNK.t.R.
+000038a0: 6805 288a 0800 b033 788b ddaa 174e 4e4b  h.(....3x....NNK
+000038b0: 0a74 9452 9468 0528 8a08 00b0 6f81 98c5  .t.R.h.(....o...
+000038c0: 7116 4e4e 4b0a 7494 5294 6805 288a 0800  q.NNK.t.R.h.(...
+000038d0: b0e7 5ace cec2 164e 4e4b 0a74 9452 9468  ..Z....NNK.t.R.h
+000038e0: 0528 8a08 00b0 826b fd02 0e17 4e4e 4b0a  .(.....k....NNK.
+000038f0: 7494 5294 6805 288a 0800 b0d5 b2ac 0648  t.R.h.(........H
 00003900: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00003910: 509e dc78 4e17 4e4e 4b0a 7494 5294 6805  P..xN.NNK.t.R.h.
-00003920: 288a 0800 b079 97ec 9e50 174e 4e4b 0a74  (....y...P.NNK.t
-00003930: 9452 9468 0528 8a08 00b0 53ff 6776 5217  .R.h.(....S.gvR.
-00003940: 4e4e 4b0a 7494 5294 6805 288a 0800 b0cb  NNK.t.R.h.(.....
-00003950: 890c eb54 174e 4e4b 0a74 9452 9468 0528  ...T.NNK.t.R.h.(
-00003960: 8a08 00b0 f482 1c11 5717 4e4e 4b0a 7494  ........W.NNK.t.
-00003970: 5294 6805 288a 0800 b01d 7c2c 3759 174e  R.h.(.....|,7Y.N
-00003980: 4e4b 0a74 9452 9468 0528 8a08 00b0 4675  NK.t.R.h.(....Fu
-00003990: 3c5d 5b17 4e4e 4b0a 7494 5294 6805 288a  <][.NNK.t.R.h.(.
+00003910: 2b5b e707 8617 4e4e 4b0a 7494 5294 6805  +[....NNK.t.R.h.
+00003920: 288a 0800 b0c9 dfed 7be9 164e 4e4b 0a74  (.......{..NNK.t
+00003930: 9452 9468 0528 8a08 00b0 96bd 3d3a f416  .R.h.(......=:..
+00003940: 4e4e 4b0a 7494 5294 6805 288a 0800 b084  NNK.t.R.h.(.....
+00003950: 2868 b48d 164e 4e4b 0a74 9452 9468 0528  (h...NNK.t.R.h.(
+00003960: 8a08 00b0 be61 bea8 c016 4e4e 4b0a 7494  .....a....NNK.t.
+00003970: 5294 6805 288a 0800 b051 06b8 7298 164e  R.h.(....Q..r..N
+00003980: 4e4b 0a74 9452 9468 0528 8a08 00b0 5ac7  NK.t.R.h.(....Z.
+00003990: 7c94 4117 4e4e 4b0a 7494 5294 6805 288a  |.A.NNK.t.R.h.(.
 000039a0: 0800 b06f 6e4c 835d 174e 4e4b 0a74 9452  ...onL.].NNK.t.R
 000039b0: 9468 0528 8a08 00b0 9867 5ca9 5f17 4e4e  .h.(.....g\._.NN
-000039c0: 4b0a 7494 5294 6805 288a 0800 b0c1 606c  K.t.R.h.(.....`l
-000039d0: cf61 174e 4e4b 0a74 9452 9468 0528 8a08  .a.NNK.t.R.h.(..
-000039e0: 00b0 ea59 7cf5 6317 4e4e 4b0a 7494 5294  ...Y|.c.NNK.t.R.
-000039f0: 6805 288a 0800 b013 538c 1b66 174e 4e4b  h.(.....S..f.NNK
-00003a00: 0a74 9452 9468 0528 8a08 00b0 3c4c 9c41  .t.R.h.(....<L.A
-00003a10: 6817 4e4e 4b0a 7494 5294 6805 288a 0800  h.NNK.t.R.h.(...
-00003a20: b065 45ac 676a 174e 4e4b 0a74 9452 9468  .eE.gj.NNK.t.R.h
-00003a30: 0528 8a08 00b0 8e3e bc8d 6c17 4e4e 4b0a  .(.....>..l.NNK.
-00003a40: 7494 5294 6805 288a 0800 b0b7 37cc b36e  t.R.h.(.....7..n
+000039c0: 4b0a 7494 5294 6805 288a 0800 b0e1 856b  K.t.R.h.(......k
+000039d0: 91a6 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+000039e0: 00b0 1a7d 7e10 b816 4e4e 4b0a 7494 5294  ...}~...NNK.t.R.
+000039f0: 6805 288a 0800 b0eb ae0b ad99 174e 4e4b  h.(..........NNK
+00003a00: 0a74 9452 9468 0528 8a08 00b0 ae63 bb4f  .t.R.h.(.....c.O
+00003a10: b117 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00003a20: b0a3 e58b 7c88 174e 4e4b 0a74 9452 9468  ....|..NNK.t.R.h
+00003a30: 0528 8a08 00b0 3aa2 7dd2 fc16 4e4e 4b0a  .(....:.}...NNK.
+00003a40: 7494 5294 6805 288a 0800 b0cd 332b 5ac0  t.R.h.(.....3+Z.
 00003a50: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00003a60: e030 dcd9 7017 4e4e 4b0a 7494 5294 6805  .0..p.NNK.t.R.h.
-00003a70: 288a 0800 b009 2aec ff72 174e 4e4b 0a74  (.....*..r.NNK.t
-00003a80: 9452 9468 0528 8a08 00b0 3223 fc25 7517  .R.h.(....2#.%u.
-00003a90: 4e4e 4b0a 7494 5294 6805 288a 0800 b05b  NNK.t.R.h.(....[
-00003aa0: 1c0c 4c77 174e 4e4b 0a74 9452 9468 0528  ..Lw.NNK.t.R.h.(
-00003ab0: 8a08 00b0 8415 1c72 7917 4e4e 4b0a 7494  .......ry.NNK.t.
-00003ac0: 5294 6805 288a 0800 b05e 7d97 497b 174e  R.h.(....^}.I{.N
-00003ad0: 4e4b 0a74 9452 9468 0528 8a08 00b0 d607  NK.t.R.h.(......
-00003ae0: 3cbe 7d17 4e4e 4b0a 7494 5294 6805 288a  <.}.NNK.t.R.h.(.
-00003af0: 0800 b0ff 004c e47f 174e 4e4b 0a74 9452  .....L...NNK.t.R
-00003b00: 9468 0528 8a08 00b0 28fa 5b0a 8217 4e4e  .h.(....(.[...NN
-00003b10: 4b0a 7494 5294 6805 288a 0800 b051 f36b  K.t.R.h.(....Q.k
-00003b20: 3084 174e 4e4b 0a74 9452 9468 0528 8a08  0..NNK.t.R.h.(..
-00003b30: 00b0 2b5b e707 8617 4e4e 4b0a 7494 5294  ..+[....NNK.t.R.
-00003b40: 6805 288a 0800 b0a3 e58b 7c88 174e 4e4b  h.(.......|..NNK
-00003b50: 0a74 9452 9468 0528 8a08 00b0 ccde 9ba2  .t.R.h.(........
-00003b60: 8a17 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00003b70: b0f5 d7ab c88c 174e 4e4b 0a74 9452 9468  .......NNK.t.R.h
-00003b80: 0528 8a08 00b0 1ed1 bbee 8e17 4e4e 4b0a  .(..........NNK.
-00003b90: 7494 5294 6805 288a 0800 b0f8 3837 c690  t.R.h.(.....87..
-00003ba0: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00003bb0: 70c3 db3a 9317 4e4e 4b0a 7494 5294 6805  p..:..NNK.t.R.h.
-00003bc0: 288a 0800 b099 bceb 6095 174e 4e4b 0a74  (.......`..NNK.t
-00003bd0: 9452 9468 0528 8a08 00b0 7324 6738 9717  .R.h.(....s$g8..
-00003be0: 4e4e 4b0a 7494 5294 6805 288a 0800 b0eb  NNK.t.R.h.(.....
-00003bf0: ae0b ad99 174e 4e4b 0a74 9452 9468 0528  .....NNK.t.R.h.(
-00003c00: 8a08 00b0 14a8 1bd3 9b17 4e4e 4b0a 7494  ..........NNK.t.
-00003c10: 5294 6805 288a 0800 b03d a12b f99d 174e  R.h.(....=.+...N
-00003c20: 4e4b 0a74 9452 9468 0528 8a08 00b0 669a  NK.t.R.h.(....f.
-00003c30: 3b1f a017 4e4e 4b0a 7494 5294 6805 288a  ;...NNK.t.R.h.(.
-00003c40: 0800 b08f 934b 45a2 174e 4e4b 0a74 9452  .....KE..NNK.t.R
-00003c50: 9468 0528 8a08 00b0 b88c 5b6b a417 4e4e  .h.(......[k..NN
-00003c60: 4b0a 7494 5294 6805 288a 0800 b0e1 856b  K.t.R.h.(......k
-00003c70: 91a6 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00003c80: 00b0 0a7f 7bb7 a817 4e4e 4b0a 7494 5294  ....{...NNK.t.R.
-00003c90: 6805 288a 0800 b033 788b ddaa 174e 4e4b  h.(....3x....NNK
-00003ca0: 0a74 9452 9468 0528 8a08 00b0 5c71 9b03  .t.R.h.(....\q..
-00003cb0: ad17 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00003cc0: b085 6aab 29af 174e 4e4b 0a74 9452 9468  ..j.)..NNK.t.R.h
-00003cd0: 0528 8a08 00b0 ae63 bb4f b117 4e4e 4b0a  .(.....c.O..NNK.
-00003ce0: 7494 5294 6805 288a 0800 b0d7 5ccb 75b3  t.R.h.(.....\.u.
+00003a60: 6c6f 9e5c bc16 4e4e 4b0a 7494 5294 6805  lo.\..NNK.t.R.h.
+00003a70: 288a 0800 b063 9b8d f8fe 164e 4e4b 0a74  (....c.....NNK.t
+00003a80: 9452 9468 0528 8a08 00b0 2f24 4eff d316  .R.h.(..../$N...
+00003a90: 4e4e 4b0a 7494 5294 6805 288a 0800 b03b  NNK.t.R.h.(....;
+00003aa0: f70c 8a32 174e 4e4b 0a74 9452 9468 0528  ...2.NNK.t.R.h.(
+00003ab0: 8a08 00b0 6246 fe40 c916 4e4e 4b0a 7494  ....bF.@..NNK.t.
+00003ac0: 5294 6805 288a 0800 b070 d627 7da7 164e  R.h.(....p.'}..N
+00003ad0: 4e4b 0a74 9452 9468 0528 8a08 00b0 987a  NK.t.R.h.(.....z
+00003ae0: a8eb 7316 4e4e 4b0a 7494 5294 6805 288a  ..s.NNK.t.R.h.(.
+00003af0: 0800 b0d6 1a88 0092 164e 4e4b 0a74 9452  .........NNK.t.R
+00003b00: 9468 0528 8a08 00b0 5b1c 0c4c 7717 4e4e  .h.(....[..Lw.NN
+00003b10: 4b0a 7494 5294 6805 288a 0800 b0f5 d7ab  K.t.R.h.(.......
+00003b20: c88c 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+00003b30: 00b0 5248 fbe7 b917 4e4e 4b0a 7494 5294  ..RH....NNK.t.R.
+00003b40: 6805 288a 0800 b05e 7d97 497b 174e 4e4b  h.(....^}.I{.NNK
+00003b50: 0a74 9452 9468 0528 8a08 00b0 28fa 5b0a  .t.R.h.(....(.[.
+00003b60: 8217 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00003b70: b08f a697 87b6 164e 4e4b 0a74 9452 9468  .......NNK.t.R.h
+00003b80: 0528 8a08 00b0 1353 8c1b 6617 4e4e 4b0a  .(.....S..f.NNK.
+00003b90: 7494 5294 6805 288a 0800 b0fe be08 6f5e  t.R.h.(.......o^
+00003ba0: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00003bb0: 79aa 38e1 6416 4e4e 4b0a 7494 5294 6805  y.8.d.NNK.t.R.h.
+00003bc0: 288a 0800 b010 54de f4c4 164e 4e4b 0a74  (.....T....NNK.t
+00003bd0: 9452 9468 0528 8a08 00b0 4f49 4dc1 1817  .R.h.(....OIM...
+00003be0: 4e4e 4b0a 7494 5294 6805 288a 0800 b0df  NNK.t.R.h.(.....
+00003bf0: db4c 223b 174e 4e4b 0a74 9452 9468 0528  .L";.NNK.t.R.h.(
+00003c00: 8a08 00b0 1f26 4ba6 c417 4e4e 4b0a 7494  .....&K...NNK.t.
+00003c10: 5294 6805 288a 0800 b0e1 e748 6809 174e  R.h.(......Hh..N
+00003c20: 4e4b 0a74 9452 9468 0528 8a08 00b0 294f  NK.t.R.h.(....)O
+00003c30: ebc1 b717 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
+00003c40: 0800 b00a 7f7b b7a8 174e 4e4b 0a74 9452  .....{...NNK.t.R
+00003c50: 9468 0528 8a08 00b0 3c5f e883 7c16 4e4e  .h.(....<_..|.NN
+00003c60: 4b0a 7494 5294 6805 288a 0800 b08f 934b  K.t.R.h.(......K
+00003c70: 45a2 174e 4e4b 0a74 9452 9468 0528 8a08  E..NNK.t.R.h.(..
+00003c80: 00b0 fd56 2d75 1417 4e4e 4b0a 7494 5294  ...V-u..NNK.t.R.
+00003c90: 6805 288a 0800 b08d e92c d636 174e 4e4b  h.(......,.6.NNK
+00003ca0: 0a74 9452 9468 0528 8a08 00b0 4ef4 bd09  .t.R.h.(....N...
+00003cb0: e316 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00003cc0: b0e8 af5d 86f8 164e 4e4b 0a74 9452 9468  ...]...NNK.t.R.h
+00003cd0: 0528 8a08 00b0 481f 5bcc c617 4e4e 4b0a  .(....H.[...NNK.
+00003ce0: 7494 5294 6805 288a 0800 b0f8 3837 c690  t.R.h.(.....87..
 00003cf0: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00003d00: 0056 db9b b517 4e4e 4b0a 7494 5294 6805  .V....NNK.t.R.h.
-00003d10: 288a 0800 b029 4feb c1b7 174e 4e4b 0a74  (....)O....NNK.t
-00003d20: 9452 9468 0528 8a08 00b0 5248 fbe7 b917  .R.h.(....RH....
-00003d30: 4e4e 4b0a 7494 5294 6805 288a 0800 b07b  NNK.t.R.h.(....{
-00003d40: 410b 0ebc 174e 4e4b 0a74 9452 9468 0528  A....NNK.t.R.h.(
-00003d50: 8a08 00b0 a43a 1b34 be17 4e4e 4b0a 7494  .....:.4..NNK.t.
-00003d60: 5294 6805 288a 0800 b0cd 332b 5ac0 174e  R.h.(.....3+Z..N
-00003d70: 4e4b 0a74 9452 9468 0528 8a08 00b0 f62c  NK.t.R.h.(.....,
-00003d80: 3b80 c217 4e4e 4b0a 7494 5294 6805 288a  ;...NNK.t.R.h.(.
-00003d90: 0800 b01f 264b a6c4 174e 4e4b 0a74 9452  ....&K...NNK.t.R
-00003da0: 9468 0528 8a08 00b0 481f 5bcc c617 4e4e  .h.(....H.[...NN
-00003db0: 4b0a 7494 5294 6805 288a 0800 b071 186b  K.t.R.h.(....q.k
-00003dc0: f2c8 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00003dd0: 00b0 9a11 7b18 cb17 4e4e 4b0a 7494 5294  ....{...NNK.t.R.
-00003de0: 6805 288a 0800 b0c3 0a8b 3ecd 174e 4e4b  h.(.......>..NNK
-00003df0: 0a74 9452 9468 0528 8a08 00b0 ec03 9b64  .t.R.h.(.......d
-00003e00: cf17 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00003e10: b03e f6ba b0d3 174e 4e4b 0a74 9452 9468  .>.....NNK.t.R.h
-00003e20: 0528 8a08 00b0 e2da fa48 dc17 4e4e 4b0a  .(.......H..NNK.
-00003e30: 7494 5294 658c 0a4d 4944 4350 4e49 4654  t.R.e..MIDCPNIFT
-00003e40: 5994 5d94 2868 0528 8a08 00b0 b438 1e8d  Y.].(h.(.....8..
-00003e50: cd16 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00003e60: b0dd 312e b3cf 164e 4e4b 0a74 9452 9468  ..1....NNK.t.R.h
-00003e70: 0528 8a08 00b0 062b 3ed9 d116 4e4e 4b0a  .(.....+>...NNK.
-00003e80: 7494 5294 6805 288a 0800 b02f 244e ffd3  t.R.h.(..../$N..
-00003e90: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00003ea0: 581d 5e25 d616 4e4e 4b0a 7494 5294 6805  X.^%..NNK.t.R.h.
-00003eb0: 288a 0800 b032 85d9 fcd7 164e 4e4b 0a74  (....2.....NNK.t
-00003ec0: 9452 9468 0528 8a08 00b0 aa0f 7e71 da16  .R.h.(......~q..
-00003ed0: 4e4e 4b0a 7494 5294 6805 288a 0800 b0d3  NNK.t.R.h.(.....
-00003ee0: 088e 97dc 164e 4e4b 0a74 9452 9468 0528  .....NNK.t.R.h.(
-00003ef0: 8a08 00b0 fc01 9ebd de16 4e4e 4b0a 7494  ..........NNK.t.
-00003f00: 5294 6805 288a 0800 b025 fbad e3e0 164e  R.h.(....%.....N
-00003f10: 4e4b 0a74 9452 9468 0528 8a08 00b0 4ef4  NK.t.R.h.(....N.
-00003f20: bd09 e316 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
-00003f30: 0800 b077 edcd 2fe5 164e 4e4b 0a74 9452  ...w../..NNK.t.R
-00003f40: 9468 0528 8a08 00b0 a0e6 dd55 e716 4e4e  .h.(.......U..NN
-00003f50: 4b0a 7494 5294 6805 288a 0800 b0c9 dfed  K.t.R.h.(.......
-00003f60: 7be9 164e 4e4b 0a74 9452 9468 0528 8a08  {..NNK.t.R.h.(..
-00003f70: 00b0 a347 6953 eb16 4e4e 4b0a 7494 5294  ...GiS..NNK.t.R.
-00003f80: 6805 288a 0800 b01b d20d c8ed 164e 4e4b  h.(..........NNK
-00003f90: 0a74 9452 9468 0528 8a08 00b0 44cb 1dee  .t.R.h.(....D...
-00003fa0: ef16 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00003fb0: b06d c42d 14f2 164e 4e4b 0a74 9452 9468  .m.-...NNK.t.R.h
-00003fc0: 0528 8a08 00b0 96bd 3d3a f416 4e4e 4b0a  .(......=:..NNK.
-00003fd0: 7494 5294 6805 288a 0800 b0bf b64d 60f6  t.R.h.(......M`.
-00003fe0: 164e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00003ff0: e8af 5d86 f816 4e4e 4b0a 7494 5294 6805  ..]...NNK.t.R.h.
-00004000: 288a 0800 b011 a96d acfa 164e 4e4b 0a74  (......m...NNK.t
-00004010: 9452 9468 0528 8a08 00b0 3aa2 7dd2 fc16  .R.h.(....:.}...
-00004020: 4e4e 4b0a 7494 5294 6805 288a 0800 b063  NNK.t.R.h.(....c
-00004030: 9b8d f8fe 164e 4e4b 0a74 9452 9468 0528  .....NNK.t.R.h.(
-00004040: 8a08 00b0 8c94 9d1e 0117 4e4e 4b0a 7494  ..........NNK.t.
-00004050: 5294 6805 288a 0800 b0b5 8dad 4403 174e  R.h.(.......D..N
-00004060: 4e4b 0a74 9452 9468 0528 8a08 00b0 de86  NK.t.R.h.(......
-00004070: bd6a 0517 4e4e 4b0a 7494 5294 6805 288a  .j..NNK.t.R.h.(.
-00004080: 0800 b007 80cd 9007 174e 4e4b 0a74 9452  .........NNK.t.R
-00004090: 9468 0528 8a08 00b0 e1e7 4868 0917 4e4e  .h.(......Hh..NN
-000040a0: 4b0a 7494 5294 6805 288a 0800 b059 72ed  K.t.R.h.(....Yr.
-000040b0: dc0b 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-000040c0: 00b0 826b fd02 0e17 4e4e 4b0a 7494 5294  ...k....NNK.t.R.
-000040d0: 6805 288a 0800 b0ab 640d 2910 174e 4e4b  h.(.....d.)..NNK
-000040e0: 0a74 9452 9468 0528 8a08 00b0 d45d 1d4f  .t.R.h.(.....].O
-000040f0: 1217 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00004100: b0fd 562d 7514 174e 4e4b 0a74 9452 9468  ..V-u..NNK.t.R.h
-00004110: 0528 8a08 00b0 2650 3d9b 1617 4e4e 4b0a  .(....&P=...NNK.
-00004120: 7494 5294 6805 288a 0800 b04f 494d c118  t.R.h.(....OIM..
+00003d00: ccf1 e7e4 9e16 4e4e 4b0a 7494 5294 6805  ......NNK.t.R.h.
+00003d10: 288a 0800 b099 cf37 a3a9 164e 4e4b 0a74  (......7...NNK.t
+00003d20: 9452 9468 0528 8a08 00b0 a0e6 dd55 e716  .R.h.(.......U..
+00003d30: 4e4e 4b0a 7494 5294 6805 288a 0800 b017  NNK.t.R.h.(.....
+00003d40: 1cf3 12b4 164e 4e4b 0a74 9452 9468 0528  .....NNK.t.R.h.(
+00003d50: 8a08 00b0 6545 ac67 6a17 4e4e 4b0a 7494  ....eE.gj.NNK.t.
+00003d60: 5294 6805 288a 0800 b08b 3f0e 67cb 164e  R.h.(.....?.g..N
+00003d70: 4e4b 0a74 9452 9468 0528 8a08 00b0 1c27  NK.t.R.h.(.....'
+00003d80: 9d7f 2317 4e4e 4b0a 7494 5294 6805 288a  ..#.NNK.t.R.h.(.
+00003d90: 0800 b099 bceb 6095 174e 4e4b 0a74 9452  ......`..NNK.t.R
+00003da0: 9468 0528 8a08 00b0 67ef cad6 d517 4e4e  .h.(....g.....NN
+00003db0: 4b0a 7494 5294 6805 288a 0800 b0c0 0bdd  K.t.R.h.(.......
+00003dc0: 172c 174e 4e4b 0a74 9452 9468 0528 8a08  .,.NNK.t.R.h.(..
+00003dd0: 00b0 1d7c 2c37 5917 4e4e 4b0a 7494 5294  ...|,7Y.NNK.t.R.
+00003de0: 6805 288a 0800 b084 151c 7279 174e 4e4b  h.(.......ry.NNK
+00003df0: 0a74 9452 9468 0528 8a08 00b0 ff13 9826  .t.R.h.(.......&
+00003e00: 9416 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00003e10: b0e0 30dc d970 174e 4e4b 0a74 9452 9468  ..0..p.NNK.t.R.h
+00003e20: 0528 8a08 00b0 b88c 5b6b a417 4e4e 4b0a  .(......[k..NNK.
+00003e30: 7494 5294 6805 288a 0800 b000 56db 9bb5  t.R.h.(.....V...
+00003e40: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00003e50: e2da fa48 dc17 4e4e 4b0a 7494 5294 6805  ...H..NNK.t.R.h.
+00003e60: 288a 0800 b0aa 0f7e 71da 164e 4e4b 0a74  (......~q..NNK.t
+00003e70: 9452 9468 0528 8a08 00b0 d75c cb75 b317  .R.h.(.....\.u..
+00003e80: 4e4e 4b0a 7494 5294 6805 288a 0800 b032  NNK.t.R.h.(....2
+00003e90: 3648 6889 164e 4e4b 0a74 9452 9468 0528  6Hh..NNK.t.R.h.(
+00003ea0: 8a08 00b0 ab64 0d29 1017 4e4e 4b0a 7494  .....d.)..NNK.t.
+00003eb0: 5294 658c 0a4d 4944 4350 4e49 4654 5994  R.e..MIDCPNIFTY.
+00003ec0: 5d94 2868 0528 8a08 00b0 3285 d9fc d716  ].(h.(....2.....
+00003ed0: 4e4e 4b0a 7494 5294 6805 288a 0800 b0de  NNK.t.R.h.(.....
+00003ee0: 86bd 6a05 174e 4e4b 0a74 9452 9468 0528  ..j..NNK.t.R.h.(
+00003ef0: 8a08 00b0 2599 d00c 7e17 4e4e 4b0a 7494  ....%...~.NNK.t.
+00003f00: 5294 6805 288a 0800 b0b4 381e 8dcd 164e  R.h.(.....8....N
+00003f10: 4e4b 0a74 9452 9468 0528 8a08 00b0 f68e  NK.t.R.h.(......
+00003f20: 1857 2517 4e4e 4b0a 7494 5294 6805 288a  .W%.NNK.t.R.h.(.
+00003f30: 0800 b02f c270 2871 174e 4e4b 0a74 9452  .../.p(q.NNK.t.R
+00003f40: 9468 0528 8a08 00b0 a347 6953 eb16 4e4e  .h.(.....GiS..NN
+00003f50: 4b0a 7494 5294 6805 288a 0800 b092 f4d6  K.t.R.h.(.......
+00003f60: 42a6 174e 4e4b 0a74 9452 9468 0528 8a08  B..NNK.t.R.h.(..
+00003f70: 00b0 53ff 6776 5217 4e4e 4b0a 7494 5294  ..S.gvR.NNK.t.R.
+00003f80: 6805 288a 0800 b026 503d 9b16 174e 4e4b  h.(....&P=...NNK
+00003f90: 0a74 9452 9468 0528 8a08 00b0 83c0 8cba  .t.R.h.(........
+00003fa0: 4317 4e4e 4b0a 7494 5294 6805 288a 0800  C.NNK.t.R.h.(...
+00003fb0: b077 edcd 2fe5 164e 4e4b 0a74 9452 9468  .w../..NNK.t.R.h
+00003fc0: 0528 8a08 00b0 27a5 cc52 4c17 4e4e 4b0a  .(....'..RL.NNK.
+00003fd0: 7494 5294 6805 288a 0800 b008 d55c 483d  t.R.h.(......\H=
+00003fe0: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00003ff0: 31ce 6c6e 3f17 4e4e 4b0a 7494 5294 6805  1.ln?.NNK.t.R.h.
+00004000: 288a 0800 b00d e006 b5ac 174e 4e4b 0a74  (..........NNK.t
+00004010: 9452 9468 0528 8a08 00b0 6dc4 2d14 f216  .R.h.(....m.-...
+00004020: 4e4e 4b0a 7494 5294 6805 288a 0800 b059  NNK.t.R.h.(....Y
+00004030: 72ed dc0b 174e 4e4b 0a74 9452 9468 0528  r....NNK.t.R.h.(
+00004040: 8a08 00b0 af1a 28de 4917 4e4e 4b0a 7494  ......(.I.NNK.t.
+00004050: 5294 6805 288a 0800 b002 62d7 e183 174e  R.h.(.....b....N
+00004060: 4e4b 0a74 9452 9468 0528 8a08 00b0 581d  NK.t.R.h.(....X.
+00004070: 5e25 d616 4e4e 4b0a 7494 5294 6805 288a  ^%..NNK.t.R.h.(.
+00004080: 0800 b062 e420 6a66 174e 4e4b 0a74 9452  ...b. jf.NNK.t.R
+00004090: 9468 0528 8a08 00b0 5454 f72d 8817 4e4e  .h.(....TT.-..NN
+000040a0: 4b0a 7494 5294 6805 288a 0800 b01b d20d  K.t.R.h.(.......
+000040b0: c8ed 164e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+000040c0: 00b0 b58d ad44 0317 4e4e 4b0a 7494 5294  .....D..NNK.t.R.
+000040d0: 6805 288a 0800 b0b0 6fb7 957f 174e 4e4b  h.(.....o....NNK
+000040e0: 0a74 9452 9468 0528 8a08 00b0 d094 b657  .t.R.h.(.......W
+000040f0: c417 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00004100: b007 80cd 9007 174e 4e4b 0a74 9452 9468  .......NNK.t.R.h
+00004110: 0528 8a08 00b0 36d9 16db ae17 4e4e 4b0a  .(....6.....NNK.
+00004120: 7494 5294 6805 288a 0800 b0e4 e6f6 8eaa  t.R.h.(.........
 00004130: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00004140: 7842 5de7 1a17 4e4e 4b0a 7494 5294 6805  xB]...NNK.t.R.h.
-00004150: 288a 0800 b0a1 3b6d 0d1d 174e 4e4b 0a74  (.....;m...NNK.t
-00004160: 9452 9468 0528 8a08 00b0 ca34 7d33 1f17  .R.h.(.....4}3..
-00004170: 4e4e 4b0a 7494 5294 6805 288a 0800 b0f3  NNK.t.R.h.(.....
-00004180: 2d8d 5921 174e 4e4b 0a74 9452 9468 0528  -.Y!.NNK.t.R.h.(
-00004190: 8a08 00b0 1c27 9d7f 2317 4e4e 4b0a 7494  .....'..#.NNK.t.
-000041a0: 5294 6805 288a 0800 b0f6 8e18 5725 174e  R.h.(.......W%.N
-000041b0: 4e4b 0a74 9452 9468 0528 8a08 00b0 6e19  NK.t.R.h.(....n.
-000041c0: bdcb 2717 4e4e 4b0a 7494 5294 6805 288a  ..'.NNK.t.R.h.(.
-000041d0: 0800 b097 12cd f129 174e 4e4b 0a74 9452  .......).NNK.t.R
-000041e0: 9468 0528 8a08 00b0 c00b dd17 2c17 4e4e  .h.(........,.NN
-000041f0: 4b0a 7494 5294 6805 288a 0800 b0e9 04ed  K.t.R.h.(.......
-00004200: 3d2e 174e 4e4b 0a74 9452 9468 0528 8a08  =..NNK.t.R.h.(..
-00004210: 00b0 12fe fc63 3017 4e4e 4b0a 7494 5294  .....c0.NNK.t.R.
-00004220: 6805 288a 0800 b03b f70c 8a32 174e 4e4b  h.(....;...2.NNK
-00004230: 0a74 9452 9468 0528 8a08 00b0 64f0 1cb0  .t.R.h.(....d...
-00004240: 3417 4e4e 4b0a 7494 5294 6805 288a 0800  4.NNK.t.R.h.(...
-00004250: b08d e92c d636 174e 4e4b 0a74 9452 9468  ...,.6.NNK.t.R.h
-00004260: 0528 8a08 00b0 b6e2 3cfc 3817 4e4e 4b0a  .(......<.8.NNK.
-00004270: 7494 5294 6805 288a 0800 b0df db4c 223b  t.R.h.(......L";
+00004140: 2132 47ec 9217 4e4e 4b0a 7494 5294 6805  !2G...NNK.t.R.h.
+00004150: 288a 0800 b09c 1d77 5e99 174e 4e4b 0a74  (......w^..NNK.t
+00004160: 9452 9468 0528 8a08 00b0 12fe fc63 3017  .R.h.(.......c0.
+00004170: 4e4e 4b0a 7494 5294 6805 288a 0800 b078  NNK.t.R.h.(....x
+00004180: 425d e71a 174e 4e4b 0a74 9452 9468 0528  B]...NNK.t.R.h.(
+00004190: 8a08 00b0 beff e0d1 5d17 4e4e 4b0a 7494  ........].NNK.t.
+000041a0: 5294 6805 288a 0800 b0b6 e23c fc38 174e  R.h.(......<.8.N
+000041b0: 4e4b 0a74 9452 9468 0528 8a08 00b0 4002  NK.t.R.h.(....@.
+000041c0: b7f6 a117 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
+000041d0: 0800 b0f3 2d8d 5921 174e 4e4b 0a74 9452  ....-.Y!.NNK.t.R
+000041e0: 9468 0528 8a08 00b0 d45d 1d4f 1217 4e4e  .h.(.....].O..NN
+000041f0: 4b0a 7494 5294 6805 288a 0800 b073 2467  K.t.R.h.(....s$g
+00004200: 3897 174e 4e4b 0a74 9452 9468 0528 8a08  8..NNK.t.R.h.(..
+00004210: 00b0 64f0 1cb0 3417 4e4e 4b0a 7494 5294  ..d...4.NNK.t.R.
+00004220: 6805 288a 0800 b011 a96d acfa 164e 4e4b  h.(......m...NNK
+00004230: 0a74 9452 9468 0528 8a08 00b0 fc01 9ebd  .t.R.h.(........
+00004240: de16 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00004250: b0f4 821c 1157 174e 4e4b 0a74 9452 9468  .....W.NNK.t.R.h
+00004260: 0528 8a08 00b0 58bb 804e 7317 4e4e 4b0a  .(....X..Ns.NNK.
+00004270: 7494 5294 6805 288a 0800 b079 97ec 9e50  t.R.h.(....y...P
 00004280: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00004290: 08d5 5c48 3d17 4e4e 4b0a 7494 5294 6805  ..\H=.NNK.t.R.h.
-000042a0: 288a 0800 b031 ce6c 6e3f 174e 4e4b 0a74  (....1.ln?.NNK.t
-000042b0: 9452 9468 0528 8a08 00b0 5ac7 7c94 4117  .R.h.(....Z.|.A.
-000042c0: 4e4e 4b0a 7494 5294 6805 288a 0800 b083  NNK.t.R.h.(.....
-000042d0: c08c ba43 174e 4e4b 0a74 9452 9468 0528  ...C.NNK.t.R.h.(
-000042e0: 8a08 00b0 acb9 9ce0 4517 4e4e 4b0a 7494  ........E.NNK.t.
-000042f0: 5294 6805 288a 0800 b0d5 b2ac 0648 174e  R.h.(........H.N
-00004300: 4e4b 0a74 9452 9468 0528 8a08 00b0 af1a  NK.t.R.h.(......
-00004310: 28de 4917 4e4e 4b0a 7494 5294 6805 288a  (.I.NNK.t.R.h.(.
-00004320: 0800 b027 a5cc 524c 174e 4e4b 0a74 9452  ...'..RL.NNK.t.R
+00004290: bfb6 4d60 f616 4e4e 4b0a 7494 5294 6805  ..M`..NNK.t.R.h.
+000042a0: 288a 0800 b039 eb10 4464 174e 4e4b 0a74  (....9..Dd.NNK.t
+000042b0: 9452 9468 0528 8a08 00b0 062b 3ed9 d116  .R.h.(.....+>...
+000042c0: 4e4e 4b0a 7494 5294 6805 288a 0800 b08e  NNK.t.R.h.(.....
+000042d0: 3ebc 8d6c 174e 4e4b 0a74 9452 9468 0528  >..l.NNK.t.R.h.(
+000042e0: 8a08 00b0 f276 20cb 8817 4e4e 4b0a 7494  .....v ...NNK.t.
+000042f0: 5294 6805 288a 0800 b074 79f6 efcc 174e  R.h.(....ty....N
+00004300: 4e4b 0a74 9452 9468 0528 8a08 00b0 8c94  NK.t.R.h.(......
+00004310: 9d1e 0117 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
+00004320: 0800 b044 cb1d eeef 164e 4e4b 0a74 9452  ...D.....NNK.t.R
 00004330: 9468 0528 8a08 00b0 509e dc78 4e17 4e4e  .h.(....P..xN.NN
-00004340: 4b0a 7494 5294 6805 288a 0800 b079 97ec  K.t.R.h.(....y..
-00004350: 9e50 174e 4e4b 0a74 9452 9468 0528 8a08  .P.NNK.t.R.h.(..
-00004360: 00b0 53ff 6776 5217 4e4e 4b0a 7494 5294  ..S.gvR.NNK.t.R.
-00004370: 6805 288a 0800 b0cb 890c eb54 174e 4e4b  h.(........T.NNK
-00004380: 0a74 9452 9468 0528 8a08 00b0 f482 1c11  .t.R.h.(........
-00004390: 5717 4e4e 4b0a 7494 5294 6805 288a 0800  W.NNK.t.R.h.(...
-000043a0: b01d 7c2c 3759 174e 4e4b 0a74 9452 9468  ..|,7Y.NNK.t.R.h
-000043b0: 0528 8a08 00b0 9506 d1ab 5b17 4e4e 4b0a  .(........[.NNK.
-000043c0: 7494 5294 6805 288a 0800 b0be ffe0 d15d  t.R.h.(........]
+00004340: 4b0a 7494 5294 6805 288a 0800 b0ca 347d  K.t.R.h.(.....4}
+00004350: 331f 174e 4e4b 0a74 9452 9468 0528 8a08  3..NNK.t.R.h.(..
+00004360: 00b0 81b4 9074 7517 4e4e 4b0a 7494 5294  .....tu.NNK.t.R.
+00004370: 6805 288a 0800 b0e9 04ed 3d2e 174e 4e4b  h.(.......=..NNK
+00004380: 0a74 9452 9468 0528 8a08 00b0 25fb ade3  .t.R.h.(....%...
+00004390: e016 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+000043a0: b07c 4709 31a3 174e 4e4b 0a74 9452 9468  .|G.1..NNK.t.R.h
+000043b0: 0528 8a08 00b0 aa0f 7e71 da16 4e4e 4b0a  .(......~q..NNK.
+000043c0: 7494 5294 6805 288a 0800 b06e 19bd cb27  t.R.h.(....n...'
 000043d0: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-000043e0: e7f8 f0f7 5f17 4e4e 4b0a 7494 5294 6805  ...._.NNK.t.R.h.
-000043f0: 288a 0800 b010 f200 1e62 174e 4e4b 0a74  (........b.NNK.t
-00004400: 9452 9468 0528 8a08 00b0 39eb 1044 6417  .R.h.(....9..Dd.
-00004410: 4e4e 4b0a 7494 5294 6805 288a 0800 b062  NNK.t.R.h.(....b
-00004420: e420 6a66 174e 4e4b 0a74 9452 9468 0528  . jf.NNK.t.R.h.(
-00004430: 8a08 00b0 8bdd 3090 6817 4e4e 4b0a 7494  ......0.h.NNK.t.
-00004440: 5294 6805 288a 0800 b0b4 d640 b66a 174e  R.h.(......@.j.N
-00004450: 4e4b 0a74 9452 9468 0528 8a08 00b0 8e3e  NK.t.R.h.(.....>
-00004460: bc8d 6c17 4e4e 4b0a 7494 5294 6805 288a  ..l.NNK.t.R.h.(.
-00004470: 0800 b006 c960 026f 174e 4e4b 0a74 9452  .....`.o.NNK.t.R
-00004480: 9468 0528 8a08 00b0 2fc2 7028 7117 4e4e  .h.(..../.p(q.NN
-00004490: 4b0a 7494 5294 6805 288a 0800 b058 bb80  K.t.R.h.(....X..
-000044a0: 4e73 174e 4e4b 0a74 9452 9468 0528 8a08  Ns.NNK.t.R.h.(..
-000044b0: 00b0 81b4 9074 7517 4e4e 4b0a 7494 5294  .....tu.NNK.t.R.
-000044c0: 6805 288a 0800 b0aa ada0 9a77 174e 4e4b  h.(........w.NNK
-000044d0: 0a74 9452 9468 0528 8a08 00b0 d3a6 b0c0  .t.R.h.(........
-000044e0: 7917 4e4e 4b0a 7494 5294 6805 288a 0800  y.NNK.t.R.h.(...
-000044f0: b0fc 9fc0 e67b 174e 4e4b 0a74 9452 9468  .....{.NNK.t.R.h
-00004500: 0528 8a08 00b0 8776 a76f 7d17 4e4e 4b0a  .(.....v.o}.NNK.
-00004510: 7494 5294 6805 288a 0800 b025 99d0 0c7e  t.R.h.(....%...~
+000043e0: acb9 9ce0 4517 4e4e 4b0a 7494 5294 6805  ....E.NNK.t.R.h.
+000043f0: 288a 0800 b097 12cd f129 174e 4e4b 0a74  (........).NNK.t
+00004400: 9452 9468 0528 8a08 00b0 dd31 2eb3 cf16  .R.h.(.....1....
+00004410: 4e4e 4b0a 7494 5294 6805 288a 0800 b0d3  NNK.t.R.h.(.....
+00004420: 088e 97dc 164e 4e4b 0a74 9452 9468 0528  .....NNK.t.R.h.(
+00004430: 8a08 00b0 5fd2 2601 b117 4e4e 4b0a 7494  ...._.&...NNK.t.
+00004440: 5294 6805 288a 0800 b0bb ede6 68a8 174e  R.h.(.......h..N
+00004450: 4e4b 0a74 9452 9468 0528 8a08 00b0 f98d  NK.t.R.h.(......
+00004460: c67d c617 4e4e 4b0a 7494 5294 6805 288a  .}..NNK.t.R.h.(.
+00004470: 0800 b093 4966 fadb 174e 4e4b 0a74 9452  ....If...NNK.t.R
+00004480: 9468 0528 8a08 00b0 cf3f 27a0 8e17 4e4e  .h.(.....?'...NN
+00004490: 4b0a 7494 5294 6805 288a 0800 b0a1 3b6d  K.t.R.h.(.....;m
+000044a0: 0d1d 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+000044b0: 00b0 b1c4 464d b517 4e4e 4b0a 7494 5294  ....FM..NNK.t.R.
+000044c0: 6805 288a 0800 b082 6bfd 020e 174e 4e4b  h.(.....k....NNK
+000044d0: 0a74 9452 9468 0528 8a08 00b0 d5b2 ac06  .t.R.h.(........
+000044e0: 4817 4e4e 4b0a 7494 5294 6805 288a 0800  H.NNK.t.R.h.(...
+000044f0: b055 a986 e5bd 174e 4e4b 0a74 9452 9468  .U.....NNK.t.R.h
+00004500: 0528 8a08 00b0 2b5b e707 8617 4e4e 4b0a  .(....+[....NNK.
+00004510: 7494 5294 6805 288a 0800 b0d9 68c7 bb81  t.R.h.(.....h...
 00004520: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00004530: b06f b795 7f17 4e4e 4b0a 7494 5294 6805  .o....NNK.t.R.h.
-00004540: 288a 0800 b04e 92e0 3280 174e 4e4b 0a74  (....N..2..NNK.t
-00004550: 9452 9468 0528 8a08 00b0 d968 c7bb 8117  .R.h.(.....h....
-00004560: 4e4e 4b0a 7494 5294 6805 288a 0800 b002  NNK.t.R.h.(.....
-00004570: 62d7 e183 174e 4e4b 0a74 9452 9468 0528  b....NNK.t.R.h.(
-00004580: 8a08 00b0 2b5b e707 8617 4e4e 4b0a 7494  ....+[....NNK.t.
-00004590: 5294 6805 288a 0800 b054 54f7 2d88 174e  R.h.(....TT.-..N
-000045a0: 4e4b 0a74 9452 9468 0528 8a08 00b0 f276  NK.t.R.h.(.....v
-000045b0: 20cb 8817 4e4e 4b0a 7494 5294 6805 288a   ...NNK.t.R.h.(.
-000045c0: 0800 b090 9949 6889 174e 4e4b 0a74 9452  .....Ih..NNK.t.R
-000045d0: 9468 0528 8a08 00b0 a646 177a 8c17 4e4e  .h.(.....F.z..NN
-000045e0: 4b0a 7494 5294 6805 288a 0800 b0cf 3f27  K.t.R.h.(.....?'
-000045f0: a08e 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00004600: 00b0 f838 37c6 9017 4e4e 4b0a 7494 5294  ...87...NNK.t.R.
-00004610: 6805 288a 0800 b021 3247 ec92 174e 4e4b  h.(....!2G...NNK
-00004620: 0a74 9452 9468 0528 8a08 00b0 4a2b 5712  .t.R.h.(....J+W.
-00004630: 9517 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00004640: b073 2467 3897 174e 4e4b 0a74 9452 9468  .s$g8..NNK.t.R.h
-00004650: 0528 8a08 00b0 9c1d 775e 9917 4e4e 4b0a  .(......w^..NNK.
-00004660: 7494 5294 6805 288a 0800 b0d8 62c9 989a  t.R.h.(.....b...
+00004530: 9d72 0616 cf17 4e4e 4b0a 7494 5294 6805  .r....NNK.t.R.h.
+00004540: 288a 0800 b0c9 dfed 7be9 164e 4e4b 0a74  (.......{..NNK.t
+00004550: 9452 9468 0528 8a08 00b0 96bd 3d3a f416  .R.h.(......=:..
+00004560: 4e4e 4b0a 7494 5294 6805 288a 0800 b088  NNK.t.R.h.(.....
+00004570: cb36 27b3 174e 4e4b 0a74 9452 9468 0528  .6'..NNK.t.R.h.(
+00004580: 8a08 00b0 8776 a76f 7d17 4e4e 4b0a 7494  .....v.o}.NNK.t.
+00004590: 5294 6805 288a 0800 b0da bd56 73b7 174e  R.h.(......Vs..N
+000045a0: 4e4b 0a74 9452 9468 0528 8a08 00b0 a79b  NK.t.R.h.(......
+000045b0: a631 c217 4e4e 4b0a 7494 5294 6805 288a  .1..NNK.t.R.h.(.
+000045c0: 0800 b006 c960 026f 174e 4e4b 0a74 9452  .....`.o.NNK.t.R
+000045d0: 9468 0528 8a08 00b0 5ac7 7c94 4117 4e4e  .h.(....Z.|.A.NN
+000045e0: 4b0a 7494 5294 6805 288a 0800 b095 06d1  K.t.R.h.(.......
+000045f0: ab5b 174e 4e4b 0a74 9452 9468 0528 8a08  .[.NNK.t.R.h.(..
+00004600: 00b0 3aa2 7dd2 fc16 4e4e 4b0a 7494 5294  ..:.}...NNK.t.R.
+00004610: 6805 288a 0800 b0aa ada0 9a77 174e 4e4b  h.(........w.NNK
+00004620: 0a74 9452 9468 0528 8a08 00b0 639b 8df8  .t.R.h.(....c...
+00004630: fe16 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00004640: b02f 244e ffd3 164e 4e4b 0a74 9452 9468  ./$N...NNK.t.R.h
+00004650: 0528 8a08 00b0 3bf7 0c8a 3217 4e4e 4b0a  .(....;...2.NNK.
+00004660: 7494 5294 6805 288a 0800 b022 87d6 a3c8  t.R.h.(...."....
 00004670: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00004680: ee0f 97aa 9d17 4e4e 4b0a 7494 5294 6805  ......NNK.t.R.h.
-00004690: 288a 0800 b017 09a7 d09f 174e 4e4b 0a74  (..........NNK.t
-000046a0: 9452 9468 0528 8a08 00b0 4002 b7f6 a117  .R.h.(....@.....
-000046b0: 4e4e 4b0a 7494 5294 6805 288a 0800 b07c  NNK.t.R.h.(....|
-000046c0: 4709 31a3 174e 4e4b 0a74 9452 9468 0528  G.1..NNK.t.R.h.(
-000046d0: 8a08 00b0 92f4 d642 a617 4e4e 4b0a 7494  .......B..NNK.t.
-000046e0: 5294 6805 288a 0800 b0bb ede6 68a8 174e  R.h.(.......h..N
-000046f0: 4e4b 0a74 9452 9468 0528 8a08 00b0 e4e6  NK.t.R.h.(......
-00004700: f68e aa17 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
-00004710: 0800 b00d e006 b5ac 174e 4e4b 0a74 9452  .........NNK.t.R
-00004720: 9468 0528 8a08 00b0 36d9 16db ae17 4e4e  .h.(....6.....NN
-00004730: 4b0a 7494 5294 6805 288a 0800 b05f d226  K.t.R.h.(...._.&
-00004740: 01b1 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00004750: 00b0 88cb 3627 b317 4e4e 4b0a 7494 5294  ....6'..NNK.t.R.
-00004760: 6805 288a 0800 b0b1 c446 4db5 174e 4e4b  h.(......FM..NNK
-00004770: 0a74 9452 9468 0528 8a08 00b0 dabd 5673  .t.R.h.(......Vs
-00004780: b717 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00004790: b003 b766 99b9 174e 4e4b 0a74 9452 9468  ...f...NNK.t.R.h
-000047a0: 0528 8a08 00b0 2cb0 76bf bb17 4e4e 4b0a  .(....,.v...NNK.
-000047b0: 7494 5294 6805 288a 0800 b055 a986 e5bd  t.R.h.(....U....
+00004680: 4b80 e6c9 ca17 4e4e 4b0a 7494 5294 6805  K.....NNK.t.R.h.
+00004690: 288a 0800 b0df db4c 223b 174e 4e4b 0a74  (......L";.NNK.t
+000046a0: 9452 9468 0528 8a08 00b0 d862 c998 9a17  .R.h.(.....b....
+000046b0: 4e4e 4b0a 7494 5294 6805 288a 0800 b04f  NNK.t.R.h.(....O
+000046c0: 494d c118 174e 4e4b 0a74 9452 9468 0528  IM...NNK.t.R.h.(
+000046d0: 8a08 00b0 8bdd 3090 6817 4e4e 4b0a 7494  ......0.h.NNK.t.
+000046e0: 5294 6805 288a 0800 b003 b766 99b9 174e  R.h.(......f...N
+000046f0: 4e4b 0a74 9452 9468 0528 8a08 00b0 e1e7  NK.t.R.h.(......
+00004700: 4868 0917 4e4e 4b0a 7494 5294 6805 288a  Hh..NNK.t.R.h.(.
+00004710: 0800 b04a 2b57 1295 174e 4e4b 0a74 9452  ...J+W...NNK.t.R
+00004720: 9468 0528 8a08 00b0 fd56 2d75 1417 4e4e  .h.(.....V-u..NN
+00004730: 4b0a 7494 5294 6805 288a 0800 b08d e92c  K.t.R.h.(......,
+00004740: d636 174e 4e4b 0a74 9452 9468 0528 8a08  .6.NNK.t.R.h.(..
+00004750: 00b0 4ef4 bd09 e316 4e4e 4b0a 7494 5294  ..N.....NNK.t.R.
+00004760: 6805 288a 0800 b090 9949 6889 174e 4e4b  h.(......Ih..NNK
+00004770: 0a74 9452 9468 0528 8a08 00b0 b4d6 40b6  .t.R.h.(......@.
+00004780: 6a17 4e4e 4b0a 7494 5294 6805 288a 0800  j.NNK.t.R.h.(...
+00004790: b0ee 0f97 aa9d 174e 4e4b 0a74 9452 9468  .......NNK.t.R.h
+000047a0: 0528 8a08 00b0 e8af 5d86 f816 4e4e 4b0a  .(......]...NNK.
+000047b0: 7494 5294 6805 288a 0800 b0f8 3837 c690  t.R.h.(.....87..
 000047c0: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-000047d0: 91ee d81f bf17 4e4e 4b0a 7494 5294 6805  ......NNK.t.R.h.
-000047e0: 288a 0800 b0a7 9ba6 31c2 174e 4e4b 0a74  (.......1..NNK.t
-000047f0: 9452 9468 0528 8a08 00b0 d094 b657 c417  .R.h.(.......W..
-00004800: 4e4e 4b0a 7494 5294 6805 288a 0800 b0f9  NNK.t.R.h.(.....
-00004810: 8dc6 7dc6 174e 4e4b 0a74 9452 9468 0528  ..}..NNK.t.R.h.(
-00004820: 8a08 00b0 2287 d6a3 c817 4e4e 4b0a 7494  ....".....NNK.t.
-00004830: 5294 6805 288a 0800 b04b 80e6 c9ca 174e  R.h.(....K.....N
-00004840: 4e4b 0a74 9452 9468 0528 8a08 00b0 7479  NK.t.R.h.(....ty
-00004850: f6ef cc17 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
-00004860: 0800 b09d 7206 16cf 174e 4e4b 0a74 9452  ....r....NNK.t.R
-00004870: 9468 0528 8a08 00b0 ef64 2662 d317 4e4e  .h.(.....d&b..NN
-00004880: 4b0a 7494 5294 6805 288a 0800 b093 4966  K.t.R.h.(.....If
-00004890: fadb 174e 4e4b 0a74 9452 9465 752e       ...NNK.t.R.eu.
+000047d0: 4e92 e032 8017 4e4e 4b0a 7494 5294 6805  N..2..NNK.t.R.h.
+000047e0: 288a 0800 b0d3 a6b0 c079 174e 4e4b 0a74  (........y.NNK.t
+000047f0: 9452 9468 0528 8a08 00b0 2cb0 76bf bb17  .R.h.(....,.v...
+00004800: 4e4e 4b0a 7494 5294 6805 288a 0800 b0fc  NNK.t.R.h.(.....
+00004810: 9fc0 e67b 174e 4e4b 0a74 9452 9468 0528  ...{.NNK.t.R.h.(
+00004820: 8a08 00b0 91ee d81f bf17 4e4e 4b0a 7494  ..........NNK.t.
+00004830: 5294 6805 288a 0800 b0a0 e6dd 55e7 164e  R.h.(.......U..N
+00004840: 4e4b 0a74 9452 9468 0528 8a08 00b0 ef64  NK.t.R.h.(.....d
+00004850: 2662 d317 4e4e 4b0a 7494 5294 6805 288a  &b..NNK.t.R.h.(.
+00004860: 0800 b017 09a7 d09f 174e 4e4b 0a74 9452  .........NNK.t.R
+00004870: 9468 0528 8a08 00b0 1c27 9d7f 2317 4e4e  .h.(.....'..#.NN
+00004880: 4b0a 7494 5294 6805 288a 0800 b0d9 b758  K.t.R.h.(......X
+00004890: 50d0 174e 4e4b 0a74 9452 9468 0528 8a08  P..NNK.t.R.h.(..
+000048a0: 00b0 185e 3688 d517 4e4e 4b0a 7494 5294  ...^6...NNK.t.R.
+000048b0: 6805 288a 0800 b0c0 0bdd 172c 174e 4e4b  h.(........,.NNK
+000048c0: 0a74 9452 9468 0528 8a08 00b0 1d7c 2c37  .t.R.h.(.....|,7
+000048d0: 5917 4e4e 4b0a 7494 5294 6805 288a 0800  Y.NNK.t.R.h.(...
+000048e0: b0e7 f8f0 f75f 174e 4e4b 0a74 9452 9468  ....._.NNK.t.R.h
+000048f0: 0528 8a08 00b0 cb89 0ceb 5417 4e4e 4b0a  .(........T.NNK.
+00004900: 7494 5294 6805 288a 0800 b010 f200 1e62  t.R.h.(........b
+00004910: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00004920: ab64 0d29 1017 4e4e 4b0a 7494 5294 6805  .d.)..NNK.t.R.h.
+00004930: 288a 0800 b0a6 4617 7a8c 174e 4e4b 0a74  (.....F.z..NNK.t
+00004940: 9452 9465 8c06 5345 4e53 4558 945d 9428  .R.e..SENSEX.].(
+00004950: 6805 288a 0800 b0af 69b9 7298 174e 4e4b  h.(.....i.r..NNK
+00004960: 0a74 9452 9468 0528 8a08 00b0 c410 8961  .t.R.h.(.......a
+00004970: b417 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00004980: b03e a729 1c85 174e 4e4b 0a74 9452 9468  .>.)...NNK.t.R.h
+00004990: 0528 8a08 00b0 e3e0 f86b c317 4e4e 4b0a  .(.......k..NNK.
+000049a0: 7494 5294 6805 288a 0800 b0c3 bbf9 a97e  t.R.h.(........~
+000049b0: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+000049c0: 48d0 c937 7817 4e4e 4b0a 7494 5294 6805  H..7x.NNK.t.R.h.
+000049d0: 288a 0800 b015 ae19 f682 174e 4e4b 0a74  (..........NNK.t
+000049e0: 9452 9468 0528 8a08 00b0 71c9 d95d 7a17  .R.h.(....q..]z.
+000049f0: 4e4e 4b0a 7494 5294 6805 288a 0800 b07c  NNK.t.R.h.(....|
+00004a00: 4709 31a3 174e 4e4b 0a74 9452 9468 0528  G.1..NNK.t.R.h.(
+00004a10: 8a08 00b0 721e 6915 b017 4e4e 4b0a 7494  ....r.i...NNK.t.
+00004a20: 5294 6805 288a 0800 b034 7e89 0092 174e  R.h.(....4~....N
+00004a30: 4e4b 0a74 9452 9468 0528 8a08 00b0 1fd7  NK.t.R.h.(......
+00004a40: b911 7617 4e4e 4b0a 7494 5294 6805 288a  ..v.NNK.t.R.h.(.
+00004a50: 0800 b00c da08 92c5 174e 4e4b 0a74 9452  .........NNK.t.R
+00004a60: 9468 0528 8a08 00b0 a540 1957 a517 4e4e  .h.(.....@.W..NN
+00004a70: 4b0a 7494 5294 6805 288a 0800 b0e2 8b69  K.t.R.h.(......i
+00004a80: b48d 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+00004a90: 00b0 d862 c998 9a17 4e4e 4b0a 7494 5294  ...b....NNK.t.R.
+00004aa0: 6805 288a 0800 b087 c538 04cc 174e 4e4b  h.(......8...NNK
+00004ab0: 0a74 9452 9468 0528 8a08 00b0 2900 5a2d  .t.R.h.(....).Z-
+00004ac0: 6917 4e4e 4b0a 7494 5294 6805 288a 0800  i.NNK.t.R.h.(...
+00004ad0: b0ec b409 d080 174e 4e4b 0a74 9452 9468  .......NNK.t.R.h
+00004ae0: 0528 8a08 00b0 ae14 2abb 6217 4e4e 4b0a  .(......*.b.NNK.
+00004af0: 7494 5294 6805 288a 0800 b067 a039 4287  t.R.h.(....g.9B.
+00004b00: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00004b10: 015c d9be 9c17 4e4e 4b0a 7494 5294 6805  .\....NNK.t.R.h.
+00004b20: 288a 0800 b0fa 93c4 a0ad 174e 4e4b 0a74  (..........NNK.t
+00004b30: 9452 9468 0528 8a08 00b0 52f9 6953 6b17  .R.h.(....R.iSk.
+00004b40: 4e4e 4b0a 7494 5294 6805 288a 0800 b090  NNK.t.R.h.(.....
+00004b50: 9949 6889 174e 4e4b 0a74 9452 9468 0528  .Ih..NNK.t.R.h.(
+00004b60: 8a08 00b0 0007 4a07 6717 4e4e 4b0a 7494  ......J.g.NNK.t.
+00004b70: 5294 6805 288a 0800 b0a4 eb89 9f6f 174e  R.h.(........o.N
+00004b80: 4e4b 0a74 9452 9468 0528 8a08 00b0 8670  NK.t.R.h.(.....p
+00004b90: a94c 9617 4e4e 4b0a 7494 5294 6805 288a  .L..NNK.t.R.h.(.
+00004ba0: 0800 b068 f5c8 f9bc 174e 4e4b 0a74 9452  ...h.....NNK.t.R
+00004bb0: 9468 0528 8a08 00b0 f06a 2485 ba17 4e4e  .h.(.....j$...NN
+00004bc0: 4b0a 7494 5294 6805 288a 0800 b09b 1779  K.t.R.h.(......y
+00004bd0: 3bb2 174e 4e4b 0a74 9452 9468 0528 8a08  ;..NNK.t.R.h.(..
+00004be0: 00b0 d70d 3ae1 6417 4e4e 4b0a 7494 5294  ....:.d.NNK.t.R.
+00004bf0: 6805 288a 0800 b07b f279 796d 174e 4e4b  h.(....{.yym.NNK
+00004c00: 0a74 9452 9468 0528 8a08 00b0 ce39 297d  .t.R.h.(.....9)}
+00004c10: a717 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00004c20: b06b 5654 f7c0 174e 4e4b 0a74 9452 9468  .kVT...NNK.t.R.h
+00004c30: 0528 8a08 00b0 f6dd a9eb 7317 4e4e 4b0a  .(........s.NNK.
+00004c40: 7494 5294 6805 288a 0800 b091 eed8 1fbf  t.R.h.(.........
+00004c50: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00004c60: 5ecc 28de c917 4e4e 4b0a 7494 5294 6805  ^.(...NNK.t.R.h.
+00004c70: 288a 0800 b053 4ef9 0aa1 174e 4e4b 0a74  (....SN....NNK.t
+00004c80: 9452 9468 0528 8a08 00b0 35d3 18b8 c717  .R.h.(....5.....
+00004c90: 4e4e 4b0a 7494 5294 6805 288a 0800 b05d  NNK.t.R.h.(....]
+00004ca0: 7799 2694 174e 4e4b 0a74 9452 9468 0528  w.&..NNK.t.R.h.(
+00004cb0: 8a08 00b0 ed09 9987 b617 4e4e 4b0a 7494  ..........NNK.t.
+00004cc0: 5294 6805 288a 0800 b09a c2e9 837c 174e  R.h.(........|.N
+00004cd0: 4e4b 0a74 9452 9468 0528 8a08 00b0 0b85  NK.t.R.h.(......
+00004ce0: 79da 8f17 4e4e 4b0a 7494 5294 6805 288a  y...NNK.t.R.h.(.
+00004cf0: 0800 b016 03a9 adb8 174e 4e4b 0a74 9452  .........NNK.t.R
+00004d00: 9468 0528 8a08 00b0 b0be 482a ce17 4e4e  .h.(......H*..NN
+00004d10: 4b0a 7494 5294 6805 288a 0800 b085 1b1a  K.t.R.h.(.......
+00004d20: 9560 174e 4e4b 0a74 9452 9468 0528 8a08  .`.NNK.t.R.h.(..
+00004d30: 00b0 2baa 789c d417 4e4e 4b0a 7494 5294  ..+.x...NNK.t.R.
+00004d40: 6805 288a 0800 b0b9 9259 8e8b 174e 4e4b  h.(......Y...NNK
+00004d50: 0a74 9452 9468 0528 8a08 00b0 2a55 e9e4  .t.R.h.(....*U..
+00004d60: 9e17 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00004d70: b0cd e499 c571 174e 4e4b 0a74 9452 9468  .....q.NNK.t.R.h
+00004d80: 0528 8a08 00b0 202c 49c9 ab17 4e4e 4b0a  .(.... ,I...NNK.
+00004d90: 7494 5294 6805 288a 0800 b0f7 3239 a3a9  t.R.h.(.....29..
+00004da0: 174e 4e4b 0a74 9452 9465 8c06 4241 4e4b  .NNK.t.R.e..BANK
+00004db0: 4558 945d 9428 6805 288a 0800 b074 79f6  EX.].(h.(....ty.
+00004dc0: efcc 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+00004dd0: 00b0 3ea7 291c 8517 4e4e 4b0a 7494 5294  ..>.)...NNK.t.R.
+00004de0: 6805 288a 0800 b0c3 bbf9 a97e 174e 4e4b  h.(........~.NNK
+00004df0: 0a74 9452 9468 0528 8a08 00b0 7324 6738  .t.R.h.(....s$g8
+00004e00: 9717 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00004e10: b048 d0c9 3778 174e 4e4b 0a74 9452 9468  .H..7x.NNK.t.R.h
+00004e20: 0528 8a08 00b0 15ae 19f6 8217 4e4e 4b0a  .(..........NNK.
+00004e30: 7494 5294 6805 288a 0800 b06f bddd 17ac  t.R.h.(....o....
+00004e40: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00004e50: 71c9 d95d 7a17 4e4e 4b0a 7494 5294 6805  q..]z.NNK.t.R.h.
+00004e60: 288a 0800 b07c 4709 31a3 174e 4e4b 0a74  (....|G.1..NNK.t
+00004e70: 9452 9468 0528 8a08 00b0 2287 d6a3 c817  .R.h.(....".....
+00004e80: 4e4e 4b0a 7494 5294 6805 288a 0800 b01f  NNK.t.R.h.(.....
+00004e90: d7b9 1176 174e 4e4b 0a74 9452 9468 0528  ...v.NNK.t.R.h.(
+00004ea0: 8a08 00b0 4b80 e6c9 ca17 4e4e 4b0a 7494  ....K.....NNK.t.
+00004eb0: 5294 6805 288a 0800 b0e2 8b69 b48d 174e  R.h.(......i...N
+00004ec0: 4e4b 0a74 9452 9468 0528 8a08 00b0 d862  NK.t.R.h.(.....b
+00004ed0: c998 9a17 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
+00004ee0: 0800 b029 005a 2d69 174e 4e4b 0a74 9452  ...).Z-i.NNK.t.R
+00004ef0: 9468 0528 8a08 00b0 ecb4 09d0 8017 4e4e  .h.(..........NN
+00004f00: 4b0a 7494 5294 6805 288a 0800 b003 b766  K.t.R.h.(......f
+00004f10: 99b9 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+00004f20: 00b0 5fd2 2601 b117 4e4e 4b0a 7494 5294  .._.&...NNK.t.R.
+00004f30: 6805 288a 0800 b0ae 142a bb62 174e 4e4b  h.(......*.b.NNK
+00004f40: 0a74 9452 9468 0528 8a08 00b0 92f4 d642  .t.R.h.(.......B
+00004f50: a617 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00004f60: b067 a039 4287 174e 4e4b 0a74 9452 9468  .g.9B..NNK.t.R.h
+00004f70: 0528 8a08 00b0 4a2b 5712 9517 4e4e 4b0a  .(....J+W...NNK.
+00004f80: 7494 5294 6805 288a 0800 b0bb ede6 68a8  t.R.h.(.......h.
+00004f90: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+00004fa0: f98d c67d c617 4e4e 4b0a 7494 5294 6805  ...}..NNK.t.R.h.
+00004fb0: 288a 0800 b0cf 3f27 a08e 174e 4e4b 0a74  (.....?'...NNK.t
+00004fc0: 9452 9468 0528 8a08 00b0 0de0 06b5 ac17  .R.h.(..........
+00004fd0: 4e4e 4b0a 7494 5294 6805 288a 0800 b090  NNK.t.R.h.(.....
+00004fe0: 9949 6889 174e 4e4b 0a74 9452 9468 0528  .Ih..NNK.t.R.h.(
+00004ff0: 8a08 00b0 0007 4a07 6717 4e4e 4b0a 7494  ......J.g.NNK.t.
+00005000: 5294 6805 288a 0800 b0a4 eb89 9f6f 174e  R.h.(........o.N
+00005010: 4e4b 0a74 9452 9468 0528 8a08 00b0 ee0f  NK.t.R.h.(......
+00005020: 97aa 9d17 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
+00005030: 0800 b0b1 c446 4db5 174e 4e4b 0a74 9452  .....FM..NNK.t.R
+00005040: 9468 0528 8a08 00b0 d70d 3ae1 6417 4e4e  .h.(......:.d.NN
+00005050: 4b0a 7494 5294 6805 288a 0800 b07b f279  K.t.R.h.(....{.y
+00005060: 796d 174e 4e4b 0a74 9452 9468 0528 8a08  ym.NNK.t.R.h.(..
+00005070: 00b0 f838 37c6 9017 4e4e 4b0a 7494 5294  ...87...NNK.t.R.
+00005080: 6805 288a 0800 b02c b076 bfbb 174e 4e4b  h.(....,.v...NNK
+00005090: 0a74 9452 9468 0528 8a08 00b0 55a9 86e5  .t.R.h.(....U...
+000050a0: bd17 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+000050b0: b0f6 dda9 eb73 174e 4e4b 0a74 9452 9468  .....s.NNK.t.R.h
+000050c0: 0528 8a08 00b0 91ee d81f bf17 4e4e 4b0a  .(..........NNK.
+000050d0: 7494 5294 6805 288a 0800 b0d0 94b6 57c4  t.R.h.(.......W.
+000050e0: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
+000050f0: ef64 2662 d317 4e4e 4b0a 7494 5294 6805  .d&b..NNK.t.R.h.
+00005100: 288a 0800 b017 09a7 d09f 174e 4e4b 0a74  (..........NNK.t
+00005110: 9452 9468 0528 8a08 00b0 36d9 16db ae17  .R.h.(....6.....
+00005120: 4e4e 4b0a 7494 5294 6805 288a 0800 b09d  NNK.t.R.h.(.....
+00005130: 7206 16cf 174e 4e4b 0a74 9452 9468 0528  r....NNK.t.R.h.(
+00005140: 8a08 00b0 88cb 3627 b317 4e4e 4b0a 7494  ......6'..NNK.t.
+00005150: 5294 6805 288a 0800 b09a c2e9 837c 174e  R.h.(........|.N
+00005160: 4e4b 0a74 9452 9468 0528 8a08 00b0 e4e6  NK.t.R.h.(......
+00005170: f68e aa17 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
+00005180: 0800 b0da bd56 73b7 174e 4e4b 0a74 9452  .....Vs..NNK.t.R
+00005190: 9468 0528 8a08 00b0 851b 1a95 6017 4e4e  .h.(........`.NN
+000051a0: 4b0a 7494 5294 6805 288a 0800 b0b9 9259  K.t.R.h.(......Y
+000051b0: 8e8b 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+000051c0: 00b0 2132 47ec 9217 4e4e 4b0a 7494 5294  ..!2G...NNK.t.R.
+000051d0: 6805 288a 0800 b09c 1d77 5e99 174e 4e4b  h.(......w^..NNK
+000051e0: 0a74 9452 9468 0528 8a08 00b0 a79b a631  .t.R.h.(.......1
+000051f0: c217 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00005200: b0cd e499 c571 174e 4e4b 0a74 9452 9468  .....q.NNK.t.R.h
+00005210: 0528 8a08 00b0 4002 b7f6 a117 4e4e 4b0a  .(....@.....NNK.
+00005220: 7494 5294 6575 2e                        t.R.eu.
```

### Comparing `volstreet-8.1.3/volstreet/historical_info/market_days.pkl` & `volstreet-8.2.0/volstreet/historical_info/market_days.pkl`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8004 95cf 4100 0000 0000 005d 9428 8c08  ....A......].(..
+00000000: 8004 9503 4200 0000 0000 005d 9428 8c08  ....B......].(..
 00000010: 6461 7465 7469 6d65 948c 0464 6174 6594  datetime...date.
 00000020: 9394 4304 07e3 0201 9485 9452 9468 0343  ..C........R.h.C
 00000030: 0407 e302 0494 8594 5294 6803 4304 07e3  ........R.h.C...
 00000040: 0205 9485 9452 9468 0343 0407 e302 0694  .....R.h.C......
 00000050: 8594 5294 6803 4304 07e3 0207 9485 9452  ..R.h.C........R
 00000060: 9468 0343 0407 e302 0894 8594 5294 6803  .h.C........R.h.
 00000070: 4304 07e3 020b 9485 9452 9468 0343 0407  C........R.h.C..
@@ -1047,8 +1047,11 @@
 00004160: 9452 9468 0343 0407 e804 0f94 8594 5294  .R.h.C........R.
 00004170: 6803 4304 07e8 0410 9485 9452 9468 0343  h.C........R.h.C
 00004180: 0407 e804 1294 8594 5294 6803 4304 07e8  ........R.h.C...
 00004190: 0413 9485 9452 9468 0343 0407 e804 1694  .....R.h.C......
 000041a0: 8594 5294 6803 4304 07e8 0417 9485 9452  ..R.h.C........R
 000041b0: 9468 0343 0407 e804 1894 8594 5294 6803  .h.C........R.h.
 000041c0: 4304 07e8 0419 9485 9452 9468 0343 0407  C........R.h.C..
-000041d0: e804 1a94 8594 5294 652e                 ......R.e.
+000041d0: e804 1a94 8594 5294 6803 4304 07e8 041d  ......R.h.C.....
+000041e0: 9485 9452 9468 0343 0407 e804 1e94 8594  ...R.h.C........
+000041f0: 5294 6803 4304 07e8 0502 9485 9452 9468  R.h.C........R.h
+00004200: 0343 0407 e805 0394 8594 5294 652e       .C........R.e.
```

### Comparing `volstreet-8.1.3/volstreet/models/__init__.py` & `volstreet-8.2.0/volstreet/models/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def load_iv_curve_model():
     resource_path = files("volstreet").joinpath("models")
     model_path = resource_path.joinpath("iv_curve_model_lite.joblib")
     try:
         model = load(model_path)
         logger.info("IV curve model loaded successfully")
     except Exception as e:
-        logger.error(f"Error loading IV curve model: {e}")
+        logger.warning(f"Unable to load IV curve model: {e}")
         model = None
 
     return model
 
 
 iv_curve_model = load_iv_curve_model()
 expiry_day_model = None
```

### Comparing `volstreet-8.1.3/volstreet/parallelization.py` & `volstreet-8.2.0/volstreet/parallelization.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/performance_tracking.py` & `volstreet-8.2.0/volstreet/performance_tracking.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/position_dashboard/app.py` & `volstreet-8.2.0/volstreet/position_dashboard/app.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/position_dashboard/formatting.py` & `volstreet-8.2.0/volstreet/position_dashboard/formatting.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/strategies/deployment.py` & `volstreet-8.2.0/volstreet/strategies/deployment.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,21 +8,20 @@
 import os
 from multiprocessing import Manager
 import numpy as np
 from SmartApi.smartExceptions import DataException
 from volstreet.config import logger
 from volstreet.utils.data_io import load_combine_save_json_data
 from volstreet.utils.communication import notifier
-from volstreet.utils.core import current_time
+from volstreet.utils.core import current_time, check_for_weekend, time_to_expiry
 from volstreet.utils.change_config import (
     set_notifier_level,
     set_error_notification_settings,
 )
 from volstreet import config
-from volstreet.dealingroom import get_strangle_indices_to_trade
 from volstreet.angel_interface.login import login, wait_for_login
 from volstreet.angel_interface.interface import (
     LiveFeeds,
     fetch_book,
     lookup_and_return,
     modify_order,
     update_order_params,
@@ -35,14 +34,15 @@
     intraday_trend,
     delta_hedged_strangle,
     overnight_straddle,
     biweekly_straddle,
     buy_weekly_hedge,
     quick_strangle,
     reentry_straddle,
+    trend_v2,
 )
 
 
 class BaseStrategy(ABC):
     def __init__(
         self,
         parameters,  # Note: The type is not specified, it can be list or dict
@@ -244,19 +244,19 @@
         )
         self.strategy_threads = self.setup_threads(self.indices_to_trade)
 
         logger.info(
             f"Waiting for {self.__class__.__name__} to start at {self.start_time}"
         )
 
+        self.subscribe_strikes()
+
         while current_time().time() < time(*self.start_time):
             sleep(1)
 
-        self.subscribe_strikes()
-
         # Start all threads
         for thread in self.strategy_threads:
             thread.start()
 
         # Join all threads
         for thread in self.strategy_threads:
             thread.join()
@@ -298,15 +298,15 @@
 
     def set_strategy_tags(self, strategy_tags: Optional[list[str]] = None) -> list[str]:
         return strategy_tags or ["Quick Strangle"]
 
     def initialize_indices(self, indices: Optional[list] = None) -> list[Index]:
         indices = indices or ["NIFTY", "BANKNIFTY", "FINNIFTY", "MIDCPNIFTY", "SENSEX"]
         indices = [Index(index) for index in indices]
-        indices: list[Index] | [] = get_strangle_indices_to_trade(*indices)
+        indices: list[Index] | [] = get_expiry_day_indices(*indices)
         indices = super().initialize_indices(
             indices
         )  # This will notify about what indices are being traded
         return indices
 
 
 class IntradayStrangle(BaseStrategy):
@@ -324,15 +324,43 @@
 
     def set_strategy_tags(self, strategy_tags: Optional[list[str]] = None) -> list[str]:
         return strategy_tags or ["Intraday strangle"]
 
     def initialize_indices(self, indices: Optional[list] = None) -> list[Index]:
         indices = indices or ["NIFTY", "BANKNIFTY", "FINNIFTY", "MIDCPNIFTY", "SENSEX"]
         indices = [Index(index) for index in indices]
-        indices: list[Index] | [] = get_strangle_indices_to_trade(*indices)
+        indices: list[Index] | [] = get_expiry_day_indices(*indices)
+        indices = super().initialize_indices(
+            indices
+        )  # This will notify about what indices are being traded
+        return indices
+
+
+class TrendV2(BaseStrategy):
+    @property
+    def strats(self):
+        return [trend_v2]
+
+    @property
+    def expiry_sub_modes(self) -> dict:
+        return {"current_expiry": 3}
+
+    @property
+    def to_divide_exposure(self) -> bool:
+        return True
+
+    def set_strategy_tags(
+        self, strategy_tags: Optional[list[str] | str] = None
+    ) -> list[str]:
+        return strategy_tags or ["Trend v2"]
+
+    def initialize_indices(self, indices: Optional[list] = None) -> list[Index]:
+        indices = indices or ["NIFTY", "BANKNIFTY", "FINNIFTY", "MIDCPNIFTY", "SENSEX"]
+        indices = [Index(index) for index in indices]
+        indices: list[Index] | [] = get_expiry_day_indices(*indices)
         indices = super().initialize_indices(
             indices
         )  # This will notify about what indices are being traded
         return indices
 
 
 class IntradayTrend(BaseStrategy):
@@ -379,15 +407,15 @@
         self, strategy_tags: Optional[list[str] | str] = None
     ) -> list[str]:
         return strategy_tags or ["Delta hedged strangle"]
 
     def initialize_indices(self, indices: Optional[list] = None) -> list[Index]:
         indices = indices or ["NIFTY", "BANKNIFTY", "FINNIFTY", "MIDCPNIFTY", "SENSEX"]
         indices = [Index(index) for index in indices]
-        indices: list[Index] | [] = get_strangle_indices_to_trade(*indices)
+        indices: list[Index] | [] = get_expiry_day_indices(*indices)
         indices = super().initialize_indices(
             indices
         )  # This will notify about what indices are being traded
         return indices
 
 
 class ReentryStraddle(BaseStrategy):
@@ -407,15 +435,15 @@
         self, strategy_tags: Optional[list[str] | str] = None
     ) -> list[str]:
         return strategy_tags or ["Reentry straddle"]
 
     def initialize_indices(self, indices: Optional[list] = None) -> list[Index]:
         indices = indices or ["NIFTY", "BANKNIFTY", "FINNIFTY", "MIDCPNIFTY", "SENSEX"]
         indices = [Index(index) for index in indices]
-        indices: list[Index] | [] = get_strangle_indices_to_trade(*indices)
+        indices: list[Index] | [] = get_expiry_day_indices(*indices)
         indices = super().initialize_indices(
             indices
         )  # This will notify about what indices are being traded
         return indices
 
 
 class OvernightStraddle(BaseStrategy):
@@ -496,14 +524,15 @@
         "quick_strangle": QuickStrangle,
         "intraday_strangle": IntradayStrangle,
         "intraday_trend": IntradayTrend,
         "overnight_straddle": OvernightStraddle,
         "biweekly_straddle": BiweeklyStraddle,
         "delta_hedged_strangle": DeltaHedgedStrangle,
         "reentry_straddle": ReentryStraddle,
+        "trend_v2": TrendV2,
     }
 
     def __init__(
         self,
         user: str,
         pin: str,
         apikey: str,
@@ -828,7 +857,53 @@
         for k, v in signature.parameters.items()
     }
     # Remove the 'underlying' parameter if it exists
     params.pop("underlying", None)
     if as_string:
         return json.dumps(params)
     return params
+
+
+def get_expiry_day_indices(*indices: Index) -> list[Index] | list[None]:
+    safe_indices = ["NIFTY", "BANKNIFTY", "FINNIFTY"]
+
+    times_to_expiries = [
+        time_to_expiry(index.current_expiry, effective_time=True, in_days=True)
+        for index in indices
+    ]
+
+    # Check if any index has less than 1 day to expiry
+    indices_less_than_1_day = [
+        index
+        for index, time_left_to_expiry in zip(indices, times_to_expiries)
+        if time_left_to_expiry < 1
+    ]
+
+    if indices_less_than_1_day:
+        return indices_less_than_1_day
+
+    # If no index has less than 1 day to expiry
+    min_expiry_time = min(times_to_expiries)
+    indices_with_closest_expiries = [
+        index
+        for index, time_left_to_expiry in zip(indices, times_to_expiries)
+        if time_left_to_expiry == min_expiry_time
+    ]
+    weekend_in_range = check_for_weekend(
+        indices_with_closest_expiries[0].current_expiry
+    )
+
+    if weekend_in_range:
+        # Checking if the closest indices are safe indices
+        safe_and_close = [
+            index
+            for index in indices_with_closest_expiries
+            if index.name in safe_indices
+        ]
+        if (
+            safe_and_close
+        ):  # If the indices with the closest expiry are safe indices then return the closest indices
+            return safe_and_close
+        else:  # If the indices with the closest expiry are not safe indices then return safe indices
+            return [index for index in indices if index.name in safe_indices]
+
+    return indices_with_closest_expiries
```

### Comparing `volstreet-8.1.3/volstreet/strategies/error_handling.py` & `volstreet-8.2.0/volstreet/strategies/monitoring.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,92 @@
-import functools
-import traceback
-from inspect import signature
-from datetime import datetime
-from time import sleep
+import pandas as pd
+import numpy as np
 import asyncio
+from datetime import datetime
+from volstreet.utils.core import parse_symbol, custom_round
 from volstreet import config
-from volstreet.utils import (
-    custom_round,
-    notifier,
-    current_time,
-    filter_orderbook_by_time,
-    log_error,
-)
+from volstreet.utils import notifier, filter_orderbook_by_time
 from volstreet.angel_interface.interface import (
-    fetch_book,
     fetch_quotes,
+    fetch_book,
     lookup_and_return,
 )
-from volstreet.trade_interface import cancel_pending_orders, execute_orders
-from volstreet.strategies.monitoring import get_current_state_of_strategy
+from volstreet.trade_interface import execute_orders, cancel_pending_orders
+from volstreet.strategies.tools import filter_orders_by_strategy
+
+
+def get_current_state_of_strategy(
+    orderbook: list,
+    index: str,
+    order_tag: str,
+    with_pnl: bool = True,
+) -> pd.DataFrame:
+    """
+    Returns the present state of a strategy. This is qty, tokens, and symbols for a given order tag.
+    Active quantity is increased for 'BUY' transactions and decreased for 'SELL' transactions.
+
+    :param orderbook: List of orderbook entries.
+    :param index: The index to search for.
+    :param order_tag: The order tag to search for.
+    :param with_pnl: Whether to include PnL in the output.
+    :return: A list dataframe with the following columns:
+        - tradingsymbol: The symbol of the contract.
+        - symboltoken: The token of the contract.
+        - lotsize: The lot size of the contract.
+        - netqty: The net quantity of the contract.
+        - active_lots: The number of active lots.
+        - underlying: The underlying of the contract.
+        - expiry: The expiry of the contract.
+        - strike: The strike of the contract.
+        - option_type: The option type of the contract.
+    """
+
+    # Filtering orders and making a dataframe
+    filtered_orders = filter_orders_by_strategy(orderbook, order_tag, index)
+    if not filtered_orders:
+        return pd.DataFrame()
+    df = pd.DataFrame(filtered_orders)
+
+    # Converting data types
+    df["filledshares"] = df["filledshares"].astype(int)
+    df["lotsize"] = df["lotsize"].astype(int)
+
+    # Converting filledshares to a signed number
+    df["filledshares"] = df["filledshares"] * np.where(
+        df.transactiontype == "BUY", 1, -1
+    )
+
+    # Filtering out incomplete orders
+    df = df[df["status"] == "complete"]
+
+    if df.empty:
+        return pd.DataFrame()
+
+    grouped = df.groupby("tradingsymbol")
+    state = (
+        grouped.agg({"filledshares": "sum", "symboltoken": "first", "lotsize": "first"})
+        .reset_index()
+        .rename(columns={"filledshares": "netqty"})
+    )
+
+    state["active_lots"] = state["netqty"] // state["lotsize"]
+    state[["underlying", "expiry", "strike", "option_type"]] = (
+        state["tradingsymbol"].apply(parse_symbol).to_list()
+    )
+
+    if with_pnl:
+        state["net_value"] = grouped.apply(
+            lambda x: np.dot(x["filledshares"], x["averageprice"]), include_groups=False
+        ).values
+        ltp_data = fetch_quotes([tok for tok in state.symboltoken], structure="dict")
+        ltp_data = {k: v["ltp"] for k, v in ltp_data.items()}
+        state["ltp"] = state["symboltoken"].apply(ltp_data.get)
+        state["outstanding_value"] = state["netqty"] * state["ltp"]
+        state["pnl"] = state["outstanding_value"] - state["net_value"]
+    return state
 
 
 def prepare_exit_params(
     positions: list[dict],
     max_lot_multiplier: int = 30,
     ltp_missing: bool = True,
 ) -> list[dict]:
@@ -72,71 +136,35 @@
             }
             order_params_list.append(params)
             total_qty -= order_qty
 
     return order_params_list
 
 
-@log_error(notify=True, raise_error=True)
-def exit_strategy(strategy: callable, execution_time: datetime, *args, **kwargs):
-    sig = signature(strategy)
-    bound = sig.bind_partial(*args, **kwargs)
-    bound.apply_defaults()
-    order_tag = bound.arguments.get("strategy_tag")
-    index = bound.arguments.get("underlying").name
+def exit_positions(execution_time: datetime, index: str, identifier: str):
     order_book = fetch_book("orderbook", from_api=True)
     order_book = filter_orderbook_by_time(order_book, start_time=execution_time)
     pending_orders = lookup_and_return(
-        order_book, ["ordertag", "status"], [order_tag, "open"], "orderid"
+        order_book, ["ordertag", "status"], [identifier, "open"], "orderid"
     )
     if pending_orders:
         cancel_pending_orders(pending_orders, variety="NORMAL")
     active_positions = get_current_state_of_strategy(
-        order_book, index, order_tag, with_pnl=False
+        order_book, index, identifier, with_pnl=False
     )
 
     if active_positions.empty:
         notifier(
-            f"No positions at all for strategy {strategy.__name__}",
+            f"No positions at all for strategy {identifier}",
             webhook_url=config.ERROR_NOTIFICATION_SETTINGS["url"],
         )
         return
 
     active_positions = active_positions.to_dict(orient="records")
     exit_params = prepare_exit_params(active_positions, ltp_missing=True)
     if not exit_params:
         notifier(
-            f"No ACTIVE positions for strategy {strategy.__name__}",
+            f"No ACTIVE positions for strategy {identifier}",
             webhook_url=config.ERROR_NOTIFICATION_SETTINGS["url"],
         )
         return
     asyncio.run(execute_orders(exit_params))
-    user_prefix = config.ERROR_NOTIFICATION_SETTINGS.get("user")
-    user_prefix = f"{user_prefix} - " if user_prefix else ""
-    notifier(
-        f"{user_prefix}Exited positions for strategy {strategy.__name__}",
-        webhook_url=config.ERROR_NOTIFICATION_SETTINGS["url"],
-        send_whatsapp=True,
-    )
-
-
-def exit_on_error(strategy):
-    @functools.wraps(strategy)
-    def wrapper(*args, **kwargs):
-        execution_time = current_time()
-        try:
-            return strategy(*args, **kwargs)
-        except Exception as e:
-            user_prefix = config.ERROR_NOTIFICATION_SETTINGS.get("user")
-            user_prefix = f"{user_prefix} - " if user_prefix else ""
-            sleep(4)  # Sleep for 4 seconds to allow the orders to be filled
-            notifier(
-                f"{user_prefix}"
-                f"Error in strategy {strategy.__name__}: {e}\nTraceback:{traceback.format_exc()}\n\n"
-                f"Exiting existing positions...",
-                webhook_url=config.ERROR_NOTIFICATION_SETTINGS["url"],
-                level="ERROR",
-                send_whatsapp=True,
-            )
-            exit_strategy(strategy, execution_time, *args, **kwargs)
-
-    return wrapper
```

### Comparing `volstreet-8.1.3/volstreet/strategies/helpers.py` & `volstreet-8.2.0/volstreet/strategies/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from datetime import datetime, timedelta, time
 from time import sleep
 from itertools import product
 import inspect
 import traceback
 from typing import Callable
 from pulp import LpStatus
-import os
 from volstreet import config
 from volstreet.config import logger
 from volstreet.blackscholes import Greeks
 from volstreet.utils.core import (
     time_to_expiry,
     current_time,
     round_shares_to_lot_size,
     filter_orderbook_by_time,
+    find_strike,
 )
 from volstreet.utils.communication import notifier
 from volstreet.utils.data_io import load_json_data, load_combine_save_json_data
 from volstreet.angel_interface.interface import (
     ActiveSession,
     LiveFeeds,
     fetch_quotes,
@@ -37,14 +37,15 @@
     place_option_order_and_notify,
     cancel_pending_orders,
 )
 from volstreet.strategies.tools import filter_orders_by_strategy
 from volstreet.strategies.optimization import (
     filter_greeks_frame,
     delta_neutral_optimization_lp,
+    trend_following_optimization_lp,
 )
 from volstreet.strategies.error_handling import log_error
 
 if config.backtest_mode:
     logger.info(
         f"Importing proxy functions in module: {__name__} since backtesting is enabled."
     )
@@ -266,28 +267,27 @@
             setattr(self, key, value)
 
     def exit_triggered(self):
         return any(self.exit_triggers.values())
 
 
 @define(slots=False)
-class DeltaPosition:
+class PositionManager:
     # Required attributes
     underlying: Index = field(validator=validators.instance_of(Index))
     base_exposure_qty = field()
 
     # Other attributes with default values
+    file_path = field(default=None)
     greek_settings = field(factory=dict, validator=validators.instance_of(dict))
     order_tag = field(default="", validator=validators.instance_of(str))
     cached_strikes = field(default=[], repr=False)
     expiry = field(validator=validators.instance_of(str))
     _prospective_calls = field(factory=list, repr=False)
     _prospective_puts = field(factory=list, repr=False)
-    hedge_call_option = field(default=None, repr=False)
-    hedge_put_option = field(default=None, repr=False)
     exit_triggers: dict[str, bool] = field(
         factory=lambda: {"end_time": False, "qty_breach_exit": False}
     )
     notifier_url: str = field(default=None)
 
     @property
     def all_options(self):
@@ -460,14 +460,27 @@
     def get_option_gammas(options: list[Option], filter_func: Callable = None):
         gammas = [option.current_greeks.gamma for option in options]
         if filter_func:
             return np.array([*filter(filter_func, gammas)])
         else:
             return np.array(gammas)
 
+    def get_option_chain_with_greeks(self) -> np.ndarray:
+        """Returns a 2d array of greeks with options as the last column.
+        Data columns: strike, ltp, delta, gamma, theta, vega, option.
+        The universe of options are the prospective calls and prospective puts."""
+
+        call_greeks = self.prepare_greek_frame_with_options(
+            self.prospective_calls, True
+        )
+        put_greeks = self.prepare_greek_frame_with_options(self.prospective_puts, False)
+        all_greeks = np.concatenate([call_greeks, put_greeks])
+
+        return all_greeks
+
     def potential_greeks(self) -> Greeks:
         greeks = np.sum(
             [
                 (opt.recommended_qty * opt.current_greeks)
                 for opt in self.recommended_options
             ]
         )
@@ -543,27 +556,215 @@
 
         # If the original attributes must be lists, convert them back
         self._prospective_calls = [*sorted(current_calls_set, key=lambda x: x.strike)]
         self._prospective_puts = [
             *sorted(current_puts_set, key=lambda x: -1 * x.strike)
         ]  # Descending order
 
+    def prepare_greek_frame_with_options(
+        self, options: list[Option], is_call: bool
+    ) -> np.ndarray:
+        greeks = self.get_option_greeks(options, informative=True)
+        array = np.array([option for option in options])
+        greeks = np.column_stack((greeks, array))
+        logger.debug(f"Greeks: {greeks}. Dispatching to filter_greeks_frame")
+        greeks = filter_greeks_frame(
+            greeks,
+            0.65,
+            self.underlying.get_synthetic_future_price(self.expiry),
+            is_call,
+        )
+        return greeks
+
+    def update_underlying(self) -> None:
+        """Updates the underlying price and the implied future interest rate."""
+        self.underlying.fetch_ltp()
+        self.underlying.get_basis_for_expiry(self.expiry)
+
+    def set_weights_in_options(
+        self, option_array: np.ndarray, weights: np.ndarray
+    ) -> None:
+        for option, weight in zip(option_array, weights):
+            option.recommended_qty = round_shares_to_lot_size(
+                weight * self.base_exposure_qty, option.lot_size
+            )
+
+    def enter_positions(self, at_market: bool) -> None:
+        instructions = {
+            option: {
+                "action": Action.BUY if option.recommended_qty >= 0 else Action.SELL,
+                "quantity_in_lots": abs(option.recommended_qty) / option.lot_size,
+                "order_tag": self.order_tag,
+            }
+            for option in self.recommended_options
+        }
+        execution_details = execute_instructions(instructions, at_market=at_market)
+        for option, avg_price in execution_details.items():
+            option.update_active_qty_and_premium(option.recommended_qty, avg_price)
+            option.recommended_qty = 0
+
+    def exit_positions(self, at_market: bool) -> None:
+        """Handles squaring up of the position"""
+        instructions = {
+            option: {
+                "action": Action.BUY if option.active_qty <= 0 else Action.SELL,
+                "quantity_in_lots": abs(option.active_qty) / option.lot_size,
+                "order_tag": self.order_tag,
+            }
+            for option in self.active_options
+        }
+        execution_details = execute_instructions(instructions, at_market=at_market)
+        for option, avg_price in execution_details.items():
+            option.update_active_qty_and_premium(-option.active_qty, avg_price)
+
+    def record_position_status(self) -> None:
+        """Designed to periodically save the position status to a file."""
+        """
+        Saves the current position status to a JSON file periodically.
+        """
+        if self.file_path is None:
+            return  # No file path set
+
+        total_premium_outstanding = sum(
+            [option.premium_outstanding for option in self.active_options]
+        )
+        total_premium_received = sum(
+            [option.premium_received for option in self.all_options]
+        )
+
+        position_status = {
+            "timestamp": current_time(),
+            "underlying": self.underlying.name,
+            "underlying_price": self.underlying.fetch_ltp(),
+            "expiry": self.expiry,
+            "base_exposure_qty": self.base_exposure_qty,
+            "active_call_options": [
+                {
+                    "strike": option.strike,
+                    "option_type": option.option_type.value,
+                    "active_qty": option.active_qty,
+                    "premium_received": option.premium_received,
+                    "current_ltp": option.current_ltp,
+                    "current_greeks": option.current_greeks.as_dict(),
+                }
+                for option in self.active_call_options
+            ],
+            "active_put_options": [
+                {
+                    "strike": option.strike,
+                    "option_type": option.option_type.value,
+                    "active_qty": option.active_qty,
+                    "premium_received": option.premium_received,
+                    "current_ltp": option.current_ltp,
+                    "current_greeks": option.current_greeks.as_dict(),
+                }
+                for option in self.active_put_options
+            ],
+            "aggregate_greeks": self.aggregate_greeks().as_dict(),
+            "total_premium_received": total_premium_received,
+            "total_premium_outstanding": total_premium_outstanding,
+            "mtm": total_premium_outstanding - total_premium_received,
+            "exit_triggers": self.exit_triggers,
+        }
+
+        load_combine_save_json_data(
+            position_status, self.file_path, default_structure=list
+        )
+
+    def reset_trigger_flags(self):
+        self.exit_triggers = {"end_time": False, "qty_breach_exit": False}
+
+
+@define(slots=False)
+class TrendPosition(PositionManager):
+
+    def set_recommended_qty_simple(
+        self, hedge_offset: float, trend_direction: Action
+    ) -> None:
+        spot = self.underlying.fetch_ltp()
+        atm_strike = find_strike(spot, self.underlying.base)
+
+        hedge_strike_multiplier = (
+            1 + hedge_offset if trend_direction == Action.BUY else 1 - hedge_offset
+        )
+        hedge_strike = find_strike(spot * hedge_strike_multiplier, self.underlying.base)
+        hedge_option_type: OptionType = (
+            OptionType.CALL if trend_direction == Action.BUY else OptionType.PUT
+        )
+
+        for option in self._prospective_calls:
+            if option.strike == atm_strike:
+                option.recommended_qty = (
+                    self.base_exposure_qty * trend_direction.num_value
+                )
+            elif hedge_option_type == OptionType.CALL and option.strike == hedge_strike:
+                option.recommended_qty = (
+                    self.base_exposure_qty * -1
+                )  # Hedge is always sold
+        for option in self._prospective_puts:
+            if option.strike == atm_strike:
+                option.recommended_qty = (
+                    -self.base_exposure_qty * trend_direction.num_value
+                )
+            elif hedge_option_type == OptionType.PUT and option.strike == hedge_strike:
+                option.recommended_qty = (
+                    self.base_exposure_qty * -1
+                )  # Hedge is always sold
+
+    def set_recommended_qty_optimized(
+        self, target_delta: float, trend_direction: Action
+    ) -> None:
+        all_greeks = self.get_option_chain_with_greeks()
+
+        prob, weights = trend_following_optimization_lp(
+            all_greeks[:, 2:6],
+            target_delta=target_delta,
+            trend_direction=trend_direction,
+        )
+        if prob.status != 1:
+            logger.warning(
+                f"Optimization in trend following failed with status {LpStatus[prob.status]}. "
+                f"Check earlier messages from logs for more details."
+            )
+            raise Exception(f"Optimization failed with status {LpStatus[prob.status]}")
+
+        self.set_weights_in_options(all_greeks[:, -1], weights)
+
+    def set_recommended_qty(
+        self,
+        optimized: bool,
+        target_delta: float,
+        trend_direction: Action,
+        hedge_offset: float,
+    ) -> None:
+        self.reset_options()
+        if optimized:
+            self.set_recommended_qty_optimized(target_delta, trend_direction)
+        else:
+            self.set_recommended_qty_simple(hedge_offset, trend_direction)
+
+
+@define(slots=False)
+class DeltaPosition(PositionManager):
+    hedge_call_option = field(default=None, repr=False)
+    hedge_put_option = field(default=None, repr=False)
+
+    def set_file_path(self):
+        date = current_time().strftime("%Y-%m-%d")
+        file_path = f"{ActiveSession.obj.userId}\\{self.underlying.name.lower()}_delta_data\\{date}.json"
+        return file_path
+
     def set_hedge_options(self):
         self.hedge_call_option = min(
             self.prospective_calls, key=lambda x: abs(x.current_greeks.delta - 0.5)
         )
         self.hedge_put_option = min(
             self.prospective_puts, key=lambda x: abs(x.current_greeks.delta + 0.5)
         )
 
-    def update_underlying(self) -> None:
-        """Updates the underlying price and the implied future interest rate."""
-        self.underlying.fetch_ltp()
-        self.underlying.get_basis_for_expiry(self.expiry)
-
     def _handle_option_type(self, options, target_delta):
         higher_options = [
             *filter(lambda x: abs(x.current_greeks.delta) >= target_delta, options)
         ]
         lower_options = [
             *filter(lambda x: abs(x.current_greeks.delta) < target_delta, options)
         ]
@@ -616,29 +817,14 @@
             self.base_exposure_qty * ratio_lower, lower_option.lot_size
         )
 
         upper_option.recommended_qty = -upper_option_qty
         lower_option.recommended_qty = -lower_option_qty
         return True
 
-    def prepare_greek_frame_with_options(
-        self, options: list[Option], is_call: bool
-    ) -> np.ndarray:
-        greeks = self.get_option_greeks(options, informative=True)
-        array = np.array([option for option in options])
-        greeks = np.column_stack((greeks, array))
-        logger.debug(f"Greeks: {greeks}. Dispatching to filter_greeks_frame")
-        greeks = filter_greeks_frame(
-            greeks,
-            0.65,
-            self.underlying.get_synthetic_future_price(self.expiry),
-            is_call,
-        )
-        return greeks
-
     def set_recommended_qty_backup(
         self, target_delta: float = None, attempt_no: int = 0
     ):
         self.reset_options()
 
         if target_delta > 0.7 or attempt_no > 5:
             raise ValueError(
@@ -669,45 +855,35 @@
             )
 
     def set_optimized_recommended_qty(self, optimize_gamma: bool):
         self.reset_options()
         ivs = self.get_option_ivs(self.prospective_calls + self.prospective_puts)
         median_iv = np.nanmedian(ivs)
         logger.info(f"Using median IV {median_iv} for optimization")
-        call_greeks = self.prepare_greek_frame_with_options(
-            self.prospective_calls, True
-        )
-        put_greeks = self.prepare_greek_frame_with_options(self.prospective_puts, False)
-        all_greeks = np.concatenate([call_greeks, put_greeks])
-        # At this point all_greeks has the following columns:
-        # [strike, ltp, delta, gamma, theta, vega, option]
+        all_greeks = self.get_option_chain_with_greeks()
 
         # Solving the optimization problem
 
         prob, weights = delta_neutral_optimization_lp(
             all_greeks[:, 2:6],
             optimize_gamma=optimize_gamma,
             spot=self.underlying.fetch_ltp(),
             time_to_expiry=time_to_expiry(self.expiry),
             r=self.underlying.get_basis_for_expiry(self.expiry),
             iv=median_iv,
         )  # Using delta, gamma, theta, vega
 
         if prob.status != 1:
             logger.warning(
-                f"Optimization failed with status {LpStatus[prob.status]}. "
+                f"Optimization in delta hedging failed with status {LpStatus[prob.status]}. "
                 f"Check earlier messages from logs for more details."
             )
             raise Exception(f"Optimization failed with status {LpStatus[prob.status]}")
 
-        # noinspection PyUnboundLocalVariable
-        for option, weight in zip(all_greeks[:, -1], weights):
-            option.recommended_qty = round_shares_to_lot_size(
-                weight * self.base_exposure_qty, option.lot_size
-            )
+        self.set_weights_in_options(all_greeks[:, -1], weights)
 
     def set_recommended_qty(
         self, target_delta: float, optimized: bool, optimize_gamma: bool
     ) -> None:
         if optimized:
             try:
                 self.set_optimized_recommended_qty(optimize_gamma=optimize_gamma)
@@ -727,31 +903,14 @@
         """Adjusts the recommended qty to account for active qty in order to avoid unnecessary
         orders."""
         for option in self.all_options:
             if option.recommended_qty == 0 and option.active_qty == 0:
                 continue
             option.recommended_qty = option.recommended_qty - option.active_qty
 
-    def enter_positions(self, at_market: bool) -> None:
-        instructions = {
-            option: {
-                "action": Action.BUY if option.recommended_qty >= 0 else Action.SELL,
-                "quantity_in_lots": abs(option.recommended_qty) / option.lot_size,
-                "order_tag": self.order_tag,
-            }
-            for option in self.recommended_options
-        }
-        execution_details = execute_instructions(instructions, at_market=at_market)
-        for option, avg_price in execution_details.items():
-            option.update_active_qty_and_premium(option.recommended_qty, avg_price)
-            option.recommended_qty = 0
-
-    def reset_trigger_flags(self):
-        self.exit_triggers = {"end_time": False, "qty_breach_exit": False}
-
     def recommend_delta_action(
         self,
         delta_threshold: float,
         aggregate_delta: float,
     ) -> tuple[ActiveOption, int] | tuple[None, np.nan]:
         """Returns a negative qty because the qty is to be sold."""
         hedge_call_delta = self.hedge_call_option.current_greeks.delta
@@ -789,84 +948,14 @@
             breach = (
                 abs(self.aggregate_put_active_qty) + adjustment_qty
             ) > max_qty_shares
         else:
             raise ValueError("Invalid option type")
         return breach
 
-    def exit_positions(self, at_market: bool) -> None:
-        """Handles squaring up of the position"""
-        instructions = {
-            option: {
-                "action": Action.BUY if option.active_qty <= 0 else Action.SELL,
-                "quantity_in_lots": abs(option.active_qty) / option.lot_size,
-                "order_tag": self.order_tag,
-            }
-            for option in self.active_options
-        }
-        execution_details = execute_instructions(instructions, at_market=at_market)
-        for option, avg_price in execution_details.items():
-            option.update_active_qty_and_premium(-option.active_qty, avg_price)
-
-    def record_position_status(self, directory: str | None = None) -> None:
-        """Designed to periodically save the position status to a file."""
-        """
-        Saves the current position status to a JSON file periodically.
-        """
-
-        date = current_time().strftime("%Y-%m-%d")
-        if directory is None:
-            file_path = f"{ActiveSession.obj.userId}\\{self.underlying.name}_delta_data\\{date}.json"
-        else:
-            file_path = os.path.join(directory, f"{date}.json")
-
-        total_premium_outstanding = sum(
-            [option.premium_outstanding for option in self.active_options]
-        )
-        total_premium_received = sum(
-            [option.premium_received for option in self.all_options]
-        )
-
-        position_status = {
-            "timestamp": current_time(),
-            "underlying": self.underlying.name,
-            "underlying_price": self.underlying.fetch_ltp(),
-            "expiry": self.expiry,
-            "base_exposure_qty": self.base_exposure_qty,
-            "active_call_options": [
-                {
-                    "strike": option.strike,
-                    "option_type": option.option_type.value,
-                    "active_qty": option.active_qty,
-                    "premium_received": option.premium_received,
-                    "current_ltp": option.current_ltp,
-                    "current_greeks": option.current_greeks.as_dict(),
-                }
-                for option in self.active_call_options
-            ],
-            "active_put_options": [
-                {
-                    "strike": option.strike,
-                    "option_type": option.option_type.value,
-                    "active_qty": option.active_qty,
-                    "premium_received": option.premium_received,
-                    "current_ltp": option.current_ltp,
-                    "current_greeks": option.current_greeks.as_dict(),
-                }
-                for option in self.active_put_options
-            ],
-            "aggregate_greeks": self.aggregate_greeks().as_dict(),
-            "total_premium_received": total_premium_received,
-            "total_premium_outstanding": total_premium_outstanding,
-            "mtm": total_premium_outstanding - total_premium_received,
-            "exit_triggers": self.exit_triggers,
-        }
-
-        load_combine_save_json_data(position_status, file_path, default_structure=list)
-
 
 def generate_optimized_result(
     greeks: np.ndarray, weights: np.ndarray, idx: np.ndarray
 ) -> np.ndarray:
     optimized_result = np.round(
         (greeks[idx] * weights.reshape(-1, 1)).sum(
             axis=0,
```

### Comparing `volstreet-8.1.3/volstreet/strategies/optimization.py` & `volstreet-8.2.0/volstreet/strategies/optimization.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from scipy.optimize import minimize, dual_annealing
 import numpy as np
 from inspect import signature
-from volstreet import logger, OptimizationError
+from volstreet import logger, OptimizationError, Action
 from volstreet.blackscholes import find_strike_for_delta, gamma
 from pulp import LpProblem, LpMaximize, LpVariable, lpSum, lpDot, LpStatus, value
 
 
 def simulate_gamma_with_delta(
     spot: float,
     iv: float,
@@ -216,14 +216,54 @@
         f"Total Delta, Theta, Gamma: {value(call_total_delta + put_total_delta)}, "
         f"{value(call_total_theta + put_total_theta)}, {value(call_total_gamma + put_total_gamma)/g_scaler}"
     )
 
     return prob, combined_weights
 
 
+def trend_following_optimization_lp(
+    greeks: np.ndarray,
+    target_delta: float,
+    trend_direction: Action,
+):
+
+    prob, vars_dict = generate_base_problem(greeks)
+
+    call_total_delta = vars_dict["call"]["total_delta"]
+    call_total_theta = vars_dict["call"]["total_theta"]
+    call_total_gamma = vars_dict["call"]["total_gamma"]
+
+    put_total_delta = vars_dict["put"]["total_delta"]
+    put_total_theta = vars_dict["put"]["total_theta"]
+    put_total_gamma = vars_dict["put"]["total_gamma"]
+
+    # Converting the target delta to match the trend direction
+    target_delta = target_delta * trend_direction.num_value
+
+    # Creating the objectives
+
+    # Theta maximization
+    prob += (call_total_theta + put_total_theta) + (call_total_gamma + put_total_gamma)
+
+    # Delta constraint to capture the trend
+    if trend_direction == Action.BUY:
+        prob += (call_total_delta + put_total_delta) >= target_delta
+    else:
+        prob += (call_total_delta + put_total_delta) <= target_delta
+
+    # Solve the problem
+    prob.solve()
+
+    call_weights = np.array([v.varValue for v in vars_dict["call"]["weights"]])
+    put_weights = np.array([v.varValue for v in vars_dict["put"]["weights"]])
+    combined_weights = np.concatenate([call_weights, put_weights])
+
+    return prob, combined_weights
+
+
 def generate_constraints(
     deltas: np.ndarray,
     gammas: np.ndarray,
     max_delta: float,
     min_delta: float,
     min_gamma: float,
     max_gamma: float,
```

### Comparing `volstreet-8.1.3/volstreet/strategies/strats.py` & `volstreet-8.2.0/volstreet/strategies/strats.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 from datetime import datetime, timedelta, time
 from threading import Thread
 from time import sleep
 from typing import Optional
+import os
 from volstreet import config
 from volstreet.config import logger
 from volstreet.utils.core import (
     current_time,
     find_strike,
     time_to_expiry,
     check_for_weekend,
@@ -39,14 +40,15 @@
     cancel_pending_orders,
 )
 from volstreet.strategies.helpers import (
     sleep_until_next_action,
     round_shares_to_lot_size,
     most_equal_strangle,
     DeltaPosition,
+    TrendPosition,
     PositionMonitor,
     load_current_strangle,
     approve_execution,
     notify_pnl,
     process_stop_loss_order_statuses,
 )
 from volstreet.strategies.error_handling import exit_on_error
@@ -356,20 +358,28 @@
         f"exposure: {exposure}, "
         f"max qty: {max_qty_shares}, "
         f"base qty: {base_qty_shares}, "
         f"delta threshold: {delta_threshold}. "
     )
     notifier(starting_message, notification_url, "INFO")
 
+    # Setting the file path
+    date = current_time().strftime("%d-%m-%Y")
+    if data_directory is None:
+        file_path = f"{ActiveSession.obj.userId}\\{underlying.name.lower()}_delta_data\\{date}.json"
+    else:
+        file_path = os.path.join(data_directory, f"{date}.json")
+
     delta_position: DeltaPosition = DeltaPosition(
         underlying=underlying,
         base_exposure_qty=base_qty_shares,
         greek_settings={"theta_time_jump": theta_time_jump_hours / (365 * 24)},
         order_tag=strategy_tag,
         notifier_url=notification_url,
+        file_path=file_path,
     )
     delta_position.update_prospective_options(25, use_cache)
     while current_time().time() < time(*exit_time):
         delta_position.update_underlying()
         delta_position.set_recommended_qty(target_delta, optimized, optimize_gamma)
         delta_position.adjust_recommended_qty()
         delta_position.enter_positions(at_market=at_market)
@@ -389,15 +399,15 @@
         while not any(delta_position.exit_triggers.values()):
             sleep_until_next_action(
                 delta_interval_minutes,
                 exit_time,
                 special_condition=interruption_condition,
             )
             try:
-                delta_position.record_position_status(directory=data_directory)
+                delta_position.record_position_status()
             except Exception as e:
                 notifier(
                     f"{underlying.name} Error while recording position status: {e}\n"
                     f"Traceback: {e.__traceback__}",
                     notification_url,
                     "ERROR",
                 )
@@ -2375,14 +2385,215 @@
         underlying=underlying,
         notification_url=notification_url,
         additional_info=f"Profit pct: {combined_pnl_pct:0.2f}",
     )
     underlying.strategy_log[strategy_tag].extend(entries_log)
 
 
+def trend_v2(
+    underlying: Index | Stock,
+    exposure: int | float,
+    exit_time: tuple[int, int] = (15, 27),
+    threshold_movement: Optional[float] = None,
+    beta: Optional[float] = 0.8,
+    stop_loss: Optional[float] = 0.003,
+    hedge_offset: Optional[float | bool] = 0.004,
+    optimized: bool = False,
+    target_delta: float = 0.65,
+    theta_time_jump_hours: int = 6,  # In hours
+    max_entries: Optional[int] = 3,
+    at_market: bool = False,
+    notification_url: Optional[str] = None,
+    strategy_tag: Optional[str] = "Trend",
+    data_directory: Optional[str] = None,
+):
+    # Entering the main function
+    if time(*exit_time) < current_time().time():
+        notifier(
+            f"{underlying.name} {strategy_tag} not being deployed after exit time",
+            notification_url,
+            "INFO",
+        )
+        return
+
+    # Start time
+    start_time = current_time()
+
+    # Quantity
+    spot_price = underlying.fetch_ltp()
+    quantity_in_shares = round_shares_to_lot_size(
+        exposure / spot_price, underlying.lot_size
+    )
+
+    # Fetching open price
+    if current_time().time() > time(9, 18):
+        try:
+            open_time = current_time().replace(hour=9, minute=16, second=0)
+            open_price_data = fetch_historical_prices(
+                underlying.token, "ONE_MINUTE", open_time, open_time
+            )
+            open_price = open_price_data[0][1]
+        except Exception as e:
+            notifier(
+                f"Error in fetching historical prices: {e}",
+                notification_url,
+                "INFO",
+            )
+            open_price = underlying.fetch_ltp()
+    else:
+        while current_time().time() < time(9, 16):
+            sleep(1)
+        open_price = underlying.fetch_ltp()
+
+    # Threshold movement and price boundaries
+    threshold_movement = threshold_movement or (IndiaVix.fetch_ltp() * (beta or 1)) / 48
+    price_boundaries = [
+        open_price * (1 + ((-1) ** i) * threshold_movement / 100) for i in range(2)
+    ]
+
+    # Exit time
+    exit_time_object = time(*exit_time)
+    scan_end_time = (
+        datetime.combine(current_time().date(), exit_time_object)
+        - timedelta(minutes=10)
+    ).time()
+
+    # Setting the file path
+    date = current_time().strftime("%Y-%m-%d")
+    if data_directory is None:
+        file_path = f"{ActiveSession.obj.userId}\\{underlying.name.lower()}_trend_data\\{date}.json"
+    else:
+        file_path = os.path.join(data_directory, f"{date}.json")
+
+    # Initializing the trend position manager
+    greek_settings = {"theta_time_jump": theta_time_jump_hours / (365 * 24)}
+    trend_position = TrendPosition(
+        underlying=underlying,
+        base_exposure_qty=quantity_in_shares,
+        greek_settings=greek_settings,
+        notifier_url=notification_url,
+        order_tag=strategy_tag,
+        file_path=file_path,
+    )
+    trend_position.update_prospective_options(
+        range_of_strikes=20, options_with_cache=True
+    )
+
+    notifier(
+        f"{underlying.name} trend following starting with {threshold_movement:0.2f} threshold movement\n"
+        f"Current Price: {open_price}\nUpper limit: {price_boundaries[0]:0.2f}\n"
+        f"Lower limit: {price_boundaries[1]:0.2f}.",
+        notification_url,
+        "INFO",
+    )
+    entries = 0
+    movement = 0
+    while entries < max_entries and current_time().time() < exit_time_object:
+        # Scan for entry condition
+        notifier(
+            f"{underlying.name} trender {entries+1} scanning for entry condition.",
+            notification_url,
+            "INFO",
+        )
+        while current_time().time() < scan_end_time:
+            ltp = underlying.fetch_ltp()
+            movement = (ltp - open_price) / open_price * 100
+            if abs(movement) > threshold_movement:
+                break
+            sleep_until_next_action(1, exit_time)
+
+        if current_time().time() >= scan_end_time:
+            notifier(
+                f"{underlying.name} trender {entries+1} exiting due to time.",
+                notification_url,
+                "CRUCIAL",
+            )
+            break
+
+        # Entry condition met taking position
+        price = underlying.fetch_ltp()
+        action: Action = Action.BUY if movement > 0 else Action.SELL
+        stop_loss_price = price * (
+            (1 - stop_loss) if action == Action.BUY else (1 + stop_loss)
+        )
+        notifier(
+            f"{underlying.name} {action} trender triggered with {movement:0.2f} movement. "
+            f"{underlying.name} at {price}. "
+            f"Stop loss at {stop_loss_price}.",
+            notification_url,
+            "INFO",
+        )
+
+        # Set quantities and enter the position
+        trend_position.set_recommended_qty(
+            optimized=optimized,
+            target_delta=target_delta,
+            trend_direction=action,
+            hedge_offset=hedge_offset,
+        )
+        trend_position.enter_positions(at_market=at_market)
+
+        notifier(
+            f"{underlying.name} {action} trender {entries+1} entered.",
+            notification_url,
+            "INFO",
+        )
+
+        # Monitoring begins
+        stop_loss_hit = False
+        early_exit = False
+        # 15% of the quantity will be the delta threshold
+        exit_threshold = 0.15 * quantity_in_shares
+        while current_time().time() < exit_time_object:
+            sleep_until_next_action(1, exit_time)
+            trend_position.record_position_status()
+            ltp = underlying.fetch_ltp()
+            movement = (ltp - open_price) / open_price * 100
+            stop_loss_hit = (
+                (ltp < stop_loss_price)
+                if action == Action.BUY
+                else (ltp > stop_loss_price)
+            )
+            if stop_loss_hit:
+                break
+            if abs(trend_position.aggregate_greeks().delta) < exit_threshold:
+                notifier(
+                    f"{underlying.name} trender {entries+1} delta threshold hit.",
+                    notification_url,
+                    "INFO",
+                )
+                early_exit = True
+                break
+
+        # Exit condition met exiting position (stop loss or time)
+        stop_loss_message = f"Trender stop loss hit. " if stop_loss_hit else ""
+        notifier(
+            f"{stop_loss_message}{underlying.name} trender {entries+1} exiting.",
+            notification_url,
+            "CRUCIAL",
+        )
+        trend_position.exit_positions(at_market=at_market)
+        notifier(
+            f"{underlying.name} {action} trender {entries+1} exited.",
+            notification_url,
+            "INFO",
+        )
+        entries += 1
+        if early_exit:
+            break
+
+    notify_pnl(
+        "trend",
+        start_time=start_time,
+        underlying=underlying,
+        notification_url=notification_url,
+        additional_info=f"Exposure: {exposure}.",
+    )
+
+
 def reentry_straddle(
     underlying: Index | Stock,
     exposure: int | float,
     exit_time: tuple[int, int] = (15, 29),
     stop_loss: Optional[float] = 0.5,
     at_market: bool = False,
     notification_url: Optional[str] = None,
@@ -2427,14 +2638,20 @@
     expiry = underlying.current_expiry
     quantity_in_lots = convert_exposure_to_lots(
         exposure, spot_price, underlying.lot_size
     )
 
     straddle = Straddle(atm_strike, underlying.name, expiry)
 
+    notifier(
+        f"{underlying.name} {strategy_tag} starting with straddle {straddle}",
+        notification_url,
+        "INFO",
+    )
+
     # Placing the main order
     execution_details = execute_instructions(
         {
             straddle: {
                 "action": Action.SELL,
                 "quantity_in_lots": quantity_in_lots,
                 "order_tag": strategy_tag,
@@ -2459,14 +2676,21 @@
         if neutral:
             call_ltp, put_ltp = straddle.fetch_ltp()
             call_sl_hit = call_ltp > call_sl_price
             put_sl_hit = put_ltp > put_sl_price
             if call_sl_hit and put_sl_hit:
                 raise ValueError("Both stop losses hit for some reason")
             elif call_sl_hit or put_sl_hit:
+                notifier(
+                    f"{underlying.name} {strategy_tag} stop loss hit. "
+                    f"Call SL: {call_sl_hit}, Put SL: {put_sl_hit}. "
+                    f"State changed to directional.",
+                    notification_url,
+                    "CRUCIAL",
+                )
                 option_to_exit = (
                     straddle.call_option if call_sl_hit else straddle.put_option
                 )
                 option_exit_price = exit_option(option_to_exit, quantity_in_lots)
                 neutral = False
 
         else:
@@ -2477,40 +2701,52 @@
                 else (straddle.put_option, put_avg_price)
             )
             reentry_condition = (
                 reentry_option.fetch_ltp() < reentry_check_price
             ) and reattempt_bank[reentry_option] > 0
 
             if reentry_condition:
+                notifier(
+                    f"{underlying.name} {strategy_tag} reentry condition met. "
+                    f"Reentering {reentry_option}.",
+                    notification_url,
+                    "INFO",
+                )
                 option_entry_price = reenter_option(reentry_option, quantity_in_lots)
                 reattempt_bank[reentry_option] -= 1
                 neutral = True
 
             # Second type of condition is trend condition
             trend_option, trend_sl_price = (
                 (straddle.put_option, put_sl_price)
                 if call_sl_hit
                 else (straddle.call_option, call_sl_price)
             )
             trend_sl_hit = trend_option.fetch_ltp() > trend_sl_price
 
             if trend_sl_hit:
+                notifier(
+                    f"{underlying.name} {strategy_tag} trend stop loss hit.",
+                    notification_url,
+                    "CRUCIAL",
+                )
                 exit_option(trend_option, quantity_in_lots)
                 # The below condition basically means that the trend option has switched
                 # Happens in the rare case that there is a significant movement
                 # in the opposite direction of the trend
                 if reentry_condition:
                     # We have already reentered the reentry option
                     # And exited the trend option
                     # We just need to change the flags
                     call_sl_hit, put_sl_hit = put_sl_hit, call_sl_hit
                     neutral = False
                     continue
                 break
 
+    notifier(f"{underlying.name} {strategy_tag} exiting.", notification_url, "INFO")
     # Exit open positions if any
     if neutral:
         # Exit the strangle
         execution_details = execute_instructions(
             {
                 straddle: {
                     "action": Action.BUY,
```

### Comparing `volstreet-8.1.3/volstreet/trade_interface/instruments.py` & `volstreet-8.2.0/volstreet/trade_interface/instruments.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/trade_interface/order_execution.py` & `volstreet-8.2.0/volstreet/trade_interface/order_execution.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/trade_interface/underlyings.py` & `volstreet-8.2.0/volstreet/trade_interface/underlyings.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,14 @@
     """Initialize an index with the name of the index in uppercase"""
 
     def __init__(self, name, caching=False):
         self.name = name.upper()
         self.current_expiry = None
         self.next_expiry = None
         self.far_expiry = None
-        self.month_expiry = None
-        self.fut_expiry = None
         self.exchange = "BSE" if self.name in ["SENSEX", "BANKEX"] else "NSE"
         self.fno_exchange = "BFO" if self.name in ["SENSEX", "BANKEX"] else "NFO"
         self.symbol, self.token = get_symbol_token(self.name)
         self.future_symbol_tokens = {}
         self.fetch_exps()
         self.lot_size = get_lot_size(self.name, self.current_expiry)
         self.freeze_qty = self.fetch_freeze_limit()
@@ -104,19 +102,14 @@
         exps = get_expiry_dates(self.name)
         exps = pd.DatetimeIndex(exps).strftime("%d%b%y").str.upper().tolist()
 
         self.current_expiry = exps[0]
         self.next_expiry = exps[1]
         self.far_expiry = exps[2]
 
-        if self.name in config.EXPIRY_FREQUENCIES:
-            self.fut_expiry = self.month_expiry = exps[3]
-        else:
-            self.fut_expiry = self.month_expiry = exps[0]
-
     def set_future_symbol_tokens(self):
         if not self.future_symbol_tokens:
             for i in range(0, 3):
                 try:
                     self.future_symbol_tokens[i] = get_symbol_token(self.name, future=i)
                 except ScripsLocationError:
                     self.future_symbol_tokens[i] = (None, None)
@@ -229,17 +222,14 @@
         self._last_basis_fetch_time = current_time()
         return adjusted_annualized_basis
 
     def fetch_atm_info(self, expiry="current", effective_iv=False):
         expiry_dict = {
             "current": self.current_expiry,
             "next": self.next_expiry,
-            "month": self.month_expiry,
-            "future": self.fut_expiry,
-            "fut": self.fut_expiry,
         }
         expiry = expiry_dict[expiry]
         price = self.fetch_ltp()
         atm_straddle = self.get_strangle(expiry, price)
         call_price, put_price = atm_straddle.fetch_ltp()
         synthetic_price = atm_straddle.strike + call_price - put_price
         r = self.get_basis_for_expiry(expiry, price, synthetic_price)
@@ -260,17 +250,14 @@
             "avg_iv": avg_iv,
         }
 
     def fetch_otm_info(self, strike_offset, expiry="current", effective_iv=False):
         expiry_dict = {
             "current": self.current_expiry,
             "next": self.next_expiry,
-            "month": self.month_expiry,
-            "future": self.fut_expiry,
-            "fut": self.fut_expiry,
         }
         expiry = expiry_dict[expiry]
         price = self.fetch_ltp()
         call_strike = price * (1 + strike_offset)
         put_strike = price * (1 - strike_offset)
         call_strike = find_strike(call_strike, self.base)
         put_strike = find_strike(put_strike, self.base)
@@ -536,14 +523,17 @@
 
             else:
                 raise ValueError(f"Index {name} not found")
         super().__init__(name)
 
 
 class IndiaVix:
-    symbol, token = None, None
+    if config.backtest_mode:
+        symbol, token = "India Vix", "India Vix"
+    else:
+        symbol, token = None, None
 
     @classmethod
     def fetch_ltp(cls):
         if cls.symbol is None or cls.token is None:
             cls.symbol, cls.token = get_symbol_token("INDIA VIX")
         return fetch_ltp("NSE", cls.symbol, cls.token)
```

### Comparing `volstreet-8.1.3/volstreet/utils/change_config.py` & `volstreet-8.2.0/volstreet/utils/change_config.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/utils/communication.py` & `volstreet-8.2.0/volstreet/utils/communication.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/utils/core.py` & `volstreet-8.2.0/volstreet/utils/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pandas as pd
 import numpy as np
 import math
 from datetime import datetime, timedelta, timezone, time
 import re
 import functools
+import calendar
 from inspect import signature
 from volstreet.config import holidays, logger
 from volstreet import config
 
 
 def word_to_num(s):
     word = {
@@ -348,15 +349,52 @@
         + sell_gst
     )
     charges_per_share = total_charges / (num_contracts * contract_size)
 
     return round(charges_per_share, 1)
 
 
+def _parse_bse_symbol(
+    symbol, index: str
+):  # todo check how months higher than 9 are handled and adapt it
+
+    if len(symbol.lstrip(index)) != 12:
+        logger.warning("BSE symbol is of unexpected length")
+        return None
+
+    pattern_one_digit_month = r"(\w+)(\d{2})(\d{1})(\d{2})(\d{5})(\w{2})"
+    # pattern_two_digit_month = r"(\w+)(\d{2})(\d{2})(\d{2})(\d{5})(\w+)"
+
+    # First try with the assumption that the month has one digit
+    match = re.match(pattern_one_digit_month, symbol)
+    if match:
+        name, year, month, day, strike, option_type = match.groups()
+        month = month.zfill(2)  # Zero-pad the month
+
+        # Format the expiry date
+        expiry_date = f"{day}{calendar.month_abbr[int(month)]}{year}"
+
+        return name, expiry_date.upper(), strike, option_type
+    else:
+        return None
+
+    # else:
+    #     # Try with the assumption that the month has two digits
+    #     match = re.match(pattern_two_digit_month, symbol)
+    #     if match:
+    #         name, year, month, day, strike, option_type = match.groups()
+    #     else:
+    #         return None  # Return None if both patterns fail
+
+
 def parse_symbol(symbol):
+
+    if symbol.startswith("SENSEX") or symbol.startswith("BANKEX"):
+        return _parse_bse_symbol(symbol, re.search(r"([A-Za-z]+)", symbol).group(1))
+
     match = re.match(r"([A-Za-z]+)(\d{2}[A-Za-z]{3}\d{2})(\d+)(\w+)", symbol)
     if match:
         return match.groups()
     return None
 
 
 def get_background_tasks(obj: object, task_name: str):
```

### Comparing `volstreet-8.1.3/volstreet/utils/data_io.py` & `volstreet-8.2.0/volstreet/utils/data_io.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/utils/scrip_processing.py` & `volstreet-8.2.0/volstreet/utils/scrip_processing.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/vectorized_blackscholes.py` & `volstreet-8.2.0/volstreet/vectorized_blackscholes.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/vslogging/formatters.py` & `volstreet-8.2.0/volstreet/vslogging/formatters.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/vslogging/logging_config.json` & `volstreet-8.2.0/volstreet/vslogging/logging_config.json`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/vslogging/logging_setup.py` & `volstreet-8.2.0/volstreet/vslogging/logging_setup.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet/vslogging/parsing.py` & `volstreet-8.2.0/volstreet/vslogging/parsing.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.1.3/volstreet.egg-info/PKG-INFO` & `volstreet-8.2.0/volstreet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volstreet
-Version: 8.1.3
+Version: 8.2.0
 Summary: VolStreet is a Python library for automated trading
 Home-page: https://github.com/rahulthakkr/volstreet
 Author: Rahul Thakkar
 Author-email: r.thakkar15@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `volstreet-8.1.3/volstreet.egg-info/SOURCES.txt` & `volstreet-8.2.0/volstreet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

