# Comparing `tmp/datarobot_early_access-3.4.0.2024.4.8.tar.gz` & `tmp/datarobot_early_access-3.5.0.2024.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/datarobot_early_access-3.4.0.2024.4.8.tar", last modified: Mon Apr  8 16:47:24 2024, max compression
+gzip compressed data, was "dist/datarobot_early_access-3.5.0.2024.5.6.tar", last modified: Mon May  6 16:47:31 2024, max compression
```

## Comparing `datarobot_early_access-3.4.0.2024.4.8.tar` & `datarobot_early_access-3.5.0.2024.5.6.tar`

### file list

```diff
@@ -1,216 +1,233 @@
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   223607 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/CHANGES.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7555 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/LICENSE.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      421 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/MANIFEST.in
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4234 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/PKG-INFO
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8911 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/README.md
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5852 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/common_setup.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2535 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      687 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_compat.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      553 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/__init__.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:46:29.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    25506 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/chunking_service.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15390 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/data_matching.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2742 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11628 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/enums.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:46:29.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5661 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/chat.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24973 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/chat_prompt.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5939 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/comparison_chat.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13717 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/comparison_prompt.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1818 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/custom_model_llm_validation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15919 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/custom_model_validation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10350 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/llm.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22662 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/llm_blueprint.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7281 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/playground.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6945 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/prompt_trace.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1200 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/user_limits.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27868 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/vector_database.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8693 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/idiomatic_project.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5416 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/incremental_learning.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6392 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    20913 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/model_lineage.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    30661 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/notebooks.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    54156 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/project_options.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9191 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/recipe_operations.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8966 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/recipes.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7408 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/retraining.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      313 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5241 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/analytics.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14682 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/client.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12682 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/config.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4664 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/context.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    32946 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/enums.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8984 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/errors.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/helpers/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27055 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/helpers/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13002 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/helpers/binary_data_utils.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1156 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/helpers/eligibility_result.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14350 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/helpers/feature_discovery.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8744 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/helpers/image_utils.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   101561 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/helpers/partitioning_methods.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/insights/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      200 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/insights/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9262 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/insights/base.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2698 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/insights/shap_impact.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1409 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/insights/shap_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1622 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/insights/shap_preview.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/mixins/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:46:29.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/mixins/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1134 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/mixins/browser_mixin.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1112 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/mixins/update_attributes_mixin.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4351 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9166 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/advanced_tuning.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27075 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/anomaly_assessment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2925 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/api_object.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9076 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/application.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15457 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/automated_documentation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    20521 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/batch_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    37053 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/batch_monitoring_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    86467 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/batch_prediction_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11451 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/blueprint.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    23822 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/calendar_file.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13301 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/change_request.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3978 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/cluster.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7233 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/cluster_insight.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12910 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/compliance_doc_template.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4889 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/confusion_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7244 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/connector.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    20307 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/credential.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    34090 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/custom_model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12413 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/custom_model_test.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    63934 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/custom_model_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15411 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/custom_task.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22991 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/custom_task_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2315 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/custom_task_version_dependency_build.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17613 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/data_engine_query_generator.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17068 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/data_slice.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17063 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/data_source.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    20149 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/data_store.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    75540 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    30524 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/datetime_trend_plots.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      544 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16779 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/accuracy.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5698 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/bias_and_fairness.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7095 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/challenger.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6170 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/champion_model_package.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    57732 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/custom_metrics.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12650 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/data_drift.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24249 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/data_exports.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   121466 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/deployment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1131 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/mixins.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10065 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/service_stats.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3450 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/sharing.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/documentai/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:46:29.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/documentai/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27024 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/documentai/document.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8427 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/driver.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9411 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/execution_environment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11344 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/execution_environment_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5376 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/external_baseline_validation.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/external_dataset_scores_insights/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      355 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/external_dataset_scores_insights/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6403 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4915 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4523 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/external_dataset_scores_insights/external_lift_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5208 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4521 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/external_dataset_scores_insights/external_roc_curve.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6789 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/external_dataset_scores_insights/external_scores.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    53938 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/feature.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/feature_association_matrix/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      237 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/feature_association_matrix/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2600 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/feature_association_matrix/feature_association_featurelists.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7052 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/feature_association_matrix/feature_association_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4753 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/feature_association_matrix/feature_association_matrix_details.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18312 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/feature_effect.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7003 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/feature_impact.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17463 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/featurelist.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7336 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/imported_model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21315 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13141 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/key_values.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6516 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/lift_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5468 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/missing_report.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   305975 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/model.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/model_registry/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      204 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/model_registry/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      408 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/model_registry/common.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3453 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/model_registry/deployment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26475 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/model_registry/registered_model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22985 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/model_registry/registered_model_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7215 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/modeljob.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14320 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/pairwise_statistics.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5438 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/pareto_front.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8726 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/payoff_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7403 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/predict_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10218 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/prediction_dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10918 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/prediction_environment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    39753 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/prediction_explanations.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2426 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/prediction_server.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15940 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/predictions.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2655 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/prime_file.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   224363 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/project.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    57175 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/project_options.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8774 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/rating_table.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4337 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/recommended_model.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/registry/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      345 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/registry/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16789 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/registry/job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10379 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/registry/job_run.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19064 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/relationships_configuration.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6645 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/residuals.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4524 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/restore_discarded_features.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11692 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/roc_curve.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2927 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/ruleset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5008 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/runtime_parameters.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19381 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/secondary_dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14217 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/segmentation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4722 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/shap_impact.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8216 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/shap_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2676 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/shap_matrix_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7314 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/sharing.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6267 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/status_check_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1431 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/trafarets.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    28260 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/training_predictions.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2029 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/types.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/use_cases/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      262 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/use_cases/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24890 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/use_cases/use_case.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13496 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/use_cases/utils.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/user_blueprints/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       49 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/user_blueprints/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    69649 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/user_blueprints/models.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8758 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/user_blueprints/trafarets.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2749 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/validators.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/visualai/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      226 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/visualai/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18528 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/visualai/augmentation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10521 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/visualai/images.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13615 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/visualai/insights.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4936 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/models/word_cloud.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:46:29.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/py.typed
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18404 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/rest.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/utils/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15618 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/utils/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2997 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/utils/deprecation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      495 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/utils/logger.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1200 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/utils/pagination.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1461 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/utils/retry.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1282 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/utils/source.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4109 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/utils/sourcedata.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4193 2024-04-08 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot/utils/waiters.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot_early_access.egg-info/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4234 2024-04-08 16:47:23.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot_early_access.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7540 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot_early_access.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        1 2024-04-08 16:47:23.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot_early_access.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1235 2024-04-08 16:47:23.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot_early_access.egg-info/requires.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       10 2024-04-08 16:47:23.000000 datarobot_early_access-3.4.0.2024.4.8/datarobot_early_access.egg-info/top_level.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3066 2024-04-08 16:46:29.000000 datarobot_early_access-3.4.0.2024.4.8/pyproject.toml
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      123 2024-04-08 16:47:24.000000 datarobot_early_access-3.4.0.2024.4.8/setup.cfg
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      965 2024-04-08 16:46:29.000000 datarobot_early_access-3.4.0.2024.4.8/setup.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2498 2024-04-08 16:46:29.000000 datarobot_early_access-3.4.0.2024.4.8/setup_weekly.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   231328 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/CHANGES.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7555 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/LICENSE.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      421 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/MANIFEST.in
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4234 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/PKG-INFO
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8911 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/README.md
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5852 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/common_setup.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2527 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      687 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_compat.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      553 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/__init__.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:46:22.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26398 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/chunking_service.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15390 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/data_matching.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2742 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5808 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/enums.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:46:22.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      379 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/chat.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14680 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/chat_prompt.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      390 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/comparison_chat.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4400 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/comparison_prompt.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5620 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/cost_metric_configurations.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      402 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/custom_model_llm_validation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9890 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/evaluation_dataset_configuration.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7350 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/evaluation_dataset_metric_aggregation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12541 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/insights_configuration.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      378 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/llm.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      388 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/llm_blueprint.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      385 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/playground.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7305 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/prompt_trace.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12780 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/sidecar_model_metric.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3237 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/synthetic_evaluation_dataset_generation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      386 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/user_limits.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9278 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/vector_database.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8693 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/idiomatic_project.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5416 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/incremental_learning.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6392 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    20913 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/model_lineage.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    31504 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/notebooks.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    54156 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/project_options.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9191 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/recipe_operations.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8966 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/recipes.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7408 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/retraining.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      313 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5241 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/analytics.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14682 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/client.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12682 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/config.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4664 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/context.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    40318 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/enums.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8984 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/errors.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/helpers/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27055 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/helpers/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13002 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/helpers/binary_data_utils.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1156 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/helpers/eligibility_result.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14350 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/helpers/feature_discovery.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8744 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/helpers/image_utils.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   101561 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/helpers/partitioning_methods.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/insights/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      200 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/insights/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9380 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/insights/base.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3057 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/insights/shap_impact.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1770 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/insights/shap_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1986 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/insights/shap_preview.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/mixins/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:46:22.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/mixins/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1134 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/mixins/browser_mixin.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1112 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/mixins/update_attributes_mixin.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4339 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9166 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/advanced_tuning.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27075 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/anomaly_assessment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2925 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/api_object.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9076 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/application.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15457 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/automated_documentation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    20521 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/batch_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    37053 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/batch_monitoring_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    86467 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/batch_prediction_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11451 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/blueprint.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    23822 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/calendar_file.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13301 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/change_request.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3978 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/cluster.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7233 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/cluster_insight.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12910 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/compliance_doc_template.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4889 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/confusion_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7244 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/connector.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    20307 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/credential.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    34090 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/custom_model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12413 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/custom_model_test.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    63934 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/custom_model_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15411 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/custom_task.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22991 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/custom_task_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2315 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/custom_task_version_dependency_build.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17613 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/data_engine_query_generator.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17068 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/data_slice.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17063 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/data_source.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    20149 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/data_store.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    75540 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    30524 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/datetime_trend_plots.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      544 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16779 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/accuracy.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5698 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/bias_and_fairness.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7095 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/challenger.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6170 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/champion_model_package.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    57732 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/custom_metrics.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12650 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/data_drift.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24249 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/data_exports.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   121466 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/deployment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1131 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/mixins.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10065 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/service_stats.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3450 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/sharing.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/documentai/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:46:22.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/documentai/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27024 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/documentai/document.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8427 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/driver.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9411 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/execution_environment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11344 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/execution_environment_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5376 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_baseline_validation.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      355 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6403 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4915 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4523 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/external_lift_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5208 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4521 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/external_roc_curve.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6789 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/external_scores.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    53938 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature_association_matrix/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      237 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature_association_matrix/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2600 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature_association_matrix/feature_association_featurelists.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7052 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature_association_matrix/feature_association_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4753 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature_association_matrix/feature_association_matrix_details.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18312 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature_effect.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7003 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature_impact.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17463 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/featurelist.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      455 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5647 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/chat.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18029 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/chat_prompt.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5925 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/comparison_chat.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12076 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/comparison_prompt.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2168 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/custom_model_llm_validation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16900 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/custom_model_validation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10350 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/llm.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22899 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/llm_blueprint.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7299 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/playground.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1200 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/user_limits.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26873 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/vector_database.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21315 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13141 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/key_values.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6516 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/lift_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5468 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/missing_report.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   303355 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/model.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/model_registry/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      204 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/model_registry/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      408 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/model_registry/common.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3453 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/model_registry/deployment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26475 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/model_registry/registered_model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22985 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/model_registry/registered_model_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7215 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/modeljob.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14320 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/pairwise_statistics.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5438 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/pareto_front.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8726 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/payoff_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7403 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/predict_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10218 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/prediction_dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10918 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/prediction_environment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    39753 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/prediction_explanations.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2426 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/prediction_server.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15940 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/predictions.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2655 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/prime_file.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   224363 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/project.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    57175 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/project_options.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8774 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/rating_table.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4337 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/recommended_model.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/registry/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      345 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/registry/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16789 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/registry/job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10379 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/registry/job_run.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19064 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/relationships_configuration.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6645 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/residuals.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4524 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/restore_discarded_features.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11692 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/roc_curve.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2927 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/ruleset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5008 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/runtime_parameters.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19381 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/secondary_dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14217 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/segmentation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4722 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/shap_impact.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8216 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/shap_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2676 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/shap_matrix_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7314 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/sharing.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6267 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/status_check_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1431 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/trafarets.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    28260 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/training_predictions.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2029 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/types.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/use_cases/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      262 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/use_cases/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24890 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/use_cases/use_case.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13496 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/use_cases/utils.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/user_blueprints/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       49 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/user_blueprints/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    69649 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/user_blueprints/models.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8758 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/user_blueprints/trafarets.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2749 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/validators.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/visualai/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      226 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/visualai/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18528 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/visualai/augmentation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10521 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/visualai/images.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13615 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/visualai/insights.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4936 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/word_cloud.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:46:22.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/py.typed
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18404 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/rest.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15618 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2997 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/deprecation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      495 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/logger.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1200 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/pagination.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1461 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/retry.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1282 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/source.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4109 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/sourcedata.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4193 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/waiters.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot_early_access.egg-info/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4234 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot_early_access.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8344 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot_early_access.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        1 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot_early_access.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1235 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot_early_access.egg-info/requires.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       10 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot_early_access.egg-info/top_level.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3066 2024-05-06 16:46:22.000000 datarobot_early_access-3.5.0.2024.5.6/pyproject.toml
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      123 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/setup.cfg
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      965 2024-05-06 16:46:22.000000 datarobot_early_access-3.5.0.2024.5.6/setup.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2498 2024-05-06 16:46:22.000000 datarobot_early_access-3.5.0.2024.5.6/setup_weekly.py
```

### Comparing `datarobot_early_access-3.4.0.2024.4.8/CHANGES.rst` & `datarobot_early_access-3.5.0.2024.5.6/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,115 @@
 #########
 Changelog
 #########
+3.5.0b0
+=======
+
+Documentation changes
+*********************
+- Updated `genai_example.rst` to link to DataRobot doc pages for external vector database and external LLM deployment creation.
+
 3.4.0b0
 =======
 
 New features
 ************
+- Added a new class :class: `EvaluationDatasetConfiguration <datarobot._experimental.models.genai.evaluation_dataset_configuration.EvaluationDatasetConfiguration>` for configuration of evaluation datasets.
+  :meth:`EvaluationDatasetConfiguration.get <datarobot._experimental.models.genai.evaluation_dataset_configuration.EvaluationDatasetConfiguration.get>` to get an evaluation dataset configuration.
+  :meth:`EvaluationDatasetConfiguration.list <datarobot._experimental.models.genai.evaluation_dataset_configuration.EvaluationDatasetConfiguration.list>` to list the evaluation dataset configurations for a Use Case.
+  :meth:`EvaluationDatasetConfiguration.create <datarobot._experimental.models.genai.evaluation_dataset_configuration.EvaluationDatasetConfiguration.create>` to create an evaluation dataset configuration.
+  :meth:`EvaluationDatasetConfiguration.update <datarobot._experimental.models.genai.evaluation_dataset_configuration.EvaluationDatasetConfiguration.update>` to update an evaluation dataset configuration.
+  :meth:`EvaluationDatasetConfiguration.delete <datarobot._experimental.models.genai.evaluation_dataset_configuration.EvaluationDatasetConfiguration.delete>` to delete an evaluation dataset configuration.
+- Added a new class :class: `EvaluationDatasetMetricAggregation <datarobot._experimental.models.genai.evaluation_dataset_metric_aggregation.EvaluationDatasetMetricAggregation>` for metric aggregation results.
+  :meth:`EvaluationDatasetMetricAggregation.list <datarobot._experimental.models.genai.evaluation_dataset_metric_aggregation.EvaluationDatasetMetricAggregation.list>` to get the metric aggregation results.
+  :meth:`EvaluationDatasetMetricAggregation.create <datarobot._experimental.models.genai.evaluation_dataset_metric_aggregation.EvaluationDatasetMetricAggregation.create>` to create the metric aggregation job.
+  :meth:`EvaluationDatasetMetricAggregation.delete <datarobot._experimental.models.genai.evaluation_dataset_metric_aggregation.EvaluationDatasetMetricAggregation.delete>` to delete metric aggregation results.
+- Added a new class :class: `SyntheticEvaluationDataset <datarobot._experimental.models.genai.synthetic_evaluation_dataset_generation.SyntheticEvaluationDataset>` for synthetic dataset generation.
+  Use :meth:`SyntheticEvaluationDataset.create <datarobot._experimental.models.genai.synthetic_evaluation_dataset_generation.SyntheticEvaluationDataset.create>` to create a synthetic evaluation dataset.
+- Added a new class :class: `SidecarModelMetricValidation <datarobot._experimental.models.genai.sidecar_model_metric.SidecarModelMetricValidation>` for sidecar model metric validations.
+  :meth:`SidecarModelMetricValidation.create <datarobot._experimental.models.genai.sidecar_model_metric.SidecarModelMetricValidation.create>` to create a sidecar model metric validation.
+  :meth:`SidecarModelMetricValidation.list <datarobot._experimental.models.genai.sidecar_model_metric.SidecarModelMetricValidation.list>` to list sidecar model metric validations.
+  :meth:`SidecarModelMetricValidation.get <datarobot._experimental.models.genai.sidecar_model_metric.SidecarModelMetricValidation.get>` to get a sidecar model metric validation.
+  :meth:`SidecarModelMetricValidation.revalidate <datarobot._experimental.models.genai.sidecar_model_metric.SidecarModelMetricValidation.revalidate>` to rerun a sidecar model metric validation.
+  :meth:`SidecarModelMetricValidation.update <datarobot._experimental.models.genai.sidecar_model_metric.SidecarModelMetricValidation.update>` to update a sidecar model metric validation.
+  :meth:`SidecarModelMetricValidation.delete <datarobot._experimental.models.genai.sidecar_model_metric.SidecarModelMetricValidation.delete>` to delete a sidecar model metric validation.
+- Added experimental support for Chunking Service:
+
+  - Added a new attribute, `is_descending_order` to:
+
+    - :class:`DatasourceDefinition <datarobot._experimental.models.chunking_service.DatasourceDefinition>`
+    - :class:`DatasourceAICatalogInfo <datarobot._experimental.models.chunking_service.DatasourceAICatalogInfo>`
+    - :class:`DatasourceDataWarehouseInfo <datarobot._experimental.models.chunking_service.DatasourceDataWarehouseInfo>`
+
+
+Enhancements
+************
+
+Bugfixes
+********
+
+API changes
+***********
+- Remove `ImportedModel` object since it was API for SSE (standalone scoring engine) which is not part of DataRobot anymore.
+
+Deprecation summary
+*******************
+
+Configuration changes
+*********************
+
+Documentation changes
+*********************
+
+Experimental changes
+********************
+
+3.4.0
+=====
+
+New features
+************
+- Added the following classes for generative AI. Importing these from `datarobot._experimental.models.genai` is deprecated and will be removed by the release of DataRobot 10.1 and SDK 3.5.
+  - :class:`Playground <datarobot.models.genai.playground.Playground>` to manage generative AI playgrounds.
+  - :class:`LLMDefinition <datarobot.models.genai.llm.LLMDefinition>` to get information about supported LLMs.
+  - :class:`LLMBlueprint <datarobot.models.genai.llm_blueprint.LLMBlueprint>` to manage LLM blueprints.
+  - :class:`Chat <datarobot.models.genai.chat.Chat>` to manage chats for LLM blueprints.
+  - :class:`ChatPrompt <datarobot.models.genai.chat_prompt.ChatPrompt>` to submit prompts within a chat.
+  - :class:`ComparisonChat <datarobot.models.genai.comparison_chat.ComparisonChat>` to manage comparison chats across multiple LLM blueprints within a playground.
+  - :class:`ComparisonPrompt <datarobot.models.genai.comparison_prompt.ComparisonPrompt>` to submit a prompt to multiple LLM blueprints within a comparison chat.
+  - :class:`VectorDatabase <datarobot.models.genai.vector_database.VectorDatabase>` to create vector databases from datasets in the AI Catalog for retrieval augmented generation with an LLM blueprint.
+  - :class:`CustomModelVectorDatabaseValidation <datarobot.models.genai.vector_database.CustomModelVectorDatabaseValidation>` to validate a deployment for use as a vector database.
+  - :class:`CustomModelLLMValidation <datarobot.models.genai.custom_model_llm_validation.CustomModelLLMValidation>` to validate a deployment for use as an LLM.
+  - :class:`UserLimits <datarobot.models.genai.user_limits.UserLimits>` to get counts of vector databases and LLM requests for a user.
 
 - Extended the advanced options available when setting a target to include new
   parameter: 'incrementalLearningEarlyStoppingRounds'(part of the AdvancedOptions object).
   This parameter allows you to specify when to stop for incremental learning automation.
 - Added experimental support for Chunking Service:
-    - :class:`DatasetChunkDefinition <datarobot._experimental.models.chunking_service.DatasetChunkDefinition>` for defining how chunks are created from a data source.
-        - :meth:`DatasetChunkDefinition.create <datarobot._experimental.models.chunking_service.DatasetChunkDefinition.create>` to create a new dataset chunk definition.
-        - :meth:`DatasetChunkDefinition.get <datarobot._experimental.models.chunking_service.DatasetChunkDefinition.get>` to get a specific dataset chunk definition.
-        - :meth:`DatasetChunkDefinition.list <datarobot._experimental.models.chunking_service.DatasetChunkDefinition.get>` to list all dataset chunk definitions.
-        - :meth:`DatasetChunkDefinition.get_datasource_definition <datarobot._experimental.models.chunking_service.DatasetChunkDefinition.get_datasource_definition>` to retrieve the data source definition.
-        - :meth:`DatasetChunkDefinition.get_chunk <datarobot._experimental.models.chunking_service.DatasetChunkDefinition.get_chunk>` to get specific chunk metadata belonging to a dataset chunk definition.
-        - :meth:`DatasetChunkDefinition.list_chunks <datarobot._experimental.models.chunking_service.DatasetChunkDefinition.list_chunks>` to list all chunk metadata belonging to a dataset chunk definition.
-        - :meth:`DatasetChunkDefinition.create_chunk <datarobot._experimental.models.chunking_service.DatasetChunkDefinition.create_chunk>` to submit a job to retrieve the data from the origin data source.
-        - :meth:`DatasetChunkDefinition.create_chunk_by_index <datarobot._experimental.models.chunking_service.DatasetChunkDefinition.create_chunk_by_index>` to submit a job to retrieve data from the origin data source by index.
-    - :class:`OriginStorageType <datarobot._experimental.models.chunking_service.OriginStorageType>`
-    - :class:`Chunk <datarobot._experimental.models.chunking_service.Chunk>`
-    - :class:`ChunkStorageType <datarobot._experimental.models.chunking_service.ChunkStorageType>`
-    - :class:`ChunkStorage <datarobot._experimental.models.chunking_service.ChunkStorage>`
-    - :class:`DatasourceDefinition <datarobot._experimental.models.chunking_service.DatasourceDefinition>`
-    - :class:`DatasourceAICatalogInfo <datarobot._experimental.models.chunking_service.DatasourceAICatalogInfo>` to define the datasource AI catalog information to create a new dataset chunk definition.
-    - :class:`DatasourceDataWarehouseInfo <datarobot._experimental.models.chunking_service.DatasourceDataWarehouseInfo>` to define the datasource data warehouse (snowflake, big query, etc) information to create a new dataset chunk definition.
-    - :class:`RuntimeParameter <datarobot.models.custom_model_version.RuntimeParameter>` for retrieving runtime parameters assigned to :class:`CustomModelVersion <datarobot.CustomModelVersion>`.
-    - :class:`RuntimeParameterValue <datarobot.models.custom_model_version.RuntimeParameterValue>` to define runtime parameter override value, to be assigned to :class:`CustomModelVersion <datarobot.CustomModelVersion>`.
+
+  - :class:`DatasetChunkDefinition <datarobot._experimental.models.chunking_service.DatasetChunkDefinition>` for defining how chunks are created from a data source.
+
+    - :meth:`DatasetChunkDefinition.create <datarobot._experimental.models.chunking_service.DatasetChunkDefinition.create>` to create a new dataset chunk definition.
+    - :meth:`DatasetChunkDefinition.get <datarobot._experimental.models.chunking_service.DatasetChunkDefinition.get>` to get a specific dataset chunk definition.
+    - :meth:`DatasetChunkDefinition.list <datarobot._experimental.models.chunking_service.DatasetChunkDefinition.get>` to list all dataset chunk definitions.
+    - :meth:`DatasetChunkDefinition.get_datasource_definition <datarobot._experimental.models.chunking_service.DatasetChunkDefinition.get_datasource_definition>` to retrieve the data source definition.
+    - :meth:`DatasetChunkDefinition.get_chunk <datarobot._experimental.models.chunking_service.DatasetChunkDefinition.get_chunk>` to get specific chunk metadata belonging to a dataset chunk definition.
+    - :meth:`DatasetChunkDefinition.list_chunks <datarobot._experimental.models.chunking_service.DatasetChunkDefinition.list_chunks>` to list all chunk metadata belonging to a dataset chunk definition.
+    - :meth:`DatasetChunkDefinition.create_chunk <datarobot._experimental.models.chunking_service.DatasetChunkDefinition.create_chunk>` to submit a job to retrieve the data from the origin data source.
+    - :meth:`DatasetChunkDefinition.create_chunk_by_index <datarobot._experimental.models.chunking_service.DatasetChunkDefinition.create_chunk_by_index>` to submit a job to retrieve data from the origin data source by index.
+
+  - :class:`OriginStorageType <datarobot._experimental.models.chunking_service.OriginStorageType>`
+  - :class:`Chunk <datarobot._experimental.models.chunking_service.Chunk>`
+  - :class:`ChunkStorageType <datarobot._experimental.models.chunking_service.ChunkStorageType>`
+  - :class:`ChunkStorage <datarobot._experimental.models.chunking_service.ChunkStorage>`
+  - :class:`DatasourceDefinition <datarobot._experimental.models.chunking_service.DatasourceDefinition>`
+  - :class:`DatasourceAICatalogInfo <datarobot._experimental.models.chunking_service.DatasourceAICatalogInfo>` to define the datasource AI catalog information to create a new dataset chunk definition.
+  - :class:`DatasourceDataWarehouseInfo <datarobot._experimental.models.chunking_service.DatasourceDataWarehouseInfo>` to define the datasource data warehouse (snowflake, big query, etc) information to create a new dataset chunk definition.
+  - :class:`RuntimeParameter <datarobot.models.custom_model_version.RuntimeParameter>` for retrieving runtime parameters assigned to :class:`CustomModelVersion <datarobot.CustomModelVersion>`.
+  - :class:`RuntimeParameterValue <datarobot.models.custom_model_version.RuntimeParameterValue>` to define runtime parameter override value, to be assigned to :class:`CustomModelVersion <datarobot.CustomModelVersion>`.
 
 - Added Snowflake Key Pair authentication for uploading datasets from Snowflake or creating a project from Snowflake data
 - Added :meth:`Project.get_model_records <datarobot.models.Project.get_model_records>` to retrieve models.
   Method :meth:`Project.get_models <datarobot.models.Project.get_models>` is deprecated and will be removed soon in favour of :meth:`Project.get_model_records <datarobot.models.Project.get_model_records>`.
 - Extended the advanced options available when setting a target to include new
   parameter: 'chunkDefinitionId'(part of the AdvancedOptions object). This parameter allows you to specify the chunking definition needed for incremental learning automation.
 - Extended the advanced options available when setting a target to include new Autopilot
@@ -46,15 +123,14 @@
 - Update method :meth:`DatetimeModel.get_or_request_feature_impact<datarobot.models.DatetimeModel.get_or_request_feature_impact>` to support use of Sliced Insights.
 - Update method :meth:`DatetimeModel.request_feature_effect<datarobot.models.DatetimeModel.request_feature_effect>` to support use of Sliced Insights.
 - Update method :meth:`DatetimeModel.get_feature_effect<datarobot.models.DatetimeModel.get_feature_effect>` to support use of Sliced Insights.
 - Update method :meth:`DatetimeModel.get_or_request_feature_effect<datarobot.models.DatetimeModel.get_or_request_feature_effect>` to support use of Sliced Insights.
 - Added a new method :meth:`FeatureAssociationMatrix.create<datarobot.models.FeatureAssociationMatrix.create>` to support the creation of FeatureAssociationMatricies for Featurelists.
 - Introduced a new method :meth:`Deployment.perform_model_replace<datarobot.models.Deployment.perform_model_replace>` as a replacement for :meth:`Deployment.replace_model<datarobot.models.Deployment.replace_model>`.
 - Introduced a new property, `model_package`, which provides an overview of the currently used model package in :class:`datarobot.models.Deployment`.
-- Updated the client configuration flow to enhance flexibility and user control. Client configuration will be overwritten via params passed to ``datarobot.client.Client()``.
 - Added new parameter `prediction_threshold` to :meth:`BatchPredictionJob.score_with_leaderboard_model <datarobot.models.BatchPredictionJob.score_with_leaderboard_model>`
   and :meth:`BatchPredictionJob.score <datarobot.models.BatchPredictionJob.score>` that automatically assigns the positive class label to any prediction exceeding the threshold.
 - Added two new enum values to  :class: `datarobot.models.data_slice.DataSlicesOperators`, "BETWEEN" and "NOT_BETWEEN", which are used to allow slicing.
 - Added a new class :class:`Challenger <datarobot.models.deployment.challenger.Challenger>` for interacting with DataRobot challengers to support the following methods:
   :meth:`Challenger.get <datarobot.models.deployment.challenger.Challenger.get>` to retrieve challenger objects by ID.
   :meth:`Challenger.list <datarobot.models.deployment.challenger.Challenger.list>` to list all challengers.
   :meth:`Challenger.create <datarobot.models.deployment.challenger.Challenger.create>` to create a new challenger.
@@ -63,21 +139,21 @@
 - Added a new method :meth:`Deployment.get_challenger_replay_settings <datarobot.models.Deployment.get_challenger_replay_settings>` to retrieve the challenger replay settings of a deployment.
 - Added a new method :meth:`Deployment.list_challengers <datarobot.models.Deployment.list_challengers>` to retrieve the challengers of a deployment.
 - Added a new method :meth:`Deployment.get_champion_model_package <datarobot.models.Deployment.get_champion_model_package>` to retrieve the champion model package from a deployment.
 - Added a new method :meth:`Deployment.list_prediction_data_exports <datarobot.models.Deployment.list_prediction_data_exports>` to retrieve deployment prediction data exports.
 - Added a new method :meth:`Deployment.list_actuals_data_exports <datarobot.models.Deployment.list_actuals_data_exports>` to retrieve deployment actuals data exports.
 - Added a new method :meth:`Deployment.list_training_data_exports <datarobot.models.Deployment.list_training_data_exports>` to retrieve deployment training data exports.
 - Manage deployment health settings with the following methods:
-    - Get health settings :meth:`Deployment.get_health_settings <datarobot.models.Deployment.get_health_settings>`
-    - Update health settings :meth:`Deployment.update_health_settings <datarobot.models.Deployment.update_health_settings>`
-    - Get default health settings :meth:`Deployment.get_default_health_settings <datarobot.models.Deployment.get_default_health_settings>`
+  - Get health settings :meth:`Deployment.get_health_settings <datarobot.models.Deployment.get_health_settings>`
+  - Update health settings :meth:`Deployment.update_health_settings <datarobot.models.Deployment.update_health_settings>`
+  - Get default health settings :meth:`Deployment.get_default_health_settings <datarobot.models.Deployment.get_default_health_settings>`
 - Added new enum value to ``datarobot.enums._SHARED_TARGET_TYPE`` to support Text Generation use case.
 - Added new enum value ``datarobotServerless`` to ``datarobot.enums.PredictionEnvironmentPlatform`` to support DataRobot Serverless prediction environments.
 - Added new enum value ``notApplicable`` to ``datarobot.enums.PredictionEnvironmentHealthType`` to support new health status from DataRobot API.
-- Added a new enum value to ``datarobot.enums.TARGET_TYPE`` and ``datarobot.enums.CUSTOM_MODEL_TARGET_TYPE`` to support text generation custom inference models.
+- Added new enum value to ``datarobot.enums.TARGET_TYPE`` and ``datarobot.enums.CUSTOM_MODEL_TARGET_TYPE`` to support text generation custom inference models.
 - Updated ``datarobot.CustomModel`` to support the creation of text generation custom models.
 - Added a new class :class:`CustomMetric <datarobot.models.deployment.custom_metrics.CustomMetric>` for interacting with DataRobot custom metrics to support the following methods:
   :meth:`CustomMetric.get <datarobot.models.deployment.custom_metrics.CustomMetric.get>` to retrieve a custom metric object by ID from a given deployment.
   :meth:`CustomMetric.list <datarobot.models.deployment.custom_metrics.CustomMetric.list>` to list all custom metrics from a given deployment.
   :meth:`CustomMetric.create <datarobot.models.deployment.custom_metrics.CustomMetric.create>` to create a new custom metric for a given deployment.
   :meth:`CustomMetric.update <datarobot.models.deployment.custom_metrics.CustomMetric.update>` to update a custom metric for a given deployment.
   :meth:`CustomMetric.delete <datarobot.models.deployment.custom_metrics.CustomMetric.delete>` to delete a custom metric for a given deployment.
@@ -111,52 +187,62 @@
   :meth:`TrainingDataExport.create <datarobot.models.deployment.data_exports.TrainingDataExport.create>` to create a new training data export for a given deployment.
   :meth:`TrainingDataExport.fetch_data <datarobot.models.deployment.data_exports.TrainingDataExport.fetch_data>` to retrieve a training export data as a DataRobot dataset.
 - Added a new parameter `base_environment_version_id` to :meth:`CustomModelVersion.create_clean <datarobot.CustomModelVersion.create_clean>` for overriding the default environment version selection behavior.
 - Added a new parameter `base_environment_version_id` to :meth:`CustomModelVersion.create_from_previous <datarobot.CustomModelVersion.create_from_previous>` for overriding the default environment version selection behavior.
 - Added a new class :class:`PromptTrace <datarobot._experimental.models.genai.prompt_trace.PromptTrace>` for interacting with DataRobot prompt trace to support the following methods:
   :meth:`PromptTrace.list <datarobot._experimental.models.genai.prompt_trace.PromptTrace.list>` to list all prompt traces from a given playground.
   :meth:`PromptTrace.export_to_ai_catalog <datarobot._experimental.models.genai.prompt_trace.PromptTrace.export_to_ai_catalog>` to export prompt traces for the playground to AI catalog.
+- Added a new class :class: `InsightsConfiguration <datarobot._experimental.models.genai.insights_configuration.InsightsConfiguration>` for describing available insights and configured insights for a playground.
+  :meth:`InsightsConfiguration.list <datarobot._experimental.models.genai.insights_configuration.InsightsConfiguration.list>` to list the insights that are available to be configured.
+- Added a new class :class: `Insights <datarobot._experimental.models.genai.insights_configuration.Insights>` for configuring insights for a playground.
+  :meth:`Insights.get <datarobot._experimental.models.genai.insights_configuration.Insights.get>` to get the current insights configuration for a playground.
+  :meth:`Insights.create <datarobot._experimental.models.genai.insights_configuration.Insights.create>` to create or update the insights configuration for a playground.
+- Added a new class :class: `CostMetricConfiguration <datarobot._experimental.models.genai.cost_metric_configurations.CostMetricConfiguration>` for describing available cost metrics and configured cost metrics for a Use Case.
+  :meth:`CostMetricConfiguration.get <datarobot._experimental.models.genai.cost_metric_configurations.CostMetricConfiguration.get>` to get the cost metric configuration.
+  :meth:`CostMetricConfiguration.create <datarobot._experimental.models.genai.cost_metric_configurations.CostMetricConfiguration.create>` to create a cost metric configuration.
+  :meth:`CostMetricConfiguration.update <datarobot._experimental.models.genai.cost_metric_configurations.CostMetricConfiguration.update>` to update the cost metric configuration.
+  :meth:`CostMetricConfiguration.delete <datarobot._experimental.models.genai.cost_metric_configurations.CostMetricConfiguration.delete>` to delete the cost metric configuration.Key
+- Added a new class :class: `LLMCostConfiguration <datarobot._experimental.models.genai.cost_metric_configurations.LLMCostConfiguration>` for the cost configuration of a specific llm within a Use Case.
+- Added new classes :class: `ShapMatrix <datarobot.insights.shap_matrix.ShapMatrix>`, :class: `ShapImpact <datarobot.insights.shap_impact.ShapImpact>`, :class: `ShapPreview <datarobot.insights.shap_preview.ShapPreview>` to interact with SHAP-based insights. See also the User Guide: :ref:`SHAP insights overview<shap_insights_overview>`
 
-Key Changes
-  1.	Parameter Overrides: Users can now override most of the previously set configuration values directly through parameters when initializing the Client.
-  2.	Exceptions: The endpoint and token values must be initiated from one source(client params, environment, or config file) and cannot be overridden individually for security and consistency reasons.
-
-Configuration Priority:
-  1.	Client Params
-  2.    Client config_path param
-  3.	Environment Variables
-  4.	Default to reading YAML config file from `~/.config/datarobot/drconfig.yaml`
 
-- `DATAROBOT_API_CONSUMER_TRACKING_ENABLED` now always defaults to `True` in all cases.
+API changes
+***********
+- Parameter Overrides: Users can now override most of the previously set configuration values directly through parameters when initializing the Client. Exceptions: The endpoint and token values must be initialized from one source (client params, environment, or config file) and cannot be overridden individually, for security and consistency reasons. The new configuration priority is as follows:
+  1.  Client Params
+  2.  Client config_path param
+  3.  Environment Variables
+  4.  Default to reading YAML config file from `~/.config/datarobot/drconfig.yaml`
+- `DATAROBOT_API_CONSUMER_TRACKING_ENABLED` now always defaults to `True`.
 - Added Databricks personal access token and service principal (also shared credentials via secure config) authentication for uploading datasets from Databricks or creating a project from Databricks data.
 - Added secure config support for AWS long term credentials.
 - Implemented support for `dr-database-v1` to `DataStore <datarobot.models.DataStore>`, `DataSource <datarobot.models.DataStore>`, and  `DataDriver <datarobot.models.DataDriver>.` Added enum classes to support the changes.
 - You can retrieve the canonical URI for a Use Case using :meth:`UseCase.get_uri <datarobot.UseCase.get_uri>`.
 - You can open a Use Case in a browser using :meth:`UseCase.open_in_browser <datarobot.UseCase.open_in_browser>`.
 
 Enhancements
 ************
 - Added a new parameter to :meth:`Dataset.create_from_url <datarobot.models.Dataset.create_from_url>` to support fast dataset registration:
-    - `sample_size`
+  - `sample_size`
 - Added a new parameter to :meth:`Dataset.create_from_data_source <datarobot.models.Dataset.create_from_data_source>` to support fast dataset registration:
-    - `sample_size`
+  - `sample_size`
 - :meth:`Job.get_result_when_complete <datarobot.models.Job.get_result_when_complete>`
   returns :class:`datarobot.models.DatetimeModel` instead of the :class:`datarobot.models.Model`
   if a datetime model was trained.
 - :meth:`Dataset.get_as_dataframe <datarobot.models.Dataset.get_as_dataframe>` can handle
   downloading parquet files as well as csv files.
 - Implement support for `dr-database-v1` in `DataStore <datarobot.models.DataStore>`
 - Added two new parameters to :meth:`BatchPredictionJobDefinition.list <datarobot.models.BatchPredictionJobDefinition.list>` for paginating long job definitions lists:
-    - `offset`
-    - `limit`
+  - `offset`
+  - `limit`
 - Added two new parameters to :meth:`BatchPredictionJobDefinition.list <datarobot.models.BatchPredictionJobDefinition.list>` for filtering the job definitions:
-    - `deployment_id`
-    - `search_name`
+  - `deployment_id`
+  - `search_name`
 - Added new parameter to :meth:`Deployment.validate_replacement_model<datarobot.models.Deployment.validate_replacement_model>` to support replacement validation based on model package ID:
-    - `new_registered_model_version_id`
+  - `new_registered_model_version_id`
 - Added support for Native Connectors to `Connector <datarobot.models.Connector>` for everything other than :meth:` Connector.create <datarobot.models.Connector.create>` and :meth:` Connector.update <datarobot.models.Connector.update>`
 
 Deprecation summary
 *******************
 - Removed `Model.get_leaderboard_ui_permalink` and `Model.open_model_browser`
 - Deprecated :meth:`Project.get_models <datarobot.models.Project.get_models>` in favour of :meth:`Project.get_model_records <datarobot.models.Project.get_model_records>`.
 - :meth:`BatchPredictionJobDefinition.list <datarobot.models.BatchPredictionJobDefinition.list>` will no longer return all job definitions after version 3.6 is released.
@@ -169,72 +255,74 @@
 
 Documentation changes
 *********************
 - Updated `genai_example.rst` to utilize latest genAI features and methods introduced most recently in the API client.
 
 Experimental changes
 *********************
+- Added new attribute, `prediction_timeout` to :class:`CustomModelValidation <datarobot.models.genai.custom_model_validation.CustomModelValidation>`.
 - Added new attributes, `feedback_result`, `metrics`, and `final_prompt` to :class:`ResultMetadata <datarobot._experimental.models.genai.chat_prompt.ResultMetadata>`.
-- Added `use_case_id` to :class:`CustomModelValidation <datarobot._experimental.models.genai.custom_model_validation.CustomModelValidation>`.
-- Added `llm_blueprints_count` and `user_name` to :class:`Playground <datarobot._experimental.models.genai.playground.Playground>`.
+- Added `use_case_id` to :class:`CustomModelValidation <datarobot.models.genai.custom_model_validation.CustomModelValidation>`.
+- Added `llm_blueprints_count` and `user_name` to :class:`Playground <datarobot.models.genai.playground.Playground>`.
 - Added `custom_model_embedding_validations` to :class:`SupportedEmbeddings <datarobot._experimental.models.genai.vector_database.SupportedEmbeddings>`.
 - Added `embedding_validation_id` and `is_separator_regex` to :class:`VectorDatabase <datarobot._experimental.models.genai.vector_database.VectorDatabase>`.
 
-- Added optional parameters, `use_case`, `name`, and `model` to :meth:`CustomModelValidation.create <datarobot._experimental.models.genai.custom_model_validation.CustomModelValidation.create>`.
-- Added a method :meth:`CustomModelValidation.list <datarobot._experimental.models.genai.custom_model_validation.CustomModelValidation.list>`, to list custom model validations available to a user with several optional parameters to filter the results.
-- Added a method :meth:`CustomModelValidation.update <datarobot._experimental.models.genai.custom_model_validation.CustomModelValidation.update>`, to update a custom model validation.
+- Added optional parameters, `use_case`, `name`, and `model` to :meth:`CustomModelValidation.create <datarobot.models.genai.custom_model_validation.CustomModelValidation.create>`.
+- Added a method :meth:`CustomModelValidation.list <datarobot.models.genai.custom_model_validation.CustomModelValidation.list>`, to list custom model validations available to a user with several optional parameters to filter the results.
+- Added a method :meth:`CustomModelValidation.update <datarobot.models.genai.custom_model_validation.CustomModelValidation.update>`, to update a custom model validation.
 
-- Added an optional parameter, `use_case`, to :meth:`LLMDefinition.list <datarobot._experimental.models.genai.llm.LLMDefinition.list>`,
+- Added an optional parameter, `use_case`, to :meth:`LLMDefinition.list <datarobot.models.genai.llm.LLMDefinition.list>`,
   to include in the returned LLMs the external LLMs available for the specified `use_case` as well.
 
-- Added optional parameter, `playground` to :meth:`VectorDatabase.list <datarobot._experimental.models.genai.vector_database.VectorDatabase.list>`
+- Added optional parameter, `playground` to :meth:`VectorDatabase.list <datarobot.models.genai.vector_database.VectorDatabase.list>`
   to list vector databases by playground.
 
-- Added optional parameter, `comparison_chat`, to :meth:`ComparisonPrompt.list <datarobot._experimental.models.genai.comparison_prompt.ComparisonPrompt.list>`, to list comparison prompts by comparison chat.
-- Added optional parameter, `comparison_chat`, to :meth:`ComparisonPrompt.create <datarobot._experimental.models.genai.comparison_prompt.ComparisonPrompt.create>`, to specify the comparison chat to create the comparison prompt in.
+- Added optional parameter, `comparison_chat`, to :meth:`ComparisonPrompt.list <datarobot.models.genai.comparison_prompt.ComparisonPrompt.list>`, to list comparison prompts by comparison chat.
+- Added optional parameter, `comparison_chat`, to :meth:`ComparisonPrompt.create <datarobot.models.genai.comparison_prompt.ComparisonPrompt.create>`, to specify the comparison chat to create the comparison prompt in.
 - Added optional parameter, `feedback_result`, to :meth:`ComparisonPrompt.update <datarobot._experimental.models.genai.comparison_prompt.ComparisonPrompt.update>`, to update a comparison prompt with feedback.
 
-- Added optional parameters, `is_starred` to :meth:`LLMBlueprint.update <datarobot._experimental.models.genai.llm_blueprint.LLMBlueprint.update>`
+- Added optional parameters, `is_starred` to :meth:`LLMBlueprint.update <datarobot.models.genai.llm_blueprint.LLMBlueprint.update>`
   to update the LLM Blueprint's starred status.
-- Added optional parameters, `is_starred` to :meth:`LLMBlueprint.list <datarobot._experimental.models.genai.llm_blueprint.LLMBlueprint.list>`
+- Added optional parameters, `is_starred` to :meth:`LLMBlueprint.list <datarobot.models.genai.llm_blueprint.LLMBlueprint.list>`
   to filter the returned LLM blueprints to those matching `is_starred`.
 
-- Added a new enum PromptType, :class:`PromptType <datarobot._experimental.models.enums.PromptType>` to identify the LLMBlueprint's prompting type.
-- Added optional parameters, `prompt_type` to :meth:`LLMBlueprint.create <datarobot._experimental.models.genai.llm_blueprint.LLMBlueprint.create>`,
-  to specify the LLM Blueprint's prompting type. This can be set with :class:`PromptType <datarobot._experimental.models.enums.PromptType>`.
-- Added optional parameters, `prompt_type` to :meth:`LLMBlueprint.update <datarobot._experimental.models.genai.llm_blueprint.LLMBlueprint.update>`,
-  to specify the updated LLM Blueprint's prompting type. This can be set with :class:`PromptType <datarobot._experimental.models.enums.PromptType>`.
-
-- Added a new class, :class:`ComparisonChat <datarobot._experimental.models.genai.comparison_chat.ComparisonChat>`, for interacting with DataRobot generative AI comparison chats.
-  :meth:`ComparisonChat.get <datarobot._experimental.models.genai.comparison_chat.ComparisonChat.get>` retrieves a comparison chat object by ID.
-  :meth:`ComparisonChat.list <datarobot._experimental.models.genai.comparison_chat.ComparisonChat.list>` lists all comparison chats available to the user.
-  :meth:`ComparisonChat.create <datarobot._experimental.models.genai.comparison_chat.ComparisonChat.create>` creates a new comparison chat.
-  :meth:`ComparisonChat.update <datarobot._experimental.models.genai.comparison_chat.ComparisonChat.update>` updates the name of a comparison chat.
-  :meth:`ComparisonChat.delete <datarobot._experimental.models.genai.comparison_chat.ComparisonChat.delete>` deletes a single comparison chat.
+- Added a new enum PromptType, :class:`PromptType <datarobot.enums.PromptType>` to identify the LLMBlueprint's prompting type.
+- Added optional parameters, `prompt_type` to :meth:`LLMBlueprint.create <datarobot.models.genai.llm_blueprint.LLMBlueprint.create>`,
+  to specify the LLM Blueprint's prompting type. This can be set with :class:`PromptType <datarobot.enums.PromptType>`.
+- Added optional parameters, `prompt_type` to :meth:`LLMBlueprint.update <datarobot.models.genai.llm_blueprint.LLMBlueprint.update>`,
+  to specify the updated LLM Blueprint's prompting type. This can be set with :class:`PromptType <datarobot.enums.PromptType>`.
+
+- Added a new class, :class:`ComparisonChat <datarobot.models.genai.comparison_chat.ComparisonChat>`, for interacting with DataRobot generative AI comparison chats.
+  :meth:`ComparisonChat.get <datarobot.models.genai.comparison_chat.ComparisonChat.get>` retrieves a comparison chat object by ID.
+  :meth:`ComparisonChat.list <datarobot.models.genai.comparison_chat.ComparisonChat.list>` lists all comparison chats available to the user.
+  :meth:`ComparisonChat.create <datarobot.models.genai.comparison_chat.ComparisonChat.create>` creates a new comparison chat.
+  :meth:`ComparisonChat.update <datarobot.models.genai.comparison_chat.ComparisonChat.update>` updates the name of a comparison chat.
+  :meth:`ComparisonChat.delete <datarobot.models.genai.comparison_chat.ComparisonChat.delete>` deletes a single comparison chat.
 
-- Added optional parameters, `playground` and `chat` to :meth:`ChatPrompt.list <datarobot._experimental.models.genai.chat_prompt.ChatPrompt.list>`, to list chat prompts by playground and chat.
-- Added optional parameter, `chat` to :meth:`ChatPrompt.create <datarobot._experimental.models.genai.chat_prompt.ChatPrompt.create>`, to specify the chat to create the chat prompt in.
+- Added optional parameters, `playground` and `chat` to :meth:`ChatPrompt.list <datarobot.models.genai.chat_prompt.ChatPrompt.list>`, to list chat prompts by playground and chat.
+- Added optional parameter, `chat` to :meth:`ChatPrompt.create <datarobot.models.genai.chat_prompt.ChatPrompt.create>`, to specify the chat to create the chat prompt in.
 - Added a new method, :meth:`ChatPrompt.update <datarobot._experimental.models.genai.chat_prompt.ChatPrompt.update>`, to update a chat prompt with custom metrics and feedback.
 
-- Added a new class, :class:`Chat <datarobot._experimental.models.genai.chat.Chat>`, for interacting with DataRobot generative AI chats.
-  :meth:`Chat.get <datarobot._experimental.models.genai.chat.Chat.get>` retrieves a chat object by ID.
-  :meth:`Chat.list <datarobot._experimental.models.genai.chat.Chat.list>` lists all chats available to the user.
-  :meth:`Chat.create <datarobot._experimental.models.genai.chat.Chat.create>` creates a new chat.
-  :meth:`Chat.update <datarobot._experimental.models.genai.chat.Chat.update>` updates the name of a chat.
-  :meth:`Chat.delete <datarobot._experimental.models.genai.chat.Chat.delete>` deletes a single chat.
+- Added a new class, :class:`Chat <datarobot.models.genai.chat.Chat>`, for interacting with DataRobot generative AI chats.
+  :meth:`Chat.get <datarobot.models.genai.chat.Chat.get>` retrieves a chat object by ID.
+  :meth:`Chat.list <datarobot.models.genai.chat.Chat.list>` lists all chats available to the user.
+  :meth:`Chat.create <datarobot.models.genai.chat.Chat.create>` creates a new chat.
+  :meth:`Chat.update <datarobot.models.genai.chat.Chat.update>` updates the name of a chat.
+  :meth:`Chat.delete <datarobot.models.genai.chat.Chat.delete>` deletes a single chat.
 
 - Removed the `model_package` module. Use :class:`RegisteredModelVersion <datarobot.models.RegisteredModelVersion>` instead.
-- Added new class :class:`UserLimits <datarobot._experimental.models.genai.user_limits.UserLimits>`
-    - Added support to get the count of users' LLM API requests. :meth:`UserLimits.get_llm_requests_count <datarobot._experimental.models.genai.user_limits.UserLimits.get_llm_requests_count>`
-    - Added support to get the count of users' vector databases. :meth:`UserLimits.get_vector_database_count <datarobot._experimental.models.genai.user_limits.UserLimits.get_vector_database_count>`
+- Added new class :class:`UserLimits <datarobot.models.genai.user_limits.UserLimits>`
+  - Added support to get the count of users' LLM API requests. :meth:`UserLimits.get_llm_requests_count <datarobot.models.genai.user_limits.UserLimits.get_llm_requests_count>`
+  - Added support to get the count of users' vector databases. :meth:`UserLimits.get_vector_database_count <datarobot.models.genai.user_limits.UserLimits.get_vector_database_count>`
 - Added new methods to the class :class:`Notebook <datarobot._experimental.models.notebooks.Notebook>` which includes :meth:`Notebook.run <datarobot._experimental.models.notebooks.Notebook.run>` and :meth:`Notebook.download_revision <datarobot._experimental.models.notebooks.Notebook.download_revision>`. See the documentation for example usage.
 - Added new class :class:`NotebookScheduledJob <datarobot._experimental.models.notebooks.NotebookScheduledJob>`.
 - Added new class :class:`NotebookScheduledRun <datarobot._experimental.models.notebooks.NotebookScheduledRun>`.
 - Added a new method :meth:`Model.get_incremental_learning_metadata <datarobot._experimental.models.model.Model.get_incremental_learning_metadata>` that retrieves incremental learning metadata for a model.
 - Added a new method :meth:`Model.start_incremental_learning <datarobot._experimental.models.model.Model.start_incremental_learning>` that starts incremental learning for a model.
+- Updated the API endpoint prefix for all GenerativeAI routes to align with the publicly documented routes.
 
 Bugfixes
 ********
 - Fixed how async url is build in :meth:`Model.get_or_request_feature_impact <datarobot.models.Model.get_or_request_feature_impact>`
 - Fixed setting ssl_verify by env variables.
 - Resolved a problem related to tilde-based paths in the Client's 'config_path' attribute.
 - Changed the force_size default of :class:`ImageOptions <datarobot.helpers.image_utils.ImageOptions>` to apply the same transformations by default, which are applied when image archive datasets are uploaded to DataRobot.
@@ -301,75 +389,75 @@
 Deprecation summary
 *******************
 - :meth:`Project.refresh <datarobot.models.Project.refresh>` will no longer set ``Project.advanced_options`` to a dictionary after version 3.5 is released.
    All interactions with ``Project.advanced_options`` should be expected to be through the :class:`AdvancedOptions <datarobot.helpers.AdvancedOptions>` class.
 
 Experimental changes
 ********************
-- Added a new class, :class:`VectorDatabase <datarobot._experimental.models.genai.vector_database.VectorDatabase>`, for interacting with DataRobot vector databases.
-  :meth:`VectorDatabase.get <datarobot._experimental.models.genai.vector_database.VectorDatabase.get>` retrieves a VectorDatabase object by ID.
-  :meth:`VectorDatabase.list <datarobot._experimental.models.genai.vector_database.VectorDatabase.list>` lists all VectorDatabases available to the user.
-  :meth:`VectorDatabase.create <datarobot._experimental.models.genai.vector_database.VectorDatabase.create>` creates a new VectorDatabase.
-  :meth:`VectorDatabase.create <datarobot._experimental.models.genai.vector_database.VectorDatabase.create_from_custom_model>` allows you to use a validated deployment of a custom model as your own Vector Database.
-  :meth:`VectorDatabase.update <datarobot._experimental.models.genai.vector_database.VectorDatabase.update>` updates the name of a VectorDatabase.
-  :meth:`VectorDatabase.delete <datarobot._experimental.models.genai.vector_database.VectorDatabase.delete>` deletes a single VectorDatabase.
-  :meth:`VectorDatabase.get_supported_embeddings <datarobot._experimental.models.genai.vector_database.VectorDatabase.get_supported_embeddings>` retrieves all supported embedding models.
-  :meth:`VectorDatabase.get_supported_text_chunkings <datarobot._experimental.models.genai.vector_database.VectorDatabase.get_supported_text_chunkings>` retrieves all supported text chunking configurations.
-  :meth:`VectorDatabase.download_text_and_embeddings_asset <datarobot._experimental.models.genai.vector_database.VectorDatabase.download_text_and_embeddings_asset>` download a parquet file with internal vector database data.
-
-- Added a new class, :class:`CustomModelVectorDatabaseValidation <datarobot._experimental.models.genai.vector_database.CustomModelVectorDatabaseValidation>`, for validating custom model deployments for use as a vector database.
-  :meth:`CustomModelVectorDatabaseValidation.get <datarobot._experimental.models.genai.custom_model_validation.CustomModelValidation.get>` retrieves a CustomModelVectorDatabaseValidation object by ID.
-  :meth:`CustomModelVectorDatabaseValidation.get_by_values <datarobot._experimental.models.genai.custom_model_validation.CustomModelValidation.get_by_values>` retrieves a CustomModelVectorDatabaseValidation object by field values.
-  :meth:`CustomModelVectorDatabaseValidation.create <datarobot._experimental.models.genai.custom_model_validation.CustomModelValidation.create>` starts validation of the deployment.
-  :meth:`CustomModelVectorDatabaseValidation.revalidate <datarobot._experimental.models.genai.custom_model_validation.CustomModelValidation.revalidate>` repairs an unlinked external vector database.
-
-- Added a new class, :class:`Playground <datarobot._experimental.models.genai.playground.Playground>`, for interacting with DataRobot generative AI playgrounds.
-  :meth:`Playground.get <datarobot._experimental.models.genai.playground.Playground.get>` retrieves a playground object by ID.
-  :meth:`Playground.list <datarobot._experimental.models.genai.playground.Playground.list>` lists all playgrounds available to the user.
-  :meth:`Playground.create <datarobot._experimental.models.genai.playground.Playground.create>` creates a new playground.
-  :meth:`Playground.update <datarobot._experimental.models.genai.playground.Playground.update>` updates the name and description of a playground.
-  :meth:`Playground.delete <datarobot._experimental.models.genai.playground.Playground.delete>` deletes a single playground.
-
-- Added a new class, :class:`LLMDefinition <datarobot._experimental.models.genai.llm.LLMDefinition>`, for interacting with DataRobot generative AI LLMs.
-  :meth:`LLMDefinition.list <datarobot._experimental.models.genai.llm.LLMDefinition.list>` lists all LLMs available to the user.
-
-- Added a new class, :class:`LLMBlueprint <datarobot._experimental.models.genai.llm_blueprint.LLMBlueprint>`, for interacting with DataRobot generative AI LLM blueprints.
-  :meth:`LLMBlueprint.get <datarobot._experimental.models.genai.llm_blueprint.LLMBlueprint.get>` retrieves an LLM blueprint object by ID.
-  :meth:`LLMBlueprint.list <datarobot._experimental.models.genai.llm_blueprint.LLMBlueprint.list>` lists all LLM blueprints available to the user.
-  :meth:`LLMBlueprint.create <datarobot._experimental.models.genai.llm_blueprint.LLMBlueprint.create>` creates a new LLM blueprint.
-  :meth:`LLMBlueprint.create_from_llm_blueprint <datarobot._experimental.models.genai.llm_blueprint.LLMBlueprint.create_from_llm_blueprint>` creates a new LLM blueprint from an existing one.
-  :meth:`LLMBlueprint.update <datarobot._experimental.models.genai.llm_blueprint.LLMBlueprint.update>` updates an LLM blueprint.
-  :meth:`LLMBlueprint.delete <datarobot._experimental.models.genai.llm_blueprint.LLMBlueprint.delete>` deletes a single LLM blueprint.
-
-- Added a new class, :class:`ChatPrompt <datarobot._experimental.models.genai.chat_prompt.ChatPrompt>`, for interacting with DataRobot generative AI chat prompts.
-  :meth:`ChatPrompt.get <datarobot._experimental.models.genai.chat_prompt.ChatPrompt.get>` retrieves a chat prompt object by ID.
-  :meth:`ChatPrompt.list <datarobot._experimental.models.genai.chat_prompt.ChatPrompt.list>` lists all chat prompts available to the user.
-  :meth:`ChatPrompt.create <datarobot._experimental.models.genai.chat_prompt.ChatPrompt.create>` creates a new chat prompt.
-  :meth:`ChatPrompt.delete <datarobot._experimental.models.genai.chat_prompt.ChatPrompt.delete>` deletes a single chat prompt.
-
-- Added a new class, :class:`CustomModelLLMValidation <datarobot._experimental.models.genai.custom_model_llm_validation.CustomModelLLMValidation>`, for validating custom model deployments for use as a custom model LLM.
-  :meth:`CustomModelLLMValidation.get <datarobot._experimental.models.genai.custom_model_validation.CustomModelValidation.get>` retrieves a CustomModelLLMValidation object by ID.
-  :meth:`CustomModelLLMValidation.get_by_values <datarobot._experimental.models.genai.custom_model_validation.CustomModelValidation.get_by_values>` retrieves a CustomModelLLMValidation object by field values.
-  :meth:`CustomModelLLMValidation.create <datarobot._experimental.models.genai.custom_model_validation.CustomModelValidation.create>` starts validation of the deployment.
-  :meth:`CustomModelLLMValidation.revalidate <datarobot._experimental.models.genai.custom_model_validation.CustomModelValidation.revalidate>` repairs an unlinked external custom model LLM.
-
-- Added a new class, :class:`ComparisonPrompt <datarobot._experimental.models.genai.comparison_prompt.ComparisonPrompt>`, for interacting with DataRobot generative AI comparison prompts.
-  :meth:`ComparisonPrompt.get <datarobot._experimental.models.genai.comparison_prompt.ComparisonPrompt.get>` retrieves a comparison prompt object by ID.
-  :meth:`ComparisonPrompt.list <datarobot._experimental.models.genai.comparison_prompt.ComparisonPrompt.list>` lists all comparison prompts available to the user.
-  :meth:`ComparisonPrompt.create <datarobot._experimental.models.genai.comparison_prompt.ComparisonPrompt.create>` creates a new comparison prompt.
-  :meth:`ComparisonPrompt.update <datarobot._experimental.models.genai.comparison_prompt.ComparisonPrompt.update>` updates a comparison prompt.
-  :meth:`ComparisonPrompt.delete <datarobot._experimental.models.genai.comparison_prompt.ComparisonPrompt.delete>` deletes a single comparison prompt.
+- Added a new class, :class:`VectorDatabase <datarobot.models.genai.vector_database.VectorDatabase>`, for interacting with DataRobot vector databases.
+  :meth:`VectorDatabase.get <datarobot.models.genai.vector_database.VectorDatabase.get>` retrieves a VectorDatabase object by ID.
+  :meth:`VectorDatabase.list <datarobot.models.genai.vector_database.VectorDatabase.list>` lists all VectorDatabases available to the user.
+  :meth:`VectorDatabase.create <datarobot.models.genai.vector_database.VectorDatabase.create>` creates a new VectorDatabase.
+  :meth:`VectorDatabase.create <datarobot.models.genai.vector_database.VectorDatabase.create_from_custom_model>` allows you to use a validated deployment of a custom model as your own Vector Database.
+  :meth:`VectorDatabase.update <datarobot.models.genai.vector_database.VectorDatabase.update>` updates the name of a VectorDatabase.
+  :meth:`VectorDatabase.delete <datarobot.models.genai.vector_database.VectorDatabase.delete>` deletes a single VectorDatabase.
+  :meth:`VectorDatabase.get_supported_embeddings <datarobot.models.genai.vector_database.VectorDatabase.get_supported_embeddings>` retrieves all supported embedding models.
+  :meth:`VectorDatabase.get_supported_text_chunkings <datarobot.models.genai.vector_database.VectorDatabase.get_supported_text_chunkings>` retrieves all supported text chunking configurations.
+  :meth:`VectorDatabase.download_text_and_embeddings_asset <datarobot.models.genai.vector_database.VectorDatabase.download_text_and_embeddings_asset>` download a parquet file with internal vector database data.
+
+- Added a new class, :class:`CustomModelVectorDatabaseValidation <datarobot.models.genai.vector_database.CustomModelVectorDatabaseValidation>`, for validating custom model deployments for use as a vector database.
+  :meth:`CustomModelVectorDatabaseValidation.get <datarobot.models.genai.custom_model_validation.CustomModelValidation.get>` retrieves a CustomModelVectorDatabaseValidation object by ID.
+  :meth:`CustomModelVectorDatabaseValidation.get_by_values <datarobot.models.genai.custom_model_validation.CustomModelValidation.get_by_values>` retrieves a CustomModelVectorDatabaseValidation object by field values.
+  :meth:`CustomModelVectorDatabaseValidation.create <datarobot.models.genai.custom_model_validation.CustomModelValidation.create>` starts validation of the deployment.
+  :meth:`CustomModelVectorDatabaseValidation.revalidate <datarobot.models.genai.custom_model_validation.CustomModelValidation.revalidate>` repairs an unlinked external vector database.
+
+- Added a new class, :class:`Playground <datarobot.models.genai.playground.Playground>`, for interacting with DataRobot generative AI playgrounds.
+  :meth:`Playground.get <datarobot.models.genai.playground.Playground.get>` retrieves a playground object by ID.
+  :meth:`Playground.list <datarobot.models.genai.playground.Playground.list>` lists all playgrounds available to the user.
+  :meth:`Playground.create <datarobot.models.genai.playground.Playground.create>` creates a new playground.
+  :meth:`Playground.update <datarobot.models.genai.playground.Playground.update>` updates the name and description of a playground.
+  :meth:`Playground.delete <datarobot.models.genai.playground.Playground.delete>` deletes a single playground.
+
+- Added a new class, :class:`LLMDefinition <datarobot.models.genai.llm.LLMDefinition>`, for interacting with DataRobot generative AI LLMs.
+  :meth:`LLMDefinition.list <datarobot.models.genai.llm.LLMDefinition.list>` lists all LLMs available to the user.
+
+- Added a new class, :class:`LLMBlueprint <datarobot.models.genai.llm_blueprint.LLMBlueprint>`, for interacting with DataRobot generative AI LLM blueprints.
+  :meth:`LLMBlueprint.get <datarobot.models.genai.llm_blueprint.LLMBlueprint.get>` retrieves an LLM blueprint object by ID.
+  :meth:`LLMBlueprint.list <datarobot.models.genai.llm_blueprint.LLMBlueprint.list>` lists all LLM blueprints available to the user.
+  :meth:`LLMBlueprint.create <datarobot.models.genai.llm_blueprint.LLMBlueprint.create>` creates a new LLM blueprint.
+  :meth:`LLMBlueprint.create_from_llm_blueprint <datarobot.models.genai.llm_blueprint.LLMBlueprint.create_from_llm_blueprint>` creates a new LLM blueprint from an existing one.
+  :meth:`LLMBlueprint.update <datarobot.models.genai.llm_blueprint.LLMBlueprint.update>` updates an LLM blueprint.
+  :meth:`LLMBlueprint.delete <datarobot.models.genai.llm_blueprint.LLMBlueprint.delete>` deletes a single LLM blueprint.
+
+- Added a new class, :class:`ChatPrompt <datarobot.models.genai.chat_prompt.ChatPrompt>`, for interacting with DataRobot generative AI chat prompts.
+  :meth:`ChatPrompt.get <datarobot.models.genai.chat_prompt.ChatPrompt.get>` retrieves a chat prompt object by ID.
+  :meth:`ChatPrompt.list <datarobot.models.genai.chat_prompt.ChatPrompt.list>` lists all chat prompts available to the user.
+  :meth:`ChatPrompt.create <datarobot.models.genai.chat_prompt.ChatPrompt.create>` creates a new chat prompt.
+  :meth:`ChatPrompt.delete <datarobot.models.genai.chat_prompt.ChatPrompt.delete>` deletes a single chat prompt.
+
+- Added a new class, :class:`CustomModelLLMValidation <datarobot.models.genai.custom_model_llm_validation.CustomModelLLMValidation>`, for validating custom model deployments for use as a custom model LLM.
+  :meth:`CustomModelLLMValidation.get <datarobot.models.genai.custom_model_validation.CustomModelValidation.get>` retrieves a CustomModelLLMValidation object by ID.
+  :meth:`CustomModelLLMValidation.get_by_values <datarobot.models.genai.custom_model_validation.CustomModelValidation.get_by_values>` retrieves a CustomModelLLMValidation object by field values.
+  :meth:`CustomModelLLMValidation.create <datarobot.models.genai.custom_model_validation.CustomModelValidation.create>` starts validation of the deployment.
+  :meth:`CustomModelLLMValidation.revalidate <datarobot.models.genai.custom_model_validation.CustomModelValidation.revalidate>` repairs an unlinked external custom model LLM.
+
+- Added a new class, :class:`ComparisonPrompt <datarobot.models.genai.comparison_prompt.ComparisonPrompt>`, for interacting with DataRobot generative AI comparison prompts.
+  :meth:`ComparisonPrompt.get <datarobot.models.genai.comparison_prompt.ComparisonPrompt.get>` retrieves a comparison prompt object by ID.
+  :meth:`ComparisonPrompt.list <datarobot.models.genai.comparison_prompt.ComparisonPrompt.list>` lists all comparison prompts available to the user.
+  :meth:`ComparisonPrompt.create <datarobot.models.genai.comparison_prompt.ComparisonPrompt.create>` creates a new comparison prompt.
+  :meth:`ComparisonPrompt.update <datarobot.models.genai.comparison_prompt.ComparisonPrompt.update>` updates a comparison prompt.
+  :meth:`ComparisonPrompt.delete <datarobot.models.genai.comparison_prompt.ComparisonPrompt.delete>` deletes a single comparison prompt.
 
 - Extended :class:`UseCase <datarobot.UseCase>`, adding two new fields to represent the count of vector databases and playgrounds.
 
-- Added a new method, :meth:`ChatPrompt.create_llm_blueprint <datarobot._experimental.models.genai.chat_prompt.ChatPrompt.create_llm_blueprint>`, to create an LLM blueprint from a chat prompt.
+- Added a new method, :meth:`ChatPrompt.create_llm_blueprint <datarobot.models.genai.chat_prompt.ChatPrompt.create_llm_blueprint>`, to create an LLM blueprint from a chat prompt.
 
-- Added a new method, :meth:`CustomModelLLMValidation.delete <datarobot._experimental.models.genai.custom_model_validation.CustomModelValidation.delete>`, to delete a custom model LLM validation record.
+- Added a new method, :meth:`CustomModelLLMValidation.delete <datarobot.models.genai.custom_model_validation.CustomModelValidation.delete>`, to delete a custom model LLM validation record.
 
-- Added a new method, :meth:`LLMBlueprint.register_custom_model <datarobot._experimental.models.genai.llm_blueprint.LLMBlueprint.register_custom_model>`, for registering a custom model from a generative AI LLM blueprint.
+- Added a new method, :meth:`LLMBlueprint.register_custom_model <datarobot.models.genai.llm_blueprint.LLMBlueprint.register_custom_model>`, for registering a custom model from a generative AI LLM blueprint.
 
 3.2.0
 =====
 
 New features
 ************
 - Added new methods to trigger batch monitoring jobs without providing a job definition.
@@ -2060,15 +2148,15 @@
   If multiseries id columns are not provided, calendar is considered to be single series and all events are applied to all series.
 - We have expanded prediction intervals availability to the following use-cases:
 
     - Time series model deployments now support prediction intervals. See
       :meth:`Deployment.get_prediction_intervals_settings<datarobot.models.Deployment.get_prediction_intervals_settings>`
       and :meth:`Deployment.update_prediction_intervals_settings<datarobot.models.Deployment.update_prediction_intervals_settings>` for usage.
     - Prediction intervals are now supported for model exports for time series. To that end, a new optional parameter
-      ``prediction_intervals_size`` has been added to :meth:`Model.request_transferable_export <datarobot.models.Model.request_transferable_export>`.
+      ``prediction_intervals_size`` has been added to `Model.request_transferable_export <datarobot.models.Model.request_transferable_export>`.
 
   More details on prediction intervals can be found in the :ref:`prediction intervals documentation <prediction_intervals>`.
 - Allowed pairwise interaction groups can now be specified in :py:class:`AdvancedOptions <datarobot.helpers.AdvancedOptions>`.
   They will be used in GAM models during training.
 - New deployments features:
 
     - Update the label and description of a deployment using :meth:`Deployment.update<datarobot.models.Deployment.update>`.
```

### Comparing `datarobot_early_access-3.4.0.2024.4.8/LICENSE.txt` & `datarobot_early_access-3.5.0.2024.5.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/PKG-INFO` & `datarobot_early_access-3.5.0.2024.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarobot_early_access
-Version: 3.4.0.2024.4.8
+Version: 3.5.0.2024.5.6
 Summary: This client library is designed to support the DataRobot API.
 Home-page: https://datarobot.com
 Author: datarobot
 Author-email: support@datarobot.com
 Maintainer: datarobot
 Maintainer-email: info@datarobot.com
 License: DataRobot Tool and Utility Agreement
```

### Comparing `datarobot_early_access-3.4.0.2024.4.8/README.md` & `datarobot_early_access-3.5.0.2024.5.6/README.md`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/common_setup.py` & `datarobot_early_access-3.5.0.2024.5.6/common_setup.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/__init__.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     FeatureAssociationMatrix,
     FeatureAssociationMatrixDetails,
     FeatureHistogram,
     FeatureImpactJob,
     FeatureLineage,
     Featurelist,
     FrozenModel,
-    ImportedModel,
+    genai,
     InteractionFeature,
     Job,
     KeyValue,
     Model,
     ModelBlueprintChart,
     ModelingFeature,
     ModelingFeaturelist,
```

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/_compat.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_compat.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/__init__.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/chunking_service.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/chunking_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,14 +193,16 @@
          The size of the dataset.
      estimated_size_per_row : str
          The estimated size per row.
      columns : str
          The list of column names in the dataset.
      order_by_columns : List[str]
          A list of columns used to sort the dataset.
+     is_descending_order : bool
+         Orders the direction of the data. Defaults to False, ordering from smallest to largest.
      select_columns : List[str]
          A list of columns to select from the dataset.
 
     """
 
     _converter = t.Dict(
         {
@@ -216,23 +218,25 @@
             t.Key("total_rows", optional=True): t.Or(t.Int, t.Null),
             t.Key("source_size", optional=True): t.Or(t.Int, t.Null),
             t.Key("estimated_size_per_row", optional=True): t.Or(t.Int, t.Null),
             t.Key("columns", optional=True): t.Or(t.List(t.String), t.Null),
             t.Key("catalog_id", optional=True): t.Or(t.String, t.Null),
             t.Key("catalog_version_id", optional=True): t.Or(t.String, t.Null),
             t.Key("order_by_columns"): t.List(t.String, min_length=0),
+            t.Key("is_descending_order", optional=True): t.Bool,
             t.Key("select_columns", optional=True): t.Or(t.List(t.String), t.Null),
         }
     ).allow_extra("*")
 
     def __init__(
         self,
         id: str,
         storage_origin: OriginStorageType,
         order_by_columns: Optional[List[str]] = None,
+        is_descending_order: Optional[bool] = False,
         table: Optional[str] = None,
         data_store_id: Optional[str] = None,
         credentials_id: Optional[str] = None,
         schema: Optional[str] = None,
         catalog: Optional[str] = None,
         name: Optional[str] = None,
         data_source_id: Optional[str] = None,
@@ -256,14 +260,15 @@
         self.total_rows = total_rows
         self.source_size = source_size
         self.estimated_size_per_row = estimated_size_per_row
         self.columns = columns
         self.catalog_id = catalog_id
         self.catalog_version_id = catalog_version_id
         self.order_by_columns = [] if order_by_columns is None else order_by_columns
+        self.is_descending_order = is_descending_order
         self.select_columns = select_columns
 
 
 class DatasourceDataWarehouseInfo(APIObject):
     """
     Data source information used at creation time with dataset chunk definition.
     Data warehouses supported: Snowflake, BigQuery, Databricks
@@ -285,24 +290,27 @@
         The offset into the dataset to create the chunk.
     catalog : str
         The database or catalog name.
     data_source_id : str
         The ID of the data request used to generate sampling and metadata.
     order_by_columns : List[str]
         A list of columns used to sort the dataset.
+    is_descending_order : bool
+        Orders the direction of the data. Defaults to False, ordering from smallest to largest.
     select_columns: List[str]
         A list of columns to select from the dataset.
     """
 
     _converter = t.Dict(
         {
             t.Key("data_store_id"): t.String,
             t.Key("credentials_id"): t.String,
             t.Key("table"): t.String,
             t.Key("order_by_columns"): t.List(t.String),
+            t.Key("is_descending_order", optional=True): t.Bool,
             t.Key("storage_origin"): t.Enum(
                 OriginStorageType.SNOWFLAKE,
                 OriginStorageType.BIGQUERY,
                 OriginStorageType.AI_CATALOG,
                 OriginStorageType.DATABRICKS,
             ),
             t.Key("schema", optional=True): t.Or(t.String, t.Null),
@@ -316,14 +324,15 @@
     def __init__(
         self,
         data_store_id: str,
         credentials_id: str,
         table: str,
         storage_origin: OriginStorageType,
         order_by_columns: List[str],
+        is_descending_order: bool = False,
         schema: Optional[str] = None,
         catalog: Optional[str] = None,
         name: Optional[str] = None,
         data_source_id: Optional[str] = None,
         select_columns: Optional[List[str]] = None,
     ):
         self.name = name
@@ -331,14 +340,15 @@
         self.credentials_id = credentials_id
         self.table = table
         self.schema = schema
         self.catalog = catalog
         self.storage_origin = storage_origin
         self.data_source_id = data_source_id
         self.order_by_columns = order_by_columns
+        self.is_descending_order = is_descending_order
         self.select_columns = select_columns
         self._converter.check(self.to_dict())
 
     def to_dict(self) -> Dict[str, Any]:
         self_dict = {
             attr[0]: attr[1]
             for attr in inspect.getmembers(self)
@@ -362,45 +372,50 @@
         The origin data source, always AI Catalog type.
     catalog_id : str
         The ID of the AI Catalog dataset.
     catalog_version_id : str
         The ID of the AI Catalog dataset version.
     order_by_columns : List[str]
         A list of columns used to sort the dataset.
+    is_descending_order : bool
+        Orders the direction of the data. Defaults to False, ordering from smallest to largest.
     select_columns: List[str]
         A list of columns to select from the dataset.
     """
 
     _converter = t.Dict(
         {
             t.Key("catalog_version_id"): t.String,
             t.Key("catalog_id", optional=True): t.Or(t.String, t.Null),
             t.Key("storage_origin"): t.Atom(OriginStorageType.AI_CATALOG),
             t.Key("table", optional=True): t.Or(t.String, t.Null),
             t.Key("name", optional=True): t.Or(t.String, t.Null),
             t.Key("order_by_columns", optional=True): t.List(t.String, min_length=0),
+            t.Key("is_descending_order", optional=True): t.Bool,
             t.Key("select_columns", optional=True): t.Or(t.List(t.String), t.Null),
         }
     )
 
     def __init__(
         self,
         catalog_version_id: str,
         catalog_id: Optional[str] = None,
         table: Optional[str] = None,
         name: Optional[str] = None,
         order_by_columns: Optional[List[str]] = None,
+        is_descending_order: Optional[bool] = False,
         select_columns: Optional[List[str]] = None,
     ):
         self.name = name
         self.catalog_version_id = catalog_version_id
         self.catalog_id = catalog_id
         self.table = table
         self.storage_origin = OriginStorageType.AI_CATALOG
         self.order_by_columns = [] if order_by_columns is None else order_by_columns
+        self.is_descending_order = is_descending_order
         self.select_columns = select_columns
         self._converter.check(self.to_dict())
 
     def to_dict(self) -> Dict[str, Any]:
         self_dict = {
             attr[0]: attr[1]
             for attr in inspect.getmembers(self)
```

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/data_matching.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/data_matching.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/dataset.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/chat.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # Released under the terms of DataRobot Tool and Utility Agreement.
 from __future__ import annotations
 
 from typing import List, Optional, Union
 
 import trafaret as t
 
-from datarobot._experimental.models.genai.llm_blueprint import LLMBlueprint
 from datarobot.models.api_object import APIObject
+from datarobot.models.genai.llm_blueprint import LLMBlueprint
 from datarobot.utils.pagination import unpaginate
 
 
 def get_entity_id(entity: Union[Chat, LLMBlueprint, str]) -> str:
     """
     Get the entity ID from the entity parameter.
 
@@ -65,15 +65,15 @@
         Checks whether the chat is frozen. Prompts cannot be submitted to frozen chats.
     creation_date : str
         The date when the chat was created.
     creation_user_id : str
         The ID of the creating user.
     """
 
-    _path = "api-gw/genai/chats"
+    _path = "api/v2/genai/chats"
 
     _converter = chat_trafaret
 
     def __init__(
         self,
         id: str,
         name: str,
```

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/chat_prompt.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/chat_prompt.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,29 +9,26 @@
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
 from __future__ import annotations
 
 from typing import Any, Dict, List, Optional, Union
 
-from mypy_extensions import TypedDict
 import trafaret as t
 
-from datarobot._experimental.models.enums import FeedbackSentiment
-from datarobot._experimental.models.genai.chat import Chat
-from datarobot._experimental.models.genai.llm import LLMDefinition
-from datarobot._experimental.models.genai.llm_blueprint import (
+from datarobot.models.api_object import APIObject
+from datarobot.models.genai.chat import Chat
+from datarobot.models.genai.llm import LLMDefinition
+from datarobot.models.genai.llm_blueprint import (
     LLMBlueprint,
     vector_database_settings_trafaret,
     VectorDatabaseSettings,
 )
-from datarobot._experimental.models.genai.playground import Playground
-from datarobot._experimental.models.genai.vector_database import VectorDatabase
-from datarobot.enums import enum_to_list
-from datarobot.models.api_object import APIObject
+from datarobot.models.genai.playground import Playground
+from datarobot.models.genai.vector_database import VectorDatabase
 from datarobot.utils.pagination import unpaginate
 from datarobot.utils.waiters import wait_for_async_resolution
 
 
 def get_entity_id(
     entity: Union[Playground, Chat, ChatPrompt, LLMBlueprint, LLMDefinition, VectorDatabase, str]
 ) -> str:
@@ -50,68 +47,23 @@
     """
     if isinstance(entity, str):
         return entity
 
     return entity.id
 
 
-class FeedbackMetadataDict(TypedDict):
-    feedback: FeedbackSentiment
-
-
-class MetricMetadataDict(TypedDict):
-    name: str
-    value: Any
-    formatted_value: Optional[str]
-    sidecar_model_metric_validation_id: Optional[str]
-    custom_model_id: Optional[str]
-    evaluation_dataset_configuration_id: Optional[str]
-    cost_configuration_id: Optional[str]
-
-
-feedback_metadata_trafaret = t.Dict(
-    {t.Key("feedback"): t.Enum(*enum_to_list(FeedbackSentiment))}
-).ignore_extra("*")
-
-
-metric_metadata_trafaret = t.Dict(
-    {
-        t.Key("name"): t.String,
-        t.Key("value"): t.Any,
-        t.Key("formatted_value", optional=True): t.Or(t.String, t.Null),
-        t.Key("sidecar_model_metric_validation_id", optional=True): t.Or(t.String, t.Null),
-        t.Key("custom_model_id", optional=True): t.Or(t.String, t.Null),
-        t.Key("evaluation_dataset_configuration_id", optional=True): t.Or(t.String, t.Null),
-        t.Key("cost_configuration_id", optional=True): t.Or(t.String, t.Null),
-    }
-).ignore_extra("*")
-
-
-feedback_result_trafaret = t.Dict(
-    {
-        t.Key("positive_user_ids"): t.List(t.String),
-        t.Key("negative_user_ids"): t.List(t.String),
-    }
-)
-
-
 result_metadata_trafaret = t.Dict(
     {
         t.Key("cost", optional=True): t.Or(t.Float, t.Null),
         t.Key("output_token_count"): t.Int,
         t.Key("input_token_count"): t.Int,
         t.Key("total_token_count"): t.Int,
         t.Key("estimated_docs_token_count"): t.Int,
         t.Key("latency_milliseconds"): t.Int,
         t.Key("error_message", optional=True): t.Or(t.String, t.Null),
-        t.Key("feedback_result"): feedback_result_trafaret,
-        t.Key("metrics"): t.List(metric_metadata_trafaret),
-        t.Key("final_prompt"): t.Or(
-            t.String, t.Dict().allow_extra("*"), t.List(t.Dict().allow_extra("*")), t.Null
-        ),
     }
 ).ignore_extra("*")
 
 
 confidence_scores_trafaret = t.Dict(
     {
         t.Key("rouge"): t.Float,
@@ -150,119 +102,14 @@
         t.Key("chat_id", optional=True): t.Or(t.String, t.Null),
         t.Key("chat_context_id", optional=True): t.Or(t.String, t.Null),
         t.Key("chat_prompt_ids_included_in_history", optional=True): t.Or(t.List(t.String), t.Null),
     }
 ).ignore_extra("*")
 
 
-class FeedbackMetadata(APIObject):
-    """
-    Metadata for feedback associated with a chat prompt.
-
-    Attributes
-    ----------
-    feedback : FeedbackSentiment
-        The sentiment of the feedback.
-    """
-
-    _converter = feedback_metadata_trafaret
-
-    def __init__(self, feedback: FeedbackSentiment):
-        self.feedback = feedback
-
-    def __repr__(self) -> str:
-        return f"{self.__class__.__name__}(feedback={self.feedback})"
-
-    def to_dict(self) -> FeedbackMetadataDict:
-        return {"feedback": self.feedback}
-
-
-class FeedbackResult(APIObject):
-    """
-    Feedback associated with a chat prompt.
-
-    Attributes
-    ----------
-    positive_user_ids : List[str]
-        The IDs of the users providing positive feedback.
-    negative_user_ids : List[str]
-        The IDs of the users providing negative feedback.
-    """
-
-    _converter = feedback_result_trafaret
-
-    def __init__(self, positive_user_ids: List[str], negative_user_ids: List[str]):
-        self.positive_user_ids = positive_user_ids
-        self.negative_user_ids = negative_user_ids
-
-    def __repr__(self) -> str:
-        return f"{self.__class__.__name__}"
-
-
-class MetricMetadata(APIObject):
-    """
-    Metadata for the custom metrics associated with a chat prompt.
-
-    Attributes
-    ----------
-    name : str
-        The name of the metric.
-    value : Any
-        The value of the metric.
-    formatted_value : Optional[str], optional
-        The formatted value of the metric, if any.
-    sidecar_model_metric_validation_id : Optional[str], optional
-        The ID of the sidecar model implementing the metric, if any.
-    custom_model_id : Optional[str], optional
-        The ID of the custom model implementing the metric, if any.
-    evaluation_dataset_configuration_id : Optional[str], optional
-        The ID of the evaluation dataset configuration associated with the metric, if any.
-    cost_configuration_id : Optional[str], optional
-        The ID of the cost configuration associated with the metric, if any.
-    """
-
-    _converter = metric_metadata_trafaret
-
-    def __init__(
-        self,
-        name: str,
-        value: Any,
-        formatted_value: Optional[str] = None,
-        sidecar_model_metric_validation_id: Optional[str] = None,
-        custom_model_id: Optional[str] = None,
-        evaluation_dataset_configuration_id: Optional[str] = None,
-        cost_configuration_id: Optional[str] = None,
-    ):
-        self.name = name
-        self.value = value
-        self.formatted_value = formatted_value
-        self.sidecar_model_metric_validation_id = sidecar_model_metric_validation_id
-        self.custom_model_id = custom_model_id
-        self.evaluation_dataset_configuration_id = evaluation_dataset_configuration_id
-        self.cost_configuration_id = cost_configuration_id
-
-    def __repr__(self) -> str:
-        return (
-            f"{self.__class__.__name__}(name={self.name}, "
-            f"value={self.value}, "
-            f"formatted_value={self.formatted_value})"
-        )
-
-    def to_dict(self) -> MetricMetadataDict:
-        return {
-            "name": self.name,
-            "value": self.value,
-            "formatted_value": self.formatted_value,
-            "sidecar_model_metric_validation_id": self.sidecar_model_metric_validation_id,
-            "custom_model_id": self.custom_model_id,
-            "evaluation_dataset_configuration_id": self.evaluation_dataset_configuration_id,
-            "cost_configuration_id": self.cost_configuration_id,
-        }
-
-
 class ResultMetadata(APIObject):
     """
     Metadata for the result of a chat prompt submission.
 
     Attributes
     ----------
     output_token_count : int
@@ -272,20 +119,14 @@
         retrieved from a vector database, if any.
     total_token_count : int
         The total number of tokens processed.
     estimated_docs_token_count : int
         The estimated number of tokens from the documents retrieved from a vector database, if any.
     latency_milliseconds : int
         The latency of the chat prompt submission in milliseconds.
-    feedback_result : FeedbackResult
-        The lists of user_ids providing positive and negative feedback.
-    metrics : MetricMetadata
-        The evaluation metrics for this prompt.
-    final_prompt : Optional[Union[str, dict]], optional
-        Representation of the final prompt sent to the LLM.
     error_message : str or None, optional
         The error message from the LLM response.
     cost : float or None, optional
         The cost of the chat prompt submission.
     """
 
     _converter = result_metadata_trafaret
@@ -293,32 +134,24 @@
     def __init__(
         self,
         output_token_count: int,
         input_token_count: int,
         total_token_count: int,
         estimated_docs_token_count: int,
         latency_milliseconds: int,
-        feedback_result: Dict[str, Any],
-        metrics: List[Dict[str, Any]],
-        final_prompt: Optional[Union[str, Dict[str, Any], List[Dict[str, Any]]]] = None,
         error_message: Optional[str] = None,
         cost: Optional[float] = None,
     ):
         self.output_token_count = output_token_count
         self.input_token_count = input_token_count
         self.total_token_count = total_token_count
         self.estimated_docs_token_count = estimated_docs_token_count
         self.latency_milliseconds = latency_milliseconds
         self.error_message = error_message
         self.cost = cost
-        self.feedback_result = FeedbackResult.from_server_data(feedback_result)
-        self.metrics = [
-            MetricMetadata.from_server_data(metric_metadata) for metric_metadata in metrics
-        ]
-        self.final_prompt = final_prompt
 
     def __repr__(self) -> str:
         return (
             f"{self.__class__.__name__}(output_token_count={self.output_token_count}, "
             f"input_token_count={self.input_token_count}, "
             f"total_token_count={self.total_token_count}, "
             f"estimated_docs_token_count={self.estimated_docs_token_count}, "
@@ -434,15 +267,15 @@
         ID of the chat associated with the chat prompt.
     chat_context_id: Optional[str]
         The ID of the chat context for the chat prompt.
     chat_prompt_ids_included_in_history: Optional[list[str]]
         The IDs of the chat prompts included in the chat history for this chat prompt.
     """
 
-    _path = "api-gw/genai/chatPrompts"
+    _path = "api/v2/genai/chatPrompts"
 
     _converter = chat_prompt_trafaret
 
     def __init__(
         self,
         id: str,
         text: str,
@@ -582,44 +415,14 @@
         chat_prompt : ChatPrompt
             The requested chat prompt.
         """
         url = f"{cls._client.domain}/{cls._path}/{get_entity_id(chat_prompt)}/"
         r_data = cls._client.get(url)
         return cls.from_server_data(r_data.json())
 
-    def update(
-        self,
-        custom_metrics: Optional[list[MetricMetadata]] = None,
-        feedback_metadata: Optional[FeedbackMetadata] = None,
-    ) -> ChatPrompt:
-        """
-        Update the chat prompt.
-
-        Parameters
-        ----------
-        custom_metrics : Optional[list[MetricMetadata]], optional
-            The new custom metrics to add to the chat prompt.
-        feedback_metadata: Optional[FeedbackMetadata], optional
-            The new feedback to add to the chat prompt.
-
-        Returns
-        -------
-        chat_prompt : ChatPrompt
-            The updated chat prompt.
-        """
-        payload = {
-            "custom_metrics": [metadata.to_dict() for metadata in custom_metrics]
-            if custom_metrics
-            else None,
-            "feedback_metadata": feedback_metadata.to_dict() if feedback_metadata else None,
-        }
-        url = f"{self._client.domain}/{self._path}/{self.id}/"
-        r_data = self._client.patch(url, data=payload)
-        return self.from_server_data(r_data.json())
-
     @classmethod
     def list(
         cls,
         llm_blueprint: Optional[Union[LLMBlueprint, str]] = None,
         playground: Optional[Union[Playground, str]] = None,
         chat: Optional[Union[Chat, str]] = None,
     ) -> List[ChatPrompt]:
```

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/comparison_chat.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/comparison_chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # Released under the terms of DataRobot Tool and Utility Agreement.
 from __future__ import annotations
 
 from typing import List, Optional, Union
 
 import trafaret as t
 
-from datarobot._experimental.models.genai.playground import Playground
 from datarobot.models.api_object import APIObject
+from datarobot.models.genai.playground import Playground
 from datarobot.utils.pagination import unpaginate
 
 
 def get_entity_id(entity: Union[ComparisonChat, Playground, str]) -> str:
     """
     Get the entity ID from the entity parameter.
 
@@ -62,15 +62,15 @@
         The ID of the playground associated with the comparison chat.
     creation_date : str
         The date when the comparison chat was created.
     creation_user_id : str
         The ID of the creating user.
     """
 
-    _path = "api-gw/genai/comparisonChats"
+    _path = "api/v2/genai/comparisonChats"
 
     _converter = comparison_chat_trafaret
 
     def __init__(
         self,
         id: str,
         name: str,
```

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/comparison_prompt.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/comparison_prompt.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,31 +9,27 @@
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
 from __future__ import annotations
 
 from typing import Any, Dict, List, Optional, Union
 
-from mypy_extensions import TypedDict
 import trafaret as t
 
-from datarobot._experimental.models.genai.chat_prompt import (
+from datarobot.models.api_object import APIObject
+from datarobot.models.genai.chat_prompt import (
     Citation,
     citation_trafaret,
     confidence_scores_trafaret,
     ConfidenceScores,
-    feedback_metadata_trafaret,
-    FeedbackMetadata,
-    FeedbackMetadataDict,
     result_metadata_trafaret,
     ResultMetadata,
 )
-from datarobot._experimental.models.genai.comparison_chat import ComparisonChat
-from datarobot._experimental.models.genai.llm_blueprint import LLMBlueprint
-from datarobot.models.api_object import APIObject
+from datarobot.models.genai.comparison_chat import ComparisonChat
+from datarobot.models.genai.llm_blueprint import LLMBlueprint
 from datarobot.utils.pagination import unpaginate
 from datarobot.utils.waiters import wait_for_async_resolution
 
 
 def _get_genai_entity_id(entity: Union[ComparisonChat, ComparisonPrompt, LLMBlueprint, str]) -> str:
     """
     Get the entity ID from the entity parameter.
@@ -50,27 +46,14 @@
     """
     if isinstance(entity, str):
         return entity
 
     return entity.id
 
 
-class FeedbackResultDict(TypedDict):
-    comparison_prompt_result_id: str
-    feedback_metadata: FeedbackMetadataDict
-
-
-feedback_result_trafaret = t.Dict(
-    {
-        t.Key("comparison_prompt_result_id"): t.String,
-        t.Key("feedback_metadata"): feedback_metadata_trafaret,
-    }
-).ignore_extra("*")
-
-
 comparison_prompt_result_trafaret = t.Dict(
     {
         t.Key("id"): t.String,
         t.Key("llm_blueprint_id"): t.String,
         t.Key("result_metadata", optional=True): t.Or(result_metadata_trafaret, t.Null),
         t.Key("result_text", optional=True): t.Or(t.String, t.Null),
         t.Key("confidence_scores", optional=True): t.Or(confidence_scores_trafaret, t.Null),
@@ -92,46 +75,14 @@
         t.Key("creation_date"): t.String,
         t.Key("creation_user_id"): t.String,
         t.Key("comparison_chat_id", optional=True): t.Or(t.String, t.Null),
     }
 ).ignore_extra("*")
 
 
-class FeedbackResult(APIObject):
-    """
-    Feedback associated with a comparison prompt result.
-
-    Attributes
-    ----------
-    comparison_prompt_result_id : str
-        The ID of the comparison prompt result associated with the feedback.
-    feedback_metadata : FeedbackMetadata
-        The metadata for the feedback.
-    """
-
-    _converter = feedback_result_trafaret
-
-    def __init__(self, comparison_prompt_result_id: str, feedback_metadata: FeedbackMetadata):
-        self.comparison_prompt_result_id = comparison_prompt_result_id
-        self.feedback_metadata = feedback_metadata
-
-    def __repr__(self) -> str:
-        return (
-            f"{self.__class__.__name__}"
-            f"(comparison_prompt_result_id={self.comparison_prompt_result_id},"
-            f"feedback_metadata={self.feedback_metadata})"
-        )
-
-    def to_dict(self) -> FeedbackResultDict:
-        return {
-            "comparison_prompt_result_id": self.comparison_prompt_result_id,
-            "feedback_metadata": self.feedback_metadata.to_dict(),
-        }
-
-
 class ComparisonPromptResult(APIObject):
     """
     Metadata for a DataRobot GenAI comparison prompt result.
 
     Attributes
     ----------
     id: str
@@ -208,15 +159,15 @@
         Date when the playground was created.
     creation_user_id : str
         ID of the creating user.
     comparison_chat_id : str
         The ID of the comparison chat this comparison prompt is associated with.
     """
 
-    _path = "api-gw/genai/comparisonPrompts"
+    _path = "api/v2/genai/comparisonPrompts"
 
     _converter = comparison_prompt_trafaret
 
     def __init__(
         self,
         id: str,
         text: str,
@@ -341,16 +292,16 @@
         url = f"{cls._client.domain}/{cls._path}/"
         r_data = unpaginate(url, params, cls._client)
         return [cls.from_server_data(data) for data in r_data]
 
     def update(
         self,
         additional_llm_blueprints: Optional[List[Union[LLMBlueprint, str]]] = None,
-        feedback_result: Optional[FeedbackResult] = None,
         wait_for_completion: bool = False,
+        **kwargs: Any,
     ) -> ComparisonPrompt:
         """
         Update the comparison prompt.
 
         Parameters
         ----------
         additional_llm_blueprints : list[LLMBlueprint or str]
@@ -363,15 +314,14 @@
         """
         payload = {
             "additionalLLMBlueprintIds": [
                 _get_genai_entity_id(bp) for bp in additional_llm_blueprints
             ]
             if additional_llm_blueprints
             else None,
-            "feedbackResult": feedback_result.to_dict() if feedback_result else None,
         }
         url = f"{self._client.domain}/{self._path}/{_get_genai_entity_id(self.id)}/"
         r_data = self._client.patch(url, data=payload)
         if wait_for_completion and additional_llm_blueprints:
             # If no additional_llm_blueprints then we get no location header
             location = wait_for_async_resolution(self._client, r_data.headers["Location"])
             return self.from_location(location)
```

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/custom_model_llm_validation.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/custom_model_llm_validation.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
 from __future__ import annotations
 
-from datarobot._experimental.models.genai.custom_model_validation import CustomModelValidation
+from datarobot.models.genai.custom_model_validation import CustomModelValidation
 
 
 class CustomModelLLMValidation(CustomModelValidation):
     """
     Validation record checking the ability of the deployment to serve
     as a custom model LLM.
 
@@ -40,10 +40,18 @@
         - authorization_header - second of 2 auth headers for the prediction server.
         - input_type - Either JSON or CSV - the input type that the model expects.
         - model_type - Target type of the deployed custom model.
     tenant_id : str
         Creating user's tenant ID.
     error_message : Optional[str]
         Additional information for errored validation.
+    deployment_name : Optional[str]
+        The name of the deployment that is validated.
+    user_name : Optional[str]
+        The name of the user
+    use_case_id : Optional[str]
+        The ID of the Use Case associated with the validation.
+    prediction_timeout: int
+        The timeout in seconds for the prediction API used in this custom model validation.
     """
 
-    _path = "api-gw/genai/customModelLLMValidations"
+    _path = "api/v2/genai/customModelLLMValidations"
```

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/custom_model_validation.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/custom_model_validation.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 # Released under the terms of DataRobot Tool and Utility Agreement.
 from __future__ import annotations
 
 from typing import Any, Dict, List, Optional, Union
 
 import trafaret as t
 
-from datarobot._experimental.models.genai.playground import Playground
 from datarobot.errors import ClientError
 from datarobot.models.api_object import APIObject
 from datarobot.models.deployment import Deployment
+from datarobot.models.genai.playground import Playground
 from datarobot.models.model import Model
 from datarobot.models.use_cases.use_case import UseCase
 from datarobot.models.use_cases.utils import get_use_case_id, resolve_use_cases, UseCaseLike
 from datarobot.utils.pagination import unpaginate
 from datarobot.utils.waiters import wait_for_async_resolution
 
 
@@ -67,14 +67,15 @@
         t.Key("tenant_id"): t.String,
         t.Key("user_id"): t.String,
         t.Key("creation_date"): t.String,
         t.Key("error_message", optional=True, default=None): t.Or(t.Null, t.String),
         t.Key("deployment_name", optional=True, default=None): t.Or(t.Null, t.String),
         t.Key("user_name", optional=True, default=None): t.Or(t.Null, t.String),
         t.Key("use_case_id", optional=True, default=None): t.Or(t.Null, t.String),
+        t.Key("prediction_timeout"): t.Int,
     }
 ).ignore_extra("*")
 
 
 class CustomModelValidation(APIObject):
     """
     Validation record checking the ability of the deployment to serve
@@ -101,16 +102,22 @@
         - authorization_header - Second of two auth headers for the prediction server.
         - input_type - Either JSON or CSV - input type model expects.
         - model_type - Target type of deployed custom model.
     tenant_id : str
         Creating user's tenant ID.
     error_message : Optional[str]
         Additional information for errored validation.
+    deployment_name : Optional[str]
+        The name of the deployment that is validated.
+    user_name : Optional[str]
+        The name of the user
     use_case_id : Optional[str]
-        The ID of the use case associated with the validation.
+        The ID of the Use Case associated with the validation.
+    prediction_timeout: int
+        The timeout, in seconds, for the prediction API used in this custom model validation.
     """
 
     _path: str
     _converter = custom_model_validation_trafaret
 
     def __init__(
         self,
@@ -125,14 +132,15 @@
         name: str,
         creation_date: str,
         user_id: str,
         error_message: Optional[str],
         deployment_name: Optional[str],
         user_name: Optional[str],
         use_case_id: Optional[str],
+        prediction_timeout: int,
     ):
         self.id = id
         self.prompt_column_name = prompt_column_name
         self.target_column_name = target_column_name
         self.deployment_id = deployment_id
         self.model_id = model_id
         self.validation_status = validation_status
@@ -141,14 +149,15 @@
         self.error_message = error_message
         self.name = name
         self.creation_date = creation_date
         self.user_id = user_id
         self.deployment_name = deployment_name
         self.user_name = user_name
         self.use_case_id = use_case_id
+        self.prediction_timeout = prediction_timeout
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(id={self.id})"
 
     @classmethod
     def get(cls, validation_id: str) -> CustomModelValidation:
         """
@@ -237,16 +246,16 @@
         deployment : Optional[Union[Deployment, str]], optional
             The returned validations are filtered to those associated with a specific deployment
             if specified, either `Deployment` or deployment ID.
         model_id : Optional[Union[Model, str]], optional
             The returned validations are filtered to those associated with a specific model
             if specified, either `Model` or model ID.
         use_cases : Optional[list[Union[UseCase, str]]], optional
-            The returned validations are filtered to those associated with specific use cases
-            if specified, either `UseCase` or use case IDs.
+            The returned validations are filtered to those associated with specific Use Cases
+            if specified, either `UseCase` or Use Case IDs.
         playground_id : Optional[Union[Playground, str]], optional
             The returned validations are filtered to those used in a specific playground
             if specified, either `Playground` or playground ID.
         completed_only : bool, optional
             Whether to retrieve only completed validations.
         search : Optional[str], optional
             String for filtering validations.
@@ -286,14 +295,15 @@
         prompt_column_name: str,
         target_column_name: str,
         deployment_id: Union[Deployment, str],
         model: Optional[Union[Model, str]] = None,
         use_case: Optional[Union[UseCase, str]] = None,
         name: Optional[str] = None,
         wait_for_completion: bool = False,
+        prediction_timeout: Optional[int] = None,
     ) -> CustomModelValidation:
         """
         Start the validation of deployment to serve as a vector database or LLM.
 
         Parameters
         ----------
         prompt_column_name : str
@@ -303,36 +313,40 @@
         deployment_id : Union[Deployment, str]
             The deployment to validate, either `Deployment` or deployment ID.
         model : Optional[Union[Model, str]], optional
             The specific model within the deployment, either `Model` or model ID.
             If not specified, the underlying model ID will be derived from the
             deployment info automatically.
         use_case : Optional[Union[UseCase, str]], optional
-            The use case to link the validation to, either `UseCase` or use case ID.
+            The Use Case to link the validation to, either `UseCase` or Use Case ID.
         name : Optional[str], optional
             The name of the validation.
         wait_for_completion : bool
             If set to True code will wait for the validation job to complete before
             returning the result (up to 10 minutes, raising timeout error after that).
             Otherwise, you can check current validation status by using
             CustomModelValidation.get with returned ID.
+        prediction_timeout : Optional[int], optional
+            The timeout, in seconds, for the prediction API used in this custom model validation.
 
         Returns
         -------
         CustomModelValidation
         """
 
         payload = {
             "prompt_column_name": prompt_column_name,
             "target_column_name": target_column_name,
             "deployment_id": get_entity_id(deployment_id),
             "model_id": get_entity_id(model) if model else None,
             "use_case_id": get_use_case_id(use_case, is_required=False),
             "name": name,
         }
+        if prediction_timeout is not None:
+            payload["prediction_timeout"] = prediction_timeout  # type: ignore[assignment]
         url = f"{cls._client.domain}/{cls._path}/"
         response = cls._client.post(url, data=payload)
         if wait_for_completion:
             location = wait_for_async_resolution(cls._client, response.headers["Location"])
             return cls.from_location(location)
         return cls.from_server_data(response.json())
 
@@ -365,14 +379,15 @@
     def update(
         self,
         name: Optional[str] = None,
         prompt_column_name: Optional[str] = None,
         target_column_name: Optional[str] = None,
         deployment: Optional[Union[Deployment, str]] = None,
         model: Optional[Union[Model, str]] = None,
+        prediction_timeout: Optional[int] = None,
     ) -> CustomModelValidation:
         """
         Update a custom model validation.
 
         Parameters
         ----------
         name : Optional[str], optional
@@ -381,25 +396,28 @@
             The new name of the prompt column.
         target_column_name : Optional[str], optional
             The new name of the target column.
         deployment : Optional[Union[Deployment, str]], optional
             The new deployment to validate.
         model : Optional[Union[Model, str]], optional
             The new model within the deployment to validate.
+        prediction_timeout : Optional[int], optional
+            The new timeout, in seconds, for the prediction API used in this custom model validation.
 
         Returns
         -------
         CustomModelValidation
         """
         payload = {
             "name": name,
             "prompt_column_name": prompt_column_name,
             "target_column_name": target_column_name,
             "deployment_id": get_entity_id(deployment) if deployment else None,
             "model_id": get_entity_id(model) if model else None,
+            "prediction_timeout": prediction_timeout,
         }
         url = f"{self._client.domain}/{self._path}/{self.id}/"
         response = self._client.patch(url, data=payload)
         return self.from_server_data(response.json())
 
     def delete(self) -> None:
         """
```

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/llm.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/llm.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,15 +270,15 @@
         Languages supported by this model.
     settings : list of LLMSettingDefinition
         Settings for this model
     context_size : int
         The context size for this model
     """
 
-    _path = "api-gw/genai/llms"
+    _path = "api/v2/genai/llms"
 
     _converter = language_model_definition_trafaret
 
     def __init__(
         self,
         id: str,
         name: str,
```

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/llm_blueprint.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/llm_blueprint.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,21 +12,20 @@
 from __future__ import annotations
 
 from typing import Any, cast, Dict, List, Optional, Union
 
 from mypy_extensions import TypedDict
 import trafaret as t
 
-from datarobot._experimental.models.enums import PromptType
-from datarobot._experimental.models.genai.llm import LLMDefinition
-from datarobot._experimental.models.genai.playground import Playground
-from datarobot._experimental.models.genai.vector_database import VectorDatabase
-from datarobot.enums import enum_to_list
+from datarobot.enums import enum_to_list, PromptType
 from datarobot.models.api_object import APIObject
 from datarobot.models.custom_model import CustomModelVersion
+from datarobot.models.genai.llm import LLMDefinition
+from datarobot.models.genai.playground import Playground
+from datarobot.models.genai.vector_database import VectorDatabase
 from datarobot.utils import to_api
 from datarobot.utils.pagination import unpaginate
 from datarobot.utils.waiters import wait_for_async_resolution
 
 
 def get_entity_id(
     entity: Union[Playground, LLMDefinition, VectorDatabase, LLMBlueprint, str]
@@ -51,14 +50,26 @@
 
 
 class VectorDatabaseSettingsDict(TypedDict):
     max_documents_retrieved_per_prompt: Optional[int]
     max_tokens: Optional[int]
 
 
+class LLMSettingsCommonDict(TypedDict):
+    system_prompt: Optional[str]
+    max_completion_length: Optional[int]
+    temperature: Optional[float]
+    top_p: Optional[float]
+
+
+class LLMSettingsCustomModelDict(TypedDict):
+    system_prompt: Optional[str]
+    validation_id: Optional[str]
+
+
 vector_database_settings_trafaret = t.Dict(
     {
         t.Key("max_documents_retrieved_per_prompt", optional=True): t.Or(t.Int, t.Null),
         t.Key("max_tokens", optional=True): t.Or(t.Int, t.Null),
     }
 ).ignore_extra("*")
 
@@ -185,15 +196,15 @@
         The status of the custom model LLM validation if the llm_id is 'custom-model'.
     custom_model_llm_error_message : str or None
         The error message for the custom model LLM, if any.
     custom_model_llm_error_resolution : str or None
         The resolution for the custom model LLM error, if any.
     """
 
-    _path = "api-gw/genai/llmBlueprints"
+    _path = "api/v2/genai/llmBlueprints"
 
     _converter = llm_blueprint_trafaret
 
     def __init__(
         self,
         id: str,
         name: str,
@@ -204,15 +215,15 @@
         creation_date: str,
         creation_user_id: str,
         last_update_date: str,
         last_update_user_id: str,
         prompt_type: PromptType,
         llm_id: Optional[str] = None,
         llm_name: Optional[str] = None,
-        llm_settings: Optional[Dict[str, Any]] = None,
+        llm_settings: Optional[LLMSettingsCommonDict | LLMSettingsCustomModelDict] = None,
         vector_database_id: Optional[str] = None,
         vector_database_settings: Optional[Dict[str, Any]] = None,
         vector_database_name: Optional[str] = None,
         vector_database_status: Optional[str] = None,
         vector_database_error_message: Optional[str] = None,
         vector_database_error_resolution: Optional[str] = None,
         custom_model_llm_validation_status: Optional[str] = None,
@@ -256,15 +267,15 @@
     def create(
         cls,
         playground: Union[Playground, str],
         name: str,
         prompt_type: PromptType = PromptType.CHAT_HISTORY_AWARE,
         description: str = "",
         llm: Optional[Union[LLMDefinition, str]] = None,
-        llm_settings: Optional[Dict[str, Optional[Union[bool, int, float, str]]]] = None,
+        llm_settings: Optional[LLMSettingsCommonDict | LLMSettingsCustomModelDict] = None,
         vector_database: Optional[Union[VectorDatabase, str]] = None,
         vector_database_settings: Optional[VectorDatabaseSettings] = None,
     ) -> LLMBlueprint:
         """
         Create a new LLM blueprint.
 
         Parameters
@@ -435,15 +446,15 @@
         return [cls.from_server_data(data) for data in r_data]
 
     def update(
         self,
         name: Optional[str] = None,
         description: Optional[str] = None,
         llm: Optional[Union[LLMDefinition, str]] = None,
-        llm_settings: Optional[Dict[str, Optional[Union[bool, int, float, str]]]] = None,
+        llm_settings: Optional[LLMSettingsCommonDict | LLMSettingsCustomModelDict] = None,
         vector_database: Optional[Union[VectorDatabase, str]] = None,
         vector_database_settings: Optional[VectorDatabaseSettings] = None,
         is_saved: Optional[bool] = None,
         is_starred: Optional[bool] = None,
         prompt_type: Optional[PromptType] = None,
         remove_vector_database: Optional[bool] = False,
     ) -> LLMBlueprint:
@@ -538,11 +549,11 @@
         """
         payload = {
             "llm_blueprint_id": self.id,
             "prompt_column_name": prompt_column_name,
             "target_column_name": target_column_name,
         }
 
-        url = f"{self._client.domain}/api-gw/genai/customModelVersions/"
+        url = f"{self._client.domain}/api/v2/genai/customModelVersions/"
         r_data = self._client.post(url, data=payload)
         location = wait_for_async_resolution(self._client, r_data.headers["Location"])
         return CustomModelVersion.from_location(location)
```

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/playground.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/playground.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         t.Key("use_case_id"): t.String,
         t.Key("creation_date"): t.String,
         t.Key("creation_user_id"): t.String,
         t.Key("last_update_date"): t.String,
         t.Key("last_update_user_id"): t.String,
         t.Key("saved_llm_blueprints_count"): t.Int,
         t.Key("llm_blueprints_count"): t.Int,
-        t.Key("user_name"): t.String,
+        t.Key("user_name"): t.String(allow_blank=True),
     }
 ).ignore_extra("*")
 
 
 class Playground(APIObject):
     """
     Metadata for a DataRobot GenAI playground.
@@ -63,15 +63,15 @@
         Number of saved LLM blueprints in the playground.
     llm_blueprints_count : int
         Number of LLM blueprints in the playground.
     user_name : str
         The name of the user who created the playground.
     """
 
-    _path = "api-gw/genai/playgrounds"
+    _path = "api/v2/genai/playgrounds"
 
     _converter = playground_trafaret
 
     def __init__(
         self,
         id: str,
         name: str,
```

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/prompt_trace.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/prompt_trace.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,16 +15,18 @@
 
 import trafaret as t
 
 from datarobot._experimental.models.genai.chat_prompt import (
     confidence_scores_trafaret,
     result_metadata_trafaret,
 )
-from datarobot._experimental.models.genai.llm_blueprint import vector_database_settings_trafaret
 from datarobot.models.api_object import APIObject
+from datarobot.models.genai.comparison_chat import get_entity_id
+from datarobot.models.genai.llm_blueprint import vector_database_settings_trafaret
+from datarobot.models.genai.playground import Playground
 from datarobot.utils.pagination import unpaginate
 
 datarobot_user = t.Dict(
     {
         t.Key("id"): t.String,
         t.Key("name"): t.String,
     }
@@ -34,17 +36,17 @@
     {
         t.Key("timestamp"): t.String,
         t.Key("user"): datarobot_user,
         t.Key("chat_prompt_id", optional=True): t.Or(t.String, t.Null),
         t.Key("use_case_id", optional=True): t.Or(t.String, t.Null),
         t.Key("comparison_prompt_id", optional=True): t.Or(t.String, t.Null),
         t.Key("llm_blueprint_id"): t.String,
-        t.Key("llm_name"): t.String,
-        t.Key("llm_vendor"): t.String,
-        t.Key("llm_license"): t.String,
+        t.Key("llm_name", optional=True): t.Or(t.String, t.Null),
+        t.Key("llm_vendor", optional=True): t.Or(t.String, t.Null),
+        t.Key("llm_license", optional=True): t.Or(t.String, t.Null),
         t.Key("llm_settings", optional=True): t.Or(t.Dict().allow_extra("*"), t.Null),
         t.Key("vector_database_id", optional=True): t.Or(t.String, t.Null),
         t.Key("vector_database_settings", optional=True): t.Or(
             vector_database_settings_trafaret, t.Null
         ),
         t.Key("result_metadata", optional=True): t.Or(result_metadata_trafaret, t.Dict()),
         t.Key("result_text", optional=True): t.Or(t.String, t.Null),
@@ -102,30 +104,30 @@
         The confidence scores if there is a vector database associated with the prompt.
     text: str
         The prompt text submitted to the LLM.
     execution_status: str
         The execution status of the chat prompt.
     """
 
-    _path = "api-gw/genai/playgrounds/{}/trace/"
-    _export_path = "api-gw/genai/playgrounds/{}/traceDatasets/"
+    _path = "api/v2/genai/playgrounds/{}/trace/"
+    _export_path = "api/v2/genai/playgrounds/{}/traceDatasets/"
 
     _converter = prompt_trace
 
     def __init__(
         self,
         timestamp: str,
         user: Dict[str, str],
         use_case_id: str,
         llm_blueprint_id: str,
-        llm_name: str,
-        llm_vendor: str,
-        llm_license: str,
         text: str,
         execution_status: str,
+        llm_name: Optional[str] = None,
+        llm_vendor: Optional[str] = None,
+        llm_license: Optional[str] = None,
         chat_prompt_id: Optional[str] = None,
         comparison_prompt_id: Optional[str] = None,
         llm_settings: Optional[Dict[str, Any]] = None,
         vector_database_id: Optional[str] = None,
         vector_database_settings: Optional[Dict[str, Any]] = None,
         result_metadata: Optional[Dict[str, Any]] = None,
         result_text: Optional[str] = None,
@@ -146,43 +148,45 @@
         self.result_metadata = result_metadata
         self.result_text = result_text
         self.confidence_scores = confidence_scores
         self.text = text
         self.execution_status = execution_status
 
     @classmethod
-    def list(cls, playground_id: str) -> List[PromptTrace]:
+    def list(cls, playground: str | Playground) -> List[PromptTrace]:
         """
         List all prompt traces for a playground.
 
         Parameters
         ----------
-        playground_id: str
+        playground: str
             The ID of the playground to list prompt traces for.
 
         Returns
         -------
         prompt_traces: list[PromptTrace]
             List of prompt traces for the playground.
         """
+        playground_id = get_entity_id(playground)
         url = f"{cls._client.domain}/{cls._path.format(playground_id)}"
         response = unpaginate(url, None, cls._client)
         return [cls.from_server_data(trace) for trace in response]
 
     @classmethod
-    def export_to_ai_catalog(cls, playground_id: str) -> Any:
+    def export_to_ai_catalog(cls, playground: str | Playground) -> Any:
         """
         Export prompt traces to AI Catalog as a CSV.
 
         Parameters
         ----------
-        playground_id: str
+        playground: str
             The ID of the playground to export prompt traces for.
 
         Returns
         -------
         status_url: str
             The URL where the status of the job can be monitored
         """
+        playground_id = get_entity_id(playground)
         url = f"{cls._client.domain}/{cls._export_path.format(playground_id)}"
         response = cls._client.post(url)
         return response.headers["Location"]
```

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/user_limits.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/user_limits.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
 
 class UserLimits(APIObject):
     """
     Counts for user limits for LLM APIs and vector databases.
     """
 
-    _llm_path = "api-gw/genai/userLimits/llmApiCalls/"
-    _vector_db_path = "api-gw/genai/userLimits/vectorDatabases/"
+    _llm_path = "api/v2/genai/userLimits/llmApiCalls/"
+    _vector_db_path = "api/v2/genai/userLimits/vectorDatabases/"
 
     _converter = t.Dict(
         {
             t.Key("counter"): t.Int(),
         }
     )
```

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/genai/vector_database.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/vector_database.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 # Released under the terms of DataRobot Tool and Utility Agreement.
 from __future__ import annotations
 
 from typing import Any, Dict, List, Optional, Union
 
 import trafaret as t
 
-from datarobot._experimental.models.genai.custom_model_validation import CustomModelValidation
-from datarobot._experimental.models.genai.playground import Playground
 from datarobot.models.api_object import APIObject
+from datarobot.models.genai.custom_model_validation import CustomModelValidation
+from datarobot.models.genai.playground import Playground
 from datarobot.models.use_cases.use_case import UseCase
 from datarobot.models.use_cases.utils import get_use_case_id, resolve_use_cases, UseCaseLike
 from datarobot.utils.pagination import unpaginate
 
 
 def get_entity_id(entity: Union[Playground, str]) -> str:
     """
@@ -58,28 +58,18 @@
         t.Key("embedding_model"): str,
         t.Key("description"): str,
         t.Key("max_sequence_length"): int,
         t.Key("languages"): str,
     }
 ).ignore_extra("*")
 
-supported_custom_model_embeddings_trafaret = t.Dict(
-    {
-        t.Key("id"): t.String,
-        t.Key("name"): t.String,
-    }
-)
-
 supported_embeddings_trafaret = t.Dict(
     {
         t.Key("embedding_models"): t.List(embedding_model_trafaret),
         t.Key("default_embedding_model"): t.String,
-        t.Key("custom_model_embedding_validations"): t.List(
-            supported_custom_model_embeddings_trafaret
-        ),
     }
 ).ignore_extra("*")
 
 text_chunking_parameter_fields_trafaret = t.Dict(
     {
         t.Key("name"): t.String,
         t.Key("type"): t.String,
@@ -133,15 +123,14 @@
         t.Key("execution_status"): t.String,
         t.Key("playgrounds_count"): t.Int,
         t.Key("dataset_name"): t.String(allow_blank=True),
         t.Key("user_name"): t.String,
         t.Key("source"): t.String,
         t.Key("validation_id", optional=True, default=None): t.Or(t.Null, t.String),
         t.Key("error_message", optional=True, default=None): t.Or(t.Null, t.String),
-        t.Key("embedding_validation_id", optional=True, default=None): t.Or(t.Null, t.String),
         t.Key("is_separator_regex"): t.Bool,
     }
 ).ignore_extra("*")
 
 
 class ChunkingParameters(APIObject):
     """
@@ -213,37 +202,14 @@
     ):
         self.embedding_model = embedding_model
         self.description = description
         self.max_sequence_length = max_sequence_length
         self.languages = languages
 
 
-class SupportedCustomModelEmbeddings(APIObject):
-    """
-    All supported custom embedding models for the use case.
-
-    Attributes
-    ----------
-    id : str
-        ID of the custom model embedding validation.
-    name : str
-        The name of the custom model embedding validation.
-    """
-
-    _converter = supported_custom_model_embeddings_trafaret
-
-    def __init__(
-        self,
-        id: str,
-        name: str,
-    ):
-        self.id = id
-        self.name = name
-
-
 class SupportedEmbeddings(APIObject):
     """
     All supported embedding models including the recommended default model.
 
     Attributes
     ----------
     embedding_models : list[EmbeddingModel]
@@ -256,24 +222,19 @@
 
     _converter = supported_embeddings_trafaret
 
     def __init__(
         self,
         embedding_models: List[Dict[str, Any]],
         default_embedding_model: str,
-        custom_model_embedding_validations: List[Dict[str, Any]],
     ):
         self.embedding_models = [
             EmbeddingModel.from_server_data(model) for model in embedding_models
         ]
         self.default_embedding_model = default_embedding_model
-        self.custom_model_embedding_validations = [
-            SupportedCustomModelEmbeddings.from_server_data(validation)
-            for validation in custom_model_embedding_validations
-        ]
 
 
 class TextChunkingParameterFields(APIObject):
     """
     Text chunking parameter fields.
 
     Attributes
@@ -458,15 +419,15 @@
         Additional information for errored vector database.
     embedding_validation_id : Optional[str]
         ID of the custom embedding validation, if any.
     is_separator_regex : bool
         Whether the separators should be treated as regular expressions.
     """
 
-    _path = "api-gw/genai/vectorDatabases"
+    _path = "api/v2/genai/vectorDatabases"
 
     _converter = vector_database_trafaret
 
     def __init__(
         self,
         id: str,
         name: str,
@@ -487,15 +448,14 @@
         execution_status: str,
         playgrounds_count: int,
         dataset_name: str,
         user_name: str,
         source: str,
         validation_id: Optional[str],
         error_message: Optional[str],
-        embedding_validation_id: Optional[str],
         is_separator_regex: bool,
     ):
         self.id = id
         self.name = name
         self.size = size
         self.use_case_id = use_case_id
         self.dataset_id = dataset_id
@@ -513,15 +473,14 @@
         self.execution_status = execution_status
         self.playgrounds_count = playgrounds_count
         self.dataset_name = dataset_name
         self.user_name = user_name
         self.source = source
         self.validation_id = validation_id
         self.error_message = error_message
-        self.embedding_validation_id = embedding_validation_id
         self.is_separator_regex = is_separator_regex
 
     def __repr__(self) -> str:
         return (
             f"{self.__class__.__name__}(id={self.id}, name={self.name}, "
             f"execution_status={self.execution_status})"
         )
@@ -804,10 +763,16 @@
         - authorization_header - second of 2 auth headers for prediction server.
         - input_type - Either JSON or CSV - input type model expects.
         - model_type - Target type of deployed custom model.
     tenant_id : str
         Creating user's tenant ID.
     error_message : Optional[str]
         Additional information for errored validation.
+    deployment_name : Optional[str]
+        The name of the deployment that is validated.
+    user_name : Optional[str]
+        The name of the user
+    use_case_id : Optional[str]
+        The ID of the use case associated with the validation.
     """
 
-    _path = "api-gw/genai/customModelVectorDatabaseValidations"
+    _path = "api/v2/genai/customModelVectorDatabaseValidations"
```

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/idiomatic_project.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/idiomatic_project.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/incremental_learning.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/incremental_learning.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/model.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/model_lineage.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/model_lineage.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/notebooks.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/notebooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,14 +128,16 @@
 
 # TODO: [NB-4787] We are using trafaret's "ignore_extra" very liberally and this is a subset of properties
 notebook_scheduled_job_trafaret = t.Dict(
     {
         t.Key("id"): t.String,
         t.Key("enabled"): t.Bool,
         t.Key("next_run_time"): t.String,
+        t.Key("run_type"): t.String,
+        t.Key("notebook_type"): t.String,
         t.Key("job_payload"): scheduled_job_payload_trafaret,
         t.Key("title", optional=True): t.String,
         t.Key("schedule", optional=True): t.String,
         t.Key("schedule_localized", optional=True): t.String,
         t.Key("last_successful_run", optional=True): t.String,
         t.Key("last_failed_run", optional=True): t.String,
         t.Key("last_run_time", optional=True): t.String,
@@ -444,14 +446,18 @@
 
     id : str
         The ID of the Notebook Scheduled Job.
     enabled : bool
         Whether job is enabled or not.
     next_run_time : str
         The next time the job is scheduled to run (assuming it is enabled).
+    run_type : RunType
+        The type of the run - either manual (triggered via UI or API) or scheduled.
+    notebook_type: NotebookType
+        The type of the notebook - either plain or codespace.
     job_payload : ScheduledJobPayload
         The payload used for the background job.
     title : Optional[str]
         The title of the job. Optional.
     schedule : Optional[str]
         Cron-like string to define how frequently job should be run. Optional.
     schedule_localized : Optional[str]
@@ -470,25 +476,29 @@
     _converter = notebook_scheduled_job_trafaret
 
     def __init__(
         self,
         id: str,
         enabled: bool,
         next_run_time: str,
+        run_type: str,
+        notebook_type: str,
         job_payload: Dict[str, Union[str, List[Dict[str, str]]]],
         title: Optional[str] = None,
         schedule: Optional[str] = None,
         schedule_localized: Optional[str] = None,
         last_successful_run: Optional[str] = None,
         last_failed_run: Optional[str] = None,
         last_run_time: Optional[str] = None,
     ):
         self.id = id
         self.enabled = enabled
         self.next_run_time = next_run_time
+        self.run_type = run_type
+        self.notebook_type = notebook_type
         self.job_payload = ScheduledJobPayload.from_server_data(job_payload)
         self.title = title
         self.schedule = schedule
         self.schedule_localized = schedule_localized
         self.last_successful_run = last_successful_run
         self.last_failed_run = last_failed_run
         self.last_run_time = last_run_time
@@ -631,14 +641,18 @@
         The tenant ID associated with the Notebook.
     description : Optional[str]
         The description of the Notebook. Optional.
     session : Optional[NotebookSession]
         Metadata on the current status of the Notebook and its kernel. Optional.
     use_case_id : Optional[str]
         The ID of the Use Case the Notebook is associated with. Optional.
+    use_case_name : Optional[str]
+        The name of the Use Case the Notebook is associated with. Optional.
+    has_schedule : bool
+        Whether or not the notebook has a schedule.
     has_enabled_schedule : bool
         Whether or not the notebook has a currently enabled schedule.
     """
 
     _notebooks_path = "api-gw/nbx/notebooks/"
     _orchestrator_path = "api-gw/nbx/orchestrator/"
     _scheduling_path = "api-gw/nbx/scheduling/"
@@ -656,35 +670,39 @@
             t.Key("updated", optional=True): notebook_activity_trafaret,
             t.Key("last_viewed"): notebook_activity_trafaret,
             t.Key("settings"): notebook_settings_trafaret,
             t.Key("org_id", optional=True): t.Or(t.String, t.Null),
             t.Key("tenant_id", optional=True): t.Or(t.String, t.Null),
             t.Key("session", optional=True): t.Or(notebook_session_trafaret, t.Null),
             t.Key("use_case_id", optional=True): t.Or(t.String, t.Null),
+            t.Key("use_case_name", optional=True): t.Or(t.String, t.Null),
+            t.Key("has_schedule"): t.Bool,
             t.Key("has_enabled_schedule"): t.Bool,
         }
     ).ignore_extra("*")
 
     def __init__(
         self,
         id: str,
         name: str,
         type: NotebookType,
         permissions: List[str],
         tags: List[str],
         created: Dict[str, Any],
         last_viewed: Dict[str, Any],
         settings: Dict[str, bool],
+        has_schedule: bool,
         has_enabled_schedule: bool,
         updated: Optional[Dict[str, Any]] = None,
         org_id: Optional[str] = None,
         tenant_id: Optional[str] = None,
         description: Optional[str] = None,
         session: Optional[Dict[str, str]] = None,
         use_case_id: Optional[str] = None,
+        use_case_name: Optional[str] = None,
     ):
         self.id = id
         self.name = name
         self.type = type
         self.description = description
         self.permissions = [NotebookPermissions[permission] for permission in permissions]
         self.tags = tags
@@ -694,14 +712,16 @@
             last_viewed if not last_viewed else NotebookActivity.from_server_data(last_viewed)
         )
         self.settings = NotebookSettings.from_server_data(settings)
         self.org_id = org_id
         self.tenant_id = tenant_id
         self.session = NotebookSession.from_server_data(session) if session else session
         self.use_case_id = use_case_id
+        self.use_case_name = use_case_name
+        self.has_schedule = has_schedule
         self.has_enabled_schedule = has_enabled_schedule
 
     @property
     def is_standalone(self) -> bool:
         return self.type == NotebookType.STANDALONE
 
     @property
@@ -911,15 +931,15 @@
 
             from datarobot._experimental.models.notebooks import Notebook
 
             notebook = Notebook.get(notebook_id='6556b00dcc4ea0bb7ea48121')
             manual_run = notebook.run()
 
             # Alternatively, with title and parameters:
-            # manual_run = notebook_scheduled_job = notebook.run(title="My Run", parameters=[{"FOO": "bar"}])
+            # manual_run = notebook.run(title="My Run", parameters=[{"FOO": "bar"}])
 
             revision_id = manual_run.wait_for_completion()
         """
         if self.is_codespace and not notebook_path:
             raise InvalidUsageError("Notebook path is required for Codespace notebooks.")
 
         url = f"{self._client.domain}/{self._scheduling_path}manualRun/"
```

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/project_options.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/project_options.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/recipe_operations.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/recipe_operations.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/recipes.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/recipes.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/_experimental/models/retraining.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/retraining.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/analytics.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/analytics.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/client.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/client.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/config.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/config.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/context.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/context.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/enums.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/enums.py`

 * *Files 16% similar despite different names*

```diff
@@ -1234,7 +1234,252 @@
     CREATED = "CREATED"
     SCHEDULED = "SCHEDULED"
     CANCELLED = "CANCELLED"
     FAILED = "FAILED"
     SUCCEEDED = "SUCCEEDED"
 
     ALL = [CREATED, SCHEDULED, CANCELLED, FAILED, SUCCEEDED]
+
+
+class ListVectorDatabasesSortQueryParams(StrEnum):
+    """supported Sort query params for the Vectordatabase.list method."""
+
+    NAME_ASCENDING = "name"
+    NAME_DESCENDING = "-name"
+    CREATION_USER_DATE_ASCENDING = "creationUserId"
+    CREATION_USER_DATE_DESCENDING = "-creationUserId"
+    CREATION_DATE_ASCENDING = "creationDate"
+    CREATION_DATE_DESCENDING = "-creationDate"
+    EMBEDDING_MODEL_ASCENDING = "embeddingModel"
+    EMBEDDING_MODEL_DESCENDING = "-embeddingModel"
+    DATASET_ID_ASCENDING = "datasetId"
+    DATASET_ID_DESCENDING = "-datasetId"
+    CHUNKING_METHOD_ASCENDING = "chunkingMethod"
+    CHUNKING_METHOD_DESCENDING = "-chunkingMethod"
+    CHUNKS_COUNT_ASCENDING = "chunksCount"
+    CHUNKS_COUNT_DESCENDING = "-chunksCount"
+    SIZE_ASCENDING = "size"
+    SIZE_DESCENDING = "-size"
+    USER_NAME_ASCENDING = "userName"
+    USER_NAME_DESCENDING = "-userName"
+    DATASET_NAME_ASCENDING = "datasetName"
+    DATASET_NAME_DESCENDING = "-datasetName"
+    PLAYGROUNDS_COUNT_ASCENDING = "playgroundsCount"
+    PLAYGROUNDS_COUNT_DESCENDING = "-playgroundsCount"
+    SOURCE_ASCENDING = "source"
+    SOURCE_DESCENDING = "-source"
+
+
+class VectorDatabaseEmbeddingModel(StrEnum):
+    """Text embedding model names for VectorDatabases."""
+
+    E5_LARGE_V2 = "intfloat/e5-large-v2"
+    E5_BASE_V2 = "intfloat/e5-base-v2"
+    MULTILINGUAL_E5_BASE = "intfloat/multilingual-e5-base"
+    ALL_MINILM_L6_V2 = "sentence-transformers/all-MiniLM-L6-v2"
+    JINA_EMBEDDING_T_EN_V1 = "jinaai/jina-embedding-t-en-v1"
+    SUP_SIMCSE_JA_BASE = "cl-nagoya/sup-simcse-ja-base"
+
+
+class VectorDatabaseChunkingMethod(StrEnum):
+    """Text chunking method names for VectorDatabases."""
+
+    RECURSIVE = "recursive"
+
+
+class VectorDatabaseDatasetLanguages(StrEnum):
+    """Dataset languages supported by VectorDatabases."""
+
+    AFRIKAANS = "Afrikaans"
+    AMHARIC = "Amharic"
+    ARABIC = "Arabic"
+    ASSAMESE = "Assamese"
+    AZERBAIJANI = "Azerbaijani"
+    BELARUSIAN = "Belarusian"
+    BULGARIAN = "Bulgarian"
+    BENGALI = "Bengali"
+    BRETON = "Breton"
+    BOSNIAN = "Bosnian"
+    CATALAN = "Catalan"
+    CZECH = "Czech"
+    WELSH = "Welsh"
+    DANISH = "Danish"
+    GERMAN = "German"
+    GREEK = "Greek"
+    ENGLISH = "English"
+    ESPERANTO = "Esperanto"
+    SPANISH = "Spanish"
+    ESTONIAN = "Estonian"
+    BASQUE = "Basque"
+    PERSIAN = "Persian"
+    FINNISH = "Finnish"
+    FRENCH = "French"
+    WESTERN_FRISIAN = "Western Frisian"
+    IRISH = "Irish"
+    SCOTTISH_GAELIC = "Scottish Gaelic"
+    GALICIAN = "Galician"
+    GUJARATI = "Gujarati"
+    HAUSA = "Hausa"
+    HEBREW = "Hebrew"
+    HINDI = "Hindi"
+    CROATIAN = "Croatian"
+    HUNGARIAN = "Hungarian"
+    ARMENIAN = "Armenian"
+    INDONESIAN = "Indonesian"
+    ICELANDIC = "Icelandic"
+    ITALIAN = "Italian"
+    JAPANESE = "Japanese"
+    JAVANESE = "Javanese"
+    GEORGIAN = "Georgian"
+    KAZAKH = "Kazakh"
+    KHMER = "Khmer"
+    KANNADA = "Kannada"
+    KOREAN = "Korean"
+    KURDISH = "Kurdish"
+    KYRGYZ = "Kyrgyz"
+    LATIN = "Latin"
+    LAO = "Lao"
+    LITHUANIAN = "Lithuanian"
+    LATVIAN = "Latvian"
+    MALAGASY = "Malagasy"
+    MACEDONIAN = "Macedonian"
+    MALAYALAM = "Malayalam"
+    MONGOLIAN = "Mongolian"
+    MARATHI = "Marathi"
+    MALAY = "Malay"
+    BURMESE = "Burmese"
+    NEPALI = "Nepali"
+    DUTCH = "Dutch"
+    NORWEGIAN = "Norwegian"
+    OROMO = "Oromo"
+    ORIYA = "Oriya"
+    PANJABI = "Panjabi"
+    POLISH = "Polish"
+    PASHTO = "Pashto"
+    PORTUGUESE = "Portuguese"
+    ROMANIAN = "Romanian"
+    RUSSIAN = "Russian"
+    SANSKRIT = "Sanskrit"
+    SINDHI = "Sindhi"
+    SINHALA = "Sinhala"
+    SLOVAK = "Slovak"
+    SLOVENIAN = "Slovenian"
+    SOMALI = "Somali"
+    ALBANIAN = "Albanian"
+    SERBIAN = "Serbian"
+    SUNDANESE = "Sundanese"
+    SWEDISH = "Swedish"
+    SWAHILI = "Swahili"
+    TAMIL = "Tamil"
+    TELUGU = "Telugu"
+    THAI = "Thai"
+    TAGALOG = "Tagalog"
+    TURKISH = "Turkish"
+    UYGHUR = "Uyghur"
+    UKRAINIAN = "Ukrainian"
+    URDU = "Urdu"
+    UZBEK = "Uzbek"
+    VIETNAMESE = "Vietnamese"
+    XHOSA = "Xhosa"
+    YIDDISH = "Yiddish"
+    CHINESE = "Chinese"
+
+    @classmethod
+    def list_all_languages(cls):
+        return list(map(lambda c: c.value, cls))  # type: ignore [attr-defined]
+
+
+class VectorDatabaseChunkingParameterType(StrEnum):
+    """Chunking parameter types supported by VectorDatabases."""
+
+    INT = "int"
+    LIST_STR = "list[str]"
+
+
+class VectorDatabaseSource(StrEnum):
+    """Supported source for VectorDatabases."""
+
+    DATAROBOT = "DataRobot"
+    EXTERNAL = "External"
+
+
+class VectorDatabaseExecutionStatus(StrEnum):
+    """Execution Statuses VectorDatabases can be in."""
+
+    NEW = "NEW"
+    RUNNING = "RUNNING"
+    COMPLETED = "COMPLETED"
+    ERROR = "ERROR"
+
+
+class ListPlaygroundsSortQueryParams(StrEnum):
+    """supported Sort query params for the Playground.list method."""
+
+    NAME_ASCENDING = "name"
+    NAME_DESCENDING = "-name"
+    DESCRIPTION_ASCENDING = "description"
+    DESCRIPTION_DESCENDING = "-description"
+    CREATION_USER_DATE_ASCENDING = "creationUserId"
+    CREATION_USER_DATE_DESCENDING = "-creationUserId"
+    CREATION_DATE_ASCENDING = "creationDate"
+    CREATION_DATE_DESCENDING = "-creationDate"
+    LAST_UPDATE_USER_DATE_ASCENDING = "lastUpdateUserId"
+    LAST_UPDATE_USER_DATE_DESCENDING = "-lastUpdateUserId"
+    SAVED_LLM_BLUEPRINTS_COUNT_ASCENDING = "savedLLMBlueprintsCount"
+    SAVED_LLM_BLUEPRINTS_COUNT_DESCENDING = "-savedLLMBlueprintsCount"
+
+
+class ListChatsSortQueryParams(StrEnum):
+    """supported Sort query params for the Chat.list method."""
+
+    NAME_ASCENDING = "name"
+    NAME_DESCENDING = "-name"
+    CREATION_DATE_ASCENDING = "creationDate"
+    CREATION_DATE_DESCENDING = "-creationDate"
+
+
+class ListComparisonChatsSortQueryParams(StrEnum):
+    """supported Sort query params for the ComparisonChat.list method."""
+
+    NAME_ASCENDING = "name"
+    NAME_DESCENDING = "-name"
+    CREATION_DATE_ASCENDING = "creationDate"
+    CREATION_DATE_DESCENDING = "-creationDate"
+
+
+class ListLLMBlueprintsSortQueryParams(StrEnum):
+    """supported Sort query params for the LLMBlueprint.list method."""
+
+    NAME_ASCENDING = "name"
+    NAME_DESCENDING = "-name"
+    DESCRIPTION_ASCENDING = "description"
+    DESCRIPTION_DESCENDING = "-description"
+    CREATION_USER_DATE_ASCENDING = "creationUserId"
+    CREATION_USER_DATE_DESCENDING = "-creationUserId"
+    CREATION_DATE_ASCENDING = "creationDate"
+    CREATION_DATE_DESCENDING = "-creationDate"
+    LAST_UPDATE_USER_DATE_ASCENDING = "lastUpdateUserId"
+    LAST_UPDATE_USER_DATE_DESCENDING = "-lastUpdateUserId"
+    LAST_UPDATE_DATE_ASCENDING = "lastUpdateDate"
+    LAST_UPDATE_DATE_DESCENDING = "-lastUpdateDate"
+    LLM_ID_ASCENDING = "llmId"
+    LLM_ID_DESCENDING = "-llmId"
+    VECTOR_DATABASE_ID_ASCENDING = "vectorDatabaseId"
+    VECTOR_DATABASE_ID_DESCENDING = "-vectorDatabaseId"
+
+
+class ListCustomModelValidationsSortQueryParams(StrEnum):
+    NAME_ASCENDING = "name"
+    NAME_DESCENDING = "-name"
+    DEPLOYMENT_NAME_ASCENDING = "deploymentName"
+    DEPLOYMENT_NAME_DESCENDING = "-deploymentName"
+    USER_NAME_ASCENDING = "userName"
+    USER_NAME_DESCENDING = "-userName"
+    CREATION_DATE_ASCENDING = "creationDate"
+    CREATION_DATE_DESCENDING = "-creationDate"
+
+
+class PromptType(StrEnum):
+    """Supported LLM Blueprint prompting types."""
+
+    ONE_TIME_PROMPT = "ONE_TIME_PROMPT"
+    CHAT_HISTORY_AWARE = "CHAT_HISTORY_AWARE"
```

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/errors.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/errors.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/helpers/__init__.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/helpers/binary_data_utils.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/helpers/binary_data_utils.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/helpers/eligibility_result.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/helpers/eligibility_result.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/helpers/feature_discovery.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/helpers/feature_discovery.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/helpers/image_utils.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/helpers/image_utils.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/helpers/partitioning_methods.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/helpers/partitioning_methods.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/insights/base.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/insights/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,55 +23,56 @@
 
 class BaseInsight(APIObject, BrowserMixin):
     """Base Insight class for modern insights
 
     This class serves as a template for modern insights created using the Root Insights framework.
     It provides most necessary functions for easily implementing classes that wrap specific insights.
 
-    To use this class it should be inherited and the `INSIGHT_NAME` and `INSIGHT_DATA` attributes
-    should be replaced with the correct values.
-
-    Example:
-    You have an insight that has the endpoint `insights/myInsight` and the insight's calculator
-    produces a response that contains a boolean field called `insight_worked` and a list of
-    string values called `insight_values`.
-
-    To make things easier for the user you may want to add some easily accessible properties
-    to allow them to quickly get the values of the insight.
-
-    Example insight result:
-
-    .. code-block:: text
-
-            {
-                "insight_worked": true,
-                "insight_values": ["hello", "world"]
-            }
-
-    You can simply create a wrapper for this new insight using this framework:
-
-    .. code-block:: python
-
-            class MyInsight(BaseInsight):
-                INSIGHT_NAME = "myInsight"
-                INSIGHT_DATA = {
-                    t.Key("insight_worked"): t.Bool(),
-                    t.Key("insight_values"): t.List(t.String()),
-                }
-
-                @property
-                def values() -> List[str]:
-                    return cast(List[str], self.data["insight_values"])
-
-    All of the computation and insight retrieval handling will be accounted for by the base insight.
-    This class can also be overridden for more complex queries by adjusting the functionality of the
-    `_get_payload` function to provide additional required options, but most insights won't need
-    this capability.
     """
 
+    # To use this class it should be inherited and the `INSIGHT_NAME` and `INSIGHT_DATA` attributes
+    # should be replaced with the correct values.
+    #
+    # Example:
+    # You have an insight that has the endpoint `insights/myInsight` and the insight's calculator
+    # produces a response that contains a boolean field called `insight_worked` and a list of
+    # string values called `insight_values`.
+    #
+    # To make things easier for the user you may want to add some easily accessible properties
+    # to allow them to quickly get the values of the insight.
+    #
+    # Example insight result:
+    #
+    # .. code-block:: text
+    #
+    #         {
+    #             "insight_worked": true,
+    #             "insight_values": ["hello", "world"]
+    #         }
+    #
+    # You can simply create a wrapper for this new insight using this framework:
+    #
+    # .. code-block:: python
+    #
+    #         class MyInsight(BaseInsight):
+    #             INSIGHT_NAME = "myInsight"
+    #             INSIGHT_DATA = {
+    #                 t.Key("insight_worked"): t.Bool(),
+    #                 t.Key("insight_values"): t.List(t.String()),
+    #             }
+    #
+    #             @property
+    #             def values() -> List[str]:
+    #                 return cast(List[str], self.data["insight_values"])
+    #
+    # All of the computation and insight retrieval handling will be accounted for by the base insight.
+    # This class can also be overridden for more complex queries by adjusting the functionality of the
+    # `_get_payload` function to provide additional required options, but most insights won't need
+    # this capability.
+
     INSIGHT_NAME: str = "base"  # Defined by subclasses to identify the formal name for endpoints
     INSIGHT_DATA = t.Any()  # Defined by subclasses for specific insights
 
     _converter = t.Dict(
         {
             t.Key("id"): t.String(),
             t.Key("entity_id"): t.String(),
@@ -155,17 +156,16 @@
         cls,
         entity_id: str,
         source: str = INSIGHTS_SOURCES.VALIDATION,
         data_slice_id: Optional[str] = None,
         external_dataset_id: Optional[str] = None,
         **kwargs: Any,
     ) -> Dict[str, Union[str, int]]:
-        """Construct a payload for a compute request
-
-        May be override by insight subclasses to accept additional parameters
+        """Construct a payload for a compute request. May be overridden by insight subclasses to
+        accept additional parameters.
         """
         _ = kwargs
         payload = {
             "entityId": entity_id,
             "source": source,
         }
         if data_slice_id is not None:
@@ -181,17 +181,16 @@
         entity_id: str,
         source: str = INSIGHTS_SOURCES.VALIDATION,
         data_slice_id: Optional[str] = None,
         external_dataset_id: Optional[str] = None,
         **kwargs: Any,
     ) -> StatusCheckJob:
         """Submit an insight compute request. You can use `create` if you want to
-        wait synchronously for the completion of the job.
-
-        May be override by insight subclasses to accept additional parameters
+        wait synchronously for the completion of the job. May be overridden by insight subclasses to
+        accept additional parameters.
 
         Parameters
         ----------
         entity_id: str
             Id of the entity to compute the insight
         source: str
             Source type to use when computing the insight
@@ -222,17 +221,16 @@
         entity_id: str,
         source: str = INSIGHTS_SOURCES.VALIDATION,
         data_slice_id: Optional[str] = None,
         external_dataset_id: Optional[str] = None,
         max_wait: Optional[int] = DEFAULT_MAX_WAIT,
         **kwargs: Any,
     ) -> Self:
-        """Create an insight and wait for completion
-
-        May be override by insight subclasses to accept additional parameters
+        """Create an insight and wait for completion. May be overridden by insight subclasses to
+        accept additional parameters.
 
         Parameters
         ----------
         entity_id: str
             Id of the entity to compute the insight
         source: str
             Source type to use when computing the insight
@@ -255,15 +253,15 @@
             external_dataset_id=external_dataset_id,
             **kwargs,
         )
         return cast(Self, status_check_job.get_result_when_complete(max_wait=cast(int, max_wait)))
 
     @classmethod
     def list(cls, entity_id: str) -> List[Self]:
-        """List all generated insights
+        """List all generated insights.
 
         Parameters
         ----------
         entity_id: str
             Id of the entity to list all generated insights
 
         Returns
```

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/insights/shap_impact.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/insights/shap_impact.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,16 +14,19 @@
 import trafaret as t
 
 from datarobot.enums import INSIGHTS_SOURCES
 from datarobot.insights.base import BaseInsight
 
 
 class ShapImpact(BaseInsight):
-    """
-    Shap Impact Insight
+    """Class for SHAP Impact calculations. Use the standard methods of BaseInsight to compute and
+    retrieve SHAP matrices:
+    * compute: submit a request to compute a SHAP impact, and return immediately
+    * create: submit a request to compute a SHAP impact, and wait for it to finish
+    * list: retrieve all ShapImpact results for a model, possibly on multiple datasets or data slices.
     """
 
     INSIGHT_NAME = "shapImpact"
     INSIGHT_DATA = {
         "shap_impacts": t.List(t.List(t.Or(t.Int(), t.Float()))),
         "base_value": t.List(t.Float()),
         "capping": t.Or(
@@ -39,15 +42,15 @@
         "row_count": t.Int(),
     }
 
     @classmethod
     def _get_payload(
         cls,
         entity_id: str,
-        source: str = INSIGHTS_SOURCES.VALIDATION,
+        source: str = INSIGHTS_SOURCES.TRAINING,
         data_slice_id: Optional[str] = None,
         external_dataset_id: Optional[str] = None,
         row_count: Optional[int] = None,
         **kwargs: Any,
     ) -> Dict[str, Union[str, int]]:
         """Construct a payload for a compute request"""
         payload = super()._get_payload(
```

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/mixins/browser_mixin.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/mixins/browser_mixin.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/mixins/update_attributes_mixin.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/mixins/update_attributes_mixin.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/__init__.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # flake8: noqa
 # because the unused imports are on purpose
 
+import datarobot.models.genai
 import datarobot.models.registry
 
 from .application import Application
 from .automated_documentation import AutomatedDocument
 from .batch_monitoring_job import BatchMonitoringJob, BatchMonitoringJobDefinition
 from .batch_prediction_job import BatchPredictionJob, BatchPredictionJobDefinition
 from .blueprint import Blueprint, BlueprintChart, BlueprintTaskDocument, ModelBlueprintChart
@@ -61,15 +62,14 @@
     FeatureEffectMetadata,
     FeatureEffectMetadataDatetime,
     FeatureEffectMetadataDatetimePerBacktest,
     FeatureEffects,
     FeatureEffectsMulticlass,
 )
 from .featurelist import DatasetFeaturelist, Featurelist, ModelingFeaturelist
-from .imported_model import ImportedModel
 from .job import FeatureImpactJob, Job, TrainingPredictionsJob
 from .key_values import KeyValue
 from .model import (
     BlenderModel,
     ClusteringModel,
     CombinedModel,
     DatetimeModel,
```

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/advanced_tuning.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/advanced_tuning.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/anomaly_assessment.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/anomaly_assessment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/api_object.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/api_object.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/application.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/application.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/automated_documentation.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/automated_documentation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/batch_job.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/batch_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/batch_monitoring_job.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/batch_monitoring_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/batch_prediction_job.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/batch_prediction_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/blueprint.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/blueprint.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/calendar_file.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/calendar_file.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/change_request.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/change_request.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/cluster.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/cluster.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/cluster_insight.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/cluster_insight.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/compliance_doc_template.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/compliance_doc_template.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/confusion_chart.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/confusion_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/connector.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/connector.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/credential.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/credential.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/custom_model.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/custom_model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/custom_model_test.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/custom_model_test.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/custom_model_version.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/custom_model_version.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/custom_task.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/custom_task.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/custom_task_version.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/custom_task_version.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/custom_task_version_dependency_build.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/custom_task_version_dependency_build.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/data_engine_query_generator.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/data_engine_query_generator.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/data_slice.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/data_slice.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/data_source.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/data_source.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/data_store.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/data_store.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/dataset.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/datetime_trend_plots.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/datetime_trend_plots.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/__init__.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/accuracy.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/accuracy.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/bias_and_fairness.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/bias_and_fairness.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/challenger.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/challenger.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/champion_model_package.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/champion_model_package.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/custom_metrics.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/custom_metrics.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/data_drift.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/data_drift.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/data_exports.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/data_exports.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/deployment.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/deployment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/mixins.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/mixins.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/service_stats.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/service_stats.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/deployment/sharing.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/sharing.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/documentai/document.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/documentai/document.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/driver.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/driver.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/execution_environment.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/execution_environment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/execution_environment_version.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/execution_environment_version.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/external_baseline_validation.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_baseline_validation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/external_dataset_scores_insights/external_lift_chart.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/external_lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/external_dataset_scores_insights/external_roc_curve.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/external_roc_curve.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/external_dataset_scores_insights/external_scores.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/external_scores.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/feature.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/feature_association_matrix/feature_association_featurelists.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature_association_matrix/feature_association_featurelists.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/feature_association_matrix/feature_association_matrix.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature_association_matrix/feature_association_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/feature_association_matrix/feature_association_matrix_details.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature_association_matrix/feature_association_matrix_details.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/feature_effect.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature_effect.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/feature_impact.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature_impact.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/featurelist.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/featurelist.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/imported_model.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/sharing.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,212 +7,195 @@
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
 from __future__ import annotations
 
-from datetime import datetime
-import os
-from typing import List, Optional
+from typing import Optional, TYPE_CHECKING
 
 import trafaret as t
 
 from datarobot._compat import String
-from datarobot.utils.waiters import wait_for_async_resolution
+from datarobot.enums import SHARING_RECIPIENT_TYPE, SHARING_ROLE
+from datarobot.errors import InvalidUsageError
+from datarobot.models.api_object import APIObject
+
+if TYPE_CHECKING:
+    from mypy_extensions import TypedDict
+
+    class SharingAccessPayload(TypedDict, total=False):
+        username: str
+        role: str
+        can_share: bool
+        can_use_data: bool
+
+    class SharingRolePayload(TypedDict, total=False):
+        id: Optional[str]
+        role: SHARING_ROLE
+        share_recipient_type: SHARING_RECIPIENT_TYPE
+        username: Optional[str]
+        can_share: Optional[bool]
+
+
+class SharingAccess(APIObject):
+    """Represents metadata about whom a entity (e.g. a data store) has been shared with
+
+    .. versionadded:: v2.14
+
+    Currently :py:class:`DataStores <datarobot.DataStore>`,
+    :py:class:`DataSources <datarobot.DataSource>`,
+    :py:class:`Datasets <datarobot.models.Dataset>`,
+    :py:class:`Projects <datarobot.models.Project>` (new in version v2.15) and
+    :py:class:`CalendarFiles <datarobot.CalendarFile>` (new in version 2.15) can be shared.
 
-from ..enums import DEFAULT_MAX_WAIT, DEFAULT_TIMEOUT
-from ..utils import parse_time
-from .api_object import APIObject
-
-
-class ImportedModel(APIObject):
-    """
-    Represents an imported model available for making predictions. These are only relevant for
-    administrators of on-premise Stand Alone Scoring Engines.
-
-    ImportedModels are trained in one DataRobot application, exported as a `.drmodel` file, and
-    then imported for use in a Stand Alone Scoring Engine.
+    This class can represent either access that has already been granted, or be used to grant access
+    to additional users.
 
     Attributes
     ----------
-    id : str
-        id of the import
-    model_name : str
-        model type describing the model generated by DataRobot
-    display_name : str
-        manually specified human-readable name of the imported model
-    note : str
-        manually added node about this imported model
-    imported_at : datetime
-        the time the model was imported
-    imported_by_username : str
-        username of the user who imported the model
-    imported_by_id : str
-        id of the user who imported the model
-    origin_url : str
-        URL of the application the model was exported from
-    model_id : str
-        original id of the model prior to export
-    featurelist_name : str
-        name of the featurelist used to train the model
-    project_id : str
-         id of the project the model belonged to prior to export
-    project_name : str
-        name of the project the model belonged to prior to export
-    target : str
-        the target of the project the model belonged to prior to export
-    dataset_name : str
-        filename of the dataset used to create the project the model belonged to
-    created_by_username : str
-        username of the user who created the model prior to export
-    created_by_id : str
-        id of the user who created the model prior to export
+    username : str
+        a particular user
+    role : str or None
+        if a string, represents a particular level of access and should be one of
+        ``datarobot.enums.SHARING_ROLE``.  For more information on the specific access levels, see
+        the :ref:`sharing <sharing>` documentation.  If None, can be passed to a `share`
+        function to revoke access for a specific user.
+    can_share : bool or None
+        if a bool, indicates whether this user is permitted to further share.  When False, the
+        user has access to the entity, but can only revoke their own access but not modify any
+        user's access role.  When True, the user can share with any other user at a access role up
+        to their own.  May be None if the SharingAccess was not retrieved from the DataRobot server
+        but intended to be passed into a `share` function; this will be equivalent to passing True.
+    can_use_data : bool or None
+        if a bool, indicates whether this user should be able to view, download and process data
+        (use to create projects, predictions, etc). For OWNER can_use_data is always True. If role
+        is empty canUseData is ignored.
+    user_id : str or None
+        the id of the user
     """
 
-    _root_path = "importedModels/"
     _converter = t.Dict(
         {
-            t.Key("id"): String,
-            t.Key("imported_at"): parse_time,
-            t.Key("model_id"): String,
-            t.Key("target"): String,
-            t.Key("featurelist_name"): String,
-            t.Key("dataset_name"): String,
-            t.Key("model_name"): String,
-            t.Key("project_id"): String,
-            t.Key("note", optional=True, default=None): t.Or(
-                String, t.Null
-            ),  # from_api strips None
-            t.Key("origin_url"): String,
-            t.Key("imported_by_username"): String,
-            t.Key("project_name"): String,
-            t.Key("created_by_username"): String,
-            t.Key("created_by_id"): String,
-            t.Key("imported_by_id"): String,
-            t.Key("display_name"): String,
+            t.Key("username"): String,
+            t.Key("role"): String,
+            t.Key("can_share", default=None): t.Or(t.Bool, t.Null),
+            t.Key("can_use_data", default=None): t.Or(t.Bool, t.Null),
+            t.Key("user_id", default=None): t.Or(String, t.Null),
         }
-    ).allow_extra("*")
+    ).ignore_extra("*")
 
     def __init__(
         self,
-        id: str,
-        imported_at: Optional[datetime] = None,
-        model_id: Optional[str] = None,
-        target: Optional[str] = None,
-        featurelist_name: Optional[str] = None,
-        dataset_name: Optional[str] = None,
-        model_name: Optional[str] = None,
-        project_id: Optional[str] = None,
-        note: Optional[str] = None,
-        origin_url: Optional[str] = None,
-        imported_by_username: Optional[str] = None,
-        project_name: Optional[str] = None,
-        created_by_username: Optional[str] = None,
-        created_by_id: Optional[str] = None,
-        imported_by_id: Optional[str] = None,
-        display_name: Optional[str] = None,
+        username: str,
+        role: str,
+        can_share: Optional[bool] = None,
+        can_use_data: Optional[bool] = None,
+        user_id: Optional[str] = None,
     ) -> None:
-
-        self.id = id
-        self.imported_at = imported_at
-        self.model_id = model_id
-        self.target = target
-        self.featurelist_name = featurelist_name
-        self.dataset_name = dataset_name
-        self.model_name = model_name
-        self.project_id = project_id
-        self.note = note
-        self.origin_url = origin_url
-        self.imported_by_username = imported_by_username
-        self.project_name = project_name
-        self.created_by_username = created_by_username
-        self.created_by_id = created_by_id
-        self.imported_by_id = imported_by_id
-        self.display_name = display_name
-
-        self._path = self._get_path(id)
-
-    @classmethod
-    def create(cls, path: str, max_wait: int = DEFAULT_MAX_WAIT) -> ImportedModel:
-        """Import a previously exported model for predictions.
-
-        Parameters
-        ----------
-        path : str
-            The path to the exported model file
-        max_wait : int, optional
-            Time in seconds after which model import is considered unsuccessful
-        """
-        name = os.path.split(path)[1]
-        response = cls._client.build_request_with_file(
-            "post", cls._root_path, name, file_path=path, read_timeout=DEFAULT_TIMEOUT.UPLOAD
+        self.username = username
+        self.role = role
+        self.can_share = can_share
+        self.can_use_data = can_use_data
+        self.user_id = user_id
+
+    def __repr__(self) -> str:
+        return (
+            "{cls}(username: {username}, role: {role}, "
+            "can_share: {can_share}, can_use_data: {can_use_data}, user_id: {user_id})"
+        ).format(
+            cls=self.__class__.__name__,
+            username=self.username,
+            role=self.role,
+            can_share=self.can_share,
+            can_use_data=self.can_use_data,
+            user_id=self.user_id,
         )
-        async_loc = response.headers["Location"]
-        imported_model_loc = wait_for_async_resolution(cls._client, async_loc, max_wait=max_wait)
-        return cls.from_location(imported_model_loc)
-
-    @classmethod
-    def _get_path(cls, id: str) -> str:
-        return f"{cls._root_path}{id}/"
-
-    @classmethod
-    def get(cls, import_id: str) -> ImportedModel:
-        """Retrieve imported model info
-
-        Parameters
-        ----------
-        import_id : str
-            The ID of the imported model.
+
+    def collect_payload(self) -> SharingAccessPayload:
+        """Set up the dict that should be sent to the server in order to share this
 
         Returns
         -------
-        imported_model : ImportedModel
-            The ImportedModel instance
+        payload : dict
         """
-        path = f"{cls._root_path}{import_id}/"
-        return cls.from_location(path)
+        payload: SharingAccessPayload = {"username": self.username, "role": self.role}
+        if self.can_share is not None:
+            payload["can_share"] = self.can_share
+        if self.can_use_data is not None:
+            payload["can_use_data"] = self.can_use_data
+        return payload
 
-    @classmethod
-    def list(cls, limit: Optional[int] = None, offset: Optional[int] = None) -> List[ImportedModel]:
-        """
-        List the imported models.
 
-        Parameters
-        ----------
-        limit : int
-            The number of records to return. The server will use a (possibly finite) default if not
-            specified.
-        offset : int
-            The number of records to skip.
+class SharingRole(APIObject):
+    """
+    Represents metadata about a user who has been granted access to an entity.
+    At least one of `id` or `username` must be set.
 
+    Attributes
+    ----------
+    id : str or None
+        The ID of the user.
+    role : str
+        Represents a particular level of access. Should be one of
+        ``datarobot.enums.SHARING_ROLE``.
+    share_recipient_type : SHARING_RECIPIENT_TYPE
+        The type of user for the object of the method. Can be ``user`` or ``organization``.
+    user_full_name : str or None
+        The full name of the user.
+    username : str or None
+        The username (usually the email) of the user.
+    can_share : bool or None
+        Indicates whether this user is permitted to share with other users. When False, the
+        user has access to the entity, but can only revoke their own access. They cannot not modify
+        any user's access role. When True, the user can share with any other user at an access
+        role up to their own.
+    """
 
-        Returns
-        -------
-        imported_models : list[ImportedModel]
-        """
-        r_data = cls._client.get(cls._root_path, params={"limit": limit, "offset": offset}).json()
-        return [cls.from_server_data(item) for item in r_data["data"]]
+    _converter = t.Dict(
+        {
+            t.Key("id", optional=True): t.String,
+            t.Key("user_full_name", optional=True): t.String,
+            t.Key("name", optional=True) >> "username": t.String,
+            t.Key("role"): t.String,
+            t.Key("share_recipient_type"): t.String,
+            t.Key("can_share", optional=True, default=None): t.Or(t.Bool, t.Null),
+        }
+    ).ignore_extra("*")
 
-    def update(self, display_name: Optional[str] = None, note: Optional[str] = None) -> None:
-        """
-        Update the display name or note for an imported model. The ImportedModel object is updated
-        in place.
+    def __init__(
+        self,
+        role: SHARING_ROLE,
+        share_recipient_type: SHARING_RECIPIENT_TYPE,
+        can_share: Optional[bool] = None,
+        id: Optional[str] = None,
+        user_full_name: Optional[str] = None,
+        username: Optional[str] = None,
+    ):
+        if not id and not username:
+            raise InvalidUsageError("Please include either a username or an ID of a user.")
+        self.id = id
+        self.user_full_name = user_full_name
+        self.role = SHARING_ROLE[role]
+        self.share_recipient_type = share_recipient_type
+        self.username = username
+        self.can_share = can_share
 
-        Parameters
-        ----------
-        display_name : str
-            The new display name.
-        note : str
-            The new note.
+    def collect_payload(self) -> SharingRolePayload:
         """
-        self._client.patch(self._path, data={"display_name": display_name, "note": note})
-        if display_name:  # Following pattern from Project.update. (Arguably technical debt.)
-            self.display_name = display_name
-        if note:
-            self.note = note
+        Generate a dictionary representation of this SharingRole.
 
-    def delete(self) -> None:
-        """
-        Delete this imported model.
+        Returns
+        -------
+        formatted_role : SharingRolePayload
+            A dictionary representation of this SharingRole ready for sending to DataRobot.
         """
-        self._client.delete(self._path)
+        formatted_role: SharingRolePayload = {
+            "role": self.role,
+            "share_recipient_type": self.share_recipient_type,
+            "can_share": self.can_share,
+        }
+        if self.id:
+            formatted_role["id"] = self.id
+        if self.username:
+            formatted_role["username"] = self.username
+        return formatted_role
```

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/job.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/key_values.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/key_values.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/lift_chart.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/missing_report.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/missing_report.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/model.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1676,79 +1676,14 @@
         -------
         rulesets : list of Ruleset
         """
         url = f"projects/{self.project_id}/models/{self.id}/primeRulesets/"
         response = self._client.get(url).json()
         return [Ruleset.from_server_data(data) for data in response]
 
-    def download_export(self, filepath: str) -> None:
-        """
-        Download an exportable model file for use in an on-premise DataRobot standalone
-        prediction environment.
-
-        This function can only be used if model export is enabled, and will only be useful
-        if you have an on-premise environment in which to import it.
-
-        Parameters
-        ----------
-        filepath : str
-            The path at which to save the exported model file.
-        """
-        url = f"{self._base_model_path}{self.id}/export/"
-        response = self._client.get(url)
-        with open(filepath, mode="wb") as out_file:
-            out_file.write(response.content)
-
-    def request_transferable_export(self, prediction_intervals_size: Optional[int] = None) -> Job:
-        """
-        Request generation of an exportable model file for use in an on-premise DataRobot standalone
-        prediction environment.
-
-        This function can only be used if model export is enabled, and will only be useful
-        if you have an on-premise environment in which to import it.
-
-        This function does not download the exported file. Use download_export for that.
-
-        Parameters
-        ----------
-        prediction_intervals_size : int, optional
-            (New in v2.19) For :ref:`time series <time_series>` projects only.
-            Represents the percentile to use for the size of the prediction intervals. Prediction
-            intervals size must be between 1 and 100 (inclusive).
-
-        Returns
-        -------
-        Job
-
-        Examples
-        --------
-        .. code-block:: python
-
-            model = datarobot.Model.get('project-id', 'model-id')
-            job = model.request_transferable_export()
-            job.wait_for_completion()
-            model.download_export('my_exported_model.drmodel')
-
-            # Client must be configured to use standalone prediction server for import:
-            datarobot.Client(token='my-token-at-standalone-server',
-                             endpoint='standalone-server-url/api/v2')
-
-            imported_model = datarobot.ImportedModel.create('my_exported_model.drmodel')
-
-        """
-        from .job import Job  # pylint: disable=import-outside-toplevel,cyclic-import
-
-        url = "modelExports/"
-        payload = {"project_id": self.project_id, "model_id": self.id}
-        if prediction_intervals_size:
-            payload.update({"percentile": prediction_intervals_size})
-        response = self._client.post(url, data=payload)
-        job_id = get_id_from_response(response)
-        return Job.get(self.project_id, job_id)
-
     def request_frozen_model(
         self, sample_pct: Optional[float] = None, training_row_count: Optional[int] = None
     ) -> ModelJob:
         """
         Train a new frozen model with parameters from this model
 
         .. note::
```

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/model_registry/deployment.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/model_registry/deployment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/model_registry/registered_model.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/model_registry/registered_model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/model_registry/registered_model_version.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/model_registry/registered_model_version.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/modeljob.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/modeljob.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/pairwise_statistics.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/pairwise_statistics.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/pareto_front.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/pareto_front.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/payoff_matrix.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/payoff_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/predict_job.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/predict_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/prediction_dataset.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/prediction_dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/prediction_environment.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/prediction_environment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/prediction_explanations.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/prediction_explanations.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/prediction_server.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/prediction_server.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/predictions.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/predictions.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/prime_file.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/prime_file.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/project.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/project.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/project_options.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/project_options.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/rating_table.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/rating_table.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/recommended_model.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/recommended_model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/registry/job.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/registry/job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/registry/job_run.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/registry/job_run.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/relationships_configuration.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/relationships_configuration.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/residuals.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/residuals.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/restore_discarded_features.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/restore_discarded_features.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/roc_curve.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/roc_curve.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/ruleset.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/ruleset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/runtime_parameters.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/runtime_parameters.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/secondary_dataset.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/secondary_dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/segmentation.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/segmentation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/shap_impact.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/shap_impact.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/shap_matrix.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/shap_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/shap_matrix_job.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/shap_matrix_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/status_check_job.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/status_check_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/trafarets.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/trafarets.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/training_predictions.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/training_predictions.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/types.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/types.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/use_cases/use_case.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/use_cases/use_case.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/use_cases/utils.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/use_cases/utils.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/user_blueprints/models.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/user_blueprints/models.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/user_blueprints/trafarets.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/user_blueprints/trafarets.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/validators.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/validators.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/visualai/augmentation.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/visualai/augmentation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/visualai/images.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/visualai/images.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/visualai/insights.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/visualai/insights.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/models/word_cloud.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/word_cloud.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/rest.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/rest.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/utils/__init__.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/utils/deprecation.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/utils/pagination.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/utils/retry.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/retry.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/utils/source.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/source.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/utils/sourcedata.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/sourcedata.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot/utils/waiters.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/waiters.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot_early_access.egg-info/PKG-INFO` & `datarobot_early_access-3.5.0.2024.5.6/datarobot_early_access.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarobot-early-access
-Version: 3.4.0.2024.4.8
+Version: 3.5.0.2024.5.6
 Summary: This client library is designed to support the DataRobot API.
 Home-page: https://datarobot.com
 Author: datarobot
 Author-email: support@datarobot.com
 Maintainer: datarobot
 Maintainer-email: info@datarobot.com
 License: DataRobot Tool and Utility Agreement
```

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot_early_access.egg-info/SOURCES.txt` & `datarobot_early_access-3.5.0.2024.5.6/datarobot_early_access.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -34,20 +34,25 @@
 datarobot/_experimental/models/recipes.py
 datarobot/_experimental/models/retraining.py
 datarobot/_experimental/models/genai/__init__.py
 datarobot/_experimental/models/genai/chat.py
 datarobot/_experimental/models/genai/chat_prompt.py
 datarobot/_experimental/models/genai/comparison_chat.py
 datarobot/_experimental/models/genai/comparison_prompt.py
+datarobot/_experimental/models/genai/cost_metric_configurations.py
 datarobot/_experimental/models/genai/custom_model_llm_validation.py
-datarobot/_experimental/models/genai/custom_model_validation.py
+datarobot/_experimental/models/genai/evaluation_dataset_configuration.py
+datarobot/_experimental/models/genai/evaluation_dataset_metric_aggregation.py
+datarobot/_experimental/models/genai/insights_configuration.py
 datarobot/_experimental/models/genai/llm.py
 datarobot/_experimental/models/genai/llm_blueprint.py
 datarobot/_experimental/models/genai/playground.py
 datarobot/_experimental/models/genai/prompt_trace.py
+datarobot/_experimental/models/genai/sidecar_model_metric.py
+datarobot/_experimental/models/genai/synthetic_evaluation_dataset_generation.py
 datarobot/_experimental/models/genai/user_limits.py
 datarobot/_experimental/models/genai/vector_database.py
 datarobot/helpers/__init__.py
 datarobot/helpers/binary_data_utils.py
 datarobot/helpers/eligibility_result.py
 datarobot/helpers/feature_discovery.py
 datarobot/helpers/image_utils.py
@@ -94,15 +99,14 @@
 datarobot/models/execution_environment.py
 datarobot/models/execution_environment_version.py
 datarobot/models/external_baseline_validation.py
 datarobot/models/feature.py
 datarobot/models/feature_effect.py
 datarobot/models/feature_impact.py
 datarobot/models/featurelist.py
-datarobot/models/imported_model.py
 datarobot/models/job.py
 datarobot/models/key_values.py
 datarobot/models/lift_chart.py
 datarobot/models/missing_report.py
 datarobot/models/model.py
 datarobot/models/modeljob.py
 datarobot/models/pairwise_statistics.py
@@ -158,14 +162,26 @@
 datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
 datarobot/models/external_dataset_scores_insights/external_roc_curve.py
 datarobot/models/external_dataset_scores_insights/external_scores.py
 datarobot/models/feature_association_matrix/__init__.py
 datarobot/models/feature_association_matrix/feature_association_featurelists.py
 datarobot/models/feature_association_matrix/feature_association_matrix.py
 datarobot/models/feature_association_matrix/feature_association_matrix_details.py
+datarobot/models/genai/__init__.py
+datarobot/models/genai/chat.py
+datarobot/models/genai/chat_prompt.py
+datarobot/models/genai/comparison_chat.py
+datarobot/models/genai/comparison_prompt.py
+datarobot/models/genai/custom_model_llm_validation.py
+datarobot/models/genai/custom_model_validation.py
+datarobot/models/genai/llm.py
+datarobot/models/genai/llm_blueprint.py
+datarobot/models/genai/playground.py
+datarobot/models/genai/user_limits.py
+datarobot/models/genai/vector_database.py
 datarobot/models/model_registry/__init__.py
 datarobot/models/model_registry/common.py
 datarobot/models/model_registry/deployment.py
 datarobot/models/model_registry/registered_model.py
 datarobot/models/model_registry/registered_model_version.py
 datarobot/models/registry/__init__.py
 datarobot/models/registry/job.py
```

### Comparing `datarobot_early_access-3.4.0.2024.4.8/datarobot_early_access.egg-info/requires.txt` & `datarobot_early_access-3.5.0.2024.5.6/datarobot_early_access.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/pyproject.toml` & `datarobot_early_access-3.5.0.2024.5.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/setup.py` & `datarobot_early_access-3.5.0.2024.5.6/setup.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.4.8/setup_weekly.py` & `datarobot_early_access-3.5.0.2024.5.6/setup_weekly.py`

 * *Files identical despite different names*

