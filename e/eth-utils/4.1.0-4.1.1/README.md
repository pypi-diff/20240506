# Comparing `tmp/eth-utils-4.1.0.tar.gz` & `tmp/eth_utils-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth-utils-4.1.0.tar", last modified: Mon Apr  1 19:54:24 2024, max compression
+gzip compressed data, was "eth_utils-4.1.1.tar", last modified: Mon May  6 18:21:45 2024, max compression
```

## Comparing `eth-utils-4.1.0.tar` & `eth_utils-4.1.1.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.939384 eth-utils-4.1.0/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1095 2023-05-01 17:17:17.000000 eth-utils-4.1.0/LICENSE
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      211 2024-01-09 21:45:03.000000 eth-utils-4.1.0/MANIFEST.in
--rw-r--r--   0 pacrob    (1000) pacrob    (1000)     5193 2024-04-01 19:54:24.939384 eth-utils-4.1.0/PKG-INFO
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3086 2024-01-09 21:45:03.000000 eth-utils-4.1.0/README.md
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.931384 eth-utils-4.1.0/eth_utils/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2343 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/__init__.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.931384 eth-utils-4.1.0/eth_utils/__json/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)   304350 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/__json/eth_networks.json
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       86 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/__main__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2050 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/abi.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4218 2024-03-25 20:53:18.000000 eth-utils-4.1.0/eth_utils/address.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4342 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/applicators.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5500 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/conversions.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      362 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/crypto.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3021 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/currency.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.931384 eth-utils-4.1.0/eth_utils/curried/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     6497 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/curried/__init__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      499 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/debug.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3995 2024-03-25 20:53:18.000000 eth-utils-4.1.0/eth_utils/decorators.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      199 2023-04-20 19:46:27.000000 eth-utils-4.1.0/eth_utils/encoding.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      110 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/exceptions.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2100 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/functional.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1828 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/hexadecimal.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4148 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/humanize.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5155 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/logging.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      842 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/module_loading.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2244 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/network.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1190 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/numeric.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-04-20 19:46:27.000000 eth-utils-4.1.0/eth_utils/py.typed
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2617 2023-04-20 19:46:27.000000 eth-utils-4.1.0/eth_utils/toolz.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1074 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/types.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.931384 eth-utils-4.1.0/eth_utils/typing/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      325 2023-10-02 20:24:48.000000 eth-utils-4.1.0/eth_utils/typing/__init__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      190 2024-01-09 21:45:03.000000 eth-utils-4.1.0/eth_utils/typing/misc.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1757 2023-04-20 19:46:27.000000 eth-utils-4.1.0/eth_utils/units.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.935384 eth-utils-4.1.0/eth_utils.egg-info/
--rw-r--r--   0 pacrob    (1000) pacrob    (1000)     5193 2024-04-01 19:54:24.000000 eth-utils-4.1.0/eth_utils.egg-info/PKG-INFO
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2619 2024-04-01 19:54:24.000000 eth-utils-4.1.0/eth_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2024-04-01 19:54:24.000000 eth-utils-4.1.0/eth_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2023-04-20 19:46:27.000000 eth-utils-4.1.0/eth_utils.egg-info/not-zip-safe
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      502 2024-04-01 19:54:24.000000 eth-utils-4.1.0/eth_utils.egg-info/requires.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       10 2024-04-01 19:54:24.000000 eth-utils-4.1.0/eth_utils.egg-info/top_level.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3419 2024-03-25 20:53:18.000000 eth-utils-4.1.0/pyproject.toml
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       38 2024-04-01 19:54:24.939384 eth-utils-4.1.0/setup.cfg
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2174 2024-04-01 19:54:03.000000 eth-utils-4.1.0/setup.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.927384 eth-utils-4.1.0/tests/
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.931384 eth-utils-4.1.0/tests/core/
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.931384 eth-utils-4.1.0/tests/core/abi-utils/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5031 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/abi-utils/test_abi_utils.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.931384 eth-utils-4.1.0/tests/core/address-utils/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    10843 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/address-utils/test_address_utils.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.931384 eth-utils-4.1.0/tests/core/applicator-utils/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     6721 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/applicator-utils/test_applicators.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.935384 eth-utils-4.1.0/tests/core/conversion-utils/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4567 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/conversion-utils/test_conversions.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.935384 eth-utils-4.1.0/tests/core/currency-utils/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4393 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/currency-utils/test_currency_tools.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      193 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/currency-utils/test_denoms_obj.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.935384 eth-utils-4.1.0/tests/core/curried-utils/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3223 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/curried-utils/test_curried.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.935384 eth-utils-4.1.0/tests/core/decorator-utils/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      666 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/decorator-utils/test_combomethod.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      690 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/decorator-utils/test_replace_exceptions.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1531 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/decorator-utils/test_validate_conversion_arguments.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.935384 eth-utils-4.1.0/tests/core/encoding-utils/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1083 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/encoding-utils/test_big_endian_integer.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.935384 eth-utils-4.1.0/tests/core/functional-utils/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1475 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/functional-utils/test_return_value_decorators.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2569 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/functional-utils/test_type_inference.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.935384 eth-utils-4.1.0/tests/core/hexadecimal-utils/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1076 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/hexadecimal-utils/test_0x_prefix_addition_and_removal.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      487 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/hexadecimal-utils/test_is_0x_prefixed.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      972 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/hexadecimal-utils/test_is_hex.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      954 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/hexadecimal-utils/test_is_hexstr.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.935384 eth-utils-4.1.0/tests/core/humanize-utils/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      374 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/humanize-utils/test_humanize_bytes.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      230 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/humanize-utils/test_humanize_hash.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      714 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/humanize-utils/test_humanize_integer_sequence.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1202 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/humanize-utils/test_humanize_ipfs_uri.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1416 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/humanize-utils/test_humanize_seconds.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1608 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/humanize-utils/test_humanize_wei.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.935384 eth-utils-4.1.0/tests/core/logging-utils/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2919 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/logging-utils/test_DEBUG2_logging.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      630 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/logging-utils/test_compat_with_abc_ABC.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2472 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/logging-utils/test_get_logger.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2760 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/logging-utils/test_has_logger_metaclass.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.935384 eth-utils-4.1.0/tests/core/module-loading-utils/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      266 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/module-loading-utils/test_import_string.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.935384 eth-utils-4.1.0/tests/core/network-utils/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2053 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/network-utils/test_network_utils.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.935384 eth-utils-4.1.0/tests/core/numeric-utils/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      369 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/numeric-utils/test_clamp.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       91 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/test_import_and_version.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.935384 eth-utils-4.1.0/tests/core/type-checks/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2216 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/type-checks/mypy_typing_of_curried_utils.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1927 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/type-checks/mypy_typing_of_functional_utils.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1352 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/type-checks/mypy_typing_of_has_logger.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:54:24.935384 eth-utils-4.1.0/tests/core/types-utils/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3014 2024-03-25 20:53:18.000000 eth-utils-4.1.0/tests/core/types-utils/test_types_utils.py
+drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-05-06 18:21:45.178264 eth_utils-4.1.1/
+-rw-r--r--   0 reedsa     (501) staff       (20)     1095 2024-03-25 20:16:33.000000 eth_utils-4.1.1/LICENSE
+-rw-r--r--   0 reedsa     (501) staff       (20)      239 2024-04-29 17:49:12.000000 eth_utils-4.1.1/MANIFEST.in
+-rw-r--r--   0 reedsa     (501) staff       (20)     5312 2024-05-06 18:21:45.176493 eth_utils-4.1.1/PKG-INFO
+-rw-r--r--   0 reedsa     (501) staff       (20)     3086 2024-03-25 20:16:33.000000 eth_utils-4.1.1/README.md
+drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-05-06 18:21:44.992322 eth_utils-4.1.1/eth_utils/
+-rw-r--r--   0 reedsa     (501) staff       (20)     2343 2024-05-06 15:03:53.000000 eth_utils-4.1.1/eth_utils/__init__.py
+drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-05-06 18:21:45.018699 eth_utils-4.1.1/eth_utils/__json/
+-rw-r--r--   0 reedsa     (501) staff       (20)   414773 2024-05-06 18:20:29.000000 eth_utils-4.1.1/eth_utils/__json/eth_networks.json
+-rw-r--r--   0 reedsa     (501) staff       (20)       86 2024-03-25 20:16:34.000000 eth_utils-4.1.1/eth_utils/__main__.py
+-rw-r--r--   0 reedsa     (501) staff       (20)     2050 2024-05-06 15:03:53.000000 eth_utils-4.1.1/eth_utils/abi.py
+-rw-r--r--   0 reedsa     (501) staff       (20)     4218 2024-03-25 20:16:34.000000 eth_utils-4.1.1/eth_utils/address.py
+-rw-r--r--   0 reedsa     (501) staff       (20)     4342 2024-03-25 20:16:34.000000 eth_utils-4.1.1/eth_utils/applicators.py
+-rw-r--r--   0 reedsa     (501) staff       (20)     5500 2024-03-25 20:16:34.000000 eth_utils-4.1.1/eth_utils/conversions.py
+-rw-r--r--   0 reedsa     (501) staff       (20)      362 2024-03-25 20:16:34.000000 eth_utils-4.1.1/eth_utils/crypto.py
+-rw-r--r--   0 reedsa     (501) staff       (20)     3021 2024-03-25 20:16:34.000000 eth_utils-4.1.1/eth_utils/currency.py
+drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-05-06 18:21:45.024030 eth_utils-4.1.1/eth_utils/curried/
+-rw-r--r--   0 reedsa     (501) staff       (20)     6497 2024-05-06 15:03:53.000000 eth_utils-4.1.1/eth_utils/curried/__init__.py
+-rw-r--r--   0 reedsa     (501) staff       (20)      499 2024-03-25 20:16:34.000000 eth_utils-4.1.1/eth_utils/debug.py
+-rw-r--r--   0 reedsa     (501) staff       (20)     3995 2024-04-08 18:45:53.000000 eth_utils-4.1.1/eth_utils/decorators.py
+-rw-r--r--   0 reedsa     (501) staff       (20)      199 2024-05-06 15:03:53.000000 eth_utils-4.1.1/eth_utils/encoding.py
+-rw-r--r--   0 reedsa     (501) staff       (20)      110 2024-04-29 17:49:14.000000 eth_utils-4.1.1/eth_utils/exceptions.py
+-rw-r--r--   0 reedsa     (501) staff       (20)     2100 2024-03-25 20:16:34.000000 eth_utils-4.1.1/eth_utils/functional.py
+-rw-r--r--   0 reedsa     (501) staff       (20)     1828 2024-03-25 20:16:34.000000 eth_utils-4.1.1/eth_utils/hexadecimal.py
+-rw-r--r--   0 reedsa     (501) staff       (20)     4148 2024-03-25 20:16:34.000000 eth_utils-4.1.1/eth_utils/humanize.py
+-rw-r--r--   0 reedsa     (501) staff       (20)     5155 2024-03-25 20:16:34.000000 eth_utils-4.1.1/eth_utils/logging.py
+-rw-r--r--   0 reedsa     (501) staff       (20)      842 2024-03-25 20:16:34.000000 eth_utils-4.1.1/eth_utils/module_loading.py
+-rw-r--r--   0 reedsa     (501) staff       (20)     2096 2024-05-06 18:20:29.000000 eth_utils-4.1.1/eth_utils/network.py
+-rw-r--r--   0 reedsa     (501) staff       (20)     1190 2024-03-25 20:16:34.000000 eth_utils-4.1.1/eth_utils/numeric.py
+-rw-r--r--   0 reedsa     (501) staff       (20)        0 2024-03-25 20:16:34.000000 eth_utils-4.1.1/eth_utils/py.typed
+-rw-r--r--   0 reedsa     (501) staff       (20)     2617 2024-03-25 20:16:34.000000 eth_utils-4.1.1/eth_utils/toolz.py
+-rw-r--r--   0 reedsa     (501) staff       (20)     1074 2024-03-25 20:16:34.000000 eth_utils-4.1.1/eth_utils/types.py
+drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-05-06 18:21:45.026699 eth_utils-4.1.1/eth_utils/typing/
+-rw-r--r--   0 reedsa     (501) staff       (20)      325 2024-03-25 20:16:34.000000 eth_utils-4.1.1/eth_utils/typing/__init__.py
+-rw-r--r--   0 reedsa     (501) staff       (20)      190 2024-03-25 20:16:34.000000 eth_utils-4.1.1/eth_utils/typing/misc.py
+-rw-r--r--   0 reedsa     (501) staff       (20)     1757 2024-03-25 20:16:34.000000 eth_utils-4.1.1/eth_utils/units.py
+drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-05-06 18:21:45.064546 eth_utils-4.1.1/eth_utils.egg-info/
+-rw-r--r--   0 reedsa     (501) staff       (20)     5312 2024-05-06 18:21:44.000000 eth_utils-4.1.1/eth_utils.egg-info/PKG-INFO
+-rw-r--r--   0 reedsa     (501) staff       (20)     2619 2024-05-06 18:21:44.000000 eth_utils-4.1.1/eth_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 reedsa     (501) staff       (20)        1 2024-05-06 18:21:44.000000 eth_utils-4.1.1/eth_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 reedsa     (501) staff       (20)        1 2024-05-06 15:21:50.000000 eth_utils-4.1.1/eth_utils.egg-info/not-zip-safe
+-rw-r--r--   0 reedsa     (501) staff       (20)      558 2024-05-06 18:21:44.000000 eth_utils-4.1.1/eth_utils.egg-info/requires.txt
+-rw-r--r--   0 reedsa     (501) staff       (20)       10 2024-05-06 18:21:44.000000 eth_utils-4.1.1/eth_utils.egg-info/top_level.txt
+-rw-r--r--   0 reedsa     (501) staff       (20)     3453 2024-05-06 15:03:53.000000 eth_utils-4.1.1/pyproject.toml
+-rw-r--r--   0 reedsa     (501) staff       (20)       38 2024-05-06 18:21:45.178483 eth_utils-4.1.1/setup.cfg
+-rw-r--r--   0 reedsa     (501) staff       (20)     2237 2024-05-06 18:21:36.000000 eth_utils-4.1.1/setup.py
+drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-05-06 18:21:44.887208 eth_utils-4.1.1/tests/
+drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-05-06 18:21:45.027449 eth_utils-4.1.1/tests/core/
+drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-05-06 18:21:45.028302 eth_utils-4.1.1/tests/core/abi-utils/
+-rw-r--r--   0 reedsa     (501) staff       (20)     5031 2024-05-06 15:03:53.000000 eth_utils-4.1.1/tests/core/abi-utils/test_abi_utils.py
+drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-05-06 18:21:45.029634 eth_utils-4.1.1/tests/core/address-utils/
+-rw-r--r--   0 reedsa     (501) staff       (20)    10843 2024-04-08 18:45:53.000000 eth_utils-4.1.1/tests/core/address-utils/test_address_utils.py
+drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-05-06 18:21:45.030545 eth_utils-4.1.1/tests/core/applicator-utils/
+-rw-r--r--   0 reedsa     (501) staff       (20)     6720 2024-05-06 15:03:53.000000 eth_utils-4.1.1/tests/core/applicator-utils/test_applicators.py
+drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-05-06 18:21:45.031511 eth_utils-4.1.1/tests/core/conversion-utils/
+-rw-r--r--   0 reedsa     (501) staff       (20)     4567 2024-04-08 18:45:53.000000 eth_utils-4.1.1/tests/core/conversion-utils/test_conversions.py
+drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-05-06 18:21:45.033609 eth_utils-4.1.1/tests/core/currency-utils/
+-rw-r--r--   0 reedsa     (501) staff       (20)     4393 2024-05-06 15:03:53.000000 eth_utils-4.1.1/tests/core/currency-utils/test_currency_tools.py
+-rw-r--r--   0 reedsa     (501) staff       (20)      193 2024-04-08 18:45:53.000000 eth_utils-4.1.1/tests/core/currency-utils/test_denoms_obj.py
+drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-05-06 18:21:45.034469 eth_utils-4.1.1/tests/core/curried-utils/
+-rw-r--r--   0 reedsa     (501) staff       (20)     3223 2024-04-08 18:45:53.000000 eth_utils-4.1.1/tests/core/curried-utils/test_curried.py
+drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-05-06 18:21:45.036600 eth_utils-4.1.1/tests/core/decorator-utils/
+-rw-r--r--   0 reedsa     (501) staff       (20)      666 2024-04-08 18:45:53.000000 eth_utils-4.1.1/tests/core/decorator-utils/test_combomethod.py
+-rw-r--r--   0 reedsa     (501) staff       (20)      690 2024-04-08 18:45:53.000000 eth_utils-4.1.1/tests/core/decorator-utils/test_replace_exceptions.py
+-rw-r--r--   0 reedsa     (501) staff       (20)     1531 2024-04-08 18:45:53.000000 eth_utils-4.1.1/tests/core/decorator-utils/test_validate_conversion_arguments.py
+drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-05-06 18:21:45.037402 eth_utils-4.1.1/tests/core/encoding-utils/
+-rw-r--r--   0 reedsa     (501) staff       (20)     1084 2024-04-29 18:00:01.000000 eth_utils-4.1.1/tests/core/encoding-utils/test_big_endian_integer.py
+drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-05-06 18:21:45.040967 eth_utils-4.1.1/tests/core/functional-utils/
+-rw-r--r--   0 reedsa     (501) staff       (20)     1475 2024-04-08 18:45:53.000000 eth_utils-4.1.1/tests/core/functional-utils/test_return_value_decorators.py
+-rw-r--r--   0 reedsa     (501) staff       (20)     2569 2024-04-29 18:00:01.000000 eth_utils-4.1.1/tests/core/functional-utils/test_type_inference.py
+drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-05-06 18:21:45.045297 eth_utils-4.1.1/tests/core/hexadecimal-utils/
+-rw-r--r--   0 reedsa     (501) staff       (20)     1076 2024-04-08 18:45:53.000000 eth_utils-4.1.1/tests/core/hexadecimal-utils/test_0x_prefix_addition_and_removal.py
+-rw-r--r--   0 reedsa     (501) staff       (20)      487 2024-04-08 18:45:53.000000 eth_utils-4.1.1/tests/core/hexadecimal-utils/test_is_0x_prefixed.py
+-rw-r--r--   0 reedsa     (501) staff       (20)      972 2024-04-08 18:45:53.000000 eth_utils-4.1.1/tests/core/hexadecimal-utils/test_is_hex.py
+-rw-r--r--   0 reedsa     (501) staff       (20)      954 2024-04-08 18:45:53.000000 eth_utils-4.1.1/tests/core/hexadecimal-utils/test_is_hexstr.py
+drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-05-06 18:21:45.051831 eth_utils-4.1.1/tests/core/humanize-utils/
+-rw-r--r--   0 reedsa     (501) staff       (20)      374 2024-04-08 18:45:53.000000 eth_utils-4.1.1/tests/core/humanize-utils/test_humanize_bytes.py
+-rw-r--r--   0 reedsa     (501) staff       (20)      230 2024-04-08 18:45:53.000000 eth_utils-4.1.1/tests/core/humanize-utils/test_humanize_hash.py
+-rw-r--r--   0 reedsa     (501) staff       (20)      714 2024-04-08 18:45:53.000000 eth_utils-4.1.1/tests/core/humanize-utils/test_humanize_integer_sequence.py
+-rw-r--r--   0 reedsa     (501) staff       (20)     1202 2024-04-08 18:45:53.000000 eth_utils-4.1.1/tests/core/humanize-utils/test_humanize_ipfs_uri.py
+-rw-r--r--   0 reedsa     (501) staff       (20)     1416 2024-04-08 18:45:53.000000 eth_utils-4.1.1/tests/core/humanize-utils/test_humanize_seconds.py
+-rw-r--r--   0 reedsa     (501) staff       (20)     1608 2024-04-08 18:45:53.000000 eth_utils-4.1.1/tests/core/humanize-utils/test_humanize_wei.py
+drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-05-06 18:21:45.054385 eth_utils-4.1.1/tests/core/logging-utils/
+-rw-r--r--   0 reedsa     (501) staff       (20)     2918 2024-05-06 15:03:53.000000 eth_utils-4.1.1/tests/core/logging-utils/test_DEBUG2_logging.py
+-rw-r--r--   0 reedsa     (501) staff       (20)      629 2024-05-06 15:03:53.000000 eth_utils-4.1.1/tests/core/logging-utils/test_compat_with_abc_ABC.py
+-rw-r--r--   0 reedsa     (501) staff       (20)     2472 2024-04-08 18:45:53.000000 eth_utils-4.1.1/tests/core/logging-utils/test_get_logger.py
+-rw-r--r--   0 reedsa     (501) staff       (20)     2760 2024-04-08 18:45:53.000000 eth_utils-4.1.1/tests/core/logging-utils/test_has_logger_metaclass.py
+drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-05-06 18:21:45.055178 eth_utils-4.1.1/tests/core/module-loading-utils/
+-rw-r--r--   0 reedsa     (501) staff       (20)      266 2024-04-08 18:45:53.000000 eth_utils-4.1.1/tests/core/module-loading-utils/test_import_string.py
+drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-05-06 18:21:45.056865 eth_utils-4.1.1/tests/core/network-utils/
+-rw-r--r--   0 reedsa     (501) staff       (20)     2054 2024-04-29 18:00:01.000000 eth_utils-4.1.1/tests/core/network-utils/test_network_utils.py
+drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-05-06 18:21:45.058661 eth_utils-4.1.1/tests/core/numeric-utils/
+-rw-r--r--   0 reedsa     (501) staff       (20)      369 2024-04-08 18:45:53.000000 eth_utils-4.1.1/tests/core/numeric-utils/test_clamp.py
+-rw-r--r--   0 reedsa     (501) staff       (20)      103 2024-04-29 17:49:12.000000 eth_utils-4.1.1/tests/core/test_import_and_version.py
+drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-05-06 18:21:45.062198 eth_utils-4.1.1/tests/core/type-checks/
+-rw-r--r--   0 reedsa     (501) staff       (20)     2216 2024-04-08 18:45:53.000000 eth_utils-4.1.1/tests/core/type-checks/mypy_typing_of_curried_utils.py
+-rw-r--r--   0 reedsa     (501) staff       (20)     1927 2024-04-08 18:45:53.000000 eth_utils-4.1.1/tests/core/type-checks/mypy_typing_of_functional_utils.py
+-rw-r--r--   0 reedsa     (501) staff       (20)     1352 2024-04-08 18:45:53.000000 eth_utils-4.1.1/tests/core/type-checks/mypy_typing_of_has_logger.py
+drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-05-06 18:21:45.063308 eth_utils-4.1.1/tests/core/types-utils/
+-rw-r--r--   0 reedsa     (501) staff       (20)     3014 2024-04-08 18:45:53.000000 eth_utils-4.1.1/tests/core/types-utils/test_types_utils.py
```

### Comparing `eth-utils-4.1.0/LICENSE` & `eth_utils-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/PKG-INFO` & `eth_utils-4.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-utils
-Version: 4.1.0
+Version: 4.1.1
 Summary: eth-utils: Common utility functions for python code that interacts with Ethereum
 Home-page: https://github.com/ethereum/eth-utils
 Author: The Ethereum Foundation
 Author-email: snakecharmers@ethereum.org
 License: MIT
 Keywords: ethereum
 Classifier: Intended Audience :: Developers
@@ -29,22 +29,24 @@
 Requires-Dist: eth-hash[pycryptodome]; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
 Requires-Dist: pre-commit>=3.4.0; extra == "dev"
 Requires-Dist: tox>=4.0.0; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 Requires-Dist: sphinx>=6.0.0; extra == "dev"
+Requires-Dist: sphinx-autobuild>=2021.3.14; extra == "dev"
 Requires-Dist: sphinx_rtd_theme>=1.0.0; extra == "dev"
 Requires-Dist: towncrier<22,>=21; extra == "dev"
 Requires-Dist: hypothesis>=4.43.0; extra == "dev"
 Requires-Dist: mypy==1.5.1; extra == "dev"
 Requires-Dist: pytest>=7.0.0; extra == "dev"
 Requires-Dist: pytest-xdist>=2.4.0; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: sphinx>=6.0.0; extra == "docs"
+Requires-Dist: sphinx-autobuild>=2021.3.14; extra == "docs"
 Requires-Dist: sphinx_rtd_theme>=1.0.0; extra == "docs"
 Requires-Dist: towncrier<22,>=21; extra == "docs"
 Provides-Extra: test
 Requires-Dist: hypothesis>=4.43.0; extra == "test"
 Requires-Dist: mypy==1.5.1; extra == "test"
 Requires-Dist: pytest>=7.0.0; extra == "test"
 Requires-Dist: pytest-xdist>=2.4.0; extra == "test"
```

### Comparing `eth-utils-4.1.0/README.md` & `eth_utils-4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/eth_utils/__init__.py` & `eth_utils-4.1.1/eth_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/eth_utils/__json/eth_networks.json` & `eth_utils-4.1.1/eth_utils/__json/eth_networks.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7247201634539006%*

 * *Differences: {'0': "{'rpc': {insert: [(4, 'https://ethereum-rpc.publicnode.com'), (5, "*

 * *      "'wss://ethereum-rpc.publicnode.com'), (15, 'https://eth.drpc.org'), (16, "*

 * *      "'wss://eth.drpc.org')], delete: [5, 4]}}",*

 * * '1002': "{'name': 'MAP Protocol', 'shortName': 'mapo', 'infoURL': 'https://mapprotocol.io/'}",*

 * * '1006': "{'rpc': ['https://testnet.sapphire.oasis.io', 'wss://testnet.sapphire.oasis.io/ws']}",*

 * * '102': "{'name': 'WorldLand Mainnet', 'nativeCurrency': {'symbol': 'WLC'}, 'rpc': {insert: [(1, "*

 * *        "'htt […]*

```diff
@@ -11,25 +11,27 @@
         },
         "networkId": 1,
         "rpc": [
             "https://mainnet.infura.io/v3/${INFURA_API_KEY}",
             "wss://mainnet.infura.io/ws/v3/${INFURA_API_KEY}",
             "https://api.mycryptoapi.com/eth",
             "https://cloudflare-eth.com",
-            "https://ethereum.publicnode.com",
-            "wss://ethereum.publicnode.com",
+            "https://ethereum-rpc.publicnode.com",
+            "wss://ethereum-rpc.publicnode.com",
             "https://mainnet.gateway.tenderly.co",
             "wss://mainnet.gateway.tenderly.co",
             "https://rpc.blocknative.com/boost",
             "https://rpc.flashbots.net",
             "https://rpc.flashbots.net/fast",
             "https://rpc.mevblocker.io",
             "https://rpc.mevblocker.io/fast",
             "https://rpc.mevblocker.io/noreverts",
-            "https://rpc.mevblocker.io/fullprivacy"
+            "https://rpc.mevblocker.io/fullprivacy",
+            "https://eth.drpc.org",
+            "wss://eth.drpc.org"
         ],
         "shortName": "eth"
     },
     {
         "chainId": 2,
         "faucets": [],
         "infoURL": "https://expanse.tech",
@@ -100,35 +102,33 @@
             "symbol": "ETH"
         },
         "networkId": 5,
         "rpc": [
             "https://goerli.infura.io/v3/${INFURA_API_KEY}",
             "wss://goerli.infura.io/v3/${INFURA_API_KEY}",
             "https://rpc.goerli.mudit.blog/",
-            "https://ethereum-goerli.publicnode.com",
-            "wss://ethereum-goerli.publicnode.com",
+            "https://ethereum-goerli-rpc.publicnode.com",
+            "wss://ethereum-goerli-rpc.publicnode.com",
             "https://goerli.gateway.tenderly.co",
             "wss://goerli.gateway.tenderly.co"
         ],
         "shortName": "gor"
     },
     {
         "chainId": 6,
         "faucets": [],
-        "infoURL": "https://explorer.jade.builders/?network=kotti",
-        "name": "Ethereum Classic Testnet Kotti",
+        "infoURL": "https://ethereumclassic.org/development/testnets",
+        "name": "Kotti Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Kotti Ether",
             "symbol": "KOT"
         },
         "networkId": 6,
-        "rpc": [
-            "https://www.ethercluster.com/kotti"
-        ],
+        "rpc": [],
         "shortName": "kot"
     },
     {
         "chainId": 7,
         "faucets": [],
         "infoURL": "https://thaichain.io",
         "name": "ThaiChain",
@@ -184,18 +184,20 @@
             "decimals": 18,
             "name": "Ether",
             "symbol": "ETH"
         },
         "networkId": 10,
         "rpc": [
             "https://mainnet.optimism.io",
-            "https://optimism.publicnode.com",
-            "wss://optimism.publicnode.com",
+            "https://optimism-rpc.publicnode.com",
+            "wss://optimism-rpc.publicnode.com",
             "https://optimism.gateway.tenderly.co",
-            "wss://optimism.gateway.tenderly.co"
+            "wss://optimism.gateway.tenderly.co",
+            "https://optimism.drpc.org",
+            "wss://optimism.drpc.org"
         ],
         "shortName": "oeth"
     },
     {
         "chainId": 11,
         "faucets": [],
         "infoURL": "https://metadium.com",
@@ -253,16 +255,22 @@
             "decimals": 18,
             "name": "Flare",
             "symbol": "FLR"
         },
         "networkId": 14,
         "rpc": [
             "https://flare-api.flare.network/ext/C/rpc",
-            "https://flare.public-rpc.com",
-            "https://rpc.ftso.au/flare"
+            "https://flare.rpc.thirdweb.com",
+            "https://flare-bundler.etherspot.io",
+            "https://rpc.ankr.com/flare",
+            "https://01-gravelines-003-01.rpc.tatum.io/ext/bc/C/rpc",
+            "https://01-vinthill-003-02.rpc.tatum.io/ext/bc/C/rpc",
+            "https://rpc.ftso.au/flare",
+            "https://flare.enosys.global/ext/C/rpc",
+            "https://flare.solidifi.app/ext/C/rpc"
         ],
         "shortName": "flr"
     },
     {
         "chainId": 15,
         "faucets": [],
         "infoURL": "https://diode.io/prenet",
@@ -278,27 +286,31 @@
             "wss://prenet.diode.io:8443/ws"
         ],
         "shortName": "diode"
     },
     {
         "chainId": 16,
         "faucets": [
-            "https://faucet.towolabs.com",
-            "https://fauceth.komputing.org?chain=16&address=${ADDRESS}"
+            "https://faucet.flare.network"
         ],
-        "infoURL": "https://flare.xyz",
-        "name": "Flare Testnet Coston",
+        "infoURL": "https://flare.network",
+        "name": "Songbird Testnet Coston",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Coston Flare",
             "symbol": "CFLR"
         },
         "networkId": 16,
         "rpc": [
-            "https://coston-api.flare.network/ext/bc/C/rpc"
+            "https://coston-api.flare.network/ext/C/rpc",
+            "https://songbird-testnet-coston.rpc.thirdweb.com",
+            "https://01-gravelines-004-01.rpc.tatum.io/ext/bc/C/rpc",
+            "https://02-chicago-004-02.rpc.tatum.io/ext/bc/C/rpc",
+            "https://02-tokyo-004-03.rpc.tatum.io/ext/bc/C/rpc",
+            "https://coston.enosys.global/ext/C/rpc"
         ],
         "shortName": "cflr"
     },
     {
         "chainId": 17,
         "faucets": [],
         "infoURL": "https://exp.thaifi.com",
@@ -324,35 +336,39 @@
         "nativeCurrency": {
             "decimals": 18,
             "name": "ThunderCore Testnet Token",
             "symbol": "TST"
         },
         "networkId": 18,
         "rpc": [
-            "https://testnet-rpc.thundercore.com"
+            "https://testnet-rpc.thundercore.com",
+            "https://thundercore-testnet.drpc.org",
+            "wss://thundercore-testnet.drpc.org"
         ],
         "shortName": "TST"
     },
     {
         "chainId": 19,
         "faucets": [],
-        "infoURL": "https://flare.xyz",
+        "infoURL": "https://flare.network",
         "name": "Songbird Canary-Network",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Songbird",
             "symbol": "SGB"
         },
         "networkId": 19,
         "rpc": [
             "https://songbird-api.flare.network/ext/C/rpc",
-            "https://sgb.ftso.com.au/ext/bc/C/rpc",
-            "https://sgb.lightft.so/rpc",
-            "https://sgb-rpc.ftso.eu",
-            "https://rpc.ftso.au/songbird"
+            "https://01-gravelines-006-01.rpc.tatum.io/ext/bc/C/rpc",
+            "https://01-vinthill-006-02.rpc.tatum.io/ext/bc/C/rpc",
+            "https://02-tokyo-006-03.rpc.tatum.io/ext/bc/C/rpc",
+            "https://rpc.ftso.au/songbird",
+            "https://songbird.enosys.global/ext/C/rpc",
+            "https://songbird.solidifi.app/ext/C/rpc"
         ],
         "shortName": "sgb"
     },
     {
         "chainId": 20,
         "faucets": [],
         "infoURL": "https://www.elastos.org/",
@@ -439,16 +455,18 @@
             "decimals": 18,
             "name": "Cronos",
             "symbol": "CRO"
         },
         "networkId": 25,
         "rpc": [
             "https://evm.cronos.org",
-            "https://cronos-evm.publicnode.com",
-            "wss://cronos-evm.publicnode.com"
+            "https://cronos-evm-rpc.publicnode.com",
+            "wss://cronos-evm-rpc.publicnode.com",
+            "https://cronos.drpc.org",
+            "wss://cronos.drpc.org"
         ],
         "shortName": "cro"
     },
     {
         "chainId": 26,
         "faucets": [],
         "infoURL": "https://www.genesisl1.com",
@@ -578,17 +596,15 @@
         "rpc": [
             "https://rpc.goodata.io"
         ],
         "shortName": "GooD"
     },
     {
         "chainId": 34,
-        "faucets": [
-            "https://faucet.securechain.ai"
-        ],
+        "faucets": [],
         "infoURL": "https://securechain.ai",
         "name": "SecureChain Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "SecureChain",
             "symbol": "SCAI"
         },
@@ -686,15 +702,17 @@
         "nativeCurrency": {
             "decimals": 18,
             "name": "Telos",
             "symbol": "TLOS"
         },
         "networkId": 40,
         "rpc": [
-            "https://mainnet.telos.net/evm"
+            "https://mainnet.telos.net/evm",
+            "https://telos.drpc.org",
+            "wss://telos.drpc.org"
         ],
         "shortName": "TelosEVM"
     },
     {
         "chainId": 41,
         "faucets": [
             "https://app.telos.net/testnet/developers"
@@ -704,15 +722,17 @@
         "nativeCurrency": {
             "decimals": 18,
             "name": "Telos",
             "symbol": "TLOS"
         },
         "networkId": 41,
         "rpc": [
-            "https://testnet.telos.net/evm"
+            "https://testnet.telos.net/evm",
+            "https://telos-testnet.drpc.org",
+            "wss://telos-testnet.drpc.org"
         ],
         "shortName": "TelosEVMTestnet"
     },
     {
         "chainId": 42,
         "faucets": [],
         "infoURL": "https://lukso.network",
@@ -756,16 +776,15 @@
             "decimals": 18,
             "name": "Crab Network Native Token",
             "symbol": "CRAB"
         },
         "networkId": 44,
         "rpc": [
             "https://crab-rpc.darwinia.network",
-            "https://crab-rpc.darwiniacommunitydao.xyz",
-            "https://darwiniacrab-rpc.dwellir.com"
+            "https://crab-rpc.darwiniacommunitydao.xyz"
         ],
         "shortName": "crab"
     },
     {
         "chainId": 45,
         "faucets": [
             "https://docs.darwinia.network/pangoro-testnet-70cfec5dc9ca42759959ba3803edaec2"
@@ -793,15 +812,14 @@
             "name": "Darwinia Network Native Token",
             "symbol": "RING"
         },
         "networkId": 46,
         "rpc": [
             "https://rpc.darwinia.network",
             "https://darwinia-rpc.darwiniacommunitydao.xyz",
-            "https://darwinia2.api.onfinality.io/public-ws",
             "https://darwinia-rpc.dwellir.com"
         ],
         "shortName": "darwinia"
     },
     {
         "chainId": 47,
         "faucets": [],
@@ -977,16 +995,16 @@
             "https://bsc-dataseed2.defibit.io",
             "https://bsc-dataseed3.defibit.io",
             "https://bsc-dataseed4.defibit.io",
             "https://bsc-dataseed1.ninicoin.io",
             "https://bsc-dataseed2.ninicoin.io",
             "https://bsc-dataseed3.ninicoin.io",
             "https://bsc-dataseed4.ninicoin.io",
-            "https://bsc.publicnode.com",
-            "wss://bsc.publicnode.com",
+            "https://bsc-rpc.publicnode.com",
+            "wss://bsc-rpc.publicnode.com",
             "wss://bsc-ws-node.nariox.org"
         ],
         "shortName": "bnb"
     },
     {
         "chainId": 57,
         "faucets": [
@@ -1065,58 +1083,64 @@
         ],
         "shortName": "go"
     },
     {
         "chainId": 61,
         "faucets": [],
         "infoURL": "https://ethereumclassic.org",
-        "name": "Ethereum Classic Mainnet",
+        "name": "Ethereum Classic",
         "nativeCurrency": {
             "decimals": 18,
-            "name": "Ethereum Classic Ether",
+            "name": "Ether",
             "symbol": "ETC"
         },
         "networkId": 1,
         "rpc": [
             "https://etc.rivet.link",
+            "https://besu-at.etc-network.info",
+            "https://besu-de.etc-network.info",
+            "https://geth-at.etc-network.info",
+            "https://geth-de.etc-network.info",
             "https://etc.etcdesktop.com",
+            "https://rpc.etcinscribe.com",
             "https://etc.mytokenpocket.vip"
         ],
         "shortName": "etc"
     },
     {
         "chainId": 62,
         "faucets": [],
-        "infoURL": "https://ethereumclassic.org",
-        "name": "Ethereum Classic Testnet Morden",
+        "infoURL": "https://ethereumclassic.org/development/testnets",
+        "name": "Morden Testnet",
         "nativeCurrency": {
             "decimals": 18,
-            "name": "Ethereum Classic Testnet Ether",
+            "name": "Morden Ether",
             "symbol": "TETC"
         },
         "networkId": 2,
         "rpc": [],
         "shortName": "tetc"
     },
     {
         "chainId": 63,
         "faucets": [
-            "https://mordor.canhaz.net/",
-            "https://easy.hebeswap.com/#/faucet"
+            "https://easy.hebeswap.com/#/faucet",
+            "https://faucet.mordortest.net"
         ],
-        "infoURL": "https://github.com/eth-classic/mordor/",
-        "name": "Ethereum Classic Testnet Mordor",
+        "infoURL": "https://ethereumclassic.org/development/testnets",
+        "name": "Mordor Testnet",
         "nativeCurrency": {
             "decimals": 18,
-            "name": "Mordor Classic Testnet Ether",
+            "name": "Mordor Ether",
             "symbol": "METC"
         },
         "networkId": 7,
         "rpc": [
-            "https://rpc.mordor.etccooperative.org"
+            "https://rpc.mordor.etccooperative.org",
+            "https://geth-mordor.etc-network.info"
         ],
         "shortName": "metc"
     },
     {
         "chainId": 64,
         "faucets": [],
         "infoURL": "https://ellaism.org",
@@ -1537,42 +1561,42 @@
             "https://rpc.novanetwork.io:9070"
         ],
         "shortName": "nnw"
     },
     {
         "chainId": 88,
         "faucets": [],
-        "infoURL": "https://tomochain.com",
-        "name": "TomoChain",
+        "infoURL": "https://viction.xyz",
+        "name": "Viction",
         "nativeCurrency": {
             "decimals": 18,
-            "name": "TomoChain",
-            "symbol": "TOMO"
+            "name": "Viction",
+            "symbol": "VIC"
         },
         "networkId": 88,
         "rpc": [
-            "https://rpc.tomochain.com"
+            "https://rpc.viction.xyz"
         ],
-        "shortName": "tomo"
+        "shortName": "vic"
     },
     {
         "chainId": 89,
         "faucets": [],
-        "infoURL": "https://tomochain.com",
-        "name": "TomoChain Testnet",
+        "infoURL": "https://viction.xyz",
+        "name": "Viction Testnet",
         "nativeCurrency": {
             "decimals": 18,
-            "name": "TomoChain",
-            "symbol": "TOMO"
+            "name": "Viction",
+            "symbol": "VIC"
         },
         "networkId": 89,
         "rpc": [
-            "https://rpc.testnet.tomochain.com"
+            "https://rpc-testnet.viction.xyz"
         ],
-        "shortName": "tomot"
+        "shortName": "vict"
     },
     {
         "chainId": 90,
         "faucets": [],
         "infoURL": "https://garizon.com",
         "name": "Garizon Stage0",
         "nativeCurrency": {
@@ -1701,16 +1725,16 @@
         "rpc": [
             "https://data-seed-prebsc-1-s1.bnbchain.org:8545",
             "https://data-seed-prebsc-2-s1.bnbchain.org:8545",
             "https://data-seed-prebsc-1-s2.bnbchain.org:8545",
             "https://data-seed-prebsc-2-s2.bnbchain.org:8545",
             "https://data-seed-prebsc-1-s3.bnbchain.org:8545",
             "https://data-seed-prebsc-2-s3.bnbchain.org:8545",
-            "https://bsc-testnet.publicnode.com",
-            "wss://bsc-testnet.publicnode.com"
+            "https://bsc-testnet-rpc.publicnode.com",
+            "wss://bsc-testnet-rpc.publicnode.com"
         ],
         "shortName": "bnbt"
     },
     {
         "chainId": 98,
         "faucets": [],
         "infoURL": "https://six.network/",
@@ -1764,16 +1788,16 @@
             "https://gnosischain-rpc.gateway.pokt.network",
             "https://gnosis-mainnet.public.blastapi.io",
             "https://gnosis.api.onfinality.io/public",
             "https://gnosis.blockpi.network/v1/rpc/public",
             "https://web3endpoints.com/gnosischain-mainnet",
             "https://gnosis.oat.farm",
             "wss://rpc.gnosischain.com/wss",
-            "https://gnosis.publicnode.com",
-            "wss://gnosis.publicnode.com"
+            "https://gnosis-rpc.publicnode.com",
+            "wss://gnosis-rpc.publicnode.com"
         ],
         "shortName": "gno"
     },
     {
         "chainId": 101,
         "faucets": [],
         "infoURL": "https://einc.io",
@@ -1807,23 +1831,24 @@
         ],
         "shortName": "tw3g"
     },
     {
         "chainId": 103,
         "faucets": [],
         "infoURL": "https://worldland.foundation",
-        "name": "Worldland Mainnet",
+        "name": "WorldLand Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Worldland",
-            "symbol": "WL"
+            "symbol": "WLC"
         },
         "networkId": 103,
         "rpc": [
-            "https://seoul.worldland.foundation"
+            "https://seoul.worldland.foundation",
+            "https://seoul2.worldland.foundation"
         ],
         "shortName": "WLC"
     },
     {
         "chainId": 104,
         "faucets": [],
         "infoURL": "https://kaibadefi.com",
@@ -1994,26 +2019,32 @@
             "https://rpc2.dehvo.com"
         ],
         "shortName": "deh"
     },
     {
         "chainId": 114,
         "faucets": [
-            "https://coston2-faucet.towolabs.com"
+            "https://faucet.flare.network"
         ],
-        "infoURL": "https://flare.xyz",
+        "infoURL": "https://flare.network",
         "name": "Flare Testnet Coston2",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Coston2 Flare",
             "symbol": "C2FLR"
         },
         "networkId": 114,
         "rpc": [
-            "https://coston2-api.flare.network/ext/bc/C/rpc"
+            "https://coston2-api.flare.network/ext/C/rpc",
+            "https://flare-testnet-coston2.rpc.thirdweb.com",
+            "https://flaretestnet-bundler.etherspot.io",
+            "https://01-gravelines-005-01.rpc.tatum.io/ext/bc/C/rpc",
+            "https://02-chicago-005-02.rpc.tatum.io/ext/bc/C/rpc",
+            "https://02-tokyo-005-03.rpc.tatum.io/ext/bc/C/rpc",
+            "https://coston2.enosys.global/ext/C/rpc"
         ],
         "shortName": "c2flr"
     },
     {
         "chainId": 115,
         "faucets": [],
         "infoURL": "https://debank.com",
@@ -2140,15 +2171,17 @@
         "nativeCurrency": {
             "decimals": 18,
             "name": "Fuse",
             "symbol": "FUSE"
         },
         "networkId": 122,
         "rpc": [
-            "https://rpc.fuse.io"
+            "https://rpc.fuse.io",
+            "https://fuse.drpc.org",
+            "wss://fuse.drpc.org"
         ],
         "shortName": "fuse"
     },
     {
         "chainId": 123,
         "faucets": [
             "https://get.fusespark.io"
@@ -2244,14 +2277,61 @@
         "rpc": [
             "https://http-mainnet.hecochain.com",
             "wss://ws-mainnet.hecochain.com"
         ],
         "shortName": "heco"
     },
     {
+        "chainId": 129,
+        "faucets": [],
+        "infoURL": "https://innovatorchain.com",
+        "name": "Innovator Chain",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "INOV8",
+            "symbol": "INOV8"
+        },
+        "networkId": 129,
+        "rpc": [
+            "https://rpc.innovatorchain.com"
+        ],
+        "shortName": "Innovator"
+    },
+    {
+        "chainId": 131,
+        "faucets": [],
+        "infoURL": "https://engramnet.io",
+        "name": "Engram Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Engram Tokio Testnet",
+            "symbol": "tGRAM"
+        },
+        "networkId": 131,
+        "rpc": [
+            "https://tokioswift.engram.tech",
+            "https://tokio-archive.engram.tech"
+        ],
+        "shortName": "tgram"
+    },
+    {
+        "chainId": 133,
+        "faucets": [],
+        "infoURL": "https://hashkey.cloud",
+        "name": "HashKey Chain Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "HashKey EcoPoints",
+            "symbol": "HSK"
+        },
+        "networkId": 133,
+        "rpc": [],
+        "shortName": "HSKT"
+    },
+    {
         "chainId": 134,
         "faucets": [],
         "infoURL": "https://iex.ec",
         "name": "iExec Sidechain",
         "nativeCurrency": {
             "decimals": 18,
             "name": "xRLC",
@@ -2311,35 +2391,37 @@
         "rpc": [
             "https://polygon-rpc.com/",
             "https://rpc-mainnet.matic.network",
             "https://matic-mainnet.chainstacklabs.com",
             "https://rpc-mainnet.maticvigil.com",
             "https://rpc-mainnet.matic.quiknode.pro",
             "https://matic-mainnet-full-rpc.bwarelabs.com",
-            "https://polygon-bor.publicnode.com",
-            "wss://polygon-bor.publicnode.com",
+            "https://polygon-bor-rpc.publicnode.com",
+            "wss://polygon-bor-rpc.publicnode.com",
             "https://polygon.gateway.tenderly.co",
-            "wss://polygon.gateway.tenderly.co"
+            "wss://polygon.gateway.tenderly.co",
+            "https://polygon.drpc.org",
+            "wss://polygon.drpc.org"
         ],
         "shortName": "matic"
     },
     {
         "chainId": 138,
         "faucets": [],
-        "infoURL": "https://defi-oracle.io/",
+        "infoURL": "https://info.defi-oracle.io/",
         "name": "Defi Oracle Meta Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Ether",
             "symbol": "ETH"
         },
         "networkId": 1,
         "rpc": [
-            "https://rpc.public-0138.defi-oracle.io",
-            "wss://rpc.public-0138.defi-oracle.io"
+            "https://rpc.defi-oracle.io",
+            "wss://wss.defi-oracle.io"
         ],
         "shortName": "dfio-meta-main"
     },
     {
         "chainId": 139,
         "faucets": [],
         "infoURL": "https://wikiwoop.com",
@@ -2400,28 +2482,44 @@
         "networkId": 144,
         "rpc": [
             "https://connect.phi.network"
         ],
         "shortName": "PHI"
     },
     {
+        "chainId": 145,
+        "faucets": [],
+        "infoURL": "https://soraai.bot",
+        "name": "SoraAI Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "SoraETH",
+            "symbol": "SETH"
+        },
+        "networkId": 145,
+        "rpc": [
+            "https://rpc-testnet.soraai.bot"
+        ],
+        "shortName": "SETH"
+    },
+    {
         "chainId": 148,
         "faucets": [],
         "infoURL": "https://shimmer.network",
-        "name": "ShimmerEVM Mainnet",
+        "name": "ShimmerEVM",
         "nativeCurrency": {
             "decimals": 18,
             "name": "SMR",
             "symbol": "SMR"
         },
         "networkId": 148,
         "rpc": [
             "https://json-rpc.evm.shimmer.network"
         ],
-        "shortName": "shimmerevm-mainnet"
+        "shortName": "shimmerevm"
     },
     {
         "chainId": 150,
         "faucets": [
             "https://faucet.sixprotocol.net"
         ],
         "infoURL": "https://six.network/",
@@ -2524,14 +2622,64 @@
         "networkId": 156,
         "rpc": [
             "https://testnet-rpc.oeblock.com"
         ],
         "shortName": "obe"
     },
     {
+        "chainId": 157,
+        "faucets": [
+            "https://beta.shibariumtech.com/faucet"
+        ],
+        "infoURL": "https://shibariumecosystem.com",
+        "name": "Puppynet Shibarium",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "BONE",
+            "symbol": "BONE"
+        },
+        "networkId": 157,
+        "rpc": [
+            "https://puppynet.shibrpc.com"
+        ],
+        "shortName": "puppynet"
+    },
+    {
+        "chainId": 158,
+        "faucets": [],
+        "infoURL": "https://www.roburna.com/",
+        "name": "Roburna Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Roburna",
+            "symbol": "RBA"
+        },
+        "networkId": 158,
+        "rpc": [
+            "https://dataseed.roburna.com"
+        ],
+        "shortName": "rba"
+    },
+    {
+        "chainId": 159,
+        "faucets": [],
+        "infoURL": "https://www.roburna.com/",
+        "name": "Roburna Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Roburna",
+            "symbol": "RBAT"
+        },
+        "networkId": 159,
+        "rpc": [
+            "https://preseed-testnet-1.roburna.com"
+        ],
+        "shortName": "rbat"
+    },
+    {
         "chainId": 160,
         "faucets": [],
         "infoURL": "https://amax.network",
         "name": "Armonia Eva Chain Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Armonia Multichain Native Token",
@@ -2590,14 +2738,28 @@
         "networkId": 163,
         "rpc": [
             "https://node.mainnet.lightstreams.io"
         ],
         "shortName": "pht"
     },
     {
+        "chainId": 164,
+        "faucets": [],
+        "infoURL": "https://docs.omni.network",
+        "name": "Omni Testnet (incubating)",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Omni",
+            "symbol": "OMNI"
+        },
+        "networkId": 164,
+        "rpc": [],
+        "shortName": "omni_testnet_164"
+    },
+    {
         "chainId": 165,
         "faucets": [],
         "infoURL": "https://docs.omni.network/",
         "name": "Omni Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Omni",
@@ -2606,14 +2768,28 @@
         "networkId": 165,
         "rpc": [
             "https://testnet.omni.network"
         ],
         "shortName": "omni_testnet"
     },
     {
+        "chainId": 166,
+        "faucets": [],
+        "infoURL": "https://docs.omni.network/",
+        "name": "Omni",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Omni",
+            "symbol": "OMNI"
+        },
+        "networkId": 166,
+        "rpc": [],
+        "shortName": "omni"
+    },
+    {
         "chainId": 167,
         "faucets": [],
         "infoURL": "https://atoshi.org",
         "name": "Atoshi Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "ATOSHI",
@@ -2649,15 +2825,17 @@
         "nativeCurrency": {
             "decimals": 18,
             "name": "Ether",
             "symbol": "ETH"
         },
         "networkId": 169,
         "rpc": [
-            "https://pacific-rpc.manta.network/http"
+            "https://pacific-rpc.manta.network/http",
+            "https://manta-pacific.drpc.org",
+            "wss://manta-pacific.drpc.org"
         ],
         "shortName": "manta"
     },
     {
         "chainId": 170,
         "faucets": [
             "https://faucet-testnet.hscscan.com/"
@@ -2755,14 +2933,30 @@
         "networkId": 189,
         "rpc": [
             "https://testnet.bmcchain.com"
         ],
         "shortName": "BMCT"
     },
     {
+        "chainId": 191,
+        "faucets": [],
+        "infoURL": "https://filefilego.com",
+        "name": "FileFileGo",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "FFG",
+            "symbol": "FFG"
+        },
+        "networkId": 191,
+        "rpc": [
+            "https://rpc.filefilego.com/rpc"
+        ],
+        "shortName": "ffg"
+    },
+    {
         "chainId": 193,
         "faucets": [],
         "infoURL": "https://cemblockchain.com/",
         "name": "Crypto Emergency",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Crypto Emergency",
@@ -2773,41 +2967,45 @@
             "https://cemchain.com"
         ],
         "shortName": "cem"
     },
     {
         "chainId": 195,
         "faucets": [
-            "https://www.oklink.com/okbc-test"
+            "https://www.okx.com/xlayer/faucet"
         ],
-        "infoURL": "https://www.okx.com/okbc/docs/dev/quick-start/introduction/introduction-to-okbchain",
-        "name": "Xgon Testnet",
+        "infoURL": "https://www.okx.com/xlayer",
+        "name": "X Layer Testnet",
         "nativeCurrency": {
             "decimals": 18,
-            "name": "Xgon Global Utility Token in testnet",
+            "name": "X Layer Global Utility Token in testnet",
             "symbol": "OKB"
         },
         "networkId": 195,
         "rpc": [
-            "https://testrpc.xgon.io"
+            "https://testrpc.xlayer.tech",
+            "https://xlayertestrpc.okx.com"
         ],
         "shortName": "tokb"
     },
     {
         "chainId": 196,
         "faucets": [],
-        "infoURL": "https://www.okx.com/okbc/docs/dev/quick-start/introduction/introduction-to-okbchain",
-        "name": "Xgon Mainnet",
+        "infoURL": "https://www.okx.com/xlayer",
+        "name": "X Layer Mainnet",
         "nativeCurrency": {
             "decimals": 18,
-            "name": "Xgon Global Utility Token",
+            "name": "X Layer Global Utility Token",
             "symbol": "OKB"
         },
         "networkId": 196,
-        "rpc": [],
+        "rpc": [
+            "https://rpc.xlayer.tech",
+            "https://xlayerrpc.okx.com"
+        ],
         "shortName": "okb"
     },
     {
         "chainId": 197,
         "faucets": [
             "https://neutrinoschain.com/faucet"
         ],
@@ -2839,24 +3037,26 @@
             "https://rpc.bitchain.biz/"
         ],
         "shortName": "bit"
     },
     {
         "chainId": 199,
         "faucets": [],
-        "infoURL": "https:/bt.io",
+        "infoURL": "https://bt.io",
         "name": "BitTorrent Chain Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "BitTorrent",
             "symbol": "BTT"
         },
         "networkId": 199,
         "rpc": [
-            "https://rpc.bittorrentchain.io/"
+            "https://rpc.bt.io",
+            "https://bittorrent.drpc.org",
+            "wss://bittorrent.drpc.org"
         ],
         "shortName": "BTT"
     },
     {
         "chainId": 200,
         "faucets": [],
         "infoURL": "https://xdaichain.com",
@@ -2885,14 +3085,30 @@
         "networkId": 201,
         "rpc": [
             "https://gateway.moac.io/testnet"
         ],
         "shortName": "moactest"
     },
     {
+        "chainId": 202,
+        "faucets": [],
+        "infoURL": "https://edgeless.network",
+        "name": "Edgeless Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Edgeless Wrapped Eth",
+            "symbol": "EwEth"
+        },
+        "networkId": 202,
+        "rpc": [
+            "https://testnet.rpc.edgeless.network/http"
+        ],
+        "shortName": "edgeless-testnet"
+    },
+    {
         "chainId": 204,
         "faucets": [],
         "infoURL": "https://opbnb.bnbchain.org/en",
         "name": "opBNB Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "BNB Chain Native Token",
@@ -2901,28 +3117,30 @@
         "networkId": 204,
         "rpc": [
             "https://opbnb-mainnet-rpc.bnbchain.org",
             "https://opbnb-mainnet.nodereal.io/v1/64a9df0874fb4a93b9d0a3849de012d3",
             "wss://opbnb-mainnet.nodereal.io/ws/v1/64a9df0874fb4a93b9d0a3849de012d3",
             "https://opbnb-mainnet.nodereal.io/v1/e9a36765eb8a40b9bd12e680a1fd2bc5",
             "wss://opbnb-mainnet.nodereal.io/ws/v1/e9a36765eb8a40b9bd12e680a1fd2bc5",
-            "https://opbnb.publicnode.com",
-            "wss://opbnb.publicnode.com"
+            "https://opbnb-rpc.publicnode.com",
+            "wss://opbnb-rpc.publicnode.com",
+            "https://opbnb.drpc.org",
+            "wss://opbnb.drpc.org"
         ],
         "shortName": "obnb"
     },
     {
         "chainId": 206,
         "faucets": [],
         "infoURL": "https://vitainu.org",
         "name": "VinuChain Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "VinuChain",
-            "symbol": "V\u0421"
+            "symbol": "VC"
         },
         "networkId": 206,
         "rpc": [
             "https://vinufoundation-rpc.com"
         ],
         "shortName": "VCTEST"
     },
@@ -2930,15 +3148,15 @@
         "chainId": 207,
         "faucets": [],
         "infoURL": "https://vitainu.org",
         "name": "VinuChain Network",
         "nativeCurrency": {
             "decimals": 18,
             "name": "VinuChain",
-            "symbol": "V\u0421"
+            "symbol": "VC"
         },
         "networkId": 207,
         "rpc": [
             "https://vinuchain-rpc.com"
         ],
         "shortName": "VC"
     },
@@ -2993,30 +3211,46 @@
             "https://app.freighttrust.net/ftn/${API_KEY}"
         ],
         "shortName": "EDI"
     },
     {
         "chainId": 212,
         "faucets": [
-            "https://faucet.maplabs.io"
+            "https://faucet.mapprotocol.io"
         ],
-        "infoURL": "https://maplabs.io",
-        "name": "MAP Makalu",
+        "infoURL": "https://mapprotocol.io/",
+        "name": "MAPO Makalu",
         "nativeCurrency": {
             "decimals": 18,
-            "name": "Makalu MAP",
-            "symbol": "MAP"
+            "name": "Makalu MAPO",
+            "symbol": "MAPO"
         },
         "networkId": 212,
         "rpc": [
             "https://testnet-rpc.maplabs.io"
         ],
         "shortName": "makalu"
     },
     {
+        "chainId": 213,
+        "faucets": [],
+        "infoURL": "https://www.bsquared.network",
+        "name": "B2 Hub Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "BSquared Token",
+            "symbol": "B2"
+        },
+        "networkId": 213,
+        "rpc": [
+            "https://hub-rpc.bsquared.network"
+        ],
+        "shortName": "B2Hub-mainnet"
+    },
+    {
         "chainId": 214,
         "faucets": [],
         "infoURL": "https://shinarium.org",
         "name": "Shinarium Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Shina Inu",
@@ -3057,14 +3291,32 @@
         "networkId": 218,
         "rpc": [
             "https://rpc.soter.one"
         ],
         "shortName": "SO1-old"
     },
     {
+        "chainId": 220,
+        "faucets": [
+            "https://faucet.scalind.com"
+        ],
+        "infoURL": "https://scalind.com",
+        "name": "Scalind Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Sepolia Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 220,
+        "rpc": [
+            "https://rpc-sepolia.scalind.com"
+        ],
+        "shortName": "sepscal"
+    },
+    {
         "chainId": 222,
         "faucets": [],
         "infoURL": "https://permission.io/",
         "name": "Permission",
         "nativeCurrency": {
             "decimals": 18,
             "name": "ASK",
@@ -3073,14 +3325,51 @@
         "networkId": 2221,
         "rpc": [
             "https://blockchain-api-mainnet.permission.io/rpc"
         ],
         "shortName": "ASK"
     },
     {
+        "chainId": 223,
+        "faucets": [],
+        "infoURL": "https://www.bsquared.network",
+        "name": "B2 Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Bitcoin",
+            "symbol": "BTC"
+        },
+        "networkId": 223,
+        "rpc": [
+            "https://mainnet.b2-rpc.com",
+            "https://rpc.bsquared.network",
+            "https://b2-mainnet.alt.technology",
+            "https://b2-mainnet-public.s.chainbase.com"
+        ],
+        "shortName": "B2-mainnet"
+    },
+    {
+        "chainId": 224,
+        "faucets": [
+            "https://faucet.vrd.network"
+        ],
+        "infoURL": "https://viridis.network",
+        "name": "Viridis Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Viridis Token",
+            "symbol": "VRD"
+        },
+        "networkId": 224,
+        "rpc": [
+            "https://testnet-rpc.vrd.network"
+        ],
+        "shortName": "VRD-Testnet"
+    },
+    {
         "chainId": 225,
         "faucets": [],
         "infoURL": "https://lachain.io",
         "name": "LACHAIN Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "LA",
@@ -3105,14 +3394,31 @@
         "networkId": 226,
         "rpc": [
             "https://rpc-testnet.lachain.io"
         ],
         "shortName": "TLA"
     },
     {
+        "chainId": 228,
+        "faucets": [],
+        "infoURL": "https://mindnetwork.xyz",
+        "name": "Mind Network Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "FHE",
+            "symbol": "FHE"
+        },
+        "networkId": 228,
+        "rpc": [
+            "https://rpc_mainnet.mindnetwork.xyz",
+            "wss://rpc_mainnet.mindnetwork.xyz"
+        ],
+        "shortName": "fhe"
+    },
+    {
         "chainId": 230,
         "faucets": [],
         "infoURL": "https://swapdex.network/",
         "name": "SwapDEX",
         "nativeCurrency": {
             "decimals": 18,
             "name": "SwapDEX",
@@ -3122,14 +3428,32 @@
         "rpc": [
             "https://rpc.swapdex.network",
             "wss://ss.swapdex.network"
         ],
         "shortName": "SDX"
     },
     {
+        "chainId": 234,
+        "faucets": [
+            "https://protojumbo.jumbochain.org/faucet-smart"
+        ],
+        "infoURL": "https://jumbochain.org",
+        "name": "ProtoJumbo Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "JNFTC",
+            "symbol": "JNFTC"
+        },
+        "networkId": 234,
+        "rpc": [
+            "https://testnode.jumbochain.org"
+        ],
+        "shortName": "ProtoJumbo"
+    },
+    {
         "chainId": 236,
         "faucets": [
             "https://faucet.deamchain.com"
         ],
         "infoURL": "https://deamchain.com",
         "name": "Deamchain Testnet",
         "nativeCurrency": {
@@ -3140,14 +3464,30 @@
         "networkId": 236,
         "rpc": [
             "https://testnet.deamchain.com"
         ],
         "shortName": "deamtest"
     },
     {
+        "chainId": 238,
+        "faucets": [],
+        "infoURL": "https://docs.blastblockchain.com",
+        "name": "Blast Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 238,
+        "rpc": [
+            "https://rpc.blastblockchain.com"
+        ],
+        "shortName": "blast"
+    },
+    {
         "chainId": 242,
         "faucets": [],
         "infoURL": "https://www.plinga.technology/",
         "name": "Plinga Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Plinga",
@@ -3203,20 +3543,38 @@
             "decimals": 18,
             "name": "Fantom",
             "symbol": "FTM"
         },
         "networkId": 250,
         "rpc": [
             "https://rpc.ftm.tools",
-            "https://fantom.publicnode.com",
-            "wss://fantom.publicnode.com"
+            "https://fantom-rpc.publicnode.com",
+            "wss://fantom-rpc.publicnode.com",
+            "https://fantom.drpc.org",
+            "wss://fantom.drpc.org"
         ],
         "shortName": "ftm"
     },
     {
+        "chainId": 252,
+        "faucets": [],
+        "infoURL": "https://mainnet.frax.com",
+        "name": "Fraxtal",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Frax Ether",
+            "symbol": "frxETH"
+        },
+        "networkId": 252,
+        "rpc": [
+            "https://rpc.frax.com"
+        ],
+        "shortName": "fraxtal"
+    },
+    {
         "chainId": 255,
         "faucets": [],
         "infoURL": "https://kroma.network",
         "name": "Kroma",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Ether",
@@ -3290,14 +3648,60 @@
         "networkId": 1,
         "rpc": [
             "https://sur.nilin.org"
         ],
         "shortName": "SUR"
     },
     {
+        "chainId": 266,
+        "faucets": [],
+        "infoURL": "https://www.neuraprotocol.io/",
+        "name": "Neura",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ankr",
+            "symbol": "ANKR"
+        },
+        "networkId": 266,
+        "rpc": [],
+        "shortName": "neura"
+    },
+    {
+        "chainId": 267,
+        "faucets": [
+            "https://testnet.neuraprotocol.io/faucet"
+        ],
+        "infoURL": "https://www.neuraprotocol.io/",
+        "name": "Neura Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Testnet Ankr",
+            "symbol": "ANKR"
+        },
+        "networkId": 267,
+        "rpc": [
+            "https://rpc.ankr.com/neura_testnet"
+        ],
+        "shortName": "tneura"
+    },
+    {
+        "chainId": 268,
+        "faucets": [],
+        "infoURL": "https://www.neuraprotocol.io/",
+        "name": "Neura Devnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Devnet Ankr",
+            "symbol": "ANKR"
+        },
+        "networkId": 268,
+        "rpc": [],
+        "shortName": "dneura"
+    },
+    {
         "chainId": 269,
         "faucets": [
             "https://myhpbwallet.com/"
         ],
         "infoURL": "https://hpb.io",
         "name": "High Performance Blockchain",
         "nativeCurrency": {
@@ -3310,17 +3714,15 @@
             "https://hpbnode.com",
             "wss://ws.hpbnode.com"
         ],
         "shortName": "hpb"
     },
     {
         "chainId": 271,
-        "faucets": [
-            "https://faucet.egonscan.com"
-        ],
+        "faucets": [],
         "infoURL": "https://egonscan.com",
         "name": "EgonCoin Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "EgonCoin",
             "symbol": "EGON"
         },
@@ -3345,32 +3747,82 @@
             "https://rpc1.mainnet.lachain.network",
             "https://rpc2.mainnet.lachain.network",
             "https://lachain.rpc-nodes.cedalio.dev"
         ],
         "shortName": "lachain"
     },
     {
-        "chainId": 280,
-        "faucets": [
-            "https://goerli.portal.zksync.io/faucet"
+        "chainId": 278,
+        "faucets": [],
+        "infoURL": "https://xfair.ai",
+        "name": "xFair.AI Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "FAI",
+            "symbol": "FAI"
+        },
+        "networkId": 278,
+        "rpc": [
+            "https://rpc_mainnet.xfair.ai",
+            "wss://rpc_mainnet.xfair.ai"
         ],
-        "infoURL": "https://era.zksync.io/docs/",
-        "name": "zkSync Era Testnet",
+        "shortName": "fai"
+    },
+    {
+        "chainId": 279,
+        "faucets": [],
+        "infoURL": "https://bpxchain.cc",
+        "name": "BPX Blockchain",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "BPX",
+            "symbol": "BPX"
+        },
+        "networkId": 279,
+        "rpc": [
+            "https://rpc.mainnet.bpxchain.cc",
+            "https://bpx-dataseed.infinex.cc"
+        ],
+        "shortName": "bpx"
+    },
+    {
+        "chainId": 280,
+        "faucets": [],
+        "infoURL": "https://zksync.io/",
+        "name": "zkSync Era Goerli Testnet (deprecated)",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Ether",
             "symbol": "ETH"
         },
         "networkId": 280,
         "rpc": [
             "https://testnet.era.zksync.dev"
         ],
         "shortName": "zksync-goerli"
     },
     {
+        "chainId": 282,
+        "faucets": [
+            "https://zkevm-t0.cronos.org/faucet"
+        ],
+        "infoURL": "https://docs.cronos.org/cronos-zkevm-chain/introduction-to-cronos-zkevm-chain-testnet",
+        "name": "Cronos zkEVM Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Cronos zkEVM Test Coin",
+            "symbol": "TCRO"
+        },
+        "networkId": 282,
+        "rpc": [
+            "https://rpc-zkevm-t0.cronos.org"
+        ],
+        "shortName": "zktcro"
+    },
+    {
         "chainId": 288,
         "faucets": [],
         "infoURL": "https://boba.network",
         "name": "Boba Network",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Ether",
@@ -3379,15 +3831,17 @@
         "networkId": 288,
         "rpc": [
             "https://mainnet.boba.network",
             "https://replica.boba.network",
             "https://boba-ethereum.gateway.tenderly.co",
             "https://gateway.tenderly.co/public/boba-ethereum",
             "wss://boba-ethereum.gateway.tenderly.co/",
-            "wss://gateway.tenderly.co/public/boba-ethereum"
+            "wss://gateway.tenderly.co/public/boba-ethereum",
+            "https://boba-eth.drpc.org",
+            "wss://boba-eth.drpc.org"
         ],
         "shortName": "Boba"
     },
     {
         "chainId": 291,
         "faucets": [],
         "infoURL": "www.orderly.network",
@@ -3469,24 +3923,28 @@
         "networkId": 298,
         "rpc": [],
         "shortName": "hedera-localnet"
     },
     {
         "chainId": 300,
         "faucets": [],
-        "infoURL": "https://docs.gnosischain.com",
-        "name": "(deprecated) Optimism on GC",
+        "infoURL": "https://zksync.io/",
+        "name": "zkSync Sepolia Testnet",
         "nativeCurrency": {
             "decimals": 18,
-            "name": "xDAI",
-            "symbol": "xDAI"
+            "name": "Ether",
+            "symbol": "ETH"
         },
         "networkId": 300,
-        "rpc": [],
-        "shortName": "ogc"
+        "rpc": [
+            "https://sepolia.era.zksync.dev",
+            "https://zksync-sepolia.drpc.org",
+            "wss://zksync-sepolia.drpc.org"
+        ],
+        "shortName": "zksync-sepolia"
     },
     {
         "chainId": 301,
         "faucets": [],
         "infoURL": "https://boba.network",
         "name": "Bobaopera",
         "nativeCurrency": {
@@ -3500,14 +3958,30 @@
             "wss://wss.bobaopera.boba.network",
             "https://replica.bobaopera.boba.network",
             "wss://replica-wss.bobaopera.boba.network"
         ],
         "shortName": "Bobaopera"
     },
     {
+        "chainId": 302,
+        "faucets": [],
+        "infoURL": "https://zkcandy.io/",
+        "name": "zkCandy Sepolia Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 302,
+        "rpc": [
+            "https://sepolia.rpc.zkcandy.io"
+        ],
+        "shortName": "zkcandy-sepolia"
+    },
+    {
         "chainId": 303,
         "faucets": [],
         "infoURL": "https://www.neurochain.ai",
         "name": "Neurochain Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Neurochain",
@@ -3516,14 +3990,64 @@
         "networkId": 303,
         "rpc": [
             "https://nc-rpc-test1.neurochain.io"
         ],
         "shortName": "ncnt"
     },
     {
+        "chainId": 305,
+        "faucets": [],
+        "infoURL": "https://zksats.io",
+        "name": "ZKSats Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "BTC",
+            "symbol": "BTC"
+        },
+        "networkId": 305,
+        "rpc": [
+            "https://mainnet.zksats.io"
+        ],
+        "shortName": "ZKSats-Mainnet"
+    },
+    {
+        "chainId": 307,
+        "faucets": [
+            "https://faucet.lovely.network"
+        ],
+        "infoURL": "https://lovely.network",
+        "name": "Lovely Network Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Lovely",
+            "symbol": "LOVELY"
+        },
+        "networkId": 307,
+        "rpc": [
+            "https://trpc.lovely.network"
+        ],
+        "shortName": "LOVELY-Testnet"
+    },
+    {
+        "chainId": 308,
+        "faucets": [],
+        "infoURL": "https://furtheon.org/",
+        "name": "Furtheon",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Furtheon",
+            "symbol": "FTH"
+        },
+        "networkId": 308,
+        "rpc": [
+            "https://rpc.furtheon.org"
+        ],
+        "shortName": "furtheon"
+    },
+    {
         "chainId": 309,
         "faucets": [],
         "infoURL": "https://wyzth.org/",
         "name": "Wyzth Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Wyzth",
@@ -3581,15 +4105,17 @@
             "symbol": "FIL"
         },
         "networkId": 314,
         "rpc": [
             "https://api.node.glif.io/",
             "https://rpc.ankr.com/filecoin",
             "https://filecoin-mainnet.chainstacklabs.com/rpc/v1",
-            "https://filfox.info/rpc/v1"
+            "https://filfox.info/rpc/v1",
+            "https://filecoin.drpc.org",
+            "wss://filecoin.drpc.org"
         ],
         "shortName": "filecoin"
     },
     {
         "chainId": 321,
         "faucets": [],
         "infoURL": "https://kcc.io",
@@ -3622,26 +4148,44 @@
         "networkId": 322,
         "rpc": [
             "https://rpc-testnet.kcc.network"
         ],
         "shortName": "kcst"
     },
     {
+        "chainId": 323,
+        "faucets": [],
+        "infoURL": "https://cosvm.network",
+        "name": "Cosvm Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Cosvm",
+            "symbol": "CVM"
+        },
+        "networkId": 323,
+        "rpc": [
+            "https://rpc.cosvm.net"
+        ],
+        "shortName": "cvm"
+    },
+    {
         "chainId": 324,
         "faucets": [],
         "infoURL": "https://zksync.io/",
-        "name": "zkSync Era Mainnet",
+        "name": "zkSync Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Ether",
             "symbol": "ETH"
         },
         "networkId": 324,
         "rpc": [
-            "https://mainnet.era.zksync.io"
+            "https://mainnet.era.zksync.io",
+            "https://zksync.drpc.org",
+            "wss://zksync.drpc.org"
         ],
         "shortName": "zksync"
     },
     {
         "chainId": 333,
         "faucets": [],
         "infoURL": "https://web3q.io/home.w3q/",
@@ -3704,35 +4248,21 @@
         "nativeCurrency": {
             "decimals": 18,
             "name": "Cronos Test Coin",
             "symbol": "TCRO"
         },
         "networkId": 338,
         "rpc": [
-            "https://evm-t3.cronos.org"
+            "https://evm-t3.cronos.org",
+            "https://cronos-testnet.drpc.org",
+            "wss://cronos-testnet.drpc.org"
         ],
         "shortName": "tcro"
     },
     {
-        "chainId": 345,
-        "faucets": [],
-        "infoURL": "https://yooldo.gg/",
-        "name": "Yooldo Verse Mainnet",
-        "nativeCurrency": {
-            "decimals": 18,
-            "name": "OAS",
-            "symbol": "OAS"
-        },
-        "networkId": 345,
-        "rpc": [
-            "https://rpc.yooldo-verse.xyz/"
-        ],
-        "shortName": "YVM"
-    },
-    {
         "chainId": 361,
         "faucets": [],
         "infoURL": "https://www.thetatoken.org/",
         "name": "Theta Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Theta Fuel",
@@ -3802,16 +4332,16 @@
             "name": "Pulse",
             "symbol": "PLS"
         },
         "networkId": 369,
         "rpc": [
             "https://rpc.pulsechain.com",
             "wss://rpc.pulsechain.com",
-            "https://pulsechain.publicnode.com",
-            "wss://pulsechain.publicnode.com",
+            "https://pulsechain-rpc.publicnode.com",
+            "wss://pulsechain-rpc.publicnode.com",
             "https://rpc-pulsechain.g4mm4.io",
             "wss://rpc-pulsechain.g4mm4.io"
         ],
         "shortName": "pls"
     },
     {
         "chainId": 371,
@@ -3826,14 +4356,47 @@
         "networkId": 371,
         "rpc": [
             "https://rpc-testnet.theconsta.com"
         ],
         "shortName": "tCNT"
     },
     {
+        "chainId": 380,
+        "faucets": [],
+        "infoURL": "https://testnet.zkamoeba.com",
+        "name": "ZKAmoeba Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "filecoin",
+            "symbol": "FIL"
+        },
+        "networkId": 380,
+        "rpc": [
+            "https://rpc.testnet.zkamoeba.com:4050/",
+            "https://rpc1.testnet.zkamoeba.com:4050/"
+        ],
+        "shortName": "zkamoeba-test"
+    },
+    {
+        "chainId": 381,
+        "faucets": [],
+        "infoURL": "https://www.zkamoeba.com",
+        "name": "ZKAmoeba Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "filecoin",
+            "symbol": "FIL"
+        },
+        "networkId": 381,
+        "rpc": [
+            "https://rpc.mainnet.zkamoeba.com/rpc"
+        ],
+        "shortName": "zkamoeba"
+    },
+    {
         "chainId": 385,
         "faucets": [
             "https://pipa.lisinski.online"
         ],
         "infoURL": "https://lisinski.online",
         "name": "Lisinski",
         "nativeCurrency": {
@@ -3844,14 +4407,60 @@
         "networkId": 385,
         "rpc": [
             "https://rpc-bitfalls1.lisinski.online"
         ],
         "shortName": "lisinski"
     },
     {
+        "chainId": 395,
+        "faucets": [
+            "https://faucet.testnet.camdl.gov.kh/"
+        ],
+        "infoURL": "https://camdl.gov.kh/",
+        "name": "CamDL Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "CADL",
+            "symbol": "CADL"
+        },
+        "networkId": 395,
+        "rpc": [
+            "https://rpc1.testnet.camdl.gov.kh/"
+        ],
+        "shortName": "camdl-testnet"
+    },
+    {
+        "chainId": 397,
+        "faucets": [],
+        "infoURL": "https://near.org/",
+        "name": "Near Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "NEAR",
+            "symbol": "NEAR"
+        },
+        "networkId": 397,
+        "rpc": [],
+        "shortName": "near"
+    },
+    {
+        "chainId": 398,
+        "faucets": [],
+        "infoURL": "https://aurora.dev",
+        "name": "Near Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Testnet NEAR",
+            "symbol": "NEAR"
+        },
+        "networkId": 398,
+        "rpc": [],
+        "shortName": "near-testnet"
+    },
+    {
         "chainId": 399,
         "faucets": [],
         "infoURL": "https://nativ3.network",
         "name": "Nativ3 Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "USNT",
@@ -3895,14 +4504,31 @@
         "networkId": 401,
         "rpc": [
             "https://node1.testnet.ozonechain.io"
         ],
         "shortName": "ozo_tst"
     },
     {
+        "chainId": 404,
+        "faucets": [],
+        "infoURL": "https://syndr.com",
+        "name": "Syndr L3",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 404,
+        "rpc": [
+            "https://rpc.syndr.com",
+            "wss://rpc.syndr.com/ws"
+        ],
+        "shortName": "syndr-l3"
+    },
+    {
         "chainId": 411,
         "faucets": [],
         "infoURL": "https://pepe-chain.vip",
         "name": "Pepe Chain Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Pepe",
@@ -3958,22 +4584,40 @@
             "decimals": 18,
             "name": "Goerli Ether",
             "symbol": "ETH"
         },
         "networkId": 420,
         "rpc": [
             "https://goerli.optimism.io",
-            "https://optimism-goerli.publicnode.com",
-            "wss://optimism-goerli.publicnode.com",
+            "https://optimism-goerli-rpc.publicnode.com",
+            "wss://optimism-goerli-rpc.publicnode.com",
             "https://optimism-goerli.gateway.tenderly.co",
-            "wss://optimism-goerli.gateway.tenderly.co"
+            "wss://optimism-goerli.gateway.tenderly.co",
+            "https://optimism-testnet.drpc.org",
+            "wss://optimism-testnet.drpc.org"
         ],
         "shortName": "ogor"
     },
     {
+        "chainId": 422,
+        "faucets": [],
+        "infoURL": "https://viridis.network",
+        "name": "Viridis Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Viridis Token",
+            "symbol": "VRD"
+        },
+        "networkId": 422,
+        "rpc": [
+            "https://mainnet-rpc.vrd.network"
+        ],
+        "shortName": "vrd"
+    },
+    {
         "chainId": 424,
         "faucets": [],
         "infoURL": "https://publicgoods.network/",
         "name": "PGN (Public Goods Network)",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Ether",
@@ -3998,28 +4642,60 @@
         "networkId": 427,
         "rpc": [
             "https://rpc.zeeth.io"
         ],
         "shortName": "zeeth"
     },
     {
+        "chainId": 428,
+        "faucets": [],
+        "infoURL": "https://gesoten.com/",
+        "name": "Geso Verse",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "OAS",
+            "symbol": "OAS"
+        },
+        "networkId": 428,
+        "rpc": [
+            "https://rpc.verse.gesoten.com/"
+        ],
+        "shortName": "GSV"
+    },
+    {
+        "chainId": 434,
+        "faucets": [],
+        "infoURL": "https://boyaa.network",
+        "name": "Boyaa Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Boyaa mainnet native coin",
+            "symbol": "BYC"
+        },
+        "networkId": 434,
+        "rpc": [
+            "https://evm-rpc.mainnet.boyaa.network"
+        ],
+        "shortName": "BYC"
+    },
+    {
         "chainId": 443,
         "faucets": [],
-        "infoURL": "https://obscu.ro",
-        "name": "Obscuro Testnet",
+        "infoURL": "https://ten.xyz",
+        "name": "Ten Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Sepolia Ether",
             "symbol": "ETH"
         },
         "networkId": 443,
         "rpc": [
-            "https://testnet.obscu.ro"
+            "https://testnet.ten.xyz"
         ],
-        "shortName": "obs-testnet"
+        "shortName": "ten-testnet"
     },
     {
         "chainId": 444,
         "faucets": [],
         "infoURL": "https://synapseprotocol.com",
         "name": "Synapse Chain Testnet",
         "nativeCurrency": {
@@ -4057,22 +4733,46 @@
         "nativeCurrency": {
             "decimals": 18,
             "name": "Areon",
             "symbol": "TAREA"
         },
         "networkId": 462,
         "rpc": [
-            "https://testnet-rpc.areon.network"
+            "https://testnet-rpc.areon.network",
+            "https://testnet-rpc2.areon.network",
+            "https://testnet-rpc3.areon.network",
+            "https://testnet-rpc4.areon.network",
+            "https://testnet-rpc5.areon.network"
         ],
         "shortName": "tarea"
     },
     {
+        "chainId": 463,
+        "faucets": [],
+        "infoURL": "https://areon.network",
+        "name": "Areon Network Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Areon",
+            "symbol": "AREA"
+        },
+        "networkId": 463,
+        "rpc": [
+            "https://mainnet-rpc.areon.network",
+            "https://mainnet-rpc2.areon.network",
+            "https://mainnet-rpc3.areon.network",
+            "https://mainnet-rpc4.areon.network",
+            "https://mainnet-rpc5.areon.network"
+        ],
+        "shortName": "area"
+    },
+    {
         "chainId": 499,
         "faucets": [],
-        "infoURL": "https://www.rupx.io",
+        "infoURL": "https://www.rupaya.io",
         "name": "Rupaya",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Rupaya",
             "symbol": "RUPX"
         },
         "networkId": 499,
@@ -4108,14 +4808,30 @@
         "networkId": 1001,
         "rpc": [
             "https://columbus.camino.network/ext/bc/C/rpc"
         ],
         "shortName": "Columbus"
     },
     {
+        "chainId": 510,
+        "faucets": [],
+        "infoURL": "https://syndicate.io",
+        "name": "Syndicate Chain",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 510,
+        "rpc": [
+            "https://rpc-mainnet.syndicate.io"
+        ],
+        "shortName": "syndicate-chain-mainnet"
+    },
+    {
         "chainId": 512,
         "faucets": [],
         "infoURL": "https://www.acuteangle.com/",
         "name": "Double-A Chain Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Acuteangle Native Token",
@@ -4189,15 +4905,15 @@
         "nativeCurrency": {
             "decimals": 18,
             "name": "Firechain",
             "symbol": "FIRE"
         },
         "networkId": 529,
         "rpc": [
-            "https://mainnet.rpc1.thefirechain.com"
+            "https://rpc-mainnet.thefirechain.com"
         ],
         "shortName": "fire"
     },
     {
         "chainId": 530,
         "faucets": [],
         "infoURL": "https://functionx.io/",
@@ -4227,14 +4943,30 @@
         "rpc": [
             "https://candle-rpc.com/",
             "https://rpc.cndlchain.com"
         ],
         "shortName": "CNDL"
     },
     {
+        "chainId": 537,
+        "faucets": [],
+        "infoURL": "https://optrust.io",
+        "name": "OpTrust Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "BSC",
+            "symbol": "BNB"
+        },
+        "networkId": 537,
+        "rpc": [
+            "https://rpc.optrust.io"
+        ],
+        "shortName": "optrust"
+    },
+    {
         "chainId": 542,
         "faucets": [],
         "infoURL": "https://pawchainx.com/",
         "name": "PAWCHAIN Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "PAW",
@@ -4243,14 +4975,32 @@
         "networkId": 542,
         "rpc": [
             "https://pawchainx.com/"
         ],
         "shortName": "PAW"
     },
     {
+        "chainId": 545,
+        "faucets": [
+            "https://testnet-faucet.onflow.org"
+        ],
+        "infoURL": "https://developers.flow.com/evm/about",
+        "name": "Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "FLOW",
+            "symbol": "FLOW"
+        },
+        "networkId": 545,
+        "rpc": [
+            "https://testnet.evm.nodes.onflow.org"
+        ],
+        "shortName": "flow-testnet"
+    },
+    {
         "chainId": 555,
         "faucets": [],
         "infoURL": "https://velaverse.io",
         "name": "Vela1 Chain Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "CLASS COIN",
@@ -4310,20 +5060,53 @@
             "decimals": 18,
             "name": "Syscoin",
             "symbol": "SYS"
         },
         "networkId": 570,
         "rpc": [
             "https://rpc.rollux.com",
-            "https://rollux.public-rpc.com",
-            "wss://rpc.rollux.com/wss"
+            "wss://rpc.rollux.com/wss",
+            "https://rollux.rpc.syscoin.org",
+            "wss://rollux.rpc.syscoin.org/wss"
         ],
         "shortName": "sys-rollux"
     },
     {
+        "chainId": 571,
+        "faucets": [],
+        "infoURL": "https://metatime.com/en",
+        "name": "MetaChain Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Metatime Coin",
+            "symbol": "MTC"
+        },
+        "networkId": 571,
+        "rpc": [
+            "https://rpc.metatime.com"
+        ],
+        "shortName": "metatime"
+    },
+    {
+        "chainId": 579,
+        "faucets": [],
+        "infoURL": "https://filenova.org",
+        "name": "Filenova Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Filecoin",
+            "symbol": "FIL"
+        },
+        "networkId": 579,
+        "rpc": [
+            "https://rpc.filenova.org"
+        ],
+        "shortName": "filenova"
+    },
+    {
         "chainId": 588,
         "faucets": [],
         "infoURL": "https://www.metis.io",
         "name": "Metis Stardust Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "tMetis",
@@ -4433,28 +5216,44 @@
         "networkId": 600,
         "rpc": [],
         "shortName": "mesh-chain-testnet"
     },
     {
         "chainId": 601,
         "faucets": [
-            "https://testnet.peer.inc"
+            "https://vne.network/rose"
         ],
-        "infoURL": "https://peer.inc",
-        "name": "PEER Testnet",
+        "infoURL": "https://www.peer.inc",
+        "name": "Vine Testnet",
         "nativeCurrency": {
             "decimals": 18,
-            "name": "PEER Token",
-            "symbol": "PEER"
+            "name": "VINE",
+            "symbol": "VNE"
         },
         "networkId": 601,
         "rpc": [
-            "http://testnet-polka-host-232813573.us-west-1.elb.amazonaws.com"
+            "https://rpc-testnet.vne.network"
         ],
-        "shortName": "PEER"
+        "shortName": "VINE"
+    },
+    {
+        "chainId": 612,
+        "faucets": [],
+        "infoURL": "",
+        "name": "EIOB Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "EIOB",
+            "symbol": "EIOB"
+        },
+        "networkId": 612,
+        "rpc": [
+            "https://rpc.eiob.xyz"
+        ],
+        "shortName": "eiob"
     },
     {
         "chainId": 614,
         "faucets": [],
         "infoURL": "https://graphlinq.io",
         "name": "Graphlinq Blockchain Mainnet",
         "nativeCurrency": {
@@ -4481,14 +5280,32 @@
         "networkId": 634,
         "rpc": [
             "https://rpc.avocado.instadapp.io"
         ],
         "shortName": "avocado"
     },
     {
+        "chainId": 646,
+        "faucets": [
+            "https://previewnet-faucet.onflow.org"
+        ],
+        "infoURL": "https://developers.flow.com/evm/about",
+        "name": "Previewnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "FLOW",
+            "symbol": "FLOW"
+        },
+        "networkId": 646,
+        "rpc": [
+            "https://previewnet.evm.nodes.onflow.org"
+        ],
+        "shortName": "flow-previewnet"
+    },
+    {
         "chainId": 647,
         "faucets": [
             "https://faucet.toronto.sx.technology"
         ],
         "infoURL": "https://www.sx.technology",
         "name": "SX Network Testnet",
         "nativeCurrency": {
@@ -4515,14 +5332,62 @@
         "networkId": 648,
         "rpc": [
             "https://rpc-endurance.fusionist.io/"
         ],
         "shortName": "ace"
     },
     {
+        "chainId": 653,
+        "faucets": [],
+        "infoURL": "https://kalichain.com",
+        "name": "Kalichain Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "kalis",
+            "symbol": "KALIS"
+        },
+        "networkId": 653,
+        "rpc": [
+            "https://rpc.kalichain.com"
+        ],
+        "shortName": "kalichain"
+    },
+    {
+        "chainId": 654,
+        "faucets": [],
+        "infoURL": "https://kalichain.com",
+        "name": "Kalichain",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "kalis",
+            "symbol": "KALIS"
+        },
+        "networkId": 654,
+        "rpc": [
+            "https://mainnet.kalichain.com"
+        ],
+        "shortName": "kalichainMainnet"
+    },
+    {
+        "chainId": 662,
+        "faucets": [],
+        "infoURL": "https://ultronsmartchain.io",
+        "name": "UltronSmartchain",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "ulc",
+            "symbol": "ULC"
+        },
+        "networkId": 662,
+        "rpc": [
+            "https://rpc.ultronsmartchain.io"
+        ],
+        "shortName": "ultronsmartchain"
+    },
+    {
         "chainId": 666,
         "faucets": [
             "https://chain.pixie.xyz/faucet"
         ],
         "infoURL": "https://scan-testnet.chain.pixie.xyz",
         "name": "Pixie Chain Testnet",
         "nativeCurrency": {
@@ -4603,14 +5468,31 @@
         "rpc": [
             "https://eth-rpc-karura.aca-api.network",
             "wss://eth-rpc-karura.aca-api.network"
         ],
         "shortName": "kar"
     },
     {
+        "chainId": 690,
+        "faucets": [],
+        "infoURL": "https://redstone.xyz",
+        "name": "Redstone",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 690,
+        "rpc": [
+            "https://rpc.redstonechain.com",
+            "wss://rpc.redstonechain.com"
+        ],
+        "shortName": "redstone"
+    },
+    {
         "chainId": 700,
         "faucets": [],
         "infoURL": "https://info.avastar.cc",
         "name": "Star Social Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Social",
@@ -4672,14 +5554,33 @@
         "rpc": [
             "https://highbury.furya.io",
             "https://rest.furya.io"
         ],
         "shortName": "fury"
     },
     {
+        "chainId": 713,
+        "faucets": [],
+        "infoURL": "https://vrccoin.com",
+        "name": "Vrcscan Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "VRC Chain",
+            "symbol": "VRC"
+        },
+        "networkId": 713,
+        "rpc": [
+            "https://rpc-mainnet-5.vrcscan.com",
+            "https://rpc-mainnet-6.vrcscan.com",
+            "https://rpc-mainnet-7.vrcscan.com",
+            "https://rpc-mainnet-8.vrcscan.com"
+        ],
+        "shortName": "vrc"
+    },
+    {
         "chainId": 719,
         "faucets": [],
         "infoURL": "https://beta.shibariumtech.com",
         "name": "Shibarium Beta",
         "nativeCurrency": {
             "decimals": 18,
             "name": "BONE",
@@ -4704,14 +5605,46 @@
         "networkId": 721,
         "rpc": [
             "https://rpc.lycanchain.com/"
         ],
         "shortName": "LYC"
     },
     {
+        "chainId": 727,
+        "faucets": [],
+        "infoURL": "https://www.blucrates.com",
+        "name": "Blucrates",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Blucrates",
+            "symbol": "BLU"
+        },
+        "networkId": 727,
+        "rpc": [
+            "https://data.bluchain.pro"
+        ],
+        "shortName": "blu"
+    },
+    {
+        "chainId": 730,
+        "faucets": [],
+        "infoURL": "https://lovely.network",
+        "name": "Lovely Network Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Lovely",
+            "symbol": "LOVELY"
+        },
+        "networkId": 730,
+        "rpc": [
+            "https://rpc.lovely.network"
+        ],
+        "shortName": "LOVELY"
+    },
+    {
         "chainId": 740,
         "faucets": [],
         "infoURL": "https://canto.io",
         "name": "Canto Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Canto",
@@ -4754,14 +5687,30 @@
         "networkId": 742,
         "rpc": [
             "https://testeth-rpc-api.script.tv/rpc"
         ],
         "shortName": "SPAY"
     },
     {
+        "chainId": 747,
+        "faucets": [],
+        "infoURL": "https://developers.flow.com/evm/about",
+        "name": "Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "FLOW",
+            "symbol": "FLOW"
+        },
+        "networkId": 747,
+        "rpc": [
+            "https://mainnet.evm.nodes.onflow.org"
+        ],
+        "shortName": "flow-mainnet"
+    },
+    {
         "chainId": 766,
         "faucets": [],
         "infoURL": "https://qom.one",
         "name": "QL1",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Shiba Predator",
@@ -4871,14 +5820,32 @@
         "networkId": 789,
         "rpc": [
             "https://rpc.patex.io/"
         ],
         "shortName": "peth"
     },
     {
+        "chainId": 799,
+        "faucets": [
+            "https://faucet.testnet.rupaya.io"
+        ],
+        "infoURL": "https://www.rupaya.io",
+        "name": "Rupaya Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Test Rupaya",
+            "symbol": "TRUPX"
+        },
+        "networkId": 799,
+        "rpc": [
+            "https://rpc.testnet.rupaya.io"
+        ],
+        "shortName": "RupayaTestnet"
+    },
+    {
         "chainId": 800,
         "faucets": [
             "https://faucet.lucidcoin.io"
         ],
         "infoURL": "https://lucidcoin.io",
         "name": "Lucid Blockchain",
         "nativeCurrency": {
@@ -4921,39 +5888,71 @@
         "networkId": 808,
         "rpc": [
             "https://subnets.avax.network/portal-fantasy/testnet/rpc"
         ],
         "shortName": "PFTEST"
     },
     {
+        "chainId": 810,
+        "faucets": [
+            "https://www.haven1.org/faucet"
+        ],
+        "infoURL": "https://www.haven1.org",
+        "name": "Haven1 Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Haven1",
+            "symbol": "H1"
+        },
+        "networkId": 810,
+        "rpc": [
+            "https://testnet-rpc.haven1.org"
+        ],
+        "shortName": "h1"
+    },
+    {
         "chainId": 813,
         "faucets": [],
         "infoURL": "https://github.com/Qitmeer",
-        "name": "Qitmeer",
+        "name": "Qitmeer Network Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Qitmeer",
             "symbol": "MEER"
         },
         "networkId": 813,
         "rpc": [
             "https://evm-dataseed1.meerscan.io",
             "https://evm-dataseed2.meerscan.io",
             "https://evm-dataseed3.meerscan.io",
             "https://evm-dataseed.meerscan.com",
-            "https://evm-dataseed1.meerscan.com",
-            "https://evm-dataseed2.meerscan.com",
             "https://qng.rpc.qitmeer.io",
             "https://mainnet.meerlabs.com",
             "https://rpc.dimai.ai",
             "https://rpc.woowow.io"
         ],
         "shortName": "meer"
     },
     {
+        "chainId": 814,
+        "faucets": [],
+        "infoURL": "https://docs.thefirechain.com/",
+        "name": "Firechain zkEVM",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 814,
+        "rpc": [
+            "https://rpc-zkevm.thefirechain.com"
+        ],
+        "shortName": "firechan-zkEVM"
+    },
+    {
         "chainId": 818,
         "faucets": [],
         "infoURL": "https://beonechain.com",
         "name": "BeOne Chain Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "BeOne Chain Mainnet",
@@ -4997,14 +5996,48 @@
             "symbol": "TCLO"
         },
         "networkId": 2,
         "rpc": [],
         "shortName": "tclo"
     },
     {
+        "chainId": 822,
+        "faucets": [
+            "https://faucet.runic.build"
+        ],
+        "infoURL": "https://runic.build",
+        "name": "Runic Chain Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Bitcoin",
+            "symbol": "rBTC"
+        },
+        "networkId": 822,
+        "rpc": [
+            "https://rpc-testnet.runic.build"
+        ],
+        "shortName": "runic-testnet"
+    },
+    {
+        "chainId": 831,
+        "faucets": [],
+        "infoURL": "https://checkdot.io",
+        "name": "CheckDot Blockchain Devnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "CDT",
+            "symbol": "CDT"
+        },
+        "networkId": 831,
+        "rpc": [
+            "https://devnet.checkdot.io"
+        ],
+        "shortName": "cdt"
+    },
+    {
         "chainId": 841,
         "faucets": [],
         "infoURL": "https://taraxa.io",
         "name": "Taraxa Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Tara",
@@ -5129,14 +6162,32 @@
         "networkId": 888,
         "rpc": [
             "https://gwan-ssl.wandevs.org:56891/"
         ],
         "shortName": "wan"
     },
     {
+        "chainId": 898,
+        "faucets": [
+            "https://faucet.maxi.network"
+        ],
+        "infoURL": "https://maxi.network",
+        "name": "MAXI Chain Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "MAXICOIN",
+            "symbol": "MAXI"
+        },
+        "networkId": 898,
+        "rpc": [
+            "https://rpc-testnet.maxi.network"
+        ],
+        "shortName": "maxi-testnet"
+    },
+    {
         "chainId": 900,
         "faucets": [
             "https://faucet-testnet.garizon.com"
         ],
         "infoURL": "https://garizon.com",
         "name": "Garizon Testnet Stage0",
         "nativeCurrency": {
@@ -5231,28 +6282,44 @@
         "networkId": 910,
         "rpc": [
             "https://layer1test.decentrabone.com"
         ],
         "shortName": "DBONE"
     },
     {
+        "chainId": 911,
+        "faucets": [],
+        "infoURL": "https://taprootchain.io",
+        "name": "TAPROOT Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "TBTC",
+            "symbol": "TBTC"
+        },
+        "networkId": 911,
+        "rpc": [
+            "https://rpc.taprootchain.io"
+        ],
+        "shortName": "TAPROOT-Mainnet"
+    },
+    {
         "chainId": 917,
         "faucets": [
             "https://faucet.thefirechain.com"
         ],
         "infoURL": "https://thefirechain.com",
         "name": "Rinia Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Firechain",
             "symbol": "FIRE"
         },
         "networkId": 917,
         "rpc": [
-            "https://rinia.rpc1.thefirechain.com"
+            "https://rinia-rpc1.thefirechain.com"
         ],
         "shortName": "tfire"
     },
     {
         "chainId": 919,
         "faucets": [
             "https://sepoliafaucet.com/"
@@ -5355,16 +6422,16 @@
             "name": "Test Pulse",
             "symbol": "tPLS"
         },
         "networkId": 943,
         "rpc": [
             "https://rpc.v4.testnet.pulsechain.com",
             "wss://rpc.v4.testnet.pulsechain.com",
-            "https://pulsechain-testnet.publicnode.com",
-            "wss://pulsechain-testnet.publicnode.com",
+            "https://pulsechain-testnet-rpc.publicnode.com",
+            "wss://pulsechain-testnet-rpc.publicnode.com",
             "https://rpc-testnet-pulsechain.g4mm4.io",
             "wss://rpc-testnet-pulsechain.g4mm4.io"
         ],
         "shortName": "t4pls"
     },
     {
         "chainId": 956,
@@ -5377,14 +6444,30 @@
             "symbol": "ETH"
         },
         "networkId": 956,
         "rpc": [],
         "shortName": "munode"
     },
     {
+        "chainId": 957,
+        "faucets": [],
+        "infoURL": "https://lyra.finance",
+        "name": "Lyra Chain",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 957,
+        "rpc": [
+            "https://rpc.lyra.finance"
+        ],
+        "shortName": "lyra"
+    },
+    {
         "chainId": 963,
         "faucets": [],
         "infoURL": "https://bitcoincode.technology",
         "name": "BTC20 Smart Chain",
         "nativeCurrency": {
             "decimals": 18,
             "name": "BTCC",
@@ -5400,19 +6483,19 @@
         "chainId": 970,
         "faucets": [],
         "infoURL": "https://oortech.com",
         "name": "Oort Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Oort",
-            "symbol": "CCN"
+            "symbol": "OORT"
         },
         "networkId": 970,
         "rpc": [
-            "https://rpc.oortech.com"
+            "https://mainnet-rpc.oortech.com"
         ],
         "shortName": "ccn"
     },
     {
         "chainId": 971,
         "faucets": [],
         "infoURL": "https://oortech.com",
@@ -5458,14 +6541,30 @@
         "rpc": [
             "https://api.nepalblockchain.dev",
             "https://api.nepalblockchain.network"
         ],
         "shortName": "yeti"
     },
     {
+        "chainId": 979,
+        "faucets": [],
+        "infoURL": "https://ethxy.com",
+        "name": "EthXY Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Settled EthXY Token",
+            "symbol": "SEXY"
+        },
+        "networkId": 979,
+        "rpc": [
+            "https://rpc.testnet.ethxy.com"
+        ],
+        "shortName": "sexyTestnet"
+    },
+    {
         "chainId": 980,
         "faucets": [],
         "infoURL": "https://www.topnetwork.org/",
         "name": "TOP Mainnet EVM",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Ether",
@@ -5597,23 +6696,24 @@
         "shortName": "gton"
     },
     {
         "chainId": 1001,
         "faucets": [
             "https://baobab.wallet.klaytn.com/access?next=faucet"
         ],
-        "infoURL": "https://www.klaytn.com/",
+        "infoURL": "https://klaytn.foundation",
         "name": "Klaytn Testnet Baobab",
         "nativeCurrency": {
             "decimals": 18,
             "name": "KLAY",
             "symbol": "KLAY"
         },
         "networkId": 1001,
         "rpc": [
+            "https://public-en-baobab.klaytn.net",
             "https://api.baobab.klaytn.net:8651"
         ],
         "shortName": "Baobab"
     },
     {
         "chainId": 1003,
         "faucets": [],
@@ -5675,14 +6775,30 @@
         "networkId": 1008,
         "rpc": [
             "https://mainnet.eurus.network/"
         ],
         "shortName": "eun"
     },
     {
+        "chainId": 1009,
+        "faucets": [],
+        "infoURL": "https://jumbochain.org",
+        "name": "Jumbochain Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "JNFTC",
+            "symbol": "JNFTC"
+        },
+        "networkId": 1009,
+        "rpc": [
+            "https://rpcpriv.jumbochain.org"
+        ],
+        "shortName": "Jumboscan"
+    },
+    {
         "chainId": 1010,
         "faucets": [],
         "infoURL": "https://evrice.com",
         "name": "Evrice Network",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Evrice",
@@ -5691,14 +6807,30 @@
         "networkId": 1010,
         "rpc": [
             "https://meta.evrice.com"
         ],
         "shortName": "EVC"
     },
     {
+        "chainId": 1011,
+        "faucets": [],
+        "infoURL": "https://www.rebuschain.com",
+        "name": "Rebus Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Rebus",
+            "symbol": "REBUS"
+        },
+        "networkId": 1011,
+        "rpc": [
+            "https://apievm.rebuschain.com/rpc"
+        ],
+        "shortName": "rebus"
+    },
+    {
         "chainId": 1012,
         "faucets": [],
         "infoURL": "https://www.newtonproject.org/",
         "name": "Newton",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Newton",
@@ -5854,27 +6986,62 @@
     {
         "chainId": 1072,
         "faucets": [
             "https://evm-toolkit.evm.testnet.shimmer.network",
             "https://evm-faucet.testnet.shimmer.network"
         ],
         "infoURL": "https://shimmer.network",
-        "name": "ShimmerEVM Testnet",
+        "name": "ShimmerEVM Testnet Deprecated 1072",
         "nativeCurrency": {
             "decimals": 6,
             "name": "SMR",
             "symbol": "SMR"
         },
         "networkId": 1072,
+        "rpc": [],
+        "shortName": "shimmerevm-testnet-deprecated-1072"
+    },
+    {
+        "chainId": 1073,
+        "faucets": [
+            "https://evm-toolkit.evm.testnet.shimmer.network",
+            "https://evm-faucet.testnet.shimmer.network"
+        ],
+        "infoURL": "https://shimmer.network",
+        "name": "ShimmerEVM Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "SMR",
+            "symbol": "SMR"
+        },
+        "networkId": 1073,
         "rpc": [
             "https://json-rpc.evm.testnet.shimmer.network"
         ],
         "shortName": "shimmerevm-testnet"
     },
     {
+        "chainId": 1075,
+        "faucets": [
+            "https://evm-toolkit.evm.testnet.iotaledger.net"
+        ],
+        "infoURL": "https://www.iota.org",
+        "name": "IOTA EVM Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "IOTA",
+            "symbol": "IOTA"
+        },
+        "networkId": 1075,
+        "rpc": [
+            "https://json-rpc.evm.testnet.iotaledger.net"
+        ],
+        "shortName": "iotaevm-testnet"
+    },
+    {
         "chainId": 1079,
         "faucets": [],
         "infoURL": "https://playthink.co.jp",
         "name": "Mintara Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "MINTARA",
@@ -5910,15 +7077,17 @@
         "nativeCurrency": {
             "decimals": 18,
             "name": "Metis",
             "symbol": "METIS"
         },
         "networkId": 1088,
         "rpc": [
-            "https://andromeda.metis.io/?owner=1088"
+            "https://andromeda.metis.io/?owner=1088",
+            "https://metis.drpc.org",
+            "wss://metis.drpc.org"
         ],
         "shortName": "metis-andromeda"
     },
     {
         "chainId": 1089,
         "faucets": [],
         "infoURL": "https://humans.ai",
@@ -5927,19 +7096,21 @@
             "decimals": 18,
             "name": "HEART",
             "symbol": "HEART"
         },
         "networkId": 1089,
         "rpc": [
             "https://jsonrpc.humans.nodestake.top",
-            "https://humans-mainnet-evm.itrocket.net:443",
+            "https://humans-mainnet-evm.itrocket.net",
             "https://humans-evm-rpc.staketab.org:443",
             "https://evm.humans.stakepool.dev.br",
             "https://mainnet-humans-evm.konsortech.xyz",
-            "https://evm-rpc.mainnet.humans.zone"
+            "https://evm-rpc.mainnet.humans.zone",
+            "https://json-rpc.humans.bh.rocks",
+            "https://evm-rpc.humans.huginn.tech"
         ],
         "shortName": "humans"
     },
     {
         "chainId": 1099,
         "faucets": [],
         "infoURL": "https://moac.io",
@@ -5950,26 +7121,46 @@
             "symbol": "mc"
         },
         "networkId": 1099,
         "rpc": [],
         "shortName": "moac"
     },
     {
+        "chainId": 1100,
+        "faucets": [],
+        "infoURL": "https://dymension.xyz",
+        "name": "Dymension",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "DYM",
+            "symbol": "DYM"
+        },
+        "networkId": 1100,
+        "rpc": [
+            "https://dymension-evm.blockpi.network/v1/rpc/public",
+            "https://dymension-evm-rpc.publicnode.com",
+            "wss://dymension-evm-rpc.publicnode.com"
+        ],
+        "shortName": "dymension"
+    },
+    {
         "chainId": 1101,
         "faucets": [],
         "infoURL": "https://polygon.technology/polygon-zkevm",
         "name": "Polygon zkEVM",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Ether",
             "symbol": "ETH"
         },
         "networkId": 1101,
         "rpc": [
-            "https://zkevm-rpc.com"
+            "https://zkevm-rpc.com",
+            "https://polygon-zkevm.drpc.org",
+            "wss://polygon-zkevm.drpc.org"
         ],
         "shortName": "zkevm"
     },
     {
         "chainId": 1107,
         "faucets": [],
         "infoURL": "https://blx.org",
@@ -6034,14 +7225,30 @@
         "rpc": [
             "https://api.test.wemix.com",
             "wss://ws.test.wemix.com"
         ],
         "shortName": "twemix"
     },
     {
+        "chainId": 1113,
+        "faucets": [],
+        "infoURL": "https://www.bsquared.network",
+        "name": "B2 Hub Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "BSquared Token",
+            "symbol": "B2"
+        },
+        "networkId": 1113,
+        "rpc": [
+            "https://testnet-hub-rpc.bsquared.network"
+        ],
+        "shortName": "B2Hub-testnet"
+    },
+    {
         "chainId": 1115,
         "faucets": [
             "https://scan.test.btcs.network/faucet"
         ],
         "infoURL": "https://www.coredao.org",
         "name": "Core Blockchain Testnet",
         "nativeCurrency": {
@@ -6064,15 +7271,17 @@
             "decimals": 18,
             "name": "Core Blockchain Native Token",
             "symbol": "CORE"
         },
         "networkId": 1116,
         "rpc": [
             "https://rpc.coredao.org/",
-            "https://rpc-core.icecreamswap.com"
+            "https://rpc-core.icecreamswap.com",
+            "https://core.drpc.org",
+            "wss://core.drpc.org"
         ],
         "shortName": "core"
     },
     {
         "chainId": 1117,
         "faucets": [
             "https://faucet.dogcoin.network"
@@ -6087,14 +7296,30 @@
         "networkId": 1117,
         "rpc": [
             "https://mainnet-rpc.dogcoin.me"
         ],
         "shortName": "DOGSm"
     },
     {
+        "chainId": 1123,
+        "faucets": [],
+        "infoURL": "https://www.bsquared.network",
+        "name": "B2 Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Bitcoin",
+            "symbol": "BTC"
+        },
+        "networkId": 1123,
+        "rpc": [
+            "https://b2-testnet.alt.technology"
+        ],
+        "shortName": "B2-testnet"
+    },
+    {
         "chainId": 1130,
         "faucets": [],
         "infoURL": "https://meta.defichain.com/",
         "name": "DeFiChain EVM Network Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "DeFiChain",
@@ -6119,28 +7344,45 @@
         "shortName": "DFI-T"
     },
     {
         "chainId": 1133,
         "faucets": [
             "http://tc04.mydefichain.com/faucet"
         ],
-        "infoURL": "https://defichain.com",
-        "name": "DeFiMetaChain",
+        "infoURL": "https://meta.defichain.com",
+        "name": "DeFiMetaChain Changi Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "DeFiChain Token",
             "symbol": "DFI"
         },
         "networkId": 1133,
         "rpc": [
+            "https://dmc.mydefichain.com/changi",
             "https://testnet-dmc.mydefichain.com:20551"
         ],
         "shortName": "changi"
     },
     {
+        "chainId": 1135,
+        "faucets": [],
+        "infoURL": "https://lisk.com",
+        "name": "Lisk",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 1135,
+        "rpc": [
+            "https://rpc.api.lisk.com"
+        ],
+        "shortName": "lisk"
+    },
+    {
         "chainId": 1138,
         "faucets": [],
         "infoURL": "https://sinso.io",
         "name": "AmStar Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "SINSO",
@@ -6232,14 +7474,30 @@
         "networkId": 1177,
         "rpc": [
             "https://s2.tl.web.tr:4041"
         ],
         "shortName": "sht"
     },
     {
+        "chainId": 1188,
+        "faucets": [],
+        "infoURL": "https://www.mosscan.com",
+        "name": "ClubMos Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "ClubMos",
+            "symbol": "MOS"
+        },
+        "networkId": 1188,
+        "rpc": [
+            "https://mainnet.mosscan.com"
+        ],
+        "shortName": "MOS"
+    },
+    {
         "chainId": 1197,
         "faucets": [],
         "infoURL": "https://iorachain.com",
         "name": "Iora Chain",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Iora",
@@ -6281,14 +7539,30 @@
         "rpc": [
             "https://rpc.cadaut.com",
             "wss://rpc.cadaut.com/ws"
         ],
         "shortName": "wtt"
     },
     {
+        "chainId": 1209,
+        "faucets": [],
+        "infoURL": "https://saitachain.com",
+        "name": "SaitaBlockChain(SBC)",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "SaitaBlockChain(SBC)",
+            "symbol": "STC"
+        },
+        "networkId": 1209,
+        "rpc": [
+            "https://rpc-nodes.saitascan.io"
+        ],
+        "shortName": "SBC"
+    },
+    {
         "chainId": 1213,
         "faucets": [],
         "infoURL": "https://popcateum.org",
         "name": "Popcateum Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Popcat",
@@ -6313,14 +7587,46 @@
         "networkId": 1214,
         "rpc": [
             "https://tapi.entercoin.net/"
         ],
         "shortName": "enter"
     },
     {
+        "chainId": 1221,
+        "faucets": [],
+        "infoURL": "https://www.cyclenetwork.io/",
+        "name": "Cycle Network Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 1221,
+        "rpc": [
+            "https://rpc-testnet.cyclenetwork.io"
+        ],
+        "shortName": "Cycle"
+    },
+    {
+        "chainId": 1224,
+        "faucets": [],
+        "infoURL": "https://buildonhybrid.com",
+        "name": "Hybrid Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Hybrid",
+            "symbol": "HYB"
+        },
+        "networkId": 1224,
+        "rpc": [
+            "https://testnet-rpc.buildonhybrid.com"
+        ],
+        "shortName": "hyb"
+    },
+    {
         "chainId": 1229,
         "faucets": [],
         "infoURL": "https://exzo.network",
         "name": "Exzo Network Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Exzo",
@@ -6427,14 +7733,30 @@
         "networkId": 1246,
         "rpc": [
             "https://rpc-cnx.omplatform.com/"
         ],
         "shortName": "om"
     },
     {
+        "chainId": 1248,
+        "faucets": [],
+        "infoURL": "https://www.dogether.dog/",
+        "name": "Dogether Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Dogether",
+            "symbol": "dogeth"
+        },
+        "networkId": 1248,
+        "rpc": [
+            "https://rpc.dogether.dog/"
+        ],
+        "shortName": "Dogether"
+    },
+    {
         "chainId": 1252,
         "faucets": [
             "https://cicfaucet.com"
         ],
         "infoURL": "https://www.cicchain.net",
         "name": "CIC Chain Testnet",
         "nativeCurrency": {
@@ -6474,16 +7796,18 @@
             "name": "Glimmer",
             "symbol": "GLMR"
         },
         "networkId": 1284,
         "rpc": [
             "https://rpc.api.moonbeam.network",
             "wss://wss.api.moonbeam.network",
-            "https://moonbeam.publicnode.com",
-            "wss://moonbeam.publicnode.com"
+            "https://moonbeam-rpc.publicnode.com",
+            "wss://moonbeam-rpc.publicnode.com",
+            "https://moonbeam.drpc.org",
+            "wss://moonbeam.drpc.org"
         ],
         "shortName": "mbeam"
     },
     {
         "chainId": 1285,
         "faucets": [],
         "infoURL": "https://moonbeam.network/networks/moonriver/",
@@ -6493,16 +7817,18 @@
             "name": "Moonriver",
             "symbol": "MOVR"
         },
         "networkId": 1285,
         "rpc": [
             "https://rpc.api.moonriver.moonbeam.network",
             "wss://wss.api.moonriver.moonbeam.network",
-            "https://moonriver.publicnode.com",
-            "wss://moonriver.publicnode.com"
+            "https://moonriver-rpc.publicnode.com",
+            "wss://moonriver-rpc.publicnode.com",
+            "https://moonriver.drpc.org",
+            "wss://moonriver.drpc.org"
         ],
         "shortName": "mriver"
     },
     {
         "chainId": 1286,
         "faucets": [],
         "infoURL": "",
@@ -6525,15 +7851,17 @@
             "decimals": 18,
             "name": "Dev",
             "symbol": "DEV"
         },
         "networkId": 1287,
         "rpc": [
             "https://rpc.api.moonbase.moonbeam.network",
-            "wss://wss.api.moonbase.moonbeam.network"
+            "wss://wss.api.moonbase.moonbeam.network",
+            "https://moonbase-alpha.drpc.org",
+            "wss://moonbase-alpha.drpc.org"
         ],
         "shortName": "mbase"
     },
     {
         "chainId": 1288,
         "faucets": [],
         "infoURL": "https://docs.moonbeam.network/learn/platform/networks/overview/",
@@ -6720,14 +8048,30 @@
         "networkId": 1339,
         "rpc": [
             "https://rpc.elysiumchain.tech/"
         ],
         "shortName": "ELSM"
     },
     {
+        "chainId": 1343,
+        "faucets": [],
+        "infoURL": "https://blitz.gg",
+        "name": "Blitz Subnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "BLITZ GAS",
+            "symbol": "BGAS"
+        },
+        "networkId": 1343,
+        "rpc": [
+            "https://subnets.avax.network/blitz/testnet/rpc"
+        ],
+        "shortName": "blitz"
+    },
+    {
         "chainId": 1353,
         "faucets": [],
         "infoURL": "https://www.cicchain.net",
         "name": "CIC Chain Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Crazy Internet Coin",
@@ -6872,15 +8216,17 @@
         "nativeCurrency": {
             "decimals": 18,
             "name": "Ether",
             "symbol": "ETH"
         },
         "networkId": 1442,
         "rpc": [
-            "https://rpc.public.zkevm-test.net"
+            "https://rpc.public.zkevm-test.net",
+            "https://polygon-zkevm-testnet.drpc.org",
+            "wss://polygon-zkevm-testnet.drpc.org"
         ],
         "shortName": "testnet-zkEVM-mango"
     },
     {
         "chainId": 1452,
         "faucets": [],
         "infoURL": "https://gaussgang.com/",
@@ -6893,14 +8239,32 @@
         "networkId": 1452,
         "rpc": [
             "https://rpc.giltestnet.com"
         ],
         "shortName": "gil"
     },
     {
+        "chainId": 1453,
+        "faucets": [
+            "https://istanbul-faucet.metachain.dev"
+        ],
+        "infoURL": "https://metatime.com/en",
+        "name": "MetaChain Istanbul",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Metatime Coin",
+            "symbol": "MTC"
+        },
+        "networkId": 1453,
+        "rpc": [
+            "https://istanbul-rpc.metachain.dev"
+        ],
+        "shortName": "metatimeistanbul"
+    },
+    {
         "chainId": 1455,
         "faucets": [
             "https://faucet.ctexscan.com"
         ],
         "infoURL": "https://ctextoken.io",
         "name": "Ctex Scan Blockchain",
         "nativeCurrency": {
@@ -6911,27 +8275,59 @@
         "networkId": 1455,
         "rpc": [
             "https://mainnet-rpc.ctexscan.com/"
         ],
         "shortName": "CTEX"
     },
     {
+        "chainId": 1490,
+        "faucets": [],
+        "infoURL": "https://www.vitruveo.xyz",
+        "name": "Vitruveo Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Vitruveo Coin",
+            "symbol": "VTRU"
+        },
+        "networkId": 1490,
+        "rpc": [
+            "https://rpc.vitruveo.xyz"
+        ],
+        "shortName": "vitruveo"
+    },
+    {
+        "chainId": 1499,
+        "faucets": [],
+        "infoURL": "https://idosgames.com/",
+        "name": "iDos Games Chain Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "iDos Games Coin",
+            "symbol": "IGC"
+        },
+        "networkId": 1499,
+        "rpc": [
+            "https://rpc-testnet.idos.games"
+        ],
+        "shortName": "IGC"
+    },
+    {
         "chainId": 1501,
         "faucets": [],
         "infoURL": "https://chainx.org",
-        "name": "BEVM",
+        "name": "BEVM Canary",
         "nativeCurrency": {
             "decimals": 18,
             "name": "BTC",
             "symbol": "BTC"
         },
         "networkId": 1501,
         "rpc": [
-            "https://rpc-1.bevm.io/",
-            "https://rpc-2.bevm.io/"
+            "https://rpc-canary-1.bevm.io/",
+            "https://rpc-canary-2.bevm.io/"
         ],
         "shortName": "chainx"
     },
     {
         "chainId": 1506,
         "faucets": [],
         "infoURL": "https://sherpax.io/",
@@ -6996,14 +8392,30 @@
             "https://rpc.tenet.org",
             "https://tenet-evm.publicnode.com",
             "wss://tenet-evm.publicnode.com"
         ],
         "shortName": "tenet"
     },
     {
+        "chainId": 1617,
+        "faucets": [],
+        "infoURL": "https://www.etins.org",
+        "name": "Ethereum Inscription Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ethereum Inscription",
+            "symbol": "ETINS"
+        },
+        "networkId": 1617,
+        "rpc": [
+            "https://rpc.etins.org"
+        ],
+        "shortName": "etins"
+    },
+    {
         "chainId": 1618,
         "faucets": [],
         "infoURL": "https://catechain.com",
         "name": "Catecoin Chain Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Catecoin",
@@ -7046,24 +8458,24 @@
             "https://dataseed1.btachain.com/"
         ],
         "shortName": "bta"
     },
     {
         "chainId": 1662,
         "faucets": [],
-        "infoURL": "https://horizen.io/",
-        "name": "Horizen Yuma Testnet Deprecated",
+        "infoURL": "https://liquichain.io/",
+        "name": "Liquichain",
         "nativeCurrency": {
             "decimals": 18,
-            "name": "Testnet Zen",
-            "symbol": "tZEN"
+            "name": "Licoin",
+            "symbol": "LCN"
         },
         "networkId": 1662,
         "rpc": [],
-        "shortName": "Yuma"
+        "shortName": "Liquichain"
     },
     {
         "chainId": 1663,
         "faucets": [
             "https://faucet.horizen.io"
         ],
         "infoURL": "https://horizen.io/",
@@ -7077,14 +8489,46 @@
         "rpc": [
             "https://gobi-rpc.horizenlabs.io/ethv1",
             "https://rpc.ankr.com/horizen_gobi_testnet"
         ],
         "shortName": "Gobi"
     },
     {
+        "chainId": 1686,
+        "faucets": [],
+        "infoURL": "https://www.mintchain.io",
+        "name": "Mint Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Sepolia Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 1686,
+        "rpc": [
+            "https://testnet-rpc.mintchain.io"
+        ],
+        "shortName": "minttest"
+    },
+    {
+        "chainId": 1687,
+        "faucets": [],
+        "infoURL": "https://www.mintchain.io",
+        "name": "Mint Sepolia Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Sepolia Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 1687,
+        "rpc": [
+            "https://sepolia-testnet-rpc.mintchain.io"
+        ],
+        "shortName": "mintsepoliatest"
+    },
+    {
         "chainId": 1688,
         "faucets": [],
         "infoURL": "https://www.ludan.org/",
         "name": "LUDAN Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "LUDAN",
@@ -7145,14 +8589,30 @@
         "networkId": 1708,
         "rpc": [
             "https://rpc.testnet.blockchain.or.th"
         ],
         "shortName": "tTBSI"
     },
     {
+        "chainId": 1717,
+        "faucets": [],
+        "infoURL": "https://doric.network",
+        "name": "Doric Network",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Doric Native Token",
+            "symbol": "DRC"
+        },
+        "networkId": 1717,
+        "rpc": [
+            "https://mainnet.doric.network"
+        ],
+        "shortName": "DRC"
+    },
+    {
         "chainId": 1718,
         "faucets": [],
         "infoURL": "https://hashpalette.com/",
         "name": "Palette Chain Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Palette Token",
@@ -7161,14 +8621,31 @@
         "networkId": 1718,
         "rpc": [
             "https://palette-rpc.com:22000"
         ],
         "shortName": "PCM"
     },
     {
+        "chainId": 1729,
+        "faucets": [],
+        "infoURL": "https://reya.network",
+        "name": "Reya Network",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 1729,
+        "rpc": [
+            "https://rpc.reya.network",
+            "wss://ws.reya.network"
+        ],
+        "shortName": "reya"
+    },
+    {
         "chainId": 1773,
         "faucets": [],
         "infoURL": "TeaPartyCrypto.com",
         "name": "PartyChain",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Grams",
@@ -7277,14 +8754,31 @@
             "wss://ws-testnet-jp.cube.network",
             "https://http-testnet-us.cube.network",
             "wss://ws-testnet-us.cube.network"
         ],
         "shortName": "cubet"
     },
     {
+        "chainId": 1821,
+        "faucets": [],
+        "infoURL": "https://rubychain.io",
+        "name": "Ruby Smart Chain MAINNET",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "RUBY Smart Chain Native Token",
+            "symbol": "RUBY"
+        },
+        "networkId": 1821,
+        "rpc": [
+            "https://mainnet-data.rubychain.io/",
+            "https://mainnet.rubychain.io/"
+        ],
+        "shortName": "RUBY"
+    },
+    {
         "chainId": 1856,
         "faucets": [],
         "infoURL": "https://teslafunds.io",
         "name": "Teslafunds",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Teslafunds Ether",
@@ -7295,24 +8789,24 @@
             "https://tsfapi.europool.me"
         ],
         "shortName": "tsf"
     },
     {
         "chainId": 1875,
         "faucets": [],
-        "infoURL": "https://whitebit.network",
-        "name": "WhiteBIT Network",
+        "infoURL": "https://whitechain.io",
+        "name": "Whitechain",
         "nativeCurrency": {
             "decimals": 18,
             "name": "WhiteBIT Coin",
             "symbol": "WBT"
         },
         "networkId": 1875,
         "rpc": [
-            "https://rpc.whitebit.network"
+            "https://rpc.whitechain.io"
         ],
         "shortName": "wbt"
     },
     {
         "chainId": 1881,
         "faucets": [],
         "infoURL": "https://gitshock.com",
@@ -7336,35 +8830,33 @@
         "nativeCurrency": {
             "decimals": 18,
             "name": "Ethereum",
             "symbol": "ETH"
         },
         "networkId": 1890,
         "rpc": [
-            "https://replicator-01.phoenix.lightlink.io/rpc/v1",
-            "https://replicator-02.phoenix.lightlink.io/rpc/v1"
+            "https://replicator.phoenix.lightlink.io/rpc/v1"
         ],
         "shortName": "lightlink_phoenix"
     },
     {
         "chainId": 1891,
         "faucets": [
-            "https://pegasus-faucet-react.vercel.app"
+            "https://faucet.pegasus.lightlink.io/"
         ],
         "infoURL": "https://lightlink.io",
         "name": "Lightlink Pegasus Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Ethereum",
             "symbol": "ETH"
         },
         "networkId": 1891,
         "rpc": [
-            "https://replicator-01.pegasus.lightlink.io/rpc/v1",
-            "https://replicator-02.pegasus.lightlink.io/rpc/v1"
+            "https://replicator.pegasus.lightlink.io/rpc/v1"
         ],
         "shortName": "lightlink_pegasus"
     },
     {
         "chainId": 1898,
         "faucets": [],
         "infoURL": "https://boyanet.org",
@@ -7428,14 +8920,80 @@
         "networkId": 1908,
         "rpc": [
             "https://testnet.bitcichain.com"
         ],
         "shortName": "tbitci"
     },
     {
+        "chainId": 1909,
+        "faucets": [],
+        "infoURL": "https://merklescan.com",
+        "name": "Merkle Scan",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Merkle",
+            "symbol": "MRK"
+        },
+        "networkId": 1909,
+        "rpc": [
+            "https://marklechain-rpc.merklescan.com"
+        ],
+        "shortName": "MRK"
+    },
+    {
+        "chainId": 1911,
+        "faucets": [],
+        "infoURL": "https://scalind.com",
+        "name": "Scalind",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 1911,
+        "rpc": [
+            "https://rpc.scalind.com"
+        ],
+        "shortName": "scal"
+    },
+    {
+        "chainId": 1912,
+        "faucets": [
+            "https://claim-faucet.rubychain.io/"
+        ],
+        "infoURL": "https://rubychain.io",
+        "name": "Ruby Smart Chain Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "RUBY Smart Chain Native Token",
+            "symbol": "tRUBY"
+        },
+        "networkId": 1912,
+        "rpc": [
+            "https://testnet-rchain.rubychain.io/"
+        ],
+        "shortName": "tRUBY"
+    },
+    {
+        "chainId": 1918,
+        "faucets": [],
+        "infoURL": "https://mobylab.docs.crescdi.pub.ro/blog/UPB-CRESCDI-Testnet",
+        "name": "UPB CRESCDI Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "UPBEth",
+            "symbol": "UPBEth"
+        },
+        "networkId": 1918,
+        "rpc": [
+            "https://testnet.crescdi.pub.ro"
+        ],
+        "shortName": "UPBEth"
+    },
+    {
         "chainId": 1945,
         "faucets": [],
         "infoURL": "https://onuschain.io",
         "name": "ONUS Chain Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "ONUS",
@@ -7460,14 +9018,31 @@
         "networkId": 1951,
         "rpc": [
             "https://mainnet.d-chain.network/ext/bc/2ZiR1Bro5E59siVuwdNuRFzqL95NkvkbzyLBdrsYR9BLSHV7H4/rpc"
         ],
         "shortName": "dchain-mainnet"
     },
     {
+        "chainId": 1953,
+        "faucets": [],
+        "infoURL": "https://selendra.org",
+        "name": "Selendra Network Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Selendra",
+            "symbol": "tSEL"
+        },
+        "networkId": 1953,
+        "rpc": [
+            "https://rpc0-testnet.selendra.org",
+            "https://rpc1-testnet.selendra.org"
+        ],
+        "shortName": "tSEL"
+    },
+    {
         "chainId": 1954,
         "faucets": [],
         "infoURL": "https://dexilla.com",
         "name": "Dexilla Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Dexilla Native Token",
@@ -7476,14 +9051,31 @@
         "networkId": 1954,
         "rpc": [
             "https://rpc.dexilla.com"
         ],
         "shortName": "Dexilla"
     },
     {
+        "chainId": 1961,
+        "faucets": [],
+        "infoURL": "https://selendra.org",
+        "name": "Selendra Network Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Selendra",
+            "symbol": "SEL"
+        },
+        "networkId": 1961,
+        "rpc": [
+            "https://rpc0.selendra.org",
+            "https://rpc1.selendra.org"
+        ],
+        "shortName": "SEL"
+    },
+    {
         "chainId": 1967,
         "faucets": [
             "https://faucet.metatime.com/eleanor"
         ],
         "infoURL": "https://eleanor.metatime.com",
         "name": "Eleanor",
         "nativeCurrency": {
@@ -7546,14 +9138,30 @@
         "rpc": [
             "https://1971.network/atlr",
             "wss://1971.network/atlr"
         ],
         "shortName": "atlr"
     },
     {
+        "chainId": 1972,
+        "faucets": [],
+        "infoURL": "https://www.redecoin.eu",
+        "name": "RedeCoin",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "RedeCoin",
+            "symbol": "REDEV2"
+        },
+        "networkId": 1972,
+        "rpc": [
+            "https://rpc2.redecoin.eu"
+        ],
+        "shortName": "rede"
+    },
+    {
         "chainId": 1975,
         "faucets": [],
         "infoURL": "https://onuschain.io",
         "name": "ONUS Chain Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "ONUS",
@@ -7627,14 +9235,31 @@
         "networkId": 1987,
         "rpc": [
             "https://jsonrpc.egem.io/custom"
         ],
         "shortName": "egem"
     },
     {
+        "chainId": 1992,
+        "faucets": [],
+        "infoURL": "https://www.hubble.exchange",
+        "name": "Hubble Exchange",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "USD Coin",
+            "symbol": "USDC"
+        },
+        "networkId": 1992,
+        "rpc": [
+            "https://rpc.hubble.exchange",
+            "wss://ws-rpc.hubble.exchange"
+        ],
+        "shortName": "hubblenet"
+    },
+    {
         "chainId": 1994,
         "faucets": [],
         "infoURL": "https://www.ekta.io",
         "name": "Ekta",
         "nativeCurrency": {
             "decimals": 18,
             "name": "EKTA",
@@ -7647,29 +9272,47 @@
         "shortName": "ekta"
     },
     {
         "chainId": 1995,
         "faucets": [
             "https://faucet.edexa.com/"
         ],
-        "infoURL": "https://edexa.com/",
+        "infoURL": "https://edexa.network/",
         "name": "edeXa Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "EDEXA",
             "symbol": "EDX"
         },
         "networkId": 1995,
         "rpc": [
-            "https://testnet.edexa.com/rpc",
+            "https://testnet.edexa.network/rpc",
             "https://io-dataseed1.testnet.edexa.io-market.com/rpc"
         ],
         "shortName": "edx"
     },
     {
+        "chainId": 1998,
+        "faucets": [
+            "https://faucet.kyotoprotocol.io"
+        ],
+        "infoURL": "https://kyotoprotocol.io",
+        "name": "Kyoto Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Kyoto",
+            "symbol": "KYOTO"
+        },
+        "networkId": 1998,
+        "rpc": [
+            "https://rpc.testnet.kyotoprotocol.io:8545"
+        ],
+        "shortName": "kyoto-testnet"
+    },
+    {
         "chainId": 2000,
         "faucets": [],
         "infoURL": "https://dogechain.dog",
         "name": "Dogechain Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Dogecoin",
@@ -7743,29 +9386,51 @@
         },
         "networkId": 2009,
         "rpc": [],
         "shortName": "cloudwalk_mainnet"
     },
     {
         "chainId": 2016,
-        "faucets": [
-            "https://faucet.mainnetz.io"
-        ],
+        "faucets": [],
         "infoURL": "https://mainnetz.io",
         "name": "MainnetZ Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "MainnetZ",
             "symbol": "NetZ"
         },
         "networkId": 2016,
         "rpc": [
-            "https://mainnet-rpc.mainnetz.io"
+            "https://mainnet-rpc.mainnetz.io",
+            "https://eu-rpc.mainnetz.io"
         ],
-        "shortName": "NetZm"
+        "shortName": "netz"
+    },
+    {
+        "chainId": 2017,
+        "faucets": [
+            "https://telcoin.network/faucet"
+        ],
+        "infoURL": "https://telcoin.network",
+        "name": "Adiri",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Telcoin",
+            "symbol": "TEL"
+        },
+        "networkId": 2017,
+        "rpc": [
+            "https://rpc.telcoin.network",
+            "https://adiri.tel",
+            "https://node1.telcoin.network",
+            "https://node2.telcoin.network",
+            "https://node3.telcoin.network",
+            "https://node4.telcoin.network"
+        ],
+        "shortName": "tel"
     },
     {
         "chainId": 2018,
         "faucets": [],
         "infoURL": "https://publicmint.com",
         "name": "PublicMint Devnet",
         "nativeCurrency": {
@@ -7820,23 +9485,23 @@
             "decimals": 18,
             "name": "Edgeware",
             "symbol": "EDG"
         },
         "networkId": 2021,
         "rpc": [
             "https://edgeware-evm.jelliedowl.net",
-            "https://mainnet2.edgewa.re/evm",
-            "https://mainnet3.edgewa.re/evm",
-            "https://mainnet4.edgewa.re/evm",
-            "https://mainnet5.edgewa.re/evm",
+            "https://edgeware-evm0.jelliedowl.net",
+            "https://edgeware-evm1.jelliedowl.net",
+            "https://edgeware-evm2.jelliedowl.net",
+            "https://edgeware-evm3.jelliedowl.net",
             "wss://edgeware.jelliedowl.net",
-            "wss://mainnet2.edgewa.re",
-            "wss://mainnet3.edgewa.re",
-            "wss://mainnet4.edgewa.re",
-            "wss://mainnet5.edgewa.re"
+            "wss://edgeware-rpc0.jelliedowl.net",
+            "wss://edgeware-rpc1.jelliedowl.net",
+            "wss://edgeware-rpc2.jelliedowl.net",
+            "wss://edgeware-rpc3.jelliedowl.net"
         ],
         "shortName": "edg"
     },
     {
         "chainId": 2022,
         "faucets": [],
         "infoURL": "https://edgeware.io/build",
@@ -7868,14 +9533,30 @@
         "networkId": 2023,
         "rpc": [
             "https://test-taycan.hupayx.io"
         ],
         "shortName": "taycan-testnet"
     },
     {
+        "chainId": 2024,
+        "faucets": [],
+        "infoURL": "https://swanchain.io/",
+        "name": "Swan Saturn Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "SWANETH",
+            "symbol": "sETH"
+        },
+        "networkId": 2024,
+        "rpc": [
+            "https://saturn-rpc.swanchain.io"
+        ],
+        "shortName": "swan"
+    },
+    {
         "chainId": 2025,
         "faucets": [],
         "infoURL": "https://rangersprotocol.com",
         "name": "Rangers Protocol Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Rangers Protocol Gas",
@@ -7884,26 +9565,49 @@
         "networkId": 2025,
         "rpc": [
             "https://mainnet.rangersprotocol.com/api/jsonrpc"
         ],
         "shortName": "rpg"
     },
     {
+        "chainId": 2026,
+        "faucets": [],
+        "infoURL": "https://edgeless.network",
+        "name": "Edgeless Network",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Edgeless Wrapped Eth",
+            "symbol": "EwEth"
+        },
+        "networkId": 2026,
+        "rpc": [
+            "https://rpc.edgeless.network/http"
+        ],
+        "shortName": "edgeless"
+    },
+    {
         "chainId": 2031,
         "faucets": [],
         "infoURL": "https://centrifuge.io",
         "name": "Centrifuge",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Centrifuge",
             "symbol": "CFG"
         },
         "networkId": 2031,
         "rpc": [
-            "wss://fullnode.parachain.centrifuge.io"
+            "https://fullnode.centrifuge.io",
+            "wss://fullnode.centrifuge.io",
+            "https://centrifuge-parachain.api.onfinality.io/public",
+            "wss://centrifuge-parachain.api.onfinality.io/public-ws",
+            "https://centrifuge-rpc.dwellir.com",
+            "wss://centrifuge-rpc.dwellir.com",
+            "https://rpc-centrifuge.luckyfriday.io",
+            "wss://rpc-centrifuge.luckyfriday.io"
         ],
         "shortName": "cfg"
     },
     {
         "chainId": 2032,
         "faucets": [],
         "infoURL": "https://centrifuge.io",
@@ -7916,14 +9620,28 @@
         "networkId": 2032,
         "rpc": [
             "wss://fullnode.catalyst.cntrfg.com"
         ],
         "shortName": "ncfg"
     },
     {
+        "chainId": 2035,
+        "faucets": [],
+        "infoURL": "https://phala.network",
+        "name": "Phala Network",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Phala",
+            "symbol": "PHA"
+        },
+        "networkId": 2035,
+        "rpc": [],
+        "shortName": "pha"
+    },
+    {
         "chainId": 2037,
         "faucets": [],
         "infoURL": "",
         "name": "Kiwi Subnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Shrapgas",
@@ -7948,14 +9666,31 @@
         "networkId": 2038,
         "rpc": [
             "https://subnets.avax.network/shrapnel/testnet/rpc"
         ],
         "shortName": "shraptest"
     },
     {
+        "chainId": 2040,
+        "faucets": [],
+        "infoURL": "https://vanarchain.com",
+        "name": "Vanar Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "VANRY",
+            "symbol": "VANRY"
+        },
+        "networkId": 2040,
+        "rpc": [
+            "https://rpc.vanarchain.com",
+            "wss://ws.vanarchain.com"
+        ],
+        "shortName": "Vanar"
+    },
+    {
         "chainId": 2043,
         "faucets": [],
         "infoURL": "https://parachain.origintrail.io",
         "name": "OriginTrail Parachain",
         "nativeCurrency": {
             "decimals": 12,
             "name": "OriginTrail Parachain Token",
@@ -8058,15 +9793,16 @@
         "nativeCurrency": {
             "decimals": 18,
             "name": "Altair",
             "symbol": "AIR"
         },
         "networkId": 2088,
         "rpc": [
-            "wss://fullnode.altair.centrifuge.io"
+            "wss://fullnode.altair.centrifuge.io",
+            "wss://altair.api.onfinality.io/public-ws"
         ],
         "shortName": "air"
     },
     {
         "chainId": 2089,
         "faucets": [],
         "infoURL": "https://centrifuge.io",
@@ -8128,14 +9864,30 @@
         "rpc": [
             "https://rpc.exosama.com",
             "wss://rpc.exosama.com"
         ],
         "shortName": "exn"
     },
     {
+        "chainId": 2121,
+        "faucets": [],
+        "infoURL": "https://catena.network",
+        "name": "Catena Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Catena",
+            "symbol": "CMCX"
+        },
+        "networkId": 2121,
+        "rpc": [
+            "https://rpc1.catenarpc.com"
+        ],
+        "shortName": "cmcx"
+    },
+    {
         "chainId": 2122,
         "faucets": [],
         "infoURL": "https://docs.metaplayer.one/",
         "name": "Metaplayerone Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "METAD",
@@ -8160,14 +9912,31 @@
         "networkId": 2124,
         "rpc": [
             "https://rpc-dubai.mp1network.com/"
         ],
         "shortName": "MEU"
     },
     {
+        "chainId": 2136,
+        "faucets": [],
+        "infoURL": "https://bigshortbets.com/",
+        "name": "BigShortBets Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Dolarz",
+            "symbol": "Dolarz"
+        },
+        "networkId": 2136,
+        "rpc": [
+            "https://test-market.bigsb.io",
+            "wss://test-market.bigsb.io"
+        ],
+        "shortName": "bigsb_testnet"
+    },
+    {
         "chainId": 2137,
         "faucets": [],
         "infoURL": "https://bigshortbets.com/",
         "name": "BigShortBets",
         "nativeCurrency": {
             "decimals": 18,
             "name": "USD Coin",
@@ -8194,14 +9963,46 @@
         "rpc": [
             "https://rpc.public-2138.defi-oracle.io",
             "wss://rpc.public-2138.defi-oracle.io"
         ],
         "shortName": "dfio-meta-test"
     },
     {
+        "chainId": 2140,
+        "faucets": [],
+        "infoURL": "",
+        "name": "Oneness Network",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "BTC",
+            "symbol": "BTC"
+        },
+        "networkId": 2140,
+        "rpc": [
+            "https://rpc.onenesslabs.io/"
+        ],
+        "shortName": "oneness"
+    },
+    {
+        "chainId": 2141,
+        "faucets": [],
+        "infoURL": "",
+        "name": "Oneness TestNet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "BTC",
+            "symbol": "BTC"
+        },
+        "networkId": 2141,
+        "rpc": [
+            "https://rpc.testnet.onenesslabs.io/"
+        ],
+        "shortName": "oneness-testnet"
+    },
+    {
         "chainId": 2151,
         "faucets": [],
         "infoURL": "https://docs.bosagora.org",
         "name": "BOSagora Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "BOSAGORA",
@@ -8343,15 +10144,17 @@
             "name": "TKava",
             "symbol": "TKAVA"
         },
         "networkId": 2221,
         "rpc": [
             "https://evm.testnet.kava.io",
             "https://kava-evm-testnet.rpc.thirdweb.com",
-            "wss://wevm.testnet.kava.io"
+            "wss://wevm.testnet.kava.io",
+            "https://kava-testnet.drpc.org",
+            "wss://kava-testnet.drpc.org"
         ],
         "shortName": "tkava"
     },
     {
         "chainId": 2222,
         "faucets": [],
         "infoURL": "https://www.kava.io",
@@ -8363,16 +10166,21 @@
         },
         "networkId": 2222,
         "rpc": [
             "https://evm.kava.io",
             "https://kava-rpc.gateway.pokt.network",
             "https://kava-evm.rpc.thirdweb.com",
             "wss://wevm.kava.io",
-            "https://kava-evm.publicnode.com",
-            "wss://kava-evm.publicnode.com"
+            "https://kava-evm-rpc.publicnode.com",
+            "wss://kava-evm-rpc.publicnode.com",
+            "https://evm.kava-rpc.com",
+            "https://rpc.ankr.com/kava_evm",
+            "wss://wevm.kava-rpc.com",
+            "https://kava.drpc.org",
+            "wss://kava.drpc.org"
         ],
         "shortName": "kava"
     },
     {
         "chainId": 2223,
         "faucets": [],
         "infoURL": "https://bo.vcex.xyz/",
@@ -8396,15 +10204,16 @@
         "nativeCurrency": {
             "decimals": 18,
             "name": "Krest",
             "symbol": "KRST"
         },
         "networkId": 2241,
         "rpc": [
-            "https://erpc-krest.peaq.network"
+            "https://erpc-krest.peaq.network",
+            "https://krest.unitedbloc.com"
         ],
         "shortName": "KRST"
     },
     {
         "chainId": 2300,
         "faucets": [],
         "infoURL": "https://www.bombchain.com",
@@ -8417,14 +10226,30 @@
         "networkId": 2300,
         "rpc": [
             "https://rpc.bombchain.com"
         ],
         "shortName": "bomb"
     },
     {
+        "chainId": 2306,
+        "faucets": [],
+        "infoURL": "https://www.ebrochain.com",
+        "name": "Ebro Network",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ebro",
+            "symbol": "ebro"
+        },
+        "networkId": 2306,
+        "rpc": [
+            "https://greendinoswap.com"
+        ],
+        "shortName": "ebro"
+    },
+    {
         "chainId": 2309,
         "faucets": [],
         "infoURL": "",
         "name": "Arevia",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Arev",
@@ -8469,14 +10294,30 @@
         "networkId": 2330,
         "rpc": [
             "https://rpc0.altcoinchain.org/rpc"
         ],
         "shortName": "alt"
     },
     {
+        "chainId": 2331,
+        "faucets": [],
+        "infoURL": "https://rss3.io",
+        "name": "RSS3 VSL Sepolia Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "RSS3",
+            "symbol": "RSS3"
+        },
+        "networkId": 2331,
+        "rpc": [
+            "https://rpc.testnet.rss3.io"
+        ],
+        "shortName": "rss3-testnet"
+    },
+    {
         "chainId": 2332,
         "faucets": [
             "https://airdrop.somanetwork.io"
         ],
         "infoURL": "https://somanetwork.io",
         "name": "SOMA Network Mainnet",
         "nativeCurrency": {
@@ -8490,14 +10331,51 @@
             "https://id-mainnet.somanetwork.io",
             "https://hk-mainnet.somanetwork.io",
             "https://sg-mainnet.somanetwork.io"
         ],
         "shortName": "smam"
     },
     {
+        "chainId": 2340,
+        "faucets": [
+            "https://faucet.atleta.network"
+        ],
+        "infoURL": "https://atleta.network",
+        "name": "Atleta Olympia",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Atla",
+            "symbol": "ATLA"
+        },
+        "networkId": 2340,
+        "rpc": [
+            "wss://testnet-rpc.atleta.network:9944",
+            "https://testnet-rpc.atleta.network:9944"
+        ],
+        "shortName": "atla"
+    },
+    {
+        "chainId": 2342,
+        "faucets": [
+            "https://www.omniaverse.io"
+        ],
+        "infoURL": "https://www.omniaverse.io",
+        "name": "Omnia Chain",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Omnia",
+            "symbol": "OMNIA"
+        },
+        "networkId": 2342,
+        "rpc": [
+            "https://rpc.omniaverse.io"
+        ],
+        "shortName": "omnia"
+    },
+    {
         "chainId": 2357,
         "faucets": [],
         "infoURL": "https://kroma.network",
         "name": "(deprecated) Kroma Sepolia",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Sepolia Ether",
@@ -8522,14 +10400,32 @@
         "networkId": 2358,
         "rpc": [
             "https://api.sepolia.kroma.network"
         ],
         "shortName": "kroma-sepolia"
     },
     {
+        "chainId": 2370,
+        "faucets": [
+            "https://evm-faucet.nexis.network"
+        ],
+        "infoURL": "https://nexis.network/",
+        "name": "Nexis Network Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Nexis",
+            "symbol": "NZT"
+        },
+        "networkId": 2370,
+        "rpc": [
+            "https://evm-testnet.nexis.network"
+        ],
+        "shortName": "nzt"
+    },
+    {
         "chainId": 2399,
         "faucets": [
             "https://faucet.bombchain-testnet.ankr.com/"
         ],
         "infoURL": "https://www.bombmoney.com",
         "name": "BOMB Chain Testnet",
         "nativeCurrency": {
@@ -8556,14 +10452,30 @@
         "networkId": 2400,
         "rpc": [
             "https://rpc.tcgverse.xyz"
         ],
         "shortName": "TCGV"
     },
     {
+        "chainId": 2410,
+        "faucets": [],
+        "infoURL": "https://karak.network",
+        "name": "Karak Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 2410,
+        "rpc": [
+            "https://rpc.karak.network"
+        ],
+        "shortName": "karak-mainnet"
+    },
+    {
         "chainId": 2415,
         "faucets": [],
         "infoURL": "https://xo-dex.com",
         "name": "XODEX",
         "nativeCurrency": {
             "decimals": 18,
             "name": "XODEX Native Token",
@@ -8573,14 +10485,83 @@
         "rpc": [
             "https://mainnet.xo-dex.com/rpc",
             "https://xo-dex.io"
         ],
         "shortName": "xodex"
     },
     {
+        "chainId": 2425,
+        "faucets": [],
+        "infoURL": "https://kingoflegends.net/",
+        "name": "King Of Legends Devnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "King Of Legends",
+            "symbol": "KOL"
+        },
+        "networkId": 2425,
+        "rpc": [
+            "https://rpc-devnet.kinggamer.org/"
+        ],
+        "shortName": "kol"
+    },
+    {
+        "chainId": 2442,
+        "faucets": [],
+        "infoURL": "https://polygon.technology/polygon-zkevm",
+        "name": "Polygon zkEVM Cardona Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 2442,
+        "rpc": [
+            "https://rpc.cardona.zkevm-rpc.com"
+        ],
+        "shortName": "zkevm-testnet-cardona"
+    },
+    {
+        "chainId": 2458,
+        "faucets": [
+            "https://faucet-testnet.hybridchain.ai"
+        ],
+        "infoURL": "https://hybridchain.ai",
+        "name": "Hybrid Chain Network Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Hybrid Chain Native Token",
+            "symbol": "tHRC"
+        },
+        "networkId": 2458,
+        "rpc": [
+            "https://rpc-testnet.hybridchain.ai/"
+        ],
+        "shortName": "thrc"
+    },
+    {
+        "chainId": 2468,
+        "faucets": [
+            "https://faucet-testnet.hybridchain.ai"
+        ],
+        "infoURL": "https://hybridchain.ai",
+        "name": "Hybrid Chain Network Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Hybrid Chain Native Token",
+            "symbol": "HRC"
+        },
+        "networkId": 2468,
+        "rpc": [
+            "https://coredata-mainnet.hybridchain.ai/",
+            "https://rpc-mainnet.hybridchain.ai"
+        ],
+        "shortName": "hrc"
+    },
+    {
         "chainId": 2484,
         "faucets": [
             "https://faucet.uniultra.xyz"
         ],
         "infoURL": "https://uniultra.xyz",
         "name": "Unicorn Ultra Nebulas Testnet",
         "nativeCurrency": {
@@ -8591,14 +10572,62 @@
         "networkId": 2484,
         "rpc": [
             "https://rpc-nebulas-testnet.uniultra.xyz"
         ],
         "shortName": "u2u_nebulas"
     },
     {
+        "chainId": 2511,
+        "faucets": [],
+        "infoURL": "https://karak.network",
+        "name": "Karak Goerli",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Karak",
+            "symbol": "KRK"
+        },
+        "networkId": 2511,
+        "rpc": [
+            "https://goerli.node1.karak.network"
+        ],
+        "shortName": "karak-goerli"
+    },
+    {
+        "chainId": 2522,
+        "faucets": [],
+        "infoURL": "https://testnet.frax.com",
+        "name": "Fraxtal Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Frax Ether",
+            "symbol": "frxETH"
+        },
+        "networkId": 2522,
+        "rpc": [
+            "https://rpc.testnet.frax.com"
+        ],
+        "shortName": "fraxtal-testnet"
+    },
+    {
+        "chainId": 2525,
+        "faucets": [],
+        "infoURL": "https://inevm.com",
+        "name": "inEVM Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Injective",
+            "symbol": "INJ"
+        },
+        "networkId": 2525,
+        "rpc": [
+            "https://mainnet.rpc.inevm.com/http"
+        ],
+        "shortName": "inevm"
+    },
+    {
         "chainId": 2559,
         "faucets": [],
         "infoURL": "https://www.kortho.io/",
         "name": "Kortho Mainnet",
         "nativeCurrency": {
             "decimals": 11,
             "name": "KorthoChain",
@@ -8692,46 +10721,141 @@
             "https://testnet-api.ezchain.com/ext/bc/C/rpc"
         ],
         "shortName": "Fuji-EZChain"
     },
     {
         "chainId": 2625,
         "faucets": [
-            "https://explorer.whitebit.network/testnet/faucet"
+            "https://testnet.whitechain.io/faucet"
         ],
-        "infoURL": "https://whitebit.com/wbt",
-        "name": "WhiteBIT Network Testnet",
+        "infoURL": "https://whitechain.io",
+        "name": "Whitechain Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "WhiteBIT Coin",
             "symbol": "WBT"
         },
         "networkId": 2625,
         "rpc": [
-            "https://rpc-testnet.whitebit.network"
+            "https://rpc-testnet.whitechain.io"
         ],
         "shortName": "twbt"
     },
     {
+        "chainId": 2662,
+        "faucets": [],
+        "infoURL": "https://apexlayer.xyz/",
+        "name": "APEX",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 2662,
+        "rpc": [],
+        "shortName": "apexmainnet"
+    },
+    {
         "chainId": 2710,
         "faucets": [],
-        "infoURL": "https://morphism.xyz",
-        "name": "Morphism Testnet",
+        "infoURL": "https://morphl2.io",
+        "name": "Morph Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Ether",
             "symbol": "ETH"
         },
         "networkId": 2710,
         "rpc": [
-            "https://rpc-testnet.morphism.xyz"
+            "https://rpc-testnet.morphl2.io"
         ],
         "shortName": "tmorph"
     },
     {
+        "chainId": 2718,
+        "faucets": [],
+        "infoURL": "https://www.laosfoundation.io/",
+        "name": "K-LAOS",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "KLAOS",
+            "symbol": "KLAOS"
+        },
+        "networkId": 2718,
+        "rpc": [
+            "https://rpc.klaos.laosfoundation.io",
+            "wss://rpc.klaos.laosfoundation.io"
+        ],
+        "shortName": "k-laos"
+    },
+    {
+        "chainId": 2730,
+        "faucets": [],
+        "infoURL": "https://xr-one.gitbook.io",
+        "name": "XR Sepolia",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "tXR",
+            "symbol": "tXR"
+        },
+        "networkId": 2730,
+        "rpc": [
+            "https://xr-sepolia-testnet.rpc.caldera.xyz/http"
+        ],
+        "shortName": "txr"
+    },
+    {
+        "chainId": 2731,
+        "faucets": [],
+        "infoURL": "https://whitepaper.anttime.net/overview/anttime",
+        "name": "Elizabeth Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "TIME",
+            "symbol": "TIME"
+        },
+        "networkId": 2731,
+        "rpc": [
+            "https://testnet-rpc.timenetwork.io"
+        ],
+        "shortName": "TIME"
+    },
+    {
+        "chainId": 2748,
+        "faucets": [],
+        "infoURL": "https://www.nanon.network",
+        "name": "Nanon",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 2748,
+        "rpc": [
+            "https://rpc.nanon.network"
+        ],
+        "shortName": "Nanon"
+    },
+    {
+        "chainId": 2810,
+        "faucets": [],
+        "infoURL": "https://morphl2.io",
+        "name": "Morph Holesky",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 2810,
+        "rpc": [
+            "https://rpc-holesky.morphl2.io"
+        ],
+        "shortName": "hmorph"
+    },
+    {
         "chainId": 2888,
         "faucets": [],
         "infoURL": "https://boba.network",
         "name": "Boba Network Goerli Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Goerli Ether",
@@ -8741,14 +10865,65 @@
         "rpc": [
             "https://goerli.boba.network/",
             "wss://wss.goerli.boba.network/"
         ],
         "shortName": "BobaGoerli"
     },
     {
+        "chainId": 2907,
+        "faucets": [],
+        "infoURL": "https://eluxscan.com",
+        "name": "Elux Chain",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Elux Chain",
+            "symbol": "ELUX"
+        },
+        "networkId": 2907,
+        "rpc": [
+            "https://rpc.eluxscan.com"
+        ],
+        "shortName": "ELUX"
+    },
+    {
+        "chainId": 2911,
+        "faucets": [],
+        "infoURL": "https://www.hychain.com",
+        "name": "HYCHAIN",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "TOPIA",
+            "symbol": "TOPIA"
+        },
+        "networkId": 2911,
+        "rpc": [
+            "https://rpc.hychain.com/http"
+        ],
+        "shortName": "hychain"
+    },
+    {
+        "chainId": 2941,
+        "faucets": [
+            "https://xfaucet.xenonchain.com"
+        ],
+        "infoURL": "https://xenonchain.com",
+        "name": "Xenon Chain Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Xenon Testnet",
+            "symbol": "tXEN"
+        },
+        "networkId": 2941,
+        "rpc": [
+            "https://testnet-chain.xenonchain.com/",
+            "https://testnet-dev.xenonchain.com/"
+        ],
+        "shortName": "xenon"
+    },
+    {
         "chainId": 2999,
         "faucets": [],
         "infoURL": "https://www.bityuan.com",
         "name": "BitYuan Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "BTY",
@@ -8839,44 +11014,74 @@
         "networkId": 3031,
         "rpc": [
             "https://rpc-testnet.orlchain.com"
         ],
         "shortName": "ORL"
     },
     {
+        "chainId": 3033,
+        "faucets": [],
+        "infoURL": "https://www.rebuschain.com",
+        "name": "Rebus Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Rebus",
+            "symbol": "REBUS"
+        },
+        "networkId": 3033,
+        "rpc": [
+            "https://testnet.rebus.money/rpc"
+        ],
+        "shortName": "rebus-testnet"
+    },
+    {
         "chainId": 3068,
         "faucets": [],
-        "infoURL": "https://thebifrost.io",
+        "infoURL": "https://bifrostnetwork.com",
         "name": "Bifrost Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Bifrost",
             "symbol": "BFC"
         },
         "networkId": 3068,
         "rpc": [
-            "https://public-01.mainnet.thebifrost.io/rpc",
-            "https://public-02.mainnet.thebifrost.io/rpc"
+            "https://public-01.mainnet.bifrostnetwork.com/rpc",
+            "https://public-02.mainnet.bifrostnetwork.com/rpc"
         ],
         "shortName": "bfc"
     },
     {
+        "chainId": 3073,
+        "faucets": [],
+        "infoURL": "https://movementlabs.xyz",
+        "name": "Movement EVM",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Move",
+            "symbol": "MOVE"
+        },
+        "networkId": 3073,
+        "rpc": [],
+        "shortName": "move"
+    },
+    {
         "chainId": 3100,
         "faucets": [],
         "infoURL": "https://immu3.io",
         "name": "Immu3 EVM",
         "nativeCurrency": {
             "decimals": 18,
             "name": "IMMU",
             "symbol": "IMMU"
         },
         "networkId": 3100,
         "rpc": [
-            "https://fraa-dancebox-3043-rpc.a.dancebox.tanssi.network",
-            "wss://fraa-dancebox-3043-rpc.a.dancebox.tanssi.network"
+            "https://fraa-flashbox-2800-rpc.a.stagenet.tanssi.network",
+            "wss://fraa-flashbox-2800-rpc.a.stagenet.tanssi.network"
         ],
         "shortName": "Immu3"
     },
     {
         "chainId": 3102,
         "faucets": [],
         "infoURL": "https://vulture.finance",
@@ -8890,14 +11095,46 @@
         "rpc": [
             "https://fraa-dancebox-3050-rpc.a.dancebox.tanssi.network",
             "wss://fraa-dancebox-3050-rpc.a.dancebox.tanssi.network"
         ],
         "shortName": "VFI"
     },
     {
+        "chainId": 3109,
+        "faucets": [],
+        "infoURL": "https://www.satoshivm.io/",
+        "name": "SatoshiVM Alpha Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "BTC",
+            "symbol": "BTC"
+        },
+        "networkId": 3109,
+        "rpc": [
+            "https://alpha-rpc-node-http.svmscan.io"
+        ],
+        "shortName": "SAVM"
+    },
+    {
+        "chainId": 3110,
+        "faucets": [],
+        "infoURL": "https://www.satoshivm.io/",
+        "name": "SatoshiVM Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "BTC",
+            "symbol": "BTC"
+        },
+        "networkId": 3110,
+        "rpc": [
+            "https://test-rpc-node-http.svmscan.io"
+        ],
+        "shortName": "tSAVM"
+    },
+    {
         "chainId": 3141,
         "faucets": [],
         "infoURL": "https://filecoin.io",
         "name": "Filecoin - Hyperspace testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "testnet filecoin",
@@ -8974,26 +11211,26 @@
             "https://rpc-testnet.zcore.cash"
         ],
         "shortName": "zcrbeach"
     },
     {
         "chainId": 3333,
         "faucets": [],
-        "infoURL": "https://testnet.web3q.io/home.w3q/",
-        "name": "Web3Q Testnet",
+        "infoURL": "https://ethstorage.io/",
+        "name": "EthStorage Testnet",
         "nativeCurrency": {
             "decimals": 18,
-            "name": "Web3Q",
-            "symbol": "W3Q"
+            "name": "Ether",
+            "symbol": "ETH"
         },
         "networkId": 3333,
         "rpc": [
-            "https://testnet.web3q.io:8545"
+            "http://testnet.ethstorage.io:9540"
         ],
-        "shortName": "w3q-t"
+        "shortName": "es-t"
     },
     {
         "chainId": 3334,
         "faucets": [],
         "infoURL": "https://galileo.web3q.io/home.w3q/",
         "name": "Web3Q Galileo",
         "nativeCurrency": {
@@ -9020,14 +11257,30 @@
         "networkId": 3400,
         "rpc": [
             "https://rpc.paribu.network"
         ],
         "shortName": "prb"
     },
     {
+        "chainId": 3424,
+        "faucets": [],
+        "infoURL": "https://evolveblockchain.io",
+        "name": "EVOLVE Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Evolve",
+            "symbol": "EVO"
+        },
+        "networkId": 3424,
+        "rpc": [
+            "https://rpc.evolveblockchain.io"
+        ],
+        "shortName": "EVOm"
+    },
+    {
         "chainId": 3434,
         "faucets": [
             "https://faucet.securechain.ai"
         ],
         "infoURL": "https://securechain.ai",
         "name": "SecureChain Testnet",
         "nativeCurrency": {
@@ -9063,21 +11316,21 @@
         "chainId": 3501,
         "faucets": [],
         "infoURL": "https://jfinchain.com",
         "name": "JFIN Chain",
         "nativeCurrency": {
             "decimals": 18,
             "name": "JFIN Coin",
-            "symbol": "jfin"
+            "symbol": "JFIN"
         },
         "networkId": 3501,
         "rpc": [
             "https://rpc.jfinchain.com"
         ],
-        "shortName": "jfin"
+        "shortName": "JFIN"
     },
     {
         "chainId": 3601,
         "faucets": [],
         "infoURL": "https://www.pandoproject.org/",
         "name": "PandoProject Mainnet",
         "nativeCurrency": {
@@ -9277,31 +11530,87 @@
         "networkId": 3737,
         "rpc": [
             "https://rpc.crossbell.io"
         ],
         "shortName": "csb"
     },
     {
+        "chainId": 3776,
+        "faucets": [],
+        "infoURL": "https://astar.network",
+        "name": "Astar zkEVM",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 3776,
+        "rpc": [
+            "https://rpc.startale.com/astar-zkevm"
+        ],
+        "shortName": "astrzk"
+    },
+    {
         "chainId": 3797,
         "faucets": [],
-        "infoURL": "https://alveyscan.com/rpc",
+        "infoURL": "https://alveychain.com/",
         "name": "AlveyChain Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "AlveyCoin",
             "symbol": "ALV"
         },
         "networkId": 3797,
         "rpc": [
-            "https://rpc.alveychain.com/rpc",
-            "https://rpc2.alvey.io/rpc"
+            "https://elves-core1.alvey.io",
+            "https://elves-core2.alvey.io",
+            "https://elves-core3.alvey.io"
         ],
         "shortName": "alv"
     },
     {
+        "chainId": 3799,
+        "faucets": [
+            "https://faucet.tangle.tools"
+        ],
+        "infoURL": "https://docs.tangle.tools",
+        "name": "Tangle Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Testnet Tangle Network Token",
+            "symbol": "tTNT"
+        },
+        "networkId": 3799,
+        "rpc": [
+            "https://testnet-rpc.tangle.tools",
+            "https://testnet-rpc-archive.tangle.tools",
+            "wss://testnet-rpc.tangle.tools",
+            "wss://testnet-rpc-archive.tangle.tools"
+        ],
+        "shortName": "tTangle"
+    },
+    {
+        "chainId": 3885,
+        "faucets": [
+            "zkevm-faucet.thefirechain.com"
+        ],
+        "infoURL": "https://docs.thefirechain.com/",
+        "name": "Firechain zkEVM Ghostrider",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 3885,
+        "rpc": [
+            "https://rpc-zkevm-ghostrider.thefirechain.com"
+        ],
+        "shortName": "firechain-zkEVM-testnet"
+    },
+    {
         "chainId": 3888,
         "faucets": [],
         "infoURL": "https://kalychain.io",
         "name": "KalyChain Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "KalyCoin",
@@ -9396,14 +11705,32 @@
         "networkId": 3967,
         "rpc": [
             "https://tapi.dynoprotocol.com"
         ],
         "shortName": "tdyno"
     },
     {
+        "chainId": 3993,
+        "faucets": [
+            "https://sepoliafaucet.com/"
+        ],
+        "infoURL": "https://docs.apexlayer.xyz/",
+        "name": "APEX Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Sepolia Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 3993,
+        "rpc": [
+            "https://rpc-testnet.apexlayer.xyz"
+        ],
+        "shortName": "apexsep"
+    },
+    {
         "chainId": 3999,
         "faucets": [],
         "infoURL": "https://www.yuan.org",
         "name": "YuanChain Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "YCC",
@@ -9458,20 +11785,54 @@
             "decimals": 18,
             "name": "Fantom",
             "symbol": "FTM"
         },
         "networkId": 4002,
         "rpc": [
             "https://rpc.testnet.fantom.network",
-            "https://fantom-testnet.publicnode.com",
-            "wss://fantom-testnet.publicnode.com"
+            "https://fantom-testnet-rpc.publicnode.com",
+            "wss://fantom-testnet-rpc.publicnode.com",
+            "https://fantom-testnet.drpc.org",
+            "wss://fantom-testnet.drpc.org"
         ],
         "shortName": "tftm"
     },
     {
+        "chainId": 4003,
+        "faucets": [],
+        "infoURL": "https://docs.xen.network/go-x1/",
+        "name": "X1 Fastnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "XN",
+            "symbol": "XN"
+        },
+        "networkId": 4003,
+        "rpc": [
+            "https://x1-fastnet.xen.network"
+        ],
+        "shortName": "x1-fastnet"
+    },
+    {
+        "chainId": 4048,
+        "faucets": [],
+        "infoURL": "https://docs.gpu.net/",
+        "name": "GAN Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "GP Token",
+            "symbol": "GP"
+        },
+        "networkId": 4048,
+        "rpc": [
+            "https://rpc.gpu.net"
+        ],
+        "shortName": "GANTestnet"
+    },
+    {
         "chainId": 4051,
         "faucets": [],
         "infoURL": "https://boba.network",
         "name": "Bobaopera Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Boba Token",
@@ -9513,14 +11874,30 @@
         "networkId": 4062,
         "rpc": [
             "https://ngeth.testnet.n3.nahmii.io"
         ],
         "shortName": "Nahmii3Testnet"
     },
     {
+        "chainId": 4078,
+        "faucets": [],
+        "infoURL": "",
+        "name": "Muster Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 4078,
+        "rpc": [
+            "https://muster.alt.technology"
+        ],
+        "shortName": "muster"
+    },
+    {
         "chainId": 4090,
         "faucets": [
             "https://faucet.oasis.fastexchain.com"
         ],
         "infoURL": "https://fastexchain.com",
         "name": "Fastex Chain (Bahamut) Oasis Testnet",
         "nativeCurrency": {
@@ -9617,14 +11994,30 @@
         "networkId": 4141,
         "rpc": [
             "https://testnet-rpc.tipboxcoin.net"
         ],
         "shortName": "TPBXt"
     },
     {
+        "chainId": 4157,
+        "faucets": [],
+        "infoURL": "https://crossfi.org/",
+        "name": "CrossFi Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "XFI",
+            "symbol": "XFI"
+        },
+        "networkId": 4157,
+        "rpc": [
+            "https://rpc.testnet.ms"
+        ],
+        "shortName": "crossfi-testnet"
+    },
+    {
         "chainId": 4181,
         "faucets": [],
         "infoURL": "https://phi.network",
         "name": "PHI Network V1",
         "nativeCurrency": {
             "decimals": 18,
             "name": "PHI",
@@ -9634,14 +12027,31 @@
         "rpc": [
             "https://rpc1.phi.network",
             "https://rpc2.phi.network"
         ],
         "shortName": "PHIv1"
     },
     {
+        "chainId": 4200,
+        "faucets": [],
+        "infoURL": "https://merlinchain.io",
+        "name": "Merlin Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "BTC",
+            "symbol": "BTC"
+        },
+        "networkId": 4200,
+        "rpc": [
+            "https://rpc.merlinchain.io",
+            "https://merlin-mainnet-enterprise.unifra.io"
+        ],
+        "shortName": "Merlin-Mainnet"
+    },
+    {
         "chainId": 4201,
         "faucets": [
             "https://faucet.testnet.lukso.network"
         ],
         "infoURL": "https://lukso.network",
         "name": "LUKSO Testnet",
         "nativeCurrency": {
@@ -9653,14 +12063,30 @@
         "rpc": [
             "https://rpc.testnet.lukso.network",
             "wss://ws-rpc.testnet.lukso.network"
         ],
         "shortName": "lukso-testnet"
     },
     {
+        "chainId": 4202,
+        "faucets": [],
+        "infoURL": "https://lisk.com",
+        "name": "Lisk Sepolia Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Sepolia Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 4202,
+        "rpc": [
+            "https://rpc.sepolia-api.lisk.com"
+        ],
+        "shortName": "lisksep"
+    },
+    {
         "chainId": 4242,
         "faucets": [],
         "infoURL": "https://www.nexi.technology/",
         "name": "Nexi Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Nexi",
@@ -9671,14 +12097,31 @@
             "https://rpc.chain.nexi.technology/",
             "https://chain.nexilix.com",
             "https://chain.nexi.evmnode.online"
         ],
         "shortName": "nexi"
     },
     {
+        "chainId": 4243,
+        "faucets": [],
+        "infoURL": "https://www.nexi.technology/",
+        "name": "Nexi V2 Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "NexiV2",
+            "symbol": "NEXI"
+        },
+        "networkId": 4243,
+        "rpc": [
+            "https://chain.nexiv2.nexilix.com",
+            "https://rpc.chainv1.nexi.technology"
+        ],
+        "shortName": "NexiV2"
+    },
+    {
         "chainId": 4328,
         "faucets": [],
         "infoURL": "https://boba.network",
         "name": "Bobafuji Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Boba Token",
@@ -9702,20 +12145,38 @@
         "nativeCurrency": {
             "decimals": 18,
             "name": "Beam",
             "symbol": "BEAM"
         },
         "networkId": 4337,
         "rpc": [
+            "https://build.onbeam.com/rpc",
+            "wss://build.onbeam.com/ws",
             "https://subnets.avax.network/beam/mainnet/rpc",
             "wss://subnets.avax.network/beam/mainnet/ws"
         ],
         "shortName": "beam"
     },
     {
+        "chainId": 4400,
+        "faucets": [],
+        "infoURL": "https://creditsmartchain.com",
+        "name": "Credit Smart Chain Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Credit",
+            "symbol": "CREDIT"
+        },
+        "networkId": 4400,
+        "rpc": [
+            "https://rpc.creditsmartchain.com"
+        ],
+        "shortName": "CreditEdge"
+    },
+    {
         "chainId": 4444,
         "faucets": [
             "https://gruvin.me/htmlcoin"
         ],
         "infoURL": "https://htmlcoin.com",
         "name": "Htmlcoin Mainnet",
         "nativeCurrency": {
@@ -9742,14 +12203,64 @@
         "networkId": 4460,
         "rpc": [
             "https://l2-orderly-l2-4460-sepolia-8tc3sd7dvy.t.conduit.xyz"
         ],
         "shortName": "orderlyl2"
     },
     {
+        "chainId": 4544,
+        "faucets": [
+            "https://faucet.emoney.network/faucet"
+        ],
+        "infoURL": "https://emoney.network/",
+        "name": "Emoney Network Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Emoney Network",
+            "symbol": "EMYC"
+        },
+        "networkId": 4544,
+        "rpc": [
+            "https://testnet.emoney.network/"
+        ],
+        "shortName": "emoney"
+    },
+    {
+        "chainId": 4613,
+        "faucets": [],
+        "infoURL": "https://www.verylabs.io/",
+        "name": "VERY Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "VERY",
+            "symbol": "VERY"
+        },
+        "networkId": 4613,
+        "rpc": [
+            "https://rpc.verylabs.io"
+        ],
+        "shortName": "very"
+    },
+    {
+        "chainId": 4653,
+        "faucets": [],
+        "infoURL": "https://gold.dev",
+        "name": "Gold Chain",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 4653,
+        "rpc": [
+            "https://chain-rpc.gold.dev"
+        ],
+        "shortName": "gold"
+    },
+    {
         "chainId": 4689,
         "faucets": [],
         "infoURL": "https://iotex.io",
         "name": "IoTeX Network Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "IoTeX",
@@ -9808,14 +12319,30 @@
         "networkId": 4777,
         "rpc": [
             "https://testnet.blackfort.network/rpc"
         ],
         "shortName": "TBXN"
     },
     {
+        "chainId": 4893,
+        "faucets": [],
+        "infoURL": "https://gcscan.io",
+        "name": "Globel Chain",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Globel Chain",
+            "symbol": "GC"
+        },
+        "networkId": 4893,
+        "rpc": [
+            "https://rpc.gcscan.io"
+        ],
+        "shortName": "GC"
+    },
+    {
         "chainId": 4918,
         "faucets": [],
         "infoURL": "https://venidium.io",
         "name": "Venidium Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Venidium",
@@ -9871,16 +12398,16 @@
             "decimals": 18,
             "name": "Mantle",
             "symbol": "MNT"
         },
         "networkId": 5000,
         "rpc": [
             "https://rpc.mantle.xyz",
-            "https://mantle.publicnode.com",
-            "wss://mantle.publicnode.com"
+            "https://mantle-rpc.publicnode.com",
+            "wss://mantle-rpc.publicnode.com"
         ],
         "shortName": "mantle"
     },
     {
         "chainId": 5001,
         "faucets": [
             "https://faucet.testnet.mantle.xyz"
@@ -9951,33 +12478,195 @@
             "https://node1.testnet.treasurenet.io",
             "https://node2.testnet.treasurenet.io",
             "https://node3.testnet.treasurenet.io"
         ],
         "shortName": "tntest"
     },
     {
+        "chainId": 5039,
+        "faucets": [],
+        "infoURL": "https://www.ongr.org/",
+        "name": "ONIGIRI Test Subnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "ONIGIRI",
+            "symbol": "ONGR"
+        },
+        "networkId": 5039,
+        "rpc": [
+            "https://subnets.avax.network/onigiri/testnet/rpc"
+        ],
+        "shortName": "onigiri"
+    },
+    {
+        "chainId": 5051,
+        "faucets": [],
+        "infoURL": "",
+        "name": "Nollie Skatechain Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 5051,
+        "rpc": [
+            "https://nollie-rpc.skatechain.org/"
+        ],
+        "shortName": "nollie-testnet"
+    },
+    {
+        "chainId": 5100,
+        "faucets": [],
+        "infoURL": "https://syndicate.io",
+        "name": "Syndicate Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "S-Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 5100,
+        "rpc": [
+            "https://rpc-testnet.syndicate.io"
+        ],
+        "shortName": "syndicate-chain-testnet"
+    },
+    {
+        "chainId": 5101,
+        "faucets": [],
+        "infoURL": "https://syndicate.io",
+        "name": "Syndicate Frame Chain",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 5101,
+        "rpc": [
+            "https://rpc-frame.syndicate.io"
+        ],
+        "shortName": "syndicate-chain-frame"
+    },
+    {
+        "chainId": 5102,
+        "faucets": [],
+        "infoURL": "https://www.fwb.help/",
+        "name": "SIC Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "ETH",
+            "symbol": "ETH"
+        },
+        "networkId": 5102,
+        "rpc": [
+            "https://rpc-sic-testnet-zvr7tlkzsi.t.conduit.xyz"
+        ],
+        "shortName": "sic-testnet"
+    },
+    {
+        "chainId": 5103,
+        "faucets": [],
+        "infoURL": "https://coordinape.com/",
+        "name": "Coordinape Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "ETH",
+            "symbol": "ETH"
+        },
+        "networkId": 5103,
+        "rpc": [
+            "https://rpc-coordinape-testnet-vs9se3oc4v.t.conduit.xyz"
+        ],
+        "shortName": "coordinape-testnet"
+    },
+    {
+        "chainId": 5104,
+        "faucets": [],
+        "infoURL": "https://charmverse.io/",
+        "name": "Charmverse Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "ETH",
+            "symbol": "ETH"
+        },
+        "networkId": 5104,
+        "rpc": [
+            "https://rpc-charmverse-testnet-g6blnaebes.t.conduit.xyz"
+        ],
+        "shortName": "charmverse-testnet"
+    },
+    {
+        "chainId": 5105,
+        "faucets": [],
+        "infoURL": "https://www.superloyal.com/",
+        "name": "Superloyalty Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "ETH",
+            "symbol": "ETH"
+        },
+        "networkId": 5105,
+        "rpc": [
+            "https://rpc-superloyalty-testnet-1m5gwjbsv1.t.conduit.xyz"
+        ],
+        "shortName": "superloyalty-testnet"
+    },
+    {
+        "chainId": 5106,
+        "faucets": [],
+        "infoURL": "https://azragames.com",
+        "name": "Azra Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "ETH",
+            "symbol": "ETH"
+        },
+        "networkId": 5106,
+        "rpc": [
+            "https://rpc-azra-testnet-6hz86owb1n.t.conduit.xyz"
+        ],
+        "shortName": "azra-testnet"
+    },
+    {
         "chainId": 5165,
         "faucets": [],
         "infoURL": "https://bahamut.io",
         "name": "Bahamut",
         "nativeCurrency": {
             "decimals": 18,
             "name": "FTN",
             "symbol": "FTN"
         },
         "networkId": 5165,
         "rpc": [
             "https://rpc1.bahamut.io",
             "https://rpc2.bahamut.io",
             "wss://ws1.sahara.bahamutchain.com",
-            "wss://ws2.sahara.bahamutchain.com"
+            "wss://ws2.sahara.bahamutchain.com",
+            "https://bahamut-rpc.publicnode.com",
+            "wss://bahamut-rpc.publicnode.com"
         ],
         "shortName": "ftn"
     },
     {
+        "chainId": 5169,
+        "faucets": [],
+        "infoURL": "https://www.smartlayer.network/",
+        "name": "Smart Layer Network",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Service Unit Token",
+            "symbol": "SU"
+        },
+        "networkId": 5169,
+        "rpc": [
+            "https://rpc.main.smartlayer.network"
+        ],
+        "shortName": "SLN"
+    },
+    {
         "chainId": 5177,
         "faucets": [],
         "infoURL": "https://tlchain.network/",
         "name": "TLChain Network Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "TLChain Network",
@@ -10051,14 +12740,30 @@
         "networkId": 5315,
         "rpc": [
             "https://network.uzmigames.com.br/"
         ],
         "shortName": "UZMI"
     },
     {
+        "chainId": 5317,
+        "faucets": [],
+        "infoURL": "https://optrust.io",
+        "name": "OpTrust Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "TestBSC",
+            "symbol": "tBNB"
+        },
+        "networkId": 5317,
+        "rpc": [
+            "https://rpctest.optrust.io"
+        ],
+        "shortName": "toptrust"
+    },
+    {
         "chainId": 5353,
         "faucets": [
             "https://faucet.tritanium.network"
         ],
         "infoURL": "https://tritanium.network",
         "name": "Tritanium Testnet",
         "nativeCurrency": {
@@ -10070,14 +12775,48 @@
         "rpc": [
             "https://nodetestnet-station-one.tritanium.network/",
             "https://nodetestnet-station-two.tritanium.network/"
         ],
         "shortName": "ttrn"
     },
     {
+        "chainId": 5424,
+        "faucets": [],
+        "infoURL": "https://edexa.network/",
+        "name": "edeXa Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "EDEXA",
+            "symbol": "EDX"
+        },
+        "networkId": 5424,
+        "rpc": [
+            "https://mainnet.edexa.network/rpc",
+            "https://mainnet.edexa.com/rpc",
+            "https://io-dataseed1.mainnet.edexa.io-market.com/rpc"
+        ],
+        "shortName": "edeXa"
+    },
+    {
+        "chainId": 5439,
+        "faucets": [],
+        "infoURL": "https://docs.egochain.org/",
+        "name": "Egochain",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "EGAX",
+            "symbol": "EGAX"
+        },
+        "networkId": 5439,
+        "rpc": [
+            "https://mainnet.egochain.org"
+        ],
+        "shortName": "egax"
+    },
+    {
         "chainId": 5522,
         "faucets": [
             "https://t.me/vexfaucetbot"
         ],
         "infoURL": "https://vexanium.com",
         "name": "VEX EVM TESTNET",
         "nativeCurrency": {
@@ -10153,19 +12892,39 @@
         },
         "networkId": 5611,
         "rpc": [
             "https://opbnb-testnet-rpc.bnbchain.org",
             "https://opbnb-testnet.nodereal.io/v1/64a9df0874fb4a93b9d0a3849de012d3",
             "wss://opbnb-testnet.nodereal.io/ws/v1/64a9df0874fb4a93b9d0a3849de012d3",
             "https://opbnb-testnet.nodereal.io/v1/e9a36765eb8a40b9bd12e680a1fd2bc5",
-            "wss://opbnb-testnet.nodereal.io/ws/v1/e9a36765eb8a40b9bd12e680a1fd2bc5"
+            "wss://opbnb-testnet.nodereal.io/ws/v1/e9a36765eb8a40b9bd12e680a1fd2bc5",
+            "https://opbnb-testnet-rpc.publicnode.com",
+            "wss://opbnb-testnet-rpc.publicnode.com"
         ],
         "shortName": "obnbt"
     },
     {
+        "chainId": 5615,
+        "faucets": [
+            "https://faucet.arcturuschain.io"
+        ],
+        "infoURL": "https://arcturuschain.io",
+        "name": "Arcturus Testneet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "tARC",
+            "symbol": "tARC"
+        },
+        "networkId": 5615,
+        "rpc": [
+            "https://rpc-testnet.arcturuschain.io/"
+        ],
+        "shortName": "arcturus-testnet"
+    },
+    {
         "chainId": 5616,
         "faucets": [],
         "infoURL": "https://arcturuschain.io",
         "name": "Arcturus Chain Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Test Arct",
@@ -10174,29 +12933,62 @@
         "networkId": 5616,
         "rpc": [
             "http://185.99.196.3:8545"
         ],
         "shortName": "ARCT"
     },
     {
+        "chainId": 5656,
+        "faucets": [],
+        "infoURL": "https://qiblockchain.online/",
+        "name": "QIE Blockchain",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "QIE Blockchain",
+            "symbol": "QIE"
+        },
+        "networkId": 5656,
+        "rpc": [
+            "https://rpc-main1.qiblockchain.online/",
+            "https://rpc-main2.qiblockchain.online/"
+        ],
+        "shortName": "QIE"
+    },
+    {
+        "chainId": 5675,
+        "faucets": [],
+        "infoURL": "https://filenova.org",
+        "name": "Filenova Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Test Filecoin",
+            "symbol": "tFIL"
+        },
+        "networkId": 5675,
+        "rpc": [
+            "https://rpctest.filenova.org"
+        ],
+        "shortName": "tfilenova"
+    },
+    {
         "chainId": 5678,
         "faucets": [],
-        "infoURL": "https://tanssi.network",
-        "name": "Tanssi EVM ContainerChain",
+        "infoURL": "https://docs.tanssi.network/builders/tanssi-network/networks/dancebox/demo-evm-containerchain",
+        "name": "Tanssi Demo",
         "nativeCurrency": {
             "decimals": 18,
-            "name": "Unit",
-            "symbol": "Unit"
+            "name": "TANGO",
+            "symbol": "TANGO"
         },
         "networkId": 5678,
         "rpc": [
             "https://fraa-dancebox-3001-rpc.a.dancebox.tanssi.network",
             "wss://fraa-dancebox-3001-rpc.a.dancebox.tanssi.network"
         ],
-        "shortName": "TanssiCC"
+        "shortName": "tango"
     },
     {
         "chainId": 5700,
         "faucets": [
             "https://faucet.tanenbaum.io"
         ],
         "infoURL": "https://syscoin.org",
@@ -10262,14 +13054,31 @@
         "networkId": 5777,
         "rpc": [
             "https://127.0.0.1:7545"
         ],
         "shortName": "ggui"
     },
     {
+        "chainId": 5845,
+        "faucets": [],
+        "infoURL": "https://docs.tangle.tools",
+        "name": "Tangle",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Tangle",
+            "symbol": "TNT"
+        },
+        "networkId": 5845,
+        "rpc": [
+            "https://rpc.tangle.tools",
+            "wss://rpc.tangle.tools"
+        ],
+        "shortName": "tangle"
+    },
+    {
         "chainId": 5851,
         "faucets": [
             "https://developer.ont.io/"
         ],
         "infoURL": "https://ont.io/",
         "name": "Ontology Testnet",
         "nativeCurrency": {
@@ -10304,14 +13113,46 @@
         "rpc": [
             "https://proxy.wegochain.io",
             "http://wallet.wegochain.io:7764"
         ],
         "shortName": "rbd"
     },
     {
+        "chainId": 6000,
+        "faucets": [],
+        "infoURL": "https://bouncebit.io",
+        "name": "BounceBit Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "BounceBit",
+            "symbol": "BB"
+        },
+        "networkId": 6000,
+        "rpc": [
+            "https://fullnode-testnet.bouncebitapi.com/"
+        ],
+        "shortName": "bouncebit-testnet"
+    },
+    {
+        "chainId": 6001,
+        "faucets": [],
+        "infoURL": "https://bouncebit.io",
+        "name": "BounceBit Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "BounceBit",
+            "symbol": "BB"
+        },
+        "networkId": 6001,
+        "rpc": [
+            "https://fullnode-mainnet.bouncebitapi.com/"
+        ],
+        "shortName": "bouncebit-mainnet"
+    },
+    {
         "chainId": 6065,
         "faucets": [
             "http://faucet.tresleches.finance:8080"
         ],
         "infoURL": "https://treschain.com",
         "name": "Tres Testnet",
         "nativeCurrency": {
@@ -10389,14 +13230,46 @@
         "networkId": 6119,
         "rpc": [
             "https://node-api.uptn.io/v1/ext/rpc"
         ],
         "shortName": "UPTN"
     },
     {
+        "chainId": 6321,
+        "faucets": [],
+        "infoURL": "https://aura.network",
+        "name": "Aura Euphoria Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "test-EAura",
+            "symbol": "eAura"
+        },
+        "networkId": 6321,
+        "rpc": [
+            "https://jsonrpc.euphoria.aura.network"
+        ],
+        "shortName": "eaura"
+    },
+    {
+        "chainId": 6363,
+        "faucets": [],
+        "infoURL": "",
+        "name": "Digit Soul Smart Chain",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Digit Coin",
+            "symbol": "DGC"
+        },
+        "networkId": 6363,
+        "rpc": [
+            "https://dsc-rpc.digitsoul.co.th"
+        ],
+        "shortName": "DGS"
+    },
+    {
         "chainId": 6502,
         "faucets": [],
         "infoURL": "https://peerpay.su.gy",
         "name": "Peerpay",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Peerpay",
@@ -10460,14 +13333,66 @@
         "rpc": [
             "https://http-mainnet.chain.pixie.xyz",
             "wss://ws-mainnet.chain.pixie.xyz"
         ],
         "shortName": "pixie-chain"
     },
     {
+        "chainId": 6660,
+        "faucets": [
+            "http://faucet.latestchain.io"
+        ],
+        "infoURL": "https://latestcoin.io",
+        "name": "Latest Chain Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Latest",
+            "symbol": "LATEST"
+        },
+        "networkId": 6660,
+        "rpc": [
+            "https://testnet-rpc.latestcoin.io"
+        ],
+        "shortName": "LATESTt"
+    },
+    {
+        "chainId": 6661,
+        "faucets": [],
+        "infoURL": "https://cybria.io",
+        "name": "Cybria Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Cybria",
+            "symbol": "CYBA"
+        },
+        "networkId": 6661,
+        "rpc": [
+            "https://rpc-mainnet.cybria.io"
+        ],
+        "shortName": "cyba"
+    },
+    {
+        "chainId": 6666,
+        "faucets": [
+            "https://faucet.cybascan.io"
+        ],
+        "infoURL": "https://cybria.io",
+        "name": "Cybria Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Cybria",
+            "symbol": "CYBA"
+        },
+        "networkId": 6666,
+        "rpc": [
+            "https://l2-rpc.cybascan.io"
+        ],
+        "shortName": "tcyba"
+    },
+    {
         "chainId": 6688,
         "faucets": [],
         "infoURL": "https://www.irisnet.org",
         "name": "IRIShub",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Eris",
@@ -10478,14 +13403,47 @@
             "https://evmrpc.irishub-1.irisnet.org",
             "https://iris-evm.publicnode.com",
             "wss://iris-evm.publicnode.com"
         ],
         "shortName": "iris"
     },
     {
+        "chainId": 6701,
+        "faucets": [],
+        "infoURL": "https://paxb.io/",
+        "name": "PAXB Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "PAXB",
+            "symbol": "PAXB"
+        },
+        "networkId": 6701,
+        "rpc": [
+            "https://chain.paxb.io"
+        ],
+        "shortName": "PAXB"
+    },
+    {
+        "chainId": 6779,
+        "faucets": [],
+        "infoURL": "https://compverse.io",
+        "name": "Compverse Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "compverse",
+            "symbol": "CPV"
+        },
+        "networkId": 6779,
+        "rpc": [
+            "https://rpc.compverse.io/",
+            "https://rpc-useast1.compverse.io/"
+        ],
+        "shortName": "compverse"
+    },
+    {
         "chainId": 6789,
         "faucets": [
             "https://faucet.goldsmartchain.com"
         ],
         "infoURL": "https://goldsmartchain.com",
         "name": "Gold Smart Chain Mainnet",
         "nativeCurrency": {
@@ -10541,15 +13499,16 @@
         "nativeCurrency": {
             "decimals": 18,
             "name": "Zeta",
             "symbol": "ZETA"
         },
         "networkId": 7000,
         "rpc": [
-            "https://api.mainnet.zetachain.com/evm"
+            "https://zetachain-evm.blockpi.network/v1/rpc/public",
+            "https://zetachain-mainnet-archive.allthatnode.com:8545"
         ],
         "shortName": "zetachain-mainnet"
     },
     {
         "chainId": 7001,
         "faucets": [
             "https://labs.zetachain.com/get-zeta"
@@ -10559,19 +13518,37 @@
         "nativeCurrency": {
             "decimals": 18,
             "name": "Zeta",
             "symbol": "ZETA"
         },
         "networkId": 7001,
         "rpc": [
-            "https://rpc.ankr.com/zetachain_evm_athens_testnet"
+            "https://zetachain-athens-evm.blockpi.network/v1/rpc/public",
+            "wss://zetachain-athens.blockpi.network/rpc/v1/public/websocket",
+            "https://zetachain-testnet-archive.allthatnode.com:8545"
         ],
         "shortName": "zetachain-athens"
     },
     {
+        "chainId": 7007,
+        "faucets": [],
+        "infoURL": "https://bstchain.io",
+        "name": "BST Chain",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "BST Chain",
+            "symbol": "BSTC"
+        },
+        "networkId": 7007,
+        "rpc": [
+            "https://rpc.bstchain.io/"
+        ],
+        "shortName": "BSTC"
+    },
+    {
         "chainId": 7027,
         "faucets": [],
         "infoURL": "https://ella.network",
         "name": "Ella the heart",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Ella",
@@ -10596,14 +13573,60 @@
         "networkId": 7070,
         "rpc": [
             "https://evm-rpc.planq.network"
         ],
         "shortName": "planq"
     },
     {
+        "chainId": 7077,
+        "faucets": [],
+        "infoURL": "https://planq.network",
+        "name": "Planq Atlas Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Planq",
+            "symbol": "tPLQ"
+        },
+        "networkId": 7077,
+        "rpc": [
+            "https://evm-rpc-atlas.planq.network"
+        ],
+        "shortName": "planq-atlas-testnet"
+    },
+    {
+        "chainId": 7100,
+        "faucets": [],
+        "infoURL": "https://numecrypto.com",
+        "name": "Nume",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Dai Stablecoin",
+            "symbol": "DAI"
+        },
+        "networkId": 7100,
+        "rpc": [
+            "https://rpc.numecrypto.com"
+        ],
+        "shortName": "nume"
+    },
+    {
+        "chainId": 7118,
+        "faucets": [],
+        "infoURL": "https://hth.world",
+        "name": "Help The Homeless",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Help The Homeless Coin",
+            "symbol": "HTH"
+        },
+        "networkId": 7118,
+        "rpc": [],
+        "shortName": "hth"
+    },
+    {
         "chainId": 7171,
         "faucets": [],
         "infoURL": "https://bit-rock.io",
         "name": "Bitrock Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "BITROCK",
@@ -10696,14 +13719,33 @@
         "networkId": 7518,
         "rpc": [
             "https://rpc.meversemainnet.io"
         ],
         "shortName": "MEV"
     },
     {
+        "chainId": 7560,
+        "faucets": [],
+        "infoURL": "https://cyber.co/",
+        "name": "Cyber Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 7560,
+        "rpc": [
+            "https://cyber.alt.technology/",
+            "wss://cyber-ws.alt.technology/",
+            "https://rpc.cyber.co/",
+            "wss://rpc.cyber.co/"
+        ],
+        "shortName": "cyeth"
+    },
+    {
         "chainId": 7575,
         "faucets": [
             "https://testnet-faucet.adil-scan.io"
         ],
         "infoURL": "https://adilchain.io",
         "name": "ADIL Testnet",
         "nativeCurrency": {
@@ -10776,22 +13818,17 @@
             "decimals": 18,
             "name": "Canto",
             "symbol": "CANTO"
         },
         "networkId": 7700,
         "rpc": [
             "https://canto.slingshot.finance",
-            "https://canto.neobase.one",
+            "https://canto-rpc.ansybl.io",
             "https://mainnode.plexnode.org:8545",
-            "https://canto.gravitychain.io/",
-            "https://canto.evm.chandrastation.com/",
-            "https://jsonrpc.canto.nodestake.top/",
-            "https://canto.dexvaults.com/",
-            "wss://canto.gravitychain.io:8546",
-            "wss://canto.dexvaults.com/ws"
+            "https://canto.gravitychain.io/"
         ],
         "shortName": "canto"
     },
     {
         "chainId": 7701,
         "faucets": [],
         "infoURL": "https://canto.io",
@@ -10822,14 +13859,30 @@
         "networkId": 7771,
         "rpc": [
             "https://testnet.bit-rock.io"
         ],
         "shortName": "tbitrock"
     },
     {
+        "chainId": 7775,
+        "faucets": [],
+        "infoURL": "https://gdcchain.com",
+        "name": "GDCC TESTNET",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "GDCC",
+            "symbol": "GDCC"
+        },
+        "networkId": 7775,
+        "rpc": [
+            "https://testnet-rpc1.gdccscan.io"
+        ],
+        "shortName": "GDCC"
+    },
+    {
         "chainId": 7777,
         "faucets": [],
         "infoURL": "https://riseofthewarbots.com/",
         "name": "Rise of the Warbots Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Nano Machines",
@@ -10842,14 +13895,69 @@
             "https://testnet3.riseofthewarbots.com",
             "https://testnet4.riseofthewarbots.com",
             "https://testnet5.riseofthewarbots.com"
         ],
         "shortName": "RiseOfTheWarbotsTestnet"
     },
     {
+        "chainId": 7778,
+        "faucets": [],
+        "infoURL": "https://orenium.org",
+        "name": "Orenium Mainnet Protocol",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "ORENIUM",
+            "symbol": "ORE"
+        },
+        "networkId": 7778,
+        "rpc": [
+            "https://validator-mainnet.orenium.org",
+            "https://rpc-oracle-mainnet.orenium.org",
+            "https://portalmainnet.orenium.org"
+        ],
+        "shortName": "ore"
+    },
+    {
+        "chainId": 7798,
+        "faucets": [
+            "https://long.hub.openex.network/faucet"
+        ],
+        "infoURL": "https://openex.network",
+        "name": "OpenEX LONG Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "USDT Testnet",
+            "symbol": "USDT"
+        },
+        "networkId": 7798,
+        "rpc": [
+            "https://long.rpc.openex.network/"
+        ],
+        "shortName": "oex"
+    },
+    {
+        "chainId": 7860,
+        "faucets": [
+            "https://faucet-testnet.maalscan.io/"
+        ],
+        "infoURL": "https://www.maalchain.com/",
+        "name": "MaalChain Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "MAAL",
+            "symbol": "MAAL"
+        },
+        "networkId": 7860,
+        "rpc": [
+            "https://node1.maalscan.io/",
+            "https://rpc-bntest.maalscan.io/"
+        ],
+        "shortName": "maal-test"
+    },
+    {
         "chainId": 7878,
         "faucets": [
             "https://faucet.hazlor.com"
         ],
         "infoURL": "https://hazlor.com",
         "name": "Hazlor Testnet",
         "nativeCurrency": {
@@ -10861,14 +13969,31 @@
         "rpc": [
             "https://hatlas.rpc.hazlor.com:8545",
             "wss://hatlas.rpc.hazlor.com:8546"
         ],
         "shortName": "tscas"
     },
     {
+        "chainId": 7887,
+        "faucets": [],
+        "infoURL": "https://kinto.xyz",
+        "name": "Kinto Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ethereum",
+            "symbol": "ETH"
+        },
+        "networkId": 7887,
+        "rpc": [
+            "https://rpc.kinto.xyz/http",
+            "https://kinto-mainnet.calderachain.xyz/http"
+        ],
+        "shortName": "kintoMainnet"
+    },
+    {
         "chainId": 7895,
         "faucets": [
             "https://faucet-athena.ardescan.com/"
         ],
         "infoURL": "https://ardenium.org",
         "name": "ARDENIUM Athena",
         "nativeCurrency": {
@@ -10879,14 +14004,30 @@
         "networkId": 7895,
         "rpc": [
             "https://rpc-athena.ardescan.com/"
         ],
         "shortName": "ard"
     },
     {
+        "chainId": 7923,
+        "faucets": [],
+        "infoURL": "https://explorer.dotblox.io",
+        "name": "Dot Blox",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Dot Blox",
+            "symbol": "DTBX"
+        },
+        "networkId": 7923,
+        "rpc": [
+            "https://rpc.dotblox.io"
+        ],
+        "shortName": "DTBX"
+    },
+    {
         "chainId": 7979,
         "faucets": [],
         "infoURL": "https://doschain.io",
         "name": "DOS Chain",
         "nativeCurrency": {
             "decimals": 18,
             "name": "DOS",
@@ -10945,14 +14086,30 @@
         "networkId": 8029,
         "rpc": [
             "https://testnet.mdgl.io"
         ],
         "shortName": "mdgl"
     },
     {
+        "chainId": 8054,
+        "faucets": [],
+        "infoURL": "https://karak.network",
+        "name": "Karak Sepolia",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 8054,
+        "rpc": [
+            "https://rpc.sepolia.karak.network"
+        ],
+        "shortName": "karak-sepolia"
+    },
+    {
         "chainId": 8080,
         "faucets": [
             "https://faucet.liberty10.shardeum.org"
         ],
         "infoURL": "https://docs.shardeum.org/",
         "name": "Shardeum Liberty 1.X",
         "nativeCurrency": {
@@ -11002,25 +14159,41 @@
         ],
         "shortName": "Sphinx10"
     },
     {
         "chainId": 8086,
         "faucets": [],
         "infoURL": "https://biteth.org",
-        "name": "BitEth",
+        "name": "Bitcoin Chain",
         "nativeCurrency": {
             "decimals": 18,
-            "name": "BitEth",
-            "symbol": "BTE"
+            "name": "Bitcoin",
+            "symbol": "BTC"
         },
         "networkId": 8086,
         "rpc": [
             "https://rpc.biteth.org"
         ],
-        "shortName": "BitEth"
+        "shortName": "Bitcoin"
+    },
+    {
+        "chainId": 8087,
+        "faucets": [],
+        "infoURL": "https://e-dollar.org",
+        "name": "E-Dollar",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "E-Dollar",
+            "symbol": "USD"
+        },
+        "networkId": 8087,
+        "rpc": [
+            "https://rpc.e-dollar.org"
+        ],
+        "shortName": "E-Dollar"
     },
     {
         "chainId": 8098,
         "faucets": [],
         "infoURL": "https://www.streamux.cloud",
         "name": "StreamuX Blockchain",
         "nativeCurrency": {
@@ -11139,14 +14312,30 @@
         "networkId": 8181,
         "rpc": [
             "https://pre-boc1.beonechain.com"
         ],
         "shortName": "tBOC"
     },
     {
+        "chainId": 8192,
+        "faucets": [],
+        "infoURL": "https://docs.toruschain.com",
+        "name": "Torus Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "TQF",
+            "symbol": "TQF"
+        },
+        "networkId": 8192,
+        "rpc": [
+            "https://rpc.toruschain.com"
+        ],
+        "shortName": "tqf"
+    },
+    {
         "chainId": 8194,
         "faucets": [],
         "infoURL": "https://docs.toruschain.com",
         "name": "Torus Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "tTQF",
@@ -11157,24 +14346,24 @@
             "https://rpc.testnet.toruschain.com"
         ],
         "shortName": "ttqf"
     },
     {
         "chainId": 8217,
         "faucets": [],
-        "infoURL": "https://www.klaytn.com/",
+        "infoURL": "https://klaytn.foundation",
         "name": "Klaytn Mainnet Cypress",
         "nativeCurrency": {
             "decimals": 18,
             "name": "KLAY",
             "symbol": "KLAY"
         },
         "networkId": 8217,
         "rpc": [
-            "https://public-node-api.klaytnapi.com/v1/cypress"
+            "https://public-en-cypress.klaytn.net"
         ],
         "shortName": "Cypress"
     },
     {
         "chainId": 8272,
         "faucets": [
             "https://faucet.blocktonscan.com/"
@@ -11236,16 +14425,16 @@
         },
         "networkId": 8453,
         "rpc": [
             "https://mainnet.base.org/",
             "https://developer-access-mainnet.base.org/",
             "https://base.gateway.tenderly.co",
             "wss://base.gateway.tenderly.co",
-            "https://base.publicnode.com",
-            "wss://base.publicnode.com"
+            "https://base-rpc.publicnode.com",
+            "wss://base-rpc.publicnode.com"
         ],
         "shortName": "base"
     },
     {
         "chainId": 8654,
         "faucets": [],
         "infoURL": "https://www.buildwithtoki.com",
@@ -11324,14 +14513,46 @@
         "networkId": 8724,
         "rpc": [
             "https://testnet-web3.wolot.io"
         ],
         "shortName": "tolo"
     },
     {
+        "chainId": 8726,
+        "faucets": [],
+        "infoURL": "https://storagechain.io/about-us",
+        "name": "Storagechain Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Storagechain",
+            "symbol": "STOR"
+        },
+        "networkId": 8726,
+        "rpc": [
+            "https://mainnet-validator.storagechain.io"
+        ],
+        "shortName": "stor"
+    },
+    {
+        "chainId": 8727,
+        "faucets": [],
+        "infoURL": "https://storagechain.io/about-us",
+        "name": "Storagechain Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Storagechain",
+            "symbol": "STOR"
+        },
+        "networkId": 8727,
+        "rpc": [
+            "https://testnet-validator.storagechain.io"
+        ],
+        "shortName": "tstor"
+    },
+    {
         "chainId": 8738,
         "faucets": [],
         "infoURL": "https://alph.network",
         "name": "Alph Network",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Alph Network",
@@ -11359,14 +14580,31 @@
         "networkId": 8768,
         "rpc": [
             "https://node1.tmyblockchain.org/rpc"
         ],
         "shortName": "tmy"
     },
     {
+        "chainId": 8822,
+        "faucets": [],
+        "infoURL": "https://www.iota.org",
+        "name": "IOTA EVM",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "IOTA",
+            "symbol": "IOTA"
+        },
+        "networkId": 8822,
+        "rpc": [
+            "https://json-rpc.evm.iotaledger.net",
+            "https://ws.json-rpc.evm.iotaledger.net"
+        ],
+        "shortName": "iotaevm"
+    },
+    {
         "chainId": 8848,
         "faucets": [],
         "infoURL": "https://ma.ro/",
         "name": "MARO Blockchain Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "MARO",
@@ -11375,14 +14613,30 @@
         "networkId": 8848,
         "rpc": [
             "https://rpc-mainnet.ma.ro"
         ],
         "shortName": "maro"
     },
     {
+        "chainId": 8866,
+        "faucets": [],
+        "infoURL": "https://lumio.io/",
+        "name": "SuperLumio",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 8866,
+        "rpc": [
+            "https://mainnet.lumio.io/"
+        ],
+        "shortName": "superlumio"
+    },
+    {
         "chainId": 8880,
         "faucets": [],
         "infoURL": "https://unique.network",
         "name": "Unique",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Unique",
@@ -11486,14 +14740,36 @@
         "networkId": 8889,
         "rpc": [
             "https://vsc-dataseed.vyvo.org:8889"
         ],
         "shortName": "vsc"
     },
     {
+        "chainId": 8890,
+        "faucets": [
+            "https://faucetcoin.orenium.org"
+        ],
+        "infoURL": "https://orenium.org",
+        "name": "Orenium Testnet Protocol",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "ORENIUM",
+            "symbol": "tORE"
+        },
+        "networkId": 8890,
+        "rpc": [
+            "https://rpc-dev-testnet.orenium.org/",
+            "https://rpc-testnet.orenium.org/",
+            "https://rpc-orc.oredex.finance",
+            "https://testnet-rpc.oredex.finance",
+            "https://oredex-node.oredex.finance"
+        ],
+        "shortName": "tore"
+    },
+    {
         "chainId": 8898,
         "faucets": [
             "https://faucet.mmtscan.io/"
         ],
         "infoURL": "https://mmtchain.io/",
         "name": "Mammoth Mainnet",
         "nativeCurrency": {
@@ -11517,15 +14793,16 @@
         "nativeCurrency": {
             "decimals": 18,
             "name": "JIBCOIN",
             "symbol": "JBC"
         },
         "networkId": 8899,
         "rpc": [
-            "https://rpc-l1.jibchain.net"
+            "https://rpc-l1.jibchain.net",
+            "https://jib-rpc.inan.in.th"
         ],
         "shortName": "jbc"
     },
     {
         "chainId": 8989,
         "faucets": [],
         "infoURL": "https://gmmtchain.io/",
@@ -11594,14 +14871,52 @@
             "wss://evmos.lava.build/websocket",
             "https://evmos-evm.publicnode.com",
             "wss://evmos-evm.publicnode.com"
         ],
         "shortName": "evmos"
     },
     {
+        "chainId": 9007,
+        "faucets": [
+            "https://testnet.shidoscan.com/faucet"
+        ],
+        "infoURL": "https://www.nexablock.io",
+        "name": "Shido Testnet Block",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Shido Testnet Token",
+            "symbol": "SHIDO"
+        },
+        "networkId": 9007,
+        "rpc": [
+            "https://rpc-testnet-nodes.shidoscan.com",
+            "wss://wss-testnet-nodes.shidoscan.com"
+        ],
+        "shortName": "ShidoTestnet"
+    },
+    {
+        "chainId": 9008,
+        "faucets": [],
+        "infoURL": "https://shido.io",
+        "name": "Shido Mainnet Block",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Shido Mainnet Token",
+            "symbol": "SHIDO"
+        },
+        "networkId": 9008,
+        "rpc": [
+            "https://rpc-nodes.shidoscan.com",
+            "wss://wss-nodes.shidoscan.com",
+            "https://rpc-delta-nodes.shidoscan.com",
+            "wss://wss-delta-nodes.shidoscan.com"
+        ],
+        "shortName": "Shido"
+    },
+    {
         "chainId": 9012,
         "faucets": [
             "https://t.me/BerylBit"
         ],
         "infoURL": "https://www.beryl-bit.com",
         "name": "BerylBit Mainnet",
         "nativeCurrency": {
@@ -11612,14 +14927,50 @@
         "networkId": 9012,
         "rpc": [
             "https://mainnet.berylbit.io"
         ],
         "shortName": "brb"
     },
     {
+        "chainId": 9024,
+        "faucets": [
+            "https://testnet.nexablockscan.io/faucet"
+        ],
+        "infoURL": "https://www.nexablock.io",
+        "name": "Nexa Testnet Block",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Nexa Testnet Token",
+            "symbol": "NEXB"
+        },
+        "networkId": 9024,
+        "rpc": [
+            "https://rpc-testnet-nodes.nexablockscan.io"
+        ],
+        "shortName": "NexaTestnet"
+    },
+    {
+        "chainId": 9025,
+        "faucets": [],
+        "infoURL": "https://www.nexablock.io",
+        "name": "Nexa Mainnet Block",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Nexa Mainnet Token",
+            "symbol": "NEXB"
+        },
+        "networkId": 9025,
+        "rpc": [
+            "https://rpc-nodes.nexablockscan.io",
+            "wss://wss-nodes.nexablockscan.io",
+            "https://rpc-nodes-delta.nexablockscan.io"
+        ],
+        "shortName": "Nexa"
+    },
+    {
         "chainId": 9100,
         "faucets": [],
         "infoURL": "https://genesis-gn.com",
         "name": "Genesis Coin",
         "nativeCurrency": {
             "decimals": 18,
             "name": "GN Coin",
@@ -11679,14 +15030,46 @@
         "networkId": 9339,
         "rpc": [
             "https://testnet-rpc.dogcoin.me"
         ],
         "shortName": "DOGSt"
     },
     {
+        "chainId": 9393,
+        "faucets": [],
+        "infoURL": "https://www.deperp.com/dela",
+        "name": "Dela Sepolia Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Sepolia Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 9393,
+        "rpc": [
+            "https://sepolia-dela.deperp.com"
+        ],
+        "shortName": "delasep"
+    },
+    {
+        "chainId": 9395,
+        "faucets": [],
+        "infoURL": "https://explorer.evokescan.org",
+        "name": "Evoke Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "MTHN",
+            "symbol": "MTHN"
+        },
+        "networkId": 9395,
+        "rpc": [
+            "https://mainnet-rpc.evokescan.org"
+        ],
+        "shortName": "MTHN"
+    },
+    {
         "chainId": 9527,
         "faucets": [
             "https://robin-faucet.rangersprotocol.com"
         ],
         "infoURL": "https://rangersprotocol.com",
         "name": "Rangers Protocol Testnet Robin",
         "nativeCurrency": {
@@ -11740,18 +15123,20 @@
         "chainId": 9700,
         "faucets": [],
         "infoURL": "https://oortech.com",
         "name": "Oort MainnetDev",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Oort",
-            "symbol": "CCN"
+            "symbol": "OORT"
         },
         "networkId": 9700,
-        "rpc": [],
+        "rpc": [
+            "https://dev-rpc.oortech.com"
+        ],
         "shortName": "MainnetDev"
     },
     {
         "chainId": 9728,
         "faucets": [],
         "infoURL": "https://boba.network",
         "name": "Boba BNB Testnet",
@@ -11872,14 +15257,62 @@
         "rpc": [
             "https://data-aws-mainnet.imperiumchain.com",
             "https://data-aws2-mainnet.imperiumchain.com"
         ],
         "shortName": "IMP"
     },
     {
+        "chainId": 9888,
+        "faucets": [],
+        "infoURL": "https://dogelayer.org",
+        "name": "Dogelayer Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Dogecoin",
+            "symbol": "DOGE"
+        },
+        "networkId": 9888,
+        "rpc": [
+            "https://dl-rpc.dogelayer.org"
+        ],
+        "shortName": "Dogelayer"
+    },
+    {
+        "chainId": 9898,
+        "faucets": [],
+        "infoURL": "https://larissa.network",
+        "name": "Larissa Chain",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Larissa",
+            "symbol": "LRS"
+        },
+        "networkId": 1,
+        "rpc": [
+            "https://rpc.larissa.network"
+        ],
+        "shortName": "lrs"
+    },
+    {
+        "chainId": 9911,
+        "faucets": [],
+        "infoURL": "https://espento.network",
+        "name": "Espento Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "ESPENTO",
+            "symbol": "SPENT"
+        },
+        "networkId": 9911,
+        "rpc": [
+            "https://rpc.escscan.com/"
+        ],
+        "shortName": "spent"
+    },
+    {
         "chainId": 9977,
         "faucets": [
             "https://faucet.mindchain.info/"
         ],
         "infoURL": "https://mindchain.info",
         "name": "Mind Smart Chain Testnet",
         "nativeCurrency": {
@@ -11891,14 +15324,30 @@
         "rpc": [
             "https://testnet-msc.mindchain.info/",
             "wss://testnet-msc.mindchain.info/ws"
         ],
         "shortName": "tMIND"
     },
     {
+        "chainId": 9980,
+        "faucets": [],
+        "infoURL": "https://combonetwork.io",
+        "name": "Combo Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "BNB Chain Native Token",
+            "symbol": "BNB"
+        },
+        "networkId": 9980,
+        "rpc": [
+            "https://rpc.combonetwork.io"
+        ],
+        "shortName": "combo-mainnet"
+    },
+    {
         "chainId": 9990,
         "faucets": [],
         "infoURL": "https://www.peaq.network",
         "name": "Agung Network",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Agung",
@@ -11920,14 +15369,17 @@
             "name": "MIND Coin",
             "symbol": "MIND"
         },
         "networkId": 9996,
         "rpc": [
             "https://rpc-msc.mindchain.info/",
             "https://seednode.mindchain.info",
+            "https://archive.mindchain.info/",
+            "https://mind-smart-chain.rpc.thirdweb.com",
+            "wss://archive.mindchain.info/ws",
             "wss://seednode.mindchain.info/ws"
         ],
         "shortName": "MIND"
     },
     {
         "chainId": 9997,
         "faucets": [],
@@ -11941,14 +15393,30 @@
         "networkId": 9997,
         "rpc": [
             "https://testnet-rollup-api.altlayer.io"
         ],
         "shortName": "alt-testnet"
     },
     {
+        "chainId": 9998,
+        "faucets": [],
+        "infoURL": "https://ztc.best",
+        "name": "Ztc Mainnet",
+        "nativeCurrency": {
+            "decimals": 5,
+            "name": "Ztcer",
+            "symbol": "ZTC"
+        },
+        "networkId": 9998,
+        "rpc": [
+            "https://zitcoin.us"
+        ],
+        "shortName": "ZTC"
+    },
+    {
         "chainId": 9999,
         "faucets": [],
         "infoURL": "https://docs.bccloud.net/",
         "name": "myOwn Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "MYN",
@@ -12080,16 +15548,18 @@
             "symbol": "XDAI"
         },
         "networkId": 10200,
         "rpc": [
             "https://rpc.chiadochain.net",
             "https://rpc.chiado.gnosis.gateway.fm",
             "wss://rpc.chiadochain.net/wss",
-            "https://gnosis-chiado.publicnode.com",
-            "wss://gnosis-chiado.publicnode.com"
+            "https://gnosis-chiado-rpc.publicnode.com",
+            "wss://gnosis-chiado-rpc.publicnode.com",
+            "https://gnosis-chiado.drpc.org",
+            "wss://gnosis-chiado.drpc.org"
         ],
         "shortName": "chi"
     },
     {
         "chainId": 10201,
         "faucets": [
             "https://faucet.maxxchain.org"
@@ -12106,14 +15576,30 @@
             "https://rpc.maxxchain.org",
             "https://rpc1.maxxchain.org",
             "https://rpc2.maxxchain.org"
         ],
         "shortName": "PWR"
     },
     {
+        "chainId": 10242,
+        "faucets": [],
+        "infoURL": "https://docs.arthera.net/build/developing-sc/using-hardhat",
+        "name": "Arthera Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Arthera",
+            "symbol": "AA"
+        },
+        "networkId": 10242,
+        "rpc": [
+            "https://rpc.arthera.net"
+        ],
+        "shortName": "aa"
+    },
+    {
         "chainId": 10243,
         "faucets": [
             "https://faucet.arthera.net"
         ],
         "infoURL": "https://docs.arthera.net",
         "name": "Arthera Testnet",
         "nativeCurrency": {
@@ -12121,15 +15607,15 @@
             "name": "Arthera",
             "symbol": "AA"
         },
         "networkId": 10243,
         "rpc": [
             "https://rpc-test.arthera.net"
         ],
-        "shortName": "aa"
+        "shortName": "aat"
     },
     {
         "chainId": 10248,
         "faucets": [],
         "infoURL": "https://www.0xtrade.finance/",
         "name": "0XTade",
         "nativeCurrency": {
@@ -12143,19 +15629,19 @@
         ],
         "shortName": "0xt"
     },
     {
         "chainId": 10395,
         "faucets": [],
         "infoURL": "https://worldland.foundation",
-        "name": "Worldland Testnet",
+        "name": "WorldLand Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Worldland",
-            "symbol": "WL"
+            "symbol": "WLC"
         },
         "networkId": 10395,
         "rpc": [
             "https://gwangju.worldland.foundation"
         ],
         "shortName": "TWLC"
     },
@@ -12315,28 +15801,46 @@
         "rpc": [
             "https://mainnet-rpc.hashbit.org",
             "https://rpc.hashbit.org"
         ],
         "shortName": "hbit"
     },
     {
+        "chainId": 11221,
+        "faucets": [],
+        "infoURL": "https://shinechain.tech",
+        "name": "Shine Chain",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Shine",
+            "symbol": "SC20"
+        },
+        "networkId": 11221,
+        "rpc": [
+            "https://rpc.shinescan.io"
+        ],
+        "shortName": "SC20"
+    },
+    {
         "chainId": 11235,
         "faucets": [],
         "infoURL": "https://islamiccoin.net",
         "name": "Haqq Network",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Islamic Coin",
             "symbol": "ISLM"
         },
         "networkId": 11235,
         "rpc": [
             "https://rpc.eth.haqq.network",
-            "https://haqq-evm.publicnode.com",
-            "wss://haqq-evm.publicnode.com"
+            "https://haqq-evm-rpc.publicnode.com",
+            "wss://haqq-evm-rpc.publicnode.com",
+            "https://haqq.drpc.org",
+            "wss://haqq.drpc.org"
         ],
         "shortName": "ISLM"
     },
     {
         "chainId": 11437,
         "faucets": [],
         "infoURL": "https://shyft.network",
@@ -12347,14 +15851,47 @@
             "symbol": "SHYFTT"
         },
         "networkId": 11437,
         "rpc": [],
         "shortName": "shyftt"
     },
     {
+        "chainId": 11501,
+        "faucets": [],
+        "infoURL": "https://bevm.io",
+        "name": "BEVM Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "BTC",
+            "symbol": "BTC"
+        },
+        "networkId": 11501,
+        "rpc": [
+            "https://rpc-mainnet-1.bevm.io/",
+            "https://rpc-mainnet-2.bevm.io/"
+        ],
+        "shortName": "bevm"
+    },
+    {
+        "chainId": 11503,
+        "faucets": [],
+        "infoURL": "https://bevm.io",
+        "name": "BEVM Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "BTC",
+            "symbol": "BTC"
+        },
+        "networkId": 11503,
+        "rpc": [
+            "https://testnet.bevm.io/"
+        ],
+        "shortName": "bevm-test"
+    },
+    {
         "chainId": 11612,
         "faucets": [
             "https://faucet.sardisnetwork.com"
         ],
         "infoURL": "https://mysardis.com",
         "name": "Sardis Testnet",
         "nativeCurrency": {
@@ -12368,19 +15905,19 @@
         ],
         "shortName": "SRDXt"
     },
     {
         "chainId": 11888,
         "faucets": [],
         "infoURL": "https://sanr.app",
-        "name": "SanR Chain",
+        "name": "Santiment Intelligence Network",
         "nativeCurrency": {
             "decimals": 18,
-            "name": "nSAN",
-            "symbol": "nSAN"
+            "name": "SANR",
+            "symbol": "SANR"
         },
         "networkId": 11888,
         "rpc": [
             "https://sanrchain-node.santiment.net"
         ],
         "shortName": "SAN"
     },
@@ -12413,14 +15950,32 @@
         "networkId": 12009,
         "rpc": [
             "https://mainnet-rpc.satoshichain.io"
         ],
         "shortName": "sats"
     },
     {
+        "chainId": 12020,
+        "faucets": [
+            "https://faucet.aternoschain.com"
+        ],
+        "infoURL": "https://aternoschain.com",
+        "name": "Aternos",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Aternos",
+            "symbol": "ATR"
+        },
+        "networkId": 12020,
+        "rpc": [
+            "https://rpc.aternoschain.com"
+        ],
+        "shortName": "ATR"
+    },
+    {
         "chainId": 12051,
         "faucets": [
             "https://nft.singularity.gold"
         ],
         "infoURL": "https://www.singularity.gold",
         "name": "Singularity ZERO Testnet",
         "nativeCurrency": {
@@ -12534,26 +16089,28 @@
         "networkId": 12345,
         "rpc": [
             "https://rpc.testnet.step.network"
         ],
         "shortName": "steptest"
     },
     {
-        "chainId": 12611,
+        "chainId": 12553,
         "faucets": [],
-        "infoURL": "https://astar.network",
-        "name": "Astar zkEVM",
+        "infoURL": "https://rss3.io",
+        "name": "RSS3 VSL Mainnet",
         "nativeCurrency": {
             "decimals": 18,
-            "name": "Ether",
-            "symbol": "ETH"
+            "name": "RSS3",
+            "symbol": "RSS3"
         },
-        "networkId": 12611,
-        "rpc": [],
-        "shortName": "astrzk"
+        "networkId": 12553,
+        "rpc": [
+            "https://rpc.rss3.io"
+        ],
+        "shortName": "rss3"
     },
     {
         "chainId": 12715,
         "faucets": [],
         "infoURL": "https://rikeza.io",
         "name": "Rikeza Network Testnet",
         "nativeCurrency": {
@@ -12626,20 +16183,42 @@
         "nativeCurrency": {
             "decimals": 18,
             "name": "Beam",
             "symbol": "BEAM"
         },
         "networkId": 13337,
         "rpc": [
+            "https://build.onbeam.com/rpc/testnet",
+            "wss://build.onbeam.com/ws/testnet",
             "https://subnets.avax.network/beam/testnet/rpc",
             "wss://subnets.avax.network/beam/testnet/ws"
         ],
         "shortName": "beam-testnet"
     },
     {
+        "chainId": 13371,
+        "faucets": [
+            "https://docs.immutable.com/docs/zkEVM/guides/faucet"
+        ],
+        "infoURL": "https://www.immutable.com",
+        "name": "Immutable zkEVM",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "IMX",
+            "symbol": "IMX"
+        },
+        "networkId": 13371,
+        "rpc": [
+            "https://rpc.immutable.com",
+            "https://immutable-zkevm.drpc.org",
+            "wss://immutable-zkevm.drpc.org"
+        ],
+        "shortName": "imx"
+    },
+    {
         "chainId": 13381,
         "faucets": [],
         "infoURL": "https://cryptophoenix.org/phoenix",
         "name": "Phoenix Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Phoenix",
@@ -12648,14 +16227,66 @@
         "networkId": 13381,
         "rpc": [
             "https://rpc.phoenixplorer.com/"
         ],
         "shortName": "Phoenix"
     },
     {
+        "chainId": 13396,
+        "faucets": [],
+        "infoURL": "https://masa.finance",
+        "name": "Masa",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Masa Token",
+            "symbol": "MASA"
+        },
+        "networkId": 13396,
+        "rpc": [
+            "https://subnets.avax.network/masanetwork/mainnet/rpc"
+        ],
+        "shortName": "masa"
+    },
+    {
+        "chainId": 13473,
+        "faucets": [
+            "https://docs.immutable.com/docs/zkEVM/guides/faucet"
+        ],
+        "infoURL": "https://www.immutable.com",
+        "name": "Immutable zkEVM Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Test IMX",
+            "symbol": "tIMX"
+        },
+        "networkId": 13473,
+        "rpc": [
+            "https://rpc.testnet.immutable.com",
+            "https://immutable-zkevm-testnet.drpc.org",
+            "wss://immutable-zkevm-testnet.drpc.org"
+        ],
+        "shortName": "imx-testnet"
+    },
+    {
+        "chainId": 13600,
+        "faucets": [],
+        "infoURL": "https://kronobit.org",
+        "name": "Kronobit Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Kronobit",
+            "symbol": "KNB"
+        },
+        "networkId": 13600,
+        "rpc": [
+            "https://mainnet-rpc.qbitscan.com"
+        ],
+        "shortName": "KNB"
+    },
+    {
         "chainId": 13812,
         "faucets": [],
         "infoURL": "",
         "name": "Susono",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Susono",
@@ -12680,14 +16311,50 @@
         "networkId": 14000,
         "rpc": [
             "https://www.3sps.net"
         ],
         "shortName": "SPS-Test"
     },
     {
+        "chainId": 14324,
+        "faucets": [
+            "https://faucet.evolveblockchain.io"
+        ],
+        "infoURL": "https://evolveblockchain.io",
+        "name": "EVOLVE Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Evolve",
+            "symbol": "EVO"
+        },
+        "networkId": 14324,
+        "rpc": [
+            "https://testnet-rpc.evolveblockchain.io"
+        ],
+        "shortName": "evo"
+    },
+    {
+        "chainId": 14333,
+        "faucets": [
+            "https://faucet.vitruveo.xyz"
+        ],
+        "infoURL": "https://www.vitruveo.xyz",
+        "name": "Vitruveo Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Vitruveo Test Coin",
+            "symbol": "tVTRU"
+        },
+        "networkId": 14333,
+        "rpc": [
+            "https://test-rpc.vitruveo.xyz"
+        ],
+        "shortName": "vitruveo-test"
+    },
+    {
         "chainId": 14853,
         "faucets": [
             "https://t.me/HumanodeTestnet5FaucetBot"
         ],
         "infoURL": "https://humanode.io",
         "name": "Humanode Testnet 5 Israfel",
         "nativeCurrency": {
@@ -12698,14 +16365,32 @@
         "networkId": 14853,
         "rpc": [
             "https://explorer-rpc-http.testnet5.stages.humanode.io"
         ],
         "shortName": "hmnd-t5"
     },
     {
+        "chainId": 15003,
+        "faucets": [
+            "https://docs.immutable.com/docs/zkEVM/guides/faucet"
+        ],
+        "infoURL": "https://www.immutable.com",
+        "name": "Immutable zkEVM Devnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Dev IMX",
+            "symbol": "dIMX"
+        },
+        "networkId": 15003,
+        "rpc": [
+            "https://rpc.dev.immutable.com"
+        ],
+        "shortName": "imx-devnet"
+    },
+    {
         "chainId": 15551,
         "faucets": [],
         "infoURL": "http://theloopnetwork.org/",
         "name": "LoopNetwork Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "LOOP",
@@ -12863,20 +16548,55 @@
             "decimals": 18,
             "name": "Testnet ETH",
             "symbol": "ETH"
         },
         "networkId": 17000,
         "rpc": [
             "https://rpc.holesky.ethpandaops.io",
-            "https://ethereum-holesky.publicnode.com",
-            "wss://ethereum-holesky.publicnode.com"
+            "https://ethereum-holesky-rpc.publicnode.com",
+            "wss://ethereum-holesky-rpc.publicnode.com",
+            "https://holesky.drpc.org",
+            "wss://holesky.drpc.org"
         ],
         "shortName": "holesky"
     },
     {
+        "chainId": 17001,
+        "faucets": [],
+        "infoURL": "https://redstone.xyz/docs/network-info",
+        "name": "Redstone Holesky Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Redstone Testnet Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 17001,
+        "rpc": [
+            "https://rpc.holesky.redstone.xyz"
+        ],
+        "shortName": "redstone-holesky"
+    },
+    {
+        "chainId": 17069,
+        "faucets": [],
+        "infoURL": "https://redstone.xyz",
+        "name": "Garnet Holesky",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 17069,
+        "rpc": [
+            "https://rpc.garnetchain.com",
+            "wss://rpc.garnetchain.com"
+        ],
+        "shortName": "garnet"
+    },
+    {
         "chainId": 17171,
         "faucets": [
             "https://faucet.oneg8.network"
         ],
         "infoURL": "https://oneg8.one",
         "name": "G8Chain Mainnet",
         "nativeCurrency": {
@@ -12887,14 +16607,30 @@
         "networkId": 17171,
         "rpc": [
             "https://mainnet-rpc.oneg8.network"
         ],
         "shortName": "G8Cm"
     },
     {
+        "chainId": 17172,
+        "faucets": [],
+        "infoURL": "http://eclipsenet.io",
+        "name": "Eclipse Subnet",
+        "nativeCurrency": {
+            "decimals": 16,
+            "name": "Eclipse",
+            "symbol": "ECLP"
+        },
+        "networkId": 17172,
+        "rpc": [
+            "https://subnets.avax.network/eclipse/testnet/rpc"
+        ],
+        "shortName": "eclipse"
+    },
+    {
         "chainId": 17180,
         "faucets": [],
         "infoURL": "https://hashpalette.com/",
         "name": "Palette Chain Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Palette Token",
@@ -12903,14 +16639,30 @@
         "networkId": 17180,
         "rpc": [
             "https://palette-opennet.com:22000"
         ],
         "shortName": "PCT"
     },
     {
+        "chainId": 17217,
+        "faucets": [],
+        "infoURL": "https://konetmain.com",
+        "name": "KONET Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "KONET",
+            "symbol": "KONET"
+        },
+        "networkId": 17217,
+        "rpc": [
+            "https://api.kon-wallet.com"
+        ],
+        "shortName": "KONET"
+    },
+    {
         "chainId": 17777,
         "faucets": [],
         "infoURL": "https://eosnetwork.com/eos-evm",
         "name": "EOS EVM Network",
         "nativeCurrency": {
             "decimals": 18,
             "name": "EOS",
@@ -12988,30 +16740,101 @@
         "networkId": 18181,
         "rpc": [
             "https://testnet-rpc.oneg8.network"
         ],
         "shortName": "G8Ct"
     },
     {
+        "chainId": 18231,
+        "faucets": [],
+        "infoURL": "https://raas.gelato.network/rollups/details/public/unreal",
+        "name": "unreal-old",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "unreal Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 18231,
+        "rpc": [
+            "https://rpc.unreal.gelato.digital",
+            "wss://ws.unreal.gelato.digital"
+        ],
+        "shortName": "unreal-old"
+    },
+    {
+        "chainId": 18233,
+        "faucets": [],
+        "infoURL": "https://raas.gelato.network/rollups/details/public/unreal",
+        "name": "unreal",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "unreal Ether",
+            "symbol": "reETH"
+        },
+        "networkId": 18233,
+        "rpc": [
+            "https://rpc.unreal-orbit.gelato.digital",
+            "wss://ws.unreal-orbit.gelato.digital"
+        ],
+        "shortName": "unreal"
+    },
+    {
         "chainId": 18686,
         "faucets": [],
         "infoURL": "https://doc.mxc.com/docs/intro",
-        "name": "MXC zkEVM Mainnet",
+        "name": "MXC zkEVM Moonchain",
         "nativeCurrency": {
             "decimals": 18,
-            "name": "MXC zkEVM Mainnet",
+            "name": "MXC zkEVM Moonchain",
             "symbol": "MXC"
         },
         "networkId": 18686,
         "rpc": [
             "https://rpc.mxc.com"
         ],
         "shortName": "MXCzkEVM"
     },
     {
+        "chainId": 18888,
+        "faucets": [],
+        "infoURL": "https://titanlab.io",
+        "name": "Titan (TKX)",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Titan tkx",
+            "symbol": "TKX"
+        },
+        "networkId": 18888,
+        "rpc": [
+            "https://titan-json-rpc.titanlab.io",
+            "https://titan-json-rpc-tokyo.titanlab.io",
+            "https://titan-json-rpc-seoul.titanlab.io",
+            "https://titan-json-rpc-hongkong.titanlab.io"
+        ],
+        "shortName": "titan_tkx"
+    },
+    {
+        "chainId": 18889,
+        "faucets": [],
+        "infoURL": "https://titanlab.io",
+        "name": "Titan (TKX) Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Titan tkx",
+            "symbol": "TKX"
+        },
+        "networkId": 18889,
+        "rpc": [
+            "https://titan-testnet-json-rpc.titanlab.io",
+            "https://titan-testnet-json-rpc-1.titanlab.io",
+            "https://titan-testnet-json-rpc-2.titanlab.io"
+        ],
+        "shortName": "titan_tkx-testnet"
+    },
+    {
         "chainId": 19011,
         "faucets": [],
         "infoURL": "https://www.homeverse.games/",
         "name": "HOME Verse Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "OAS",
@@ -13020,14 +16843,62 @@
         "networkId": 19011,
         "rpc": [
             "https://rpc.mainnet.oasys.homeverse.games/"
         ],
         "shortName": "HMV"
     },
     {
+        "chainId": 19224,
+        "faucets": [],
+        "infoURL": "https://docs.decentraconnect.io",
+        "name": "Decentraconnect Social",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Decentraconnect Social",
+            "symbol": "DCSM"
+        },
+        "networkId": 19224,
+        "rpc": [
+            "https://rpc.decentraconnect.io"
+        ],
+        "shortName": "DCSMs"
+    },
+    {
+        "chainId": 19527,
+        "faucets": [],
+        "infoURL": "https://magnet.magport.io/",
+        "name": "Magnet Network",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Magnet Network",
+            "symbol": "DOT"
+        },
+        "networkId": 19527,
+        "rpc": [
+            "https://magnet-rpc.magport.io/"
+        ],
+        "shortName": "mgt"
+    },
+    {
+        "chainId": 19600,
+        "faucets": [],
+        "infoURL": "https://lbry.com",
+        "name": "LBRY Mainnet",
+        "nativeCurrency": {
+            "decimals": 8,
+            "name": "LBRY Credits",
+            "symbol": "LBC"
+        },
+        "networkId": 19600,
+        "rpc": [
+            "https://lbry.nl/rpc"
+        ],
+        "shortName": "LBRY"
+    },
+    {
         "chainId": 19845,
         "faucets": [],
         "infoURL": "https://bitcolojix.org",
         "name": "BTCIX Network",
         "nativeCurrency": {
             "decimals": 18,
             "name": "BTCIX Network",
@@ -13086,14 +16957,66 @@
         "networkId": 20736,
         "rpc": [
             "https://rpc-chain.p12.games"
         ],
         "shortName": "p12"
     },
     {
+        "chainId": 20765,
+        "faucets": [],
+        "infoURL": "",
+        "name": "Jono11 Subnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Jono11 Token",
+            "symbol": "JONO"
+        },
+        "networkId": 20765,
+        "rpc": [
+            "https://subnets.avax.network/jono11/testnet/rpc"
+        ],
+        "shortName": "jono11"
+    },
+    {
+        "chainId": 21004,
+        "faucets": [
+            "https://play.google.com/store/apps/details?id=net.c4ei.fps2"
+        ],
+        "infoURL": "https://c4ei.net",
+        "name": "C4EI",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "C4EI",
+            "symbol": "C4EI"
+        },
+        "networkId": 21004,
+        "rpc": [
+            "https://rpc.c4ei.net"
+        ],
+        "shortName": "c4ei"
+    },
+    {
+        "chainId": 21133,
+        "faucets": [
+            "https://t.me/c4eiAirdrop"
+        ],
+        "infoURL": "https://c4ex.net",
+        "name": "All About Healthy",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "AAH",
+            "symbol": "AAH"
+        },
+        "networkId": 21133,
+        "rpc": [
+            "https://rpc.c4ex.net"
+        ],
+        "shortName": "aah"
+    },
+    {
         "chainId": 21337,
         "faucets": [],
         "infoURL": "https://cennz.net",
         "name": "CENNZnet Azalea",
         "nativeCurrency": {
             "decimals": 18,
             "name": "CPAY",
@@ -13118,14 +17041,31 @@
         "networkId": 21816,
         "rpc": [
             "https://seed.omchain.io"
         ],
         "shortName": "omc"
     },
     {
+        "chainId": 21912,
+        "faucets": [],
+        "infoURL": "https://bsquarelab.com/",
+        "name": "BSL Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Origin NFT",
+            "symbol": "ONF"
+        },
+        "networkId": 21912,
+        "rpc": [
+            "http://rpc-mainnet.nftruth.io:8545",
+            "ws://rpc-mainnet.nftruth.io:8645"
+        ],
+        "shortName": "onf"
+    },
+    {
         "chainId": 22023,
         "faucets": [],
         "infoURL": "https://hupayx.io",
         "name": "Taycan",
         "nativeCurrency": {
             "decimals": 18,
             "name": "shuffle",
@@ -13166,28 +17106,46 @@
         "networkId": 22222,
         "rpc": [
             "https://api.nautilus.nautchain.xyz"
         ],
         "shortName": "NAUTCHAIN"
     },
     {
+        "chainId": 22324,
+        "faucets": [
+            "https://faucet.goldxchain.io"
+        ],
+        "infoURL": "https://goldxchain.io",
+        "name": "GoldXChain Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "GoldX",
+            "symbol": "GOLDX"
+        },
+        "networkId": 22324,
+        "rpc": [
+            "https://testnet-rpc.goldxchain.io"
+        ],
+        "shortName": "goldx-testnet"
+    },
+    {
         "chainId": 22776,
         "faucets": [],
-        "infoURL": "https://maplabs.io",
-        "name": "MAP Mainnet",
+        "infoURL": "https://mapprotocol.io/",
+        "name": "MAP Protocol",
         "nativeCurrency": {
             "decimals": 18,
             "name": "MAPO",
             "symbol": "MAPO"
         },
         "networkId": 22776,
         "rpc": [
             "https://rpc.maplabs.io"
         ],
-        "shortName": "map"
+        "shortName": "mapo"
     },
     {
         "chainId": 23006,
         "faucets": [
             "https://faucet.antofy.io"
         ],
         "infoURL": "https://antofy.io",
@@ -13246,20 +17204,68 @@
         "nativeCurrency": {
             "decimals": 18,
             "name": "Sapphire Test Rose",
             "symbol": "TEST"
         },
         "networkId": 23295,
         "rpc": [
-            "https://testnet.sapphire.oasis.dev",
-            "wss://testnet.sapphire.oasis.dev/ws"
+            "https://testnet.sapphire.oasis.io",
+            "wss://testnet.sapphire.oasis.io/ws"
         ],
         "shortName": "sapphire-testnet"
     },
     {
+        "chainId": 23451,
+        "faucets": [],
+        "infoURL": "https://dreyerx.com",
+        "name": "DreyerX Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "DreyerX",
+            "symbol": "DRX"
+        },
+        "networkId": 23451,
+        "rpc": [
+            "https://rpc.dreyerx.com"
+        ],
+        "shortName": "dreyerx"
+    },
+    {
+        "chainId": 23452,
+        "faucets": [],
+        "infoURL": "https://dreyerx.com",
+        "name": "DreyerX Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "DreyerX",
+            "symbol": "DRX"
+        },
+        "networkId": 23452,
+        "rpc": [
+            "https://testnet-rpc.dreyerx.com"
+        ],
+        "shortName": "dreyerx-testnet"
+    },
+    {
+        "chainId": 23888,
+        "faucets": [],
+        "infoURL": "https://docs.blastblockchain.com",
+        "name": "Blast Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 23888,
+        "rpc": [
+            "http://testnet-rpc.blastblockchain.com"
+        ],
+        "shortName": "blastT"
+    },
+    {
         "chainId": 24484,
         "faucets": [],
         "infoURL": "https://webchain.network",
         "name": "Webchain",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Webchain Ether",
@@ -13282,14 +17288,48 @@
         "networkId": 37480,
         "rpc": [
             "https://node1.mintme.com"
         ],
         "shortName": "mintme"
     },
     {
+        "chainId": 25186,
+        "faucets": [],
+        "infoURL": "https://scan.liquidlayer.network",
+        "name": "LiquidLayer Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "LiquidLayer",
+            "symbol": "LILA"
+        },
+        "networkId": 25186,
+        "rpc": [
+            "https://mainnet.liquidlayer.network"
+        ],
+        "shortName": "LILA"
+    },
+    {
+        "chainId": 25839,
+        "faucets": [
+            "https://faucet.alveytestnet.com"
+        ],
+        "infoURL": "https://alveychain.com/",
+        "name": "AlveyChain Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "AlveyCoin Testnet",
+            "symbol": "tALV"
+        },
+        "networkId": 25839,
+        "rpc": [
+            "https://testnet-rpc.alvey.io"
+        ],
+        "shortName": "talv"
+    },
+    {
         "chainId": 25888,
         "faucets": [],
         "infoURL": "https://www.hammerchain.io",
         "name": "Hammer Chain Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "GOLDT",
@@ -13371,14 +17411,95 @@
             "https://rpc1.oasischain.io",
             "https://rpc2.oasischain.io",
             "https://rpc3.oasischain.io"
         ],
         "shortName": "OAC"
     },
     {
+        "chainId": 27181,
+        "faucets": [],
+        "infoURL": "https://www.laosfoundation.io/",
+        "name": "KLAOS Nova",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "KLAOS",
+            "symbol": "KLAOS"
+        },
+        "networkId": 27181,
+        "rpc": [
+            "https://rpc.klaosnova.laosfoundation.io",
+            "wss://rpc.klaosnova.laosfoundation.io"
+        ],
+        "shortName": "klaosnova"
+    },
+    {
+        "chainId": 27483,
+        "faucets": [],
+        "infoURL": "https://www.nanon.network",
+        "name": "Nanon Sepolia",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Sepolia Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 27483,
+        "rpc": [
+            "https://sepolia-rpc.nanon.network"
+        ],
+        "shortName": "Nanon-Testnet"
+    },
+    {
+        "chainId": 27827,
+        "faucets": [],
+        "infoURL": "https://zeroone.art/",
+        "name": "zeroone Mainnet Subnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "ZERO",
+            "symbol": "ZERO"
+        },
+        "networkId": 27827,
+        "rpc": [
+            "https://subnets.avax.network/zeroonemai/mainnet/rpc"
+        ],
+        "shortName": "zeroonemai"
+    },
+    {
+        "chainId": 28516,
+        "faucets": [],
+        "infoURL": "https://vizing.com",
+        "name": "Vizing Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 28516,
+        "rpc": [
+            "https://rpc-sepolia.vizing.com"
+        ],
+        "shortName": "Vizing-Testnet"
+    },
+    {
+        "chainId": 28518,
+        "faucets": [],
+        "infoURL": "https://vizing.com",
+        "name": "Vizing Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 28518,
+        "rpc": [
+            "https://rpc.vizing.com"
+        ],
+        "shortName": "Vizing"
+    },
+    {
         "chainId": 28528,
         "faucets": [],
         "infoURL": "https://community.optimism.io/docs/developers/bedrock",
         "name": "Optimism Bedrock (Goerli Alpha Testnet)",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Goerli Ether",
@@ -13390,14 +17511,70 @@
             "https://alpha-1-replica-1.bedrock-goerli.optimism.io",
             "https://alpha-1-replica-2.bedrock-goerli.optimism.io",
             "https://alpha-1-replica-2.bedrock-goerli.optimism.io"
         ],
         "shortName": "obgor"
     },
     {
+        "chainId": 28882,
+        "faucets": [
+            "https://www.l2faucet.com/boba"
+        ],
+        "infoURL": "https://boba.network",
+        "name": "Boba Sepolia",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 28882,
+        "rpc": [
+            "https://sepolia.boba.network",
+            "https://boba-sepolia.gateway.tenderly.co",
+            "https://gateway.tenderly.co/public/boba-sepolia",
+            "wss://boba-sepolia.gateway.tenderly.co/",
+            "wss://gateway.tenderly.co/public/boba-sepolia"
+        ],
+        "shortName": "BobaSepolia"
+    },
+    {
+        "chainId": 29112,
+        "faucets": [],
+        "infoURL": "https://www.hychain.com",
+        "name": "HYCHAIN Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "TOPIA",
+            "symbol": "TOPIA"
+        },
+        "networkId": 29112,
+        "rpc": [
+            "https://testnet-rpc.hychain.com/http"
+        ],
+        "shortName": "hychain-testnet"
+    },
+    {
+        "chainId": 29536,
+        "faucets": [
+            "https://faucet.kaichain.net"
+        ],
+        "infoURL": "https://kaichain.net",
+        "name": "KaiChain Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "KaiChain Testnet Native Token",
+            "symbol": "KEC"
+        },
+        "networkId": 29536,
+        "rpc": [
+            "https://testnet-rpc.kaichain.net"
+        ],
+        "shortName": "tkec"
+    },
+    {
         "chainId": 29548,
         "faucets": [],
         "infoURL": "https://www.mycryptoheroes.net/verse",
         "name": "MCH Verse Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "OAS",
@@ -13424,14 +17601,31 @@
         "networkId": 30067,
         "rpc": [
             "https://testnet-rpc0.piecenetwork.com"
         ],
         "shortName": "Piece"
     },
     {
+        "chainId": 30088,
+        "faucets": [],
+        "infoURL": "https://www.miyou.io",
+        "name": "MiYou Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Miyou",
+            "symbol": "MY"
+        },
+        "networkId": 30088,
+        "rpc": [
+            "https://blockchain.miyou.io",
+            "https://blockchain.miyoulab.com"
+        ],
+        "shortName": "MiYou"
+    },
+    {
         "chainId": 30103,
         "faucets": [],
         "infoURL": "https://canxium.org",
         "name": "Cerium Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Canxium",
@@ -13440,14 +17634,56 @@
         "networkId": 30103,
         "rpc": [
             "https://cerium-rpc.canxium.net"
         ],
         "shortName": "ceri"
     },
     {
+        "chainId": 30730,
+        "faucets": [],
+        "infoURL": "https://movementlabs.xyz",
+        "name": "Movement EVM Legacy",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Move",
+            "symbol": "MOVE"
+        },
+        "networkId": 30730,
+        "rpc": [],
+        "shortName": "moveleg"
+    },
+    {
+        "chainId": 30731,
+        "faucets": [],
+        "infoURL": "https://movementlabs.xyz",
+        "name": "Movement EVM Devnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Move",
+            "symbol": "MOVE"
+        },
+        "networkId": 30731,
+        "rpc": [],
+        "shortName": "movedev"
+    },
+    {
+        "chainId": 30732,
+        "faucets": [],
+        "infoURL": "https://movementlabs.xyz",
+        "name": "Movement EVM Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Move",
+            "symbol": "MOVE"
+        },
+        "networkId": 30732,
+        "rpc": [],
+        "shortName": "movetest"
+    },
+    {
         "chainId": 31102,
         "faucets": [],
         "infoURL": "https://ethersocial.org",
         "name": "Ethersocial Network",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Ethersocial Network Ether",
@@ -13506,28 +17742,62 @@
         "networkId": 31337,
         "rpc": [
             "https://testnet-rpc.gochain.io"
         ],
         "shortName": "got"
     },
     {
+        "chainId": 31414,
+        "faucets": [
+            "https://faucet.evokescan.org"
+        ],
+        "infoURL": "https://testnet-explorer.evokescan.org",
+        "name": "Evoke Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "MTHN Testnet",
+            "symbol": "MTHN"
+        },
+        "networkId": 31414,
+        "rpc": [
+            "https://testnet-rpc.evokescan.org"
+        ],
+        "shortName": "tmthn"
+    },
+    {
         "chainId": 31415,
         "faucets": [],
         "infoURL": "https://filecoin.io",
         "name": "Filecoin - Wallaby testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "testnet filecoin",
             "symbol": "tFIL"
         },
         "networkId": 31415,
         "rpc": [],
         "shortName": "filecoin-wallaby"
     },
     {
+        "chainId": 32001,
+        "faucets": [],
+        "infoURL": "https://web3games.com/",
+        "name": "W3Gamez Holesky Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "W3Gamez Testnet Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 32001,
+        "rpc": [
+            "https://rpc-holesky.w3gamez.network"
+        ],
+        "shortName": "w3gamez"
+    },
+    {
         "chainId": 32520,
         "faucets": [],
         "infoURL": "https://bitgert.com/",
         "name": "Bitgert Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Bitrise Token",
@@ -13608,14 +17878,30 @@
         "networkId": 33101,
         "rpc": [
             "https://dev-api.zilliqa.com"
         ],
         "shortName": "zil-testnet"
     },
     {
+        "chainId": 33210,
+        "faucets": [],
+        "infoURL": "https://muadao.build/",
+        "name": "Cloudverse Subnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "XCLOUD",
+            "symbol": "XCLOUD"
+        },
+        "networkId": 33210,
+        "rpc": [
+            "https://subnets.avax.network/cloudverse/mainnet/rpc"
+        ],
+        "shortName": "cloudverse"
+    },
+    {
         "chainId": 33333,
         "faucets": [],
         "infoURL": "https://avescoin.io",
         "name": "Aves Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Aves",
@@ -13644,30 +17930,48 @@
             "https://api.devnet.zilliqa.com/"
         ],
         "shortName": "zil-devnet"
     },
     {
         "chainId": 33469,
         "faucets": [
-            "https://faucet.zq2-devnet.zilstg.dev"
+            "https://faucet.zq2-devnet.zilliqa.com"
         ],
         "infoURL": "https://www.zilliqa.com/",
-        "name": "Zilliqa 2 EVM Devnet",
+        "name": "Zilliqa-2 EVM Devnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Zilliqa",
             "symbol": "ZIL"
         },
         "networkId": 33469,
         "rpc": [
-            "https://api.zq2-devnet.zilstg.dev"
+            "https://api.zq2-devnet.zilliqa.com"
         ],
         "shortName": "zq2-devnet"
     },
     {
+        "chainId": 34443,
+        "faucets": [],
+        "infoURL": "https://docs.mode.network/",
+        "name": "Mode",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 34443,
+        "rpc": [
+            "https://mainnet.mode.network",
+            "https://mode.drpc.org",
+            "wss://mode.drpc.org"
+        ],
+        "shortName": "mode"
+    },
+    {
         "chainId": 35011,
         "faucets": [],
         "infoURL": "https://j2o.io",
         "name": "J2O Taro",
         "nativeCurrency": {
             "decimals": 18,
             "name": "TARO Coin",
@@ -13682,16 +17986,16 @@
     {
         "chainId": 35441,
         "faucets": [],
         "infoURL": "https://q.org",
         "name": "Q Mainnet",
         "nativeCurrency": {
             "decimals": 18,
-            "name": "Q token",
-            "symbol": "Q"
+            "name": "QGOV",
+            "symbol": "QGOV"
         },
         "networkId": 35441,
         "rpc": [
             "https://rpc.q.org"
         ],
         "shortName": "q"
     },
@@ -13861,27 +18165,27 @@
             "wss://forno.celo.org/ws"
         ],
         "shortName": "celo"
     },
     {
         "chainId": 42261,
         "faucets": [
-            "https://faucet.testnet.oasis.dev/"
+            "https://faucet.testnet.oasis.io/"
         ],
         "infoURL": "https://docs.oasis.io/dapp/emerald",
         "name": "Oasis Emerald Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Emerald Rose",
             "symbol": "ROSE"
         },
         "networkId": 42261,
         "rpc": [
-            "https://testnet.emerald.oasis.dev/",
-            "wss://testnet.emerald.oasis.dev/ws"
+            "https://testnet.emerald.oasis.io/",
+            "wss://testnet.emerald.oasis.io/ws"
         ],
         "shortName": "emerald-testnet"
     },
     {
         "chainId": 42262,
         "faucets": [],
         "infoURL": "https://docs.oasis.io/dapp/emerald",
@@ -13889,20 +18193,52 @@
         "nativeCurrency": {
             "decimals": 18,
             "name": "Emerald Rose",
             "symbol": "ROSE"
         },
         "networkId": 42262,
         "rpc": [
-            "https://emerald.oasis.dev",
-            "wss://emerald.oasis.dev/ws"
+            "https://emerald.oasis.io",
+            "wss://emerald.oasis.io/ws"
         ],
         "shortName": "emerald"
     },
     {
+        "chainId": 42355,
+        "faucets": [],
+        "infoURL": "https://goldxchain.io",
+        "name": "GoldXChain Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "GoldX",
+            "symbol": "GOLDX"
+        },
+        "networkId": 42355,
+        "rpc": [
+            "https://mainnet-rpc.goldxchain.io"
+        ],
+        "shortName": "goldx"
+    },
+    {
+        "chainId": 42766,
+        "faucets": [],
+        "infoURL": "https://zkfair.io",
+        "name": "ZKFair Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "USDC Token",
+            "symbol": "USDC"
+        },
+        "networkId": 42766,
+        "rpc": [
+            "https://rpc.zkfair.io"
+        ],
+        "shortName": "ZKFair-Mainnet"
+    },
+    {
         "chainId": 42801,
         "faucets": [],
         "infoURL": "https://gesoten.com/",
         "name": "Gesoten Verse Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "OAS",
@@ -13945,30 +18281,44 @@
         "networkId": 43110,
         "rpc": [
             "https://ava.network:21015/ext/evm/rpc"
         ],
         "shortName": "avaeth"
     },
     {
+        "chainId": 43111,
+        "faucets": [],
+        "infoURL": "https://hemi.xyz",
+        "name": "Hemi Network",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 43111,
+        "rpc": [],
+        "shortName": "hemi"
+    },
+    {
         "chainId": 43113,
         "faucets": [
             "https://faucet.avax-test.network/"
         ],
         "infoURL": "https://cchain.explorer.avax-test.network",
         "name": "Avalanche Fuji Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Avalanche",
             "symbol": "AVAX"
         },
         "networkId": 1,
         "rpc": [
             "https://api.avax-test.network/ext/bc/C/rpc",
-            "https://avalanche-fuji-c-chain.publicnode.com",
-            "wss://avalanche-fuji-c-chain.publicnode.com"
+            "https://avalanche-fuji-c-chain-rpc.publicnode.com",
+            "wss://avalanche-fuji-c-chain-rpc.publicnode.com"
         ],
         "shortName": "Fuji"
     },
     {
         "chainId": 43114,
         "faucets": [],
         "infoURL": "https://www.avax.network/",
@@ -13977,16 +18327,16 @@
             "decimals": 18,
             "name": "Avalanche",
             "symbol": "AVAX"
         },
         "networkId": 43114,
         "rpc": [
             "https://api.avax.network/ext/bc/C/rpc",
-            "https://avalanche-c-chain.publicnode.com",
-            "wss://avalanche-c-chain.publicnode.com"
+            "https://avalanche-c-chain-rpc.publicnode.com",
+            "wss://avalanche-c-chain-rpc.publicnode.com"
         ],
         "shortName": "avax"
     },
     {
         "chainId": 43288,
         "faucets": [],
         "infoURL": "https://docs.boba.network/for-developers/network-avalanche",
@@ -14002,14 +18352,30 @@
             "wss://wss.avax.boba.network",
             "https://replica.avax.boba.network",
             "wss://replica-wss.avax.boba.network"
         ],
         "shortName": "bobaavax"
     },
     {
+        "chainId": 43851,
+        "faucets": [],
+        "infoURL": "https://zkfair.io",
+        "name": "ZKFair Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "USDC Token",
+            "symbol": "USDC"
+        },
+        "networkId": 43851,
+        "rpc": [
+            "https://testnet-rpc.zkfair.io"
+        ],
+        "shortName": "ZKFair-Testnet"
+    },
+    {
         "chainId": 44444,
         "faucets": [],
         "infoURL": "https://frenchain.app",
         "name": "Frenchain",
         "nativeCurrency": {
             "decimals": 18,
             "name": "FREN",
@@ -14018,14 +18384,30 @@
         "networkId": 44444,
         "rpc": [
             "https://rpc-02.frenscan.io"
         ],
         "shortName": "FREN"
     },
     {
+        "chainId": 44445,
+        "faucets": [],
+        "infoURL": "https://avescoin.io/",
+        "name": "Quantum Network",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Quantum",
+            "symbol": "QTM"
+        },
+        "networkId": 44445,
+        "rpc": [
+            "https://rpcqtm.avescoin.io"
+        ],
+        "shortName": "QTM"
+    },
+    {
         "chainId": 44787,
         "faucets": [
             "https://celo.org/developers/faucet",
             "https://cauldron.pretoriaresearchlab.io/alfajores-faucet"
         ],
         "infoURL": "https://docs.celo.org/",
         "name": "Celo Alfajores Testnet",
@@ -14054,14 +18436,48 @@
         "networkId": 45000,
         "rpc": [
             "https://rpc.autobahn.network"
         ],
         "shortName": "AutobahnNetwork"
     },
     {
+        "chainId": 45454,
+        "faucets": [],
+        "infoURL": "https://www.swamps.fi",
+        "name": "Swamps L2",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "SWP",
+            "symbol": "SWP"
+        },
+        "networkId": 45454,
+        "rpc": [
+            "https://swamps.tc.l2aas.com"
+        ],
+        "shortName": "SWP"
+    },
+    {
+        "chainId": 45510,
+        "faucets": [
+            "https://faucet.deelance.com"
+        ],
+        "infoURL": "https://deelance.com",
+        "name": "Deelance Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Deelance",
+            "symbol": "DEE"
+        },
+        "networkId": 45510,
+        "rpc": [
+            "https://rpc.deelance.com"
+        ],
+        "shortName": "dee"
+    },
+    {
         "chainId": 46688,
         "faucets": [],
         "infoURL": "https://fusion.org",
         "name": "Fusion Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Testnet Fusion",
@@ -14107,29 +18523,45 @@
             "https://wireshape-floripa-testnet.rpc.thirdweb.com"
         ],
         "shortName": "floripa"
     },
     {
         "chainId": 49088,
         "faucets": [],
-        "infoURL": "https://thebifrost.io",
+        "infoURL": "https://bifrostnetwork.com",
         "name": "Bifrost Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Bifrost",
             "symbol": "BFC"
         },
         "networkId": 49088,
         "rpc": [
-            "https://public-01.testnet.thebifrost.io/rpc",
-            "https://public-02.testnet.thebifrost.io/rpc"
+            "https://public-01.testnet.bifrostnetwork.com/rpc",
+            "https://public-02.testnet.bifrostnetwork.com/rpc"
         ],
         "shortName": "tbfc"
     },
     {
+        "chainId": 49321,
+        "faucets": [],
+        "infoURL": "https://gunbygunz.com",
+        "name": "GUNZ Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "GUN",
+            "symbol": "GUN"
+        },
+        "networkId": 49321,
+        "rpc": [
+            "https://rpc.gunz.dev/ext/bc/ryk9vkvNuKtewME2PeCgybo9sdWXGmCkBrrx4VPuZPdVdAak8/rpc"
+        ],
+        "shortName": "Stork"
+    },
+    {
         "chainId": 49797,
         "faucets": [],
         "infoURL": "https://www.energi.world/",
         "name": "Energi Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Energi",
@@ -14154,14 +18586,46 @@
         "networkId": 50001,
         "rpc": [
             "https://rpc.oracle.liveplex.io"
         ],
         "shortName": "LOE"
     },
     {
+        "chainId": 50005,
+        "faucets": [],
+        "infoURL": "https://yooldo.gg/",
+        "name": "Yooldo Verse Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "OAS",
+            "symbol": "OAS"
+        },
+        "networkId": 50005,
+        "rpc": [
+            "https://rpc.yooldo-verse.xyz/"
+        ],
+        "shortName": "YVM"
+    },
+    {
+        "chainId": 50006,
+        "faucets": [],
+        "infoURL": "https://yooldo.gg/",
+        "name": "Yooldo Verse Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "OAS",
+            "symbol": "OAS"
+        },
+        "networkId": 50006,
+        "rpc": [
+            "https://rpc.testnet.yooldo-verse.xyz/"
+        ],
+        "shortName": "YVT"
+    },
+    {
         "chainId": 50021,
         "faucets": [],
         "infoURL": "https://gton.capital",
         "name": "GTON Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "GCD",
@@ -14216,19 +18680,52 @@
         "nativeCurrency": {
             "decimals": 18,
             "name": "Electroneum",
             "symbol": "ETN"
         },
         "networkId": 52014,
         "rpc": [
-            "https://api.electroneum.com"
+            "https://rpc.electroneum.com"
         ],
         "shortName": "etn-mainnet"
     },
     {
+        "chainId": 53277,
+        "faucets": [],
+        "infoURL": "https://doid.tech",
+        "name": "DOID",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "DOID",
+            "symbol": "DOID"
+        },
+        "networkId": 53277,
+        "rpc": [
+            "https://rpc.doid.tech"
+        ],
+        "shortName": "DOID"
+    },
+    {
+        "chainId": 53457,
+        "faucets": [],
+        "infoURL": "https://www.dodochain.com",
+        "name": "DODOchain testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Berd",
+            "symbol": "BERD"
+        },
+        "networkId": 53457,
+        "rpc": [
+            "https://dodochain-testnet.alt.technology",
+            "wss://dodochain-testnet.alt.technology/ws"
+        ],
+        "shortName": "dodochain"
+    },
+    {
         "chainId": 53935,
         "faucets": [],
         "infoURL": "https://defikingdoms.com",
         "name": "DFK Chain",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Jewel",
@@ -14271,14 +18768,32 @@
         "networkId": 54321,
         "rpc": [
             "http://testnet.toronet.org/rpc"
         ],
         "shortName": "ToronetTestnet"
     },
     {
+        "chainId": 54555,
+        "faucets": [
+            "https://photonchain.io/airdrop"
+        ],
+        "infoURL": "https://photonchain.io",
+        "name": "Photon Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Photon",
+            "symbol": "PTON"
+        },
+        "networkId": 54555,
+        "rpc": [
+            "https://rpc-test.photonchain.io"
+        ],
+        "shortName": "pton"
+    },
+    {
         "chainId": 55004,
         "faucets": [],
         "infoURL": "https://tokamak.network",
         "name": "Titan",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Ether",
@@ -14324,14 +18839,30 @@
         "networkId": 55556,
         "rpc": [
             "https://rei-testnet-rpc.moonrhythm.io"
         ],
         "shortName": "trei"
     },
     {
+        "chainId": 56026,
+        "faucets": [],
+        "infoURL": "https://lambda.im",
+        "name": "Lambda Chain Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "ETH",
+            "symbol": "ETH"
+        },
+        "networkId": 56026,
+        "rpc": [
+            "https://nrpc.lambda.im/"
+        ],
+        "shortName": "lambda"
+    },
+    {
         "chainId": 56288,
         "faucets": [],
         "infoURL": "https://boba.network",
         "name": "Boba BNB Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Boba Token",
@@ -14345,14 +18876,30 @@
             "https://replica.bnb.boba.network",
             "wss://boba-bnb.gateway.tenderly.co/",
             "wss://gateway.tenderly.co/public/boba-bnb"
         ],
         "shortName": "BobaBnb"
     },
     {
+        "chainId": 56400,
+        "faucets": [],
+        "infoURL": "https://zeroone.art/",
+        "name": "Testnet Zeroone Subnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "ZERO",
+            "symbol": "ZERO"
+        },
+        "networkId": 56400,
+        "rpc": [
+            "https://subnets.avax.network/testnetzer/testnet/rpc"
+        ],
+        "shortName": "testnetzer"
+    },
+    {
         "chainId": 56789,
         "faucets": [
             "https://nova-faucet.velo.org"
         ],
         "infoURL": "https://velo.org",
         "name": "VELO Labs Mainnet",
         "nativeCurrency": {
@@ -14363,14 +18910,30 @@
         "networkId": 56789,
         "rpc": [
             "https://nova.velo.org"
         ],
         "shortName": "VELO"
     },
     {
+        "chainId": 56797,
+        "faucets": [],
+        "infoURL": "https://doid.tech",
+        "name": "DOID Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "DOID",
+            "symbol": "DOID"
+        },
+        "networkId": 56797,
+        "rpc": [
+            "https://rpc.testnet.doid.tech"
+        ],
+        "shortName": "doidTestnet"
+    },
+    {
         "chainId": 57000,
         "faucets": [
             "https://rollux.id/faucetapp"
         ],
         "infoURL": "https://rollux.com",
         "name": "Rollux Testnet",
         "nativeCurrency": {
@@ -14378,15 +18941,17 @@
             "name": "Testnet Syscoin",
             "symbol": "TSYS"
         },
         "networkId": 57000,
         "rpc": [
             "https://rpc-tanenbaum.rollux.com",
             "https://rpc.ankr.com/rollux_testnet/${ANKR_API_KEY}",
-            "wss://rpc-tanenbaum.rollux.com/wss"
+            "wss://rpc-tanenbaum.rollux.com/wss",
+            "https://rollux.rpc.tanenbaum.io",
+            "wss://rollux.rpc.tanenbaum.io/wss"
         ],
         "shortName": "tsys-rollux"
     },
     {
         "chainId": 58008,
         "faucets": [],
         "infoURL": "https://publicgoods.network/",
@@ -14404,28 +18969,47 @@
     },
     {
         "chainId": 59140,
         "faucets": [
             "https://faucetlink.to/goerli"
         ],
         "infoURL": "https://linea.build",
-        "name": "Linea Testnet",
+        "name": "Linea Goerli",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Linea Ether",
             "symbol": "ETH"
         },
         "networkId": 59140,
         "rpc": [
             "https://rpc.goerli.linea.build",
             "wss://rpc.goerli.linea.build",
             "https://linea-goerli.infura.io/v3/${INFURA_API_KEY}",
             "wss://linea-goerli.infura.io/ws/v3/${INFURA_API_KEY}"
         ],
-        "shortName": "linea-testnet"
+        "shortName": "linea-goerli"
+    },
+    {
+        "chainId": 59141,
+        "faucets": [],
+        "infoURL": "https://linea.build",
+        "name": "Linea Sepolia",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Linea Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 59141,
+        "rpc": [
+            "https://rpc.sepolia.linea.build",
+            "wss://rpc.sepolia.linea.build",
+            "https://linea-sepolia.infura.io/v3/${INFURA_API_KEY}",
+            "wss://linea-sepolia.infura.io/ws/v3/${INFURA_API_KEY}"
+        ],
+        "shortName": "linea-sepolia"
     },
     {
         "chainId": 59144,
         "faucets": [],
         "infoURL": "https://linea.build",
         "name": "Linea",
         "nativeCurrency": {
@@ -14439,14 +19023,30 @@
             "wss://rpc.linea.build",
             "https://linea-mainnet.infura.io/v3/${INFURA_API_KEY}",
             "wss://linea-mainnet.infura.io/ws/v3/${INFURA_API_KEY}"
         ],
         "shortName": "linea"
     },
     {
+        "chainId": 59971,
+        "faucets": [],
+        "infoURL": "https://genesyscode.io",
+        "name": "Genesys Code Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "GenesysCode",
+            "symbol": "GCODE"
+        },
+        "networkId": 59971,
+        "rpc": [
+            "https://mainnet.genesyscode.io/"
+        ],
+        "shortName": "gcode"
+    },
+    {
         "chainId": 60000,
         "faucets": [
             "https://www.thinkiumdev.net/faucet"
         ],
         "infoURL": "https://thinkium.net/",
         "name": "Thinkium Testnet Chain 0",
         "nativeCurrency": {
@@ -14511,14 +19111,47 @@
         "networkId": 60103,
         "rpc": [
             "https://test103.thinkiumrpc.net/"
         ],
         "shortName": "TKM-test103"
     },
     {
+        "chainId": 60808,
+        "faucets": [],
+        "infoURL": "https://gobob.xyz",
+        "name": "BOB",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 60808,
+        "rpc": [
+            "https://rpc.gobob.xyz",
+            "wss://rpc.gobob.xyz"
+        ],
+        "shortName": "bob"
+    },
+    {
+        "chainId": 61406,
+        "faucets": [],
+        "infoURL": "https://kaichain.net",
+        "name": "KaiChain",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "KaiChain Native Token",
+            "symbol": "KEC"
+        },
+        "networkId": 61406,
+        "rpc": [
+            "https://mainnet-rpc.kaichain.net"
+        ],
+        "shortName": "kec"
+    },
+    {
         "chainId": 61800,
         "faucets": [],
         "infoURL": "https://www.axel.org",
         "name": "AxelChain Dev-Net",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Axelium",
@@ -14564,14 +19197,44 @@
             "https://sgrpc.doken.dev",
             "https://nyrpc.doken.dev",
             "https://ukrpc.doken.dev"
         ],
         "shortName": "DoKEN"
     },
     {
+        "chainId": 62049,
+        "faucets": [],
+        "infoURL": "https://optopia.ai",
+        "name": "OPTOPIA Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 62049,
+        "rpc": [
+            "https://rpc-testnet.optopia.ai"
+        ],
+        "shortName": "OPTOPIA-Testnet"
+    },
+    {
+        "chainId": 62050,
+        "faucets": [],
+        "infoURL": "https://optopia.ai",
+        "name": "Optopia Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 62050,
+        "rpc": [],
+        "shortName": "Optopia"
+    },
+    {
         "chainId": 62320,
         "faucets": [
             "https://docs.google.com/forms/d/e/1FAIpQLSdfr1BwUTYepVmmvfVUDRCwALejZ-TUva2YujNpvrEmPAX2pg/viewform",
             "https://cauldron.pretoriaresearchlab.io/baklava-faucet"
         ],
         "infoURL": "https://docs.celo.org/",
         "name": "Celo Baklava Testnet",
@@ -14650,14 +19313,30 @@
         "networkId": 65450,
         "rpc": [
             "https://mainnet-rpc.scolcoin.com"
         ],
         "shortName": "SRC"
     },
     {
+        "chainId": 66988,
+        "faucets": [],
+        "infoURL": "https://janus-network.gitbook.io/janus",
+        "name": "Janus Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Janus",
+            "symbol": "JNS"
+        },
+        "networkId": 66988,
+        "rpc": [
+            "https://rpc.test.janusnetwork.io"
+        ],
+        "shortName": "janusnetwork-testnet"
+    },
+    {
         "chainId": 67390,
         "faucets": [],
         "infoURL": "https://macaucasinolisboa.xyz",
         "name": "SiriusNet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "MCD",
@@ -14780,14 +19459,30 @@
         "networkId": 70103,
         "rpc": [
             "https://proxy103.thinkiumrpc.net/"
         ],
         "shortName": "TKM103"
     },
     {
+        "chainId": 70700,
+        "faucets": [],
+        "infoURL": "https://proofofplay.com",
+        "name": "Proof of Play - Apex",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 70700,
+        "rpc": [
+            "https://rpc.apex.proofofplay.com"
+        ],
+        "shortName": "pop-apex"
+    },
+    {
         "chainId": 71111,
         "faucets": [],
         "infoURL": "https://guapcoin.org/",
         "name": "GuapcoinX",
         "nativeCurrency": {
             "decimals": 18,
             "name": "GuapcoinX",
@@ -14852,14 +19547,81 @@
         "networkId": 71402,
         "rpc": [
             "https://v1.mainnet.godwoken.io/rpc"
         ],
         "shortName": "gw-mainnet-v1"
     },
     {
+        "chainId": 72778,
+        "faucets": [],
+        "infoURL": "https://www.cagacrypto.com/",
+        "name": "CAGA crypto Ankara testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Caga",
+            "symbol": "CAGA"
+        },
+        "networkId": 72778,
+        "rpc": [
+            "https://www.ankara-cagacrypto.com",
+            "wss://wss.ankara-cagacrypto.com"
+        ],
+        "shortName": "caga"
+    },
+    {
+        "chainId": 72992,
+        "faucets": [],
+        "infoURL": "https://grokchain.dev",
+        "name": "Grok Chain Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Groc",
+            "symbol": "GROC"
+        },
+        "networkId": 72992,
+        "rpc": [
+            "https://mainnet-rpc.grokchain.dev"
+        ],
+        "shortName": "GrokChain"
+    },
+    {
+        "chainId": 73114,
+        "faucets": [],
+        "infoURL": "https://icb.network",
+        "name": "ICB Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "ICB Testnet Token",
+            "symbol": "ICBT"
+        },
+        "networkId": 73114,
+        "rpc": [
+            "https://rpc1-testnet.icbnetwork.info/",
+            "https://rpc2-testnet.icbnetwork.info/"
+        ],
+        "shortName": "ICBT"
+    },
+    {
+        "chainId": 73115,
+        "faucets": [],
+        "infoURL": "https://icb.network",
+        "name": "ICB Network",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "ICB Native Token",
+            "symbol": "ICBX"
+        },
+        "networkId": 73115,
+        "rpc": [
+            "https://rpc1-mainnet.icbnetwork.info/",
+            "https://rpc2-mainnet.icbnetwork.info/"
+        ],
+        "shortName": "ICBX"
+    },
+    {
         "chainId": 73799,
         "faucets": [
             "https://voltafaucet.energyweb.org"
         ],
         "infoURL": "https://energyweb.org",
         "name": "Energy Web Volta Testnet",
         "nativeCurrency": {
@@ -14901,14 +19663,30 @@
             "symbol": "RESIN"
         },
         "networkId": 75000,
         "rpc": [],
         "shortName": "resin"
     },
     {
+        "chainId": 77001,
+        "faucets": [],
+        "infoURL": "https://www.boraportal.com",
+        "name": "BORAchain mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "BGAS",
+            "symbol": "BGAS"
+        },
+        "networkId": 77001,
+        "rpc": [
+            "https://public-node.api.boraportal.com/bora/mainnet"
+        ],
+        "shortName": "BORAchain"
+    },
+    {
         "chainId": 77238,
         "faucets": [
             "https://faucet.foundryscan.org"
         ],
         "infoURL": "https://foundrychain.org",
         "name": "Foundry Chain Testnet",
         "nativeCurrency": {
@@ -15036,14 +19814,33 @@
         "networkId": 78432,
         "rpc": [
             "https://subnets.avax.network/conduit/testnet/rpc"
         ],
         "shortName": "conduit"
     },
     {
+        "chainId": 78600,
+        "faucets": [
+            "https://faucet.vanarchain.com"
+        ],
+        "infoURL": "https://vanarchain.com",
+        "name": "Vanguard",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Vanguard Vanry",
+            "symbol": "VANRY"
+        },
+        "networkId": 78600,
+        "rpc": [
+            "https://rpc-vanguard.vanarchain.com",
+            "wss://ws-vanguard.vanarchain.com"
+        ],
+        "shortName": "vanguard"
+    },
+    {
         "chainId": 79879,
         "faucets": [
             "https://faucet.goldsmartchain.com"
         ],
         "infoURL": "https://goldsmartchain.com",
         "name": "Gold Smart Chain Testnet",
         "nativeCurrency": {
@@ -15068,22 +19865,93 @@
             "decimals": 18,
             "name": "MATIC",
             "symbol": "MATIC"
         },
         "networkId": 80001,
         "rpc": [
             "https://rpc-mumbai.maticvigil.com",
-            "https://polygon-mumbai-bor.publicnode.com",
-            "wss://polygon-mumbai-bor.publicnode.com",
+            "https://polygon-mumbai-bor-rpc.publicnode.com",
+            "wss://polygon-mumbai-bor-rpc.publicnode.com",
             "https://polygon-mumbai.gateway.tenderly.co",
             "wss://polygon-mumbai.gateway.tenderly.co"
         ],
         "shortName": "maticmum"
     },
     {
+        "chainId": 80002,
+        "faucets": [
+            "https://faucet.polygon.technology/"
+        ],
+        "infoURL": "https://polygon.technology/",
+        "name": "Amoy",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "MATIC",
+            "symbol": "MATIC"
+        },
+        "networkId": 80002,
+        "rpc": [
+            "https://rpc-amoy.polygon.technology",
+            "https://polygon-amoy-bor-rpc.publicnode.com",
+            "wss://polygon-amoy-bor-rpc.publicnode.com"
+        ],
+        "shortName": "polygonamoy"
+    },
+    {
+        "chainId": 80085,
+        "faucets": [
+            "https://artio.faucet.berachain.com"
+        ],
+        "infoURL": "https://www.berachain.com",
+        "name": "Berachain Artio",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "BERA Token",
+            "symbol": "BERA"
+        },
+        "networkId": 80085,
+        "rpc": [
+            "https://artio.rpc.berachain.com",
+            "https://rpc.ankr.com/berachain_testnet"
+        ],
+        "shortName": "berachainArtio"
+    },
+    {
+        "chainId": 80096,
+        "faucets": [],
+        "infoURL": "http://hizoco.net",
+        "name": "Hizoco mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Hizoco",
+            "symbol": "HZC"
+        },
+        "networkId": 80096,
+        "rpc": [
+            "https://hizoco.net/rpc"
+        ],
+        "shortName": "hzc"
+    },
+    {
+        "chainId": 81041,
+        "faucets": [],
+        "infoURL": "https://nordekscan.com",
+        "name": "Nordek Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "NRK",
+            "symbol": "NRK"
+        },
+        "networkId": 81041,
+        "rpc": [
+            "https://mainnet-rpc.nordekscan.com"
+        ],
+        "shortName": "nordek"
+    },
+    {
         "chainId": 81341,
         "faucets": [],
         "infoURL": "https://github.com/Qitmeer",
         "name": "Amana Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Amana Testnet",
@@ -15202,14 +20070,34 @@
             "symbol": "MEER-P"
         },
         "networkId": 81363,
         "rpc": [],
         "shortName": "mizanapriv"
     },
     {
+        "chainId": 81457,
+        "faucets": [],
+        "infoURL": "https://blast.io/",
+        "name": "Blast",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 81457,
+        "rpc": [
+            "https://rpc.blast.io",
+            "https://rpc.ankr.com/blast",
+            "https://blast.din.dev/rpc",
+            "https://blastl2-mainnet.public.blastapi.io",
+            "https://blast.blockpi.network/v1/rpc/public"
+        ],
+        "shortName": "blastmainnet"
+    },
+    {
         "chainId": 81720,
         "faucets": [],
         "infoURL": "https://quantumnetwork.gg",
         "name": "Quantum Chain Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Quantum Chain",
@@ -15218,14 +20106,46 @@
         "networkId": 81720,
         "rpc": [
             "https://rpc.quantumscan.org"
         ],
         "shortName": "qnet"
     },
     {
+        "chainId": 82459,
+        "faucets": [],
+        "infoURL": "https://www.smartlayer.network/",
+        "name": "Smart Layer Network Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Service Unit Token",
+            "symbol": "SU"
+        },
+        "networkId": 82459,
+        "rpc": [
+            "https://rpc.test.smartlayer.network"
+        ],
+        "shortName": "tSLN"
+    },
+    {
+        "chainId": 83872,
+        "faucets": [],
+        "infoURL": "https://docs.zedscan.net",
+        "name": "ZEDXION",
+        "nativeCurrency": {
+            "decimals": 9,
+            "name": "Zedxion",
+            "symbol": "zedx"
+        },
+        "networkId": 83872,
+        "rpc": [
+            "https://mainnet-rpc.zedscan.net"
+        ],
+        "shortName": "ZEDX"
+    },
+    {
         "chainId": 84531,
         "faucets": [
             "https://www.coinbase.com/faucets/base-ethereum-goerli-faucet"
         ],
         "infoURL": "https://base.org",
         "name": "Base Goerli Testnet",
         "nativeCurrency": {
@@ -15234,16 +20154,16 @@
             "symbol": "ETH"
         },
         "networkId": 84531,
         "rpc": [
             "https://goerli.base.org",
             "https://base-goerli.gateway.tenderly.co",
             "wss://base-goerli.gateway.tenderly.co",
-            "https://base-goerli.publicnode.com",
-            "wss://base-goerli.publicnode.com"
+            "https://base-goerli-rpc.publicnode.com",
+            "wss://base-goerli-rpc.publicnode.com"
         ],
         "shortName": "basegor"
     },
     {
         "chainId": 84532,
         "faucets": [],
         "infoURL": "https://base.org",
@@ -15251,15 +20171,17 @@
         "nativeCurrency": {
             "decimals": 18,
             "name": "Sepolia Ether",
             "symbol": "ETH"
         },
         "networkId": 84532,
         "rpc": [
-            "https://sepolia.base.org"
+            "https://sepolia.base.org",
+            "https://base-sepolia-rpc.publicnode.com",
+            "wss://base-sepolia-rpc.publicnode.com"
         ],
         "shortName": "basesep"
     },
     {
         "chainId": 84886,
         "faucets": [],
         "infoURL": "https://aerielab.io/",
@@ -15306,14 +20228,46 @@
         "networkId": 88002,
         "rpc": [
             "https://api.proteus.nautchain.xyz/solana"
         ],
         "shortName": "NAUTTest"
     },
     {
+        "chainId": 88817,
+        "faucets": [],
+        "infoURL": "https://units.network",
+        "name": "Unit Zero Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "UNIT0",
+            "symbol": "UNIT0"
+        },
+        "networkId": 88817,
+        "rpc": [
+            "https://rpc-testnet.unit0.dev"
+        ],
+        "shortName": "unit0-testnet"
+    },
+    {
+        "chainId": 88819,
+        "faucets": [],
+        "infoURL": "https://units.network",
+        "name": "Unit Zero Stagenet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "UNIT0",
+            "symbol": "UNIT0"
+        },
+        "networkId": 88819,
+        "rpc": [
+            "https://rpc-stagenet.unit0.dev"
+        ],
+        "shortName": "unit0-stagenet"
+    },
+    {
         "chainId": 88880,
         "faucets": [
             "https://scoville-faucet.chiliz.com"
         ],
         "infoURL": "https://www.chiliz.com/en/chain",
         "name": "Chiliz Scoville Testnet",
         "nativeCurrency": {
@@ -15342,14 +20296,30 @@
         "networkId": 88888,
         "rpc": [
             "https://mainnet-rpc.ivarex.com"
         ],
         "shortName": "ivar"
     },
     {
+        "chainId": 90001,
+        "faucets": [],
+        "infoURL": "https://functionx.io/",
+        "name": "F(x)Core Testnet Network",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Function X",
+            "symbol": "FX"
+        },
+        "networkId": 90001,
+        "rpc": [
+            "https://testnet-fx-json-web3.functionx.io:8545"
+        ],
+        "shortName": "dhobyghaut"
+    },
+    {
         "chainId": 90210,
         "faucets": [
             "https://faucet.beverlyhills.ethdevops.io"
         ],
         "infoURL": "https://beverlyhills.ethdevops.io",
         "name": "Beverly Hills",
         "nativeCurrency": {
@@ -15360,14 +20330,32 @@
         "networkId": 90210,
         "rpc": [
             "https://rpc.beverlyhills.ethdevops.io:8545"
         ],
         "shortName": "bvhl"
     },
     {
+        "chainId": 90354,
+        "faucets": [
+            "https://www.campnetwork.xyz/faucet"
+        ],
+        "infoURL": "https://campaign-1.gitbook.io/camp-technical-docs\u00e5",
+        "name": "Camp Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ethereum",
+            "symbol": "ETH"
+        },
+        "networkId": 90354,
+        "rpc": [
+            "https://rpc-camp-network-4xje7wy105.t.conduit.xyz"
+        ],
+        "shortName": "camp"
+    },
+    {
         "chainId": 91002,
         "faucets": [
             "https://faucet.eclipse.builders"
         ],
         "infoURL": "https://docs.nautchain.xyz",
         "name": "Nautilus Trition Chain",
         "nativeCurrency": {
@@ -15378,14 +20366,47 @@
         "networkId": 91002,
         "rpc": [
             "https://triton.api.nautchain.xyz"
         ],
         "shortName": "NAUT"
     },
     {
+        "chainId": 91120,
+        "faucets": [],
+        "infoURL": "https://metadap.io/",
+        "name": "MetaDAP Enterprise Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "DAP",
+            "symbol": "DAP"
+        },
+        "networkId": 91120,
+        "rpc": [
+            "https://rpc.chain.metadap.io",
+            "wss://rpc-ws.chain.metadap.io"
+        ],
+        "shortName": "MetaDAP"
+    },
+    {
+        "chainId": 91715,
+        "faucets": [],
+        "infoURL": "https://combonetwork.io",
+        "name": "Combo Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "BNB Chain Native Token",
+            "symbol": "tcBNB"
+        },
+        "networkId": 91715,
+        "rpc": [
+            "https://test-rpc.combonetwork.io"
+        ],
+        "shortName": "combo-testnet"
+    },
+    {
         "chainId": 92001,
         "faucets": [
             "https://faucet.lambda.top"
         ],
         "infoURL": "https://lambda.im",
         "name": "Lambda Testnet",
         "nativeCurrency": {
@@ -15396,14 +20417,32 @@
         "networkId": 92001,
         "rpc": [
             "https://evm.lambda.top/"
         ],
         "shortName": "lambda-testnet"
     },
     {
+        "chainId": 93572,
+        "faucets": [
+            "https://claim.liquidlayer.network"
+        ],
+        "infoURL": "https://testnet-scan.liquidlayer.network",
+        "name": "LiquidLayer Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "LiquidLayer Testnet",
+            "symbol": "LILA"
+        },
+        "networkId": 93572,
+        "rpc": [
+            "https://testnet.liquidlayer.network"
+        ],
+        "shortName": "tLILA"
+    },
+    {
         "chainId": 96970,
         "faucets": [
             "https://mantis.switch.ch/faucet",
             "https://mantis.kore-technologies.ch/faucet",
             "https://mantis.phoenix-systems.io/faucet",
             "https://mantis.block-spirit.ch/faucet"
         ],
@@ -15680,29 +20719,43 @@
         },
         "networkId": 100100,
         "rpc": [],
         "shortName": "chi1"
     },
     {
         "chainId": 101010,
-        "faucets": [
-            "https://faucet.soverun.com"
-        ],
-        "infoURL": "https://soverun.com",
-        "name": "Soverun Testnet",
+        "faucets": [],
+        "infoURL": "https://stabilityprotocol.com",
+        "name": "Global Trust Network",
         "nativeCurrency": {
             "decimals": 18,
-            "name": "Soverun",
-            "symbol": "SVRN"
+            "name": "FREE",
+            "symbol": "FREE"
         },
         "networkId": 101010,
         "rpc": [
-            "https://testnet-rpc.soverun.com"
+            "https://gtn.stabilityprotocol.com"
         ],
-        "shortName": "SVRNt"
+        "shortName": "stabilityprotocol"
+    },
+    {
+        "chainId": 102031,
+        "faucets": [],
+        "infoURL": "https://creditcoin.org",
+        "name": "Creditcoin Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Testnet CTC",
+            "symbol": "tCTC"
+        },
+        "networkId": 102031,
+        "rpc": [
+            "https://rpc.cc3-testnet.creditcoin.network"
+        ],
+        "shortName": "ctctest"
     },
     {
         "chainId": 103090,
         "faucets": [],
         "infoURL": "https://crystaleum.org",
         "name": "Crystaleum",
         "nativeCurrency": {
@@ -15714,14 +20767,63 @@
         "rpc": [
             "https://evm.cryptocurrencydevs.org",
             "https://rpc.crystaleum.org"
         ],
         "shortName": "CRFI"
     },
     {
+        "chainId": 103454,
+        "faucets": [],
+        "infoURL": "https://masa.finance",
+        "name": "Masa Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Masa Token",
+            "symbol": "MASA"
+        },
+        "networkId": 103454,
+        "rpc": [
+            "https://subnets.avax.network/masatestne/testnet/rpc"
+        ],
+        "shortName": "masatest"
+    },
+    {
+        "chainId": 104566,
+        "faucets": [],
+        "infoURL": "https://kaspaclassic.com/",
+        "name": "KaspaClassic Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "KaspaClassic",
+            "symbol": "CAS"
+        },
+        "networkId": 104566,
+        "rpc": [
+            "https://api.kaspaclassic.world/",
+            "http://80.178.101.118:8000/"
+        ],
+        "shortName": "cas"
+    },
+    {
+        "chainId": 105105,
+        "faucets": [],
+        "infoURL": "https://www.stratisplatform.com",
+        "name": "Stratis Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Stratis",
+            "symbol": "STRAX"
+        },
+        "networkId": 105105,
+        "rpc": [
+            "https://rpc.stratisevm.com"
+        ],
+        "shortName": "stratis"
+    },
+    {
         "chainId": 108801,
         "faucets": [],
         "infoURL": "https://brochain.org",
         "name": "BROChain Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Brother",
@@ -15918,14 +21020,31 @@
         "rpc": [
             "https://rpc.main.siberium.net",
             "https://rpc.main.siberium.net.ru"
         ],
         "shortName": "sbr"
     },
     {
+        "chainId": 111188,
+        "faucets": [],
+        "infoURL": "https://re.al",
+        "name": "re.al",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "re.al Ether",
+            "symbol": "reETH"
+        },
+        "networkId": 111188,
+        "rpc": [
+            "https://real.drpc.org",
+            "wss://real.drpc.org"
+        ],
+        "shortName": "re-al"
+    },
+    {
         "chainId": 112358,
         "faucets": [],
         "infoURL": "https://metachain.one",
         "name": "Metachain One Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Metao",
@@ -15935,14 +21054,31 @@
         "rpc": [
             "https://rpc.metachain.one",
             "https://rpc2.metachain.one"
         ],
         "shortName": "metao"
     },
     {
+        "chainId": 119139,
+        "faucets": [],
+        "infoURL": "https://metadap.io/",
+        "name": "MetaDAP Enterprise Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "DAP",
+            "symbol": "DAP"
+        },
+        "networkId": 119139,
+        "rpc": [
+            "https://rpc.testnet.chain.metadap.io",
+            "wss://rpc-ws.testnet.chain.metadap.io"
+        ],
+        "shortName": "MetaDAP-T"
+    },
+    {
         "chainId": 123456,
         "faucets": [],
         "infoURL": "https://adilchain.io",
         "name": "ADIL Devnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Devnet ADIL",
@@ -15951,14 +21087,50 @@
         "networkId": 123456,
         "rpc": [
             "https://devnet.adilchain-rpc.io"
         ],
         "shortName": "dadil"
     },
     {
+        "chainId": 128123,
+        "faucets": [
+            "https://faucet.etherlink.com"
+        ],
+        "infoURL": "https://etherlink.com",
+        "name": "Etherlink Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "tez",
+            "symbol": "XTZ"
+        },
+        "networkId": 128123,
+        "rpc": [
+            "https://node.ghostnet.etherlink.com"
+        ],
+        "shortName": "etlt"
+    },
+    {
+        "chainId": 131313,
+        "faucets": [
+            "https://faucet.dioneprotocol.com/"
+        ],
+        "infoURL": "https://www.dioneprotocol.com/",
+        "name": "Odyssey Chain (Testnet)",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "DIONE",
+            "symbol": "DIONE"
+        },
+        "networkId": 131313,
+        "rpc": [
+            "https://testnode.dioneprotocol.com/ext/bc/D/rpc"
+        ],
+        "shortName": "DIONE"
+    },
+    {
         "chainId": 131419,
         "faucets": [],
         "infoURL": "https://www.etnd.pro",
         "name": "ETND Chain Mainnets",
         "nativeCurrency": {
             "decimals": 18,
             "name": "ETND",
@@ -15967,14 +21139,30 @@
         "networkId": 131419,
         "rpc": [
             "https://rpc.node1.etnd.pro/"
         ],
         "shortName": "ETND"
     },
     {
+        "chainId": 141319,
+        "faucets": [],
+        "infoURL": "https://magape.io",
+        "name": "MagApe Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "MagApe",
+            "symbol": "MAG"
+        },
+        "networkId": 141319,
+        "rpc": [
+            "https://testnet-api.magape.io/chain/"
+        ],
+        "shortName": "mag"
+    },
+    {
         "chainId": 142857,
         "faucets": [],
         "infoURL": "https://docs.ic-plaza.org/",
         "name": "ICPlaza Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "ict",
@@ -15983,14 +21171,45 @@
         "networkId": 142857,
         "rpc": [
             "https://rpcmainnet.ic-plaza.org/"
         ],
         "shortName": "ICPlaza"
     },
     {
+        "chainId": 161212,
+        "faucets": [],
+        "infoURL": "https://www.playfi.ai/",
+        "name": "PlayFi Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Play",
+            "symbol": "PLAY"
+        },
+        "networkId": 161212,
+        "rpc": [],
+        "shortName": "playfi"
+    },
+    {
+        "chainId": 167000,
+        "faucets": [],
+        "infoURL": "https://taiko.xyz",
+        "name": "Taiko Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 167000,
+        "rpc": [
+            "https://rpc.taiko.xyz",
+            "wss://ws.taiko.xyz"
+        ],
+        "shortName": "tko-mainnet"
+    },
+    {
         "chainId": 167004,
         "faucets": [],
         "infoURL": "https://taiko.xyz",
         "name": "Taiko (Alpha-2 Testnet)",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Ether",
@@ -16047,14 +21266,50 @@
         "networkId": 167007,
         "rpc": [
             "https://rpc.jolnir.taiko.xyz"
         ],
         "shortName": "tko-jolnir"
     },
     {
+        "chainId": 167008,
+        "faucets": [],
+        "infoURL": "https://taiko.xyz",
+        "name": "Taiko Katla L2",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 167008,
+        "rpc": [
+            "https://rpc.katla.taiko.xyz",
+            "wss://ws.katla.taiko.xyz",
+            "https://taiko-katla.drpc.org",
+            "wss://taiko-katla.drpc.org"
+        ],
+        "shortName": "tko-katla"
+    },
+    {
+        "chainId": 167009,
+        "faucets": [],
+        "infoURL": "https://taiko.xyz",
+        "name": "Taiko Hekla L2",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 167009,
+        "rpc": [
+            "https://rpc.hekla.taiko.xyz",
+            "wss://ws.hekla.taiko.xyz"
+        ],
+        "shortName": "tko-hekla"
+    },
+    {
         "chainId": 188710,
         "faucets": [],
         "infoURL": "https://biticablockchain.com/",
         "name": "Bitica Chain Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Bitica Coin",
@@ -16081,14 +21336,48 @@
         "networkId": 188881,
         "rpc": [
             "https://testnet.condor.systems/rpc"
         ],
         "shortName": "condor"
     },
     {
+        "chainId": 192940,
+        "faucets": [],
+        "infoURL": "https://mindnetwork.xyz",
+        "name": "Mind Network Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "FHE",
+            "symbol": "FHE"
+        },
+        "networkId": 192940,
+        "rpc": [
+            "https://rpc-testnet.mindnetwork.xyz",
+            "wss://rpc-testnet.mindnetwork.xyz"
+        ],
+        "shortName": "fhet"
+    },
+    {
+        "chainId": 200000,
+        "faucets": [],
+        "infoURL": "https://xfair.ai",
+        "name": "xFair.AI Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "FAI",
+            "symbol": "FAI"
+        },
+        "networkId": 200000,
+        "rpc": [
+            "https://rpc_testnet.xfair.ai",
+            "wss://rpc_testnet.xfair.ai"
+        ],
+        "shortName": "fait"
+    },
+    {
         "chainId": 200101,
         "faucets": [],
         "infoURL": "https://milkomeda.com",
         "name": "Milkomeda C1 Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "milkTAda",
@@ -16130,14 +21419,56 @@
         "networkId": 200625,
         "rpc": [
             "https://remote.akroma.io"
         ],
         "shortName": "aka"
     },
     {
+        "chainId": 200810,
+        "faucets": [
+            "https://www.bitlayer.org/faucet"
+        ],
+        "infoURL": "https://docs.bitlayer.org/",
+        "name": "Bitlayer Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "BTC",
+            "symbol": "BTC"
+        },
+        "networkId": 200810,
+        "rpc": [
+            "https://testnet-rpc.bitlayer.org",
+            "wss://testnet-ws.bitlayer.org",
+            "https://testnet-rpc.bitlayer-rpc.com",
+            "wss://testnet-ws.bitlayer-rpc.com",
+            "https://rpc.ankr.com/bitlayer_testnet"
+        ],
+        "shortName": "btrt"
+    },
+    {
+        "chainId": 200901,
+        "faucets": [],
+        "infoURL": "https://docs.bitlayer.org/",
+        "name": "Bitlayer Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "BTC",
+            "symbol": "BTC"
+        },
+        "networkId": 200901,
+        "rpc": [
+            "https://rpc.bitlayer.org",
+            "https://rpc.bitlayer-rpc.com",
+            "https://rpc.ankr.com/bitlayer",
+            "wss://ws.bitlayer.org",
+            "wss://ws.bitlayer-rpc.com"
+        ],
+        "shortName": "btr"
+    },
+    {
         "chainId": 201018,
         "faucets": [],
         "infoURL": "https://www.alaya.network/",
         "name": "Alaya Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "ATP",
@@ -16198,14 +21529,46 @@
         "networkId": 202020,
         "rpc": [
             "https://testnet-val.decimalchain.com/web3/"
         ],
         "shortName": "tDSC"
     },
     {
+        "chainId": 202212,
+        "faucets": [],
+        "infoURL": "https://docs.xen.network/x1/",
+        "name": "X1 Devnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "XN",
+            "symbol": "XN"
+        },
+        "networkId": 202212,
+        "rpc": [
+            "https://x1-devnet.xen.network"
+        ],
+        "shortName": "x1-devnet"
+    },
+    {
+        "chainId": 202401,
+        "faucets": [],
+        "infoURL": "https://www.ymtech.co.kr",
+        "name": "YMTECH-BESU Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "ETH",
+            "symbol": "ETH"
+        },
+        "networkId": 202401,
+        "rpc": [
+            "http://39.119.118.216:8545"
+        ],
+        "shortName": "YMTECH-BESU"
+    },
+    {
         "chainId": 202624,
         "faucets": [],
         "infoURL": "https://twala.io/",
         "name": "Jellie",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Twala Coin",
@@ -16215,14 +21578,64 @@
         "rpc": [
             "https://jellie-rpc.twala.io/",
             "wss://jellie-rpc-wss.twala.io/"
         ],
         "shortName": "twl-jellie"
     },
     {
+        "chainId": 204005,
+        "faucets": [],
+        "infoURL": "https://docs.xen.network/go-x1/",
+        "name": "X1 Network",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "XN",
+            "symbol": "XN"
+        },
+        "networkId": 204005,
+        "rpc": [
+            "https://x1-testnet.xen.network"
+        ],
+        "shortName": "x1-testnet"
+    },
+    {
+        "chainId": 205205,
+        "faucets": [
+            "https://auroria.faucet.stratisevm.com"
+        ],
+        "infoURL": "https://www.stratisplatform.com",
+        "name": "Auroria Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Auroria Stratis",
+            "symbol": "tSTRAX"
+        },
+        "networkId": 205205,
+        "rpc": [
+            "https://auroria.rpc.stratisevm.com"
+        ],
+        "shortName": "auroria"
+    },
+    {
+        "chainId": 210049,
+        "faucets": [],
+        "infoURL": "https://gitagi.org/",
+        "name": "GitAGI Atlas Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "GitAGI",
+            "symbol": "tGAGI"
+        },
+        "networkId": 210049,
+        "rpc": [
+            "https://rpc.gitagi.org"
+        ],
+        "shortName": "atlas"
+    },
+    {
         "chainId": 210425,
         "faucets": [],
         "infoURL": "https://www.platon.network",
         "name": "PlatON Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "LAT",
@@ -16282,14 +21695,65 @@
         "networkId": 221231,
         "rpc": [
             "https://test-eth.reapchain.org"
         ],
         "shortName": "reap-testnet"
     },
     {
+        "chainId": 222222,
+        "faucets": [],
+        "infoURL": "https://hydradx.io",
+        "name": "HydraDX",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Wrapped ETH",
+            "symbol": "WETH"
+        },
+        "networkId": 222222,
+        "rpc": [
+            "https://rpc.hydradx.cloud",
+            "wss://rpc.hydradx.cloud"
+        ],
+        "shortName": "hdx"
+    },
+    {
+        "chainId": 222555,
+        "faucets": [],
+        "infoURL": "https://deeplnetwork.org",
+        "name": "DeepL Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "DeepL",
+            "symbol": "DEEPL"
+        },
+        "networkId": 222555,
+        "rpc": [
+            "https://rpc.deeplnetwork.org"
+        ],
+        "shortName": "deepl"
+    },
+    {
+        "chainId": 222666,
+        "faucets": [
+            "https://faucet.deeplnetwork.org"
+        ],
+        "infoURL": "https://deeplnetwork.org",
+        "name": "DeepL Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "DeepL",
+            "symbol": "DEEPL"
+        },
+        "networkId": 222666,
+        "rpc": [
+            "https://testnet.deeplnetwork.org"
+        ],
+        "shortName": "tdeepl"
+    },
+    {
         "chainId": 224168,
         "faucets": [],
         "infoURL": "https://www.tafchain.com",
         "name": "Taf ECO Chain Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Taf ECO Chain Mainnet",
@@ -16298,20 +21762,52 @@
         "networkId": 224168,
         "rpc": [
             "https://mainnet.tafchain.com/v1"
         ],
         "shortName": "TAFECO"
     },
     {
+        "chainId": 224422,
+        "faucets": [],
+        "infoURL": "https://conet.network",
+        "name": "CONET Sebolia Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "CONET Sebolia",
+            "symbol": "CONET"
+        },
+        "networkId": 224422,
+        "rpc": [
+            "https://rpc1.conet.network"
+        ],
+        "shortName": "conet-sebolia"
+    },
+    {
+        "chainId": 224433,
+        "faucets": [],
+        "infoURL": "https://conet.network",
+        "name": "CONET Holesky",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "CONET Holesky",
+            "symbol": "CONET"
+        },
+        "networkId": 224433,
+        "rpc": [
+            "https://rpc.conet.network"
+        ],
+        "shortName": "conet-holesky"
+    },
+    {
         "chainId": 230315,
         "faucets": [
             "https://testnet.hashkeychain/faucet"
         ],
         "infoURL": "https://www.hashkey.com",
-        "name": "HashKey Chain Testnet",
+        "name": "HashKey Chain Testnet(discard)",
         "nativeCurrency": {
             "decimals": 18,
             "name": "HashKey Token",
             "symbol": "tHSK"
         },
         "networkId": 230315,
         "rpc": [
@@ -16447,14 +21943,46 @@
         "networkId": 281121,
         "rpc": [
             "https://socialsmartchain.digitalnext.business"
         ],
         "shortName": "SoChain"
     },
     {
+        "chainId": 282828,
+        "faucets": [],
+        "infoURL": "https://zillnet.io",
+        "name": "Zillion Sepolia Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Sepolia Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 282828,
+        "rpc": [
+            "https://sepolia.zillnet.io/rpc"
+        ],
+        "shortName": "zillsep"
+    },
+    {
+        "chainId": 313313,
+        "faucets": [],
+        "infoURL": "https://saharalabs.ai",
+        "name": "SaharaAI Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "SAHARA",
+            "symbol": "SAH"
+        },
+        "networkId": 313313,
+        "rpc": [
+            "https://testnet.saharalabs.ai"
+        ],
+        "shortName": "saharatest"
+    },
+    {
         "chainId": 314159,
         "faucets": [
             "https://faucet.calibration.fildev.network/"
         ],
         "infoURL": "https://filecoin.io",
         "name": "Filecoin - Calibration testnet",
         "nativeCurrency": {
@@ -16464,19 +21992,55 @@
         },
         "networkId": 314159,
         "rpc": [
             "https://api.calibration.node.glif.io/rpc/v1",
             "https://rpc.ankr.com/filecoin_testnet",
             "https://filecoin-calibration.chainstacklabs.com/rpc/v1",
             "https://filecoin-calibration.chainup.net/rpc/v1",
-            "https://calibration.filfox.info/rpc/v1"
+            "https://calibration.filfox.info/rpc/v1",
+            "https://filecoin-calibration.drpc.org",
+            "wss://filecoin-calibration.drpc.org"
         ],
         "shortName": "filecoin-calibration"
     },
     {
+        "chainId": 322202,
+        "faucets": [],
+        "infoURL": "https://parex.network",
+        "name": "Parex Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "PAREX",
+            "symbol": "PRX"
+        },
+        "networkId": 322202,
+        "rpc": [
+            "https://mainnet-rpc.parex.network"
+        ],
+        "shortName": "parex"
+    },
+    {
+        "chainId": 323213,
+        "faucets": [
+            "https://faucet.bloomgenesis.com"
+        ],
+        "infoURL": "https://www.bloomgenesis.com",
+        "name": "Bloom Genesis Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Bloom",
+            "symbol": "BGBC"
+        },
+        "networkId": 323213,
+        "rpc": [
+            "https://testnet-rpc.bloomgenesis.com"
+        ],
+        "shortName": "BGBC-Testnet"
+    },
+    {
         "chainId": 330844,
         "faucets": [
             "https://faucet.tscscan.com"
         ],
         "infoURL": "https://ttcoin.info/",
         "name": "TTcoin Smart Chain Mainnet",
         "nativeCurrency": {
@@ -16487,14 +22051,30 @@
         "networkId": 330844,
         "rpc": [
             "https://mainnet-rpc.tscscan.com"
         ],
         "shortName": "tc"
     },
     {
+        "chainId": 333313,
+        "faucets": [],
+        "infoURL": "https://www.bloomgenesis.com",
+        "name": "Bloom Genesis Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Bloom",
+            "symbol": "BGBC"
+        },
+        "networkId": 333313,
+        "rpc": [
+            "https://mainnet-rpc.bloomgenesis.com"
+        ],
+        "shortName": "BGBC"
+    },
+    {
         "chainId": 333331,
         "faucets": [],
         "infoURL": "https://ethereum.org",
         "name": "Aves Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "AvesT",
@@ -16592,14 +22172,48 @@
         "networkId": 333999,
         "rpc": [
             "https://rpc.polis.tech"
         ],
         "shortName": "olympus"
     },
     {
+        "chainId": 336655,
+        "faucets": [
+            "https://faucet-testnet.uniport.network"
+        ],
+        "infoURL": "https://uniport.network",
+        "name": "UPchain Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "UBTC",
+            "symbol": "UBTC"
+        },
+        "networkId": 336655,
+        "rpc": [
+            "https://rpc-testnet.uniport.network"
+        ],
+        "shortName": "UPchain-testnet"
+    },
+    {
+        "chainId": 336666,
+        "faucets": [],
+        "infoURL": "https://uniport.network",
+        "name": "UPchain Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "UBTC",
+            "symbol": "UBTC"
+        },
+        "networkId": 336666,
+        "rpc": [
+            "https://rpc.uniport.network"
+        ],
+        "shortName": "UPchain-mainnet"
+    },
+    {
         "chainId": 355113,
         "faucets": [
             "https://bitfinity.network/faucet"
         ],
         "infoURL": "https://bitfinity.network",
         "name": "Bitfinity Network Testnet",
         "nativeCurrency": {
@@ -16610,14 +22224,30 @@
         "networkId": 355113,
         "rpc": [
             "https://testnet.bitfinity.network"
         ],
         "shortName": "Bitfinity"
     },
     {
+        "chainId": 363636,
+        "faucets": [],
+        "infoURL": "",
+        "name": "Digit Soul Smart Chain 2",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Digit Coin",
+            "symbol": "DGC"
+        },
+        "networkId": 363636,
+        "rpc": [
+            "https://dgs-rpc.digitsoul.co.th"
+        ],
+        "shortName": "DS2"
+    },
+    {
         "chainId": 373737,
         "faucets": [],
         "infoURL": "https://hap.land",
         "name": "HAPchain Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "HAP",
@@ -16676,14 +22306,30 @@
         "networkId": 404040,
         "rpc": [
             "https://mainnet-rpc.tipboxcoin.net"
         ],
         "shortName": "TPBXm"
     },
     {
+        "chainId": 413413,
+        "faucets": [],
+        "infoURL": "https://testnet.aiescan.io",
+        "name": "AIE Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "AIE",
+            "symbol": "tAIE"
+        },
+        "networkId": 413413,
+        "rpc": [
+            "https://rpc1-testnet.aiechain.io"
+        ],
+        "shortName": "aiet"
+    },
+    {
         "chainId": 420420,
         "faucets": [],
         "infoURL": "https://kekchain.com",
         "name": "Kekchain",
         "nativeCurrency": {
             "decimals": 18,
             "name": "KEK",
@@ -16771,15 +22417,16 @@
         "nativeCurrency": {
             "decimals": 18,
             "name": "Sepolia Ether",
             "symbol": "ETH"
         },
         "networkId": 421614,
         "rpc": [
-            "https://sepolia-rollup.arbitrum.io/rpc"
+            "https://sepolia-rollup.arbitrum.io/rpc",
+            "https://arbitrum-sepolia.infura.io/v3/${INFURA_API_KEY}"
         ],
         "shortName": "arb-sep"
     },
     {
         "chainId": 424242,
         "faucets": [],
         "infoURL": "https://fastex.com",
@@ -16842,14 +22489,31 @@
         "networkId": 432204,
         "rpc": [
             "https://subnets.avax.network/dexalot/mainnet/rpc"
         ],
         "shortName": "dexalot"
     },
     {
+        "chainId": 444444,
+        "faucets": [],
+        "infoURL": "https://syndr.com",
+        "name": "Syndr L3 Sepolia",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Sepolia Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 444444,
+        "rpc": [
+            "https://sepolia.syndr.com/http",
+            "wss://sepolia.syndr.com/ws"
+        ],
+        "shortName": "syndr"
+    },
+    {
         "chainId": 444900,
         "faucets": [
             "https://faucet.weelink.gw002.oneitfarm.com"
         ],
         "infoURL": "https://weelink.cloud",
         "name": "Weelink Testnet",
         "nativeCurrency": {
@@ -16876,14 +22540,30 @@
         "networkId": 471100,
         "rpc": [
             "https://test-rpc.patex.io/"
         ],
         "shortName": "psep"
     },
     {
+        "chainId": 473861,
+        "faucets": [],
+        "infoURL": "https://ultrapro.info",
+        "name": "Ultra Pro Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ultra Pro",
+            "symbol": "UPRO"
+        },
+        "networkId": 473861,
+        "rpc": [
+            "https://mainnet-rpc.ultraproscan.io"
+        ],
+        "shortName": "ultrapro"
+    },
+    {
         "chainId": 474142,
         "faucets": [],
         "infoURL": "https://www.openchain.live",
         "name": "OpenChain Mainnet",
         "nativeCurrency": {
             "decimals": 10,
             "name": "OpenCoin",
@@ -16913,26 +22593,42 @@
             "wss://galaxy.block.caduceus.foundation"
         ],
         "shortName": "cmp"
     },
     {
         "chainId": 513100,
         "faucets": [],
-        "infoURL": "https://etherfair.org",
-        "name": "ethereum Fair",
+        "infoURL": "https://dischain.xyz",
+        "name": "DisChain",
         "nativeCurrency": {
             "decimals": 18,
-            "name": "EthereumFair",
-            "symbol": "ETHF"
+            "name": "DisChain",
+            "symbol": "DIS"
         },
         "networkId": 513100,
         "rpc": [
-            "https://rpc.etherfair.org"
+            "https://rpc.dischain.xyz"
         ],
-        "shortName": "ethf"
+        "shortName": "dis"
+    },
+    {
+        "chainId": 526916,
+        "faucets": [],
+        "infoURL": "https://docoin.network",
+        "name": "DoCoin Community Chain",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "DO",
+            "symbol": "DCT"
+        },
+        "networkId": 526916,
+        "rpc": [
+            "https://rpc.docoin.shop"
+        ],
+        "shortName": "DoCoin"
     },
     {
         "chainId": 534351,
         "faucets": [],
         "infoURL": "https://scroll.io",
         "name": "Scroll Sepolia Testnet",
         "nativeCurrency": {
@@ -16958,15 +22654,14 @@
             "decimals": 18,
             "name": "Ether",
             "symbol": "ETH"
         },
         "networkId": 534352,
         "rpc": [
             "https://rpc.scroll.io",
-            "https://rpc-scroll.icecreamswap.com",
             "https://rpc.ankr.com/scroll",
             "https://scroll-mainnet.chainstacklabs.com"
         ],
         "shortName": "scr"
     },
     {
         "chainId": 534353,
@@ -17029,30 +22724,48 @@
         "networkId": 535037,
         "rpc": [
             "https://mainnet-rpc.bescscan.io"
         ],
         "shortName": "BESC"
     },
     {
+        "chainId": 555666,
+        "faucets": [],
+        "infoURL": "http://eclipsenet.io",
+        "name": "Eclipse Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Eclipse",
+            "symbol": "ECLPS"
+        },
+        "networkId": 555666,
+        "rpc": [
+            "https://subnets.avax.network/eclipsecha/testnet/rpc"
+        ],
+        "shortName": "eclipset"
+    },
+    {
         "chainId": 622277,
         "faucets": [],
-        "infoURL": "https://www.rethereum.org",
-        "name": "Rethereum Mainnet",
+        "infoURL": "https://www.hypra.network",
+        "name": "Hypra Mainnet",
         "nativeCurrency": {
             "decimals": 18,
-            "name": "Rethereum",
-            "symbol": "RTH"
+            "name": "Hypra",
+            "symbol": "HYP"
         },
         "networkId": 622277,
         "rpc": [
+            "https://rpc.hypra.network",
             "https://rpc.rethereum.org",
             "https://rethereum.rpc.restratagem.com",
-            "https://rpc.rthcentral.org"
+            "https://rpc.rthcentral.org",
+            "https://hypra.rpc.thirdweb.com"
         ],
-        "shortName": "rth"
+        "shortName": "hyp"
     },
     {
         "chainId": 641230,
         "faucets": [],
         "infoURL": "https://bearnetwork.net",
         "name": "Bear Network Chain Mainnet",
         "nativeCurrency": {
@@ -17080,14 +22793,30 @@
         "networkId": 651940,
         "rpc": [
             "https://mainnet-rpc.alltra.global"
         ],
         "shortName": "ALL"
     },
     {
+        "chainId": 660279,
+        "faucets": [],
+        "infoURL": "https://xai.games",
+        "name": "Xai Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Xai",
+            "symbol": "XAI"
+        },
+        "networkId": 660279,
+        "rpc": [
+            "https://xai-chain.net/rpc"
+        ],
+        "shortName": "xai"
+    },
+    {
         "chainId": 666666,
         "faucets": [
             "https://vpioneerfaucet.visionscan.org"
         ],
         "infoURL": "https://visionscan.org",
         "name": "Vision - Vpioneer Test Chain",
         "nativeCurrency": {
@@ -17116,14 +22845,102 @@
         "networkId": 666888,
         "rpc": [
             "https://testnet-rpc.helachain.com"
         ],
         "shortName": "hela-testnet"
     },
     {
+        "chainId": 686868,
+        "faucets": [
+            "https://faucet.wondollars.org"
+        ],
+        "infoURL": "https://wonnetwork.org",
+        "name": "Won Network",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Won",
+            "symbol": "WON"
+        },
+        "networkId": 686868,
+        "rpc": [
+            "https://rpc.wonnetwork.org"
+        ],
+        "shortName": "WonChain"
+    },
+    {
+        "chainId": 696969,
+        "faucets": [
+            "https://docs.galadriel.com/faucet"
+        ],
+        "infoURL": "https://galadriel.com",
+        "name": "Galadriel Devnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Galadriel Devnet token",
+            "symbol": "GAL"
+        },
+        "networkId": 696969,
+        "rpc": [
+            "https://devnet.galadriel.com"
+        ],
+        "shortName": "galadriel-devnet"
+    },
+    {
+        "chainId": 710420,
+        "faucets": [],
+        "infoURL": "https://play.tiltyard.gg/",
+        "name": "Tiltyard Mainnet Subnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "TILT",
+            "symbol": "TILT"
+        },
+        "networkId": 710420,
+        "rpc": [
+            "https://subnets.avax.network/tiltyard/mainnet/rpc"
+        ],
+        "shortName": "tiltyardmainnet"
+    },
+    {
+        "chainId": 713715,
+        "faucets": [
+            "https://sei-faucet.nima.enterprises",
+            "https://sei-evm.faucetme.pro"
+        ],
+        "infoURL": "https://www.sei.io",
+        "name": "Sei Devnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Sei",
+            "symbol": "SEI"
+        },
+        "networkId": 713715,
+        "rpc": [
+            "https://evm-rpc-arctic-1.sei-apis.com",
+            "https://evm-rpc.arctic-1.seinetwork.io"
+        ],
+        "shortName": "sei-devnet"
+    },
+    {
+        "chainId": 743111,
+        "faucets": [],
+        "infoURL": "https://hemi.xyz",
+        "name": "Hemi Sepolia",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Sepolia Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 743111,
+        "rpc": [
+            "https://testnet.rpc.hemi.network/rpc"
+        ],
+        "shortName": "hemi-sep"
+    },
+    {
         "chainId": 751230,
         "faucets": [
             "https://faucet.bearnetwork.net"
         ],
         "infoURL": "https://bearnetwork.net",
         "name": "Bear Network Chain Testnet",
         "nativeCurrency": {
@@ -17183,14 +23000,81 @@
         "rpc": [
             "https://rpc.octa.space",
             "wss://rpc.octa.space"
         ],
         "shortName": "octa"
     },
     {
+        "chainId": 808080,
+        "faucets": [],
+        "infoURL": "https://www.biztoken.io/",
+        "name": "BIZ Smart Chain Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "tBIZT",
+            "symbol": "tBIZT"
+        },
+        "networkId": 808080,
+        "rpc": [
+            "https://rpc-testnet.bizex.io/"
+        ],
+        "shortName": "bizt-testnet"
+    },
+    {
+        "chainId": 810180,
+        "faucets": [],
+        "infoURL": "https://zklink.io",
+        "name": "zkLink Nova Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 810180,
+        "rpc": [
+            "https://rpc.zklink.io",
+            "wss://rpc.zklink.io"
+        ],
+        "shortName": "zklink-nova"
+    },
+    {
+        "chainId": 810181,
+        "faucets": [],
+        "infoURL": "https://zklink.io",
+        "name": "zkLink Nova Sepolia Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 810181,
+        "rpc": [
+            "https://sepolia.rpc.zklink.io",
+            "wss://sepolia.rpc.zklink.io"
+        ],
+        "shortName": "zklink-nova-sepolia"
+    },
+    {
+        "chainId": 810182,
+        "faucets": [],
+        "infoURL": "https://zklink.io",
+        "name": "zkLink Nova Goerli Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 810182,
+        "rpc": [
+            "https://goerli.rpc.zklink.io",
+            "wss://goerli.rpc.zklink.io"
+        ],
+        "shortName": "zklink-nova-goerli"
+    },
+    {
         "chainId": 827431,
         "faucets": [],
         "infoURL": "https://curvescan.io",
         "name": "CURVE Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Curve",
@@ -17232,14 +23116,46 @@
         "rpc": [
             "https://fraa-dancebox-3041-rpc.a.dancebox.tanssi.network",
             "wss://fraa-dancebox-3041-rpc.a.dancebox.tanssi.network"
         ],
         "shortName": "dodao"
     },
     {
+        "chainId": 879151,
+        "faucets": [],
+        "infoURL": "https://www.blocxchain.org/",
+        "name": "BlocX Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "BlocX",
+            "symbol": "BLX"
+        },
+        "networkId": 879151,
+        "rpc": [
+            "https://mainnet-rpc.blxscan.com/"
+        ],
+        "shortName": "blx"
+    },
+    {
+        "chainId": 888882,
+        "faucets": [],
+        "infoURL": "https://rexxnetwork.com",
+        "name": "REXX Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "REXX",
+            "symbol": "REXX"
+        },
+        "networkId": 888882,
+        "rpc": [
+            "https://rpc.rexxnetwork.com"
+        ],
+        "shortName": "REXX"
+    },
+    {
         "chainId": 888888,
         "faucets": [],
         "infoURL": "https://www.v.network",
         "name": "Vision - Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "VS",
@@ -17283,14 +23199,32 @@
         "networkId": 910000,
         "rpc": [
             "https://api.s0.t.posichain.org"
         ],
         "shortName": "psc-t-s0"
     },
     {
+        "chainId": 912559,
+        "faucets": [
+            "https://faucet.evm.dusk-3.devnet.astria.org/"
+        ],
+        "infoURL": "https://docs.astria.org",
+        "name": "Astria EVM Dusknet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "RIA",
+            "symbol": "RIA"
+        },
+        "networkId": 912559,
+        "rpc": [
+            "https://rpc.evm.dusk-3.devnet.astria.org"
+        ],
+        "shortName": "ria-dev"
+    },
+    {
         "chainId": 920000,
         "faucets": [
             "https://faucet.posichain.org/"
         ],
         "infoURL": "https://posichain.org",
         "name": "Posichain Devnet Shard 0",
         "nativeCurrency": {
@@ -17337,14 +23271,30 @@
         "networkId": 923018,
         "rpc": [
             "https://fncy-testnet-seed.fncy.world"
         ],
         "shortName": "tFNCY"
     },
     {
+        "chainId": 955081,
+        "faucets": [],
+        "infoURL": "",
+        "name": "Jono12 Subnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Jono12 Token",
+            "symbol": "JONO"
+        },
+        "networkId": 955081,
+        "rpc": [
+            "https://subnets.avax.network/jono12/testnet/rpc"
+        ],
+        "shortName": "jono12"
+    },
+    {
         "chainId": 955305,
         "faucets": [],
         "infoURL": "https://eluv.io",
         "name": "Eluvio Content Fabric",
         "nativeCurrency": {
             "decimals": 18,
             "name": "ELV",
@@ -17378,27 +23328,77 @@
         "networkId": 988207,
         "rpc": [
             "https://mainnet-rpc.ecroxscan.com/"
         ],
         "shortName": "ecrox"
     },
     {
+        "chainId": 999999,
+        "faucets": [],
+        "infoURL": "https://hewe.io/",
+        "name": "AmChain",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "AMC",
+            "symbol": "AMC"
+        },
+        "networkId": 999999,
+        "rpc": [
+            "https://node1.amchain.net"
+        ],
+        "shortName": "AMC"
+    },
+    {
+        "chainId": 1100789,
+        "faucets": [],
+        "infoURL": "https://netmind.ai",
+        "name": "Netmind Chain Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "NMT",
+            "symbol": "NMT"
+        },
+        "networkId": 1100789,
+        "rpc": [
+            "https://testblock.protago-dev.com"
+        ],
+        "shortName": "nmtTest"
+    },
+    {
+        "chainId": 1127469,
+        "faucets": [],
+        "infoURL": "",
+        "name": "Tiltyard Subnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Tiltyard Token",
+            "symbol": "TILTG"
+        },
+        "networkId": 1127469,
+        "rpc": [
+            "https://subnets.avax.network/tiltyard/testnet/rpc"
+        ],
+        "shortName": "tiltyard"
+    },
+    {
         "chainId": 1261120,
         "faucets": [],
         "infoURL": "https://astar.network",
         "name": "zKatana",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Sepolia Ether",
             "symbol": "ETH"
         },
         "networkId": 1261120,
         "rpc": [
             "https://rpc.zkatana.gelato.digital",
-            "https://rpc.startale.com/zkatana"
+            "https://rpc.startale.com/zkatana",
+            "https://astar-zkatana.drpc.org",
+            "wss://astar-zkatana.drpc.org"
         ],
         "shortName": "azktn"
     },
     {
         "chainId": 1313114,
         "faucets": [],
         "infoURL": "https://ethoprotocol.com",
@@ -17485,14 +23485,46 @@
         "networkId": 1337803,
         "rpc": [
             "https://rpc.zhejiang.ethpandaops.io"
         ],
         "shortName": "zhejiang"
     },
     {
+        "chainId": 1612127,
+        "faucets": [],
+        "infoURL": "https://www.playfi.ai/",
+        "name": "PlayFi Albireo Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 1612127,
+        "rpc": [
+            "https://albireo-rpc.playfi.ai"
+        ],
+        "shortName": "alberio"
+    },
+    {
+        "chainId": 1731313,
+        "faucets": [],
+        "infoURL": "",
+        "name": "Turkey Demo Dev",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 1731313,
+        "rpc": [
+            "https://devchain-poa.huabeizhenxuan.com"
+        ],
+        "shortName": "TDD"
+    },
+    {
         "chainId": 2021398,
         "faucets": [],
         "infoURL": "https://debank.com",
         "name": "DeBank Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "DeBank USD",
@@ -17561,24 +23593,40 @@
     {
         "chainId": 2611555,
         "faucets": [],
         "infoURL": "",
         "name": "DPU Chain",
         "nativeCurrency": {
             "decimals": 18,
-            "name": "DGS",
-            "symbol": "DGS"
+            "name": "DGC",
+            "symbol": "DGC"
         },
         "networkId": 2611555,
         "rpc": [
             "https://sc-rpc.dpu.ac.th"
         ],
         "shortName": "DPU"
     },
     {
+        "chainId": 3132023,
+        "faucets": [],
+        "infoURL": "https://saharalabs.ai",
+        "name": "SaharaAI Network",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "SAHARA",
+            "symbol": "SAH"
+        },
+        "networkId": 3132023,
+        "rpc": [
+            "https://mainnet.saharalabs.ai"
+        ],
+        "shortName": "sahara"
+    },
+    {
         "chainId": 3141592,
         "faucets": [
             "https://faucet.butterfly.fildev.network"
         ],
         "infoURL": "https://filecoin.io",
         "name": "Filecoin - Butterfly testnet",
         "nativeCurrency": {
@@ -17598,19 +23646,37 @@
         "nativeCurrency": {
             "decimals": 18,
             "name": "Manta",
             "symbol": "MANTA"
         },
         "networkId": 3441005,
         "rpc": [
-            "https://manta-testnet.calderachain.xyz/http"
+            "https://manta-testnet.calderachain.xyz/http",
+            "https://manta-pacific-testnet.drpc.org",
+            "wss://manta-pacific-testnet.drpc.org"
         ],
         "shortName": "mantaTestnet"
     },
     {
+        "chainId": 3441006,
+        "faucets": [],
+        "infoURL": "https://manta-testnet.caldera.dev/",
+        "name": "Manta Pacific Sepolia Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 3441006,
+        "rpc": [
+            "https://pacific-rpc.sepolia-testnet.manta.network/http"
+        ],
+        "shortName": "mantaSepoliaTestnet"
+    },
+    {
         "chainId": 4000003,
         "faucets": [],
         "infoURL": "https://altlayer.io",
         "name": "AltLayer Zero Gas Network",
         "nativeCurrency": {
             "decimals": 18,
             "name": "ZERO",
@@ -17648,33 +23714,68 @@
             "name": "MXC Wannsee zkEVM Testnet",
             "symbol": "MXC"
         },
         "networkId": 5167003,
         "rpc": [
             "https://wannsee-rpc.mxc.com"
         ],
+        "shortName": "MXCdiscontinued"
+    },
+    {
+        "chainId": 5167004,
+        "faucets": [],
+        "infoURL": "https://doc.mxc.com/docs/intro",
+        "name": "Moonchain Geneva Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Moonchain Geneva Testnet",
+            "symbol": "MXC"
+        },
+        "networkId": 5167004,
+        "rpc": [
+            "https://geneva-rpc.moonchain.com"
+        ],
         "shortName": "MXC"
     },
     {
         "chainId": 5201420,
         "faucets": [],
         "infoURL": "https://electroneum.com",
         "name": "Electroneum Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Electroneum",
             "symbol": "ETN"
         },
         "networkId": 5201420,
         "rpc": [
-            "https://api.electroneum.com"
+            "https://testnet-rpc.electroneum.com"
         ],
         "shortName": "etn-testnet"
     },
     {
+        "chainId": 5318008,
+        "faucets": [
+            "https://dev.reactive.network/docs/kopli-testnet#faucet"
+        ],
+        "infoURL": "https://reactive.network",
+        "name": "Reactive Kopli",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Kopli React",
+            "symbol": "REACT"
+        },
+        "networkId": 5318008,
+        "rpc": [
+            "https://kopli-rpc.reactive.network",
+            "http://kopli-rpc.rkt.ink"
+        ],
+        "shortName": "kreact"
+    },
+    {
         "chainId": 5555555,
         "faucets": [],
         "infoURL": "https://imversed.com",
         "name": "Imversed Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Imversed Token",
@@ -17701,14 +23802,63 @@
         "rpc": [
             "https://jsonrpc-test.imversed.network",
             "https://ws-jsonrpc-test.imversed.network"
         ],
         "shortName": "imversed-testnet"
     },
     {
+        "chainId": 6038361,
+        "faucets": [],
+        "infoURL": "https://astar.network",
+        "name": "Astar zKyoto",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Sepolia Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 6038361,
+        "rpc": [
+            "https://rpc.startale.com/zkyoto",
+            "https://rpc.zkyoto.gelato.digital"
+        ],
+        "shortName": "azkyt"
+    },
+    {
+        "chainId": 6666665,
+        "faucets": [],
+        "infoURL": "https://www.anwang.com",
+        "name": "Safe(AnWang) Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "SAFE(AnWang)",
+            "symbol": "SAFE"
+        },
+        "networkId": 6666665,
+        "rpc": [
+            "https://rpc.anwang.com"
+        ],
+        "shortName": "SafeMainnet"
+    },
+    {
+        "chainId": 6666666,
+        "faucets": [],
+        "infoURL": "https://www.anwang.com",
+        "name": "Safe(AnWang) Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "SAFE(AnWang)",
+            "symbol": "SAFE"
+        },
+        "networkId": 6666666,
+        "rpc": [
+            "https://rpc-testnet.anwang.com"
+        ],
+        "shortName": "SafeTestnet"
+    },
+    {
         "chainId": 7225878,
         "faucets": [],
         "infoURL": "https://saakuru.network",
         "name": "Saakuru Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "OAS",
@@ -17799,14 +23949,30 @@
         "networkId": 8007736,
         "rpc": [
             "https://mainnet.plian.io/child_0"
         ],
         "shortName": "plian-mainnet-l2"
     },
     {
+        "chainId": 8080808,
+        "faucets": [],
+        "infoURL": "https://hokum.gg",
+        "name": "Hokum",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 8080808,
+        "rpc": [
+            "https://mainnet.hokum.gg"
+        ],
+        "shortName": "hokum"
+    },
+    {
         "chainId": 8794598,
         "faucets": [],
         "infoURL": "https://hap.land",
         "name": "HAPchain",
         "nativeCurrency": {
             "decimals": 18,
             "name": "HAP",
@@ -17843,14 +24009,46 @@
             "symbol": "QARE"
         },
         "networkId": 8888888,
         "rpc": [],
         "shortName": "quarix"
     },
     {
+        "chainId": 9322252,
+        "faucets": [],
+        "infoURL": "https://xcap.network/",
+        "name": "XCAP",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Gas",
+            "symbol": "GAS"
+        },
+        "networkId": 9322252,
+        "rpc": [
+            "https://xcap-mainnet.relay.xcap.network/znzvh2ueyvm2yts5fv5gnul395jbkfb2/rpc1"
+        ],
+        "shortName": "xcap"
+    },
+    {
+        "chainId": 9322253,
+        "faucets": [],
+        "infoURL": "https://xcap.network/",
+        "name": "Milvine",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Gas",
+            "symbol": "GAS"
+        },
+        "networkId": 9322253,
+        "rpc": [
+            "https://xcap-milvine.relay.xcap.network/zj5l55ftsgi027kz4nf14vs8d89inego/rpc1"
+        ],
+        "shortName": "milv"
+    },
+    {
         "chainId": 10067275,
         "faucets": [],
         "infoURL": "https://plian.org/",
         "name": "Plian Testnet Subchain 1",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Plian Token",
@@ -17898,20 +24096,42 @@
             "https://rpc2.sepolia.org",
             "https://rpc-sepolia.rockx.com",
             "https://rpc.sepolia.ethpandaops.io",
             "https://sepolia.infura.io/v3/${INFURA_API_KEY}",
             "wss://sepolia.infura.io/v3/${INFURA_API_KEY}",
             "https://sepolia.gateway.tenderly.co",
             "wss://sepolia.gateway.tenderly.co",
-            "https://ethereum-sepolia.publicnode.com",
-            "wss://ethereum-sepolia.publicnode.com"
+            "https://ethereum-sepolia-rpc.publicnode.com",
+            "wss://ethereum-sepolia-rpc.publicnode.com",
+            "https://sepolia.drpc.org",
+            "wss://sepolia.drpc.org"
         ],
         "shortName": "sep"
     },
     {
+        "chainId": 11155420,
+        "faucets": [
+            "https://app.optimism.io/faucet"
+        ],
+        "infoURL": "https://optimism.io",
+        "name": "OP Sepolia Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Sepolia Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 11155420,
+        "rpc": [
+            "https://sepolia.optimism.io",
+            "https://optimism-sepolia.drpc.org",
+            "wss://optimism-sepolia.drpc.org"
+        ],
+        "shortName": "opsep"
+    },
+    {
         "chainId": 13371337,
         "faucets": [],
         "infoURL": "https://pepchain.io",
         "name": "PepChain Churchill",
         "nativeCurrency": {
             "decimals": 18,
             "name": "PepChain Churchill Ether",
@@ -17953,14 +24173,30 @@
         "networkId": 16658437,
         "rpc": [
             "https://testnet.plian.io/testnet"
         ],
         "shortName": "plian-testnet"
     },
     {
+        "chainId": 17000920,
+        "faucets": [],
+        "infoURL": "https://lambda.im",
+        "name": "Lambda Chain Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "ETH",
+            "symbol": "ETH"
+        },
+        "networkId": 17000920,
+        "rpc": [
+            "https://testnrpc.lambda.im/"
+        ],
+        "shortName": "tlambda"
+    },
+    {
         "chainId": 18289463,
         "faucets": [],
         "infoURL": "https://iolite.io",
         "name": "IOLite",
         "nativeCurrency": {
             "decimals": 18,
             "name": "IOLite Ether",
@@ -17969,14 +24205,30 @@
         "networkId": 18289463,
         "rpc": [
             "https://net.iolite.io"
         ],
         "shortName": "ilt"
     },
     {
+        "chainId": 20180427,
+        "faucets": [],
+        "infoURL": "https://stabilityprotocol.com",
+        "name": "Stability Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "FREE",
+            "symbol": "FREE"
+        },
+        "networkId": 20180427,
+        "rpc": [
+            "https://free.testnet.stabilityprotocol.com"
+        ],
+        "shortName": "stabilitytestnet"
+    },
+    {
         "chainId": 20180430,
         "faucets": [],
         "infoURL": "https://smartmesh.io",
         "name": "SmartMesh Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "SmartMesh Native Token",
@@ -18024,14 +24276,46 @@
             "https://node1.pegorpc.com",
             "https://node2.pegorpc.com",
             "https://node3.pegorpc.com"
         ],
         "shortName": "pg"
     },
     {
+        "chainId": 20240324,
+        "faucets": [],
+        "infoURL": "https://debank.com",
+        "name": "DeBank Sepolia Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "DeBank USD",
+            "symbol": "USD"
+        },
+        "networkId": 20240324,
+        "rpc": [
+            "https://sepolia-rpc.testnet.debank.com"
+        ],
+        "shortName": "dbkse"
+    },
+    {
+        "chainId": 20482050,
+        "faucets": [],
+        "infoURL": "https://hokum.gg",
+        "name": "Hokum Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 20482050,
+        "rpc": [
+            "https://testnet.hokum.gg"
+        ],
+        "shortName": "hokum-testnet"
+    },
+    {
         "chainId": 22052002,
         "faucets": [],
         "infoURL": "https://xlon.org",
         "name": "Excelon Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Excelon",
@@ -18074,14 +24358,30 @@
         "networkId": 27082022,
         "rpc": [
             "https://rpc.exlscan.com"
         ],
         "shortName": "exl"
     },
     {
+        "chainId": 28122024,
+        "faucets": [],
+        "infoURL": "https://ancient8.gg/",
+        "name": "Ancient8 Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 28122024,
+        "rpc": [
+            "https://rpcv2-testnet.ancient8.gg"
+        ],
+        "shortName": "a8"
+    },
+    {
         "chainId": 28945486,
         "faucets": [],
         "infoURL": "https://auxilium.global",
         "name": "Auxilium Network Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Auxilium coin",
@@ -18136,14 +24436,49 @@
         "networkId": 35855456,
         "rpc": [
             "https://node.joys.digital"
         ],
         "shortName": "JOYS"
     },
     {
+        "chainId": 37084624,
+        "faucets": [
+            "https://www.sfuelstation.com/"
+        ],
+        "infoURL": "https://nebulachain.io/",
+        "name": "SKALE Nebula Hub Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "sFUEL",
+            "symbol": "sFUEL"
+        },
+        "networkId": 37084624,
+        "rpc": [
+            "https://testnet.skalenodes.com/v1/lanky-ill-funny-testnet",
+            "wss://testnet.skalenodes.com/v1/ws/lanky-ill-funny-testnet"
+        ],
+        "shortName": "nebula-testnet"
+    },
+    {
+        "chainId": 39916801,
+        "faucets": [],
+        "infoURL": "https://www.beastkingdom.io/",
+        "name": "Kingdom Chain",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Kozi",
+            "symbol": "KOZI"
+        },
+        "networkId": 39916801,
+        "rpc": [
+            "https://kingdomchain.observer/rpc"
+        ],
+        "shortName": "kchain"
+    },
+    {
         "chainId": 43214913,
         "faucets": [],
         "infoURL": "",
         "name": "maistestsubnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "maistestsubnet",
@@ -18183,38 +24518,98 @@
         "name": "Autonity Bakerloo (Thames) Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Bakerloo Auton",
             "symbol": "ATN"
         },
         "networkId": 65010000,
+        "rpc": [],
+        "shortName": "bakerloo-0"
+    },
+    {
+        "chainId": 65010001,
+        "faucets": [
+            "https://faucet.autonity.org/"
+        ],
+        "infoURL": "https://autonity.org/",
+        "name": "Autonity Bakerloo (Barada) Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Bakerloo Auton",
+            "symbol": "ATN"
+        },
+        "networkId": 65010001,
+        "rpc": [],
+        "shortName": "bakerloo-01"
+    },
+    {
+        "chainId": 65010002,
+        "faucets": [
+            "https://faucet.autonity.org/"
+        ],
+        "infoURL": "https://autonity.org/",
+        "name": "Autonity Bakerloo (Sumida) Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Bakerloo Auton",
+            "symbol": "ATN"
+        },
+        "networkId": 65010002,
         "rpc": [
             "https://rpc1.bakerloo.autonity.org/",
             "wss://rpc1.bakerloo.autonity.org/ws/"
         ],
-        "shortName": "bakerloo-0"
+        "shortName": "bakerloo-02"
     },
     {
         "chainId": 65100000,
         "faucets": [
             "https://faucet.autonity.org/"
         ],
         "infoURL": "https://autonity.org/",
         "name": "Autonity Piccadilly (Thames) Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Piccadilly Auton",
             "symbol": "ATN"
         },
         "networkId": 65100000,
+        "rpc": [],
+        "shortName": "piccadilly-0"
+    },
+    {
+        "chainId": 65100001,
+        "faucets": [],
+        "infoURL": "https://autonity.org/",
+        "name": "Autonity Piccadilly (Barada) Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Piccadilly Auton",
+            "symbol": "ATN"
+        },
+        "networkId": 65100001,
+        "rpc": [],
+        "shortName": "piccadilly-01"
+    },
+    {
+        "chainId": 65100002,
+        "faucets": [],
+        "infoURL": "https://autonity.org/",
+        "name": "Autonity Piccadilly (Sumida) Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Piccadilly Auton",
+            "symbol": "ATN"
+        },
+        "networkId": 65100002,
         "rpc": [
             "https://rpc1.piccadilly.autonity.org/",
             "wss://rpc1.piccadilly.autonity.org/ws/"
         ],
-        "shortName": "piccadilly-0"
+        "shortName": "piccadilly-02"
     },
     {
         "chainId": 68840142,
         "faucets": [
             "https://faucet.triangleplatform.com/frame/testnet"
         ],
         "infoURL": "https://www.frame.xyz/",
@@ -18227,14 +24622,30 @@
         "networkId": 68840142,
         "rpc": [
             "https://rpc.testnet.frame.xyz/http"
         ],
         "shortName": "frametest"
     },
     {
+        "chainId": 77787778,
+        "faucets": [],
+        "infoURL": "https://0xhash.io",
+        "name": "0xHash Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "0xHash",
+            "symbol": "HETH"
+        },
+        "networkId": 77787778,
+        "rpc": [
+            "https://rpc-test.0xhash.io"
+        ],
+        "shortName": "HETH"
+    },
+    {
         "chainId": 88888888,
         "faucets": [],
         "infoURL": "https://teamblockchain.team",
         "name": "T.E.A.M Blockchain",
         "nativeCurrency": {
             "decimals": 18,
             "name": "TEAM",
@@ -18243,14 +24654,31 @@
         "networkId": 88888888,
         "rpc": [
             "https://rpc.teamblockchain.team"
         ],
         "shortName": "team"
     },
     {
+        "chainId": 94204209,
+        "faucets": [],
+        "infoURL": "https://raas.gelato.network/rollups/details/public/polygon-blackberry",
+        "name": "Polygon Blackberry",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Sepolia Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 94204209,
+        "rpc": [
+            "https://rpc.polygon-blackberry.gelato.digital",
+            "wss://ws.polygon-blackberry.gelato.digital"
+        ],
+        "shortName": "polygon-blackberry"
+    },
+    {
         "chainId": 99415706,
         "faucets": [
             "https://faucet.joys.digital/"
         ],
         "infoURL": "https://joys.digital",
         "name": "Joys Digital TestNet",
         "nativeCurrency": {
@@ -18261,14 +24689,87 @@
         "networkId": 99415706,
         "rpc": [
             "https://toys.joys.cash/"
         ],
         "shortName": "TOYS"
     },
     {
+        "chainId": 111557560,
+        "faucets": [],
+        "infoURL": "https://cyber.co/",
+        "name": "Cyber Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Sepolia Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 111557560,
+        "rpc": [
+            "https://cyber-testnet.alt.technology/",
+            "wss://cyber-testnet.alt.technology/ws",
+            "https://rpc.testnet.cyber.co/",
+            "wss://rpc.testnet.cyber.co/"
+        ],
+        "shortName": "cysep"
+    },
+    {
+        "chainId": 123420111,
+        "faucets": [],
+        "infoURL": "https://raas.gelato.network/rollups/details/public/opcelestia-raspberry",
+        "name": "OP Celestia Raspberry",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Sepolia Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 123420111,
+        "rpc": [
+            "https://rpc.opcelestia-raspberry.gelato.digital",
+            "wss://ws.opcelestia-raspberry.gelato.digital"
+        ],
+        "shortName": "opcelestia-raspberry"
+    },
+    {
+        "chainId": 161221135,
+        "faucets": [],
+        "infoURL": "https://www.plumenetwork.xyz/",
+        "name": "Plume Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Plume Sepolia Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 161221135,
+        "rpc": [
+            "https://testnet-rpc.plumenetwork.xyz/http",
+            "wss://testnet-rpc.plumenetwork.xyz/ws"
+        ],
+        "shortName": "plume-testnet"
+    },
+    {
+        "chainId": 168587773,
+        "faucets": [
+            "https://faucet.quicknode.com/blast/sepolia"
+        ],
+        "infoURL": "https://blast.io/",
+        "name": "Blast Sepolia Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Sepolia Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 168587773,
+        "rpc": [
+            "https://sepolia.blast.io",
+            "https://blast-sepolia.drpc.org",
+            "wss://blast-sepolia.drpc.org"
+        ],
+        "shortName": "blastsepolia"
+    },
+    {
         "chainId": 192837465,
         "faucets": [],
         "infoURL": "https://gather.network",
         "name": "Gather Mainnet Network",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Gather",
@@ -18288,48 +24789,54 @@
         "nativeCurrency": {
             "decimals": 18,
             "name": "gMeld",
             "symbol": "gMELD"
         },
         "networkId": 222000222,
         "rpc": [
-            "https://subnets.avax.network/meld/testnet/rpc"
+            "https://testnet-rpc.meld.com"
         ],
         "shortName": "kanazawa"
     },
     {
         "chainId": 245022926,
         "faucets": [
             "https://neonfaucet.org"
         ],
         "infoURL": "https://neon-labs.org",
-        "name": "Neon EVM DevNet",
+        "name": "Neon EVM Devnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Neon",
             "symbol": "NEON"
         },
         "networkId": 245022926,
         "rpc": [
-            "https://devnet.neonevm.org"
+            "https://devnet.neonevm.org",
+            "https://neon-evm-devnet.drpc.org",
+            "wss://neon-evm-devnet.drpc.org"
         ],
         "shortName": "neonevm-devnet"
     },
     {
         "chainId": 245022934,
         "faucets": [],
         "infoURL": "https://neonevm.org",
-        "name": "Neon EVM MainNet",
+        "name": "Neon EVM Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Neon",
             "symbol": "NEON"
         },
         "networkId": 245022934,
-        "rpc": [],
+        "rpc": [
+            "https://neon-proxy-mainnet.solana.p2p.org",
+            "https://neon-evm.drpc.org",
+            "wss://neon-evm.drpc.org"
+        ],
         "shortName": "neonevm-mainnet"
     },
     {
         "chainId": 245022940,
         "faucets": [],
         "infoURL": "https://neon-labs.org",
         "name": "Neon EVM TestNet",
@@ -18386,35 +24893,35 @@
         "nativeCurrency": {
             "decimals": 18,
             "name": "gMeld",
             "symbol": "gMELD"
         },
         "networkId": 333000333,
         "rpc": [
-            "https://subnets.avax.network/meld/mainnet/rpc"
+            "https://rpc-1.meld.com"
         ],
         "shortName": "meld"
     },
     {
         "chainId": 344106930,
         "faucets": [
             "https://sfuel.dirtroad.dev/staging"
         ],
         "infoURL": "https://calypsohub.network/",
-        "name": "Calypso NFT Hub (SKALE Testnet)",
+        "name": "Deprecated SKALE Calypso Hub Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "sFUEL",
             "symbol": "sFUEL"
         },
         "networkId": 344106930,
         "rpc": [
             "https://staging-v3.skalenodes.com/v1/staging-utter-unripe-menkar"
         ],
-        "shortName": "calypso-testnet"
+        "shortName": "deprected-calypso-testnet"
     },
     {
         "chainId": 356256156,
         "faucets": [],
         "infoURL": "https://gather.network",
         "name": "Gather Testnet Network",
         "nativeCurrency": {
@@ -18425,14 +24932,32 @@
         "networkId": 356256156,
         "rpc": [
             "https://testnet.gather.network"
         ],
         "shortName": "tGTH"
     },
     {
+        "chainId": 476158412,
+        "faucets": [
+            "https://sfuel.dirtroad.dev/staging"
+        ],
+        "infoURL": "https://europahub.network/",
+        "name": "Deprecated SKALE Europa Hub Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "sFUEL",
+            "symbol": "sFUEL"
+        },
+        "networkId": 476158412,
+        "rpc": [
+            "https://staging-v3.skalenodes.com/v1/staging-legal-crazy-castor"
+        ],
+        "shortName": "deprecated-europa-testnet"
+    },
+    {
         "chainId": 486217935,
         "faucets": [],
         "infoURL": "https://gather.network",
         "name": "Gather Devnet Network",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Gather",
@@ -18442,28 +24967,114 @@
         "rpc": [
             "https://devnet.gather.network"
         ],
         "shortName": "dGTH"
     },
     {
         "chainId": 503129905,
-        "faucets": [],
+        "faucets": [
+            "https://sfuel.dirtroad.dev/staging"
+        ],
         "infoURL": "https://nebulachain.io/",
-        "name": "Nebula Staging",
+        "name": "Deprecated SKALE Nebula Hub Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "sFUEL",
             "symbol": "sFUEL"
         },
         "networkId": 503129905,
         "rpc": [
             "https://staging-v3.skalenodes.com/v1/staging-faint-slimy-achird",
             "wss://staging-v3.skalenodes.com/v1/ws/staging-faint-slimy-achird"
         ],
-        "shortName": "nebula-staging"
+        "shortName": "deprecated-nebula-testnet"
+    },
+    {
+        "chainId": 666666666,
+        "faucets": [],
+        "infoURL": "https://degen.tips",
+        "name": "Degen Chain",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "DEGEN",
+            "symbol": "DEGEN"
+        },
+        "networkId": 666666666,
+        "rpc": [
+            "https://rpc.degen.tips"
+        ],
+        "shortName": "degen-chain"
+    },
+    {
+        "chainId": 888888888,
+        "faucets": [],
+        "infoURL": "https://ancient8.gg/",
+        "name": "Ancient8",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 888888888,
+        "rpc": [
+            "https://rpc.ancient8.gg"
+        ],
+        "shortName": "ancient8"
+    },
+    {
+        "chainId": 889910245,
+        "faucets": [
+            "https://faucet.ptcscan.io/"
+        ],
+        "infoURL": "https://ptcscan.io",
+        "name": "PTCESCAN Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "PTCE",
+            "symbol": "PTCE"
+        },
+        "networkId": 889910245,
+        "rpc": [
+            "https://rpc-testnet.ptcscan.io"
+        ],
+        "shortName": "PTCE"
+    },
+    {
+        "chainId": 889910246,
+        "faucets": [],
+        "infoURL": "https://ptcscan.io",
+        "name": "PTCESCAN Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "PTCE",
+            "symbol": "PTCE"
+        },
+        "networkId": 889910246,
+        "rpc": [
+            "https://rpc.ptcscan.io"
+        ],
+        "shortName": "POLYTECH"
+    },
+    {
+        "chainId": 974399131,
+        "faucets": [
+            "https://www.sfuelstation.com/"
+        ],
+        "infoURL": "https://calypsohub.network/",
+        "name": "SKALE Calypso Hub Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "sFUEL",
+            "symbol": "sFUEL"
+        },
+        "networkId": 974399131,
+        "rpc": [
+            "https://testnet.skalenodes.com/v1/giant-half-dual-testnet"
+        ],
+        "shortName": "calypso-testnet"
     },
     {
         "chainId": 999999999,
         "faucets": [],
         "infoURL": "https://zora.energy",
         "name": "Zora Sepolia Testnet",
         "nativeCurrency": {
@@ -18474,14 +25085,33 @@
         "networkId": 999999999,
         "rpc": [
             "https://sepolia.rpc.zora.energy"
         ],
         "shortName": "zsep"
     },
     {
+        "chainId": 1020352220,
+        "faucets": [
+            "https://www.sfuelstation.com/"
+        ],
+        "infoURL": "",
+        "name": "SKALE Titan Hub Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "sFUEL",
+            "symbol": "sFUEL"
+        },
+        "networkId": 1020352220,
+        "rpc": [
+            "https://testnet.skalenodes.com/v1/aware-fake-trim-testnet",
+            "wss://testnet.skalenodes.com/v1/ws/aware-fake-trim-testnet"
+        ],
+        "shortName": "titan-testnet"
+    },
+    {
         "chainId": 1122334455,
         "faucets": [],
         "infoURL": "https://iposlab.com",
         "name": "IPOS Network",
         "nativeCurrency": {
             "decimals": 18,
             "name": "IPOS Network Ether",
@@ -18536,15 +25166,17 @@
         "nativeCurrency": {
             "decimals": 18,
             "name": "Ether",
             "symbol": "ETH"
         },
         "networkId": 1313161554,
         "rpc": [
-            "https://mainnet.aurora.dev"
+            "https://mainnet.aurora.dev",
+            "https://aurora.drpc.org",
+            "wss://aurora.drpc.org"
         ],
         "shortName": "aurora"
     },
     {
         "chainId": 1313161555,
         "faucets": [],
         "infoURL": "https://aurora.dev",
@@ -18552,15 +25184,17 @@
         "nativeCurrency": {
             "decimals": 18,
             "name": "Ether",
             "symbol": "ETH"
         },
         "networkId": 1313161555,
         "rpc": [
-            "https://testnet.aurora.dev/"
+            "https://testnet.aurora.dev/",
+            "https://aurora-testnet.drpc.org",
+            "wss://aurora-testnet.drpc.org"
         ],
         "shortName": "aurora-testnet"
     },
     {
         "chainId": 1313161556,
         "faucets": [],
         "infoURL": "https://aurora.dev",
@@ -18571,14 +25205,49 @@
             "symbol": "ETH"
         },
         "networkId": 1313161556,
         "rpc": [],
         "shortName": "aurora-betanet"
     },
     {
+        "chainId": 1313161560,
+        "faucets": [],
+        "infoURL": "https://www.powergold.tech",
+        "name": "PowerGold",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 1313161560,
+        "rpc": [
+            "https://powergold.aurora.dev"
+        ],
+        "shortName": "powergold"
+    },
+    {
+        "chainId": 1350216234,
+        "faucets": [
+            "https://sfuel.skale.network/"
+        ],
+        "infoURL": "",
+        "name": "SKALE Titan Hub",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "sFUEL",
+            "symbol": "sFUEL"
+        },
+        "networkId": 1350216234,
+        "rpc": [
+            "https://mainnet.skalenodes.com/v1/parallel-stormy-spica",
+            "wss://mainnet.skalenodes.com/v1/ws/parallel-stormy-spica"
+        ],
+        "shortName": "titan-mainnet"
+    },
+    {
         "chainId": 1351057110,
         "faucets": [
             "https://sfuel.skale.network/staging/chaos"
         ],
         "infoURL": "https://docs.skale.network/develop/",
         "name": "Chaos (SKALE Testnet)",
         "nativeCurrency": {
@@ -18589,14 +25258,30 @@
         "networkId": 1351057110,
         "rpc": [
             "https://staging-v3.skalenodes.com/v1/staging-fast-active-bellatrix"
         ],
         "shortName": "chaos-tenet"
     },
     {
+        "chainId": 1380012617,
+        "faucets": [],
+        "infoURL": "https://rarichain.org/",
+        "name": "RARI Chain Mainnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ethereum",
+            "symbol": "ETH"
+        },
+        "networkId": 1380012617,
+        "rpc": [
+            "https://rari.calderachain.xyz/http"
+        ],
+        "shortName": "rari-mainnet"
+    },
+    {
         "chainId": 1380996178,
         "faucets": [],
         "infoURL": "https://raptorchain.io",
         "name": "RaptorChain",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Raptor",
@@ -18605,37 +25290,76 @@
         "networkId": 1380996178,
         "rpc": [
             "https://rpc.raptorchain.io/web3"
         ],
         "shortName": "rptr"
     },
     {
+        "chainId": 1444673419,
+        "faucets": [
+            "https://www.sfuelstation.com/"
+        ],
+        "infoURL": "https://europahub.network/",
+        "name": "SKALE Europa Hub Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "sFUEL",
+            "symbol": "sFUEL"
+        },
+        "networkId": 1444673419,
+        "rpc": [
+            "https://testnet.skalenodes.com/v1/juicy-low-small-testnet"
+        ],
+        "shortName": "europa-testnet"
+    },
+    {
         "chainId": 1482601649,
-        "faucets": [],
+        "faucets": [
+            "https://sfuel.skale.network/"
+        ],
         "infoURL": "https://nebulachain.io/",
-        "name": "Nebula Mainnet",
+        "name": "SKALE Nebula Hub",
         "nativeCurrency": {
             "decimals": 18,
             "name": "sFUEL",
             "symbol": "sFUEL"
         },
         "networkId": 1482601649,
         "rpc": [
             "https://mainnet.skalenodes.com/v1/green-giddy-denebola",
             "wss://mainnet-proxy.skalenodes.com/v1/ws/green-giddy-denebola"
         ],
         "shortName": "nebula-mainnet"
     },
     {
+        "chainId": 1517929550,
+        "faucets": [
+            "https://sfuel.dirtroad.dev/staging"
+        ],
+        "infoURL": "",
+        "name": "Deprecated SKALE Titan Hub Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "sFUEL",
+            "symbol": "sFUEL"
+        },
+        "networkId": 1517929550,
+        "rpc": [
+            "https://staging-v3.skalenodes.com/v1/staging-aware-chief-gianfar",
+            "wss://staging-v3.skalenodes.com/v1/ws/staging-aware-chief-gianfar"
+        ],
+        "shortName": "deprecated-titan-testnet"
+    },
+    {
         "chainId": 1564830818,
         "faucets": [
             "https://sfuel.dirtroad.dev"
         ],
         "infoURL": "https://calypsohub.network/",
-        "name": "Calypso NFT Hub (SKALE)",
+        "name": "SKALE Calypso Hub",
         "nativeCurrency": {
             "decimals": 18,
             "name": "sFUEL",
             "symbol": "sFUEL"
         },
         "networkId": 1564830818,
         "rpc": [
@@ -18656,15 +25380,17 @@
         "networkId": 1666600000,
         "rpc": [
             "https://api.harmony.one",
             "https://a.api.s0.t.hmny.io",
             "https://api.s0.t.hmny.io",
             "https://rpc.ankr.com/harmony",
             "https://harmony.api.onfinality.io/public",
-            "https://1rpc.io/one"
+            "https://1rpc.io/one",
+            "https://harmony-0.drpc.org",
+            "wss://harmony-0.drpc.org"
         ],
         "shortName": "hmy-s0"
     },
     {
         "chainId": 1666600001,
         "faucets": [],
         "infoURL": "https://www.harmony.one/",
@@ -18672,15 +25398,17 @@
         "nativeCurrency": {
             "decimals": 18,
             "name": "ONE",
             "symbol": "ONE"
         },
         "networkId": 1666600001,
         "rpc": [
-            "https://api.s1.t.hmny.io"
+            "https://api.s1.t.hmny.io",
+            "https://harmony-1.drpc.org",
+            "wss://harmony-1.drpc.org"
         ],
         "shortName": "hmy-s1"
     },
     {
         "chainId": 1666600002,
         "faucets": [],
         "infoURL": "https://www.harmony.one/",
@@ -18777,14 +25505,46 @@
         "networkId": 1666900001,
         "rpc": [
             "https://api.s1.ps.hmny.io"
         ],
         "shortName": "hmy-ps-s1"
     },
     {
+        "chainId": 1802203764,
+        "faucets": [],
+        "infoURL": "https://kakarot.org",
+        "name": "Kakarot Sepolia",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 1802203764,
+        "rpc": [
+            "https://sepolia-rpc.kakarot.org"
+        ],
+        "shortName": "kkrt-sepolia"
+    },
+    {
+        "chainId": 1918988905,
+        "faucets": [],
+        "infoURL": "https://rarichain.org/",
+        "name": "RARI Chain Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ethereum",
+            "symbol": "ETH"
+        },
+        "networkId": 1918988905,
+        "rpc": [
+            "https://testnet.rpc.rarichain.org/http"
+        ],
+        "shortName": "rari-testnet"
+    },
+    {
         "chainId": 2021121117,
         "faucets": [],
         "infoURL": "https://www.DataHopper.com",
         "name": "DataHopper",
         "nativeCurrency": {
             "decimals": 18,
             "name": "DataHoppers",
@@ -18799,15 +25559,15 @@
     {
         "chainId": 2046399126,
         "faucets": [
             "https://ruby.exchange/faucet.html",
             "https://sfuel.mylilius.com/"
         ],
         "infoURL": "https://europahub.network/",
-        "name": "Europa SKALE Chain",
+        "name": "SKALE Europa Hub",
         "nativeCurrency": {
             "decimals": 18,
             "name": "sFUEL",
             "symbol": "sFUEL"
         },
         "networkId": 2046399126,
         "rpc": [
@@ -18816,25 +25576,25 @@
         ],
         "shortName": "europa"
     },
     {
         "chainId": 2863311531,
         "faucets": [],
         "infoURL": "https://ancient8.gg/",
-        "name": "Ancient8 Testnet",
+        "name": "Ancient8 Testnet (deprecated)",
         "nativeCurrency": {
             "decimals": 18,
             "name": "Ether",
             "symbol": "ETH"
         },
         "networkId": 2863311531,
         "rpc": [
             "https://rpc-testnet.ancient8.gg"
         ],
-        "shortName": "a8"
+        "shortName": "a8old"
     },
     {
         "chainId": 3125659152,
         "faucets": [],
         "infoURL": "https://pirl.io",
         "name": "Pirl",
         "nativeCurrency": {
@@ -18865,44 +25625,109 @@
             "https://frankenstein-rpc.oneledger.network"
         ],
         "shortName": "frankenstein"
     },
     {
         "chainId": 11297108099,
         "faucets": [],
-        "infoURL": "https://palm.io",
+        "infoURL": "https://palm.network",
         "name": "Palm Testnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "PALM",
             "symbol": "PALM"
         },
         "networkId": 11297108099,
         "rpc": [
-            "https://palm-testnet.infura.io/v3/${INFURA_API_KEY}"
+            "https://palm-testnet.infura.io/v3/${INFURA_API_KEY}",
+            "https://palm-testnet.public.blastapi.io"
         ],
         "shortName": "tpalm"
     },
     {
         "chainId": 11297108109,
         "faucets": [],
-        "infoURL": "https://palm.io",
+        "infoURL": "https://palm.network",
         "name": "Palm",
         "nativeCurrency": {
             "decimals": 18,
             "name": "PALM",
             "symbol": "PALM"
         },
         "networkId": 11297108109,
         "rpc": [
-            "https://palm-mainnet.infura.io/v3/${INFURA_API_KEY}"
+            "https://palm-mainnet.infura.io/v3/${INFURA_API_KEY}",
+            "https://palm-mainnet.public.blastapi.io"
         ],
         "shortName": "palm"
     },
     {
+        "chainId": 28872323069,
+        "faucets": [],
+        "infoURL": "https://gitswarm.com/",
+        "name": "GitSwarm Test Network",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "GitSwarm Ether",
+            "symbol": "GS-ETH"
+        },
+        "networkId": 28872323069,
+        "rpc": [
+            "https://gitswarm.com:2096"
+        ],
+        "shortName": "GS-ETH"
+    },
+    {
+        "chainId": 37714555429,
+        "faucets": [],
+        "infoURL": "https://xai.games",
+        "name": "Xai Testnet v2",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "sXai",
+            "symbol": "sXAI"
+        },
+        "networkId": 37714555429,
+        "rpc": [
+            "https://testnet-v2.xai-chain.net/rpc"
+        ],
+        "shortName": "xaitestnet"
+    },
+    {
+        "chainId": 88153591557,
+        "faucets": [],
+        "infoURL": "https://raas.gelato.network/rollups/details/public/arb-blueberry",
+        "name": "Arbitrum Blueberry",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "GelatoCGT",
+            "symbol": "CGT"
+        },
+        "networkId": 88153591557,
+        "rpc": [
+            "https://rpc.arb-blueberry.gelato.digital",
+            "wss://ws.arb-blueberry.gelato.digital"
+        ],
+        "shortName": "arb-blueberry"
+    },
+    {
+        "chainId": 107107114116,
+        "faucets": [],
+        "infoURL": "https://kakarot.org",
+        "name": "Kakarot Sepolia Deprecated",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 107107114116,
+        "rpc": [],
+        "shortName": "kkrt-sepolia-deprecated"
+    },
+    {
         "chainId": 111222333444,
         "faucets": [],
         "infoURL": "https://alphabetnetwork.org",
         "name": "Alphabet Mainnet",
         "nativeCurrency": {
             "decimals": 18,
             "name": "ALT",
@@ -19012,9 +25837,25 @@
             "symbol": "CKB"
         },
         "networkId": 868455272153094,
         "rpc": [
             "https://godwoken-testnet-web3-v1-rpc.ckbapp.dev"
         ],
         "shortName": "gw-testnet-v1-deprecated"
+    },
+    {
+        "chainId": 2713017997578000,
+        "faucets": [],
+        "infoURL": "https://www.dchain.foundation/",
+        "name": "DCHAIN Testnet",
+        "nativeCurrency": {
+            "decimals": 18,
+            "name": "Ether",
+            "symbol": "ETH"
+        },
+        "networkId": 2713017997578000,
+        "rpc": [
+            "https://dchaintestnet-2713017997578000-1.jsonrpc.testnet.sagarpc.io"
+        ],
+        "shortName": "dchaint"
     }
 ]
```

### Comparing `eth-utils-4.1.0/eth_utils/abi.py` & `eth_utils-4.1.1/eth_utils/abi.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/eth_utils/address.py` & `eth_utils-4.1.1/eth_utils/address.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/eth_utils/applicators.py` & `eth_utils-4.1.1/eth_utils/applicators.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/eth_utils/conversions.py` & `eth_utils-4.1.1/eth_utils/conversions.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/eth_utils/currency.py` & `eth_utils-4.1.1/eth_utils/currency.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/eth_utils/curried/__init__.py` & `eth_utils-4.1.1/eth_utils/curried/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/eth_utils/decorators.py` & `eth_utils-4.1.1/eth_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/eth_utils/functional.py` & `eth_utils-4.1.1/eth_utils/functional.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/eth_utils/hexadecimal.py` & `eth_utils-4.1.1/eth_utils/hexadecimal.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/eth_utils/humanize.py` & `eth_utils-4.1.1/eth_utils/humanize.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/eth_utils/logging.py` & `eth_utils-4.1.1/eth_utils/logging.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/eth_utils/module_loading.py` & `eth_utils-4.1.1/eth_utils/module_loading.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/eth_utils/network.py` & `eth_utils-4.1.1/eth_utils/network.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,14 @@
     dataclass,
 )
 import json
 import os
 from typing import (
     List,
 )
-import warnings
 
 from eth_typing import (
     ChainId,
 )
 
 from eth_utils import (
     ValidationError,
@@ -43,21 +42,18 @@
                 chain_id=entry["chainId"],
                 name=entry["name"],
                 shortName=entry["shortName"],
                 symbol=ChainId(entry["chainId"]),
             )
             networks_obj.append(network)
         except ValueError:
-            # Entry does not have a valid ChainId constant in eth-typing
-            warnings.warn(
-                f"Network {entry['chainId']} with name '{entry['name']}' does not have "
-                f"a valid ChainId. eth-typing should be updated with the latest "
-                f"networks.",
-                stacklevel=2,
-            )
+            # Chain does not have a valid ChainId, network files in eth-utils and
+            # eth-typing should to be updated. Run `python update_networks.py` in the
+            # project root.
+            pass
 
     return networks_obj
 
 
 networks = initialize_network_objects()
 
 networks_by_id = {network.chain_id: network for network in networks}
```

### Comparing `eth-utils-4.1.0/eth_utils/numeric.py` & `eth_utils-4.1.1/eth_utils/numeric.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/eth_utils/toolz.py` & `eth_utils-4.1.1/eth_utils/toolz.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/eth_utils/types.py` & `eth_utils-4.1.1/eth_utils/types.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/eth_utils/units.py` & `eth_utils-4.1.1/eth_utils/units.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/eth_utils.egg-info/PKG-INFO` & `eth_utils-4.1.1/eth_utils.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-utils
-Version: 4.1.0
+Version: 4.1.1
 Summary: eth-utils: Common utility functions for python code that interacts with Ethereum
 Home-page: https://github.com/ethereum/eth-utils
 Author: The Ethereum Foundation
 Author-email: snakecharmers@ethereum.org
 License: MIT
 Keywords: ethereum
 Classifier: Intended Audience :: Developers
@@ -29,22 +29,24 @@
 Requires-Dist: eth-hash[pycryptodome]; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
 Requires-Dist: pre-commit>=3.4.0; extra == "dev"
 Requires-Dist: tox>=4.0.0; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 Requires-Dist: sphinx>=6.0.0; extra == "dev"
+Requires-Dist: sphinx-autobuild>=2021.3.14; extra == "dev"
 Requires-Dist: sphinx_rtd_theme>=1.0.0; extra == "dev"
 Requires-Dist: towncrier<22,>=21; extra == "dev"
 Requires-Dist: hypothesis>=4.43.0; extra == "dev"
 Requires-Dist: mypy==1.5.1; extra == "dev"
 Requires-Dist: pytest>=7.0.0; extra == "dev"
 Requires-Dist: pytest-xdist>=2.4.0; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: sphinx>=6.0.0; extra == "docs"
+Requires-Dist: sphinx-autobuild>=2021.3.14; extra == "docs"
 Requires-Dist: sphinx_rtd_theme>=1.0.0; extra == "docs"
 Requires-Dist: towncrier<22,>=21; extra == "docs"
 Provides-Extra: test
 Requires-Dist: hypothesis>=4.43.0; extra == "test"
 Requires-Dist: mypy==1.5.1; extra == "test"
 Requires-Dist: pytest>=7.0.0; extra == "test"
 Requires-Dist: pytest-xdist>=2.4.0; extra == "test"
```

### Comparing `eth-utils-4.1.0/eth_utils.egg-info/SOURCES.txt` & `eth_utils-4.1.1/eth_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/pyproject.toml` & `eth_utils-4.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 [tool.autoflake]
-remove_all_unused_imports = true
 exclude = "__init__.py"
+remove_all_unused_imports = true
 
 [tool.isort]
 combine_as_imports = true
 extra_standard_library = "pytest"
 force_grid_wrap = 1
 force_sort_within_sections = true
-known_third_party = "hypothesis,pytest"
+honor_noqa = true
 known_first_party = "eth_utils"
+known_third_party = "hypothesis"
 multi_line_output = 3
 profile = "black"
+use_parentheses = true
 
 [tool.mypy]
 check_untyped_defs = true
-disallow_incomplete_defs = true
-disallow_untyped_defs = true
 disallow_any_generics = true
+disallow_incomplete_defs = true
+disallow_subclassing_any = true
 disallow_untyped_calls = true
 disallow_untyped_decorators = true
-disallow_subclassing_any = true
+disallow_untyped_defs = true
 ignore_missing_imports = true
-strict_optional = true
 strict_equality = true
+strict_optional = true
 warn_redundant_casts = true
 warn_return_any = true
 warn_unused_configs = true
 warn_unused_ignores = true
 
 
 [tool.pydocstyle]
@@ -59,26 +61,26 @@
 # D400 - Enabling this error code seems to make it a requirement that the first
 # sentence in a docstring is not split across two lines.  It also makes it a
 # requirement that no docstring can have a multi-sentence description without a
 # summary line.  Neither one of those requirements seem appropriate.
 
 [tool.pytest.ini_options]
 addopts = "-v --showlocals --durations 10"
-xfail_strict = true
-log_format = "%(levelname)8s  %(asctime)s  %(filename)20s  %(message)s"
 log_date_format = "%m-%d %H:%M:%S"
+log_format = "%(levelname)8s  %(asctime)s  %(filename)20s  %(message)s"
+xfail_strict = true
 
 [tool.towncrier]
 # Read https://github.com/ethereum/eth-utils/blob/main/newsfragments/README.md for instructions
-package = "eth_utils"
-filename = "docs/release_notes.rst"
 directory = "newsfragments"
-underlines = ["-", "~", "^"]
-title_format = "eth-utils v{version} ({project_date})"
+filename = "docs/release_notes.rst"
 issue_format = "`#{issue} <https://github.com/ethereum/eth-utils/issues/{issue}>`__"
+package = "eth_utils"
+title_format = "eth-utils v{version} ({project_date})"
+underlines = ["-", "~", "^"]
 
 [[tool.towncrier.type]]
 directory = "breaking"
 name = "Breaking Changes"
 showcontent = true
 
 [[tool.towncrier.type]]
```

### Comparing `eth-utils-4.1.0/setup.py` & `eth_utils-4.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
         "pre-commit>=3.4.0",
         "tox>=4.0.0",
         "twine",
         "wheel",
     ],
     "docs": [
         "sphinx>=6.0.0",
+        "sphinx-autobuild>=2021.3.14",
         "sphinx_rtd_theme>=1.0.0",
         "towncrier>=21,<22",
     ],
     "test": [
         "hypothesis>=4.43.0",
         "mypy==1.5.1",
         "pytest>=7.0.0",
@@ -36,15 +37,15 @@
 with open("./README.md") as readme:
     long_description = readme.read()
 
 
 setup(
     name="eth-utils",
     # *IMPORTANT*: Don't manually change the version here. Use `make bump`, as described in readme
-    version="4.1.0",
+    version="4.1.1",
     description=(
         """eth-utils: Common utility functions for python code that interacts with Ethereum"""
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="The Ethereum Foundation",
     author_email="snakecharmers@ethereum.org",
@@ -58,15 +59,15 @@
     ],
     python_requires=">=3.8, <4",
     extras_require=extras_require,
     py_modules=["eth_utils"],
     license="MIT",
     zip_safe=False,
     keywords="ethereum",
-    packages=find_packages(exclude=["tests", "tests.*"]),
+    packages=find_packages(exclude=["scripts", "scripts.*", "tests", "tests.*"]),
     package_data={"eth_utils": ["py.typed"]},
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
```

### Comparing `eth-utils-4.1.0/tests/core/abi-utils/test_abi_utils.py` & `eth_utils-4.1.1/tests/core/abi-utils/test_abi_utils.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/tests/core/address-utils/test_address_utils.py` & `eth_utils-4.1.1/tests/core/address-utils/test_address_utils.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/tests/core/applicator-utils/test_applicators.py` & `eth_utils-4.1.1/tests/core/applicator-utils/test_applicators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import collections
-
 import pytest
 
 import eth_utils
 from eth_utils.curried import (
     apply_formatter_at_index,
     apply_formatter_if,
     apply_formatter_to_array,
```

### Comparing `eth-utils-4.1.0/tests/core/conversion-utils/test_conversions.py` & `eth_utils-4.1.1/tests/core/conversion-utils/test_conversions.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/tests/core/currency-utils/test_currency_tools.py` & `eth_utils-4.1.1/tests/core/currency-utils/test_currency_tools.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import decimal
+import pytest
 
 from hypothesis import (
     given,
     strategies as st,
 )
-import pytest
 
 from eth_utils.currency import (
     MAX_WEI,
     MIN_WEI,
     from_wei,
     to_wei,
     units,
```

### Comparing `eth-utils-4.1.0/tests/core/curried-utils/test_curried.py` & `eth_utils-4.1.1/tests/core/curried-utils/test_curried.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/tests/core/decorator-utils/test_combomethod.py` & `eth_utils-4.1.1/tests/core/decorator-utils/test_combomethod.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/tests/core/decorator-utils/test_replace_exceptions.py` & `eth_utils-4.1.1/tests/core/decorator-utils/test_replace_exceptions.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/tests/core/decorator-utils/test_validate_conversion_arguments.py` & `eth_utils-4.1.1/tests/core/decorator-utils/test_validate_conversion_arguments.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/tests/core/encoding-utils/test_big_endian_integer.py` & `eth_utils-4.1.1/tests/core/encoding-utils/test_big_endian_integer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import pytest
+
 from hypothesis import (
     given,
     strategies as st,
 )
-import pytest
 
 from eth_utils.encoding import (
     big_endian_to_int,
     int_to_big_endian,
 )
```

### Comparing `eth-utils-4.1.0/tests/core/functional-utils/test_return_value_decorators.py` & `eth_utils-4.1.1/tests/core/functional-utils/test_return_value_decorators.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/tests/core/functional-utils/test_type_inference.py` & `eth_utils-4.1.1/tests/core/functional-utils/test_type_inference.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
+import pytest
 from typing import (
     List,
 )
 
 from mypy import (
     api,
 )
-import pytest
 
 MYPY_ARGS = ["--ignore-missing-imports"]
 FIXTURE_DIR = "fixtures/mypy/"
 
 
 def fixture_dir(val: str):
     return FIXTURE_DIR + val
```

### Comparing `eth-utils-4.1.0/tests/core/hexadecimal-utils/test_0x_prefix_addition_and_removal.py` & `eth_utils-4.1.1/tests/core/hexadecimal-utils/test_0x_prefix_addition_and_removal.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/tests/core/hexadecimal-utils/test_is_hex.py` & `eth_utils-4.1.1/tests/core/hexadecimal-utils/test_is_hex.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/tests/core/hexadecimal-utils/test_is_hexstr.py` & `eth_utils-4.1.1/tests/core/hexadecimal-utils/test_is_hexstr.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/tests/core/humanize-utils/test_humanize_integer_sequence.py` & `eth_utils-4.1.1/tests/core/humanize-utils/test_humanize_integer_sequence.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/tests/core/humanize-utils/test_humanize_ipfs_uri.py` & `eth_utils-4.1.1/tests/core/humanize-utils/test_humanize_ipfs_uri.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/tests/core/humanize-utils/test_humanize_seconds.py` & `eth_utils-4.1.1/tests/core/humanize-utils/test_humanize_seconds.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/tests/core/humanize-utils/test_humanize_wei.py` & `eth_utils-4.1.1/tests/core/humanize-utils/test_humanize_wei.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/tests/core/logging-utils/test_DEBUG2_logging.py` & `eth_utils-4.1.1/tests/core/logging-utils/test_DEBUG2_logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
-import uuid
-
 import pytest
+import uuid
 
 from eth_utils import (
     ExtendedDebugLogger,
 )
 from eth_utils.logging import (
     DEBUG2_LEVEL_NUM,
 )
```

### Comparing `eth-utils-4.1.0/tests/core/logging-utils/test_compat_with_abc_ABC.py` & `eth_utils-4.1.1/tests/core/logging-utils/test_compat_with_abc_ABC.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from abc import (
     ABCMeta,
     abstractmethod,
 )
 import logging
-
 import pytest
 
 from eth_utils import (
     HasLoggerMeta,
 )
```

### Comparing `eth-utils-4.1.0/tests/core/logging-utils/test_get_logger.py` & `eth_utils-4.1.1/tests/core/logging-utils/test_get_logger.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/tests/core/logging-utils/test_has_logger_metaclass.py` & `eth_utils-4.1.1/tests/core/logging-utils/test_has_logger_metaclass.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/tests/core/network-utils/test_network_utils.py` & `eth_utils-4.1.1/tests/core/network-utils/test_network_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+import pytest
+
 from eth_typing import (
     ChainId,
 )
-import pytest
 
 from eth_utils import (
     Network,
     ValidationError,
     name_from_chain_id,
     network_from_chain_id,
     short_name_from_chain_id,
```

### Comparing `eth-utils-4.1.0/tests/core/type-checks/mypy_typing_of_curried_utils.py` & `eth_utils-4.1.1/tests/core/type-checks/mypy_typing_of_curried_utils.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/tests/core/type-checks/mypy_typing_of_functional_utils.py` & `eth_utils-4.1.1/tests/core/type-checks/mypy_typing_of_functional_utils.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/tests/core/type-checks/mypy_typing_of_has_logger.py` & `eth_utils-4.1.1/tests/core/type-checks/mypy_typing_of_has_logger.py`

 * *Files identical despite different names*

### Comparing `eth-utils-4.1.0/tests/core/types-utils/test_types_utils.py` & `eth_utils-4.1.1/tests/core/types-utils/test_types_utils.py`

 * *Files identical despite different names*

