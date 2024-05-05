# Comparing `tmp/tradedangerous-11.1.6.tar.gz` & `tmp/tradedangerous-11.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradedangerous-11.1.6.tar", last modified: Wed May  1 19:04:21 2024, max compression
+gzip compressed data, was "tradedangerous-11.2.0.tar", last modified: Sun May  5 23:36:53 2024, max compression
```

## Comparing `tradedangerous-11.1.6.tar` & `tradedangerous-11.2.0.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:04:21.563217 tradedangerous-11.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-01 19:04:21.563217 tradedangerous-11.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-01 19:04:21.563217 tradedangerous-11.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:04:21.547217 tradedangerous-11.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tests/test_bootstrap_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tests/test_bootstrap_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tests/test_peek.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tests/test_trade.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tests/test_trade_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/trade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:04:21.555217 tradedangerous-11.1.6/tradedangerous/
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36080 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:04:21.559217 tradedangerous-11.1.6/tradedangerous/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/commands/TEMPLATE.py
--rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/commands/buildcache_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/commands/buy_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/commands/commandenv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/commands/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/commands/export_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/commands/import_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8392 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/commands/local_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/commands/market_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/commands/nav_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/commands/olddata_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/commands/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/commands/rares_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    47650 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/commands/run_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7943 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/commands/sell_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/commands/shipvendor_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    16219 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/commands/station_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/commands/trade_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    14551 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/commands/update_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    23318 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/commands/update_gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/corrections.py
--rw-r--r--   0 runner    (1001) docker     (127)     8653 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/csvexport.py
--rw-r--r--   0 runner    (1001) docker     (127)    17297 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/edscupdate.py
--rw-r--r--   0 runner    (1001) docker     (127)    14915 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/edsmupdate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6931 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)    43676 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/jsonprices.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:04:21.559217 tradedangerous-11.1.6/tradedangerous/mfd/
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/mfd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:04:21.559217 tradedangerous-11.1.6/tradedangerous/mfd/saitek/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/mfd/saitek/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24840 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/mfd/saitek/directoutput.py
--rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/mfd/saitek/x52pro.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:04:21.563217 tradedangerous-11.1.6/tradedangerous/misc/
--rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/misc/checkpricebounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/misc/clipboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/misc/coord64.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/misc/derp-sentinel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/misc/diff-system-csvs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/misc/eddb.py
--rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/misc/eddn.py
--rw-r--r--   0 runner    (1001) docker     (127)    14367 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/misc/edsc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/misc/edsm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/misc/importeddbstats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/misc/prices-json-exp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/misc/progress.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:04:21.563217 tradedangerous-11.1.6/tradedangerous/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42262 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/plugins/edapi_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    14412 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/plugins/edcd_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    21931 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/plugins/eddblink_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/plugins/edmc_batch_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    23746 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/plugins/journal_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    13469 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/plugins/netlog_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    27048 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/plugins/spansh_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/prices.py
--rw-r--r--   0 runner    (1001) docker     (127)    11709 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/submit-distances.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:04:21.563217 tradedangerous-11.1.6/tradedangerous/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/templates/Added.csv
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/templates/Category.csv
--rw-r--r--   0 runner    (1001) docker     (127)    10483 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/templates/RareItem.csv
--rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/templates/TradeDangerous.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    42075 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/tradecalc.py
--rw-r--r--   0 runner    (1001) docker     (127)    72282 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/tradedb.py
--rw-r--r--   0 runner    (1001) docker     (127)    10576 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/tradeenv.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/tradeexcept.py
--rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/transfers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradedangerous/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-01 19:03:29.000000 tradedangerous-11.1.6/tradedangerous/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:04:21.563217 tradedangerous-11.1.6/tradedangerous.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-01 19:04:21.000000 tradedangerous-11.1.6/tradedangerous.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-01 19:04:21.000000 tradedangerous-11.1.6/tradedangerous.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 19:04:21.000000 tradedangerous-11.1.6/tradedangerous.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-01 19:04:21.000000 tradedangerous-11.1.6/tradedangerous.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 19:04:21.000000 tradedangerous-11.1.6/tradedangerous.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-01 19:04:21.000000 tradedangerous-11.1.6/tradedangerous.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-01 19:04:21.000000 tradedangerous-11.1.6/tradedangerous.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-01 19:03:03.000000 tradedangerous-11.1.6/tradegui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:36:53.851349 tradedangerous-11.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-05 23:36:53.851349 tradedangerous-11.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-05 23:36:53.851349 tradedangerous-11.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:36:53.835349 tradedangerous-11.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tests/test_bootstrap_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tests/test_bootstrap_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tests/test_peek.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tests/test_trade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tests/test_trade_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tests/test_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1769 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/trade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:36:53.839349 tradedangerous-11.2.0/tradedangerous/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36080 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:36:53.843349 tradedangerous-11.2.0/tradedangerous/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/TEMPLATE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/buildcache_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/buy_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/commandenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/export_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/import_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8392 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/local_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/market_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/nav_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/olddata_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/rares_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47650 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/run_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7943 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/sell_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/shipvendor_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16232 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/station_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/trade_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14564 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/update_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23331 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/commands/update_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/corrections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8653 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/csvexport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17310 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/edscupdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14928 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/edsmupdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6931 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43676 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/jsonprices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:36:53.843349 tradedangerous-11.2.0/tradedangerous/mfd/
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/mfd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:36:53.843349 tradedangerous-11.2.0/tradedangerous/mfd/saitek/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/mfd/saitek/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24840 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/mfd/saitek/directoutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/mfd/saitek/x52pro.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:36:53.847349 tradedangerous-11.2.0/tradedangerous/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/misc/checkpricebounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/misc/clipboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/misc/coord64.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/misc/derp-sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/misc/diff-system-csvs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/misc/eddb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/misc/eddn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14367 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/misc/edsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/misc/edsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/misc/importeddbstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/misc/prices-json-exp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/misc/progress.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:36:53.847349 tradedangerous-11.2.0/tradedangerous/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42262 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/plugins/edapi_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14412 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/plugins/edcd_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21931 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/plugins/eddblink_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/plugins/edmc_batch_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23746 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/plugins/journal_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13469 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/plugins/netlog_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27048 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/plugins/spansh_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/prices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11749 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/submit-distances.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:36:53.847349 tradedangerous-11.2.0/tradedangerous/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/templates/Added.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/templates/Category.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10483 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/templates/RareItem.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/templates/TradeDangerous.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42075 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/tradecalc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72282 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/tradedb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11885 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/tradeenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/tradeexcept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradedangerous/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-05 23:36:01.000000 tradedangerous-11.2.0/tradedangerous/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:36:53.851349 tradedangerous-11.2.0/tradedangerous.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-05 23:36:53.000000 tradedangerous-11.2.0/tradedangerous.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-05 23:36:53.000000 tradedangerous-11.2.0/tradedangerous.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 23:36:53.000000 tradedangerous-11.2.0/tradedangerous.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-05 23:36:53.000000 tradedangerous-11.2.0/tradedangerous.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 23:36:53.000000 tradedangerous-11.2.0/tradedangerous.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-05 23:36:53.000000 tradedangerous-11.2.0/tradedangerous.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-05 23:36:53.000000 tradedangerous-11.2.0/tradedangerous.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-05 23:35:35.000000 tradedangerous-11.2.0/tradegui.py
```

### Comparing `tradedangerous-11.1.6/LICENSE` & `tradedangerous-11.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/PKG-INFO` & `tradedangerous-11.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradedangerous
-Version: 11.1.6
+Version: 11.2.0
 Summary: Trade-Dangerous is a set of powerful trading tools for Elite Dangerous, organized around one of the most powerful trade run optimizers available.
 Home-page: https://github.com/eyeonus/Trade-Dangerous
 Author: eyeonus
 Author-email: eyeonus@gmail.com
 License: MPL
 Project-URL: Bug Tracker, https://github.com/eyeonus/Trade-Dangerous/issues
 Project-URL: Documentation, https://github.com/eyeonus/Trade-Dangerous/wiki
```

### Comparing `tradedangerous-11.1.6/README.md` & `tradedangerous-11.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/setup.py` & `tradedangerous-11.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tests/test_bootstrap_commands.py` & `tradedangerous-11.2.0/tests/test_bootstrap_commands.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tests/test_bootstrap_plugins.py` & `tradedangerous-11.2.0/tests/test_bootstrap_plugins.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tests/test_cache.py` & `tradedangerous-11.2.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tests/test_commands.py` & `tradedangerous-11.2.0/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tests/test_fs.py` & `tradedangerous-11.2.0/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tests/test_peek.py` & `tradedangerous-11.2.0/tests/test_peek.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tests/test_trade.py` & `tradedangerous-11.2.0/tests/test_trade.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tests/test_trade_run.py` & `tradedangerous-11.2.0/tests/test_trade_run.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tests/test_utils.py` & `tradedangerous-11.2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/trade.py` & `tradedangerous-11.2.0/trade.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/__init__.py` & `tradedangerous-11.2.0/tradedangerous/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/cache.py` & `tradedangerous-11.2.0/tradedangerous/cache.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/cli.py` & `tradedangerous-11.2.0/tradedangerous/cli.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/commands/TEMPLATE.py` & `tradedangerous-11.2.0/tradedangerous/commands/TEMPLATE.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/commands/__init__.py` & `tradedangerous-11.2.0/tradedangerous/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/commands/buildcache_cmd.py` & `tradedangerous-11.2.0/tradedangerous/commands/buildcache_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/commands/buy_cmd.py` & `tradedangerous-11.2.0/tradedangerous/commands/buy_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/commands/commandenv.py` & `tradedangerous-11.2.0/tradedangerous/commands/commandenv.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/commands/exceptions.py` & `tradedangerous-11.2.0/tradedangerous/commands/exceptions.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/commands/export_cmd.py` & `tradedangerous-11.2.0/tradedangerous/commands/export_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/commands/import_cmd.py` & `tradedangerous-11.2.0/tradedangerous/commands/import_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/commands/local_cmd.py` & `tradedangerous-11.2.0/tradedangerous/commands/local_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/commands/market_cmd.py` & `tradedangerous-11.2.0/tradedangerous/commands/market_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/commands/nav_cmd.py` & `tradedangerous-11.2.0/tradedangerous/commands/nav_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/commands/olddata_cmd.py` & `tradedangerous-11.2.0/tradedangerous/commands/olddata_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/commands/parsing.py` & `tradedangerous-11.2.0/tradedangerous/commands/parsing.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/commands/rares_cmd.py` & `tradedangerous-11.2.0/tradedangerous/commands/rares_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/commands/run_cmd.py` & `tradedangerous-11.2.0/tradedangerous/commands/run_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/commands/sell_cmd.py` & `tradedangerous-11.2.0/tradedangerous/commands/sell_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/commands/shipvendor_cmd.py` & `tradedangerous-11.2.0/tradedangerous/commands/shipvendor_cmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Deprecated
+# Can already use buy command for ship searching
 from .commandenv import ResultRow
 from .exceptions import CommandLineError
 from .parsing import MutuallyExclusiveGroup, ParseArgument
 from ..formatting import RowFormat, ColumnFormat, max_len
 from itertools import chain
 from ..tradedb import Station
```

### Comparing `tradedangerous-11.1.6/tradedangerous/commands/station_cmd.py` & `tradedangerous-11.2.0/tradedangerous/commands/station_cmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Deprecated
 from .commandenv import ResultRow
 from .exceptions import CommandLineError
 from .parsing import MutuallyExclusiveGroup, ParseArgument
 from ..tradedb import AmbiguityError
 from ..tradedb import Station
 from ..tradedb import TradeDB
 from .. import utils
```

### Comparing `tradedangerous-11.1.6/tradedangerous/commands/trade_cmd.py` & `tradedangerous-11.2.0/tradedangerous/commands/trade_cmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from .parsing import ParseArgument
 from ..tradecalc import TradeCalc
 from ..formatting import RowFormat, max_len
 
 ######################################################################
 # Parser config
 
-help='Find places to buy a given item within range of a given station.'
+help='Find potential trades between two given stations.'
 name='trade'
 epilog=None
 wantsTradeDB=True
 arguments = [
     ParseArgument(
         'origin',
         help='Station you are purchasing from.',
```

### Comparing `tradedangerous-11.1.6/tradedangerous/commands/update_cmd.py` & `tradedangerous-11.2.0/tradedangerous/commands/update_cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Deprecated
 from .parsing import MutuallyExclusiveGroup, ParseArgument
 from ..tradeexcept import TradeException
 from .exceptions import CommandLineError
 from ..tradedb import System
 from .. import prices, cache
 import subprocess
 import os
```

### Comparing `tradedangerous-11.1.6/tradedangerous/commands/update_gui.py` & `tradedangerous-11.2.0/tradedangerous/commands/update_gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Deprecated
 import tkinter as tk
 import tkinter.messagebox as mbox
 import sqlite3
 import re
 
 """
 This is a crude attempt at a GUI for updating trade prices.
```

### Comparing `tradedangerous-11.1.6/tradedangerous/corrections.py` & `tradedangerous-11.2.0/tradedangerous/corrections.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/csvexport.py` & `tradedangerous-11.2.0/tradedangerous/csvexport.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/edscupdate.py` & `tradedangerous-11.2.0/tradedangerous/edscupdate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Deprecated
 #!/usr/bin/env python3.6
 
 """
 This tool looks for changes in the EDSC service since the most
 recent "modified" date in the System table or the date supplied
 on the command line.
```

### Comparing `tradedangerous-11.1.6/tradedangerous/edsmupdate.py` & `tradedangerous-11.2.0/tradedangerous/edsmupdate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Deprecated
 #!/usr/bin/env python3.6
 
 """
 based on edscupdate.py without the submit_distance()
 
 This tool looks for changes in the EDSM service since the most
 recent "modified" date in the System table or the date supplied
```

### Comparing `tradedangerous-11.1.6/tradedangerous/formatting.py` & `tradedangerous-11.2.0/tradedangerous/formatting.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/fs.py` & `tradedangerous-11.2.0/tradedangerous/fs.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/gui.py` & `tradedangerous-11.2.0/tradedangerous/gui.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/jsonprices.py` & `tradedangerous-11.2.0/tradedangerous/jsonprices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Deprecated
 from tradedangerous import tradedb
 from tradedangerous.tradeexcept import TradeException
 
 import json
 import sys
```

### Comparing `tradedangerous-11.1.6/tradedangerous/mapping.py` & `tradedangerous-11.2.0/tradedangerous/mapping.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #
 # Mapping class for FDEV-IDs to TD names
 #
-
+# Deprecated
+# FDEVMappingItems and FDEVMappingShips used by edapi plugin
 class FDEVMappingBase:
     """
     Base class to map FDEV-IDs to TD names, do not use directly.
     
     Derived class must declare "tableName" and "colNames" which are used
     to select the ID->Name mapping from the database.
```

### Comparing `tradedangerous-11.1.6/tradedangerous/mfd/__init__.py` & `tradedangerous-11.2.0/tradedangerous/mfd/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/mfd/saitek/directoutput.py` & `tradedangerous-11.2.0/tradedangerous/mfd/saitek/directoutput.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/mfd/saitek/x52pro.py` & `tradedangerous-11.2.0/tradedangerous/mfd/saitek/x52pro.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/misc/checkpricebounds.py` & `tradedangerous-11.2.0/tradedangerous/misc/checkpricebounds.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/misc/clipboard.py` & `tradedangerous-11.2.0/tradedangerous/misc/clipboard.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/misc/coord64.py` & `tradedangerous-11.2.0/tradedangerous/misc/coord64.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/misc/derp-sentinel.py` & `tradedangerous-11.2.0/tradedangerous/misc/derp-sentinel.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/misc/diff-system-csvs.py` & `tradedangerous-11.2.0/tradedangerous/misc/diff-system-csvs.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/misc/eddb.py` & `tradedangerous-11.2.0/tradedangerous/misc/eddb.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/misc/eddn.py` & `tradedangerous-11.2.0/tradedangerous/misc/eddn.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/misc/edsc.py` & `tradedangerous-11.2.0/tradedangerous/misc/edsc.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/misc/edsm.py` & `tradedangerous-11.2.0/tradedangerous/misc/edsm.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/misc/importeddbstats.py` & `tradedangerous-11.2.0/tradedangerous/misc/importeddbstats.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/misc/prices-json-exp.py` & `tradedangerous-11.2.0/tradedangerous/misc/prices-json-exp.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/misc/progress.py` & `tradedangerous-11.2.0/tradedangerous/misc/progress.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/plugins/__init__.py` & `tradedangerous-11.2.0/tradedangerous/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/plugins/edapi_plug.py` & `tradedangerous-11.2.0/tradedangerous/plugins/edapi_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/plugins/edcd_plug.py` & `tradedangerous-11.2.0/tradedangerous/plugins/edcd_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/plugins/eddblink_plug.py` & `tradedangerous-11.2.0/tradedangerous/plugins/eddblink_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/plugins/edmc_batch_plug.py` & `tradedangerous-11.2.0/tradedangerous/plugins/edmc_batch_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/plugins/journal_plug.py` & `tradedangerous-11.2.0/tradedangerous/plugins/journal_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/plugins/netlog_plug.py` & `tradedangerous-11.2.0/tradedangerous/plugins/netlog_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/plugins/spansh_plug.py` & `tradedangerous-11.2.0/tradedangerous/plugins/spansh_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/prices.py` & `tradedangerous-11.2.0/tradedangerous/prices.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/submit-distances.py` & `tradedangerous-11.2.0/tradedangerous/submit-distances.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 #!/usr/bin/env python3.6
+# Deprecated
+# Website no longer exists
 
 """
 Small tool to submit new star data to EDStarCoordinator.
 
 Use:
     submit-distances.py "system name"
 """
```

### Comparing `tradedangerous-11.1.6/tradedangerous/templates/Added.csv` & `tradedangerous-11.2.0/tradedangerous/templates/Added.csv`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/templates/RareItem.csv` & `tradedangerous-11.2.0/tradedangerous/templates/RareItem.csv`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/templates/TradeDangerous.sql` & `tradedangerous-11.2.0/tradedangerous/templates/TradeDangerous.sql`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/tools.py` & `tradedangerous-11.2.0/tradedangerous/tools.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/tradecalc.py` & `tradedangerous-11.2.0/tradedangerous/tradecalc.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/tradedb.py` & `tradedangerous-11.2.0/tradedangerous/tradedb.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/tradeenv.py` & `tradedangerous-11.2.0/tradedangerous/tradeenv.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # The runtime environment TD tools are expected to run with is encapsulated
 # into a single object, the TradeEnv. See TradeEnv docstring for more.
 from __future__ import annotations
 
+from pathlib import Path
 import os
 import sys
 import traceback
 import typing
 
 # Import some utilities from the 'rich' library that provide ways to colorize and animate
 # the console output, along with other useful features.
@@ -266,7 +267,40 @@
                 pass
             
             noteFn = _WARN_DISABLED if self.quiet > 1 else _WARN_ENABLED
             setattr(self, key, noteFn)
             return noteFn
         
         return None
+
+    def remove_file(self, *args) -> bool:
+        """ Unlinks a file, as long as it exists, and logs the action at level 1. """
+        path = Path(*args)
+        if not path.exists():
+            return False
+        path.unlink()
+        self.DEBUG1(":cross_mark: deleted {}", path)
+        return True
+
+    def rename_file(self, *, old: os.PathLike, new: os.PathLike) -> bool:
+        """
+        If 'new' exists, deletes it, and then attempts to rename old -> new. If new is not specified,
+        then '.old' is appended to the end of the old filename while retaining the original suffix.
+        
+        :param old:             The current path/name of the file.
+        :param new:             The path/name to rename the file to and remove before attempting.
+        :returns:               True if the file existed and was renamed.
+        """
+        # Promote new to a guaranteed Path and remove it if it's present.
+        new = Path(new)
+        self.remove_file(new)
+
+        # Promote new to a guaranteed Path and confirm it exists.
+        old = Path(old)
+        if not old.exists():
+            return False
+
+        # Perform the rename and log it at level 1.
+        old.rename(new)
+        self.DEBUG1(":recycle: moved {} to {}", old, new)
+
+        return True
```

### Comparing `tradedangerous-11.1.6/tradedangerous/transfers.py` & `tradedangerous-11.2.0/tradedangerous/transfers.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from collections import deque
 from pathlib import Path
 from .tradeexcept import TradeException
 from .misc import progress as pbar
 from . import fs
 
-import csv
 import json
 import time
 import typing
 
 import requests
 
 
@@ -46,14 +45,15 @@
             headers:    Optional[dict] = None,
             backup:     bool = False,
             shebang:    Optional[str] = None,
             chunkSize:  int = 4096,
             timeout:    int = 90,
             *,
             length:     Optional[Union[int, str]] = None,
+            session:    Optional[requests.Session] = None,
         ):
     """
     Fetch data from a URL and save the output
     to a local file. Returns the response headers.
     
     tdenv:
         TradeEnv we're working under
@@ -71,25 +71,26 @@
         function to call on the first line
     """
     tdenv.NOTE("Requesting {}".format(url))
 
     if isinstance(length, str):
         length = int(length)
 
-    req = requests.get(url, headers=headers or None, stream=True, timeout=timeout)
+    # If the caller provided an existing session stream, use that the fetch the request.
+    req = (session or requests).get(url, headers=headers or None, stream=True, timeout=timeout)
     req.raise_for_status()
     
     encoding = req.headers.get('content-encoding', 'uncompress')
     content_length = req.headers.get('content-length', length)
     transfer = req.headers.get('transfer-encoding', None)
     if not length and transfer != 'chunked':
         # chunked transfer-encoding doesn't need a content-length
         if content_length is None:
             print(req.headers)
-            raise Exception("Remote server replied with invalid content-length.")
+            raise TradeException("Remote server replied with invalid content-length.")
         content_length = int(content_length)
         if content_length <= 0:
             raise TradeException(
                 "Remote server gave an empty response. Please try again later."
             )
 
     # if the file is being compressed by the server, the headers tell us the
@@ -206,56 +207,7 @@
                 " {}/{}".format(
                     makeUnit(value),
                     makeUnit(goal),
             ))
         progBar.clear()
     
     return json.loads(jsData.decode())
-
-class CSVStream:
-    """
-    Provides an iterator that fetches CSV data from a given URL
-    and presents it as an iterable of (columns, values).
-    
-    Example:
-        stream = transfers.CSVStream("http://blah.com/foo.csv")
-        for cols, vals in stream:
-            print("{} = {}".format(cols[0], vals[0]))
-    """
-    
-    def __init__(self, url, tdenv=None, *, timeout: int = 90):
-        self.url = url
-        self.tdenv = tdenv
-        if not url.startswith("file:///"):
-            self.req = requests.get(self.url, stream=True, timeout=timeout)
-            self.lines = self.req.iter_lines()
-        else:
-            self.lines = open(url[8:], "rUb")
-        self.columns = self.next_line().split(',')
-    
-    def next_line(self):
-        """ Fetch the next line as a text string """
-        while True:
-            line = next(self.lines)
-            try:
-                return line.decode(encoding="utf-8")
-            except UnicodeDecodeError as e:
-                if not self.tdenv:
-                    raise e
-                self.tdenv.WARN(
-                    "{}: line:{}: {}\n{}",
-                    self.url, self.csvin.line_num, line, e
-                )
-    
-    def __iter__(self):
-        """
-        Iterate across data received as csv values.
-        Yields [column headings], [column values]
-        """
-        self.csvin = csvin = csv.reader(
-            iter(self.next_line, 'END'),
-            delimiter=',', quotechar="'", doublequote=True
-        )
-        columns = self.columns
-        for values in csvin:
-            if values and len(values) == len(columns):
-                yield columns, values
```

### Comparing `tradedangerous-11.1.6/tradedangerous/utils.py` & `tradedangerous-11.2.0/tradedangerous/utils.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradedangerous/version.py` & `tradedangerous-11.2.0/tradedangerous/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 # this software so long as you include this copyright notice.
 # I guarantee there is at least one bug neither of us knew about.
 # --------------------------------------------------------------------
 
 """just keeper of current version"""
 
 # TODO: remember to update tests when version changes
-__version__ = '11.1.6'
+__version__ = '11.2.0'
```

### Comparing `tradedangerous-11.1.6/tradedangerous.egg-info/PKG-INFO` & `tradedangerous-11.2.0/tradedangerous.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradedangerous
-Version: 11.1.6
+Version: 11.2.0
 Summary: Trade-Dangerous is a set of powerful trading tools for Elite Dangerous, organized around one of the most powerful trade run optimizers available.
 Home-page: https://github.com/eyeonus/Trade-Dangerous
 Author: eyeonus
 Author-email: eyeonus@gmail.com
 License: MPL
 Project-URL: Bug Tracker, https://github.com/eyeonus/Trade-Dangerous/issues
 Project-URL: Documentation, https://github.com/eyeonus/Trade-Dangerous/wiki
```

### Comparing `tradedangerous-11.1.6/tradedangerous.egg-info/SOURCES.txt` & `tradedangerous-11.2.0/tradedangerous.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.6/tradegui.py` & `tradedangerous-11.2.0/tradegui.py`

 * *Files identical despite different names*

