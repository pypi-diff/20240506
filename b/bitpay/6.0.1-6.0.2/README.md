# Comparing `tmp/bitpay-6.0.1.tar.gz` & `tmp/bitpay-6.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitpay-6.0.1.tar", last modified: Mon Mar 11 15:29:34 2024, max compression
+gzip compressed data, was "bitpay-6.0.2.tar", last modified: Mon May  6 16:53:20 2024, max compression
```

## Comparing `bitpay-6.0.1.tar` & `bitpay-6.0.2.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:29:34.482579 bitpay-6.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-03-11 15:29:30.000000 bitpay-6.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-03-11 15:29:34.482579 bitpay-6.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-03-11 15:29:30.000000 bitpay-6.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-03-11 15:29:30.000000 bitpay-6.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 15:29:34.482579 bitpay-6.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:29:34.462579 bitpay-6.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:29:34.466579 bitpay-6.0.1/src/bitpay/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/bitpay_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    36869 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:29:34.470579 bitpay-6.0.1/src/bitpay/clients/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/clients/bill_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/clients/bitpay_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/clients/currency_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12655 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/clients/invoice_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/clients/ledger_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7625 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/clients/payout_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/clients/payout_recipient_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/clients/rate_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9970 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/clients/refund_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/clients/response_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4531 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/clients/settlement_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/clients/wallet_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/config.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:29:34.470579 bitpay-6.0.1/src/bitpay/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/exceptions/bitpay_api_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/exceptions/bitpay_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/exceptions/bitpay_exception_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/exceptions/bitpay_generic_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/exceptions/bitpay_validation_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:29:34.470579 bitpay-6.0.1/src/bitpay/logger/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/logger/bitpay_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/logger/logger_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/logger/logging_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:29:34.470579 bitpay-6.0.1/src/bitpay/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:29:34.474579 bitpay-6.0.1/src/bitpay/models/bill/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/bill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/bill/bill.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/bill/bill_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/bill/item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/bitpay_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/currency.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:29:34.474579 bitpay-6.0.1/src/bitpay/models/invoice/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/invoice/buyer.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/invoice/buyer_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/invoice/buyer_provided_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/invoice/invoice.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/invoice/invoice_event_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/invoice/invoice_refund_addresses.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/invoice/invoice_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/invoice/invoice_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/invoice/itemized_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/invoice/miner_fees.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/invoice/miner_fees_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/invoice/refund.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/invoice/refund_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/invoice/refund_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/invoice/refund_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/invoice/shopper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/invoice/supported_transaction_currencies.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/invoice/supported_transaction_currency.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/invoice/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/invoice/universal_codes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:29:34.478579 bitpay-6.0.1/src/bitpay/models/ledger/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/ledger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/ledger/buyer.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/ledger/ledger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/ledger/ledger_entry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:29:34.478579 bitpay-6.0.1/src/bitpay/models/payout/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/payout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/payout/payout.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/payout/payout_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/payout/payout_group_failed.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/payout/payout_recipient.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/payout/payout_recipients.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/payout/payout_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/payout/payout_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/payout/payout_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/payout/recipient_status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:29:34.478579 bitpay-6.0.1/src/bitpay/models/rate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/rate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/rate/rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/rate/rates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:29:34.478579 bitpay-6.0.1/src/bitpay/models/settlement/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/settlement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/settlement/invoice_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/settlement/payout_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/settlement/refund_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/settlement/settlement.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/settlement/settlement_ledger_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/settlement/with_holdings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:29:34.482579 bitpay-6.0.1/src/bitpay/models/wallet/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/wallet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/wallet/currencies.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/wallet/currency_qr.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/models/wallet/wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:29:34.482579 bitpay-6.0.1/src/bitpay/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/utils/guid_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/utils/key_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/utils/model_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-03-11 15:29:30.000000 bitpay-6.0.1/src/bitpay/utils/token_container.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:29:34.482579 bitpay-6.0.1/src/bitpay.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-03-11 15:29:34.000000 bitpay-6.0.1/src/bitpay.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-03-11 15:29:34.000000 bitpay-6.0.1/src/bitpay.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 15:29:34.000000 bitpay-6.0.1/src/bitpay.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-11 15:29:34.000000 bitpay-6.0.1/src/bitpay.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-11 15:29:34.000000 bitpay-6.0.1/src/bitpay.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:20.027037 bitpay-6.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-06 16:53:16.000000 bitpay-6.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-06 16:53:20.027037 bitpay-6.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-06 16:53:16.000000 bitpay-6.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-06 16:53:16.000000 bitpay-6.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 16:53:20.027037 bitpay-6.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:20.007037 bitpay-6.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:20.011037 bitpay-6.0.2/src/bitpay/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/bitpay_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36869 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:20.015037 bitpay-6.0.2/src/bitpay/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/clients/bill_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/clients/bitpay_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/clients/currency_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12655 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/clients/invoice_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/clients/ledger_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7625 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/clients/payout_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/clients/payout_recipient_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/clients/rate_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9970 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/clients/refund_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/clients/response_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4531 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/clients/settlement_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/clients/wallet_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:20.015037 bitpay-6.0.2/src/bitpay/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/exceptions/bitpay_api_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/exceptions/bitpay_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/exceptions/bitpay_exception_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/exceptions/bitpay_generic_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/exceptions/bitpay_validation_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:20.015037 bitpay-6.0.2/src/bitpay/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/logger/bitpay_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/logger/logger_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/logger/logging_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:20.015037 bitpay-6.0.2/src/bitpay/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:20.015037 bitpay-6.0.2/src/bitpay/models/bill/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/bill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/bill/bill.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/bill/bill_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/bill/item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/bitpay_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/currency.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:20.019037 bitpay-6.0.2/src/bitpay/models/invoice/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/buyer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/buyer_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/buyer_provided_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/invoice_event_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/invoice_refund_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/invoice_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/invoice_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/itemized_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/miner_fees.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/miner_fees_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/refund.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/refund_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/refund_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/refund_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/shopper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/supported_transaction_currencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/supported_transaction_currency.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/universal_codes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:20.019037 bitpay-6.0.2/src/bitpay/models/ledger/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/ledger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/ledger/buyer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/ledger/ledger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/ledger/ledger_entry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:20.023037 bitpay-6.0.2/src/bitpay/models/payout/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/payout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/payout/payout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/payout/payout_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/payout/payout_group_failed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/payout/payout_recipient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/payout/payout_recipients.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/payout/payout_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/payout/payout_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/payout/payout_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/payout/recipient_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:20.023037 bitpay-6.0.2/src/bitpay/models/rate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/rate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/rate/rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/rate/rates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:20.023037 bitpay-6.0.2/src/bitpay/models/settlement/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/settlement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/settlement/invoice_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/settlement/payout_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/settlement/refund_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/settlement/settlement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/settlement/settlement_ledger_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/settlement/with_holdings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:20.023037 bitpay-6.0.2/src/bitpay/models/wallet/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/wallet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/wallet/currencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/wallet/currency_qr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/wallet/wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:20.027037 bitpay-6.0.2/src/bitpay/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/utils/guid_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/utils/key_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/utils/model_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/utils/token_container.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:20.027037 bitpay-6.0.2/src/bitpay.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-06 16:53:19.000000 bitpay-6.0.2/src/bitpay.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-05-06 16:53:20.000000 bitpay-6.0.2/src/bitpay.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:53:19.000000 bitpay-6.0.2/src/bitpay.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-06 16:53:19.000000 bitpay-6.0.2/src/bitpay.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-06 16:53:19.000000 bitpay-6.0.2/src/bitpay.egg-info/top_level.txt
```

### Comparing `bitpay-6.0.1/LICENSE` & `bitpay-6.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/PKG-INFO` & `bitpay-6.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitpay
-Version: 6.0.1
+Version: 6.0.2
 Summary: Accept bitcoin with BitPay
 Author-email: Antonio Buedo <sales-engineering@bitpay.com>
 Project-URL: Homepage, https://github.com/bitpay/python-bitpay-client
 Project-URL: Bug Tracker, https://github.com/bitpay/python-bitpay-client/issues
 Keywords: bitcoin,payments,crypto,cash,ethereum,online payments
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `bitpay-6.0.1/README.md` & `bitpay-6.0.2/README.md`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/pyproject.toml` & `bitpay-6.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bitpay"
-version = "6.0.1"
+version = "6.0.2"
 authors = [
   { name="Antonio Buedo", email="sales-engineering@bitpay.com" },
 ]
 requires-python = ">=3.8"
 dependencies = [
     "ecdsa >= 0.18.0",
     "requests >= 2.31.0",
```

### Comparing `bitpay-6.0.1/src/bitpay/bitpay_setup.py` & `bitpay-6.0.2/src/bitpay/bitpay_setup.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/client.py` & `bitpay-6.0.2/src/bitpay/client.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/clients/bill_client.py` & `bitpay-6.0.2/src/bitpay/clients/bill_client.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/clients/bitpay_client.py` & `bitpay-6.0.2/src/bitpay/clients/bitpay_client.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/clients/currency_client.py` & `bitpay-6.0.2/src/bitpay/clients/currency_client.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/clients/invoice_client.py` & `bitpay-6.0.2/src/bitpay/clients/invoice_client.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/clients/ledger_client.py` & `bitpay-6.0.2/src/bitpay/clients/ledger_client.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/clients/payout_client.py` & `bitpay-6.0.2/src/bitpay/clients/payout_client.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/clients/payout_recipient_client.py` & `bitpay-6.0.2/src/bitpay/clients/payout_recipient_client.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/clients/rate_client.py` & `bitpay-6.0.2/src/bitpay/clients/rate_client.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/clients/refund_client.py` & `bitpay-6.0.2/src/bitpay/clients/refund_client.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/clients/response_parser.py` & `bitpay-6.0.2/src/bitpay/clients/response_parser.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/clients/settlement_client.py` & `bitpay-6.0.2/src/bitpay/clients/settlement_client.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/clients/wallet_client.py` & `bitpay-6.0.2/src/bitpay/clients/wallet_client.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/exceptions/bitpay_api_exception.py` & `bitpay-6.0.2/src/bitpay/exceptions/bitpay_api_exception.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/exceptions/bitpay_exception_provider.py` & `bitpay-6.0.2/src/bitpay/exceptions/bitpay_exception_provider.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/logger/logger_provider.py` & `bitpay-6.0.2/src/bitpay/logger/logger_provider.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/logger/logging_logger.py` & `bitpay-6.0.2/src/bitpay/logger/logging_logger.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/models/bill/bill.py` & `bitpay-6.0.2/src/bitpay/models/bill/bill.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/models/bitpay_model.py` & `bitpay-6.0.2/src/bitpay/models/bitpay_model.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/models/currency.py` & `bitpay-6.0.2/src/bitpay/models/currency.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/models/invoice/buyer.py` & `bitpay-6.0.2/src/bitpay/models/invoice/buyer.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/models/invoice/buyer_fields.py` & `bitpay-6.0.2/src/bitpay/models/invoice/buyer_fields.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/models/invoice/buyer_provided_info.py` & `bitpay-6.0.2/src/bitpay/models/invoice/buyer_provided_info.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/models/invoice/invoice.py` & `bitpay-6.0.2/src/bitpay/models/invoice/invoice.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/models/invoice/invoice_webhook.py` & `bitpay-6.0.2/src/bitpay/models/invoice/invoice_webhook.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/models/invoice/miner_fees.py` & `bitpay-6.0.2/src/bitpay/models/invoice/miner_fees.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/models/invoice/miner_fees_item.py` & `bitpay-6.0.2/src/bitpay/models/invoice/miner_fees_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,10 +11,10 @@
     """
     The total amount of fees that the purchaser will pay to cover BitPay's
      UTXO sweep cost for an invoice. The key is the currency and the value is
       an amount in satoshis. This is referenced as "Network Cost" on an invoice,
     see this support article for more information
     """
 
-    satoshis_per_byte: Union[int, None] = None
+    satoshis_per_byte: Union[float, None] = None
     total_fee: Union[int, None] = None
     fiat_amount: Union[float, None] = None
```

### Comparing `bitpay-6.0.1/src/bitpay/models/invoice/refund.py` & `bitpay-6.0.2/src/bitpay/models/invoice/refund.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/models/invoice/refund_webhook.py` & `bitpay-6.0.2/src/bitpay/models/invoice/refund_webhook.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/models/invoice/supported_transaction_currencies.py` & `bitpay-6.0.2/src/bitpay/models/invoice/supported_transaction_currencies.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/models/invoice/transaction.py` & `bitpay-6.0.2/src/bitpay/models/invoice/transaction.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/models/ledger/buyer.py` & `bitpay-6.0.2/src/bitpay/models/ledger/buyer.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/models/ledger/ledger_entry.py` & `bitpay-6.0.2/src/bitpay/models/ledger/ledger_entry.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/models/payout/payout.py` & `bitpay-6.0.2/src/bitpay/models/payout/payout.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/models/payout/payout_recipient.py` & `bitpay-6.0.2/src/bitpay/models/payout/payout_recipient.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/models/payout/payout_transaction.py` & `bitpay-6.0.2/src/bitpay/models/payout/payout_transaction.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/models/payout/payout_webhook.py` & `bitpay-6.0.2/src/bitpay/models/payout/payout_webhook.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/models/rate/rates.py` & `bitpay-6.0.2/src/bitpay/models/rate/rates.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/models/settlement/invoice_data.py` & `bitpay-6.0.2/src/bitpay/models/settlement/invoice_data.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/models/settlement/payout_info.py` & `bitpay-6.0.2/src/bitpay/models/settlement/payout_info.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/models/settlement/settlement.py` & `bitpay-6.0.2/src/bitpay/models/settlement/settlement.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/models/settlement/settlement_ledger_entry.py` & `bitpay-6.0.2/src/bitpay/models/settlement/settlement_ledger_entry.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/models/wallet/currencies.py` & `bitpay-6.0.2/src/bitpay/models/wallet/currencies.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/models/wallet/wallet.py` & `bitpay-6.0.2/src/bitpay/models/wallet/wallet.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/utils/key_utils.py` & `bitpay-6.0.2/src/bitpay/utils/key_utils.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/utils/model_util.py` & `bitpay-6.0.2/src/bitpay/utils/model_util.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay/utils/token_container.py` & `bitpay-6.0.2/src/bitpay/utils/token_container.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.1/src/bitpay.egg-info/PKG-INFO` & `bitpay-6.0.2/src/bitpay.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitpay
-Version: 6.0.1
+Version: 6.0.2
 Summary: Accept bitcoin with BitPay
 Author-email: Antonio Buedo <sales-engineering@bitpay.com>
 Project-URL: Homepage, https://github.com/bitpay/python-bitpay-client
 Project-URL: Bug Tracker, https://github.com/bitpay/python-bitpay-client/issues
 Keywords: bitcoin,payments,crypto,cash,ethereum,online payments
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `bitpay-6.0.1/src/bitpay.egg-info/SOURCES.txt` & `bitpay-6.0.2/src/bitpay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

