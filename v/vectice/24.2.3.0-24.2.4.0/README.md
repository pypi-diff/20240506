# Comparing `tmp/vectice-24.2.3.0.tar.gz` & `tmp/vectice-24.2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectice-24.2.3.0.tar", last modified: Mon Apr 29 07:48:51 2024, max compression
+gzip compressed data, was "vectice-24.2.4.0.tar", last modified: Mon May  6 07:58:51 2024, max compression
```

## Comparing `vectice-24.2.3.0.tar` & `vectice-24.2.4.0.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:48:51.054334 vectice-24.2.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-29 07:48:44.000000 vectice-24.2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-29 07:48:51.054334 vectice-24.2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-29 07:48:44.000000 vectice-24.2.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-29 07:48:44.000000 vectice-24.2.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-29 07:48:51.058334 vectice-24.2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-29 07:48:44.000000 vectice-24.2.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:48:51.014334 vectice-24.2.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:48:51.018334 vectice-24.2.3.0/src/vectice/
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:48:51.022334 vectice-24.2.3.0/src/vectice/api/
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)    20510 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/gql_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/gql_attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/gql_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/gql_entity_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/gql_feature_flag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/gql_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/gql_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/gql_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/gql_property.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/gql_user_workspace_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/http_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    13467 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/http_error_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12109 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/iteration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:48:51.030334 vectice-24.2.3.0/src/vectice/api/json/
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/artifact_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/code_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/dataset_register.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/dataset_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/dataset_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/dataset_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/entity_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/files_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/iteration.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/json_to_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/json_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/model_register.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/model_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/model_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/model_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/organization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/page.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/paged_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/phase.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/property.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/public_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/requirement.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/section.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/user_and_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/json_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/phase.py
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/rest_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/api/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:48:51.030334 vectice-24.2.3.0/src/vectice/autolog/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/autolog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:48:51.034334 vectice-24.2.3.0/src/vectice/autolog/asset_services/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/autolog/asset_services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/autolog/asset_services/catboost_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/autolog/asset_services/keras_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/autolog/asset_services/lightgbm_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/autolog/asset_services/metric_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/autolog/asset_services/pandas_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/autolog/asset_services/pyspark_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/autolog/asset_services/pytorch_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/autolog/asset_services/sklearn_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/autolog/asset_services/vectice_asset_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    10107 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/autolog/autolog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/autolog/autolog_asset_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    30199 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/autolog/autolog_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/autolog/model_library.py
--rw-r--r--   0 runner    (1001) docker     (127)    21843 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:48:51.038334 vectice-24.2.3.0/src/vectice/models/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/additional_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/attachment_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/code_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11659 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    19022 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/iteration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    11174 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/model_exp_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/model_mlflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/phase.py
--rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:48:51.038334 vectice-24.2.3.0/src/vectice/models/representation/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/representation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/representation/dataset_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/representation/dataset_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/representation/model_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/representation/model_version_representation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:48:51.038334 vectice-24.2.3.0/src/vectice/models/resource/
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8191 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/bigquery_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11464 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/databricks_table_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/description.py
--rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/file_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/gcs_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:48:51.042334 vectice-24.2.3.0/src/vectice/models/resource/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/metadata/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/metadata/column_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/metadata/dataframe_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/metadata/db_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/metadata/df_wrapper_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/metadata/df_wrapper_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11952 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/metadata/df_wrapper_spark_df.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/metadata/extra_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/metadata/files_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/metadata/pyspark_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/metadata/source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/no_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     8655 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/s3_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/resource/snowflake_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:48:51.042334 vectice-24.2.3.0/src/vectice/models/test_library/
--rw-r--r--   0 runner    (1001) docker     (127)    11948 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/test_library/binary_classification_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/models/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:48:51.042334 vectice-24.2.3.0/src/vectice/services/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/services/iteration_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/services/phase_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:48:51.042334 vectice-24.2.3.0/src/vectice/types/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/types/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:48:51.046334 vectice-24.2.3.0/src/vectice/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/utils/api_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9729 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/utils/code_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    13972 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/utils/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/utils/dataframe_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9540 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/utils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/utils/instance_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/utils/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/utils/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-29 07:48:44.000000 vectice-24.2.3.0/src/vectice/utils/vectice_ids_regex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:48:51.046334 vectice-24.2.3.0/src/vectice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-29 07:48:50.000000 vectice-24.2.3.0/src/vectice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-04-29 07:48:51.000000 vectice-24.2.3.0/src/vectice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 07:48:50.000000 vectice-24.2.3.0/src/vectice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-29 07:48:51.000000 vectice-24.2.3.0/src/vectice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 07:48:51.000000 vectice-24.2.3.0/src/vectice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:58:51.276828 vectice-24.2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-06 07:58:45.000000 vectice-24.2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-06 07:58:51.276828 vectice-24.2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-06 07:58:45.000000 vectice-24.2.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-06 07:58:45.000000 vectice-24.2.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-06 07:58:51.276828 vectice-24.2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-05-06 07:58:45.000000 vectice-24.2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:58:51.240828 vectice-24.2.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:58:51.240828 vectice-24.2.4.0/src/vectice/
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:58:51.248828 vectice-24.2.4.0/src/vectice/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20510 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/gql_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/gql_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/gql_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/gql_entity_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/gql_feature_flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/gql_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/gql_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/gql_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/gql_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/gql_user_workspace_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/http_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13467 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/http_error_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12109 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/iteration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:58:51.252828 vectice-24.2.4.0/src/vectice/api/json/
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/json/artifact_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/json/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/json/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/json/code_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/json/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/json/dataset_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/json/dataset_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/json/dataset_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/json/dataset_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/json/entity_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/json/files_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/json/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/json/json_to_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/json/json_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/json/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/json/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/json/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/json/model_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/json/model_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/json/model_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/json/model_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/json/organization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/json/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/json/paged_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/json/phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/json/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/json/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/json/public_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/json/requirement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/json/section.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/json/user_and_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/json/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/json_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/rest_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/api/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:58:51.252828 vectice-24.2.4.0/src/vectice/autolog/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/autolog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:58:51.256828 vectice-24.2.4.0/src/vectice/autolog/asset_services/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/autolog/asset_services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/autolog/asset_services/catboost_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/autolog/asset_services/keras_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/autolog/asset_services/lightgbm_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/autolog/asset_services/metric_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/autolog/asset_services/pandas_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/autolog/asset_services/pyspark_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/autolog/asset_services/pytorch_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/autolog/asset_services/sklearn_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/autolog/asset_services/vectice_asset_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9912 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/autolog/autolog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/autolog/autolog_asset_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30626 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/autolog/autolog_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/autolog/model_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21843 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:58:51.260828 vectice-24.2.4.0/src/vectice/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/additional_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/attachment_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/code_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11659 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19022 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11174 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/model_exp_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/model_mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:58:51.260828 vectice-24.2.4.0/src/vectice/models/representation/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/representation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/representation/dataset_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/representation/dataset_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/representation/model_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/representation/model_version_representation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:58:51.260828 vectice-24.2.4.0/src/vectice/models/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8191 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/resource/bigquery_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11464 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/resource/databricks_table_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/resource/description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/resource/file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/resource/gcs_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:58:51.264828 vectice-24.2.4.0/src/vectice/models/resource/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/resource/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/resource/metadata/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/resource/metadata/column_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/resource/metadata/dataframe_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/resource/metadata/db_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/resource/metadata/df_wrapper_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/resource/metadata/df_wrapper_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11952 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/resource/metadata/df_wrapper_spark_df.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/resource/metadata/extra_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/resource/metadata/files_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/resource/metadata/pyspark_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/resource/metadata/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/resource/no_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8655 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/resource/s3_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/resource/snowflake_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:58:51.264828 vectice-24.2.4.0/src/vectice/models/test_library/
+-rw-r--r--   0 runner    (1001) docker     (127)    11948 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/test_library/binary_classification_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/models/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:58:51.264828 vectice-24.2.4.0/src/vectice/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/services/iteration_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/services/phase_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:58:51.264828 vectice-24.2.4.0/src/vectice/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/types/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:58:51.268828 vectice-24.2.4.0/src/vectice/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/utils/api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/utils/code_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13972 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/utils/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/utils/dataframe_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9540 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/utils/instance_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/utils/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/utils/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-06 07:58:45.000000 vectice-24.2.4.0/src/vectice/utils/vectice_ids_regex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:58:51.268828 vectice-24.2.4.0/src/vectice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-06 07:58:51.000000 vectice-24.2.4.0/src/vectice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-05-06 07:58:51.000000 vectice-24.2.4.0/src/vectice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 07:58:51.000000 vectice-24.2.4.0/src/vectice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-06 07:58:51.000000 vectice-24.2.4.0/src/vectice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-06 07:58:51.000000 vectice-24.2.4.0/src/vectice.egg-info/top_level.txt
```

### Comparing `vectice-24.2.3.0/LICENSE` & `vectice-24.2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/PKG-INFO` & `vectice-24.2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectice
-Version: 24.2.3.0
+Version: 24.2.4.0
 Summary: Vectice Python library
 Home-page: https://www.vectice.com
 Author: Vectice Inc.
 Author-email: sdk@vectice.com
 License: Apache License 2.0
 Keywords: Vectice,Client,API,Adapter
 Platform: Linux
@@ -12,15 +12,14 @@
 Platform: Windows
 Classifier: Topic :: Internet
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -37,14 +36,15 @@
 Requires-Dist: gql[requests]
 Requires-Dist: GitPython
 Requires-Dist: packaging
 Requires-Dist: Pillow
 Requires-Dist: pandas
 Requires-Dist: typing-extensions>=4.5.0
 Requires-Dist: dataclasses-json==0.5.8
+Requires-Dist: IPython
 Provides-Extra: dev
 Requires-Dist: black==24.2.0; extra == "dev"
 Requires-Dist: gitpython; extra == "dev"
 Requires-Dist: pyright==1.1.360; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-requests; extra == "dev"
 Requires-Dist: types-urllib3; extra == "dev"
@@ -94,19 +94,16 @@
 Requires-Dist: catboost; extra == "test"
 Requires-Dist: torch; extra == "test"
 Provides-Extra: gcs
 Requires-Dist: google-cloud-storage>=1.17.0; extra == "gcs"
 Requires-Dist: google-cloud-bigquery; extra == "gcs"
 Provides-Extra: s3
 Requires-Dist: boto3; extra == "s3"
-Provides-Extra: autolog
-Requires-Dist: IPython; extra == "autolog"
 Provides-Extra: validation
 Requires-Dist: shap; extra == "validation"
 Requires-Dist: scipy; extra == "validation"
-Requires-Dist: pandas; extra == "validation"
 
 Auto-documentation for ML projects & their governance. View https://github.com/vectice/GettingStarted to get started.
 
 # Documentation
 
 Official documentation for Vectice can be found at https://docs.vectice.com.
```

### Comparing `vectice-24.2.3.0/pyproject.toml` & `vectice-24.2.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/setup.py` & `vectice-24.2.4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         "gql[requests]",
         "GitPython",
         "packaging",
         "Pillow",
         "pandas",
         "typing-extensions>=4.5.0",  # Prior to 4.6.2 because of colab issues with tensorflow 2.13.0
         "dataclasses-json==0.5.8",
+        "IPython",
     ],
     extras_require={
         "dev": [
             "black==24.2.0",
             "gitpython",
             "pyright==1.1.360",
             "ruff",
@@ -100,25 +101,23 @@
             "xgboost",
             "kaleido",
             "catboost",
             "torch",
         ],
         "gcs": ["google-cloud-storage>=1.17.0", "google-cloud-bigquery"],
         "s3": ["boto3"],
-        "autolog": ["IPython"],
-        "validation": ["shap", "scipy", "pandas"],
+        "validation": ["shap", "scipy"],
     },
     classifiers=[
         "Topic :: Internet",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
```

### Comparing `vectice-24.2.3.0/src/vectice/__init__.py` & `vectice-24.2.4.0/src/vectice/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/_auth.py` & `vectice-24.2.4.0/src/vectice/api/_auth.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/attachment.py` & `vectice-24.2.4.0/src/vectice/api/attachment.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/client.py` & `vectice-24.2.4.0/src/vectice/api/client.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/gql_api.py` & `vectice-24.2.4.0/src/vectice/api/gql_api.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/gql_attachment.py` & `vectice-24.2.4.0/src/vectice/api/gql_attachment.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/gql_dataset.py` & `vectice-24.2.4.0/src/vectice/api/gql_dataset.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/gql_entity_file.py` & `vectice-24.2.4.0/src/vectice/api/gql_entity_file.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/gql_feature_flag.py` & `vectice-24.2.4.0/src/vectice/api/gql_feature_flag.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/gql_metric.py` & `vectice-24.2.4.0/src/vectice/api/gql_metric.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/gql_model.py` & `vectice-24.2.4.0/src/vectice/api/gql_model.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/gql_organization.py` & `vectice-24.2.4.0/src/vectice/api/gql_organization.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/gql_property.py` & `vectice-24.2.4.0/src/vectice/api/gql_property.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/gql_user_workspace_api.py` & `vectice-24.2.4.0/src/vectice/api/gql_user_workspace_api.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/http_error.py` & `vectice-24.2.4.0/src/vectice/api/http_error.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/http_error_handlers.py` & `vectice-24.2.4.0/src/vectice/api/http_error_handlers.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/iteration.py` & `vectice-24.2.4.0/src/vectice/api/iteration.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/json/__init__.py` & `vectice-24.2.4.0/src/vectice/api/json/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/json/artifact_version.py` & `vectice-24.2.4.0/src/vectice/api/json/artifact_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/json/code.py` & `vectice-24.2.4.0/src/vectice/api/json/code.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/json/code_version.py` & `vectice-24.2.4.0/src/vectice/api/json/code_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/json/dataset_register.py` & `vectice-24.2.4.0/src/vectice/api/json/dataset_register.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/json/dataset_representation.py` & `vectice-24.2.4.0/src/vectice/api/json/dataset_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/json/dataset_version.py` & `vectice-24.2.4.0/src/vectice/api/json/dataset_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/json/dataset_version_representation.py` & `vectice-24.2.4.0/src/vectice/api/json/dataset_version_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/json/files_metadata.py` & `vectice-24.2.4.0/src/vectice/api/json/files_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/json/iteration.py` & `vectice-24.2.4.0/src/vectice/api/json/iteration.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/json/json_to_class.py` & `vectice-24.2.4.0/src/vectice/api/json/json_to_class.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/json/last_assets.py` & `vectice-24.2.4.0/src/vectice/api/json/last_assets.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/json/metric.py` & `vectice-24.2.4.0/src/vectice/api/json/metric.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/json/model.py` & `vectice-24.2.4.0/src/vectice/api/json/model.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/json/model_register.py` & `vectice-24.2.4.0/src/vectice/api/json/model_register.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/json/model_representation.py` & `vectice-24.2.4.0/src/vectice/api/json/model_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/json/model_version.py` & `vectice-24.2.4.0/src/vectice/api/json/model_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/json/model_version_representation.py` & `vectice-24.2.4.0/src/vectice/api/json/model_version_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/json/paged_response.py` & `vectice-24.2.4.0/src/vectice/api/json/paged_response.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/json/phase.py` & `vectice-24.2.4.0/src/vectice/api/json/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/json/project.py` & `vectice-24.2.4.0/src/vectice/api/json/project.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/json/property.py` & `vectice-24.2.4.0/src/vectice/api/json/property.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/json/public_config.py` & `vectice-24.2.4.0/src/vectice/api/json/public_config.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/json/requirement.py` & `vectice-24.2.4.0/src/vectice/api/json/requirement.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/json/user_and_workspace.py` & `vectice-24.2.4.0/src/vectice/api/json/user_and_workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/json/workspace.py` & `vectice-24.2.4.0/src/vectice/api/json/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/phase.py` & `vectice-24.2.4.0/src/vectice/api/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/project.py` & `vectice-24.2.4.0/src/vectice/api/project.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/rest_api.py` & `vectice-24.2.4.0/src/vectice/api/rest_api.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/version.py` & `vectice-24.2.4.0/src/vectice/api/version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/api/workspace.py` & `vectice-24.2.4.0/src/vectice/api/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/autolog/asset_services/__init__.py` & `vectice-24.2.4.0/src/vectice/autolog/asset_services/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/autolog/asset_services/catboost_service.py` & `vectice-24.2.4.0/src/vectice/autolog/asset_services/catboost_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/autolog/asset_services/keras_service.py` & `vectice-24.2.4.0/src/vectice/autolog/asset_services/keras_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/autolog/asset_services/lightgbm_service.py` & `vectice-24.2.4.0/src/vectice/autolog/asset_services/lightgbm_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/autolog/asset_services/metric_service.py` & `vectice-24.2.4.0/src/vectice/autolog/asset_services/metric_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/autolog/asset_services/pytorch_service.py` & `vectice-24.2.4.0/src/vectice/autolog/asset_services/pytorch_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/autolog/asset_services/sklearn_service.py` & `vectice-24.2.4.0/src/vectice/autolog/asset_services/sklearn_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/autolog/asset_services/vectice_asset_service.py` & `vectice-24.2.4.0/src/vectice/autolog/asset_services/vectice_asset_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/autolog/autolog.py` & `vectice-24.2.4.0/src/vectice/autolog/autolog.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-# This captures the code called, we then use regex to identify the variables in locals. The variables found can then be logged to vectice.
 """Auto-Logging assets with Vectice.
 
 NOTE: **IMPORTANT INFORMATION**
     Autolog is continuously evolving to enhance supported libraries, environments, and functionalities to provide an improved user experience.
 
     Your feedback is highly valued. Please send any feedback to support@vectice.com.
 
 ------------
-The enhanced auto-logging feature in Vectice allows for seamless documentation and management of your data science projects. Please note the following details about this feature.
+The autolog feature in Vectice allows for seamless documentation and management of your data science projects. Please note the following details about this feature.
 
 NOTE: **This feature is designed to work specifically with notebooks.**
 
 1.** Installation:**
-    To enable the auto-logging feature, install the additional dependencies using the following command:
+    Make sure you install Vectice package using the following command:
 
     ```bash
-    pip install vectice[autolog]
+    pip install vectice
     ```
 
 2.** Supported libraries and environment:**
     Vectice automatically identifies and log assets encapsulated within a specified list of supported libraries and environement mentioned below
 
 NOTE: **Supported libraries and environment**
     - Dataframe: Pandas, Spark.
@@ -34,14 +33,15 @@
     - For GRAPHS, ensure they are saved as files to be automatically logged in the iteration i.e:
         - plt.savefig("my figure.png") (for seaborn or matploltlib)
         - fig.write_image("my figure.png") (for plotly)
     - For METRICS, Vectice currently recognizes sklearn metrics for automatic association with models.
         - In cases there's ambiguity due to multiple models with different metrics, Vectice won't automatically link them. To establish the link, make sure each model and its respective metrics are placed within the same notebook cell.
 
 """
+
 from __future__ import annotations
 
 import logging
 from typing import TYPE_CHECKING
 
 from typing_extensions import TypedDict
```

### Comparing `vectice-24.2.3.0/src/vectice/autolog/autolog_asset_factory.py` & `vectice-24.2.4.0/src/vectice/autolog/autolog_asset_factory.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/autolog/autolog_class.py` & `vectice-24.2.4.0/src/vectice/autolog/autolog_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,14 +220,15 @@
 
         self._iteration = iteration
         self._iteration_service = iteration._service  # pyright: ignore[reportPrivateUsage]
         self._capture_schema_only = capture_schema_only
         self._ip = ipy
         self._local_vars = self._ip.user_global_ns
         self._capture_comments = capture_comments
+        self._is_notebook = is_notebook
         self._cell_content = self._get_notebook_cell_content() if is_notebook is True else self._get_cell_content()
         self._vectice_data = self._get_variable_matches(self._local_vars)
         self._failed_assets = []
 
         # Get back objects to log
         self._assets = self._get_assets()
         graphs = self._get_graphs(is_notebook)
@@ -252,14 +253,15 @@
         if len(self._failed_assets):
             _logger.warning("The following assets failed to log:")
         for failed_asset in self._failed_assets:
             _logger.warning(f"{failed_asset['type']} {failed_asset['asset']!r}, reason: {failed_asset['reason']}")
 
     def _get_variable_matches(self, local_vars: dict[str, Any]) -> list[dict[Any, Any]]:
         vectice_data = []
+        all_cell_vars = set()
         all_vectice_calls = set()
         for cell_not_processed in self._cell_content:
             cell = preprocess_code(cell_not_processed)
             variable_comments = parse_comments(cell_not_processed) if self._capture_comments else []
             vectice_match = {}
             all_vars: OrderedDict[str, Any] = OrderedDict()
 
@@ -279,14 +281,19 @@
             # Keep set of all vectice call vars
             all_vectice_calls = all_vectice_calls.union(visitor.vectice_call_vars)
 
             # Update all_vars with variable names and values in the order they appear
             for var in visitor.variables:
                 if var in local_vars and var not in all_vars:
                     all_vars[var] = local_vars[var]
+                # check if the var exists in a previous cell for autolog.notebook before the vectice object uses the var
+                if self._is_notebook:
+                    all_vectice_calls = {vect_var for vect_var in all_vectice_calls if vect_var not in all_cell_vars}
+                # Keep track of all vars
+                all_cell_vars.add(var)
 
             vectice_match["variables"] = all_vars
             vectice_data.append(vectice_match)
         clean_vectice_data = []
         for data in vectice_data:
             for var in all_vectice_calls:
                 # the order of cells misses vars
```

### Comparing `vectice-24.2.3.0/src/vectice/connection.py` & `vectice-24.2.4.0/src/vectice/connection.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/__init__.py` & `vectice-24.2.4.0/src/vectice/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/additional_info.py` & `vectice-24.2.4.0/src/vectice/models/additional_info.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/attachment_container.py` & `vectice-24.2.4.0/src/vectice/models/attachment_container.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/code_version.py` & `vectice-24.2.4.0/src/vectice/models/code_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/dataset.py` & `vectice-24.2.4.0/src/vectice/models/dataset.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/iteration.py` & `vectice-24.2.4.0/src/vectice/models/iteration.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/metric.py` & `vectice-24.2.4.0/src/vectice/models/metric.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/model.py` & `vectice-24.2.4.0/src/vectice/models/model.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/model_exp_tracker.py` & `vectice-24.2.4.0/src/vectice/models/model_exp_tracker.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/model_mlflow.py` & `vectice-24.2.4.0/src/vectice/models/model_mlflow.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/phase.py` & `vectice-24.2.4.0/src/vectice/models/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/project.py` & `vectice-24.2.4.0/src/vectice/models/project.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/property.py` & `vectice-24.2.4.0/src/vectice/models/property.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/representation/dataset_representation.py` & `vectice-24.2.4.0/src/vectice/models/representation/dataset_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/representation/dataset_version_representation.py` & `vectice-24.2.4.0/src/vectice/models/representation/dataset_version_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/representation/model_representation.py` & `vectice-24.2.4.0/src/vectice/models/representation/model_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/representation/model_version_representation.py` & `vectice-24.2.4.0/src/vectice/models/representation/model_version_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/resource/__init__.py` & `vectice-24.2.4.0/src/vectice/models/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/resource/base.py` & `vectice-24.2.4.0/src/vectice/models/resource/base.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/resource/bigquery_resource.py` & `vectice-24.2.4.0/src/vectice/models/resource/bigquery_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/resource/databricks_table_resource.py` & `vectice-24.2.4.0/src/vectice/models/resource/databricks_table_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/resource/description.py` & `vectice-24.2.4.0/src/vectice/models/resource/description.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/resource/file_resource.py` & `vectice-24.2.4.0/src/vectice/models/resource/file_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/resource/gcs_resource.py` & `vectice-24.2.4.0/src/vectice/models/resource/gcs_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/resource/metadata/__init__.py` & `vectice-24.2.4.0/src/vectice/models/resource/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/resource/metadata/base.py` & `vectice-24.2.4.0/src/vectice/models/resource/metadata/base.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/resource/metadata/column_metadata.py` & `vectice-24.2.4.0/src/vectice/models/resource/metadata/column_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/resource/metadata/dataframe_config.py` & `vectice-24.2.4.0/src/vectice/models/resource/metadata/dataframe_config.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/resource/metadata/db_metadata.py` & `vectice-24.2.4.0/src/vectice/models/resource/metadata/db_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/resource/metadata/df_wrapper_pandas.py` & `vectice-24.2.4.0/src/vectice/models/resource/metadata/df_wrapper_pandas.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py` & `vectice-24.2.4.0/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py` & `vectice-24.2.4.0/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/resource/metadata/df_wrapper_resource.py` & `vectice-24.2.4.0/src/vectice/models/resource/metadata/df_wrapper_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/resource/metadata/df_wrapper_spark_df.py` & `vectice-24.2.4.0/src/vectice/models/resource/metadata/df_wrapper_spark_df.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/resource/metadata/files_metadata.py` & `vectice-24.2.4.0/src/vectice/models/resource/metadata/files_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py` & `vectice-24.2.4.0/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/resource/metadata/source.py` & `vectice-24.2.4.0/src/vectice/models/resource/metadata/source.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/resource/no_resource.py` & `vectice-24.2.4.0/src/vectice/models/resource/no_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/resource/s3_resource.py` & `vectice-24.2.4.0/src/vectice/models/resource/s3_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/resource/snowflake_resource.py` & `vectice-24.2.4.0/src/vectice/models/resource/snowflake_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/table.py` & `vectice-24.2.4.0/src/vectice/models/table.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/test_library/binary_classification_test.py` & `vectice-24.2.4.0/src/vectice/models/test_library/binary_classification_test.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/validation.py` & `vectice-24.2.4.0/src/vectice/models/validation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/models/workspace.py` & `vectice-24.2.4.0/src/vectice/models/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/services/iteration_service.py` & `vectice-24.2.4.0/src/vectice/services/iteration_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/services/phase_service.py` & `vectice-24.2.4.0/src/vectice/services/phase_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/types/version.py` & `vectice-24.2.4.0/src/vectice/types/version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/utils/code_parser.py` & `vectice-24.2.4.0/src/vectice/utils/code_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -127,25 +127,33 @@
             for arg in args:
                 arg_value = self._get_arg_or_kwarg_val(arg)
                 if arg_value:
                     if hasattr(arg_value, "__iter__") and not isinstance(arg_value, str):
                         self.function_call_args = self.function_call_args.union(arg_value)
                     else:
                         self.function_call_args.add(arg_value)  # pyright: ignore[reportAttributeAccessIssue]
-                if (
-                    hasattr(node.func, "id")
-                    and self._is_vectice_call_vars(node.func.id)  # pyright: ignore[reportAttributeAccessIssue]
-                    and arg_value
-                ):
+
+                func_name = self._get_function_name(node)
+                if self._is_vectice_call_vars(func_name) and arg_value:  # pyright: ignore[reportAttributeAccessIssue]
                     if hasattr(arg_value, "__iter__") and not isinstance(arg_value, str):
                         self.vectice_call_vars = self.vectice_call_vars.union(arg_value)
                     else:
                         self.vectice_call_vars.add(arg_value)
         self.generic_visit(node)
 
+    def _get_function_name(self, node: ast.Call) -> str | None:
+        try:
+            if hasattr(node.func, "id"):
+                return node.func.id  # pyright: ignore[reportAttributeAccessIssue]
+            if hasattr(node.func, "value"):
+                return node.func.value.id  # pyright: ignore[reportAttributeAccessIssue]
+        except AttributeError:
+            pass
+        return None
+
     ##### VariableVisitor methods
 
     def _extract_variables_from_target(self, target: ast.expr) -> None:
         if isinstance(target, ast.Constant):
             return
         if isinstance(target, ast.Name):
             self.visit_Name(target)
@@ -187,31 +195,35 @@
             pass
         try:
             # kwarg value if it is a variable
             return arg.value.id
         except AttributeError:
             pass
         try:
-            # kwarg value if it is a list
-            return {arg_value.id for arg_value in arg.value.elts}
+            # kwarg value if it is a list, list can contain multiple var types so we recursilvely get the arg/kwarg
+            return {self._get_arg_or_kwarg_val(arg_value) for arg_value in arg.value.elts}
         except AttributeError:
             pass
         return None
 
-    def _is_vectice_call_vars(self, func_name: str) -> bool:
+    def _is_vectice_call_vars(self, func_name: str | None) -> bool:
+        if not func_name:
+            return False
         vectice_functions = [
             "NoResource",
             "Resource",
             "Table",
             "SnowflakeResource",
             "FileResource",
             "GCSResource",
             "S3Resource",
             "BigQueryResource",
             "DatabricksTableResource",
+            "Dataset",
+            "Model",
         ]
         if func_name in vectice_functions:
             return True
         return False
 
     def _is_metric_call_vars(self, func_name: str) -> bool:
         from sklearn.metrics import (
```

### Comparing `vectice-24.2.3.0/src/vectice/utils/common_utils.py` & `vectice-24.2.4.0/src/vectice/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/utils/configuration.py` & `vectice-24.2.4.0/src/vectice/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/utils/dataframe_utils.py` & `vectice-24.2.4.0/src/vectice/utils/dataframe_utils.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/utils/deprecation.py` & `vectice-24.2.4.0/src/vectice/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/utils/instance_helper.py` & `vectice-24.2.4.0/src/vectice/utils/instance_helper.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/utils/last_assets.py` & `vectice-24.2.4.0/src/vectice/utils/last_assets.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice/utils/logging_utils.py` & `vectice-24.2.4.0/src/vectice/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice.egg-info/PKG-INFO` & `vectice-24.2.4.0/src/vectice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectice
-Version: 24.2.3.0
+Version: 24.2.4.0
 Summary: Vectice Python library
 Home-page: https://www.vectice.com
 Author: Vectice Inc.
 Author-email: sdk@vectice.com
 License: Apache License 2.0
 Keywords: Vectice,Client,API,Adapter
 Platform: Linux
@@ -12,15 +12,14 @@
 Platform: Windows
 Classifier: Topic :: Internet
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -37,14 +36,15 @@
 Requires-Dist: gql[requests]
 Requires-Dist: GitPython
 Requires-Dist: packaging
 Requires-Dist: Pillow
 Requires-Dist: pandas
 Requires-Dist: typing-extensions>=4.5.0
 Requires-Dist: dataclasses-json==0.5.8
+Requires-Dist: IPython
 Provides-Extra: dev
 Requires-Dist: black==24.2.0; extra == "dev"
 Requires-Dist: gitpython; extra == "dev"
 Requires-Dist: pyright==1.1.360; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-requests; extra == "dev"
 Requires-Dist: types-urllib3; extra == "dev"
@@ -94,19 +94,16 @@
 Requires-Dist: catboost; extra == "test"
 Requires-Dist: torch; extra == "test"
 Provides-Extra: gcs
 Requires-Dist: google-cloud-storage>=1.17.0; extra == "gcs"
 Requires-Dist: google-cloud-bigquery; extra == "gcs"
 Provides-Extra: s3
 Requires-Dist: boto3; extra == "s3"
-Provides-Extra: autolog
-Requires-Dist: IPython; extra == "autolog"
 Provides-Extra: validation
 Requires-Dist: shap; extra == "validation"
 Requires-Dist: scipy; extra == "validation"
-Requires-Dist: pandas; extra == "validation"
 
 Auto-documentation for ML projects & their governance. View https://github.com/vectice/GettingStarted to get started.
 
 # Documentation
 
 Official documentation for Vectice can be found at https://docs.vectice.com.
```

### Comparing `vectice-24.2.3.0/src/vectice.egg-info/SOURCES.txt` & `vectice-24.2.4.0/src/vectice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vectice-24.2.3.0/src/vectice.egg-info/requires.txt` & `vectice-24.2.4.0/src/vectice.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 gql[requests]
 GitPython
 packaging
 Pillow
 pandas
 typing-extensions>=4.5.0
 dataclasses-json==0.5.8
-
-[autolog]
 IPython
 
 [dev]
 black==24.2.0
 gitpython
 pyright==1.1.360
 ruff
@@ -74,8 +72,7 @@
 xgboost
 kaleido
 torch
 
 [validation]
 shap
 scipy
-pandas
```

