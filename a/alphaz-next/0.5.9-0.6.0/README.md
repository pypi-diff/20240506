# Comparing `tmp/alphaz-next-0.5.9.tar.gz` & `tmp/alphaz-next-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphaz-next-0.5.9.tar", last modified: Fri Apr 26 10:35:01 2024, max compression
+gzip compressed data, was "alphaz-next-0.6.0.tar", last modified: Mon May  6 08:49:33 2024, max compression
```

## Comparing `alphaz-next-0.5.9.tar` & `alphaz-next-0.6.0.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:35:01.518655 alphaz-next-0.5.9/
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-26 10:35:01.518655 alphaz-next-0.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:35:01.514655 alphaz-next-0.5.9/alphaz_next/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/alphaz_next/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:35:01.514655 alphaz-next-0.5.9/alphaz_next/asyncio/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/alphaz_next/asyncio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:35:01.514655 alphaz-next-0.5.9/alphaz_next/auth/
--rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/alphaz_next/auth/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:35:01.514655 alphaz-next-0.5.9/alphaz_next/core/
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/alphaz_next/core/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/alphaz_next/core/_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)    12965 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/alphaz_next/core/application.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/alphaz_next/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/alphaz_next/core/exception_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/alphaz_next/core/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:35:01.514655 alphaz-next-0.5.9/alphaz_next/core/responses/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/alphaz_next/core/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/alphaz_next/core/responses/file_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/alphaz_next/core/responses/html_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/alphaz_next/core/responses/json_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/alphaz_next/core/responses/orjson_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/alphaz_next/core/responses/plaintext_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/alphaz_next/core/responses/redirect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/alphaz_next/core/responses/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/alphaz_next/core/responses/streaming_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/alphaz_next/core/responses/ujson_response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:35:01.514655 alphaz-next-0.5.9/alphaz_next/libs/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/alphaz_next/libs/file_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/alphaz_next/libs/httpx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:35:01.510655 alphaz-next-0.5.9/alphaz_next/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:35:01.518655 alphaz-next-0.5.9/alphaz_next/models/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/alphaz_next/models/auth/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:35:01.518655 alphaz-next-0.5.9/alphaz_next/models/config/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:35:01.518655 alphaz-next-0.5.9/alphaz_next/models/config/_base/
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/alphaz_next/models/config/_base/internal_config_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/alphaz_next/models/config/_base/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/alphaz_next/models/config/alpha_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/alphaz_next/models/config/api_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/alphaz_next/models/config/apm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/alphaz_next/models/config/config_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/alphaz_next/models/config/database_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/alphaz_next/models/config/directories_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/alphaz_next/models/config/logging_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/alphaz_next/models/config/openapi_config_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:35:01.510655 alphaz-next-0.5.9/alphaz_next/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:35:01.518655 alphaz-next-0.5.9/alphaz_next/tests/utils/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:35:01.518655 alphaz-next-0.5.9/alphaz_next/tests/utils/mocking/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/alphaz_next/tests/utils/mocking/mock_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    27232 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/alphaz_next/tests/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:35:01.518655 alphaz-next-0.5.9/alphaz_next/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/alphaz_next/utils/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/alphaz_next/utils/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    11706 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/alphaz_next/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/alphaz_next/utils/logging_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-26 10:34:58.000000 alphaz-next-0.5.9/alphaz_next/utils/loguru.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:35:01.514655 alphaz-next-0.5.9/alphaz_next.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-26 10:35:01.000000 alphaz-next-0.5.9/alphaz_next.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-26 10:35:01.000000 alphaz-next-0.5.9/alphaz_next.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 10:35:01.000000 alphaz-next-0.5.9/alphaz_next.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-26 10:35:01.000000 alphaz-next-0.5.9/alphaz_next.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-26 10:35:01.000000 alphaz-next-0.5.9/alphaz_next.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 10:35:01.518655 alphaz-next-0.5.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-26 10:34:59.000000 alphaz-next-0.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:49:33.913218 alphaz-next-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-05-06 08:49:33.913218 alphaz-next-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:49:33.905218 alphaz-next-0.6.0/alphaz_next/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:49:33.905218 alphaz-next-0.6.0/alphaz_next/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/asyncio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:49:33.909218 alphaz-next-0.6.0/alphaz_next/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/auth/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:49:33.909218 alphaz-next-0.6.0/alphaz_next/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/core/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/core/_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12059 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/core/_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10133 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/core/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/core/exception_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/core/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:49:33.909218 alphaz-next-0.6.0/alphaz_next/core/responses/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/core/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/core/responses/file_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/core/responses/html_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/core/responses/json_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/core/responses/orjson_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/core/responses/plaintext_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/core/responses/redirect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/core/responses/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/core/responses/streaming_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/core/responses/ujson_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:49:33.909218 alphaz-next-0.6.0/alphaz_next/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/libs/file_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/libs/httpx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:49:33.905218 alphaz-next-0.6.0/alphaz_next/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:49:33.909218 alphaz-next-0.6.0/alphaz_next/models/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/models/auth/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:49:33.913218 alphaz-next-0.6.0/alphaz_next/models/config/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:49:33.913218 alphaz-next-0.6.0/alphaz_next/models/config/_base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/models/config/_base/internal_config_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/models/config/_base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/models/config/alpha_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/models/config/api_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/models/config/apm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/models/config/config_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/models/config/database_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/models/config/directories_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/models/config/logging_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/models/config/openapi_config_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:49:33.905218 alphaz-next-0.6.0/alphaz_next/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:49:33.913218 alphaz-next-0.6.0/alphaz_next/tests/utils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:49:33.913218 alphaz-next-0.6.0/alphaz_next/tests/utils/mocking/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/tests/utils/mocking/mock_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27232 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/tests/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:49:33.913218 alphaz-next-0.6.0/alphaz_next/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/utils/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/utils/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/utils/logging_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-06 08:49:28.000000 alphaz-next-0.6.0/alphaz_next/utils/loguru.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:49:33.905218 alphaz-next-0.6.0/alphaz_next.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-05-06 08:49:33.000000 alphaz-next-0.6.0/alphaz_next.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-06 08:49:33.000000 alphaz-next-0.6.0/alphaz_next.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 08:49:33.000000 alphaz-next-0.6.0/alphaz_next.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-06 08:49:33.000000 alphaz-next-0.6.0/alphaz_next.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-06 08:49:33.000000 alphaz-next-0.6.0/alphaz_next.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 08:49:33.913218 alphaz-next-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-06 08:49:32.000000 alphaz-next-0.6.0/setup.py
```

### Comparing `alphaz-next-0.5.9/PKG-INFO` & `alphaz-next-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: alphaz-next
-Version: 0.5.9
+Version: 0.6.0
 Summary: A project to make a lib to start FASTAPI quickly
 Home-page: https://github.com/STDef200mm/alphaz-next
-Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.5.9.tar.gz
+Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.6.0.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `alphaz-next-0.5.9/README.md` & `alphaz-next-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.9/alphaz_next/auth/auth.py` & `alphaz-next-0.6.0/alphaz_next/auth/auth.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.9/alphaz_next/core/_base.py` & `alphaz-next-0.6.0/alphaz_next/core/_base.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.9/alphaz_next/core/_middleware.py` & `alphaz-next-0.6.0/alphaz_next/core/_middleware.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # MODULES
 import http
+import logging as _logging
 import time
 from typing import Optional, Sequence
-from loguru import logger
 
 # FASTAPI
 from fastapi import Request, Response
 from fastapi.middleware.cors import CORSMiddleware as _CORSMiddleware
 
 # STARLETTE
 from starlette.types import ASGIApp
 
 # CORE
 from alphaz_next.core.constants import HeaderEnum
 
-uvicorn_logger = logger.bind(service="uvicorn")
+uvicorn_logger = _logging.getLogger("uvicorn")
 
 
 class CORSMiddleware(_CORSMiddleware):
     def __init__(
         self,
         app: ASGIApp,
         allow_origins: Sequence[str] = (),
@@ -70,12 +70,11 @@
     try:
         status_phrase = http.HTTPStatus(response.status_code).phrase
     except ValueError:
         status_phrase = ""
 
     response.headers[HeaderEnum.PROCESS_TIME.value] = str(process_time)
 
-    with uvicorn_logger.contextualize(endpoint=request.url.path):
-        uvicorn_logger.info(
-            f'{host}:{port} - "{request.method} {url}" {response.status_code} {status_phrase} {formatted_process_time}ms'
-        )
+    uvicorn_logger.info(
+        f'{host}:{port} - "{request.method} {url}" {response.status_code} {status_phrase} {formatted_process_time}ms'
+    )
     return response
```

### Comparing `alphaz-next-0.5.9/alphaz_next/core/application.py` & `alphaz-next-0.6.0/alphaz_next/core/application.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # MODULES
-import os
+from logging.handlers import TimedRotatingFileHandler
+from pathlib import Path
 import sys as _sys
 from typing import (
     Any as _Any,
     AsyncContextManager as _AsyncContextManager,
     Dict as _Dict,
     List as _List,
     Optional as _Optional,
     Sequence as _Sequence,
     Union as _Union,
 )
-import logging
-from loguru import logger
+import logging as _logging
 
 # FASTAPI
 from fastapi import (
     APIRouter as _APIRouter,
     FastAPI as _FastAPI,
     HTTPException as _HTTPException,
     Request as _Request,
@@ -34,45 +34,38 @@
 from fastapi.responses import (
     HTMLResponse as _HTMLResponse,
     JSONResponse as _JSONResponse,
     PlainTextResponse as _PlainTextResponse,
     RedirectResponse as _RedirectResponse,
 )
 
-# OPENTELEMETRY
-from opentelemetry import metrics, trace
-from opentelemetry.exporter.otlp.proto.http.metric_exporter import OTLPMetricExporter
-from opentelemetry.exporter.otlp.proto.http.trace_exporter import OTLPSpanExporter
-from opentelemetry.sdk.metrics import MeterProvider
-from opentelemetry.sdk.metrics.export import PeriodicExportingMetricReader
-from opentelemetry.sdk.resources import Resource
-from opentelemetry.sdk.trace import TracerProvider
-from opentelemetry.sdk.trace.export import BatchSpanProcessor
-from opentelemetry.instrumentation.fastapi import FastAPIInstrumentor
-
 # MODELS
 from alphaz_next.models.config.alpha_config import (
     AlphaConfigSchema as _AlphaConfigSchema,
 )
 
 # CORE
 from alphaz_next.core._middleware import (
     log_request_middleware as _log_request_middleware,
     CORSMiddleware as _CORSMiddleware,
 )
+from alphaz_next.core._telemetry import setup_telemetry
 
-
-# ELASTICAPM
+# UTILS
+# UTILS
+from alphaz_next.utils.logging_filters import (
+    ExcludeRoutersFilter as _ExcludeRoutersFilter,
+)
 
 _DEFAULT_FAVICON_URL = "https://fastapi.tiangolo.com/img/favicon.png"
 
-_uvicorn_access = logging.getLogger("uvicorn.access")
+_uvicorn_access = _logging.getLogger("uvicorn.access")
 _uvicorn_access.disabled = True
 
-uvicorn_logger = logger.bind(service="uvicorn")
+uvicorn_logger = _logging.getLogger("uvicorn")
 
 
 def _custom_openapi(
     config: _AlphaConfigSchema, routes: _List[_BaseRoute]
 ) -> _Dict[str, _Any]:
     """
     Generate a custom OpenAPI schema based on the provided configuration and routes.
@@ -105,110 +98,14 @@
         routes=routes,
         **openapi_dict,
     )
 
     return openapi_schema
 
 
-def _setup_opentelemetry(config: _AlphaConfigSchema, app: _FastAPI) -> None:
-    """
-    Sets up OpenTelemetry for the application.
-
-    Args:
-        config (_AlphaConfigSchema): The configuration object.
-        app (_FastAPI): The FastAPI application object.
-
-    Returns:
-        None
-    """
-
-    if config.api_config.apm is None or not config.api_config.apm.active:
-        return None
-
-    otel_service_name = config.project_name
-    apm_server_url = config.api_config.apm.server_url
-    certificate_path = config.api_config.apm.certificate_file
-    environment = config.environment.lower()
-    version = config.version
-
-    otel_exporter_otlp_headers = os.environ.get(
-        "OTEL_EXPORTER_OTLP_HEADERS",
-        None,
-    )
-
-    otel_exporter_otlp_endpoint = os.environ.get(
-        "OTEL_EXPORTER_OTLP_ENDPOINT",
-        apm_server_url,
-    )
-
-    otel_exporter_otl_certificate = os.environ.get(
-        "OTEL_EXPORTER_OTLP_CERTIFICATE",
-        certificate_path,
-    )
-
-    # Ressource
-    resource_attributes = (
-        os.environ.get("OTEL_RESOURCE_ATTRIBUTES")
-        or f"service.version={version},deployment.environment={environment}"
-    )
-    key_value_pairs = resource_attributes.split(",")
-    result_dict = {}
-
-    for pair in key_value_pairs:
-        key, value = pair.split("=")
-        result_dict[key] = value
-
-    resourceAttributes = {
-        "service.name": otel_service_name,
-        "service.version": result_dict["service.version"],
-        "deployment.environment": result_dict["deployment.environment"],
-    }
-
-    resource = Resource.create(resourceAttributes)
-
-    # Traces
-    otel_exported_otlp_traces_endpoint = os.environ.get(
-        "OTEL_EXPORTER_OTLP_TRACES_ENDPOINT",
-        f"{otel_exporter_otlp_endpoint}/v1/traces",
-    )
-
-    exporter = OTLPSpanExporter(
-        endpoint=otel_exported_otlp_traces_endpoint,
-        certificate_file=otel_exporter_otl_certificate,
-        headers=otel_exporter_otlp_headers,
-    )
-
-    processor = BatchSpanProcessor(exporter)
-    traceProvider = TracerProvider(resource=resource)
-    traceProvider.add_span_processor(processor)
-    trace.set_tracer_provider(traceProvider)
-
-    provider = TracerProvider(resource=resource)
-    provider.add_span_processor(processor)
-
-    # Metrics
-    otel_exported_otlp_metrics_endpoint = os.environ.get(
-        "OTEL_EXPORTER_OTLP_METRICS_ENDPOINT",
-        f"{otel_exporter_otlp_endpoint}/v1/metrics",
-    )
-    exporter = OTLPMetricExporter(
-        endpoint=otel_exported_otlp_metrics_endpoint,
-        certificate_file=otel_exporter_otl_certificate,
-        headers=otel_exporter_otlp_headers,
-    )
-    reader = PeriodicExportingMetricReader(exporter=exporter)
-    meterProvider = MeterProvider(
-        resource=resource,
-        metric_readers=[reader],
-    )
-    metrics.set_meter_provider(meterProvider)
-
-    FastAPIInstrumentor().instrument_app(app)
-
-
 def create_app(
     config: _AlphaConfigSchema,
     routes: _Optional[_BaseRoute] = None,
     routers: _Optional[_List[_APIRouter]] = None,
     lifespan: _Optional[_AsyncContextManager] = None,
     allow_origins: _Sequence[str] = (),
     allow_methods: _Sequence[str] = ("GET",),
@@ -232,28 +129,14 @@
         allow_private_network (bool): Whether to allow private network for CORS. Defaults to False.
         status_response (Dict): The response to return for the "/status" endpoint. Defaults to {"status": "OK"}.
 
     Returns:
         FastAPI: The created FastAPI application.
     """
 
-    if config.api_config.logging is not None:
-        uvicorn_logger.add(
-            _sys.stderr,
-            level=config.api_config.logging.level.upper(),
-            filter=lambda record: all(
-                [
-                    record["extra"].get("service") == "uvicorn",
-                    record["extra"].get("endpoint")
-                    not in config.api_config.logging.excluded_routers,
-                ]
-            ),
-            colorize=True,
-        )
-
     # APP
     app = _FastAPI(
         routes=routes,
         title=config.project_name.upper(),
         version=config.version,
         docs_url=None,
         redoc_url=None,
@@ -267,29 +150,60 @@
         allow_methods=allow_methods,
         allow_headers=allow_headers,
         allow_private_network=allow_private_network,
     )
 
     app.middleware("http")(_log_request_middleware)
 
-    _setup_opentelemetry(config=config, app=app)
+    setup_telemetry(config=config, app=app)
 
     [app.include_router(router) for router in routers or []]
 
     app.openapi_schema = _custom_openapi(config=config, routes=app.routes)
 
     swagger_favicon_url = _DEFAULT_FAVICON_URL
     redoc_favicon_url = _DEFAULT_FAVICON_URL
     if (openapi_config := config.api_config.openapi) is not None:
         if openapi_config.swagger_favicon_url:
             swagger_favicon_url = openapi_config.swagger_favicon_url
 
         if openapi_config.redoc_favicon_url:
             redoc_favicon_url = openapi_config.redoc_favicon_url
 
+    if (
+        config.api_config.logging is not None
+        and config.api_config.logging.rotation is not None
+    ):
+        uvicorn_formatter = _logging.Formatter(
+            config.api_config.logging.uvicorn_format,
+            datefmt=config.api_config.logging.date_format,
+        )
+
+        directory_path = Path(config.api_config.directories.logs)
+        directory_path.mkdir(parents=True, exist_ok=True)
+
+        handler = TimedRotatingFileHandler(
+            filename=directory_path / "uvicorn.log",
+            when=config.api_config.logging.rotation,
+            backupCount=config.api_config.logging.retention,
+        )
+        handler.setFormatter(uvicorn_formatter)
+
+        uvicorn_logger.addHandler(handler)
+
+        telemetry_handler = app.extra.get("telemetry_handler")
+        if telemetry_handler is not None:
+            uvicorn_logger.addHandler(telemetry_handler)
+
+        uvicorn_logger.addFilter(
+            _ExcludeRoutersFilter(
+                router_names=config.api_config.logging.excluded_routers
+            )
+        )
+
     @app.exception_handler(_RequestValidationError)
     async def request_validation_exception_handler(
         request: _Request, exc: _RequestValidationError
     ) -> _JSONResponse:
         """
         This is a wrapper to the default RequestValidationException handler of FastAPI.
         This function will be called when client input is not valid.
@@ -298,16 +212,15 @@
         query_params = request.query_params._dict
         detail = {
             "errors": exc.errors(),
             "body": body.decode(),
             "query_params": query_params,
         }
 
-        with uvicorn_logger.contextualize(endpoint=request.base_url):
-            uvicorn_logger.info(detail)
+        uvicorn_logger.info(detail)
         return await _request_validation_exception_handler(request, exc)
 
     @app.exception_handler(_HTTPException)
     async def http_exception_handler(
         request: _Request, exc: _HTTPException
     ) -> _Union[_JSONResponse, _Response]:
         """
@@ -330,18 +243,17 @@
             f"{request.url.path}?{request.query_params}"
             if request.query_params
             else request.url.path
         )
         exception_type, exception_value, exception_traceback = _sys.exc_info()
         exception_name = getattr(exception_type, "__name__", None)
 
-        with uvicorn_logger.contextualize(endpoint=request.base_url):
-            uvicorn_logger.error(
-                f'{host}:{port} - "{request.method} {url}" 500 Internal Server Error <{exception_name}: {exception_value}>'
-            )
+        uvicorn_logger.error(
+            f'{host}:{port} - "{request.method} {url}" 500 Internal Server Error <{exception_name}: {exception_value}>'
+        )
         return _PlainTextResponse(str(exc), status_code=500)
 
     @app.get("/status", include_in_schema=False)
     async def get_api_status():
         return status_response
 
     @app.get("/docs", include_in_schema=False)
```

### Comparing `alphaz-next-0.5.9/alphaz_next/core/exception_handlers.py` & `alphaz-next-0.6.0/alphaz_next/core/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.9/alphaz_next/core/exceptions.py` & `alphaz-next-0.6.0/alphaz_next/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.9/alphaz_next/core/responses/__init__.py` & `alphaz-next-0.6.0/alphaz_next/core/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.9/alphaz_next/core/responses/file_response.py` & `alphaz-next-0.6.0/alphaz_next/core/responses/file_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.9/alphaz_next/core/responses/html_response.py` & `alphaz-next-0.6.0/alphaz_next/core/responses/html_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.9/alphaz_next/core/responses/json_response.py` & `alphaz-next-0.6.0/alphaz_next/core/responses/json_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.9/alphaz_next/core/responses/orjson_response.py` & `alphaz-next-0.6.0/alphaz_next/core/responses/orjson_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.9/alphaz_next/core/responses/plaintext_response.py` & `alphaz-next-0.6.0/alphaz_next/core/responses/plaintext_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.9/alphaz_next/core/responses/redirect_response.py` & `alphaz-next-0.6.0/alphaz_next/core/responses/redirect_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.9/alphaz_next/core/responses/response.py` & `alphaz-next-0.6.0/alphaz_next/core/responses/response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.9/alphaz_next/core/responses/streaming_response.py` & `alphaz-next-0.6.0/alphaz_next/core/responses/streaming_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.9/alphaz_next/core/responses/ujson_response.py` & `alphaz-next-0.6.0/alphaz_next/core/responses/ujson_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.9/alphaz_next/libs/httpx.py` & `alphaz-next-0.6.0/alphaz_next/libs/httpx.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.9/alphaz_next/models/config/_base/internal_config_settings.py` & `alphaz-next-0.6.0/alphaz_next/models/config/_base/internal_config_settings.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.9/alphaz_next/models/config/_base/utils.py` & `alphaz-next-0.6.0/alphaz_next/models/config/_base/utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.9/alphaz_next/models/config/alpha_config.py` & `alphaz-next-0.6.0/alphaz_next/models/config/alpha_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.9/alphaz_next/models/config/api_config.py` & `alphaz-next-0.6.0/alphaz_next/models/config/api_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.9/alphaz_next/models/config/apm_config.py` & `alphaz-next-0.6.0/alphaz_next/models/config/apm_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # MODULES
-from typing import Optional as _Optional
+from typing import Dict as _Dict, List as _List, Optional as _Optional
 
 # PYDANTIC
 from pydantic import (
     BaseModel as _BaseModel,
     ConfigDict as _ConfigDict,
     Field as _Field,
 )
@@ -17,7 +17,8 @@
     model_config = _ConfigDict(from_attributes=True)
 
     server_url: str
     certificate_file: _Optional[str] = _Field(default=None)
     ssl_verify: bool = _Field(default=True)
     debug: bool = _Field(default=True)
     active: bool = _Field(default=False)
+    configuration: _Optional[_Dict[str, _Optional[_List[str]]]] = _Field(default=None)
```

### Comparing `alphaz-next-0.5.9/alphaz_next/models/config/config_settings.py` & `alphaz-next-0.6.0/alphaz_next/models/config/config_settings.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.9/alphaz_next/models/config/database_config.py` & `alphaz-next-0.6.0/alphaz_next/models/config/database_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.9/alphaz_next/models/config/logging_config.py` & `alphaz-next-0.6.0/alphaz_next/models/config/logging_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,17 @@
     level: _Annotated[
         str,
         _StringConstraints(
             strip_whitespace=True,
             to_upper=True,
         ),
     ]
-    format: _Optional[str] = _Field(default=None)
+    format: str
+    uvicorn_format: str
+    date_format: str
     rotation: _Optional[str] = _Field(default=None)
     retention: _Optional[int] = _Field(default=None)
     excluded_routers: _List[str] = _Field(default_factory=lambda: [])
 
     @_field_validator("format")
     @classmethod
     def validate_format(cls, value: str, info: _FieldValidationInfo):
```

### Comparing `alphaz-next-0.5.9/alphaz_next/models/config/openapi_config_schema.py` & `alphaz-next-0.6.0/alphaz_next/models/config/openapi_config_schema.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.9/alphaz_next/tests/utils/utils.py` & `alphaz-next-0.6.0/alphaz_next/tests/utils/utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.9/alphaz_next/utils/format.py` & `alphaz-next-0.6.0/alphaz_next/utils/format.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.9/alphaz_next/utils/logger.py` & `alphaz-next-0.6.0/alphaz_next/utils/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         stream_output: bool = True,
         when: str = "midnight",
         interval: int = 1,
         backup_count: int = 10,
         file_name: _Optional[str] = None,
         logging_formatter: str = DEFAULT_FORMAT,
         date_formatter: str = DEFAULT_DATE_FORMAT,
+        telemetry_handler: _Optional[_logging.Handler] = None,
     ):
         """
         Initializes a Logger object.
 
         Args:
             name (str): The name of the logger.
             directory (str): The directory where log files will be stored.
@@ -57,29 +58,26 @@
 
         if file_name is None:
             file_name = name
 
         directory_path = _Path(directory)
         directory_path.mkdir(parents=True, exist_ok=True)
 
-        logger_config = {
-            "level": level,
-            "directory_path": directory_path,
-            "when": when,
-            "interval": interval,
-            "backup_count": backup_count,
-            "logging_formatter": logging_formatter,
-            "date_formatter": date_formatter,
-        }
-
         self._logger = self._create_logger(
             name=name,
+            level=level,
+            directory_path=directory_path,
             file_name=file_name,
+            when=when,
+            interval=interval,
+            backup_count=backup_count,
+            logging_formatter=logging_formatter,
+            date_formatter=date_formatter,
             stream_output=stream_output,
-            **logger_config,
+            telemetry_handler=telemetry_handler,
         )
 
     def info(
         self,
         message: str,
         exc_info: Exception = None,
         stack_level: int = 1,
@@ -195,14 +193,15 @@
         file_name: str,
         when: str,
         interval: int,
         backup_count: int,
         logging_formatter: str,
         date_formatter: str,
         stream_output: bool = False,
+        telemetry_handler: _Optional[_logging.Handler] = None,
     ) -> _logging.Logger:
         """
         Create and configure a logger with the specified parameters.
 
         Args:
             name (str): The name of the logger.
             level (int): The logging level for the logger.
@@ -210,14 +209,15 @@
             file_name (str): The name of the log file.
             when (str): The interval at which log files should be rotated (e.g., 'midnight', 'D', 'H', 'M', 'S').
             interval (int): The number of intervals between log file rotations.
             backup_count (int): The number of backup log files to keep.
             logging_formatter (str): The logging formatter string.
             date_formatter (str): The date formatter string.
             stream_output (bool, optional): Whether to log messages to stdout as well. Defaults to False.
+            telemetry_handler (Optional[logging.Handler]): The telemetry handler to be added to the logger. Defaults to None.
 
         Returns:
             logging.Logger: The configured logger.
 
         """
         logger = _logging.getLogger(name=name)
         logger.propagate = False
@@ -297,14 +297,17 @@
         )
 
         logger.addHandler(time_rotating_handler)
         logger.addHandler(warning_time_rotating_handler)
         logger.addHandler(error_time_rotating_handler)
         logger.addHandler(monitoring_time_rotating_handler)
 
+        if telemetry_handler is not None:
+            logger.addHandler(telemetry_handler)
+
         return logger
 
     def _create_time_rotating_handler(
         self,
         file_path: _Path,
         level: int,
         formatter: _logging.Formatter,
```

### Comparing `alphaz-next-0.5.9/alphaz_next/utils/logging_filters.py` & `alphaz-next-0.6.0/alphaz_next/utils/logging_filters.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.9/alphaz_next/utils/loguru.py` & `alphaz-next-0.6.0/alphaz_next/utils/loguru.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.5.9/alphaz_next.egg-info/PKG-INFO` & `alphaz-next-0.6.0/alphaz_next.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: alphaz-next
-Version: 0.5.9
+Version: 0.6.0
 Summary: A project to make a lib to start FASTAPI quickly
 Home-page: https://github.com/STDef200mm/alphaz-next
-Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.5.9.tar.gz
+Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.6.0.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `alphaz-next-0.5.9/alphaz_next.egg-info/SOURCES.txt` & `alphaz-next-0.6.0/alphaz_next.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 alphaz_next.egg-info/dependency_links.txt
 alphaz_next.egg-info/requires.txt
 alphaz_next.egg-info/top_level.txt
 alphaz_next/asyncio/__init__.py
 alphaz_next/auth/auth.py
 alphaz_next/core/_base.py
 alphaz_next/core/_middleware.py
+alphaz_next/core/_telemetry.py
 alphaz_next/core/application.py
 alphaz_next/core/constants.py
 alphaz_next/core/exception_handlers.py
 alphaz_next/core/exceptions.py
 alphaz_next/core/responses/__init__.py
 alphaz_next/core/responses/file_response.py
 alphaz_next/core/responses/html_response.py
```

### Comparing `alphaz-next-0.5.9/setup.py` & `alphaz-next-0.6.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.5.9"
+version = "0.6.0"
 
 with open("requirements.txt") as f:
     required_packages = f.read().splitlines()
 
 
 EXTRAS_REQUIRE = {
     "dependency-injector": ["dependency-injector"],
```

