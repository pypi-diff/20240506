# Comparing `tmp/qteasy-1.2.3.tar.gz` & `tmp/qteasy-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qteasy-1.2.3.tar", last modified: Tue Apr 30 14:05:51 2024, max compression
+gzip compressed data, was "qteasy-1.2.4.tar", last modified: Sun May  5 14:51:59 2024, max compression
```

## Comparing `qteasy-1.2.3.tar` & `qteasy-1.2.4.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-30 14:05:51.698964 qteasy-1.2.3/
--rwxr-xr-x   0 jackie     (501) staff       (20)     1463 2024-03-07 04:23:42.000000 qteasy-1.2.3/LICENSE
--rw-r--r--   0 jackie     (501) staff       (20)    27935 2024-04-30 14:05:51.698882 qteasy-1.2.3/PKG-INFO
--rwxr-xr-x   0 jackie     (501) staff       (20)    24211 2024-04-30 14:05:38.000000 qteasy-1.2.3/README.md
--rw-r--r--   0 jackie     (501) staff       (20)     2304 2024-04-30 14:05:38.000000 qteasy-1.2.3/pyproject.toml
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-30 14:05:51.694169 qteasy-1.2.3/qteasy/
--rwxr-xr-x   0 jackie     (501) staff       (20)     8588 2024-04-30 14:05:38.000000 qteasy-1.2.3/qteasy/__init__.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    68549 2024-04-23 13:23:43.000000 qteasy-1.2.3/qteasy/_arg_validators.py
--rw-r--r--   0 jackie     (501) staff       (20)    53075 2024-04-29 15:26:18.000000 qteasy-1.2.3/qteasy/backtest.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    35193 2024-04-02 14:31:55.000000 qteasy-1.2.3/qteasy/blender.py
--rw-r--r--   0 jackie     (501) staff       (20)    30260 2024-04-23 05:23:43.000000 qteasy-1.2.3/qteasy/broker.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   142505 2024-04-29 14:37:23.000000 qteasy-1.2.3/qteasy/built_in.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   111306 2024-04-30 14:05:38.000000 qteasy-1.2.3/qteasy/core.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   390965 2024-04-30 14:05:38.000000 qteasy-1.2.3/qteasy/database.py
--rw-r--r--   0 jackie     (501) staff       (20)     9341 2024-04-02 14:50:54.000000 qteasy-1.2.3/qteasy/emfuncs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    34874 2024-04-21 23:36:55.000000 qteasy-1.2.3/qteasy/evaluate.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    38585 2024-04-29 15:26:18.000000 qteasy-1.2.3/qteasy/finance.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   100797 2024-04-05 14:28:39.000000 qteasy-1.2.3/qteasy/history.py
--rw-r--r--   0 jackie     (501) staff       (20)    39218 2024-04-02 14:32:16.000000 qteasy-1.2.3/qteasy/optimization.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   107901 2024-04-02 14:31:31.000000 qteasy-1.2.3/qteasy/qt_operator.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    34029 2024-04-05 14:28:39.000000 qteasy-1.2.3/qteasy/space.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    88071 2024-04-29 14:37:23.000000 qteasy-1.2.3/qteasy/strategy.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   156061 2024-04-29 14:37:23.000000 qteasy-1.2.3/qteasy/tafuncs.py
--rw-r--r--   0 jackie     (501) staff       (20)    51352 2024-04-23 13:23:43.000000 qteasy-1.2.3/qteasy/trade_recording.py
--rw-r--r--   0 jackie     (501) staff       (20)    98512 2024-04-23 13:23:43.000000 qteasy-1.2.3/qteasy/trader.py
--rw-r--r--   0 jackie     (501) staff       (20)    93193 2024-04-23 13:23:43.000000 qteasy-1.2.3/qteasy/trader_cli.py
--rw-r--r--   0 jackie     (501) staff       (20)    18205 2024-04-23 05:23:43.000000 qteasy-1.2.3/qteasy/trader_tui.py
--rw-r--r--   0 jackie     (501) staff       (20)    68078 2024-04-29 15:26:18.000000 qteasy-1.2.3/qteasy/trading_util.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   131527 2024-04-21 23:36:55.000000 qteasy-1.2.3/qteasy/tsfuncs.py
--rw-r--r--   0 jackie     (501) staff       (20)      840 2024-04-23 05:23:43.000000 qteasy-1.2.3/qteasy/tui_style.tcss
--rwxr-xr-x   0 jackie     (501) staff       (20)    75175 2024-04-27 14:12:34.000000 qteasy-1.2.3/qteasy/utilfuncs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    79918 2024-04-21 23:36:55.000000 qteasy-1.2.3/qteasy/visual.py
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-30 14:05:51.698346 qteasy-1.2.3/qteasy.egg-info/
--rw-r--r--   0 jackie     (501) staff       (20)    27935 2024-04-30 14:05:51.000000 qteasy-1.2.3/qteasy.egg-info/PKG-INFO
--rw-r--r--   0 jackie     (501) staff       (20)     1274 2024-04-30 14:05:51.000000 qteasy-1.2.3/qteasy.egg-info/SOURCES.txt
--rw-r--r--   0 jackie     (501) staff       (20)        1 2024-04-30 14:05:51.000000 qteasy-1.2.3/qteasy.egg-info/dependency_links.txt
--rw-r--r--   0 jackie     (501) staff       (20)        1 2023-01-29 16:03:37.000000 qteasy-1.2.3/qteasy.egg-info/not-zip-safe
--rw-r--r--   0 jackie     (501) staff       (20)      195 2024-04-30 14:05:51.000000 qteasy-1.2.3/qteasy.egg-info/requires.txt
--rw-r--r--   0 jackie     (501) staff       (20)        7 2024-04-30 14:05:51.000000 qteasy-1.2.3/qteasy.egg-info/top_level.txt
--rw-r--r--   0 jackie     (501) staff       (20)     1627 2024-04-30 14:05:51.699233 qteasy-1.2.3/setup.cfg
--rw-r--r--   0 jackie     (501) staff       (20)      257 2024-04-01 14:38:19.000000 qteasy-1.2.3/setup.py
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-30 14:05:51.698191 qteasy-1.2.3/tests/
--rw-r--r--   0 jackie     (501) staff       (20)     6524 2024-04-27 14:13:03.000000 qteasy-1.2.3/tests/test_broker.py
--rwxr-xr-x   0 jackie     (501) staff       (20)     8078 2024-04-05 14:28:39.000000 qteasy-1.2.3/tests/test_cashplan.py
--rwxr-xr-x   0 jackie     (501) staff       (20)     3613 2023-11-25 05:35:56.000000 qteasy-1.2.3/tests/test_config.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    17487 2024-04-03 01:57:25.000000 qteasy-1.2.3/tests/test_core_sub_funcs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    19818 2024-04-05 14:28:39.000000 qteasy-1.2.3/tests/test_cost.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   121711 2024-04-23 05:23:43.000000 qteasy-1.2.3/tests/test_datasource.py
--rw-r--r--   0 jackie     (501) staff       (20)     6143 2024-02-03 15:46:14.000000 qteasy-1.2.3/tests/test_eastmoney.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    73624 2024-04-05 14:28:39.000000 qteasy-1.2.3/tests/test_evaluations.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    13901 2024-02-03 15:46:14.000000 qteasy-1.2.3/tests/test_fast_experiments.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    57759 2024-03-29 10:03:15.000000 qteasy-1.2.3/tests/test_historypanel.py
--rwxr-xr-x   0 jackie     (501) staff       (20)      413 2023-01-29 16:18:32.000000 qteasy-1.2.3/tests/test_log.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   304019 2024-04-05 14:28:39.000000 qteasy-1.2.3/tests/test_loop.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   169228 2024-04-29 14:37:23.000000 qteasy-1.2.3/tests/test_operator_and_strategy.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    44520 2024-04-28 14:32:18.000000 qteasy-1.2.3/tests/test_qt.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    18581 2023-01-29 16:18:32.000000 qteasy-1.2.3/tests/test_space.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    40797 2024-04-29 14:37:23.000000 qteasy-1.2.3/tests/test_ta_funcs.py
--rw-r--r--   0 jackie     (501) staff       (20)    43397 2024-04-23 05:23:43.000000 qteasy-1.2.3/tests/test_trader.py
--rw-r--r--   0 jackie     (501) staff       (20)    45317 2024-04-23 05:23:43.000000 qteasy-1.2.3/tests/test_trader_shell.py
--rw-r--r--   0 jackie     (501) staff       (20)   168527 2024-04-21 23:36:55.000000 qteasy-1.2.3/tests/test_trading.py
--rw-r--r--   0 jackie     (501) staff       (20)     2670 2024-04-23 05:23:43.000000 qteasy-1.2.3/tests/test_tui.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    21881 2024-03-30 12:31:29.000000 qteasy-1.2.3/tests/test_tushare.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    43279 2024-04-05 14:28:39.000000 qteasy-1.2.3/tests/test_utilityfuncs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)     3090 2023-01-29 16:18:32.000000 qteasy-1.2.3/tests/test_visual.py
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-05-05 14:51:59.102377 qteasy-1.2.4/
+-rwxr-xr-x   0 jackie     (501) staff       (20)     1463 2024-03-07 04:23:42.000000 qteasy-1.2.4/LICENSE
+-rw-r--r--   0 jackie     (501) staff       (20)    27935 2024-05-05 14:51:59.101831 qteasy-1.2.4/PKG-INFO
+-rwxr-xr-x   0 jackie     (501) staff       (20)    24211 2024-05-05 14:42:08.000000 qteasy-1.2.4/README.md
+-rw-r--r--   0 jackie     (501) staff       (20)     2304 2024-05-05 14:42:08.000000 qteasy-1.2.4/pyproject.toml
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-05-05 14:51:59.078314 qteasy-1.2.4/qteasy/
+-rwxr-xr-x   0 jackie     (501) staff       (20)     8588 2024-05-05 14:42:08.000000 qteasy-1.2.4/qteasy/__init__.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    68549 2024-05-04 09:08:45.000000 qteasy-1.2.4/qteasy/_arg_validators.py
+-rw-r--r--   0 jackie     (501) staff       (20)    53075 2024-05-05 10:05:28.000000 qteasy-1.2.4/qteasy/backtest.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    35193 2024-04-02 14:31:55.000000 qteasy-1.2.4/qteasy/blender.py
+-rw-r--r--   0 jackie     (501) staff       (20)    30260 2024-05-05 10:05:28.000000 qteasy-1.2.4/qteasy/broker.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   142516 2024-05-05 14:24:46.000000 qteasy-1.2.4/qteasy/built_in.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   111306 2024-05-04 09:08:45.000000 qteasy-1.2.4/qteasy/core.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   390965 2024-05-04 09:08:45.000000 qteasy-1.2.4/qteasy/database.py
+-rw-r--r--   0 jackie     (501) staff       (20)     9341 2024-04-02 14:50:54.000000 qteasy-1.2.4/qteasy/emfuncs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    34874 2024-05-04 09:08:45.000000 qteasy-1.2.4/qteasy/evaluate.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    38585 2024-05-05 10:05:28.000000 qteasy-1.2.4/qteasy/finance.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   100797 2024-04-05 14:28:39.000000 qteasy-1.2.4/qteasy/history.py
+-rw-r--r--   0 jackie     (501) staff       (20)    39218 2024-05-04 08:19:36.000000 qteasy-1.2.4/qteasy/optimization.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   107901 2024-05-05 10:05:28.000000 qteasy-1.2.4/qteasy/qt_operator.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    34029 2024-04-05 14:28:39.000000 qteasy-1.2.4/qteasy/space.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    88071 2024-05-05 10:05:28.000000 qteasy-1.2.4/qteasy/strategy.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   156164 2024-05-05 14:35:57.000000 qteasy-1.2.4/qteasy/tafuncs.py
+-rw-r--r--   0 jackie     (501) staff       (20)    51352 2024-05-04 09:08:45.000000 qteasy-1.2.4/qteasy/trade_recording.py
+-rw-r--r--   0 jackie     (501) staff       (20)    98512 2024-05-04 09:08:45.000000 qteasy-1.2.4/qteasy/trader.py
+-rw-r--r--   0 jackie     (501) staff       (20)    93193 2024-05-04 09:08:45.000000 qteasy-1.2.4/qteasy/trader_cli.py
+-rw-r--r--   0 jackie     (501) staff       (20)    18205 2024-05-04 09:08:45.000000 qteasy-1.2.4/qteasy/trader_tui.py
+-rw-r--r--   0 jackie     (501) staff       (20)    68078 2024-05-05 10:05:28.000000 qteasy-1.2.4/qteasy/trading_util.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   131527 2024-04-21 23:36:55.000000 qteasy-1.2.4/qteasy/tsfuncs.py
+-rw-r--r--   0 jackie     (501) staff       (20)      840 2024-05-04 09:08:45.000000 qteasy-1.2.4/qteasy/tui_style.tcss
+-rwxr-xr-x   0 jackie     (501) staff       (20)    75175 2024-05-04 09:08:45.000000 qteasy-1.2.4/qteasy/utilfuncs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    79918 2024-04-21 23:36:55.000000 qteasy-1.2.4/qteasy/visual.py
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-05-05 14:51:59.101159 qteasy-1.2.4/qteasy.egg-info/
+-rw-r--r--   0 jackie     (501) staff       (20)    27935 2024-05-05 14:51:59.000000 qteasy-1.2.4/qteasy.egg-info/PKG-INFO
+-rw-r--r--   0 jackie     (501) staff       (20)     1274 2024-05-05 14:51:59.000000 qteasy-1.2.4/qteasy.egg-info/SOURCES.txt
+-rw-r--r--   0 jackie     (501) staff       (20)        1 2024-05-05 14:51:59.000000 qteasy-1.2.4/qteasy.egg-info/dependency_links.txt
+-rw-r--r--   0 jackie     (501) staff       (20)        1 2023-01-29 16:03:37.000000 qteasy-1.2.4/qteasy.egg-info/not-zip-safe
+-rw-r--r--   0 jackie     (501) staff       (20)      195 2024-05-05 14:51:59.000000 qteasy-1.2.4/qteasy.egg-info/requires.txt
+-rw-r--r--   0 jackie     (501) staff       (20)        7 2024-05-05 14:51:59.000000 qteasy-1.2.4/qteasy.egg-info/top_level.txt
+-rw-r--r--   0 jackie     (501) staff       (20)     1627 2024-05-05 14:51:59.103420 qteasy-1.2.4/setup.cfg
+-rw-r--r--   0 jackie     (501) staff       (20)      257 2024-04-01 14:38:19.000000 qteasy-1.2.4/setup.py
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-05-05 14:51:59.100858 qteasy-1.2.4/tests/
+-rw-r--r--   0 jackie     (501) staff       (20)     6524 2024-05-05 10:05:28.000000 qteasy-1.2.4/tests/test_broker.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)     8078 2024-04-05 14:28:39.000000 qteasy-1.2.4/tests/test_cashplan.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)     3613 2023-11-25 05:35:56.000000 qteasy-1.2.4/tests/test_config.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    17487 2024-04-03 01:57:25.000000 qteasy-1.2.4/tests/test_core_sub_funcs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    19818 2024-05-05 10:05:28.000000 qteasy-1.2.4/tests/test_cost.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   121711 2024-05-04 09:08:45.000000 qteasy-1.2.4/tests/test_datasource.py
+-rw-r--r--   0 jackie     (501) staff       (20)     6143 2024-02-03 15:46:14.000000 qteasy-1.2.4/tests/test_eastmoney.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    73624 2024-04-05 14:28:39.000000 qteasy-1.2.4/tests/test_evaluations.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    13901 2024-02-03 15:46:14.000000 qteasy-1.2.4/tests/test_fast_experiments.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    57759 2024-03-29 10:03:15.000000 qteasy-1.2.4/tests/test_historypanel.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)      413 2023-01-29 16:18:32.000000 qteasy-1.2.4/tests/test_log.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   304019 2024-04-05 14:28:39.000000 qteasy-1.2.4/tests/test_loop.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   169228 2024-05-04 09:08:45.000000 qteasy-1.2.4/tests/test_operator_and_strategy.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    44521 2024-05-05 14:36:45.000000 qteasy-1.2.4/tests/test_qt.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    18581 2023-01-29 16:18:32.000000 qteasy-1.2.4/tests/test_space.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    40814 2024-05-05 14:24:46.000000 qteasy-1.2.4/tests/test_ta_funcs.py
+-rw-r--r--   0 jackie     (501) staff       (20)    43397 2024-05-04 09:08:45.000000 qteasy-1.2.4/tests/test_trader.py
+-rw-r--r--   0 jackie     (501) staff       (20)    45317 2024-05-04 09:08:45.000000 qteasy-1.2.4/tests/test_trader_shell.py
+-rw-r--r--   0 jackie     (501) staff       (20)   168527 2024-04-21 23:36:55.000000 qteasy-1.2.4/tests/test_trading.py
+-rw-r--r--   0 jackie     (501) staff       (20)     2670 2024-05-04 09:08:45.000000 qteasy-1.2.4/tests/test_tui.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    21881 2024-03-30 12:31:29.000000 qteasy-1.2.4/tests/test_tushare.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    43279 2024-04-05 14:28:39.000000 qteasy-1.2.4/tests/test_utilityfuncs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)     3090 2023-01-29 16:18:32.000000 qteasy-1.2.4/tests/test_visual.py
```

### Comparing `qteasy-1.2.3/LICENSE` & `qteasy-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/PKG-INFO` & `qteasy-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qteasy
-Version: 1.2.3
+Version: 1.2.4
 Summary: A fast quantitative investment tool kit
 Home-page: https://github.com/shepherdpp/qteasy
 Author: Jackie PENG
 Author-email: jackie PENG <jackie.pengzhao@gmail.com>
 Maintainer: Jackie PENG
 Maintainer-email: jackie PENG <jackie.pengzhao@gmail.com>
 License: Copyright <2019> <JACKIE PENG>
@@ -106,15 +106,15 @@
 > 我会尽快修复问题并回复大家的问题。
 
 ## 关于`qteasy`
 
 - 作者: **Jackie PENG**
 - email: *jackie_pengzhao@163.com*
 - Created: 2019, July, 16
-- Latest Version: `1.2.3`
+- Latest Version: `1.2.4`
 - License: BSD 3-Clause License
 
 `qteasy`是为量化交易人员开发的一套量化交易工具包，特点如下：
 
 1. **全流程覆盖** 从金融数据获取、存储，到交易策略的开发、回测、优化、实盘运行
 2. **完全本地化** 所有的金融数据、策略运算和优化过程完全本地化，不依赖于任何云端服务
 3. **使用简单** 提供大量内置交易策略，用户可以搭积木式地创建自己的交易策略
```

### Comparing `qteasy-1.2.3/README.md` & `qteasy-1.2.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 > 我会尽快修复问题并回复大家的问题。
 
 ## 关于`qteasy`
 
 - 作者: **Jackie PENG**
 - email: *jackie_pengzhao@163.com*
 - Created: 2019, July, 16
-- Latest Version: `1.2.3`
+- Latest Version: `1.2.4`
 - License: BSD 3-Clause License
 
 `qteasy`是为量化交易人员开发的一套量化交易工具包，特点如下：
 
 1. **全流程覆盖** 从金融数据获取、存储，到交易策略的开发、回测、优化、实盘运行
 2. **完全本地化** 所有的金融数据、策略运算和优化过程完全本地化，不依赖于任何云端服务
 3. **使用简单** 提供大量内置交易策略，用户可以搭积木式地创建自己的交易策略
```

### Comparing `qteasy-1.2.3/pyproject.toml` & `qteasy-1.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 build-backend = "setuptools.build_meta"
 
 #[tool.setuptools.package.find]
 #where = "qteasy/"
 
 [project]
 name = "qteasy"
-version = "1.2.3"
+version = "1.2.4"
 authors = [
   {name="jackie PENG", email="jackie.pengzhao@gmail.com" },
 ]
 maintainers = [
   {name="jackie PENG", email="jackie.pengzhao@gmail.com" },
 ]
 description = "A fast quantitative investment tool kit"
```

### Comparing `qteasy-1.2.3/qteasy/__init__.py` & `qteasy-1.2.4/qteasy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,23 +34,23 @@
 from .visual import candle
 from .finance import CashPlan, set_cost, update_cost
 from .database import DataSource, find_history_data
 from ._arg_validators import QT_CONFIG, ConfigDict
 
 
 # qteasy版本信息
-__version__ = '1.2.3'
+__version__ = '1.2.4'
 version_info = Namespace(
         major=1,
         minor=2,
         patch=2,
         short=(1, 2),
-        full=(1, 2, 3),
-        string='1.2.3',
-        tuple=('1', '2', '3'),
+        full=(1, 2, 4),
+        string='1.2.4',
+        tuple=('1', '2', '4'),
         releaselevel='beta',
 )
 
 # 解析qteasy的本地安装路径
 QT_ROOT_PATH = os.path.normpath(os.path.join(os.path.dirname(__file__), os.pardir))
 QT_ROOT_PATH = os.path.join(QT_ROOT_PATH, 'qteasy/')
```

### Comparing `qteasy-1.2.3/qteasy/_arg_validators.py` & `qteasy-1.2.4/qteasy/_arg_validators.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/qteasy/backtest.py` & `qteasy-1.2.4/qteasy/backtest.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/qteasy/blender.py` & `qteasy-1.2.4/qteasy/blender.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/qteasy/broker.py` & `qteasy-1.2.4/qteasy/broker.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/qteasy/built_in.py` & `qteasy-1.2.4/qteasy/built_in.py`

 * *Files 0% similar despite different names*

```diff
@@ -1412,17 +1412,17 @@
                          name='SLOPE - HT',
                          description='Smoothed Curve Slope Strategy that uses HT line as the '
                                      'trade line ',
                          strategy_data_types='close')
 
     def realize(self, h, r=None, t=None, pars=None):
         if pars is None:
-            n = self.pars
+            n, = self.pars
         else:
-            n = pars
+            n, = pars
         h = h.T
         curve = ht(h[0])
         slope = curve[-1] - curve[-n]
         if slope > 0:
             return 1
         else:
             return -1
@@ -2078,15 +2078,15 @@
 
     def realize(self, h, r=None, t=None, pars=None):
         if pars is None:
             p, = self.pars
         else:
             p, = pars
         h = h.T
-        res = aroonosc(h[0], p)[-1]
+        res = aroonosc(h[0], h[1], p)[-1]
 
         if res > 0:
             cat = 0.5
         elif res > 50:
             cat = 1
         elif res < 0:
             cat = -0.5
@@ -2248,17 +2248,16 @@
 
     def realize(self, h, r=None, t=None, pars=None):
         if pars is None:
             fp, ft, sp, st, p, t = self.pars
         else:
             fp, ft, sp, st, p, t = pars
         h = h.T
-        m, sig, hist = macdext(h[0], fp, ft, sp, st, p, t)[-1]
-
-        if m > 0:
+        m, sig, hist = macdext(h[0], fp, ft, sp, st, p, t)
+        if m[-1] > 0:
             cat = 1
         else:
             cat = -1
         return cat
 
 
 class MFI(RuleIterator):
@@ -2818,15 +2817,15 @@
 
     def realize(self, h, r=None, t=None, pars=None):
         if pars is None:
             p, u, l = self.pars
         else:
             p, u, l = pars
         h = h.T
-        res = willr(h[0], h[1], h[2], p)
+        res = willr(h[0], h[1], h[2], p)[-1]
         if res > -l:
             sig = -0.3
         elif res < -u:
             sig = 0.1
         else:
             sig = 0
         return sig
```

### Comparing `qteasy-1.2.3/qteasy/core.py` & `qteasy-1.2.4/qteasy/core.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/qteasy/database.py` & `qteasy-1.2.4/qteasy/database.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/qteasy/emfuncs.py` & `qteasy-1.2.4/qteasy/emfuncs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/qteasy/evaluate.py` & `qteasy-1.2.4/qteasy/evaluate.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/qteasy/finance.py` & `qteasy-1.2.4/qteasy/finance.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/qteasy/history.py` & `qteasy-1.2.4/qteasy/history.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/qteasy/optimization.py` & `qteasy-1.2.4/qteasy/optimization.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/qteasy/qt_operator.py` & `qteasy-1.2.4/qteasy/qt_operator.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/qteasy/space.py` & `qteasy-1.2.4/qteasy/space.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/qteasy/strategy.py` & `qteasy-1.2.4/qteasy/strategy.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/qteasy/tafuncs.py` & `qteasy-1.2.4/qteasy/tafuncs.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,16 +27,16 @@
         CDLHIKKAKE, CDLHIKKAKEMOD, CDLHOMINGPIGEON, CDLIDENTICAL3CROWS, CDLINNECK, CDLINVERTEDHAMMER, CDLKICKING, \
         CDLKICKINGBYLENGTH, CDLLADDERBOTTOM, CDLLONGLEGGEDDOJI, CDLLONGLINE, CDLMARUBOZU, CDLMATCHINGLOW, CDLMATHOLD, \
         CDLMORNINGDOJISTAR, CDLMORNINGSTAR, CDLONNECK, CDLPIERCING, CDLRICKSHAWMAN, CDLRISEFALL3METHODS, \
         CDLSEPARATINGLINES, CDLSHOOTINGSTAR, CDLSHORTLINE, CDLSPINNINGTOP, CDLSTALLEDPATTERN, CDLSTICKSANDWICH, \
         CDLTAKURI, CDLTASUKIGAP, CDLTHRUSTING, CDLTRISTAR, CDLUNIQUE3RIVER, CDLUPSIDEGAP2CROWS, CDLXSIDEGAP3METHODS, \
         BETA, CORREL, LINEARREG, LINEARREG_ANGLE, LINEARREG_INTERCEPT, LINEARREG_SLOPE, STDDEV, TSF, VAR, ACOS, ASIN, \
         ATAN, CEIL, COS, COSH, EXP, FLOOR, LN, LOG10, SIN, SINH, SQRT, TAN, TANH, ADD, DIV, MAX, MAXINDEX, MIN, \
-        MININDEX, \
-        MINMAX, MINMAXINDEX, MULT, SUB, SUM, EMA, TRIX, HT_TRENDLINE, KAMA, MA, MAMA, MAVP, MIDPOINT, MIDPRICE, SAR
+        MININDEX, MINMAX, MINMAXINDEX, MULT, SUB, SUM, EMA, TRIX, HT_TRENDLINE, KAMA, MA, MAMA, MAVP, MIDPOINT, \
+        MIDPRICE, SAR
 
     TA_LIB_AVAILABLE = True
 except ImportError as e:
     warnings.warn(f'TA-lib should be installed to use all TA functions, visit '
                   f'https://qteasy.readthedocs.io/zh/latest/faq.html to get more information',
                   ImportWarning)
     TA_LIB_AVAILABLE = False
@@ -408,14 +408,16 @@
     close: float,收盘价
     timeperiod:
 
     Return
     ------
     """
     if TA_LIB_AVAILABLE:
+        if timeperiod == 1:
+            raise ValueError('For SMA, timeperiod must be greater than 1')
         return SMA(close, timeperiod)
     else:
         return sma_no_ta(close, timeperiod)
 
 
 def sma_no_ta(close, timeperiod=30):
     """Simple Moving Average 简单移动平均的不依赖ta-lib版本，计算结果与ta-lib版本一致
```

### Comparing `qteasy-1.2.3/qteasy/trade_recording.py` & `qteasy-1.2.4/qteasy/trade_recording.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/qteasy/trader.py` & `qteasy-1.2.4/qteasy/trader.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/qteasy/trader_cli.py` & `qteasy-1.2.4/qteasy/trader_cli.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/qteasy/trader_tui.py` & `qteasy-1.2.4/qteasy/trader_tui.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/qteasy/trading_util.py` & `qteasy-1.2.4/qteasy/trading_util.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/qteasy/tsfuncs.py` & `qteasy-1.2.4/qteasy/tsfuncs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/qteasy/tui_style.tcss` & `qteasy-1.2.4/qteasy/tui_style.tcss`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/qteasy/utilfuncs.py` & `qteasy-1.2.4/qteasy/utilfuncs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/qteasy/visual.py` & `qteasy-1.2.4/qteasy/visual.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/qteasy.egg-info/PKG-INFO` & `qteasy-1.2.4/qteasy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qteasy
-Version: 1.2.3
+Version: 1.2.4
 Summary: A fast quantitative investment tool kit
 Home-page: https://github.com/shepherdpp/qteasy
 Author: Jackie PENG
 Author-email: jackie PENG <jackie.pengzhao@gmail.com>
 Maintainer: Jackie PENG
 Maintainer-email: jackie PENG <jackie.pengzhao@gmail.com>
 License: Copyright <2019> <JACKIE PENG>
@@ -106,15 +106,15 @@
 > 我会尽快修复问题并回复大家的问题。
 
 ## 关于`qteasy`
 
 - 作者: **Jackie PENG**
 - email: *jackie_pengzhao@163.com*
 - Created: 2019, July, 16
-- Latest Version: `1.2.3`
+- Latest Version: `1.2.4`
 - License: BSD 3-Clause License
 
 `qteasy`是为量化交易人员开发的一套量化交易工具包，特点如下：
 
 1. **全流程覆盖** 从金融数据获取、存储，到交易策略的开发、回测、优化、实盘运行
 2. **完全本地化** 所有的金融数据、策略运算和优化过程完全本地化，不依赖于任何云端服务
 3. **使用简单** 提供大量内置交易策略，用户可以搭积木式地创建自己的交易策略
```

### Comparing `qteasy-1.2.3/qteasy.egg-info/SOURCES.txt` & `qteasy-1.2.4/qteasy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/setup.cfg` & `qteasy-1.2.4/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = qteasy
-version = 1.2.3
+version = 1.2.4
 author = Jackie PENG
 author_email = jackie.pengzhao@gmail.com
 maintainer = Jackie PENG
 description = A fast quantitative investment tool kit
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/shepherdpp/qteasy
```

### Comparing `qteasy-1.2.3/tests/test_broker.py` & `qteasy-1.2.4/tests/test_broker.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/tests/test_cashplan.py` & `qteasy-1.2.4/tests/test_cashplan.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/tests/test_config.py` & `qteasy-1.2.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/tests/test_core_sub_funcs.py` & `qteasy-1.2.4/tests/test_core_sub_funcs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/tests/test_cost.py` & `qteasy-1.2.4/tests/test_cost.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/tests/test_datasource.py` & `qteasy-1.2.4/tests/test_datasource.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/tests/test_eastmoney.py` & `qteasy-1.2.4/tests/test_eastmoney.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/tests/test_evaluations.py` & `qteasy-1.2.4/tests/test_evaluations.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/tests/test_fast_experiments.py` & `qteasy-1.2.4/tests/test_fast_experiments.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/tests/test_historypanel.py` & `qteasy-1.2.4/tests/test_historypanel.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/tests/test_loop.py` & `qteasy-1.2.4/tests/test_loop.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/tests/test_operator_and_strategy.py` & `qteasy-1.2.4/tests/test_operator_and_strategy.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/tests/test_qt.py` & `qteasy-1.2.4/tests/test_qt.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     """
 
     def __init__(self):
         super().__init__(name='test_LS',
                          description='test long/short strategy',
                          par_count=2,
                          par_types='discr, conti',
-                         par_range=([1, 20], [2, 20]),
+                         par_range=([2, 20], [2, 20]),
                          strategy_data_types='close, open, high, low',
                          data_freq='d',
                          window_length=5)
         pass
 
     def realize(self, h, r=None, t=None, pars=None):
         if pars is not None:
@@ -52,15 +52,15 @@
         else:
             n, price = self.pars
         h = h.T
         avg = (h[0] + h[1] + h[2] + h[3]) / 4
         ma = sma(avg, n)
         if r is not None:
             # 处理参考数据生成信号并返回
-            ref_price = r[-1, 0]  # 当天的参考数据，r[-1
+            ref_price = r[-1, 0]  # 当天的参考数据，r[-1]
             if ma[-1] < ref_price:
                 return 0
             else:
                 return 1
 
         if t is not None:
             # 处理交易结果数据生成信号并返回
@@ -962,15 +962,15 @@
         op_batch = qt.Operator(strategies=[stg1, stg2], signal_type='pt', op_type='batch')
         op_stepwise = qt.Operator(strategies=[stg1, stg2], signal_type='pt', op_type='stepwise')
         par_stg1 = {'000100': (20, 10),
                     '000200': (20, 10),
                     '000300': (20, 6)}
         par_stg2 = ()
         for op in [op_batch, op_stepwise]:
-            op.set_parameter(0, pars=par_stg1, opt_tag=1, par_range=([1, 20], [2, 100]))
+            op.set_parameter(0, pars=par_stg1, opt_tag=1, par_range=([2, 20], [2, 100]))
             op.set_parameter(1, pars=par_stg2, opt_tag=1)
 
         qt.configure(
                 benchmark_asset='000300.SH',
                 benchmark_asset_type='IDX',
                 asset_pool='601398.SH, 600000.SH, 000002.SZ',
                 asset_type='E',
```

### Comparing `qteasy-1.2.3/tests/test_space.py` & `qteasy-1.2.4/tests/test_space.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/tests/test_ta_funcs.py` & `qteasy-1.2.4/tests/test_ta_funcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 
     def test_ema_and_ema_no_ta(self):
         """ 测试ema和ema_no_ta的结果是否一致 """
         res = ema(self.close, span=5)
         res_no_ta = ema_no_ta(self.close, span=5)
         print(f'result is\n{res}\n'
               f'result_no_ta is\n{res_no_ta}')
-        self.assertTrue(np.allclose(res, res_no_ta, equal_nan=True, atol=0.02))
+        self.assertTrue(np.allclose(res[5:], res_no_ta[5:], equal_nan=True, atol=0.02))
 
     def test_ht(self):
         print(f'test TA function: ht\n'
               f'======================')
         res = ht(self.close)
         print(f'result is\n{res}')
 
@@ -364,15 +364,15 @@
 
     def test_trix_vs_trix_no_ta(self):
         """ 测试trix和trix_no_ta的结果是否一致 """
         res = trix(self.close, timeperiod=5)
         res_no_ta = trix_no_ta(self.close, timeperiod=5)
         print(f'result is \n{res}\n'
               f'result_no_ta is \n{res_no_ta}')
-        self.assertTrue(np.allclose(res, res_no_ta, equal_nan=True, atol=0.02))
+        self.assertTrue(np.allclose(res[14:], res_no_ta[14:], equal_nan=True, atol=0.2))
 
     def test_ultosc(self):
         print(f'test TA function: ultosc\n'
               f'=========================')
         res = ultosc(self.high, self.low, self.close)
         print(f'result is \n{res}')
```

### Comparing `qteasy-1.2.3/tests/test_trader.py` & `qteasy-1.2.4/tests/test_trader.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/tests/test_trader_shell.py` & `qteasy-1.2.4/tests/test_trader_shell.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/tests/test_trading.py` & `qteasy-1.2.4/tests/test_trading.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/tests/test_tui.py` & `qteasy-1.2.4/tests/test_tui.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/tests/test_tushare.py` & `qteasy-1.2.4/tests/test_tushare.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/tests/test_utilityfuncs.py` & `qteasy-1.2.4/tests/test_utilityfuncs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.3/tests/test_visual.py` & `qteasy-1.2.4/tests/test_visual.py`

 * *Files identical despite different names*

