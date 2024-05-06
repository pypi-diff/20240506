# Comparing `tmp/safe_cli-1.0.0.tar.gz` & `tmp/safe_cli-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safe_cli-1.0.0.tar", last modified: Wed Jan 24 09:49:20 2024, max compression
+gzip compressed data, was "safe_cli-1.1.0.tar", last modified: Mon May  6 11:09:16 2024, max compression
```

## Comparing `safe_cli-1.0.0.tar` & `safe_cli-1.1.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 09:49:20.514562 safe_cli-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-01-24 09:49:10.000000 safe_cli-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15161 2024-01-24 09:49:20.514562 safe_cli-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14115 2024-01-24 09:49:10.000000 safe_cli-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 09:49:20.506562 safe_cli-1.0.0/safe_cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 09:49:10.000000 safe_cli-1.0.0/safe_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-01-24 09:49:10.000000 safe_cli-1.0.0/safe_cli/argparse_validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 09:49:20.506562 safe_cli-1.0.0/safe_cli/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-01-24 09:49:10.000000 safe_cli-1.0.0/safe_cli/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28478 2024-01-24 09:49:10.000000 safe_cli-1.0.0/safe_cli/contracts/safe_to_l2_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-01-24 09:49:10.000000 safe_cli-1.0.0/safe_cli/ethereum_hd_wallet.py
--rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-01-24 09:49:10.000000 safe_cli-1.0.0/safe_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 09:49:20.510562 safe_cli-1.0.0/safe_cli/operators/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-01-24 09:49:10.000000 safe_cli-1.0.0/safe_cli/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-01-24 09:49:10.000000 safe_cli-1.0.0/safe_cli/operators/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-01-24 09:49:10.000000 safe_cli-1.0.0/safe_cli/operators/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 09:49:20.510562 safe_cli-1.0.0/safe_cli/operators/hw_wallets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 09:49:10.000000 safe_cli-1.0.0/safe_cli/operators/hw_wallets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-01-24 09:49:10.000000 safe_cli-1.0.0/safe_cli/operators/hw_wallets/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-01-24 09:49:10.000000 safe_cli-1.0.0/safe_cli/operators/hw_wallets/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-01-24 09:49:10.000000 safe_cli-1.0.0/safe_cli/operators/hw_wallets/hw_wallet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7384 2024-01-24 09:49:10.000000 safe_cli-1.0.0/safe_cli/operators/hw_wallets/hw_wallet_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-01-24 09:49:10.000000 safe_cli-1.0.0/safe_cli/operators/hw_wallets/ledger_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-01-24 09:49:10.000000 safe_cli-1.0.0/safe_cli/operators/hw_wallets/ledger_wallet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-01-24 09:49:10.000000 safe_cli-1.0.0/safe_cli/operators/hw_wallets/trezor_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-01-24 09:49:10.000000 safe_cli-1.0.0/safe_cli/operators/hw_wallets/trezor_wallet.py
--rw-r--r--   0 runner    (1001) docker     (127)    46071 2024-01-24 09:49:10.000000 safe_cli-1.0.0/safe_cli/operators/safe_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)    15725 2024-01-24 09:49:10.000000 safe_cli-1.0.0/safe_cli/operators/safe_tx_service_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)    18985 2024-01-24 09:49:10.000000 safe_cli-1.0.0/safe_cli/prompt_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-01-24 09:49:10.000000 safe_cli-1.0.0/safe_cli/safe_addresses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-01-24 09:49:10.000000 safe_cli-1.0.0/safe_cli/safe_completer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9280 2024-01-24 09:49:10.000000 safe_cli-1.0.0/safe_cli/safe_completer_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-01-24 09:49:10.000000 safe_cli-1.0.0/safe_cli/safe_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-01-24 09:49:10.000000 safe_cli-1.0.0/safe_cli/safe_lexer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-01-24 09:49:10.000000 safe_cli-1.0.0/safe_cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-24 09:49:10.000000 safe_cli-1.0.0/safe_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 09:49:20.514562 safe_cli-1.0.0/safe_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15161 2024-01-24 09:49:20.000000 safe_cli-1.0.0/safe_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-01-24 09:49:20.000000 safe_cli-1.0.0/safe_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-24 09:49:20.000000 safe_cli-1.0.0/safe_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-01-24 09:49:20.000000 safe_cli-1.0.0/safe_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-01-24 09:49:20.000000 safe_cli-1.0.0/safe_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-24 09:49:20.000000 safe_cli-1.0.0/safe_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-01-24 09:49:20.514562 safe_cli-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-01-24 09:49:10.000000 safe_cli-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 09:49:20.514562 safe_cli-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 09:49:10.000000 safe_cli-1.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 09:49:20.514562 safe_cli-1.0.0/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 09:49:10.000000 safe_cli-1.0.0/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-01-24 09:49:10.000000 safe_cli-1.0.0/tests/mocks/balances_mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-01-24 09:49:10.000000 safe_cli-1.0.0/tests/mocks/data_decoded_mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-01-24 09:49:10.000000 safe_cli-1.0.0/tests/mocks/multisig_tx_mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-01-24 09:49:10.000000 safe_cli-1.0.0/tests/mocks/txs_mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-01-24 09:49:10.000000 safe_cli-1.0.0/tests/safe_cli_test_case_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-01-24 09:49:10.000000 safe_cli-1.0.0/tests/test_argparse_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-01-24 09:49:10.000000 safe_cli-1.0.0/tests/test_entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-01-24 09:49:10.000000 safe_cli-1.0.0/tests/test_ethereum_hd_wallet.py
--rw-r--r--   0 runner    (1001) docker     (127)     8216 2024-01-24 09:49:10.000000 safe_cli-1.0.0/tests/test_hw_wallet_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     8870 2024-01-24 09:49:10.000000 safe_cli-1.0.0/tests/test_ledger_wallet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-01-24 09:49:10.000000 safe_cli-1.0.0/tests/test_safe_addresses.py
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-01-24 09:49:10.000000 safe_cli-1.0.0/tests/test_safe_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-01-24 09:49:10.000000 safe_cli-1.0.0/tests/test_safe_completer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-01-24 09:49:10.000000 safe_cli-1.0.0/tests/test_safe_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-01-24 09:49:10.000000 safe_cli-1.0.0/tests/test_safe_lexer.py
--rw-r--r--   0 runner    (1001) docker     (127)    21356 2024-01-24 09:49:10.000000 safe_cli-1.0.0/tests/test_safe_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)    17588 2024-01-24 09:49:10.000000 safe_cli-1.0.0/tests/test_safe_tx_service_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9082 2024-01-24 09:49:10.000000 safe_cli-1.0.0/tests/test_trezor_wallet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-01-24 09:49:10.000000 safe_cli-1.0.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-01-24 09:49:10.000000 safe_cli-1.0.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:16.845550 safe_cli-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-06 11:09:06.000000 safe_cli-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-05-06 11:09:16.845550 safe_cli-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-06 11:09:06.000000 safe_cli-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:16.837550 safe_cli-1.1.0/safe_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:06.000000 safe_cli-1.1.0/safe_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-06 11:09:06.000000 safe_cli-1.1.0/safe_cli/argparse_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:16.837550 safe_cli-1.1.0/safe_cli/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-06 11:09:06.000000 safe_cli-1.1.0/safe_cli/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28478 2024-05-06 11:09:06.000000 safe_cli-1.1.0/safe_cli/contracts/safe_to_l2_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-06 11:09:06.000000 safe_cli-1.1.0/safe_cli/ethereum_hd_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-05-06 11:09:06.000000 safe_cli-1.1.0/safe_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:16.841550 safe_cli-1.1.0/safe_cli/operators/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-06 11:09:06.000000 safe_cli-1.1.0/safe_cli/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-06 11:09:06.000000 safe_cli-1.1.0/safe_cli/operators/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-06 11:09:06.000000 safe_cli-1.1.0/safe_cli/operators/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:16.841550 safe_cli-1.1.0/safe_cli/operators/hw_wallets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:06.000000 safe_cli-1.1.0/safe_cli/operators/hw_wallets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-06 11:09:06.000000 safe_cli-1.1.0/safe_cli/operators/hw_wallets/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-06 11:09:06.000000 safe_cli-1.1.0/safe_cli/operators/hw_wallets/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-06 11:09:06.000000 safe_cli-1.1.0/safe_cli/operators/hw_wallets/hw_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7501 2024-05-06 11:09:06.000000 safe_cli-1.1.0/safe_cli/operators/hw_wallets/hw_wallet_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-06 11:09:06.000000 safe_cli-1.1.0/safe_cli/operators/hw_wallets/ledger_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-06 11:09:06.000000 safe_cli-1.1.0/safe_cli/operators/hw_wallets/ledger_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-06 11:09:06.000000 safe_cli-1.1.0/safe_cli/operators/hw_wallets/trezor_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-05-06 11:09:06.000000 safe_cli-1.1.0/safe_cli/operators/hw_wallets/trezor_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46368 2024-05-06 11:09:06.000000 safe_cli-1.1.0/safe_cli/operators/safe_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18731 2024-05-06 11:09:06.000000 safe_cli-1.1.0/safe_cli/operators/safe_tx_service_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19504 2024-05-06 11:09:06.000000 safe_cli-1.1.0/safe_cli/prompt_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-05-06 11:09:06.000000 safe_cli-1.1.0/safe_cli/safe_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-06 11:09:06.000000 safe_cli-1.1.0/safe_cli/safe_completer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9529 2024-05-06 11:09:06.000000 safe_cli-1.1.0/safe_cli/safe_completer_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-05-06 11:09:06.000000 safe_cli-1.1.0/safe_cli/safe_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-06 11:09:06.000000 safe_cli-1.1.0/safe_cli/safe_lexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-06 11:09:06.000000 safe_cli-1.1.0/safe_cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-06 11:09:06.000000 safe_cli-1.1.0/safe_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:16.845550 safe_cli-1.1.0/safe_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-05-06 11:09:16.000000 safe_cli-1.1.0/safe_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-06 11:09:16.000000 safe_cli-1.1.0/safe_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 11:09:16.000000 safe_cli-1.1.0/safe_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-06 11:09:16.000000 safe_cli-1.1.0/safe_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-06 11:09:16.000000 safe_cli-1.1.0/safe_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-06 11:09:16.000000 safe_cli-1.1.0/safe_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-06 11:09:16.849550 safe_cli-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-06 11:09:06.000000 safe_cli-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:16.845550 safe_cli-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:06.000000 safe_cli-1.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:16.845550 safe_cli-1.1.0/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:06.000000 safe_cli-1.1.0/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-05-06 11:09:06.000000 safe_cli-1.1.0/tests/mocks/balances_mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-05-06 11:09:06.000000 safe_cli-1.1.0/tests/mocks/data_decoded_mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-06 11:09:06.000000 safe_cli-1.1.0/tests/mocks/multisig_tx_mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-05-06 11:09:06.000000 safe_cli-1.1.0/tests/mocks/txs_mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-06 11:09:06.000000 safe_cli-1.1.0/tests/safe_cli_test_case_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-06 11:09:06.000000 safe_cli-1.1.0/tests/test_argparse_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-05-06 11:09:06.000000 safe_cli-1.1.0/tests/test_entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-06 11:09:06.000000 safe_cli-1.1.0/tests/test_ethereum_hd_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8216 2024-05-06 11:09:06.000000 safe_cli-1.1.0/tests/test_hw_wallet_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8870 2024-05-06 11:09:06.000000 safe_cli-1.1.0/tests/test_ledger_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-06 11:09:06.000000 safe_cli-1.1.0/tests/test_safe_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-06 11:09:06.000000 safe_cli-1.1.0/tests/test_safe_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-06 11:09:06.000000 safe_cli-1.1.0/tests/test_safe_completer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-06 11:09:06.000000 safe_cli-1.1.0/tests/test_safe_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-06 11:09:06.000000 safe_cli-1.1.0/tests/test_safe_lexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21356 2024-05-06 11:09:06.000000 safe_cli-1.1.0/tests/test_safe_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19108 2024-05-06 11:09:06.000000 safe_cli-1.1.0/tests/test_safe_tx_service_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9113 2024-05-06 11:09:06.000000 safe_cli-1.1.0/tests/test_trezor_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-06 11:09:06.000000 safe_cli-1.1.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-06 11:09:06.000000 safe_cli-1.1.0/tests/utils.py
```

### Comparing `safe_cli-1.0.0/LICENSE` & `safe_cli-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `safe_cli-1.0.0/safe_cli/argparse_validators.py` & `safe_cli-1.1.0/safe_cli/argparse_validators.py`

 * *Files identical despite different names*

### Comparing `safe_cli-1.0.0/safe_cli/contracts/safe_to_l2_migration.py` & `safe_cli-1.1.0/safe_cli/contracts/safe_to_l2_migration.py`

 * *Files identical despite different names*

### Comparing `safe_cli-1.0.0/safe_cli/ethereum_hd_wallet.py` & `safe_cli-1.1.0/safe_cli/ethereum_hd_wallet.py`

 * *Files identical despite different names*

### Comparing `safe_cli-1.0.0/safe_cli/main.py` & `safe_cli-1.1.0/safe_cli/main.py`

 * *Files identical despite different names*

### Comparing `safe_cli-1.0.0/safe_cli/operators/exceptions.py` & `safe_cli-1.1.0/safe_cli/operators/exceptions.py`

 * *Files identical despite different names*

### Comparing `safe_cli-1.0.0/safe_cli/operators/hw_wallets/hw_wallet.py` & `safe_cli-1.1.0/safe_cli/operators/hw_wallets/hw_wallet.py`

 * *Files identical despite different names*

### Comparing `safe_cli-1.0.0/safe_cli/operators/hw_wallets/hw_wallet_manager.py` & `safe_cli-1.1.0/safe_cli/operators/hw_wallets/hw_wallet_manager.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 
 from eth_typing import ChecksumAddress
 from hexbytes import HexBytes
 from prompt_toolkit import HTML, print_formatted_text
 from web3.types import TxParams, Wei
 
 from gnosis.eth import TxSpeed
-from gnosis.eth.eip712 import eip712_encode
+from gnosis.eth.eip712 import eip712_encode, eip712_encode_hash
 from gnosis.safe import SafeTx
+from gnosis.safe.safe_signature import SafeSignature, SafeSignatureEOA
 
 from .hw_wallet import HwWallet
 
 
 class HwWalletType(Enum):
     TREZOR = 0
     LEDGER = 1
@@ -29,22 +30,22 @@
         self.wallets: Set[HwWallet] = set()
         self.supported_hw_wallet_types: Dict[str, HwWallet] = {}
         self.sender: Optional[HwWallet] = None
         try:
             from .ledger_wallet import LedgerWallet
 
             self.supported_hw_wallet_types[HwWalletType.LEDGER] = LedgerWallet
-        except (ImportError):
+        except ImportError:
             pass
 
         try:
             from .trezor_wallet import TrezorWallet
 
             self.supported_hw_wallet_types[HwWalletType.TREZOR] = TrezorWallet
-        except (ImportError):
+        except ImportError:
             pass
 
     def is_supported_hw_wallet(self, hw_wallet_type: HwWalletType) -> bool:
         return hw_wallet_type in self.supported_hw_wallet_types
 
     def get_hw_wallet(self, hw_wallet_type: HwWalletType) -> Optional[HwWallet]:
         if hw_wallet_type in self.supported_hw_wallet_types:
@@ -109,48 +110,48 @@
                 if account.address == address:
                     if self.sender and self.sender.address == address:
                         self.sender = None
                     accounts_to_remove.add(account)
         self.wallets = self.wallets.difference(accounts_to_remove)
         return accounts_to_remove
 
-    def sign_eip712(self, safe_tx: SafeTx, wallets: List[HwWallet]) -> SafeTx:
+    def sign_eip712(self, eip712_message: Dict, wallets: List[HwWallet]) -> HexBytes:
         """
-        Sign a safeTx EIP-712 hashes with supported hw wallet devices
+        Sign an EIP712 message
 
-        :param domain_hash:
-        :param message_hash:
-        :param wallets: list of HwWallet
-        :return: signed safeTx
-        """
-        encode_hash = eip712_encode(safe_tx.eip712_structured_data)
-        domain_hash = encode_hash[1]
-        message_hash = encode_hash[2]
+        :param eip712_message:
+        :param wallets:
+        :return: Appended sorted signatures for all the provided wallets
+        """
+        _, domain_hash, message_hash = eip712_encode(eip712_message)
+        eip712_message_hash = eip712_encode_hash(eip712_message)
+        safe_signatures: List[SafeSignature] = []
         for wallet in wallets:
             print_formatted_text(
                 HTML(
                     f"<ansired>Make sure before signing in your {wallet} that the domain_hash and message_hash are both correct</ansired>"
                 )
             )
             print_formatted_text(HTML(f"Domain_hash: <b>{domain_hash.hex()}</b>"))
             print_formatted_text(HTML(f"Message_hash: <b>{message_hash.hex()}</b>"))
             signature = wallet.sign_typed_hash(domain_hash, message_hash)
+            safe_signatures.append(SafeSignatureEOA(signature, eip712_message_hash))
 
-            # Insert signature sorted
-            if wallet.address not in safe_tx.signers:
-                new_owners = safe_tx.signers + [wallet.address]
-                new_owner_pos = sorted(new_owners, key=lambda x: int(x, 16)).index(
-                    wallet.address
-                )
-                safe_tx.signatures = (
-                    safe_tx.signatures[: 65 * new_owner_pos]
-                    + signature
-                    + safe_tx.signatures[65 * new_owner_pos :]
-                )
+        return SafeSignature.export_signatures(safe_signatures)
 
+    def sign_safe_tx(self, safe_tx: SafeTx, wallets: List[HwWallet]) -> SafeTx:
+        """
+        Sign a safe transaction with the provided hardware wallets
+
+        :param safe_tx:
+        :param wallets:
+        :return: SafeTx with signature.
+        """
+        signatures = self.sign_eip712(safe_tx.eip712_structured_data, wallets)
+        safe_tx.signatures = signatures
         return safe_tx
 
     def execute_safe_tx(
         self,
         safe_tx: SafeTx,
         tx_gas: Optional[int] = None,
         tx_gas_price: Optional[int] = None,
```

### Comparing `safe_cli-1.0.0/safe_cli/operators/hw_wallets/ledger_exceptions.py` & `safe_cli-1.1.0/safe_cli/operators/hw_wallets/ledger_exceptions.py`

 * *Files identical despite different names*

### Comparing `safe_cli-1.0.0/safe_cli/operators/hw_wallets/ledger_wallet.py` & `safe_cli-1.1.0/safe_cli/operators/hw_wallets/ledger_wallet.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,13 +65,13 @@
         signed_transaction = create_transaction(
             destination=tx_parameters["to"],
             amount=tx_parameters["value"],
             gas=tx_parameters["gas"],
             nonce=tx_parameters["nonce"],
             data=tx_parameters.get("data"),
             max_priority_fee_per_gas=tx_parameters.get("maxPriorityFeePerGas"),
-            max_fee_per_gas=tx_parameters.get("maxPriorityFeePerGas"),
+            max_fee_per_gas=tx_parameters.get("maxFeePerGas"),
             chain_id=chain_id,
             sender_path=self.derivation_path,
             dongle=self.dongle,
         )
         return HexBytes(signed_transaction.raw_transaction())
```

### Comparing `safe_cli-1.0.0/safe_cli/operators/hw_wallets/trezor_exceptions.py` & `safe_cli-1.1.0/safe_cli/operators/hw_wallets/trezor_exceptions.py`

 * *Files identical despite different names*

### Comparing `safe_cli-1.0.0/safe_cli/operators/hw_wallets/trezor_wallet.py` & `safe_cli-1.1.0/safe_cli/operators/hw_wallets/trezor_wallet.py`

 * *Files identical despite different names*

### Comparing `safe_cli-1.0.0/safe_cli/operators/safe_operator.py` & `safe_cli-1.1.0/safe_cli/operators/safe_operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     get_erc20_contract,
     get_erc721_contract,
     get_safe_V1_1_1_contract,
     get_sign_message_lib_contract,
 )
 from gnosis.eth.eip712 import eip712_encode
 from gnosis.eth.utils import get_empty_tx_params
-from gnosis.safe import InvalidInternalTx, Safe, SafeOperation, SafeTx
+from gnosis.safe import InvalidInternalTx, Safe, SafeOperationEnum, SafeTx
 from gnosis.safe.api import TransactionServiceApi
 from gnosis.safe.multi_send import MultiSend, MultiSendOperation, MultiSendTx
 from gnosis.safe.safe_deployments import safe_deployments
 
 from safe_cli.ethereum_hd_wallet import get_account_from_words
 from safe_cli.operators.exceptions import (
     AccountNotLoadedException,
@@ -220,15 +220,17 @@
         if self.safe_cli_info.master_copy == last_safe_contract_address:
             return True
         else:  # Check versions, maybe safe-cli addresses were not updated
             try:
                 safe_contract_version = Safe(
                     last_safe_contract_address, self.ethereum_client
                 ).retrieve_version()
-            except BadFunctionCallOutput:  # Safe master copy is not deployed or errored, maybe custom network
+            except (
+                BadFunctionCallOutput
+            ):  # Safe master copy is not deployed or errored, maybe custom network
                 return True  # We cannot say you are not updated ¯\_(ツ)_/¯
 
             return semantic_version.parse(
                 self.safe_cli_info.version
             ) >= semantic_version.parse(safe_contract_version)
 
     def load_cli_owners_from_words(self, words: List[str]):
@@ -474,15 +476,15 @@
             )["data"]
         )
         print_formatted_text(HTML(f"Signing message: \n {message}"))
         if self.prepare_and_execute_safe_transaction(
             sign_message_lib_address,
             0,
             sign_message_data,
-            operation=SafeOperation.DELEGATE_CALL,
+            operation=SafeOperationEnum.DELEGATE_CALL,
         ):
             print_formatted_text(
                 HTML(f"Message was signed correctly: {safe_message_hash.hex()}")
             )
 
     def add_owner(self, new_owner: str, threshold: Optional[int] = None) -> bool:
         threshold = threshold if threshold is not None else self.safe_cli_info.threshold
@@ -529,15 +531,17 @@
         safe_nonce: Optional[int] = None,
         delegate_call: bool = False,
     ) -> bool:
         if value > 0:
             safe_balance = self.ethereum_client.get_balance(self.address)
             if safe_balance < value:
                 raise NotEnoughEtherToSend(safe_balance)
-        operation = SafeOperation.DELEGATE_CALL if delegate_call else SafeOperation.CALL
+        operation = (
+            SafeOperationEnum.DELEGATE_CALL if delegate_call else SafeOperationEnum.CALL
+        )
         return self.prepare_and_execute_safe_transaction(
             to, value, data, operation, safe_nonce=safe_nonce
         )
 
     def send_ether(self, to: str, value: int, **kwargs) -> bool:
         return self.send_custom(to, value, b"", **kwargs)
 
@@ -663,15 +667,18 @@
                 ).build_transaction(tx_params)["data"],
             )
         ]
 
         multisend_data = multisend.build_tx_data(multisend_txs)
 
         if self.prepare_and_execute_safe_transaction(
-            multisend.address, 0, multisend_data, operation=SafeOperation.DELEGATE_CALL
+            multisend.address,
+            0,
+            multisend_data,
+            operation=SafeOperationEnum.DELEGATE_CALL,
         ):
             self.safe_cli_info.master_copy = self.last_safe_contract_address
             self.safe_cli_info.fallback_handler = (
                 self.last_default_fallback_handler_address
             )
             self.safe_cli_info.version = self.safe.retrieve_version()
 
@@ -722,15 +729,18 @@
             )
         else:
             raise InvalidMasterCopyException(
                 "Current version is not supported to migrate to L2"
             )
 
         if self.prepare_and_execute_safe_transaction(
-            migration_contract_address, 0, data, operation=SafeOperation.DELEGATE_CALL
+            migration_contract_address,
+            0,
+            data,
+            operation=SafeOperationEnum.DELEGATE_CALL,
         ):
             self.safe_cli_info.master_copy = safe_l2_singleton
             self.safe_cli_info.fallback_handler = fallback_handler
             self.safe_cli_info.version = self.safe.retrieve_version()
 
     def change_threshold(self, threshold: int):
         if threshold == self.safe_cli_info.threshold:
@@ -884,29 +894,29 @@
         return self.prepare_and_execute_safe_transaction(self.address, 0, data)
 
     def prepare_safe_transaction(
         self,
         to: str,
         value: int,
         data: bytes,
-        operation: SafeOperation = SafeOperation.CALL,
+        operation: SafeOperationEnum = SafeOperationEnum.CALL,
         safe_nonce: Optional[int] = None,
     ) -> SafeTx:
         safe_tx = self.safe.build_multisig_tx(
             to, value, data, operation=operation.value, safe_nonce=safe_nonce
         )
         self.sign_transaction(safe_tx)  # Raises exception if it cannot be signed
         return safe_tx
 
     def prepare_and_execute_safe_transaction(
         self,
         to: str,
         value: int,
         data: bytes,
-        operation: SafeOperation = SafeOperation.CALL,
+        operation: SafeOperationEnum = SafeOperationEnum.CALL,
         safe_nonce: Optional[int] = None,
     ) -> bool:
         safe_tx = self.prepare_safe_transaction(
             to, value, data, operation, safe_nonce=safe_nonce
         )
         return self.execute_safe_transaction(safe_tx)
 
@@ -1007,15 +1017,15 @@
         elif multisend:
             safe_tx = SafeTx(
                 self.ethereum_client,
                 self.address,
                 multisend.address,
                 0,
                 multisend.build_tx_data(multisend_txs),
-                SafeOperation.DELEGATE_CALL.value,
+                SafeOperationEnum.DELEGATE_CALL.value,
                 0,
                 0,
                 0,
                 None,
                 None,
                 safe_nonce=safe_nonce,
             )
@@ -1035,17 +1045,17 @@
     def get_signers(self) -> Tuple[List[LocalAccount], List[HwWallet]]:
         """
 
         :return: Tuple with eoa signers and hw_wallet signers
         """
         permitted_signers = self.get_permitted_signers()
         threshold = self.safe_cli_info.threshold
-        eoa_signers: List[
-            Account
-        ] = []  # Some accounts that are not an owner can be loaded
+        eoa_signers: List[Account] = (
+            []
+        )  # Some accounts that are not an owner can be loaded
         for account in self.accounts:
             if account.address in permitted_signers:
                 eoa_signers.append(account)
                 threshold -= 1
                 if threshold == 0:
                     break
         # If still pending required signatures continue with ledger owners
@@ -1067,15 +1077,15 @@
     def sign_transaction(self, safe_tx: SafeTx) -> SafeTx:
         eoa_signers, hw_wallets_signers = self.get_signers()
         for selected_account in eoa_signers:
             safe_tx.sign(selected_account.key)
 
         # Sign with ledger
         if len(hw_wallets_signers):
-            safe_tx = self.hw_wallet_manager.sign_eip712(safe_tx, hw_wallets_signers)
+            safe_tx = self.hw_wallet_manager.sign_safe_tx(safe_tx, hw_wallets_signers)
 
         return safe_tx
 
     @require_tx_service
     def _require_tx_service_mode(self):
         print_formatted_text(
             HTML(
@@ -1129,27 +1139,27 @@
                     .build_transaction({"from": self.address, "gas": 0, "gasPrice": 0})
                 )
 
                 safe_tx = self.prepare_safe_transaction(
                     token_address,
                     0,
                     HexBytes(transaction["data"]),
-                    SafeOperation.CALL,
+                    SafeOperationEnum.CALL,
                     safe_nonce=None,
                 )
                 safe_txs.append(safe_tx)
 
         # Getting ethereum balance
         balance_eth = self.ethereum_client.get_balance(self.address)
         if balance_eth:
             safe_tx = self.prepare_safe_transaction(
                 to,
                 balance_eth,
                 b"",
-                SafeOperation.CALL,
+                SafeOperationEnum.CALL,
                 safe_nonce=None,
             )
             safe_txs.append(safe_tx)
 
         if safe_txs:
             multisend_tx = self.batch_safe_txs(self.get_nonce(), safe_txs)
             if multisend_tx is not None:
@@ -1160,14 +1170,17 @@
                         )
                     )
         else:
             print_formatted_text(
                 HTML("<ansigreen>Safe account is currently empty</ansigreen>")
             )
 
+    def remove_proposed_transaction(self, safe_tx_hash: bytes):
+        return self._require_tx_service_mode()
+
     def process_command(self, first_command: str, rest_command: List[str]) -> bool:
         if first_command == "help":
             print_formatted_text("I still cannot help you")
         elif first_command == "refresh":
             print_formatted_text("Reloading Safe information")
             self.refresh_safe_cli_info()
```

### Comparing `safe_cli-1.0.0/safe_cli/operators/safe_tx_service_operator.py` & `safe_cli-1.1.0/safe_cli/operators/safe_tx_service_operator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 import json
-from typing import Any, Dict, List, Optional, Sequence, Set
+from itertools import chain
+from typing import Any, Dict, List, Optional, Sequence, Set, Union
 
 from colorama import Fore, Style
 from eth_account.messages import defunct_hash_message
+from eth_account.signers.local import LocalAccount
 from eth_typing import ChecksumAddress
 from hexbytes import HexBytes
 from prompt_toolkit import HTML, print_formatted_text
 from tabulate import tabulate
 
 from gnosis.eth.contracts import get_erc20_contract
 from gnosis.eth.eip712 import eip712_encode_hash
-from gnosis.safe import SafeOperation, SafeTx
+from gnosis.safe import SafeOperationEnum, SafeTx
 from gnosis.safe.api import SafeAPIException
+from gnosis.safe.api.transaction_service_api.transaction_service_messages import (
+    get_remove_transaction_message,
+)
 from gnosis.safe.multi_send import MultiSend, MultiSendOperation, MultiSendTx
 from gnosis.safe.safe_signature import SafeSignature, SafeSignatureEOA
 from gnosis.safe.signatures import signature_to_bytes
 
 from safe_cli.utils import yes_or_no_question
 
 from . import SafeServiceNotAvailable
 from .exceptions import AccountNotLoadedException, NonExistingOwnerException
+from .hw_wallets.hw_wallet import HwWallet
 from .safe_operator import SafeOperator
 
 
 class SafeTxServiceOperator(SafeOperator):
     def __init__(self, address: str, node_url: str):
         super().__init__(address, node_url)
         if not self.safe_tx_service:
@@ -60,16 +66,21 @@
             signature = signature_to_bytes(
                 signature_dict["v"], signature_dict["r"], signature_dict["s"]
             )
             safe_signatures.append(SafeSignatureEOA(signature, safe_message_hash))
 
         signatures = SafeSignature.export_signatures(safe_signatures)
 
-        if len(hw_wallet_signers):
-            raise NotImplementedError("SignHash by hardware wallet is not implemented")
+        if hw_wallet_signers:
+            print_formatted_text(
+                HTML(
+                    "<ansired>Signing messages is not currently supported by hardware wallets</ansired>"
+                )
+            )
+            return False
 
         if self.safe_tx_service.post_message(self.address, message, signatures):
             print_formatted_text(
                 HTML(
                     "<ansigreen>Message was correctly created on Safe Transaction Service</ansigreen>"
                 )
             )
@@ -152,15 +163,15 @@
             # Check if there are ledger signers
             if self.hw_wallet_manager.wallets:
                 selected_ledger_accounts = []
                 for ledger_account in self.hw_wallet_manager.wallets:
                     if ledger_account.address in owners:
                         selected_ledger_accounts.append(ledger_account)
                 if len(selected_ledger_accounts) > 0:
-                    safe_tx = self.hw_wallet_manager.sign_eip712(
+                    safe_tx = self.hw_wallet_manager.sign_safe_tx(
                         safe_tx, selected_ledger_accounts
                     )
 
             if safe_tx.signers:
                 self.safe_tx_service.post_signatures(safe_tx_hash, safe_tx.signatures)
                 print_formatted_text(
                     HTML(
@@ -211,15 +222,15 @@
         if len(multisend_txs) > 1:
             safe_tx = SafeTx(
                 self.ethereum_client,
                 self.address,
                 multisend.address,
                 0,
                 multisend.build_tx_data(multisend_txs),
-                SafeOperation.DELEGATE_CALL.value,
+                SafeOperationEnum.DELEGATE_CALL.value,
                 0,
                 0,
                 0,
                 None,
                 None,
                 safe_nonce=safe_nonce,
             )
@@ -322,15 +333,15 @@
         return rows
 
     def prepare_and_execute_safe_transaction(
         self,
         to: str,
         value: int,
         data: bytes,
-        operation: SafeOperation = SafeOperation.CALL,
+        operation: SafeOperationEnum = SafeOperationEnum.CALL,
         safe_nonce: Optional[int] = None,
     ) -> bool:
         safe_tx = self.prepare_safe_transaction(
             to, value, data, operation, safe_nonce=safe_nonce
         )
         return self.post_transaction_to_tx_service(safe_tx)
 
@@ -371,28 +382,28 @@
             amount = int(balance["balance"])
             if balance["tokenAddress"] is None:  # Then is ether
                 if amount != 0:
                     safe_tx = self.prepare_safe_transaction(
                         to,
                         amount,
                         b"",
-                        SafeOperation.CALL,
+                        SafeOperationEnum.CALL,
                         safe_nonce=None,
                     )
             else:
                 transaction = (
                     get_erc20_contract(self.ethereum_client.w3, balance["tokenAddress"])
                     .functions.transfer(to, amount)
                     .build_transaction({"from": self.address, "gas": 0, "gasPrice": 0})
                 )
                 safe_tx = self.prepare_safe_transaction(
                     balance["tokenAddress"],
                     0,
                     HexBytes(transaction["data"]),
-                    SafeOperation.CALL,
+                    SafeOperationEnum.CALL,
                     safe_nonce=None,
                 )
             if safe_tx:
                 safe_txs.append(safe_tx)
         if len(safe_txs) > 0:
             multisend_tx = self.batch_safe_txs(safe_tx.safe_nonce, safe_txs)
             if multisend_tx is not None:
@@ -402,7 +413,69 @@
                         "<ansigreen>Transaction to drain account correctly created</ansigreen>"
                     )
                 )
         else:
             print_formatted_text(
                 HTML("<ansigreen>Safe account is currently empty</ansigreen>")
             )
+
+    def search_account(
+        self, address: ChecksumAddress
+    ) -> Optional[Union[LocalAccount, HwWallet]]:
+        """
+        Search the provided address between loaded owners
+
+        :param address:
+        :return: LocalAccount or HwWallet of the provided address
+        """
+        for account in chain(self.accounts, self.hw_wallet_manager.wallets):
+            if account.address == address:
+                return account
+
+    def remove_proposed_transaction(self, safe_tx_hash: bytes):
+        eip712_message = get_remove_transaction_message(
+            self.address, safe_tx_hash, self.ethereum_client.get_chain_id()
+        )
+        message_hash = eip712_encode_hash(eip712_message)
+        try:
+            safe_tx, _ = self.safe_tx_service.get_safe_transaction(safe_tx_hash)
+            signer = self.search_account(safe_tx.proposer)
+            if not signer:
+                print_formatted_text(
+                    HTML(
+                        f"<ansired>The proposer with address: {safe_tx.proposer} was not loaded</ansired>"
+                    )
+                )
+                return False
+
+            if isinstance(signer, LocalAccount):
+                signature = signer.signHash(message_hash).signature
+            else:
+                signature = self.hw_wallet_manager.sign_eip712(eip712_message, [signer])
+
+            if len(safe_tx.signers) >= self.safe.retrieve_threshold():
+                print_formatted_text(
+                    HTML(
+                        "<ansired>The transaction has all the required signatures to be executed!!!\n"
+                        "This means that the transaction can be executed by a 3rd party monitoring your Safe even after removal!\n"
+                        f"Make sure you execute a transaction with nonce {safe_tx.safe_nonce} to void the current transaction"
+                        "</ansired>"
+                    )
+                )
+
+            if not yes_or_no_question(
+                f"Do you want to remove the tx with safe-tx-hash={safe_tx.safe_tx_hash.hex()}"
+            ):
+                return False
+
+            self.safe_tx_service.delete_transaction(safe_tx_hash.hex(), signature.hex())
+            print_formatted_text(
+                HTML(
+                    f"<ansigreen>Transaction {safe_tx_hash.hex()} was removed correctly</ansigreen>"
+                )
+            )
+            return True
+        except SafeAPIException as e:
+            print_formatted_text(
+                HTML(f"<ansired>Transaction wasn't removed due an error: {e}</ansired>")
+            )
+            return False
```

### Comparing `safe_cli-1.0.0/safe_cli/prompt_parser.py` & `safe_cli-1.1.0/safe_cli/prompt_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -311,14 +311,18 @@
     def add_delegate(args):
         safe_operator.add_delegate(args.address, args.label, args.signer)
 
     @safe_exception
     def remove_delegate(args):
         safe_operator.remove_delegate(args.address, args.signer)
 
+    @safe_exception
+    def remove_proposed_transaction(args):
+        safe_operator.remove_proposed_transaction(args.safe_tx_hash)
+
     # Cli owners
     parser_show_cli_owners = subparsers.add_parser("show_cli_owners")
     parser_show_cli_owners.set_defaults(func=show_cli_owners)
 
     parser_load_cli_owners_from_words = subparsers.add_parser(
         "load_cli_owners_from_words"
     )
@@ -495,24 +499,26 @@
     parser_tx_service.set_defaults(func=get_balances)
 
     parser_tx_service = subparsers.add_parser("history")
     parser_tx_service.set_defaults(func=get_history)
 
     parser_tx_service = subparsers.add_parser("sign-tx")
     parser_tx_service.set_defaults(func=sign_tx)
-    parser_tx_service.add_argument("safe_tx_hash", type=check_hex_str)
+    parser_tx_service.add_argument("safe_tx_hash", type=check_keccak256_hash)
 
     parser_tx_service = subparsers.add_parser("batch-txs")
     parser_tx_service.set_defaults(func=batch_txs)
     parser_tx_service.add_argument("safe_nonce", type=int)
-    parser_tx_service.add_argument("safe_tx_hashes", type=check_hex_str, nargs="+")
+    parser_tx_service.add_argument(
+        "safe_tx_hashes", type=check_keccak256_hash, nargs="+"
+    )
 
     parser_tx_service = subparsers.add_parser("execute-tx")
     parser_tx_service.set_defaults(func=execute_tx)
-    parser_tx_service.add_argument("safe_tx_hash", type=check_hex_str)
+    parser_tx_service.add_argument("safe_tx_hash", type=check_keccak256_hash)
 
     # List delegates
     parser_delegates = subparsers.add_parser("get_delegates")
     parser_delegates.set_defaults(func=get_delegates)
 
     # Add delegate
     parser_add_delegate = subparsers.add_parser("add_delegate")
@@ -523,8 +529,17 @@
 
     # Remove delegate
     parser_remove_delegate = subparsers.add_parser("remove_delegate")
     parser_remove_delegate.set_defaults(func=remove_delegate)
     parser_remove_delegate.add_argument("address", type=check_ethereum_address)
     parser_remove_delegate.add_argument("signer", type=check_ethereum_address)
 
+    # Remove not executed proposed transaction
+    parser_remove_proposed_transaction = subparsers.add_parser(
+        "remove_proposed_transaction"
+    )
+    parser_remove_proposed_transaction.set_defaults(func=remove_proposed_transaction)
+    parser_remove_proposed_transaction.add_argument(
+        "safe_tx_hash", type=check_keccak256_hash
+    )
+
     return prompt_parser
```

### Comparing `safe_cli-1.0.0/safe_cli/safe_addresses.py` & `safe_cli-1.1.0/safe_cli/safe_addresses.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Get the correct addresses for the contracts by testing the deployment addresses using the RPC
 Currently using Safe v1.4.1 when available, and 1.3.0 as fallback as they are compatible
 https://github.com/gnosis/safe-deployments/tree/main/src/assets/v1.4.1
 https://github.com/gnosis/safe-deployments/tree/main/src/assets/v1.3.0
 """
+
 from typing import Sequence
 
 from eth_typing import ChecksumAddress
 
 from gnosis.eth import EthereumClient
```

### Comparing `safe_cli-1.0.0/safe_cli/safe_completer.py` & `safe_cli-1.1.0/safe_cli/safe_completer.py`

 * *Files identical despite different names*

### Comparing `safe_cli-1.0.0/safe_cli/safe_completer_constants.py` & `safe_cli-1.1.0/safe_cli/safe_completer_constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     "load_cli_owners": "<account-private-key> [<account-private-key>...]",
     "load_ledger_cli_owners": "[--legacy-accounts] [--derivation-path <str>]",
     "load_trezor_cli_owners": "[--legacy-accounts] [--derivation-path <str>]",
     "load_cli_owners_from_words": "<word_1> <word_2> ... <word_12>",
     "refresh": "",
     "remove_delegate": "<address> <signer-address>",
     "remove_owner": "<address> [--threshold <int>]",
+    "remove_proposed_transaction": "safe-tx-hash",
     "send_custom": "<address> <value-wei> <data> [--delegate] [--safe-nonce <int>]",
     "send_erc20": "<address> <token-address> <value-wei> [--safe-nonce <int>]",
     "send_erc721": "<address> <token-address> <token-id> [--safe-nonce <int>]",
     "send_ether": "<address> <value-wei> [--safe-nonce <int>]",
     "show_cli_owners": "(read-only)",
     "sign_message": "[--eip191_message <str>] [--eip712_path <file-path>]",
     "sign-tx": "<safe-tx-hash>",
@@ -114,14 +115,18 @@
     "add_delegate": HTML(
         "Command <b>add_delegate</b> will add a check-summed <u>&lt;address&gt;</u> delegate account."
     ),
     "remove_delegate": HTML(
         "Command <b>remove_delegate</b> will remove a delegate <u>&lt;address&gt;</u> from the "
         "current loaded safe."
     ),
+    "remove_proposed_transaction": HTML(
+        "Command <b>remove_proposed_transaction</b> will remove proposed not executed transaction for "
+        "provided<u>&lt;safe-tx-hash&gt;</u>"
+    ),
     "enable_module": HTML(
         "Command <b>enable_module</b> will enable a check-summed <u>&lt;address&gt;</u> module."
     ),
     "disable_module": HTML(
         "Command <b>disable_module</b> will disable a check-summed <u>&lt;address&gt;</u> module."
     ),
     "get_threshold": HTML(
```

### Comparing `safe_cli-1.0.0/safe_cli/safe_creator.py` & `safe_cli-1.1.0/safe_cli/safe_creator.py`

 * *Files identical despite different names*

### Comparing `safe_cli-1.0.0/safe_cli/safe_lexer.py` & `safe_cli-1.1.0/safe_cli/safe_lexer.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         "remove_owner",
         "change_master_copy",
         "add_delegate",
         "remove_delegate",
         "send_ether",
         "send_erc20",
         "send_erc721",
+        "remove_proposed_transaction",
     }
 
     def get_tokens_unprocessed(self, text: str) -> (int, Token, str):
         for index, token, value in BashLexer.get_tokens_unprocessed(self, text):
             if token is Text and value in self.EXTRA_KEYWORDS:
                 yield index, Name.Builtin, value
             elif token is Text and re.search(self.ADDRESS, value):
```

### Comparing `safe_cli-1.0.0/safe_cli/utils.py` & `safe_cli-1.1.0/safe_cli/utils.py`

 * *Files identical despite different names*

### Comparing `safe_cli-1.0.0/safe_cli.egg-info/SOURCES.txt` & `safe_cli-1.1.0/safe_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `safe_cli-1.0.0/setup.cfg` & `safe_cli-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `safe_cli-1.0.0/setup.py` & `safe_cli-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,29 +20,29 @@
     test_suite="tests",
     install_requires=[
         "art>=6",
         "colorama>=0.4",
         "prompt_toolkit>=3",
         "pygments>=2",
         "requests>=2",
-        "safe-eth-py==6.0.0b14",
+        "safe-eth-py==6.0.0b26",
         "tabulate>=0.8",
     ],
     extras_require={"ledger": ["ledgereth==0.9.1"], "trezor": ["trezor==0.13.8"]},
     packages=setuptools.find_packages(),
     entry_points={
         "console_scripts": [
             "safe-cli=safe_cli.main:main",
             "safe-creator=safe_cli.safe_creator:main",
         ],
     },
     classifiers=[
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires=">=3.8",
+    python_requires=">=3.9",
 )
```

### Comparing `safe_cli-1.0.0/tests/mocks/balances_mock.py` & `safe_cli-1.1.0/tests/mocks/balances_mock.py`

 * *Files identical despite different names*

### Comparing `safe_cli-1.0.0/tests/mocks/data_decoded_mock.py` & `safe_cli-1.1.0/tests/mocks/data_decoded_mock.py`

 * *Files identical despite different names*

### Comparing `safe_cli-1.0.0/tests/mocks/multisig_tx_mock.py` & `safe_cli-1.1.0/tests/mocks/multisig_tx_mock.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,19 @@
             "gasPrice": "0",
             "refundReceiver": "0x0000000000000000000000000000000000000000",
             "nonce": 6,
             "executionDate": "2023-02-28T20:18:24Z",
             "submissionDate": "2023-02-28T20:18:24Z",
             "modified": "2023-02-28T20:18:24Z",
             "blockNumber": 8573938,
-            "transactionHash": "0x7d229cdd1a197acdd23787cedcb7ec4d746ce0e730dff75e209359894af7fb52"
-            if self.executed
-            else None,
+            "transactionHash": (
+                "0x7d229cdd1a197acdd23787cedcb7ec4d746ce0e730dff75e209359894af7fb52"
+                if self.executed
+                else None
+            ),
             "safeTxHash": "0xeb5fa8e85dd530397172da07792c5d05dff9ffe5816fc0a260d672e924825b01",
             "proposer": None,
             "executor": "0x5aC255889882aCd3da2aA939679E3f3d4cea221e",
             "isExecuted": True,
             "isSuccessful": True,
             "ethGasPrice": "37052821773",
             "maxFeePerGas": "100000000000",
```

### Comparing `safe_cli-1.0.0/tests/mocks/txs_mock.py` & `safe_cli-1.1.0/tests/mocks/txs_mock.py`

 * *Files identical despite different names*

### Comparing `safe_cli-1.0.0/tests/safe_cli_test_case_mixin.py` & `safe_cli-1.1.0/tests/safe_cli_test_case_mixin.py`

 * *Files identical despite different names*

### Comparing `safe_cli-1.0.0/tests/test_argparse_validators.py` & `safe_cli-1.1.0/tests/test_argparse_validators.py`

 * *Files identical despite different names*

### Comparing `safe_cli-1.0.0/tests/test_entrypoint.py` & `safe_cli-1.1.0/tests/test_entrypoint.py`

 * *Files identical despite different names*

### Comparing `safe_cli-1.0.0/tests/test_ethereum_hd_wallet.py` & `safe_cli-1.1.0/tests/test_ethereum_hd_wallet.py`

 * *Files identical despite different names*

### Comparing `safe_cli-1.0.0/tests/test_hw_wallet_manager.py` & `safe_cli-1.1.0/tests/test_hw_wallet_manager.py`

 * *Files identical despite different names*

### Comparing `safe_cli-1.0.0/tests/test_ledger_wallet.py` & `safe_cli-1.1.0/tests/test_ledger_wallet.py`

 * *Files identical despite different names*

### Comparing `safe_cli-1.0.0/tests/test_safe_addresses.py` & `safe_cli-1.1.0/tests/test_safe_addresses.py`

 * *Files identical despite different names*

### Comparing `safe_cli-1.0.0/tests/test_safe_cli.py` & `safe_cli-1.1.0/tests/test_safe_cli.py`

 * *Files identical despite different names*

### Comparing `safe_cli-1.0.0/tests/test_safe_completer.py` & `safe_cli-1.1.0/tests/test_safe_completer.py`

 * *Files identical despite different names*

### Comparing `safe_cli-1.0.0/tests/test_safe_creator.py` & `safe_cli-1.1.0/tests/test_safe_creator.py`

 * *Files identical despite different names*

### Comparing `safe_cli-1.0.0/tests/test_safe_lexer.py` & `safe_cli-1.1.0/tests/test_safe_lexer.py`

 * *Files identical despite different names*

### Comparing `safe_cli-1.0.0/tests/test_safe_operator.py` & `safe_cli-1.1.0/tests/test_safe_operator.py`

 * *Files identical despite different names*

### Comparing `safe_cli-1.0.0/tests/test_safe_tx_service_operator.py` & `safe_cli-1.1.0/tests/test_safe_tx_service_operator.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,14 +95,46 @@
         delegate_address = Account.create().address
         signer = list(safe_operator.accounts)[0]
         self.assertTrue(safe_operator.remove_delegate(delegate_address, signer.address))
         remove_delegate_mock.assert_called_with(
             safe_operator.address, delegate_address, signer
         )
 
+    @mock.patch.object(TransactionServiceApi, "delete_transaction", return_value=None)
+    @mock.patch.object(TransactionServiceApi, "get_safe_transaction")
+    @mock.patch(
+        "gnosis.safe.api.transaction_service_api.transaction_service_messages.get_totp",
+        return_value=8365,
+    )
+    def test_remove_transaction(
+        self,
+        mock_get_totp,
+        get_transaction_mock: MagicMock,
+        remove_transaction_mock: MagicMock,
+    ):
+        safe_operator = self.setup_operator(
+            number_owners=1, mode=SafeOperatorMode.TX_SERVICE
+        )
+        safe_operator.address = "0x23793e7Ce4f2Fd31C993893f658181fD39fB5dEb"
+        signer = list(safe_operator.accounts)[0]
+        safe_tx_mock = MagicMock()
+        get_transaction_mock.return_value = (safe_tx_mock, None)
+        safe_tx_hash = HexBytes(
+            "0x07eeea19b7d005b561f367e714bf65734d0ecc477de3e8b1fbc20ccb18c8747b"
+        )
+        expected_signature = "0xbc305f59a62c5bbb002645f658ee62cfa1966f20aca4dc1922b813e9d41bf1f02abd356891a3725af2066dd1758c930574298b4ba180117dc6146bbc4369cc0c1c"
+        safe_tx_mock.proposer = signer.address
+        self.assertTrue(safe_operator.remove_proposed_transaction(safe_tx_hash))
+        remove_transaction_mock.assert_called_with(
+            safe_tx_hash.hex(), expected_signature
+        )
+        # Different proposer should return False
+        safe_tx_mock.proposer = Account.create().address
+        self.assertFalse(safe_operator.remove_proposed_transaction(safe_tx_hash))
+
     @mock.patch.object(SafeTxServiceOperator, "get_permitted_signers", return_value=[])
     @mock.patch.object(
         SafeTx, "safe_version", return_value="1.4.1", new_callable=mock.PropertyMock
     )
     @mock.patch.object(TransactionServiceApi, "post_signatures", return_value=None)
     @mock.patch.object(TransactionServiceApi, "_get_request")
     def test_submit_signatures(
@@ -135,15 +167,15 @@
         get_safe_transaction_mock.return_value = GetMultisigTxRequestMock(executed=True)
         self.assertFalse(safe_operator.submit_signatures(safe_tx_hash))
 
         # Test ledger signers
         with mock.patch.object(
             SafeTx, "signers", return_value=["signer"], new_callable=mock.PropertyMock
         ) as mock_safe_tx:
-            safe_operator.hw_wallet_manager.sign_eip712 = MagicMock(
+            safe_operator.hw_wallet_manager.sign_safe_tx = MagicMock(
                 return_value=mock_safe_tx
             )
             get_safe_transaction_mock.return_value = GetMultisigTxRequestMock(
                 executed=False
             )
             safe_operator.hw_wallet_manager.wallets.add(
                 LedgerAccount("44'/60'/0'/0", Account.create().address)
```

### Comparing `safe_cli-1.0.0/tests/test_trezor_wallet.py` & `safe_cli-1.1.0/tests/test_trezor_wallet.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
             None,
             safe_nonce=0,
         )
         encode_hash = eip712_encode(safe_tx.eip712_structured_data)
         expected_signature = safe_tx.sign(owner.key)
 
         trezor_return_signature = EthereumTypedDataSignature(
-            signature=expected_signature
+            signature=expected_signature, address=trezor_wallet.address
         )
         mock_trezor_client.return_value.call = MagicMock(
             return_value=trezor_return_signature
         )
         signature = trezor_wallet.sign_typed_hash(encode_hash[1], encode_hash[2])
         self.assertEqual(expected_signature, signature)
```

### Comparing `safe_cli-1.0.0/tests/test_utils.py` & `safe_cli-1.1.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `safe_cli-1.0.0/tests/utils.py` & `safe_cli-1.1.0/tests/utils.py`

 * *Files identical despite different names*

