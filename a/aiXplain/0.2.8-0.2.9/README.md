# Comparing `tmp/aiXplain-0.2.8.tar.gz` & `tmp/aiXplain-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiXplain-0.2.8.tar", last modified: Wed Jan 17 15:16:00 2024, max compression
+gzip compressed data, was "aiXplain-0.2.9.tar", last modified: Thu Feb 15 19:47:59 2024, max compression
```

## Comparing `aiXplain-0.2.8.tar` & `aiXplain-0.2.9.tar`

### file list

```diff
@@ -1,179 +1,181 @@
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.241858 aiXplain-0.2.8/
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      198 2023-11-02 17:22:20.000000 aiXplain-0.2.8/.env.example
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1799 2023-11-02 17:22:20.000000 aiXplain-0.2.8/.gitignore
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      435 2023-11-02 17:22:20.000000 aiXplain-0.2.8/.pre-commit-config.yaml
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)    11357 2023-11-02 17:22:20.000000 aiXplain-0.2.8/LICENSE
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     5001 2024-01-17 15:16:00.241769 aiXplain-0.2.8/PKG-INFO
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     2937 2023-11-02 17:22:20.000000 aiXplain-0.2.8/README.md
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.241011 aiXplain-0.2.8/aiXplain.egg-info/
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     5001 2024-01-17 15:16:00.000000 aiXplain-0.2.8/aiXplain.egg-info/PKG-INFO
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     5229 2024-01-17 15:16:00.000000 aiXplain-0.2.8/aiXplain.egg-info/SOURCES.txt
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)        1 2024-01-17 15:16:00.000000 aiXplain-0.2.8/aiXplain.egg-info/dependency_links.txt
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)       57 2024-01-17 15:16:00.000000 aiXplain-0.2.8/aiXplain.egg-info/entry_points.txt
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      248 2024-01-17 15:16:00.000000 aiXplain-0.2.8/aiXplain.egg-info/requires.txt
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)        9 2024-01-17 15:16:00.000000 aiXplain-0.2.8/aiXplain.egg-info/top_level.txt
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.212978 aiXplain-0.2.8/aixplain/
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1340 2023-11-02 17:22:20.000000 aiXplain-0.2.8/aixplain/__init__.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1344 2023-11-02 17:22:20.000000 aiXplain-0.2.8/aixplain/cli_groups.py
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.213355 aiXplain-0.2.8/aixplain/decorators/
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)       43 2023-11-02 17:22:20.000000 aiXplain-0.2.8/aixplain/decorators/__init__.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      398 2023-11-02 17:22:20.000000 aiXplain-0.2.8/aixplain/decorators/api_key_checker.py
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.216228 aiXplain-0.2.8/aixplain/enums/
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      532 2023-12-19 21:15:52.000000 aiXplain-0.2.8/aixplain/enums/__init__.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      793 2023-11-02 17:22:20.000000 aiXplain-0.2.8/aixplain/enums/data_split.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      924 2023-11-02 17:22:20.000000 aiXplain-0.2.8/aixplain/enums/data_subtype.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      938 2023-11-02 17:22:20.000000 aiXplain-0.2.8/aixplain/enums/data_type.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      944 2023-11-02 17:22:20.000000 aiXplain-0.2.8/aixplain/enums/error_handler.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1007 2023-11-02 17:22:20.000000 aiXplain-0.2.8/aixplain/enums/file_type.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     2241 2023-11-02 17:22:20.000000 aiXplain-0.2.8/aixplain/enums/function.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     2162 2023-11-02 17:22:20.000000 aiXplain-0.2.8/aixplain/enums/language.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1935 2023-11-02 17:22:20.000000 aiXplain-0.2.8/aixplain/enums/license.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      837 2023-11-02 17:22:20.000000 aiXplain-0.2.8/aixplain/enums/onboard_status.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      839 2023-11-29 15:32:29.000000 aiXplain-0.2.8/aixplain/enums/ownership_type.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      796 2023-11-02 17:22:20.000000 aiXplain-0.2.8/aixplain/enums/privacy.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      816 2023-12-19 21:15:52.000000 aiXplain-0.2.8/aixplain/enums/sort_by.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      760 2023-12-19 21:15:52.000000 aiXplain-0.2.8/aixplain/enums/sort_order.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      832 2023-11-02 17:22:20.000000 aiXplain-0.2.8/aixplain/enums/storage_type.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     2053 2023-11-02 17:22:20.000000 aiXplain-0.2.8/aixplain/enums/supplier.py
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.218507 aiXplain-0.2.8/aixplain/factories/
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1105 2023-11-02 17:22:20.000000 aiXplain-0.2.8/aixplain/factories/__init__.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1250 2023-11-29 15:32:29.000000 aiXplain-0.2.8/aixplain/factories/asset_factory.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)    10421 2023-11-29 15:32:29.000000 aiXplain-0.2.8/aixplain/factories/benchmark_factory.py
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.218684 aiXplain-0.2.8/aixplain/factories/cli/
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     5454 2023-11-02 17:22:20.000000 aiXplain-0.2.8/aixplain/factories/cli/model_factory_cli.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)    14768 2023-11-29 15:32:29.000000 aiXplain-0.2.8/aixplain/factories/corpus_factory.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     3582 2023-11-29 15:32:29.000000 aiXplain-0.2.8/aixplain/factories/data_factory.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)    22124 2023-11-29 15:32:29.000000 aiXplain-0.2.8/aixplain/factories/dataset_factory.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     5387 2023-11-02 17:22:20.000000 aiXplain-0.2.8/aixplain/factories/file_factory.py
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.219185 aiXplain-0.2.8/aixplain/factories/finetune_factory/
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     5341 2024-01-17 15:12:00.000000 aiXplain-0.2.8/aixplain/factories/finetune_factory/__init__.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1724 2023-11-29 15:32:29.000000 aiXplain-0.2.8/aixplain/factories/finetune_factory/prompt_validator.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     5932 2023-11-29 15:32:29.000000 aiXplain-0.2.8/aixplain/factories/metric_factory.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)    17685 2024-01-10 14:13:03.000000 aiXplain-0.2.8/aixplain/factories/model_factory.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     8972 2023-11-29 15:32:29.000000 aiXplain-0.2.8/aixplain/factories/pipeline_factory.py
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.221743 aiXplain-0.2.8/aixplain/modules/
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1040 2023-11-29 15:32:29.000000 aiXplain-0.2.8/aixplain/modules/__init__.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     2388 2023-11-02 17:22:20.000000 aiXplain-0.2.8/aixplain/modules/asset.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     4491 2023-11-02 17:22:20.000000 aiXplain-0.2.8/aixplain/modules/benchmark.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     4201 2023-11-02 17:22:20.000000 aiXplain-0.2.8/aixplain/modules/benchmark_job.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1620 2023-11-02 17:22:20.000000 aiXplain-0.2.8/aixplain/modules/content_interval.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     3899 2023-12-19 21:15:52.000000 aiXplain-0.2.8/aixplain/modules/corpus.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     3505 2023-11-02 17:22:20.000000 aiXplain-0.2.8/aixplain/modules/data.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     6357 2023-12-19 21:15:52.000000 aiXplain-0.2.8/aixplain/modules/dataset.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1918 2023-11-02 17:22:20.000000 aiXplain-0.2.8/aixplain/modules/file.py
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.222371 aiXplain-0.2.8/aixplain/modules/finetune/
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     6511 2024-01-17 15:12:00.000000 aiXplain-0.2.8/aixplain/modules/finetune/__init__.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1681 2023-11-29 15:32:29.000000 aiXplain-0.2.8/aixplain/modules/finetune/cost.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     2193 2024-01-17 15:12:00.000000 aiXplain-0.2.8/aixplain/modules/finetune/hyperparameters.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     3663 2023-11-02 17:22:20.000000 aiXplain-0.2.8/aixplain/modules/metadata.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     4624 2023-11-02 17:22:20.000000 aiXplain-0.2.8/aixplain/modules/metric.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)    12080 2024-01-10 14:13:03.000000 aiXplain-0.2.8/aixplain/modules/model.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)    13346 2023-11-02 17:22:20.000000 aiXplain-0.2.8/aixplain/modules/pipeline.py
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.222587 aiXplain-0.2.8/aixplain/processes/
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)        0 2023-11-02 17:22:20.000000 aiXplain-0.2.8/aixplain/processes/__init__.py
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.223342 aiXplain-0.2.8/aixplain/processes/data_onboarding/
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)        0 2023-11-02 17:22:20.000000 aiXplain-0.2.8/aixplain/processes/data_onboarding/__init__.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)    14075 2023-12-19 21:15:52.000000 aiXplain-0.2.8/aixplain/processes/data_onboarding/onboard_functions.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     8284 2023-12-19 21:15:52.000000 aiXplain-0.2.8/aixplain/processes/data_onboarding/process_interval_files.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)    11930 2023-11-02 17:22:20.000000 aiXplain-0.2.8/aixplain/processes/data_onboarding/process_media_files.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     4626 2023-11-02 17:22:20.000000 aiXplain-0.2.8/aixplain/processes/data_onboarding/process_text_files.py
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.224311 aiXplain-0.2.8/aixplain/utils/
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      680 2023-11-02 17:22:20.000000 aiXplain-0.2.8/aixplain/utils/__init__.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1073 2023-11-02 17:22:20.000000 aiXplain-0.2.8/aixplain/utils/config.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1218 2023-11-02 17:22:20.000000 aiXplain-0.2.8/aixplain/utils/convert_datatype_utils.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     9681 2023-11-02 17:22:20.000000 aiXplain-0.2.8/aixplain/utils/file_utils.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      779 2023-11-02 17:22:20.000000 aiXplain-0.2.8/aixplain/utils/request_utils.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     4017 2023-11-02 17:22:20.000000 aiXplain-0.2.8/aixplain/utils/validation_utils.py
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.209289 aiXplain-0.2.8/docs/
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.226780 aiXplain-0.2.8/docs/assets/
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)    74843 2023-11-02 17:22:20.000000 aiXplain-0.2.8/docs/assets/aixplain-brandmark-line.png
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)   127670 2023-11-02 17:22:20.000000 aiXplain-0.2.8/docs/assets/data-onboard.png
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)   242066 2023-11-02 17:22:20.000000 aiXplain-0.2.8/docs/assets/designer-subtitling-sample.png
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)    36529 2023-11-02 17:22:20.000000 aiXplain-0.2.8/docs/assets/model-id-on-platform.png
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)    99855 2023-11-02 17:22:20.000000 aiXplain-0.2.8/docs/assets/navigate-api-key.png
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     3179 2023-11-02 17:22:20.000000 aiXplain-0.2.8/docs/assets/subtitle-generator-output.json
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.226930 aiXplain-0.2.8/docs/development/
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      694 2023-11-02 17:22:20.000000 aiXplain-0.2.8/docs/development/developer_guide.md
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.209093 aiXplain-0.2.8/docs/samples/
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.227253 aiXplain-0.2.8/docs/samples/corpus_onboarding/
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)    17854 2023-11-02 17:22:20.000000 aiXplain-0.2.8/docs/samples/corpus_onboarding/corpus_onboarding.ipynb
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     3976 2023-11-02 17:22:20.000000 aiXplain-0.2.8/docs/samples/corpus_onboarding/data.csv
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.227631 aiXplain-0.2.8/docs/samples/dataset_onboarding/
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     4122 2023-11-02 17:22:20.000000 aiXplain-0.2.8/docs/samples/dataset_onboarding/data.csv
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)    22698 2023-11-02 17:22:20.000000 aiXplain-0.2.8/docs/samples/dataset_onboarding/dataset_onboarding.ipynb
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.227958 aiXplain-0.2.8/docs/samples/subtitle_generator/
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1333 2023-11-02 17:22:20.000000 aiXplain-0.2.8/docs/samples/subtitle_generator/README.md
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     4197 2023-11-02 17:22:20.000000 aiXplain-0.2.8/docs/samples/subtitle_generator/subtitle_generator.py
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.229040 aiXplain-0.2.8/docs/streaming/
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     2922 2023-11-02 17:22:20.000000 aiXplain-0.2.8/docs/streaming/README.md
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     4831 2023-11-02 17:22:20.000000 aiXplain-0.2.8/docs/streaming/aixplain_diarization_streaming_client.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     6538 2023-11-02 17:22:20.000000 aiXplain-0.2.8/docs/streaming/aixplain_speech_transcription_streaming_client.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1346 2023-11-02 17:22:20.000000 aiXplain-0.2.8/docs/streaming/make_audio_compatible.py
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.231258 aiXplain-0.2.8/docs/streaming/proto/
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     5650 2023-11-02 17:22:20.000000 aiXplain-0.2.8/docs/streaming/proto/aixplain_diarization_streaming.proto
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     5578 2023-11-02 17:22:20.000000 aiXplain-0.2.8/docs/streaming/proto/aixplain_speech_transcription_streaming.proto
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)       36 2023-11-02 17:22:20.000000 aiXplain-0.2.8/docs/streaming/requirements.txt
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)  1000044 2023-11-02 17:22:20.000000 aiXplain-0.2.8/docs/streaming/test_dia.wav
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.232018 aiXplain-0.2.8/docs/user/
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      750 2023-11-02 17:22:20.000000 aiXplain-0.2.8/docs/user/api_setup.md
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)    22847 2023-11-29 15:32:29.000000 aiXplain-0.2.8/docs/user/user_doc.md
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     2145 2023-12-21 19:23:51.000000 aiXplain-0.2.8/pyproject.toml
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)       30 2023-11-02 17:22:20.000000 aiXplain-0.2.8/pytest.ini
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      107 2024-01-17 15:16:00.242084 aiXplain-0.2.8/setup.cfg
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.234480 aiXplain-0.2.8/tests/
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      680 2023-11-02 17:22:20.000000 aiXplain-0.2.8/tests/__init__.py
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.210113 aiXplain-0.2.8/tests/functional/
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.234636 aiXplain-0.2.8/tests/functional/benchmark/
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     3125 2023-12-19 21:15:52.000000 aiXplain-0.2.8/tests/functional/benchmark/benchmark_functional_test.py
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.235169 aiXplain-0.2.8/tests/functional/benchmark/data/
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)       67 2023-11-02 17:22:20.000000 aiXplain-0.2.8/tests/functional/benchmark/data/benchmark_module_test_data.json
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      291 2023-12-19 21:15:52.000000 aiXplain-0.2.8/tests/functional/benchmark/data/benchmark_test_run_data.json
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.235694 aiXplain-0.2.8/tests/functional/data_asset/
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)        0 2023-11-02 17:22:20.000000 aiXplain-0.2.8/tests/functional/data_asset/__init__.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     2247 2023-12-19 21:15:52.000000 aiXplain-0.2.8/tests/functional/data_asset/corpus_onboarding_test.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     4852 2023-12-19 21:15:52.000000 aiXplain-0.2.8/tests/functional/data_asset/dataset_onboarding_test.py
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.236388 aiXplain-0.2.8/tests/functional/data_asset/input/
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     4027 2023-11-02 17:22:20.000000 aiXplain-0.2.8/tests/functional/data_asset/input/audio-en_url.csv
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      246 2023-11-02 17:22:20.000000 aiXplain-0.2.8/tests/functional/data_asset/input/audio-en_with_invalid_split_url.csv
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     4179 2023-11-02 17:22:20.000000 aiXplain-0.2.8/tests/functional/data_asset/input/audio-en_with_split_url.csv
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.236687 aiXplain-0.2.8/tests/functional/file_asset/
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)        0 2023-11-02 17:22:20.000000 aiXplain-0.2.8/tests/functional/file_asset/__init__.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1278 2023-11-02 17:22:20.000000 aiXplain-0.2.8/tests/functional/file_asset/file_create_test.py
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.236838 aiXplain-0.2.8/tests/functional/file_asset/input/
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)       11 2023-11-02 17:22:20.000000 aiXplain-0.2.8/tests/functional/file_asset/input/test.csv
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.237079 aiXplain-0.2.8/tests/functional/finetune/
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)        0 2023-11-02 17:22:20.000000 aiXplain-0.2.8/tests/functional/finetune/__init__.py
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.238084 aiXplain-0.2.8/tests/functional/finetune/data/
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      367 2024-01-17 15:12:00.000000 aiXplain-0.2.8/tests/functional/finetune/data/finetune_test_cost_estimation.json
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      423 2024-01-17 15:12:00.000000 aiXplain-0.2.8/tests/functional/finetune/data/finetune_test_end2end.json
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)       95 2023-11-29 15:32:29.000000 aiXplain-0.2.8/tests/functional/finetune/data/finetune_test_list_data.json
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      400 2023-11-29 15:32:29.000000 aiXplain-0.2.8/tests/functional/finetune/data/finetune_test_prompt_validator.json
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     4834 2023-12-19 21:15:52.000000 aiXplain-0.2.8/tests/functional/finetune/finetune_functional_test.py
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.238231 aiXplain-0.2.8/tests/functional/general_assets/
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     3267 2024-01-17 15:12:00.000000 aiXplain-0.2.8/tests/functional/general_assets/asset_functional_test.py
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.238412 aiXplain-0.2.8/tests/functional/general_assets/data/
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      391 2024-01-17 15:12:00.000000 aiXplain-0.2.8/tests/functional/general_assets/data/asset_run_test_data.json
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.238575 aiXplain-0.2.8/tests/functional/pipelines/
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     3805 2023-11-02 17:22:20.000000 aiXplain-0.2.8/tests/functional/pipelines/run_test.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     3040 2023-11-29 15:32:29.000000 aiXplain-0.2.8/tests/image_upload_e2e_test.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     2550 2023-11-02 17:22:20.000000 aiXplain-0.2.8/tests/image_upload_functional_test.py
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     3234 2023-11-02 17:22:20.000000 aiXplain-0.2.8/tests/image_upload_test.py
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.239466 aiXplain-0.2.8/tests/mock_responses/
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)       27 2023-11-02 17:22:20.000000 aiXplain-0.2.8/tests/mock_responses/create_asset_repo_response.json
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)    95980 2023-11-02 17:22:20.000000 aiXplain-0.2.8/tests/mock_responses/list_functions_response.json
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      368 2023-11-02 17:22:20.000000 aiXplain-0.2.8/tests/mock_responses/list_host_machines_response.json
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)       32 2023-11-02 17:22:20.000000 aiXplain-0.2.8/tests/mock_responses/list_image_repo_tags_response.json
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     2261 2023-11-02 17:22:20.000000 aiXplain-0.2.8/tests/mock_responses/login_response.json
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.239620 aiXplain-0.2.8/tests/test_requests/
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      201 2023-11-02 17:22:20.000000 aiXplain-0.2.8/tests/test_requests/create_asset_request.json
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      738 2023-11-02 17:22:20.000000 aiXplain-0.2.8/tests/test_utils.py
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.239974 aiXplain-0.2.8/tests/unit/
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.240136 aiXplain-0.2.8/tests/unit/data/
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      222 2023-11-02 17:22:20.000000 aiXplain-0.2.8/tests/unit/data/create_finetune_percentage_exception.json
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     4583 2023-11-02 17:22:20.000000 aiXplain-0.2.8/tests/unit/finetune_test.py
-drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-01-17 15:16:00.240805 aiXplain-0.2.8/tests/unit/mock_responses/
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      676 2023-11-02 17:22:20.000000 aiXplain-0.2.8/tests/unit/mock_responses/cost_estimation_response.json
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)       54 2023-11-02 17:22:20.000000 aiXplain-0.2.8/tests/unit/mock_responses/finetune_response.json
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)    43263 2023-11-02 17:22:20.000000 aiXplain-0.2.8/tests/unit/mock_responses/list_models_response.json
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     3335 2023-11-02 17:22:20.000000 aiXplain-0.2.8/tests/unit/mock_responses/model_response.json
--rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     2350 2023-11-02 17:22:20.000000 aiXplain-0.2.8/tests/unit/model_test.py
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.211420 aiXplain-0.2.9/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      198 2023-11-02 17:22:20.000000 aiXplain-0.2.9/.env.example
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1799 2023-11-02 17:22:20.000000 aiXplain-0.2.9/.gitignore
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      435 2023-11-02 17:22:20.000000 aiXplain-0.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)    11357 2023-11-02 17:22:20.000000 aiXplain-0.2.9/LICENSE
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     5001 2024-02-15 19:47:59.211346 aiXplain-0.2.9/PKG-INFO
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     2937 2023-11-02 17:22:20.000000 aiXplain-0.2.9/README.md
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.210621 aiXplain-0.2.9/aiXplain.egg-info/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     5001 2024-02-15 19:47:59.000000 aiXplain-0.2.9/aiXplain.egg-info/PKG-INFO
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     5274 2024-02-15 19:47:59.000000 aiXplain-0.2.9/aiXplain.egg-info/SOURCES.txt
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)        1 2024-02-15 19:47:59.000000 aiXplain-0.2.9/aiXplain.egg-info/dependency_links.txt
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)       57 2024-02-15 19:47:59.000000 aiXplain-0.2.9/aiXplain.egg-info/entry_points.txt
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      248 2024-02-15 19:47:59.000000 aiXplain-0.2.9/aiXplain.egg-info/requires.txt
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)       15 2024-02-15 19:47:59.000000 aiXplain-0.2.9/aiXplain.egg-info/top_level.txt
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.179243 aiXplain-0.2.9/aixplain/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1340 2023-11-02 17:22:20.000000 aiXplain-0.2.9/aixplain/__init__.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1493 2024-01-23 12:26:44.000000 aiXplain-0.2.9/aixplain/cli_groups.py
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.179696 aiXplain-0.2.9/aixplain/decorators/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)       43 2023-11-02 17:22:20.000000 aiXplain-0.2.9/aixplain/decorators/__init__.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      398 2023-11-02 17:22:20.000000 aiXplain-0.2.9/aixplain/decorators/api_key_checker.py
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.182675 aiXplain-0.2.9/aixplain/enums/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      532 2023-12-19 21:15:52.000000 aiXplain-0.2.9/aixplain/enums/__init__.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      793 2023-11-02 17:22:20.000000 aiXplain-0.2.9/aixplain/enums/data_split.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      924 2023-11-02 17:22:20.000000 aiXplain-0.2.9/aixplain/enums/data_subtype.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      938 2023-11-02 17:22:20.000000 aiXplain-0.2.9/aixplain/enums/data_type.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      944 2023-11-02 17:22:20.000000 aiXplain-0.2.9/aixplain/enums/error_handler.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1007 2023-11-02 17:22:20.000000 aiXplain-0.2.9/aixplain/enums/file_type.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     2241 2023-11-02 17:22:20.000000 aiXplain-0.2.9/aixplain/enums/function.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     2162 2023-11-02 17:22:20.000000 aiXplain-0.2.9/aixplain/enums/language.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1935 2023-11-02 17:22:20.000000 aiXplain-0.2.9/aixplain/enums/license.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      837 2023-11-02 17:22:20.000000 aiXplain-0.2.9/aixplain/enums/onboard_status.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      839 2023-11-29 15:32:29.000000 aiXplain-0.2.9/aixplain/enums/ownership_type.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      796 2023-11-02 17:22:20.000000 aiXplain-0.2.9/aixplain/enums/privacy.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      816 2023-12-19 21:15:52.000000 aiXplain-0.2.9/aixplain/enums/sort_by.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      760 2023-12-19 21:15:52.000000 aiXplain-0.2.9/aixplain/enums/sort_order.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      832 2023-11-02 17:22:20.000000 aiXplain-0.2.9/aixplain/enums/storage_type.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     2053 2023-11-02 17:22:20.000000 aiXplain-0.2.9/aixplain/enums/supplier.py
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.185655 aiXplain-0.2.9/aixplain/factories/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1105 2023-11-02 17:22:20.000000 aiXplain-0.2.9/aixplain/factories/__init__.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1250 2023-11-29 15:32:29.000000 aiXplain-0.2.9/aixplain/factories/asset_factory.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)    10421 2023-11-29 15:32:29.000000 aiXplain-0.2.9/aixplain/factories/benchmark_factory.py
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.185939 aiXplain-0.2.9/aixplain/factories/cli/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     7174 2024-01-23 12:26:44.000000 aiXplain-0.2.9/aixplain/factories/cli/model_factory_cli.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)    14768 2024-02-15 19:46:06.000000 aiXplain-0.2.9/aixplain/factories/corpus_factory.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     3582 2023-11-29 15:32:29.000000 aiXplain-0.2.9/aixplain/factories/data_factory.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)    22124 2024-02-15 19:46:06.000000 aiXplain-0.2.9/aixplain/factories/dataset_factory.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     5387 2023-11-02 17:22:20.000000 aiXplain-0.2.9/aixplain/factories/file_factory.py
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.186488 aiXplain-0.2.9/aixplain/factories/finetune_factory/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     5341 2024-01-17 15:12:00.000000 aiXplain-0.2.9/aixplain/factories/finetune_factory/__init__.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1724 2023-11-29 15:32:29.000000 aiXplain-0.2.9/aixplain/factories/finetune_factory/prompt_validator.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     5932 2023-11-29 15:32:29.000000 aiXplain-0.2.9/aixplain/factories/metric_factory.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)    20582 2024-01-23 12:26:44.000000 aiXplain-0.2.9/aixplain/factories/model_factory.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     8972 2023-11-29 15:32:29.000000 aiXplain-0.2.9/aixplain/factories/pipeline_factory.py
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.189209 aiXplain-0.2.9/aixplain/modules/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1040 2023-11-29 15:32:29.000000 aiXplain-0.2.9/aixplain/modules/__init__.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     2388 2023-11-02 17:22:20.000000 aiXplain-0.2.9/aixplain/modules/asset.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     4491 2023-11-02 17:22:20.000000 aiXplain-0.2.9/aixplain/modules/benchmark.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     4201 2023-11-02 17:22:20.000000 aiXplain-0.2.9/aixplain/modules/benchmark_job.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1620 2023-11-02 17:22:20.000000 aiXplain-0.2.9/aixplain/modules/content_interval.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     3899 2023-12-19 21:15:52.000000 aiXplain-0.2.9/aixplain/modules/corpus.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     3505 2023-11-02 17:22:20.000000 aiXplain-0.2.9/aixplain/modules/data.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     6357 2023-12-19 21:15:52.000000 aiXplain-0.2.9/aixplain/modules/dataset.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1918 2023-11-02 17:22:20.000000 aiXplain-0.2.9/aixplain/modules/file.py
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.189820 aiXplain-0.2.9/aixplain/modules/finetune/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     6511 2024-01-17 15:12:00.000000 aiXplain-0.2.9/aixplain/modules/finetune/__init__.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1681 2023-11-29 15:32:29.000000 aiXplain-0.2.9/aixplain/modules/finetune/cost.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     2193 2024-02-15 19:46:06.000000 aiXplain-0.2.9/aixplain/modules/finetune/hyperparameters.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     3663 2023-11-02 17:22:20.000000 aiXplain-0.2.9/aixplain/modules/metadata.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     4624 2023-11-02 17:22:20.000000 aiXplain-0.2.9/aixplain/modules/metric.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)    12080 2024-01-10 14:13:03.000000 aiXplain-0.2.9/aixplain/modules/model.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)    13346 2023-11-02 17:22:20.000000 aiXplain-0.2.9/aixplain/modules/pipeline.py
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.190160 aiXplain-0.2.9/aixplain/processes/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)        0 2023-11-02 17:22:20.000000 aiXplain-0.2.9/aixplain/processes/__init__.py
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.191166 aiXplain-0.2.9/aixplain/processes/data_onboarding/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)        0 2023-11-02 17:22:20.000000 aiXplain-0.2.9/aixplain/processes/data_onboarding/__init__.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)    14075 2024-02-15 19:46:06.000000 aiXplain-0.2.9/aixplain/processes/data_onboarding/onboard_functions.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     8284 2023-12-19 21:15:52.000000 aiXplain-0.2.9/aixplain/processes/data_onboarding/process_interval_files.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)    11930 2023-11-02 17:22:20.000000 aiXplain-0.2.9/aixplain/processes/data_onboarding/process_media_files.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     4626 2024-02-15 19:46:06.000000 aiXplain-0.2.9/aixplain/processes/data_onboarding/process_text_files.py
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.192273 aiXplain-0.2.9/aixplain/utils/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      680 2023-11-02 17:22:20.000000 aiXplain-0.2.9/aixplain/utils/__init__.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1073 2024-02-15 19:46:06.000000 aiXplain-0.2.9/aixplain/utils/config.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1218 2023-11-02 17:22:20.000000 aiXplain-0.2.9/aixplain/utils/convert_datatype_utils.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     9681 2023-11-02 17:22:20.000000 aiXplain-0.2.9/aixplain/utils/file_utils.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      779 2023-11-02 17:22:20.000000 aiXplain-0.2.9/aixplain/utils/request_utils.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     4017 2023-11-02 17:22:20.000000 aiXplain-0.2.9/aixplain/utils/validation_utils.py
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.174922 aiXplain-0.2.9/docs/
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.194140 aiXplain-0.2.9/docs/assets/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)    74843 2023-11-02 17:22:20.000000 aiXplain-0.2.9/docs/assets/aixplain-brandmark-line.png
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)   127670 2023-11-02 17:22:20.000000 aiXplain-0.2.9/docs/assets/data-onboard.png
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)   242066 2023-11-02 17:22:20.000000 aiXplain-0.2.9/docs/assets/designer-subtitling-sample.png
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)    36529 2023-11-02 17:22:20.000000 aiXplain-0.2.9/docs/assets/model-id-on-platform.png
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)    99855 2023-11-02 17:22:20.000000 aiXplain-0.2.9/docs/assets/navigate-api-key.png
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     3179 2023-11-02 17:22:20.000000 aiXplain-0.2.9/docs/assets/subtitle-generator-output.json
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.194400 aiXplain-0.2.9/docs/development/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      694 2023-11-02 17:22:20.000000 aiXplain-0.2.9/docs/development/developer_guide.md
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.174727 aiXplain-0.2.9/docs/samples/
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.194722 aiXplain-0.2.9/docs/samples/corpus_onboarding/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)    17854 2023-11-02 17:22:20.000000 aiXplain-0.2.9/docs/samples/corpus_onboarding/corpus_onboarding.ipynb
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     3976 2023-11-02 17:22:20.000000 aiXplain-0.2.9/docs/samples/corpus_onboarding/data.csv
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.195127 aiXplain-0.2.9/docs/samples/dataset_onboarding/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     4122 2023-11-02 17:22:20.000000 aiXplain-0.2.9/docs/samples/dataset_onboarding/data.csv
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)    22698 2023-11-02 17:22:20.000000 aiXplain-0.2.9/docs/samples/dataset_onboarding/dataset_onboarding.ipynb
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.195459 aiXplain-0.2.9/docs/samples/subtitle_generator/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1333 2023-11-02 17:22:20.000000 aiXplain-0.2.9/docs/samples/subtitle_generator/README.md
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     4197 2023-11-02 17:22:20.000000 aiXplain-0.2.9/docs/samples/subtitle_generator/subtitle_generator.py
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.196628 aiXplain-0.2.9/docs/streaming/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     2922 2023-11-02 17:22:20.000000 aiXplain-0.2.9/docs/streaming/README.md
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     4831 2023-11-02 17:22:20.000000 aiXplain-0.2.9/docs/streaming/aixplain_diarization_streaming_client.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     6538 2023-11-02 17:22:20.000000 aiXplain-0.2.9/docs/streaming/aixplain_speech_transcription_streaming_client.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1346 2023-11-02 17:22:20.000000 aiXplain-0.2.9/docs/streaming/make_audio_compatible.py
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.198464 aiXplain-0.2.9/docs/streaming/proto/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     5650 2023-11-02 17:22:20.000000 aiXplain-0.2.9/docs/streaming/proto/aixplain_diarization_streaming.proto
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     5578 2023-11-02 17:22:20.000000 aiXplain-0.2.9/docs/streaming/proto/aixplain_speech_transcription_streaming.proto
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)       36 2023-11-02 17:22:20.000000 aiXplain-0.2.9/docs/streaming/requirements.txt
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)  1000044 2023-11-02 17:22:20.000000 aiXplain-0.2.9/docs/streaming/test_dia.wav
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.200108 aiXplain-0.2.9/docs/user/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      750 2023-11-02 17:22:20.000000 aiXplain-0.2.9/docs/user/api_setup.md
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)    23791 2024-01-23 12:26:44.000000 aiXplain-0.2.9/docs/user/user_doc.md
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     2154 2024-02-15 19:46:22.000000 aiXplain-0.2.9/pyproject.toml
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)       30 2023-11-02 17:22:20.000000 aiXplain-0.2.9/pytest.ini
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      107 2024-02-15 19:47:59.211640 aiXplain-0.2.9/setup.cfg
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.203363 aiXplain-0.2.9/tests/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      680 2023-11-02 17:22:20.000000 aiXplain-0.2.9/tests/__init__.py
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.176007 aiXplain-0.2.9/tests/functional/
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.203555 aiXplain-0.2.9/tests/functional/benchmark/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     3125 2024-01-30 18:26:45.000000 aiXplain-0.2.9/tests/functional/benchmark/benchmark_functional_test.py
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.203995 aiXplain-0.2.9/tests/functional/benchmark/data/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)       67 2023-11-02 17:22:20.000000 aiXplain-0.2.9/tests/functional/benchmark/data/benchmark_module_test_data.json
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      291 2023-12-19 21:15:52.000000 aiXplain-0.2.9/tests/functional/benchmark/data/benchmark_test_run_data.json
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.204584 aiXplain-0.2.9/tests/functional/data_asset/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)        0 2023-11-02 17:22:20.000000 aiXplain-0.2.9/tests/functional/data_asset/__init__.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     2247 2023-12-19 21:15:52.000000 aiXplain-0.2.9/tests/functional/data_asset/corpus_onboarding_test.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     4852 2023-12-19 21:15:52.000000 aiXplain-0.2.9/tests/functional/data_asset/dataset_onboarding_test.py
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.205120 aiXplain-0.2.9/tests/functional/data_asset/input/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     4027 2023-11-02 17:22:20.000000 aiXplain-0.2.9/tests/functional/data_asset/input/audio-en_url.csv
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      246 2023-11-02 17:22:20.000000 aiXplain-0.2.9/tests/functional/data_asset/input/audio-en_with_invalid_split_url.csv
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     4179 2023-11-02 17:22:20.000000 aiXplain-0.2.9/tests/functional/data_asset/input/audio-en_with_split_url.csv
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.205420 aiXplain-0.2.9/tests/functional/file_asset/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)        0 2023-11-02 17:22:20.000000 aiXplain-0.2.9/tests/functional/file_asset/__init__.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1278 2023-11-02 17:22:20.000000 aiXplain-0.2.9/tests/functional/file_asset/file_create_test.py
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.205556 aiXplain-0.2.9/tests/functional/file_asset/input/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)       11 2023-11-02 17:22:20.000000 aiXplain-0.2.9/tests/functional/file_asset/input/test.csv
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.205784 aiXplain-0.2.9/tests/functional/finetune/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)        0 2023-11-02 17:22:20.000000 aiXplain-0.2.9/tests/functional/finetune/__init__.py
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.206817 aiXplain-0.2.9/tests/functional/finetune/data/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      367 2024-02-15 19:46:06.000000 aiXplain-0.2.9/tests/functional/finetune/data/finetune_test_cost_estimation.json
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      423 2024-01-17 15:12:00.000000 aiXplain-0.2.9/tests/functional/finetune/data/finetune_test_end2end.json
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)       95 2023-11-29 15:32:29.000000 aiXplain-0.2.9/tests/functional/finetune/data/finetune_test_list_data.json
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      400 2024-02-15 19:46:06.000000 aiXplain-0.2.9/tests/functional/finetune/data/finetune_test_prompt_validator.json
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     4834 2024-02-15 19:46:06.000000 aiXplain-0.2.9/tests/functional/finetune/finetune_functional_test.py
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.207044 aiXplain-0.2.9/tests/functional/general_assets/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     3267 2024-01-17 15:12:00.000000 aiXplain-0.2.9/tests/functional/general_assets/asset_functional_test.py
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.207398 aiXplain-0.2.9/tests/functional/general_assets/data/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      391 2024-01-17 15:12:00.000000 aiXplain-0.2.9/tests/functional/general_assets/data/asset_run_test_data.json
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.207672 aiXplain-0.2.9/tests/functional/model/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1486 2024-02-15 19:46:06.000000 aiXplain-0.2.9/tests/functional/model/hf_onboarding_test.py
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.207898 aiXplain-0.2.9/tests/functional/pipelines/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     3805 2023-11-02 17:22:20.000000 aiXplain-0.2.9/tests/functional/pipelines/run_test.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     3040 2023-11-29 15:32:29.000000 aiXplain-0.2.9/tests/image_upload_e2e_test.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     2550 2023-11-02 17:22:20.000000 aiXplain-0.2.9/tests/image_upload_functional_test.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     3234 2023-11-02 17:22:20.000000 aiXplain-0.2.9/tests/image_upload_test.py
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.208753 aiXplain-0.2.9/tests/mock_responses/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)       27 2023-11-02 17:22:20.000000 aiXplain-0.2.9/tests/mock_responses/create_asset_repo_response.json
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)    95980 2023-11-02 17:22:20.000000 aiXplain-0.2.9/tests/mock_responses/list_functions_response.json
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      368 2023-11-02 17:22:20.000000 aiXplain-0.2.9/tests/mock_responses/list_host_machines_response.json
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)       32 2023-11-02 17:22:20.000000 aiXplain-0.2.9/tests/mock_responses/list_image_repo_tags_response.json
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     2261 2023-11-02 17:22:20.000000 aiXplain-0.2.9/tests/mock_responses/login_response.json
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.209078 aiXplain-0.2.9/tests/test_requests/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      201 2023-11-02 17:22:20.000000 aiXplain-0.2.9/tests/test_requests/create_asset_request.json
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      738 2023-11-02 17:22:20.000000 aiXplain-0.2.9/tests/test_utils.py
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.209404 aiXplain-0.2.9/tests/unit/
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.209645 aiXplain-0.2.9/tests/unit/data/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      222 2023-11-02 17:22:20.000000 aiXplain-0.2.9/tests/unit/data/create_finetune_percentage_exception.json
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     4583 2023-11-02 17:22:20.000000 aiXplain-0.2.9/tests/unit/finetune_test.py
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2024-02-15 19:47:59.210440 aiXplain-0.2.9/tests/unit/mock_responses/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      676 2023-11-02 17:22:20.000000 aiXplain-0.2.9/tests/unit/mock_responses/cost_estimation_response.json
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)       54 2023-11-02 17:22:20.000000 aiXplain-0.2.9/tests/unit/mock_responses/finetune_response.json
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)    43263 2023-11-02 17:22:20.000000 aiXplain-0.2.9/tests/unit/mock_responses/list_models_response.json
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     3335 2023-11-02 17:22:20.000000 aiXplain-0.2.9/tests/unit/mock_responses/model_response.json
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     2350 2023-11-02 17:22:20.000000 aiXplain-0.2.9/tests/unit/model_test.py
```

### Comparing `aiXplain-0.2.8/.gitignore` & `aiXplain-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/LICENSE` & `aiXplain-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/PKG-INFO` & `aiXplain-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiXplain
-Version: 0.2.8
+Version: 0.2.9
 Summary: aiXplain SDK adds AI functions to software.
 Author-email: thiago.ferreira@aixplain.com, krishna.durai@aixplain.com, lucas.pavanelli@aixplain.com
 License: Apache License, Version 2.0: http://www.apache.org/licenses/LICENSE-2.0
 Project-URL: Homepage, https://github.com/aixplain/aiXplain
 Project-URL: Documentation, https://github.com/aixplain/pipelines/tree/main/docs
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Web Environment
```

### Comparing `aiXplain-0.2.8/README.md` & `aiXplain-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aiXplain.egg-info/PKG-INFO` & `aiXplain-0.2.9/aiXplain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiXplain
-Version: 0.2.8
+Version: 0.2.9
 Summary: aiXplain SDK adds AI functions to software.
 Author-email: thiago.ferreira@aixplain.com, krishna.durai@aixplain.com, lucas.pavanelli@aixplain.com
 License: Apache License, Version 2.0: http://www.apache.org/licenses/LICENSE-2.0
 Project-URL: Homepage, https://github.com/aixplain/aiXplain
 Project-URL: Documentation, https://github.com/aixplain/pipelines/tree/main/docs
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Web Environment
```

### Comparing `aiXplain-0.2.8/aiXplain.egg-info/SOURCES.txt` & `aiXplain-0.2.9/aiXplain.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -117,14 +117,15 @@
 tests/functional/finetune/finetune_functional_test.py
 tests/functional/finetune/data/finetune_test_cost_estimation.json
 tests/functional/finetune/data/finetune_test_end2end.json
 tests/functional/finetune/data/finetune_test_list_data.json
 tests/functional/finetune/data/finetune_test_prompt_validator.json
 tests/functional/general_assets/asset_functional_test.py
 tests/functional/general_assets/data/asset_run_test_data.json
+tests/functional/model/hf_onboarding_test.py
 tests/functional/pipelines/run_test.py
 tests/mock_responses/create_asset_repo_response.json
 tests/mock_responses/list_functions_response.json
 tests/mock_responses/list_host_machines_response.json
 tests/mock_responses/list_image_repo_tags_response.json
 tests/mock_responses/login_response.json
 tests/test_requests/create_asset_request.json
```

### Comparing `aiXplain-0.2.8/aixplain/__init__.py` & `aiXplain-0.2.9/aixplain/__init__.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/cli_groups.py` & `aiXplain-0.2.9/aixplain/cli_groups.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 Author: Michael Lam
 Date: September 18th 2023
 Description:
     CLI Runner
 """
 import click
-from aixplain.factories.cli.model_factory_cli import list_host_machines, list_functions, create_asset_repo, asset_repo_login, onboard_model
+from aixplain.factories.cli.model_factory_cli import list_host_machines, list_functions, create_asset_repo, asset_repo_login, onboard_model, deploy_huggingface_model, get_huggingface_model_status
 
 @click.group('cli')
 def cli():
     pass
 
 @click.group('list')
 def list():
@@ -48,11 +48,14 @@
 cli.add_command(create)
 cli.add_command(onboard)
 
 create.add_command(create_asset_repo)
 list.add_command(list_host_machines)
 list.add_command(list_functions)
 get.add_command(asset_repo_login)
+get.add_command(get_huggingface_model_status)
 onboard.add_command(onboard_model)
+onboard.add_command(deploy_huggingface_model)
+
 
 def run_cli():
     cli()
```

### Comparing `aiXplain-0.2.8/aixplain/enums/__init__.py` & `aiXplain-0.2.9/aixplain/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/enums/data_split.py` & `aiXplain-0.2.9/aixplain/enums/data_split.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/enums/data_subtype.py` & `aiXplain-0.2.9/aixplain/enums/data_subtype.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/enums/data_type.py` & `aiXplain-0.2.9/aixplain/enums/data_type.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/enums/error_handler.py` & `aiXplain-0.2.9/aixplain/enums/error_handler.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/enums/file_type.py` & `aiXplain-0.2.9/aixplain/enums/file_type.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/enums/function.py` & `aiXplain-0.2.9/aixplain/enums/function.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/enums/language.py` & `aiXplain-0.2.9/aixplain/enums/language.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/enums/license.py` & `aiXplain-0.2.9/aixplain/enums/license.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/enums/onboard_status.py` & `aiXplain-0.2.9/aixplain/enums/onboard_status.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/enums/ownership_type.py` & `aiXplain-0.2.9/aixplain/enums/ownership_type.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/enums/privacy.py` & `aiXplain-0.2.9/aixplain/enums/privacy.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/enums/sort_by.py` & `aiXplain-0.2.9/aixplain/enums/sort_by.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/enums/sort_order.py` & `aiXplain-0.2.9/aixplain/enums/sort_order.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/enums/storage_type.py` & `aiXplain-0.2.9/aixplain/enums/storage_type.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/enums/supplier.py` & `aiXplain-0.2.9/aixplain/enums/supplier.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/factories/__init__.py` & `aiXplain-0.2.9/aixplain/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/factories/asset_factory.py` & `aiXplain-0.2.9/aixplain/factories/asset_factory.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/factories/benchmark_factory.py` & `aiXplain-0.2.9/aixplain/factories/benchmark_factory.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/factories/cli/model_factory_cli.py` & `aiXplain-0.2.9/aixplain/factories/cli/model_factory_cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -131,7 +131,45 @@
 
     Returns:
         None
     """   
     ret_val = ModelFactory.onboard_model(model_id, image_tag, image_hash, api_key)
     ret_val_yaml = yaml.dump(ret_val)
     click.echo(ret_val_yaml)
+
+@click.command("hf-model")
+@click.option("--name", help="User-defined name for Hugging Face model.")
+@click.option("--hf-repo-id", help="Repository ID from Hugging Face in {supplier}/{model name} form.")
+@click.option("--hf-token", help="Hugging Face token used to authenticate to this model.")
+@click.option("--api-key", default=None, help="TEAM_API_KEY if not already set in environment.")
+def deploy_huggingface_model(name: Text, hf_repo_id: Text, 
+                             hf_token: Optional[Text] = None, 
+                             api_key: Optional[Text] = None) -> None:
+    """CLI wrapper function for the DEPLOY_HUGGINGFACE_MODEL function in ModelFactory.
+
+    Args:
+        name (Text): User-defined name for Hugging Face model.
+        api_key (Text, optional): Team API key. Defaults to None.
+
+    Returns:
+        None
+    """
+    ret_val = ModelFactory.deploy_huggingface_model(name, hf_repo_id, hf_token, api_key)
+    ret_val_yaml = yaml.dump(ret_val)
+    click.echo(ret_val_yaml)
+
+@click.command("hf-model-status")
+@click.option("--model-id", help="Model ID from DEPLOY_HUGGINGFACE_MODEL.")
+@click.option("--api-key", default=None, help="TEAM_API_KEY if not already set in environment.")
+def get_huggingface_model_status(model_id: Text, api_key: Optional[Text] = None) -> None:
+    """CLI wrapper function for the GET_HUGGINGFACE_MODEL_STATUS function in ModelFactory.
+
+    Args:
+        model_id (Text): Model ID obtained from DEPLOY_HUGGINGFACE_MODEL.
+        api_key (Text, optional): Team API key. Defaults to None.
+
+    Returns:
+        None
+    """
+    ret_val = ModelFactory.get_huggingface_model_status(model_id, api_key)
+    ret_val_yaml = yaml.dump(ret_val)
+    click.echo(ret_val_yaml)
```

### Comparing `aiXplain-0.2.8/aixplain/factories/corpus_factory.py` & `aiXplain-0.2.9/aixplain/factories/corpus_factory.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/factories/data_factory.py` & `aiXplain-0.2.9/aixplain/factories/data_factory.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/factories/dataset_factory.py` & `aiXplain-0.2.9/aixplain/factories/dataset_factory.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/factories/file_factory.py` & `aiXplain-0.2.9/aixplain/factories/file_factory.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/factories/finetune_factory/__init__.py` & `aiXplain-0.2.9/aixplain/factories/finetune_factory/__init__.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/factories/finetune_factory/prompt_validator.py` & `aiXplain-0.2.9/aixplain/factories/finetune_factory/prompt_validator.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/factories/metric_factory.py` & `aiXplain-0.2.9/aixplain/factories/metric_factory.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/factories/model_factory.py` & `aiXplain-0.2.9/aixplain/factories/model_factory.py`

 * *Files 7% similar despite different names*

```diff
@@ -400,7 +400,72 @@
         payload = {"image": image_tag, "sha": image_hash}
         payload = json.dumps(payload)
         logging.debug(f"Body: {str(payload)}")
         response = _request_with_retry("post", onboard_url, headers=headers, data=payload)
         message = "Your onboarding request has been submitted to an aiXplain specialist for finalization. We will notify you when the process is completed."
         logging.info(message)
         return response
+    
+    @classmethod
+    def deploy_huggingface_model(cls, name: Text, hf_repo_id: Text, hf_token: Optional[Text] = "", api_key: Optional[Text] = None) -> Dict:
+        """Onboards and deploys a Hugging Face large language model.
+
+        Args:
+            name (Text): The user's name for the model.
+            hf_repo_id (Text): The Hugging Face repository ID for this model ({author}/{model name}).
+            hf_token (Text, optional): Hugging Face access token. Defaults to None.
+            api_key (Text, optional): Team API key. Defaults to None.
+        Returns:
+            Dict: Backend response
+        """
+        supplier, model_name = hf_repo_id.split("/")
+        deploy_url = urljoin(config.BACKEND_URL, f"sdk/model-onboarding/onboard")
+        if api_key:
+            headers = {"Authorization": f"Token {api_key}", "Content-Type": "application/json"}
+        else:
+            headers = {"Authorization": f"Token {config.TEAM_API_KEY}", "Content-Type": "application/json"}
+        body = {
+            "model": {
+                "name": name,
+                "description": "A user-deployed Hugging Face model",
+                "connectionType": ["synchronous"],
+                "function": "text-generation",
+                "documentationUrl": "aiXplain",
+                "sourceLanguage": "en",
+            },
+            "source": "huggingface",
+            "onboardingParams": {
+                "hf_model_name": model_name,
+                "hf_supplier": supplier,
+                "hf_token": hf_token
+            }
+        }
+        response = _request_with_retry("post", deploy_url, headers=headers, json=body)
+        logging.debug(response.text)
+        response_dicts = json.loads(response.text)
+        return response_dicts
+    
+    @classmethod
+    def get_huggingface_model_status(cls, model_id: Text, api_key: Optional[Text] = None):
+        """Gets the on-boarding status of a Hugging Face model with ID MODEL_ID. 
+
+        Args:
+            model_id (Text): The model's ID as returned by DEPLOY_HUGGINGFACE_MODEL
+            api_key (Text, optional): Team API key. Defaults to None.
+        Returns:
+            Dict: Backend response
+        """
+        status_url = urljoin(config.BACKEND_URL, f"sdk/models/{model_id}")
+        if api_key:
+            headers = {"Authorization": f"Token {api_key}", "Content-Type": "application/json"}
+        else:
+            headers = {"Authorization": f"Token {config.TEAM_API_KEY}", "Content-Type": "application/json"}
+        response = _request_with_retry("get", status_url, headers=headers)
+        logging.debug(response.text)
+        response_dicts = json.loads(response.text)
+        ret_dict = {
+            "status": response_dicts["status"],
+            "name": response_dicts["name"],
+            "id": response_dicts["id"],
+            "pricing": response_dicts["pricing"]
+        }
+        return ret_dict
```

### Comparing `aiXplain-0.2.8/aixplain/factories/pipeline_factory.py` & `aiXplain-0.2.9/aixplain/factories/pipeline_factory.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/modules/__init__.py` & `aiXplain-0.2.9/aixplain/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/modules/asset.py` & `aiXplain-0.2.9/aixplain/modules/asset.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/modules/benchmark.py` & `aiXplain-0.2.9/aixplain/modules/benchmark.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/modules/benchmark_job.py` & `aiXplain-0.2.9/aixplain/modules/benchmark_job.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/modules/content_interval.py` & `aiXplain-0.2.9/aixplain/modules/content_interval.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/modules/corpus.py` & `aiXplain-0.2.9/aixplain/modules/corpus.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/modules/data.py` & `aiXplain-0.2.9/aixplain/modules/data.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/modules/dataset.py` & `aiXplain-0.2.9/aixplain/modules/dataset.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/modules/file.py` & `aiXplain-0.2.9/aixplain/modules/file.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/modules/finetune/__init__.py` & `aiXplain-0.2.9/aixplain/modules/finetune/__init__.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/modules/finetune/cost.py` & `aiXplain-0.2.9/aixplain/modules/finetune/cost.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/modules/finetune/hyperparameters.py` & `aiXplain-0.2.9/aixplain/modules/finetune/hyperparameters.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/modules/metadata.py` & `aiXplain-0.2.9/aixplain/modules/metadata.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/modules/metric.py` & `aiXplain-0.2.9/aixplain/modules/metric.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/modules/model.py` & `aiXplain-0.2.9/aixplain/modules/model.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/modules/pipeline.py` & `aiXplain-0.2.9/aixplain/modules/pipeline.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/processes/data_onboarding/onboard_functions.py` & `aiXplain-0.2.9/aixplain/processes/data_onboarding/onboard_functions.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/processes/data_onboarding/process_interval_files.py` & `aiXplain-0.2.9/aixplain/processes/data_onboarding/process_interval_files.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/processes/data_onboarding/process_media_files.py` & `aiXplain-0.2.9/aixplain/processes/data_onboarding/process_media_files.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/processes/data_onboarding/process_text_files.py` & `aiXplain-0.2.9/aixplain/processes/data_onboarding/process_text_files.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/utils/__init__.py` & `aiXplain-0.2.9/aixplain/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/utils/config.py` & `aiXplain-0.2.9/aixplain/utils/config.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/utils/convert_datatype_utils.py` & `aiXplain-0.2.9/aixplain/utils/convert_datatype_utils.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/utils/file_utils.py` & `aiXplain-0.2.9/aixplain/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/utils/request_utils.py` & `aiXplain-0.2.9/aixplain/utils/request_utils.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/aixplain/utils/validation_utils.py` & `aiXplain-0.2.9/aixplain/utils/validation_utils.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/docs/assets/aixplain-brandmark-line.png` & `aiXplain-0.2.9/docs/assets/aixplain-brandmark-line.png`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/docs/assets/data-onboard.png` & `aiXplain-0.2.9/docs/assets/data-onboard.png`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/docs/assets/designer-subtitling-sample.png` & `aiXplain-0.2.9/docs/assets/designer-subtitling-sample.png`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/docs/assets/model-id-on-platform.png` & `aiXplain-0.2.9/docs/assets/model-id-on-platform.png`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/docs/assets/navigate-api-key.png` & `aiXplain-0.2.9/docs/assets/navigate-api-key.png`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/docs/assets/subtitle-generator-output.json` & `aiXplain-0.2.9/docs/assets/subtitle-generator-output.json`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/docs/development/developer_guide.md` & `aiXplain-0.2.9/docs/development/developer_guide.md`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/docs/samples/corpus_onboarding/corpus_onboarding.ipynb` & `aiXplain-0.2.9/docs/samples/corpus_onboarding/corpus_onboarding.ipynb`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/docs/samples/corpus_onboarding/data.csv` & `aiXplain-0.2.9/docs/samples/corpus_onboarding/data.csv`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/docs/samples/dataset_onboarding/data.csv` & `aiXplain-0.2.9/docs/samples/dataset_onboarding/data.csv`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/docs/samples/dataset_onboarding/dataset_onboarding.ipynb` & `aiXplain-0.2.9/docs/samples/dataset_onboarding/dataset_onboarding.ipynb`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/docs/samples/subtitle_generator/README.md` & `aiXplain-0.2.9/docs/samples/subtitle_generator/README.md`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/docs/samples/subtitle_generator/subtitle_generator.py` & `aiXplain-0.2.9/docs/samples/subtitle_generator/subtitle_generator.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/docs/streaming/README.md` & `aiXplain-0.2.9/docs/streaming/README.md`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/docs/streaming/aixplain_diarization_streaming_client.py` & `aiXplain-0.2.9/docs/streaming/aixplain_diarization_streaming_client.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/docs/streaming/aixplain_speech_transcription_streaming_client.py` & `aiXplain-0.2.9/docs/streaming/aixplain_speech_transcription_streaming_client.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/docs/streaming/make_audio_compatible.py` & `aiXplain-0.2.9/docs/streaming/make_audio_compatible.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/docs/streaming/proto/aixplain_diarization_streaming.proto` & `aiXplain-0.2.9/docs/streaming/proto/aixplain_diarization_streaming.proto`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/docs/streaming/proto/aixplain_speech_transcription_streaming.proto` & `aiXplain-0.2.9/docs/streaming/proto/aixplain_speech_transcription_streaming.proto`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/docs/streaming/test_dia.wav` & `aiXplain-0.2.9/docs/streaming/test_dia.wav`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/docs/user/api_setup.md` & `aiXplain-0.2.9/docs/user/api_setup.md`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/docs/user/user_doc.md` & `aiXplain-0.2.9/docs/user/user_doc.md`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,25 @@
 # Run Asynchronously
 ## Start async job
 start_response = model.run_async("This is a sample text")
 poll_url = start_response["url"]
 ## Poll to see current job status
 poll_response = model.poll(poll_url)
 ```
+### Deploying Hugging Face Large Language Models
+You can deploy your very own Hugging Face large language models on our platform using the aiXplain SDK:
+```console
+$ aixplain onboard hf-model --name <what you'd like to name your model> --hf-repo-id <Hugging Face repository ID ({supplier}/{name})> --hf-token <Hugging Face token> [--api-key <TEAM_API_KEY>]
+```
+This command will return your model's ID. The on-boarding process will take 5 to 15 minutes, during which you can check the on-boarding status by running the following:
+```console
+$ aixplain get hf-model-status --model-id <model ID> [--api-key <TEAM_API_KEY>]
+```
+
+Once the on-boarding process has completed, you can use this newly-deployed large language model just like any other model on our platform. Note that our platform currently only supports language models up 7 billion parameters in size (~30 GB), so any attempts to deploy larger models will result in an error message.
 
 ### Uploading Models
 In addition to exploring and running models, the aiXplain SDK allows you to upload your own models to the aiXplain platform. This requires a working model image in line with the template specified [here](https://github.com/aixplain/model-interfaces/blob/main/docs/user/model_setup.md). [These](https://github.com/aixplain/model-interfaces/tree/main) are the interfaces with which you will be working. You will also be required to have an aiXplain account as well as a TEAM_API_KEY which should be set either as an environment variable or passed into each of the following functions.
 
 First, choose a hosting machine appropriate for your model. Note down the host machines "code". You can list the available hosting machines' specifications by running the following:
 ```console
 $ aixplain list hosts [--api-key <TEAM_API_KEY>]
```

### Comparing `aiXplain-0.2.8/pyproject.toml` & `aiXplain-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # aixplain/pyproject.toml
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["."]
-include = ["aixplain"]
+include = ["aixplain", "tests"]
 namespaces = true
 
 [project]
 name = "aiXplain"
-version = "0.2.8"
+version = "0.2.9"
 description = "aiXplain SDK adds AI functions to software."
 readme = "README.md"
 requires-python = ">=3.5, <4"
 license = { text = "Apache License, Version 2.0: http://www.apache.org/licenses/LICENSE-2.0" }
 authors = [
   {email = "thiago.ferreira@aixplain.com"},
   {email = "krishna.durai@aixplain.com"},
```

### Comparing `aiXplain-0.2.8/tests/__init__.py` & `aiXplain-0.2.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/tests/functional/benchmark/benchmark_functional_test.py` & `aiXplain-0.2.9/tests/functional/benchmark/benchmark_functional_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 @pytest.fixture(scope="module", params=read_data(MODULE_FILE))
 def module_input_map(request):
     return request.param
 
 def is_job_finshed(benchmark_job):
     time_taken = 0
     sleep_time = 15
-    timeout = 10 * 60
+    timeout = 20 * 60
     while True:
         if time_taken > timeout:
             break
         job_status = benchmark_job.check_status()
         if job_status == "in_progress":
             time.sleep(sleep_time)
             time_taken += sleep_time
```

### Comparing `aiXplain-0.2.8/tests/functional/data_asset/corpus_onboarding_test.py` & `aiXplain-0.2.9/tests/functional/data_asset/corpus_onboarding_test.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/tests/functional/data_asset/dataset_onboarding_test.py` & `aiXplain-0.2.9/tests/functional/data_asset/dataset_onboarding_test.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/tests/functional/data_asset/input/audio-en_url.csv` & `aiXplain-0.2.9/tests/functional/data_asset/input/audio-en_url.csv`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/tests/functional/data_asset/input/audio-en_with_split_url.csv` & `aiXplain-0.2.9/tests/functional/data_asset/input/audio-en_with_split_url.csv`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/tests/functional/file_asset/file_create_test.py` & `aiXplain-0.2.9/tests/functional/file_asset/file_create_test.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/tests/functional/finetune/finetune_functional_test.py` & `aiXplain-0.2.9/tests/functional/finetune/finetune_functional_test.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/tests/functional/general_assets/asset_functional_test.py` & `aiXplain-0.2.9/tests/functional/general_assets/asset_functional_test.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/tests/functional/pipelines/run_test.py` & `aiXplain-0.2.9/tests/functional/pipelines/run_test.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/tests/image_upload_e2e_test.py` & `aiXplain-0.2.9/tests/image_upload_e2e_test.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/tests/image_upload_functional_test.py` & `aiXplain-0.2.9/tests/image_upload_functional_test.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/tests/image_upload_test.py` & `aiXplain-0.2.9/tests/image_upload_test.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/tests/mock_responses/list_functions_response.json` & `aiXplain-0.2.9/tests/mock_responses/list_functions_response.json`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/tests/mock_responses/login_response.json` & `aiXplain-0.2.9/tests/mock_responses/login_response.json`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/tests/test_utils.py` & `aiXplain-0.2.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/tests/unit/finetune_test.py` & `aiXplain-0.2.9/tests/unit/finetune_test.py`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/tests/unit/mock_responses/cost_estimation_response.json` & `aiXplain-0.2.9/tests/unit/mock_responses/cost_estimation_response.json`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/tests/unit/mock_responses/list_models_response.json` & `aiXplain-0.2.9/tests/unit/mock_responses/list_models_response.json`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/tests/unit/mock_responses/model_response.json` & `aiXplain-0.2.9/tests/unit/mock_responses/model_response.json`

 * *Files identical despite different names*

### Comparing `aiXplain-0.2.8/tests/unit/model_test.py` & `aiXplain-0.2.9/tests/unit/model_test.py`

 * *Files identical despite different names*

