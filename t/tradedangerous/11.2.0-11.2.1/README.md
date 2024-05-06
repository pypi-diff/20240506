# Comparing `tmp/tradedangerous-11.2.0.tar.gz` & `tmp/tradedangerous-11.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradedangerous-11.2.0.tar", last modified: Sun May  5 23:36:53 2024, max compression
+gzip compressed data, was "tradedangerous-11.2.1.tar", last modified: Mon May  6 04:15:31 2024, max compression
```

## Comparing `tradedangerous-11.2.0.tar` & `tradedangerous-11.2.1.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:36:53.851349 tradedangerous-11.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-05 23:36:53.851349 tradedangerous-11.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-05 23:36:53.851349 tradedangerous-11.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:36:53.835349 tradedangerous-11.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tests/test_bootstrap_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tests/test_bootstrap_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tests/test_peek.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tests/test_trade.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tests/test_trade_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tests/test_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1769 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/trade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:36:53.839349 tradedangerous-11.2.0/tradedangerous/
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36080 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:36:53.843349 tradedangerous-11.2.0/tradedangerous/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/TEMPLATE.py
--rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/buildcache_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/buy_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/commandenv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/export_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/import_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8392 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/local_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/market_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/nav_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/olddata_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/rares_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    47650 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/run_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7943 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/sell_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/shipvendor_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    16232 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/station_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/trade_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    14564 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/update_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    23331 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/update_gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/corrections.py
--rw-r--r--   0 runner    (1001) docker     (127)     8653 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/csvexport.py
--rw-r--r--   0 runner    (1001) docker     (127)    17310 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/edscupdate.py
--rw-r--r--   0 runner    (1001) docker     (127)    14928 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/edsmupdate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6931 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)    43676 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/jsonprices.py
--rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:36:53.843349 tradedangerous-11.2.0/tradedangerous/mfd/
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/mfd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:36:53.843349 tradedangerous-11.2.0/tradedangerous/mfd/saitek/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/mfd/saitek/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24840 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/mfd/saitek/directoutput.py
--rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/mfd/saitek/x52pro.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:36:53.847349 tradedangerous-11.2.0/tradedangerous/misc/
--rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/misc/checkpricebounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/misc/clipboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/misc/coord64.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/misc/derp-sentinel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/misc/diff-system-csvs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/misc/eddb.py
--rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/misc/eddn.py
--rw-r--r--   0 runner    (1001) docker     (127)    14367 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/misc/edsc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/misc/edsm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/misc/importeddbstats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/misc/prices-json-exp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/misc/progress.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:36:53.847349 tradedangerous-11.2.0/tradedangerous/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42262 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/plugins/edapi_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    14412 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/plugins/edcd_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    21931 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/plugins/eddblink_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/plugins/edmc_batch_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    23746 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/plugins/journal_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    13469 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/plugins/netlog_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    27048 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/plugins/spansh_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/prices.py
--rw-r--r--   0 runner    (1001) docker     (127)    11749 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/submit-distances.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:36:53.847349 tradedangerous-11.2.0/tradedangerous/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/templates/Added.csv
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/templates/Category.csv
--rw-r--r--   0 runner    (1001) docker     (127)    10483 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/templates/RareItem.csv
--rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/templates/TradeDangerous.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    42075 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/tradecalc.py
--rw-r--r--   0 runner    (1001) docker     (127)    72282 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/tradedb.py
--rw-r--r--   0 runner    (1001) docker     (127)    11885 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/tradeenv.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/tradeexcept.py
--rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/transfers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-05 23:36:01.000000 tradedangerous-11.2.0/tradedangerous/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:36:53.851349 tradedangerous-11.2.0/tradedangerous.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-05 23:36:53.000000 tradedangerous-11.2.0/tradedangerous.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-05 23:36:53.000000 tradedangerous-11.2.0/tradedangerous.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 23:36:53.000000 tradedangerous-11.2.0/tradedangerous.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-05 23:36:53.000000 tradedangerous-11.2.0/tradedangerous.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 23:36:53.000000 tradedangerous-11.2.0/tradedangerous.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-05 23:36:53.000000 tradedangerous-11.2.0/tradedangerous.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-05 23:36:53.000000 tradedangerous-11.2.0/tradedangerous.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradegui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 04:15:31.628094 tradedangerous-11.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-06 04:15:31.628094 tradedangerous-11.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-06 04:15:31.628094 tradedangerous-11.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 04:15:31.616093 tradedangerous-11.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tests/test_bootstrap_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tests/test_bootstrap_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tests/test_peek.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tests/test_trade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tests/test_trade_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tests/test_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1769 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/trade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 04:15:31.616093 tradedangerous-11.2.1/tradedangerous/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36080 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 04:15:31.624094 tradedangerous-11.2.1/tradedangerous/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/commands/TEMPLATE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/commands/buildcache_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/commands/buy_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/commands/commandenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/commands/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/commands/export_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/commands/import_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8392 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/commands/local_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/commands/market_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/commands/nav_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/commands/olddata_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6595 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/commands/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/commands/rares_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47650 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/commands/run_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7943 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/commands/sell_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/commands/shipvendor_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16232 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/commands/station_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/commands/trade_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14564 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/commands/update_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23331 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/commands/update_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/corrections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8653 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/csvexport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17310 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/edscupdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14928 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/edsmupdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6931 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43676 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/jsonprices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 04:15:31.624094 tradedangerous-11.2.1/tradedangerous/mfd/
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/mfd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 04:15:31.624094 tradedangerous-11.2.1/tradedangerous/mfd/saitek/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/mfd/saitek/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24840 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/mfd/saitek/directoutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/mfd/saitek/x52pro.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 04:15:31.624094 tradedangerous-11.2.1/tradedangerous/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/misc/checkpricebounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/misc/clipboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/misc/coord64.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/misc/derp-sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/misc/diff-system-csvs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/misc/eddb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/misc/eddn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14367 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/misc/edsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/misc/edsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/misc/importeddbstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/misc/prices-json-exp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/misc/progress.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 04:15:31.628094 tradedangerous-11.2.1/tradedangerous/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42262 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/plugins/edapi_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14412 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/plugins/edcd_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21414 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/plugins/eddblink_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/plugins/edmc_batch_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23746 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/plugins/journal_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13469 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/plugins/netlog_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27048 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/plugins/spansh_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/prices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11749 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/submit-distances.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 04:15:31.628094 tradedangerous-11.2.1/tradedangerous/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/templates/Added.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/templates/Category.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10483 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/templates/RareItem.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/templates/TradeDangerous.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42075 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/tradecalc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72282 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/tradedb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11885 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/tradeenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/tradeexcept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradedangerous/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-06 04:14:38.000000 tradedangerous-11.2.1/tradedangerous/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 04:15:31.628094 tradedangerous-11.2.1/tradedangerous.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-06 04:15:31.000000 tradedangerous-11.2.1/tradedangerous.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-06 04:15:31.000000 tradedangerous-11.2.1/tradedangerous.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 04:15:31.000000 tradedangerous-11.2.1/tradedangerous.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-06 04:15:31.000000 tradedangerous-11.2.1/tradedangerous.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 04:15:31.000000 tradedangerous-11.2.1/tradedangerous.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-06 04:15:31.000000 tradedangerous-11.2.1/tradedangerous.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-06 04:15:31.000000 tradedangerous-11.2.1/tradedangerous.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-06 04:14:16.000000 tradedangerous-11.2.1/tradegui.py
```

### Comparing `tradedangerous-11.2.0/LICENSE` & `tradedangerous-11.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/PKG-INFO` & `tradedangerous-11.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradedangerous
-Version: 11.2.0
+Version: 11.2.1
 Summary: Trade-Dangerous is a set of powerful trading tools for Elite Dangerous, organized around one of the most powerful trade run optimizers available.
 Home-page: https://github.com/eyeonus/Trade-Dangerous
 Author: eyeonus
 Author-email: eyeonus@gmail.com
 License: MPL
 Project-URL: Bug Tracker, https://github.com/eyeonus/Trade-Dangerous/issues
 Project-URL: Documentation, https://github.com/eyeonus/Trade-Dangerous/wiki
```

### Comparing `tradedangerous-11.2.0/README.md` & `tradedangerous-11.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/setup.py` & `tradedangerous-11.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tests/test_bootstrap_commands.py` & `tradedangerous-11.2.1/tests/test_bootstrap_commands.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tests/test_bootstrap_plugins.py` & `tradedangerous-11.2.1/tests/test_bootstrap_plugins.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tests/test_cache.py` & `tradedangerous-11.2.1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tests/test_commands.py` & `tradedangerous-11.2.1/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tests/test_fs.py` & `tradedangerous-11.2.1/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tests/test_peek.py` & `tradedangerous-11.2.1/tests/test_peek.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tests/test_trade.py` & `tradedangerous-11.2.1/tests/test_trade.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tests/test_trade_run.py` & `tradedangerous-11.2.1/tests/test_trade_run.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tests/test_utils.py` & `tradedangerous-11.2.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/trade.py` & `tradedangerous-11.2.1/trade.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/__init__.py` & `tradedangerous-11.2.1/tradedangerous/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/cache.py` & `tradedangerous-11.2.1/tradedangerous/cache.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/cli.py` & `tradedangerous-11.2.1/tradedangerous/cli.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/commands/TEMPLATE.py` & `tradedangerous-11.2.1/tradedangerous/commands/TEMPLATE.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/commands/__init__.py` & `tradedangerous-11.2.1/tradedangerous/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/commands/buildcache_cmd.py` & `tradedangerous-11.2.1/tradedangerous/commands/buildcache_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/commands/buy_cmd.py` & `tradedangerous-11.2.1/tradedangerous/commands/buy_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/commands/commandenv.py` & `tradedangerous-11.2.1/tradedangerous/commands/commandenv.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/commands/exceptions.py` & `tradedangerous-11.2.1/tradedangerous/commands/exceptions.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/commands/export_cmd.py` & `tradedangerous-11.2.1/tradedangerous/commands/export_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/commands/import_cmd.py` & `tradedangerous-11.2.1/tradedangerous/commands/import_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/commands/local_cmd.py` & `tradedangerous-11.2.1/tradedangerous/commands/local_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/commands/market_cmd.py` & `tradedangerous-11.2.1/tradedangerous/commands/market_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/commands/nav_cmd.py` & `tradedangerous-11.2.1/tradedangerous/commands/nav_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/commands/olddata_cmd.py` & `tradedangerous-11.2.1/tradedangerous/commands/olddata_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/commands/parsing.py` & `tradedangerous-11.2.1/tradedangerous/commands/parsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,14 @@
                 'Limit to stations with one of the specified pad sizes, '
                 'e.g. --pad SML? matches any pad, --pad M matches only '
                 'medium pads.'
             ),
             'dest': 'padSize',
             'metavar': 'PADSIZES',
             'type': 'padsize',
-            'choices': 'SsMmLl?',
         }
 
 
 class AvoidPlacesArgument(ParseArgument):
     def __init__(self):
         self.args = ['--avoid']
         self.kwargs = {
@@ -149,15 +148,14 @@
                 'Limit to stations with one of the specified planetary, '
                 'e.g. --pla YN? matches any station, --pla Y matches only '
                 'planetary stations.'
             ),
             'dest': 'planetary',
             'metavar': 'PLANETARY',
             'type': 'planetary',
-            'choices': 'YyNn?',
         }
 
 
 class FleetCarrierArgument(int):
     """
     argparse helper for --fleet-carrier
     """
@@ -177,15 +175,14 @@
                 'Limit to stations with one of the specified fleet-carrier, '
                 'e.g. --fc YN? matches any station, --fc Y matches only '
                 'fleet-carrier stations.'
             ),
             'dest': 'fleet',
             'metavar': 'FLEET',
             'type': 'fleet',
-            'choices': 'YyNn?',
         }
 
 class OdysseyArgument(int):
     """
     argparse helper for --odyssey
     """
     class OdysseyParser(str):
@@ -204,15 +201,14 @@
                 'Limit to stations with one of the specified odyssey, '
                 'e.g. --od YN? matches any station, --od Y matches only '
                 'odyssey stations.'
             ),
             'dest': 'odyssey',
             'metavar': 'ODYSSEY',
             'type': 'odyssey',
-            'choices': 'YyNn?',
         }
 
 
 __tdParserHelpers = {
     'credits': CreditParser,
     'padsize': PadSizeArgument.PadSizeParser,
     'planetary': PlanetaryArgument.PlanetaryParser,
```

### Comparing `tradedangerous-11.2.0/tradedangerous/commands/rares_cmd.py` & `tradedangerous-11.2.1/tradedangerous/commands/rares_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/commands/run_cmd.py` & `tradedangerous-11.2.1/tradedangerous/commands/run_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/commands/sell_cmd.py` & `tradedangerous-11.2.1/tradedangerous/commands/sell_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/commands/shipvendor_cmd.py` & `tradedangerous-11.2.1/tradedangerous/commands/shipvendor_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/commands/station_cmd.py` & `tradedangerous-11.2.1/tradedangerous/commands/station_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/commands/trade_cmd.py` & `tradedangerous-11.2.1/tradedangerous/commands/trade_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/commands/update_cmd.py` & `tradedangerous-11.2.1/tradedangerous/commands/update_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/commands/update_gui.py` & `tradedangerous-11.2.1/tradedangerous/commands/update_gui.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/corrections.py` & `tradedangerous-11.2.1/tradedangerous/corrections.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/csvexport.py` & `tradedangerous-11.2.1/tradedangerous/csvexport.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/edscupdate.py` & `tradedangerous-11.2.1/tradedangerous/edscupdate.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Deprecated
 #!/usr/bin/env python3.6
+# Deprecated
 
 """
 This tool looks for changes in the EDSC service since the most
 recent "modified" date in the System table or the date supplied
 on the command line.
 
 It then tries to do some validation but also requires user
```

### Comparing `tradedangerous-11.2.0/tradedangerous/edsmupdate.py` & `tradedangerous-11.2.1/tradedangerous/edsmupdate.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Deprecated
 #!/usr/bin/env python3.6
+# Deprecated
 
 """
 based on edscupdate.py without the submit_distance()
 
 This tool looks for changes in the EDSM service since the most
 recent "modified" date in the System table or the date supplied
 on the command line.
```

### Comparing `tradedangerous-11.2.0/tradedangerous/formatting.py` & `tradedangerous-11.2.1/tradedangerous/formatting.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/fs.py` & `tradedangerous-11.2.1/tradedangerous/fs.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/gui.py` & `tradedangerous-11.2.1/tradedangerous/gui.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/jsonprices.py` & `tradedangerous-11.2.1/tradedangerous/jsonprices.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/mapping.py` & `tradedangerous-11.2.1/tradedangerous/mapping.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/mfd/__init__.py` & `tradedangerous-11.2.1/tradedangerous/mfd/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/mfd/saitek/directoutput.py` & `tradedangerous-11.2.1/tradedangerous/mfd/saitek/directoutput.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/mfd/saitek/x52pro.py` & `tradedangerous-11.2.1/tradedangerous/mfd/saitek/x52pro.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/misc/checkpricebounds.py` & `tradedangerous-11.2.1/tradedangerous/misc/checkpricebounds.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/misc/clipboard.py` & `tradedangerous-11.2.1/tradedangerous/misc/clipboard.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/misc/coord64.py` & `tradedangerous-11.2.1/tradedangerous/misc/coord64.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/misc/derp-sentinel.py` & `tradedangerous-11.2.1/tradedangerous/misc/derp-sentinel.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/misc/diff-system-csvs.py` & `tradedangerous-11.2.1/tradedangerous/misc/diff-system-csvs.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/misc/eddb.py` & `tradedangerous-11.2.1/tradedangerous/misc/eddb.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/misc/eddn.py` & `tradedangerous-11.2.1/tradedangerous/misc/eddn.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/misc/edsc.py` & `tradedangerous-11.2.1/tradedangerous/misc/edsc.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/misc/edsm.py` & `tradedangerous-11.2.1/tradedangerous/misc/edsm.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/misc/importeddbstats.py` & `tradedangerous-11.2.1/tradedangerous/misc/importeddbstats.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/misc/prices-json-exp.py` & `tradedangerous-11.2.1/tradedangerous/misc/prices-json-exp.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/misc/progress.py` & `tradedangerous-11.2.1/tradedangerous/misc/progress.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/plugins/__init__.py` & `tradedangerous-11.2.1/tradedangerous/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/plugins/edapi_plug.py` & `tradedangerous-11.2.1/tradedangerous/plugins/edapi_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/plugins/edcd_plug.py` & `tradedangerous-11.2.1/tradedangerous/plugins/edcd_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/plugins/eddblink_plug.py` & `tradedangerous-11.2.1/tradedangerous/plugins/eddblink_plug.py`

 * *Files 3% similar despite different names*

```diff
@@ -114,14 +114,15 @@
         'listings':     "Update market data using latest listings.csv dump. (Implies '-O item,system,station')",
         'all':          "Update everything with latest dumpfiles. (Regenerates all tables)",
         'clean':        "Erase entire database and rebuild from empty. (Regenerates all tables.)",
         'skipvend':     "Don't regenerate ShipVendors or UpgradeVendors. (Supercedes '-O all', '-O clean'.)",
         'force':        "Force regeneration of selected items even if source file not updated since previous run. "
                         "(Useful for updating Vendor tables if they were skipped during a '-O clean' run.)",
         'purge':        "Remove any empty systems that previously had fleet carriers.",
+        'optimize':     "Optimize ('vacuum') database after processing.",
         'solo':         "Don't download crowd-sourced market data. (Implies '-O skipvend', supercedes '-O all', '-O clean', '-O listings'.)",
     }
     
     def __init__(self, tdb, tdenv):
         super().__init__(tdb, tdenv)
         
         self.dataPath = Path(os.environ.get('TD_EDDB')) if os.environ.get('TD_EDDB') else self.tdb.dataPath / Path("eddb")
@@ -193,30 +194,18 @@
         """
         Purges systems from the System table that do not have any stations claiming to be in them.
         Keeps table from becoming too large because of fleet carriers moving to unpopulated systems.
         """
         db = self.tdb.getDB()
         self.tdenv.NOTE("Purging Systems with no stations: Start time = {}", self.now())
 
-        db.execute("PRAGMA foreign_keys = OFF")
-
-        self.tdenv.DEBUG0("Saving systems with stations.... " + str(self.now()) + "\t\t\t\t", end="\r")
-        db.execute("DROP TABLE IF EXISTS System_copy")
-        db.execute("""CREATE TABLE System_copy AS SELECT * FROM System
-                            WHERE system_id IN (SELECT system_id FROM Station)
-                    """)
-
-        self.tdenv.DEBUG0("Erasing table and reinserting kept systems.... " + str(self.now()) + "\t\t\t\t", end="\r")
-        db.execute("DELETE FROM System")
-        db.execute("INSERT INTO System SELECT * FROM System_copy")
-
-        self.tdenv.DEBUG0("Removing copy.... " + str(self.now()) + "\t\t\t\t", end="\r")
-        db.execute("PRAGMA foreign_keys = ON")
-        db.execute("DROP TABLE IF EXISTS System_copy")
-
+        db.execute("""
+            DELETE FROM System
+             WHERE NOT EXISTS(SELECT 1 FROM Station WHERE Station.system_id = System.system_id)
+        """)
         db.commit()
 
         self.tdenv.NOTE("Finished purging Systems. End time = {}", self.now())
     
     def importListings(self, listings_file):
         """
         Updates the market data (AKA the StationItem table) using listings_file
@@ -345,15 +334,15 @@
             if option not in ('force', 'skipvend', 'purge'):
                 default = False
         if default:
             self.options["listings"] = True
         
         # We can probably safely assume that the plugin
         # has never been run if the db file doesn't exist.
-        if not (self.tdb.dataPath / Path("TradeDangerous.db")).exists():
+        if not self.tdb.dbPath.exists():
             self.options["clean"] = True
         
         if self.getOption("clean"):
             # Rebuild the tables from scratch. Must be done on first run of plugin.
             # Can be done at anytime with the "clean" option.
             for name in [
                 "Category",
@@ -388,16 +377,19 @@
             # because there's nothing in the Station table it tries to pull from.
             ri_path = self.tdb.dataPath / Path("RareItem.csv")
             rib_path = ri_path.with_suffix(".tmp")
             if ri_path.exists():
                 if rib_path.exists():
                     rib_path.unlink()
                 ri_path.rename(rib_path)
-            
+
+            self.tdb.close()
+
             self.tdb.reloadCache()
+            self.tdb.close()
             
             # Now it's safe to move RareItems back.
             if ri_path.exists():
                 ri_path.unlink()
             if rib_path.exists():
                 rib_path.rename(ri_path)
             
@@ -447,15 +439,15 @@
         
         # Download required files and update tables.
         buildCache = False
         if self.getOption("upgrade"):
             if self.downloadFile(self.upgradesPath) or self.getOption("force"):
                 transfers.download(self.tdenv, self.urlOutfitting, self.FDevOutfittingPath)
                 buildCache = True
-        
+
         if self.getOption("ship"):
             if self.downloadFile(self.shipPath) or self.getOption("force"):
                 transfers.download(self.tdenv, self.urlShipyard, self.FDevShipyardPath)
                 buildCache = True
         
         if self.getOption("rare"):
             if self.downloadFile(self.rareItemPath) or self.getOption("force"):
@@ -482,24 +474,26 @@
                 self.downloadFile(self.categoriesPath)
                 buildCache = True
         
         # Remake the .db files with the updated info.
         if buildCache:
             self.tdb.close()
             self.tdb.reloadCache()
-        
+            self.tdb.close()
+
         if self.getOption("purge"):
             self.purgeSystems()
+            self.tdb.close()
         
         if self.getOption("listings"):
             if self.downloadFile(self.listingsPath) or self.getOption("force"):
                 self.importListings(self.listingsPath)
             if self.downloadFile(self.liveListingsPath) or self.getOption("force"):
                 self.importListings(self.liveListingsPath)
-        
+
         if self.getOption("listings"):
             self.tdenv.NOTE("Regenerating .prices file.")
             cache.regeneratePricesFile(self.tdb, self.tdenv)
         
         self.tdenv.NOTE("Import completed.")
         
         # TD doesn't need to do anything, tell it to just quit.
```

### Comparing `tradedangerous-11.2.0/tradedangerous/plugins/edmc_batch_plug.py` & `tradedangerous-11.2.1/tradedangerous/plugins/edmc_batch_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/plugins/journal_plug.py` & `tradedangerous-11.2.1/tradedangerous/plugins/journal_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/plugins/netlog_plug.py` & `tradedangerous-11.2.1/tradedangerous/plugins/netlog_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/plugins/spansh_plug.py` & `tradedangerous-11.2.1/tradedangerous/plugins/spansh_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/prices.py` & `tradedangerous-11.2.1/tradedangerous/prices.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/submit-distances.py` & `tradedangerous-11.2.1/tradedangerous/submit-distances.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/templates/Added.csv` & `tradedangerous-11.2.1/tradedangerous/templates/Added.csv`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/templates/RareItem.csv` & `tradedangerous-11.2.1/tradedangerous/templates/RareItem.csv`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/templates/TradeDangerous.sql` & `tradedangerous-11.2.1/tradedangerous/templates/TradeDangerous.sql`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/tools.py` & `tradedangerous-11.2.1/tradedangerous/tools.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/tradecalc.py` & `tradedangerous-11.2.1/tradedangerous/tradecalc.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/tradedb.py` & `tradedangerous-11.2.1/tradedangerous/tradedb.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/tradeenv.py` & `tradedangerous-11.2.1/tradedangerous/tradeenv.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/transfers.py` & `tradedangerous-11.2.1/tradedangerous/transfers.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/utils.py` & `tradedangerous-11.2.1/tradedangerous/utils.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradedangerous/version.py` & `tradedangerous-11.2.1/tradedangerous/version.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 # this software so long as you include this copyright notice.
 # I guarantee there is at least one bug neither of us knew about.
 # --------------------------------------------------------------------
 
 """just keeper of current version"""
 
 # TODO: remember to update tests when version changes
-__version__ = '11.2.0'
+__version__ = '11.2.1'
```

### Comparing `tradedangerous-11.2.0/tradedangerous.egg-info/PKG-INFO` & `tradedangerous-11.2.1/tradedangerous.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradedangerous
-Version: 11.2.0
+Version: 11.2.1
 Summary: Trade-Dangerous is a set of powerful trading tools for Elite Dangerous, organized around one of the most powerful trade run optimizers available.
 Home-page: https://github.com/eyeonus/Trade-Dangerous
 Author: eyeonus
 Author-email: eyeonus@gmail.com
 License: MPL
 Project-URL: Bug Tracker, https://github.com/eyeonus/Trade-Dangerous/issues
 Project-URL: Documentation, https://github.com/eyeonus/Trade-Dangerous/wiki
```

### Comparing `tradedangerous-11.2.0/tradedangerous.egg-info/SOURCES.txt` & `tradedangerous-11.2.1/tradedangerous.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.2.0/tradegui.py` & `tradedangerous-11.2.1/tradegui.py`

 * *Files identical despite different names*

