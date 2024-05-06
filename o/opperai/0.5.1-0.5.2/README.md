# Comparing `tmp/opperai-0.5.1.tar.gz` & `tmp/opperai-0.5.2.tar.gz`

## Comparing `opperai-0.5.1.tar` & `opperai-0.5.2.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 opperai-0.5.1/pytest.ini
--rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 opperai-0.5.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 opperai-0.5.1/src/opperai/__init__.py
--rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 opperai-0.5.1/src/opperai/_client.py
--rw-r--r--   0        0        0     4314 2020-02-02 00:00:00.000000 opperai-0.5.1/src/opperai/functions.py
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 opperai-0.5.1/src/opperai/indexes.py
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 opperai-0.5.1/src/opperai/spans.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 opperai-0.5.1/src/opperai/core/_http_clients.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.5.1/src/opperai/core/functions/__init__.py
--rw-r--r--   0        0        0     6556 2020-02-02 00:00:00.000000 opperai-0.5.1/src/opperai/core/functions/_async_functions.py
--rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 opperai-0.5.1/src/opperai/core/functions/_functions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.5.1/src/opperai/core/functions/decorator/__init__.py
--rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 opperai-0.5.1/src/opperai/core/functions/decorator/_decorator.py
--rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 opperai-0.5.1/src/opperai/core/functions/decorator/_schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.5.1/src/opperai/core/indexes/__init__.py
--rw-r--r--   0        0        0     5136 2020-02-02 00:00:00.000000 opperai-0.5.1/src/opperai/core/indexes/_async_indexes.py
--rw-r--r--   0        0        0     5077 2020-02-02 00:00:00.000000 opperai-0.5.1/src/opperai/core/indexes/_indexes.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 opperai-0.5.1/src/opperai/core/spans/__init__.py
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 opperai-0.5.1/src/opperai/core/spans/_async_spans.py
--rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 opperai-0.5.1/src/opperai/core/spans/_decorator.py
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 opperai-0.5.1/src/opperai/core/spans/_spans.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 opperai-0.5.1/src/opperai/core/utils/__init__.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 opperai-0.5.1/src/opperai/types/__init__.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 opperai-0.5.1/src/opperai/types/exceptions.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 opperai-0.5.1/src/opperai/types/indexes.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 opperai-0.5.1/src/opperai/types/spans.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 opperai-0.5.1/src/opperai/types/validators.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/conftest.py
--rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/test_async_functions.py
--rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/test_async_indexes.py
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/test_async_spans.py
--rw-r--r--   0        0        0     6083 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/test_decorator.py
--rw-r--r--   0        0        0     8185 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/test_functions.py
--rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/test_indexes.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/test_spans.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/test_trace_decorator.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/test_types.py
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat.yaml
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat_stream.yaml
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml
--rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache.yaml
--rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache_flush.yaml
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function.yaml
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_functions/test_failed_structured_generation.yaml
--rw-r--r--   0        0        0     3899 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_functions/test_get.yaml
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_id.yaml
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_path.yaml
--rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_functions/test_update_function.yaml
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_create_index.yaml
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_delete_index.yaml
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_id.yaml
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_name.yaml
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_index_document.yaml
--rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_list_indexes.yaml
--rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_document.yaml
--rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_filters.yaml
--rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_spans/test_save_metric.yaml
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_functions/test_chat.yaml
--rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_functions/test_chat_stream.yaml
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_functions/test_create_function.yaml
--rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache_flush.yaml
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_id.yaml
--rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_path.yaml
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_functions/test_failed_structured_generation.yaml
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_functions/test_get_by_id.yaml
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_functions/test_get_by_path.yaml
--rw-r--r--   0        0        0     5892 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_functions/test_update_function.yaml
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_indexes/test_create_index.yaml
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_indexes/test_delete_index.yaml
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_id.yaml
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_name.yaml
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_indexes/test_index_document.yaml
--rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_indexes/test_list_indexes.yaml
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_document.yaml
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_filters.yaml
--rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 opperai-0.5.1/tests/fixtures/vcr_cassettes/test_spans/test_crud.yaml
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 opperai-0.5.1/.gitignore
--rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 opperai-0.5.1/LICENSE
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 opperai-0.5.1/README.md
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 opperai-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 opperai-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 opperai-0.5.2/pytest.ini
+-rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 opperai-0.5.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/__init__.py
+-rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/_client.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/functions.py
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/indexes.py
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/spans.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/core/_http_clients.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/core/functions/__init__.py
+-rw-r--r--   0        0        0     6556 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/core/functions/_async_functions.py
+-rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/core/functions/_functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/core/functions/decorator/__init__.py
+-rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/core/functions/decorator/_decorator.py
+-rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/core/functions/decorator/_schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/core/indexes/__init__.py
+-rw-r--r--   0        0        0     5136 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/core/indexes/_async_indexes.py
+-rw-r--r--   0        0        0     5077 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/core/indexes/_indexes.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/core/spans/__init__.py
+-rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/core/spans/_async_spans.py
+-rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/core/spans/_decorator.py
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/core/spans/_spans.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/core/utils/__init__.py
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/types/__init__.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/types/exceptions.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/types/indexes.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/types/spans.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/types/validators.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/conftest.py
+-rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/test_async_functions.py
+-rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/test_async_indexes.py
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/test_async_spans.py
+-rw-r--r--   0        0        0     6083 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/test_decorator.py
+-rw-r--r--   0        0        0     8185 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/test_functions.py
+-rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/test_indexes.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/test_spans.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/test_trace_decorator.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/test_types.py
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat.yaml
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat_stream.yaml
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml
+-rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache.yaml
+-rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache_flush.yaml
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function.yaml
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_failed_structured_generation.yaml
+-rw-r--r--   0        0        0     3899 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_get.yaml
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_id.yaml
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_path.yaml
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_update_function.yaml
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_create_index.yaml
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_delete_index.yaml
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_id.yaml
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_name.yaml
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_index_document.yaml
+-rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_list_indexes.yaml
+-rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_document.yaml
+-rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_filters.yaml
+-rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_spans/test_save_metric.yaml
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_chat.yaml
+-rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_chat_stream.yaml
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_create_function.yaml
+-rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml
+-rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache_flush.yaml
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_id.yaml
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_path.yaml
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_failed_structured_generation.yaml
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_get_by_id.yaml
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_get_by_path.yaml
+-rw-r--r--   0        0        0     5892 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_update_function.yaml
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_indexes/test_create_index.yaml
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_indexes/test_delete_index.yaml
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_id.yaml
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_name.yaml
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_indexes/test_index_document.yaml
+-rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_indexes/test_list_indexes.yaml
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_document.yaml
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_filters.yaml
+-rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_spans/test_crud.yaml
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 opperai-0.5.2/.gitignore
+-rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 opperai-0.5.2/LICENSE
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 opperai-0.5.2/README.md
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 opperai-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 opperai-0.5.2/PKG-INFO
```

### Comparing `opperai-0.5.1/.github/workflows/publish.yml` & `opperai-0.5.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/src/opperai/_client.py` & `opperai-0.5.2/src/opperai/_client.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/src/opperai/functions.py` & `opperai-0.5.2/src/opperai/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,50 +65,56 @@
         self._function = updated_function
 
         return self
 
 
 @dataclass
 class Functions:
-    _client: Client = Client()
+    _client: Client = None
+
+    def __init__(self, client: Client = None):
+        if client is None:
+            client = Client()
+
+        self._client = client
 
     def create(
         self,
         path: str,
+        instructions: str,
         description: Optional[str] = None,
         input_type: Optional[Any] = None,
         output_type: Optional[Any] = None,
-        instructions: Optional[str] = None,
         model: Optional[str] = None,
     ) -> Function:
         try:
             function = self.get(path=path)
             if function:
                 return function.update(
+                    instructions=instructions,
                     description=description,
                     input_type=input_type,
                     output_type=output_type,
-                    instructions=instructions,
                     model=model,
                 )
         except Exception:
             pass
 
         if input_type:
             input_schema = type_to_json_schema(input_type)
         if output_type:
             output_schema = type_to_json_schema(output_type)
 
         function = self._client.functions.create(
             FunctionModel(
                 path=path,
+                instructions=instructions,
                 description=description,
                 input_schema=input_schema if input_type else None,
                 out_schema=output_schema if output_type else None,
-                instructions=instructions,
                 model=model,
             )
         )
 
         return Function(self._client, function)
 
     def get(self, id: int = None, path: str = None) -> Optional[Function]:
```

### Comparing `opperai-0.5.1/src/opperai/indexes.py` & `opperai-0.5.2/src/opperai/indexes.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,59 +8,75 @@
 
 @dataclass
 class Index:
     _client: Client
     _index: IndexModel
 
     def upload_file(self, file_path: str, **kwargs):
+        """Upload a file to the index."""
         return self._client.indexes.upload_file(
             id=self._index.id, file_path=file_path, **kwargs
         )
 
     def index(self, doc: Document) -> Document:
+        """Index a document."""
         return self._client.indexes.index(id=self._index.id, doc=doc)
 
     def query(
         self, query: str, k: int = 10, filters: List[Filter] = None
     ) -> List[RetrievalResponse]:
+        """Retrieve documents from the index."""
+
         return self._client.indexes.retrieve(
             id=self._index.id, query=query, k=k, filters=filters
         )
 
     def delete(self) -> bool:
+        """Delete the index."""
         return self._client.indexes.delete(id=self._index.id)
 
 
-@dataclass
 class Indexes:
-    _client: Client = Client()
+    _client: Client = None
+
+    def __init__(self, client: Client = None):
+        if client is None:
+            client = Client()
+
+        self._client = client
 
     def create(self, name: str) -> Index:
+        """Create an index with the given name.
+        If an index with the given name already exists, return it.
+        """
         try:
             index = self.get(name=name)
             if index:
                 return index
         except Exception:
             pass
 
         index = self._client.indexes.create(name=name)
         return Index(self._client, index)
 
     def get(self, id: int = None, name: str = None) -> Optional[Index]:
+        """Get an index by id or name."""
         if id is not None:
             index = self._client.indexes.get(id=id)
         elif name is not None:
             index = self._client.indexes.get(name=name)
         else:
             raise ValueError("Either id or name must be provided")
 
         if not index:
             return None
 
         return Index(self._client, index)
 
     def delete(self, id: int) -> bool:
+        """Delete an index by id."""
         return self._client.indexes.delete(id=id)
 
     def list(self) -> List[Index]:
+        """List all indexes for the organization owning the API key."""
         indexes = self._client.indexes.list()
         return [Index(self._client, index) for index in indexes]
```

### Comparing `opperai-0.5.1/src/opperai/spans.py` & `opperai-0.5.2/src/opperai/spans.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,17 +29,22 @@
                 dimension=dimension,
                 value=value,
                 comment=comment,
             ),
         )
 
 
-@dataclass
 class Spans:
-    _client: Client = Client()
+    _client: Client = None
+
+    def __init__(self, client: Client = None):
+        if client is None:
+            client = Client()
+
+        self._client = client
 
     @contextmanager
     def start(
         self,
         project: str,
         name: str,
         input: str = None,
```

### Comparing `opperai-0.5.1/src/opperai/core/_http_clients.py` & `opperai-0.5.2/src/opperai/core/_http_clients.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/src/opperai/core/functions/_async_functions.py` & `opperai-0.5.2/src/opperai/core/functions/_async_functions.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/src/opperai/core/functions/_functions.py` & `opperai-0.5.2/src/opperai/core/functions/_functions.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/src/opperai/core/functions/decorator/_decorator.py` & `opperai-0.5.2/src/opperai/core/functions/decorator/_decorator.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/src/opperai/core/functions/decorator/_schemas.py` & `opperai-0.5.2/src/opperai/core/functions/decorator/_schemas.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/src/opperai/core/indexes/_async_indexes.py` & `opperai-0.5.2/src/opperai/core/indexes/_async_indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/src/opperai/core/indexes/_indexes.py` & `opperai-0.5.2/src/opperai/core/indexes/_indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/src/opperai/core/spans/_async_spans.py` & `opperai-0.5.2/src/opperai/core/spans/_async_spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/src/opperai/core/spans/_decorator.py` & `opperai-0.5.2/src/opperai/core/spans/_decorator.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/src/opperai/core/spans/_spans.py` & `opperai-0.5.2/src/opperai/core/spans/_spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/src/opperai/core/utils/__init__.py` & `opperai-0.5.2/src/opperai/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/src/opperai/types/__init__.py` & `opperai-0.5.2/src/opperai/types/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ruff: noqa: F401
 from typing import Any, Dict, List, Optional, Union
 from uuid import UUID
 
 from pydantic import BaseModel, ConfigDict, Field
 
-from .indexes import Document
+from .indexes import Document, Filter, RetrievalResponse
 from .spans import SpanMetric
 from .validators import validate_id_xor_path
 
 
 class Message(BaseModel):
     role: str
     content: str
@@ -56,15 +56,15 @@
 class Function(BaseModel):
     id: Optional[int] = None
     path: str = Field(
         ...,
         pattern=r"^[a-zA-Z0-9_]+(\/[a-zA-Z0-9_-]+)*$",
         description="Path should not contain characters that could break URLs.",
     )
-    description: str
+    description: Optional[str] = None
     input_schema: Optional[Dict[str, Any]] = None
     out_schema: Optional[Dict[str, Any]] = None
     instructions: str
     model: Optional[str] = None
     index_ids: Optional[List[int]] = []
     use_semantic_search: Optional[bool] = None
     few_shot: Optional[bool] = None
```

### Comparing `opperai-0.5.1/src/opperai/types/indexes.py` & `opperai-0.5.2/src/opperai/types/indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/src/opperai/types/spans.py` & `opperai-0.5.2/src/opperai/types/spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/src/opperai/types/validators.py` & `opperai-0.5.2/src/opperai/types/validators.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/conftest.py` & `opperai-0.5.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/test_async_functions.py` & `opperai-0.5.2/tests/test_async_functions.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/test_async_indexes.py` & `opperai-0.5.2/tests/test_async_indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/test_async_spans.py` & `opperai-0.5.2/tests/test_async_spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/test_decorator.py` & `opperai-0.5.2/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/test_functions.py` & `opperai-0.5.2/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/test_indexes.py` & `opperai-0.5.2/tests/test_indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/test_spans.py` & `opperai-0.5.2/tests/test_spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/test_trace_decorator.py` & `opperai-0.5.2/tests/test_trace_decorator.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/test_types.py` & `opperai-0.5.2/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat_stream.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat_stream.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache_flush.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache_flush.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_functions/test_failed_structured_generation.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_failed_structured_generation.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_functions/test_get.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_get.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_id.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_id.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_path.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_path.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_functions/test_update_function.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_update_function.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_create_index.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_create_index.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_delete_index.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_delete_index.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_id.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_id.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_name.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_name.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_index_document.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_index_document.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_list_indexes.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_list_indexes.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_document.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_document.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_filters.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_filters.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_async_spans/test_save_metric.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_spans/test_save_metric.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_functions/test_chat.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_chat.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_functions/test_chat_stream.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_chat_stream.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_functions/test_create_function.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_create_function.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache_flush.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache_flush.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_id.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_id.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_path.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_path.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_functions/test_failed_structured_generation.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_failed_structured_generation.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_functions/test_get_by_id.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_get_by_id.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_functions/test_get_by_path.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_get_by_path.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_functions/test_update_function.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_update_function.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_indexes/test_create_index.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_indexes/test_create_index.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_indexes/test_delete_index.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_indexes/test_delete_index.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_id.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_id.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_name.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_name.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_indexes/test_index_document.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_indexes/test_index_document.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_indexes/test_list_indexes.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_indexes/test_list_indexes.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_document.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_document.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_filters.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_filters.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/tests/fixtures/vcr_cassettes/test_spans/test_crud.yaml` & `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_spans/test_crud.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/LICENSE` & `opperai-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/README.md` & `opperai-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `opperai-0.5.1/pyproject.toml` & `opperai-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "opperai"
-version = "0.5.1"
+version = "0.5.2"
 description = "Opper Python client"
 authors = [
   {name = "Opper", email = "opper@opper.ai"},
 ]
 
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `opperai-0.5.1/PKG-INFO` & `opperai-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: opperai
-Version: 0.5.1
+Version: 0.5.2
 Summary: Opper Python client
 Project-URL: Homepage, https://opper.ai
 Project-URL: Documentation, https://docs.opper.ai
 Project-URL: Platform, https://platform.opper.ai
 Author-email: Opper <opper@opper.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

