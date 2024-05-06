# Comparing `tmp/shelchin-safe-eth-py-6.0.0b26.tar.gz` & `tmp/shelchin-safe-eth-py-6.0.1b26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shelchin-safe-eth-py-6.0.0b26.tar", last modified: Fri Apr 26 06:29:45 2024, max compression
+gzip compressed data, was "shelchin-safe-eth-py-6.0.1b26.tar", last modified: Mon May  6 06:28:36 2024, max compression
```

## Comparing `shelchin-safe-eth-py-6.0.0b26.tar` & `shelchin-safe-eth-py-6.0.1b26.tar`

### file list

```diff
@@ -1,234 +1,234 @@
-drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-04-26 06:29:45.765837 shelchin-safe-eth-py-6.0.0b26/
--rw-r--r--   0 shelchin   (501) staff       (20)     1082 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/LICENSE
--rw-r--r--   0 shelchin   (501) staff       (20)       71 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/MANIFEST.in
--rw-r--r--   0 shelchin   (501) staff       (20)     7105 2024-04-26 06:29:45.765927 shelchin-safe-eth-py-6.0.0b26/PKG-INFO
--rw-r--r--   0 shelchin   (501) staff       (20)     5786 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/README.rst
-drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-04-26 06:29:45.700761 shelchin-safe-eth-py-6.0.0b26/docs/
--rw-r--r--   0 shelchin   (501) staff       (20)      638 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/docs/Makefile
--rw-r--r--   0 shelchin   (501) staff       (20)      799 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/docs/make.bat
-drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-04-26 06:29:45.705269 shelchin-safe-eth-py-6.0.0b26/docs/source/
--rw-r--r--   0 shelchin   (501) staff       (20)     1987 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/docs/source/conf.py
--rw-r--r--   0 shelchin   (501) staff       (20)      978 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/docs/source/gnosis.eth.clients.rst
--rw-r--r--   0 shelchin   (501) staff       (20)      183 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/docs/source/gnosis.eth.contracts.rst
--rw-r--r--   0 shelchin   (501) staff       (20)      954 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/docs/source/gnosis.eth.django.rst
--rw-r--r--   0 shelchin   (501) staff       (20)      177 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/docs/source/gnosis.eth.eip712.rst
--rw-r--r--   0 shelchin   (501) staff       (20)     1198 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/docs/source/gnosis.eth.oracles.abis.rst
--rw-r--r--   0 shelchin   (501) staff       (20)      450 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/docs/source/gnosis.eth.oracles.rst
--rw-r--r--   0 shelchin   (501) staff       (20)      936 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/docs/source/gnosis.eth.rst
--rw-r--r--   0 shelchin   (501) staff       (20)      226 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/docs/source/gnosis.rst
--rw-r--r--   0 shelchin   (501) staff       (20)     1852 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/docs/source/gnosis.safe.rst
--rw-r--r--   0 shelchin   (501) staff       (20)      894 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/docs/source/index.rst
--rw-r--r--   0 shelchin   (501) staff       (20)       55 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/docs/source/modules.rst
--rw-r--r--   0 shelchin   (501) staff       (20)     8368 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/docs/source/quickstart.rst
-drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-04-26 06:29:45.705687 shelchin-safe-eth-py-6.0.0b26/gnosis/
--rw-r--r--   0 shelchin   (501) staff       (20)        0 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/__init__.py
-drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-04-26 06:29:45.706246 shelchin-safe-eth-py-6.0.0b26/gnosis/cowsap/
--rw-r--r--   0 shelchin   (501) staff       (20)      156 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/cowsap/__init__.py
--rw-r--r--   0 shelchin   (501) staff       (20)     8465 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/cowsap/cow_swap_api.py
--rw-r--r--   0 shelchin   (501) staff       (20)     2700 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/cowsap/order.py
-drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-04-26 06:29:45.707049 shelchin-safe-eth-py-6.0.0b26/gnosis/cowsap/tests/
--rw-r--r--   0 shelchin   (501) staff       (20)        0 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/cowsap/tests/__init__.py
--rw-r--r--   0 shelchin   (501) staff       (20)     5604 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/cowsap/tests/test_cow_swap_api.py
-drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-04-26 06:29:45.709374 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/
--rw-r--r--   0 shelchin   (501) staff       (20)     1064 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/__init__.py
-drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-04-26 06:29:45.710502 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/account_abstraction/
--rw-r--r--   0 shelchin   (501) staff       (20)      348 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/account_abstraction/__init__.py
--rw-r--r--   0 shelchin   (501) staff       (20)     7060 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/account_abstraction/bundler_client.py
--rw-r--r--   0 shelchin   (501) staff       (20)      986 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/account_abstraction/constants.py
--rw-r--r--   0 shelchin   (501) staff       (20)      208 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/account_abstraction/exceptions.py
--rw-r--r--   0 shelchin   (501) staff       (20)     4259 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/account_abstraction/user_operation.py
--rw-r--r--   0 shelchin   (501) staff       (20)     3357 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/account_abstraction/user_operation_receipt.py
-drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-04-26 06:29:45.711772 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/clients/
--rw-r--r--   0 shelchin   (501) staff       (20)      878 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/clients/__init__.py
--rw-r--r--   0 shelchin   (501) staff       (20)     9333 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/clients/blockscout_client.py
--rw-r--r--   0 shelchin   (501) staff       (20)      194 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/clients/contract_metadata.py
--rw-r--r--   0 shelchin   (501) staff       (20)     4839 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/clients/ens_client.py
--rw-r--r--   0 shelchin   (501) staff       (20)     9677 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/clients/etherscan_client.py
--rw-r--r--   0 shelchin   (501) staff       (20)     3345 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/clients/sourcify_client.py
--rw-r--r--   0 shelchin   (501) staff       (20)     1020 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/constants.py
-drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-04-26 06:29:45.712153 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/
--rw-r--r--   0 shelchin   (501) staff       (20)    10273 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/__init__.py
-drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-04-26 06:29:45.731241 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/
--rw-r--r--   0 shelchin   (501) staff       (20)   328664 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/CPKFactory.json
--rw-r--r--   0 shelchin   (501) staff       (20)    28908 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_3_0.json
--rw-r--r--   0 shelchin   (501) staff       (20)    29485 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_4_1.json
--rw-r--r--   0 shelchin   (501) staff       (20)    26897 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/DelegateConstructorProxy.json
--rw-r--r--   0 shelchin   (501) staff       (20)    29068 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/ERC1155.json
--rw-r--r--   0 shelchin   (501) staff       (20)    54748 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/ERC20.json
--rw-r--r--   0 shelchin   (501) staff       (20)    89890 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/ERC20TestToken.json
--rw-r--r--   0 shelchin   (501) staff       (20)   622260 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/ERC721.json
--rw-r--r--   0 shelchin   (501) staff       (20)   983403 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/GnosisSafe_V0_0_1.json
--rw-r--r--   0 shelchin   (501) staff       (20)  1158944 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/GnosisSafe_V1_0_0.json
--rw-r--r--   0 shelchin   (501) staff       (20)  1347363 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/GnosisSafe_V1_1_1.json
--rw-r--r--   0 shelchin   (501) staff       (20)   119875 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/GnosisSafe_V1_3_0.json
--rw-r--r--   0 shelchin   (501) staff       (20)    19886 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/MultiSend.json
--rw-r--r--   0 shelchin   (501) staff       (20)    78793 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/PayingProxy.json
--rw-r--r--   0 shelchin   (501) staff       (20)   136946 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/ProxyFactory_V1_0_0.json
--rw-r--r--   0 shelchin   (501) staff       (20)   288861 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/ProxyFactory_V1_1_1.json
--rw-r--r--   0 shelchin   (501) staff       (20)    18975 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/ProxyFactory_V1_3_0.json
--rw-r--r--   0 shelchin   (501) staff       (20)    15538 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/ProxyFactory_V1_4_1.json
--rw-r--r--   0 shelchin   (501) staff       (20)    32495 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/Proxy_V1_0_0.json
--rw-r--r--   0 shelchin   (501) staff       (20)    39032 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/Proxy_V1_1_1.json
--rw-r--r--   0 shelchin   (501) staff       (20)     1862 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/Proxy_V1_3_0.json
--rw-r--r--   0 shelchin   (501) staff       (20)     1849 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/Proxy_V1_4_1.json
--rw-r--r--   0 shelchin   (501) staff       (20)   121611 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/Safe_V1_4_1.json
--rw-r--r--   0 shelchin   (501) staff       (20)     5069 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/SignMessageLib.json
--rw-r--r--   0 shelchin   (501) staff       (20)     4913 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/SimulateTxAccessor_V1_4_1.json
--rw-r--r--   0 shelchin   (501) staff       (20)        0 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/__init__.py
--rw-r--r--   0 shelchin   (501) staff       (20)     7351 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/kyber_network_proxy.json
--rw-r--r--   0 shelchin   (501) staff       (20)    19012 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/multicall.py
--rw-r--r--   0 shelchin   (501) staff       (20)    17165 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/uniswap_exchange.json
--rw-r--r--   0 shelchin   (501) staff       (20)     2480 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/uniswap_factory.json
--rw-r--r--   0 shelchin   (501) staff       (20)     2242 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/uniswap_v2_factory.json
--rw-r--r--   0 shelchin   (501) staff       (20)     8293 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/uniswap_v2_pair.json
--rw-r--r--   0 shelchin   (501) staff       (20)    11889 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/uniswap_v2_router.json
--rw-r--r--   0 shelchin   (501) staff       (20)      954 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/contract_base.py
-drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-04-26 06:29:45.732655 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/django/
--rw-r--r--   0 shelchin   (501) staff       (20)        0 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/django/__init__.py
--rw-r--r--   0 shelchin   (501) staff       (20)     3735 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/django/admin.py
--rw-r--r--   0 shelchin   (501) staff       (20)      269 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/django/filters.py
--rw-r--r--   0 shelchin   (501) staff       (20)     2435 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/django/forms.py
--rw-r--r--   0 shelchin   (501) staff       (20)     9936 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/django/models.py
--rw-r--r--   0 shelchin   (501) staff       (20)     6191 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/django/serializers.py
-drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-04-26 06:29:45.733634 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/django/tests/
--rw-r--r--   0 shelchin   (501) staff       (20)        0 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/django/tests/__init__.py
--rw-r--r--   0 shelchin   (501) staff       (20)      711 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/django/tests/models.py
--rw-r--r--   0 shelchin   (501) staff       (20)     3028 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/django/tests/test_forms.py
--rw-r--r--   0 shelchin   (501) staff       (20)     8621 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/django/tests/test_models.py
--rw-r--r--   0 shelchin   (501) staff       (20)     7877 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/django/tests/test_serializers.py
--rw-r--r--   0 shelchin   (501) staff       (20)      484 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/django/tests/test_validators.py
--rw-r--r--   0 shelchin   (501) staff       (20)      320 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/django/validators.py
-drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-04-26 06:29:45.733809 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/eip712/
--rw-r--r--   0 shelchin   (501) staff       (20)     5915 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/eip712/__init__.py
--rw-r--r--   0 shelchin   (501) staff       (20)    82106 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/ethereum_client.py
--rw-r--r--   0 shelchin   (501) staff       (20)    35581 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/ethereum_network.py
--rw-r--r--   0 shelchin   (501) staff       (20)     1332 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/exceptions.py
--rw-r--r--   0 shelchin   (501) staff       (20)    13617 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/multicall.py
-drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-04-26 06:29:45.735907 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/
--rw-r--r--   0 shelchin   (501) staff       (20)     1093 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/__init__.py
-drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-04-26 06:29:45.738620 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/abis/
--rw-r--r--   0 shelchin   (501) staff       (20)        0 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/abis/__init__.py
--rw-r--r--   0 shelchin   (501) staff       (20)    15986 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/abis/aave_abis.py
--rw-r--r--   0 shelchin   (501) staff       (20)    30036 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/abis/balancer_abis.py
--rw-r--r--   0 shelchin   (501) staff       (20)    29731 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/abis/cream_abis.py
--rw-r--r--   0 shelchin   (501) staff       (20)    27567 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/abis/curve_abis.py
--rw-r--r--   0 shelchin   (501) staff       (20)    25872 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/abis/mooniswap_abis.py
--rw-r--r--   0 shelchin   (501) staff       (20)      239 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/abis/superfluid_abis.py
--rw-r--r--   0 shelchin   (501) staff       (20)    45208 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/abis/uniswap_v3.py
--rw-r--r--   0 shelchin   (501) staff       (20)    36257 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/abis/yearn_abis.py
--rw-r--r--   0 shelchin   (501) staff       (20)     1464 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/abis/zerion_abis.py
--rw-r--r--   0 shelchin   (501) staff       (20)     2375 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/cowswap.py
--rw-r--r--   0 shelchin   (501) staff       (20)      161 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/exceptions.py
-drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-04-26 06:29:45.738948 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/helpers/
--rw-r--r--   0 shelchin   (501) staff       (20)        0 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/helpers/__init__.py
--rw-r--r--   0 shelchin   (501) staff       (20)     5856 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/helpers/curve_gauge_list.py
--rw-r--r--   0 shelchin   (501) staff       (20)     4117 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/kyber.py
--rw-r--r--   0 shelchin   (501) staff       (20)    32169 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/oracles.py
--rw-r--r--   0 shelchin   (501) staff       (20)     1677 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/superfluid.py
--rw-r--r--   0 shelchin   (501) staff       (20)     1516 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/sushiswap.py
--rw-r--r--   0 shelchin   (501) staff       (20)     7154 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/uniswap_v3.py
--rw-r--r--   0 shelchin   (501) staff       (20)     1064 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/utils.py
-drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-04-26 06:29:45.741333 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/
--rw-r--r--   0 shelchin   (501) staff       (20)        0 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/__init__.py
-drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-04-26 06:29:45.742701 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/account_abstraction/
--rw-r--r--   0 shelchin   (501) staff       (20)        0 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/account_abstraction/__init__.py
--rw-r--r--   0 shelchin   (501) staff       (20)     6695 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/account_abstraction/test_bundler_client.py
--rw-r--r--   0 shelchin   (501) staff       (20)     2727 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/account_abstraction/test_e2e_bundler_client.py
--rw-r--r--   0 shelchin   (501) staff       (20)      671 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/account_abstraction/test_user_operation.py
--rw-r--r--   0 shelchin   (501) staff       (20)      947 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/account_abstraction/test_user_operation_receipt.py
-drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-04-26 06:29:45.744059 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/clients/
--rw-r--r--   0 shelchin   (501) staff       (20)        0 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/clients/__init__.py
--rw-r--r--   0 shelchin   (501) staff       (20)   107388 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/clients/mocks.py
--rw-r--r--   0 shelchin   (501) staff       (20)     1047 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/clients/test_blockscout_client.py
--rw-r--r--   0 shelchin   (501) staff       (20)     6185 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/clients/test_ens_client.py
--rw-r--r--   0 shelchin   (501) staff       (20)     1686 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/clients/test_etherscan_client.py
--rw-r--r--   0 shelchin   (501) staff       (20)     2521 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/clients/test_sourcify_client.py
-drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-04-26 06:29:45.744365 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/eip712/
--rw-r--r--   0 shelchin   (501) staff       (20)        0 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/eip712/__init__.py
--rw-r--r--   0 shelchin   (501) staff       (20)    13327 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/eip712/test_eip712.py
--rw-r--r--   0 shelchin   (501) staff       (20)     3189 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/ethereum_test_case.py
-drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-04-26 06:29:45.751022 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/mocks/
--rw-r--r--   0 shelchin   (501) staff       (20)        0 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/mocks/__init__.py
--rw-r--r--   0 shelchin   (501) staff       (20)    29208 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/mocks/mock_bundler.py
--rw-r--r--   0 shelchin   (501) staff       (20)    31306 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/mocks/mock_internal_txs.py
--rw-r--r--   0 shelchin   (501) staff       (20)    10570 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/mocks/mock_log_receipts.py
--rw-r--r--   0 shelchin   (501) staff       (20)   792720 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/mocks/mock_trace_block.py
--rw-r--r--   0 shelchin   (501) staff       (20)    92795 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/mocks/mock_trace_filter.py
--rw-r--r--   0 shelchin   (501) staff       (20)   171076 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/mocks/mock_trace_transaction.py
-drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-04-26 06:29:45.753077 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/oracles/
--rw-r--r--   0 shelchin   (501) staff       (20)        0 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/oracles/__init__.py
--rw-r--r--   0 shelchin   (501) staff       (20)     2706 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/oracles/test_cowswap.py
--rw-r--r--   0 shelchin   (501) staff       (20)     1820 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/oracles/test_kyber.py
--rw-r--r--   0 shelchin   (501) staff       (20)     1460 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/oracles/test_superfluid.py
--rw-r--r--   0 shelchin   (501) staff       (20)     2043 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/oracles/test_sushiswap.py
--rw-r--r--   0 shelchin   (501) staff       (20)     3544 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/oracles/test_uniswap_v3.py
--rw-r--r--   0 shelchin   (501) staff       (20)    61025 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/test_ethereum_client.py
--rw-r--r--   0 shelchin   (501) staff       (20)     7087 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/test_multicall.py
--rw-r--r--   0 shelchin   (501) staff       (20)    21137 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/test_oracles.py
--rw-r--r--   0 shelchin   (501) staff       (20)     7287 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/test_utils.py
--rw-r--r--   0 shelchin   (501) staff       (20)     5069 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/utils.py
--rw-r--r--   0 shelchin   (501) staff       (20)      390 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/typing.py
--rw-r--r--   0 shelchin   (501) staff       (20)     6977 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/eth/utils.py
--rw-r--r--   0 shelchin   (501) staff       (20)        0 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/py.typed
-drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-04-26 06:29:45.758401 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/
--rw-r--r--   0 shelchin   (501) staff       (20)      742 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/__init__.py
-drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-04-26 06:29:45.758893 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/account_abstraction/
--rw-r--r--   0 shelchin   (501) staff       (20)      101 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/account_abstraction/__init__.py
--rw-r--r--   0 shelchin   (501) staff       (20)     5647 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/account_abstraction/safe_operation.py
--rw-r--r--   0 shelchin   (501) staff       (20)    64078 2024-04-26 06:23:40.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/addresses.py
-drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-04-26 06:29:45.759585 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/api/
--rw-r--r--   0 shelchin   (501) staff       (20)      346 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/api/__init__.py
--rw-r--r--   0 shelchin   (501) staff       (20)     2224 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/api/base_api.py
--rw-r--r--   0 shelchin   (501) staff       (20)     2913 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/api/relay_service_api.py
-drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-04-26 06:29:45.760391 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/api/transaction_service_api/
--rw-r--r--   0 shelchin   (501) staff       (20)      103 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/api/transaction_service_api/__init__.py
--rw-r--r--   0 shelchin   (501) staff       (20)    14033 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/api/transaction_service_api/transaction_service_api.py
--rw-r--r--   0 shelchin   (501) staff       (20)     1732 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/api/transaction_service_api/transaction_service_messages.py
--rw-r--r--   0 shelchin   (501) staff       (20)      252 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/api/transaction_service_api/transaction_service_tx.py
--rw-r--r--   0 shelchin   (501) staff       (20)      105 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/enums.py
--rw-r--r--   0 shelchin   (501) staff       (20)     1451 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/exceptions.py
--rw-r--r--   0 shelchin   (501) staff       (20)    11459 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/multi_send.py
--rw-r--r--   0 shelchin   (501) staff       (20)    10479 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/proxy_factory.py
--rw-r--r--   0 shelchin   (501) staff       (20)    36823 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/safe.py
--rw-r--r--   0 shelchin   (501) staff       (20)    11975 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/safe_create2_tx.py
--rw-r--r--   0 shelchin   (501) staff       (20)     9736 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/safe_creator.py
--rw-r--r--   0 shelchin   (501) staff       (20)   121198 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/safe_deployments.py
--rw-r--r--   0 shelchin   (501) staff       (20)    12587 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/safe_signature.py
--rw-r--r--   0 shelchin   (501) staff       (20)    17225 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/safe_tx.py
--rw-r--r--   0 shelchin   (501) staff       (20)     4194 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/serializers.py
--rw-r--r--   0 shelchin   (501) staff       (20)     2000 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/signatures.py
-drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-04-26 06:29:45.763252 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/tests/
--rw-r--r--   0 shelchin   (501) staff       (20)        0 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/tests/__init__.py
-drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-04-26 06:29:45.763641 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/tests/account_abstraction/
--rw-r--r--   0 shelchin   (501) staff       (20)        0 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/tests/account_abstraction/__init__.py
--rw-r--r--   0 shelchin   (501) staff       (20)     3469 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/tests/account_abstraction/test_safe_operation.py
-drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-04-26 06:29:45.763981 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/tests/api/
--rw-r--r--   0 shelchin   (501) staff       (20)        0 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/tests/api/__init__.py
--rw-r--r--   0 shelchin   (501) staff       (20)     5341 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/tests/api/test_transaction_service_api.py
--rw-r--r--   0 shelchin   (501) staff       (20)    20692 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/tests/safe_test_case.py
--rw-r--r--   0 shelchin   (501) staff       (20)     1398 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/tests/test_addresses.py
--rw-r--r--   0 shelchin   (501) staff       (20)    10515 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/tests/test_multi_send.py
-drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-04-26 06:29:45.764327 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/tests/test_proxy_factory/
--rw-r--r--   0 shelchin   (501) staff       (20)        0 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/tests/test_proxy_factory/__init__.py
--rw-r--r--   0 shelchin   (501) staff       (20)     7798 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/tests/test_proxy_factory/test_proxy_factory.py
--rw-r--r--   0 shelchin   (501) staff       (20)    33486 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/tests/test_safe.py
--rw-r--r--   0 shelchin   (501) staff       (20)    16674 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/tests/test_safe_create2_tx.py
--rw-r--r--   0 shelchin   (501) staff       (20)    18510 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/tests/test_safe_signature.py
--rw-r--r--   0 shelchin   (501) staff       (20)    13004 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/tests/test_safe_tx.py
--rw-r--r--   0 shelchin   (501) staff       (20)     2563 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/tests/test_safe_v1_0_0.py
--rw-r--r--   0 shelchin   (501) staff       (20)     1073 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/tests/test_safe_v1_3_0.py
--rw-r--r--   0 shelchin   (501) staff       (20)     3731 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/tests/test_serializers.py
--rw-r--r--   0 shelchin   (501) staff       (20)     3711 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/tests/test_signatures.py
--rw-r--r--   0 shelchin   (501) staff       (20)      287 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/safe/tests/utils.py
-drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-04-26 06:29:45.764941 shelchin-safe-eth-py-6.0.0b26/gnosis/util/
--rw-r--r--   0 shelchin   (501) staff       (20)       83 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/util/__init__.py
--rw-r--r--   0 shelchin   (501) staff       (20)     1003 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/util/http.py
--rw-r--r--   0 shelchin   (501) staff       (20)      450 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/gnosis/util/util.py
--rw-r--r--   0 shelchin   (501) staff       (20)     2485 2024-04-26 06:29:45.766350 shelchin-safe-eth-py-6.0.0b26/setup.cfg
--rw-r--r--   0 shelchin   (501) staff       (20)       69 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.0b26/setup.py
-drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-04-26 06:29:45.765687 shelchin-safe-eth-py-6.0.0b26/shelchin_safe_eth_py.egg-info/
--rw-r--r--   0 shelchin   (501) staff       (20)     7105 2024-04-26 06:29:45.000000 shelchin-safe-eth-py-6.0.0b26/shelchin_safe_eth_py.egg-info/PKG-INFO
--rw-r--r--   0 shelchin   (501) staff       (20)     7506 2024-04-26 06:29:45.000000 shelchin-safe-eth-py-6.0.0b26/shelchin_safe_eth_py.egg-info/SOURCES.txt
--rw-r--r--   0 shelchin   (501) staff       (20)        1 2024-04-26 06:29:45.000000 shelchin-safe-eth-py-6.0.0b26/shelchin_safe_eth_py.egg-info/dependency_links.txt
--rw-r--r--   0 shelchin   (501) staff       (20)      129 2024-04-26 06:29:45.000000 shelchin-safe-eth-py-6.0.0b26/shelchin_safe_eth_py.egg-info/requires.txt
--rw-r--r--   0 shelchin   (501) staff       (20)        7 2024-04-26 06:29:45.000000 shelchin-safe-eth-py-6.0.0b26/shelchin_safe_eth_py.egg-info/top_level.txt
+drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-05-06 06:28:36.347558 shelchin-safe-eth-py-6.0.1b26/
+-rw-r--r--   0 shelchin   (501) staff       (20)     1082 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/LICENSE
+-rw-r--r--   0 shelchin   (501) staff       (20)       71 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/MANIFEST.in
+-rw-r--r--   0 shelchin   (501) staff       (20)     7105 2024-05-06 06:28:36.347660 shelchin-safe-eth-py-6.0.1b26/PKG-INFO
+-rw-r--r--   0 shelchin   (501) staff       (20)     5786 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/README.rst
+drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-05-06 06:28:36.308004 shelchin-safe-eth-py-6.0.1b26/docs/
+-rw-r--r--   0 shelchin   (501) staff       (20)      638 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/docs/Makefile
+-rw-r--r--   0 shelchin   (501) staff       (20)      799 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/docs/make.bat
+drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-05-06 06:28:36.310078 shelchin-safe-eth-py-6.0.1b26/docs/source/
+-rw-r--r--   0 shelchin   (501) staff       (20)     1987 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/docs/source/conf.py
+-rw-r--r--   0 shelchin   (501) staff       (20)      978 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/docs/source/gnosis.eth.clients.rst
+-rw-r--r--   0 shelchin   (501) staff       (20)      183 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/docs/source/gnosis.eth.contracts.rst
+-rw-r--r--   0 shelchin   (501) staff       (20)      954 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/docs/source/gnosis.eth.django.rst
+-rw-r--r--   0 shelchin   (501) staff       (20)      177 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/docs/source/gnosis.eth.eip712.rst
+-rw-r--r--   0 shelchin   (501) staff       (20)     1198 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/docs/source/gnosis.eth.oracles.abis.rst
+-rw-r--r--   0 shelchin   (501) staff       (20)      450 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/docs/source/gnosis.eth.oracles.rst
+-rw-r--r--   0 shelchin   (501) staff       (20)      936 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/docs/source/gnosis.eth.rst
+-rw-r--r--   0 shelchin   (501) staff       (20)      226 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/docs/source/gnosis.rst
+-rw-r--r--   0 shelchin   (501) staff       (20)     1852 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/docs/source/gnosis.safe.rst
+-rw-r--r--   0 shelchin   (501) staff       (20)      894 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/docs/source/index.rst
+-rw-r--r--   0 shelchin   (501) staff       (20)       55 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/docs/source/modules.rst
+-rw-r--r--   0 shelchin   (501) staff       (20)     8368 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/docs/source/quickstart.rst
+drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-05-06 06:28:36.310363 shelchin-safe-eth-py-6.0.1b26/gnosis/
+-rw-r--r--   0 shelchin   (501) staff       (20)        0 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/__init__.py
+drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-05-06 06:28:36.310865 shelchin-safe-eth-py-6.0.1b26/gnosis/cowsap/
+-rw-r--r--   0 shelchin   (501) staff       (20)      156 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/cowsap/__init__.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     8465 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/cowsap/cow_swap_api.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     2700 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/cowsap/order.py
+drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-05-06 06:28:36.311133 shelchin-safe-eth-py-6.0.1b26/gnosis/cowsap/tests/
+-rw-r--r--   0 shelchin   (501) staff       (20)        0 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/cowsap/tests/__init__.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     5604 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/cowsap/tests/test_cow_swap_api.py
+drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-05-06 06:28:36.312276 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/
+-rw-r--r--   0 shelchin   (501) staff       (20)     1064 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/__init__.py
+drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-05-06 06:28:36.313172 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/account_abstraction/
+-rw-r--r--   0 shelchin   (501) staff       (20)      348 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/account_abstraction/__init__.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     7060 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/account_abstraction/bundler_client.py
+-rw-r--r--   0 shelchin   (501) staff       (20)      986 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/account_abstraction/constants.py
+-rw-r--r--   0 shelchin   (501) staff       (20)      208 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/account_abstraction/exceptions.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     4259 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/account_abstraction/user_operation.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     3357 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/account_abstraction/user_operation_receipt.py
+drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-05-06 06:28:36.314105 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/clients/
+-rw-r--r--   0 shelchin   (501) staff       (20)      878 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/clients/__init__.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     9333 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/clients/blockscout_client.py
+-rw-r--r--   0 shelchin   (501) staff       (20)      194 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/clients/contract_metadata.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     4839 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/clients/ens_client.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     9677 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/clients/etherscan_client.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     3345 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/clients/sourcify_client.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     1020 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/constants.py
+drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-05-06 06:28:36.314378 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/
+-rw-r--r--   0 shelchin   (501) staff       (20)    10273 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/__init__.py
+drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-05-06 06:28:36.324884 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/
+-rw-r--r--   0 shelchin   (501) staff       (20)   328664 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/CPKFactory.json
+-rw-r--r--   0 shelchin   (501) staff       (20)    28908 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_3_0.json
+-rw-r--r--   0 shelchin   (501) staff       (20)    29485 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_4_1.json
+-rw-r--r--   0 shelchin   (501) staff       (20)    26897 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/DelegateConstructorProxy.json
+-rw-r--r--   0 shelchin   (501) staff       (20)    29068 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/ERC1155.json
+-rw-r--r--   0 shelchin   (501) staff       (20)    54748 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/ERC20.json
+-rw-r--r--   0 shelchin   (501) staff       (20)    89890 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/ERC20TestToken.json
+-rw-r--r--   0 shelchin   (501) staff       (20)   622260 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/ERC721.json
+-rw-r--r--   0 shelchin   (501) staff       (20)   983403 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/GnosisSafe_V0_0_1.json
+-rw-r--r--   0 shelchin   (501) staff       (20)  1158944 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/GnosisSafe_V1_0_0.json
+-rw-r--r--   0 shelchin   (501) staff       (20)  1347363 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/GnosisSafe_V1_1_1.json
+-rw-r--r--   0 shelchin   (501) staff       (20)   119875 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/GnosisSafe_V1_3_0.json
+-rw-r--r--   0 shelchin   (501) staff       (20)    19886 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/MultiSend.json
+-rw-r--r--   0 shelchin   (501) staff       (20)    78793 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/PayingProxy.json
+-rw-r--r--   0 shelchin   (501) staff       (20)   136946 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/ProxyFactory_V1_0_0.json
+-rw-r--r--   0 shelchin   (501) staff       (20)   288861 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/ProxyFactory_V1_1_1.json
+-rw-r--r--   0 shelchin   (501) staff       (20)    18975 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/ProxyFactory_V1_3_0.json
+-rw-r--r--   0 shelchin   (501) staff       (20)    15538 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/ProxyFactory_V1_4_1.json
+-rw-r--r--   0 shelchin   (501) staff       (20)    32495 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/Proxy_V1_0_0.json
+-rw-r--r--   0 shelchin   (501) staff       (20)    39032 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/Proxy_V1_1_1.json
+-rw-r--r--   0 shelchin   (501) staff       (20)     1862 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/Proxy_V1_3_0.json
+-rw-r--r--   0 shelchin   (501) staff       (20)     1849 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/Proxy_V1_4_1.json
+-rw-r--r--   0 shelchin   (501) staff       (20)   121611 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/Safe_V1_4_1.json
+-rw-r--r--   0 shelchin   (501) staff       (20)     5069 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/SignMessageLib.json
+-rw-r--r--   0 shelchin   (501) staff       (20)     4913 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/SimulateTxAccessor_V1_4_1.json
+-rw-r--r--   0 shelchin   (501) staff       (20)        0 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/__init__.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     7351 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/kyber_network_proxy.json
+-rw-r--r--   0 shelchin   (501) staff       (20)    19012 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/multicall.py
+-rw-r--r--   0 shelchin   (501) staff       (20)    17165 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/uniswap_exchange.json
+-rw-r--r--   0 shelchin   (501) staff       (20)     2480 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/uniswap_factory.json
+-rw-r--r--   0 shelchin   (501) staff       (20)     2242 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/uniswap_v2_factory.json
+-rw-r--r--   0 shelchin   (501) staff       (20)     8293 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/uniswap_v2_pair.json
+-rw-r--r--   0 shelchin   (501) staff       (20)    11889 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/uniswap_v2_router.json
+-rw-r--r--   0 shelchin   (501) staff       (20)      954 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/contract_base.py
+drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-05-06 06:28:36.325961 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/django/
+-rw-r--r--   0 shelchin   (501) staff       (20)        0 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/django/__init__.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     3735 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/django/admin.py
+-rw-r--r--   0 shelchin   (501) staff       (20)      269 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/django/filters.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     2435 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/django/forms.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     9936 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/django/models.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     6191 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/django/serializers.py
+drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-05-06 06:28:36.327098 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/django/tests/
+-rw-r--r--   0 shelchin   (501) staff       (20)        0 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/django/tests/__init__.py
+-rw-r--r--   0 shelchin   (501) staff       (20)      711 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/django/tests/models.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     3028 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/django/tests/test_forms.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     8621 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/django/tests/test_models.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     7877 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/django/tests/test_serializers.py
+-rw-r--r--   0 shelchin   (501) staff       (20)      484 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/django/tests/test_validators.py
+-rw-r--r--   0 shelchin   (501) staff       (20)      320 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/django/validators.py
+drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-05-06 06:28:36.327247 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/eip712/
+-rw-r--r--   0 shelchin   (501) staff       (20)     5915 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/eip712/__init__.py
+-rw-r--r--   0 shelchin   (501) staff       (20)    82106 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/ethereum_client.py
+-rw-r--r--   0 shelchin   (501) staff       (20)    35581 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/ethereum_network.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     1332 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/exceptions.py
+-rw-r--r--   0 shelchin   (501) staff       (20)    13617 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/multicall.py
+drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-05-06 06:28:36.328604 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/
+-rw-r--r--   0 shelchin   (501) staff       (20)     1093 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/__init__.py
+drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-05-06 06:28:36.330172 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/abis/
+-rw-r--r--   0 shelchin   (501) staff       (20)        0 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/abis/__init__.py
+-rw-r--r--   0 shelchin   (501) staff       (20)    15986 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/abis/aave_abis.py
+-rw-r--r--   0 shelchin   (501) staff       (20)    30036 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/abis/balancer_abis.py
+-rw-r--r--   0 shelchin   (501) staff       (20)    29731 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/abis/cream_abis.py
+-rw-r--r--   0 shelchin   (501) staff       (20)    27567 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/abis/curve_abis.py
+-rw-r--r--   0 shelchin   (501) staff       (20)    25872 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/abis/mooniswap_abis.py
+-rw-r--r--   0 shelchin   (501) staff       (20)      239 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/abis/superfluid_abis.py
+-rw-r--r--   0 shelchin   (501) staff       (20)    45208 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/abis/uniswap_v3.py
+-rw-r--r--   0 shelchin   (501) staff       (20)    36257 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/abis/yearn_abis.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     1464 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/abis/zerion_abis.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     2375 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/cowswap.py
+-rw-r--r--   0 shelchin   (501) staff       (20)      161 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/exceptions.py
+drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-05-06 06:28:36.330429 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/helpers/
+-rw-r--r--   0 shelchin   (501) staff       (20)        0 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/helpers/__init__.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     5856 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/helpers/curve_gauge_list.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     4117 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/kyber.py
+-rw-r--r--   0 shelchin   (501) staff       (20)    32169 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/oracles.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     1677 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/superfluid.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     1516 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/sushiswap.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     7154 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/uniswap_v3.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     1064 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/utils.py
+drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-05-06 06:28:36.331411 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/
+-rw-r--r--   0 shelchin   (501) staff       (20)        0 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/__init__.py
+drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-05-06 06:28:36.332124 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/account_abstraction/
+-rw-r--r--   0 shelchin   (501) staff       (20)        0 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/account_abstraction/__init__.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     6695 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/account_abstraction/test_bundler_client.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     2727 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/account_abstraction/test_e2e_bundler_client.py
+-rw-r--r--   0 shelchin   (501) staff       (20)      671 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/account_abstraction/test_user_operation.py
+-rw-r--r--   0 shelchin   (501) staff       (20)      947 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/account_abstraction/test_user_operation_receipt.py
+drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-05-06 06:28:36.333921 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/clients/
+-rw-r--r--   0 shelchin   (501) staff       (20)        0 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/clients/__init__.py
+-rw-r--r--   0 shelchin   (501) staff       (20)   107388 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/clients/mocks.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     1047 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/clients/test_blockscout_client.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     6185 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/clients/test_ens_client.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     1686 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/clients/test_etherscan_client.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     2521 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/clients/test_sourcify_client.py
+drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-05-06 06:28:36.334207 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/eip712/
+-rw-r--r--   0 shelchin   (501) staff       (20)        0 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/eip712/__init__.py
+-rw-r--r--   0 shelchin   (501) staff       (20)    13327 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/eip712/test_eip712.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     3189 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/ethereum_test_case.py
+drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-05-06 06:28:36.336087 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/mocks/
+-rw-r--r--   0 shelchin   (501) staff       (20)        0 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/mocks/__init__.py
+-rw-r--r--   0 shelchin   (501) staff       (20)    29208 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/mocks/mock_bundler.py
+-rw-r--r--   0 shelchin   (501) staff       (20)    31306 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/mocks/mock_internal_txs.py
+-rw-r--r--   0 shelchin   (501) staff       (20)    10570 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/mocks/mock_log_receipts.py
+-rw-r--r--   0 shelchin   (501) staff       (20)   792720 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/mocks/mock_trace_block.py
+-rw-r--r--   0 shelchin   (501) staff       (20)    92795 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/mocks/mock_trace_filter.py
+-rw-r--r--   0 shelchin   (501) staff       (20)   171076 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/mocks/mock_trace_transaction.py
+drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-05-06 06:28:36.337103 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/oracles/
+-rw-r--r--   0 shelchin   (501) staff       (20)        0 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/oracles/__init__.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     2706 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/oracles/test_cowswap.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     1820 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/oracles/test_kyber.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     1460 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/oracles/test_superfluid.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     2043 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/oracles/test_sushiswap.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     3544 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/oracles/test_uniswap_v3.py
+-rw-r--r--   0 shelchin   (501) staff       (20)    61025 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/test_ethereum_client.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     7087 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/test_multicall.py
+-rw-r--r--   0 shelchin   (501) staff       (20)    21137 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/test_oracles.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     7287 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/test_utils.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     5069 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/utils.py
+-rw-r--r--   0 shelchin   (501) staff       (20)      390 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/typing.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     6977 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/eth/utils.py
+-rw-r--r--   0 shelchin   (501) staff       (20)        0 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/py.typed
+drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-05-06 06:28:36.340311 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/
+-rw-r--r--   0 shelchin   (501) staff       (20)      742 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/__init__.py
+drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-05-06 06:28:36.340741 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/account_abstraction/
+-rw-r--r--   0 shelchin   (501) staff       (20)      101 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/account_abstraction/__init__.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     5647 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/account_abstraction/safe_operation.py
+-rw-r--r--   0 shelchin   (501) staff       (20)    64078 2024-05-06 06:25:26.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/addresses.py
+drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-05-06 06:28:36.341536 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/api/
+-rw-r--r--   0 shelchin   (501) staff       (20)      346 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/api/__init__.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     2224 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/api/base_api.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     2913 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/api/relay_service_api.py
+drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-05-06 06:28:36.342249 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/api/transaction_service_api/
+-rw-r--r--   0 shelchin   (501) staff       (20)      103 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/api/transaction_service_api/__init__.py
+-rw-r--r--   0 shelchin   (501) staff       (20)    14033 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/api/transaction_service_api/transaction_service_api.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     1732 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/api/transaction_service_api/transaction_service_messages.py
+-rw-r--r--   0 shelchin   (501) staff       (20)      252 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/api/transaction_service_api/transaction_service_tx.py
+-rw-r--r--   0 shelchin   (501) staff       (20)      105 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/enums.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     1451 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/exceptions.py
+-rw-r--r--   0 shelchin   (501) staff       (20)    11459 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/multi_send.py
+-rw-r--r--   0 shelchin   (501) staff       (20)    10479 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/proxy_factory.py
+-rw-r--r--   0 shelchin   (501) staff       (20)    36823 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/safe.py
+-rw-r--r--   0 shelchin   (501) staff       (20)    11975 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/safe_create2_tx.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     9736 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/safe_creator.py
+-rw-r--r--   0 shelchin   (501) staff       (20)   121198 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/safe_deployments.py
+-rw-r--r--   0 shelchin   (501) staff       (20)    12587 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/safe_signature.py
+-rw-r--r--   0 shelchin   (501) staff       (20)    17225 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/safe_tx.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     4194 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/serializers.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     2000 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/signatures.py
+drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-05-06 06:28:36.344749 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/tests/
+-rw-r--r--   0 shelchin   (501) staff       (20)        0 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/tests/__init__.py
+drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-05-06 06:28:36.345088 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/tests/account_abstraction/
+-rw-r--r--   0 shelchin   (501) staff       (20)        0 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/tests/account_abstraction/__init__.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     3469 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/tests/account_abstraction/test_safe_operation.py
+drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-05-06 06:28:36.345457 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/tests/api/
+-rw-r--r--   0 shelchin   (501) staff       (20)        0 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/tests/api/__init__.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     5341 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/tests/api/test_transaction_service_api.py
+-rw-r--r--   0 shelchin   (501) staff       (20)    20692 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/tests/safe_test_case.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     1398 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/tests/test_addresses.py
+-rw-r--r--   0 shelchin   (501) staff       (20)    10515 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/tests/test_multi_send.py
+drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-05-06 06:28:36.345779 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/tests/test_proxy_factory/
+-rw-r--r--   0 shelchin   (501) staff       (20)        0 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/tests/test_proxy_factory/__init__.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     7798 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/tests/test_proxy_factory/test_proxy_factory.py
+-rw-r--r--   0 shelchin   (501) staff       (20)    33486 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/tests/test_safe.py
+-rw-r--r--   0 shelchin   (501) staff       (20)    16674 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/tests/test_safe_create2_tx.py
+-rw-r--r--   0 shelchin   (501) staff       (20)    18510 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/tests/test_safe_signature.py
+-rw-r--r--   0 shelchin   (501) staff       (20)    13004 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/tests/test_safe_tx.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     2563 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/tests/test_safe_v1_0_0.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     1073 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/tests/test_safe_v1_3_0.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     3731 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/tests/test_serializers.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     3711 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/tests/test_signatures.py
+-rw-r--r--   0 shelchin   (501) staff       (20)      287 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/safe/tests/utils.py
+drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-05-06 06:28:36.346262 shelchin-safe-eth-py-6.0.1b26/gnosis/util/
+-rw-r--r--   0 shelchin   (501) staff       (20)       83 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/util/__init__.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     1003 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/util/http.py
+-rw-r--r--   0 shelchin   (501) staff       (20)      450 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/gnosis/util/util.py
+-rw-r--r--   0 shelchin   (501) staff       (20)     2485 2024-05-06 06:28:36.348117 shelchin-safe-eth-py-6.0.1b26/setup.cfg
+-rw-r--r--   0 shelchin   (501) staff       (20)       69 2024-04-26 06:17:33.000000 shelchin-safe-eth-py-6.0.1b26/setup.py
+drwxr-xr-x   0 shelchin   (501) staff       (20)        0 2024-05-06 06:28:36.347376 shelchin-safe-eth-py-6.0.1b26/shelchin_safe_eth_py.egg-info/
+-rw-r--r--   0 shelchin   (501) staff       (20)     7105 2024-05-06 06:28:36.000000 shelchin-safe-eth-py-6.0.1b26/shelchin_safe_eth_py.egg-info/PKG-INFO
+-rw-r--r--   0 shelchin   (501) staff       (20)     7506 2024-05-06 06:28:36.000000 shelchin-safe-eth-py-6.0.1b26/shelchin_safe_eth_py.egg-info/SOURCES.txt
+-rw-r--r--   0 shelchin   (501) staff       (20)        1 2024-05-06 06:28:36.000000 shelchin-safe-eth-py-6.0.1b26/shelchin_safe_eth_py.egg-info/dependency_links.txt
+-rw-r--r--   0 shelchin   (501) staff       (20)      129 2024-05-06 06:28:36.000000 shelchin-safe-eth-py-6.0.1b26/shelchin_safe_eth_py.egg-info/requires.txt
+-rw-r--r--   0 shelchin   (501) staff       (20)        7 2024-05-06 06:28:36.000000 shelchin-safe-eth-py-6.0.1b26/shelchin_safe_eth_py.egg-info/top_level.txt
```

### Comparing `shelchin-safe-eth-py-6.0.0b26/LICENSE` & `shelchin-safe-eth-py-6.0.1b26/LICENSE`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/PKG-INFO` & `shelchin-safe-eth-py-6.0.1b26/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shelchin-safe-eth-py
-Version: 6.0.0b26
+Version: 6.0.1b26
 Summary: Safe Ecosystem Foundation utilities for Ethereum projects
 Home-page: https://github.com/safe-global/safe-eth-py
 Author: Uxío
 Author-email: uxio@safe.global
 License: MIT License
 Project-URL: Documentation, https://safe-eth-py.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/safe-global/safe-eth-py
```

### Comparing `shelchin-safe-eth-py-6.0.0b26/README.rst` & `shelchin-safe-eth-py-6.0.1b26/README.rst`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/docs/Makefile` & `shelchin-safe-eth-py-6.0.1b26/docs/Makefile`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/docs/make.bat` & `shelchin-safe-eth-py-6.0.1b26/docs/make.bat`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/docs/source/conf.py` & `shelchin-safe-eth-py-6.0.1b26/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/docs/source/gnosis.eth.clients.rst` & `shelchin-safe-eth-py-6.0.1b26/docs/source/gnosis.eth.clients.rst`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/docs/source/gnosis.eth.django.rst` & `shelchin-safe-eth-py-6.0.1b26/docs/source/gnosis.eth.django.rst`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/docs/source/gnosis.eth.oracles.abis.rst` & `shelchin-safe-eth-py-6.0.1b26/docs/source/gnosis.eth.oracles.abis.rst`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/docs/source/gnosis.eth.rst` & `shelchin-safe-eth-py-6.0.1b26/docs/source/gnosis.eth.rst`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/docs/source/gnosis.safe.rst` & `shelchin-safe-eth-py-6.0.1b26/docs/source/gnosis.safe.rst`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/docs/source/index.rst` & `shelchin-safe-eth-py-6.0.1b26/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/docs/source/quickstart.rst` & `shelchin-safe-eth-py-6.0.1b26/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/cowsap/cow_swap_api.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/cowsap/cow_swap_api.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/cowsap/order.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/cowsap/order.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/cowsap/tests/test_cow_swap_api.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/cowsap/tests/test_cow_swap_api.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/__init__.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/__init__.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/account_abstraction/bundler_client.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/account_abstraction/bundler_client.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/account_abstraction/constants.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/account_abstraction/constants.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/account_abstraction/user_operation.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/account_abstraction/user_operation.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/account_abstraction/user_operation_receipt.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/account_abstraction/user_operation_receipt.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/clients/__init__.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/clients/blockscout_client.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/clients/blockscout_client.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/clients/ens_client.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/clients/ens_client.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/clients/etherscan_client.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/clients/etherscan_client.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/clients/sourcify_client.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/clients/sourcify_client.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/constants.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/constants.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/__init__.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/CPKFactory.json` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/CPKFactory.json`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_3_0.json` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_4_1.json` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_4_1.json`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/DelegateConstructorProxy.json` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/DelegateConstructorProxy.json`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/ERC1155.json` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/ERC1155.json`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/ERC20.json` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/ERC20.json`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/ERC20TestToken.json` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/ERC20TestToken.json`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/ERC721.json` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/ERC721.json`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/GnosisSafe_V0_0_1.json` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/GnosisSafe_V0_0_1.json`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/GnosisSafe_V1_0_0.json` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/GnosisSafe_V1_0_0.json`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/GnosisSafe_V1_1_1.json` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/GnosisSafe_V1_1_1.json`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/GnosisSafe_V1_3_0.json` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/GnosisSafe_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/MultiSend.json` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/MultiSend.json`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/PayingProxy.json` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/PayingProxy.json`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/ProxyFactory_V1_0_0.json` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/ProxyFactory_V1_0_0.json`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/ProxyFactory_V1_1_1.json` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/ProxyFactory_V1_1_1.json`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/ProxyFactory_V1_3_0.json` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/ProxyFactory_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/ProxyFactory_V1_4_1.json` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/ProxyFactory_V1_4_1.json`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/Proxy_V1_0_0.json` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/Proxy_V1_0_0.json`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/Proxy_V1_1_1.json` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/Proxy_V1_1_1.json`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/Proxy_V1_3_0.json` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/Proxy_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/Proxy_V1_4_1.json` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/Proxy_V1_4_1.json`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/Safe_V1_4_1.json` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/Safe_V1_4_1.json`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/SignMessageLib.json` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/SignMessageLib.json`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/SimulateTxAccessor_V1_4_1.json` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/SimulateTxAccessor_V1_4_1.json`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/kyber_network_proxy.json` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/kyber_network_proxy.json`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/multicall.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/multicall.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/uniswap_exchange.json` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/uniswap_exchange.json`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/uniswap_factory.json` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/uniswap_factory.json`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/uniswap_v2_factory.json` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/uniswap_v2_factory.json`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/uniswap_v2_pair.json` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/uniswap_v2_pair.json`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/abis/uniswap_v2_router.json` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/abis/uniswap_v2_router.json`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/contracts/contract_base.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/contracts/contract_base.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/django/admin.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/django/admin.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/django/forms.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/django/forms.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/django/models.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/django/models.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/django/serializers.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/django/serializers.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/django/tests/models.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/django/tests/models.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/django/tests/test_forms.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/django/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/django/tests/test_models.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/django/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/django/tests/test_serializers.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/django/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/eip712/__init__.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/eip712/__init__.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/ethereum_client.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/ethereum_client.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/ethereum_network.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/ethereum_network.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/exceptions.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/exceptions.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/multicall.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/multicall.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/__init__.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/__init__.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/abis/aave_abis.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/abis/aave_abis.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/abis/balancer_abis.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/abis/balancer_abis.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/abis/cream_abis.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/abis/cream_abis.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/abis/curve_abis.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/abis/curve_abis.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/abis/mooniswap_abis.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/abis/mooniswap_abis.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/abis/uniswap_v3.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/abis/uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/abis/yearn_abis.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/abis/yearn_abis.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/abis/zerion_abis.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/abis/zerion_abis.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/cowswap.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/cowswap.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/helpers/curve_gauge_list.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/helpers/curve_gauge_list.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/kyber.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/kyber.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/oracles.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/oracles.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/superfluid.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/superfluid.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/sushiswap.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/sushiswap.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/uniswap_v3.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/oracles/utils.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/oracles/utils.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/account_abstraction/test_bundler_client.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/account_abstraction/test_bundler_client.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/account_abstraction/test_e2e_bundler_client.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/account_abstraction/test_e2e_bundler_client.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/account_abstraction/test_user_operation.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/account_abstraction/test_user_operation.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/account_abstraction/test_user_operation_receipt.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/account_abstraction/test_user_operation_receipt.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/clients/mocks.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/clients/mocks.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/clients/test_blockscout_client.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/clients/test_blockscout_client.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/clients/test_ens_client.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/clients/test_ens_client.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/clients/test_etherscan_client.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/clients/test_etherscan_client.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/clients/test_sourcify_client.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/clients/test_sourcify_client.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/eip712/test_eip712.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/eip712/test_eip712.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/ethereum_test_case.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/ethereum_test_case.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/mocks/mock_bundler.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/mocks/mock_bundler.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/mocks/mock_internal_txs.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/mocks/mock_internal_txs.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/mocks/mock_log_receipts.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/mocks/mock_log_receipts.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/mocks/mock_trace_block.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/mocks/mock_trace_block.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/mocks/mock_trace_filter.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/mocks/mock_trace_filter.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/mocks/mock_trace_transaction.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/mocks/mock_trace_transaction.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/oracles/test_cowswap.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/oracles/test_cowswap.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/oracles/test_kyber.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/oracles/test_kyber.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/oracles/test_superfluid.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/oracles/test_superfluid.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/oracles/test_sushiswap.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/oracles/test_sushiswap.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/oracles/test_uniswap_v3.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/oracles/test_uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/test_ethereum_client.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/test_ethereum_client.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/test_multicall.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/test_multicall.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/test_oracles.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/test_oracles.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/test_utils.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/tests/utils.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/tests/utils.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/eth/utils.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/eth/utils.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/safe/__init__.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/safe/__init__.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/safe/account_abstraction/safe_operation.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/safe/account_abstraction/safe_operation.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/safe/addresses.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/safe/addresses.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 SAFE_SIMULATE_TX_ACCESSOR_ADDRESS: ChecksumAddress = (
     "0x3d4BA2E0884aa488718476ca2FB8Efc291A46199"
 )
 
 MASTER_COPIES: Dict[EthereumNetwork, List[Tuple[str, int, str]]] = {
     EthereumNetwork.ENDURANCE_SMART_CHAIN_MAINNET:[
-          ("0xBB6e90eBF1cF74af708c160E622A87d40A9AC388", 353904, "1.4.1"),
+          ("0x7de94E90A09E70b85AC2B47d39bCcFe968DCE58C", 353904, "1.4.1"),
     ],
     EthereumNetwork.MAINNET: [
         ("0x29fcB43b46531BcA003ddC8FCB67FFE91900C762", 17486982, "1.4.1+L2"),
         ("0x41675C099F32341bf84BFc5382aF534df5C7461a", 17487000, "1.4.1"),
         (
             "0xfb1bffC9d739B8D520DaF37dF666da4C687191EA",
             14981217,
```

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/safe/api/base_api.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/safe/api/base_api.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/safe/api/relay_service_api.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/safe/api/relay_service_api.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/safe/api/transaction_service_api/transaction_service_api.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/safe/api/transaction_service_api/transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/safe/api/transaction_service_api/transaction_service_messages.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/safe/api/transaction_service_api/transaction_service_messages.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/safe/exceptions.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/safe/exceptions.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/safe/multi_send.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/safe/multi_send.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/safe/proxy_factory.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/safe/proxy_factory.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/safe/safe.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/safe/safe.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/safe/safe_create2_tx.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/safe/safe_create2_tx.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/safe/safe_creator.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/safe/safe_creator.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/safe/safe_deployments.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/safe/safe_deployments.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/safe/safe_signature.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/safe/safe_signature.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/safe/safe_tx.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/safe/safe_tx.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/safe/serializers.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/safe/serializers.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/safe/signatures.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/safe/signatures.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/safe/tests/account_abstraction/test_safe_operation.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/safe/tests/account_abstraction/test_safe_operation.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/safe/tests/api/test_transaction_service_api.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/safe/tests/api/test_transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/safe/tests/safe_test_case.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/safe/tests/safe_test_case.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/safe/tests/test_addresses.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/safe/tests/test_addresses.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/safe/tests/test_multi_send.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/safe/tests/test_multi_send.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/safe/tests/test_proxy_factory/test_proxy_factory.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/safe/tests/test_proxy_factory/test_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/safe/tests/test_safe.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/safe/tests/test_safe.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/safe/tests/test_safe_create2_tx.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/safe/tests/test_safe_create2_tx.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/safe/tests/test_safe_signature.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/safe/tests/test_safe_signature.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/safe/tests/test_safe_tx.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/safe/tests/test_safe_tx.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/safe/tests/test_safe_v1_0_0.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/safe/tests/test_safe_v1_0_0.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/safe/tests/test_safe_v1_3_0.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/safe/tests/test_safe_v1_3_0.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/safe/tests/test_serializers.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/safe/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/safe/tests/test_signatures.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/safe/tests/test_signatures.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/gnosis/util/http.py` & `shelchin-safe-eth-py-6.0.1b26/gnosis/util/http.py`

 * *Files identical despite different names*

### Comparing `shelchin-safe-eth-py-6.0.0b26/setup.cfg` & `shelchin-safe-eth-py-6.0.1b26/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = shelchin-safe-eth-py
-version = 6.0.0b26
+version = 6.0.1b26
 description = Safe Ecosystem Foundation utilities for Ethereum projects
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 keywords = 
 	ethereum
 	web3
 	django
```

### Comparing `shelchin-safe-eth-py-6.0.0b26/shelchin_safe_eth_py.egg-info/PKG-INFO` & `shelchin-safe-eth-py-6.0.1b26/shelchin_safe_eth_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shelchin-safe-eth-py
-Version: 6.0.0b26
+Version: 6.0.1b26
 Summary: Safe Ecosystem Foundation utilities for Ethereum projects
 Home-page: https://github.com/safe-global/safe-eth-py
 Author: Uxío
 Author-email: uxio@safe.global
 License: MIT License
 Project-URL: Documentation, https://safe-eth-py.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/safe-global/safe-eth-py
```

### Comparing `shelchin-safe-eth-py-6.0.0b26/shelchin_safe_eth_py.egg-info/SOURCES.txt` & `shelchin-safe-eth-py-6.0.1b26/shelchin_safe_eth_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

