# Comparing `tmp/helix.fhir.client.sdk-2.0.6.tar.gz` & `tmp/helix.fhir.client.sdk-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helix.fhir.client.sdk-2.0.6.tar", last modified: Tue Apr 16 18:55:07 2024, max compression
+gzip compressed data, was "helix.fhir.client.sdk-2.0.7.tar", last modified: Mon May  6 13:15:31 2024, max compression
```

## Comparing `helix.fhir.client.sdk-2.0.6.tar` & `helix.fhir.client.sdk-2.0.7.tar`

### file list

```diff
@@ -1,162 +1,162 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:55:07.039429 helix.fhir.client.sdk-2.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-16 18:55:07.039429 helix.fhir.client.sdk-2.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-16 18:55:06.000000 helix.fhir.client.sdk-2.0.6/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:55:07.039429 helix.fhir.client.sdk-2.0.6/helix.fhir.client.sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-16 18:55:06.000000 helix.fhir.client.sdk-2.0.6/helix.fhir.client.sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6997 2024-04-16 18:55:06.000000 helix.fhir.client.sdk-2.0.6/helix.fhir.client.sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 18:55:06.000000 helix.fhir.client.sdk-2.0.6/helix.fhir.client.sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 18:55:06.000000 helix.fhir.client.sdk-2.0.6/helix.fhir.client.sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-16 18:55:06.000000 helix.fhir.client.sdk-2.0.6/helix.fhir.client.sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-16 18:55:06.000000 helix.fhir.client.sdk-2.0.6/helix.fhir.client.sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:55:07.019429 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/dictionary_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/dictionary_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:55:07.019429 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/exceptions/fhir_sender_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/exceptions/fhir_validation_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/fhir_bundle.py
--rw-r--r--   0 runner    (1001) docker     (127)     9465 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/fhir_bundle_appender.py
--rw-r--r--   0 runner    (1001) docker     (127)   116519 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/fhir_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:55:07.019429 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/filters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/filters/base_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/filters/identifier_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/filters/last_updated_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/filters/property_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/filters/property_missing_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/filters/security_access_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/filters/security_owner_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/filters/sort_field.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/filters/source_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/filters/version_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/function_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:55:07.019429 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/graph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/graph/graph_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    22276 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/graph/simulated_graph_processor_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:55:07.023429 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/loggers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/loggers/fhir_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:55:07.023429 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/responses/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/responses/fhir_delete_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    14056 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/responses/fhir_get_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/responses/fhir_merge_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/responses/fhir_update_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/responses/get_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/responses/paging_result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:55:07.023429 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/utilities/fhir_json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/utilities/fhir_scope_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/utilities/fhir_scope_parser_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/utilities/json_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/utilities/request_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:55:07.023429 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/utilities/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/utilities/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12844 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/utilities/test/test_fhir_scope_parser_can_parse_scopes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/utilities/test/test_fhir_scope_parser_correct_allow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:55:07.023429 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/validators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/validators/async_fhir_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/validators/fhir_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/well_known_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-16 18:55:07.039429 helix.fhir.client.sdk-2.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-16 18:55:06.000000 helix.fhir.client.sdk-2.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:55:07.027429 helix.fhir.client.sdk-2.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:55:07.027429 helix.fhir.client.sdk-2.0.6/tests/async/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:55:07.031429 helix.fhir.client.sdk-2.0.6/tests/async/graph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/graph/test_fhir_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:55:07.031429 helix.fhir.client.sdk-2.0.6/tests/async/simulated_graph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/simulated_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/simulated_graph/test_fhir_simulated_graph_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     7647 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/simulated_graph/test_fhir_simulated_graph_caching_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/simulated_graph/test_fhir_simulated_graph_caching_scope_parser_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     9713 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/simulated_graph/test_fhir_simulated_graph_separate_resources_async.py
--rw-r--r--   0 runner    (1001) docker     (127)    13698 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/simulated_graph/test_fhir_simulated_graph_with_errors_async.py
--rw-r--r--   0 runner    (1001) docker     (127)    18264 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/simulated_graph/test_fhir_simulated_graph_with_operation_outcomes_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/simulated_graph/test_fhir_simulated_graph_with_url_column_async.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:55:07.031429 helix.fhir.client.sdk-2.0.6/tests/async/simulated_graph_practitioner/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/simulated_graph_practitioner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/simulated_graph_practitioner/test_fhir_simulated_graph_multiple_practitioner_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/simulated_graph_practitioner/test_fhir_simulated_graph_multiple_practitioner_in_one_call_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     4762 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/simulated_graph_practitioner/test_fhir_simulated_graph_practitioner_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/simulated_graph_practitioner/test_fhir_simulated_graph_practitioner_separate_resources_async.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:55:07.031429 helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_bundle/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_bundle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:55:07.031429 helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_bundle/not_expanded/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_bundle/not_expanded/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_bundle/not_expanded/test_fhir_client_bundle_not_expanded.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:55:07.031429 helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_bundle/not_separated/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_bundle/not_separated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_bundle/not_separated/test_fhir_client_bundle_not_separated.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:55:07.035429 helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_bundle/separated/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_bundle/separated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_bundle/separated/test_fhir_client_bundle_separated.py
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_fetch_response_in_chunks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_patient_by_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_patient_by_identifier_missing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_patient_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_patient_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_patient_list_auth_fail.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_patient_list_auth_fail_retry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_patient_list_auth_fail_retry_custom_refresh_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_patient_list_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_patient_list_in_batches.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_patient_list_streaming.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_patient_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_patient_merge_with_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_patient_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_practitioner_role_for_diff_req.py
--rw-r--r--   0 runner    (1001) docker     (127)     8096 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/async/test_get_resources_by_query_async_with_additional_params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:55:07.035429 helix.fhir.client.sdk-2.0.6/tests/sync/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:55:07.035429 helix.fhir.client.sdk-2.0.6/tests/sync/graph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/sync/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/sync/graph/test_fhir_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:55:07.035429 helix.fhir.client.sdk-2.0.6/tests/sync/test_fhir_client_bundle/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/sync/test_fhir_client_bundle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:55:07.035429 helix.fhir.client.sdk-2.0.6/tests/sync/test_fhir_client_bundle/not_expanded/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/sync/test_fhir_client_bundle/not_expanded/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/sync/test_fhir_client_bundle/not_expanded/test_fhir_client_bundle_not_expanded.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:55:07.035429 helix.fhir.client.sdk-2.0.6/tests/sync/test_fhir_client_bundle/not_separated/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/sync/test_fhir_client_bundle/not_separated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/sync/test_fhir_client_bundle/not_separated/test_fhir_client_bundle_not_separated.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:55:07.039429 helix.fhir.client.sdk-2.0.6/tests/sync/test_fhir_client_bundle/separated/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/sync/test_fhir_client_bundle/separated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/sync/test_fhir_client_bundle/separated/test_fhir_client_bundle_separated.py
--rw-r--r--   0 runner    (1001) docker     (127)     6487 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/sync/test_fhir_client_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/sync/test_fhir_client_patient_by_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/sync/test_fhir_client_patient_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/sync/test_fhir_client_patient_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/sync/test_fhir_client_patient_list_auth_fail.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/sync/test_fhir_client_patient_list_auth_fail_retry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/sync/test_fhir_client_patient_list_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/sync/test_fhir_client_patient_list_in_batches.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/sync/test_fhir_client_patient_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/sync/test_fhir_client_patient_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/sync/test_fhir_client_patient_update_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/test_get_nested_property.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests/test_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:55:07.039429 helix.fhir.client.sdk-2.0.6/tests_integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests_integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests_integration/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests_integration/test_aetna_server_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests_integration/test_aetna_server_auth_aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests_integration/test_aetna_server_auth_httpx.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests_integration/test_dev_server_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests_integration/test_dev_server_get_patients.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests_integration/test_dev_server_get_patients_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests_integration/test_dev_server_no_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-04-16 18:54:23.000000 helix.fhir.client.sdk-2.0.6/tests_integration/test_staging_server_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:15:31.148215 helix.fhir.client.sdk-2.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-06 13:15:31.148215 helix.fhir.client.sdk-2.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-06 13:15:30.000000 helix.fhir.client.sdk-2.0.7/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:15:31.148215 helix.fhir.client.sdk-2.0.7/helix.fhir.client.sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-06 13:15:31.000000 helix.fhir.client.sdk-2.0.7/helix.fhir.client.sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6997 2024-05-06 13:15:31.000000 helix.fhir.client.sdk-2.0.7/helix.fhir.client.sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 13:15:31.000000 helix.fhir.client.sdk-2.0.7/helix.fhir.client.sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 13:15:31.000000 helix.fhir.client.sdk-2.0.7/helix.fhir.client.sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-06 13:15:31.000000 helix.fhir.client.sdk-2.0.7/helix.fhir.client.sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-06 13:15:31.000000 helix.fhir.client.sdk-2.0.7/helix.fhir.client.sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:15:31.128215 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/dictionary_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/dictionary_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:15:31.128215 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/exceptions/fhir_sender_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/exceptions/fhir_validation_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/fhir_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9465 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/fhir_bundle_appender.py
+-rw-r--r--   0 runner    (1001) docker     (127)   116548 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/fhir_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:15:31.132215 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/filters/base_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/filters/identifier_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/filters/last_updated_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/filters/property_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/filters/property_missing_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/filters/security_access_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/filters/security_owner_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/filters/sort_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/filters/source_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/filters/version_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/function_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:15:31.132215 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/graph/graph_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22276 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/graph/simulated_graph_processor_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:15:31.132215 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/loggers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/loggers/fhir_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:15:31.132215 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/responses/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/responses/fhir_delete_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14056 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/responses/fhir_get_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/responses/fhir_merge_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/responses/fhir_update_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/responses/get_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/responses/paging_result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:15:31.132215 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/utilities/fhir_json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/utilities/fhir_scope_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/utilities/fhir_scope_parser_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/utilities/json_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/utilities/request_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:15:31.132215 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/utilities/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/utilities/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12844 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/utilities/test/test_fhir_scope_parser_can_parse_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/utilities/test/test_fhir_scope_parser_correct_allow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:15:31.136215 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/validators/async_fhir_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/validators/fhir_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/well_known_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-06 13:15:31.148215 helix.fhir.client.sdk-2.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-06 13:15:30.000000 helix.fhir.client.sdk-2.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:15:31.136215 helix.fhir.client.sdk-2.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:15:31.140215 helix.fhir.client.sdk-2.0.7/tests/async/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:15:31.140215 helix.fhir.client.sdk-2.0.7/tests/async/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/graph/test_fhir_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:15:31.140215 helix.fhir.client.sdk-2.0.7/tests/async/simulated_graph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/simulated_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/simulated_graph/test_fhir_simulated_graph_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7647 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/simulated_graph/test_fhir_simulated_graph_caching_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/simulated_graph/test_fhir_simulated_graph_caching_scope_parser_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9713 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/simulated_graph/test_fhir_simulated_graph_separate_resources_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13698 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/simulated_graph/test_fhir_simulated_graph_with_errors_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18264 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/simulated_graph/test_fhir_simulated_graph_with_operation_outcomes_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/simulated_graph/test_fhir_simulated_graph_with_url_column_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:15:31.140215 helix.fhir.client.sdk-2.0.7/tests/async/simulated_graph_practitioner/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/simulated_graph_practitioner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/simulated_graph_practitioner/test_fhir_simulated_graph_multiple_practitioner_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/simulated_graph_practitioner/test_fhir_simulated_graph_multiple_practitioner_in_one_call_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4762 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/simulated_graph_practitioner/test_fhir_simulated_graph_practitioner_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/simulated_graph_practitioner/test_fhir_simulated_graph_practitioner_separate_resources_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:15:31.140215 helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_bundle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_bundle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:15:31.140215 helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_bundle/not_expanded/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_bundle/not_expanded/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_bundle/not_expanded/test_fhir_client_bundle_not_expanded.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:15:31.144215 helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_bundle/not_separated/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_bundle/not_separated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_bundle/not_separated/test_fhir_client_bundle_not_separated.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:15:31.144215 helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_bundle/separated/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_bundle/separated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_bundle/separated/test_fhir_client_bundle_separated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_fetch_response_in_chunks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_patient_by_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_patient_by_identifier_missing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_patient_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_patient_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_patient_list_auth_fail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_patient_list_auth_fail_retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_patient_list_auth_fail_retry_custom_refresh_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_patient_list_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_patient_list_in_batches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_patient_list_streaming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_patient_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_patient_merge_with_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_patient_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_practitioner_role_for_diff_req.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8096 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/async/test_get_resources_by_query_async_with_additional_params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:15:31.144215 helix.fhir.client.sdk-2.0.7/tests/sync/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:15:31.144215 helix.fhir.client.sdk-2.0.7/tests/sync/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/sync/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/sync/graph/test_fhir_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:15:31.144215 helix.fhir.client.sdk-2.0.7/tests/sync/test_fhir_client_bundle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/sync/test_fhir_client_bundle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:15:31.144215 helix.fhir.client.sdk-2.0.7/tests/sync/test_fhir_client_bundle/not_expanded/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/sync/test_fhir_client_bundle/not_expanded/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/sync/test_fhir_client_bundle/not_expanded/test_fhir_client_bundle_not_expanded.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:15:31.148215 helix.fhir.client.sdk-2.0.7/tests/sync/test_fhir_client_bundle/not_separated/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/sync/test_fhir_client_bundle/not_separated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/sync/test_fhir_client_bundle/not_separated/test_fhir_client_bundle_not_separated.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:15:31.148215 helix.fhir.client.sdk-2.0.7/tests/sync/test_fhir_client_bundle/separated/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/sync/test_fhir_client_bundle/separated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/sync/test_fhir_client_bundle/separated/test_fhir_client_bundle_separated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6487 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/sync/test_fhir_client_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/sync/test_fhir_client_patient_by_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/sync/test_fhir_client_patient_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/sync/test_fhir_client_patient_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/sync/test_fhir_client_patient_list_auth_fail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/sync/test_fhir_client_patient_list_auth_fail_retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/sync/test_fhir_client_patient_list_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/sync/test_fhir_client_patient_list_in_batches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/sync/test_fhir_client_patient_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/sync/test_fhir_client_patient_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/sync/test_fhir_client_patient_update_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/test_get_nested_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:15:31.148215 helix.fhir.client.sdk-2.0.7/tests_integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests_integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests_integration/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests_integration/test_aetna_server_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests_integration/test_aetna_server_auth_aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests_integration/test_aetna_server_auth_httpx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests_integration/test_dev_server_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests_integration/test_dev_server_get_patients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests_integration/test_dev_server_get_patients_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests_integration/test_dev_server_no_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-05-06 13:14:53.000000 helix.fhir.client.sdk-2.0.7/tests_integration/test_staging_server_graph.py
```

### Comparing `helix.fhir.client.sdk-2.0.6/LICENSE` & `helix.fhir.client.sdk-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/Makefile` & `helix.fhir.client.sdk-2.0.7/Makefile`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/PKG-INFO` & `helix.fhir.client.sdk-2.0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helix.fhir.client.sdk
-Version: 2.0.6
+Version: 2.0.7
 Summary: helix.fhir.client.sdk
 Home-page: https://github.com/icanbwell/helix.fhir.client.sdk
 Author: Imran Qureshi
 Author-email: imran@icanbwell.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: helix.fhir.client.sdk Version: 2.0.6 Summary:
+Metadata-Version: 2.1 Name: helix.fhir.client.sdk Version: 2.0.7 Summary:
 helix.fhir.client.sdk Home-page: https://github.com/icanbwell/
 helix.fhir.client.sdk Author: Imran Qureshi Author-email: imran@icanbwell.com
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 furl Requires-Dist: requests Requires-Dist: urllib3 Requires-Dist: chardet
```

### Comparing `helix.fhir.client.sdk-2.0.6/README.md` & `helix.fhir.client.sdk-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/helix.fhir.client.sdk.egg-info/PKG-INFO` & `helix.fhir.client.sdk-2.0.7/helix.fhir.client.sdk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helix.fhir.client.sdk
-Version: 2.0.6
+Version: 2.0.7
 Summary: helix.fhir.client.sdk
 Home-page: https://github.com/icanbwell/helix.fhir.client.sdk
 Author: Imran Qureshi
 Author-email: imran@icanbwell.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: helix.fhir.client.sdk Version: 2.0.6 Summary:
+Metadata-Version: 2.1 Name: helix.fhir.client.sdk Version: 2.0.7 Summary:
 helix.fhir.client.sdk Home-page: https://github.com/icanbwell/
 helix.fhir.client.sdk Author: Imran Qureshi Author-email: imran@icanbwell.com
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 furl Requires-Dist: requests Requires-Dist: urllib3 Requires-Dist: chardet
```

### Comparing `helix.fhir.client.sdk-2.0.6/helix.fhir.client.sdk.egg-info/SOURCES.txt` & `helix.fhir.client.sdk-2.0.7/helix.fhir.client.sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/dictionary_parser.py` & `helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/dictionary_parser.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/dictionary_writer.py` & `helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/dictionary_writer.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/exceptions/fhir_sender_exception.py` & `helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/exceptions/fhir_sender_exception.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/exceptions/fhir_validation_exception.py` & `helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/exceptions/fhir_validation_exception.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/fhir_bundle.py` & `helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/fhir_bundle.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/fhir_bundle_appender.py` & `helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/fhir_bundle_appender.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/fhir_client.py` & `helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/fhir_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1560,15 +1560,15 @@
         if not auth_server_url or not login_token:
             return None
         assert auth_server_url, "No auth server url was set"
         assert login_token, "No login token was set"
         payload: str = (
             "grant_type=client_credentials&scope=" + "%20".join(auth_scopes)
             if auth_scopes
-            else ""
+            else "grant_type=client_credentials"
         )
         # noinspection SpellCheckingInspection
         headers: Dict[str, str] = {
             "Accept": "application/json",
             "Authorization": "Basic " + login_token,
             "Content-Type": "application/x-www-form-urlencoded",
         }
```

### Comparing `helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/filters/identifier_filter.py` & `helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/filters/identifier_filter.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/filters/last_updated_filter.py` & `helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/filters/last_updated_filter.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/filters/property_filter.py` & `helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/filters/property_filter.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/filters/property_missing_filter.py` & `helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/filters/property_missing_filter.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/function_types.py` & `helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/function_types.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/graph/graph_definition.py` & `helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/graph/graph_definition.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/graph/simulated_graph_processor_mixin.py` & `helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/graph/simulated_graph_processor_mixin.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/responses/fhir_delete_response.py` & `helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/responses/fhir_delete_response.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/responses/fhir_get_response.py` & `helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/responses/fhir_get_response.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/responses/fhir_merge_response.py` & `helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/responses/fhir_merge_response.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/responses/fhir_update_response.py` & `helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/responses/fhir_update_response.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/utilities/fhir_json_encoder.py` & `helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/utilities/fhir_json_encoder.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/utilities/fhir_scope_parser.py` & `helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/utilities/fhir_scope_parser.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/utilities/json_helpers.py` & `helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/utilities/json_helpers.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/utilities/request_cache.py` & `helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/utilities/request_cache.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/utilities/test/test_fhir_scope_parser_can_parse_scopes.py` & `helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/utilities/test/test_fhir_scope_parser_can_parse_scopes.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/utilities/test/test_fhir_scope_parser_correct_allow.py` & `helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/utilities/test/test_fhir_scope_parser_correct_allow.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/validators/async_fhir_validator.py` & `helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/validators/async_fhir_validator.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/helix_fhir_client_sdk/validators/fhir_validator.py` & `helix.fhir.client.sdk-2.0.7/helix_fhir_client_sdk/validators/fhir_validator.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/setup.cfg` & `helix.fhir.client.sdk-2.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/setup.py` & `helix.fhir.client.sdk-2.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/async/graph/test_fhir_graph.py` & `helix.fhir.client.sdk-2.0.7/tests/async/graph/test_fhir_graph.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/async/simulated_graph/test_fhir_simulated_graph_async.py` & `helix.fhir.client.sdk-2.0.7/tests/async/simulated_graph/test_fhir_simulated_graph_async.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/async/simulated_graph/test_fhir_simulated_graph_caching_async.py` & `helix.fhir.client.sdk-2.0.7/tests/async/simulated_graph/test_fhir_simulated_graph_caching_async.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/async/simulated_graph/test_fhir_simulated_graph_caching_scope_parser_async.py` & `helix.fhir.client.sdk-2.0.7/tests/async/simulated_graph/test_fhir_simulated_graph_caching_scope_parser_async.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/async/simulated_graph/test_fhir_simulated_graph_separate_resources_async.py` & `helix.fhir.client.sdk-2.0.7/tests/async/simulated_graph/test_fhir_simulated_graph_separate_resources_async.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/async/simulated_graph/test_fhir_simulated_graph_with_errors_async.py` & `helix.fhir.client.sdk-2.0.7/tests/async/simulated_graph/test_fhir_simulated_graph_with_errors_async.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/async/simulated_graph/test_fhir_simulated_graph_with_operation_outcomes_async.py` & `helix.fhir.client.sdk-2.0.7/tests/async/simulated_graph/test_fhir_simulated_graph_with_operation_outcomes_async.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/async/simulated_graph/test_fhir_simulated_graph_with_url_column_async.py` & `helix.fhir.client.sdk-2.0.7/tests/async/simulated_graph/test_fhir_simulated_graph_with_url_column_async.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/async/simulated_graph_practitioner/test_fhir_simulated_graph_multiple_practitioner_async.py` & `helix.fhir.client.sdk-2.0.7/tests/async/simulated_graph_practitioner/test_fhir_simulated_graph_multiple_practitioner_async.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/async/simulated_graph_practitioner/test_fhir_simulated_graph_multiple_practitioner_in_one_call_async.py` & `helix.fhir.client.sdk-2.0.7/tests/async/simulated_graph_practitioner/test_fhir_simulated_graph_multiple_practitioner_in_one_call_async.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/async/simulated_graph_practitioner/test_fhir_simulated_graph_practitioner_async.py` & `helix.fhir.client.sdk-2.0.7/tests/async/simulated_graph_practitioner/test_fhir_simulated_graph_practitioner_async.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/async/simulated_graph_practitioner/test_fhir_simulated_graph_practitioner_separate_resources_async.py` & `helix.fhir.client.sdk-2.0.7/tests/async/simulated_graph_practitioner/test_fhir_simulated_graph_practitioner_separate_resources_async.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_bundle/not_expanded/test_fhir_client_bundle_not_expanded.py` & `helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_bundle/not_expanded/test_fhir_client_bundle_not_expanded.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_bundle/not_separated/test_fhir_client_bundle_not_separated.py` & `helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_bundle/not_separated/test_fhir_client_bundle_not_separated.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_bundle/separated/test_fhir_client_bundle_separated.py` & `helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_bundle/separated/test_fhir_client_bundle_separated.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_fetch_response_in_chunks.py` & `helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_fetch_response_in_chunks.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_filter.py` & `helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_filter.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_patient_by_id.py` & `helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_patient_by_id.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_patient_by_identifier_missing.py` & `helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_patient_by_identifier_missing.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_patient_delete.py` & `helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_patient_delete.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_patient_list.py` & `helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_patient_list.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_patient_list_auth_fail.py` & `helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_patient_list_auth_fail.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_patient_list_auth_fail_retry.py` & `helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_patient_list_auth_fail_retry.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_patient_list_auth_fail_retry_custom_refresh_function.py` & `helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_patient_list_auth_fail_retry_custom_refresh_function.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_patient_list_ids.py` & `helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_patient_list_ids.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_patient_list_in_batches.py` & `helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_patient_list_in_batches.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_patient_list_streaming.py` & `helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_patient_list_streaming.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_patient_merge.py` & `helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_patient_merge.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_patient_merge_with_validate.py` & `helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_patient_merge_with_validate.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_patient_update.py` & `helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_patient_update.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/async/test_async_fhir_client_practitioner_role_for_diff_req.py` & `helix.fhir.client.sdk-2.0.7/tests/async/test_async_fhir_client_practitioner_role_for_diff_req.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/async/test_get_resources_by_query_async_with_additional_params.py` & `helix.fhir.client.sdk-2.0.7/tests/async/test_get_resources_by_query_async_with_additional_params.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/sync/graph/test_fhir_graph.py` & `helix.fhir.client.sdk-2.0.7/tests/sync/graph/test_fhir_graph.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/sync/test_fhir_client_bundle/not_expanded/test_fhir_client_bundle_not_expanded.py` & `helix.fhir.client.sdk-2.0.7/tests/sync/test_fhir_client_bundle/not_expanded/test_fhir_client_bundle_not_expanded.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/sync/test_fhir_client_bundle/not_separated/test_fhir_client_bundle_not_separated.py` & `helix.fhir.client.sdk-2.0.7/tests/sync/test_fhir_client_bundle/not_separated/test_fhir_client_bundle_not_separated.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/sync/test_fhir_client_bundle/separated/test_fhir_client_bundle_separated.py` & `helix.fhir.client.sdk-2.0.7/tests/sync/test_fhir_client_bundle/separated/test_fhir_client_bundle_separated.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/sync/test_fhir_client_filter.py` & `helix.fhir.client.sdk-2.0.7/tests/sync/test_fhir_client_filter.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/sync/test_fhir_client_patient_by_id.py` & `helix.fhir.client.sdk-2.0.7/tests/sync/test_fhir_client_patient_by_id.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/sync/test_fhir_client_patient_delete.py` & `helix.fhir.client.sdk-2.0.7/tests/sync/test_fhir_client_patient_delete.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/sync/test_fhir_client_patient_list.py` & `helix.fhir.client.sdk-2.0.7/tests/sync/test_fhir_client_patient_list.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/sync/test_fhir_client_patient_list_auth_fail.py` & `helix.fhir.client.sdk-2.0.7/tests/sync/test_fhir_client_patient_list_auth_fail.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/sync/test_fhir_client_patient_list_auth_fail_retry.py` & `helix.fhir.client.sdk-2.0.7/tests/sync/test_fhir_client_patient_list_auth_fail_retry.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/sync/test_fhir_client_patient_list_ids.py` & `helix.fhir.client.sdk-2.0.7/tests/sync/test_fhir_client_patient_list_ids.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/sync/test_fhir_client_patient_list_in_batches.py` & `helix.fhir.client.sdk-2.0.7/tests/sync/test_fhir_client_patient_list_in_batches.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/sync/test_fhir_client_patient_merge.py` & `helix.fhir.client.sdk-2.0.7/tests/sync/test_fhir_client_patient_merge.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/sync/test_fhir_client_patient_update.py` & `helix.fhir.client.sdk-2.0.7/tests/sync/test_fhir_client_patient_update.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/sync/test_fhir_client_patient_update_patch.py` & `helix.fhir.client.sdk-2.0.7/tests/sync/test_fhir_client_patient_update_patch.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests/test_get_nested_property.py` & `helix.fhir.client.sdk-2.0.7/tests/test_get_nested_property.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests_integration/test_aetna_server_auth.py` & `helix.fhir.client.sdk-2.0.7/tests_integration/test_aetna_server_auth.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests_integration/test_aetna_server_auth_aiohttp.py` & `helix.fhir.client.sdk-2.0.7/tests_integration/test_aetna_server_auth_aiohttp.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests_integration/test_aetna_server_auth_httpx.py` & `helix.fhir.client.sdk-2.0.7/tests_integration/test_aetna_server_auth_httpx.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests_integration/test_dev_server_auth.py` & `helix.fhir.client.sdk-2.0.7/tests_integration/test_dev_server_auth.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests_integration/test_dev_server_get_patients.py` & `helix.fhir.client.sdk-2.0.7/tests_integration/test_dev_server_get_patients.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests_integration/test_dev_server_get_patients_error.py` & `helix.fhir.client.sdk-2.0.7/tests_integration/test_dev_server_get_patients_error.py`

 * *Files identical despite different names*

### Comparing `helix.fhir.client.sdk-2.0.6/tests_integration/test_staging_server_graph.py` & `helix.fhir.client.sdk-2.0.7/tests_integration/test_staging_server_graph.py`

 * *Files identical despite different names*

