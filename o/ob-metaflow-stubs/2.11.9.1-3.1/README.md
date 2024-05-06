# Comparing `tmp/ob-metaflow-stubs-2.11.9.1.tar.gz` & `tmp/ob-metaflow-stubs-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ob-metaflow-stubs-2.11.9.1.tar", last modified: Sat Mar 30 09:14:02 2024, max compression
+gzip compressed data, was "ob-metaflow-stubs-3.1.tar", last modified: Mon May  6 19:56:37 2024, max compression
```

## Comparing `ob-metaflow-stubs-2.11.9.1.tar` & `ob-metaflow-stubs-3.1.tar`

### file list

```diff
@@ -1,165 +1,166 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.624047 ob-metaflow-stubs-2.11.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-30 09:13:40.000000 ob-metaflow-stubs-2.11.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-30 09:14:02.624047 ob-metaflow-stubs-2.11.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-30 09:13:40.000000 ob-metaflow-stubs-2.11.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.604047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)   107562 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/cards.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/cli.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.604047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/client/
--rw-r--r--   0 runner    (1001) docker     (127)    28941 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/client/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    40806 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/client/core.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/client/filecache.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/clone_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/events.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/exception.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/flowspec.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/generated_for.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18152 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/includefile.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.604047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)    12396 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/metadata/metadata.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/metadata/util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/metaflow_config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/metaflow_current.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.604047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/mflog/
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/mflog/mflog.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/multicore_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/parameters.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.608047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.608047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/airflow.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/airflow_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/airflow_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/airflow_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/exception.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.608047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/sensors/
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/sensors/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.608047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/argo/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/argo/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/argo/argo_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/argo/argo_events.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14373 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/argo/argo_workflows.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.612047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/aws_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/aws_utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.612047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/batch/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/batch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/batch/batch.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/batch/batch_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/batch/batch_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.612047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/secrets_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/secrets_manager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.612047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/step_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/step_functions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/step_functions/dynamo_db_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/step_functions/event_bridge_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/step_functions/production_token.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/step_functions/schedule_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.616047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/azure/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/azure/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/azure/azure_credential.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/azure/azure_exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/azure/azure_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/azure/includefile_support.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.616047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    18088 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_creator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_datastore.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.616047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/basic.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/card.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.620047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/chevron/
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/chevron/metadata.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/components.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/convert_to_native_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/renderer_tools.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_resolver.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/component_serializer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/exception.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/catch_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.620047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/datatools/
--rw-r--r--   0 runner    (1001) docker     (127)    12909 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/datatools/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/datatools/local.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.620047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/datatools/s3/
--rw-r--r--   0 runner    (1001) docker     (127)    20310 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/datatools/s3/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    29021 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/datatools/s3/s3.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/datatools/s3/s3tail.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/datatools/s3/s3util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/debug_logger.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/debug_monitor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/environment_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/events_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.620047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/frameworks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/frameworks/pytorch.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.620047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/gcp/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/gcp/gcp_secret_manager_secrets_provider.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/gcp/gs_exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/gcp/gs_storage_client_factory.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/gcp/gs_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/gcp/includefile_support.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.620047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/kubernetes/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/kubernetes/kubernetes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/kubernetes/kubernetes_job.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/package_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/parallel_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/project_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.624047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/pypi/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/pypi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/pypi/conda_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/pypi/conda_environment.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/pypi/pypi_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/pypi/pypi_environment.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/pypi/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/resources_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/retry_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.624047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/secrets/
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/secrets/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/secrets/secrets_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/storage_executor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/tag_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/timeout_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/procpoll.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/pylint_wrapper.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/tagging_util.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.624047 ob-metaflow-stubs-2.11.9.1/ob_metaflow_stubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-30 09:14:02.000000 ob-metaflow-stubs-2.11.9.1/ob_metaflow_stubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-03-30 09:14:02.000000 ob-metaflow-stubs-2.11.9.1/ob_metaflow_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 09:14:02.000000 ob-metaflow-stubs-2.11.9.1/ob_metaflow_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-30 09:14:02.000000 ob-metaflow-stubs-2.11.9.1/ob_metaflow_stubs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-30 09:14:02.000000 ob-metaflow-stubs-2.11.9.1/ob_metaflow_stubs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 09:14:02.624047 ob-metaflow-stubs-2.11.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-30 09:13:40.000000 ob-metaflow-stubs-2.11.9.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-30 09:14:02.000000 ob-metaflow-stubs-2.11.9.1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:56:37.008879 ob-metaflow-stubs-3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-06 19:56:18.000000 ob-metaflow-stubs-3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-06 19:56:37.008879 ob-metaflow-stubs-3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-06 19:56:18.000000 ob-metaflow-stubs-3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:56:36.992879 ob-metaflow-stubs-3.1/metaflow-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)   107671 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/cards.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/cli.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:56:36.992879 ob-metaflow-stubs-3.1/metaflow-stubs/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    28941 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/client/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    40806 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/client/core.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/client/filecache.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/clone_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/events.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/exception.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/flowspec.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/generated_for.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18152 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/includefile.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:56:36.992879 ob-metaflow-stubs-3.1/metaflow-stubs/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)    12396 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/metadata/metadata.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/metadata/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/metaflow_config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/metaflow_current.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:56:36.992879 ob-metaflow-stubs-3.1/metaflow-stubs/mflog/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/mflog/mflog.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/multicore_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/parameters.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:56:36.996879 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:56:36.996879 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/airflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/airflow/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/airflow/airflow.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/airflow/airflow_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/airflow/airflow_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/airflow/airflow_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/airflow/exception.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:56:36.996879 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/airflow/sensors/
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/airflow/sensors/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:56:36.996879 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/argo/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/argo/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/argo/argo_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/argo/argo_events.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14373 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/argo/argo_workflows.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:56:36.996879 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/aws/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/aws/aws_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/aws/aws_utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:56:36.996879 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/aws/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/aws/batch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/aws/batch/batch.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/aws/batch/batch_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/aws/batch/batch_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:56:37.000879 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/aws/secrets_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/aws/secrets_manager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:56:37.000879 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/aws/step_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/aws/step_functions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/aws/step_functions/dynamo_db_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/aws/step_functions/event_bridge_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/aws/step_functions/production_token.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/aws/step_functions/schedule_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:56:37.000879 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/azure/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/azure/azure_credential.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/azure/azure_exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/azure/azure_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/azure/includefile_support.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:56:37.004879 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18088 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/card_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/card_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/card_creator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/card_datastore.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/card_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:56:37.004879 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/card_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/card_modules/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/card_modules/basic.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/card_modules/card.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:56:37.004879 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/card_modules/chevron/
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/card_modules/chevron/metadata.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/card_modules/components.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/card_modules/convert_to_native_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/card_modules/renderer_tools.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/card_resolver.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/component_serializer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/exception.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/catch_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:56:37.004879 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/datatools/
+-rw-r--r--   0 runner    (1001) docker     (127)    12909 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/datatools/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/datatools/local.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:56:37.004879 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/datatools/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)    20310 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/datatools/s3/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    29021 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/datatools/s3/s3.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/datatools/s3/s3tail.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/datatools/s3/s3util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/debug_logger.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/debug_monitor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/environment_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/events_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:56:37.004879 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/frameworks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/frameworks/pytorch.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:56:37.008879 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/gcp/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/gcp/gcp_secret_manager_secrets_provider.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/gcp/gs_exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/gcp/gs_storage_client_factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/gcp/gs_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/gcp/includefile_support.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:56:37.008879 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/kubernetes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/kubernetes/kubernetes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/package_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/parallel_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/perimeters.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/project_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:56:37.008879 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/pypi/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/pypi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/pypi/conda_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/pypi/conda_environment.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/pypi/pypi_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/pypi/pypi_environment.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/pypi/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/resources_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/retry_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:56:37.008879 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/secrets/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/secrets/secrets_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/storage_executor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/tag_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/plugins/timeout_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/procpoll.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:56:37.008879 ob-metaflow-stubs-3.1/metaflow-stubs/profilers/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/profilers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/pylint_wrapper.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-06 19:56:35.000000 ob-metaflow-stubs-3.1/metaflow-stubs/tagging_util.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:56:37.008879 ob-metaflow-stubs-3.1/ob_metaflow_stubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-06 19:56:36.000000 ob-metaflow-stubs-3.1/ob_metaflow_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-05-06 19:56:36.000000 ob-metaflow-stubs-3.1/ob_metaflow_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 19:56:36.000000 ob-metaflow-stubs-3.1/ob_metaflow_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-06 19:56:36.000000 ob-metaflow-stubs-3.1/ob_metaflow_stubs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 19:56:37.008879 ob-metaflow-stubs-3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-06 19:56:18.000000 ob-metaflow-stubs-3.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-06 19:56:18.000000 ob-metaflow-stubs-3.1/version.py
```

### Comparing `ob-metaflow-stubs-2.11.9.1/PKG-INFO` & `ob-metaflow-stubs-3.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: ob-metaflow-stubs
-Version: 2.11.9.1
+Version: 3.1
 Summary: Metaflow Stubs: Stubs for the metaflow package
 Author: Netflix, Outerbounds & the Metaflow Community
 Author-email: help@outerbounds.co
 License: Apache License 2.0
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
-Requires-Dist: ob-metaflow==2.11.9.1
 
 # Metaflow Stubs
 
 This package contains stub files for `metaflow` and thus offers type hints for various editors (such as `VSCode`) and language servers (such as `Pylance`).
 
 ## Installation
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/__init__.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:00.953272                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.236170                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.parameters
-    import metaflow.datastore.inputs
     import metaflow.client.core
-    import metaflow.events
-    import metaflow.plugins.datatools.s3.s3
-    import io
+    import metaflow.parameters
+    import metaflow.metaflow_current
     import datetime
-    import typing
     import metaflow._vendor.click.types
-    import metaflow.metaflow_current
+    import metaflow.events
+    import typing
+    import io
+    import metaflow.datastore.inputs
+    import metaflow.plugins.datatools.s3.s3
 FlowSpecDerived = typing.TypeVar("FlowSpecDerived", bound="FlowSpec", contravariant=False, covariant=False)
 StepFlag = typing.NewType("StepFlag", bool)
 
 CURRENT_DIRECTORY: str
 
 INFO_FILE: str
 
@@ -722,14 +722,124 @@
     -------
     Union[Callable[[FlowSpecDerived, StepFlag], None], Callable[[FlowSpecDerived, Any, StepFlag], None]]
         Function that is a Metaflow Step
     """
     ...
 
 @typing.overload
+def timeout(*, seconds: int = 0, minutes: int = 0, hours: int = 0) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+    """
+    Specifies a timeout for your step.
+    
+    This decorator is useful if this step may hang indefinitely.
+    
+    This can be used in conjunction with the `@retry` decorator as well as the `@catch` decorator.
+    A timeout is considered to be an exception thrown by the step. It will cause the step to be
+    retried if needed and the exception will be caught by the `@catch` decorator, if present.
+    
+    Note that all the values specified in parameters are added together so if you specify
+    60 seconds and 1 hour, the decorator will have an effective timeout of 1 hour and 1 minute.
+    
+    Parameters
+    ----------
+    seconds : int, default 0
+        Number of seconds to wait prior to timing out.
+    minutes : int, default 0
+        Number of minutes to wait prior to timing out.
+    hours : int, default 0
+        Number of hours to wait prior to timing out.
+    """
+    ...
+
+@typing.overload
+def timeout(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+    ...
+
+@typing.overload
+def timeout(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+    ...
+
+def timeout(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, seconds: int = 0, minutes: int = 0, hours: int = 0):
+    """
+    Specifies a timeout for your step.
+    
+    This decorator is useful if this step may hang indefinitely.
+    
+    This can be used in conjunction with the `@retry` decorator as well as the `@catch` decorator.
+    A timeout is considered to be an exception thrown by the step. It will cause the step to be
+    retried if needed and the exception will be caught by the `@catch` decorator, if present.
+    
+    Note that all the values specified in parameters are added together so if you specify
+    60 seconds and 1 hour, the decorator will have an effective timeout of 1 hour and 1 minute.
+    
+    Parameters
+    ----------
+    seconds : int, default 0
+        Number of seconds to wait prior to timing out.
+    minutes : int, default 0
+        Number of minutes to wait prior to timing out.
+    hours : int, default 0
+        Number of hours to wait prior to timing out.
+    """
+    ...
+
+@typing.overload
+def retry(*, times: int = 3, minutes_between_retries: int = 2) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+    """
+    Specifies the number of times the task corresponding
+    to a step needs to be retried.
+    
+    This decorator is useful for handling transient errors, such as networking issues.
+    If your task contains operations that can't be retried safely, e.g. database updates,
+    it is advisable to annotate it with `@retry(times=0)`.
+    
+    This can be used in conjunction with the `@catch` decorator. The `@catch`
+    decorator will execute a no-op task after all retries have been exhausted,
+    ensuring that the flow execution can continue.
+    
+    Parameters
+    ----------
+    times : int, default 3
+        Number of times to retry this task.
+    minutes_between_retries : int, default 2
+        Number of minutes between retries.
+    """
+    ...
+
+@typing.overload
+def retry(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+    ...
+
+@typing.overload
+def retry(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+    ...
+
+def retry(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, times: int = 3, minutes_between_retries: int = 2):
+    """
+    Specifies the number of times the task corresponding
+    to a step needs to be retried.
+    
+    This decorator is useful for handling transient errors, such as networking issues.
+    If your task contains operations that can't be retried safely, e.g. database updates,
+    it is advisable to annotate it with `@retry(times=0)`.
+    
+    This can be used in conjunction with the `@catch` decorator. The `@catch`
+    decorator will execute a no-op task after all retries have been exhausted,
+    ensuring that the flow execution can continue.
+    
+    Parameters
+    ----------
+    times : int, default 3
+        Number of times to retry this task.
+    minutes_between_retries : int, default 2
+        Number of minutes between retries.
+    """
+    ...
+
+@typing.overload
 def resources(*, cpu: int = 1, gpu: int = 0, disk: typing.Optional[int] = None, memory: int = 4096, shared_memory: typing.Optional[int] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
     Specifies the resources needed when executing this step.
     
     Use `@resources` to specify the resource requirements
     independently of the specific compute layer (`@batch`, `@kubernetes`).
     
@@ -799,120 +909,206 @@
     shared_memory : int, optional, default None
         The value for the size (in MiB) of the /dev/shm volume for this step.
         This parameter maps to the `--shm-size` option in Docker.
     """
     ...
 
 @typing.overload
-def retry(*, times: int = 3, minutes_between_retries: int = 2) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def conda(*, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Specifies the number of times the task corresponding
-    to a step needs to be retried.
-    
-    This decorator is useful for handling transient errors, such as networking issues.
-    If your task contains operations that can't be retried safely, e.g. database updates,
-    it is advisable to annotate it with `@retry(times=0)`.
+    Specifies the Conda environment for the step.
     
-    This can be used in conjunction with the `@catch` decorator. The `@catch`
-    decorator will execute a no-op task after all retries have been exhausted,
-    ensuring that the flow execution can continue.
+    Information in this decorator will augment any
+    attributes set in the `@conda_base` flow-level decorator. Hence,
+    you can use `@conda_base` to set packages required by all
+    steps and use `@conda` to specify step-specific overrides.
     
     Parameters
     ----------
-    times : int, default 3
-        Number of times to retry this task.
-    minutes_between_retries : int, default 2
-        Number of minutes between retries.
+    packages : Dict[str, str], default {}
+        Packages to use for this step. The key is the name of the package
+        and the value is the version to use.
+    libraries : Dict[str, str], default {}
+        Supported for backward compatibility. When used with packages, packages will take precedence.
+    python : str, optional, default None
+        Version of Python to use, e.g. '3.7.4'. A default value of None implies
+        that the version used will correspond to the version of the Python interpreter used to start the run.
+    disabled : bool, default False
+        If set to True, disables @conda.
     """
     ...
 
 @typing.overload
-def retry(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def conda(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
 @typing.overload
-def retry(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+def conda(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
     ...
 
-def retry(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, times: int = 3, minutes_between_retries: int = 2):
+def conda(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False):
     """
-    Specifies the number of times the task corresponding
-    to a step needs to be retried.
-    
-    This decorator is useful for handling transient errors, such as networking issues.
-    If your task contains operations that can't be retried safely, e.g. database updates,
-    it is advisable to annotate it with `@retry(times=0)`.
+    Specifies the Conda environment for the step.
     
-    This can be used in conjunction with the `@catch` decorator. The `@catch`
-    decorator will execute a no-op task after all retries have been exhausted,
-    ensuring that the flow execution can continue.
+    Information in this decorator will augment any
+    attributes set in the `@conda_base` flow-level decorator. Hence,
+    you can use `@conda_base` to set packages required by all
+    steps and use `@conda` to specify step-specific overrides.
     
     Parameters
     ----------
-    times : int, default 3
-        Number of times to retry this task.
-    minutes_between_retries : int, default 2
-        Number of minutes between retries.
+    packages : Dict[str, str], default {}
+        Packages to use for this step. The key is the name of the package
+        and the value is the version to use.
+    libraries : Dict[str, str], default {}
+        Supported for backward compatibility. When used with packages, packages will take precedence.
+    python : str, optional, default None
+        Version of Python to use, e.g. '3.7.4'. A default value of None implies
+        that the version used will correspond to the version of the Python interpreter used to start the run.
+    disabled : bool, default False
+        If set to True, disables @conda.
     """
     ...
 
 @typing.overload
-def timeout(*, seconds: int = 0, minutes: int = 0, hours: int = 0) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def pypi(*, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Specifies a timeout for your step.
-    
-    This decorator is useful if this step may hang indefinitely.
-    
-    This can be used in conjunction with the `@retry` decorator as well as the `@catch` decorator.
-    A timeout is considered to be an exception thrown by the step. It will cause the step to be
-    retried if needed and the exception will be caught by the `@catch` decorator, if present.
+    Specifies the PyPI packages for the step.
     
-    Note that all the values specified in parameters are added together so if you specify
-    60 seconds and 1 hour, the decorator will have an effective timeout of 1 hour and 1 minute.
+    Information in this decorator will augment any
+    attributes set in the `@pyi_base` flow-level decorator. Hence,
+    you can use `@pypi_base` to set packages required by all
+    steps and use `@pypi` to specify step-specific overrides.
     
     Parameters
     ----------
-    seconds : int, default 0
-        Number of seconds to wait prior to timing out.
-    minutes : int, default 0
-        Number of minutes to wait prior to timing out.
-    hours : int, default 0
-        Number of hours to wait prior to timing out.
+    packages : Dict[str, str], default: {}
+        Packages to use for this step. The key is the name of the package
+        and the value is the version to use.
+    python : str, optional, default: None
+        Version of Python to use, e.g. '3.7.4'. A default value of None implies
+        that the version used will correspond to the version of the Python interpreter used to start the run.
     """
     ...
 
 @typing.overload
-def timeout(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def pypi(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
 @typing.overload
-def timeout(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+def pypi(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
     ...
 
-def timeout(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, seconds: int = 0, minutes: int = 0, hours: int = 0):
+def pypi(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None):
     """
-    Specifies a timeout for your step.
+    Specifies the PyPI packages for the step.
     
-    This decorator is useful if this step may hang indefinitely.
+    Information in this decorator will augment any
+    attributes set in the `@pyi_base` flow-level decorator. Hence,
+    you can use `@pypi_base` to set packages required by all
+    steps and use `@pypi` to specify step-specific overrides.
     
-    This can be used in conjunction with the `@retry` decorator as well as the `@catch` decorator.
-    A timeout is considered to be an exception thrown by the step. It will cause the step to be
-    retried if needed and the exception will be caught by the `@catch` decorator, if present.
+    Parameters
+    ----------
+    packages : Dict[str, str], default: {}
+        Packages to use for this step. The key is the name of the package
+        and the value is the version to use.
+    python : str, optional, default: None
+        Version of Python to use, e.g. '3.7.4'. A default value of None implies
+        that the version used will correspond to the version of the Python interpreter used to start the run.
+    """
+    ...
+
+@typing.overload
+def environment(*, vars: typing.Dict[str, str] = {}) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+    """
+    Specifies environment variables to be set prior to the execution of a step.
     
-    Note that all the values specified in parameters are added together so if you specify
-    60 seconds and 1 hour, the decorator will have an effective timeout of 1 hour and 1 minute.
+    Parameters
+    ----------
+    vars : Dict[str, str], default {}
+        Dictionary of environment variables to set.
+    """
+    ...
+
+@typing.overload
+def environment(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+    ...
+
+@typing.overload
+def environment(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+    ...
+
+def environment(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, vars: typing.Dict[str, str] = {}):
+    """
+    Specifies environment variables to be set prior to the execution of a step.
     
     Parameters
     ----------
-    seconds : int, default 0
-        Number of seconds to wait prior to timing out.
-    minutes : int, default 0
-        Number of minutes to wait prior to timing out.
-    hours : int, default 0
-        Number of hours to wait prior to timing out.
+    vars : Dict[str, str], default {}
+        Dictionary of environment variables to set.
+    """
+    ...
+
+def kubernetes(*, cpu: int = 1, memory: int = 4096, disk: int = 10240, image: typing.Optional[str] = None, image_pull_policy: str = "KUBERNETES_IMAGE_PULL_POLICY", service_account: str = "METAFLOW_KUBERNETES_SERVICE_ACCOUNT", secrets: typing.Optional[typing.List[str]] = None, namespace: str = "METAFLOW_KUBERNETES_NAMESPACE", gpu: typing.Optional[int] = None, gpu_vendor: str = "KUBERNETES_GPU_VENDOR", tolerations: typing.List[str] = [], use_tmpfs: bool = False, tmpfs_tempdir: bool = True, tmpfs_size: typing.Optional[int] = None, tmpfs_path: typing.Optional[str] = "/metaflow_temp", persistent_volume_claims: typing.Optional[typing.Dict[str, str]] = None, shared_memory: typing.Optional[int] = None, port: typing.Optional[int] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+    """
+    Specifies that this step should execute on Kubernetes.
+    
+    Parameters
+    ----------
+    cpu : int, default 1
+        Number of CPUs required for this step. If `@resources` is
+        also present, the maximum value from all decorators is used.
+    memory : int, default 4096
+        Memory size (in MB) required for this step. If
+        `@resources` is also present, the maximum value from all decorators is
+        used.
+    disk : int, default 10240
+        Disk size (in MB) required for this step. If
+        `@resources` is also present, the maximum value from all decorators is
+        used.
+    image : str, optional, default None
+        Docker image to use when launching on Kubernetes. If not specified, and
+        METAFLOW_KUBERNETES_CONTAINER_IMAGE is specified, that image is used. If
+        not, a default Docker image mapping to the current version of Python is used.
+    image_pull_policy: str, default KUBERNETES_IMAGE_PULL_POLICY
+        If given, the imagePullPolicy to be applied to the Docker image of the step.
+    service_account : str, default METAFLOW_KUBERNETES_SERVICE_ACCOUNT
+        Kubernetes service account to use when launching pod in Kubernetes.
+    secrets : List[str], optional, default None
+        Kubernetes secrets to use when launching pod in Kubernetes. These
+        secrets are in addition to the ones defined in `METAFLOW_KUBERNETES_SECRETS`
+        in Metaflow configuration.
+    namespace : str, default METAFLOW_KUBERNETES_NAMESPACE
+        Kubernetes namespace to use when launching pod in Kubernetes.
+    gpu : int, optional, default None
+        Number of GPUs required for this step. A value of zero implies that
+        the scheduled node should not have GPUs.
+    gpu_vendor : str, default KUBERNETES_GPU_VENDOR
+        The vendor of the GPUs to be used for this step.
+    tolerations : List[str], default []
+        The default is extracted from METAFLOW_KUBERNETES_TOLERATIONS.
+        Kubernetes tolerations to use when launching pod in Kubernetes.
+    use_tmpfs : bool, default False
+        This enables an explicit tmpfs mount for this step.
+    tmpfs_tempdir : bool, default True
+        sets METAFLOW_TEMPDIR to tmpfs_path if set for this step.
+    tmpfs_size : int, optional, default: None
+        The value for the size (in MiB) of the tmpfs mount for this step.
+        This parameter maps to the `--tmpfs` option in Docker. Defaults to 50% of the
+        memory allocated for this step.
+    tmpfs_path : str, optional, default /metaflow_temp
+        Path to tmpfs mount for this step.
+    persistent_volume_claims : Dict[str, str], optional, default None
+        A map (dictionary) of persistent volumes to be mounted to the pod for this step. The map is from persistent
+        volumes to the path to which the volume is to be mounted, e.g., `{'pvc-name': '/path/to/mount/on'}`.
+    shared_memory: int, optional
+        Shared memory size (in MiB) required for this step
+    port: int, optional
+        Port number to specify in the Kubernetes job object
     """
     ...
 
 @typing.overload
 def batch(*, cpu: int = 1, gpu: int = 0, memory: int = 4096, image: typing.Optional[str] = None, queue: str = "METAFLOW_BATCH_JOB_QUEUE", iam_role: str = "METAFLOW_ECS_S3_ACCESS_IAM_ROLE", execution_role: str = "METAFLOW_ECS_FARGATE_EXECUTION_ROLE", shared_memory: typing.Optional[int] = None, max_swap: typing.Optional[int] = None, swappiness: typing.Optional[int] = None, use_tmpfs: bool = False, tmpfs_tempdir: bool = True, tmpfs_size: typing.Optional[int] = None, tmpfs_path: typing.Optional[str] = None, inferentia: int = 0, trainium: int = None, efa: int = 0, ephemeral_storage: int = None, log_driver: typing.Optional[str] = None, log_options: typing.Optional[typing.List[str]] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
     Specifies that this step should execute on [AWS Batch](https://aws.amazon.com/batch/).
@@ -1056,14 +1252,47 @@
         List of strings containing options for the chosen log driver. The configurable values
         depend on the `log driver` chosen. Validation of these options is not supported yet.
         Example usage: ["awslogs-group:aws/batch/job"]
     """
     ...
 
 @typing.overload
+def secrets(*, sources: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = []) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+    """
+    Specifies secrets to be retrieved and injected as environment variables prior to
+    the execution of a step.
+    
+    Parameters
+    ----------
+    sources : List[Union[str, Dict[str, Any]]], default: []
+        List of secret specs, defining how the secrets are to be retrieved
+    """
+    ...
+
+@typing.overload
+def secrets(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+    ...
+
+@typing.overload
+def secrets(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+    ...
+
+def secrets(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, sources: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = []):
+    """
+    Specifies secrets to be retrieved and injected as environment variables prior to
+    the execution of a step.
+    
+    Parameters
+    ----------
+    sources : List[Union[str, Dict[str, Any]]], default: []
+        List of secret specs, defining how the secrets are to be retrieved
+    """
+    ...
+
+@typing.overload
 def card(*, type: str = "default", id: typing.Optional[str] = None, options: typing.Dict[str, typing.Any] = {}, timeout: int = 45) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
     Creates a human-readable report, a Metaflow Card, after this step completes.
     
     Note that you may add multiple `@card` decorators in a step with different parameters.
     
     Parameters
@@ -1155,240 +1384,53 @@
         If not specified, the exception is not stored.
     print_exception : bool, default True
         Determines whether or not the exception is printed to
         stdout when caught.
     """
     ...
 
-@typing.overload
-def secrets(*, sources: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = []) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
-    """
-    Specifies secrets to be retrieved and injected as environment variables prior to
-    the execution of a step.
-    
-    Parameters
-    ----------
-    sources : List[Union[str, Dict[str, Any]]], default: []
-        List of secret specs, defining how the secrets are to be retrieved
-    """
-    ...
-
-@typing.overload
-def secrets(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
-    ...
-
-@typing.overload
-def secrets(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
-    ...
-
-def secrets(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, sources: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = []):
-    """
-    Specifies secrets to be retrieved and injected as environment variables prior to
-    the execution of a step.
-    
-    Parameters
-    ----------
-    sources : List[Union[str, Dict[str, Any]]], default: []
-        List of secret specs, defining how the secrets are to be retrieved
-    """
-    ...
-
-def kubernetes(*, cpu: int = 1, memory: int = 4096, disk: int = 10240, image: typing.Optional[str] = None, image_pull_policy: str = "KUBERNETES_IMAGE_PULL_POLICY", service_account: str = "METAFLOW_KUBERNETES_SERVICE_ACCOUNT", secrets: typing.Optional[typing.List[str]] = None, namespace: str = "METAFLOW_KUBERNETES_NAMESPACE", gpu: typing.Optional[int] = None, gpu_vendor: str = "KUBERNETES_GPU_VENDOR", tolerations: typing.List[str] = [], use_tmpfs: bool = False, tmpfs_tempdir: bool = True, tmpfs_size: typing.Optional[int] = None, tmpfs_path: typing.Optional[str] = "/metaflow_temp", persistent_volume_claims: typing.Optional[typing.Dict[str, str]] = None, port: typing.Optional[int] = None, shared_memory: typing.Optional[int] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
-    """
-    Specifies that this step should execute on Kubernetes.
-    
-    Parameters
-    ----------
-    cpu : int, default 1
-        Number of CPUs required for this step. If `@resources` is
-        also present, the maximum value from all decorators is used.
-    memory : int, default 4096
-        Memory size (in MB) required for this step. If
-        `@resources` is also present, the maximum value from all decorators is
-        used.
-    disk : int, default 10240
-        Disk size (in MB) required for this step. If
-        `@resources` is also present, the maximum value from all decorators is
-        used.
-    image : str, optional, default None
-        Docker image to use when launching on Kubernetes. If not specified, and
-        METAFLOW_KUBERNETES_CONTAINER_IMAGE is specified, that image is used. If
-        not, a default Docker image mapping to the current version of Python is used.
-    image_pull_policy: str, default KUBERNETES_IMAGE_PULL_POLICY
-        If given, the imagePullPolicy to be applied to the Docker image of the step.
-    service_account : str, default METAFLOW_KUBERNETES_SERVICE_ACCOUNT
-        Kubernetes service account to use when launching pod in Kubernetes.
-    secrets : List[str], optional, default None
-        Kubernetes secrets to use when launching pod in Kubernetes. These
-        secrets are in addition to the ones defined in `METAFLOW_KUBERNETES_SECRETS`
-        in Metaflow configuration.
-    namespace : str, default METAFLOW_KUBERNETES_NAMESPACE
-        Kubernetes namespace to use when launching pod in Kubernetes.
-    gpu : int, optional, default None
-        Number of GPUs required for this step. A value of zero implies that
-        the scheduled node should not have GPUs.
-    gpu_vendor : str, default KUBERNETES_GPU_VENDOR
-        The vendor of the GPUs to be used for this step.
-    tolerations : List[str], default []
-        The default is extracted from METAFLOW_KUBERNETES_TOLERATIONS.
-        Kubernetes tolerations to use when launching pod in Kubernetes.
-    use_tmpfs : bool, default False
-        This enables an explicit tmpfs mount for this step.
-    tmpfs_tempdir : bool, default True
-        sets METAFLOW_TEMPDIR to tmpfs_path if set for this step.
-    tmpfs_size : int, optional, default: None
-        The value for the size (in MiB) of the tmpfs mount for this step.
-        This parameter maps to the `--tmpfs` option in Docker. Defaults to 50% of the
-        memory allocated for this step.
-    tmpfs_path : str, optional, default /metaflow_temp
-        Path to tmpfs mount for this step.
-    persistent_volume_claims : Dict[str, str], optional, default None
-        A map (dictionary) of persistent volumes to be mounted to the pod for this step. The map is from persistent
-        volumes to the path to which the volume is to be mounted, e.g., `{'pvc-name': '/path/to/mount/on'}`.
-    port: int, optional
-        Number of the port to specify in the Kubernetes job object
-    shared_memory: int, optional
-        Shared memory size (in MiB) required for this steps
-    """
-    ...
-
-@typing.overload
-def pypi(*, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
-    """
-    Specifies the PyPI packages for the step.
-    
-    Information in this decorator will augment any
-    attributes set in the `@pyi_base` flow-level decorator. Hence,
-    you can use `@pypi_base` to set packages required by all
-    steps and use `@pypi` to specify step-specific overrides.
-    
-    Parameters
-    ----------
-    packages : Dict[str, str], default: {}
-        Packages to use for this step. The key is the name of the package
-        and the value is the version to use.
-    python : str, optional, default: None
-        Version of Python to use, e.g. '3.7.4'. A default value of None implies
-        that the version used will correspond to the version of the Python interpreter used to start the run.
-    """
-    ...
-
-@typing.overload
-def pypi(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
-    ...
-
-@typing.overload
-def pypi(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
-    ...
-
-def pypi(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None):
-    """
-    Specifies the PyPI packages for the step.
-    
-    Information in this decorator will augment any
-    attributes set in the `@pyi_base` flow-level decorator. Hence,
-    you can use `@pypi_base` to set packages required by all
-    steps and use `@pypi` to specify step-specific overrides.
-    
-    Parameters
-    ----------
-    packages : Dict[str, str], default: {}
-        Packages to use for this step. The key is the name of the package
-        and the value is the version to use.
-    python : str, optional, default: None
-        Version of Python to use, e.g. '3.7.4'. A default value of None implies
-        that the version used will correspond to the version of the Python interpreter used to start the run.
-    """
-    ...
-
-@typing.overload
-def conda(*, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
-    """
-    Specifies the Conda environment for the step.
-    
-    Information in this decorator will augment any
-    attributes set in the `@conda_base` flow-level decorator. Hence,
-    you can use `@conda_base` to set packages required by all
-    steps and use `@conda` to specify step-specific overrides.
-    
-    Parameters
-    ----------
-    packages : Dict[str, str], default {}
-        Packages to use for this step. The key is the name of the package
-        and the value is the version to use.
-    libraries : Dict[str, str], default {}
-        Supported for backward compatibility. When used with packages, packages will take precedence.
-    python : str, optional, default None
-        Version of Python to use, e.g. '3.7.4'. A default value of None implies
-        that the version used will correspond to the version of the Python interpreter used to start the run.
-    disabled : bool, default False
-        If set to True, disables @conda.
-    """
-    ...
-
-@typing.overload
-def conda(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
-    ...
-
-@typing.overload
-def conda(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
-    ...
-
-def conda(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False):
-    """
-    Specifies the Conda environment for the step.
-    
-    Information in this decorator will augment any
-    attributes set in the `@conda_base` flow-level decorator. Hence,
-    you can use `@conda_base` to set packages required by all
-    steps and use `@conda` to specify step-specific overrides.
-    
-    Parameters
-    ----------
-    packages : Dict[str, str], default {}
-        Packages to use for this step. The key is the name of the package
-        and the value is the version to use.
-    libraries : Dict[str, str], default {}
-        Supported for backward compatibility. When used with packages, packages will take precedence.
-    python : str, optional, default None
-        Version of Python to use, e.g. '3.7.4'. A default value of None implies
-        that the version used will correspond to the version of the Python interpreter used to start the run.
-    disabled : bool, default False
-        If set to True, disables @conda.
-    """
-    ...
-
-@typing.overload
-def environment(*, vars: typing.Dict[str, str] = {}) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
-    """
-    Specifies environment variables to be set prior to the execution of a step.
-    
-    Parameters
-    ----------
-    vars : Dict[str, str], default {}
-        Dictionary of environment variables to set.
-    """
-    ...
-
-@typing.overload
-def environment(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
-    ...
-
-@typing.overload
-def environment(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
-    ...
-
-def environment(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, vars: typing.Dict[str, str] = {}):
+def airflow_s3_key_sensor(*, timeout: int, poke_interval: int, mode: str, exponential_backoff: bool, pool: str, soft_fail: bool, name: str, description: str, bucket_key: typing.Union[str, typing.List[str]], bucket_name: str, wildcard_match: bool, aws_conn_id: str, verify: bool) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
-    Specifies environment variables to be set prior to the execution of a step.
+    The `@airflow_s3_key_sensor` decorator attaches a Airflow [S3KeySensor](https://airflow.apache.org/docs/apache-airflow-providers-amazon/stable/_api/airflow/providers/amazon/aws/sensors/s3/index.html#airflow.providers.amazon.aws.sensors.s3.S3KeySensor)
+    before the start step of the flow. This decorator only works when a flow is scheduled on Airflow
+    and is compiled using `airflow create`. More than one `@airflow_s3_key_sensor` can be
+    added as a flow decorators. Adding more than one decorator will ensure that `start` step
+    starts only after all sensors finish.
     
     Parameters
     ----------
-    vars : Dict[str, str], default {}
-        Dictionary of environment variables to set.
+    timeout : int
+        Time, in seconds before the task times out and fails. (Default: 3600)
+    poke_interval : int
+        Time in seconds that the job should wait in between each try. (Default: 60)
+    mode : str
+        How the sensor operates. Options are: { poke | reschedule }. (Default: "poke")
+    exponential_backoff : bool
+        allow progressive longer waits between pokes by using exponential backoff algorithm. (Default: True)
+    pool : str
+        the slot pool this task should run in,
+        slot pools are a way to limit concurrency for certain tasks. (Default:None)
+    soft_fail : bool
+        Set to true to mark the task as SKIPPED on failure. (Default: False)
+    name : str
+        Name of the sensor on Airflow
+    description : str
+        Description of sensor in the Airflow UI
+    bucket_key : Union[str, List[str]]
+        The key(s) being waited on. Supports full s3:// style url or relative path from root level.
+        When it's specified as a full s3:// url, please leave `bucket_name` as None
+    bucket_name : str
+        Name of the S3 bucket. Only needed when bucket_key is not provided as a full s3:// url.
+        When specified, all the keys passed to bucket_key refers to this bucket. (Default:None)
+    wildcard_match : bool
+        whether the bucket_key should be interpreted as a Unix wildcard pattern. (Default: False)
+    aws_conn_id : str
+        a reference to the s3 connection on Airflow. (Default: None)
+    verify : bool
+        Whether or not to verify SSL certificates for S3 connection. (Default: None)
     """
     ...
 
 def airflow_external_task_sensor(*, timeout: int, poke_interval: int, mode: str, exponential_backoff: bool, pool: str, soft_fail: bool, name: str, description: str, external_dag_id: str, external_task_ids: typing.List[str], allowed_states: typing.List[str], failed_states: typing.List[str], execution_delta: "datetime.timedelta", check_existence: bool) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
     The `@airflow_external_task_sensor` decorator attaches a Airflow [ExternalTaskSensor](https://airflow.apache.org/docs/apache-airflow/stable/_api/airflow/sensors/external_task/index.html#airflow.sensors.external_task.ExternalTaskSensor) before the start step of the flow.
     This decorator only works when a flow is scheduled on Airflow and is compiled using `airflow create`. More than one `@airflow_external_task_sensor` can be added as a flow decorators. Adding more than one decorator will ensure that `start` step starts only after all sensors finish.
@@ -1426,14 +1468,117 @@
         the default is the same logical date as the current task or DAG. (Default: None)
     check_existence: bool
         Set to True to check if the external task exists or check if
         the DAG to wait for exists. (Default: True)
     """
     ...
 
+@typing.overload
+def trigger_on_finish(*, flow: typing.Union[str, typing.Dict[str, str], None] = None, flows: typing.List[typing.Union[str, typing.Dict[str, str]]] = [], options: typing.Dict[str, typing.Any] = {}) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+    """
+    Specifies the flow(s) that this flow depends on.
+    
+    ```
+    @trigger_on_finish(flow='FooFlow')
+    ```
+    or
+    ```
+    @trigger_on_finish(flows=['FooFlow', 'BarFlow'])
+    ```
+    This decorator respects the @project decorator and triggers the flow
+    when upstream runs within the same namespace complete successfully
+    
+    Additionally, you can specify project aware upstream flow dependencies
+    by specifying the fully qualified project_flow_name.
+    ```
+    @trigger_on_finish(flow='my_project.branch.my_branch.FooFlow')
+    ```
+    or
+    ```
+    @trigger_on_finish(flows=['my_project.branch.my_branch.FooFlow', 'BarFlow'])
+    ```
+    
+    You can also specify just the project or project branch (other values will be
+    inferred from the current project or project branch):
+    ```
+    @trigger_on_finish(flow={"name": "FooFlow", "project": "my_project", "project_branch": "branch"})
+    ```
+    
+    Note that `branch` is typically one of:
+      - `prod`
+      - `user.bob`
+      - `test.my_experiment`
+      - `prod.staging`
+    
+    Parameters
+    ----------
+    flow : Union[str, Dict[str, str]], optional, default None
+        Upstream flow dependency for this flow.
+    flows : List[Union[str, Dict[str, str]]], default []
+        Upstream flow dependencies for this flow.
+    options : Dict[str, Any], default {}
+        Backend-specific configuration for tuning eventing behavior.
+    
+    
+    """
+    ...
+
+@typing.overload
+def trigger_on_finish(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
+    ...
+
+def trigger_on_finish(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, flow: typing.Union[str, typing.Dict[str, str], None] = None, flows: typing.List[typing.Union[str, typing.Dict[str, str]]] = [], options: typing.Dict[str, typing.Any] = {}):
+    """
+    Specifies the flow(s) that this flow depends on.
+    
+    ```
+    @trigger_on_finish(flow='FooFlow')
+    ```
+    or
+    ```
+    @trigger_on_finish(flows=['FooFlow', 'BarFlow'])
+    ```
+    This decorator respects the @project decorator and triggers the flow
+    when upstream runs within the same namespace complete successfully
+    
+    Additionally, you can specify project aware upstream flow dependencies
+    by specifying the fully qualified project_flow_name.
+    ```
+    @trigger_on_finish(flow='my_project.branch.my_branch.FooFlow')
+    ```
+    or
+    ```
+    @trigger_on_finish(flows=['my_project.branch.my_branch.FooFlow', 'BarFlow'])
+    ```
+    
+    You can also specify just the project or project branch (other values will be
+    inferred from the current project or project branch):
+    ```
+    @trigger_on_finish(flow={"name": "FooFlow", "project": "my_project", "project_branch": "branch"})
+    ```
+    
+    Note that `branch` is typically one of:
+      - `prod`
+      - `user.bob`
+      - `test.my_experiment`
+      - `prod.staging`
+    
+    Parameters
+    ----------
+    flow : Union[str, Dict[str, str]], optional, default None
+        Upstream flow dependency for this flow.
+    flows : List[Union[str, Dict[str, str]]], default []
+        Upstream flow dependencies for this flow.
+    options : Dict[str, Any], default {}
+        Backend-specific configuration for tuning eventing behavior.
+    
+    
+    """
+    ...
+
 def project(*, name: str) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
     Specifies what flows belong to the same project.
     
     A project-specific namespace is created for all flows that
     use the same `@project(name)`.
     
@@ -1445,14 +1590,63 @@
         contain only lowercase alphanumeric characters and underscores.
     
     
     """
     ...
 
 @typing.overload
+def schedule(*, hourly: bool = False, daily: bool = True, weekly: bool = False, cron: typing.Optional[str] = None, timezone: typing.Optional[str] = None) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+    """
+    Specifies the times when the flow should be run when running on a
+    production scheduler.
+    
+    Parameters
+    ----------
+    hourly : bool, default False
+        Run the workflow hourly.
+    daily : bool, default True
+        Run the workflow daily.
+    weekly : bool, default False
+        Run the workflow weekly.
+    cron : str, optional, default None
+        Run the workflow at [a custom Cron schedule](https://docs.aws.amazon.com/eventbridge/latest/userguide/scheduled-events.html#cron-expressions)
+        specified by this expression.
+    timezone : str, optional, default None
+        Timezone on which the schedule runs (default: None). Currently supported only for Argo workflows,
+        which accepts timezones in [IANA format](https://nodatime.org/TimeZones).
+    """
+    ...
+
+@typing.overload
+def schedule(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
+    ...
+
+def schedule(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, hourly: bool = False, daily: bool = True, weekly: bool = False, cron: typing.Optional[str] = None, timezone: typing.Optional[str] = None):
+    """
+    Specifies the times when the flow should be run when running on a
+    production scheduler.
+    
+    Parameters
+    ----------
+    hourly : bool, default False
+        Run the workflow hourly.
+    daily : bool, default True
+        Run the workflow daily.
+    weekly : bool, default False
+        Run the workflow weekly.
+    cron : str, optional, default None
+        Run the workflow at [a custom Cron schedule](https://docs.aws.amazon.com/eventbridge/latest/userguide/scheduled-events.html#cron-expressions)
+        specified by this expression.
+    timezone : str, optional, default None
+        Timezone on which the schedule runs (default: None). Currently supported only for Argo workflows,
+        which accepts timezones in [IANA format](https://nodatime.org/TimeZones).
+    """
+    ...
+
+@typing.overload
 def pypi_base(*, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
     Specifies the PyPI packages for all steps of the flow.
     
     Use `@pypi_base` to set common packages required by all
     steps and use `@pypi` to specify step-specific overrides.
     Parameters
@@ -1579,63 +1773,14 @@
         Backend-specific configuration for tuning eventing behavior.
     
     
     """
     ...
 
 @typing.overload
-def schedule(*, hourly: bool = False, daily: bool = True, weekly: bool = False, cron: typing.Optional[str] = None, timezone: typing.Optional[str] = None) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
-    """
-    Specifies the times when the flow should be run when running on a
-    production scheduler.
-    
-    Parameters
-    ----------
-    hourly : bool, default False
-        Run the workflow hourly.
-    daily : bool, default True
-        Run the workflow daily.
-    weekly : bool, default False
-        Run the workflow weekly.
-    cron : str, optional, default None
-        Run the workflow at [a custom Cron schedule](https://docs.aws.amazon.com/eventbridge/latest/userguide/scheduled-events.html#cron-expressions)
-        specified by this expression.
-    timezone : str, optional, default None
-        Timezone on which the schedule runs (default: None). Currently supported only for Argo workflows,
-        which accepts timezones in [IANA format](https://nodatime.org/TimeZones).
-    """
-    ...
-
-@typing.overload
-def schedule(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
-    ...
-
-def schedule(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, hourly: bool = False, daily: bool = True, weekly: bool = False, cron: typing.Optional[str] = None, timezone: typing.Optional[str] = None):
-    """
-    Specifies the times when the flow should be run when running on a
-    production scheduler.
-    
-    Parameters
-    ----------
-    hourly : bool, default False
-        Run the workflow hourly.
-    daily : bool, default True
-        Run the workflow daily.
-    weekly : bool, default False
-        Run the workflow weekly.
-    cron : str, optional, default None
-        Run the workflow at [a custom Cron schedule](https://docs.aws.amazon.com/eventbridge/latest/userguide/scheduled-events.html#cron-expressions)
-        specified by this expression.
-    timezone : str, optional, default None
-        Timezone on which the schedule runs (default: None). Currently supported only for Argo workflows,
-        which accepts timezones in [IANA format](https://nodatime.org/TimeZones).
-    """
-    ...
-
-@typing.overload
 def conda_base(*, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
     Specifies the Conda environment for all steps of the flow.
     
     Use `@conda_base` to set common libraries required by all
     steps and use `@conda` to specify step-specific additions.
     
@@ -1676,159 +1821,14 @@
         Version of Python to use, e.g. '3.7.4'. A default value of None implies
         that the version used will correspond to the version of the Python interpreter used to start the run.
     disabled : bool, default False
         If set to True, disables Conda.
     """
     ...
 
-def airflow_s3_key_sensor(*, timeout: int, poke_interval: int, mode: str, exponential_backoff: bool, pool: str, soft_fail: bool, name: str, description: str, bucket_key: typing.Union[str, typing.List[str]], bucket_name: str, wildcard_match: bool, aws_conn_id: str, verify: bool) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
-    """
-    The `@airflow_s3_key_sensor` decorator attaches a Airflow [S3KeySensor](https://airflow.apache.org/docs/apache-airflow-providers-amazon/stable/_api/airflow/providers/amazon/aws/sensors/s3/index.html#airflow.providers.amazon.aws.sensors.s3.S3KeySensor)
-    before the start step of the flow. This decorator only works when a flow is scheduled on Airflow
-    and is compiled using `airflow create`. More than one `@airflow_s3_key_sensor` can be
-    added as a flow decorators. Adding more than one decorator will ensure that `start` step
-    starts only after all sensors finish.
-    
-    Parameters
-    ----------
-    timeout : int
-        Time, in seconds before the task times out and fails. (Default: 3600)
-    poke_interval : int
-        Time in seconds that the job should wait in between each try. (Default: 60)
-    mode : str
-        How the sensor operates. Options are: { poke | reschedule }. (Default: "poke")
-    exponential_backoff : bool
-        allow progressive longer waits between pokes by using exponential backoff algorithm. (Default: True)
-    pool : str
-        the slot pool this task should run in,
-        slot pools are a way to limit concurrency for certain tasks. (Default:None)
-    soft_fail : bool
-        Set to true to mark the task as SKIPPED on failure. (Default: False)
-    name : str
-        Name of the sensor on Airflow
-    description : str
-        Description of sensor in the Airflow UI
-    bucket_key : Union[str, List[str]]
-        The key(s) being waited on. Supports full s3:// style url or relative path from root level.
-        When it's specified as a full s3:// url, please leave `bucket_name` as None
-    bucket_name : str
-        Name of the S3 bucket. Only needed when bucket_key is not provided as a full s3:// url.
-        When specified, all the keys passed to bucket_key refers to this bucket. (Default:None)
-    wildcard_match : bool
-        whether the bucket_key should be interpreted as a Unix wildcard pattern. (Default: False)
-    aws_conn_id : str
-        a reference to the s3 connection on Airflow. (Default: None)
-    verify : bool
-        Whether or not to verify SSL certificates for S3 connection. (Default: None)
-    """
-    ...
-
-@typing.overload
-def trigger_on_finish(*, flow: typing.Union[str, typing.Dict[str, str], None] = None, flows: typing.List[typing.Union[str, typing.Dict[str, str]]] = [], options: typing.Dict[str, typing.Any] = {}) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
-    """
-    Specifies the flow(s) that this flow depends on.
-    
-    ```
-    @trigger_on_finish(flow='FooFlow')
-    ```
-    or
-    ```
-    @trigger_on_finish(flows=['FooFlow', 'BarFlow'])
-    ```
-    This decorator respects the @project decorator and triggers the flow
-    when upstream runs within the same namespace complete successfully
-    
-    Additionally, you can specify project aware upstream flow dependencies
-    by specifying the fully qualified project_flow_name.
-    ```
-    @trigger_on_finish(flow='my_project.branch.my_branch.FooFlow')
-    ```
-    or
-    ```
-    @trigger_on_finish(flows=['my_project.branch.my_branch.FooFlow', 'BarFlow'])
-    ```
-    
-    You can also specify just the project or project branch (other values will be
-    inferred from the current project or project branch):
-    ```
-    @trigger_on_finish(flow={"name": "FooFlow", "project": "my_project", "project_branch": "branch"})
-    ```
-    
-    Note that `branch` is typically one of:
-      - `prod`
-      - `user.bob`
-      - `test.my_experiment`
-      - `prod.staging`
-    
-    Parameters
-    ----------
-    flow : Union[str, Dict[str, str]], optional, default None
-        Upstream flow dependency for this flow.
-    flows : List[Union[str, Dict[str, str]]], default []
-        Upstream flow dependencies for this flow.
-    options : Dict[str, Any], default {}
-        Backend-specific configuration for tuning eventing behavior.
-    
-    
-    """
-    ...
-
-@typing.overload
-def trigger_on_finish(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
-    ...
-
-def trigger_on_finish(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, flow: typing.Union[str, typing.Dict[str, str], None] = None, flows: typing.List[typing.Union[str, typing.Dict[str, str]]] = [], options: typing.Dict[str, typing.Any] = {}):
-    """
-    Specifies the flow(s) that this flow depends on.
-    
-    ```
-    @trigger_on_finish(flow='FooFlow')
-    ```
-    or
-    ```
-    @trigger_on_finish(flows=['FooFlow', 'BarFlow'])
-    ```
-    This decorator respects the @project decorator and triggers the flow
-    when upstream runs within the same namespace complete successfully
-    
-    Additionally, you can specify project aware upstream flow dependencies
-    by specifying the fully qualified project_flow_name.
-    ```
-    @trigger_on_finish(flow='my_project.branch.my_branch.FooFlow')
-    ```
-    or
-    ```
-    @trigger_on_finish(flows=['my_project.branch.my_branch.FooFlow', 'BarFlow'])
-    ```
-    
-    You can also specify just the project or project branch (other values will be
-    inferred from the current project or project branch):
-    ```
-    @trigger_on_finish(flow={"name": "FooFlow", "project": "my_project", "project_branch": "branch"})
-    ```
-    
-    Note that `branch` is typically one of:
-      - `prod`
-      - `user.bob`
-      - `test.my_experiment`
-      - `prod.staging`
-    
-    Parameters
-    ----------
-    flow : Union[str, Dict[str, str]], optional, default None
-        Upstream flow dependency for this flow.
-    flows : List[Union[str, Dict[str, str]]], default []
-        Upstream flow dependencies for this flow.
-    options : Dict[str, Any], default {}
-        Backend-specific configuration for tuning eventing behavior.
-    
-    
-    """
-    ...
-
 def namespace(ns: typing.Optional[str]) -> typing.Optional[str]:
     """
     Switch namespace to the one provided.
     
     This call has a global effect. No objects outside this namespace
     will be accessible. To access all objects regardless of namespaces,
     pass None to this call.
@@ -2771,7 +2771,10 @@
         ...
     def __getstate__(self):
         ...
     def __setstate__(self, state):
         ...
     ...
 
+def get_aws_client(module, with_error = False, role_arn = None, session_vars = None, client_params = None):
+    ...
+
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/cards.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/cards.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:00.979633                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.256262                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.cards.card_modules.basic
     import metaflow.plugins.cards.card_modules.card
     import metaflow.plugins.cards.card_client
-    import typing
     import metaflow
+    import typing
+    import metaflow.plugins.cards.card_modules.basic
     import metaflow.plugins.cards.card_modules.components
 
 def get_cards(task: typing.Union[str, "metaflow.Task"], id: typing.Optional[str] = None, type: typing.Optional[str] = None, follow_resumed: bool = True) -> metaflow.plugins.cards.card_client.CardContainer:
     """
     Get cards related to a `Task`.
     
     Note that `get_cards` resolves the cards contained by the task, but it doesn't actually
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/cli.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/cli.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:00.985572                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.261107                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/client/__init__.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/client/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:00.982872                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.258762                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import typing
+    import metaflow.client.core
     import metaflow.events
     import datetime
-    import metaflow.client.core
 
 def namespace(ns: typing.Optional[str]) -> typing.Optional[str]:
     """
     Switch namespace to the one provided.
     
     This call has a global effect. No objects outside this namespace
     will be accessible. To access all objects regardless of namespaces,
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/client/core.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/client/core.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:00.964242                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.245307                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import tarfile
     import metaflow.client.core
-    import metaflow.events
-    import datetime
     import metaflow.exception
+    import metaflow.metaflow_current
+    import datetime
     import typing
-    import tarfile
+    import metaflow.events
     import metaflow
-    import metaflow.metaflow_current
 
 current: metaflow.metaflow_current.Current
 
 class Trigger(object, metaclass=type):
     def __init__(self, _meta = None):
         ...
     @classmethod
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/client/filecache.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/client/filecache.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:00.986643                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.261945                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.datastore.content_addressed_store
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/clone_util.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/clone_util.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:00.983241                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.259314                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaDatum(tuple, metaclass=type):
     @staticmethod
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/events.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/events.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:00.966700                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.247187                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.events
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/exception.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/exception.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:00.954414                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.237983                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/flowspec.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/flowspec.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:00.965966                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.246610                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.unbounded_foreach
     import metaflow.parameters
-    import metaflow.datastore.inputs
-    import typing
     import metaflow.exception
+    import typing
+    import metaflow.datastore.inputs
 
 class DelayedEvaluationParameter(object, metaclass=type):
     def __init__(self, name, field, fun):
         ...
     def __call__(self, return_str = False):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/includefile.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/includefile.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:00.977307                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.254498                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.parameters
-    import metaflow.plugins.datatools.s3.s3
-    import typing
     import metaflow._vendor.click.types
+    import typing
     import io
+    import metaflow.plugins.datatools.s3.s3
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/metadata/metadata.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/metadata/metadata.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.008282                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.279508                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/metadata/util.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/metadata/util.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.061559                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.320773                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def copy_tree(src, dst, update = False):
     ...
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/metaflow_config.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/metaflow_config.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:00.955711                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.238921                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
@@ -261,7 +261,9 @@
 MAX_CPU_PER_TASK: None
 
 MAX_ATTEMPTS: int
 
 def get_pinned_conda_libs(python_version, datastore_type):
     ...
 
+DEFAULT_AZURE_CLIENT_PROVIDER: str
+
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/metaflow_current.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/metaflow_current.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.065876                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.323341                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.cards.component_serializer
-    import metaflow.events
+    import metaflow.metaflow_current
     import typing
+    import metaflow.events
     import metaflow
-    import metaflow.metaflow_current
 
 TYPE_CHECKING: bool
 
 TEMPDIR: str
 
 class Parallel(tuple, metaclass=type):
     @staticmethod
@@ -238,14 +238,27 @@
         Returns
         -------
         CardComponentCollector
             The or one of the cards attached to this step.
         """
         ...
     @property
+    def trigger(self) -> "metaflow.events.Trigger":
+        """
+        (only in the presence of the @trigger_on_finish, or @trigger decorators)
+        
+        Returns `Trigger` if the current run is triggered by an event
+        
+        Returns
+        -------
+        Trigger
+            `Trigger` if triggered by an event
+        """
+        ...
+    @property
     def project_name(self) -> str:
         """
         (only in the presence of the @project decorator)
         
         The name of the project assigned to this flow, i.e. `X` in `@project(name=X)`.
         
         Returns
@@ -304,24 +317,11 @@
         
         Returns
         -------
         bool
             True if the flow is deployed with `--production`.
         """
         ...
-    @property
-    def trigger(self) -> "metaflow.events.Trigger":
-        """
-        (only in the presence of the @trigger, or @trigger_on_finish decorators)
-        
-        Returns `Trigger` if the current run is triggered by an event
-        
-        Returns
-        -------
-        Trigger
-            `Trigger` if triggered by an event
-        """
-        ...
     ...
 
 current: Current
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/multicore_utils.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/multicore_utils.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:00.956222                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.239334                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import typing
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/parameters.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/parameters.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:00.957659                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.240447                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import typing
-    import metaflow.exception
     import metaflow.parameters
+    import metaflow.exception
+    import typing
     import metaflow._vendor.click.types
 
 class ParameterFieldFailed(metaflow.exception.MetaflowException, metaclass=type):
     def __init__(self, name, field):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/__init__.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:00.968728                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.248678                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.cards.card_modules.card
     import metaflow.unbounded_foreach
+    import metaflow.plugins.cards.card_modules.card
 
 CLIS_DESC: list
 
 class InternalTestUnboundedForeachInput(metaflow.unbounded_foreach.UnboundedForeachInput, metaclass=type):
     def __init__(self, iterable):
         ...
     def __iter__(self):
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/airflow.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/airflow/airflow.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.034343                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.286451                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
-    import metaflow.metaflow_current
     import metaflow._vendor.click.types
+    import metaflow.metaflow_current
+    import metaflow.exception
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
@@ -92,15 +92,15 @@
     ...
 
 class Kubernetes(object, metaclass=type):
     def __init__(self, datastore, metadata, environment):
         ...
     def launch_job(self, **kwargs):
         ...
-    def create_job(self, flow_name, run_id, step_name, task_id, attempt, user, code_package_sha, code_package_url, code_package_ds, step_cli, docker_image, docker_image_pull_policy, service_account = None, secrets = None, node_selector = None, namespace = None, cpu = None, gpu = None, gpu_vendor = None, disk = None, memory = None, use_tmpfs = None, tmpfs_tempdir = None, tmpfs_size = None, tmpfs_path = None, run_time_limit = None, env = None, persistent_volume_claims = None, tolerations = None, labels = None, annotations = None, num_parallel = 0, attrs = {}, port = None, shared_memory = None):
+    def create_job(self, flow_name, run_id, step_name, task_id, attempt, user, code_package_sha, code_package_url, code_package_ds, step_cli, docker_image, docker_image_pull_policy, service_account = None, secrets = None, node_selector = None, namespace = None, cpu = None, gpu = None, gpu_vendor = None, disk = None, memory = None, use_tmpfs = None, tmpfs_tempdir = None, tmpfs_size = None, tmpfs_path = None, run_time_limit = None, env = None, persistent_volume_claims = None, tolerations = None, labels = None, annotations = None, num_parallel = 0, attrs = {}, shared_memory = None, port = None):
         ...
     def wait(self, stdout_location, stderr_location, echo = None):
         ...
     ...
 
 def get_run_time_limit_for_task(step_decos):
     ...
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/airflow_cli.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/airflow/airflow_cli.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.035535                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.287394                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/airflow_decorator.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/airflow/airflow_decorator.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.031906                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.284529                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/airflow_utils.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/airflow/airflow_utils.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.031444                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.284159                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 TASK_ID_XCOM_KEY: str
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/exception.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/airflow/exception.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.032182                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.284752                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.062186                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.319426                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.062665                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.320195                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
@@ -39,16 +39,12 @@
     ...
 
 class AirflowException(metaflow.exception.MetaflowException, metaclass=type):
     def __init__(self, msg):
         ...
     ...
 
-AIRFLOW_STATES: dict
-
-class ExternalTaskSensorDecorator(metaflow.plugins.airflow.sensors.base_sensor.AirflowSensorDecorator, metaclass=type):
-    def serialize_operator_args(self):
-        ...
+class S3KeySensorDecorator(metaflow.plugins.airflow.sensors.base_sensor.AirflowSensorDecorator, metaclass=type):
     def validate(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.063109                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.319837                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
@@ -39,12 +39,16 @@
     ...
 
 class AirflowException(metaflow.exception.MetaflowException, metaclass=type):
     def __init__(self, msg):
         ...
     ...
 
-class S3KeySensorDecorator(metaflow.plugins.airflow.sensors.base_sensor.AirflowSensorDecorator, metaclass=type):
+AIRFLOW_STATES: dict
+
+class ExternalTaskSensorDecorator(metaflow.plugins.airflow.sensors.base_sensor.AirflowSensorDecorator, metaclass=type):
+    def serialize_operator_args(self):
+        ...
     def validate(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/argo/argo_client.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/argo/argo_client.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.037738                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.301405                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
@@ -20,14 +20,16 @@
 class KubernetesClient(object, metaclass=type):
     def __init__(self):
         ...
     def get(self):
         ...
     def job(self, **kwargs):
         ...
+    def jobset(self, **kwargs):
+        ...
     ...
 
 class ArgoClientException(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
 class ArgoClient(object, metaclass=type):
     def __init__(self, namespace = None):
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/argo/argo_events.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/argo/argo_events.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.036014                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.300089                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/argo/argo_workflows.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/argo/argo_workflows.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.043275                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.305467                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
-    import metaflow.metaflow_current
     import metaflow.parameters
     import metaflow._vendor.click.types
+    import metaflow.metaflow_current
+    import metaflow.exception
 
 JSONType: metaflow.parameters.JSONTypeClass
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.045224                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.307480                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.parameters
     import metaflow.exception
     import metaflow.metaflow_current
-    import metaflow.parameters
     import metaflow.decorators
 
 JSONType: metaflow.parameters.JSONTypeClass
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.036966                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.300838                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.events
     import metaflow.metaflow_current
-    import metaflow.decorators
     import metaflow
+    import metaflow.decorators
 
 current: metaflow.metaflow_current.Current
 
 class Trigger(object, metaclass=type):
     def __init__(self, _meta = None):
         ...
     @classmethod
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/aws_client.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/aws/aws_client.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.009718                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.259058                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 cached_aws_sandbox_creds: None
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/aws_utils.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/aws/aws_utils.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.009459                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.280350                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/batch/batch.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/aws/batch/batch.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.058308                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.317268                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/batch/batch_cli.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/aws/batch/batch_cli.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.059917                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.318551                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/batch/batch_client.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/aws/batch/batch_client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.056893                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.316289                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.059210                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.317991                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.060403                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.318938                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import abc
     import metaflow.exception
     import metaflow.plugins.secrets
-    import abc
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/step_functions/event_bridge_client.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/gcp/gs_exceptions.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.050865                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.309120                                        #
 ##################################################################################
 
 from __future__ import annotations
 
+import typing
+if typing.TYPE_CHECKING:
+    import metaflow.exception
 
-class EventBridgeClient(object, metaclass=type):
-    def __init__(self, name):
+class MetaflowException(Exception, metaclass=type):
+    def __init__(self, msg = "", lineno = None):
         ...
-    def cron(self, cron):
-        ...
-    def role_arn(self, role_arn):
-        ...
-    def state_machine_arn(self, state_machine_arn):
-        ...
-    def schedule(self):
-        ...
-    def delete(self):
+    def __str__(self):
         ...
     ...
 
-def format(name):
+class MetaflowGSPackageError(metaflow.exception.MetaflowException, metaclass=type):
     ...
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/step_functions/production_token.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/aws/step_functions/production_token.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.050519                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.311402                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def new_token(token_prefix, prev_token = None):
     ...
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/step_functions/schedule_decorator.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/aws/step_functions/schedule_decorator.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.050250                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.311178                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.053794                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.313852                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.055379                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.315133                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.parameters
     import metaflow.exception
     import metaflow.metaflow_current
-    import metaflow.parameters
     import metaflow.decorators
 
 JSONType: metaflow.parameters.JSONTypeClass
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.051240                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.236762                                        #
 ##################################################################################
 
 from __future__ import annotations
 
+import typing
+if typing.TYPE_CHECKING:
+    import metaflow.exception
 
-AWS_SANDBOX_ENABLED: bool
+class MetaflowException(Exception, metaclass=type):
+    def __init__(self, msg = "", lineno = None):
+        ...
+    def __str__(self):
+        ...
+    ...
 
-AWS_SANDBOX_REGION: None
+CLIENT_REFRESH_INTERVAL_SECONDS: int
 
-SFN_EXECUTION_LOG_GROUP_ARN: None
+class KubernetesClientException(metaflow.exception.MetaflowException, metaclass=type):
+    ...
 
-class StepFunctionsClient(object, metaclass=type):
+class KubernetesClient(object, metaclass=type):
     def __init__(self):
         ...
-    def search(self, name):
-        ...
-    def push(self, name, definition, role_arn, log_execution_history):
-        ...
-    def get(self, name):
-        ...
-    def trigger(self, state_machine_arn, input):
-        ...
-    def list_executions(self, state_machine_arn, states):
-        ...
-    def terminate_execution(self, execution_arn):
+    def get(self):
         ...
-    def get_state_machine_arn(self, name):
+    def job(self, **kwargs):
         ...
-    def delete(self, name):
+    def jobset(self, **kwargs):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.050055                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.311014                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/azure/azure_credential.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/azure/azure_credential.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.045958                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.307720                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class AzureDefaultClientProvider(object, metaclass=type):
     @staticmethod
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/azure/azure_exceptions.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/azure/azure_exceptions.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.046234                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.307973                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/azure/azure_utils.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/azure/azure_utils.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.046748                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.308378                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.047160                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.308704                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/azure/includefile_support.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/azure/includefile_support.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.001988                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.274525                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_cli.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/card_cli.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.021198                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.299639                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.client.core
     import metaflow.parameters
-    import datetime
     import metaflow.exception
     import typing
+    import datetime
 
 class Task(metaflow.client.core.MetaflowObject, metaclass=type):
     def __init__(self, *args, **kwargs):
         ...
     @property
     def metadata(self) -> typing.List[metaflow.client.core.Metadata]:
         """
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_client.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/card_client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.003898                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.276070                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
     import metaflow.plugins.cards.card_client
+    import metaflow.exception
     import metaflow
 
 TYPE_CHECKING: bool
 
 CARD_SUFFIX: str
 
 def resolve_paths_from_task(flow_datastore, pathspec = None, type = None, hash = None, card_id = None):
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_creator.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/pylint_wrapper.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.015845                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.260029                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
+    import metaflow.exception
 
-current: metaflow.metaflow_current.Current
-
-ASYNC_TIMEOUT: int
+class MetaflowException(Exception, metaclass=type):
+    def __init__(self, msg = "", lineno = None):
+        ...
+    def __str__(self):
+        ...
+    ...
 
-class CardProcessManager(object, metaclass=type):
+class PyLintWarn(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
-class CardCreator(object, metaclass=type):
-    def __init__(self, top_level_options):
+class PyLint(object, metaclass=type):
+    def __init__(self, fname):
+        ...
+    def has_pylint(self):
         ...
-    def create(self, card_uuid = None, user_set_card_id = None, runtime_card = False, decorator_attributes = None, card_options = None, logger = None, mode = "render", final = False, sync = False):
+    def run(self, logger = None, warnings = False, pylint_config = []):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_datastore.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/card_datastore.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.017729                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.296903                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_decorator.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/card_decorator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.016737                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.296175                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.metaflow_current
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/__init__.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/card_modules/__init__.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.013091                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.293267                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/basic.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/card_modules/basic.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:00.996941                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.270529                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.cards.card_modules.card
     import metaflow.plugins.cards.card_modules.basic
+    import metaflow.plugins.cards.card_modules.card
     import metaflow
 
 class MetaflowCard(object, metaclass=type):
     def __init__(self, options = {}, components = [], graph = None):
         ...
     def render(self, task: "metaflow.Task") -> str:
         """
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/card.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/card_modules/card.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.004418                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.276469                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.061217                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.320522                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def main(template, data = None, **kwargs):
     ...
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.064491                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.322245                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def render(template = "", data = {}, partials_path = ".", partials_ext = "mustache", partials_dict = {}, padding = "", def_ldel = "{{", def_rdel = "}}", scopes = None, warn = False, keep = False):
     """
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.064043                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.321871                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 linesep: str
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.063586                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.321499                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class ChevronError(SyntaxError, metaclass=type):
     ...
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/components.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/card_modules/components.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.006778                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.278348                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.cards.card_modules.card
-    import typing
     import metaflow.plugins.cards.card_modules.basic
     import metaflow.plugins.cards.card_modules.components
+    import metaflow.plugins.cards.card_modules.card
+    import typing
 
 class LogComponent(metaflow.plugins.cards.card_modules.basic.DefaultComponent, metaclass=type):
     def __init__(self, data = None):
         ...
     def render(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/convert_to_native_type.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/card_modules/convert_to_native_type.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.048995                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.310176                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class TypeResolvedObject(tuple, metaclass=type):
     @staticmethod
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/renderer_tools.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/debug_logger.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.049253                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.267887                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.cards.card_modules.basic
+    import metaflow.event_logger
 
-class SerializationErrorComponent(metaflow.plugins.cards.card_modules.basic.ErrorComponent, metaclass=type):
-    def __init__(self, component_name, error_message):
+class DebugEventLogger(metaflow.event_logger.NullEventLogger, metaclass=type):
+    @classmethod
+    def get_worker(cls):
         ...
     ...
 
-def render_safely(func):
-    """
-    This is a decorator that can be added to any `MetaflowCardComponent.render`
-    The goal is to render subcomponents safely and ensure that they are JSON serializable.
-    """
+class DebugEventLoggerSidecar(object, metaclass=type):
+    def __init__(self):
+        ...
+    def process_message(self, msg):
+        ...
     ...
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:00.998424                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.271679                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.cards.card_modules.card
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_resolver.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/card_resolver.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.018338                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.297384                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class CardDatastore(object, metaclass=type):
     @classmethod
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/component_serializer.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/component_serializer.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.015546                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.295157                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.cards.card_modules.card
-    import metaflow.exception
     import metaflow.plugins.cards.card_modules.basic
+    import metaflow.plugins.cards.card_modules.card
     import metaflow.plugins.cards.card_modules.components
+    import metaflow.exception
 
 class MetaflowCardComponent(object, metaclass=type):
     @property
     def component_id(self):
         ...
     @component_id.setter
     def component_id(self, value):
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/exception.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/cards/exception.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.013838                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.293812                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/catch_decorator.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/catch_decorator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:00.990715                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.266382                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/datatools/__init__.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/datatools/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:00.989923                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.265435                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import io
     import metaflow.exception
     import metaflow.plugins.datatools.s3.s3
-    import io
 
 def read_in_chunks(dst, src, src_sz, max_chunk_size):
     ...
 
 class MetaflowLocalNotFound(metaflow.exception.MetaflowException, metaclass=type):
     ...
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/datatools/local.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/pypi/conda_decorator.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,82 +1,59 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.001414                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.281478                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
+    import metaflow.decorators
 
-class MetaflowException(Exception, metaclass=type):
-    def __init__(self, msg = "", lineno = None):
-        ...
-    def __str__(self):
-        ...
-    ...
-
-DATATOOLS_LOCALROOT: None
-
-DATATOOLS_SUFFIX: str
+EXT_PKG: str
 
-class MetaflowLocalURLException(metaflow.exception.MetaflowException, metaclass=type):
-    ...
-
-class MetaflowLocalNotFound(metaflow.exception.MetaflowException, metaclass=type):
-    ...
-
-class LocalObject(object, metaclass=type):
-    def __init__(self, url, path):
-        ...
-    @property
-    def exists(self):
+class MetaDatum(tuple, metaclass=type):
+    @staticmethod
+    def __new__(_cls, field, value, type, tags):
         """
-        Does this key correspond to an actual file?
+        Create new instance of MetaDatum(field, value, type, tags)
         """
         ...
-    @property
-    def url(self):
+    def __repr__(self):
         """
-        Local location of the object; this is the path prefixed with local://
+        Return a nicely formatted representation string
         """
         ...
-    @property
-    def path(self):
+    def __getnewargs__(self):
         """
-        Path to the local file
-        """
-        ...
-    @property
-    def size(self):
-        """
-        Size of the local file (in bytes)
-        
-        Returns None if the key does not correspond to an actual object
+        Return self as a plain tuple.  Used by copy and pickle.
         """
         ...
     ...
 
-class Local(object, metaclass=type):
-    @classmethod
-    def get_root_from_config(cls, echo, create_on_absent = True):
+INFO_FILE: str
+
+class CondaStepDecorator(metaflow.decorators.StepDecorator, metaclass=type):
+    def __init__(self, attributes = None, statically_defined = False):
         ...
-    def __init__(self):
-        """
-        Initialize a new context for Local file operations. This object is based used as
-        a context manager for a with statement.
-        """
+    def step_init(self, flow, graph, step, decos, environment, flow_datastore, logger):
+        ...
+    def runtime_init(self, flow, graph, package, run_id):
+        ...
+    def runtime_task_created(self, task_datastore, task_id, split_index, input_paths, is_cloned, ubf_context):
         ...
-    def __enter__(self):
+    def task_pre_step(self, step_name, task_datastore, meta, run_id, task_id, flow, graph, retry_count, max_retries, ubf_context, inputs):
         ...
-    def __exit__(self, *args):
+    def runtime_step_cli(self, cli_args, retry_count, max_user_code_retries, ubf_context):
         ...
-    def get(self, key = None, return_missing = False):
+    def runtime_finished(self, exception):
         ...
-    def put(self, key, obj, overwrite = True):
+    ...
+
+class CondaFlowDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
+    def __init__(self, attributes = None, statically_defined = False):
         ...
-    def info(self, key = None, return_missing = False):
+    def flow_init(self, flow, graph, environment, flow_datastore, metadata, logger, echo, options):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/datatools/s3/__init__.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/datatools/s3/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.012493                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.291965                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import io
     import metaflow.exception
     import metaflow.plugins.datatools.s3.s3
-    import io
 
 class RangeInfo(tuple, metaclass=type):
     @staticmethod
     def __new__(_cls, total_size: int, request_offset: int = 0, request_length: int = -1):
         """
         Create new instance of RangeInfo(total_size, request_offset, request_length)
         """
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/datatools/s3/s3.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/datatools/s3/s3.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:00.973739                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.251794                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.datastore.inputs
-    import metaflow.plugins.datatools.s3.s3
-    import typing
     import metaflow.exception
     import metaflow.metaflow_current
+    import typing
     import io
+    import metaflow.datastore.inputs
+    import metaflow.plugins.datatools.s3.s3
 
 TYPE_CHECKING: bool
 
 class FlowSpec(object, metaclass=type):
     def __init__(self, use_cli = True):
         """
         Construct a FlowSpec
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/datatools/s3/s3tail.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/datatools/s3/s3tail.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.060817                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.321104                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def aws_retry(f):
     ...
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/datatools/s3/s3util.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/datatools/s3/s3util.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.000722                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.273535                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/debug_monitor.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/debug_monitor.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:00.994425                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.268119                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.monitor
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/environment_decorator.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/environment_decorator.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:00.992178                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.264215                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/events_decorator.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/events_decorator.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:00.993116                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.266700                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.metaflow_current
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/frameworks/pytorch.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/frameworks/pytorch.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.045698                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.280939                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.parallel_decorator
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/gcp/gcp_secret_manager_secrets_provider.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/gcp/gcp_secret_manager_secrets_provider.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.048553                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.309820                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import abc
     import metaflow.exception
     import metaflow.plugins.secrets
-    import abc
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/gcp/gs_exceptions.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/resources_decorator.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,15 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.047671                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.263157                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
+    import metaflow.decorators
 
-class MetaflowException(Exception, metaclass=type):
-    def __init__(self, msg = "", lineno = None):
-        ...
-    def __str__(self):
-        ...
-    ...
-
-class MetaflowGSPackageError(metaflow.exception.MetaflowException, metaclass=type):
+class ResourcesDecorator(metaflow.decorators.StepDecorator, metaclass=type):
     ...
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/gcp/gs_storage_client_factory.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/gcp/gs_storage_client_factory.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.047451                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.308940                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class GcpDefaultClientProvider(object, metaclass=type):
     @staticmethod
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/gcp/gs_utils.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/gcp/gs_utils.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.048031                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.309402                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/gcp/includefile_support.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/gcp/includefile_support.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.002562                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.274974                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/kubernetes/kubernetes.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/kubernetes/kubernetes.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.025008                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.288341                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
@@ -81,14 +81,16 @@
 class KubernetesClient(object, metaclass=type):
     def __init__(self):
         ...
     def get(self):
         ...
     def job(self, **kwargs):
         ...
+    def jobset(self, **kwargs):
+        ...
     ...
 
 LOGS_DIR: str
 
 STDOUT_FILE: str
 
 STDERR_FILE: str
@@ -104,15 +106,15 @@
     ...
 
 class Kubernetes(object, metaclass=type):
     def __init__(self, datastore, metadata, environment):
         ...
     def launch_job(self, **kwargs):
         ...
-    def create_job(self, flow_name, run_id, step_name, task_id, attempt, user, code_package_sha, code_package_url, code_package_ds, step_cli, docker_image, docker_image_pull_policy, service_account = None, secrets = None, node_selector = None, namespace = None, cpu = None, gpu = None, gpu_vendor = None, disk = None, memory = None, use_tmpfs = None, tmpfs_tempdir = None, tmpfs_size = None, tmpfs_path = None, run_time_limit = None, env = None, persistent_volume_claims = None, tolerations = None, labels = None, annotations = None, num_parallel = 0, attrs = {}, port = None, shared_memory = None):
+    def create_job(self, flow_name, run_id, step_name, task_id, attempt, user, code_package_sha, code_package_url, code_package_ds, step_cli, docker_image, docker_image_pull_policy, service_account = None, secrets = None, node_selector = None, namespace = None, cpu = None, gpu = None, gpu_vendor = None, disk = None, memory = None, use_tmpfs = None, tmpfs_tempdir = None, tmpfs_size = None, tmpfs_path = None, run_time_limit = None, env = None, persistent_volume_claims = None, tolerations = None, labels = None, annotations = None, num_parallel = 0, attrs = {}, shared_memory = None, port = None):
         ...
     def wait(self, stdout_location, stderr_location, echo = None):
         ...
     ...
 
 def validate_kube_labels(labels: typing.Optional[typing.Dict[str, typing.Optional[str]]]) -> bool:
     """
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.027175                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.289987                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow._vendor.click.types
     import metaflow.exception
     import metaflow.decorators
-    import metaflow._vendor.click.types
 
 class JSONTypeClass(metaflow._vendor.click.types.ParamType, metaclass=type):
     def convert(self, value, param, ctx):
         ...
     def __str__(self):
         ...
     def __repr__(self):
@@ -36,15 +36,15 @@
 TASK_LOG_SOURCE: str
 
 class Kubernetes(object, metaclass=type):
     def __init__(self, datastore, metadata, environment):
         ...
     def launch_job(self, **kwargs):
         ...
-    def create_job(self, flow_name, run_id, step_name, task_id, attempt, user, code_package_sha, code_package_url, code_package_ds, step_cli, docker_image, docker_image_pull_policy, service_account = None, secrets = None, node_selector = None, namespace = None, cpu = None, gpu = None, gpu_vendor = None, disk = None, memory = None, use_tmpfs = None, tmpfs_tempdir = None, tmpfs_size = None, tmpfs_path = None, run_time_limit = None, env = None, persistent_volume_claims = None, tolerations = None, labels = None, annotations = None, num_parallel = 0, attrs = {}, port = None, shared_memory = None):
+    def create_job(self, flow_name, run_id, step_name, task_id, attempt, user, code_package_sha, code_package_url, code_package_ds, step_cli, docker_image, docker_image_pull_policy, service_account = None, secrets = None, node_selector = None, namespace = None, cpu = None, gpu = None, gpu_vendor = None, disk = None, memory = None, use_tmpfs = None, tmpfs_tempdir = None, tmpfs_size = None, tmpfs_path = None, run_time_limit = None, env = None, persistent_volume_claims = None, tolerations = None, labels = None, annotations = None, num_parallel = 0, attrs = {}, shared_memory = None, port = None):
         ...
     def wait(self, stdout_location, stderr_location, echo = None):
         ...
     ...
 
 class KubernetesKilledException(metaflow.exception.MetaflowException, metaclass=type):
     ...
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/procpoll.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,62 +1,51 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.023864                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.259713                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
+    import metaflow.procpoll
 
-class MetaflowException(Exception, metaclass=type):
-    def __init__(self, msg = "", lineno = None):
-        ...
-    def __str__(self):
+class ProcPollEvent(object, metaclass=type):
+    def __init__(self, fd, can_read = False, is_terminated = False):
         ...
     ...
 
-class KubernetesJob(object, metaclass=type):
-    def __init__(self, client, **kwargs):
-        ...
-    def create(self):
-        ...
-    def execute(self):
-        ...
-    def step_name(self, step_name):
+class ProcPoll(object, metaclass=type):
+    def poll(self):
         ...
-    def namespace(self, namespace):
+    def add(self, fd):
         ...
-    def name(self, name):
+    def remove(self, fd):
         ...
-    def command(self, command):
-        ...
-    def image(self, image):
-        ...
-    def cpu(self, cpu):
-        ...
-    def memory(self, mem):
+    ...
+
+class LinuxProcPoll(ProcPoll, metaclass=type):
+    def __init__(self):
         ...
-    def environment_variable(self, name, value):
+    def add(self, fd):
         ...
-    def label(self, name, value):
+    def remove(self, fd):
         ...
-    def annotation(self, name, value):
+    def poll(self, timeout):
         ...
     ...
 
-CLIENT_REFRESH_INTERVAL_SECONDS: int
-
-class KubernetesClientException(metaflow.exception.MetaflowException, metaclass=type):
-    ...
-
-class KubernetesClient(object, metaclass=type):
+class DarwinProcPoll(ProcPoll, metaclass=type):
     def __init__(self):
         ...
-    def get(self):
+    def add(self, fd):
+        ...
+    def remove(self, fd):
         ...
-    def job(self, **kwargs):
+    def poll(self, timeout):
         ...
     ...
 
+def make_poll():
+    ...
+
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.026184                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.289206                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/parallel_decorator.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/retry_decorator.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,28 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:00.991992                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.263036                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
 
-UBF_CONTROL: str
-
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-class ParallelDecorator(metaflow.decorators.StepDecorator, metaclass=type):
-    def __init__(self, attributes = None, statically_defined = False):
-        ...
-    def runtime_step_cli(self, cli_args, retry_count, max_user_code_retries, ubf_context):
-        ...
-    def step_init(self, flow, graph, step_name, decorators, environment, flow_datastore, logger):
-        ...
-    def task_decorate(self, step_func, flow, graph, retry_count, max_user_code_retries, ubf_context):
+MAX_ATTEMPTS: int
+
+class RetryDecorator(metaflow.decorators.StepDecorator, metaclass=type):
+    def step_init(self, flow, graph, step, decos, environment, flow_datastore, logger):
         ...
-    def setup_distributed_env(self, flow):
+    def step_task_retry_count(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/project_decorator.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/project_decorator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:00.992693                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.267018                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.metaflow_current
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/pypi/__init__.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/pypi/__init__.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:00.991333                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.263946                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/pypi/conda_decorator.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/datatools/local.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,82 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.028134                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.274067                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
+    import metaflow.exception
 
-EXT_PKG: str
+class MetaflowException(Exception, metaclass=type):
+    def __init__(self, msg = "", lineno = None):
+        ...
+    def __str__(self):
+        ...
+    ...
+
+DATATOOLS_LOCALROOT: None
+
+DATATOOLS_SUFFIX: str
 
-class MetaDatum(tuple, metaclass=type):
-    @staticmethod
-    def __new__(_cls, field, value, type, tags):
+class MetaflowLocalURLException(metaflow.exception.MetaflowException, metaclass=type):
+    ...
+
+class MetaflowLocalNotFound(metaflow.exception.MetaflowException, metaclass=type):
+    ...
+
+class LocalObject(object, metaclass=type):
+    def __init__(self, url, path):
+        ...
+    @property
+    def exists(self):
         """
-        Create new instance of MetaDatum(field, value, type, tags)
+        Does this key correspond to an actual file?
         """
         ...
-    def __repr__(self):
+    @property
+    def url(self):
         """
-        Return a nicely formatted representation string
+        Local location of the object; this is the path prefixed with local://
         """
         ...
-    def __getnewargs__(self):
+    @property
+    def path(self):
         """
-        Return self as a plain tuple.  Used by copy and pickle.
+        Path to the local file
+        """
+        ...
+    @property
+    def size(self):
+        """
+        Size of the local file (in bytes)
+        
+        Returns None if the key does not correspond to an actual object
         """
         ...
     ...
 
-INFO_FILE: str
-
-class CondaStepDecorator(metaflow.decorators.StepDecorator, metaclass=type):
-    def __init__(self, attributes = None, statically_defined = False):
-        ...
-    def step_init(self, flow, graph, step, decos, environment, flow_datastore, logger):
+class Local(object, metaclass=type):
+    @classmethod
+    def get_root_from_config(cls, echo, create_on_absent = True):
         ...
-    def runtime_init(self, flow, graph, package, run_id):
-        ...
-    def runtime_task_created(self, task_datastore, task_id, split_index, input_paths, is_cloned, ubf_context):
+    def __init__(self):
+        """
+        Initialize a new context for Local file operations. This object is based used as
+        a context manager for a with statement.
+        """
         ...
-    def task_pre_step(self, step_name, task_datastore, meta, run_id, task_id, flow, graph, retry_count, max_retries, ubf_context, inputs):
+    def __enter__(self):
         ...
-    def runtime_step_cli(self, cli_args, retry_count, max_user_code_retries, ubf_context):
+    def __exit__(self, *args):
         ...
-    def runtime_finished(self, exception):
+    def get(self, key = None, return_missing = False):
         ...
-    ...
-
-class CondaFlowDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
-    def __init__(self, attributes = None, statically_defined = False):
+    def put(self, key, obj, overwrite = True):
         ...
-    def flow_init(self, flow, graph, environment, flow_datastore, metadata, logger, echo, options):
+    def info(self, key = None, return_missing = False):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/pypi/conda_environment.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/pypi/conda_environment.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.029681                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.282775                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
-    import metaflow.metaflow_environment
-    import io
     import abc
+    import io
+    import metaflow.metaflow_environment
+    import metaflow.exception
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/pypi/pypi_decorator.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/pypi/pypi_decorator.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.027468                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.281720                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/pypi/pypi_environment.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/pypi/pypi_environment.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.030186                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.283175                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.metaflow_environment
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/pypi/utils.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/pypi/utils.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.028509                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.282017                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/retry_decorator.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/parallel_decorator.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:00.987724                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.263688                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
 
+UBF_CONTROL: str
+
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-MAX_ATTEMPTS: int
-
-class RetryDecorator(metaflow.decorators.StepDecorator, metaclass=type):
-    def step_init(self, flow, graph, step, decos, environment, flow_datastore, logger):
+class ParallelDecorator(metaflow.decorators.StepDecorator, metaclass=type):
+    def __init__(self, attributes = None, statically_defined = False):
+        ...
+    def runtime_step_cli(self, cli_args, retry_count, max_user_code_retries, ubf_context):
+        ...
+    def step_init(self, flow, graph, step_name, decorators, environment, flow_datastore, logger):
+        ...
+    def task_decorate(self, step_func, flow, graph, retry_count, max_user_code_retries, ubf_context):
         ...
-    def step_task_retry_count(self):
+    def setup_distributed_env(self, flow):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.022371                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.292823                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.secrets
     import abc
+    import metaflow.plugins.secrets
 
 class SecretsProvider(abc.ABC, metaclass=abc.ABCMeta):
     def get_secret_as_dict(self, secret_id, options = {}, role = None) -> typing.Dict[str, str]:
         """
         Retrieve the secret from secrets backend, and return a dictionary of
         environment variables.
         """
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/secrets/secrets_decorator.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/secrets/secrets_decorator.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.022030                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.292590                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/tag_cli.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/tag_cli.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:01.000114                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.272838                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.client.core
-    import metaflow.events
-    import datetime
     import metaflow.exception
     import metaflow.metaflow_current
+    import metaflow.events
+    import datetime
 
 def namespace(ns: typing.Optional[str]) -> typing.Optional[str]:
     """
     Switch namespace to the one provided.
     
     This call has a global effect. No objects outside this namespace
     will be accessible. To access all objects regardless of namespaces,
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:00.987273                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.262426                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.unbounded_foreach
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/timeout_decorator.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/plugins/timeout_decorator.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:00.988298                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.262789                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/tagging_util.pyi` & `ob-metaflow-stubs-3.1/metaflow-stubs/tagging_util.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9.1                                                           #
-# Generated on 2024-03-30T09:14:00.958044                                        #
+# MF version: 2.11.10.3+ob(v1)                                                   #
+# Generated on 2024-05-06T19:56:35.240760                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.9.1/ob_metaflow_stubs.egg-info/PKG-INFO` & `ob-metaflow-stubs-3.1/ob_metaflow_stubs.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: ob-metaflow-stubs
-Version: 2.11.9.1
+Version: 3.1
 Summary: Metaflow Stubs: Stubs for the metaflow package
 Author: Netflix, Outerbounds & the Metaflow Community
 Author-email: help@outerbounds.co
 License: Apache License 2.0
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
-Requires-Dist: ob-metaflow==2.11.9.1
 
 # Metaflow Stubs
 
 This package contains stub files for `metaflow` and thus offers type hints for various editors (such as `VSCode`) and language servers (such as `Pylance`).
 
 ## Installation
```

### Comparing `ob-metaflow-stubs-2.11.9.1/ob_metaflow_stubs.egg-info/SOURCES.txt` & `ob-metaflow-stubs-3.1/ob_metaflow_stubs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 metaflow-stubs/plugins/catch_decorator.pyi
 metaflow-stubs/plugins/debug_logger.pyi
 metaflow-stubs/plugins/debug_monitor.pyi
 metaflow-stubs/plugins/environment_decorator.pyi
 metaflow-stubs/plugins/events_decorator.pyi
 metaflow-stubs/plugins/package_cli.pyi
 metaflow-stubs/plugins/parallel_decorator.pyi
+metaflow-stubs/plugins/perimeters.pyi
 metaflow-stubs/plugins/project_decorator.pyi
 metaflow-stubs/plugins/resources_decorator.pyi
 metaflow-stubs/plugins/retry_decorator.pyi
 metaflow-stubs/plugins/storage_executor.pyi
 metaflow-stubs/plugins/tag_cli.pyi
 metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi
 metaflow-stubs/plugins/timeout_decorator.pyi
@@ -117,22 +118,21 @@
 metaflow-stubs/plugins/gcp/gs_utils.pyi
 metaflow-stubs/plugins/gcp/includefile_support.pyi
 metaflow-stubs/plugins/kubernetes/__init__.pyi
 metaflow-stubs/plugins/kubernetes/kubernetes.pyi
 metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi
 metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi
 metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi
-metaflow-stubs/plugins/kubernetes/kubernetes_job.pyi
 metaflow-stubs/plugins/pypi/__init__.pyi
 metaflow-stubs/plugins/pypi/conda_decorator.pyi
 metaflow-stubs/plugins/pypi/conda_environment.pyi
 metaflow-stubs/plugins/pypi/pypi_decorator.pyi
 metaflow-stubs/plugins/pypi/pypi_environment.pyi
 metaflow-stubs/plugins/pypi/utils.pyi
 metaflow-stubs/plugins/secrets/__init__.pyi
 metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi
 metaflow-stubs/plugins/secrets/secrets_decorator.pyi
+metaflow-stubs/profilers/__init__.pyi
 ob_metaflow_stubs.egg-info/PKG-INFO
 ob_metaflow_stubs.egg-info/SOURCES.txt
 ob_metaflow_stubs.egg-info/dependency_links.txt
-ob_metaflow_stubs.egg-info/requires.txt
 ob_metaflow_stubs.egg-info/top_level.txt
```

### Comparing `ob-metaflow-stubs-2.11.9.1/setup.py` & `ob-metaflow-stubs-3.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,10 +20,9 @@
     long_description_content_type="text/markdown",
     author="Netflix, Outerbounds & the Metaflow Community",
     author_email="help@outerbounds.co",
     license="Apache License 2.0",
     packages=["metaflow-stubs"],
     package_data={"metaflow-stubs": ["generated_for.txt", "py.typed", "**/*.pyi"]},
     py_modules=["metaflow-stubs"],
-    install_requires=[f"ob-metaflow=={version}"],
     python_requires=">=3.7.0",
 )
```

