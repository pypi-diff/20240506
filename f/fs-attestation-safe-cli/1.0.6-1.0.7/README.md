# Comparing `tmp/fs_attestation_safe_cli-1.0.6.tar.gz` & `tmp/fs_attestation_safe_cli-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fs_attestation_safe_cli-1.0.6.tar", last modified: Sun May  5 03:05:32 2024, max compression
+gzip compressed data, was "fs_attestation_safe_cli-1.0.7.tar", last modified: Mon May  6 08:38:39 2024, max compression
```

## Comparing `fs_attestation_safe_cli-1.0.6.tar` & `fs_attestation_safe_cli-1.0.7.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-05 03:05:32.137019 fs_attestation_safe_cli-1.0.6/
--rw-r--r--   0 mohan      (501) staff       (20)     1082 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/LICENSE
--rw-r--r--   0 mohan      (501) staff       (20)     4248 2024-05-05 03:05:32.137236 fs_attestation_safe_cli-1.0.6/PKG-INFO
--rw-r--r--   0 mohan      (501) staff       (20)     3392 2024-05-03 11:53:59.000000 fs_attestation_safe_cli-1.0.6/README.md
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-05 03:05:32.098831 fs_attestation_safe_cli-1.0.6/fs_attestation_safe_cli.egg-info/
--rw-r--r--   0 mohan      (501) staff       (20)     4248 2024-05-05 03:05:32.000000 fs_attestation_safe_cli-1.0.6/fs_attestation_safe_cli.egg-info/PKG-INFO
--rw-r--r--   0 mohan      (501) staff       (20)     1997 2024-05-05 03:05:32.000000 fs_attestation_safe_cli-1.0.6/fs_attestation_safe_cli.egg-info/SOURCES.txt
--rw-r--r--   0 mohan      (501) staff       (20)        1 2024-05-05 03:05:32.000000 fs_attestation_safe_cli-1.0.6/fs_attestation_safe_cli.egg-info/dependency_links.txt
--rw-r--r--   0 mohan      (501) staff       (20)      105 2024-05-05 03:05:32.000000 fs_attestation_safe_cli-1.0.6/fs_attestation_safe_cli.egg-info/entry_points.txt
--rw-r--r--   0 mohan      (501) staff       (20)      163 2024-05-05 03:05:32.000000 fs_attestation_safe_cli-1.0.6/fs_attestation_safe_cli.egg-info/requires.txt
--rw-r--r--   0 mohan      (501) staff       (20)       15 2024-05-05 03:05:32.000000 fs_attestation_safe_cli-1.0.6/fs_attestation_safe_cli.egg-info/top_level.txt
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-05 03:05:32.110242 fs_attestation_safe_cli-1.0.6/safe_cli/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/safe_cli/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     2085 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/safe_cli/argparse_validators.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-05 03:05:32.111500 fs_attestation_safe_cli-1.0.6/safe_cli/contracts/
--rw-r--r--   0 mohan      (501) staff       (20)       75 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/safe_cli/contracts/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)    28478 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/safe_cli/contracts/safe_to_l2_migration.py
--rw-r--r--   0 mohan      (501) staff       (20)     1262 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/safe_cli/ethereum_hd_wallet.py
--rw-r--r--   0 mohan      (501) staff       (20)     6461 2024-05-04 05:09:20.000000 fs_attestation_safe_cli-1.0.6/safe_cli/main.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-05 03:05:32.117587 fs_attestation_safe_cli-1.0.6/safe_cli/operators/
--rw-r--r--   0 mohan      (501) staff       (20)      347 2024-05-02 12:28:51.000000 fs_attestation_safe_cli-1.0.6/safe_cli/operators/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)       87 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/safe_cli/operators/enums.py
--rw-r--r--   0 mohan      (501) staff       (20)     1644 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/safe_cli/operators/exceptions.py
--rw-r--r--   0 mohan      (501) staff       (20)     2945 2024-05-02 12:26:43.000000 fs_attestation_safe_cli-1.0.6/safe_cli/operators/fs_attestation_auth.py
--rw-r--r--   0 mohan      (501) staff       (20)    13749 2024-05-05 03:04:49.000000 fs_attestation_safe_cli-1.0.6/safe_cli/operators/fs_attestation_service_operator.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-05 03:05:32.123245 fs_attestation_safe_cli-1.0.6/safe_cli/operators/hw_wallets/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/safe_cli/operators/hw_wallets/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)      113 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/safe_cli/operators/hw_wallets/constants.py
--rw-r--r--   0 mohan      (501) staff       (20)       98 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/safe_cli/operators/hw_wallets/exceptions.py
--rw-r--r--   0 mohan      (501) staff       (20)     1925 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/safe_cli/operators/hw_wallets/hw_wallet.py
--rw-r--r--   0 mohan      (501) staff       (20)     7501 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/safe_cli/operators/hw_wallets/hw_wallet_manager.py
--rw-r--r--   0 mohan      (501) staff       (20)     1081 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/safe_cli/operators/hw_wallets/ledger_exceptions.py
--rw-r--r--   0 mohan      (501) staff       (20)     2555 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/safe_cli/operators/hw_wallets/ledger_wallet.py
--rw-r--r--   0 mohan      (501) staff       (20)     1092 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/safe_cli/operators/hw_wallets/trezor_exceptions.py
--rw-r--r--   0 mohan      (501) staff       (20)     4527 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/safe_cli/operators/hw_wallets/trezor_wallet.py
--rw-r--r--   0 mohan      (501) staff       (20)    46560 2024-05-04 05:19:18.000000 fs_attestation_safe_cli-1.0.6/safe_cli/operators/safe_operator.py
--rw-r--r--   0 mohan      (501) staff       (20)    18731 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/safe_cli/operators/safe_tx_service_operator.py
--rw-r--r--   0 mohan      (501) staff       (20)    24053 2024-05-03 11:26:34.000000 fs_attestation_safe_cli-1.0.6/safe_cli/prompt_parser.py
--rw-r--r--   0 mohan      (501) staff       (20)     4030 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/safe_cli/safe_addresses.py
--rw-r--r--   0 mohan      (501) staff       (20)     1824 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/safe_cli/safe_completer.py
--rw-r--r--   0 mohan      (501) staff       (20)    10873 2024-05-03 11:30:32.000000 fs_attestation_safe_cli-1.0.6/safe_cli/safe_completer_constants.py
--rw-r--r--   0 mohan      (501) staff       (20)     7416 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/safe_cli/safe_creator.py
--rw-r--r--   0 mohan      (501) staff       (20)     1536 2024-05-03 11:27:04.000000 fs_attestation_safe_cli-1.0.6/safe_cli/safe_lexer.py
--rw-r--r--   0 mohan      (501) staff       (20)     3329 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/safe_cli/utils.py
--rw-r--r--   0 mohan      (501) staff       (20)       17 2024-05-05 03:05:21.000000 fs_attestation_safe_cli-1.0.6/safe_cli/version.py
--rw-r--r--   0 mohan      (501) staff       (20)      533 2024-05-05 03:05:32.138214 fs_attestation_safe_cli-1.0.6/setup.cfg
--rw-r--r--   0 mohan      (501) staff       (20)     1577 2024-05-04 05:16:29.000000 fs_attestation_safe_cli-1.0.6/setup.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-05 03:05:32.133493 fs_attestation_safe_cli-1.0.6/tests/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/tests/__init__.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-05 03:05:32.136305 fs_attestation_safe_cli-1.0.6/tests/mocks/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/tests/mocks/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     7755 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/tests/mocks/balances_mock.py
--rw-r--r--   0 mohan      (501) staff       (20)     2161 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/tests/mocks/data_decoded_mock.py
--rw-r--r--   0 mohan      (501) staff       (20)     2275 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/tests/mocks/multisig_tx_mock.py
--rw-r--r--   0 mohan      (501) staff       (20)     4217 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/tests/mocks/txs_mock.py
--rw-r--r--   0 mohan      (501) staff       (20)     1980 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/tests/safe_cli_test_case_mixin.py
--rw-r--r--   0 mohan      (501) staff       (20)     2335 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/tests/test_argparse_validators.py
--rw-r--r--   0 mohan      (501) staff       (20)     4030 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/tests/test_entrypoint.py
--rw-r--r--   0 mohan      (501) staff       (20)     2700 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/tests/test_ethereum_hd_wallet.py
--rw-r--r--   0 mohan      (501) staff       (20)     8216 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/tests/test_hw_wallet_manager.py
--rw-r--r--   0 mohan      (501) staff       (20)     8870 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/tests/test_ledger_wallet.py
--rw-r--r--   0 mohan      (501) staff       (20)     2309 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/tests/test_safe_addresses.py
--rw-r--r--   0 mohan      (501) staff       (20)     3051 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/tests/test_safe_cli.py
--rw-r--r--   0 mohan      (501) staff       (20)      753 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/tests/test_safe_completer.py
--rw-r--r--   0 mohan      (501) staff       (20)     1644 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/tests/test_safe_creator.py
--rw-r--r--   0 mohan      (501) staff       (20)      577 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/tests/test_safe_lexer.py
--rw-r--r--   0 mohan      (501) staff       (20)    21356 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/tests/test_safe_operator.py
--rw-r--r--   0 mohan      (501) staff       (20)    19108 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/tests/test_safe_tx_service_operator.py
--rw-r--r--   0 mohan      (501) staff       (20)     9113 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/tests/test_trezor_wallet.py
--rw-r--r--   0 mohan      (501) staff       (20)     2050 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/tests/test_utils.py
--rw-r--r--   0 mohan      (501) staff       (20)     1172 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.6/tests/utils.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-06 08:38:39.553099 fs_attestation_safe_cli-1.0.7/
+-rw-r--r--   0 mohan      (501) staff       (20)     1082 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/LICENSE
+-rw-r--r--   0 mohan      (501) staff       (20)     4248 2024-05-06 08:38:39.553667 fs_attestation_safe_cli-1.0.7/PKG-INFO
+-rw-r--r--   0 mohan      (501) staff       (20)     3392 2024-05-03 11:53:59.000000 fs_attestation_safe_cli-1.0.7/README.md
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-06 08:38:39.506248 fs_attestation_safe_cli-1.0.7/fs_attestation_safe_cli.egg-info/
+-rw-r--r--   0 mohan      (501) staff       (20)     4248 2024-05-06 08:38:39.000000 fs_attestation_safe_cli-1.0.7/fs_attestation_safe_cli.egg-info/PKG-INFO
+-rw-r--r--   0 mohan      (501) staff       (20)     1997 2024-05-06 08:38:39.000000 fs_attestation_safe_cli-1.0.7/fs_attestation_safe_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 mohan      (501) staff       (20)        1 2024-05-06 08:38:39.000000 fs_attestation_safe_cli-1.0.7/fs_attestation_safe_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 mohan      (501) staff       (20)      105 2024-05-06 08:38:39.000000 fs_attestation_safe_cli-1.0.7/fs_attestation_safe_cli.egg-info/entry_points.txt
+-rw-r--r--   0 mohan      (501) staff       (20)      163 2024-05-06 08:38:39.000000 fs_attestation_safe_cli-1.0.7/fs_attestation_safe_cli.egg-info/requires.txt
+-rw-r--r--   0 mohan      (501) staff       (20)       15 2024-05-06 08:38:39.000000 fs_attestation_safe_cli-1.0.7/fs_attestation_safe_cli.egg-info/top_level.txt
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-06 08:38:39.515403 fs_attestation_safe_cli-1.0.7/safe_cli/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2085 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/argparse_validators.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-06 08:38:39.516812 fs_attestation_safe_cli-1.0.7/safe_cli/contracts/
+-rw-r--r--   0 mohan      (501) staff       (20)       75 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/contracts/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)    28478 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/contracts/safe_to_l2_migration.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1262 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/ethereum_hd_wallet.py
+-rw-r--r--   0 mohan      (501) staff       (20)     6461 2024-05-04 05:09:20.000000 fs_attestation_safe_cli-1.0.7/safe_cli/main.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-06 08:38:39.524676 fs_attestation_safe_cli-1.0.7/safe_cli/operators/
+-rw-r--r--   0 mohan      (501) staff       (20)      347 2024-05-02 12:28:51.000000 fs_attestation_safe_cli-1.0.7/safe_cli/operators/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)       87 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/operators/enums.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1644 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/operators/exceptions.py
+-rw-r--r--   0 mohan      (501) staff       (20)     3344 2024-05-06 08:31:50.000000 fs_attestation_safe_cli-1.0.7/safe_cli/operators/fs_attestation_auth.py
+-rw-r--r--   0 mohan      (501) staff       (20)    17956 2024-05-06 08:34:53.000000 fs_attestation_safe_cli-1.0.7/safe_cli/operators/fs_attestation_service_operator.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-06 08:38:39.532834 fs_attestation_safe_cli-1.0.7/safe_cli/operators/hw_wallets/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/operators/hw_wallets/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)      113 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/operators/hw_wallets/constants.py
+-rw-r--r--   0 mohan      (501) staff       (20)       98 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/operators/hw_wallets/exceptions.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1925 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/operators/hw_wallets/hw_wallet.py
+-rw-r--r--   0 mohan      (501) staff       (20)     7501 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/operators/hw_wallets/hw_wallet_manager.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1081 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/operators/hw_wallets/ledger_exceptions.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2555 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/operators/hw_wallets/ledger_wallet.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1092 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/operators/hw_wallets/trezor_exceptions.py
+-rw-r--r--   0 mohan      (501) staff       (20)     4527 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/operators/hw_wallets/trezor_wallet.py
+-rw-r--r--   0 mohan      (501) staff       (20)    46560 2024-05-04 05:19:18.000000 fs_attestation_safe_cli-1.0.7/safe_cli/operators/safe_operator.py
+-rw-r--r--   0 mohan      (501) staff       (20)    18731 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/operators/safe_tx_service_operator.py
+-rw-r--r--   0 mohan      (501) staff       (20)    25088 2024-05-06 06:17:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/prompt_parser.py
+-rw-r--r--   0 mohan      (501) staff       (20)     4030 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/safe_addresses.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1824 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/safe_completer.py
+-rw-r--r--   0 mohan      (501) staff       (20)    11341 2024-05-06 06:18:41.000000 fs_attestation_safe_cli-1.0.7/safe_cli/safe_completer_constants.py
+-rw-r--r--   0 mohan      (501) staff       (20)     7416 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/safe_creator.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1657 2024-05-06 06:19:12.000000 fs_attestation_safe_cli-1.0.7/safe_cli/safe_lexer.py
+-rw-r--r--   0 mohan      (501) staff       (20)     3329 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/safe_cli/utils.py
+-rw-r--r--   0 mohan      (501) staff       (20)       17 2024-05-06 08:38:26.000000 fs_attestation_safe_cli-1.0.7/safe_cli/version.py
+-rw-r--r--   0 mohan      (501) staff       (20)      533 2024-05-06 08:38:39.554832 fs_attestation_safe_cli-1.0.7/setup.cfg
+-rw-r--r--   0 mohan      (501) staff       (20)     1577 2024-05-04 05:16:29.000000 fs_attestation_safe_cli-1.0.7/setup.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-06 08:38:39.548483 fs_attestation_safe_cli-1.0.7/tests/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/__init__.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-06 08:38:39.552280 fs_attestation_safe_cli-1.0.7/tests/mocks/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/mocks/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     7755 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/mocks/balances_mock.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2161 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/mocks/data_decoded_mock.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2275 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/mocks/multisig_tx_mock.py
+-rw-r--r--   0 mohan      (501) staff       (20)     4217 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/mocks/txs_mock.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1980 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/safe_cli_test_case_mixin.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2335 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/test_argparse_validators.py
+-rw-r--r--   0 mohan      (501) staff       (20)     4030 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/test_entrypoint.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2700 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/test_ethereum_hd_wallet.py
+-rw-r--r--   0 mohan      (501) staff       (20)     8216 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/test_hw_wallet_manager.py
+-rw-r--r--   0 mohan      (501) staff       (20)     8870 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/test_ledger_wallet.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2309 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/test_safe_addresses.py
+-rw-r--r--   0 mohan      (501) staff       (20)     3051 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/test_safe_cli.py
+-rw-r--r--   0 mohan      (501) staff       (20)      753 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/test_safe_completer.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1644 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/test_safe_creator.py
+-rw-r--r--   0 mohan      (501) staff       (20)      577 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/test_safe_lexer.py
+-rw-r--r--   0 mohan      (501) staff       (20)    21356 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/test_safe_operator.py
+-rw-r--r--   0 mohan      (501) staff       (20)    19108 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/test_safe_tx_service_operator.py
+-rw-r--r--   0 mohan      (501) staff       (20)     9113 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/test_trezor_wallet.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2050 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/test_utils.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1172 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.7/tests/utils.py
```

### Comparing `fs_attestation_safe_cli-1.0.6/LICENSE` & `fs_attestation_safe_cli-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/PKG-INFO` & `fs_attestation_safe_cli-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fs_attestation_safe_cli
-Version: 1.0.6
+Version: 1.0.7
 Summary: Modified Command Line Interface for FailSafe Attestation Service to administrate Gnosis Safe Wallets and FailSafe Attestation Guard Contracts
 Home-page: https://github.com/gnosis/safe-cli
 Download-URL: https://github.com/gnosis/safe-cli/releases
 Author: Mohan
 Author-email: mohan@ethlas.com
 License: MIT
 Classifier: Programming Language :: Python
```

### Comparing `fs_attestation_safe_cli-1.0.6/README.md` & `fs_attestation_safe_cli-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/fs_attestation_safe_cli.egg-info/PKG-INFO` & `fs_attestation_safe_cli-1.0.7/fs_attestation_safe_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fs-attestation-safe-cli
-Version: 1.0.6
+Version: 1.0.7
 Summary: Modified Command Line Interface for FailSafe Attestation Service to administrate Gnosis Safe Wallets and FailSafe Attestation Guard Contracts
 Home-page: https://github.com/gnosis/safe-cli
 Download-URL: https://github.com/gnosis/safe-cli/releases
 Author: Mohan
 Author-email: mohan@ethlas.com
 License: MIT
 Classifier: Programming Language :: Python
```

### Comparing `fs_attestation_safe_cli-1.0.6/fs_attestation_safe_cli.egg-info/SOURCES.txt` & `fs_attestation_safe_cli-1.0.7/fs_attestation_safe_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/safe_cli/argparse_validators.py` & `fs_attestation_safe_cli-1.0.7/safe_cli/argparse_validators.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/safe_cli/contracts/safe_to_l2_migration.py` & `fs_attestation_safe_cli-1.0.7/safe_cli/contracts/safe_to_l2_migration.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/safe_cli/ethereum_hd_wallet.py` & `fs_attestation_safe_cli-1.0.7/safe_cli/ethereum_hd_wallet.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/safe_cli/main.py` & `fs_attestation_safe_cli-1.0.7/safe_cli/main.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/safe_cli/operators/exceptions.py` & `fs_attestation_safe_cli-1.0.7/safe_cli/operators/exceptions.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/safe_cli/operators/fs_attestation_auth.py` & `fs_attestation_safe_cli-1.0.7/safe_cli/operators/fs_attestation_auth.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 import requests
 from web3 import Web3
 from web3.auto import w3
 from eth_account.messages import encode_defunct
 import json
 
 class FailSafeAttestationServiceAuth:
-    def __init__(self, fs_attestation_service_base_url: str, safe_cli_owner: str, safe_cli_owner_private_key: str):
+    def __init__(self, fs_attestation_service_base_url: str, chain_id: int, safe_address: str, safe_cli_owner: str, safe_cli_owner_private_key: str):
         self.fs_attestation_service_base_url = fs_attestation_service_base_url
+        self.chain_id = chain_id
+        self.safe_address = safe_address
         self.safe_cli_owner = safe_cli_owner
         self.safe_cli_owner_private_key = safe_cli_owner_private_key
         self.fs_api_key = "1Rm0ER9VPn8tNsQRQf7Iia9Koq7I33b728Ml7dvO"
         # TO DO - Remove below line
         self.fs_attestation_service_base_url = "https://1fw43grxlf.execute-api.us-east-1.amazonaws.com/v1"
 
     def initiate_auth(self):
         endpoint_url = "{}/auth/login".format(self.fs_attestation_service_base_url)
         headers = {
             'x-api-key': self.fs_api_key,
         }
         data = {
-            'wallet_address': self.safe_cli_owner.lower(),
+            'wallet_address': self.safe_address.lower(),
+            'wallet_owner': self.safe_cli_owner.lower(),
+            'chain_id': self.chain_id,
+            'wallet_type': "gnosis",
         }
         response = requests.post(endpoint_url, json=data, headers=headers)
         return response.json()
 
     def sign_challenge(self, challenge):
         web3_instance = Web3()
         try:
@@ -33,17 +38,20 @@
             return signature_hash
         except Exception as error:
             raise
 
     def verify_challenge(self, signature, session_token):
         endpoint_url = "{}/auth/login".format(self.fs_attestation_service_base_url)
         payload = {
-            'wallet_address': self.safe_cli_owner.lower(),
-            'challengeResponse': { 'signature': signature },
-            'sessionToken': session_token
+            'wallet_address': self.safe_address.lower(),
+            'wallet_owner': self.safe_cli_owner.lower(),
+            'challengeResponse': { 'signature': signature, 'network_id': self.chain_id },
+            'sessionToken': session_token,
+            'chain_id': self.chain_id,
+            'wallet_type': "gnosis"
         }
 
         # Configuration object with headers including the x-api-key
         headers = {
             'x-api-key': self.fs_api_key
         }
```

### Comparing `fs_attestation_safe_cli-1.0.6/safe_cli/operators/fs_attestation_service_operator.py` & `fs_attestation_safe_cli-1.0.7/safe_cli/operators/fs_attestation_service_operator.py`

 * *Files 22% similar despite different names*

```diff
@@ -148,26 +148,34 @@
             print_formatted_text(
                 response_text
             )
 
     def fs_attestation_auth_decorator(func):
         @wraps(func)
         def auth_token_expiry_time_check_wrapper(self, *args, **kwargs):
+
+            if not hasattr(self, 'last_login_time'):
+                response_text = HTML("<ansired>No active session exists. Please log into FS Attestation Service by executing the command <b><ansigreen>fs_attestation_service_auth</ansigreen></b> and then try this command</ansired>")
+                print_formatted_text(
+                    response_text
+                )
+                return
+
             current_time = int(time.time())
             # The Auth token issued by the FailSafe Attestation Service is valid for 10 minutes
             # If the token is nearing expiry time (more than 9 minutes), let's re-authenticate with the FailSafe Attestation Service
             if current_time - self.last_login_time > 540:
                 self.fs_attestation_user_login_internal()
             return func(self, *args, **kwargs)
 
         return auth_token_expiry_time_check_wrapper
 
     def fs_attestation_user_login(self, safe_cli_owner: str, safe_cli_owner_private_key: str) -> str:
         try:
-            self.fs_attestation_service_auth = FailSafeAttestationServiceAuth(self.fs_attestation_service_base_url, safe_cli_owner, safe_cli_owner_private_key)
+            self.fs_attestation_service_auth = FailSafeAttestationServiceAuth(self.fs_attestation_service_base_url, self.network.value, self.address, safe_cli_owner, safe_cli_owner_private_key)
             self.fs_attestation_user_login_internal()
         except Exception:
             response_text = HTML("<ansired>Some error occurred when performing FailSafe Attestation Service Authentication flow</ansired>")
             print_formatted_text(
                 response_text
             )
 
@@ -179,15 +187,16 @@
             data = {'multisig_wallet_address': self.address, 'multisig_wallet_provider': 'gnosis_safe', 'chain_id': self.network.value}
             # Make the POST request
             response = requests.post(enrolment_url, json=data, headers=headers)
 
             # Check if the request was successful (status code 200)
             if response.status_code == 200:
                 # Print the response content
-                response_text = HTML("<ansigreen>{response_text}</ansigreen>").format(response_text=response.text)
+                response_json = json.loads(response.text)
+                response_text = HTML("<ansigreen>{response_text}</ansigreen>").format(response_text=json.dumps(response_json, indent=4))
                 print_formatted_text(
                     response_text
                 )
                 return response.text
             else:
                 # Print an error message if the request was not successful
                 response_text = HTML("<ansired>Status code {response_code}: {response_text}</ansired>").format(response_code=response.status_code, response_text=response.text)
@@ -209,15 +218,16 @@
             data = {'multisig_wallet_address': self.address, 'chain_id': self.network.value}
             # Make the POST request
             response = requests.post(deploy_guard_contract_url, json=data, headers=headers)
 
             # Check if the request was successful (status code 200)
             if response.status_code == 200:
                 # Print the response content
-                response_text = HTML("<ansigreen>{response_text}</ansigreen>").format(response_text=response.text)
+                response_json = json.loads(response.text)
+                response_text = HTML("<ansigreen>{response_text}</ansigreen>").format(response_text=json.dumps(response_json, indent=4))
                 print_formatted_text(
                     response_text
                 )
                 return response.text
             else:
                 # Print an error message if the request was not successful
                 response_text = HTML("<ansired>Status code {response_code}: {response_text}</ansired>").format(response_code=response.status_code, response_text=response.text)
@@ -244,15 +254,16 @@
 
             # Make the POST request
             response = requests.post(set_constraints_url, json=data, headers=headers)
 
             # Check if the request was successful (status code 200)
             if response.status_code == 200:
                 # Print the response content
-                response_text = HTML("<ansigreen>{response_text}</ansigreen>").format(response_text=response.text)
+                response_json = json.loads(response.text)
+                response_text = HTML("<ansigreen>{response_text}</ansigreen>").format(response_text=json.dumps(response_json, indent=4))
                 print_formatted_text(
                     response_text
                 )
                 return response.text
             else:
                 # Print an error message if the request was not successful
                 response_text = HTML("<ansired>Status code {response_code}: {response_text}</ansired>").format(response_code=response.status_code, response_text=response.text)
@@ -275,15 +286,16 @@
 
             # Make the POST request
             response = requests.post(set_constraints_url, json=data, headers=headers)
 
             # Check if the request was successful (status code 200)
             if response.status_code == 200:
                 # Print the response content
-                response_text = HTML("<ansigreen>{response_text}</ansigreen>").format(response_text=response.text)
+                response_json = json.loads(response.text)
+                response_text = HTML("<ansigreen>{response_text}</ansigreen>").format(response_text=json.dumps(response_json, indent=4))
                 print_formatted_text(
                     response_text
                 )
                 return response.text
             else:
                 # Print an error message if the request was not successful
                 response_text = HTML("<ansired>Status code {response_code}: {response_text}</ansired>").format(response_code=response.status_code, response_text=response.text)
@@ -292,7 +304,71 @@
                 )
                 return ""
         except Exception as error:
             response_text = HTML("<ansired>Some error occurred when updating the FailSafe Attestation Service settings for the Safe Multi-Sig Wallet</ansired>")
             print_formatted_text(
                 response_text
             )
+
+    @fs_attestation_auth_decorator
+    def fs_attestation_get_attestation_authority_wallet_address(self) -> str:
+        try:
+            get_attestation_wallet_address_url = "{}/{}".format(self.fs_attestation_service_base_url, "attestation-service/get-attestation-key")
+            headers = {'Authorization': 'Bearer {}'.format(self.access_token)}
+            params = {'multisig_wallet_address': self.address, 'chain_id': self.network.value}
+            # Make the GET request
+            response = requests.get(get_attestation_wallet_address_url, params=params, headers=headers)
+
+            # Check if the request was successful (status code 200)
+            if response.status_code == 200:
+                # Print the response content
+                response_json = json.loads(response.text)
+                response_text = HTML("<ansigreen>{response_text}</ansigreen>").format(response_text=json.dumps(response_json, indent=4))
+                print_formatted_text(
+                    response_text
+                )
+                return response.text
+            else:
+                # Print an error message if the request was not successful
+                response_text = HTML("<ansired>Status code {response_code}: {response_text}</ansired>").format(response_code=response.status_code, response_text=response.text)
+                print_formatted_text(
+                    response_text
+                )
+                return ""
+        except Exception as error:
+            print(error)
+            response_text = HTML("<ansired>Some error occurred when retrieving FailSafe Attestation Authority Wallet address</ansired>")
+            print_formatted_text(
+                response_text
+            )
+
+    @fs_attestation_auth_decorator
+    def fs_attestation_get_attestation_constraints(self) -> str:
+        try:
+            get_attestation_service_enrolment_url = "{}/{}".format(self.fs_attestation_service_base_url, "attestation-service/get-enrolment")
+            headers = {'Authorization': 'Bearer {}'.format(self.access_token)}
+            params = {'multisig_wallet_address': self.address, 'chain_id': self.network.value}
+            # Make the GET request
+            response = requests.get(get_attestation_service_enrolment_url, params=params, headers=headers)
+
+            # Check if the request was successful (status code 200)
+            if response.status_code == 200:
+                # Print the response content
+                response_json = json.loads(response.text)
+                response_text = HTML("<ansigreen>{response_text}</ansigreen>").format(response_text=json.dumps(response_json['enrolment']['constraints'], indent=4))
+                print_formatted_text(
+                    response_text
+                )
+                return response.text
+            else:
+                # Print an error message if the request was not successful
+                response_text = HTML("<ansired>Status code {response_code}: {response_text}</ansired>").format(response_code=response.status_code, response_text=response.text)
+                print_formatted_text(
+                    response_text
+                )
+                return ""
+        except Exception as error:
+            print(error)
+            response_text = HTML("<ansired>Some error occurred when retrieving FailSafe Attestation Constraints</ansired>")
+            print_formatted_text(
+                response_text
+            )
```

### Comparing `fs_attestation_safe_cli-1.0.6/safe_cli/operators/hw_wallets/hw_wallet.py` & `fs_attestation_safe_cli-1.0.7/safe_cli/operators/hw_wallets/hw_wallet.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/safe_cli/operators/hw_wallets/hw_wallet_manager.py` & `fs_attestation_safe_cli-1.0.7/safe_cli/operators/hw_wallets/hw_wallet_manager.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/safe_cli/operators/hw_wallets/ledger_exceptions.py` & `fs_attestation_safe_cli-1.0.7/safe_cli/operators/hw_wallets/ledger_exceptions.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/safe_cli/operators/hw_wallets/ledger_wallet.py` & `fs_attestation_safe_cli-1.0.7/safe_cli/operators/hw_wallets/ledger_wallet.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/safe_cli/operators/hw_wallets/trezor_exceptions.py` & `fs_attestation_safe_cli-1.0.7/safe_cli/operators/hw_wallets/trezor_exceptions.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/safe_cli/operators/hw_wallets/trezor_wallet.py` & `fs_attestation_safe_cli-1.0.7/safe_cli/operators/hw_wallets/trezor_wallet.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/safe_cli/operators/safe_operator.py` & `fs_attestation_safe_cli-1.0.7/safe_cli/operators/safe_operator.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/safe_cli/operators/safe_tx_service_operator.py` & `fs_attestation_safe_cli-1.0.7/safe_cli/operators/safe_tx_service_operator.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/safe_cli/prompt_parser.py` & `fs_attestation_safe_cli-1.0.7/safe_cli/prompt_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -354,14 +354,22 @@
     def fs_attestation_service_set_constraints(args):
         fs_attestation_service_operator.fs_attestation_service_set_constraints(args.signer_ip_address_constraints, args.expiry_time_constrint, args.risk_score_threshold_constraint)
 
     @safe_exception
     def fs_attestation_settings(args):
         fs_attestation_service_operator.fs_attestation_settings(args.contact_email_address, args.slack_url)
 
+    @safe_exception
+    def fs_attestation_get_attestation_authority_wallet_address(args):
+        fs_attestation_service_operator.fs_attestation_get_attestation_authority_wallet_address()
+
+    @safe_exception
+    def fs_attestation_get_attestation_constraints(args):
+        fs_attestation_service_operator.fs_attestation_get_attestation_constraints()
+
     # Cli owners
     parser_show_cli_owners = subparsers.add_parser("show_cli_owners")
     parser_show_cli_owners.set_defaults(func=show_cli_owners)
 
     parser_load_cli_owners_from_words = subparsers.add_parser(
         "load_cli_owners_from_words"
     )
@@ -628,8 +636,20 @@
     parser_fs_attestation_settings.add_argument(
         "contact_email_address", type=str
     )
     parser_fs_attestation_settings.add_argument(
         "slack_url", type=str
     )
 
+    # Get FailSafe Attestation Authority Wallet Address
+    parser_fs_attestation_get_attestation_authority_wallet_address = subparsers.add_parser(
+        "fs_attestation_get_attestation_authority_wallet_address"
+    )
+    parser_fs_attestation_get_attestation_authority_wallet_address.set_defaults(func=fs_attestation_get_attestation_authority_wallet_address)
+
+    # Get FailSafe Attestation Service Attestation Constraints
+    parser_fs_attestation_get_attestation_constraints = subparsers.add_parser(
+        "fs_attestation_get_attestation_constraints"
+    )
+    parser_fs_attestation_get_attestation_constraints.set_defaults(func=fs_attestation_get_attestation_constraints)
+
     return prompt_parser
```

### Comparing `fs_attestation_safe_cli-1.0.6/safe_cli/safe_addresses.py` & `fs_attestation_safe_cli-1.0.7/safe_cli/safe_addresses.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/safe_cli/safe_completer.py` & `fs_attestation_safe_cli-1.0.7/safe_cli/safe_completer.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/safe_cli/safe_completer_constants.py` & `fs_attestation_safe_cli-1.0.7/safe_cli/safe_completer_constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,15 +44,17 @@
     "blockchain": "",
     "tx-service": "",
     "drain": "<address>",
     "fs_attestation_service_enrolment": "",
     "fs_attestation_service_auth": "<safe_cli_owner> <safe_cli_owner_private_key>",
     "fs_attestation_service_deploy_guard_contract": "",
     "fs_attestation_service_set_constraints": "<signer_wallet_address:ip_address_range> [<signer_wallet_address:ip_address_range>...] <multi_sig_tx_expiry_duration> <risk_score_threshold>",
-    "fs_attestation_settings": "<contact_email> <slack_web_hook_url>"
+    "fs_attestation_settings": "<contact_email> <slack_web_hook_url>",
+    "fs_attestation_get_attestation_authority_wallet_address": "",
+    "fs_attestation_get_attestation_constraints": "",
 }
 
 safe_commands = list(safe_commands_arguments.keys())
 
 safe_color_arguments = {
     "(read-only)": SAFE_ARGUMENT_COLOR,
     "<account-private-key>": SAFE_ARGUMENT_COLOR,
@@ -231,8 +233,14 @@
     ),
     "fs_attestation_service_set_constraints": HTML(
         "Will set the ip address range, multi-sig transaction expiry duration and risk score threshold constraints for the current safe wallet address"
     ),
     "fs_attestation_settings": HTML(
         "Will update the additional settings FailSafe Attestation Service settings (contact emails and slack integrations, etc) for the current safe wallet address"
     ),
+    "fs_attestation_get_attestation_authority_wallet_address": HTML(
+        "Will retrieve the FailSafe Attestation Authority Wallet Address for the current safe wallet address"
+    ),
+    "fs_attestation_get_attestation_constraints": HTML(
+        "Will retrieve the FailSafe Attestation Constraints for the current safe wallet address"
+    ),
 }
```

### Comparing `fs_attestation_safe_cli-1.0.6/safe_cli/safe_creator.py` & `fs_attestation_safe_cli-1.0.7/safe_cli/safe_creator.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/safe_cli/safe_lexer.py` & `fs_attestation_safe_cli-1.0.7/safe_cli/safe_lexer.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,17 @@
         "send_erc20",
         "send_erc721",
         "remove_proposed_transaction",
         "fs_attestation_service_auth",
         "fs_attestation_service_enrolment",
         "fs_attestation_service_deploy_guard_contract",
         "fs_attestation_service_set_constraints",
-        "fs_attestation_settings"
+        "fs_attestation_settings",
+        "fs_attestation_get_attestation_authority_wallet_address",
+        "fs_attestation_get_attestation_constraints"
     }
 
     def get_tokens_unprocessed(self, text: str) -> (int, Token, str):
         for index, token, value in BashLexer.get_tokens_unprocessed(self, text):
             if token is Text and value in self.EXTRA_KEYWORDS:
                 yield index, Name.Builtin, value
             elif token is Text and re.search(self.ADDRESS, value):
```

### Comparing `fs_attestation_safe_cli-1.0.6/safe_cli/utils.py` & `fs_attestation_safe_cli-1.0.7/safe_cli/utils.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/setup.cfg` & `fs_attestation_safe_cli-1.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/setup.py` & `fs_attestation_safe_cli-1.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/tests/mocks/balances_mock.py` & `fs_attestation_safe_cli-1.0.7/tests/mocks/balances_mock.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/tests/mocks/data_decoded_mock.py` & `fs_attestation_safe_cli-1.0.7/tests/mocks/data_decoded_mock.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/tests/mocks/multisig_tx_mock.py` & `fs_attestation_safe_cli-1.0.7/tests/mocks/multisig_tx_mock.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/tests/mocks/txs_mock.py` & `fs_attestation_safe_cli-1.0.7/tests/mocks/txs_mock.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/tests/safe_cli_test_case_mixin.py` & `fs_attestation_safe_cli-1.0.7/tests/safe_cli_test_case_mixin.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/tests/test_argparse_validators.py` & `fs_attestation_safe_cli-1.0.7/tests/test_argparse_validators.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/tests/test_entrypoint.py` & `fs_attestation_safe_cli-1.0.7/tests/test_entrypoint.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/tests/test_ethereum_hd_wallet.py` & `fs_attestation_safe_cli-1.0.7/tests/test_ethereum_hd_wallet.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/tests/test_hw_wallet_manager.py` & `fs_attestation_safe_cli-1.0.7/tests/test_hw_wallet_manager.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/tests/test_ledger_wallet.py` & `fs_attestation_safe_cli-1.0.7/tests/test_ledger_wallet.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/tests/test_safe_addresses.py` & `fs_attestation_safe_cli-1.0.7/tests/test_safe_addresses.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/tests/test_safe_cli.py` & `fs_attestation_safe_cli-1.0.7/tests/test_safe_cli.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/tests/test_safe_completer.py` & `fs_attestation_safe_cli-1.0.7/tests/test_safe_completer.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/tests/test_safe_creator.py` & `fs_attestation_safe_cli-1.0.7/tests/test_safe_creator.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/tests/test_safe_lexer.py` & `fs_attestation_safe_cli-1.0.7/tests/test_safe_lexer.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/tests/test_safe_operator.py` & `fs_attestation_safe_cli-1.0.7/tests/test_safe_operator.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/tests/test_safe_tx_service_operator.py` & `fs_attestation_safe_cli-1.0.7/tests/test_safe_tx_service_operator.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/tests/test_trezor_wallet.py` & `fs_attestation_safe_cli-1.0.7/tests/test_trezor_wallet.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/tests/test_utils.py` & `fs_attestation_safe_cli-1.0.7/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.6/tests/utils.py` & `fs_attestation_safe_cli-1.0.7/tests/utils.py`

 * *Files identical despite different names*

