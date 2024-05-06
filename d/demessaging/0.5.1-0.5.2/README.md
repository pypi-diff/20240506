# Comparing `tmp/demessaging-0.5.1.tar.gz` & `tmp/demessaging-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "demessaging-0.5.1.tar", last modified: Wed Apr  3 08:35:22 2024, max compression
+gzip compressed data, was "demessaging-0.5.2.tar", last modified: Mon May  6 09:29:07 2024, max compression
```

## Comparing `demessaging-0.5.1.tar` & `demessaging-0.5.2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:35:22.150555 demessaging-0.5.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:35:22.117552 demessaging-0.5.1/LICENSES/
--rw-rw-rw-   0 root         (0) root         (0)    10280 2024-03-20 13:01:01.000000 demessaging-0.5.1/LICENSES/Apache-2.0.txt
--rw-rw-rw-   0 root         (0) root         (0)    17023 2024-03-20 13:01:01.000000 demessaging-0.5.1/LICENSES/CC-BY-4.0.txt
--rw-rw-rw-   0 root         (0) root         (0)     7048 2024-03-20 13:01:01.000000 demessaging-0.5.1/LICENSES/CC0-1.0.txt
--rw-rw-rw-   0 root         (0) root         (0)      399 2024-03-20 13:40:10.000000 demessaging-0.5.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    10026 2024-04-03 08:35:22.150555 demessaging-0.5.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6570 2024-03-21 08:53:42.000000 demessaging-0.5.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:35:22.126553 demessaging-0.5.1/demessaging/
--rw-rw-rw-   0 root         (0) root         (0)     3174 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/NetCDFDecoder.py
--rw-rw-rw-   0 root         (0) root         (0)     1002 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/PulsarConnection.py
--rw-rw-rw-   0 root         (0) root         (0)      545 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/PulsarMessageConstants.py
--rw-rw-rw-   0 root         (0) root         (0)      995 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/PulsarMessageConsumer.py
--rw-rw-rw-   0 root         (0) root         (0)      995 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/PulsarMessageProducer.py
--rw-rw-rw-   0 root         (0) root         (0)     1086 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      481 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2024-04-03 08:35:22.163557 demessaging-0.5.1/demessaging/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:35:22.128553 demessaging-0.5.1/demessaging/backend/
--rw-rw-rw-   0 root         (0) root         (0)     3243 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/backend/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10346 2024-04-03 07:35:06.000000 demessaging-0.5.1/demessaging/backend/class_.py
--rw-rw-rw-   0 root         (0) root         (0)     8919 2024-04-03 07:35:06.000000 demessaging-0.5.1/demessaging/backend/function.py
--rw-rw-rw-   0 root         (0) root         (0)    16124 2024-04-03 07:35:06.000000 demessaging-0.5.1/demessaging/backend/module.py
--rw-rw-rw-   0 root         (0) root         (0)     7683 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/backend/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    15359 2024-04-03 06:53:23.000000 demessaging-0.5.1/demessaging/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:35:22.138554 demessaging-0.5.1/demessaging/config/
--rw-rw-rw-   0 root         (0) root         (0)      686 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2812 2024-04-03 07:35:06.000000 demessaging-0.5.1/demessaging/config/api.py
--rw-rw-rw-   0 root         (0) root         (0)    10632 2024-04-03 07:35:06.000000 demessaging-0.5.1/demessaging/config/backend.py
--rw-rw-rw-   0 root         (0) root         (0)     4108 2024-04-03 07:35:06.000000 demessaging-0.5.1/demessaging/config/logging.py
--rw-rw-rw-   0 root         (0) root         (0)      823 2024-03-28 10:17:25.000000 demessaging-0.5.1/demessaging/config/logging.yaml
--rw-rw-rw-   0 root         (0) root         (0)     6238 2024-03-28 13:56:45.000000 demessaging-0.5.1/demessaging/config/messaging.py
--rw-rw-rw-   0 root         (0) root         (0)     2854 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/config/registry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:35:22.139554 demessaging-0.5.1/demessaging/messaging/
--rw-rw-rw-   0 root         (0) root         (0)      497 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/messaging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2944 2024-03-28 13:56:45.000000 demessaging-0.5.1/demessaging/messaging/connection.py
--rw-rw-rw-   0 root         (0) root         (0)     2435 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/messaging/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    18285 2024-04-03 07:35:06.000000 demessaging-0.5.1/demessaging/messaging/consumer.py
--rw-rw-rw-   0 root         (0) root         (0)     9907 2024-03-28 13:56:45.000000 demessaging-0.5.1/demessaging/messaging/producer.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 08:34:46.000000 demessaging-0.5.1/demessaging/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:35:22.139554 demessaging-0.5.1/demessaging/serializers/
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/serializers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1359 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/serializers/xarray.py
--rw-rw-rw-   0 root         (0) root         (0)     1235 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:35:22.140554 demessaging-0.5.1/demessaging/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2715 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/templates/class_.py.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1310 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/templates/function.py.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1500 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/templates/module.py.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     2287 2024-04-03 07:35:06.000000 demessaging-0.5.1/demessaging/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:35:22.140554 demessaging-0.5.1/demessaging/validators/
--rw-rw-rw-   0 root         (0) root         (0)      158 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/validators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4170 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/validators/xarray.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:35:22.141554 demessaging-0.5.1/demessaging.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10026 2024-04-03 08:35:22.000000 demessaging-0.5.1/demessaging.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1616 2024-04-03 08:35:22.000000 demessaging-0.5.1/demessaging.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 08:35:22.000000 demessaging-0.5.1/demessaging.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2024-04-03 08:35:22.000000 demessaging-0.5.1/demessaging.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 08:35:21.000000 demessaging-0.5.1/demessaging.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      661 2024-04-03 08:35:22.000000 demessaging-0.5.1/demessaging.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-04-03 08:35:22.000000 demessaging-0.5.1/demessaging.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     3904 2024-03-28 10:17:25.000000 demessaging-0.5.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 08:35:22.150555 demessaging-0.5.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      472 2024-03-20 13:40:10.000000 demessaging-0.5.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:35:22.141554 demessaging-0.5.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     6971 2024-04-03 07:35:06.000000 demessaging-0.5.1/tests/test_backend_class_.py
--rw-rw-rw-   0 root         (0) root         (0)    11385 2024-04-03 07:35:06.000000 demessaging-0.5.1/tests/test_backend_function.py
--rw-rw-rw-   0 root         (0) root         (0)    17479 2024-04-03 07:35:06.000000 demessaging-0.5.1/tests/test_backend_module.py
--rw-rw-rw-   0 root         (0) root         (0)     3533 2024-04-03 07:35:06.000000 demessaging-0.5.1/tests/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)     2233 2024-03-20 13:40:10.000000 demessaging-0.5.1/tests/test_logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:29:07.654363 demessaging-0.5.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:29:07.638363 demessaging-0.5.2/LICENSES/
+-rw-rw-rw-   0 root         (0) root         (0)    10280 2024-05-06 09:28:40.000000 demessaging-0.5.2/LICENSES/Apache-2.0.txt
+-rw-rw-rw-   0 root         (0) root         (0)    17023 2024-05-06 09:28:40.000000 demessaging-0.5.2/LICENSES/CC-BY-4.0.txt
+-rw-rw-rw-   0 root         (0) root         (0)     7048 2024-05-06 09:28:40.000000 demessaging-0.5.2/LICENSES/CC0-1.0.txt
+-rw-rw-rw-   0 root         (0) root         (0)      399 2024-05-06 09:28:40.000000 demessaging-0.5.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     9634 2024-05-06 09:29:07.654363 demessaging-0.5.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6012 2024-05-06 09:28:40.000000 demessaging-0.5.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:29:07.641363 demessaging-0.5.2/demessaging/
+-rw-rw-rw-   0 root         (0) root         (0)     3174 2024-05-06 09:28:40.000000 demessaging-0.5.2/demessaging/NetCDFDecoder.py
+-rw-rw-rw-   0 root         (0) root         (0)     1002 2024-05-06 09:28:40.000000 demessaging-0.5.2/demessaging/PulsarConnection.py
+-rw-rw-rw-   0 root         (0) root         (0)      545 2024-05-06 09:28:40.000000 demessaging-0.5.2/demessaging/PulsarMessageConstants.py
+-rw-rw-rw-   0 root         (0) root         (0)      995 2024-05-06 09:28:40.000000 demessaging-0.5.2/demessaging/PulsarMessageConsumer.py
+-rw-rw-rw-   0 root         (0) root         (0)      995 2024-05-06 09:28:40.000000 demessaging-0.5.2/demessaging/PulsarMessageProducer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1086 2024-05-06 09:28:40.000000 demessaging-0.5.2/demessaging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      481 2024-05-06 09:28:40.000000 demessaging-0.5.2/demessaging/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-06 09:29:07.654363 demessaging-0.5.2/demessaging/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:29:07.644363 demessaging-0.5.2/demessaging/backend/
+-rw-rw-rw-   0 root         (0) root         (0)     3243 2024-05-06 09:28:40.000000 demessaging-0.5.2/demessaging/backend/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10346 2024-05-06 09:28:40.000000 demessaging-0.5.2/demessaging/backend/class_.py
+-rw-rw-rw-   0 root         (0) root         (0)     8919 2024-05-06 09:28:40.000000 demessaging-0.5.2/demessaging/backend/function.py
+-rw-rw-rw-   0 root         (0) root         (0)    16124 2024-05-06 09:28:40.000000 demessaging-0.5.2/demessaging/backend/module.py
+-rw-rw-rw-   0 root         (0) root         (0)     7683 2024-05-06 09:28:40.000000 demessaging-0.5.2/demessaging/backend/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    15440 2024-05-06 09:28:40.000000 demessaging-0.5.2/demessaging/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:29:07.645363 demessaging-0.5.2/demessaging/config/
+-rw-rw-rw-   0 root         (0) root         (0)      686 2024-05-06 09:28:40.000000 demessaging-0.5.2/demessaging/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2812 2024-05-06 09:28:40.000000 demessaging-0.5.2/demessaging/config/api.py
+-rw-rw-rw-   0 root         (0) root         (0)    10632 2024-05-06 09:28:40.000000 demessaging-0.5.2/demessaging/config/backend.py
+-rw-rw-rw-   0 root         (0) root         (0)     4108 2024-05-06 09:28:40.000000 demessaging-0.5.2/demessaging/config/logging.py
+-rw-rw-rw-   0 root         (0) root         (0)      823 2024-05-06 09:28:40.000000 demessaging-0.5.2/demessaging/config/logging.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     6238 2024-05-06 09:28:40.000000 demessaging-0.5.2/demessaging/config/messaging.py
+-rw-rw-rw-   0 root         (0) root         (0)     2854 2024-05-06 09:28:40.000000 demessaging-0.5.2/demessaging/config/registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:29:07.646363 demessaging-0.5.2/demessaging/messaging/
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-06 09:28:40.000000 demessaging-0.5.2/demessaging/messaging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2944 2024-05-06 09:28:40.000000 demessaging-0.5.2/demessaging/messaging/connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     2435 2024-05-06 09:28:40.000000 demessaging-0.5.2/demessaging/messaging/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    18285 2024-05-06 09:28:40.000000 demessaging-0.5.2/demessaging/messaging/consumer.py
+-rw-rw-rw-   0 root         (0) root         (0)     9907 2024-05-06 09:28:40.000000 demessaging-0.5.2/demessaging/messaging/producer.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 09:28:40.000000 demessaging-0.5.2/demessaging/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:29:07.647363 demessaging-0.5.2/demessaging/serializers/
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-06 09:28:40.000000 demessaging-0.5.2/demessaging/serializers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2024-05-06 09:28:40.000000 demessaging-0.5.2/demessaging/serializers/xarray.py
+-rw-rw-rw-   0 root         (0) root         (0)     1235 2024-05-06 09:28:40.000000 demessaging-0.5.2/demessaging/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:29:07.647363 demessaging-0.5.2/demessaging/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2715 2024-05-06 09:28:40.000000 demessaging-0.5.2/demessaging/templates/class_.py.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1310 2024-05-06 09:28:40.000000 demessaging-0.5.2/demessaging/templates/function.py.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1500 2024-05-06 09:28:40.000000 demessaging-0.5.2/demessaging/templates/module.py.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     2287 2024-05-06 09:28:40.000000 demessaging-0.5.2/demessaging/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:29:07.648363 demessaging-0.5.2/demessaging/validators/
+-rw-rw-rw-   0 root         (0) root         (0)      158 2024-05-06 09:28:40.000000 demessaging-0.5.2/demessaging/validators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4170 2024-05-06 09:28:40.000000 demessaging-0.5.2/demessaging/validators/xarray.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:29:07.649363 demessaging-0.5.2/demessaging.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9634 2024-05-06 09:29:07.000000 demessaging-0.5.2/demessaging.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1616 2024-05-06 09:29:07.000000 demessaging-0.5.2/demessaging.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 09:29:07.000000 demessaging-0.5.2/demessaging.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2024-05-06 09:29:07.000000 demessaging-0.5.2/demessaging.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 09:29:07.000000 demessaging-0.5.2/demessaging.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      661 2024-05-06 09:29:07.000000 demessaging-0.5.2/demessaging.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-05-06 09:29:07.000000 demessaging-0.5.2/demessaging.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     4050 2024-05-06 09:28:40.000000 demessaging-0.5.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-06 09:29:07.654363 demessaging-0.5.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      472 2024-05-06 09:28:40.000000 demessaging-0.5.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:29:07.649363 demessaging-0.5.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     6971 2024-05-06 09:28:40.000000 demessaging-0.5.2/tests/test_backend_class_.py
+-rw-rw-rw-   0 root         (0) root         (0)    11385 2024-05-06 09:28:40.000000 demessaging-0.5.2/tests/test_backend_function.py
+-rw-rw-rw-   0 root         (0) root         (0)    17479 2024-05-06 09:28:40.000000 demessaging-0.5.2/tests/test_backend_module.py
+-rw-rw-rw-   0 root         (0) root         (0)     3533 2024-05-06 09:28:40.000000 demessaging-0.5.2/tests/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2233 2024-05-06 09:28:40.000000 demessaging-0.5.2/tests/test_logging.py
```

### Comparing `demessaging-0.5.1/LICENSES/Apache-2.0.txt` & `demessaging-0.5.2/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.1/LICENSES/CC-BY-4.0.txt` & `demessaging-0.5.2/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.1/LICENSES/CC0-1.0.txt` & `demessaging-0.5.2/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.1/PKG-INFO` & `demessaging-0.5.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 Metadata-Version: 2.1
 Name: demessaging
-Version: 0.5.1
+Version: 0.5.2
 Summary: python module wrapper for the data analytics software framework DASF
 Author: Mike Sips, Doris Dransch
 Author-email: Daniel Eggert <daniel.eggert@gfz-potsdam.de>, "Philipp S. Sommer" <philipp.sommer@hereon.de>
 Maintainer-email: "Philipp S. Sommer" <philipp.sommer@hereon.de>
 License: Apache-2.0
-Project-URL: Homepage, https://git.geomar.de/digital-earth/dasf/dasf-messaging-python
-Project-URL: Documentation, https://digital-earth.pages.geomar.de/dasf/dasf-messaging-python/
-Project-URL: Source, https://git.geomar.de/digital-earth/dasf/dasf-messaging-python
-Project-URL: Tracker, https://git.geomar.de/digital-earth/dasf/dasf-messaging-python/issues/
+Project-URL: Homepage, https://codebase.helmholtz.cloud/dasf/dasf-messaging-python
+Project-URL: Documentation, https://dasf.readthedocs.io/en/latest/
+Project-URL: Source, https://codebase.helmholtz.cloud/dasf/dasf-messaging-python
+Project-URL: Tracker, https://codebase.helmholtz.cloud/dasf/dasf-messaging-python/issues/
 Keywords: digital-earth,dasf,pulsar,gfz,hzg,hereon,hgf,helmholtz,remote procedure call,rpc,django,python,websocket
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSES/Apache-2.0.txt
 License-File: LICENSES/CC-BY-4.0.txt
 License-File: LICENSES/CC0-1.0.txt
 Requires-Dist: websocket-client<1.8,>=1.5
 Requires-Dist: docstring_parser<0.16
 Requires-Dist: pydantic<3.0,>=2.2
@@ -75,54 +79,47 @@
 SPDX-FileCopyrightText: 2019-2024 Helmholtz Centre Potsdam GFZ German Research Centre for Geosciences
 SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht GmbH
 SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
 
 SPDX-License-Identifier: CC-BY-4.0
 -->
 
-![DASF Logo](https://git.geomar.de/digital-earth/dasf/dasf-messaging-python/-/raw/master/docs/_static/dasf_logo.svg)
+![DASF Logo](https://codebase.helmholtz.cloud/dasf/dasf-messaging-python/-/raw/master/docs/_static/dasf_logo.svg)
 
 # Data Analytics Software Framework
 
-[![CI](https://git.geomar.de/digital-earth/dasf/dasf-messaging-python/badges/master/pipeline.svg)](https://git.geomar.de/digital-earth/dasf/dasf-messaging-python/-/pipelines?page=1&scope=all&ref=master)
-[![Code coverage](https://git.geomar.de/digital-earth/dasf/dasf-messaging-python/badges/master/coverage.svg)](https://git.geomar.de/digital-earth/dasf/dasf-messaging-python/-/graphs/master/charts)
-[![Latest Release](https://git.geomar.de/digital-earth/dasf/dasf-messaging-python/-/badges/release.svg)](https://git.geomar.de/digital-earth/dasf/dasf-messaging-python)
+[![CI](https://codebase.helmholtz.cloud/dasf/dasf-messaging-python/badges/master/pipeline.svg)](https://codebase.helmholtz.cloud/dasf/dasf-messaging-python/-/pipelines?page=1&scope=all&ref=master)
+[![Code coverage](https://codebase.helmholtz.cloud/dasf/dasf-messaging-python/badges/master/coverage.svg)](https://codebase.helmholtz.cloud/dasf/dasf-messaging-python/-/graphs/master/charts)
+[![Docs](https://readthedocs.org/projects/dasf-messaging-python/badge/?version=latest)](https://dasf.readthedocs.io/en/latest/)
+[![Latest Release](https://codebase.helmholtz.cloud/dasf/dasf-messaging-python/-/badges/release.svg)](https://codebase.helmholtz.cloud/dasf/dasf-messaging-python)
 [![PyPI version](https://img.shields.io/pypi/v/demessaging.svg)](https://pypi.python.org/pypi/demessaging/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![PEP8](https://img.shields.io/badge/code%20style-pep8-orange.svg)](https://www.python.org/dev/peps/pep-0008/)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
-[![REUSE status](https://api.reuse.software/badge/git.geomar.de/digital-earth/dasf/dasf-messaging-python)](https://api.reuse.software/info/git.geomar.de/digital-earth/dasf/dasf-messaging-python)
+[![REUSE status](https://api.reuse.software/badge/codebase.helmholtz.cloud/dasf/dasf-messaging-python)](https://api.reuse.software/info/codebase.helmholtz.cloud/dasf/dasf-messaging-python)
 [![DOI](https://img.shields.io/badge/DOI-10.5880%2FGFZ.1.4.2021.005-blue)](https://doi.org/10.5880/GFZ.1.4.2021.005)
 [![JOSS](https://joss.theoj.org/papers/e8022c832c1bb6e879b89508a83fa75e/status.svg)](https://joss.theoj.org/papers/e8022c832c1bb6e879b89508a83fa75e)
 
 python module wrapper for the data analytics software framework DASF
 
 ## Abstract
 
-`DASF: Messaging Python` is part of the Data Analytics Software Framework (DASF, https://git.geomar.de/digital-earth/dasf),
+`DASF: Messaging Python` is part of the Data Analytics Software Framework (DASF, https://codebase.helmholtz.cloud/dasf),
 developed at the GFZ German Research Centre for Geosciences (https://www.gfz-potsdam.de).
 It is funded by the Initiative and Networking Fund of the Helmholtz Association through the Digital Earth project
 (https://www.digitalearth-hgf.de/).
 
-`DASF: Messaging Python` is a RPC (remote procedure call) wrapper library for the python programming language. As part of the data analytics software framework DASF, it implements the DASF RPC messaging protocol. This message broker based RPC implementation supports the integration of algorithms and methods implemented in python in a distributed environment. It utilizes pydantic (https://pydantic-docs.helpmanual.io/) for data and model validation using python type annotations. DASF distributes messages via a central message broker. Currently we support a self-developed message broker called dasf-broker-django, as well as an ‘off-the-shelf’ solution called Apache Pulsar. (also see: [Message Broker](https://digital-earth.pages.geomar.de/dasf/dasf-messaging-python/developers/messaging.html#messagebroker))
+`DASF: Messaging Python` is a RPC (remote procedure call) wrapper library for the python programming language. As part of the data analytics software framework DASF, it implements the DASF RPC messaging protocol. This message broker based RPC implementation supports the integration of algorithms and methods implemented in python in a distributed environment. It utilizes pydantic (https://pydantic-docs.helpmanual.io/) for data and model validation using python type annotations. DASF distributes messages via a central message broker. Currently we support a self-developed message broker called dasf-broker-django, as well as an ‘off-the-shelf’ solution called Apache Pulsar. (also see: [Message Broker](https://dasf.readthedocs.io/en/latest/developers/messaging.html#messagebroker))
 
 ---
 
-## Service Desk
-
-For everyone without a Geomar Gitlab account, we setup the Service Desk feature for this repository.
-It lets you communicate with the developers via a repository specific eMail address. Each request will be tracked via the Gitlab issuse tracker.
-In order to send a follow-up message, simply reply to the corresponding notification eMail.
-
-eMail: [gitlab+digital-earth-dasf-dasf-messaging-python-1576-issue-@git-issues.geomar.de](mailto:gitlab+digital-earth-dasf-dasf-messaging-python-1576-issue-@git-issues.geomar.de)
-
 ## Documentation
 
-see: https://digital-earth.pages.geomar.de/dasf/dasf-messaging-python/
+see: https://dasf.readthedocs.io/en/latest/
 
 
 
 ## Installation
 
 Install this package in a dedicated python environment via
 
@@ -132,41 +129,41 @@
 pip install demessaging
 ```
 
 To use this in a development setup, clone the [source code][source code] from
 gitlab, start the development server and make your changes::
 
 ```bash
-git clone https://git.geomar.de/digital-earth/dasf/dasf-messaging-python
+git clone https://codebase.helmholtz.cloud/dasf/dasf-messaging-python
 cd dasf-messaging-python
 python -m venv venv
 source venv/bin/activate
 make dev-install
 ```
 
 More detailed installation instructions my be found in the [docs][docs].
 
 
-[source code]: https://git.geomar.de/digital-earth/dasf/dasf-messaging-python
-[docs]: https://digital-earth.pages.geomar.de/dasf/dasf-messaging-python/installation.html
+[source code]: https://codebase.helmholtz.cloud/dasf/dasf-messaging-python
+[docs]: https://dasf.readthedocs.io/en/latest/installation.html
 
 ## Technical note
 
 This package has been generated from the template
 https://codebase.helmholtz.cloud/hcdc/software-templates/python-package-template.git.
 
 See the template repository for instructions on how to update the skeleton for
 this package.
 
 ### **Source Code Examples**
-see: https://git.geomar.de/digital-earth/dasf/dasf-messaging-python/-/blob/master/ExampleMessageConsumer.py
+see: https://codebase.helmholtz.cloud/dasf/dasf-messaging-python/-/blob/master/ExampleMessageConsumer.py
 
 - generate the counterpart via `python ExampleMessageConsumer.py generate > ExampleMessageProducerGen.py`
 - call the consumer module via the generated producer,
-see https://git.geomar.de/digital-earth/dasf/dasf-messaging-python/-/blob/master/ExampleMessageProducer.py
+see https://codebase.helmholtz.cloud/dasf/dasf-messaging-python/-/blob/master/ExampleMessageProducer.py
 
 
 ## Recommended Software Citation
 
 `Eggert, Daniel; Sommer, Philipp; Dransch, Doris (2021): DASF: Messaging Python: A python RPC wrapper for the data analytics software framework. GFZ Data Services. https://doi.org/10.5880/GFZ.1.4.2021.005`
 
 
@@ -191,15 +188,15 @@
 ### License management
 
 License management is handled with [``reuse``](https://reuse.readthedocs.io/).
 If you have any questions on this, please have a look into the
 [contributing guide][contributing] or contact the maintainers of
 `dasf-messaging-python`.
 
-[contributing]: https://digital-earth.pages.geomar.de/dasf/dasf-messaging-python/contributing.html
+[contributing]: https://dasf.readthedocs.io/en/latest/contributing.html
 
 
 ## Contact
 Philipp S. Sommer
 eMail: <philipp.sommer@hereon.de>
```

### Comparing `demessaging-0.5.1/README.md` & `demessaging-0.5.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -2,54 +2,47 @@
 SPDX-FileCopyrightText: 2019-2024 Helmholtz Centre Potsdam GFZ German Research Centre for Geosciences
 SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht GmbH
 SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
 
 SPDX-License-Identifier: CC-BY-4.0
 -->
 
-![DASF Logo](https://git.geomar.de/digital-earth/dasf/dasf-messaging-python/-/raw/master/docs/_static/dasf_logo.svg)
+![DASF Logo](https://codebase.helmholtz.cloud/dasf/dasf-messaging-python/-/raw/master/docs/_static/dasf_logo.svg)
 
 # Data Analytics Software Framework
 
-[![CI](https://git.geomar.de/digital-earth/dasf/dasf-messaging-python/badges/master/pipeline.svg)](https://git.geomar.de/digital-earth/dasf/dasf-messaging-python/-/pipelines?page=1&scope=all&ref=master)
-[![Code coverage](https://git.geomar.de/digital-earth/dasf/dasf-messaging-python/badges/master/coverage.svg)](https://git.geomar.de/digital-earth/dasf/dasf-messaging-python/-/graphs/master/charts)
-[![Latest Release](https://git.geomar.de/digital-earth/dasf/dasf-messaging-python/-/badges/release.svg)](https://git.geomar.de/digital-earth/dasf/dasf-messaging-python)
+[![CI](https://codebase.helmholtz.cloud/dasf/dasf-messaging-python/badges/master/pipeline.svg)](https://codebase.helmholtz.cloud/dasf/dasf-messaging-python/-/pipelines?page=1&scope=all&ref=master)
+[![Code coverage](https://codebase.helmholtz.cloud/dasf/dasf-messaging-python/badges/master/coverage.svg)](https://codebase.helmholtz.cloud/dasf/dasf-messaging-python/-/graphs/master/charts)
+[![Docs](https://readthedocs.org/projects/dasf-messaging-python/badge/?version=latest)](https://dasf.readthedocs.io/en/latest/)
+[![Latest Release](https://codebase.helmholtz.cloud/dasf/dasf-messaging-python/-/badges/release.svg)](https://codebase.helmholtz.cloud/dasf/dasf-messaging-python)
 [![PyPI version](https://img.shields.io/pypi/v/demessaging.svg)](https://pypi.python.org/pypi/demessaging/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![PEP8](https://img.shields.io/badge/code%20style-pep8-orange.svg)](https://www.python.org/dev/peps/pep-0008/)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
-[![REUSE status](https://api.reuse.software/badge/git.geomar.de/digital-earth/dasf/dasf-messaging-python)](https://api.reuse.software/info/git.geomar.de/digital-earth/dasf/dasf-messaging-python)
+[![REUSE status](https://api.reuse.software/badge/codebase.helmholtz.cloud/dasf/dasf-messaging-python)](https://api.reuse.software/info/codebase.helmholtz.cloud/dasf/dasf-messaging-python)
 [![DOI](https://img.shields.io/badge/DOI-10.5880%2FGFZ.1.4.2021.005-blue)](https://doi.org/10.5880/GFZ.1.4.2021.005)
 [![JOSS](https://joss.theoj.org/papers/e8022c832c1bb6e879b89508a83fa75e/status.svg)](https://joss.theoj.org/papers/e8022c832c1bb6e879b89508a83fa75e)
 
 python module wrapper for the data analytics software framework DASF
 
 ## Abstract
 
-`DASF: Messaging Python` is part of the Data Analytics Software Framework (DASF, https://git.geomar.de/digital-earth/dasf),
+`DASF: Messaging Python` is part of the Data Analytics Software Framework (DASF, https://codebase.helmholtz.cloud/dasf),
 developed at the GFZ German Research Centre for Geosciences (https://www.gfz-potsdam.de).
 It is funded by the Initiative and Networking Fund of the Helmholtz Association through the Digital Earth project
 (https://www.digitalearth-hgf.de/).
 
-`DASF: Messaging Python` is a RPC (remote procedure call) wrapper library for the python programming language. As part of the data analytics software framework DASF, it implements the DASF RPC messaging protocol. This message broker based RPC implementation supports the integration of algorithms and methods implemented in python in a distributed environment. It utilizes pydantic (https://pydantic-docs.helpmanual.io/) for data and model validation using python type annotations. DASF distributes messages via a central message broker. Currently we support a self-developed message broker called dasf-broker-django, as well as an ‘off-the-shelf’ solution called Apache Pulsar. (also see: [Message Broker](https://digital-earth.pages.geomar.de/dasf/dasf-messaging-python/developers/messaging.html#messagebroker))
+`DASF: Messaging Python` is a RPC (remote procedure call) wrapper library for the python programming language. As part of the data analytics software framework DASF, it implements the DASF RPC messaging protocol. This message broker based RPC implementation supports the integration of algorithms and methods implemented in python in a distributed environment. It utilizes pydantic (https://pydantic-docs.helpmanual.io/) for data and model validation using python type annotations. DASF distributes messages via a central message broker. Currently we support a self-developed message broker called dasf-broker-django, as well as an ‘off-the-shelf’ solution called Apache Pulsar. (also see: [Message Broker](https://dasf.readthedocs.io/en/latest/developers/messaging.html#messagebroker))
 
 ---
 
-## Service Desk
-
-For everyone without a Geomar Gitlab account, we setup the Service Desk feature for this repository.
-It lets you communicate with the developers via a repository specific eMail address. Each request will be tracked via the Gitlab issuse tracker.
-In order to send a follow-up message, simply reply to the corresponding notification eMail.
-
-eMail: [gitlab+digital-earth-dasf-dasf-messaging-python-1576-issue-@git-issues.geomar.de](mailto:gitlab+digital-earth-dasf-dasf-messaging-python-1576-issue-@git-issues.geomar.de)
-
 ## Documentation
 
-see: https://digital-earth.pages.geomar.de/dasf/dasf-messaging-python/
+see: https://dasf.readthedocs.io/en/latest/
 
 
 
 ## Installation
 
 Install this package in a dedicated python environment via
 
@@ -59,41 +52,41 @@
 pip install demessaging
 ```
 
 To use this in a development setup, clone the [source code][source code] from
 gitlab, start the development server and make your changes::
 
 ```bash
-git clone https://git.geomar.de/digital-earth/dasf/dasf-messaging-python
+git clone https://codebase.helmholtz.cloud/dasf/dasf-messaging-python
 cd dasf-messaging-python
 python -m venv venv
 source venv/bin/activate
 make dev-install
 ```
 
 More detailed installation instructions my be found in the [docs][docs].
 
 
-[source code]: https://git.geomar.de/digital-earth/dasf/dasf-messaging-python
-[docs]: https://digital-earth.pages.geomar.de/dasf/dasf-messaging-python/installation.html
+[source code]: https://codebase.helmholtz.cloud/dasf/dasf-messaging-python
+[docs]: https://dasf.readthedocs.io/en/latest/installation.html
 
 ## Technical note
 
 This package has been generated from the template
 https://codebase.helmholtz.cloud/hcdc/software-templates/python-package-template.git.
 
 See the template repository for instructions on how to update the skeleton for
 this package.
 
 ### **Source Code Examples**
-see: https://git.geomar.de/digital-earth/dasf/dasf-messaging-python/-/blob/master/ExampleMessageConsumer.py
+see: https://codebase.helmholtz.cloud/dasf/dasf-messaging-python/-/blob/master/ExampleMessageConsumer.py
 
 - generate the counterpart via `python ExampleMessageConsumer.py generate > ExampleMessageProducerGen.py`
 - call the consumer module via the generated producer,
-see https://git.geomar.de/digital-earth/dasf/dasf-messaging-python/-/blob/master/ExampleMessageProducer.py
+see https://codebase.helmholtz.cloud/dasf/dasf-messaging-python/-/blob/master/ExampleMessageProducer.py
 
 
 ## Recommended Software Citation
 
 `Eggert, Daniel; Sommer, Philipp; Dransch, Doris (2021): DASF: Messaging Python: A python RPC wrapper for the data analytics software framework. GFZ Data Services. https://doi.org/10.5880/GFZ.1.4.2021.005`
 
 
@@ -118,15 +111,15 @@
 ### License management
 
 License management is handled with [``reuse``](https://reuse.readthedocs.io/).
 If you have any questions on this, please have a look into the
 [contributing guide][contributing] or contact the maintainers of
 `dasf-messaging-python`.
 
-[contributing]: https://digital-earth.pages.geomar.de/dasf/dasf-messaging-python/contributing.html
+[contributing]: https://dasf.readthedocs.io/en/latest/contributing.html
 
 
 ## Contact
 Philipp S. Sommer
 eMail: <philipp.sommer@hereon.de>
```

### Comparing `demessaging-0.5.1/demessaging/NetCDFDecoder.py` & `demessaging-0.5.2/demessaging/NetCDFDecoder.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.1/demessaging/PulsarConnection.py` & `demessaging-0.5.2/demessaging/PulsarConnection.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.1/demessaging/PulsarMessageConstants.py` & `demessaging-0.5.2/demessaging/PulsarMessageConstants.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.1/demessaging/PulsarMessageConsumer.py` & `demessaging-0.5.2/demessaging/PulsarMessageConsumer.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.1/demessaging/PulsarMessageProducer.py` & `demessaging-0.5.2/demessaging/PulsarMessageProducer.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.1/demessaging/__init__.py` & `demessaging-0.5.2/demessaging/__init__.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.1/demessaging/backend/__init__.py` & `demessaging-0.5.2/demessaging/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.1/demessaging/backend/class_.py` & `demessaging-0.5.2/demessaging/backend/class_.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.1/demessaging/backend/function.py` & `demessaging-0.5.2/demessaging/backend/function.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.1/demessaging/backend/module.py` & `demessaging-0.5.2/demessaging/backend/module.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.1/demessaging/backend/utils.py` & `demessaging-0.5.2/demessaging/backend/utils.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.1/demessaging/cli.py` & `demessaging-0.5.2/demessaging/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 """Command-line options for the backend module."""
 from __future__ import annotations
 
 import argparse
 import json
 import logging
 from itertools import chain
+from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, Optional, Tuple, Type
 
 import yaml
 
 from demessaging.config import (
     LoggingConfig,
     ModuleConfig,
@@ -336,34 +337,37 @@
     )
 
     # logging config
     logging_group.add_argument(
         "--log-config",
         default=log_config.config_file,
         dest="log_config.config_file",
+        type=Path,
         help=desc("config_file", LoggingConfig),
     )
 
     logging_group.add_argument(
         "--log-level",
         default=log_config.level,
         dest="log_config.level",
         help=desc("level", LoggingConfig),
+        type=int,
         choices=[
             logging.DEBUG,
             logging.INFO,
             logging.WARNING,
             logging.ERROR,
             logging.CRITICAL,
         ],
     )
 
     logging_group.add_argument(
         "--log-file",
         default=log_config.logfile,
+        type=Path,
         dest="log_config.logfile",
         help=desc("logfile", LoggingConfig),
     )
 
     logging_group.add_argument(
         "--merge-log-config",
         action="store_true",
```

### Comparing `demessaging-0.5.1/demessaging/config/__init__.py` & `demessaging-0.5.2/demessaging/config/__init__.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.1/demessaging/config/api.py` & `demessaging-0.5.2/demessaging/config/api.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.1/demessaging/config/backend.py` & `demessaging-0.5.2/demessaging/config/backend.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.1/demessaging/config/logging.py` & `demessaging-0.5.2/demessaging/config/logging.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.1/demessaging/config/logging.yaml` & `demessaging-0.5.2/demessaging/config/logging.yaml`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.1/demessaging/config/messaging.py` & `demessaging-0.5.2/demessaging/config/messaging.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.1/demessaging/config/registry.py` & `demessaging-0.5.2/demessaging/config/registry.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.1/demessaging/messaging/connection.py` & `demessaging-0.5.2/demessaging/messaging/connection.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.1/demessaging/messaging/constants.py` & `demessaging-0.5.2/demessaging/messaging/constants.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.1/demessaging/messaging/consumer.py` & `demessaging-0.5.2/demessaging/messaging/consumer.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.1/demessaging/messaging/producer.py` & `demessaging-0.5.2/demessaging/messaging/producer.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.1/demessaging/serializers/xarray.py` & `demessaging-0.5.2/demessaging/serializers/xarray.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.1/demessaging/template.py` & `demessaging-0.5.2/demessaging/template.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.1/demessaging/templates/class_.py.jinja2` & `demessaging-0.5.2/demessaging/templates/class_.py.jinja2`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.1/demessaging/templates/function.py.jinja2` & `demessaging-0.5.2/demessaging/templates/function.py.jinja2`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.1/demessaging/templates/module.py.jinja2` & `demessaging-0.5.2/demessaging/templates/module.py.jinja2`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.1/demessaging/utils.py` & `demessaging-0.5.2/demessaging/utils.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.1/demessaging/validators/xarray.py` & `demessaging-0.5.2/demessaging/validators/xarray.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.1/demessaging.egg-info/PKG-INFO` & `demessaging-0.5.2/demessaging.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 Metadata-Version: 2.1
 Name: demessaging
-Version: 0.5.1
+Version: 0.5.2
 Summary: python module wrapper for the data analytics software framework DASF
 Author: Mike Sips, Doris Dransch
 Author-email: Daniel Eggert <daniel.eggert@gfz-potsdam.de>, "Philipp S. Sommer" <philipp.sommer@hereon.de>
 Maintainer-email: "Philipp S. Sommer" <philipp.sommer@hereon.de>
 License: Apache-2.0
-Project-URL: Homepage, https://git.geomar.de/digital-earth/dasf/dasf-messaging-python
-Project-URL: Documentation, https://digital-earth.pages.geomar.de/dasf/dasf-messaging-python/
-Project-URL: Source, https://git.geomar.de/digital-earth/dasf/dasf-messaging-python
-Project-URL: Tracker, https://git.geomar.de/digital-earth/dasf/dasf-messaging-python/issues/
+Project-URL: Homepage, https://codebase.helmholtz.cloud/dasf/dasf-messaging-python
+Project-URL: Documentation, https://dasf.readthedocs.io/en/latest/
+Project-URL: Source, https://codebase.helmholtz.cloud/dasf/dasf-messaging-python
+Project-URL: Tracker, https://codebase.helmholtz.cloud/dasf/dasf-messaging-python/issues/
 Keywords: digital-earth,dasf,pulsar,gfz,hzg,hereon,hgf,helmholtz,remote procedure call,rpc,django,python,websocket
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSES/Apache-2.0.txt
 License-File: LICENSES/CC-BY-4.0.txt
 License-File: LICENSES/CC0-1.0.txt
 Requires-Dist: websocket-client<1.8,>=1.5
 Requires-Dist: docstring_parser<0.16
 Requires-Dist: pydantic<3.0,>=2.2
@@ -75,54 +79,47 @@
 SPDX-FileCopyrightText: 2019-2024 Helmholtz Centre Potsdam GFZ German Research Centre for Geosciences
 SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht GmbH
 SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
 
 SPDX-License-Identifier: CC-BY-4.0
 -->
 
-![DASF Logo](https://git.geomar.de/digital-earth/dasf/dasf-messaging-python/-/raw/master/docs/_static/dasf_logo.svg)
+![DASF Logo](https://codebase.helmholtz.cloud/dasf/dasf-messaging-python/-/raw/master/docs/_static/dasf_logo.svg)
 
 # Data Analytics Software Framework
 
-[![CI](https://git.geomar.de/digital-earth/dasf/dasf-messaging-python/badges/master/pipeline.svg)](https://git.geomar.de/digital-earth/dasf/dasf-messaging-python/-/pipelines?page=1&scope=all&ref=master)
-[![Code coverage](https://git.geomar.de/digital-earth/dasf/dasf-messaging-python/badges/master/coverage.svg)](https://git.geomar.de/digital-earth/dasf/dasf-messaging-python/-/graphs/master/charts)
-[![Latest Release](https://git.geomar.de/digital-earth/dasf/dasf-messaging-python/-/badges/release.svg)](https://git.geomar.de/digital-earth/dasf/dasf-messaging-python)
+[![CI](https://codebase.helmholtz.cloud/dasf/dasf-messaging-python/badges/master/pipeline.svg)](https://codebase.helmholtz.cloud/dasf/dasf-messaging-python/-/pipelines?page=1&scope=all&ref=master)
+[![Code coverage](https://codebase.helmholtz.cloud/dasf/dasf-messaging-python/badges/master/coverage.svg)](https://codebase.helmholtz.cloud/dasf/dasf-messaging-python/-/graphs/master/charts)
+[![Docs](https://readthedocs.org/projects/dasf-messaging-python/badge/?version=latest)](https://dasf.readthedocs.io/en/latest/)
+[![Latest Release](https://codebase.helmholtz.cloud/dasf/dasf-messaging-python/-/badges/release.svg)](https://codebase.helmholtz.cloud/dasf/dasf-messaging-python)
 [![PyPI version](https://img.shields.io/pypi/v/demessaging.svg)](https://pypi.python.org/pypi/demessaging/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![PEP8](https://img.shields.io/badge/code%20style-pep8-orange.svg)](https://www.python.org/dev/peps/pep-0008/)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
-[![REUSE status](https://api.reuse.software/badge/git.geomar.de/digital-earth/dasf/dasf-messaging-python)](https://api.reuse.software/info/git.geomar.de/digital-earth/dasf/dasf-messaging-python)
+[![REUSE status](https://api.reuse.software/badge/codebase.helmholtz.cloud/dasf/dasf-messaging-python)](https://api.reuse.software/info/codebase.helmholtz.cloud/dasf/dasf-messaging-python)
 [![DOI](https://img.shields.io/badge/DOI-10.5880%2FGFZ.1.4.2021.005-blue)](https://doi.org/10.5880/GFZ.1.4.2021.005)
 [![JOSS](https://joss.theoj.org/papers/e8022c832c1bb6e879b89508a83fa75e/status.svg)](https://joss.theoj.org/papers/e8022c832c1bb6e879b89508a83fa75e)
 
 python module wrapper for the data analytics software framework DASF
 
 ## Abstract
 
-`DASF: Messaging Python` is part of the Data Analytics Software Framework (DASF, https://git.geomar.de/digital-earth/dasf),
+`DASF: Messaging Python` is part of the Data Analytics Software Framework (DASF, https://codebase.helmholtz.cloud/dasf),
 developed at the GFZ German Research Centre for Geosciences (https://www.gfz-potsdam.de).
 It is funded by the Initiative and Networking Fund of the Helmholtz Association through the Digital Earth project
 (https://www.digitalearth-hgf.de/).
 
-`DASF: Messaging Python` is a RPC (remote procedure call) wrapper library for the python programming language. As part of the data analytics software framework DASF, it implements the DASF RPC messaging protocol. This message broker based RPC implementation supports the integration of algorithms and methods implemented in python in a distributed environment. It utilizes pydantic (https://pydantic-docs.helpmanual.io/) for data and model validation using python type annotations. DASF distributes messages via a central message broker. Currently we support a self-developed message broker called dasf-broker-django, as well as an ‘off-the-shelf’ solution called Apache Pulsar. (also see: [Message Broker](https://digital-earth.pages.geomar.de/dasf/dasf-messaging-python/developers/messaging.html#messagebroker))
+`DASF: Messaging Python` is a RPC (remote procedure call) wrapper library for the python programming language. As part of the data analytics software framework DASF, it implements the DASF RPC messaging protocol. This message broker based RPC implementation supports the integration of algorithms and methods implemented in python in a distributed environment. It utilizes pydantic (https://pydantic-docs.helpmanual.io/) for data and model validation using python type annotations. DASF distributes messages via a central message broker. Currently we support a self-developed message broker called dasf-broker-django, as well as an ‘off-the-shelf’ solution called Apache Pulsar. (also see: [Message Broker](https://dasf.readthedocs.io/en/latest/developers/messaging.html#messagebroker))
 
 ---
 
-## Service Desk
-
-For everyone without a Geomar Gitlab account, we setup the Service Desk feature for this repository.
-It lets you communicate with the developers via a repository specific eMail address. Each request will be tracked via the Gitlab issuse tracker.
-In order to send a follow-up message, simply reply to the corresponding notification eMail.
-
-eMail: [gitlab+digital-earth-dasf-dasf-messaging-python-1576-issue-@git-issues.geomar.de](mailto:gitlab+digital-earth-dasf-dasf-messaging-python-1576-issue-@git-issues.geomar.de)
-
 ## Documentation
 
-see: https://digital-earth.pages.geomar.de/dasf/dasf-messaging-python/
+see: https://dasf.readthedocs.io/en/latest/
 
 
 
 ## Installation
 
 Install this package in a dedicated python environment via
 
@@ -132,41 +129,41 @@
 pip install demessaging
 ```
 
 To use this in a development setup, clone the [source code][source code] from
 gitlab, start the development server and make your changes::
 
 ```bash
-git clone https://git.geomar.de/digital-earth/dasf/dasf-messaging-python
+git clone https://codebase.helmholtz.cloud/dasf/dasf-messaging-python
 cd dasf-messaging-python
 python -m venv venv
 source venv/bin/activate
 make dev-install
 ```
 
 More detailed installation instructions my be found in the [docs][docs].
 
 
-[source code]: https://git.geomar.de/digital-earth/dasf/dasf-messaging-python
-[docs]: https://digital-earth.pages.geomar.de/dasf/dasf-messaging-python/installation.html
+[source code]: https://codebase.helmholtz.cloud/dasf/dasf-messaging-python
+[docs]: https://dasf.readthedocs.io/en/latest/installation.html
 
 ## Technical note
 
 This package has been generated from the template
 https://codebase.helmholtz.cloud/hcdc/software-templates/python-package-template.git.
 
 See the template repository for instructions on how to update the skeleton for
 this package.
 
 ### **Source Code Examples**
-see: https://git.geomar.de/digital-earth/dasf/dasf-messaging-python/-/blob/master/ExampleMessageConsumer.py
+see: https://codebase.helmholtz.cloud/dasf/dasf-messaging-python/-/blob/master/ExampleMessageConsumer.py
 
 - generate the counterpart via `python ExampleMessageConsumer.py generate > ExampleMessageProducerGen.py`
 - call the consumer module via the generated producer,
-see https://git.geomar.de/digital-earth/dasf/dasf-messaging-python/-/blob/master/ExampleMessageProducer.py
+see https://codebase.helmholtz.cloud/dasf/dasf-messaging-python/-/blob/master/ExampleMessageProducer.py
 
 
 ## Recommended Software Citation
 
 `Eggert, Daniel; Sommer, Philipp; Dransch, Doris (2021): DASF: Messaging Python: A python RPC wrapper for the data analytics software framework. GFZ Data Services. https://doi.org/10.5880/GFZ.1.4.2021.005`
 
 
@@ -191,15 +188,15 @@
 ### License management
 
 License management is handled with [``reuse``](https://reuse.readthedocs.io/).
 If you have any questions on this, please have a look into the
 [contributing guide][contributing] or contact the maintainers of
 `dasf-messaging-python`.
 
-[contributing]: https://digital-earth.pages.geomar.de/dasf/dasf-messaging-python/contributing.html
+[contributing]: https://dasf.readthedocs.io/en/latest/contributing.html
 
 
 ## Contact
 Philipp S. Sommer
 eMail: <philipp.sommer@hereon.de>
```

### Comparing `demessaging-0.5.1/demessaging.egg-info/SOURCES.txt` & `demessaging-0.5.2/demessaging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.1/demessaging.egg-info/requires.txt` & `demessaging-0.5.2/demessaging.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.1/pyproject.toml` & `demessaging-0.5.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -44,37 +44,41 @@
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Typing :: Typed",
 ]
 
-requires-python = '>= 3.9'
+requires-python = '>= 3.7'
 dependencies = [
     # add your dependencies here
     "websocket-client>=1.5,<1.8",
     "docstring_parser<0.16",
     "pydantic>=2.2,<3.0",
     "pydantic-settings",
     "typing_extensions",
     "jinja2==3.1.2",
     "deprogressapi>=0.3.0",
     "PyYAML>=4.2b",
 ]
 
 [project.urls]
-Homepage = 'https://git.geomar.de/digital-earth/dasf/dasf-messaging-python'
-Documentation = "https://digital-earth.pages.geomar.de/dasf/dasf-messaging-python/"
-Source = "https://git.geomar.de/digital-earth/dasf/dasf-messaging-python"
-Tracker = "https://git.geomar.de/digital-earth/dasf/dasf-messaging-python/issues/"
+Homepage = 'https://codebase.helmholtz.cloud/dasf/dasf-messaging-python'
+Documentation = "https://dasf.readthedocs.io/en/latest/"
+Source = "https://codebase.helmholtz.cloud/dasf/dasf-messaging-python"
+Tracker = "https://codebase.helmholtz.cloud/dasf/dasf-messaging-python/issues/"
 
 
 [project.optional-dependencies]
 
 backend = [
     "isort>=5.10.1",
     "black>=22.3.0",
```

### Comparing `demessaging-0.5.1/tests/test_backend_class_.py` & `demessaging-0.5.2/tests/test_backend_class_.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.1/tests/test_backend_function.py` & `demessaging-0.5.2/tests/test_backend_function.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.1/tests/test_backend_module.py` & `demessaging-0.5.2/tests/test_backend_module.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.1/tests/test_config.py` & `demessaging-0.5.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.1/tests/test_logging.py` & `demessaging-0.5.2/tests/test_logging.py`

 * *Files identical despite different names*

