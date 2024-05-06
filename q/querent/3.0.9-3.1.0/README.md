# Comparing `tmp/querent-3.0.9.tar.gz` & `tmp/querent-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "querent-3.0.9.tar", last modified: Sat May  4 17:16:42 2024, max compression
+gzip compressed data, was "querent-3.1.0.tar", last modified: Mon May  6 16:58:17 2024, max compression
```

## Comparing `querent-3.0.9.tar` & `querent-3.1.0.tar`

### file list

```diff
@@ -1,261 +1,261 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.203027 querent-3.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-05-04 17:12:08.000000 querent-3.0.9/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)    16923 2024-05-04 17:16:42.203027 querent-3.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12233 2024-05-04 17:12:08.000000 querent-3.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.131027 querent-3.0.9/querent/
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-04 17:12:08.000000 querent-3.0.9/querent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.131027 querent-3.0.9/querent/callback/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-04 17:12:08.000000 querent-3.0.9/querent/callback/event_callback_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-04 17:12:08.000000 querent-3.0.9/querent/callback/event_callback_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.131027 querent-3.0.9/querent/channel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-04 17:12:08.000000 querent-3.0.9/querent/channel/channel_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.135027 querent-3.0.9/querent/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.135027 querent-3.0.9/querent/collectors/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.135027 querent-3.0.9/querent/collectors/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/aws/aws_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.135027 querent-3.0.9/querent/collectors/azure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/azure/azure_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/collector_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/collector_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/collector_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/collector_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.135027 querent-3.0.9/querent/collectors/drive/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/drive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/drive/google_drive_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.139027 querent-3.0.9/querent/collectors/dropbox/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/dropbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/dropbox/dropbox_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.139027 querent-3.0.9/querent/collectors/email/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/email/email_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/email/imap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.139027 querent-3.0.9/querent/collectors/fs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/fs/fs_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.139027 querent-3.0.9/querent/collectors/gcs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/gcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/gcs/gcs_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.143027 querent-3.0.9/querent/collectors/github/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/github/github_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.143027 querent-3.0.9/querent/collectors/jira/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/jira/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/jira/jira_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.143027 querent-3.0.9/querent/collectors/news/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/news/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/news/news_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.143027 querent-3.0.9/querent/collectors/slack/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/slack/slack_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.143027 querent-3.0.9/querent/collectors/webscaper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/webscaper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-04 17:12:08.000000 querent-3.0.9/querent/collectors/webscaper/web_scraper_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.147027 querent-3.0.9/querent/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/common_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.147027 querent-3.0.9/querent/common/errors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/errors/metric_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.155027 querent-3.0.9/querent/common/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/types/collected_bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/types/collector_config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/types/config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/types/engine_config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/types/file_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/types/ingested_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/types/ingested_images.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/types/ingested_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/types/ingested_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/types/ingested_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/types/querent_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/types/querent_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/types/resource_config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/types/workflow_config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-04 17:12:08.000000 querent-3.0.9/querent/common/uri.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.155027 querent-3.0.9/querent/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.155027 querent-3.0.9/querent/config/collector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/collector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13454 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/collector/collector_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.155027 querent-3.0.9/querent/config/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/core/gpt_llm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/core/llm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/core/opensource_llm_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.155027 querent-3.0.9/querent/config/engine/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/engine/engine_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/graph_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.159027 querent-3.0.9/querent/config/ingestor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/ingestor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/ingestor/ingestor_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.159027 querent-3.0.9/querent/config/logger/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/logger/logger_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.159027 querent-3.0.9/querent/config/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/metric/prometheus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.159027 querent-3.0.9/querent/config/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/resource/resource_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.159027 querent-3.0.9/querent/config/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-04 17:12:08.000000 querent-3.0.9/querent/config/workflow/workflow_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.159027 querent-3.0.9/querent/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/controllers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.159027 querent-3.0.9/querent/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12319 2024-05-04 17:12:08.000000 querent-3.0.9/querent/core/base_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.163027 querent-3.0.9/querent/core/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/core/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18047 2024-05-04 17:12:08.000000 querent-3.0.9/querent/core/transformers/bert_ner_opensourcellm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10072 2024-05-04 17:12:08.000000 querent-3.0.9/querent/core/transformers/fixed_entities_set_opensourcellm.py
--rw-r--r--   0 runner    (1001) docker     (127)    18879 2024-05-04 17:12:08.000000 querent-3.0.9/querent/core/transformers/gpt_llm_bert_ner_or_fixed_entities_set_ner.py
--rw-r--r--   0 runner    (1001) docker     (127)    13098 2024-05-04 17:12:08.000000 querent-3.0.9/querent/core/transformers/gpt_llm_gpt_ner.py
--rw-r--r--   0 runner    (1001) docker     (127)    10137 2024-05-04 17:12:08.000000 querent-3.0.9/querent/core/transformers/relationship_extraction_llm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.163027 querent-3.0.9/querent/dal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/dal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.163027 querent-3.0.9/querent/gnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/gnn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.167027 querent-3.0.9/querent/graph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-04 17:12:08.000000 querent-3.0.9/querent/graph/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-05-04 17:12:08.000000 querent-3.0.9/querent/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-05-04 17:12:08.000000 querent-3.0.9/querent/graph/graph_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-04 17:12:08.000000 querent-3.0.9/querent/graph/ontology.py
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-04 17:12:08.000000 querent-3.0.9/querent/graph/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-05-04 17:12:08.000000 querent-3.0.9/querent/graph/shacl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-05-04 17:12:08.000000 querent-3.0.9/querent/graph/subject.py
--rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-05-04 17:12:08.000000 querent-3.0.9/querent/graph/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.167027 querent-3.0.9/querent/ingestors/
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.171027 querent-3.0.9/querent/ingestors/audio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/audio/audio_ingestors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/base_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.171027 querent-3.0.9/querent/ingestors/code/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/code/code_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.171027 querent-3.0.9/querent/ingestors/csv/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/csv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/csv/csv_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.171027 querent-3.0.9/querent/ingestors/doc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/doc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7983 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/doc/doc_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.171027 querent-3.0.9/querent/ingestors/email/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8651 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/email/email_ingestor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/email/email_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.171027 querent-3.0.9/querent/ingestors/github/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/github/github_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.175027 querent-3.0.9/querent/ingestors/html/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/html/html_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.175027 querent-3.0.9/querent/ingestors/images/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/images/image_ingestor.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/ingestor_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8332 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/ingestor_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.175027 querent-3.0.9/querent/ingestors/json/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/json/json_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.175027 querent-3.0.9/querent/ingestors/pdfs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/pdfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8423 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/pdfs/pdf_ingestor_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.175027 querent-3.0.9/querent/ingestors/ppt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/ppt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/ppt/ppt_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.175027 querent-3.0.9/querent/ingestors/texts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/texts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/texts/text_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.179027 querent-3.0.9/querent/ingestors/video/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/video/video_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.179027 querent-3.0.9/querent/ingestors/xlsx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/xlsx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/xlsx/xlsx_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.179027 querent-3.0.9/querent/ingestors/xml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-04 17:12:08.000000 querent-3.0.9/querent/ingestors/xml/xml_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.179027 querent-3.0.9/querent/kg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.183027 querent-3.0.9/querent/kg/ner_helperfunctions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/ner_helperfunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/ner_helperfunctions/attn_scores.py
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/ner_helperfunctions/contextual_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/ner_helperfunctions/dependency_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/ner_helperfunctions/filter_triples.py
--rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/ner_helperfunctions/fixed_entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/ner_helperfunctions/fixed_predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)    18240 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/ner_helperfunctions/ner_llm_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/querent_kg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.187027 querent-3.0.9/querent/kg/rel_helperfunctions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/rel_helperfunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/rel_helperfunctions/contextual_predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/rel_helperfunctions/embedding_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/rel_helperfunctions/fixed_relationships.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/rel_helperfunctions/gpt_pydantic_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/rel_helperfunctions/opeai_ratelimiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/rel_helperfunctions/openai_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/rel_helperfunctions/openllm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/rel_helperfunctions/questionanswer_llama2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/rel_helperfunctions/rel_normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-04 17:12:08.000000 querent-3.0.9/querent/kg/rel_helperfunctions/triple_to_json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.191027 querent-3.0.9/querent/logging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-04 17:12:08.000000 querent-3.0.9/querent/logging/custom_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-04 17:12:08.000000 querent-3.0.9/querent/logging/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-04 17:12:08.000000 querent-3.0.9/querent/logging/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-04 17:12:08.000000 querent-3.0.9/querent/logging/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.191027 querent-3.0.9/querent/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/metric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.191027 querent-3.0.9/querent/metric/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/metric/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-04 17:12:08.000000 querent-3.0.9/querent/metric/adapters/promethus_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-04 17:12:08.000000 querent-3.0.9/querent/metric/base_metric_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-04 17:12:08.000000 querent-3.0.9/querent/metric/metric_logging_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-04 17:12:08.000000 querent-3.0.9/querent/metric/metric_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.195027 querent-3.0.9/querent/processors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-04 17:12:08.000000 querent-3.0.9/querent/processors/async_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-04 17:12:08.000000 querent-3.0.9/querent/processors/text_cleanup_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-04 17:12:08.000000 querent-3.0.9/querent/processors/text_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.199027 querent-3.0.9/querent/querent/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/querent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-05-04 17:12:08.000000 querent-3.0.9/querent/querent/auto_scaler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-04 17:12:08.000000 querent-3.0.9/querent/querent/querent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-04 17:12:08.000000 querent-3.0.9/querent/querent/resource_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/querent/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.199027 querent-3.0.9/querent/storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-04 17:12:08.000000 querent-3.0.9/querent/storage/gcs_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-04 17:12:08.000000 querent-3.0.9/querent/storage/milvus_vectorevent_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-04 17:12:08.000000 querent-3.0.9/querent/storage/neo4j_graphevent_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-04 17:12:08.000000 querent-3.0.9/querent/storage/postgres_graphevent_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.199027 querent-3.0.9/querent/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10882 2024-05-04 17:12:08.000000 querent-3.0.9/querent/tools/web_page_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.199027 querent-3.0.9/querent/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:12:08.000000 querent-3.0.9/querent/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-05-04 17:12:08.000000 querent-3.0.9/querent/utils/webpage_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.203027 querent-3.0.9/querent/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-04 17:12:08.000000 querent-3.0.9/querent/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7164 2024-05-04 17:12:08.000000 querent-3.0.9/querent/workflow/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-05-04 17:12:08.000000 querent-3.0.9/querent/workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:16:42.203027 querent-3.0.9/querent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16923 2024-05-04 17:16:42.000000 querent-3.0.9/querent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7202 2024-05-04 17:16:42.000000 querent-3.0.9/querent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 17:16:42.000000 querent-3.0.9/querent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-04 17:16:42.000000 querent-3.0.9/querent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-04 17:16:42.000000 querent-3.0.9/querent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 17:16:42.203027 querent-3.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-04 17:12:08.000000 querent-3.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.601502 querent-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-05-06 16:53:38.000000 querent-3.1.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)    16923 2024-05-06 16:58:17.601502 querent-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12233 2024-05-06 16:53:38.000000 querent-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.533502 querent-3.1.0/querent/
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-06 16:53:38.000000 querent-3.1.0/querent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.533502 querent-3.1.0/querent/callback/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/callback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-06 16:53:38.000000 querent-3.1.0/querent/callback/event_callback_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-06 16:53:38.000000 querent-3.1.0/querent/callback/event_callback_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.533502 querent-3.1.0/querent/channel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-06 16:53:38.000000 querent-3.1.0/querent/channel/channel_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.537502 querent-3.1.0/querent/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.537502 querent-3.1.0/querent/collectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.537502 querent-3.1.0/querent/collectors/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/aws/aws_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.537502 querent-3.1.0/querent/collectors/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/azure/azure_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/collector_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/collector_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/collector_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/collector_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.537502 querent-3.1.0/querent/collectors/drive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/drive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/drive/google_drive_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.541502 querent-3.1.0/querent/collectors/dropbox/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/dropbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/dropbox/dropbox_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.541502 querent-3.1.0/querent/collectors/email/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/email/email_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/email/imap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.541502 querent-3.1.0/querent/collectors/fs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/fs/fs_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.541502 querent-3.1.0/querent/collectors/gcs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/gcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/gcs/gcs_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.541502 querent-3.1.0/querent/collectors/github/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/github/github_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.541502 querent-3.1.0/querent/collectors/jira/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/jira/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/jira/jira_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.545502 querent-3.1.0/querent/collectors/news/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/news/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/news/news_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.545502 querent-3.1.0/querent/collectors/slack/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/slack/slack_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.545502 querent-3.1.0/querent/collectors/webscaper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/webscaper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/webscaper/web_scraper_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.545502 querent-3.1.0/querent/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/common_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.545502 querent-3.1.0/querent/common/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/errors/metric_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.553502 querent-3.1.0/querent/common/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/types/collected_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/types/collector_config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/types/config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/types/engine_config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/types/file_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/types/ingested_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/types/ingested_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/types/ingested_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/types/ingested_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/types/ingested_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/types/querent_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/types/querent_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/types/resource_config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/types/workflow_config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/uri.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.553502 querent-3.1.0/querent/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.553502 querent-3.1.0/querent/config/collector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/collector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13454 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/collector/collector_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.557502 querent-3.1.0/querent/config/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/core/gpt_llm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/core/llm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/core/opensource_llm_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.557502 querent-3.1.0/querent/config/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/engine/engine_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/graph_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.557502 querent-3.1.0/querent/config/ingestor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/ingestor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/ingestor/ingestor_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.557502 querent-3.1.0/querent/config/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/logger/logger_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.557502 querent-3.1.0/querent/config/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/metric/prometheus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.557502 querent-3.1.0/querent/config/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/resource/resource_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.561502 querent-3.1.0/querent/config/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/workflow/workflow_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.561502 querent-3.1.0/querent/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/controllers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.561502 querent-3.1.0/querent/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12319 2024-05-06 16:53:38.000000 querent-3.1.0/querent/core/base_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.561502 querent-3.1.0/querent/core/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/core/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17628 2024-05-06 16:53:38.000000 querent-3.1.0/querent/core/transformers/bert_ner_opensourcellm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10986 2024-05-06 16:53:38.000000 querent-3.1.0/querent/core/transformers/fixed_entities_set_opensourcellm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22298 2024-05-06 16:53:38.000000 querent-3.1.0/querent/core/transformers/gpt_llm_bert_ner_or_fixed_entities_set_ner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13083 2024-05-06 16:53:38.000000 querent-3.1.0/querent/core/transformers/gpt_llm_gpt_ner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-05-06 16:53:38.000000 querent-3.1.0/querent/core/transformers/relationship_extraction_llm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.561502 querent-3.1.0/querent/dal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/dal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.565502 querent-3.1.0/querent/gnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/gnn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.565502 querent-3.1.0/querent/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-06 16:53:38.000000 querent-3.1.0/querent/graph/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-05-06 16:53:38.000000 querent-3.1.0/querent/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-05-06 16:53:38.000000 querent-3.1.0/querent/graph/graph_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-06 16:53:38.000000 querent-3.1.0/querent/graph/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-06 16:53:38.000000 querent-3.1.0/querent/graph/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-05-06 16:53:38.000000 querent-3.1.0/querent/graph/shacl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-05-06 16:53:38.000000 querent-3.1.0/querent/graph/subject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-05-06 16:53:38.000000 querent-3.1.0/querent/graph/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.569502 querent-3.1.0/querent/ingestors/
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.569502 querent-3.1.0/querent/ingestors/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/audio/audio_ingestors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/base_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.569502 querent-3.1.0/querent/ingestors/code/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/code/code_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.569502 querent-3.1.0/querent/ingestors/csv/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/csv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/csv/csv_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.569502 querent-3.1.0/querent/ingestors/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/doc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/doc/doc_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.573502 querent-3.1.0/querent/ingestors/email/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8651 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/email/email_ingestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/email/email_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.573502 querent-3.1.0/querent/ingestors/github/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/github/github_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.573502 querent-3.1.0/querent/ingestors/html/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/html/html_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.573502 querent-3.1.0/querent/ingestors/images/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/images/image_ingestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/ingestor_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8332 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/ingestor_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.577502 querent-3.1.0/querent/ingestors/json/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/json/json_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.577502 querent-3.1.0/querent/ingestors/pdfs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/pdfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/pdfs/pdf_ingestor_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.577502 querent-3.1.0/querent/ingestors/ppt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/ppt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7421 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/ppt/ppt_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.577502 querent-3.1.0/querent/ingestors/texts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/texts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/texts/text_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.577502 querent-3.1.0/querent/ingestors/video/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/video/video_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.577502 querent-3.1.0/querent/ingestors/xlsx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/xlsx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/xlsx/xlsx_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.581502 querent-3.1.0/querent/ingestors/xml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/xml/xml_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.581502 querent-3.1.0/querent/kg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.585502 querent-3.1.0/querent/kg/ner_helperfunctions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/ner_helperfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/ner_helperfunctions/attn_scores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/ner_helperfunctions/contextual_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/ner_helperfunctions/dependency_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/ner_helperfunctions/filter_triples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/ner_helperfunctions/fixed_entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/ner_helperfunctions/fixed_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18269 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/ner_helperfunctions/ner_llm_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/querent_kg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.589502 querent-3.1.0/querent/kg/rel_helperfunctions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/rel_helperfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/rel_helperfunctions/contextual_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/rel_helperfunctions/embedding_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/rel_helperfunctions/fixed_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/rel_helperfunctions/gpt_pydantic_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/rel_helperfunctions/opeai_ratelimiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/rel_helperfunctions/openai_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/rel_helperfunctions/openllm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/rel_helperfunctions/questionanswer_llama2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/rel_helperfunctions/rel_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/rel_helperfunctions/triple_to_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.593502 querent-3.1.0/querent/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-06 16:53:38.000000 querent-3.1.0/querent/logging/custom_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-06 16:53:38.000000 querent-3.1.0/querent/logging/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-06 16:53:38.000000 querent-3.1.0/querent/logging/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-06 16:53:38.000000 querent-3.1.0/querent/logging/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.593502 querent-3.1.0/querent/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/metric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.593502 querent-3.1.0/querent/metric/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/metric/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-06 16:53:38.000000 querent-3.1.0/querent/metric/adapters/promethus_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-06 16:53:38.000000 querent-3.1.0/querent/metric/base_metric_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-06 16:53:38.000000 querent-3.1.0/querent/metric/metric_logging_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-06 16:53:38.000000 querent-3.1.0/querent/metric/metric_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.597502 querent-3.1.0/querent/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-06 16:53:38.000000 querent-3.1.0/querent/processors/async_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-06 16:53:38.000000 querent-3.1.0/querent/processors/text_cleanup_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-06 16:53:38.000000 querent-3.1.0/querent/processors/text_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.597502 querent-3.1.0/querent/querent/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/querent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-05-06 16:53:38.000000 querent-3.1.0/querent/querent/auto_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-06 16:53:38.000000 querent-3.1.0/querent/querent/querent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-06 16:53:38.000000 querent-3.1.0/querent/querent/resource_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/querent/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.597502 querent-3.1.0/querent/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-06 16:53:38.000000 querent-3.1.0/querent/storage/gcs_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-06 16:53:38.000000 querent-3.1.0/querent/storage/milvus_vectorevent_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-06 16:53:38.000000 querent-3.1.0/querent/storage/neo4j_graphevent_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-06 16:53:38.000000 querent-3.1.0/querent/storage/postgres_graphevent_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.601502 querent-3.1.0/querent/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10882 2024-05-06 16:53:38.000000 querent-3.1.0/querent/tools/web_page_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.601502 querent-3.1.0/querent/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-05-06 16:53:38.000000 querent-3.1.0/querent/utils/webpage_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.601502 querent-3.1.0/querent/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-06 16:53:38.000000 querent-3.1.0/querent/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7164 2024-05-06 16:53:38.000000 querent-3.1.0/querent/workflow/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-05-06 16:53:38.000000 querent-3.1.0/querent/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.601502 querent-3.1.0/querent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16923 2024-05-06 16:58:17.000000 querent-3.1.0/querent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7202 2024-05-06 16:58:17.000000 querent-3.1.0/querent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:58:17.000000 querent-3.1.0/querent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-06 16:58:17.000000 querent-3.1.0/querent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-06 16:58:17.000000 querent-3.1.0/querent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 16:58:17.601502 querent-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-06 16:53:38.000000 querent-3.1.0/setup.py
```

### Comparing `querent-3.0.9/LICENCE` & `querent-3.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/PKG-INFO` & `querent-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: querent
-Version: 3.0.9
+Version: 3.1.0
 Summary: The Asynchronous Data Dynamo and Graph Neural Network Catalyst
 Home-page: https://github.com/Querent-ai/querent-ai
 Author: Querent AI
 License: Business Source License 1.1
 Project-URL: Documentation, https://github.com/Querent-ai/querent-ai/docs
 Project-URL: Issue Tracker, https://github.com/Querent-ai/querent-ai/issues
 Keywords: Graph Neural Network,Scalability,Data-Driven Insights,GNN,Async,Knowledge Graphs,KG,Large Language Models,asyncio,Insights,aysnchronous,LLM,transformers,pytorch,Llama-index,AI,Artificial Intelligence,Neo4j,Queues,QuiAssisstant,Collectors,Data,Data Science,Data Engineering,Data Analysis,Data Analytics,News,NLP,Natural Language Processing,Text,Text Analysis,Deep Learning,Graphs,Graph Theory,Graph Algorithms,Graph Analytics,Graph Databases,Graph Processing,Graph Mining,Graph Neural Networks,GNN,GNNs,Graph Neural Network
```

### Comparing `querent-3.0.9/README.md` & `querent-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/__init__.py` & `querent-3.1.0/querent/__init__.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/callback/event_callback_dispatcher.py` & `querent-3.1.0/querent/callback/event_callback_dispatcher.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/callback/event_callback_interface.py` & `querent-3.1.0/querent/callback/event_callback_interface.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/channel/channel_interface.py` & `querent-3.1.0/querent/channel/channel_interface.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/collectors/aws/aws_collector.py` & `querent-3.1.0/querent/collectors/aws/aws_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/collectors/azure/azure_collector.py` & `querent-3.1.0/querent/collectors/azure/azure_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/collectors/collector_errors.py` & `querent-3.1.0/querent/collectors/collector_errors.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/collectors/collector_factory.py` & `querent-3.1.0/querent/collectors/collector_factory.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/collectors/collector_resolver.py` & `querent-3.1.0/querent/collectors/collector_resolver.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/collectors/drive/google_drive_collector.py` & `querent-3.1.0/querent/collectors/drive/google_drive_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/collectors/dropbox/dropbox_collector.py` & `querent-3.1.0/querent/collectors/dropbox/dropbox_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/collectors/email/email_collector.py` & `querent-3.1.0/querent/collectors/email/email_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/collectors/email/imap.py` & `querent-3.1.0/querent/collectors/email/imap.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/collectors/fs/fs_collector.py` & `querent-3.1.0/querent/collectors/fs/fs_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/collectors/gcs/gcs_collector.py` & `querent-3.1.0/querent/collectors/gcs/gcs_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/collectors/github/github_collector.py` & `querent-3.1.0/querent/collectors/github/github_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/collectors/jira/jira_collector.py` & `querent-3.1.0/querent/collectors/jira/jira_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/collectors/news/news_collector.py` & `querent-3.1.0/querent/collectors/news/news_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/collectors/slack/slack_collector.py` & `querent-3.1.0/querent/collectors/slack/slack_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/collectors/webscaper/web_scraper_collector.py` & `querent-3.1.0/querent/collectors/webscaper/web_scraper_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/common/common_errors.py` & `querent-3.1.0/querent/common/common_errors.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/common/errors/metric_errors.py` & `querent-3.1.0/querent/common/errors/metric_errors.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/common/types/collected_bytes.py` & `querent-3.1.0/querent/common/types/collected_bytes.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/common/types/file_buffer.py` & `querent-3.1.0/querent/common/types/file_buffer.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/common/types/ingested_code.py` & `querent-3.1.0/querent/common/types/ingested_code.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/common/types/ingested_images.py` & `querent-3.1.0/querent/common/types/ingested_images.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/common/types/ingested_messages.py` & `querent-3.1.0/querent/common/types/ingested_messages.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/common/types/ingested_table.py` & `querent-3.1.0/querent/common/types/ingested_table.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/common/types/ingested_tokens.py` & `querent-3.1.0/querent/common/types/ingested_tokens.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/common/types/querent_queue.py` & `querent-3.1.0/querent/common/types/querent_queue.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/common/uri.py` & `querent-3.1.0/querent/common/uri.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/config/collector/collector_config.py` & `querent-3.1.0/querent/config/collector/collector_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/config/config.py` & `querent-3.1.0/querent/config/config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/config/core/gpt_llm_config.py` & `querent-3.1.0/querent/config/core/gpt_llm_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/config/core/llm_config.py` & `querent-3.1.0/querent/config/core/llm_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,19 +14,15 @@
     ner_model_name: str = "dbmdz/bert-large-cased-finetuned-conll03-english"
     spacy_model_path: str = 'en_core_web_lg'
     nltk_path: str = '/model/nltk_data'
     rel_model_type: str = 'llama'
     rel_model_path: str = './tests/llama-2-7b-chat.Q5_K_M.gguf'
     grammar_file_path: str = './querent/kg/rel_helperfunctions/json.gbnf'
     emb_model_name: str = 'sentence-transformers/all-MiniLM-L6-v2'
-    user_context: str = Field(default="""Please analyze the provided context and two entities. Use this information to answer the users query below.
-Context: {context}
-Entity 1: {entity1} and Entity 2: {entity2}
-Query: In a semantic triple (Subject, Predicate & Object) framework, determine which of the above entity is the subject and which is the object based on the context along with the predicate between these entities. Please also identify the subject type, object type & predicate type.
-Answer:""")
+    user_context: str = Field(default="In a semantic triple (Subject, Predicate & Object) framework, determine which of the above entity is the subject and which is the object based on the context along with the predicate between these entities. Please also identify the subject type, object type & predicate type.")
     enable_filtering: bool = False
     filter_params: dict = Field(default_factory=lambda: {
         'score_threshold': 0.6,
         'attention_score_threshold': 0.1,
         'similarity_threshold': 0.5,
         'min_cluster_size': 5,
         'min_samples': 3,
```

### Comparing `querent-3.0.9/querent/config/core/opensource_llm_config.py` & `querent-3.1.0/querent/config/core/opensource_llm_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/config/engine/engine_config.py` & `querent-3.1.0/querent/config/engine/engine_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/config/graph_config.py` & `querent-3.1.0/querent/config/graph_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/config/ingestor/ingestor_config.py` & `querent-3.1.0/querent/config/ingestor/ingestor_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/config/metric/prometheus.py` & `querent-3.1.0/querent/config/metric/prometheus.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/config/resource/resource_config.py` & `querent-3.1.0/querent/config/resource/resource_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/config/workflow/workflow_config.py` & `querent-3.1.0/querent/config/workflow/workflow_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/core/base_engine.py` & `querent-3.1.0/querent/core/base_engine.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/core/transformers/bert_ner_opensourcellm.py` & `querent-3.1.0/querent/core/transformers/bert_ner_opensourcellm.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,29 +25,14 @@
 from querent.config.graph_config import GraphConfig
 from querent.kg.ner_helperfunctions.attn_scores import EntityAttentionExtractor
 from querent.kg.ner_helperfunctions.filter_triples import TripleFilter
 from querent.config.core.llm_config import LLM_Config
 from querent.kg.rel_helperfunctions.triple_to_json import TripleToJsonConverter
 from querent.kg.rel_helperfunctions.embedding_store import EmbeddingStore
 
-"""
-    BERTLLM is a class derived from BaseEngine designed for processing language models, particularly focusing on named entity recognition and relationship extraction in text. It integrates various components for handling different types of input data (messages, images, code, tokens), extracting entities, filtering relevant information, and constructing knowledge graphs.
-
-    Key functionalities include:
-    - Initializing with a specific configuration for named entity recognition (NER) and language model processing.
-    - Validating the presence of NER models and tokenizers.
-    - Processing various types of input data like messages, images, code, and tokens.
-    - Implementing methods for counting entity pairs, setting filter parameters, and processing tokens.
-    - Extracting and clustering entities and relationships from the text, and converting them into graph and vector formats.
-    - Handling errors and maintaining robustness in data processing.
-
-    The class also incorporates mechanisms for filtering and clustering entities and relationships, as well as extracting embeddings and generating output in different formats.
-    """
-
-
 class BERTLLM(BaseEngine):
     def __init__(
         self,
         input_queue:QuerentQueue,
         config: LLM_Config,
         Embedding=None
     ):  
@@ -96,16 +81,20 @@
                 self.entity_context_extractor = None
             self.fixed_relationships = config.fixed_relationships
             self.sample_relationships = config.sample_relationships
             if self.fixed_relationships and not self.sample_relationships:
                 raise ValueError("If specific predicates are provided, their types should also be provided.")
             if self.fixed_relationships and self.sample_relationships:
                 self.predicate_context_extractor = FixedPredicateExtractor(fixed_predicates=self.fixed_relationships, predicate_types=self.sample_relationships,model = self.nlp_model)
+                self.predicate_json = self.predicate_context_extractor.construct_predicate_json(self.fixed_relationships, self.sample_relationships)
+                self.predicate_json_emb = self.create_emb.generate_relationship_embeddings(self.predicate_json)
             elif self.sample_relationships:
                 self.predicate_context_extractor = FixedPredicateExtractor(predicate_types=self.sample_relationships,model = self.nlp_model)
+                self.predicate_json = self.predicate_context_extractor.construct_predicate_json(relationship_types=self.sample_relationships)
+                self.predicate_json_emb = self.create_emb.generate_relationship_embeddings(self.predicate_json)
             else:
                 self.predicate_context_extractor = None
             self.user_context = config.user_context
             self.isConfinedSearch = config.is_confined_search
         except Exception as e:
             self.logger.error("Error initializing BERT LLM Class", e)
             raise e
@@ -220,17 +209,15 @@
         doc_entity_pairs = []
         try:
             doc_source = data.doc_source
             if not BERTLLM.validate_ingested_tokens(data):
                     self.set_termination_event()                                      
                     return
             if data.data:
-                single_string = ' '.join(data.data)
-                clean_text = single_string
-                
+                clean_text = ' '.join(data.data)
             else:
                 clean_text = data.data
             if not data.is_token_stream : 
                 file, content = self.file_buffer.add_chunk(
                 data.get_file_path(), clean_text)
             else:
                 content = clean_text
@@ -244,45 +231,48 @@
                                                                                                   content=content,
                                                                                                   fixed_entities=self.fixed_entities,
                                                                                                   sample_entities=self.sample_entities)
             else:
                 return
             if self.sample_entities:
                 doc_entity_pairs = self.entity_context_extractor.process_entity_types(doc_entities=doc_entity_pairs)
-            if doc_entity_pairs and any(doc_entity_pairs):
+            if any(doc_entity_pairs):
                 doc_entity_pairs = self.ner_llm_instance.remove_duplicates(doc_entity_pairs)
                 pairs_withattn = self.attn_scores_instance.extract_and_append_attention_weights(doc_entity_pairs)
                 if self.enable_filtering == True and not self.entity_context_extractor and self.count_entity_pairs(pairs_withattn)>1 and not self.predicate_context_extractor:
                     self.entity_embedding_extractor = EntityEmbeddingExtractor(self.ner_model, self.ner_tokenizer)
                     pairs_withemb = self.entity_embedding_extractor.extract_and_append_entity_embeddings(pairs_withattn)
                 else:
                     pairs_withemb = pairs_withattn
                 pairs_with_predicates = process_data(pairs_withemb, file)
                 if self.enable_filtering == True and not self.entity_context_extractor and self.count_entity_pairs(pairs_withattn)>1 and not self.predicate_context_extractor:
                     cluster_output = self.triple_filter.cluster_triples(pairs_with_predicates)
                     clustered_triples = cluster_output['filtered_triples']
                     cluster_labels = cluster_output['cluster_labels']
                     cluster_persistence = cluster_output['cluster_persistence']
-                    # final_clustered_triples = self.triple_filter.filter_by_cluster_persistence(pairs_with_predicates, cluster_persistence, cluster_labels)
                     if clustered_triples:
                         filtered_triples, reduction_count = self.triple_filter.filter_triples(clustered_triples)
                     else:
-                        # filtered_triples, _ = self.triple_filter.filter_triples(clustered_triples)
                         self.logger.debug(f"Filtering in {self.__class__.__name__} producing 0 entity pairs. Filtering Disabled. ")
                         filtered_triples = pairs_with_predicates
                 else:
                     filtered_triples = pairs_with_predicates
                 if not filtered_triples:
                     return
                 elif not self.skip_inferences:
-                    relationships = self.semantic_extractor.process_tokens(filtered_triples)
+                    relationships = self.semantic_extractor.process_tokens(filtered_triples, fixed_entities=(len(self.sample_entities) >= 1))
                     if len(relationships) > 0:
-                        embedding_triples = self.create_emb.generate_embeddings(relationships)
+                        if self.fixed_relationships and self.sample_relationships:
+                            embedding_triples = self.create_emb.generate_embeddings(relationships, relationship_finder=True, generate_embeddings_with_fixed_relationship = True)
+                        elif self.sample_relationships:
+                            embedding_triples = self.create_emb.generate_embeddings(relationships, relationship_finder=True)
+                        else:
+                            embedding_triples = self.create_emb.generate_embeddings(relationships)
                         if self.sample_relationships:
-                            embedding_triples = self.predicate_context_extractor.process_predicate_types(embedding_triples)
+                            embedding_triples = self.predicate_context_extractor.update_embedding_triples_with_similarity(self.predicate_json_emb, embedding_triples)
                         for triple in embedding_triples:
                             if not self.termination_event.is_set():
                                 graph_json = json.dumps(TripleToJsonConverter.convert_graphjson(triple))
                                 if graph_json:
                                     current_state = EventState(event_type=EventType.Graph, timestamp=time.time(), payload=graph_json, file=file, doc_source=doc_source)
                                     await self.set_state(new_state=current_state)
                                 vector_json = json.dumps(TripleToJsonConverter.convert_vectorjson(triple))
```

### Comparing `querent-3.0.9/querent/core/transformers/fixed_entities_set_opensourcellm.py` & `querent-3.1.0/querent/core/transformers/fixed_entities_set_opensourcellm.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,16 +76,20 @@
             self.entity_context_extractor = None
         self.fixed_relationships = config.fixed_relationships
         self.sample_relationships = config.sample_relationships
         if self.fixed_relationships and not self.sample_relationships:
             raise ValueError("If specific predicates are provided, their types should also be provided.")
         if self.fixed_relationships and self.sample_relationships:
             self.predicate_context_extractor = FixedPredicateExtractor(fixed_predicates=self.fixed_relationships, predicate_types=self.sample_relationships,model = self.nlp_model)
+            self.predicate_json = self.predicate_context_extractor.construct_predicate_json(self.fixed_relationships, self.sample_relationships)
+            self.predicate_json_emb = self.create_emb.generate_relationship_embeddings(self.predicate_json)
         elif self.sample_relationships:
             self.predicate_context_extractor = FixedPredicateExtractor(predicate_types=self.sample_relationships,model = self.nlp_model)
+            self.predicate_json = self.predicate_context_extractor.construct_predicate_json(relationship_types=self.sample_relationships)
+            self.predicate_json_emb = self.create_emb.generate_relationship_embeddings(self.predicate_json)
         else:
             self.predicate_context_extractor = None
         self.user_context = config.user_context
         self.isConfinedSearch = config.is_confined_search
         
  
 
@@ -125,17 +129,15 @@
         doc_entity_pairs = []
         try:
             doc_source = data.doc_source
             if not Fixed_Entities_LLM.validate_ingested_tokens(data):
                     self.set_termination_event()                                      
                     return
             if data.data:
-                single_string = ' '.join(data.data)
-                clean_text = single_string
-                # clean_text = unidecode(single_string)
+                clean_text = ' '.join(data.data)
             else:
                 clean_text = data.data
             if not data.is_token_stream : 
                 file, content = self.file_buffer.add_chunk(
                 data.get_file_path(), clean_text)
             else:
                 content = clean_text
@@ -159,17 +161,22 @@
                 if not filtered_triples:
                     self.logger.debug("No entity pairs")
                     return
                 elif not self.skip_inferences:
                     relationships = self.semantic_extractor.process_tokens(filtered_triples)
                     self.logger.debug(f"length of relationships {len(relationships)}")
                     if len(relationships) > 0:
-                        embedding_triples = self.create_emb.generate_embeddings(relationships)
+                        if self.fixed_relationships and self.sample_relationships:
+                            embedding_triples = self.create_emb.generate_embeddings(relationships, relationship_finder=True, generate_embeddings_with_fixed_relationship = True)
+                        elif self.sample_relationships:
+                            embedding_triples = self.create_emb.generate_embeddings(relationships, relationship_finder=True)
+                        else:
+                            embedding_triples = self.create_emb.generate_embeddings(relationships)
                         if self.sample_relationships:
-                            embedding_triples = self.predicate_context_extractor.process_predicate_types(embedding_triples)
+                            embedding_triples = self.predicate_context_extractor.update_embedding_triples_with_similarity(self.predicate_json_emb, embedding_triples)
                         for triple in embedding_triples:
                             if not self.termination_event.is_set():
                                 graph_json = json.dumps(TripleToJsonConverter.convert_graphjson(triple))
                                 if graph_json:
                                     current_state = EventState(event_type=EventType.Graph,timestamp=time.time(), payload=graph_json, file=file, doc_source=doc_source)
                                     await self.set_state(new_state=current_state)
                                 vector_json = json.dumps(TripleToJsonConverter.convert_vectorjson(triple))
```

### Comparing `querent-3.0.9/querent/core/transformers/gpt_llm_bert_ner_or_fixed_entities_set_ner.py` & `querent-3.1.0/querent/core/transformers/gpt_llm_bert_ner_or_fixed_entities_set_ner.py`

 * *Files 13% similar despite different names*

```diff
@@ -55,31 +55,37 @@
             },
             sample_entities = config.sample_entities,
             fixed_entities = config.fixed_entities,
             skip_inferences= True,
             is_confined_search = config.is_confined_search,
             huggingface_token = config.huggingface_token,
             spacy_model_path = config.spacy_model_path,
-            nltk_path = config.nltk_path)
+            nltk_path = config.nltk_path,
+            fixed_relationships = config.fixed_relationships,
+            sample_relationships = config.sample_relationships)
             self.fixed_entities = config.fixed_entities
             self.is_confined_search = config.is_confined_search
             self.fixed_relationships = config.fixed_relationships
             self.sample_relationships = config.sample_relationships
             self.user_context = config.user_context
             self.nlp_model = NER_LLM.set_nlp_model(config.spacy_model_path)
             self.nlp_model = NER_LLM.get_class_variable()
+            self.create_emb = EmbeddingStore()
             if self.fixed_relationships and not self.sample_relationships:
                 raise ValueError("If specific predicates are provided, their types should also be provided.")
             if self.fixed_relationships and self.sample_relationships:
-                self.predicate_context_extractor = FixedPredicateExtractor(fixed_predicates=self.fixed_relationships, predicate_types=self.sample_relationships,  model = self.nlp_model)
+                self.predicate_context_extractor = FixedPredicateExtractor(fixed_predicates=self.fixed_relationships, predicate_types=self.sample_relationships,model = self.nlp_model)
+                self.predicate_json = self.predicate_context_extractor.construct_predicate_json(self.fixed_relationships, self.sample_relationships)
+                self.predicate_json_emb = self.create_emb.generate_relationship_embeddings(self.predicate_json)
             elif self.sample_relationships:
-                self.predicate_context_extractor = FixedPredicateExtractor(predicate_types=self.sample_relationships,  model = self.nlp_model)
+                self.predicate_context_extractor = FixedPredicateExtractor(predicate_types=self.sample_relationships,model = self.nlp_model)
+                self.predicate_json = self.predicate_context_extractor.construct_predicate_json(relationship_types=self.sample_relationships)
+                self.predicate_json_emb = self.create_emb.generate_relationship_embeddings(self.predicate_json)
             else:
                 self.predicate_context_extractor = None
-            self.create_emb = EmbeddingStore()
             if config.is_confined_search:
                 self.llm_instance = Fixed_Entities_LLM(input_queue, llm_config, self.create_emb)
             else :
                 self.llm_instance = BERTLLM(input_queue, llm_config, self.create_emb)
             if not isinstance (self.llm_instance, BERTLLM):
                 self.process_image_instance = BERTLLM(input_queue, llm_config, self.create_emb)
             else:
@@ -175,15 +181,15 @@
             modified_tuple = (tup[0], modified_json_str, tup[2])
             result.append(modified_tuple)
 
         return result
     
     async def process_triples(self, context, entity1, entity2, entity1_label, entity2_label):
         try: 
-            if not self.user_context:
+            if not self.user_context and not self.fixed_entities:
                 identify_entity_message = f"""Please analyze the provided context below. Once you have understood the context, answer the user query using the specified output format.
         
                     Context: {context}
                     Entity 1: {entity1} and Entity 2: {entity2}
                     Output Format:
                     [
                         {{
@@ -194,15 +200,37 @@
                             'object_type': 'The category of the object entity e.g. location, person, event, material, process etc.',
                             'predicate_type': 'The category of the predicate e.g. causative, action, ownership, occurance etc.'
                         }},
                     ]
                     """
                 messages_classify_entity = [
                     {"role": "user", "content": identify_entity_message},
-                    {"role": "user", "content": "Query: First, identify all geological entities in the provided context. Then, create relevant semantic triples (Subject, Predicate, Object) and also categorize the respective the Subject, Object types (e.g. location, person, event, material, process etc.) and Predicate type. Use the above output format to provide all the relevant semantic triples."},
+                    {"role": "user", "content": "Query : In the context of a semantic triple framework, first identify which entity is subject and which is the object along with their respective types. Also determine the predicate and predicate type."},
+                ]
+            elif not self.user_context and self.fixed_entities :
+                identify_entity_message = f"""Please analyze the provided context below. Once you have understood the context, answer the user query using the specified output format.
+        
+                    Context: {context}
+                    Entity 1: {entity1} and Entity 2: {entity2}
+                    Entity 1_Type: {entity1_label} and Entity 2_Type: {entity2_label}
+                    Output Format:
+                    [
+                        {{
+                            'subject': 'Identified as the main entity in the context, typically the initiator or primary focus of the action or topic being discussed.',
+                            'predicate': 'The relationship (predicate) between the subject and the object.',
+                            'object': 'This parameter represents the entity in the context directly impacted by or involved in the action, typically the recipient or target of the main verb's action.',
+                            'subject_type': 'The category of the subject entity e.g. location, person, event, material, process etc.',
+                            'object_type': 'The category of the object entity e.g. location, person, event, material, process etc.',
+                            'predicate_type': 'The category of the predicate e.g. causative, action, ownership, occurance etc.'
+                        }},
+                    ]
+                    """
+                messages_classify_entity = [
+                    {"role": "user", "content": identify_entity_message},
+                    {"role": "user", "content": "Query : In the context of a semantic triple framework, first identify which entity is subject and which is the object and also validate and output their their respective types. Also determine the predicate and predicate type."},
                 ]
             elif self.user_context and self.fixed_entities :
                 identify_entity_message = f"""Please analyze the provided context below. Once you have understood the context, answer the user query using the specified output format.
         
                     Context: {context}
                     Entity 1: {entity1} and Entity 2: {entity2}
                     Entity 1_Type: {entity1_label} and Entity 2_Type: {entity2_label}
@@ -284,51 +312,68 @@
         output_tuple = (
             subject,
             f'{{"predicate": "{predicate}", "predicate_type": "{predicate_type}", "context": "{context}", "file": "{context_data.get("file_path", "")}", "subject_type": "{subject_type}", "object_type": "{object_type}"}}',
             object
         )
 
         return output_tuple
-      
+    
+    def extract_key(tup):
+        subject, json_string, obj = tup
+        data = json.loads(json_string.replace("\n", ""))
+        return (subject, data.get('predicate'), obj)
+   
     async def process_tokens(self, data: IngestedTokens):
         try:
             if not GPTLLM.validate_ingested_tokens(data):
                     self.set_termination_event()                    
                     return 
             doc_source = data.doc_source
             relationships = []
-            result = await self.llm_instance.process_tokens(data)
+            unique_keys = set()
+            result = await self.llm_instance.process_tokens(data)      
             if not result: return 
             else:
                 filtered_triples, file = result
                 modified_data = GPTLLM.remove_items_from_tuples(filtered_triples)
                 for entity1, context_json, entity2 in modified_data:
                     context_data = json.loads(context_json)
                     context = context_data.get("context", "")
                     entity1_label = context_data.get("entity1_label", "")
                     entity2_label = context_data.get("entity2_label", "")
                     entity1_nn_chunk = context_data.get("entity1_nn_chunk","")
                     entity2_nn_chunk = context_data.get("entity2_nn_chunk","")
                     result = await self.process_triples(context, entity1_nn_chunk, entity2_nn_chunk, entity1_label, entity2_label)
                     if result:
                         output_tuple = self.generate_output_tuple(result, context_json)
-                        relationships.append(output_tuple)
+                        key = GPTLLM.extract_key(output_tuple)
+                        if key not in unique_keys:
+                            unique_keys.add(key)
+                            relationships.append(output_tuple)
                 if len(relationships) > 0:
-                    embedding_triples = self.create_emb.generate_embeddings(relationships)
+                    if self.fixed_relationships and self.sample_relationships:
+                        embedding_triples = self.create_emb.generate_embeddings(relationships, relationship_finder=True, generate_embeddings_with_fixed_relationship = True)
+                    elif self.sample_relationships:
+                        embedding_triples = self.create_emb.generate_embeddings(relationships, relationship_finder=True)
+                    else:
+                        embedding_triples = self.create_emb.generate_embeddings(relationships)
+                    if self.sample_relationships:
+                        embedding_triples = self.predicate_context_extractor.update_embedding_triples_with_similarity(self.predicate_json_emb, embedding_triples)
                     for triple in embedding_triples:
                         if not self.termination_event.is_set():
                             graph_json = json.dumps(TripleToJsonConverter.convert_graphjson(triple))
                             if graph_json:
                                 current_state = EventState(event_type=EventType.Graph,timestamp = time.time(), payload= graph_json, file=file, doc_source=doc_source)
                                 await self.set_state(new_state=current_state)
                             vector_json = json.dumps(TripleToJsonConverter.convert_vectorjson(triple))
                             if vector_json:
                                 current_state = EventState(event_type=EventType.Vector,timestamp=time.time(), payload = vector_json, file=file, doc_source=doc_source)
                                 await self.set_state(new_state=current_state)
                         else:
                             return
+                else:
+                    return
         except Exception as e:
             self.logger.error(f"Invalid {self.__class__.__name__} configuration. Unable to extract predicates using GPT. {e}")
-            raise Exception(f"An error occurred while extracting predicates using GPT: {e}")
 
     async def process_messages(self, data: IngestedMessages):
         raise NotImplementedError
```

### Comparing `querent-3.0.9/querent/core/transformers/gpt_llm_gpt_ner.py` & `querent-3.1.0/querent/core/transformers/gpt_llm_gpt_ner.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,14 @@
             if not GPTNERLLM.validate_ingested_tokens(data):
                     self.set_termination_event()                    
                     return 
 
             doc_source = data.doc_source
             if data.data:
                 clean_text = ' '.join(data.data)
-                #clean_text = unidecode(single_string)
             else:
                 clean_text = data.data
             if not data.is_token_stream : 
                 file, content = self.file_buffer.add_chunk(
                 data.get_file_path(), clean_text)
             else:
                 content = clean_text
@@ -254,13 +253,14 @@
                             triple['context'] = triple['sentence']
                             vector_json = json.dumps(TripleToJsonConverter.convert_vectorjson((triple['subject'],json.dumps(triple), triple['object'])))
                             if vector_json:
                                     current_state = EventState(event_type=EventType.Vector,timestamp=time.time(), payload=vector_json, file=file, doc_source=doc_source)
                                     await self.set_state(new_state=current_state)
                         else:
                             return
-
+            else:
+                return
         except Exception as e:
             self.logger.debug(f"Invalid {self.__class__.__name__} configuration. Unable to extract predicates using GPT NER LLM class. {e}")
     
     async def process_messages(self, data: IngestedMessages):
         raise NotImplementedError
```

### Comparing `querent-3.0.9/querent/core/transformers/relationship_extraction_llm.py` & `querent-3.1.0/querent/core/transformers/relationship_extraction_llm.py`

 * *Files 6% similar despite different names*

```diff
@@ -94,19 +94,19 @@
                 return False
 
             return True
         except Exception as e:
             self.logger.error(f"Error in validation: {e}")
             return False
     
-    def process_tokens(self, payload):
+    def process_tokens(self, payload, fixed_entities = False):
         try:
             triples = payload
             trimmed_triples = self.normalizetriples_buildindex(triples)
-            relationships = self.extract_relationships(triples)
+            relationships = self.extract_relationships(triples, fixed_entities)
         
             return relationships
         
         except Exception as e:
             self.logger.error(f"Error in processing event: {e}")
             raise Exception(f"Invalid in processing event: {e}")
 
@@ -157,33 +157,50 @@
         if data.get("object", "").strip() == "Entity 1":
             data["object"] = entity1
         elif data.get("object", "").strip() == "Entity 2":
             data["object"] = entity2
 
         return data
 
-    def extract_relationships(self, triples):
+    def extract_relationships(self, triples, fixed_entities = False):
         try:
             self.logger.debug(f"Length of identified triples {len(triples)}")
             updated_triples = []
             for _, predicate_str, _ in triples:
                 data = json.loads(predicate_str)
                 context = data['context']
                 predicate = predicate_str if isinstance(predicate_str, dict) else json.loads(predicate_str)
-                query = """Please analyze the provided context and two entities. Use this information to answer the users query below.
+                if fixed_entities == False:
+                    query = """Please analyze the provided context and two entities. Use this information to answer the users query below.
 Context: {context}
 Entity 1: {entity1} and Entity 2: {entity2}
 Query:{question}
-Answer:"""
-                if not self.config.qa_template:
-                    question = "In the context of reservoir studies, identify the subject, predicate, and object in a semantic triple framework, focusing on reservoir attributes (e.g., porosity, permeability), processes (e.g., influences, determines), and outcomes (e.g., recovery efficiency). Specify the types for the subject (attribute), predicate (process), and object (outcome)."
-                    query = query.format(question = question, context = context, entity1=predicate.get('entity1_nn_chunk', ''), entity2=predicate.get('entity2_nn_chunk', ''))   
+Answer:"""          
+                    if not self.config.qa_template:
+                        question = "In the context of a semantic triple framework, first identify which entity is subject and which is the object along with their respective types. Also determine the predicate and predicate type."   
+                    else:
+                        question = self.config.qa_template
+                    query = query.format(question = question, context = context, entity1=predicate.get('entity1_nn_chunk', ''), entity2=predicate.get('entity2_nn_chunk', ''))
                 else:
-                    question = self.config.qa_template
-                    query = query.format(question = question, context = context, entity1=predicate.get('entity1_nn_chunk', ''), entity2=predicate.get('entity2_nn_chunk', ''))    
+                    query = """Please analyze the provided context and two entities along with their identified labels. Use this information to answer the users query below.
+Context: {context}
+Entity 1: {entity1} and Entity 1_label: {entity1_label}
+Entity 2: {entity2} and Entity 2_label: {entity2_label}
+Query:{question}
+Answer:"""          
+                    if not self.config.qa_template:
+                        question = "In the context of a semantic triple framework, first identify which entity is subject and which is the object, validate and output their respective types. Also determine the predicate and predicate type."      
+                    else:
+                        question = self.config.qa_template
+                    query = query.format(question = question, 
+                                                context = context, 
+                                                entity1=predicate.get('entity1_nn_chunk', ''), 
+                                                entity2=predicate.get('entity2_nn_chunk', ''),
+                                                entity1_label=predicate.get('entity1_label', ''), 
+                                                entity2_label=predicate.get('entity2_label', ''))
                 answer_relation = self.qa_system.ask_question(prompt=query, llm=self.qa_system.llm, grammar=self.grammar)
                 try:
                     choices_text = answer_relation['choices'][0]['text']
                     answer_relation = self.replace_entities(choices_text,entity1=predicate.get('entity1_nn_chunk', ''), entity2=predicate.get('entity2_nn_chunk'))
                     updated_triple= self.create_semantic_triple(answer_relation, predicate_str)
                     updated_triples.append(updated_triple)
                 except Exception as e:
@@ -197,14 +214,16 @@
             trimmed_data = []
             for entity1, predicate, entity2 in data:
                 predicate_dict = json.loads(predicate)
                 trimmed_predicate = {
                     'context': predicate_dict.get('context', ''),
                     'entity1_nn_chunk': predicate_dict.get('entity1_nn_chunk', ''),
                     'entity2_nn_chunk': predicate_dict.get('entity2_nn_chunk', ''),
+                    'entity1_label': predicate_dict.get('entity1_label', ''),
+                    'entity2_label': predicate_dict.get('entity2_label', ''),
                     'file_path': predicate_dict.get('file_path', '')
                 }
                 trimmed_data.append((entity1, trimmed_predicate, entity2))
 
             return trimmed_data
         
         except Exception as e:
```

### Comparing `querent-3.0.9/querent/graph/errors.py` & `querent-3.1.0/querent/graph/errors.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/graph/graph.py` & `querent-3.1.0/querent/graph/graph.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/graph/graph_namespace.py` & `querent-3.1.0/querent/graph/graph_namespace.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/graph/ontology.py` & `querent-3.1.0/querent/graph/ontology.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/graph/schema.py` & `querent-3.1.0/querent/graph/schema.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/graph/shacl.py` & `querent-3.1.0/querent/graph/shacl.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/graph/subject.py` & `querent-3.1.0/querent/graph/subject.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/graph/utils.py` & `querent-3.1.0/querent/graph/utils.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/ingestors/audio/audio_ingestors.py` & `querent-3.1.0/querent/ingestors/audio/audio_ingestors.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/ingestors/base_ingestor.py` & `querent-3.1.0/querent/ingestors/base_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/ingestors/code/code_ingestor.py` & `querent-3.1.0/querent/ingestors/code/code_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/ingestors/csv/csv_ingestor.py` & `querent-3.1.0/querent/ingestors/csv/csv_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/ingestors/doc/doc_ingestor.py` & `querent-3.1.0/querent/ingestors/doc/doc_ingestor.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
                         error=None,
                         doc_source=chunk_bytes.doc_source
                     )
                     collected_bytes = b""
                     current_file = chunk_bytes.file
                 collected_bytes += chunk_bytes.data
         except Exception as e:
-            yield IngestedTokens(file=current_file, data=None, error=f"Exception: {e}")
+            yield IngestedTokens(file=current_file, doc_source = chunk_bytes.doc_source, data=None, error=f"Exception: {e}")
         finally:
             # process the last file
             async for ingested_data in self.extract_and_process_doc(
                 CollectedBytes(file=current_file, data=collected_bytes), doc_source=chunk_bytes.doc_source
             ):
                 yield ingested_data
             yield IngestedTokens(file=current_file, data=None, doc_source = chunk_bytes.doc_source, error=None)
@@ -112,15 +112,15 @@
             for rel in doc.part.rels.values():
                 if "image" in rel.reltype:
                     image = rel.target_part.blob 
                     ocr_text = await self.process_image(image)
                     if not ocr_text:
                         continue
                     encoded_image = base64.b64encode(image)
-                    yield IngestedImages(file = collected_bytes.file, image = encoded_image.decode('utf-8'), image_name=str(uuid.uuid4()), page_num=i, text=text, ocr_text=[ocr_text], error=None, coordinates=None)
+                    yield IngestedImages(file = collected_bytes.file, doc_source=doc_source, image = str(encoded_image), image_name=str(uuid.uuid4()), page_num=i, text=text, ocr_text=[ocr_text], error=None, coordinates=None)
                     i += 1
 
         elif file_extension == "doc":
             current_doc_text = await self.temp_extract_from(collected_bytes)
             yield IngestedTokens(
                 file=collected_bytes.file, data=current_doc_text, error=None, doc_source=doc_source
             )
```

### Comparing `querent-3.0.9/querent/ingestors/email/email_ingestor.py` & `querent-3.1.0/querent/ingestors/email/email_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/ingestors/email/email_reader.py` & `querent-3.1.0/querent/ingestors/email/email_reader.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/ingestors/github/github_ingestor.py` & `querent-3.1.0/querent/ingestors/github/github_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/ingestors/html/html_ingestor.py` & `querent-3.1.0/querent/ingestors/html/html_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/ingestors/images/image_ingestor.py` & `querent-3.1.0/querent/ingestors/images/image_ingestor.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,29 +53,29 @@
                 if chunk_bytes.file != current_file:
                     if current_file:
                         text = await self.extract_and_process_image(
                             CollectedBytes(file=current_file, data=collected_bytes)
                         )
                         if text is not None:
                             yield IngestedTokens(file=current_file, data=[text], error=None, doc_source=chunk_bytes.doc_source)
-                            yield IngestedImages(file=current_file, image=base64.b64encode(collected_bytes).decode('utf-8'), image_name=f"{str(uuid.uuid4())}.{chunk_bytes.extension}", page_num=0, text=[], ocr_text=[text], doc_source=chunk_bytes.doc_source)
+                            yield IngestedImages(file=current_file, image=str(base64.b64encode(collected_bytes)), image_name=f"{str(uuid.uuid4())}.{chunk_bytes.extension}", page_num=0, text=[], ocr_text=[text], doc_source=chunk_bytes.doc_source)
                             yield IngestedTokens(file=current_file, data=None, error=None, doc_source=chunk_bytes.doc_source)
 
                     current_file = chunk_bytes.file
                     collected_bytes = b""
 
                 collected_bytes += chunk_bytes.data
 
             if current_file:
                 text = await self.extract_and_process_image(
                     CollectedBytes(file=current_file, data=collected_bytes)
                 )
                 if text is not None:
                     yield IngestedTokens(file=current_file, data=[text], error=None, doc_source=chunk_bytes.doc_source)
-                    yield IngestedImages(file=current_file, image=base64.b64encode(collected_bytes).decode('utf-8'), image_name=f"{str(uuid.uuid4())}.{chunk_bytes.extension}", page_num=0, text=[], ocr_text=[text], doc_source=chunk_bytes.doc_source)
+                    yield IngestedImages(file=current_file, image=str(base64.b64encode(collected_bytes)), image_name=f"{str(uuid.uuid4())}.{chunk_bytes.extension}", page_num=0, text=[], ocr_text=[text], doc_source=chunk_bytes.doc_source)
                     yield IngestedTokens(file=current_file, data=None, error=None, doc_source=chunk_bytes.doc_source)
 
         except Exception as e:
             yield IngestedTokens(file=current_file, data=None, error=f"Exception: {e}", doc_source=chunk_bytes.doc_source)
 
     async def extract_and_process_image(self, collected_bytes: CollectedBytes) -> str:
         text = await self.extract_text_from_image(collected_bytes)
```

### Comparing `querent-3.0.9/querent/ingestors/ingestor_factory.py` & `querent-3.1.0/querent/ingestors/ingestor_factory.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/ingestors/ingestor_manager.py` & `querent-3.1.0/querent/ingestors/ingestor_manager.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/ingestors/json/json_ingestor.py` & `querent-3.1.0/querent/ingestors/json/json_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/ingestors/pdfs/pdf_ingestor_v1.py` & `querent-3.1.0/querent/ingestors/pdfs/pdf_ingestor_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,15 +170,15 @@
                 if page_index < len(doc):
                     text_content = doc[page_index].get_text()
                 else:
                     text_content = "Page not in document."
 
                 yield IngestedImages(
                     file=file_path,
-                    image=base64.b64encode(image_data).decode('utf-8'),
+                    image=str(base64.b64encode(image_data)),
                     image_name=f"{str(uuid.uuid4())}.{image_ext}",
                     page_num=page_num,
                     text=[text_content],
                     coordinates=None,
                     ocr_text=[ocr_text],
                     doc_source=doc_source,
                 )
```

### Comparing `querent-3.0.9/querent/ingestors/ppt/ppt_ingestor.py` & `querent-3.1.0/querent/ingestors/ppt/ppt_ingestor.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
                     for shape in slide.shapes:
                         if hasattr(shape, "text"):
                             text.append(shape.text)
                         if shape.shape_type == MSO_SHAPE_TYPE.PICTURE or (shape.shape_type in [MSO_SHAPE_TYPE.PLACEHOLDER, MSO_SHAPE_TYPE.AUTO_SHAPE] and hasattr(shape, "image")):
                             ocr_text = await self.process_image(shape)
                             if not ocr_text:
                                 continue
-                            yield IngestedImages(file=collected_bytes.file, image=pybase64.b64encode(shape.image.blob), image_name=str(uuid.uuid4()), page_num=i, text = text, ocr_text=[ocr_text], coordinates=None)
+                            yield IngestedImages(file=collected_bytes.file, doc_source=doc_source, image=str(pybase64.b64encode(shape.image.blob)), image_name=str(uuid.uuid4()), page_num=i, text = text, ocr_text=[ocr_text], coordinates=None)
 
                         if shape.has_table:
                             table = shape.table
                             
                             table_data = []
                             # for row in table.rows:
                             #     row_data = []
```

### Comparing `querent-3.0.9/querent/ingestors/texts/text_ingestor.py` & `querent-3.1.0/querent/ingestors/texts/text_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/ingestors/video/video_ingestor.py` & `querent-3.1.0/querent/ingestors/video/video_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/ingestors/xlsx/xlsx_ingestor.py` & `querent-3.1.0/querent/ingestors/xlsx/xlsx_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/ingestors/xml/xml_ingestor.py` & `querent-3.1.0/querent/ingestors/xml/xml_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/kg/ner_helperfunctions/attn_scores.py` & `querent-3.1.0/querent/kg/ner_helperfunctions/attn_scores.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/kg/ner_helperfunctions/contextual_embeddings.py` & `querent-3.1.0/querent/kg/ner_helperfunctions/contextual_embeddings.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/kg/ner_helperfunctions/dependency_parsing.py` & `querent-3.1.0/querent/kg/ner_helperfunctions/dependency_parsing.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/kg/ner_helperfunctions/filter_triples.py` & `querent-3.1.0/querent/kg/ner_helperfunctions/filter_triples.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/kg/ner_helperfunctions/fixed_entities.py` & `querent-3.1.0/querent/kg/ner_helperfunctions/fixed_entities.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/kg/ner_helperfunctions/ner_llm_transformer.py` & `querent-3.1.0/querent/kg/ner_helperfunctions/ner_llm_transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -378,15 +378,15 @@
         info = json.loads(info_json)
         info['subject_type'] = info.pop('entity1_label')
         info['object_type'] = info.pop('entity2_label')
         info['predicate'] = "has image"
         info['predicate_type'] = "has image"
         info['context_embeddings'] = create_embeddings.get_embeddings([info['context']])[0]
         updated_json = json.dumps(info)
-        updated_tuple = (entity, updated_json, second_entity)
+        updated_tuple = (info['entity1_nn_chunk'], updated_json, info['entity2_nn_chunk'])
         return updated_tuple
     
     def remove_duplicates(self, data):
         seen = set()
         new_data = []
 
         for sublist in data:
```

### Comparing `querent-3.0.9/querent/kg/querent_kg.py` & `querent-3.1.0/querent/kg/querent_kg.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/kg/rel_helperfunctions/contextual_predicate.py` & `querent-3.1.0/querent/kg/rel_helperfunctions/contextual_predicate.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/kg/rel_helperfunctions/fixed_relationships.py` & `querent-3.1.0/querent/kg/rel_helperfunctions/fixed_relationships.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/kg/rel_helperfunctions/gpt_pydantic_classes.py` & `querent-3.1.0/querent/kg/rel_helperfunctions/gpt_pydantic_classes.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/kg/rel_helperfunctions/openai_functions.py` & `querent-3.1.0/querent/kg/rel_helperfunctions/openai_functions.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/kg/rel_helperfunctions/questionanswer_llama2.py` & `querent-3.1.0/querent/kg/rel_helperfunctions/questionanswer_llama2.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/kg/rel_helperfunctions/rel_normalize.py` & `querent-3.1.0/querent/kg/rel_helperfunctions/rel_normalize.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/kg/rel_helperfunctions/triple_to_json.py` & `querent-3.1.0/querent/kg/rel_helperfunctions/triple_to_json.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,19 +34,19 @@
         try:
             subject, json_str, object_ = triple
             predicate_info = TripleToJsonConverter._parse_json_str(json_str)
             if predicate_info is None:
                 return {}
 
             json_object = {
-                "subject": TripleToJsonConverter._normalize_text(subject),
+                "subject": TripleToJsonConverter._normalize_text(subject, replace_space=True),
                 "subject_type": TripleToJsonConverter._normalize_text(predicate_info.get("subject_type", "Unlabeled"), replace_space=True),
-                "object": TripleToJsonConverter._normalize_text(object_),
+                "object": TripleToJsonConverter._normalize_text(object_, replace_space=True),
                 "object_type": TripleToJsonConverter._normalize_text(predicate_info.get("object_type", "Unlabeled"), replace_space=True),
-                "predicate": TripleToJsonConverter._normalize_text(predicate_info.get("predicate", "")),
+                "predicate": TripleToJsonConverter._normalize_text(predicate_info.get("predicate", ""), replace_space=True),
                 "predicate_type": TripleToJsonConverter._normalize_text(predicate_info.get("predicate_type", "Unlabeled"), replace_space=True),
                 "sentence": predicate_info.get("context", "").lower()
             }
 
             return json_object
         except Exception as e:
             raise Exception(f"Error in convert_graphjson: {e}")
@@ -55,17 +55,17 @@
     def convert_vectorjson(triple, blob = None):
         try:
             subject, json_str, object_ = triple
             data = TripleToJsonConverter._parse_json_str(json_str)
             if data is None:
                 return {}
 
-            id_format = f"{TripleToJsonConverter._normalize_text(subject)}-{TripleToJsonConverter._normalize_text(data.get('predicate', ''))}-{TripleToJsonConverter._normalize_text(object_)}"
+            id_format = f"{TripleToJsonConverter._normalize_text(subject,replace_space=True)}-{TripleToJsonConverter._normalize_text(data.get('predicate', ''),replace_space=True)}-{TripleToJsonConverter._normalize_text(object_,replace_space=True)}"
             json_object = {
-                "id": TripleToJsonConverter._normalize_text(id_format,replace_space=True).replace(",","_"),
+                "id": TripleToJsonConverter._normalize_text(id_format),
                 "embeddings": data.get("context_embeddings", []),
                 "size": len(data.get("context_embeddings", [])),
                 "namespace": TripleToJsonConverter._normalize_text(data.get("predicate", ""),replace_space=True),
                 "sentence": data.get("context", "").lower(),
                 "blob": blob,
             }
 
@@ -73,12 +73,12 @@
         except Exception as e:
             raise Exception(f"Error in convert_vectorjson: {e}")
         
 
     @staticmethod
     def replace_special_chars_with_underscore(data):
         # This pattern will match anything that is not a letter, number, or underscore
-        pattern = r'[^-a-zA-Z0-9_]'
+        pattern = r'[^a-zA-Z0-9_]'
         # Replace matched patterns with an underscore
         return re.sub(pattern, '_', data)
```

### Comparing `querent-3.0.9/querent/logging/filters.py` & `querent-3.1.0/querent/logging/filters.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/logging/handlers.py` & `querent-3.1.0/querent/logging/handlers.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/logging/logger.py` & `querent-3.1.0/querent/logging/logger.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/metric/adapters/promethus_adapter.py` & `querent-3.1.0/querent/metric/adapters/promethus_adapter.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/metric/metric_logging_handler.py` & `querent-3.1.0/querent/metric/metric_logging_handler.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/metric/metric_registry.py` & `querent-3.1.0/querent/metric/metric_registry.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/processors/text_cleanup_processor.py` & `querent-3.1.0/querent/processors/text_cleanup_processor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/processors/text_processor.py` & `querent-3.1.0/querent/processors/text_processor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/querent/auto_scaler.py` & `querent-3.1.0/querent/querent/auto_scaler.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/querent/querent.py` & `querent-3.1.0/querent/querent/querent.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/querent/resource_manager.py` & `querent-3.1.0/querent/querent/resource_manager.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/storage/gcs_query.py` & `querent-3.1.0/querent/storage/gcs_query.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/storage/milvus_vectorevent_storage.py` & `querent-3.1.0/querent/storage/milvus_vectorevent_storage.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/storage/neo4j_graphevent_storage.py` & `querent-3.1.0/querent/storage/neo4j_graphevent_storage.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/storage/postgres_graphevent_storage.py` & `querent-3.1.0/querent/storage/postgres_graphevent_storage.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/tools/web_page_extractor.py` & `querent-3.1.0/querent/tools/web_page_extractor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/utils/webpage_extractor.py` & `querent-3.1.0/querent/utils/webpage_extractor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/workflow/_helpers.py` & `querent-3.1.0/querent/workflow/_helpers.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent/workflow/workflow.py` & `querent-3.1.0/querent/workflow/workflow.py`

 * *Files 24% similar despite different names*

```diff
@@ -34,14 +34,21 @@
             
             if engine_params.get("ner_model_name") is not None:
                 engine_params_json["ner_model_name"] = engine_params.get("ner_model_name")
             
             if engine_params.get("enable_filtering") is not None:
                 engine_params_json["enable_filtering"] = engine_params.get("enable_filtering")
             
+            if engine_params.get("fixed_relationships") is not None:
+                engine_params_json["fixed_relationships"] = [x for x in engine_params.get("fixed_relationships").split(",")]
+            
+            if engine_params.get("sample_relationships") is not None:
+                engine_params_json["sample_relationships"] = [x for x in engine_params.get("sample_relationships").split(",")]
+            
+            
             engine_params_json["filter_params"] = {
                 "score_threshold": float(engine_params.get("score_threshold")) if engine_params.get("score_threshold") is not None else None,
                 "attention_score_threshold": float(engine_params.get("attention_score_threshold")) if engine_params.get("attention_score_threshold") is not None else None,
                 "similarity_threshold": float(engine_params.get("similarity_threshold")) if engine_params.get("similarity_threshold") is not None else None,
                 "min_cluster_size": int(engine_params.get("min_cluster_size")) if engine_params.get("min_cluster_size") is not None else None,
                 "min_samples": int(engine_params.get("min_samples")) if engine_params.get("min_samples") is not None else None,
                 "cluster_persistence_threshold": float(engine_params.get("cluster_persistence_threshold")) if engine_params.get("cluster_persistence_threshold") is not None else None,
```

### Comparing `querent-3.0.9/querent.egg-info/PKG-INFO` & `querent-3.1.0/querent.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: querent
-Version: 3.0.9
+Version: 3.1.0
 Summary: The Asynchronous Data Dynamo and Graph Neural Network Catalyst
 Home-page: https://github.com/Querent-ai/querent-ai
 Author: Querent AI
 License: Business Source License 1.1
 Project-URL: Documentation, https://github.com/Querent-ai/querent-ai/docs
 Project-URL: Issue Tracker, https://github.com/Querent-ai/querent-ai/issues
 Keywords: Graph Neural Network,Scalability,Data-Driven Insights,GNN,Async,Knowledge Graphs,KG,Large Language Models,asyncio,Insights,aysnchronous,LLM,transformers,pytorch,Llama-index,AI,Artificial Intelligence,Neo4j,Queues,QuiAssisstant,Collectors,Data,Data Science,Data Engineering,Data Analysis,Data Analytics,News,NLP,Natural Language Processing,Text,Text Analysis,Deep Learning,Graphs,Graph Theory,Graph Algorithms,Graph Analytics,Graph Databases,Graph Processing,Graph Mining,Graph Neural Networks,GNN,GNNs,Graph Neural Network
```

### Comparing `querent-3.0.9/querent.egg-info/SOURCES.txt` & `querent-3.1.0/querent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/querent.egg-info/requires.txt` & `querent-3.1.0/querent.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `querent-3.0.9/setup.py` & `querent-3.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 ]
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="querent",
-    version="3.0.9",
+    version="3.1.0",
     author="Querent AI",
     description="The Asynchronous Data Dynamo and Graph Neural Network Catalyst",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Querent-ai/querent-ai",
     project_urls={
         "Documentation": "https://github.com/Querent-ai/querent-ai/docs",
```

