# Comparing `tmp/opengamedata-core-0.0.1.tar.gz` & `tmp/opengamedata_core-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opengamedata-core-0.0.1.tar", last modified: Thu Apr  4 14:32:33 2024, max compression
+gzip compressed data, was "opengamedata_core-0.0.2.tar", last modified: Mon May  6 17:29:13 2024, max compression
```

## Comparing `opengamedata-core-0.0.1.tar` & `opengamedata_core-0.0.2.tar`

### file list

```diff
@@ -1,507 +1,522 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.313212 opengamedata-core-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-04-04 14:32:33.313212 opengamedata-core-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 14:32:33.313212 opengamedata-core-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.233212 opengamedata-core-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.233212 opengamedata-core-0.0.1/src/ogd/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.237212 opengamedata-core-0.0.1/src/ogd/core/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.237212 opengamedata-core-0.0.1/src/ogd/core/exec/
--rw-r--r--   0 runner    (1001) docker     (127)     9329 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/exec/Commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/exec/Generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/exec/Parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.237212 opengamedata-core-0.0.1/src/ogd/core/generators/
--rw-r--r--   0 runner    (1001) docker     (127)     7343 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/generators/Generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/generators/GeneratorLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.237212 opengamedata-core-0.0.1/src/ogd/core/generators/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/generators/detectors/Detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/generators/detectors/DetectorEvent.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/generators/detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.237212 opengamedata-core-0.0.1/src/ogd/core/generators/extractors/
--rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/generators/extractors/Extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/generators/extractors/Feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/generators/extractors/PerCountFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/generators/extractors/PerLevelFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/generators/extractors/SessionFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/generators/extractors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.237212 opengamedata-core-0.0.1/src/ogd/core/generators/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/generators/legacy/LegacyDetector.py
--rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/generators/legacy/LegacyFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/generators/legacy/LegacyLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/generators/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.241212 opengamedata-core-0.0.1/src/ogd/core/generators/registries/
--rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/generators/registries/DetectorRegistry.py
--rw-r--r--   0 runner    (1001) docker     (127)    13575 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/generators/registries/ExtractorRegistry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/generators/registries/GeneratorRegistry.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/generators/registries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.241212 opengamedata-core-0.0.1/src/ogd/core/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)    10850 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/interfaces/BQFirebaseInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     9699 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/interfaces/BigQueryCodingInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)    10392 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/interfaces/BigQueryInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/interfaces/CSVInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/interfaces/CodingInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/interfaces/DataInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/interfaces/Interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    23918 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/interfaces/MySQLInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.241212 opengamedata-core-0.0.1/src/ogd/core/interfaces/outerfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/interfaces/outerfaces/DataOuterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/interfaces/outerfaces/DebugOuterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/interfaces/outerfaces/DictionaryOuterface.py
--rw-r--r--   0 runner    (1001) docker     (127)    33502 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/interfaces/outerfaces/TSVOuterface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.245212 opengamedata-core-0.0.1/src/ogd/core/managers/
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/managers/EventManager.py
--rw-r--r--   0 runner    (1001) docker     (127)    18587 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/managers/ExportManager.py
--rw-r--r--   0 runner    (1001) docker     (127)    12108 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/managers/FeatureManager.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/managers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.245212 opengamedata-core-0.0.1/src/ogd/core/processors/
--rw-r--r--   0 runner    (1001) docker     (127)     6040 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/processors/ClassroomDetector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/processors/DetectorProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/processors/EventProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/processors/ExtractorProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/processors/GeneratorProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/processors/PlayerProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/processors/PopulationProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/processors/Processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/processors/SessionProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/processors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.245212 opengamedata-core-0.0.1/src/ogd/core/requests/
--rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/requests/Request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/requests/RequestResult.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/requests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.249212 opengamedata-core-0.0.1/src/ogd/core/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    13389 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/schemas/Event.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/schemas/ExportMode.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/schemas/ExtractionMode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/schemas/FeatureData.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/schemas/IDMode.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/schemas/IterationMode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/schemas/Schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.249212 opengamedata-core-0.0.1/src/ogd/core/schemas/configs/
--rw-r--r--   0 runner    (1001) docker     (127)    10898 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/schemas/configs/ConfigSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/schemas/configs/GameSourceSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/schemas/configs/IndexingSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/schemas/configs/LegacyConfigSchema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.249212 opengamedata-core-0.0.1/src/ogd/core/schemas/configs/data_sources/
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/schemas/configs/data_sources/BigQuerySourceSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/schemas/configs/data_sources/DataSourceSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/schemas/configs/data_sources/FileSourceSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)    10140 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/schemas/configs/data_sources/MySQLSourceSchema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.249212 opengamedata-core-0.0.1/src/ogd/core/schemas/games/
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/schemas/games/AggregateSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/schemas/games/DetectorMapSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/schemas/games/DetectorSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/schemas/games/EventDataElementSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/schemas/games/EventSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/schemas/games/ExtractorSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/schemas/games/FeatureMapSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/schemas/games/FeatureSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)    22039 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/schemas/games/GameSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/schemas/games/GameStateSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/schemas/games/PerCountSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/schemas/games/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.253212 opengamedata-core-0.0.1/src/ogd/core/schemas/table_schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/schemas/table_schemas/BIGQUERY.json
--rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/schemas/table_schemas/FIELDDAY_MYSQL.json
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/schemas/table_schemas/FIREBASE.json
--rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/schemas/table_schemas/MASHOPOLIS_MYSQL.json
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/schemas/table_schemas/OGD_EVENT_FILE.json
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_BIGQUERY.json
--rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_MYSQL.json
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/schemas/table_schemas/SHIPWRECKS.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.253212 opengamedata-core-0.0.1/src/ogd/core/schemas/tables/
--rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/schemas/tables/ColumnMapSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/schemas/tables/ColumnSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)    22774 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/schemas/tables/TableSchema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.253212 opengamedata-core-0.0.1/src/ogd/core/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/utils/Logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/utils/Readme.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/core/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.253212 opengamedata-core-0.0.1/src/ogd/games/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.225212 opengamedata-core-0.0.1/src/ogd/games/ALL_YOU_CAN_ET/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.253212 opengamedata-core-0.0.1/src/ogd/games/ALL_YOU_CAN_ET/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    20816 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/ALL_YOU_CAN_ET/schemas/ALL_YOU_CAN_ET.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.257212 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/
--rw-r--r--   0 runner    (1001) docker     (127)    12275 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/AqualabLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)   278275 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/DBExport.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.257212 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/detectors/CollectFactNoJob.py
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/detectors/DiveSiteNoEvidence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/detectors/EchoRoomChange.py
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/detectors/HintAndLeave.py
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/detectors/Idle.py
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/detectors/SceneChangeFrequently.py
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/detectors/TwoHints.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.265212 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/ActiveJobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/ActiveTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/EchoSessionID.py
--rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/EventList.py
--rw-r--r--   0 runner    (1001) docker     (127)     7864 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/JobActiveTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/JobArgumentationTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/JobCompletionTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/JobDiveSitesCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/JobDiveTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/JobExperimentationTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/JobGuideCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/JobHelpCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/JobLocationChanges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/JobModelingTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/JobStartCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/JobTasksCompleted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/JobTriesInArgument.py
--rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/JobsAttempted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/JobsCompleted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/ModelExportCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/ModelInterveneCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/ModelPredictCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/PerJobFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/PlayerSummary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/PopulationSummary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/SessionDiveSitesCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/SessionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/SessionGuideCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/SessionHelpCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/SessionID.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/SessionJobsCompleted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/SwitchJobsCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/SyncCompletionTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/TankRulesCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/TopJobCompletionDestinations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/TopJobSwitchDestinations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/TotalArgumentationTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/TotalDiveTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/TotalExperimentationTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/UserAvgActiveTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/UserAvgSessionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/UserTotalSessionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.265212 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    29283 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/AQUALAB/schemas/AQUALAB.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.225212 opengamedata-core-0.0.1/src/ogd/games/BACTERIA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.265212 opengamedata-core-0.0.1/src/ogd/games/BACTERIA/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/BACTERIA/schemas/BACTERIA.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.225212 opengamedata-core-0.0.1/src/ogd/games/BALLOON/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.265212 opengamedata-core-0.0.1/src/ogd/games/BALLOON/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/BALLOON/schemas/BALLOON.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.225212 opengamedata-core-0.0.1/src/ogd/games/CRUSH_STATION/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.265212 opengamedata-core-0.0.1/src/ogd/games/CRUSH_STATION/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    11756 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/CRUSH_STATION/schemas/CRUSH_STATION.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.265212 opengamedata-core-0.0.1/src/ogd/games/CRYSTAL/
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/CRYSTAL/CrystalLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.265212 opengamedata-core-0.0.1/src/ogd/games/CRYSTAL/features/
--rw-r--r--   0 runner    (1001) docker     (127)    14123 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/CRYSTAL/features/CrystalExtractor.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/CRYSTAL/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.265212 opengamedata-core-0.0.1/src/ogd/games/CRYSTAL/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    14066 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/CRYSTAL/schemas/CRYSTAL.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.229212 opengamedata-core-0.0.1/src/ogd/games/CYCLE_CARBON/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.269212 opengamedata-core-0.0.1/src/ogd/games/CYCLE_CARBON/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/CYCLE_CARBON/schemas/CYCLE_CARBON.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.229212 opengamedata-core-0.0.1/src/ogd/games/CYCLE_NITROGEN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.269212 opengamedata-core-0.0.1/src/ogd/games/CYCLE_NITROGEN/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/CYCLE_NITROGEN/schemas/CYCLE_NITROGEN.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.229212 opengamedata-core-0.0.1/src/ogd/games/CYCLE_WATER/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.269212 opengamedata-core-0.0.1/src/ogd/games/CYCLE_WATER/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/CYCLE_WATER/schemas/CYCLE_WATER.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.229212 opengamedata-core-0.0.1/src/ogd/games/EARTHQUAKE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.269212 opengamedata-core-0.0.1/src/ogd/games/EARTHQUAKE/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/EARTHQUAKE/schemas/EARTHQUAKE.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.229212 opengamedata-core-0.0.1/src/ogd/games/GWAKKAMOLE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.269212 opengamedata-core-0.0.1/src/ogd/games/GWAKKAMOLE/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    12879 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/GWAKKAMOLE/schemas/GWAKKAMOLE.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.269212 opengamedata-core-0.0.1/src/ogd/games/ICECUBE/
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/ICECUBE/DBExport.json
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/ICECUBE/DBExport.py
--rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/ICECUBE/IcecubeLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.269212 opengamedata-core-0.0.1/src/ogd/games/ICECUBE/features/
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/ICECUBE/features/HeadsetOnCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/ICECUBE/features/ObjectSelectionsDuringVoiceover.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/ICECUBE/features/PerSceneFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/ICECUBE/features/SceneDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/ICECUBE/features/SceneFailureCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/ICECUBE/features/SceneFailures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/ICECUBE/features/ScenesEncountered.py
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/ICECUBE/features/SessionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/ICECUBE/features/Session_Language.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/ICECUBE/features/TaskTimeToComplete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/ICECUBE/features/ViewportCountPerScene.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/ICECUBE/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.269212 opengamedata-core-0.0.1/src/ogd/games/ICECUBE/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/ICECUBE/schemas/ICECUBE.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.273212 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/
--rw-r--r--   0 runner    (1001) docker     (127)     7717 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/JournalismLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.277212 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/AttributeView.py
--rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/ChoiceClickCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/ContinuesOnFail.py
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/EditorNoteOpen.py
--rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/FailureCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/GameComplete.py
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/LevelCompleteCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/LevelCompleted.py
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/LevelTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/MaxedPlayerAttribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/MeanSnippetTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/PlayTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/PlayerAttributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/QuitLevel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/QuitNode.py
--rw-r--r--   0 runner    (1001) docker     (127)     7743 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/QuitType.py
--rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/QuitTypePerLevel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/SessionPlayTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/SkillSequenceCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/SnippetReceivedCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/SnippetReplace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/SnippetsCollected.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/SnippetsSubmitted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/StoryAlignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/StoryAlignmentSequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/StoryCompleteTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/StoryEditorTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/StoryScore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/StoryScoreSequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/TextClickCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/TopAttribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/TopPlayerAttribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/TopPlayerQuitType.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/TotalFails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/TotalLevelTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/UserPlayTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/WorstAttribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/WorstPlayerAttribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.277212 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    45415 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/schemas/JOURNALISM.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.277212 opengamedata-core-0.0.1/src/ogd/games/JOWILDER/
--rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOWILDER/JowilderLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)    16451 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOWILDER/Jowilder_Enumerators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.281212 opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/ActiveStateTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/Clicks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/EventCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/FirstInteraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/GameScript.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/GameVersion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/Hovers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/IdleState.py
--rw-r--r--   0 runner    (1001) docker     (127)     7609 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/Interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/InteractionName.py
--rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/InteractionTextBoxesPerSecond.py
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/InteractionWordsPerSecond.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/LastInteraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/MeaningfulActions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/NotebookUses.py
--rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/QuestionAnswers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/SessionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/SessionStart.py
--rw-r--r--   0 runner    (1001) docker     (127)     5056 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/SurveyItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/SurveyTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/UsedContinue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/UsedSaveCode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/UserEnabled.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOWILDER/get_jowilder_all_items.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.281212 opengamedata-core-0.0.1/src/ogd/games/JOWILDER/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    35912 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/JOWILDER/schemas/JOWILDER.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.285212 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/LakelandLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.289212 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/ActionsLastXSecondsModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/DeathCountModel.py
--rw-r--r--   0 runner    (1001) docker     (127)    11750 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/DeathPredModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     8664 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/DeathThresholdModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/DiagonalFarmDetectorModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/FeatSeqPercent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/FeatVelocity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/FeatureModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/LAKELAND_models.json
--rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/LakelandEnumerators.json
--rw-r--r--   0 runner    (1001) docker     (127)    69740 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/LakelandExtractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/LinearModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/LogisticModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/MapSummaryModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/Model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/MoneyAccumulationModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/NthEventModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/PlayingTimeModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/PopulationModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/RecentPurchasesModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/SequenceModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/SimpleFarmAbandonmentModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/SingleFeatureModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/TimeSinceEventTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/TimeSinceLastSaleModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/TownCompositionFeatureModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/TownCompositionModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/TutorialProgressionModel.py
--rw-r--r--   0 runner    (1001) docker     (127)    82382 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/WAVES_models.json
--rw-r--r--   0 runner    (1001) docker     (127)    82382 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/WAVES_models_L8_Q0_Q1.json
--rw-r--r--   0 runner    (1001) docker     (127)    49819 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/WAVES_models_L8_and_Q0.json
--rw-r--r--   0 runner    (1001) docker     (127)    28429 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/WAVES_models_L8_complete_and_current.json
--rw-r--r--   0 runner    (1001) docker     (127)    21021 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/WAVES_models_L8_only_complete.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 14:31:57.000000 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/produce_lakeland_enumerators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.289212 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)   115553 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/LAKELAND/schemas/LAKELAND.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.289212 opengamedata-core-0.0.1/src/ogd/games/MAGNET/
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/MAGNET/MagnetLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.289212 opengamedata-core-0.0.1/src/ogd/games/MAGNET/features/
--rw-r--r--   0 runner    (1001) docker     (127)     8596 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/MAGNET/features/MagnetExtractor.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/MAGNET/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.289212 opengamedata-core-0.0.1/src/ogd/games/MAGNET/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/MAGNET/schemas/MAGNET.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.229212 opengamedata-core-0.0.1/src/ogd/games/MASHOPOLIS/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.289212 opengamedata-core-0.0.1/src/ogd/games/MASHOPOLIS/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    10063 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/MASHOPOLIS/schemas/MASHOPOLIS.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.289212 opengamedata-core-0.0.1/src/ogd/games/PENGUINS/
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/PENGUINS/DBExport.json
--rw-r--r--   0 runner    (1001) docker     (127)     7109 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/PENGUINS/PenguinsLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/PENGUINS/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.293212 opengamedata-core-0.0.1/src/ogd/games/PENGUINS/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/PENGUINS/detectors/RegionEnter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/PENGUINS/detectors/RegionExit.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/PENGUINS/detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.293212 opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/ActivityCompleted.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/ActivityDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/EatFishCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/EggLostCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/EggRecoverTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/GazeCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/GazeDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/MirrorWaddleDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/PerRegionFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/PickupRockCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/PlayerInactiveAvgDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/PlayerWaddleCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/RegionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/RegionEnterCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/RegionsEncountered.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/RingChimesCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/SessionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/SnowBallDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/WaddlePerRegion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.293212 opengamedata-core-0.0.1/src/ogd/games/PENGUINS/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    24158 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/PENGUINS/schemas/PENGUINS.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.297212 opengamedata-core-0.0.1/src/ogd/games/SHADOWSPECT/
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/SHADOWSPECT/ShadowspectLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.297212 opengamedata-core-0.0.1/src/ogd/games/SHADOWSPECT/features/
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/SHADOWSPECT/features/FunnelByUser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/SHADOWSPECT/features/LevelsOfDifficulty.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/SHADOWSPECT/features/MoveShapeCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/SHADOWSPECT/features/SequenceBetweenPuzzles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/SHADOWSPECT/features/SessionID.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/SHADOWSPECT/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.297212 opengamedata-core-0.0.1/src/ogd/games/SHADOWSPECT/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    29173 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/SHADOWSPECT/schemas/SHADOWSPECT.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.297212 opengamedata-core-0.0.1/src/ogd/games/SHIPWRECKS/
--rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/SHIPWRECKS/ShipwrecksLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.301212 opengamedata-core-0.0.1/src/ogd/games/SHIPWRECKS/features/
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/SHIPWRECKS/features/ActiveJobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/SHIPWRECKS/features/EventList.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/SHIPWRECKS/features/EvidenceBoardCompleteCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/SHIPWRECKS/features/JobsAttempted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/SHIPWRECKS/features/JobsCompleted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/SHIPWRECKS/features/MissionDiveTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/SHIPWRECKS/features/MissionSonarTimeToComplete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/SHIPWRECKS/features/PlayerSummary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/SHIPWRECKS/features/PopulationSummary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/SHIPWRECKS/features/SessionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/SHIPWRECKS/features/SessionID.py
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/SHIPWRECKS/features/TopJobCompletionDestinations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/SHIPWRECKS/features/TopJobSwitchDestinations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/SHIPWRECKS/features/TotalDiveTime.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/SHIPWRECKS/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.301212 opengamedata-core-0.0.1/src/ogd/games/SHIPWRECKS/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/SHIPWRECKS/schemas/SHIPWRECKS.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.301212 opengamedata-core-0.0.1/src/ogd/games/THERMOVR/
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/THERMOVR/DBExport.json
--rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/THERMOVR/ThermoVRLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/THERMOVR/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.301212 opengamedata-core-0.0.1/src/ogd/games/THERMOVR/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/THERMOVR/detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.301212 opengamedata-core-0.0.1/src/ogd/games/THERMOVR/features/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/THERMOVR/features/LabCompleteCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/THERMOVR/features/TaskCompleteCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/THERMOVR/features/ToolNudegCount.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/THERMOVR/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.301212 opengamedata-core-0.0.1/src/ogd/games/THERMOVR/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    49519 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/THERMOVR/schemas/THERMOVR.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.301212 opengamedata-core-0.0.1/src/ogd/games/TRANSFORMATION_QUEST/
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/TRANSFORMATION_QUEST/DBExport.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.301212 opengamedata-core-0.0.1/src/ogd/games/TRANSFORMATION_QUEST/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    25177 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/TRANSFORMATION_QUEST/schemas/TRANSFORMATION_QUEST.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.301212 opengamedata-core-0.0.1/src/ogd/games/WAVES/
--rw-r--r--   0 runner    (1001) docker     (127)    37332 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/WaveLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.309212 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/AmplitudeGoodMoveCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/AverageFails.py
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/AverageLevelTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/AverageMoveTypeChanges.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/AverageSliderMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/BeginCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/ClosenessIntercept.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/ClosenessR2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/ClosenessSlope.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/Completed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/FirstMoveType.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/MenuButtonCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/OffsetGoodMoveCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/OverallPercentAmplitudeMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/OverallPercentOffsetMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/OverallPercentWavelengthMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/OverallSliderAverageRange.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/OverallSliderAverageStandardDeviations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/PercentAmplitudeGoodMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/PercentAmplitudeMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/PercentOffsetGoodMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/PercentOffsetMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/PercentWavelengthGoodMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/PercentWavelengthMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/PersistentSessionID.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/QuestionAnswered.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/QuestionCorrect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/RangeIntercept.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/RangeR2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/RangeSlope.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/SequenceLevel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/SessionID.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/SliderAverageRange.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/SliderAverageStandardDeviations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/SucceedCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/TimeToAnswerMS.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/TotalArrowMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/TotalFails.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/TotalLevelTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/TotalMoveTypeChanges.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/TotalResets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/TotalSkips.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/TotalSliderMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/WavelengthGoodMoveCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.309212 opengamedata-core-0.0.1/src/ogd/games/WAVES/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    21383 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WAVES/schemas/WAVES.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.233212 opengamedata-core-0.0.1/src/ogd/games/WEATHER_STATION/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.309212 opengamedata-core-0.0.1/src/ogd/games/WEATHER_STATION/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    34344 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WEATHER_STATION/schemas/WEATHER_STATION.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.233212 opengamedata-core-0.0.1/src/ogd/games/WIND/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.309212 opengamedata-core-0.0.1/src/ogd/games/WIND/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/WIND/schemas/WIND.json.template
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/src/ogd/games/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.313212 opengamedata-core-0.0.1/src/opengamedata_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-04-04 14:32:33.000000 opengamedata-core-0.0.1/src/opengamedata_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20297 2024-04-04 14:32:33.000000 opengamedata-core-0.0.1/src/opengamedata_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:32:33.000000 opengamedata-core-0.0.1/src/opengamedata_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-04 14:32:33.000000 opengamedata-core-0.0.1/src/opengamedata_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:33.309212 opengamedata-core-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-04 14:31:58.000000 opengamedata-core-0.0.1/tests/test_lakeland_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.802339 opengamedata_core-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-05-06 17:29:13.802339 opengamedata_core-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 17:29:13.802339 opengamedata_core-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.726339 opengamedata_core-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.726339 opengamedata_core-0.0.2/src/ogd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.726339 opengamedata_core-0.0.2/src/ogd/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.726339 opengamedata_core-0.0.2/src/ogd/core/exec/
+-rw-r--r--   0 runner    (1001) docker     (127)     9329 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/exec/Commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/exec/Generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/exec/Parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.730339 opengamedata_core-0.0.2/src/ogd/core/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/Generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/GeneratorLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.730339 opengamedata_core-0.0.2/src/ogd/core/generators/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/detectors/Detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/detectors/DetectorEvent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.730339 opengamedata_core-0.0.2/src/ogd/core/generators/extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/extractors/Extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/extractors/Feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/extractors/PerCountFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/extractors/PerLevelFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/extractors/SessionFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/extractors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.730339 opengamedata_core-0.0.2/src/ogd/core/generators/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/legacy/LegacyDetector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/legacy/LegacyFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/legacy/LegacyLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.730339 opengamedata_core-0.0.2/src/ogd/core/generators/registries/
+-rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/registries/DetectorRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13575 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/registries/ExtractorRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/registries/GeneratorRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/registries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.734340 opengamedata_core-0.0.2/src/ogd/core/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)    10850 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/interfaces/BQFirebaseInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9699 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/interfaces/BigQueryCodingInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11865 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/interfaces/BigQueryInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/interfaces/CSVInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/interfaces/CodingInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/interfaces/DataInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/interfaces/Interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23918 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/interfaces/MySQLInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.734340 opengamedata_core-0.0.2/src/ogd/core/interfaces/outerfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/interfaces/outerfaces/DataOuterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/interfaces/outerfaces/DebugOuterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/interfaces/outerfaces/DictionaryOuterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33757 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/interfaces/outerfaces/TSVOuterface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.734340 opengamedata_core-0.0.2/src/ogd/core/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/managers/EventManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18830 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/managers/ExportManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12108 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/managers/FeatureManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/managers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.734340 opengamedata_core-0.0.2/src/ogd/core/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)     6040 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/processors/ClassroomDetector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/processors/DetectorProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/processors/EventProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/processors/ExtractorProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/processors/GeneratorProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/processors/PlayerProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/processors/PopulationProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/processors/Processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/processors/SessionProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/processors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.738340 opengamedata_core-0.0.2/src/ogd/core/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/requests/Request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/requests/RequestResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/requests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.738340 opengamedata_core-0.0.2/src/ogd/core/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    14401 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/Event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/ExportMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/ExtractionMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/FeatureData.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/IDMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/IterationMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/Schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.738340 opengamedata_core-0.0.2/src/ogd/core/schemas/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)    10898 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/configs/ConfigSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/configs/GameSourceSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/configs/IndexingSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/configs/LegacyConfigSchema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.738340 opengamedata_core-0.0.2/src/ogd/core/schemas/configs/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/configs/data_sources/BigQuerySourceSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/configs/data_sources/DataSourceSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/configs/data_sources/FileSourceSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10140 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/configs/data_sources/MySQLSourceSchema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.742339 opengamedata_core-0.0.2/src/ogd/core/schemas/games/
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/games/AggregateSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/games/DataElementSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/games/DetectorMapSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/games/DetectorSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/games/EventSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/games/ExtractorSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/games/FeatureMapSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/games/FeatureSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26726 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/games/GameSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/games/GameStateSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/games/PerCountSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/games/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.742339 opengamedata_core-0.0.2/src/ogd/core/schemas/table_schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/table_schemas/BIGQUERY.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/table_schemas/FIELDDAY_MYSQL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/table_schemas/FIREBASE.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/table_schemas/MASHOPOLIS_MYSQL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/table_schemas/OGD_EVENT_FILE.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_BIGQUERY.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_MYSQL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/table_schemas/SHIPWRECKS.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.742339 opengamedata_core-0.0.2/src/ogd/core/schemas/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/tables/ColumnMapSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/tables/ColumnSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23084 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/tables/TableSchema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.742339 opengamedata_core-0.0.2/src/ogd/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/utils/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/utils/Readme.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.742339 opengamedata_core-0.0.2/src/ogd/games/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.718340 opengamedata_core-0.0.2/src/ogd/games/ALL_YOU_CAN_ET/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.746339 opengamedata_core-0.0.2/src/ogd/games/ALL_YOU_CAN_ET/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    20816 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/ALL_YOU_CAN_ET/schemas/ALL_YOU_CAN_ET.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.746339 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/
+-rw-r--r--   0 runner    (1001) docker     (127)    12275 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/AqualabLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)   278275 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/DBExport.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.746339 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/detectors/CollectFactNoJob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/detectors/DiveSiteNoEvidence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/detectors/EchoRoomChange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/detectors/HintAndLeave.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/detectors/Idle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/detectors/SceneChangeFrequently.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/detectors/TwoHints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.754339 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/ActiveJobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/ActiveTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/EchoSessionID.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/EventList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobActiveTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobArgumentationTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobCompletionTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobDiveSitesCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobDiveTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobExperimentationTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobGuideCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobHelpCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobLocationChanges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobModelingTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobPlayTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobStartCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobTasksCompleted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobTriesInArgument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6192 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobsAttempted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobsCompleted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/ModelExportCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/ModelInterveneCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/ModelPredictCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/PerJobFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/PlayerSummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/PopulationSummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/SessionDiveSitesCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/SessionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/SessionGuideCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/SessionHelpCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/SessionID.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/SessionJobsCompleted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/SwitchJobsCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/SyncCompletionTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/TankRulesCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/TopJobCompletionDestinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/TopJobSwitchDestinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/TotalArgumentationTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/TotalDiveTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/TotalExperimentationTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/UserAvgActiveTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/UserAvgSessionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/UserTotalSessionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.754339 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    29283 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/schemas/AQUALAB.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.718340 opengamedata_core-0.0.2/src/ogd/games/BACTERIA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.754339 opengamedata_core-0.0.2/src/ogd/games/BACTERIA/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/BACTERIA/schemas/BACTERIA.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.718340 opengamedata_core-0.0.2/src/ogd/games/BALLOON/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.754339 opengamedata_core-0.0.2/src/ogd/games/BALLOON/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/BALLOON/schemas/BALLOON.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.718340 opengamedata_core-0.0.2/src/ogd/games/BLOOM/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.754339 opengamedata_core-0.0.2/src/ogd/games/BLOOM/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    20765 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/BLOOM/schemas/BLOOM.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.718340 opengamedata_core-0.0.2/src/ogd/games/CENSIO_SLIDE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.754339 opengamedata_core-0.0.2/src/ogd/games/CENSIO_SLIDE/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    11446 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/CENSIO_SLIDE/schemas/CENSIO_SLIDE.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.718340 opengamedata_core-0.0.2/src/ogd/games/CENSIO_STACK/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.754339 opengamedata_core-0.0.2/src/ogd/games/CENSIO_STACK/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    21742 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/CENSIO_STACK/schemas/CENSIO_STACK.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.722339 opengamedata_core-0.0.2/src/ogd/games/CRUSH_STATION/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.754339 opengamedata_core-0.0.2/src/ogd/games/CRUSH_STATION/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    11756 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/CRUSH_STATION/schemas/CRUSH_STATION.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.754339 opengamedata_core-0.0.2/src/ogd/games/CRYSTAL/
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/CRYSTAL/CrystalLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.754339 opengamedata_core-0.0.2/src/ogd/games/CRYSTAL/features/
+-rw-r--r--   0 runner    (1001) docker     (127)    14123 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/CRYSTAL/features/CrystalExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/CRYSTAL/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.754339 opengamedata_core-0.0.2/src/ogd/games/CRYSTAL/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    14066 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/CRYSTAL/schemas/CRYSTAL.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.722339 opengamedata_core-0.0.2/src/ogd/games/CYCLE_CARBON/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.754339 opengamedata_core-0.0.2/src/ogd/games/CYCLE_CARBON/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/CYCLE_CARBON/schemas/CYCLE_CARBON.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.722339 opengamedata_core-0.0.2/src/ogd/games/CYCLE_NITROGEN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.758339 opengamedata_core-0.0.2/src/ogd/games/CYCLE_NITROGEN/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/CYCLE_NITROGEN/schemas/CYCLE_NITROGEN.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.722339 opengamedata_core-0.0.2/src/ogd/games/CYCLE_WATER/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.758339 opengamedata_core-0.0.2/src/ogd/games/CYCLE_WATER/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/CYCLE_WATER/schemas/CYCLE_WATER.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.722339 opengamedata_core-0.0.2/src/ogd/games/EARTHQUAKE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.758339 opengamedata_core-0.0.2/src/ogd/games/EARTHQUAKE/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/EARTHQUAKE/schemas/EARTHQUAKE.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.722339 opengamedata_core-0.0.2/src/ogd/games/GWAKKAMOLE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.758339 opengamedata_core-0.0.2/src/ogd/games/GWAKKAMOLE/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    12879 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/GWAKKAMOLE/schemas/GWAKKAMOLE.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.758339 opengamedata_core-0.0.2/src/ogd/games/ICECUBE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/ICECUBE/DBExport.json
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/ICECUBE/DBExport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/ICECUBE/IcecubeLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.758339 opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/HeadsetOnCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/ObjectSelectionsDuringVoiceover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/PerSceneFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/SceneDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/SceneFailureCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/SceneFailures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/ScenesEncountered.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/SessionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/Session_Language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/TaskTimeToComplete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/ViewportCountPerScene.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.758339 opengamedata_core-0.0.2/src/ogd/games/ICECUBE/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/ICECUBE/schemas/ICECUBE.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.758339 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/
+-rw-r--r--   0 runner    (1001) docker     (127)     7717 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/JournalismLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.766339 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/AttributeView.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/ChoiceClickCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/ContinuesOnFail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/EditorNoteOpen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/FailureCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/GameComplete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/LevelCompleteCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/LevelCompleted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/LevelTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/MaxedPlayerAttribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/MeanSnippetTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/PlayTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/PlayerAttributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/QuitLevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/QuitNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/QuitType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/QuitTypePerLevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/SessionPlayTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/SkillSequenceCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/SnippetReceivedCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/SnippetReplace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/SnippetsCollected.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/SnippetsSubmitted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/StoryAlignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/StoryAlignmentSequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/StoryCompleteTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/StoryEditorTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/StoryScore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/StoryScoreSequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/TextClickCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/TopAttribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/TopPlayerAttribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/TopPlayerQuitType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/TotalFails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/TotalLevelTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/UserPlayTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/WorstAttribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/WorstPlayerAttribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.766339 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    45415 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/schemas/JOURNALISM.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.766339 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/
+-rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/JowilderLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16451 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/Jowilder_Enumerators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.770339 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/ActiveStateTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/Clicks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/EventCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/FirstInteraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/GameScript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/GameVersion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/Hovers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/IdleState.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7609 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/Interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/InteractionName.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/InteractionTextBoxesPerSecond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/InteractionWordsPerSecond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/LastInteraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/MeaningfulActions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/NotebookUses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/QuestionAnswers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/SessionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/SessionStart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/SurveyItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/SurveyTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/UsedContinue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/UsedSaveCode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/UserEnabled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/get_jowilder_all_items.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.770339 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    35912 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/schemas/JOWILDER.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.774339 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/LakelandLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.778339 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/ActionsLastXSecondsModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/DeathCountModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11750 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/DeathPredModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8664 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/DeathThresholdModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/DiagonalFarmDetectorModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/FeatSeqPercent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/FeatVelocity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/FeatureModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/LAKELAND_models.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/LakelandEnumerators.json
+-rw-r--r--   0 runner    (1001) docker     (127)    69732 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/LakelandExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/LinearModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/LogisticModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/MapSummaryModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/Model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/MoneyAccumulationModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/NthEventModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/PlayingTimeModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/PopulationModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/RecentPurchasesModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/SequenceModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/SimpleFarmAbandonmentModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/SingleFeatureModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/TimeSinceEventTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/TimeSinceLastSaleModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/TownCompositionFeatureModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/TownCompositionModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/TutorialProgressionModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82382 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/WAVES_models.json
+-rw-r--r--   0 runner    (1001) docker     (127)    82382 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/WAVES_models_L8_Q0_Q1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    49819 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/WAVES_models_L8_and_Q0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    28429 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/WAVES_models_L8_complete_and_current.json
+-rw-r--r--   0 runner    (1001) docker     (127)    21021 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/WAVES_models_L8_only_complete.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/produce_lakeland_enumerators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.778339 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)   115553 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/schemas/LAKELAND.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.778339 opengamedata_core-0.0.2/src/ogd/games/MAGNET/
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/MAGNET/MagnetLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.778339 opengamedata_core-0.0.2/src/ogd/games/MAGNET/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     8596 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/MAGNET/features/MagnetExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/MAGNET/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.778339 opengamedata_core-0.0.2/src/ogd/games/MAGNET/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/MAGNET/schemas/MAGNET.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.722339 opengamedata_core-0.0.2/src/ogd/games/MASHOPOLIS/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.778339 opengamedata_core-0.0.2/src/ogd/games/MASHOPOLIS/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    10063 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/MASHOPOLIS/schemas/MASHOPOLIS.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.782339 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/DBExport.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7109 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/PenguinsLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.782339 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/detectors/RegionEnter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/detectors/RegionExit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.786339 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/ActivityCompleted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/ActivityDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/EatFishCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/EggLostCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/EggRecoverTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/GazeCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/GazeDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/MirrorWaddleDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/PerRegionFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/PickupRockCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/PlayerInactiveAvgDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/PlayerWaddleCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/RegionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/RegionEnterCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/RegionsEncountered.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/RingChimesCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/SessionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/SnowBallDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/WaddlePerRegion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.786339 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    24103 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/schemas/PENGUINS.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.786339 opengamedata_core-0.0.2/src/ogd/games/SHADOWSPECT/
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHADOWSPECT/ShadowspectLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.786339 opengamedata_core-0.0.2/src/ogd/games/SHADOWSPECT/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHADOWSPECT/features/FunnelByUser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHADOWSPECT/features/LevelsOfDifficulty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHADOWSPECT/features/MoveShapeCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHADOWSPECT/features/SequenceBetweenPuzzles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHADOWSPECT/features/SessionID.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHADOWSPECT/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.786339 opengamedata_core-0.0.2/src/ogd/games/SHADOWSPECT/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    29173 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHADOWSPECT/schemas/SHADOWSPECT.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.786339 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/
+-rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/ShipwrecksLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.790339 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/ActiveJobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/EventList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/EvidenceBoardCompleteCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/JobsAttempted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/JobsCompleted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/MissionDiveTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/MissionSonarTimeToComplete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/PlayerSummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/PopulationSummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/SessionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/SessionID.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/TopJobCompletionDestinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/TopJobSwitchDestinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/TotalDiveTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.790339 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/schemas/SHIPWRECKS.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.790339 opengamedata_core-0.0.2/src/ogd/games/THERMOVR/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/THERMOVR/DBExport.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/THERMOVR/ThermoVRLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/THERMOVR/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.790339 opengamedata_core-0.0.2/src/ogd/games/THERMOVR/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/THERMOVR/detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.790339 opengamedata_core-0.0.2/src/ogd/games/THERMOVR/features/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/THERMOVR/features/LabCompleteCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/THERMOVR/features/LeftHandMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/THERMOVR/features/PhasesReached.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/THERMOVR/features/PlayMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/THERMOVR/features/RightHandMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/THERMOVR/features/TaskCompleteCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/THERMOVR/features/ToolNudgeCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/THERMOVR/features/ToolSliderTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/THERMOVR/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.790339 opengamedata_core-0.0.2/src/ogd/games/THERMOVR/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    51378 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/THERMOVR/schemas/THERMOVR.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.790339 opengamedata_core-0.0.2/src/ogd/games/TRANSFORMATION_QUEST/
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/TRANSFORMATION_QUEST/DBExport.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.790339 opengamedata_core-0.0.2/src/ogd/games/TRANSFORMATION_QUEST/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    25177 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/TRANSFORMATION_QUEST/schemas/TRANSFORMATION_QUEST.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.790339 opengamedata_core-0.0.2/src/ogd/games/WAVES/
+-rw-r--r--   0 runner    (1001) docker     (127)    37332 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/WaveLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.802339 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/AmplitudeGoodMoveCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/AverageFails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/AverageLevelTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/AverageMoveTypeChanges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/AverageSliderMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/BeginCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/ClosenessIntercept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/ClosenessR2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/ClosenessSlope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/Completed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/FirstMoveType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/MenuButtonCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/OffsetGoodMoveCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/OverallPercentAmplitudeMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/OverallPercentOffsetMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/OverallPercentWavelengthMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/OverallSliderAverageRange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/OverallSliderAverageStandardDeviations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/PercentAmplitudeGoodMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/PercentAmplitudeMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/PercentOffsetGoodMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/PercentOffsetMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/PercentWavelengthGoodMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/PercentWavelengthMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/PersistentSessionID.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/QuestionAnswered.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/QuestionCorrect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/RangeIntercept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/RangeR2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/RangeSlope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/SequenceLevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/SessionID.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/SliderAverageRange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/SliderAverageStandardDeviations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/SucceedCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/TimeToAnswerMS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/TotalArrowMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/TotalFails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/TotalLevelTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/TotalMoveTypeChanges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/TotalResets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/TotalSkips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/TotalSliderMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/WavelengthGoodMoveCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.802339 opengamedata_core-0.0.2/src/ogd/games/WAVES/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    21383 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/schemas/WAVES.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.726339 opengamedata_core-0.0.2/src/ogd/games/WEATHER_STATION/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.802339 opengamedata_core-0.0.2/src/ogd/games/WEATHER_STATION/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    34344 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WEATHER_STATION/schemas/WEATHER_STATION.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.726339 opengamedata_core-0.0.2/src/ogd/games/WIND/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.802339 opengamedata_core-0.0.2/src/ogd/games/WIND/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WIND/schemas/WIND.json.template
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.802339 opengamedata_core-0.0.2/src/opengamedata_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-05-06 17:29:13.000000 opengamedata_core-0.0.2/src/opengamedata_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20752 2024-05-06 17:29:13.000000 opengamedata_core-0.0.2/src/opengamedata_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 17:29:13.000000 opengamedata_core-0.0.2/src/opengamedata_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-06 17:29:13.000000 opengamedata_core-0.0.2/src/opengamedata_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.802339 opengamedata_core-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-06 17:28:33.000000 opengamedata_core-0.0.2/tests/test_lakeland_models.py
```

### Comparing `opengamedata-core-0.0.1/LICENSE` & `opengamedata_core-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/PKG-INFO` & `opengamedata_core-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opengamedata-core
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for retrieving and processing event-based video game data. Additional authors: Nick Spevacek, Renee Li, John McCloskey, Zach Studdiford, Glenn Palmer, Haishuo Chen, Daus, Ameya Kshirsagar, Yunqing Xiao, Erik Harpstead, Manuel Jesus Gomez Moratilla
 Author-email: Luke Swanson <superscription58@gmail.com>, David Gagnon <djgagnon@wisc.edu>
 Project-URL: Homepage, https://github.com/opengamedata/opengamedata-core
 Project-URL: Bug Tracker, https://github.com/opengamedata/opengamedata-core/issues
 Project-URL: Documentation, https://opengamedata-doc.readthedocs.io/en/latest/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,29 +13,29 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Python3 implementation of the Open Game Gata feature extractor  
 
 This code pulls raw game data from a SQL database, BigQuery database, or export file; chooses appropiate features to extract based on the "game_id"; and writes results to a file for data mining.
 
-See http://fielddaylab.wisc.edu/opengamedata for exports of raw events and the features created by this code for a collection of education games.
-See https://www.youtube.com/watch?v=gelyDJjxIeg for a walkthorugh of the high-level code structure.
+See [http://fielddaylab.wisc.edu/opengamedata](http://fielddaylab.wisc.edu/opengamedata) for exports of raw events and the features created by this code for a collection of education games.
+See [https://www.youtube.com/watch?v=gelyDJjxIeg](https://www.youtube.com/watch?v=gelyDJjxIeg) for a walkthorugh of the high-level code structure.
 
 Please feel free to modify this code, add new features or games and share back to the authors. We will deploy improvements to the Open Game Data site.
 
 Setup:
 
 * Install python3 (could write a whole chapter on this)
 * Install python dependencies: "pip3 install -r requirements.txt"
 * Copy `config.py.template` to `config.py` and set server/authentication data
 * Download any authentication keys needed for BigQuery game data projects
 
 Running Data Exports:  
 
-```
+```none
 usage: <python> main.py <cmd> [<args>]
 
 <python> is your python command.
 <cmd>    is one of the available commands:
          - export
          - export-events
          - export-features
@@ -60,34 +60,40 @@
          - readme: game_id
              game_id    = id of game whose readme should be generated
          - help: *None*
 [<opt-args>] are option arguments, which affect certain commands:
          --file: specifies a file to export events or features
          --monthly: with this flag, specify dates by mm/yyyy instead of mm/dd/yyyy
 ```
+
 (you can see a similar printout directly from the system by running ```python3 main.py --help```)
 
 Example use:
-```
+
+```none
 python3 main.py export JOWILDER 1/1/2019 2/28/2019
 ```
+
 In the example above, all JOWILDER data from beginning of January to end of February (in 2019) is exported. This includes both the events and the processed session features.
 
-```
+```none
 python3 main.py export JOWILDER --monthly 1/2019
 ```
+
 In the example above, all JOWILDER data from the month of January 2019 is exported. This includes both the events and the processed session features.
 
-```
+```none
 python3 main.py export-events JOWILDER 1/1/2019 2/28/2019
 ```
+
 In the example above, only the events from the JOWILDER data during given date range are exported.
 
-```
+```none
 python3 main.py export-features JOWILDER 1/1/2019 2/28/2019
 ```
+
 In the example above, only the processed session/player/population features from the JOWILDER data during given date range are exported.
 
 <!-- ```
 python3 main.py export JOWILDER --file=C:\path\to\opengamedata-backend\data\JOWILDER\JOWILDER_20190101_to_20190228_1234abc_events.zip
 ```
 In the example above, events and processed session features are exported from the data at the specified file path. -->
```

### Comparing `opengamedata-core-0.0.1/README.md` & `opengamedata_core-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Python3 implementation of the Open Game Gata feature extractor  
 
 This code pulls raw game data from a SQL database, BigQuery database, or export file; chooses appropiate features to extract based on the "game_id"; and writes results to a file for data mining.
 
-See http://fielddaylab.wisc.edu/opengamedata for exports of raw events and the features created by this code for a collection of education games.
-See https://www.youtube.com/watch?v=gelyDJjxIeg for a walkthorugh of the high-level code structure.
+See [http://fielddaylab.wisc.edu/opengamedata](http://fielddaylab.wisc.edu/opengamedata) for exports of raw events and the features created by this code for a collection of education games.
+See [https://www.youtube.com/watch?v=gelyDJjxIeg](https://www.youtube.com/watch?v=gelyDJjxIeg) for a walkthorugh of the high-level code structure.
 
 Please feel free to modify this code, add new features or games and share back to the authors. We will deploy improvements to the Open Game Data site.
 
 Setup:
 
 * Install python3 (could write a whole chapter on this)
 * Install python dependencies: "pip3 install -r requirements.txt"
 * Copy `config.py.template` to `config.py` and set server/authentication data
 * Download any authentication keys needed for BigQuery game data projects
 
 Running Data Exports:  
 
-```
+```none
 usage: <python> main.py <cmd> [<args>]
 
 <python> is your python command.
 <cmd>    is one of the available commands:
          - export
          - export-events
          - export-features
@@ -45,34 +45,40 @@
          - readme: game_id
              game_id    = id of game whose readme should be generated
          - help: *None*
 [<opt-args>] are option arguments, which affect certain commands:
          --file: specifies a file to export events or features
          --monthly: with this flag, specify dates by mm/yyyy instead of mm/dd/yyyy
 ```
+
 (you can see a similar printout directly from the system by running ```python3 main.py --help```)
 
 Example use:
-```
+
+```none
 python3 main.py export JOWILDER 1/1/2019 2/28/2019
 ```
+
 In the example above, all JOWILDER data from beginning of January to end of February (in 2019) is exported. This includes both the events and the processed session features.
 
-```
+```none
 python3 main.py export JOWILDER --monthly 1/2019
 ```
+
 In the example above, all JOWILDER data from the month of January 2019 is exported. This includes both the events and the processed session features.
 
-```
+```none
 python3 main.py export-events JOWILDER 1/1/2019 2/28/2019
 ```
+
 In the example above, only the events from the JOWILDER data during given date range are exported.
 
-```
+```none
 python3 main.py export-features JOWILDER 1/1/2019 2/28/2019
 ```
+
 In the example above, only the processed session/player/population features from the JOWILDER data during given date range are exported.
 
 <!-- ```
 python3 main.py export JOWILDER --file=C:\path\to\opengamedata-backend\data\JOWILDER\JOWILDER_20190101_to_20190228_1234abc_events.zip
 ```
 In the example above, events and processed session features are exported from the data at the specified file path. -->
```

### Comparing `opengamedata-core-0.0.1/pyproject.toml` & `opengamedata_core-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/exec/Commands.py` & `opengamedata_core-0.0.2/src/ogd/core/exec/Commands.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/exec/Generators.py` & `opengamedata_core-0.0.2/src/ogd/core/exec/Generators.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/exec/Parsers.py` & `opengamedata_core-0.0.2/src/ogd/core/exec/Parsers.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/generators/Generator.py` & `opengamedata_core-0.0.2/src/ogd/core/generators/Generator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 ## import standard libraries
 import abc
+import logging
 from typing import List, Optional
 # import locals
 from ogd.core.schemas.Event import Event
 from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.utils.Logger import Logger
 
 ## @class ExtractorParams
 class GeneratorParameters:
     """Dumb struct to hold the data that should be available to every Generator.
     This just makes it easier to add/manage any new params,
     so that we don't need to change the param list for hundreds of individual
     extractor subclasses every time something changes.
@@ -66,27 +68,23 @@
         self._params = params
 
     def __str__(self):
         return f"{self.Name} : {self.Description}"
 
     # *** PUBLIC STATICS ***
 
-    # *** PUBLIC METHODS ***
-
-    @classmethod
-    def EventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return cls._eventFilter(mode=mode)
-
-    @classmethod
-    def FeatureFilter(cls, mode:ExtractionMode) -> List[str]:
-        return cls._featureFilter(mode=mode)
+    @staticmethod
+    def WarningMessage(message:str):
+        """
+        Simple wrapper for the Logger in utils, makes it easier for subclasses to print warning messages without extra imports.
 
-    def UpdateFromEvent(self, event:Event):
-        if self._validateEvent(event=event):
-            self._updateFromEvent(event=event)
+        :param message: The warning message to print
+        :type message: str
+        """
+        Logger.Log(message=message, level=logging.WARN, depth=3)
 
     ## Base function to get the minimum log version the feature can handle.
     @staticmethod
     def MinVersion() -> Optional[str]:
         """ Base function to get the minimum log version the feature can handle.
             A value of None will set no minimum, so all levels are accepted (unless a max is set).
             Typically default to None, unless there is a required element of the event data that was not added until a certain version.        
@@ -118,14 +116,28 @@
 
         Base function to give a list of which ExtractionModes an extractor will handle.
         :return: _description_
         :rtype: List[ExtractionMode]
         """
         return [ExtractionMode.POPULATION, ExtractionMode.PLAYER, ExtractionMode.SESSION, ExtractionMode.DETECTOR]
 
+    # *** PUBLIC METHODS ***
+
+    @classmethod
+    def EventFilter(cls, mode:ExtractionMode) -> List[str]:
+        return cls._eventFilter(mode=mode)
+
+    @classmethod
+    def FeatureFilter(cls, mode:ExtractionMode) -> List[str]:
+        return cls._featureFilter(mode=mode)
+
+    def UpdateFromEvent(self, event:Event):
+        if self._validateEvent(event=event):
+            self._updateFromEvent(event=event)
+
     # *** PROPERTIES ***
 
     @property
     def Name(self) -> str:
         return self._params._name
 
     @property
```

### Comparing `opengamedata-core-0.0.1/src/ogd/core/generators/GeneratorLoader.py` & `opengamedata_core-0.0.2/src/ogd/core/generators/GeneratorLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/generators/detectors/Detector.py` & `opengamedata_core-0.0.2/src/ogd/core/generators/detectors/Detector.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/generators/detectors/DetectorEvent.py` & `opengamedata_core-0.0.2/src/ogd/core/generators/detectors/DetectorEvent.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/generators/extractors/Extractor.py` & `opengamedata_core-0.0.2/src/ogd/core/generators/extractors/Extractor.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/generators/extractors/Feature.py` & `opengamedata_core-0.0.2/src/ogd/core/generators/extractors/Feature.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/generators/extractors/PerCountFeature.py` & `opengamedata_core-0.0.2/src/ogd/core/generators/extractors/PerCountFeature.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/generators/extractors/PerLevelFeature.py` & `opengamedata_core-0.0.2/src/ogd/core/generators/extractors/PerLevelFeature.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/generators/extractors/SessionFeature.py` & `opengamedata_core-0.0.2/src/ogd/core/generators/extractors/SessionFeature.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/generators/legacy/LegacyDetector.py` & `opengamedata_core-0.0.2/src/ogd/core/generators/legacy/LegacyDetector.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/generators/legacy/LegacyFeature.py` & `opengamedata_core-0.0.2/src/ogd/core/generators/legacy/LegacyFeature.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/generators/legacy/LegacyLoader.py` & `opengamedata_core-0.0.2/src/ogd/core/generators/legacy/LegacyLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/generators/registries/DetectorRegistry.py` & `opengamedata_core-0.0.2/src/ogd/core/generators/registries/DetectorRegistry.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/generators/registries/ExtractorRegistry.py` & `opengamedata_core-0.0.2/src/ogd/core/generators/registries/ExtractorRegistry.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/generators/registries/GeneratorRegistry.py` & `opengamedata_core-0.0.2/src/ogd/core/generators/registries/GeneratorRegistry.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/interfaces/BQFirebaseInterface.py` & `opengamedata_core-0.0.2/src/ogd/core/interfaces/BQFirebaseInterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/interfaces/BigQueryCodingInterface.py` & `opengamedata_core-0.0.2/src/ogd/core/interfaces/BigQueryCodingInterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/interfaces/BigQueryInterface.py` & `opengamedata_core-0.0.2/src/ogd/core/interfaces/BigQueryInterface.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import logging
 import os
 from datetime import datetime, date
 from google.cloud import bigquery
+from google.api_core.exceptions import BadRequest
 from typing import Dict, Final, List, Tuple, Optional
 # import locals
 from ogd.core.interfaces.DataInterface import DataInterface
 from ogd.core.schemas.IDMode import IDMode
 from ogd.core.schemas.configs.GameSourceSchema import GameSourceSchema
 from ogd.core.schemas.configs.data_sources.BigQuerySourceSchema import BigQuerySchema
 from ogd.core.utils.Logger import Logger
@@ -48,104 +49,131 @@
     def _close(self) -> bool:
         self._client.close()
         self._is_open = False
         Logger.Log("Closed connection to BigQuery.", logging.DEBUG)
         return True
 
     def _allIDs(self) -> List[str]:
+        ret_val = []
+
         query = f"""
             SELECT DISTINCT session_id
             FROM `{self.DBPath()}`,
         """
         Logger.Log(f"Running query for all ids:\n{query}", logging.DEBUG, depth=3)
-        data = self._client.query(query)
-        ids = [str(row['session_id']) for row in data]
-        return ids if ids != None else []
+        try:
+            data = self._client.query(query)
+            session_ids = [str(row['session_id']) for row in data]
+        except BadRequest as err:
+            Logger.Log(f"In _allIDs, got a BadRequest error when trying to retrieve data from BigQuery, defaulting to empty result!\n{err}")
+        else:
+            ret_val = session_ids
+        return ret_val
 
     def _fullDateRange(self) -> Dict[str, datetime]:
+        ret_val : Dict[str, datetime] = {}
+
         query = f"""
             SELECT MIN(server_time), MAX(server_time)
             FROM `{self.DBPath()}`
         """
         Logger.Log(f"Running query for full date range:\n{query}", logging.DEBUG, depth=3)
-        data = list(self._client.query(query))
-        return {'min':data[0][0], 'max':data[0][1]}
+        try:
+            data = list(self._client.query(query))
+            date_range : Dict[str, datetime] = { 'min':data[0][0], 'max':data[0][1] }
+        except BadRequest as err:
+            Logger.Log(f"In _fullDateRange, got a BadRequest error when trying to retrieve data from BigQuery, defaulting to empty result!\n{err}")
+        else:
+            ret_val = date_range
+        return ret_val
 
     def _rowsFromIDs(self, id_list:List[str], id_mode:IDMode=IDMode.SESSION, versions:Optional[List[int]] = None, exclude_rows:Optional[List[str]]=None) -> List[Tuple]:
         # 2) Set up clauses to select based on Session ID or Player ID.
-        events = None
+        ret_val = []
         if self._client != None:
             query = self._generateRowFromIDQuery(id_list=id_list, id_mode=id_mode, exclude_rows=exclude_rows)
             Logger.Log(f"Running query for rows from IDs:\n{query}", logging.DEBUG, depth=3)
-            data = self._client.query(query)
-            events = []
-            for row in data:
-                items = tuple(row.items())
-                event = []
-                for item in items:
-                    match item[0]:
-                        case "event_params":
-                            _params = {param['key']:param['value'] for param in item[1]}
-                            event.append(json.dumps(_params, sort_keys=True))
-                        case "device" | "geo":
-                            event.append(json.dumps(item[1], sort_keys=True))
-                        case _:
-                            event.append(item[1])
-                events.append(tuple(event))
-        return events if events != None else []
+            try:
+                data = self._client.query(query)
+                Logger.Log(f"...Query yielded results, with query in state: {data.state}", logging.DEBUG, depth=3)
+            except BadRequest as err:
+                Logger.Log(f"In _rowsFromIDs, got a BadRequest error when trying to retrieve data from BigQuery, defaulting to empty result!\n{err}")
+            else:
+                for row in data:
+                    items = tuple(row.items())
+                    event = []
+                    for item in items:
+                        match item[0]:
+                            case "event_params":
+                                _params = {param['key']:param['value'] for param in item[1]}
+                                event.append(json.dumps(_params, sort_keys=True))
+                            case "device" | "geo":
+                                event.append(json.dumps(item[1], sort_keys=True))
+                            case _:
+                                event.append(item[1])
+                    ret_val.append(tuple(event))
+        return ret_val
 
     def _IDsFromDates(self, min:datetime, max:datetime, versions:Optional[List[int]] = None) -> List[str]:
         ret_val = []
         str_min, str_max = min.strftime("%Y%m%d"), max.strftime("%Y%m%d")
         query = f"""
             SELECT DISTINCT session_id
             FROM `{self.DBPath(min_date=min.date(), max_date=max.date())}`
             WHERE _TABLE_SUFFIX BETWEEN '{str_min}' AND '{str_max}'
         """
         Logger.Log(f"Running query for ids from dates:\n{query}", logging.DEBUG, depth=3)
-        data = self._client.query(query)
-        ids = [str(row['session_id']) for row in data]
-        if ids is not None:
+        try:
+            data = self._client.query(query)
+            ids = [str(row['session_id']) for row in data]
+        except BadRequest as err:
+            Logger.Log(f"In _IDsFromDates, got a BadRequest error when trying to retrieve data from BigQuery, defaulting to empty result!\n{err}")
+        else:
             ret_val = ids
-        Logger.Log(f"Found {len(ret_val)} ids. {ret_val if len(ret_val) <= 5 else ''}", logging.DEBUG, depth=3)
+            Logger.Log(f"Found {len(ret_val)} ids. {ret_val if len(ret_val) <= 5 else ''}", logging.DEBUG, depth=3)
         return ret_val
 
     def _datesFromIDs(self, id_list:List[str], id_mode:IDMode=IDMode.SESSION, versions:Optional[List[int]] = None) -> Dict[str, datetime]:
+        ret_val : Dict[str, datetime] = {}
+
         match id_mode:
             case IDMode.SESSION:
-                id_string = ','.join([f"{x}" for x in id_list])
+                id_string = ','.join([f"'{x}'" for x in id_list])
                 where_clause = f"WHERE session_id IN ({id_string})"
             case IDMode.USER:
                 id_string = ','.join([f"'{x}'" for x in id_list])
                 where_clause = f"WHERE user_id IN ({id_string})"
             case _:
                 Logger.Log(f"Invalid ID mode given (name={id_mode.name}, val={id_mode.value}), defaulting to session mode.", logging.WARNING, depth=3)
                 id_string = ','.join([f"{x}" for x in id_list])
                 where_clause = f"WHERE session_id IN ({id_string})"
         query = f"""
             SELECT MIN(server_time), MAX(server_time)
             FROM `{self.DBPath()}`
             {where_clause}
         """
         Logger.Log(f"Running query for dates from IDs:\n{query}", logging.DEBUG, depth=3)
-        data = list(self._client.query(query))
-        Logger.Log(f"...Query yielded results:\n{data}", logging.DEBUG, depth=3)
-        ret_val : Dict[str, datetime] = {}
-        if len(data) == 1:
-            dates = data[0]
-            if len(dates) == 2 and dates[0] is not None and dates[1] is not None:
-                _min = dates[0] if type(dates[0]) == datetime else datetime.strptime(str(dates[0]), "%m-%d-%Y %H:%M:%S")
-                _max = dates[1] if type(dates[1]) == datetime else datetime.strptime(str(dates[1]), "%m-%d-%Y %H:%M:%S")
-                ret_val = {'min':_min, 'max':_max}
+        try:
+            data = list(self._client.query(query))
+            Logger.Log(f"...Query yielded results:\n{data}", logging.DEBUG, depth=3)
+        except BadRequest as err:
+            Logger.Log(f"In _datesFromIDs, got a BadRequest error when trying to retrieve data from BigQuery, defaulting to empty result!\n{err}", logging.WARNING)
+        else:
+            if len(data) == 1:
+                dates = data[0]
+                if len(dates) == 2 and dates[0] is not None and dates[1] is not None:
+                    _min = dates[0] if type(dates[0]) == datetime else datetime.strptime(str(dates[0]), "%m-%d-%Y %H:%M:%S")
+                    _max = dates[1] if type(dates[1]) == datetime else datetime.strptime(str(dates[1]), "%m-%d-%Y %H:%M:%S")
+                    ret_val = {'min':_min, 'max':_max}
+                else:
+                    Logger.Log(f"BigQueryInterface query did not give both a min and a max, setting both to 'now'", logging.WARNING, depth=3)
+                    ret_val = {'min':datetime.now(), 'max':datetime.now()}
             else:
-                Logger.Log(f"BigQueryInterface query did not give both a min and a max, setting both to 'now'", logging.WARNING, depth=3)
+                Logger.Log(f"BigQueryInterface query did not return any results, setting both min and max to 'now'", logging.WARNING, depth=3)
                 ret_val = {'min':datetime.now(), 'max':datetime.now()}
-        else:
-            Logger.Log(f"BigQueryInterface query did not return any results, setting both min and max to 'now'", logging.WARNING, depth=3)
-            ret_val = {'min':datetime.now(), 'max':datetime.now()}
         return ret_val
 
     # *** PUBLIC STATICS ***
 
     # *** PUBLIC METHODS ***
 
     def IsOpen(self) -> bool:
```

### Comparing `opengamedata-core-0.0.1/src/ogd/core/interfaces/CSVInterface.py` & `opengamedata_core-0.0.2/src/ogd/core/interfaces/CSVInterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/interfaces/CodingInterface.py` & `opengamedata_core-0.0.2/src/ogd/core/interfaces/CodingInterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/interfaces/DataInterface.py` & `opengamedata_core-0.0.2/src/ogd/core/interfaces/DataInterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/interfaces/Interface.py` & `opengamedata_core-0.0.2/src/ogd/core/interfaces/Interface.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/interfaces/MySQLInterface.py` & `opengamedata_core-0.0.2/src/ogd/core/interfaces/MySQLInterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/interfaces/outerfaces/DataOuterface.py` & `opengamedata_core-0.0.2/src/ogd/core/interfaces/outerfaces/DataOuterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/interfaces/outerfaces/DebugOuterface.py` & `opengamedata_core-0.0.2/src/ogd/core/interfaces/outerfaces/DebugOuterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/interfaces/outerfaces/DictionaryOuterface.py` & `opengamedata_core-0.0.2/src/ogd/core/interfaces/outerfaces/DictionaryOuterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/interfaces/outerfaces/TSVOuterface.py` & `opengamedata_core-0.0.2/src/ogd/core/interfaces/outerfaces/TSVOuterface.py`

 * *Files 1% similar despite different names*

```diff
@@ -332,16 +332,19 @@
                     os.rename(_existing_sess_file, str(self._zip_paths['sessions']))
                 if _existing_players_file is not None and Path(_existing_players_file).is_file() and self._zip_paths['players'] is not None:
                     Logger.Log(f"Renaming {str(_existing_players_file)} -> {self._zip_paths['players']}", logging.DEBUG)
                     os.rename(_existing_players_file, str(self._zip_paths['players']))
                 if _existing_pop_file is not None and Path(_existing_pop_file).is_file() and self._zip_paths['population'] is not None:
                     Logger.Log(f"Renaming {str(_existing_pop_file)} -> {self._zip_paths['population']}", logging.DEBUG)
                     os.rename(_existing_pop_file, str(self._zip_paths['population']))
+            except FileExistsError as err:
+                msg = f"Error while setting up zip files, could not rename an existing file because another file is already using the target name! {err}"
+                Logger.Log(msg, logging.ERROR)
             except Exception as err:
-                msg = f"Error while setting up zip files! {type(err)} : {err}"
+                msg = f"Unexpected error while setting up zip files! {type(err)} : {err}"
                 Logger.Log(msg, logging.ERROR)
                 traceback.print_tb(err.__traceback__)
         # for each file, try to save out the csv/tsv to a file - if it's one that should be exported, that is.
         if self._zip_paths['population'] is not None:
             with zipfile.ZipFile(self._zip_paths["population"], "w", compression=zipfile.ZIP_DEFLATED) as population_zip_file:
                 try:
                     population_file = Path(self._dataset_id) / f"{self._dataset_id}_{self._short_hash}_population-features.{self._extension}"
```

### Comparing `opengamedata-core-0.0.1/src/ogd/core/managers/EventManager.py` & `opengamedata_core-0.0.2/src/ogd/core/managers/EventManager.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/managers/ExportManager.py` & `opengamedata_core-0.0.2/src/ogd/core/managers/ExportManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,16 +86,19 @@
             # Output population/player features as post-slicing data.
             Logger.Log(f"Outputting post-process data...", logging.INFO, depth=2)
             self._postProcess(request=request)
             Logger.Log(f"Done", logging.INFO)
 
             ret_val.SessionCount = len(_sess_ids)
             ret_val.RequestSucceeded(msg=f"Successfully executed data request {request}.")
+        except ValueError as err:
+            msg = f"Failed to execute data request {str(request)}, an invalid value was found:\n{str(err)}"
+            ret_val.RequestErrored(msg=msg)
         except Exception as err:
-            msg = f"Failed to execute data request {str(request)}, an error occurred:\n{type(err)} {str(err)}\n{traceback.format_exc()}"
+            msg = f"Failed to execute data request {str(request)}, an unexpected error occurred:\n{type(err)} {str(err)}\n{traceback.format_exc()}"
             ret_val.RequestErrored(msg=msg)
         finally:
             time_delta = datetime.now() - start
             ret_val.Duration = time_delta
             return ret_val
 
     # *** PRIVATE STATICS ***
@@ -109,15 +112,15 @@
             self._debug_count += 1
         self._processEvent(next_event=event)
 
     def _preProcess(self, request:Request) -> None:
         _games_path  = Path(games.__file__) if Path(games.__file__).is_dir() else Path(games.__file__).parent
         _game_schema  : GameSchema  = GameSchema.FromFile(game_id=request.GameID, schema_path=_games_path / request.GameID / "schemas")
         # 1. Get LoaderClass and set up Event and Feature managers.
-        load_class = self._loadLoaderClass(request.GameID)
+        load_class = ExportManager._loadLoaderClass(request.GameID)
         if load_class is None:
             # If game doesn't have an extractor, make sure we don't try to export it.
             request.RemoveExportMode(ExportMode.DETECTORS)
             request.RemoveExportMode(ExportMode.SESSION)
             request.RemoveExportMode(ExportMode.PLAYER)
             request.RemoveExportMode(ExportMode.POPULATION)
 
@@ -162,15 +165,16 @@
 
     def _postProcess(self, request:Request):
         start = datetime.now()
         self._outputPostSlice(request=request)
         time_delta = datetime.now() - start
         Logger.Log(f"Output time for population: {time_delta}", logging.INFO, depth=2)
 
-    def _loadLoaderClass(self, game_id:str) -> Optional[Type[GeneratorLoader]]:
+    @staticmethod
+    def _loadLoaderClass(game_id:str) -> Optional[Type[GeneratorLoader]]:
         _loader_class: Optional[Type[GeneratorLoader]] = None
         match game_id:
             case "AQUALAB":
                 from ogd.games.AQUALAB.AqualabLoader import AqualabLoader
                 _loader_class = AqualabLoader
             case "CRYSTAL":
                 from ogd.games.CRYSTAL.CrystalLoader import CrystalLoader
@@ -202,19 +206,19 @@
             case "WAVES":
                 from ogd.games.WAVES.WaveLoader import WaveLoader
                 _loader_class = WaveLoader
             case "PENGUINS":
                 from ogd.games.PENGUINS.PenguinsLoader import PenguinsLoader
                 _loader_class = PenguinsLoader
             case _:
-                if game_id in {"BACTERIA", "BALLOON", "CYCLE_CARBON", "CYCLE_NITROGEN", "CYCLE_WATER", "EARTHQUAKE", "MASHOPOLIS", "WIND"}:
+                if game_id in {"BACTERIA", "BALLOON", "CYCLE_CARBON", "CYCLE_NITROGEN", "CYCLE_WATER", "EARTHQUAKE", "MASHOPOLIS", "WEATHER_STATION", "WIND"}:
                     # all games with data but no extractor.
                     pass
                 else:
-                    raise Exception(f"Got an invalid game ID ({game_id})!")
+                    raise ValueError(f"Got an unrecognized game ID ({game_id})!")
         return _loader_class
 
     def _generateSlices(self, sess_ids:List[str]) -> List[List[str]]:
         _num_sess = len(sess_ids)
         _slice_size = self._config.BatchSize
         Logger.Log(f"With slice size = {_slice_size}, there are {math.ceil(_num_sess / _slice_size)} slices", logging.INFO, depth=1)
         return [[sess_ids[i] for i in range( j*_slice_size, min((j+1)*_slice_size, _num_sess) )]
```

### Comparing `opengamedata-core-0.0.1/src/ogd/core/managers/FeatureManager.py` & `opengamedata_core-0.0.2/src/ogd/core/managers/FeatureManager.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/processors/ClassroomDetector.py` & `opengamedata_core-0.0.2/src/ogd/core/processors/ClassroomDetector.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/processors/DetectorProcessor.py` & `opengamedata_core-0.0.2/src/ogd/core/processors/DetectorProcessor.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/processors/EventProcessor.py` & `opengamedata_core-0.0.2/src/ogd/core/processors/EventProcessor.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/processors/ExtractorProcessor.py` & `opengamedata_core-0.0.2/src/ogd/core/processors/ExtractorProcessor.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/processors/GeneratorProcessor.py` & `opengamedata_core-0.0.2/src/ogd/core/processors/GeneratorProcessor.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/processors/PlayerProcessor.py` & `opengamedata_core-0.0.2/src/ogd/core/processors/PlayerProcessor.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/processors/PopulationProcessor.py` & `opengamedata_core-0.0.2/src/ogd/core/processors/PopulationProcessor.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/processors/Processor.py` & `opengamedata_core-0.0.2/src/ogd/core/processors/Processor.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/processors/SessionProcessor.py` & `opengamedata_core-0.0.2/src/ogd/core/processors/SessionProcessor.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/requests/Request.py` & `opengamedata_core-0.0.2/src/ogd/core/requests/Request.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/requests/RequestResult.py` & `opengamedata_core-0.0.2/src/ogd/core/requests/RequestResult.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/schemas/Event.py` & `opengamedata_core-0.0.2/src/ogd/core/schemas/Event.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 from datetime import date, datetime, timedelta
 from enum import IntEnum
-from typing import List, Optional, Union
+from typing import Dict, List, Optional, Union
 
 from ogd.core.utils import utils
 class EventSource(IntEnum):
     GAME = 1
     GENERATED = 2
 
 ## @class Event
@@ -81,14 +81,33 @@
     def FallbackDefaults(self, app_id:Optional[str]=None, index:Optional[int]=None):
         if self.app_id == None and app_id != None:
             self.app_id = app_id
         if self.event_sequence_index == None:
             self.event_sequence_index = index
 
     @staticmethod
+    def FromJSON(json_data:Dict):
+        return Event(
+            session_id  =json_data.get("session_id", "SESSION ID NOT FOUND"),
+            app_id      =json_data.get("app_id", "APP ID NOT FOUND"),
+            timestamp   =json_data.get("client_time", "CLIENT TIME NOT FOUND"),
+            event_name  =json_data.get("event_name", "EVENT NAME NOT FOUND"),
+            event_data  =json_data.get("event_data", "EVENT DATA NOT FOUND"),
+            event_source=EventSource.GAME,
+            app_version =json_data.get("app_version", None),
+            app_branch  =json_data.get("app_branch", None),
+            log_version =json_data.get("log_version", None),
+            time_offset =None,
+            user_id     =json_data.get("user_id", None),
+            user_data   =json_data.get("user_data", None),
+            game_state  =json_data.get("game_state", None),
+            event_sequence_index=json_data.get("event_sequence_index", json_data).get("session_n", None)
+        )
+
+    @staticmethod
     def CompareVersions(a:str, b:str, version_separator='.') -> int:
         a_parts : Optional[List[int]]
         b_parts : Optional[List[int]]
         try:
             a_parts = [int(i) for i in a.split(version_separator)]
         except ValueError:
             a_parts = None
```

### Comparing `opengamedata-core-0.0.1/src/ogd/core/schemas/FeatureData.py` & `opengamedata_core-0.0.2/src/ogd/core/schemas/FeatureData.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/schemas/Schema.py` & `opengamedata_core-0.0.2/src/ogd/core/schemas/Schema.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/schemas/configs/ConfigSchema.py` & `opengamedata_core-0.0.2/src/ogd/core/schemas/configs/ConfigSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/schemas/configs/GameSourceSchema.py` & `opengamedata_core-0.0.2/src/ogd/core/schemas/configs/GameSourceSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/schemas/configs/IndexingSchema.py` & `opengamedata_core-0.0.2/src/ogd/core/schemas/configs/IndexingSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/schemas/configs/LegacyConfigSchema.py` & `opengamedata_core-0.0.2/src/ogd/core/schemas/configs/LegacyConfigSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/schemas/configs/data_sources/BigQuerySourceSchema.py` & `opengamedata_core-0.0.2/src/ogd/core/schemas/configs/data_sources/BigQuerySourceSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/schemas/configs/data_sources/DataSourceSchema.py` & `opengamedata_core-0.0.2/src/ogd/core/schemas/configs/data_sources/DataSourceSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/schemas/configs/data_sources/FileSourceSchema.py` & `opengamedata_core-0.0.2/src/ogd/core/schemas/configs/data_sources/FileSourceSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/schemas/configs/data_sources/MySQLSourceSchema.py` & `opengamedata_core-0.0.2/src/ogd/core/schemas/configs/data_sources/MySQLSourceSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/schemas/games/AggregateSchema.py` & `opengamedata_core-0.0.2/src/ogd/core/schemas/games/AggregateSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/schemas/games/DetectorMapSchema.py` & `opengamedata_core-0.0.2/src/ogd/core/schemas/games/DetectorMapSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/schemas/games/DetectorSchema.py` & `opengamedata_core-0.0.2/src/ogd/core/schemas/games/DetectorSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/schemas/games/EventDataElementSchema.py` & `opengamedata_core-0.0.2/src/ogd/core/schemas/games/DataElementSchema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # import standard libraries
 import logging
 from typing import Any, Dict, List, Optional
 # import local files
 from ogd.core.schemas.Schema import Schema
 from ogd.core.utils.Logger import Logger
 
-class EventDataElementSchema(Schema):
+class DataElementSchema(Schema):
     """
     Dumb struct to contain a specification of a data element from the EventData, GameState, or UserData attributes of an Event.
     """
     def __init__(self, name:str, all_elements:Dict[str, Any]):
         self._type        : str
         self._description : str
         self._details     : Optional[Dict[str, str]]
@@ -18,25 +18,25 @@
             if isinstance(all_elements, str):
                 all_elements = { 'description' : all_elements }
                 Logger.Log(f"For EventDataElement config of `{name}`, all_elements was a str, probably in legacy format. Defaulting to all_elements = {'{'} description : {all_elements['description']} {'}'}", logging.WARN)
             else:
                 all_elements = {}
                 Logger.Log(f"For EventDataElement config of `{name}`, all_elements was not a dict, defaulting to empty dict", logging.WARN)
         if "type" in all_elements.keys():
-            self._type = EventDataElementSchema._parseElementType(all_elements['type'])
+            self._type = DataElementSchema._parseElementType(all_elements['type'])
         else:
             self._type = "Unknown"
             Logger.Log(f"{name} EventDataElement config does not have a 'type' element; defaulting to type='{self._type}", logging.WARN)
         if "description" in all_elements.keys():
-            self._description = EventDataElementSchema._parseDescription(all_elements['description'])
+            self._description = DataElementSchema._parseDescription(all_elements['description'])
         else:
             self._description = "Unknown"
             Logger.Log(f"{name} EventDataElement config does not have a 'description' element; defaulting to description='{self._description}", logging.WARN)
         if "details" in all_elements.keys():
-            self._details = EventDataElementSchema._parseDetails(details=all_elements['details'])
+            self._details = DataElementSchema._parseDetails(details=all_elements['details'])
         else:
             self._details = None
         _leftovers = { key : val for key,val in all_elements.items() if key not in {"type", "description", "details"} }
         super().__init__(name=name, other_elements=_leftovers)
 
     @property
     def AsMarkdown(self) -> str:
```

### Comparing `opengamedata-core-0.0.1/src/ogd/core/schemas/games/EventSchema.py` & `opengamedata_core-0.0.2/src/ogd/core/schemas/games/EventSchema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # import standard libraries
 import logging
 from typing import Any, Dict, Optional
 # import local files
-from ogd.core.schemas.games.EventDataElementSchema import EventDataElementSchema
+from ogd.core.schemas.games.DataElementSchema import DataElementSchema
 from ogd.core.schemas.Schema import Schema
 from ogd.core.utils.Logger import Logger
 
 class EventSchema(Schema):
     """
     Dumb struct to contain a specification of an Event in a GameSchema file.
 
     These essentially are just a description of the event, and a set of elements in the EventData attribute of the Event.
     """
     def __init__(self, name:str, all_elements:Dict[str, Dict]):
         self._description : str                               = "No description available"
-        self._event_data  : Dict[str, EventDataElementSchema] = {}
+        self._event_data  : Dict[str, DataElementSchema] = {}
 
         if not isinstance(all_elements, dict):
             all_elements = {}
             Logger.Log(f"For {name} Event config, all_elements was not a dict, defaulting to empty dict", logging.WARN)
         if "description" in all_elements.keys():
             self._description = EventSchema._parseDescription(description=all_elements['description'])
         else:
@@ -33,15 +33,15 @@
         super().__init__(name=name, other_elements=_leftovers)
 
     @property
     def Description(self) -> str:
         return self._description
 
     @property
-    def EventData(self) -> Dict[str, EventDataElementSchema]:
+    def EventData(self) -> Dict[str, DataElementSchema]:
         return self._event_data
 
     @property
     def AsMarkdown(self) -> str:
         return "\n\n".join([
             f"### **{self.Name}**",
             self.Description,
@@ -70,17 +70,17 @@
                 [f"- **{elem_name}**: {elem_desc}  " for elem_name,elem_desc in self.NonStandardElements]
                 if len(self.NonStandardElements) > 0 else ["- None"]
             )
         ])
 
     @staticmethod
     def _parseEventDataElements(event_data):
-        ret_val : Dict[str, EventDataElementSchema]
+        ret_val : Dict[str, DataElementSchema]
         if isinstance(event_data, dict):
-            ret_val = {name:EventDataElementSchema(name=name, all_elements=elems) for name,elems in event_data.items()}
+            ret_val = {name:DataElementSchema(name=name, all_elements=elems) for name,elems in event_data.items()}
         else:
             ret_val = {}
             Logger.Log(f"event_data was unexpected type {type(event_data)}, defaulting to empty dict.", logging.WARN)
         return ret_val
 
     @staticmethod
     def _parseDescription(description):
```

### Comparing `opengamedata-core-0.0.1/src/ogd/core/schemas/games/ExtractorSchema.py` & `opengamedata_core-0.0.2/src/ogd/core/schemas/games/ExtractorSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/schemas/games/FeatureMapSchema.py` & `opengamedata_core-0.0.2/src/ogd/core/schemas/games/FeatureMapSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/schemas/games/FeatureSchema.py` & `opengamedata_core-0.0.2/src/ogd/core/schemas/games/FeatureSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/schemas/games/GameSchema.py` & `opengamedata_core-0.0.2/src/ogd/core/schemas/games/GameSchema.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from shutil import copyfile
 from typing import Any, Dict, List, Optional, Set, Tuple, Union
 # import local files
 from ogd.core.schemas.Schema import Schema
 from ogd.core.schemas.games.AggregateSchema import AggregateSchema
 from ogd.core.schemas.games.DetectorSchema import DetectorSchema
 from ogd.core.schemas.games.DetectorMapSchema import DetectorMapSchema
+from ogd.core.schemas.games.DataElementSchema import DataElementSchema
 from ogd.core.schemas.games.EventSchema import EventSchema
 from ogd.core.schemas.games.PerCountSchema import PerCountSchema
 from ogd.core.schemas.games.FeatureSchema import FeatureSchema
 from ogd.core.schemas.games.FeatureMapSchema import FeatureMapSchema
 from ogd.core.schemas.IterationMode import IterationMode
 from ogd.core.schemas.ExtractionMode import ExtractionMode
 from ogd.core.utils import utils
@@ -38,79 +39,127 @@
 
         :param schema_name: The name of the JSON schema file (if .json is not the file extension, .json will be appended)
         :type schema_name: str
         :param schema_path: schema_path Path to the folder containing the JSON schema file; if None is given, defaults to ./ogd/games/{game_id}/schemas/
         :type schema_path: str, optional
         """
     # 1. define instance vars
-        self._event_list             : List[EventSchema] = []
+        self._game_id                : str                                  = name
+        self._enum_defs              : Dict[str, List[str]]                 = {}
+        self._game_state             : Dict[str, Any]                       = {}
+        self._user_data              : Dict[str, Any]                       = {}
+        self._event_list             : List[EventSchema]                    = []
         self._detector_map           : Dict[str, Dict[str, DetectorSchema]] = {'perlevel':{}, 'per_count':{}, 'aggregate':{}}
         self._aggregate_feats        : Dict[str, AggregateSchema]           = {}
         self._percount_feats         : Dict[str, PerCountSchema]            = {}
         self._legacy_perlevel_feats  : Dict[str, PerCountSchema]            = {}
         self._legacy_mode            : bool                                 = False
-        self._game_id                : str                                  = name
-        self._config                 : Dict[str, Any]
-        self._game_state             : Dict[str, Any]
-        self._other_ranges           : Dict[str, range]
+        self._config                 : Dict[str, Any]                       = {}
         self._min_level              : Optional[int]                        = None
         self._max_level              : Optional[int]                        = None
+        self._other_ranges           : Dict[str, range]
         self._supported_vers         : Optional[List[int]]
-    # 2. set instance vars
+
         if not isinstance(all_elements, dict):
             all_elements   = {}
             Logger.Log(f"For {self._game_id} GameSchema, all_elements was not a dict, defaulting to empty dict", logging.WARN)
+
+    # 2. set instance vars, starting with event data
+
+        if "enums" in all_elements.keys():
+            self._enum_defs = GameSchema._parseEnumDefs(enums_list=all_elements['enums'])
+        else:
+            Logger.Log(f"{self._game_id} game schema does not specify any custom enums", logging.INFO)
+
+        if "game_state" in all_elements.keys():
+            self._game_state = GameSchema._parseGameState(game_state=all_elements['game_state'])
+        else:
+            Logger.Log(f"{self._game_id} game schema does not specify the structure of the game state colum, defaulting to empty dictn", logging.INFO)
+
+        if "user_data" in all_elements.keys():
+            self._user_data = GameSchema._parseUserData(user_data=all_elements['user_data'])
+        else:
+            Logger.Log(f"{self._game_id} game schema does not specify the structure of the user data colum, defaulting to empty dictn", logging.INFO)
         if "events" in all_elements.keys():
             self._event_list = GameSchema._parseEventList(events_list=all_elements['events'])
         else:
             Logger.Log(f"{self._game_id} game schema does not document any events.", logging.INFO)
+
+    # 3. Get detector information
         if "detectors" in all_elements.keys():
             # TODO : Just have DetectorMapSchema directly
             _detector_map = GameSchema._parseDetectorMap(detector_map=all_elements['detectors'])
             self._detector_map = _detector_map.AsDict
         else:
             Logger.Log(f"{self._game_id} game schema does not define any detectors.", logging.INFO)
+
+    # 4. Get feature information
         if "features" in all_elements.keys():
             # TODO : Just have the FeatureMapSchema directly, not 4 different things.
             _feat_map = GameSchema._parseFeatureMap(feature_map=all_elements['features'])
-            self._legacy_mode = _feat_map.LegacyMode
-            self._legacy_perlevel_feats.update(_feat_map.LegacyPerLevelFeatures)
-            self._percount_feats.update(_feat_map.PerCountFeatures)
             self._aggregate_feats.update(_feat_map.AggregateFeatures)
+            self._percount_feats.update(_feat_map.PerCountFeatures)
+            self._legacy_perlevel_feats.update(_feat_map.LegacyPerLevelFeatures)
+            self._legacy_mode = _feat_map.LegacyMode
         else:
             Logger.Log(f"{self._game_id} game schema does not define any features.", logging.INFO)
+
+    # 5. Get config, if any
+        if "config" in all_elements.keys():
+            self._config = all_elements['config']
+        else:
+            Logger.Log(f"{self._game_id} game schema does not define any config items.", logging.INFO)
+        if "SUPPORTED_VERS" in self._config:
+            self._supported_vers = self._config['SUPPORTED_VERS']
+        else:
+            self._supported_vers = None
+            Logger.Log(f"{self._game_id} game schema does not define supported versions, defaulting to support all versions.", logging.INFO)
+
+    # 6. Get level range and other ranges, if any
         if "level_range" in all_elements.keys():
             self._min_level, self._max_level = GameSchema._parseLevelRange(all_elements['level_range'])
         else:
             Logger.Log(f"{self._game_id} game schema does not define a level range.", logging.INFO)
-    # 7. Get other ranges, if any
+
         self._other_ranges = {key : range(val.get('min', 0), val.get('max', 1)) for key,val in all_elements.items() if key.endswith("_range")}
-    # 8. Get config, if any
-        self._config = all_elements.get('config', {})
-        if "SUPPORTED_VERS" in all_elements['config']:
-            self._supported_vers = all_elements['config']['SUPPORTED_VERS']
-        else:
-            self._supported_vers = None
-            Logger.Log(f"{self._game_id} game schema does not define supported versions, defaulting to support all versions.", logging.INFO)
-    # 9. Collect any other, unexpected elements
-        _leftovers = { key:val for key,val in all_elements.items() if key not in {'events', 'detectors', 'features', 'level_range', 'config'}.union(self._other_ranges.keys()) }
+
+    # 7. Collect any other, unexpected elements
+        _leftovers = { key:val for key,val in all_elements.items() if key not in {'enums', 'game_state', 'user_data', 'events', 'detectors', 'features', 'level_range', 'config'}.union(self._other_ranges.keys()) }
         super().__init__(name=self._game_id, other_elements=_leftovers)
 
     # *** BUILT-INS & PROPERTIES ***
 
     # def __getitem__(self, key) -> Any:
     #     return _schema[key] if _schema is not None else None
 
     @property
     def GameName(self) -> str:
         """Property for the name of the game configured by this schema
         """
         return self._game_id
 
     @property
+    def EnumDefs(self) -> Dict[str, List[str]]:
+        """Property for the dict of all enums defined for sub-elements in the given game's schema.
+        """
+        return self._enum_defs
+
+    @property
+    def GameState(self) -> Dict[str, Any]:
+        """Property for the dictionary describing the structure of the GameState column for the given game.
+        """
+        return self._game_state
+
+    @property
+    def UserData(self) -> Dict[str, Any]:
+        """Property for the dictionary describing the structure of the UserData column for the given game.
+        """
+        return self._user_data
+
+    @property
     def Events(self) -> List[EventSchema]:
         """Property for the list of events the game logs.
         """
         return self._event_list
 
     @property
     def EventTypes(self) -> List[str]:
@@ -197,16 +246,34 @@
     @property
     def Config(self) -> Dict[str, Any]:
         return self._config
 
     @property
     def AsMarkdown(self) -> str:
         event_summary = ["## Logged Events",
-                         "The individual fields encoded in the *event_data* Event element for each type of event logged by the game."
+                         "The individual fields encoded in the *game_state* and *user_data* Event element for all event types, and the fields in the *event_data* Event element for each individual event type logged by the game."
                         ]
+        enum_list     = ["### Enums",
+                         "\n".join(
+                             ["| **Name** | **Values** |",
+                             "| ---      | ---        |"]
+                         + [f"| {name} | {val_list} |" for name,val_list in self.EnumDefs.items()]
+                        )]
+        game_state_list = ["### Game State",
+                           "\n".join(
+                               ["| **Name** | **Type** | **Description** | **Sub-Elements** |",
+                               "| ---      | ---      | ---             | ---         |"]
+                           + [elem.AsMarkdownRow for elem in self.GameState.values()]
+                          )]
+        user_data_list = ["### User Data",
+                          "\n".join(
+                              ["| **Name** | **Type** | **Description** | **Sub-Elements** |",
+                              "| ---      | ---      | ---             | ---         |"]
+                          + [elem.AsMarkdownRow for elem in self.UserData.values()]
+                         )]
         # Set up list of events
         event_list = [event.AsMarkdownTable for event in self.Events] if len(self.Events) > 0 else ["None"]
         # Set up list of detectors
         detector_summary = ["## Detected Events",
                             "The custom, data-driven Events calculated from this game's logged events by OpenGameData when an 'export' is run."
                            ]
         detector_list = []
@@ -226,15 +293,16 @@
                          ]
         other_element_list = [ f"{key} : {self._other_elements[key]}" for key in self._other_elements.keys()]
         other_range_summary = ["### Other Ranges",
                          "Extra ranges specified in the game's schema, which may be referenced by event/feature processors."
                          ]
         other_range_list = [ f"{key} : {self.OtherRanges[key]}" for key in self.OtherRanges ]
 
-        ret_val = "  \n\n".join(event_summary + event_list
+        ret_val = "  \n\n".join(event_summary
+                              + enum_list + game_state_list + user_data_list + event_list
                               + detector_summary + detector_list
                               + feature_summary + feature_list
                               + other_summary + other_element_list
                               + other_range_summary + other_range_list)
 
         return ret_val
 
@@ -386,14 +454,45 @@
             except Exception as cp_err:
                 Logger.Log(       f"Could not copy {schema_name} from template, a {type(cp_err)} error occurred:\n{cp_err}", logging.WARN, depth=2)
                 print(f"(via print) Could not copy {schema_name} from template, a {type(cp_err)} error occurred:\n{cp_err}")
             else:
                 Logger.Log(       f"Successfully copied {schema_name} from template.", logging.DEBUG, depth=2)
         return ret_val
 
+
+    @staticmethod
+    def _parseEnumDefs(enums_list:Dict[str, Any]) -> Dict[str, List[str]]:
+        ret_val : Dict[str, List[str]]
+        if isinstance(enums_list, dict):
+            ret_val = enums_list
+        else:
+            ret_val = {}
+            Logger.Log(f"enums_list was unexpected type {type(enums_list)}, defaulting to empty Dict.", logging.WARN)
+        return ret_val
+
+    @staticmethod
+    def _parseGameState(game_state:Dict[str, Any]) -> Dict[str, DataElementSchema]:
+        ret_val : Dict[str, DataElementSchema]
+        if isinstance(game_state, dict):
+            ret_val = {name:DataElementSchema(name=name, all_elements=elems) for name,elems in game_state.items()}
+        else:
+            ret_val = {}
+            Logger.Log(f"game_state was unexpected type {type(game_state)}, defaulting to empty dict.", logging.WARN)
+        return ret_val
+
+    @staticmethod
+    def _parseUserData(user_data:Dict[str, Any]) -> Dict[str, DataElementSchema]:
+        ret_val : Dict[str, DataElementSchema]
+        if isinstance(user_data, dict):
+            ret_val = {name:DataElementSchema(name=name, all_elements=elems) for name,elems in user_data.items()}
+        else:
+            ret_val = {}
+            Logger.Log(f"user_data was unexpected type {type(user_data)}, defaulting to empty dict.", logging.WARN)
+        return ret_val
+
     @staticmethod
     def _parseEventList(events_list:Dict[str, Any]) -> List[EventSchema]:
         ret_val : List[EventSchema]
         if isinstance(events_list, dict):
             ret_val = [EventSchema(name=key, all_elements=val) for key,val in events_list.items()]
         else:
             ret_val = []
```

### Comparing `opengamedata-core-0.0.1/src/ogd/core/schemas/games/GameStateSchema.py` & `opengamedata_core-0.0.2/src/ogd/core/schemas/games/GameStateSchema.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # import standard libraries
 import logging
 from typing import Dict
 # import local files
-from ogd.core.schemas.games.EventDataElementSchema import EventDataElementSchema
+from ogd.core.schemas.games.DataElementSchema import DataElementSchema
 from ogd.core.schemas.Schema import Schema
 from ogd.core.utils.Logger import Logger
 
 class GameStateSchema(Schema):
     """
     Dumb struct to contain a specification of a game's GameState in a GameSchema file.
 
     These essentially are just a set of elements in the GameState attribute of the game's Events.
     """
     def __init__(self, name:str, all_elements:Dict[str, Dict]):
-        self._game_state  : Dict[str, EventDataElementSchema]
+        self._game_state  : Dict[str, DataElementSchema]
 
         if not isinstance(all_elements, dict):
             all_elements   = {}
             Logger.Log(f"For {name} Event config, all_elements was not a dict, defaulting to empty dict", logging.WARN)
         self._game_state = GameStateSchema._parseGameStateElements(event_data=all_elements)
         super().__init__(name=name, other_elements=None)
 
     @property
-    def GameStateElements(self) -> Dict[str, EventDataElementSchema]:
+    def GameStateElements(self) -> Dict[str, DataElementSchema]:
         return self._game_state
 
     @property
     def AsMarkdown(self) -> str:
         return "\n\n".join([
             f"### **{self.Name}**",
             "\n".join(
@@ -52,14 +52,14 @@
                 [f"- **{elem_name}**: {elem_desc}  " for elem_name,elem_desc in self.NonStandardElements]
                 if len(self.NonStandardElements) > 0 else ["- None"]
             )
         ])
 
     @staticmethod
     def _parseGameStateElements(event_data):
-        ret_val : Dict[str, EventDataElementSchema]
+        ret_val : Dict[str, DataElementSchema]
         if isinstance(event_data, dict):
-            ret_val = {name:EventDataElementSchema(name=name, all_elements=elems) for name,elems in event_data.items()}
+            ret_val = {name:DataElementSchema(name=name, all_elements=elems) for name,elems in event_data.items()}
         else:
             ret_val = {}
             Logger.Log(f"event_data was unexpected type {type(event_data)}, defaulting to empty dict.", logging.WARN)
         return ret_val
```

### Comparing `opengamedata-core-0.0.1/src/ogd/core/schemas/games/PerCountSchema.py` & `opengamedata_core-0.0.2/src/ogd/core/schemas/games/PerCountSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/schemas/table_schemas/BIGQUERY.json` & `opengamedata_core-0.0.2/src/ogd/core/schemas/table_schemas/BIGQUERY.json`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/schemas/table_schemas/FIELDDAY_MYSQL.json` & `opengamedata_core-0.0.2/src/ogd/core/schemas/table_schemas/FIELDDAY_MYSQL.json`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/schemas/table_schemas/FIREBASE.json` & `opengamedata_core-0.0.2/src/ogd/core/schemas/table_schemas/FIREBASE.json`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/schemas/table_schemas/MASHOPOLIS_MYSQL.json` & `opengamedata_core-0.0.2/src/ogd/core/schemas/table_schemas/MASHOPOLIS_MYSQL.json`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/schemas/table_schemas/OGD_EVENT_FILE.json` & `opengamedata_core-0.0.2/src/ogd/core/schemas/table_schemas/OGD_EVENT_FILE.json`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_BIGQUERY.json` & `opengamedata_core-0.0.2/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_BIGQUERY.json`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_MYSQL.json` & `opengamedata_core-0.0.2/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_MYSQL.json`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/schemas/table_schemas/SHIPWRECKS.json` & `opengamedata_core-0.0.2/src/ogd/core/schemas/table_schemas/SHIPWRECKS.json`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/schemas/tables/ColumnMapSchema.py` & `opengamedata_core-0.0.2/src/ogd/core/schemas/tables/ColumnMapSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/schemas/tables/ColumnSchema.py` & `opengamedata_core-0.0.2/src/ogd/core/schemas/tables/ColumnSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/schemas/tables/TableSchema.py` & `opengamedata_core-0.0.2/src/ogd/core/schemas/tables/TableSchema.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,15 +334,15 @@
                      app_version=app_ver, app_branch=app_br, log_version=log_ver,
                      time_offset=offset, user_id=uid, user_data=udata,
                      game_state=state, event_sequence_index=index)
 
     # *** PRIVATE STATICS ***
 
     @staticmethod
-    def _parse(input:str, col_schema:ColumnSchema) -> Any:
+    def _parse(input:Any, col_schema:ColumnSchema) -> Any:
         """Applies whatever parsing is appropriate based on what type the schema said a column contained.
 
         :param input: _description_
         :type input: str
         :param col_schema: _description_
         :type col_schema: ColumnSchema
         :return: _description_
@@ -359,22 +359,28 @@
         elif col_schema.ValueType == 'float':
             return float(input)
         elif col_schema.ValueType == 'datetime':
             return input if isinstance(input, datetime) else TableSchema._convertDateTime(str(input))
         elif col_schema.ValueType == 'timedelta':
             return input if isinstance(input, timedelta) else TableSchema._convertTimedelta(str(input))
         elif col_schema.ValueType == 'json':
-            if input != 'None' and input != '': # watch out for nasty corner cases.
-                try:
+            try:
+                if isinstance(input, dict):
+                    # if input was a dict already, then just give it back. Else, try to load it from string.
+                    return input
+                elif isinstance(input, str):
+                    if input != 'None' and input != '': # watch out for nasty corner cases.
+                        return json.loads(input)
+                    else:
+                        return None
+                else:
                     return json.loads(str(input))
-                except JSONDecodeError as err:
-                    Logger.Log(f"Could not parse input '{input}' of type {type(input)} from column {col_schema.Name}, got the following error:\n{str(err)}", logging.WARN)
-                    return {}
-            else:
-                return None
+            except JSONDecodeError as err:
+                Logger.Log(f"Could not parse input '{input}' of type {type(input)} from column {col_schema.Name}, got the following error:\n{str(err)}", logging.WARN)
+                return {}
         elif col_schema.ValueType.startswith('enum'):
             # if the column is supposed to be an enum, for now we just stick with the string.
             return str(input)
 
     @staticmethod
     def _convertDateTime(time_str:str) -> datetime:
         ret_val : datetime
```

### Comparing `opengamedata-core-0.0.1/src/ogd/core/utils/Logger.py` & `opengamedata_core-0.0.2/src/ogd/core/utils/Logger.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/utils/Readme.py` & `opengamedata_core-0.0.2/src/ogd/core/utils/Readme.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/core/utils/utils.py` & `opengamedata_core-0.0.2/src/ogd/core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/ALL_YOU_CAN_ET/schemas/ALL_YOU_CAN_ET.json.template` & `opengamedata_core-0.0.2/src/ogd/games/ALL_YOU_CAN_ET/schemas/ALL_YOU_CAN_ET.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/AqualabLoader.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/AqualabLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/DBExport.json` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/DBExport.json`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/detectors/CollectFactNoJob.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/detectors/CollectFactNoJob.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/detectors/DiveSiteNoEvidence.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/detectors/DiveSiteNoEvidence.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/detectors/EchoRoomChange.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/detectors/EchoRoomChange.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/detectors/HintAndLeave.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/detectors/HintAndLeave.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/detectors/Idle.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/detectors/Idle.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/detectors/SceneChangeFrequently.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/detectors/SceneChangeFrequently.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/detectors/TwoHints.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/detectors/TwoHints.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/ActiveJobs.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/ActiveJobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,9 +59,9 @@
 
     # *** Other local functions
     def _validate_job(self, job_data):
         ret_val : bool = False
         if job_data and job_data in self._job_map:
             ret_val = True
         else:
-            Logger.Log(f"Got invalid job_name data in JobsAttempted", logging.WARNING)
+            self.WarningMessage(f"Got invalid job_name data in JobsAttempted")
         return ret_val
```

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/ActiveTime.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/ActiveTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/EchoSessionID.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/EchoSessionID.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/EventList.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/EventList.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/JobActiveTime.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobActiveTime.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,18 +15,17 @@
     def __init__(self, params:GeneratorParameters, job_map:dict):
         super().__init__(params=params, job_map=job_map)
         self._total_time = timedelta(0)
         if self.ExtractionMode == ExtractionMode.PLAYER:
             self._session_id      = None
             self._last_start_time = None
             self._last_event_time = None
-        elif self.ExtractionMode == ExtractionMode.POPULATION:
-            self._session_id      = None
-            self._last_start_time = None
-            self._last_event_time = None
+            self._last_event_session = None
+            self._last_event_name = None
+            self._last_event_index = None
         else:
             raise NotImplementedError(f"Got invalid export mode of {self.ExtractionMode.name} in JobActiveTime!")
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
         return ["all_events"]
@@ -43,57 +42,50 @@
         #     return ["JobActiveTime"]
         # else:
         #     return []
 
     def _updateFromEvent(self, event:Event) -> None:
         self._player_id = event.UserID
         if event.SessionID != self._session_id:
-            _old_sess = self._session_id
-            self._session_id = event.SessionID
-            # if we jumped to a new session, we only want to count time up to last event, then skip the time between sessions to new timestamp;
-            # but only if we had a previous session, i.e. this isn't the first event seen.
-            if _old_sess is not None:
-                # Logger.Log(f"JobActiveTime attempting to update total time for {event.UserID} ({_old_sess} -> {self._session_id}) following change in session, index={event.EventSequenceIndex}", logging.INFO)
-                self._updateTotalTime()
-                # Logger.Log("Done", logging.INFO)
-                self._last_start_time = event.timestamp
-                if event.Timestamp is None:
-                    Logger.Log(f"JobActiveTime received an initial event with Timestamp == None!", logging.WARN)
+            self._handleNewSession(event)
 
         if event.EventName == "accept_job":
             self._last_start_time = event.timestamp
         elif event.EventName == "switch_job":
             new_job = event.GameState.get('job_name', event.EventData.get('job_name', None))
             if new_job is None:
                 raise KeyError("Could not find key 'job_name' in GameState or EventData!")
             old_job = event.EventData["prev_job_name"]
             # if we switched into "this" job, this becomes new start time
             if self._job_map.get(new_job, None) == self.CountIndex:
                 self._last_start_time = event.Timestamp
                 if event.Timestamp is None:
-                    Logger.Log(f"JobActiveTime received a switch_job event with Timestamp == None!", logging.WARN)
+                    self.WarningMessage(f"JobActiveTime received a switch_job event with Timestamp == None!")
             # if we switched out of "this" job, update total time in the job.
             # note, if "this" job is no-active-job, we don't care. Further, if we switched into no-active-job, then we just completed a job and don't care.
             elif self._job_map.get(old_job, None) == self.CountIndex and new_job != "no-active-job" and old_job != "no-active-job":
                 self._updateTotalTime()
         elif event.EventName == "complete_job":
             self._updateTotalTime()
         # if we got an event unrelated to job change, but didn't have a start (e.g. new session started mid-job), then make now the start.
         elif self._last_start_time is None:
             self._last_start_time = event.Timestamp
         # if we got an event earlier than last start, we are out of order
         elif self._last_start_time > event.Timestamp:
-            Logger.Log(f"Got out-of-order events in JobActiveTime; event {event.EventName}:{event.EventSequenceIndex} had timestamp {event.Timestamp} earlier than start event, with time {self._last_start_time}!", logging.WARN)
+            self.WarningMessage(f"Got out-of-order events in JobActiveTime; event {event.EventName}:{event.EventSequenceIndex} had timestamp {event.Timestamp} earlier than start event, with time {self._last_start_time}!")
             self._last_start_time = event.Timestamp
 
         # finally, update latest timestamp
         if self._last_event_time and self._last_event_time > event.Timestamp:
-            Logger.Log(f"Got out-of-order events in SessionDuration; event {event.EventName}:{event.EventSequenceIndex} had timestamp {event.Timestamp} earlier than end event, with time {self._last_event_time}!", logging.WARN)
+            self.WarningMessage(f"Got out-of-order events in SessionDuration; event {event.EventName}:{event.EventSequenceIndex} had timestamp {event.Timestamp} earlier than end event, with time {self._last_event_time}!")
         else:
             self._last_event_time = event.timestamp
+            self._last_event_session = event.SessionID
+            self._last_event_name = event.UserID
+            self._last_event_index = event.EventSequenceIndex
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
         # if self.ExtractionMode == ExtractionMode.PLAYER \
         # or self.ExtractionMode == ExtractionMode.SESSION:
         #     pass
         # elif self.ExtractionMode == ExtractionMode.POPULATION:
@@ -113,15 +105,15 @@
                     ret_val = True
             elif event.EventName == "switch_job":
                 # if we got switch job, and were switching away from this instance's job, we still want to process it.
                 old_job = event.EventData["prev_job_name"]
                 if self._job_map.get(old_job, None) == self.CountIndex:
                     ret_val = True
         else:
-            Logger.Log(f"Got invalid job_name data in {type(self).__name__}", logging.WARNING)
+            self.WarningMessage(f"Got invalid job_name data in {type(self).__name__}")
 
         return ret_val
 
 
     # *** Optionally override public functions. ***
 
     @staticmethod
@@ -130,23 +122,54 @@
 
     @staticmethod
     def AvailableModes() -> List[ExtractionMode]:
         return [ExtractionMode.PLAYER]
 
     # *** PRIVATE METHODS ***
 
+    def _handleNewSession(self, event:Event):
+            _old_sess = self._session_id
+            self._session_id = event.SessionID
+            # if we jumped to a new session, we only want to count time up to last event, then skip the time between sessions to new timestamp;
+            # but only if we had a previous session, i.e. this isn't the first event seen.
+            if _old_sess is not None:
+                # Logger.Log(f"JobActiveTime attempting to update total time for {event.UserID} ({_old_sess} -> {self._session_id}) following change in session, index={event.EventSequenceIndex}", logging.INFO)
+                self._updateTotalTime()
+                # Logger.Log("Done", logging.INFO)
+                if event.app_version == 'Aqualab' or event.app_version == 'None':
+                    current_job = event.EventData.get("job_name", {}).get('string_value')
+                else:
+                    current_job = event.EventData.get("job_name")
+                if current_job is not None and self._job_map.get(current_job, None) == self.CountIndex:
+                    self._last_start_time = event.Timestamp
+                    self._last_event_time = event.Timestamp
+                if event.Timestamp is None:
+                    Logger.Log(f"JobActiveTime received an initial event with Timestamp == None!", logging.WARN)
+            # _old_sess = self._session_id
+            # self._session_id = event.SessionID
+            # # if we jumped to a new session, we only want to count time up to last event, then skip the time between sessions to new timestamp;
+            # # but only if we had a previous session, i.e. this isn't the first event seen.
+            # if _old_sess is not None:
+            #     # Logger.Log(f"JobActiveTime attempting to update total time for {event.UserID} ({_old_sess} -> {self._session_id}) following change in session, index={event.EventSequenceIndex}", logging.INFO)
+            #     self._updateTotalTime()
+            #     # Logger.Log("Done", logging.INFO)
+            #     self._last_start_time = event.timestamp
+            #     if event.Timestamp is None:
+            #         self.WarningMessage(f"JobActiveTime received an initial event with Timestamp == None!")
+
     def _updateTotalTime(self):
         if self._last_start_time:
             if self._last_event_time:
                 self._total_time += (self._last_event_time - self._last_start_time)
                 self._last_start_time = None
+                self._last_event_time = None
             else:
-                Logger.Log(f"JobActiveTime could not update total time, missing previous event time!", logging.WARNING)
+                self.WarningMessage(f"JobActiveTime could not update total time, missing previous event time!")
         elif self.ExtractionMode == ExtractionMode.PLAYER:
-            Logger.Log(f"JobActiveTime could not update total time for player {self._player_id}, session {self._session_id} missing start time!", logging.WARNING)
+            self.WarningMessage(f"JobActiveTime could not update total time for player {self._player_id}, session {self._session_id} missing start time!")
 
     # def _handle_population(self, feature:FeatureData):
     #     if feature.ExportMode == ExtractionMode.PLAYER:
     #         _val = feature.FeatureValues[0]
     #         if type(_val) == timedelta:
     #             self._total_seconds += _val
     #         else:
```

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/JobArgumentationTime.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobArgumentationTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/JobCompletionTime.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobCompletionTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/JobDiveSitesCount.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobDiveSitesCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/JobDiveTime.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobDiveTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/JobExperimentationTime.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobExperimentationTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/JobGuideCount.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobGuideCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/JobHelpCount.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobHelpCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/JobLocationChanges.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobLocationChanges.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/JobModelingTime.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobModelingTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/JobStartCount.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobStartCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/JobTasksCompleted.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobTasksCompleted.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/JobTriesInArgument.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobTriesInArgument.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/JobsAttempted.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobsAttempted.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,9 +133,9 @@
 
     # *** Other local functions
     def _validate_job(self, job_data):
         ret_val : bool = False
         if job_data and job_data in self._job_map:
             ret_val = True
         else:
-            Logger.Log(f"Got invalid job_name data in JobsAttempted", logging.WARNING)
+            self.WarningMessage(f"Got invalid job_name data in JobsAttempted")
         return ret_val
```

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/JobsCompleted.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobsCompleted.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/ModelExportCount.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/ModelExportCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/ModelInterveneCount.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/ModelInterveneCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/ModelPredictCount.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/ModelPredictCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/PerJobFeature.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/PerJobFeature.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         ret_val : bool = False
 
         job_name = event.GameState.get('job_name', event.EventData.get('job_name', "JOB NAME NOT FOUND"))
         if job_name is not None:
             if job_name in self._job_map and self._job_map[job_name] == self.CountIndex:
                 ret_val = True
         else:
-            Logger.Log(f"Got invalid job_name data in {type(self).__name__}", logging.WARNING)
+            self.WarningMessage(f"Got invalid job_name data in {type(self).__name__}")
 
         return ret_val
 
     # *** Optionally override public functions. ***
 
     @staticmethod
     def MinVersion() -> Optional[str]:
```

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/PlayerSummary.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/PlayerSummary.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/PopulationSummary.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/PopulationSummary.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/SessionDiveSitesCount.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/SessionDiveSitesCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/SessionDuration.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/SessionDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/SessionGuideCount.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/SessionGuideCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/SessionHelpCount.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/SessionHelpCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/SessionID.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/SessionID.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/SessionJobsCompleted.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/SessionJobsCompleted.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/SwitchJobsCount.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/SwitchJobsCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/SyncCompletionTime.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/SyncCompletionTime.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         if event.EventName == "begin_simulation":
             self._sim_start_time = event.Timestamp
         elif event.EventName == "simulation_sync_achieved":
             if self._sim_start_time is not None:
                 self._time += (event.Timestamp - self._sim_start_time).total_seconds()
                 self._sim_start_time = None
             else:
-                Logger.Log("Simulation synced when we had no active start time!", logging.WARNING)
+                self.WarningMessage("Simulation synced when we had no active start time!")
 
         self._prev_timestamp = event.Timestamp
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
```

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/TankRulesCount.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/TankRulesCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/TopJobCompletionDestinations.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/TopJobCompletionDestinations.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,9 +78,9 @@
 
     # *** Other local functions
     def _validate_job(self, job_data):
         ret_val : bool = False
         if job_data and job_data in self._job_map:
                 ret_val = True
         else:
-            Logger.Log(f"Got invalid job_name data in JobsAttempted", logging.WARNING)
+            self.WarningMessage(f"Got invalid job_name data in JobsAttempted")
         return ret_val
```

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/TopJobSwitchDestinations.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/TopJobSwitchDestinations.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,9 +77,9 @@
 
     # *** Other local functions
     def _validate_job(self, job_data):
         ret_val : bool = False
         if job_data and job_data in self._job_map:
             ret_val = True
         else:
-            Logger.Log(f"Got invalid job_name data in JobsAttempted", logging.WARNING)
+            self.WarningMessage(f"Got invalid job_name data in JobsAttempted")
         return ret_val
```

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/TotalArgumentationTime.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/TotalArgumentationTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/TotalDiveTime.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/TotalDiveTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/TotalExperimentationTime.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/TotalExperimentationTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/UserAvgActiveTime.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/UserAvgActiveTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/UserAvgSessionDuration.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/UserAvgSessionDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/UserTotalSessionDuration.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/UserTotalSessionDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/features/__init__.py` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/__init__.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/AQUALAB/schemas/AQUALAB.json.template` & `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/schemas/AQUALAB.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/CRUSH_STATION/schemas/CRUSH_STATION.json.template` & `opengamedata_core-0.0.2/src/ogd/games/CRUSH_STATION/schemas/CRUSH_STATION.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/CRYSTAL/CrystalLoader.py` & `opengamedata_core-0.0.2/src/ogd/games/CRYSTAL/CrystalLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/CRYSTAL/features/CrystalExtractor.py` & `opengamedata_core-0.0.2/src/ogd/games/CRYSTAL/features/CrystalExtractor.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/CRYSTAL/schemas/CRYSTAL.json.template` & `opengamedata_core-0.0.2/src/ogd/games/CRYSTAL/schemas/CRYSTAL.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/GWAKKAMOLE/schemas/GWAKKAMOLE.json.template` & `opengamedata_core-0.0.2/src/ogd/games/GWAKKAMOLE/schemas/GWAKKAMOLE.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/ICECUBE/DBExport.json` & `opengamedata_core-0.0.2/src/ogd/games/ICECUBE/DBExport.json`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/ICECUBE/DBExport.py` & `opengamedata_core-0.0.2/src/ogd/games/ICECUBE/DBExport.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/ICECUBE/IcecubeLoader.py` & `opengamedata_core-0.0.2/src/ogd/games/ICECUBE/IcecubeLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/ICECUBE/features/HeadsetOnCount.py` & `opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/HeadsetOnCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/ICECUBE/features/ObjectSelectionsDuringVoiceover.py` & `opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/ObjectSelectionsDuringVoiceover.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/ICECUBE/features/PerSceneFeature.py` & `opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/PerSceneFeature.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/ICECUBE/features/SceneDuration.py` & `opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/SceneDuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,13 +67,13 @@
         scene_data = event.game_state.get("scene_name")
         # if scene_data in scenes_map and scenes_map[scene_data] == self.CountIndex:
         #         ret_val = True
         if scene_data is not None:
             if scene_data in scenes_map and scenes_map[scene_data] == self.CountIndex:
                 ret_val = True
         else:
-            Logger.Log(f"Got invalid scene data in {type(self).__name__}", logging.WARNING)
+            self.WarningMessage(f"Got invalid scene data in {type(self).__name__}")
 
         return ret_val
     @staticmethod
     def MinVersion() -> Optional[str]:
         return "2"
```

### Comparing `opengamedata-core-0.0.1/src/ogd/games/ICECUBE/features/SceneFailureCount.py` & `opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/SceneFailureCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/ICECUBE/features/SceneFailures.py` & `opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/SceneFailures.py`

 * *Files 7% similar despite different names*

```diff
@@ -68,13 +68,13 @@
             if scenes_map[scene_data] == self.CountIndex:
                 # Logger.Log(f"count index is {self.CountIndex}")
                 # Logger.Log(f"map index is {scenes_map[scene_data]}")
             # Logger.Log(f"scene_data is {scene_data}")
                 ret_val = True
         
         # else:
-        #     Logger.Log(f"Got invalid job_name data in {type(self).__name__}", logging.WARNING)
+        #     self.WarningMessage(f"Got invalid job_name data in {type(self).__name__}")
 
         return ret_val
     @staticmethod
     def MinVersion() -> Optional[str]:
         return "2"
```

### Comparing `opengamedata-core-0.0.1/src/ogd/games/ICECUBE/features/ScenesEncountered.py` & `opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/ScenesEncountered.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/ICECUBE/features/SessionDuration.py` & `opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/SessionDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/ICECUBE/features/Session_Language.py` & `opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/Session_Language.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/ICECUBE/features/TaskTimeToComplete.py` & `opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/TaskTimeToComplete.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/ICECUBE/features/ViewportCountPerScene.py` & `opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/ViewportCountPerScene.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/ICECUBE/features/__init__.py` & `opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/__init__.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/ICECUBE/schemas/ICECUBE.json.template` & `opengamedata_core-0.0.2/src/ogd/games/ICECUBE/schemas/ICECUBE.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/JournalismLoader.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/JournalismLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/AttributeView.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/AttributeView.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/ChoiceClickCount.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/ChoiceClickCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/ContinuesOnFail.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/ContinuesOnFail.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/EditorNoteOpen.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/EditorNoteOpen.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/FailureCount.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/FailureCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/GameComplete.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/GameComplete.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/LevelCompleteCount.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/LevelCompleteCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/LevelCompleted.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/LevelCompleted.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/LevelTime.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/LevelTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/MaxedPlayerAttribute.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/MaxedPlayerAttribute.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/MeanSnippetTime.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/MeanSnippetTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/PlayTime.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/PlayTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/PlayerAttributes.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/PlayerAttributes.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/QuitLevel.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/QuitLevel.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/QuitNode.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/QuitNode.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/QuitType.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/QuitType.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 # import libraries
 import json
-from typing import Any, List, Optional
+from typing import Any, Final, List, Optional
 import json
-from time import time
-from datetime  import timedelta, datetime
 # import local files
-from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.schemas.Event import Event
 from ogd.core.schemas.ExtractionMode import ExtractionMode
 from ogd.core.schemas.FeatureData import FeatureData
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 
 
@@ -52,15 +49,15 @@
         self._on_fail : bool = False
         self._on_checkpoint : bool = False
         self._other : bool = False
 
         
 
         #buffer for event margin before quit type is no longer considered something besides "other"
-        self._BUFFER_LIMIT: int = 9
+        self._BUFFER_LIMIT: Final[int] = 9
         #counters            
         self._event_counter : int = 0
     
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
```

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/QuitTypePerLevel.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/QuitTypePerLevel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 # import libraries
 import json
-from typing import Any, List, Optional
+from typing import Any, Final, List, Optional
 import json
-from time import time
-from datetime  import timedelta, datetime
 # import local files
-from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.schemas.Event import Event
 from ogd.core.schemas.ExtractionMode import ExtractionMode
 from ogd.core.schemas.FeatureData import FeatureData
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.generators.extractors.SessionFeature import SessionFeature
 
 
 """
 
 """
 
 
@@ -44,15 +40,15 @@
         self._on_fail : bool = False
         self._on_checkpoint : bool = False
         self._other : bool = False
 
         
 
         #buffer for event margin before quit type is no longer considered something besides "other"
-        self._BUFFER_LIMIT: int = 9
+        self._BUFFER_LIMIT: Final[int] = 9
         #counters            
         self._event_counter : int = 0
     
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
```

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/SessionPlayTime.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/SessionPlayTime.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # import libraries
 import json
-from typing import Any, List, Optional
+from typing import Any, Final, List, Optional
 import json
-from time import time
 from datetime  import timedelta, datetime
 # import local files
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.schemas.Event import Event
 from ogd.core.schemas.ExtractionMode import ExtractionMode
 from ogd.core.schemas.FeatureData import FeatureData
 from ogd.core.generators.Generator import GeneratorParameters
@@ -18,15 +17,15 @@
 
 class SessionPlayTime(SessionFeature):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
     :type Feature: _type_
     """
-    IDLE_TIME_THRESHOLD = timedelta(seconds=60)
+    IDLE_TIME_THRESHOLD : Final[timedelta] = timedelta(seconds=60)
 
     def __init__(self, params:GeneratorParameters, threshold: int):
         super().__init__(params=params)
         self._first_event_timestamp : Optional[datetime] = None
         self._last_event_timestamp : Optional[datetime] = None
 
         self._idle_time : Optional[timedelta] = None
```

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/SkillSequenceCount.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/SkillSequenceCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/SnippetReceivedCount.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/SnippetReceivedCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/SnippetReplace.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/SnippetReplace.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/SnippetsCollected.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/SnippetsCollected.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/SnippetsSubmitted.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/SnippetsSubmitted.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/StoryAlignment.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/StoryAlignment.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/StoryAlignmentSequence.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/StoryAlignmentSequence.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/StoryCompleteTime.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/StoryCompleteTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/StoryEditorTime.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/StoryEditorTime.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # import libraries
 import json
-from typing import Any, List, Optional
+from typing import Any, Final, List, Optional
 import json
-from time import time
 from datetime  import timedelta, datetime
 # import local files
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.schemas.Event import Event
 from ogd.core.schemas.ExtractionMode import ExtractionMode
 from ogd.core.schemas.FeatureData import FeatureData
@@ -19,15 +18,15 @@
 
 class StoryEditorTime(PerLevelFeature):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
     :type Feature: _type_
     """
-    IDLE_TIME_THRESHOLD = timedelta(seconds=60)
+    IDLE_TIME_THRESHOLD : Final[timedelta] = timedelta(seconds=60)
 
     def __init__(self, params:GeneratorParameters, threshold: int):
         super().__init__(params=params)
         PerLevelFeature.__init__(self, params=params)
 
 
         ##enable feature logic only when in the story editor
```

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/StoryScore.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/StoryScore.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/StoryScoreSequence.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/StoryScoreSequence.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/TextClickCount.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/TextClickCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/TopAttribute.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/TopAttribute.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/TopPlayerAttribute.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/TopPlayerAttribute.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/TopPlayerQuitType.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/TopPlayerQuitType.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/TotalFails.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/TotalFails.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/TotalLevelTime.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/TotalLevelTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/UserPlayTime.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/UserPlayTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/WorstAttribute.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/WorstAttribute.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/WorstPlayerAttribute.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/WorstPlayerAttribute.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/features/__init__.py` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/__init__.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOURNALISM/schemas/JOURNALISM.json.template` & `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/schemas/JOURNALISM.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOWILDER/JowilderLoader.py` & `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/JowilderLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOWILDER/Jowilder_Enumerators.py` & `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/Jowilder_Enumerators.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/ActiveStateTime.py` & `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/ActiveStateTime.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # import libraries
 import json
-from time import time
-from typing import Any, List, Optional
+from typing import Any, Final, List, Optional
 from datetime  import timedelta, datetime
 # import local files
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 from ogd.core.schemas.ExtractionMode import ExtractionMode
 from ogd.core.schemas.FeatureData import FeatureData
 from ogd.core.schemas.Event import Event
@@ -13,16 +12,16 @@
 class ActiveStateTime(SessionFeature):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
     :type Feature: _type_
     """
 
-    ACTIVE_TIME_THRESHOLD = timedelta(seconds=15)
-    CLICK_EVENTS_NAME = [f"CUSTOM.{i}" for i in range(3, 12)]
+    ACTIVE_TIME_THRESHOLD : Final[timedelta] = timedelta(seconds=15)
+    CLICK_EVENTS_NAME     : Final[List[str]] = [f"CUSTOM.{i}" for i in range(3, 12)]
 
     def __init__(self, params:GeneratorParameters, threshold:int):
         super().__init__(params=params)
         self._time : timedelta = timedelta(0)
         self._clicking_time : timedelta = timedelta(0)
         self._last_hover_or_click_timestamp : Optional[datetime] = None
         self._last_click_timestamp : Optional[datetime] = None
```

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/Clicks.py` & `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/Clicks.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/EventCount.py` & `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/EventCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/FirstInteraction.py` & `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/FirstInteraction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # import libraries
 import json
-from typing import Any, List, Optional
+from typing import Any, Final, List, Optional
 # import local files
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 from ogd.core.schemas.ExtractionMode import ExtractionMode
 from ogd.core.schemas.FeatureData import FeatureData
 from ogd.core.schemas.Event import Event
 
 class FirstInteraction(SessionFeature):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
     :type Feature: _type_
     """
-    NO_SENSE = 'tunic.historicalsociety.closet.intro'
+    NO_SENSE : Final[str] = 'tunic.historicalsociety.closet.intro'
 
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self._interaction : Optional[str] = None
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
```

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/GameScript.py` & `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/GameScript.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # import libraries
-from lib2to3.pgen2.token import OP
-from typing import Any, List, Optional
+from typing import Any, Dict, Final, List, Optional
 from ogd.core.generators.Generator import GeneratorParameters
 # import local files
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 from ogd.core.schemas.ExtractionMode import ExtractionMode
 from ogd.core.schemas.FeatureData import FeatureData
 from ogd.core.schemas.Event import Event
 
 class GameScript(SessionFeature):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
     :type Feature: _type_
     """
 
-    TYPE = {0: 'Dry', 1: 'No Humor', 2: 'No Snark', 3: 'Normal'}
+    TYPE : Final[Dict[int, str]] = {0: 'Dry', 1: 'No Humor', 2: 'No Snark', 3: 'Normal'}
 
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self._name : Optional[str] = None
         self._version : Optional[int] = None
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
```

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/GameVersion.py` & `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/GameVersion.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/Hovers.py` & `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/Hovers.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/IdleState.py` & `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/IdleState.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # import libraries
 import json
 from time import time
-from typing import Any, List, Optional
+from typing import Any, Final, List, Optional
 from datetime  import timedelta, datetime
 # import local files
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 from ogd.core.schemas.ExtractionMode import ExtractionMode
 from ogd.core.schemas.FeatureData import FeatureData
 from ogd.core.schemas.Event import Event
@@ -13,15 +13,15 @@
 class IdleState(SessionFeature):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
     :type Feature: _type_
     """
 
-    IDLE_TIME_THRESHOLD = timedelta(seconds=15)
+    IDLE_TIME_THRESHOLD : Final[timedelta] = timedelta(seconds=15)
 
     def __init__(self, params:GeneratorParameters, threshold:int):
         super().__init__(params=params)
         self._time : timedelta = timedelta(0)
         self._count : int = 0
         self._last_timestamp : Optional[datetime] = None
         self._threshold : timedelta = timedelta(seconds=threshold)
```

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/Interaction.py` & `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/Interaction.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/InteractionName.py` & `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/InteractionName.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/InteractionTextBoxesPerSecond.py` & `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/InteractionTextBoxesPerSecond.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/InteractionWordsPerSecond.py` & `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/InteractionWordsPerSecond.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/LastInteraction.py` & `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/LastInteraction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # import libraries
 import json
-from typing import Any, List, Optional
+from typing import Any, Final, List, Optional
 # import local files
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 from ogd.core.schemas.ExtractionMode import ExtractionMode
 from ogd.core.schemas.FeatureData import FeatureData
 from ogd.core.schemas.Event import Event
 
 class LastInteraction(SessionFeature):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
     :type Feature: _type_
     """
-    NO_SENSE = 'tunic.historicalsociety.closet.intro'
+    NO_SENSE : Final[str] = 'tunic.historicalsociety.closet.intro'
 
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self._interaction : Optional[str] = None
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
```

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/MeaningfulActions.py` & `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/MeaningfulActions.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/NotebookUses.py` & `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/NotebookUses.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/QuestionAnswers.py` & `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/QuestionAnswers.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/SessionDuration.py` & `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/SessionDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/SessionStart.py` & `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/SessionStart.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/SurveyItem.py` & `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/SurveyItem.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # import libraries
 import json
 import logging
 from datetime import datetime, timedelta
-from typing import Any, List, Optional
+from typing import Any, Dict, Final, List, Optional
 # import local files
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.PerCountFeature import PerCountFeature
 from ogd.core.schemas.ExtractionMode import ExtractionMode
 from ogd.core.schemas.FeatureData import FeatureData
 from ogd.core.schemas.Event import Event
 from ogd.core.utils.Logger import Logger
 
 # BUG: Question0 and quiz 0 don't have start time
 # NOTE: Assumptions are: Every quiz should have a quizstart.
 
-QUIZ_INDEXES = {
+QUIZ_INDEXES : Final[Dict[int, Dict[int, int]]] = {
     0: {0: 0, 1: 1},
     2: {0: 2, 1: 3, 2: 4, 3: 5},
     3: {0: 6, 1: 7, 2: 8, 3: 9},
     4: {0: 10, 1: 11, 2: 12, 3: 13},
     5: {0: 14, 1: 15, 2: 16, 3: 17}
 }
```

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/SurveyTime.py` & `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/SurveyTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/UsedContinue.py` & `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/UsedContinue.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # import libraries
-from typing import Any, List, Optional
+from typing import Any, Final, List, Optional
 from ogd.core.generators.Generator import GeneratorParameters
 # import local files
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 from ogd.core.schemas.ExtractionMode import ExtractionMode
 from ogd.core.schemas.FeatureData import FeatureData
 from ogd.core.schemas.Event import Event
 
 class UsedContinue(SessionFeature):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
     :type Feature: _type_
     """
 
-    START_SIGN = "tunic.historicalsociety.closet.gramps.intro_0_cs_0"
+    START_SIGN : Final[str] = "tunic.historicalsociety.closet.gramps.intro_0_cs_0"
 
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self._continue : int = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
```

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/UsedSaveCode.py` & `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/UsedSaveCode.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/UserEnabled.py` & `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/UserEnabled.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOWILDER/features/__init__.py` & `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/__init__.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOWILDER/get_jowilder_all_items.py` & `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/get_jowilder_all_items.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/JOWILDER/schemas/JOWILDER.json.template` & `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/schemas/JOWILDER.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/LAKELAND/LakelandLoader.py` & `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/LakelandLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/ActionsLastXSecondsModel.py` & `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/ActionsLastXSecondsModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/DeathCountModel.py` & `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/DeathCountModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/DeathPredModel.py` & `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/DeathPredModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/DeathThresholdModel.py` & `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/DeathThresholdModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/DiagonalFarmDetectorModel.py` & `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/DiagonalFarmDetectorModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/FeatSeqPercent.py` & `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/FeatSeqPercent.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/FeatVelocity.py` & `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/FeatVelocity.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/FeatureModel.py` & `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/FeatureModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/LAKELAND_models.json` & `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/LAKELAND_models.json`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/LakelandEnumerators.json` & `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/LakelandEnumerators.json`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/LakelandExtractor.py` & `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/LakelandExtractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -945,15 +945,15 @@
         emote_str = LakelandExtractor._ENUM_TO_STR['EMOTES'][_emote_enum]
         affect = LakelandExtractor._EMOTE_STR_TO_AFFECT[emote_str]
         self.feature_time_since_start(f"time_to_first_{emote_str.replace('_txt','')}_emote")
         is_positive = affect == 1
         is_neutral = affect == 0
         is_negative = affect == -1
         if(self._num_farmbits) < 1:
-            # Logger.Log(f"Num farmbits < 1 @ {self._num_farmbits}!! Setting to 1.", logging.WARNING)
+            # self.WarningMessage(f"Num farmbits < 1 @ {self._num_farmbits}!! Setting to 1.")
             self.log_warning(f"Num farmbits < 1 @ {self._num_farmbits}!! Setting to 1.")
             self._num_farmbits = 1
 
         per_capita_val = 1/self._num_farmbits
 
         # set features
         self.feature_inc(f"count_{emote_str}_emotes_per_capita", per_capita_val)
```

### Comparing `opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/LinearModel.py` & `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/LinearModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/LogisticModel.py` & `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/LogisticModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/MapSummaryModel.py` & `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/MapSummaryModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/Model.py` & `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/Model.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/MoneyAccumulationModel.py` & `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/MoneyAccumulationModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/PopulationModel.py` & `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/PopulationModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/RecentPurchasesModel.py` & `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/RecentPurchasesModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/SequenceModel.py` & `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/SequenceModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/SimpleFarmAbandonmentModel.py` & `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/SimpleFarmAbandonmentModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/SingleFeatureModel.py` & `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/SingleFeatureModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/TimeSinceEventTypes.py` & `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/TimeSinceEventTypes.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/TimeSinceLastSaleModel.py` & `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/TimeSinceLastSaleModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/TownCompositionModel.py` & `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/TownCompositionModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/TutorialProgressionModel.py` & `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/TutorialProgressionModel.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,9 @@
 from typing import List
-import abc
-import typing
-import logging
-from abc import ABC
 from statistics import median
-import pandas as pd
-import numpy as np
-import json
 from datetime import datetime as dt
 ## import local libraries
 from models.FeatureModel import FeatureModel
 
 ## @class TutorialProgressionModel
 # Returns dictionary of time of first pivotal tutorial events in the game
 # @param levels: Levels applicable for model, tut_features: tutorial features
```

### Comparing `opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/WAVES_models.json` & `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/WAVES_models.json`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/WAVES_models_L8_Q0_Q1.json` & `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/WAVES_models_L8_Q0_Q1.json`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/WAVES_models_L8_and_Q0.json` & `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/WAVES_models_L8_and_Q0.json`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/WAVES_models_L8_complete_and_current.json` & `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/WAVES_models_L8_complete_and_current.json`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/LAKELAND/features/WAVES_models_L8_only_complete.json` & `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/WAVES_models_L8_only_complete.json`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/LAKELAND/produce_lakeland_enumerators.py` & `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/produce_lakeland_enumerators.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/LAKELAND/schemas/LAKELAND.json.template` & `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/schemas/LAKELAND.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/MAGNET/MagnetLoader.py` & `opengamedata_core-0.0.2/src/ogd/games/MAGNET/MagnetLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/MAGNET/features/MagnetExtractor.py` & `opengamedata_core-0.0.2/src/ogd/games/MAGNET/features/MagnetExtractor.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/MAGNET/schemas/MAGNET.json.template` & `opengamedata_core-0.0.2/src/ogd/games/MAGNET/schemas/MAGNET.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/MASHOPOLIS/schemas/MASHOPOLIS.json.template` & `opengamedata_core-0.0.2/src/ogd/games/MASHOPOLIS/schemas/MASHOPOLIS.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/PENGUINS/DBExport.json` & `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/DBExport.json`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/PENGUINS/PenguinsLoader.py` & `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/PenguinsLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/PENGUINS/detectors/RegionEnter.py` & `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/detectors/RegionEnter.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/PENGUINS/detectors/RegionExit.py` & `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/detectors/RegionExit.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/ActivityCompleted.py` & `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/ActivityCompleted.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/ActivityDuration.py` & `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/ActivityDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/EatFishCount.py` & `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/EatFishCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/EggLostCount.py` & `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/EggLostCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/EggRecoverTime.py` & `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/EggRecoverTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/GazeCount.py` & `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/GazeCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/GazeDuration.py` & `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/GazeDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/MirrorWaddleDuration.py` & `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/MirrorWaddleDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/PerRegionFeature.py` & `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/PerRegionFeature.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,22 +32,22 @@
             current_position['x'] < target_region['maxX'] and
             current_position['y'] > target_region['minY'] and
             current_position['y'] < target_region['maxY'] and
             current_position['z'] > target_region['minZ'] and
             current_position['z'] < target_region['maxZ']):
             ret_val = True
         # else:
-        #     Logger.Log(f"Got invalid region_name data in {type(self).__name__}", logging.WARNING)
+        #     self.WarningMessage(f"Got invalid region_name data in {type(self).__name__}")
         return ret_val
 
         #if region_data is not None:
             #if region_data in self.region_map and self.region_map[region_data] == self.CountIndex:
                 #ret_val = True
         #else:
-            #Logger.Log(f"Got invalid region_name data in {type(self).__name__}", logging.WARNING)
+            #self.WarningMessage(f"Got invalid region_name data in {type(self).__name__}")
         #return ret_val
 
     # *** Optionally override public functions. ***
 
     @staticmethod
     def MinVersion() -> Optional[str]:
         return "1"
```

### Comparing `opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/PickupRockCount.py` & `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/PickupRockCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/PlayerInactiveAvgDuration.py` & `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/PlayerInactiveAvgDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/PlayerWaddleCount.py` & `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/PlayerWaddleCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/RegionDuration.py` & `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/RegionDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/RegionEnterCount.py` & `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/RegionEnterCount.py`

 * *Files 15% similar despite different names*

```diff
@@ -41,10 +41,10 @@
     def _validateEventCountIndex(self, event: Event):
         ret_val : bool = False
         region_data = event.EventData.get("region_name")
         if region_data is not None:
             if region_data in region_map and region_map[region_data] == self.CountIndex:
                 ret_val = True
         else:
-            Logger.Log(f"Got invalid region data in {type(self).__name__}", logging.WARNING)
+            self.WarningMessage(f"Got invalid region data in {type(self).__name__}")
 
         return ret_val
```

### Comparing `opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/RegionsEncountered.py` & `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/RegionsEncountered.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/RingChimesCount.py` & `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/RingChimesCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/SessionDuration.py` & `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/SessionDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/SnowBallDuration.py` & `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/SnowBallDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/WaddlePerRegion.py` & `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/WaddlePerRegion.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/PENGUINS/features/__init__.py` & `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/__init__.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/PENGUINS/schemas/PENGUINS.json.template` & `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/schemas/PENGUINS.json.template`

 * *Files 2% similar despite different names*

```diff
@@ -13,1498 +13,1495 @@
 000000c0: 6f6e 6473 206f 6620 6761 6d65 2074 696d  onds of game tim
 000000d0: 6520 656c 6170 7365 6420 7369 6e63 6520  e elapsed since 
 000000e0: 7468 6520 6761 6d65 2077 6173 206c 6175  the game was lau
 000000f0: 6e63 6865 642c 202a 6e6f 7420 696e 636c  nched, *not incl
 00000100: 7564 696e 6720 7469 6d65 2077 6865 6e20  uding time when 
 00000110: 7468 6520 6761 6d65 2077 6173 2070 6175  the game was pau
 00000120: 7365 642a 2e22 0a20 2020 2020 2020 207d  sed*.".        }
-00000130: 2c0a 2020 2020 2020 2020 2270 6f73 5822  ,.        "posX"
-00000140: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-00000150: 2274 7970 6522 3a20 2266 6c6f 6174 222c  "type": "float",
-00000160: 0a20 2020 2020 2020 2020 2020 2022 6465  .            "de
-00000170: 7363 7269 7074 696f 6e22 3a20 2254 6865  scription": "The
-00000180: 2063 7572 7265 6e74 2078 2d70 6f73 6974   current x-posit
-00000190: 696f 6e20 6f66 205f 5f5f 5f5f 5f20 6174  ion of ______ at
-000001a0: 2074 6865 206d 6f6d 656e 7420 7468 6520   the moment the 
-000001b0: 6576 656e 7420 6f63 6375 7272 6564 2e22  event occurred."
-000001c0: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
-000001d0: 2020 2020 2270 6f73 5922 3a20 7b0a 2020      "posY": {.  
-000001e0: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
-000001f0: 3a20 2266 6c6f 6174 222c 0a20 2020 2020  : "float",.     
-00000200: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
-00000210: 696f 6e22 3a20 2254 6865 2063 7572 7265  ion": "The curre
-00000220: 6e74 2079 2d70 6f73 6974 696f 6e20 6f66  nt y-position of
-00000230: 205f 5f5f 5f5f 5f20 6174 2074 6865 206d   ______ at the m
-00000240: 6f6d 656e 7420 7468 6520 6576 656e 7420  oment the event 
-00000250: 6f63 6375 7272 6564 2e22 0a20 2020 2020  occurred.".     
-00000260: 2020 207d 2c0a 2020 2020 2020 2020 2270     },.        "p
-00000270: 6f73 5a22 3a20 7b0a 2020 2020 2020 2020  osZ": {.        
-00000280: 2020 2020 2274 7970 6522 3a20 2266 6c6f      "type": "flo
-00000290: 6174 222c 0a20 2020 2020 2020 2020 2020  at",.           
-000002a0: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
-000002b0: 2254 6865 2063 7572 7265 6e74 207a 2d70  "The current z-p
-000002c0: 6f73 6974 696f 6e20 6f66 205f 5f5f 5f5f  osition of _____
-000002d0: 5f20 6174 2074 6865 206d 6f6d 656e 7420  _ at the moment 
-000002e0: 7468 6520 6576 656e 7420 6f63 6375 7272  the event occurr
-000002f0: 6564 2e22 0a20 2020 2020 2020 207d 2c0a  ed.".        },.
-00000300: 2020 2020 2020 2020 2272 6f74 5822 3a20          "rotX": 
-00000310: 7b0a 2020 2020 2020 2020 2020 2020 2274  {.            "t
-00000320: 7970 6522 3a20 2266 6c6f 6174 222c 0a20  ype": "float",. 
-00000330: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
-00000340: 7269 7074 696f 6e22 3a20 2254 6865 2078  ription": "The x
-00000350: 2d63 6f6d 706f 6e65 6e74 206f 6620 7468  -component of th
-00000360: 6520 6f72 6965 6e74 6174 696f 6e20 6f66  e orientation of
-00000370: 205f 5f5f 5f5f 5f20 6174 2074 6865 206d   ______ at the m
-00000380: 6f6d 656e 7420 7468 6520 6576 656e 7420  oment the event 
-00000390: 6f63 6375 7272 6564 2e22 0a20 2020 2020  occurred.".     
-000003a0: 2020 207d 2c0a 2020 2020 2020 2020 2272     },.        "r
-000003b0: 6f74 5922 3a20 7b0a 2020 2020 2020 2020  otY": {.        
-000003c0: 2020 2020 2274 7970 6522 3a20 2266 6c6f      "type": "flo
-000003d0: 6174 222c 0a20 2020 2020 2020 2020 2020  at",.           
-000003e0: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
-000003f0: 2254 6865 2079 2d63 6f6d 706f 6e65 6e74  "The y-component
-00000400: 206f 6620 7468 6520 6f72 6965 6e74 6174   of the orientat
-00000410: 696f 6e20 6f66 205f 5f5f 5f5f 5f20 6174  ion of ______ at
-00000420: 2074 6865 206d 6f6d 656e 7420 7468 6520   the moment the 
-00000430: 6576 656e 7420 6f63 6375 7272 6564 2e22  event occurred."
-00000440: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
-00000450: 2020 2020 2272 6f74 5a22 3a20 7b0a 2020      "rotZ": {.  
-00000460: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
-00000470: 3a20 2266 6c6f 6174 222c 0a20 2020 2020  : "float",.     
-00000480: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
-00000490: 696f 6e22 3a20 2254 6865 207a 2d63 6f6d  ion": "The z-com
-000004a0: 706f 6e65 6e74 206f 6620 7468 6520 6f72  ponent of the or
-000004b0: 6965 6e74 6174 696f 6e20 6f66 205f 5f5f  ientation of ___
-000004c0: 5f5f 5f20 6174 2074 6865 206d 6f6d 656e  ___ at the momen
-000004d0: 7420 7468 6520 6576 656e 7420 6f63 6375  t the event occu
-000004e0: 7272 6564 2e22 0a20 2020 2020 2020 207d  rred.".        }
-000004f0: 2c0a 2020 2020 2020 2020 2272 6f74 5722  ,.        "rotW"
-00000500: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-00000510: 2274 7970 6522 3a20 2266 6c6f 6174 222c  "type": "float",
-00000520: 0a20 2020 2020 2020 2020 2020 2022 6465  .            "de
-00000530: 7363 7269 7074 696f 6e22 3a20 2254 6865  scription": "The
-00000540: 2077 2d63 6f6d 706f 6e65 6e74 206f 6620   w-component of 
-00000550: 7468 6520 6f72 6965 6e74 6174 696f 6e20  the orientation 
-00000560: 6f66 205f 5f5f 5f5f 5f20 6174 2074 6865  of ______ at the
-00000570: 206d 6f6d 656e 7420 7468 6520 6576 656e   moment the even
-00000580: 7420 6f63 6375 7272 6564 2e22 0a20 2020  t occurred.".   
-00000590: 2020 2020 207d 0a20 2020 207d 2c0a 2020       }.    },.  
-000005a0: 2020 2265 7665 6e74 7322 3a20 7b0a 2020    "events": {.  
-000005b0: 2020 2020 2020 2273 6573 7369 6f6e 5f73        "session_s
-000005c0: 7461 7274 223a 207b 0a20 2020 2020 2020  tart": {.       
-000005d0: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
-000005e0: 6e22 3a20 2257 6865 6e20 7468 6520 6170  n": "When the ap
-000005f0: 7020 6973 2073 7461 7274 6564 2061 6e64  p is started and
-00000600: 2074 6865 2067 616d 6570 6c61 7920 7365   the gameplay se
-00000610: 7373 696f 6e20 6973 2061 7373 6967 6e65  ssion is assigne
-00000620: 6420 6120 7365 7373 696f 6e20 4944 2e20  d a session ID. 
-00000630: 5468 6520 706c 6179 6572 2068 6173 206e  The player has n
-00000640: 6f74 206e 6563 6573 7361 7269 6c79 2062  ot necessarily b
-00000650: 6567 756e 2074 6865 2067 616d 6520 6974  egun the game it
-00000660: 7365 6c66 2079 6574 2e22 2c0a 2020 2020  self yet.",.    
-00000670: 2020 2020 2020 2020 2265 7665 6e74 5f64          "event_d
-00000680: 6174 6122 3a20 7b0a 2020 2020 2020 2020  ata": {.        
-00000690: 2020 2020 2020 2020 2272 616e 646f 6d5f          "random_
-000006a0: 7365 6564 223a 2022 5468 6520 7261 6e64  seed": "The rand
-000006b0: 6f6d 2073 6565 6420 7573 6564 2066 6f72  om seed used for
-000006c0: 2061 6c6c 2072 616e 646f 6d20 6e75 6d62   all random numb
-000006d0: 6572 2f70 6f73 6974 696f 6e2f 726f 7461  er/position/rota
-000006e0: 7469 6f6e 2067 656e 6572 6174 696f 6e20  tion generation 
-000006f0: 696e 2074 6865 2067 616d 652e 220a 2020  in the game.".  
-00000700: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-00000710: 2020 2020 7d2c 0a20 2020 2020 2020 2022      },.        "
-00000720: 6761 6d65 5f73 7461 7274 223a 207b 0a20  game_start": {. 
-00000730: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
-00000740: 7269 7074 696f 6e22 3a20 2257 6865 6e20  ription": "When 
-00000750: 6120 6e65 7720 6761 6d65 2069 7320 7374  a new game is st
-00000760: 6172 7465 6422 2c0a 2020 2020 2020 2020  arted",.        
-00000770: 2020 2020 2265 7665 6e74 5f64 6174 6122      "event_data"
-00000780: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-00000790: 2020 2020 226d 6f64 6522 3a20 7b0a 2020      "mode": {.  
-000007a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000007b0: 2020 2274 7970 6522 3a20 2265 6e75 6d28    "type": "enum(
-000007c0: 484f 4d45 5f4d 4f44 452c 202e 2e2e 2922  HOME_MODE, ...)"
-000007d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000007e0: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
-000007f0: 6f6e 223a 2022 5468 6520 6761 6d65 206d  on": "The game m
-00000800: 6f64 6520 7468 6174 2074 6865 2070 6c61  ode that the pla
-00000810: 7965 7220 6c61 756e 6368 6564 220a 2020  yer launched".  
-00000820: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
-00000830: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-00000840: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00000850: 2022 6f70 656e 5f6d 656e 7522 3a20 7b0a   "open_menu": {.
-00000860: 2020 2020 2020 2020 2020 2020 2264 6573              "des
-00000870: 6372 6970 7469 6f6e 223a 2022 5768 656e  cription": "When
-00000880: 2074 6865 2070 6c61 7965 7220 6f70 656e   the player open
-00000890: 7320 7468 6520 6761 6d65 206d 656e 7522  s the game menu"
-000008a0: 2c0a 2020 2020 2020 2020 2020 2020 2265  ,.            "e
-000008b0: 7665 6e74 5f64 6174 6122 3a20 7b7d 0a20  vent_data": {}. 
-000008c0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-000008d0: 2020 2263 6c6f 7365 5f6d 656e 7522 3a20    "close_menu": 
-000008e0: 7b0a 2020 2020 2020 2020 2020 2020 2264  {.            "d
-000008f0: 6573 6372 6970 7469 6f6e 223a 2022 5768  escription": "Wh
-00000900: 656e 2074 6865 2070 6c61 7965 7220 636c  en the player cl
-00000910: 6f73 6573 2074 6865 2067 616d 6520 6d65  oses the game me
-00000920: 6e75 222c 0a20 2020 2020 2020 2020 2020  nu",.           
-00000930: 2022 6576 656e 745f 6461 7461 223a 207b   "event_data": {
-00000940: 7d0a 2020 2020 2020 2020 7d2c 0a20 2020  }.        },.   
-00000950: 2020 2020 2022 7365 6c65 6374 5f6d 656e       "select_men
-00000960: 755f 6974 656d 223a 207b 0a20 2020 2020  u_item": {.     
-00000970: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
-00000980: 696f 6e22 3a20 2257 6865 6e20 7468 6520  ion": "When the 
-00000990: 706c 6179 6572 2063 6c69 636b 7320 616e  player clicks an
-000009a0: 6420 6974 656d 2069 6e20 7468 6520 6d65  d item in the me
-000009b0: 6e75 222c 0a20 2020 2020 2020 2020 2020  nu",.           
-000009c0: 2022 6576 656e 745f 6461 7461 223a 207b   "event_data": {
-000009d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000009e0: 2022 6974 656d 223a 207b 0a20 2020 2020   "item": {.     
-000009f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000a00: 7479 7065 223a 2022 7374 7222 2c0a 2020  type": "str",.  
-00000a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a20: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-00000a30: 2022 5468 6520 6e61 6d65 206f 6620 7468   "The name of th
-00000a40: 6520 6d65 6e75 2069 7465 6d20 7468 6520  e menu item the 
-00000a50: 706c 6179 6572 2073 656c 6563 7465 6422  player selected"
-00000a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000a70: 207d 0a20 2020 2020 2020 2020 2020 207d   }.            }
-00000a80: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
-00000a90: 2020 2020 2268 6561 6473 6574 5f6f 6e22      "headset_on"
-00000aa0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-00000ab0: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
-00000ac0: 5768 656e 2074 6865 2070 6c61 7965 7220  When the player 
-00000ad0: 7075 7473 2074 6865 2068 6561 6473 6574  puts the headset
-00000ae0: 206f 6e2c 2072 6573 756d 696e 6720 7468   on, resuming th
-00000af0: 6520 6761 6d65 222c 0a20 2020 2020 2020  e game",.       
-00000b00: 2020 2020 2022 6576 656e 745f 6461 7461       "event_data
-00000b10: 223a 207b 7d0a 2020 2020 2020 2020 7d2c  ": {}.        },
-00000b20: 0a20 2020 2020 2020 2022 6865 6164 7365  .        "headse
-00000b30: 745f 6f66 6622 3a20 7b0a 2020 2020 2020  t_off": {.      
-00000b40: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
-00000b50: 6f6e 223a 2022 5768 656e 2074 6865 2070  on": "When the p
-00000b60: 6c61 7965 7220 7265 6d6f 7665 7320 7468  layer removes th
-00000b70: 6520 6865 6164 7365 7420 6672 6f6d 2074  e headset from t
-00000b80: 6865 6972 2068 6561 642c 2070 6175 7369  heir head, pausi
-00000b90: 6e67 2074 6865 2067 616d 6522 2c0a 2020  ng the game",.  
-00000ba0: 2020 2020 2020 2020 2020 2265 7665 6e74            "event
-00000bb0: 5f64 6174 6122 3a20 7b7d 0a20 2020 2020  _data": {}.     
-00000bc0: 2020 207d 2c0a 2020 2020 2020 2020 2276     },.        "v
-00000bd0: 6965 7770 6f72 745f 6461 7461 223a 207b  iewport_data": {
-00000be0: 0a20 2020 2020 2020 2020 2020 2022 6465  .            "de
-00000bf0: 7363 7269 7074 696f 6e22 3a20 2241 6e20  scription": "An 
-00000c00: 6576 656e 7420 7365 6e74 2061 7070 726f  event sent appro
-00000c10: 7869 6d61 7465 6c79 206f 6e63 6520 7065  ximately once pe
-00000c20: 7220 7365 636f 6e64 2c20 636f 6e74 6169  r second, contai
-00000c30: 6e69 6e67 2074 6865 2069 6e2d 6761 6d65  ning the in-game
-00000c40: 2070 6f73 6974 696f 6e20 616e 6420 6f72   position and or
-00000c50: 6965 6e74 6174 696f 6e20 6f66 2074 6865  ientation of the
-00000c60: 2070 6c61 7965 7220 6865 6164 7365 7420   player headset 
-00000c70: 666f 7220 6561 6368 2066 7261 6d65 2069  for each frame i
-00000c80: 6e20 7468 6520 7061 7374 2073 6563 6f6e  n the past secon
-00000c90: 6422 2c0a 2020 2020 2020 2020 2020 2020  d",.            
-00000ca0: 2265 7665 6e74 5f64 6174 6122 3a20 7b0a  "event_data": {.
-00000cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000cc0: 2267 617a 655f 6461 7461 5f70 6163 6b61  "gaze_data_packa
-00000cd0: 6765 223a 207b 0a20 2020 2020 2020 2020  ge": {.         
-00000ce0: 2020 2020 2020 2020 2020 2022 7479 7065             "type
-00000cf0: 223a 2022 4c69 7374 5b44 6963 745d 222c  ": "List[Dict]",
-00000d00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000d10: 2020 2020 2022 6465 7461 696c 7322 3a20       "details": 
-00000d20: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00000d30: 2020 2020 2020 2020 2020 2270 6f73 223a            "pos":
-00000d40: 2022 4c69 7374 5b66 6c6f 6174 5d22 2c0a   "List[float]",.
-00000d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d60: 2020 2020 2020 2020 2272 6f74 223a 2022          "rot": "
-00000d70: 4c69 7374 5b66 6c6f 6174 5d22 0a20 2020  List[float]".   
-00000d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d90: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
-00000da0: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
-00000db0: 7469 6f6e 223a 2022 4120 6c69 7374 206f  tion": "A list o
-00000dc0: 6620 6469 6374 732c 2077 6865 7265 2065  f dicts, where e
-00000dd0: 6163 6820 6469 6374 2069 7320 6f6e 6520  ach dict is one 
-00000de0: 6672 616d 6520 6f66 2068 6561 6473 6574  frame of headset
-00000df0: 2064 6174 612c 2063 6f6e 7461 696e 696e   data, containin
-00000e00: 6720 6120 706f 7369 7469 6f6e 2061 6e64  g a position and
-00000e10: 2072 6f74 6174 696f 6e20 7665 6374 6f72   rotation vector
-00000e20: 2c20 652e 672e 207b 5c22 706f 735c 223a  , e.g. {\"pos\":
-00000e30: 5b31 2c32 2c33 5d2c 205c 2272 6f74 5c22  [1,2,3], \"rot\"
-00000e40: 3a5b 342c 352c 362c 375d 7d2e 220a 2020  :[4,5,6,7]}.".  
-00000e50: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
-00000e60: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-00000e70: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00000e80: 2022 6c65 6674 5f68 616e 645f 6461 7461   "left_hand_data
-00000e90: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-00000ea0: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
-00000eb0: 2241 6e20 6576 656e 7420 7365 6e74 2061  "An event sent a
-00000ec0: 7070 726f 7869 6d61 7465 6c79 206f 6e63  pproximately onc
-00000ed0: 6520 7065 7220 7365 636f 6e64 2c20 636f  e per second, co
-00000ee0: 6e74 6169 6e69 6e67 2074 6865 2069 6e2d  ntaining the in-
-00000ef0: 6761 6d65 2070 6f73 6974 696f 6e20 616e  game position an
-00000f00: 6420 6f72 6965 6e74 6174 696f 6e20 6f66  d orientation of
-00000f10: 2074 6865 2070 6c61 7965 7227 7320 6c65   the player's le
-00000f20: 6674 2068 616e 6420 666f 7220 6561 6368  ft hand for each
-00000f30: 2066 7261 6d65 2069 6e20 7468 6520 7061   frame in the pa
-00000f40: 7374 2073 6563 6f6e 6422 2c0a 2020 2020  st second",.    
-00000f50: 2020 2020 2020 2020 2265 7665 6e74 5f64          "event_d
-00000f60: 6174 6122 3a20 7b0a 2020 2020 2020 2020  ata": {.        
-00000f70: 2020 2020 2020 2020 226c 6566 745f 6861          "left_ha
-00000f80: 6e64 5f64 6174 615f 7061 636b 6167 6522  nd_data_package"
-00000f90: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-00000fa0: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
-00000fb0: 224c 6973 745b 4469 6374 5d22 2c0a 2020  "List[Dict]",.  
-00000fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fd0: 2020 2264 6574 6169 6c73 223a 207b 0a20    "details": {. 
-00000fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ff0: 2020 2020 2020 2022 706f 7322 3a20 224c         "pos": "L
-00001000: 6973 745b 666c 6f61 745d 222c 0a20 2020  ist[float]",.   
-00001010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001020: 2020 2020 2022 726f 7422 3a20 224c 6973       "rot": "Lis
-00001030: 745b 666c 6f61 745d 220a 2020 2020 2020  t[float]".      
-00001040: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
-00001050: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001060: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
-00001070: 6e22 3a20 2241 206c 6973 7420 6f66 2064  n": "A list of d
-00001080: 6963 7473 2c20 7768 6572 6520 6561 6368  icts, where each
-00001090: 2064 6963 7420 6973 206f 6e65 2066 7261   dict is one fra
-000010a0: 6d65 206f 6620 6c65 6674 2d68 616e 6420  me of left-hand 
-000010b0: 6461 7461 2c20 636f 6e74 6169 6e69 6e67  data, containing
-000010c0: 2061 2070 6f73 6974 696f 6e20 616e 6420   a position and 
-000010d0: 726f 7461 7469 6f6e 2076 6563 746f 722c  rotation vector,
-000010e0: 2065 2e67 2e20 7b5c 2270 6f73 5c22 3a5b   e.g. {\"pos\":[
-000010f0: 312c 322c 335d 2c20 5c22 726f 745c 223a  1,2,3], \"rot\":
-00001100: 5b34 2c35 2c36 2c37 5d7d 2e22 0a20 2020  [4,5,6,7]}.".   
-00001110: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
-00001120: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-00001130: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-00001140: 2272 6967 6874 5f68 616e 645f 6461 7461  "right_hand_data
-00001150: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-00001160: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
-00001170: 2241 6e20 6576 656e 7420 7365 6e74 2061  "An event sent a
-00001180: 7070 726f 7869 6d61 7465 6c79 206f 6e63  pproximately onc
-00001190: 6520 7065 7220 7365 636f 6e64 2c20 636f  e per second, co
-000011a0: 6e74 6169 6e69 6e67 2074 6865 2069 6e2d  ntaining the in-
-000011b0: 6761 6d65 2070 6f73 6974 696f 6e20 616e  game position an
-000011c0: 6420 6f72 6965 6e74 6174 696f 6e20 6f66  d orientation of
-000011d0: 2074 6865 2070 6c61 7965 7227 7320 7269   the player's ri
-000011e0: 6768 7420 6861 6e64 2066 6f72 2065 6163  ght hand for eac
-000011f0: 6820 6672 616d 6520 696e 2074 6865 2070  h frame in the p
-00001200: 6173 7420 7365 636f 6e64 222c 0a20 2020  ast second",.   
-00001210: 2020 2020 2020 2020 2022 6576 656e 745f           "event_
-00001220: 6461 7461 223a 207b 0a20 2020 2020 2020  data": {.       
-00001230: 2020 2020 2020 2020 2022 7269 6768 745f           "right_
-00001240: 6861 6e64 5f64 6174 615f 7061 636b 6167  hand_data_packag
-00001250: 6522 3a20 7b0a 2020 2020 2020 2020 2020  e": {.          
-00001260: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
-00001270: 3a20 224c 6973 745b 4469 6374 5d22 2c0a  : "List[Dict]",.
-00001280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001290: 2020 2020 2264 6574 6169 6c73 223a 207b      "details": {
-000012a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000012b0: 2020 2020 2020 2020 2022 706f 7322 3a20           "pos": 
-000012c0: 224c 6973 745b 666c 6f61 745d 222c 0a20  "List[float]",. 
-000012d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012e0: 2020 2020 2020 2022 726f 7422 3a20 224c         "rot": "L
-000012f0: 6973 745b 666c 6f61 745d 220a 2020 2020  ist[float]".    
-00001300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001310: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
-00001320: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
-00001330: 696f 6e22 3a20 2241 206c 6973 7420 6f66  ion": "A list of
-00001340: 2064 6963 7473 2c20 7768 6572 6520 6561   dicts, where ea
-00001350: 6368 2064 6963 7420 6973 206f 6e65 2066  ch dict is one f
-00001360: 7261 6d65 206f 6620 7269 6768 742d 6861  rame of right-ha
-00001370: 6e64 2064 6174 612c 2063 6f6e 7461 696e  nd data, contain
-00001380: 696e 6720 6120 706f 7369 7469 6f6e 2061  ing a position a
-00001390: 6e64 2072 6f74 6174 696f 6e20 7665 6374  nd rotation vect
-000013a0: 6f72 2c20 652e 672e 207b 5c22 706f 735c  or, e.g. {\"pos\
-000013b0: 223a 5b31 2c32 2c33 5d2c 205c 2272 6f74  ":[1,2,3], \"rot
-000013c0: 5c22 3a5b 342c 352c 362c 375d 7d2e 220a  \":[4,5,6,7]}.".
-000013d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000013e0: 7d0a 2020 2020 2020 2020 2020 2020 7d0a  }.            }.
-000013f0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00001400: 2020 2022 706c 6179 6572 5f77 6164 646c     "player_waddl
-00001410: 6522 3a20 7b0a 2020 2020 2020 2020 2020  e": {.          
-00001420: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-00001430: 2022 5768 656e 2061 2070 6c61 7965 7220   "When a player 
-00001440: 7065 7266 6f72 6d73 2061 2077 6164 646c  performs a waddl
-00001450: 6520 6d6f 7665 6d65 6e74 2074 6f20 6d6f  e movement to mo
-00001460: 7665 2074 6865 6972 2070 656e 6775 696e  ve their penguin
-00001470: 2061 7661 7461 7220 666f 7277 6172 6422   avatar forward"
-00001480: 2c0a 2020 2020 2020 2020 2020 2020 2265  ,.            "e
-00001490: 7665 6e74 5f64 6174 6122 3a20 7b0a 2020  vent_data": {.  
-000014a0: 2020 2020 2020 2020 2020 2020 2020 226f                "o
-000014b0: 626a 6563 745f 6964 223a 207b 0a20 2020  bject_id": {.   
-000014c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000014d0: 2022 7479 7065 223a 2022 7374 7222 2c0a   "type": "str",.
-000014e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000014f0: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
-00001500: 223a 2022 5468 6520 6e61 6d65 206f 662e  ": "The name of.
-00001510: 2e2e 2073 6f6d 6520 6f62 6a65 6374 220a  .. some object".
-00001520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001530: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
-00001540: 2020 2022 6f6c 645f 706f 7358 223a 207b     "old_posX": {
-00001550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001560: 2020 2020 2022 7479 7065 223a 2022 666c       "type": "fl
-00001570: 6f61 7422 2c0a 2020 2020 2020 2020 2020  oat",.          
-00001580: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
-00001590: 6970 7469 6f6e 223a 2022 5468 6520 7072  iption": "The pr
-000015a0: 6576 696f 7573 2058 2d70 6f73 6974 696f  evious X-positio
-000015b0: 6e2c 2077 6865 7265 2074 6865 2077 6164  n, where the wad
-000015c0: 646c 6520 7374 6172 7465 642e 220a 2020  dle started.".  
-000015d0: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
-000015e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000015f0: 2022 6f6c 645f 706f 7359 223a 207b 0a20   "old_posY": {. 
-00001600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001610: 2020 2022 7479 7065 223a 2022 666c 6f61     "type": "floa
-00001620: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
-00001630: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
-00001640: 7469 6f6e 223a 2022 5468 6520 7072 6576  tion": "The prev
-00001650: 696f 7573 2059 2d70 6f73 6974 696f 6e2c  ious Y-position,
-00001660: 2077 6865 7265 2074 6865 2077 6164 646c   where the waddl
-00001670: 6520 7374 6172 7465 642e 220a 2020 2020  e started.".    
-00001680: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
-00001690: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000016a0: 6f6c 645f 706f 735a 223a 207b 0a20 2020  old_posZ": {.   
-000016b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016c0: 2022 7479 7065 223a 2022 666c 6f61 7422   "type": "float"
-000016d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000016e0: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
-000016f0: 6f6e 223a 2022 5468 6520 7072 6576 696f  on": "The previo
-00001700: 7573 205a 2d70 6f73 6974 696f 6e2c 2077  us Z-position, w
-00001710: 6865 7265 2074 6865 2077 6164 646c 6520  here the waddle 
-00001720: 7374 6172 7465 642e 220a 2020 2020 2020  started.".      
-00001730: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-00001740: 2020 2020 2020 2020 2020 2020 2022 706f               "po
-00001750: 7358 223a 207b 0a20 2020 2020 2020 2020  sX": {.         
-00001760: 2020 2020 2020 2020 2020 2022 7479 7065             "type
-00001770: 223a 2022 666c 6f61 7422 2c0a 2020 2020  ": "float",.    
-00001780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001790: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
-000017a0: 5468 6520 6e65 7720 582d 706f 7369 7469  The new X-positi
-000017b0: 6f6e 2c20 7768 6572 6520 7468 6520 7761  on, where the wa
-000017c0: 6464 6c65 2065 6e64 6564 2e22 0a20 2020  ddle ended.".   
-000017d0: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
-000017e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017f0: 2270 6f73 5922 3a20 7b0a 2020 2020 2020  "posY": {.      
-00001800: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-00001810: 7970 6522 3a20 2266 6c6f 6174 222c 0a20  ype": "float",. 
-00001820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001830: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
-00001840: 3a20 2254 6865 206e 6577 2059 2d70 6f73  : "The new Y-pos
-00001850: 6974 696f 6e2c 2077 6865 7265 2074 6865  ition, where the
-00001860: 2077 6164 646c 6520 656e 6465 642e 220a   waddle ended.".
-00001870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001880: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
-00001890: 2020 2022 706f 735a 223a 207b 0a20 2020     "posZ": {.   
-000018a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018b0: 2022 7479 7065 223a 2022 666c 6f61 7422   "type": "float"
-000018c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000018d0: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
-000018e0: 6f6e 223a 2022 5468 6520 6e65 7720 5a2d  on": "The new Z-
-000018f0: 706f 7369 7469 6f6e 2c20 7768 6572 6520  position, where 
-00001900: 7468 6520 7761 6464 6c65 2065 6e64 6564  the waddle ended
-00001910: 2e22 0a20 2020 2020 2020 2020 2020 2020  .".             
-00001920: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
-00001930: 2020 2020 2020 2272 6f74 5822 3a20 7b0a        "rotX": {.
-00001940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001950: 2020 2020 2274 7970 6522 3a20 2266 6c6f      "type": "flo
-00001960: 6174 222c 0a20 2020 2020 2020 2020 2020  at",.           
-00001970: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
-00001980: 7074 696f 6e22 3a20 2254 6865 2058 2d63  ption": "The X-c
-00001990: 6f6d 706f 6e65 6e74 206f 6620 7468 6520  omponent of the 
-000019a0: 726f 7461 7469 6f6e 2077 6865 6e20 7468  rotation when th
-000019b0: 6520 7761 6464 6c65 2065 6e64 6564 2e22  e waddle ended."
-000019c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000019d0: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
-000019e0: 2020 2020 2272 6f74 5922 3a20 7b0a 2020      "rotY": {.  
-000019f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a00: 2020 2274 7970 6522 3a20 2266 6c6f 6174    "type": "float
-00001a10: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00001a20: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
-00001a30: 696f 6e22 3a20 2254 6865 2059 2d63 6f6d  ion": "The Y-com
-00001a40: 706f 6e65 6e74 206f 6620 7468 6520 726f  ponent of the ro
-00001a50: 7461 7469 6f6e 2077 6865 6e20 7468 6520  tation when the 
-00001a60: 7761 6464 6c65 2065 6e64 6564 2e22 0a20  waddle ended.". 
-00001a70: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00001a80: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001a90: 2020 2272 6f74 5a22 3a20 7b0a 2020 2020    "rotZ": {.    
-00001aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ab0: 2274 7970 6522 3a20 2266 6c6f 6174 222c  "type": "float",
-00001ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001ad0: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
-00001ae0: 6e22 3a20 2254 6865 205a 2d63 6f6d 706f  n": "The Z-compo
-00001af0: 6e65 6e74 206f 6620 7468 6520 726f 7461  nent of the rota
-00001b00: 7469 6f6e 2077 6865 6e20 7468 6520 7761  tion when the wa
-00001b10: 6464 6c65 2065 6e64 6564 2e22 0a20 2020  ddle ended.".   
-00001b20: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
-00001b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b40: 2272 6f74 5722 3a20 7b0a 2020 2020 2020  "rotW": {.      
-00001b50: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-00001b60: 7970 6522 3a20 2266 6c6f 6174 222c 0a20  ype": "float",. 
-00001b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b80: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
-00001b90: 3a20 2254 6865 2057 2d63 6f6d 706f 6e65  : "The W-compone
-00001ba0: 6e74 206f 6620 7468 6520 726f 7461 7469  nt of the rotati
-00001bb0: 6f6e 2077 6865 6e20 7468 6520 7761 6464  on when the wadd
-00001bc0: 6c65 2065 6e64 6564 2e22 0a20 2020 2020  le ended.".     
-00001bd0: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
-00001be0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-00001bf0: 6f75 7263 6522 3a20 7b0a 2020 2020 2020  ource": {.      
-00001c00: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-00001c10: 7970 6522 3a20 2265 6e75 6d28 4255 5454  ype": "enum(BUTT
-00001c20: 4f4e 2c20 5741 4444 4c45 2922 2c0a 2020  ON, WADDLE)",.  
-00001c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c40: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-00001c50: 2022 496e 6469 6361 746f 7220 666f 7220   "Indicator for 
-00001c60: 7768 6574 6865 7220 7468 6520 706c 6179  whether the play
-00001c70: 6572 2077 6164 646c 6564 2062 7920 7072  er waddled by pr
-00001c80: 6573 7369 6e67 2061 2062 7574 746f 6e2c  essing a button,
-00001c90: 206f 7220 6279 206d 616b 696e 6720 7468   or by making th
-00001ca0: 6520 2777 6164 646c 6527 2067 6573 7475  e 'waddle' gestu
-00001cb0: 7265 2077 6974 6820 7468 6569 7220 6865  re with their he
-00001cc0: 6164 2e22 0a20 2020 2020 2020 2020 2020  ad.".           
-00001cd0: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
-00001ce0: 2020 207d 0a20 2020 2020 2020 207d 2c0a     }.        },.
-00001cf0: 2020 2020 2020 2020 2267 617a 655f 6f62          "gaze_ob
-00001d00: 6a65 6374 5f62 6567 696e 223a 207b 0a20  ject_begin": {. 
-00001d10: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
-00001d20: 7269 7074 696f 6e22 3a20 2241 6e20 6576  ription": "An ev
-00001d30: 656e 7420 7472 6967 6765 7265 6420 7768  ent triggered wh
-00001d40: 656e 2074 6865 2070 6c61 7965 7220 6861  en the player ha
-00001d50: 7320 6761 7a65 6420 6174 2061 6e20 6f62  s gazed at an ob
-00001d60: 6a65 6374 2066 6f72 2061 7420 6c65 6173  ject for at leas
-00001d70: 7420 302e 3235 2073 6563 6f6e 6473 2c20  t 0.25 seconds, 
-00001d80: 7768 6572 6520 2767 617a 6564 2061 7427  where 'gazed at'
-00001d90: 206d 6561 6e73 2074 6865 206f 626a 6563   means the objec
-00001da0: 7420 6973 2074 6865 206e 6561 7265 7374  t is the nearest
-00001db0: 206f 6e20 6120 7261 7963 6173 7420 6672   on a raycast fr
-00001dc0: 6f6d 2074 6865 2076 6965 7770 6f72 7420  om the viewport 
-00001dd0: 6365 6e74 6572 222c 0a20 2020 2020 2020  center",.       
-00001de0: 2020 2020 2022 6576 656e 745f 6461 7461       "event_data
-00001df0: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-00001e00: 2020 2020 2022 6f62 6a65 6374 5f69 6422       "object_id"
-00001e10: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-00001e20: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
-00001e30: 2273 7472 222c 0a20 2020 2020 2020 2020  "str",.         
-00001e40: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
-00001e50: 7269 7074 696f 6e22 3a20 2254 6865 206e  ription": "The n
-00001e60: 616d 6520 6f66 2074 6865 206f 626a 6563  ame of the objec
-00001e70: 7420 7468 6520 706c 6179 6572 2069 7320  t the player is 
-00001e80: 6761 7a69 6e67 2061 7422 0a20 2020 2020  gazing at".     
-00001e90: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-00001ea0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00001eb0: 2020 207d 2c0a 2020 2020 2020 2020 2267     },.        "g
-00001ec0: 617a 655f 6f62 6a65 6374 5f65 6e64 223a  aze_object_end":
-00001ed0: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
-00001ee0: 6465 7363 7269 7074 696f 6e22 3a20 2241  description": "A
-00001ef0: 6e20 6576 656e 7420 7472 6967 6765 7265  n event triggere
-00001f00: 6420 7768 656e 2074 6865 2070 6c61 7965  d when the playe
-00001f10: 7220 7475 726e 7320 6177 6179 2066 726f  r turns away fro
-00001f20: 6d20 616e 206f 626a 6563 7420 7468 6579  m an object they
-00001f30: 2764 2067 617a 6564 2061 742c 2073 6f20  'd gazed at, so 
-00001f40: 7468 6520 6f62 6a65 6374 2069 7320 6e6f  the object is no
-00001f50: 206c 6f6e 6765 7220 6e65 6172 6573 7420   longer nearest 
-00001f60: 6f6e 2061 2072 6179 6361 7374 2066 726f  on a raycast fro
-00001f70: 6d20 7468 6520 7669 6577 706f 7274 2063  m the viewport c
-00001f80: 656e 7465 722e 204e 6f74 6520 7468 6572  enter. Note ther
-00001f90: 6520 6d61 7920 6265 2061 2073 6d61 6c6c  e may be a small
-00001fa0: 2062 7566 6665 7220 6172 6f75 6e64 2074   buffer around t
-00001fb0: 6865 206f 626a 6563 7420 666f 7220 7468  he object for th
-00001fc0: 6520 7261 7963 6173 742e 222c 0a20 2020  e raycast.",.   
-00001fd0: 2020 2020 2020 2020 2022 6576 656e 745f           "event_
-00001fe0: 6461 7461 223a 207b 0a20 2020 2020 2020  data": {.       
-00001ff0: 2020 2020 2020 2020 2022 6f62 6a65 6374           "object
-00002000: 5f69 6422 3a20 7b0a 2020 2020 2020 2020  _id": {.        
-00002010: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
-00002020: 6522 3a20 2273 7472 222c 0a20 2020 2020  e": "str",.     
-00002030: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00002040: 6465 7363 7269 7074 696f 6e22 3a20 2254  description": "T
-00002050: 6865 206e 616d 6520 6f66 2074 6865 206f  he name of the o
-00002060: 626a 6563 7420 7468 6520 706c 6179 6572  bject the player
-00002070: 2068 6164 2070 7265 7669 6f75 736c 7920   had previously 
-00002080: 6761 7a65 6420 6174 220a 2020 2020 2020  gazed at".      
-00002090: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-000020a0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-000020b0: 2020 7d2c 0a20 2020 2020 2020 2022 6275    },.        "bu
-000020c0: 6262 6c65 5f70 6f70 223a 207b 0a20 2020  bble_pop": {.   
-000020d0: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
-000020e0: 7074 696f 6e22 3a20 2241 6e20 6576 656e  ption": "An even
-000020f0: 7420 7472 6967 6765 7265 6420 7768 656e  t triggered when
-00002100: 2074 6865 2070 6c61 7965 7220 706f 7073   the player pops
-00002110: 2061 2062 7562 626c 6520 696e 2074 6865   a bubble in the
-00002120: 2062 7562 626c 652d 706f 7070 696e 6720   bubble-popping 
-00002130: 6d69 6e69 2d67 616d 652e 2041 2062 7562  mini-game. A bub
-00002140: 626c 6520 7368 6f75 6c64 2062 6520 706f  ble should be po
-00002150: 7070 6564 206f 6e20 6120 2762 6561 7427  pped on a 'beat'
-00002160: 206f 6620 7468 6520 6d75 7369 632c 2062   of the music, b
-00002170: 7574 2063 616e 2062 6520 706f 7070 6564  ut can be popped
-00002180: 2075 7020 746f 2030 2e35 2073 6563 6f6e   up to 0.5 secon
-00002190: 6473 2062 6566 6f72 6520 6f72 2061 6674  ds before or aft
-000021a0: 6572 2074 6865 2027 6265 6174 2e27 222c  er the 'beat.'",
-000021b0: 0a20 2020 2020 2020 2020 2020 2022 6576  .            "ev
-000021c0: 656e 745f 6461 7461 223a 207b 0a20 2020  ent_data": {.   
-000021d0: 2020 2020 2020 2020 2020 2020 2022 6f62               "ob
-000021e0: 6a65 6374 5f69 6422 3a20 7b0a 2020 2020  ject_id": {.    
-000021f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002200: 2274 7970 6522 3a20 2273 7472 222c 0a20  "type": "str",. 
-00002210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002220: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
-00002230: 3a20 2254 6865 206e 616d 6520 6f66 2074  : "The name of t
-00002240: 6865 2062 7562 626c 6520 6f62 6a65 6374  he bubble object
-00002250: 2074 6865 2070 6c61 7965 7220 706f 7070   the player popp
-00002260: 6564 220a 2020 2020 2020 2020 2020 2020  ed".            
-00002270: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-00002280: 2020 2020 2020 2022 7469 6d69 6e67 5f65         "timing_e
-00002290: 7272 6f72 223a 207b 0a20 2020 2020 2020  rror": {.       
-000022a0: 2020 2020 2020 2020 2020 2020 2022 7479               "ty
-000022b0: 7065 223a 2022 666c 6f61 7422 2c0a 2020  pe": "float",.  
-000022c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022d0: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-000022e0: 2022 5468 6520 7469 6d69 6e67 2064 6966   "The timing dif
-000022f0: 6665 7265 6e63 6520 6265 7477 6565 6e20  ference between 
-00002300: 7468 6520 706f 7020 6576 656e 7420 616e  the pop event an
-00002310: 6420 7468 6520 6d75 7369 6320 2762 6561  d the music 'bea
-00002320: 742e 2720 5468 6973 2076 616c 7565 2069  t.' This value i
-00002330: 7320 696e 2074 6865 2072 616e 6765 205b  s in the range [
-00002340: 2d30 2e35 2c20 302e 355d 2c20 7768 6572  -0.5, 0.5], wher
-00002350: 6520 6120 6e65 6761 7469 7665 2069 6e64  e a negative ind
-00002360: 6963 6174 6573 2074 6865 2062 7562 626c  icates the bubbl
-00002370: 6520 7761 7320 706f 7070 6564 2062 6566  e was popped bef
-00002380: 6f72 6520 7468 6520 2762 6561 742c 2720  ore the 'beat,' 
-00002390: 616e 6420 706f 7369 7469 7665 2069 6e64  and positive ind
-000023a0: 6963 6174 6573 2070 6f70 7069 6e67 2061  icates popping a
-000023b0: 6674 6572 2074 6865 2027 6265 6174 2e27  fter the 'beat.'
-000023c0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-000023d0: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
-000023e0: 7d0a 2020 2020 2020 2020 7d2c 0a20 2020  }.        },.   
-000023f0: 2020 2020 2022 6561 745f 6669 7368 223a       "eat_fish":
-00002400: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
-00002410: 6465 7363 7269 7074 696f 6e22 3a20 2241  description": "A
-00002420: 6e20 6576 656e 7420 7472 6967 6765 7265  n event triggere
-00002430: 6420 7768 656e 2074 6865 2070 6c61 7965  d when the playe
-00002440: 7220 6561 7473 2061 2066 6973 682e 222c  r eats a fish.",
-00002450: 0a20 2020 2020 2020 2020 2020 2022 6576  .            "ev
-00002460: 656e 745f 6461 7461 223a 207b 0a20 2020  ent_data": {.   
-00002470: 2020 2020 2020 2020 2020 2020 2022 6f62               "ob
-00002480: 6a65 6374 5f69 6422 3a20 7b0a 2020 2020  ject_id": {.    
-00002490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024a0: 2274 7970 6522 3a20 2273 7472 222c 0a20  "type": "str",. 
-000024b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024c0: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
-000024d0: 3a20 2254 6865 206e 616d 6520 6f66 2074  : "The name of t
-000024e0: 6865 2066 6973 6820 6f62 6a65 6374 2074  he fish object t
-000024f0: 6865 2070 6c61 7965 7220 6174 6522 0a20  he player ate". 
-00002500: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00002510: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
-00002520: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00002530: 2020 2266 6c69 7070 6572 5f62 6173 685f    "flipper_bash_
-00002540: 736b 7561 223a 207b 0a20 2020 2020 2020  skua": {.       
-00002550: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
-00002560: 6e22 3a20 2241 6e20 6576 656e 7420 7472  n": "An event tr
-00002570: 6967 6765 7265 6420 7768 656e 2074 6865  iggered when the
-00002580: 2070 6c61 7965 7220 6d61 6b65 7320 6120   player makes a 
-00002590: 666c 6970 7065 722d 6261 7368 696e 6720  flipper-bashing 
-000025a0: 6d6f 7665 2074 6f20 7368 6f6f 2061 2073  move to shoo a s
-000025b0: 6b75 6120 6177 6179 2066 726f 6d20 7468  kua away from th
-000025c0: 6569 7220 6e65 7374 2f65 6767 2e22 2c0a  eir nest/egg.",.
-000025d0: 2020 2020 2020 2020 2020 2020 2265 7665              "eve
-000025e0: 6e74 5f64 6174 6122 3a20 7b0a 2020 2020  nt_data": {.    
-000025f0: 2020 2020 2020 2020 2020 2020 226f 626a              "obj
-00002600: 6563 745f 6964 223a 207b 0a20 2020 2020  ect_id": {.     
-00002610: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00002620: 7479 7065 223a 2022 7374 7222 2c0a 2020  type": "str",.  
-00002630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002640: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-00002650: 2022 5468 6520 6e61 6d65 206f 6620 7468   "The name of th
-00002660: 6520 736b 7561 206f 626a 6563 7420 7468  e skua object th
-00002670: 6520 706c 6179 6572 2062 6173 6865 6422  e player bashed"
-00002680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002690: 207d 0a20 2020 2020 2020 2020 2020 207d   }.            }
-000026a0: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
-000026b0: 2020 2020 2270 6963 6b75 705f 726f 636b      "pickup_rock
-000026c0: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-000026d0: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
-000026e0: 2241 6e20 6576 656e 7420 7472 6967 6765  "An event trigge
-000026f0: 7265 6420 7768 656e 2074 6865 2070 6c61  red when the pla
-00002700: 7965 7220 7069 636b 7320 7570 2061 2072  yer picks up a r
-00002710: 6f63 6b20 6c79 696e 6720 6f6e 2074 6865  ock lying on the
-00002720: 2067 726f 756e 642c 2077 6869 6368 2063   ground, which c
-00002730: 6f6e 7472 6962 7574 6573 2074 6f20 7468  ontributes to th
-00002740: 6520 6275 696c 6469 6e67 206f 6620 7468  e building of th
-00002750: 6569 7220 6e65 7374 2e22 2c0a 2020 2020  eir nest.",.    
-00002760: 2020 2020 2020 2020 2265 7665 6e74 5f64          "event_d
-00002770: 6174 6122 3a20 7b0a 2020 2020 2020 2020  ata": {.        
-00002780: 2020 2020 2020 2020 2274 6f74 616c 5f70          "total_p
-00002790: 6963 6b65 645f 7570 223a 207b 0a20 2020  icked_up": {.   
-000027a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027b0: 2022 7479 7065 223a 2022 696e 7422 2c0a   "type": "int",.
-000027c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027d0: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
-000027e0: 223a 2022 5468 6520 7275 6e6e 696e 6720  ": "The running 
-000027f0: 746f 7461 6c20 6f66 2072 6f63 6b73 2074  total of rocks t
-00002800: 6865 2070 6c61 7965 7220 6861 7320 7069  he player has pi
-00002810: 636b 6564 2075 702e 220a 2020 2020 2020  cked up.".      
-00002820: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-00002830: 2020 2020 2020 2020 2020 2020 2022 7078               "px
-00002840: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-00002850: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
-00002860: 2022 666c 6f61 7422 2c0a 2020 2020 2020   "float",.      
-00002870: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-00002880: 6573 6372 6970 7469 6f6e 223a 2022 5468  escription": "Th
-00002890: 6520 782d 706f 7369 7469 6f6e 206f 6620  e x-position of 
-000028a0: 7468 6520 706c 6179 6572 2077 6865 6e20  the player when 
-000028b0: 7468 6520 6576 656e 7420 6861 7070 656e  the event happen
-000028c0: 6564 220a 2020 2020 2020 2020 2020 2020  ed".            
-000028d0: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-000028e0: 2020 2020 2020 2022 7079 223a 207b 0a20         "py": {. 
-000028f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002900: 2020 2022 7479 7065 223a 2022 666c 6f61     "type": "floa
-00002910: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
-00002920: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
-00002930: 7469 6f6e 223a 2022 5468 6520 792d 706f  tion": "The y-po
-00002940: 7369 7469 6f6e 206f 6620 7468 6520 706c  sition of the pl
-00002950: 6179 6572 2077 6865 6e20 7468 6520 6576  ayer when the ev
-00002960: 656e 7420 6861 7070 656e 6564 220a 2020  ent happened".  
-00002970: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
-00002980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002990: 2022 707a 223a 207b 0a20 2020 2020 2020   "pz": {.       
-000029a0: 2020 2020 2020 2020 2020 2020 2022 7479               "ty
-000029b0: 7065 223a 2022 666c 6f61 7422 2c0a 2020  pe": "float",.  
-000029c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029d0: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-000029e0: 2022 5468 6520 7a2d 706f 7369 7469 6f6e   "The z-position
-000029f0: 206f 6620 7468 6520 706c 6179 6572 2077   of the player w
-00002a00: 6865 6e20 7468 6520 6576 656e 7420 6861  hen the event ha
-00002a10: 7070 656e 6564 220a 2020 2020 2020 2020  ppened".        
-00002a20: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00002a30: 2020 2020 2020 2020 2020 2022 7178 223a             "qx":
-00002a40: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00002a50: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-00002a60: 666c 6f61 7422 2c0a 2020 2020 2020 2020  float",.        
-00002a70: 2020 2020 2020 2020 2020 2020 2264 6573              "des
-00002a80: 6372 6970 7469 6f6e 223a 2022 5468 6520  cription": "The 
-00002a90: 782d 636f 6d70 6f6e 656e 7420 6f66 2074  x-component of t
-00002aa0: 6865 2071 7561 7465 726e 696f 6e20 666f  he quaternion fo
-00002ab0: 7220 7468 6520 706c 6179 6572 2773 206f  r the player's o
-00002ac0: 7269 656e 7461 7469 6f6e 2077 6865 6e20  rientation when 
-00002ad0: 7468 6520 6576 656e 7420 6861 7070 656e  the event happen
-00002ae0: 6564 220a 2020 2020 2020 2020 2020 2020  ed".            
-00002af0: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-00002b00: 2020 2020 2020 2022 7179 223a 207b 0a20         "qy": {. 
-00002b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b20: 2020 2022 7479 7065 223a 2022 666c 6f61     "type": "floa
-00002b30: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
-00002b40: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
-00002b50: 7469 6f6e 223a 2022 5468 6520 792d 636f  tion": "The y-co
-00002b60: 6d70 6f6e 656e 7420 6f66 2074 6865 2071  mponent of the q
-00002b70: 7561 7465 726e 696f 6e20 666f 7220 7468  uaternion for th
-00002b80: 6520 706c 6179 6572 2773 206f 7269 656e  e player's orien
-00002b90: 7461 7469 6f6e 2077 6865 6e20 7468 6520  tation when the 
-00002ba0: 6576 656e 7420 6861 7070 656e 6564 220a  event happened".
-00002bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002bc0: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
-00002bd0: 2020 2022 717a 223a 207b 0a20 2020 2020     "qz": {.     
-00002be0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00002bf0: 7479 7065 223a 2022 666c 6f61 7422 2c0a  type": "float",.
-00002c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c10: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
-00002c20: 223a 2022 5468 6520 7a2d 636f 6d70 6f6e  ": "The z-compon
-00002c30: 656e 7420 6f66 2074 6865 2071 7561 7465  ent of the quate
-00002c40: 726e 696f 6e20 666f 7220 7468 6520 706c  rnion for the pl
-00002c50: 6179 6572 2773 206f 7269 656e 7461 7469  ayer's orientati
-00002c60: 6f6e 2077 6865 6e20 7468 6520 6576 656e  on when the even
-00002c70: 7420 6861 7070 656e 6564 220a 2020 2020  t happened".    
-00002c80: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
-00002c90: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00002ca0: 7177 223a 207b 0a20 2020 2020 2020 2020  qw": {.         
-00002cb0: 2020 2020 2020 2020 2020 2022 7479 7065             "type
-00002cc0: 223a 2022 666c 6f61 7422 2c0a 2020 2020  ": "float",.    
-00002cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ce0: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
-00002cf0: 5468 6520 772d 636f 6d70 6f6e 656e 7420  The w-component 
-00002d00: 6f66 2074 6865 2071 7561 7465 726e 696f  of the quaternio
-00002d10: 6e20 666f 7220 7468 6520 706c 6179 6572  n for the player
-00002d20: 2773 206f 7269 656e 7461 7469 6f6e 2077  's orientation w
-00002d30: 6865 6e20 7468 6520 6576 656e 7420 6861  hen the event ha
-00002d40: 7070 656e 6564 220a 2020 2020 2020 2020  ppened".        
-00002d50: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00002d60: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00002d70: 7d2c 0a20 2020 2020 2020 2022 7075 7368  },.        "push
-00002d80: 5f73 6e6f 7762 616c 6c22 3a20 7b0a 2020  _snowball": {.  
-00002d90: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
-00002da0: 6970 7469 6f6e 223a 2022 416e 2065 7665  iption": "An eve
-00002db0: 6e74 2074 7269 6767 6572 6564 2077 6865  nt triggered whe
-00002dc0: 6e20 7468 6520 706c 6179 6572 2070 7573  n the player pus
-00002dd0: 6865 7320 6120 736e 6f77 6261 6c6c 2064  hes a snowball d
-00002de0: 6f77 6e20 7468 6520 6869 6c6c 2e22 2c0a  own the hill.",.
-00002df0: 2020 2020 2020 2020 2020 2020 2265 7665              "eve
-00002e00: 6e74 5f64 6174 6122 3a20 7b0a 2020 2020  nt_data": {.    
-00002e10: 2020 2020 2020 2020 2020 2020 226f 626a              "obj
-00002e20: 6563 745f 6964 223a 207b 0a20 2020 2020  ect_id": {.     
-00002e30: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00002e40: 7479 7065 223a 2022 7374 7222 2c0a 2020  type": "str",.  
-00002e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e60: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-00002e70: 2022 5468 6520 6e61 6d65 206f 6620 7468   "The name of th
-00002e80: 6520 736e 6f77 6261 6c6c 206f 626a 6563  e snowball objec
-00002e90: 7420 7468 6520 706c 6179 6572 2070 7573  t the player pus
-00002ea0: 6865 6422 0a20 2020 2020 2020 2020 2020  hed".           
-00002eb0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-00002ec0: 2020 2020 2020 2020 2270 7822 3a20 7b0a          "px": {.
-00002ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ee0: 2020 2020 2274 7970 6522 3a20 2266 6c6f      "type": "flo
-00002ef0: 6174 222c 0a20 2020 2020 2020 2020 2020  at",.           
-00002f00: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
-00002f10: 7074 696f 6e22 3a20 2254 6865 2078 2d70  ption": "The x-p
-00002f20: 6f73 6974 696f 6e20 6f66 2074 6865 2070  osition of the p
-00002f30: 6c61 7965 7220 7768 656e 2074 6865 2065  layer when the e
-00002f40: 7665 6e74 2068 6170 7065 6e65 6422 0a20  vent happened". 
-00002f50: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00002f60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002f70: 2020 2270 7922 3a20 7b0a 2020 2020 2020    "py": {.      
-00002f80: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-00002f90: 7970 6522 3a20 2266 6c6f 6174 222c 0a20  ype": "float",. 
-00002fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002fb0: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
-00002fc0: 3a20 2254 6865 2079 2d70 6f73 6974 696f  : "The y-positio
-00002fd0: 6e20 6f66 2074 6865 2070 6c61 7965 7220  n of the player 
-00002fe0: 7768 656e 2074 6865 2065 7665 6e74 2068  when the event h
-00002ff0: 6170 7065 6e65 6422 0a20 2020 2020 2020  appened".       
-00003000: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00003010: 2020 2020 2020 2020 2020 2020 2270 7a22              "pz"
-00003020: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-00003030: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
-00003040: 2266 6c6f 6174 222c 0a20 2020 2020 2020  "float",.       
-00003050: 2020 2020 2020 2020 2020 2020 2022 6465               "de
-00003060: 7363 7269 7074 696f 6e22 3a20 2254 6865  scription": "The
-00003070: 207a 2d70 6f73 6974 696f 6e20 6f66 2074   z-position of t
-00003080: 6865 2070 6c61 7965 7220 7768 656e 2074  he player when t
-00003090: 6865 2065 7665 6e74 2068 6170 7065 6e65  he event happene
-000030a0: 6422 0a20 2020 2020 2020 2020 2020 2020  d".             
-000030b0: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
-000030c0: 2020 2020 2020 2271 7822 3a20 7b0a 2020        "qx": {.  
-000030d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030e0: 2020 2274 7970 6522 3a20 2266 6c6f 6174    "type": "float
-000030f0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00003100: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
-00003110: 696f 6e22 3a20 2254 6865 2078 2d63 6f6d  ion": "The x-com
-00003120: 706f 6e65 6e74 206f 6620 7468 6520 7175  ponent of the qu
-00003130: 6174 6572 6e69 6f6e 2066 6f72 2074 6865  aternion for the
-00003140: 2070 6c61 7965 7227 7320 6f72 6965 6e74   player's orient
-00003150: 6174 696f 6e20 7768 656e 2074 6865 2065  ation when the e
-00003160: 7665 6e74 2068 6170 7065 6e65 6422 0a20  vent happened". 
-00003170: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00003180: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00003190: 2020 2271 7922 3a20 7b0a 2020 2020 2020    "qy": {.      
-000031a0: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-000031b0: 7970 6522 3a20 2266 6c6f 6174 222c 0a20  ype": "float",. 
-000031c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031d0: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
-000031e0: 3a20 2254 6865 2079 2d63 6f6d 706f 6e65  : "The y-compone
-000031f0: 6e74 206f 6620 7468 6520 7175 6174 6572  nt of the quater
-00003200: 6e69 6f6e 2066 6f72 2074 6865 2070 6c61  nion for the pla
-00003210: 7965 7227 7320 6f72 6965 6e74 6174 696f  yer's orientatio
-00003220: 6e20 7768 656e 2074 6865 2065 7665 6e74  n when the event
-00003230: 2068 6170 7065 6e65 6422 0a20 2020 2020   happened".     
-00003240: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
-00003250: 2020 2020 2020 2020 2020 2020 2020 2271                "q
-00003260: 7a22 3a20 7b0a 2020 2020 2020 2020 2020  z": {.          
-00003270: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
-00003280: 3a20 2266 6c6f 6174 222c 0a20 2020 2020  : "float",.     
-00003290: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000032a0: 6465 7363 7269 7074 696f 6e22 3a20 2254  description": "T
-000032b0: 6865 207a 2d63 6f6d 706f 6e65 6e74 206f  he z-component o
-000032c0: 6620 7468 6520 7175 6174 6572 6e69 6f6e  f the quaternion
-000032d0: 2066 6f72 2074 6865 2070 6c61 7965 7227   for the player'
-000032e0: 7320 6f72 6965 6e74 6174 696f 6e20 7768  s orientation wh
-000032f0: 656e 2074 6865 2065 7665 6e74 2068 6170  en the event hap
-00003300: 7065 6e65 6422 0a20 2020 2020 2020 2020  pened".         
-00003310: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00003320: 2020 2020 2020 2020 2020 2271 7722 3a20            "qw": 
-00003330: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00003340: 2020 2020 2020 2274 7970 6522 3a20 2266        "type": "f
-00003350: 6c6f 6174 222c 0a20 2020 2020 2020 2020  loat",.         
-00003360: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
-00003370: 7269 7074 696f 6e22 3a20 2254 6865 2077  ription": "The w
-00003380: 2d63 6f6d 706f 6e65 6e74 206f 6620 7468  -component of th
-00003390: 6520 7175 6174 6572 6e69 6f6e 2066 6f72  e quaternion for
-000033a0: 2074 6865 2070 6c61 7965 7227 7320 6f72   the player's or
-000033b0: 6965 6e74 6174 696f 6e20 7768 656e 2074  ientation when t
-000033c0: 6865 2065 7665 6e74 2068 6170 7065 6e65  he event happene
-000033d0: 6422 0a20 2020 2020 2020 2020 2020 2020  d".             
-000033e0: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
-000033f0: 207d 0a20 2020 2020 2020 207d 2c0a 2020   }.        },.  
-00003400: 2020 2020 2020 2272 696e 675f 6368 696d        "ring_chim
-00003410: 6522 3a20 7b0a 2020 2020 2020 2020 2020  e": {.          
-00003420: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-00003430: 2022 416e 2065 7665 6e74 2077 6865 6e20   "An event when 
-00003440: 7468 6520 706c 6179 6572 2072 696e 6773  the player rings
-00003450: 206f 6e65 206f 6620 7468 6520 6368 696d   one of the chim
-00003460: 6573 2069 6e20 7468 6520 6368 696d 6520  es in the chime 
-00003470: 6d69 6e69 2d67 616d 652e 222c 0a20 2020  mini-game.",.   
-00003480: 2020 2020 2020 2020 2022 6576 656e 745f           "event_
-00003490: 6461 7461 223a 207b 0a20 2020 2020 2020  data": {.       
-000034a0: 2020 2020 2020 2020 2022 6e6f 7465 5f70           "note_p
-000034b0: 6c61 7965 6422 3a20 7b0a 2020 2020 2020  layed": {.      
-000034c0: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-000034d0: 7970 6522 3a20 2273 7472 222c 0a20 2020  ype": "str",.   
-000034e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000034f0: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
-00003500: 2254 6865 206e 616d 6520 6f66 2074 6865  "The name of the
-00003510: 2063 6869 6d65 2074 6865 2070 6c61 7965   chime the playe
-00003520: 7220 7261 6e67 220a 2020 2020 2020 2020  r rang".        
-00003530: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00003540: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00003550: 7d2c 0a20 2020 2020 2020 2022 6275 6262  },.        "bubb
-00003560: 6c65 5f61 7070 6561 7265 6422 3a20 7b0a  le_appeared": {.
-00003570: 2020 2020 2020 2020 2020 2020 2264 6573              "des
-00003580: 6372 6970 7469 6f6e 223a 2022 4576 656e  cription": "Even
-00003590: 7420 7768 656e 2061 206e 6577 2062 7562  t when a new bub
-000035a0: 626c 6520 6170 7065 6172 7320 696e 2074  ble appears in t
-000035b0: 6865 206d 6174 696e 6720 6461 6e63 6520  he mating dance 
-000035c0: 6d69 6e69 6761 6d65 2e22 2c0a 2020 2020  minigame.",.    
-000035d0: 2020 2020 2020 2020 2265 7665 6e74 5f64          "event_d
-000035e0: 6174 6122 3a20 7b0a 2020 2020 2020 2020  ata": {.        
-000035f0: 2020 2020 2020 2020 226f 626a 6563 745f          "object_
-00003600: 6964 223a 207b 0a20 2020 2020 2020 2020  id": {.         
-00003610: 2020 2020 2020 2020 2020 2022 7479 7065             "type
-00003620: 223a 2022 7374 7222 2c0a 2020 2020 2020  ": "str",.      
-00003630: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-00003640: 6573 6372 6970 7469 6f6e 223a 2022 5468  escription": "Th
-00003650: 6520 6e61 6d65 206f 6620 7468 6520 6275  e name of the bu
-00003660: 6262 6c65 206f 626a 6563 7420 7468 6174  bble object that
-00003670: 2061 7070 6561 7265 6422 0a20 2020 2020   appeared".     
-00003680: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
-00003690: 2020 2020 2020 2020 2020 2020 2020 2270                "p
-000036a0: 6f73 5822 3a20 7b0a 2020 2020 2020 2020  osX": {.        
-000036b0: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
-000036c0: 6522 3a20 2266 6c6f 6174 222c 0a20 2020  e": "float",.   
-000036d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036e0: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
-000036f0: 2254 6865 2078 2d70 6f73 6974 696f 6e20  "The x-position 
-00003700: 6f66 2074 6865 2062 7562 626c 6520 7468  of the bubble th
-00003710: 6174 2061 7070 6561 7265 6422 0a20 2020  at appeared".   
-00003720: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
-00003730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003740: 2270 6f73 5922 3a20 7b0a 2020 2020 2020  "posY": {.      
-00003750: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-00003760: 7970 6522 3a20 2266 6c6f 6174 222c 0a20  ype": "float",. 
-00003770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003780: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
-00003790: 3a20 2254 6865 2079 2d70 6f73 6974 696f  : "The y-positio
-000037a0: 6e20 6f66 2074 6865 2062 7562 626c 6520  n of the bubble 
-000037b0: 7468 6174 2061 7070 6561 7265 6422 0a20  that appeared". 
-000037c0: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-000037d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000037e0: 2020 2270 6f73 5a22 3a20 7b0a 2020 2020    "posZ": {.    
-000037f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003800: 2274 7970 6522 3a20 2266 6c6f 6174 222c  "type": "float",
-00003810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003820: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
-00003830: 6e22 3a20 2254 6865 207a 2d70 6f73 6974  n": "The z-posit
-00003840: 696f 6e20 6f66 2074 6865 2062 7562 626c  ion of the bubbl
-00003850: 6520 7468 6174 2061 7070 6561 7265 6422  e that appeared"
-00003860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003870: 207d 0a20 2020 2020 2020 2020 2020 207d   }.            }
-00003880: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
-00003890: 2020 2020 2262 7562 626c 655f 6578 7069      "bubble_expi
-000038a0: 7265 6422 3a20 7b0a 2020 2020 2020 2020  red": {.        
-000038b0: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
-000038c0: 223a 2022 4576 656e 7420 7768 656e 2061  ": "Event when a
-000038d0: 2062 7562 626c 6527 7320 706f 702d 6162   bubble's pop-ab
-000038e0: 6c65 2074 696d 6520 656e 6473 2061 6e64  le time ends and
-000038f0: 2074 6865 2062 7562 626c 6520 6469 7361   the bubble disa
-00003900: 7070 6561 7273 2e22 2c0a 2020 2020 2020  ppears.",.      
-00003910: 2020 2020 2020 2265 7665 6e74 5f64 6174        "event_dat
-00003920: 6122 3a20 7b0a 2020 2020 2020 2020 2020  a": {.          
-00003930: 2020 2020 2020 226f 626a 6563 745f 6964        "object_id
-00003940: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-00003950: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
-00003960: 2022 7374 7222 2c0a 2020 2020 2020 2020   "str",.        
-00003970: 2020 2020 2020 2020 2020 2020 2264 6573              "des
-00003980: 6372 6970 7469 6f6e 223a 2022 5468 6520  cription": "The 
-00003990: 6e61 6d65 206f 6620 7468 6520 6275 6262  name of the bubb
-000039a0: 6c65 206f 626a 6563 7420 7468 6174 2064  le object that d
-000039b0: 6973 6170 7065 6172 6564 220a 2020 2020  isappeared".    
-000039c0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-000039d0: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-000039e0: 2020 2020 7d2c 0a20 2020 2020 2020 2022      },.        "
-000039f0: 6567 675f 6861 7463 685f 696e 6469 6361  egg_hatch_indica
-00003a00: 746f 725f 7570 6461 7465 6422 3a20 7b0a  tor_updated": {.
-00003a10: 2020 2020 2020 2020 2020 2020 2264 6573              "des
-00003a20: 6372 6970 7469 6f6e 223a 2022 4e4f 5420  cription": "NOT 
-00003a30: 5945 5420 444f 4355 4d45 4e54 4544 222c  YET DOCUMENTED",
-00003a40: 0a20 2020 2020 2020 2020 2020 2022 6576  .            "ev
-00003a50: 656e 745f 6461 7461 223a 207b 0a20 2020  ent_data": {.   
-00003a60: 2020 2020 2020 2020 2020 2020 2022 7469               "ti
-00003a70: 6d65 5f72 656d 6169 6e69 6e67 223a 207b  me_remaining": {
-00003a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003a90: 2020 2020 2022 7479 7065 223a 2022 696e       "type": "in
-00003aa0: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
-00003ab0: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
-00003ac0: 7469 6f6e 223a 2022 5468 6520 7469 6d65  tion": "The time
-00003ad0: 206c 6566 7420 756e 7469 6c20 7468 6520   left until the 
-00003ae0: 6567 6720 7769 6c6c 2068 6174 6368 220a  egg will hatch".
-00003af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b00: 7d0a 2020 2020 2020 2020 2020 2020 7d0a  }.            }.
-00003b10: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00003b20: 2020 2022 6567 675f 6861 7463 6865 6422     "egg_hatched"
-00003b30: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-00003b40: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
-00003b50: 4576 656e 7420 7768 656e 2074 6865 2065  Event when the e
-00003b60: 6767 2068 6174 6368 6573 222c 0a20 2020  gg hatches",.   
-00003b70: 2020 2020 2020 2020 2022 6576 656e 745f           "event_
-00003b80: 6461 7461 223a 207b 7d0a 2020 2020 2020  data": {}.      
-00003b90: 2020 7d2c 0a20 2020 2020 2020 2022 6567    },.        "eg
-00003ba0: 675f 6c6f 7374 223a 207b 0a20 2020 2020  g_lost": {.     
-00003bb0: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
-00003bc0: 696f 6e22 3a20 2245 7665 6e74 2077 6865  ion": "Event whe
-00003bd0: 6e20 7468 6520 706c 6179 6572 2773 2065  n the player's e
-00003be0: 6767 2069 7320 7374 6f6c 656e 2062 7920  gg is stolen by 
-00003bf0: 6120 736b 7561 2e22 2c0a 2020 2020 2020  a skua.",.      
-00003c00: 2020 2020 2020 2265 7665 6e74 5f64 6174        "event_dat
-00003c10: 6122 3a20 7b0a 2020 2020 2020 2020 2020  a": {.          
-00003c20: 2020 2020 2020 226f 626a 6563 745f 6964        "object_id
-00003c30: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-00003c40: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
-00003c50: 2022 7374 7222 2c0a 2020 2020 2020 2020   "str",.        
-00003c60: 2020 2020 2020 2020 2020 2020 2264 6573              "des
-00003c70: 6372 6970 7469 6f6e 223a 2022 5468 6520  cription": "The 
-00003c80: 6e61 6d65 206f 6620 7468 6520 736b 7561  name of the skua
-00003c90: 2074 6861 7420 7374 6f6c 6520 7468 6520   that stole the 
-00003ca0: 6567 6722 0a20 2020 2020 2020 2020 2020  egg".           
-00003cb0: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
-00003cc0: 2020 207d 0a20 2020 2020 2020 207d 2c0a     }.        },.
-00003cd0: 2020 2020 2020 2020 2265 6767 5f72 6563          "egg_rec
-00003ce0: 6f76 6572 6564 223a 207b 0a20 2020 2020  overed": {.     
-00003cf0: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
-00003d00: 696f 6e22 3a20 2245 7665 6e74 2077 6865  ion": "Event whe
-00003d10: 6e20 7468 6520 706c 6179 6572 2072 6563  n the player rec
-00003d20: 6f76 6572 7320 7468 6520 6567 6720 6672  overs the egg fr
-00003d30: 6f6d 2074 6865 2073 6b75 6173 2e22 2c0a  om the skuas.",.
-00003d40: 2020 2020 2020 2020 2020 2020 2265 7665              "eve
-00003d50: 6e74 5f64 6174 6122 3a20 7b7d 0a20 2020  nt_data": {}.   
-00003d60: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-00003d70: 226d 6174 696e 675f 6461 6e63 655f 696e  "mating_dance_in
-00003d80: 6469 6361 746f 725f 7570 6461 7465 6422  dicator_updated"
-00003d90: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-00003da0: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
-00003db0: 4576 656e 7420 7768 656e 2061 2062 7562  Event when a bub
-00003dc0: 626c 6520 6973 2070 6f70 7065 6420 616e  ble is popped an
-00003dd0: 6420 7468 6520 696e 6469 6361 746f 7220  d the indicator 
-00003de0: 666f 7220 7072 6f67 7265 7373 2074 6f20  for progress to 
-00003df0: 636f 6d70 6c65 7469 6f6e 206f 6620 7468  completion of th
-00003e00: 6520 6d61 7469 6e67 2064 616e 6365 2075  e mating dance u
-00003e10: 7064 6174 6573 2e22 2c0a 2020 2020 2020  pdates.",.      
-00003e20: 2020 2020 2020 2265 7665 6e74 5f64 6174        "event_dat
-00003e30: 6122 3a20 7b0a 2020 2020 2020 2020 2020  a": {.          
-00003e40: 2020 2020 2020 2270 6572 6365 6e74 5f66        "percent_f
-00003e50: 756c 6c22 3a20 7b0a 2020 2020 2020 2020  ull": {.        
-00003e60: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
-00003e70: 6522 3a20 2269 6e74 222c 0a20 2020 2020  e": "int",.     
-00003e80: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00003e90: 6465 7363 7269 7074 696f 6e22 3a20 2254  description": "T
-00003ea0: 6865 206e 6577 2070 6572 6365 6e74 2074  he new percent t
-00003eb0: 6f20 7768 6963 6820 7468 6520 6461 6e63  o which the danc
-00003ec0: 6520 636f 6d70 6c65 7469 6f6e 2069 6e64  e completion ind
-00003ed0: 6963 6174 6f72 2069 7320 6669 6c6c 6564  icator is filled
-00003ee0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00003ef0: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
-00003f00: 7d0a 2020 2020 2020 2020 7d2c 0a20 2020  }.        },.   
-00003f10: 2020 2020 2022 6e65 7374 5f63 6f6d 706c       "nest_compl
-00003f20: 6574 6522 3a20 7b0a 2020 2020 2020 2020  ete": {.        
-00003f30: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
-00003f40: 223a 2022 4576 656e 7420 7768 656e 2074  ": "Event when t
-00003f50: 6865 2070 6c61 7965 7220 636f 6d70 6c65  he player comple
-00003f60: 7465 7320 7468 6520 6275 696c 6469 6e67  tes the building
-00003f70: 206f 6620 7468 6569 7220 6e65 7374 2e22   of their nest."
-00003f80: 2c0a 2020 2020 2020 2020 2020 2020 2265  ,.            "e
-00003f90: 7665 6e74 5f64 6174 6122 3a20 7b7d 0a20  vent_data": {}. 
-00003fa0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00003fb0: 2020 2270 656e 6775 696e 5f70 696e 5f66    "penguin_pin_f
-00003fc0: 656c 6c22 3a20 7b0a 2020 2020 2020 2020  ell": {.        
-00003fd0: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
-00003fe0: 223a 2022 5768 656e 206f 6e65 206f 6620  ": "When one of 
-00003ff0: 7468 6520 7069 6e73 2066 656c 6c20 696e  the pins fell in
-00004000: 2074 6865 2062 6f77 6c69 6e67 2061 7265   the bowling are
-00004010: 612e 222c 0a20 2020 2020 2020 2020 2020  a.",.           
-00004020: 2022 6576 656e 745f 6461 7461 223a 207b   "event_data": {
-00004030: 7d0a 2020 2020 2020 2020 7d2c 0a20 2020  }.        },.   
-00004040: 2020 2020 2022 736b 7561 5f73 7061 776e       "skua_spawn
-00004050: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-00004060: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
-00004070: 2245 7665 6e74 2077 6865 6e20 6120 6e65  "Event when a ne
-00004080: 7720 736b 7561 2069 7320 6164 6465 6420  w skua is added 
-00004090: 696e 2074 6865 206e 6573 742f 6567 6720  in the nest/egg 
-000040a0: 6465 6665 6e73 6520 6d69 6e69 2d67 616d  defense mini-gam
-000040b0: 652e 222c 0a20 2020 2020 2020 2020 2020  e.",.           
-000040c0: 2022 6576 656e 745f 6461 7461 223a 207b   "event_data": {
-000040d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000040e0: 2022 6f62 6a65 6374 5f69 6422 3a20 7b0a   "object_id": {.
-000040f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004100: 2020 2020 2274 7970 6522 3a20 2273 7472      "type": "str
-00004110: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00004120: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
-00004130: 696f 6e22 3a20 2254 6865 206e 616d 6520  ion": "The name 
-00004140: 6f66 2074 6865 2073 6b75 6120 6f62 6a65  of the skua obje
-00004150: 6374 2074 6861 7420 6170 7065 6172 6564  ct that appeared
-00004160: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00004170: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
-00004180: 2020 2020 2022 706f 7358 223a 207b 0a20       "posX": {. 
-00004190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000041a0: 2020 2022 7479 7065 223a 2022 666c 6f61     "type": "floa
-000041b0: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
-000041c0: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
-000041d0: 7469 6f6e 223a 2022 5468 6520 782d 706f  tion": "The x-po
-000041e0: 7369 7469 6f6e 206f 6620 7468 6520 736b  sition of the sk
-000041f0: 7561 2074 6861 7420 6170 7065 6172 6564  ua that appeared
-00004200: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00004210: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
-00004220: 2020 2020 2022 706f 7359 223a 207b 0a20       "posY": {. 
-00004230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004240: 2020 2022 7479 7065 223a 2022 666c 6f61     "type": "floa
-00004250: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
-00004260: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
-00004270: 7469 6f6e 223a 2022 5468 6520 792d 706f  tion": "The y-po
-00004280: 7369 7469 6f6e 206f 6620 7468 6520 736b  sition of the sk
-00004290: 7561 2074 6861 7420 6170 7065 6172 6564  ua that appeared
-000042a0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-000042b0: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
-000042c0: 2020 2020 2022 706f 735a 223a 207b 0a20       "posZ": {. 
-000042d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000042e0: 2020 2022 7479 7065 223a 2022 666c 6f61     "type": "floa
-000042f0: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
-00004300: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
-00004310: 7469 6f6e 223a 2022 5468 6520 7a2d 706f  tion": "The z-po
-00004320: 7369 7469 6f6e 206f 6620 7468 6520 736b  sition of the sk
-00004330: 7561 2074 6861 7420 6170 7065 6172 6564  ua that appeared
-00004340: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00004350: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
-00004360: 7d0a 2020 2020 2020 2020 7d2c 0a20 2020  }.        },.   
-00004370: 2020 2020 2022 736b 7561 5f6d 6f76 6522       "skua_move"
-00004380: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-00004390: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
-000043a0: 4576 656e 7420 7768 656e 2061 2073 6b75  Event when a sku
-000043b0: 6120 6d6f 7665 7320 746f 2061 206e 6577  a moves to a new
-000043c0: 206c 6f63 6174 696f 6e20 696e 2074 6865   location in the
-000043d0: 206e 6573 742f 6567 6720 6465 6665 6e73   nest/egg defens
-000043e0: 6520 6d69 6e69 2d67 616d 652e 222c 0a20  e mini-game.",. 
-000043f0: 2020 2020 2020 2020 2020 2022 6576 656e             "even
-00004400: 745f 6461 7461 223a 207b 0a20 2020 2020  t_data": {.     
-00004410: 2020 2020 2020 2020 2020 2022 6f62 6a65             "obje
-00004420: 6374 5f69 6422 3a20 7b0a 2020 2020 2020  ct_id": {.      
-00004430: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-00004440: 7970 6522 3a20 2273 7472 222c 0a20 2020  ype": "str",.   
-00004450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004460: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
-00004470: 2254 6865 206e 616d 6520 6f66 2074 6865  "The name of the
-00004480: 2073 6b75 6120 6f62 6a65 6374 2074 6861   skua object tha
-00004490: 7420 6d6f 7665 6422 0a20 2020 2020 2020  t moved".       
-000044a0: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-000044b0: 2020 2020 2020 2020 2020 2020 2266 726f              "fro
-000044c0: 6d5f 706f 7369 7469 6f6e 5f78 223a 207b  m_position_x": {
-000044d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000044e0: 2020 2020 2022 7479 7065 223a 2022 666c       "type": "fl
-000044f0: 6f61 7422 2c0a 2020 2020 2020 2020 2020  oat",.          
-00004500: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
-00004510: 6970 7469 6f6e 223a 2022 5468 6520 696e  iption": "The in
-00004520: 6974 6961 6c20 782d 706f 7369 7469 6f6e  itial x-position
-00004530: 206f 6620 7468 6520 736b 7561 2074 6861   of the skua tha
-00004540: 7420 6d6f 7665 6422 0a20 2020 2020 2020  t moved".       
-00004550: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00004560: 2020 2020 2020 2020 2020 2020 2266 726f              "fro
-00004570: 6d5f 706f 7369 7469 6f6e 5f79 223a 207b  m_position_y": {
-00004580: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004590: 2020 2020 2022 7479 7065 223a 2022 666c       "type": "fl
-000045a0: 6f61 7422 2c0a 2020 2020 2020 2020 2020  oat",.          
-000045b0: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
-000045c0: 6970 7469 6f6e 223a 2022 5468 6520 696e  iption": "The in
-000045d0: 6974 6961 6c20 792d 706f 7369 7469 6f6e  itial y-position
-000045e0: 206f 6620 7468 6520 736b 7561 2074 6861   of the skua tha
-000045f0: 7420 6d6f 7665 6422 0a20 2020 2020 2020  t moved".       
-00004600: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00004610: 2020 2020 2020 2020 2020 2020 2266 726f              "fro
-00004620: 6d5f 706f 7369 7469 6f6e 5f7a 223a 207b  m_position_z": {
-00004630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004640: 2020 2020 2022 7479 7065 223a 2022 666c       "type": "fl
-00004650: 6f61 7422 2c0a 2020 2020 2020 2020 2020  oat",.          
-00004660: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
-00004670: 6970 7469 6f6e 223a 2022 5468 6520 696e  iption": "The in
-00004680: 6974 6961 6c20 7a2d 706f 7369 7469 6f6e  itial z-position
-00004690: 206f 6620 7468 6520 736b 7561 2074 6861   of the skua tha
-000046a0: 7420 6d6f 7665 6422 0a20 2020 2020 2020  t moved".       
-000046b0: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-000046c0: 2020 2020 2020 2020 2020 2020 2274 6f5f              "to_
-000046d0: 706f 7369 7469 6f6e 5f78 223a 207b 0a20  position_x": {. 
-000046e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000046f0: 2020 2022 7479 7065 223a 2022 666c 6f61     "type": "floa
-00004700: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
-00004710: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
-00004720: 7469 6f6e 223a 2022 5468 6520 6e65 7720  tion": "The new 
-00004730: 782d 706f 7369 7469 6f6e 206f 6620 7468  x-position of th
-00004740: 6520 736b 7561 2074 6861 7420 6d6f 7665  e skua that move
-00004750: 6422 0a20 2020 2020 2020 2020 2020 2020  d".             
-00004760: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
-00004770: 2020 2020 2020 2274 6f5f 706f 7369 7469        "to_positi
-00004780: 6f6e 5f79 223a 207b 0a20 2020 2020 2020  on_y": {.       
-00004790: 2020 2020 2020 2020 2020 2020 2022 7479               "ty
-000047a0: 7065 223a 2022 666c 6f61 7422 2c0a 2020  pe": "float",.  
-000047b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000047c0: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-000047d0: 2022 5468 6520 6e65 7720 792d 706f 7369   "The new y-posi
-000047e0: 7469 6f6e 206f 6620 7468 6520 736b 7561  tion of the skua
-000047f0: 2074 6861 7420 6d6f 7665 6422 0a20 2020   that moved".   
-00004800: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
-00004810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004820: 2274 6f5f 706f 7369 7469 6f6e 5f7a 223a  "to_position_z":
-00004830: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00004840: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-00004850: 666c 6f61 7422 2c0a 2020 2020 2020 2020  float",.        
-00004860: 2020 2020 2020 2020 2020 2020 2264 6573              "des
-00004870: 6372 6970 7469 6f6e 223a 2022 5468 6520  cription": "The 
-00004880: 6e65 7720 7a2d 706f 7369 7469 6f6e 206f  new z-position o
-00004890: 6620 7468 6520 736b 7561 2074 6861 7420  f the skua that 
-000048a0: 6d6f 7665 6422 0a20 2020 2020 2020 2020  moved".         
-000048b0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-000048c0: 2020 2020 207d 0a20 2020 2020 2020 207d       }.        }
-000048d0: 2c0a 2020 2020 2020 2020 2265 6e74 6572  ,.        "enter
-000048e0: 5f72 6567 696f 6e22 3a20 7b0a 2020 2020  _region": {.    
-000048f0: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
-00004900: 7469 6f6e 223a 2022 4576 656e 7420 7768  tion": "Event wh
-00004910: 656e 2074 6865 2070 6c61 7965 7220 6d6f  en the player mo
-00004920: 7665 7320 696e 746f 206f 6e65 206f 6620  ves into one of 
-00004930: 7468 6520 7265 6769 6f6e 7320 636f 6e74  the regions cont
-00004940: 6169 6e69 6e67 2061 206d 696e 692d 6761  aining a mini-ga
-00004950: 6d65 206f 7220 6f74 6865 7220 6665 6174  me or other feat
-00004960: 7572 652e 222c 0a20 2020 2020 2020 2020  ure.",.         
-00004970: 2020 2022 6576 656e 745f 6461 7461 223a     "event_data":
-00004980: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00004990: 2020 2022 7265 6769 6f6e 5f6e 616d 6522     "region_name"
-000049a0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-000049b0: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
-000049c0: 2273 7472 222c 0a20 2020 2020 2020 2020  "str",.         
-000049d0: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
-000049e0: 7269 7074 696f 6e22 3a20 2254 6865 206e  ription": "The n
-000049f0: 616d 6520 6f66 2074 6865 2072 6567 696f  ame of the regio
-00004a00: 6e20 7468 6520 706c 6179 6572 2065 6e74  n the player ent
-00004a10: 6572 6564 220a 2020 2020 2020 2020 2020  ered".          
-00004a20: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00004a30: 2020 2020 7d0a 2020 2020 2020 2020 7d2c      }.        },
-00004a40: 0a20 2020 2020 2020 2022 6578 6974 5f72  .        "exit_r
-00004a50: 6567 696f 6e22 3a20 7b0a 2020 2020 2020  egion": {.      
-00004a60: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
-00004a70: 6f6e 223a 2022 4576 656e 7420 7768 656e  on": "Event when
-00004a80: 2061 206d 6f76 6573 206f 7574 206f 6620   a moves out of 
-00004a90: 6f6e 6520 6f66 2074 6865 2072 6567 696f  one of the regio
-00004aa0: 6e73 2063 6f6e 7461 696e 696e 6720 6120  ns containing a 
-00004ab0: 6d69 6e69 2d67 616d 6520 6f72 206f 7468  mini-game or oth
-00004ac0: 6572 2066 6561 7475 7265 2e22 2c0a 2020  er feature.",.  
-00004ad0: 2020 2020 2020 2020 2020 2265 7665 6e74            "event
-00004ae0: 5f64 6174 6122 3a20 7b0a 2020 2020 2020  _data": {.      
-00004af0: 2020 2020 2020 2020 2020 2272 6567 696f            "regio
-00004b00: 6e5f 6e61 6d65 223a 207b 0a20 2020 2020  n_name": {.     
-00004b10: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00004b20: 7479 7065 223a 2022 7374 7222 2c0a 2020  type": "str",.  
-00004b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b40: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-00004b50: 2022 5468 6520 6e61 6d65 206f 6620 7468   "The name of th
-00004b60: 6520 7265 6769 6f6e 2074 6865 2070 6c61  e region the pla
-00004b70: 7965 7220 6c65 6674 220a 2020 2020 2020  yer left".      
-00004b80: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-00004b90: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00004ba0: 2020 7d2c 0a20 2020 2020 2020 2022 6163    },.        "ac
-00004bb0: 7469 7669 7479 5f62 6567 696e 223a 207b  tivity_begin": {
-00004bc0: 0a20 2020 2020 2020 2020 2020 2022 6465  .            "de
-00004bd0: 7363 7269 7074 696f 6e22 3a20 2245 7665  scription": "Eve
-00004be0: 6e74 2077 6865 6e20 7468 6520 706c 6179  nt when the play
-00004bf0: 6572 2062 6567 696e 7320 746f 2065 6e67  er begins to eng
-00004c00: 6167 6520 7769 7468 2061 206d 696e 692d  age with a mini-
-00004c10: 6761 6d65 2e22 2c0a 2020 2020 2020 2020  game.",.        
-00004c20: 2020 2020 2265 7665 6e74 5f64 6174 6122      "event_data"
-00004c30: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-00004c40: 2020 2020 2261 6374 6976 6974 795f 6e61      "activity_na
-00004c50: 6d65 223a 207b 0a20 2020 2020 2020 2020  me": {.         
-00004c60: 2020 2020 2020 2020 2020 2022 7479 7065             "type
-00004c70: 223a 2022 656e 756d 2873 6b75 6173 2c20  ": "enum(skuas, 
-00004c80: 6d61 7469 6e67 5f64 616e 6365 2c20 2e2e  mating_dance, ..
-00004c90: 2e29 222c 0a20 2020 2020 2020 2020 2020  .)",.           
-00004ca0: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
-00004cb0: 7074 696f 6e22 3a20 2254 6865 206e 616d  ption": "The nam
-00004cc0: 6520 6f66 2074 6865 206d 696e 692d 6761  e of the mini-ga
-00004cd0: 6d65 2f61 6374 6976 6974 7920 7769 7468  me/activity with
-00004ce0: 2077 6869 6368 2074 6865 2070 6c61 7965   which the playe
-00004cf0: 7220 6265 6761 6e20 746f 2065 6e67 6167  r began to engag
-00004d00: 6522 0a20 2020 2020 2020 2020 2020 2020  e".             
-00004d10: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
-00004d20: 207d 0a20 2020 2020 2020 207d 2c0a 2020   }.        },.  
-00004d30: 2020 2020 2020 2261 6374 6976 6974 795f        "activity_
-00004d40: 656e 6422 3a20 7b0a 2020 2020 2020 2020  end": {.        
-00004d50: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
-00004d60: 223a 2022 4e4f 5420 5945 5420 444f 4355  ": "NOT YET DOCU
-00004d70: 4d45 4e54 4544 222c 0a20 2020 2020 2020  MENTED",.       
-00004d80: 2020 2020 2022 6576 656e 745f 6461 7461       "event_data
-00004d90: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-00004da0: 2020 2020 2022 6163 7469 7669 7479 5f6e       "activity_n
-00004db0: 616d 6522 3a20 7b0a 2020 2020 2020 2020  ame": {.        
-00004dc0: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
-00004dd0: 6522 3a20 2265 6e75 6d28 736b 7561 732c  e": "enum(skuas,
-00004de0: 206d 6174 696e 675f 6461 6e63 652c 202e   mating_dance, .
-00004df0: 2e2e 2922 2c0a 2020 2020 2020 2020 2020  ..)",.          
-00004e00: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
-00004e10: 6970 7469 6f6e 223a 2022 4e4f 5420 5945  iption": "NOT YE
-00004e20: 5420 444f 4355 4d45 4e54 4544 220a 2020  T DOCUMENTED".  
-00004e30: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
-00004e40: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-00004e50: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00004e60: 2022 676c 6f62 616c 5f74 696d 6572 5f62   "global_timer_b
-00004e70: 6567 696e 223a 207b 0a20 2020 2020 2020  egin": {.       
-00004e80: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
-00004e90: 6e22 3a20 224e 4f54 2059 4554 2044 4f43  n": "NOT YET DOC
-00004ea0: 554d 454e 5445 4422 2c0a 2020 2020 2020  UMENTED",.      
-00004eb0: 2020 2020 2020 2265 7665 6e74 5f64 6174        "event_dat
-00004ec0: 6122 3a20 7b0a 2020 2020 2020 2020 2020  a": {.          
-00004ed0: 2020 2020 2020 2274 696d 655f 7265 6d61        "time_rema
-00004ee0: 696e 696e 6722 3a20 7b0a 2020 2020 2020  ining": {.      
-00004ef0: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-00004f00: 7970 6522 3a20 2269 6e74 222c 0a20 2020  ype": "int",.   
-00004f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f20: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
-00004f30: 2254 6865 206c 6566 7420 6f6e 2074 6865  "The left on the
-00004f40: 2067 6c6f 6261 6c20 7469 6d65 7222 0a20   global timer". 
-00004f50: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00004f60: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
-00004f70: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00004f80: 2020 2267 6c6f 6261 6c5f 7469 6d65 725f    "global_timer_
-00004f90: 7061 7573 6522 3a20 7b0a 2020 2020 2020  pause": {.      
-00004fa0: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
-00004fb0: 6f6e 223a 2022 4e4f 5420 5945 5420 444f  on": "NOT YET DO
-00004fc0: 4355 4d45 4e54 4544 222c 0a20 2020 2020  CUMENTED",.     
-00004fd0: 2020 2020 2020 2022 6576 656e 745f 6461         "event_da
-00004fe0: 7461 223a 207b 0a20 2020 2020 2020 2020  ta": {.         
-00004ff0: 2020 2020 2020 2022 6461 7461 223a 2022         "data": "
-00005000: 4e4f 5420 5945 5420 444f 4355 4d45 4e54  NOT YET DOCUMENT
-00005010: 4544 220a 2020 2020 2020 2020 2020 2020  ED".            
-00005020: 7d0a 2020 2020 2020 2020 7d2c 0a20 2020  }.        },.   
-00005030: 2020 2020 2022 676c 6f62 616c 5f74 696d       "global_tim
-00005040: 6572 5f65 7870 6972 6564 223a 207b 0a20  er_expired": {. 
-00005050: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
-00005060: 7269 7074 696f 6e22 3a20 224e 4f54 2059  ription": "NOT Y
-00005070: 4554 2044 4f43 554d 454e 5445 4422 2c0a  ET DOCUMENTED",.
-00005080: 2020 2020 2020 2020 2020 2020 2265 7665              "eve
-00005090: 6e74 5f64 6174 6122 3a20 7b0a 2020 2020  nt_data": {.    
-000050a0: 2020 2020 2020 2020 2020 2020 2264 6174              "dat
-000050b0: 6122 3a20 224e 4f54 2059 4554 2044 4f43  a": "NOT YET DOC
-000050c0: 554d 454e 5445 4422 0a20 2020 2020 2020  UMENTED".       
-000050d0: 2020 2020 207d 0a20 2020 2020 2020 207d       }.        }
-000050e0: 0a20 2020 207d 2c0a 2020 2020 2264 6574  .    },.    "det
-000050f0: 6563 746f 7273 223a 207b 0a20 2020 2020  ectors": {.     
-00005100: 2020 2022 7065 725f 636f 756e 7422 3a20     "per_count": 
-00005110: 7b0a 2020 2020 2020 2020 2020 2020 2252  {.            "R
-00005120: 6567 696f 6e45 6e74 6572 223a 207b 0a20  egionEnter": {. 
-00005130: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00005140: 7479 7065 223a 2022 5265 6769 6f6e 456e  type": "RegionEn
-00005150: 7465 7222 2c0a 2020 2020 2020 2020 2020  ter",.          
-00005160: 2020 2020 2020 2265 6e61 626c 6564 223a        "enabled":
-00005170: 2074 7275 652c 0a20 2020 2020 2020 2020   true,.         
-00005180: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
-00005190: 696f 6e22 3a20 2254 7269 6767 6572 7320  ion": "Triggers 
-000051a0: 616e 2065 7665 6e74 2077 6865 6e20 6120  an event when a 
-000051b0: 706c 6179 6572 2065 6e74 6572 2061 2072  player enter a r
-000051c0: 6567 696f 6e22 0a20 2020 2020 2020 2020  egion".         
-000051d0: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
-000051e0: 2020 2252 6567 696f 6e45 7869 7422 3a20    "RegionExit": 
-000051f0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00005200: 2020 2274 7970 6522 3a20 2252 6567 696f    "type": "Regio
-00005210: 6e45 7869 7422 2c0a 2020 2020 2020 2020  nExit",.        
-00005220: 2020 2020 2020 2020 2265 6e61 626c 6564          "enabled
-00005230: 223a 2074 7275 652c 0a20 2020 2020 2020  ": true,.       
-00005240: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
-00005250: 7074 696f 6e22 3a20 2254 7269 6767 6572  ption": "Trigger
-00005260: 7320 616e 2065 7665 6e74 2077 6865 6e20  s an event when 
-00005270: 6120 706c 6179 6572 2065 7869 7420 6120  a player exit a 
-00005280: 7265 6769 6f6e 220a 2020 2020 2020 2020  region".        
-00005290: 2020 2020 7d0a 2020 2020 2020 2020 7d2c      }.        },
-000052a0: 0a20 2020 2020 2020 2022 6167 6772 6567  .        "aggreg
-000052b0: 6174 6522 3a20 7b7d 0a20 2020 207d 2c0a  ate": {}.    },.
-000052c0: 2020 2020 2266 6561 7475 7265 7322 3a20      "features": 
-000052d0: 7b0a 2020 2020 2020 2020 2270 6572 5f63  {.        "per_c
-000052e0: 6f75 6e74 223a 207b 0a20 2020 2020 2020  ount": {.       
-000052f0: 2020 2020 2022 5265 6769 6f6e 4475 7261       "RegionDura
-00005300: 7469 6f6e 223a 207b 0a20 2020 2020 2020  tion": {.       
-00005310: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
-00005320: 2022 5265 6769 6f6e 4475 7261 7469 6f6e   "RegionDuration
-00005330: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00005340: 2020 2022 656e 6162 6c65 6422 3a20 7472     "enabled": tr
-00005350: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-00005360: 2020 2020 2263 6f75 6e74 223a 2031 312c      "count": 11,
-00005370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005380: 2022 7072 6566 6978 223a 2022 7265 6769   "prefix": "regi
-00005390: 6f6e 222c 0a20 2020 2020 2020 2020 2020  on",.           
-000053a0: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
-000053b0: 6e22 3a20 2254 6865 2064 7572 6174 696f  n": "The duratio
-000053c0: 6e20 6f66 2074 696d 6520 6120 706c 6179  n of time a play
-000053d0: 6572 2070 6c61 7965 6420 696e 2061 2067  er played in a g
-000053e0: 6976 656e 2072 6567 696f 6e20 6f66 2074  iven region of t
-000053f0: 6865 2067 616d 652e 222c 0a20 2020 2020  he game.",.     
-00005400: 2020 2020 2020 2020 2020 2022 7265 7475             "retu
-00005410: 726e 5f74 7970 6522 3a20 2274 696d 6564  rn_type": "timed
-00005420: 656c 7461 220a 2020 2020 2020 2020 2020  elta".          
-00005430: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
-00005440: 2022 5761 6464 6c65 5065 7252 6567 696f   "WaddlePerRegio
-00005450: 6e22 3a20 7b0a 2020 2020 2020 2020 2020  n": {.          
-00005460: 2020 2020 2020 2274 7970 6522 3a20 2257        "type": "W
-00005470: 6164 646c 6550 6572 5265 6769 6f6e 222c  addlePerRegion",
-00005480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005490: 2022 656e 6162 6c65 6422 3a20 7472 7565   "enabled": true
-000054a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000054b0: 2020 2263 6f75 6e74 223a 2031 312c 0a20    "count": 11,. 
-000054c0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000054d0: 7072 6566 6978 223a 2022 7265 6769 6f6e  prefix": "region
-000054e0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-000054f0: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
-00005500: 3a20 2254 6865 206e 756d 6265 7220 6f66  : "The number of
-00005510: 2074 696d 6573 2061 2070 6c61 7965 7220   times a player 
-00005520: 7761 6464 6c65 6420 696e 2061 2067 6976  waddled in a giv
-00005530: 656e 2072 6567 696f 6e20 6f66 2074 6865  en region of the
-00005540: 2067 616d 652e 222c 0a20 2020 2020 2020   game.",.       
-00005550: 2020 2020 2020 2020 2022 7265 7475 726e           "return
-00005560: 5f74 7970 6522 3a20 2269 6e74 220a 2020  _type": "int".  
-00005570: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-00005580: 2020 2020 7d2c 0a20 2020 2020 2020 2022      },.        "
-00005590: 6167 6772 6567 6174 6522 3a20 7b0a 2020  aggregate": {.  
-000055a0: 2020 2020 2020 2020 2020 2247 617a 6543            "GazeC
-000055b0: 6f75 6e74 223a 207b 0a20 2020 2020 2020  ount": {.       
-000055c0: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
-000055d0: 2022 4761 7a65 436f 756e 7422 2c0a 2020   "GazeCount",.  
-000055e0: 2020 2020 2020 2020 2020 2020 2020 2265                "e
-000055f0: 6e61 626c 6564 223a 2074 7275 652c 0a20  nabled": true,. 
-00005600: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00005610: 6465 7363 7269 7074 696f 6e22 3a20 2254  description": "T
-00005620: 6865 206e 756d 6265 7220 6f66 2074 696d  he number of tim
-00005630: 6573 2061 2070 6c61 7965 7220 7761 6464  es a player wadd
-00005640: 6c65 6420 696e 2061 2067 6976 656e 2072  led in a given r
-00005650: 6567 696f 6e20 6f66 2074 6865 2067 616d  egion of the gam
-00005660: 652e 222c 0a20 2020 2020 2020 2020 2020  e.",.           
-00005670: 2020 2020 2022 7265 7475 726e 5f74 7970       "return_typ
-00005680: 6522 3a20 2269 6e74 220a 2020 2020 2020  e": "int".      
-00005690: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-000056a0: 2020 2020 2022 5069 636b 7570 526f 636b       "PickupRock
-000056b0: 436f 756e 7422 3a20 7b0a 2020 2020 2020  Count": {.      
-000056c0: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
-000056d0: 3a20 2250 6963 6b75 7052 6f63 6b43 6f75  : "PickupRockCou
-000056e0: 6e74 222c 0a20 2020 2020 2020 2020 2020  nt",.           
-000056f0: 2020 2020 2022 656e 6162 6c65 6422 3a20       "enabled": 
-00005700: 7472 7565 2c0a 2020 2020 2020 2020 2020  true,.          
-00005710: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
-00005720: 6f6e 223a 2022 5468 6520 6475 7261 7469  on": "The durati
-00005730: 6f6e 2065 6163 6820 7365 7373 696f 6e20  on each session 
-00005740: 746f 6f6b 2e22 2c0a 2020 2020 2020 2020  took.",.        
-00005750: 2020 2020 2020 2020 2272 6574 7572 6e5f          "return_
-00005760: 7479 7065 223a 2022 696e 7422 0a20 2020  type": "int".   
-00005770: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00005780: 2020 2020 2020 2020 2250 6c61 7965 7257          "PlayerW
-00005790: 6164 646c 6543 6f75 6e74 223a 207b 0a20  addleCount": {. 
-000057a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000057b0: 7479 7065 223a 2022 506c 6179 6572 5761  type": "PlayerWa
-000057c0: 6464 6c65 436f 756e 7422 2c0a 2020 2020  ddleCount",.    
-000057d0: 2020 2020 2020 2020 2020 2020 2265 6e61              "ena
-000057e0: 626c 6564 223a 2074 7275 652c 0a20 2020  bled": true,.   
-000057f0: 2020 2020 2020 2020 2020 2020 2022 6465               "de
-00005800: 7363 7269 7074 696f 6e22 3a20 2254 6865  scription": "The
-00005810: 206e 756d 6265 7220 6f66 2074 696d 6573   number of times
-00005820: 2061 2070 6c61 7965 7220 7761 6464 6c65   a player waddle
-00005830: 642e 222c 0a20 2020 2020 2020 2020 2020  d.",.           
-00005840: 2020 2020 2022 7265 7475 726e 5f74 7970       "return_typ
-00005850: 6522 3a20 2269 6e74 220a 2020 2020 2020  e": "int".      
-00005860: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00005870: 2020 2020 2022 5365 7373 696f 6e44 7572       "SessionDur
-00005880: 6174 696f 6e22 3a20 7b0a 2020 2020 2020  ation": {.      
-00005890: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
-000058a0: 3a20 2253 6573 7369 6f6e 4475 7261 7469  : "SessionDurati
-000058b0: 6f6e 222c 0a20 2020 2020 2020 2020 2020  on",.           
-000058c0: 2020 2020 2022 656e 6162 6c65 6422 3a20       "enabled": 
-000058d0: 7472 7565 2c0a 2020 2020 2020 2020 2020  true,.          
-000058e0: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
-000058f0: 6f6e 223a 2022 5468 6520 6475 7261 7469  on": "The durati
-00005900: 6f6e 2065 6163 6820 7365 7373 696f 6e20  on each session 
-00005910: 746f 6f6b 2e22 2c0a 2020 2020 2020 2020  took.",.        
-00005920: 2020 2020 2020 2020 2272 6574 7572 6e5f          "return_
-00005930: 7479 7065 223a 2022 7469 6d65 6465 6c74  type": "timedelt
-00005940: 6122 0a20 2020 2020 2020 2020 2020 207d  a".            }
-00005950: 2c0a 2020 2020 2020 2020 2020 2020 2247  ,.            "G
-00005960: 617a 6544 7572 6174 696f 6e22 3a20 7b0a  azeDuration": {.
-00005970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005980: 2274 7970 6522 3a20 2247 617a 6544 7572  "type": "GazeDur
-00005990: 6174 696f 6e22 2c0a 2020 2020 2020 2020  ation",.        
-000059a0: 2020 2020 2020 2020 2265 6e61 626c 6564          "enabled
-000059b0: 223a 2074 7275 652c 0a20 2020 2020 2020  ": true,.       
-000059c0: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
-000059d0: 7074 696f 6e22 3a20 2248 6f77 206c 6f6e  ption": "How lon
-000059e0: 6720 6761 7a65 2065 7665 6e74 206c 6173  g gaze event las
-000059f0: 7420 666f 722e 222c 0a20 2020 2020 2020  t for.",.       
-00005a00: 2020 2020 2020 2020 2022 7265 7475 726e           "return
-00005a10: 5f74 7970 6522 3a20 2274 696d 6564 656c  _type": "timedel
-00005a20: 7461 220a 2020 2020 2020 2020 2020 2020  ta".            
-00005a30: 7d2c 0a20 2020 2020 2020 2020 2020 2022  },.            "
-00005a40: 5265 6769 6f6e 456e 7465 7243 6f75 6e74  RegionEnterCount
-00005a50: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-00005a60: 2020 2020 2022 7479 7065 223a 2022 5265       "type": "Re
-00005a70: 6769 6f6e 456e 7465 7243 6f75 6e74 222c  gionEnterCount",
-00005a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005a90: 2022 656e 6162 6c65 6422 3a20 6661 6c73   "enabled": fals
-00005aa0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00005ab0: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
-00005ac0: 3a20 2254 6865 206e 756d 6265 7220 6f66  : "The number of
-00005ad0: 2074 696d 6573 2061 2070 6c61 7965 7220   times a player 
-00005ae0: 656e 7465 7264 2066 6f72 2061 2067 6976  enterd for a giv
-00005af0: 656e 2072 6567 696f 6e20 6f66 2074 6865  en region of the
-00005b00: 2067 616d 652e 222c 0a20 2020 2020 2020   game.",.       
-00005b10: 2020 2020 2020 2020 2022 7265 7475 726e           "return
-00005b20: 5f74 7970 6522 3a20 2269 6e74 220a 2020  _type": "int".  
-00005b30: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-00005b40: 2020 2020 2020 2020 2022 4163 7469 7669           "Activi
-00005b50: 7479 436f 6d70 6c65 7465 6422 3a20 7b0a  tyCompleted": {.
-00005b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b70: 2274 7970 6522 3a20 2241 6374 6976 6974  "type": "Activit
-00005b80: 7943 6f6d 706c 6574 6564 222c 0a20 2020  yCompleted",.   
-00005b90: 2020 2020 2020 2020 2020 2020 2022 656e               "en
-00005ba0: 6162 6c65 6422 3a20 7472 7565 2c0a 2020  abled": true,.  
-00005bb0: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-00005bc0: 6573 6372 6970 7469 6f6e 223a 2022 5468  escription": "Th
-00005bd0: 6520 6163 7469 7669 7469 6573 2063 6f6d  e activities com
-00005be0: 706c 6574 6564 2069 6e20 6120 6769 7665  pleted in a give
-00005bf0: 6e20 7365 7373 696f 6e2e 222c 0a20 2020  n session.",.   
-00005c00: 2020 2020 2020 2020 2020 2020 2022 7265               "re
-00005c10: 7475 726e 5f74 7970 6522 3a20 2269 6e74  turn_type": "int
-00005c20: 220a 2020 2020 2020 2020 2020 2020 7d2c  ".            },
-00005c30: 0a20 2020 2020 2020 2020 2020 2022 4163  .            "Ac
-00005c40: 7469 7669 7479 4475 7261 7469 6f6e 223a  tivityDuration":
-00005c50: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00005c60: 2020 2022 7479 7065 223a 2022 4163 7469     "type": "Acti
-00005c70: 7669 7479 4475 7261 7469 6f6e 222c 0a20  vityDuration",. 
-00005c80: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00005c90: 656e 6162 6c65 6422 3a20 7472 7565 2c0a  enabled": true,.
-00005ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cb0: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
-00005cc0: 486f 7720 6c6f 6e67 2061 6374 6976 6974  How long activit
-00005cd0: 7920 6c61 7374 2066 6f72 2e22 2c0a 2020  y last for.",.  
-00005ce0: 2020 2020 2020 2020 2020 2020 2020 2272                "r
-00005cf0: 6574 7572 6e5f 7479 7065 223a 2022 696e  eturn_type": "in
-00005d00: 7422 0a20 2020 2020 2020 2020 2020 207d  t".            }
-00005d10: 2c0a 2020 2020 2020 2020 2020 2020 2252  ,.            "R
-00005d20: 6567 696f 6e73 456e 636f 756e 7465 7265  egionsEncountere
-00005d30: 6422 3a20 7b0a 2020 2020 2020 2020 2020  d": {.          
-00005d40: 2020 2020 2020 2274 7970 6522 3a20 2252        "type": "R
-00005d50: 6567 696f 6e73 456e 636f 756e 7465 7265  egionsEncountere
-00005d60: 6422 2c0a 2020 2020 2020 2020 2020 2020  d",.            
-00005d70: 2020 2020 2265 6e61 626c 6564 223a 2074      "enabled": t
-00005d80: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-00005d90: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
-00005da0: 6e22 3a20 2254 6865 2072 6567 696f 6e73  n": "The regions
-00005db0: 2065 6e74 6572 6564 2069 6e20 6120 6769   entered in a gi
-00005dc0: 7665 6e20 7365 7373 696f 6e2e 222c 0a20  ven session.",. 
-00005dd0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00005de0: 7265 7475 726e 5f74 7970 6522 3a20 2269  return_type": "i
-00005df0: 6e74 220a 2020 2020 2020 2020 2020 2020  nt".            
-00005e00: 7d0a 2020 2020 2020 2020 7d0a 2020 2020  }.        }.    
-00005e10: 7d2c 0a20 2020 2022 636f 6e66 6967 223a  },.    "config":
-00005e20: 207b 0a20 2020 2020 2020 2022 5355 5050   {.        "SUPP
-00005e30: 4f52 5445 445f 5645 5253 223a 205b 0a20  ORTED_VERS": [. 
-00005e40: 2020 2020 2020 2020 2020 2031 0a20 2020             1.   
-00005e50: 2020 2020 205d 0a20 2020 207d 0a7d            ].    }.}
+00000130: 2c0a 2020 2020 2020 2020 2270 6f73 223a  ,.        "pos":
+00000140: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+00000150: 7479 7065 223a 2022 4c69 7374 5b66 6c6f  type": "List[flo
+00000160: 6174 5d22 2c0a 2020 2020 2020 2020 2020  at]",.          
+00000170: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
+00000180: 2022 5468 6520 6375 7272 656e 7420 706f   "The current po
+00000190: 7369 7469 6f6e 206f 6620 7468 6520 706c  sition of the pl
+000001a0: 6179 6572 2068 6561 6473 6574 2061 7420  ayer headset at 
+000001b0: 7468 6520 6d6f 6d65 6e74 2074 6865 2065  the moment the e
+000001c0: 7665 6e74 206f 6363 7572 7265 642c 2066  vent occurred, f
+000001d0: 6f72 6d61 7474 6564 2061 7320 5b78 2c20  ormatted as [x, 
+000001e0: 792c 207a 5d22 0a20 2020 2020 2020 207d  y, z]".        }
+000001f0: 2c0a 2020 2020 2020 2020 2272 6f74 223a  ,.        "rot":
+00000200: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+00000210: 7479 7065 223a 2022 4c69 7374 5b66 6c6f  type": "List[flo
+00000220: 6174 5d22 2c0a 2020 2020 2020 2020 2020  at]",.          
+00000230: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
+00000240: 2022 5468 6520 6375 7272 656e 7420 6f72   "The current or
+00000250: 6965 6e74 6174 696f 6e20 6f66 2074 6865  ientation of the
+00000260: 2070 6c61 7965 7220 6865 6164 7365 7420   player headset 
+00000270: 6174 2074 6865 206d 6f6d 656e 7420 7468  at the moment th
+00000280: 6520 6576 656e 7420 6f63 6375 7272 6564  e event occurred
+00000290: 2c20 666f 726d 6174 7465 6420 6173 205b  , formatted as [
+000002a0: 782c 2079 2c20 7a2c 2077 5d22 0a20 2020  x, y, z, w]".   
+000002b0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+000002c0: 2268 6173 5f72 6f63 6b22 3a20 7b0a 2020  "has_rock": {.  
+000002d0: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
+000002e0: 3a20 2262 6f6f 6c22 2c0a 2020 2020 2020  : "bool",.      
+000002f0: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
+00000300: 6f6e 223a 2022 5768 6574 6865 7220 7468  on": "Whether th
+00000310: 6520 706c 6179 6572 2077 6173 2068 6f6c  e player was hol
+00000320: 6469 6e67 2061 2072 6f63 6b20 696e 2074  ding a rock in t
+00000330: 6865 6972 2062 6561 6b20 6174 2074 6865  heir beak at the
+00000340: 2074 696d 6520 7468 6520 6576 656e 7420   time the event 
+00000350: 6f63 6375 7272 6564 2e22 0a20 2020 2020  occurred.".     
+00000360: 2020 207d 0a20 2020 207d 2c0a 2020 2020     }.    },.    
+00000370: 2265 7665 6e74 7322 3a20 7b0a 2020 2020  "events": {.    
+00000380: 2020 2020 2273 6573 7369 6f6e 5f73 7461      "session_sta
+00000390: 7274 223a 207b 0a20 2020 2020 2020 2020  rt": {.         
+000003a0: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
+000003b0: 3a20 2257 6865 6e20 7468 6520 6170 7020  : "When the app 
+000003c0: 6973 2073 7461 7274 6564 2061 6e64 2074  is started and t
+000003d0: 6865 2067 616d 6570 6c61 7920 7365 7373  he gameplay sess
+000003e0: 696f 6e20 6973 2061 7373 6967 6e65 6420  ion is assigned 
+000003f0: 6120 7365 7373 696f 6e20 4944 2e20 5468  a session ID. Th
+00000400: 6520 706c 6179 6572 2068 6173 206e 6f74  e player has not
+00000410: 206e 6563 6573 7361 7269 6c79 2062 6567   necessarily beg
+00000420: 756e 2074 6865 2067 616d 6520 6974 7365  un the game itse
+00000430: 6c66 2079 6574 2e22 2c0a 2020 2020 2020  lf yet.",.      
+00000440: 2020 2020 2020 2265 7665 6e74 5f64 6174        "event_dat
+00000450: 6122 3a20 7b0a 2020 2020 2020 2020 2020  a": {.          
+00000460: 2020 2020 2020 2272 616e 646f 6d5f 7365        "random_se
+00000470: 6564 223a 2022 5468 6520 7261 6e64 6f6d  ed": "The random
+00000480: 2073 6565 6420 7573 6564 2066 6f72 2061   seed used for a
+00000490: 6c6c 2072 616e 646f 6d20 6e75 6d62 6572  ll random number
+000004a0: 2f70 6f73 6974 696f 6e2f 726f 7461 7469  /position/rotati
+000004b0: 6f6e 2067 656e 6572 6174 696f 6e20 696e  on generation in
+000004c0: 2074 6865 2067 616d 652e 220a 2020 2020   the game.".    
+000004d0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+000004e0: 2020 7d2c 0a20 2020 2020 2020 2022 6761    },.        "ga
+000004f0: 6d65 5f73 7461 7274 223a 207b 0a20 2020  me_start": {.   
+00000500: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
+00000510: 7074 696f 6e22 3a20 2257 6865 6e20 6120  ption": "When a 
+00000520: 6e65 7720 6761 6d65 2069 7320 7374 6172  new game is star
+00000530: 7465 6422 2c0a 2020 2020 2020 2020 2020  ted",.          
+00000540: 2020 2265 7665 6e74 5f64 6174 6122 3a20    "event_data": 
+00000550: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00000560: 2020 226d 6f64 6522 3a20 7b0a 2020 2020    "mode": {.    
+00000570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000580: 2274 7970 6522 3a20 2265 6e75 6d28 484f  "type": "enum(HO
+00000590: 4d45 5f4d 4f44 452c 202e 2e2e 2922 2c0a  ME_MODE, ...)",.
+000005a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000005b0: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
+000005c0: 223a 2022 5468 6520 6761 6d65 206d 6f64  ": "The game mod
+000005d0: 6520 7468 6174 2074 6865 2070 6c61 7965  e that the playe
+000005e0: 7220 6c61 756e 6368 6564 220a 2020 2020  r launched".    
+000005f0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00000600: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00000610: 2020 2020 7d2c 0a20 2020 2020 2020 2022      },.        "
+00000620: 6f70 656e 5f6d 656e 7522 3a20 7b0a 2020  open_menu": {.  
+00000630: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
+00000640: 6970 7469 6f6e 223a 2022 5768 656e 2074  iption": "When t
+00000650: 6865 2070 6c61 7965 7220 6f70 656e 7320  he player opens 
+00000660: 7468 6520 6761 6d65 206d 656e 7522 2c0a  the game menu",.
+00000670: 2020 2020 2020 2020 2020 2020 2265 7665              "eve
+00000680: 6e74 5f64 6174 6122 3a20 7b7d 0a20 2020  nt_data": {}.   
+00000690: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+000006a0: 2263 6c6f 7365 5f6d 656e 7522 3a20 7b0a  "close_menu": {.
+000006b0: 2020 2020 2020 2020 2020 2020 2264 6573              "des
+000006c0: 6372 6970 7469 6f6e 223a 2022 5768 656e  cription": "When
+000006d0: 2074 6865 2070 6c61 7965 7220 636c 6f73   the player clos
+000006e0: 6573 2074 6865 2067 616d 6520 6d65 6e75  es the game menu
+000006f0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00000700: 6576 656e 745f 6461 7461 223a 207b 7d0a  event_data": {}.
+00000710: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00000720: 2020 2022 7365 6c65 6374 5f6d 656e 755f     "select_menu_
+00000730: 6974 656d 223a 207b 0a20 2020 2020 2020  item": {.       
+00000740: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
+00000750: 6e22 3a20 2257 6865 6e20 7468 6520 706c  n": "When the pl
+00000760: 6179 6572 2063 6c69 636b 7320 616e 6420  ayer clicks and 
+00000770: 6974 656d 2069 6e20 7468 6520 6d65 6e75  item in the menu
+00000780: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00000790: 6576 656e 745f 6461 7461 223a 207b 0a20  event_data": {. 
+000007a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000007b0: 6974 656d 223a 207b 0a20 2020 2020 2020  item": {.       
+000007c0: 2020 2020 2020 2020 2020 2020 2022 7479               "ty
+000007d0: 7065 223a 2022 7374 7222 2c0a 2020 2020  pe": "str",.    
+000007e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007f0: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
+00000800: 5468 6520 6e61 6d65 206f 6620 7468 6520  The name of the 
+00000810: 6d65 6e75 2069 7465 6d20 7468 6520 706c  menu item the pl
+00000820: 6179 6572 2073 656c 6563 7465 6422 0a20  ayer selected". 
+00000830: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+00000840: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
+00000850: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00000860: 2020 2268 6561 6473 6574 5f6f 6e22 3a20    "headset_on": 
+00000870: 7b0a 2020 2020 2020 2020 2020 2020 2264  {.            "d
+00000880: 6573 6372 6970 7469 6f6e 223a 2022 5768  escription": "Wh
+00000890: 656e 2074 6865 2070 6c61 7965 7220 7075  en the player pu
+000008a0: 7473 2074 6865 2068 6561 6473 6574 206f  ts the headset o
+000008b0: 6e2c 2072 6573 756d 696e 6720 7468 6520  n, resuming the 
+000008c0: 6761 6d65 222c 0a20 2020 2020 2020 2020  game",.         
+000008d0: 2020 2022 6576 656e 745f 6461 7461 223a     "event_data":
+000008e0: 207b 7d0a 2020 2020 2020 2020 7d2c 0a20   {}.        },. 
+000008f0: 2020 2020 2020 2022 6865 6164 7365 745f         "headset_
+00000900: 6f66 6622 3a20 7b0a 2020 2020 2020 2020  off": {.        
+00000910: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
+00000920: 223a 2022 5768 656e 2074 6865 2070 6c61  ": "When the pla
+00000930: 7965 7220 7265 6d6f 7665 7320 7468 6520  yer removes the 
+00000940: 6865 6164 7365 7420 6672 6f6d 2074 6865  headset from the
+00000950: 6972 2068 6561 642c 2070 6175 7369 6e67  ir head, pausing
+00000960: 2074 6865 2067 616d 6522 2c0a 2020 2020   the game",.    
+00000970: 2020 2020 2020 2020 2265 7665 6e74 5f64          "event_d
+00000980: 6174 6122 3a20 7b7d 0a20 2020 2020 2020  ata": {}.       
+00000990: 207d 2c0a 2020 2020 2020 2020 2276 6965   },.        "vie
+000009a0: 7770 6f72 745f 6461 7461 223a 207b 0a20  wport_data": {. 
+000009b0: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
+000009c0: 7269 7074 696f 6e22 3a20 2241 6e20 6576  ription": "An ev
+000009d0: 656e 7420 7365 6e74 2061 7070 726f 7869  ent sent approxi
+000009e0: 6d61 7465 6c79 206f 6e63 6520 7065 7220  mately once per 
+000009f0: 7365 636f 6e64 2c20 636f 6e74 6169 6e69  second, containi
+00000a00: 6e67 2074 6865 2069 6e2d 6761 6d65 2070  ng the in-game p
+00000a10: 6f73 6974 696f 6e20 616e 6420 6f72 6965  osition and orie
+00000a20: 6e74 6174 696f 6e20 6f66 2074 6865 2070  ntation of the p
+00000a30: 6c61 7965 7220 6865 6164 7365 7420 666f  layer headset fo
+00000a40: 7220 6561 6368 2066 7261 6d65 2069 6e20  r each frame in 
+00000a50: 7468 6520 7061 7374 2073 6563 6f6e 6422  the past second"
+00000a60: 2c0a 2020 2020 2020 2020 2020 2020 2265  ,.            "e
+00000a70: 7665 6e74 5f64 6174 6122 3a20 7b0a 2020  vent_data": {.  
+00000a80: 2020 2020 2020 2020 2020 2020 2020 2267                "g
+00000a90: 617a 655f 6461 7461 5f70 6163 6b61 6765  aze_data_package
+00000aa0: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+00000ab0: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
+00000ac0: 2022 4c69 7374 5b44 6963 745d 222c 0a20   "List[Dict]",. 
+00000ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ae0: 2020 2022 6465 7461 696c 7322 3a20 7b0a     "details": {.
+00000af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b00: 2020 2020 2020 2020 2270 6f73 223a 2022          "pos": "
+00000b10: 4c69 7374 5b66 6c6f 6174 5d22 2c0a 2020  List[float]",.  
+00000b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b30: 2020 2020 2020 2272 6f74 223a 2022 4c69        "rot": "Li
+00000b40: 7374 5b66 6c6f 6174 5d22 0a20 2020 2020  st[float]".     
+00000b50: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+00000b60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000b70: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
+00000b80: 6f6e 223a 2022 4120 6c69 7374 206f 6620  on": "A list of 
+00000b90: 6469 6374 732c 2077 6865 7265 2065 6163  dicts, where eac
+00000ba0: 6820 6469 6374 2069 7320 6f6e 6520 6672  h dict is one fr
+00000bb0: 616d 6520 6f66 2068 6561 6473 6574 2064  ame of headset d
+00000bc0: 6174 612c 2063 6f6e 7461 696e 696e 6720  ata, containing 
+00000bd0: 6120 706f 7369 7469 6f6e 2061 6e64 2072  a position and r
+00000be0: 6f74 6174 696f 6e20 7665 6374 6f72 2c20  otation vector, 
+00000bf0: 652e 672e 207b 5c22 706f 735c 223a 5b31  e.g. {\"pos\":[1
+00000c00: 2c32 2c33 5d2c 205c 2272 6f74 5c22 3a5b  ,2,3], \"rot\":[
+00000c10: 342c 352c 362c 375d 7d2e 220a 2020 2020  4,5,6,7]}.".    
+00000c20: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00000c30: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00000c40: 2020 2020 7d2c 0a20 2020 2020 2020 2022      },.        "
+00000c50: 6c65 6674 5f68 616e 645f 6461 7461 223a  left_hand_data":
+00000c60: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+00000c70: 6465 7363 7269 7074 696f 6e22 3a20 2241  description": "A
+00000c80: 6e20 6576 656e 7420 7365 6e74 2061 7070  n event sent app
+00000c90: 726f 7869 6d61 7465 6c79 206f 6e63 6520  roximately once 
+00000ca0: 7065 7220 7365 636f 6e64 2c20 636f 6e74  per second, cont
+00000cb0: 6169 6e69 6e67 2074 6865 2069 6e2d 6761  aining the in-ga
+00000cc0: 6d65 2070 6f73 6974 696f 6e20 616e 6420  me position and 
+00000cd0: 6f72 6965 6e74 6174 696f 6e20 6f66 2074  orientation of t
+00000ce0: 6865 2070 6c61 7965 7227 7320 6c65 6674  he player's left
+00000cf0: 2068 616e 6420 666f 7220 6561 6368 2066   hand for each f
+00000d00: 7261 6d65 2069 6e20 7468 6520 7061 7374  rame in the past
+00000d10: 2073 6563 6f6e 6422 2c0a 2020 2020 2020   second",.      
+00000d20: 2020 2020 2020 2265 7665 6e74 5f64 6174        "event_dat
+00000d30: 6122 3a20 7b0a 2020 2020 2020 2020 2020  a": {.          
+00000d40: 2020 2020 2020 226c 6566 745f 6861 6e64        "left_hand
+00000d50: 5f64 6174 615f 7061 636b 6167 6522 3a20  _data_package": 
+00000d60: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00000d70: 2020 2020 2020 2274 7970 6522 3a20 224c        "type": "L
+00000d80: 6973 745b 4469 6374 5d22 2c0a 2020 2020  ist[Dict]",.    
+00000d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000da0: 2264 6574 6169 6c73 223a 207b 0a20 2020  "details": {.   
+00000db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000dc0: 2020 2020 2022 706f 7322 3a20 224c 6973       "pos": "Lis
+00000dd0: 745b 666c 6f61 745d 222c 0a20 2020 2020  t[float]",.     
+00000de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000df0: 2020 2022 726f 7422 3a20 224c 6973 745b     "rot": "List[
+00000e00: 666c 6f61 745d 220a 2020 2020 2020 2020  float]".        
+00000e10: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+00000e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e30: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
+00000e40: 3a20 2241 206c 6973 7420 6f66 2064 6963  : "A list of dic
+00000e50: 7473 2c20 7768 6572 6520 6561 6368 2064  ts, where each d
+00000e60: 6963 7420 6973 206f 6e65 2066 7261 6d65  ict is one frame
+00000e70: 206f 6620 6c65 6674 2d68 616e 6420 6461   of left-hand da
+00000e80: 7461 2c20 636f 6e74 6169 6e69 6e67 2061  ta, containing a
+00000e90: 2070 6f73 6974 696f 6e20 616e 6420 726f   position and ro
+00000ea0: 7461 7469 6f6e 2076 6563 746f 722c 2065  tation vector, e
+00000eb0: 2e67 2e20 7b5c 2270 6f73 5c22 3a5b 312c  .g. {\"pos\":[1,
+00000ec0: 322c 335d 2c20 5c22 726f 745c 223a 5b34  2,3], \"rot\":[4
+00000ed0: 2c35 2c36 2c37 5d7d 2e22 0a20 2020 2020  ,5,6,7]}.".     
+00000ee0: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+00000ef0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00000f00: 2020 207d 2c0a 2020 2020 2020 2020 2272     },.        "r
+00000f10: 6967 6874 5f68 616e 645f 6461 7461 223a  ight_hand_data":
+00000f20: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+00000f30: 6465 7363 7269 7074 696f 6e22 3a20 2241  description": "A
+00000f40: 6e20 6576 656e 7420 7365 6e74 2061 7070  n event sent app
+00000f50: 726f 7869 6d61 7465 6c79 206f 6e63 6520  roximately once 
+00000f60: 7065 7220 7365 636f 6e64 2c20 636f 6e74  per second, cont
+00000f70: 6169 6e69 6e67 2074 6865 2069 6e2d 6761  aining the in-ga
+00000f80: 6d65 2070 6f73 6974 696f 6e20 616e 6420  me position and 
+00000f90: 6f72 6965 6e74 6174 696f 6e20 6f66 2074  orientation of t
+00000fa0: 6865 2070 6c61 7965 7227 7320 7269 6768  he player's righ
+00000fb0: 7420 6861 6e64 2066 6f72 2065 6163 6820  t hand for each 
+00000fc0: 6672 616d 6520 696e 2074 6865 2070 6173  frame in the pas
+00000fd0: 7420 7365 636f 6e64 222c 0a20 2020 2020  t second",.     
+00000fe0: 2020 2020 2020 2022 6576 656e 745f 6461         "event_da
+00000ff0: 7461 223a 207b 0a20 2020 2020 2020 2020  ta": {.         
+00001000: 2020 2020 2020 2022 7269 6768 745f 6861         "right_ha
+00001010: 6e64 5f64 6174 615f 7061 636b 6167 6522  nd_data_package"
+00001020: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00001030: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
+00001040: 224c 6973 745b 4469 6374 5d22 2c0a 2020  "List[Dict]",.  
+00001050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001060: 2020 2264 6574 6169 6c73 223a 207b 0a20    "details": {. 
+00001070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001080: 2020 2020 2020 2022 706f 7322 3a20 224c         "pos": "L
+00001090: 6973 745b 666c 6f61 745d 222c 0a20 2020  ist[float]",.   
+000010a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010b0: 2020 2020 2022 726f 7422 3a20 224c 6973       "rot": "Lis
+000010c0: 745b 666c 6f61 745d 220a 2020 2020 2020  t[float]".      
+000010d0: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
+000010e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000010f0: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
+00001100: 6e22 3a20 2241 206c 6973 7420 6f66 2064  n": "A list of d
+00001110: 6963 7473 2c20 7768 6572 6520 6561 6368  icts, where each
+00001120: 2064 6963 7420 6973 206f 6e65 2066 7261   dict is one fra
+00001130: 6d65 206f 6620 7269 6768 742d 6861 6e64  me of right-hand
+00001140: 2064 6174 612c 2063 6f6e 7461 696e 696e   data, containin
+00001150: 6720 6120 706f 7369 7469 6f6e 2061 6e64  g a position and
+00001160: 2072 6f74 6174 696f 6e20 7665 6374 6f72   rotation vector
+00001170: 2c20 652e 672e 207b 5c22 706f 735c 223a  , e.g. {\"pos\":
+00001180: 5b31 2c32 2c33 5d2c 205c 2272 6f74 5c22  [1,2,3], \"rot\"
+00001190: 3a5b 342c 352c 362c 375d 7d2e 220a 2020  :[4,5,6,7]}.".  
+000011a0: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
+000011b0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+000011c0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+000011d0: 2022 706c 6179 6572 5f77 6164 646c 6522   "player_waddle"
+000011e0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+000011f0: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
+00001200: 5768 656e 2061 2070 6c61 7965 7220 7065  When a player pe
+00001210: 7266 6f72 6d73 2061 2077 6164 646c 6520  rforms a waddle 
+00001220: 6d6f 7665 6d65 6e74 2074 6f20 6d6f 7665  movement to move
+00001230: 2074 6865 6972 2070 656e 6775 696e 2061   their penguin a
+00001240: 7661 7461 7220 666f 7277 6172 6422 2c0a  vatar forward",.
+00001250: 2020 2020 2020 2020 2020 2020 2265 7665              "eve
+00001260: 6e74 5f64 6174 6122 3a20 7b0a 2020 2020  nt_data": {.    
+00001270: 2020 2020 2020 2020 2020 2020 226f 626a              "obj
+00001280: 6563 745f 6964 223a 207b 0a20 2020 2020  ect_id": {.     
+00001290: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000012a0: 7479 7065 223a 2022 7374 7222 2c0a 2020  type": "str",.  
+000012b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012c0: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
+000012d0: 2022 5468 6520 6e61 6d65 206f 662e 2e2e   "The name of...
+000012e0: 2073 6f6d 6520 6f62 6a65 6374 220a 2020   some object".  
+000012f0: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
+00001300: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001310: 2022 706f 735f 6f6c 6422 3a20 7b0a 2020   "pos_old": {.  
+00001320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001330: 2020 2274 7970 6522 3a20 224c 6973 745b    "type": "List[
+00001340: 666c 6f61 745d 222c 0a20 2020 2020 2020  float]",.       
+00001350: 2020 2020 2020 2020 2020 2020 2022 6465               "de
+00001360: 7363 7269 7074 696f 6e22 3a20 2254 6865  scription": "The
+00001370: 2070 7265 7669 6f75 7320 706f 7369 7469   previous positi
+00001380: 6f6e 206f 6620 7468 6520 706c 6179 6572  on of the player
+00001390: 2061 7661 7461 7227 7320 6665 6574 2c20   avatar's feet, 
+000013a0: 696e 205b 782c 2079 2c20 7a5d 2066 6f72  in [x, y, z] for
+000013b0: 6d2c 2069 2e65 2e20 7768 6572 6520 7468  m, i.e. where th
+000013c0: 6520 7761 6464 6c65 2073 7461 7274 6564  e waddle started
+000013d0: 2e22 0a20 2020 2020 2020 2020 2020 2020  .".             
+000013e0: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
+000013f0: 2020 2020 2020 2270 6f73 5f6e 6577 223a        "pos_new":
+00001400: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00001410: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
+00001420: 4c69 7374 5b66 6c6f 6174 5d22 2c0a 2020  List[float]",.  
+00001430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001440: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
+00001450: 2022 5468 6520 7265 7375 6c74 696e 6720   "The resulting 
+00001460: 706f 7369 7469 6f6e 206f 6620 7468 6520  position of the 
+00001470: 706c 6179 6572 2061 7661 7461 7227 7320  player avatar's 
+00001480: 6665 6574 2c20 696e 205b 782c 2079 2c20  feet, in [x, y, 
+00001490: 7a5d 2066 6f72 6d2c 2069 2e65 2e20 7768  z] form, i.e. wh
+000014a0: 6572 6520 7468 6520 7761 6464 6c65 2065  ere the waddle e
+000014b0: 6e64 6564 2e22 0a20 2020 2020 2020 2020  nded.".         
+000014c0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+000014d0: 2020 2020 2020 2020 2020 2273 6f75 7263            "sourc
+000014e0: 6522 3a20 7b0a 2020 2020 2020 2020 2020  e": {.          
+000014f0: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
+00001500: 3a20 2265 6e75 6d28 4255 5454 4f4e 2c20  : "enum(BUTTON, 
+00001510: 5741 4444 4c45 2922 2c0a 2020 2020 2020  WADDLE)",.      
+00001520: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+00001530: 6573 6372 6970 7469 6f6e 223a 2022 496e  escription": "In
+00001540: 6469 6361 746f 7220 666f 7220 7768 6574  dicator for whet
+00001550: 6865 7220 7468 6520 706c 6179 6572 2077  her the player w
+00001560: 6164 646c 6564 2062 7920 7072 6573 7369  addled by pressi
+00001570: 6e67 2061 2062 7574 746f 6e2c 206f 7220  ng a button, or 
+00001580: 6279 206d 616b 696e 6720 7468 6520 2777  by making the 'w
+00001590: 6164 646c 6527 2067 6573 7475 7265 2077  addle' gesture w
+000015a0: 6974 6820 7468 6569 7220 6865 6164 2e22  ith their head."
+000015b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000015c0: 207d 0a20 2020 2020 2020 2020 2020 207d   }.            }
+000015d0: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
+000015e0: 2020 2020 2267 617a 655f 6f62 6a65 6374      "gaze_object
+000015f0: 5f62 6567 696e 223a 207b 0a20 2020 2020  _begin": {.     
+00001600: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
+00001610: 696f 6e22 3a20 2241 6e20 6576 656e 7420  ion": "An event 
+00001620: 7472 6967 6765 7265 6420 7768 656e 2074  triggered when t
+00001630: 6865 2070 6c61 7965 7220 6861 7320 6761  he player has ga
+00001640: 7a65 6420 6174 2061 6e20 6f62 6a65 6374  zed at an object
+00001650: 2066 6f72 2061 7420 6c65 6173 7420 302e   for at least 0.
+00001660: 3235 2073 6563 6f6e 6473 2c20 7768 6572  25 seconds, wher
+00001670: 6520 2767 617a 6564 2061 7427 206d 6561  e 'gazed at' mea
+00001680: 6e73 2074 6865 206f 626a 6563 7420 6973  ns the object is
+00001690: 2074 6865 206e 6561 7265 7374 206f 6e20   the nearest on 
+000016a0: 6120 7261 7963 6173 7420 6672 6f6d 2074  a raycast from t
+000016b0: 6865 2076 6965 7770 6f72 7420 6365 6e74  he viewport cent
+000016c0: 6572 222c 0a20 2020 2020 2020 2020 2020  er",.           
+000016d0: 2022 6576 656e 745f 6461 7461 223a 207b   "event_data": {
+000016e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000016f0: 2022 6f62 6a65 6374 5f69 6422 3a20 7b0a   "object_id": {.
+00001700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001710: 2020 2020 2274 7970 6522 3a20 2273 7472      "type": "str
+00001720: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00001730: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
+00001740: 696f 6e22 3a20 2254 6865 206e 616d 6520  ion": "The name 
+00001750: 6f66 2074 6865 206f 626a 6563 7420 7468  of the object th
+00001760: 6520 706c 6179 6572 2069 7320 6761 7a69  e player is gazi
+00001770: 6e67 2061 7422 0a20 2020 2020 2020 2020  ng at".         
+00001780: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00001790: 2020 2020 207d 0a20 2020 2020 2020 207d       }.        }
+000017a0: 2c0a 2020 2020 2020 2020 2267 617a 655f  ,.        "gaze_
+000017b0: 6f62 6a65 6374 5f65 6e64 223a 207b 0a20  object_end": {. 
+000017c0: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
+000017d0: 7269 7074 696f 6e22 3a20 2241 6e20 6576  ription": "An ev
+000017e0: 656e 7420 7472 6967 6765 7265 6420 7768  ent triggered wh
+000017f0: 656e 2074 6865 2070 6c61 7965 7220 7475  en the player tu
+00001800: 726e 7320 6177 6179 2066 726f 6d20 616e  rns away from an
+00001810: 206f 626a 6563 7420 7468 6579 2764 2067   object they'd g
+00001820: 617a 6564 2061 742c 2073 6f20 7468 6520  azed at, so the 
+00001830: 6f62 6a65 6374 2069 7320 6e6f 206c 6f6e  object is no lon
+00001840: 6765 7220 6e65 6172 6573 7420 6f6e 2061  ger nearest on a
+00001850: 2072 6179 6361 7374 2066 726f 6d20 7468   raycast from th
+00001860: 6520 7669 6577 706f 7274 2063 656e 7465  e viewport cente
+00001870: 722e 204e 6f74 6520 7468 6572 6520 6d61  r. Note there ma
+00001880: 7920 6265 2061 2073 6d61 6c6c 2062 7566  y be a small buf
+00001890: 6665 7220 6172 6f75 6e64 2074 6865 206f  fer around the o
+000018a0: 626a 6563 7420 666f 7220 7468 6520 7261  bject for the ra
+000018b0: 7963 6173 742e 222c 0a20 2020 2020 2020  ycast.",.       
+000018c0: 2020 2020 2022 6576 656e 745f 6461 7461       "event_data
+000018d0: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+000018e0: 2020 2020 2022 6f62 6a65 6374 5f69 6422       "object_id"
+000018f0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00001900: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
+00001910: 2273 7472 222c 0a20 2020 2020 2020 2020  "str",.         
+00001920: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
+00001930: 7269 7074 696f 6e22 3a20 2254 6865 206e  ription": "The n
+00001940: 616d 6520 6f66 2074 6865 206f 626a 6563  ame of the objec
+00001950: 7420 7468 6520 706c 6179 6572 2068 6164  t the player had
+00001960: 2070 7265 7669 6f75 736c 7920 6761 7a65   previously gaze
+00001970: 6420 6174 220a 2020 2020 2020 2020 2020  d at".          
+00001980: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00001990: 2020 2020 7d0a 2020 2020 2020 2020 7d2c      }.        },
+000019a0: 0a20 2020 2020 2020 2022 6275 6262 6c65  .        "bubble
+000019b0: 5f70 6f70 223a 207b 0a20 2020 2020 2020  _pop": {.       
+000019c0: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
+000019d0: 6e22 3a20 2241 6e20 6576 656e 7420 7472  n": "An event tr
+000019e0: 6967 6765 7265 6420 7768 656e 2074 6865  iggered when the
+000019f0: 2070 6c61 7965 7220 706f 7073 2061 2062   player pops a b
+00001a00: 7562 626c 6520 696e 2074 6865 2062 7562  ubble in the bub
+00001a10: 626c 652d 706f 7070 696e 6720 6d69 6e69  ble-popping mini
+00001a20: 2d67 616d 652e 2041 2062 7562 626c 6520  -game. A bubble 
+00001a30: 7368 6f75 6c64 2062 6520 706f 7070 6564  should be popped
+00001a40: 206f 6e20 6120 2762 6561 7427 206f 6620   on a 'beat' of 
+00001a50: 7468 6520 6d75 7369 632c 2062 7574 2063  the music, but c
+00001a60: 616e 2062 6520 706f 7070 6564 2075 7020  an be popped up 
+00001a70: 746f 2030 2e35 2073 6563 6f6e 6473 2062  to 0.5 seconds b
+00001a80: 6566 6f72 6520 6f72 2061 6674 6572 2074  efore or after t
+00001a90: 6865 2027 6265 6174 2e27 222c 0a20 2020  he 'beat.'",.   
+00001aa0: 2020 2020 2020 2020 2022 6576 656e 745f           "event_
+00001ab0: 6461 7461 223a 207b 0a20 2020 2020 2020  data": {.       
+00001ac0: 2020 2020 2020 2020 2022 6f62 6a65 6374           "object
+00001ad0: 5f69 6422 3a20 7b0a 2020 2020 2020 2020  _id": {.        
+00001ae0: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
+00001af0: 6522 3a20 2273 7472 222c 0a20 2020 2020  e": "str",.     
+00001b00: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001b10: 6465 7363 7269 7074 696f 6e22 3a20 2254  description": "T
+00001b20: 6865 206e 616d 6520 6f66 2074 6865 2062  he name of the b
+00001b30: 7562 626c 6520 6f62 6a65 6374 2074 6865  ubble object the
+00001b40: 2070 6c61 7965 7220 706f 7070 6564 220a   player popped".
+00001b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b60: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
+00001b70: 2020 2022 7469 6d69 6e67 5f65 7272 6f72     "timing_error
+00001b80: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+00001b90: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
+00001ba0: 2022 666c 6f61 7422 2c0a 2020 2020 2020   "float",.      
+00001bb0: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+00001bc0: 6573 6372 6970 7469 6f6e 223a 2022 5468  escription": "Th
+00001bd0: 6520 7469 6d69 6e67 2064 6966 6665 7265  e timing differe
+00001be0: 6e63 6520 6265 7477 6565 6e20 7468 6520  nce between the 
+00001bf0: 706f 7020 6576 656e 7420 616e 6420 7468  pop event and th
+00001c00: 6520 6d75 7369 6320 2762 6561 742e 2720  e music 'beat.' 
+00001c10: 5468 6973 2076 616c 7565 2069 7320 696e  This value is in
+00001c20: 2074 6865 2072 616e 6765 205b 2d30 2e35   the range [-0.5
+00001c30: 2c20 302e 355d 2c20 7768 6572 6520 6120  , 0.5], where a 
+00001c40: 6e65 6761 7469 7665 2069 6e64 6963 6174  negative indicat
+00001c50: 6573 2074 6865 2062 7562 626c 6520 7761  es the bubble wa
+00001c60: 7320 706f 7070 6564 2062 6566 6f72 6520  s popped before 
+00001c70: 7468 6520 2762 6561 742c 2720 616e 6420  the 'beat,' and 
+00001c80: 706f 7369 7469 7665 2069 6e64 6963 6174  positive indicat
+00001c90: 6573 2070 6f70 7069 6e67 2061 6674 6572  es popping after
+00001ca0: 2074 6865 2027 6265 6174 2e27 220a 2020   the 'beat.'".  
+00001cb0: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
+00001cc0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00001cd0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00001ce0: 2022 6561 745f 6669 7368 223a 207b 0a20   "eat_fish": {. 
+00001cf0: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
+00001d00: 7269 7074 696f 6e22 3a20 2241 6e20 6576  ription": "An ev
+00001d10: 656e 7420 7472 6967 6765 7265 6420 7768  ent triggered wh
+00001d20: 656e 2074 6865 2070 6c61 7965 7220 6561  en the player ea
+00001d30: 7473 2061 2066 6973 682e 222c 0a20 2020  ts a fish.",.   
+00001d40: 2020 2020 2020 2020 2022 6576 656e 745f           "event_
+00001d50: 6461 7461 223a 207b 0a20 2020 2020 2020  data": {.       
+00001d60: 2020 2020 2020 2020 2022 6f62 6a65 6374           "object
+00001d70: 5f69 6422 3a20 7b0a 2020 2020 2020 2020  _id": {.        
+00001d80: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
+00001d90: 6522 3a20 2273 7472 222c 0a20 2020 2020  e": "str",.     
+00001da0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001db0: 6465 7363 7269 7074 696f 6e22 3a20 2254  description": "T
+00001dc0: 6865 206e 616d 6520 6f66 2074 6865 2066  he name of the f
+00001dd0: 6973 6820 6f62 6a65 6374 2074 6865 2070  ish object the p
+00001de0: 6c61 7965 7220 6174 6522 0a20 2020 2020  layer ate".     
+00001df0: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+00001e00: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00001e10: 2020 207d 2c0a 2020 2020 2020 2020 2266     },.        "f
+00001e20: 6c69 7070 6572 5f62 6173 685f 6e65 7374  lipper_bash_nest
+00001e30: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+00001e40: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
+00001e50: 2241 6e20 6576 656e 7420 7472 6967 6765  "An event trigge
+00001e60: 7265 6420 7768 656e 2074 6865 2070 6c61  red when the pla
+00001e70: 7965 7220 6d61 6b65 7320 6120 666c 6970  yer makes a flip
+00001e80: 7065 722d 6261 7368 696e 6720 6d6f 7665  per-bashing move
+00001e90: 2061 6e64 206d 616b 6573 2063 6f6e 7461   and makes conta
+00001ea0: 6374 2077 6974 6820 6120 6e65 7374 2e22  ct with a nest."
+00001eb0: 2c0a 2020 2020 2020 2020 2020 2020 2265  ,.            "e
+00001ec0: 7665 6e74 5f64 6174 6122 3a20 7b0a 2020  vent_data": {.  
+00001ed0: 2020 2020 2020 2020 2020 2020 2020 226e                "n
+00001ee0: 6573 745f 6964 223a 207b 0a20 2020 2020  est_id": {.     
+00001ef0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001f00: 7479 7065 223a 2022 7374 7222 2c0a 2020  type": "str",.  
+00001f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f20: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
+00001f30: 2022 5468 6520 6e61 6d65 206f 6620 7468   "The name of th
+00001f40: 6520 6e65 7374 206f 626a 6563 7420 7468  e nest object th
+00001f50: 6520 706c 6179 6572 2062 6173 6865 6422  e player bashed"
+00001f60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001f70: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
+00001f80: 2020 2020 226e 6573 745f 706f 7322 3a20      "nest_pos": 
+00001f90: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00001fa0: 2020 2020 2020 2274 7970 6522 3a20 224c        "type": "L
+00001fb0: 6973 745b 666c 6f61 745d 222c 0a20 2020  ist[float]",.   
+00001fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001fd0: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
+00001fe0: 2254 6865 2070 6f73 6974 696f 6e20 6f66  "The position of
+00001ff0: 2074 6865 206e 6573 7420 7468 6520 706c   the nest the pl
+00002000: 6179 6572 2062 6173 6865 6422 0a20 2020  ayer bashed".   
+00002010: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
+00002020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002030: 2268 616e 6422 3a20 7b0a 2020 2020 2020  "hand": {.      
+00002040: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+00002050: 7970 6522 3a20 224c 6973 745b 666c 6f61  ype": "List[floa
+00002060: 745d 222c 0a20 2020 2020 2020 2020 2020  t]",.           
+00002070: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
+00002080: 7074 696f 6e22 3a20 2254 6865 2070 6f73  ption": "The pos
+00002090: 6974 696f 6e20 6f66 2074 6865 206e 6573  ition of the nes
+000020a0: 7420 7468 6520 706c 6179 6572 2062 6173  t the player bas
+000020b0: 6865 6422 0a20 2020 2020 2020 2020 2020  hed".           
+000020c0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+000020d0: 2020 2020 7d0a 2020 2020 2020 2020 7d2c      }.        },
+000020e0: 0a20 2020 2020 2020 2022 666c 6970 7065  .        "flippe
+000020f0: 725f 6261 7368 5f70 656e 6775 696e 223a  r_bash_penguin":
+00002100: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+00002110: 6465 7363 7269 7074 696f 6e22 3a20 2241  description": "A
+00002120: 6e20 6576 656e 7420 7472 6967 6765 7265  n event triggere
+00002130: 6420 7768 656e 2074 6865 2070 6c61 7965  d when the playe
+00002140: 7220 6d61 6b65 7320 6120 666c 6970 7065  r makes a flippe
+00002150: 722d 6261 7368 696e 6720 6d6f 7665 2061  r-bashing move a
+00002160: 6e64 206d 616b 6573 2063 6f6e 7461 6374  nd makes contact
+00002170: 2077 6974 6820 616e 6f74 6865 7220 7065   with another pe
+00002180: 6e67 7569 6e2e 222c 0a20 2020 2020 2020  nguin.",.       
+00002190: 2020 2020 2022 6576 656e 745f 6461 7461       "event_data
+000021a0: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+000021b0: 2020 2020 2022 7065 6e67 7569 6e5f 6964       "penguin_id
+000021c0: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+000021d0: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
+000021e0: 2022 7374 7222 2c0a 2020 2020 2020 2020   "str",.        
+000021f0: 2020 2020 2020 2020 2020 2020 2264 6573              "des
+00002200: 6372 6970 7469 6f6e 223a 2022 5468 6520  cription": "The 
+00002210: 6e61 6d65 206f 6620 7468 6520 7065 6e67  name of the peng
+00002220: 7569 6e20 6f62 6a65 6374 2074 6865 2070  uin object the p
+00002230: 6c61 7965 7220 6261 7368 6564 220a 2020  layer bashed".  
+00002240: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
+00002250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002260: 2022 7065 6e67 7569 6e5f 706f 7322 3a20   "penguin_pos": 
+00002270: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00002280: 2020 2020 2020 2274 7970 6522 3a20 224c        "type": "L
+00002290: 6973 745b 666c 6f61 745d 222c 0a20 2020  ist[float]",.   
+000022a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022b0: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
+000022c0: 2254 6865 2070 6f73 6974 696f 6e20 6f66  "The position of
+000022d0: 2074 6865 206f 7468 6572 2070 656e 6775   the other pengu
+000022e0: 696e 2077 6865 6e20 6974 2067 6f74 2062  in when it got b
+000022f0: 6173 6865 6422 0a20 2020 2020 2020 2020  ashed".         
+00002300: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00002310: 2020 2020 207d 0a20 2020 2020 2020 207d       }.        }
+00002320: 2c0a 2020 2020 2020 2020 2266 6c69 7070  ,.        "flipp
+00002330: 6572 5f62 6173 685f 736b 7561 223a 207b  er_bash_skua": {
+00002340: 0a20 2020 2020 2020 2020 2020 2022 6465  .            "de
+00002350: 7363 7269 7074 696f 6e22 3a20 2241 6e20  scription": "An 
+00002360: 6576 656e 7420 7472 6967 6765 7265 6420  event triggered 
+00002370: 7768 656e 2074 6865 2070 6c61 7965 7220  when the player 
+00002380: 6d61 6b65 7320 6120 666c 6970 7065 722d  makes a flipper-
+00002390: 6261 7368 696e 6720 6d6f 7665 2074 6f20  bashing move to 
+000023a0: 7368 6f6f 2061 2073 6b75 6120 6177 6179  shoo a skua away
+000023b0: 2066 726f 6d20 7468 6569 7220 6e65 7374   from their nest
+000023c0: 2f65 6767 2e22 2c0a 2020 2020 2020 2020  /egg.",.        
+000023d0: 2020 2020 2265 7665 6e74 5f64 6174 6122      "event_data"
+000023e0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+000023f0: 2020 2020 2273 6b75 615f 6964 223a 207b      "skua_id": {
+00002400: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002410: 2020 2020 2022 7479 7065 223a 2022 7374       "type": "st
+00002420: 7222 2c0a 2020 2020 2020 2020 2020 2020  r",.            
+00002430: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
+00002440: 7469 6f6e 223a 2022 5468 6520 6e61 6d65  tion": "The name
+00002450: 206f 6620 7468 6520 736b 7561 206f 626a   of the skua obj
+00002460: 6563 7420 7468 6520 706c 6179 6572 2062  ect the player b
+00002470: 6173 6865 6422 0a20 2020 2020 2020 2020  ashed".         
+00002480: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00002490: 2020 2020 2020 2020 2020 2273 6b75 615f            "skua_
+000024a0: 706f 7322 3a20 7b0a 2020 2020 2020 2020  pos": {.        
+000024b0: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
+000024c0: 6522 3a20 224c 6973 745b 666c 6f61 745d  e": "List[float]
+000024d0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+000024e0: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
+000024f0: 696f 6e22 3a20 2254 6865 2070 6f73 6974  ion": "The posit
+00002500: 696f 6e20 6f66 2068 7420 6573 6b75 6120  ion of ht eskua 
+00002510: 7768 656e 2069 7420 676f 7420 6261 7368  when it got bash
+00002520: 6564 220a 2020 2020 2020 2020 2020 2020  ed".            
+00002530: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
+00002540: 2020 2020 2020 2022 7065 6e67 7569 6e5f         "penguin_
+00002550: 706f 7322 3a20 7b0a 2020 2020 2020 2020  pos": {.        
+00002560: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
+00002570: 6522 3a20 2273 7472 222c 0a20 2020 2020  e": "str",.     
+00002580: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00002590: 6465 7363 7269 7074 696f 6e22 3a20 2254  description": "T
+000025a0: 6865 2070 6f73 6974 696f 6e20 6f66 2074  he position of t
+000025b0: 6865 2070 6c61 7965 7220 7768 656e 2074  he player when t
+000025c0: 6865 7920 736c 6170 7065 6420 7468 6520  hey slapped the 
+000025d0: 736b 7561 2e20 4e4f 5445 203a 2054 6869  skua. NOTE : Thi
+000025e0: 7320 7761 7320 6164 6465 6420 6475 6520  s was added due 
+000025f0: 746f 2061 206d 6973 7461 6b65 2069 6e20  to a mistake in 
+00002600: 7370 6563 6966 6963 6174 696f 6e2c 2061  specification, a
+00002610: 6e64 2069 7320 7265 6475 6e64 616e 7420  nd is redundant 
+00002620: 7769 7468 2074 6865 2070 6f73 6974 696f  with the positio
+00002630: 6e20 656c 656d 656e 7420 696e 2067 616d  n element in gam
+00002640: 655f 7374 6174 652e 220a 2020 2020 2020  e_state.".      
+00002650: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00002660: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00002670: 2020 7d2c 0a20 2020 2020 2020 2022 7069    },.        "pi
+00002680: 636b 7570 5f72 6f63 6b22 3a20 7b0a 2020  ckup_rock": {.  
+00002690: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
+000026a0: 6970 7469 6f6e 223a 2022 416e 2065 7665  iption": "An eve
+000026b0: 6e74 2074 7269 6767 6572 6564 2077 6865  nt triggered whe
+000026c0: 6e20 7468 6520 706c 6179 6572 2070 6963  n the player pic
+000026d0: 6b73 2075 7020 6120 726f 636b 206c 7969  ks up a rock lyi
+000026e0: 6e67 206f 6e20 7468 6520 6772 6f75 6e64  ng on the ground
+000026f0: 2c20 7768 6963 6820 636f 6e74 7269 6275  , which contribu
+00002700: 7465 7320 746f 2074 6865 2062 7569 6c64  tes to the build
+00002710: 696e 6720 6f66 2074 6865 6972 206e 6573  ing of their nes
+00002720: 742e 222c 0a20 2020 2020 2020 2020 2020  t.",.           
+00002730: 2022 6576 656e 745f 6461 7461 223a 207b   "event_data": {
+00002740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002750: 2022 746f 7461 6c5f 7069 636b 6564 5f75   "total_picked_u
+00002760: 7022 3a20 7b0a 2020 2020 2020 2020 2020  p": {.          
+00002770: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
+00002780: 3a20 2269 6e74 222c 0a20 2020 2020 2020  : "int",.       
+00002790: 2020 2020 2020 2020 2020 2020 2022 6465               "de
+000027a0: 7363 7269 7074 696f 6e22 3a20 2254 6865  scription": "The
+000027b0: 2072 756e 6e69 6e67 2074 6f74 616c 206f   running total o
+000027c0: 6620 726f 636b 7320 7468 6520 706c 6179  f rocks the play
+000027d0: 6572 2068 6173 2070 6963 6b65 6420 7570  er has picked up
+000027e0: 2e22 0a20 2020 2020 2020 2020 2020 2020  .".             
+000027f0: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
+00002800: 2020 2020 2020 2270 7822 3a20 7b0a 2020        "px": {.  
+00002810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002820: 2020 2274 7970 6522 3a20 2266 6c6f 6174    "type": "float
+00002830: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00002840: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
+00002850: 696f 6e22 3a20 2254 6865 2078 2d70 6f73  ion": "The x-pos
+00002860: 6974 696f 6e20 6f66 2074 6865 2070 6c61  ition of the pla
+00002870: 7965 7220 7768 656e 2074 6865 2065 7665  yer when the eve
+00002880: 6e74 2068 6170 7065 6e65 6422 0a20 2020  nt happened".   
+00002890: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
+000028a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028b0: 2270 7922 3a20 7b0a 2020 2020 2020 2020  "py": {.        
+000028c0: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
+000028d0: 6522 3a20 2266 6c6f 6174 222c 0a20 2020  e": "float",.   
+000028e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028f0: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
+00002900: 2254 6865 2079 2d70 6f73 6974 696f 6e20  "The y-position 
+00002910: 6f66 2074 6865 2070 6c61 7965 7220 7768  of the player wh
+00002920: 656e 2074 6865 2065 7665 6e74 2068 6170  en the event hap
+00002930: 7065 6e65 6422 0a20 2020 2020 2020 2020  pened".         
+00002940: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00002950: 2020 2020 2020 2020 2020 2270 7a22 3a20            "pz": 
+00002960: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00002970: 2020 2020 2020 2274 7970 6522 3a20 2266        "type": "f
+00002980: 6c6f 6174 222c 0a20 2020 2020 2020 2020  loat",.         
+00002990: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
+000029a0: 7269 7074 696f 6e22 3a20 2254 6865 207a  ription": "The z
+000029b0: 2d70 6f73 6974 696f 6e20 6f66 2074 6865  -position of the
+000029c0: 2070 6c61 7965 7220 7768 656e 2074 6865   player when the
+000029d0: 2065 7665 6e74 2068 6170 7065 6e65 6422   event happened"
+000029e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000029f0: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
+00002a00: 2020 2020 2271 7822 3a20 7b0a 2020 2020      "qx": {.    
+00002a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a20: 2274 7970 6522 3a20 2266 6c6f 6174 222c  "type": "float",
+00002a30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002a40: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
+00002a50: 6e22 3a20 2254 6865 2078 2d63 6f6d 706f  n": "The x-compo
+00002a60: 6e65 6e74 206f 6620 7468 6520 7175 6174  nent of the quat
+00002a70: 6572 6e69 6f6e 2066 6f72 2074 6865 2070  ernion for the p
+00002a80: 6c61 7965 7227 7320 6f72 6965 6e74 6174  layer's orientat
+00002a90: 696f 6e20 7768 656e 2074 6865 2065 7665  ion when the eve
+00002aa0: 6e74 2068 6170 7065 6e65 6422 0a20 2020  nt happened".   
+00002ab0: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
+00002ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ad0: 2271 7922 3a20 7b0a 2020 2020 2020 2020  "qy": {.        
+00002ae0: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
+00002af0: 6522 3a20 2266 6c6f 6174 222c 0a20 2020  e": "float",.   
+00002b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b10: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
+00002b20: 2254 6865 2079 2d63 6f6d 706f 6e65 6e74  "The y-component
+00002b30: 206f 6620 7468 6520 7175 6174 6572 6e69   of the quaterni
+00002b40: 6f6e 2066 6f72 2074 6865 2070 6c61 7965  on for the playe
+00002b50: 7227 7320 6f72 6965 6e74 6174 696f 6e20  r's orientation 
+00002b60: 7768 656e 2074 6865 2065 7665 6e74 2068  when the event h
+00002b70: 6170 7065 6e65 6422 0a20 2020 2020 2020  appened".       
+00002b80: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+00002b90: 2020 2020 2020 2020 2020 2020 2271 7a22              "qz"
+00002ba0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00002bb0: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
+00002bc0: 2266 6c6f 6174 222c 0a20 2020 2020 2020  "float",.       
+00002bd0: 2020 2020 2020 2020 2020 2020 2022 6465               "de
+00002be0: 7363 7269 7074 696f 6e22 3a20 2254 6865  scription": "The
+00002bf0: 207a 2d63 6f6d 706f 6e65 6e74 206f 6620   z-component of 
+00002c00: 7468 6520 7175 6174 6572 6e69 6f6e 2066  the quaternion f
+00002c10: 6f72 2074 6865 2070 6c61 7965 7227 7320  or the player's 
+00002c20: 6f72 6965 6e74 6174 696f 6e20 7768 656e  orientation when
+00002c30: 2074 6865 2065 7665 6e74 2068 6170 7065   the event happe
+00002c40: 6e65 6422 0a20 2020 2020 2020 2020 2020  ned".           
+00002c50: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00002c60: 2020 2020 2020 2020 2271 7722 3a20 7b0a          "qw": {.
+00002c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c80: 2020 2020 2274 7970 6522 3a20 2266 6c6f      "type": "flo
+00002c90: 6174 222c 0a20 2020 2020 2020 2020 2020  at",.           
+00002ca0: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
+00002cb0: 7074 696f 6e22 3a20 2254 6865 2077 2d63  ption": "The w-c
+00002cc0: 6f6d 706f 6e65 6e74 206f 6620 7468 6520  omponent of the 
+00002cd0: 7175 6174 6572 6e69 6f6e 2066 6f72 2074  quaternion for t
+00002ce0: 6865 2070 6c61 7965 7227 7320 6f72 6965  he player's orie
+00002cf0: 6e74 6174 696f 6e20 7768 656e 2074 6865  ntation when the
+00002d00: 2065 7665 6e74 2068 6170 7065 6e65 6422   event happened"
+00002d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002d20: 207d 0a20 2020 2020 2020 2020 2020 207d   }.            }
+00002d30: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
+00002d40: 2020 2020 2270 7573 685f 736e 6f77 6261      "push_snowba
+00002d50: 6c6c 223a 207b 0a20 2020 2020 2020 2020  ll": {.         
+00002d60: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
+00002d70: 3a20 2241 6e20 6576 656e 7420 7472 6967  : "An event trig
+00002d80: 6765 7265 6420 7768 656e 2074 6865 2070  gered when the p
+00002d90: 6c61 7965 7220 7075 7368 6573 2061 2073  layer pushes a s
+00002da0: 6e6f 7762 616c 6c20 646f 776e 2074 6865  nowball down the
+00002db0: 2068 696c 6c2e 222c 0a20 2020 2020 2020   hill.",.       
+00002dc0: 2020 2020 2022 6576 656e 745f 6461 7461       "event_data
+00002dd0: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+00002de0: 2020 2020 2022 6f62 6a65 6374 5f69 6422       "object_id"
+00002df0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00002e00: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
+00002e10: 2273 7472 222c 0a20 2020 2020 2020 2020  "str",.         
+00002e20: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
+00002e30: 7269 7074 696f 6e22 3a20 2254 6865 206e  ription": "The n
+00002e40: 616d 6520 6f66 2074 6865 2073 6e6f 7762  ame of the snowb
+00002e50: 616c 6c20 6f62 6a65 6374 2074 6865 2070  all object the p
+00002e60: 6c61 7965 7220 7075 7368 6564 220a 2020  layer pushed".  
+00002e70: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
+00002e80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002e90: 2022 7078 223a 207b 0a20 2020 2020 2020   "px": {.       
+00002ea0: 2020 2020 2020 2020 2020 2020 2022 7479               "ty
+00002eb0: 7065 223a 2022 666c 6f61 7422 2c0a 2020  pe": "float",.  
+00002ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ed0: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
+00002ee0: 2022 5468 6520 782d 706f 7369 7469 6f6e   "The x-position
+00002ef0: 206f 6620 7468 6520 706c 6179 6572 2077   of the player w
+00002f00: 6865 6e20 7468 6520 6576 656e 7420 6861  hen the event ha
+00002f10: 7070 656e 6564 220a 2020 2020 2020 2020  ppened".        
+00002f20: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00002f30: 2020 2020 2020 2020 2020 2022 7079 223a             "py":
+00002f40: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00002f50: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
+00002f60: 666c 6f61 7422 2c0a 2020 2020 2020 2020  float",.        
+00002f70: 2020 2020 2020 2020 2020 2020 2264 6573              "des
+00002f80: 6372 6970 7469 6f6e 223a 2022 5468 6520  cription": "The 
+00002f90: 792d 706f 7369 7469 6f6e 206f 6620 7468  y-position of th
+00002fa0: 6520 706c 6179 6572 2077 6865 6e20 7468  e player when th
+00002fb0: 6520 6576 656e 7420 6861 7070 656e 6564  e event happened
+00002fc0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00002fd0: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
+00002fe0: 2020 2020 2022 707a 223a 207b 0a20 2020       "pz": {.   
+00002ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003000: 2022 7479 7065 223a 2022 666c 6f61 7422   "type": "float"
+00003010: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00003020: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
+00003030: 6f6e 223a 2022 5468 6520 7a2d 706f 7369  on": "The z-posi
+00003040: 7469 6f6e 206f 6620 7468 6520 706c 6179  tion of the play
+00003050: 6572 2077 6865 6e20 7468 6520 6576 656e  er when the even
+00003060: 7420 6861 7070 656e 6564 220a 2020 2020  t happened".    
+00003070: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+00003080: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00003090: 7178 223a 207b 0a20 2020 2020 2020 2020  qx": {.         
+000030a0: 2020 2020 2020 2020 2020 2022 7479 7065             "type
+000030b0: 223a 2022 666c 6f61 7422 2c0a 2020 2020  ": "float",.    
+000030c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030d0: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
+000030e0: 5468 6520 782d 636f 6d70 6f6e 656e 7420  The x-component 
+000030f0: 6f66 2074 6865 2071 7561 7465 726e 696f  of the quaternio
+00003100: 6e20 666f 7220 7468 6520 706c 6179 6572  n for the player
+00003110: 2773 206f 7269 656e 7461 7469 6f6e 2077  's orientation w
+00003120: 6865 6e20 7468 6520 6576 656e 7420 6861  hen the event ha
+00003130: 7070 656e 6564 220a 2020 2020 2020 2020  ppened".        
+00003140: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00003150: 2020 2020 2020 2020 2020 2022 7179 223a             "qy":
+00003160: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00003170: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
+00003180: 666c 6f61 7422 2c0a 2020 2020 2020 2020  float",.        
+00003190: 2020 2020 2020 2020 2020 2020 2264 6573              "des
+000031a0: 6372 6970 7469 6f6e 223a 2022 5468 6520  cription": "The 
+000031b0: 792d 636f 6d70 6f6e 656e 7420 6f66 2074  y-component of t
+000031c0: 6865 2071 7561 7465 726e 696f 6e20 666f  he quaternion fo
+000031d0: 7220 7468 6520 706c 6179 6572 2773 206f  r the player's o
+000031e0: 7269 656e 7461 7469 6f6e 2077 6865 6e20  rientation when 
+000031f0: 7468 6520 6576 656e 7420 6861 7070 656e  the event happen
+00003200: 6564 220a 2020 2020 2020 2020 2020 2020  ed".            
+00003210: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
+00003220: 2020 2020 2020 2022 717a 223a 207b 0a20         "qz": {. 
+00003230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003240: 2020 2022 7479 7065 223a 2022 666c 6f61     "type": "floa
+00003250: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
+00003260: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
+00003270: 7469 6f6e 223a 2022 5468 6520 7a2d 636f  tion": "The z-co
+00003280: 6d70 6f6e 656e 7420 6f66 2074 6865 2071  mponent of the q
+00003290: 7561 7465 726e 696f 6e20 666f 7220 7468  uaternion for th
+000032a0: 6520 706c 6179 6572 2773 206f 7269 656e  e player's orien
+000032b0: 7461 7469 6f6e 2077 6865 6e20 7468 6520  tation when the 
+000032c0: 6576 656e 7420 6861 7070 656e 6564 220a  event happened".
+000032d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000032e0: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
+000032f0: 2020 2022 7177 223a 207b 0a20 2020 2020     "qw": {.     
+00003300: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00003310: 7479 7065 223a 2022 666c 6f61 7422 2c0a  type": "float",.
+00003320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003330: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
+00003340: 223a 2022 5468 6520 772d 636f 6d70 6f6e  ": "The w-compon
+00003350: 656e 7420 6f66 2074 6865 2071 7561 7465  ent of the quate
+00003360: 726e 696f 6e20 666f 7220 7468 6520 706c  rnion for the pl
+00003370: 6179 6572 2773 206f 7269 656e 7461 7469  ayer's orientati
+00003380: 6f6e 2077 6865 6e20 7468 6520 6576 656e  on when the even
+00003390: 7420 6861 7070 656e 6564 220a 2020 2020  t happened".    
+000033a0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+000033b0: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+000033c0: 2020 2020 7d2c 0a20 2020 2020 2020 2022      },.        "
+000033d0: 7269 6e67 5f63 6869 6d65 223a 207b 0a20  ring_chime": {. 
+000033e0: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
+000033f0: 7269 7074 696f 6e22 3a20 2241 6e20 6576  ription": "An ev
+00003400: 656e 7420 7768 656e 2074 6865 2070 6c61  ent when the pla
+00003410: 7965 7220 7269 6e67 7320 6f6e 6520 6f66  yer rings one of
+00003420: 2074 6865 2063 6869 6d65 7320 696e 2074   the chimes in t
+00003430: 6865 2063 6869 6d65 206d 696e 692d 6761  he chime mini-ga
+00003440: 6d65 2e22 2c0a 2020 2020 2020 2020 2020  me.",.          
+00003450: 2020 2265 7665 6e74 5f64 6174 6122 3a20    "event_data": 
+00003460: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00003470: 2020 226e 6f74 655f 706c 6179 6564 223a    "note_played":
+00003480: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00003490: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
+000034a0: 7374 7222 2c0a 2020 2020 2020 2020 2020  str",.          
+000034b0: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
+000034c0: 6970 7469 6f6e 223a 2022 5468 6520 6e61  iption": "The na
+000034d0: 6d65 206f 6620 7468 6520 6368 696d 6520  me of the chime 
+000034e0: 7468 6520 706c 6179 6572 2072 616e 6722  the player rang"
+000034f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003500: 207d 0a20 2020 2020 2020 2020 2020 207d   }.            }
+00003510: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
+00003520: 2020 2020 2262 7562 626c 655f 6170 7065      "bubble_appe
+00003530: 6172 6564 223a 207b 0a20 2020 2020 2020  ared": {.       
+00003540: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
+00003550: 6e22 3a20 2245 7665 6e74 2077 6865 6e20  n": "Event when 
+00003560: 6120 6e65 7720 6275 6262 6c65 2061 7070  a new bubble app
+00003570: 6561 7273 2069 6e20 7468 6520 6d61 7469  ears in the mati
+00003580: 6e67 2064 616e 6365 206d 696e 6967 616d  ng dance minigam
+00003590: 652e 222c 0a20 2020 2020 2020 2020 2020  e.",.           
+000035a0: 2022 6576 656e 745f 6461 7461 223a 207b   "event_data": {
+000035b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000035c0: 2022 6f62 6a65 6374 5f69 6422 3a20 7b0a   "object_id": {.
+000035d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000035e0: 2020 2020 2274 7970 6522 3a20 2273 7472      "type": "str
+000035f0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00003600: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
+00003610: 696f 6e22 3a20 2254 6865 206e 616d 6520  ion": "The name 
+00003620: 6f66 2074 6865 2062 7562 626c 6520 6f62  of the bubble ob
+00003630: 6a65 6374 2074 6861 7420 6170 7065 6172  ject that appear
+00003640: 6564 220a 2020 2020 2020 2020 2020 2020  ed".            
+00003650: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
+00003660: 2020 2020 2020 2022 706f 7358 223a 207b         "posX": {
+00003670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003680: 2020 2020 2022 7479 7065 223a 2022 666c       "type": "fl
+00003690: 6f61 7422 2c0a 2020 2020 2020 2020 2020  oat",.          
+000036a0: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
+000036b0: 6970 7469 6f6e 223a 2022 5468 6520 782d  iption": "The x-
+000036c0: 706f 7369 7469 6f6e 206f 6620 7468 6520  position of the 
+000036d0: 6275 6262 6c65 2074 6861 7420 6170 7065  bubble that appe
+000036e0: 6172 6564 220a 2020 2020 2020 2020 2020  ared".          
+000036f0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00003700: 2020 2020 2020 2020 2022 706f 7359 223a           "posY":
+00003710: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00003720: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
+00003730: 666c 6f61 7422 2c0a 2020 2020 2020 2020  float",.        
+00003740: 2020 2020 2020 2020 2020 2020 2264 6573              "des
+00003750: 6372 6970 7469 6f6e 223a 2022 5468 6520  cription": "The 
+00003760: 792d 706f 7369 7469 6f6e 206f 6620 7468  y-position of th
+00003770: 6520 6275 6262 6c65 2074 6861 7420 6170  e bubble that ap
+00003780: 7065 6172 6564 220a 2020 2020 2020 2020  peared".        
+00003790: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+000037a0: 2020 2020 2020 2020 2020 2022 706f 735a             "posZ
+000037b0: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+000037c0: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
+000037d0: 2022 666c 6f61 7422 2c0a 2020 2020 2020   "float",.      
+000037e0: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+000037f0: 6573 6372 6970 7469 6f6e 223a 2022 5468  escription": "Th
+00003800: 6520 7a2d 706f 7369 7469 6f6e 206f 6620  e z-position of 
+00003810: 7468 6520 6275 6262 6c65 2074 6861 7420  the bubble that 
+00003820: 6170 7065 6172 6564 220a 2020 2020 2020  appeared".      
+00003830: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00003840: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00003850: 2020 7d2c 0a20 2020 2020 2020 2022 6275    },.        "bu
+00003860: 6262 6c65 5f65 7870 6972 6564 223a 207b  bble_expired": {
+00003870: 0a20 2020 2020 2020 2020 2020 2022 6465  .            "de
+00003880: 7363 7269 7074 696f 6e22 3a20 2245 7665  scription": "Eve
+00003890: 6e74 2077 6865 6e20 6120 6275 6262 6c65  nt when a bubble
+000038a0: 2773 2070 6f70 2d61 626c 6520 7469 6d65  's pop-able time
+000038b0: 2065 6e64 7320 616e 6420 7468 6520 6275   ends and the bu
+000038c0: 6262 6c65 2064 6973 6170 7065 6172 732e  bble disappears.
+000038d0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+000038e0: 6576 656e 745f 6461 7461 223a 207b 0a20  event_data": {. 
+000038f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00003900: 6f62 6a65 6374 5f69 6422 3a20 7b0a 2020  object_id": {.  
+00003910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003920: 2020 2274 7970 6522 3a20 2273 7472 222c    "type": "str",
+00003930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003940: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
+00003950: 6e22 3a20 2254 6865 206e 616d 6520 6f66  n": "The name of
+00003960: 2074 6865 2062 7562 626c 6520 6f62 6a65   the bubble obje
+00003970: 6374 2074 6861 7420 6469 7361 7070 6561  ct that disappea
+00003980: 7265 6422 0a20 2020 2020 2020 2020 2020  red".           
+00003990: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
+000039a0: 2020 207d 0a20 2020 2020 2020 207d 2c0a     }.        },.
+000039b0: 2020 2020 2020 2020 2265 6767 5f68 6174          "egg_hat
+000039c0: 6368 5f69 6e64 6963 6174 6f72 5f75 7064  ch_indicator_upd
+000039d0: 6174 6564 223a 207b 0a20 2020 2020 2020  ated": {.       
+000039e0: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
+000039f0: 6e22 3a20 224e 4f54 2059 4554 2044 4f43  n": "NOT YET DOC
+00003a00: 554d 454e 5445 4422 2c0a 2020 2020 2020  UMENTED",.      
+00003a10: 2020 2020 2020 2265 7665 6e74 5f64 6174        "event_dat
+00003a20: 6122 3a20 7b0a 2020 2020 2020 2020 2020  a": {.          
+00003a30: 2020 2020 2020 2274 696d 655f 7265 6d61        "time_rema
+00003a40: 696e 696e 6722 3a20 7b0a 2020 2020 2020  ining": {.      
+00003a50: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+00003a60: 7970 6522 3a20 2269 6e74 222c 0a20 2020  ype": "int",.   
+00003a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a80: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
+00003a90: 2254 6865 2074 696d 6520 6c65 6674 2075  "The time left u
+00003aa0: 6e74 696c 2074 6865 2065 6767 2077 696c  ntil the egg wil
+00003ab0: 6c20 6861 7463 6822 0a20 2020 2020 2020  l hatch".       
+00003ac0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00003ad0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00003ae0: 207d 2c0a 2020 2020 2020 2020 2265 6767   },.        "egg
+00003af0: 5f68 6174 6368 6564 223a 207b 0a20 2020  _hatched": {.   
+00003b00: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
+00003b10: 7074 696f 6e22 3a20 2245 7665 6e74 2077  ption": "Event w
+00003b20: 6865 6e20 7468 6520 6567 6720 6861 7463  hen the egg hatc
+00003b30: 6865 7322 2c0a 2020 2020 2020 2020 2020  hes",.          
+00003b40: 2020 2265 7665 6e74 5f64 6174 6122 3a20    "event_data": 
+00003b50: 7b7d 0a20 2020 2020 2020 207d 2c0a 2020  {}.        },.  
+00003b60: 2020 2020 2020 2265 6767 5f6c 6f73 7422        "egg_lost"
+00003b70: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00003b80: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
+00003b90: 4576 656e 7420 7768 656e 2074 6865 2070  Event when the p
+00003ba0: 6c61 7965 7227 7320 6567 6720 6973 2073  layer's egg is s
+00003bb0: 746f 6c65 6e20 6279 2061 2073 6b75 612e  tolen by a skua.
+00003bc0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00003bd0: 6576 656e 745f 6461 7461 223a 207b 0a20  event_data": {. 
+00003be0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00003bf0: 6f62 6a65 6374 5f69 6422 3a20 7b0a 2020  object_id": {.  
+00003c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c10: 2020 2274 7970 6522 3a20 2273 7472 222c    "type": "str",
+00003c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003c30: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
+00003c40: 6e22 3a20 2254 6865 206e 616d 6520 6f66  n": "The name of
+00003c50: 2074 6865 2073 6b75 6120 7468 6174 2073   the skua that s
+00003c60: 746f 6c65 2074 6865 2065 6767 220a 2020  tole the egg".  
+00003c70: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
+00003c80: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00003c90: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00003ca0: 2022 6567 675f 7265 636f 7665 7265 6422   "egg_recovered"
+00003cb0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00003cc0: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
+00003cd0: 4576 656e 7420 7768 656e 2074 6865 2070  Event when the p
+00003ce0: 6c61 7965 7220 7265 636f 7665 7273 2074  layer recovers t
+00003cf0: 6865 2065 6767 2066 726f 6d20 7468 6520  he egg from the 
+00003d00: 736b 7561 732e 222c 0a20 2020 2020 2020  skuas.",.       
+00003d10: 2020 2020 2022 6576 656e 745f 6461 7461       "event_data
+00003d20: 223a 207b 7d0a 2020 2020 2020 2020 7d2c  ": {}.        },
+00003d30: 0a20 2020 2020 2020 2022 6d61 7469 6e67  .        "mating
+00003d40: 5f64 616e 6365 5f69 6e64 6963 6174 6f72  _dance_indicator
+00003d50: 5f75 7064 6174 6564 223a 207b 0a20 2020  _updated": {.   
+00003d60: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
+00003d70: 7074 696f 6e22 3a20 2245 7665 6e74 2077  ption": "Event w
+00003d80: 6865 6e20 6120 6275 6262 6c65 2069 7320  hen a bubble is 
+00003d90: 706f 7070 6564 2061 6e64 2074 6865 2069  popped and the i
+00003da0: 6e64 6963 6174 6f72 2066 6f72 2070 726f  ndicator for pro
+00003db0: 6772 6573 7320 746f 2063 6f6d 706c 6574  gress to complet
+00003dc0: 696f 6e20 6f66 2074 6865 206d 6174 696e  ion of the matin
+00003dd0: 6720 6461 6e63 6520 7570 6461 7465 732e  g dance updates.
+00003de0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00003df0: 6576 656e 745f 6461 7461 223a 207b 0a20  event_data": {. 
+00003e00: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00003e10: 7065 7263 656e 745f 6675 6c6c 223a 207b  percent_full": {
+00003e20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003e30: 2020 2020 2022 7479 7065 223a 2022 696e       "type": "in
+00003e40: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
+00003e50: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
+00003e60: 7469 6f6e 223a 2022 5468 6520 6e65 7720  tion": "The new 
+00003e70: 7065 7263 656e 7420 746f 2077 6869 6368  percent to which
+00003e80: 2074 6865 2064 616e 6365 2063 6f6d 706c   the dance compl
+00003e90: 6574 696f 6e20 696e 6469 6361 746f 7220  etion indicator 
+00003ea0: 6973 2066 696c 6c65 6422 0a20 2020 2020  is filled".     
+00003eb0: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+00003ec0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00003ed0: 2020 207d 2c0a 2020 2020 2020 2020 226e     },.        "n
+00003ee0: 6573 745f 636f 6d70 6c65 7465 223a 207b  est_complete": {
+00003ef0: 0a20 2020 2020 2020 2020 2020 2022 6465  .            "de
+00003f00: 7363 7269 7074 696f 6e22 3a20 2245 7665  scription": "Eve
+00003f10: 6e74 2077 6865 6e20 7468 6520 706c 6179  nt when the play
+00003f20: 6572 2063 6f6d 706c 6574 6573 2074 6865  er completes the
+00003f30: 2062 7569 6c64 696e 6720 6f66 2074 6865   building of the
+00003f40: 6972 206e 6573 742e 222c 0a20 2020 2020  ir nest.",.     
+00003f50: 2020 2020 2020 2022 6576 656e 745f 6461         "event_da
+00003f60: 7461 223a 207b 7d0a 2020 2020 2020 2020  ta": {}.        
+00003f70: 7d2c 0a20 2020 2020 2020 2022 7065 6e67  },.        "peng
+00003f80: 7569 6e5f 7069 6e5f 6665 6c6c 223a 207b  uin_pin_fell": {
+00003f90: 0a20 2020 2020 2020 2020 2020 2022 6465  .            "de
+00003fa0: 7363 7269 7074 696f 6e22 3a20 2257 6865  scription": "Whe
+00003fb0: 6e20 6f6e 6520 6f66 2074 6865 2070 696e  n one of the pin
+00003fc0: 7320 6665 6c6c 2069 6e20 7468 6520 626f  s fell in the bo
+00003fd0: 776c 696e 6720 6172 6561 2e22 2c0a 2020  wling area.",.  
+00003fe0: 2020 2020 2020 2020 2020 2265 7665 6e74            "event
+00003ff0: 5f64 6174 6122 3a20 7b7d 0a20 2020 2020  _data": {}.     
+00004000: 2020 207d 2c0a 2020 2020 2020 2020 2273     },.        "s
+00004010: 6b75 615f 7370 6177 6e22 3a20 7b0a 2020  kua_spawn": {.  
+00004020: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
+00004030: 6970 7469 6f6e 223a 2022 4576 656e 7420  iption": "Event 
+00004040: 7768 656e 2061 206e 6577 2073 6b75 6120  when a new skua 
+00004050: 6973 2061 6464 6564 2069 6e20 7468 6520  is added in the 
+00004060: 6e65 7374 2f65 6767 2064 6566 656e 7365  nest/egg defense
+00004070: 206d 696e 692d 6761 6d65 2e22 2c0a 2020   mini-game.",.  
+00004080: 2020 2020 2020 2020 2020 2265 7665 6e74            "event
+00004090: 5f64 6174 6122 3a20 7b0a 2020 2020 2020  _data": {.      
+000040a0: 2020 2020 2020 2020 2020 226f 626a 6563            "objec
+000040b0: 745f 6964 223a 207b 0a20 2020 2020 2020  t_id": {.       
+000040c0: 2020 2020 2020 2020 2020 2020 2022 7479               "ty
+000040d0: 7065 223a 2022 7374 7222 2c0a 2020 2020  pe": "str",.    
+000040e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000040f0: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
+00004100: 5468 6520 6e61 6d65 206f 6620 7468 6520  The name of the 
+00004110: 736b 7561 206f 626a 6563 7420 7468 6174  skua object that
+00004120: 2061 7070 6561 7265 6422 0a20 2020 2020   appeared".     
+00004130: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
+00004140: 2020 2020 2020 2020 2020 2020 2020 2270                "p
+00004150: 6f73 5822 3a20 7b0a 2020 2020 2020 2020  osX": {.        
+00004160: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
+00004170: 6522 3a20 2266 6c6f 6174 222c 0a20 2020  e": "float",.   
+00004180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004190: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
+000041a0: 2254 6865 2078 2d70 6f73 6974 696f 6e20  "The x-position 
+000041b0: 6f66 2074 6865 2073 6b75 6120 7468 6174  of the skua that
+000041c0: 2061 7070 6561 7265 6422 0a20 2020 2020   appeared".     
+000041d0: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
+000041e0: 2020 2020 2020 2020 2020 2020 2020 2270                "p
+000041f0: 6f73 5922 3a20 7b0a 2020 2020 2020 2020  osY": {.        
+00004200: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
+00004210: 6522 3a20 2266 6c6f 6174 222c 0a20 2020  e": "float",.   
+00004220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004230: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
+00004240: 2254 6865 2079 2d70 6f73 6974 696f 6e20  "The y-position 
+00004250: 6f66 2074 6865 2073 6b75 6120 7468 6174  of the skua that
+00004260: 2061 7070 6561 7265 6422 0a20 2020 2020   appeared".     
+00004270: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
+00004280: 2020 2020 2020 2020 2020 2020 2020 2270                "p
+00004290: 6f73 5a22 3a20 7b0a 2020 2020 2020 2020  osZ": {.        
+000042a0: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
+000042b0: 6522 3a20 2266 6c6f 6174 222c 0a20 2020  e": "float",.   
+000042c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000042d0: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
+000042e0: 2254 6865 207a 2d70 6f73 6974 696f 6e20  "The z-position 
+000042f0: 6f66 2074 6865 2073 6b75 6120 7468 6174  of the skua that
+00004300: 2061 7070 6561 7265 6422 0a20 2020 2020   appeared".     
+00004310: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+00004320: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00004330: 2020 207d 2c0a 2020 2020 2020 2020 2273     },.        "s
+00004340: 6b75 615f 6d6f 7665 223a 207b 0a20 2020  kua_move": {.   
+00004350: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
+00004360: 7074 696f 6e22 3a20 2245 7665 6e74 2077  ption": "Event w
+00004370: 6865 6e20 6120 736b 7561 206d 6f76 6573  hen a skua moves
+00004380: 2074 6f20 6120 6e65 7720 6c6f 6361 7469   to a new locati
+00004390: 6f6e 2069 6e20 7468 6520 6e65 7374 2f65  on in the nest/e
+000043a0: 6767 2064 6566 656e 7365 206d 696e 692d  gg defense mini-
+000043b0: 6761 6d65 2e22 2c0a 2020 2020 2020 2020  game.",.        
+000043c0: 2020 2020 2265 7665 6e74 5f64 6174 6122      "event_data"
+000043d0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+000043e0: 2020 2020 226f 626a 6563 745f 6964 223a      "object_id":
+000043f0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00004400: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
+00004410: 7374 7222 2c0a 2020 2020 2020 2020 2020  str",.          
+00004420: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
+00004430: 6970 7469 6f6e 223a 2022 5468 6520 6e61  iption": "The na
+00004440: 6d65 206f 6620 7468 6520 736b 7561 206f  me of the skua o
+00004450: 626a 6563 7420 7468 6174 206d 6f76 6564  bject that moved
+00004460: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00004470: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
+00004480: 2020 2020 2022 6672 6f6d 5f70 6f73 6974       "from_posit
+00004490: 696f 6e5f 7822 3a20 7b0a 2020 2020 2020  ion_x": {.      
+000044a0: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+000044b0: 7970 6522 3a20 2266 6c6f 6174 222c 0a20  ype": "float",. 
+000044c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000044d0: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
+000044e0: 3a20 2254 6865 2069 6e69 7469 616c 2078  : "The initial x
+000044f0: 2d70 6f73 6974 696f 6e20 6f66 2074 6865  -position of the
+00004500: 2073 6b75 6120 7468 6174 206d 6f76 6564   skua that moved
+00004510: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00004520: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
+00004530: 2020 2020 2022 6672 6f6d 5f70 6f73 6974       "from_posit
+00004540: 696f 6e5f 7922 3a20 7b0a 2020 2020 2020  ion_y": {.      
+00004550: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+00004560: 7970 6522 3a20 2266 6c6f 6174 222c 0a20  ype": "float",. 
+00004570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004580: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
+00004590: 3a20 2254 6865 2069 6e69 7469 616c 2079  : "The initial y
+000045a0: 2d70 6f73 6974 696f 6e20 6f66 2074 6865  -position of the
+000045b0: 2073 6b75 6120 7468 6174 206d 6f76 6564   skua that moved
+000045c0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+000045d0: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
+000045e0: 2020 2020 2022 6672 6f6d 5f70 6f73 6974       "from_posit
+000045f0: 696f 6e5f 7a22 3a20 7b0a 2020 2020 2020  ion_z": {.      
+00004600: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+00004610: 7970 6522 3a20 2266 6c6f 6174 222c 0a20  ype": "float",. 
+00004620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004630: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
+00004640: 3a20 2254 6865 2069 6e69 7469 616c 207a  : "The initial z
+00004650: 2d70 6f73 6974 696f 6e20 6f66 2074 6865  -position of the
+00004660: 2073 6b75 6120 7468 6174 206d 6f76 6564   skua that moved
+00004670: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00004680: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
+00004690: 2020 2020 2022 746f 5f70 6f73 6974 696f       "to_positio
+000046a0: 6e5f 7822 3a20 7b0a 2020 2020 2020 2020  n_x": {.        
+000046b0: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
+000046c0: 6522 3a20 2266 6c6f 6174 222c 0a20 2020  e": "float",.   
+000046d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046e0: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
+000046f0: 2254 6865 206e 6577 2078 2d70 6f73 6974  "The new x-posit
+00004700: 696f 6e20 6f66 2074 6865 2073 6b75 6120  ion of the skua 
+00004710: 7468 6174 206d 6f76 6564 220a 2020 2020  that moved".    
+00004720: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+00004730: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00004740: 746f 5f70 6f73 6974 696f 6e5f 7922 3a20  to_position_y": 
+00004750: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00004760: 2020 2020 2020 2274 7970 6522 3a20 2266        "type": "f
+00004770: 6c6f 6174 222c 0a20 2020 2020 2020 2020  loat",.         
+00004780: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
+00004790: 7269 7074 696f 6e22 3a20 2254 6865 206e  ription": "The n
+000047a0: 6577 2079 2d70 6f73 6974 696f 6e20 6f66  ew y-position of
+000047b0: 2074 6865 2073 6b75 6120 7468 6174 206d   the skua that m
+000047c0: 6f76 6564 220a 2020 2020 2020 2020 2020  oved".          
+000047d0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+000047e0: 2020 2020 2020 2020 2022 746f 5f70 6f73           "to_pos
+000047f0: 6974 696f 6e5f 7a22 3a20 7b0a 2020 2020  ition_z": {.    
+00004800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004810: 2274 7970 6522 3a20 2266 6c6f 6174 222c  "type": "float",
+00004820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004830: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
+00004840: 6e22 3a20 2254 6865 206e 6577 207a 2d70  n": "The new z-p
+00004850: 6f73 6974 696f 6e20 6f66 2074 6865 2073  osition of the s
+00004860: 6b75 6120 7468 6174 206d 6f76 6564 220a  kua that moved".
+00004870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004880: 7d0a 2020 2020 2020 2020 2020 2020 7d0a  }.            }.
+00004890: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+000048a0: 2020 2022 656e 7465 725f 7265 6769 6f6e     "enter_region
+000048b0: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+000048c0: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
+000048d0: 2245 7665 6e74 2077 6865 6e20 7468 6520  "Event when the 
+000048e0: 706c 6179 6572 206d 6f76 6573 2069 6e74  player moves int
+000048f0: 6f20 6f6e 6520 6f66 2074 6865 2072 6567  o one of the reg
+00004900: 696f 6e73 2063 6f6e 7461 696e 696e 6720  ions containing 
+00004910: 6120 6d69 6e69 2d67 616d 6520 6f72 206f  a mini-game or o
+00004920: 7468 6572 2066 6561 7475 7265 2e22 2c0a  ther feature.",.
+00004930: 2020 2020 2020 2020 2020 2020 2265 7665              "eve
+00004940: 6e74 5f64 6174 6122 3a20 7b0a 2020 2020  nt_data": {.    
+00004950: 2020 2020 2020 2020 2020 2020 2272 6567              "reg
+00004960: 696f 6e5f 6e61 6d65 223a 207b 0a20 2020  ion_name": {.   
+00004970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004980: 2022 7479 7065 223a 2022 7374 7222 2c0a   "type": "str",.
+00004990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000049a0: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
+000049b0: 223a 2022 5468 6520 6e61 6d65 206f 6620  ": "The name of 
+000049c0: 7468 6520 7265 6769 6f6e 2074 6865 2070  the region the p
+000049d0: 6c61 7965 7220 656e 7465 7265 6422 0a20  layer entered". 
+000049e0: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+000049f0: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
+00004a00: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00004a10: 2020 2265 7869 745f 7265 6769 6f6e 223a    "exit_region":
+00004a20: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+00004a30: 6465 7363 7269 7074 696f 6e22 3a20 2245  description": "E
+00004a40: 7665 6e74 2077 6865 6e20 6120 6d6f 7665  vent when a move
+00004a50: 7320 6f75 7420 6f66 206f 6e65 206f 6620  s out of one of 
+00004a60: 7468 6520 7265 6769 6f6e 7320 636f 6e74  the regions cont
+00004a70: 6169 6e69 6e67 2061 206d 696e 692d 6761  aining a mini-ga
+00004a80: 6d65 206f 7220 6f74 6865 7220 6665 6174  me or other feat
+00004a90: 7572 652e 222c 0a20 2020 2020 2020 2020  ure.",.         
+00004aa0: 2020 2022 6576 656e 745f 6461 7461 223a     "event_data":
+00004ab0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00004ac0: 2020 2022 7265 6769 6f6e 5f6e 616d 6522     "region_name"
+00004ad0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00004ae0: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
+00004af0: 2273 7472 222c 0a20 2020 2020 2020 2020  "str",.         
+00004b00: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
+00004b10: 7269 7074 696f 6e22 3a20 2254 6865 206e  ription": "The n
+00004b20: 616d 6520 6f66 2074 6865 2072 6567 696f  ame of the regio
+00004b30: 6e20 7468 6520 706c 6179 6572 206c 6566  n the player lef
+00004b40: 7422 0a20 2020 2020 2020 2020 2020 2020  t".             
+00004b50: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
+00004b60: 207d 0a20 2020 2020 2020 207d 2c0a 2020   }.        },.  
+00004b70: 2020 2020 2020 2261 6374 6976 6974 795f        "activity_
+00004b80: 6265 6769 6e22 3a20 7b0a 2020 2020 2020  begin": {.      
+00004b90: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
+00004ba0: 6f6e 223a 2022 4576 656e 7420 7768 656e  on": "Event when
+00004bb0: 2074 6865 2070 6c61 7965 7220 6265 6769   the player begi
+00004bc0: 6e73 2074 6f20 656e 6761 6765 2077 6974  ns to engage wit
+00004bd0: 6820 6120 6d69 6e69 2d67 616d 652e 222c  h a mini-game.",
+00004be0: 0a20 2020 2020 2020 2020 2020 2022 6576  .            "ev
+00004bf0: 656e 745f 6461 7461 223a 207b 0a20 2020  ent_data": {.   
+00004c00: 2020 2020 2020 2020 2020 2020 2022 6163               "ac
+00004c10: 7469 7669 7479 5f6e 616d 6522 3a20 7b0a  tivity_name": {.
+00004c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c30: 2020 2020 2274 7970 6522 3a20 2265 6e75      "type": "enu
+00004c40: 6d28 736b 7561 732c 206d 6174 696e 675f  m(skuas, mating_
+00004c50: 6461 6e63 652c 202e 2e2e 2922 2c0a 2020  dance, ...)",.  
+00004c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c70: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
+00004c80: 2022 5468 6520 6e61 6d65 206f 6620 7468   "The name of th
+00004c90: 6520 6d69 6e69 2d67 616d 652f 6163 7469  e mini-game/acti
+00004ca0: 7669 7479 2077 6974 6820 7768 6963 6820  vity with which 
+00004cb0: 7468 6520 706c 6179 6572 2062 6567 616e  the player began
+00004cc0: 2074 6f20 656e 6761 6765 220a 2020 2020   to engage".    
+00004cd0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00004ce0: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00004cf0: 2020 2020 7d2c 0a20 2020 2020 2020 2022      },.        "
+00004d00: 6163 7469 7669 7479 5f65 6e64 223a 207b  activity_end": {
+00004d10: 0a20 2020 2020 2020 2020 2020 2022 6465  .            "de
+00004d20: 7363 7269 7074 696f 6e22 3a20 224e 4f54  scription": "NOT
+00004d30: 2059 4554 2044 4f43 554d 454e 5445 4422   YET DOCUMENTED"
+00004d40: 2c0a 2020 2020 2020 2020 2020 2020 2265  ,.            "e
+00004d50: 7665 6e74 5f64 6174 6122 3a20 7b0a 2020  vent_data": {.  
+00004d60: 2020 2020 2020 2020 2020 2020 2020 2261                "a
+00004d70: 6374 6976 6974 795f 6e61 6d65 223a 207b  ctivity_name": {
+00004d80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004d90: 2020 2020 2022 7479 7065 223a 2022 656e       "type": "en
+00004da0: 756d 2873 6b75 6173 2c20 6d61 7469 6e67  um(skuas, mating
+00004db0: 5f64 616e 6365 2c20 2e2e 2e29 222c 0a20  _dance, ...)",. 
+00004dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004dd0: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
+00004de0: 3a20 224e 4f54 2059 4554 2044 4f43 554d  : "NOT YET DOCUM
+00004df0: 454e 5445 4422 0a20 2020 2020 2020 2020  ENTED".         
+00004e00: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00004e10: 2020 2020 207d 0a20 2020 2020 2020 207d       }.        }
+00004e20: 2c0a 2020 2020 2020 2020 2267 6c6f 6261  ,.        "globa
+00004e30: 6c5f 7469 6d65 725f 6265 6769 6e22 3a20  l_timer_begin": 
+00004e40: 7b0a 2020 2020 2020 2020 2020 2020 2264  {.            "d
+00004e50: 6573 6372 6970 7469 6f6e 223a 2022 4e4f  escription": "NO
+00004e60: 5420 5945 5420 444f 4355 4d45 4e54 4544  T YET DOCUMENTED
+00004e70: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00004e80: 6576 656e 745f 6461 7461 223a 207b 0a20  event_data": {. 
+00004e90: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00004ea0: 7469 6d65 5f72 656d 6169 6e69 6e67 223a  time_remaining":
+00004eb0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00004ec0: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
+00004ed0: 696e 7422 2c0a 2020 2020 2020 2020 2020  int",.          
+00004ee0: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
+00004ef0: 6970 7469 6f6e 223a 2022 5468 6520 6c65  iption": "The le
+00004f00: 6674 206f 6e20 7468 6520 676c 6f62 616c  ft on the global
+00004f10: 2074 696d 6572 220a 2020 2020 2020 2020   timer".        
+00004f20: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00004f30: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00004f40: 7d2c 0a20 2020 2020 2020 2022 676c 6f62  },.        "glob
+00004f50: 616c 5f74 696d 6572 5f70 6175 7365 223a  al_timer_pause":
+00004f60: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+00004f70: 6465 7363 7269 7074 696f 6e22 3a20 224e  description": "N
+00004f80: 4f54 2059 4554 2044 4f43 554d 454e 5445  OT YET DOCUMENTE
+00004f90: 4422 2c0a 2020 2020 2020 2020 2020 2020  D",.            
+00004fa0: 2265 7665 6e74 5f64 6174 6122 3a20 7b0a  "event_data": {.
+00004fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004fc0: 2264 6174 6122 3a20 224e 4f54 2059 4554  "data": "NOT YET
+00004fd0: 2044 4f43 554d 454e 5445 4422 0a20 2020   DOCUMENTED".   
+00004fe0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00004ff0: 2020 207d 2c0a 2020 2020 2020 2020 2267     },.        "g
+00005000: 6c6f 6261 6c5f 7469 6d65 725f 6578 7069  lobal_timer_expi
+00005010: 7265 6422 3a20 7b0a 2020 2020 2020 2020  red": {.        
+00005020: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
+00005030: 223a 2022 4e4f 5420 5945 5420 444f 4355  ": "NOT YET DOCU
+00005040: 4d45 4e54 4544 222c 0a20 2020 2020 2020  MENTED",.       
+00005050: 2020 2020 2022 6576 656e 745f 6461 7461       "event_data
+00005060: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+00005070: 2020 2020 2022 6461 7461 223a 2022 4e4f       "data": "NO
+00005080: 5420 5945 5420 444f 4355 4d45 4e54 4544  T YET DOCUMENTED
+00005090: 220a 2020 2020 2020 2020 2020 2020 7d0a  ".            }.
+000050a0: 2020 2020 2020 2020 7d0a 2020 2020 7d2c          }.    },
+000050b0: 0a20 2020 2022 6465 7465 6374 6f72 7322  .    "detectors"
+000050c0: 3a20 7b0a 2020 2020 2020 2020 2270 6572  : {.        "per
+000050d0: 5f63 6f75 6e74 223a 207b 0a20 2020 2020  _count": {.     
+000050e0: 2020 2020 2020 2022 5265 6769 6f6e 456e         "RegionEn
+000050f0: 7465 7222 3a20 7b0a 2020 2020 2020 2020  ter": {.        
+00005100: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
+00005110: 2252 6567 696f 6e45 6e74 6572 222c 0a20  "RegionEnter",. 
+00005120: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00005130: 656e 6162 6c65 6422 3a20 7472 7565 2c0a  enabled": true,.
+00005140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005150: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
+00005160: 5472 6967 6765 7273 2061 6e20 6576 656e  Triggers an even
+00005170: 7420 7768 656e 2061 2070 6c61 7965 7220  t when a player 
+00005180: 656e 7465 7220 6120 7265 6769 6f6e 220a  enter a region".
+00005190: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+000051a0: 2020 2020 2020 2020 2020 2022 5265 6769             "Regi
+000051b0: 6f6e 4578 6974 223a 207b 0a20 2020 2020  onExit": {.     
+000051c0: 2020 2020 2020 2020 2020 2022 7479 7065             "type
+000051d0: 223a 2022 5265 6769 6f6e 4578 6974 222c  ": "RegionExit",
+000051e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000051f0: 2022 656e 6162 6c65 6422 3a20 7472 7565   "enabled": true
+00005200: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00005210: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
+00005220: 2022 5472 6967 6765 7273 2061 6e20 6576   "Triggers an ev
+00005230: 656e 7420 7768 656e 2061 2070 6c61 7965  ent when a playe
+00005240: 7220 6578 6974 2061 2072 6567 696f 6e22  r exit a region"
+00005250: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
+00005260: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00005270: 2020 2261 6767 7265 6761 7465 223a 207b    "aggregate": {
+00005280: 7d0a 2020 2020 7d2c 0a20 2020 2022 6665  }.    },.    "fe
+00005290: 6174 7572 6573 223a 207b 0a20 2020 2020  atures": {.     
+000052a0: 2020 2022 7065 725f 636f 756e 7422 3a20     "per_count": 
+000052b0: 7b0a 2020 2020 2020 2020 2020 2020 2252  {.            "R
+000052c0: 6567 696f 6e44 7572 6174 696f 6e22 3a20  egionDuration": 
+000052d0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+000052e0: 2020 2274 7970 6522 3a20 2252 6567 696f    "type": "Regio
+000052f0: 6e44 7572 6174 696f 6e22 2c0a 2020 2020  nDuration",.    
+00005300: 2020 2020 2020 2020 2020 2020 2265 6e61              "ena
+00005310: 626c 6564 223a 2074 7275 652c 0a20 2020  bled": true,.   
+00005320: 2020 2020 2020 2020 2020 2020 2022 636f               "co
+00005330: 756e 7422 3a20 3131 2c0a 2020 2020 2020  unt": 11,.      
+00005340: 2020 2020 2020 2020 2020 2270 7265 6669            "prefi
+00005350: 7822 3a20 2272 6567 696f 6e22 2c0a 2020  x": "region",.  
+00005360: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+00005370: 6573 6372 6970 7469 6f6e 223a 2022 5468  escription": "Th
+00005380: 6520 6475 7261 7469 6f6e 206f 6620 7469  e duration of ti
+00005390: 6d65 2061 2070 6c61 7965 7220 706c 6179  me a player play
+000053a0: 6564 2069 6e20 6120 6769 7665 6e20 7265  ed in a given re
+000053b0: 6769 6f6e 206f 6620 7468 6520 6761 6d65  gion of the game
+000053c0: 2e22 2c0a 2020 2020 2020 2020 2020 2020  .",.            
+000053d0: 2020 2020 2272 6574 7572 6e5f 7479 7065      "return_type
+000053e0: 223a 2022 7469 6d65 6465 6c74 6122 0a20  ": "timedelta". 
+000053f0: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
+00005400: 2020 2020 2020 2020 2020 2257 6164 646c            "Waddl
+00005410: 6550 6572 5265 6769 6f6e 223a 207b 0a20  ePerRegion": {. 
+00005420: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00005430: 7479 7065 223a 2022 5761 6464 6c65 5065  type": "WaddlePe
+00005440: 7252 6567 696f 6e22 2c0a 2020 2020 2020  rRegion",.      
+00005450: 2020 2020 2020 2020 2020 2265 6e61 626c            "enabl
+00005460: 6564 223a 2074 7275 652c 0a20 2020 2020  ed": true,.     
+00005470: 2020 2020 2020 2020 2020 2022 636f 756e             "coun
+00005480: 7422 3a20 3131 2c0a 2020 2020 2020 2020  t": 11,.        
+00005490: 2020 2020 2020 2020 2270 7265 6669 7822          "prefix"
+000054a0: 3a20 2272 6567 696f 6e22 2c0a 2020 2020  : "region",.    
+000054b0: 2020 2020 2020 2020 2020 2020 2264 6573              "des
+000054c0: 6372 6970 7469 6f6e 223a 2022 5468 6520  cription": "The 
+000054d0: 6e75 6d62 6572 206f 6620 7469 6d65 7320  number of times 
+000054e0: 6120 706c 6179 6572 2077 6164 646c 6564  a player waddled
+000054f0: 2069 6e20 6120 6769 7665 6e20 7265 6769   in a given regi
+00005500: 6f6e 206f 6620 7468 6520 6761 6d65 2e22  on of the game."
+00005510: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00005520: 2020 2272 6574 7572 6e5f 7479 7065 223a    "return_type":
+00005530: 2022 696e 7422 0a20 2020 2020 2020 2020   "int".         
+00005540: 2020 207d 0a20 2020 2020 2020 207d 2c0a     }.        },.
+00005550: 2020 2020 2020 2020 2261 6767 7265 6761          "aggrega
+00005560: 7465 223a 207b 0a20 2020 2020 2020 2020  te": {.         
+00005570: 2020 2022 4761 7a65 436f 756e 7422 3a20     "GazeCount": 
+00005580: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00005590: 2020 2274 7970 6522 3a20 2247 617a 6543    "type": "GazeC
+000055a0: 6f75 6e74 222c 0a20 2020 2020 2020 2020  ount",.         
+000055b0: 2020 2020 2020 2022 656e 6162 6c65 6422         "enabled"
+000055c0: 3a20 7472 7565 2c0a 2020 2020 2020 2020  : true,.        
+000055d0: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
+000055e0: 7469 6f6e 223a 2022 5468 6520 6e75 6d62  tion": "The numb
+000055f0: 6572 206f 6620 7469 6d65 7320 6120 706c  er of times a pl
+00005600: 6179 6572 2077 6164 646c 6564 2069 6e20  ayer waddled in 
+00005610: 6120 6769 7665 6e20 7265 6769 6f6e 206f  a given region o
+00005620: 6620 7468 6520 6761 6d65 2e22 2c0a 2020  f the game.",.  
+00005630: 2020 2020 2020 2020 2020 2020 2020 2272                "r
+00005640: 6574 7572 6e5f 7479 7065 223a 2022 696e  eturn_type": "in
+00005650: 7422 0a20 2020 2020 2020 2020 2020 207d  t".            }
+00005660: 2c0a 2020 2020 2020 2020 2020 2020 2250  ,.            "P
+00005670: 6963 6b75 7052 6f63 6b43 6f75 6e74 223a  ickupRockCount":
+00005680: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00005690: 2020 2022 7479 7065 223a 2022 5069 636b     "type": "Pick
+000056a0: 7570 526f 636b 436f 756e 7422 2c0a 2020  upRockCount",.  
+000056b0: 2020 2020 2020 2020 2020 2020 2020 2265                "e
+000056c0: 6e61 626c 6564 223a 2074 7275 652c 0a20  nabled": true,. 
+000056d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000056e0: 6465 7363 7269 7074 696f 6e22 3a20 2254  description": "T
+000056f0: 6865 2064 7572 6174 696f 6e20 6561 6368  he duration each
+00005700: 2073 6573 7369 6f6e 2074 6f6f 6b2e 222c   session took.",
+00005710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005720: 2022 7265 7475 726e 5f74 7970 6522 3a20   "return_type": 
+00005730: 2269 6e74 220a 2020 2020 2020 2020 2020  "int".          
+00005740: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
+00005750: 2022 506c 6179 6572 5761 6464 6c65 436f   "PlayerWaddleCo
+00005760: 756e 7422 3a20 7b0a 2020 2020 2020 2020  unt": {.        
+00005770: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
+00005780: 2250 6c61 7965 7257 6164 646c 6543 6f75  "PlayerWaddleCou
+00005790: 6e74 222c 0a20 2020 2020 2020 2020 2020  nt",.           
+000057a0: 2020 2020 2022 656e 6162 6c65 6422 3a20       "enabled": 
+000057b0: 7472 7565 2c0a 2020 2020 2020 2020 2020  true,.          
+000057c0: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
+000057d0: 6f6e 223a 2022 5468 6520 6e75 6d62 6572  on": "The number
+000057e0: 206f 6620 7469 6d65 7320 6120 706c 6179   of times a play
+000057f0: 6572 2077 6164 646c 6564 2e22 2c0a 2020  er waddled.",.  
+00005800: 2020 2020 2020 2020 2020 2020 2020 2272                "r
+00005810: 6574 7572 6e5f 7479 7065 223a 2022 696e  eturn_type": "in
+00005820: 7422 0a20 2020 2020 2020 2020 2020 207d  t".            }
+00005830: 2c0a 2020 2020 2020 2020 2020 2020 2253  ,.            "S
+00005840: 6573 7369 6f6e 4475 7261 7469 6f6e 223a  essionDuration":
+00005850: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00005860: 2020 2022 7479 7065 223a 2022 5365 7373     "type": "Sess
+00005870: 696f 6e44 7572 6174 696f 6e22 2c0a 2020  ionDuration",.  
+00005880: 2020 2020 2020 2020 2020 2020 2020 2265                "e
+00005890: 6e61 626c 6564 223a 2074 7275 652c 0a20  nabled": true,. 
+000058a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000058b0: 6465 7363 7269 7074 696f 6e22 3a20 2254  description": "T
+000058c0: 6865 2064 7572 6174 696f 6e20 6561 6368  he duration each
+000058d0: 2073 6573 7369 6f6e 2074 6f6f 6b2e 222c   session took.",
+000058e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000058f0: 2022 7265 7475 726e 5f74 7970 6522 3a20   "return_type": 
+00005900: 2274 696d 6564 656c 7461 220a 2020 2020  "timedelta".    
+00005910: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00005920: 2020 2020 2020 2022 4761 7a65 4475 7261         "GazeDura
+00005930: 7469 6f6e 223a 207b 0a20 2020 2020 2020  tion": {.       
+00005940: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
+00005950: 2022 4761 7a65 4475 7261 7469 6f6e 222c   "GazeDuration",
+00005960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005970: 2022 656e 6162 6c65 6422 3a20 7472 7565   "enabled": true
+00005980: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00005990: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
+000059a0: 2022 486f 7720 6c6f 6e67 2067 617a 6520   "How long gaze 
+000059b0: 6576 656e 7420 6c61 7374 2066 6f72 2e22  event last for."
+000059c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000059d0: 2020 2272 6574 7572 6e5f 7479 7065 223a    "return_type":
+000059e0: 2022 7469 6d65 6465 6c74 6122 0a20 2020   "timedelta".   
+000059f0: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+00005a00: 2020 2020 2020 2020 2252 6567 696f 6e45          "RegionE
+00005a10: 6e74 6572 436f 756e 7422 3a20 7b0a 2020  nterCount": {.  
+00005a20: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+00005a30: 7970 6522 3a20 2252 6567 696f 6e45 6e74  ype": "RegionEnt
+00005a40: 6572 436f 756e 7422 2c0a 2020 2020 2020  erCount",.      
+00005a50: 2020 2020 2020 2020 2020 2265 6e61 626c            "enabl
+00005a60: 6564 223a 2066 616c 7365 2c0a 2020 2020  ed": false,.    
+00005a70: 2020 2020 2020 2020 2020 2020 2264 6573              "des
+00005a80: 6372 6970 7469 6f6e 223a 2022 5468 6520  cription": "The 
+00005a90: 6e75 6d62 6572 206f 6620 7469 6d65 7320  number of times 
+00005aa0: 6120 706c 6179 6572 2065 6e74 6572 6420  a player enterd 
+00005ab0: 666f 7220 6120 6769 7665 6e20 7265 6769  for a given regi
+00005ac0: 6f6e 206f 6620 7468 6520 6761 6d65 2e22  on of the game."
+00005ad0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00005ae0: 2020 2272 6574 7572 6e5f 7479 7065 223a    "return_type":
+00005af0: 2022 696e 7422 0a20 2020 2020 2020 2020   "int".         
+00005b00: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
+00005b10: 2020 2241 6374 6976 6974 7943 6f6d 706c    "ActivityCompl
+00005b20: 6574 6564 223a 207b 0a20 2020 2020 2020  eted": {.       
+00005b30: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
+00005b40: 2022 4163 7469 7669 7479 436f 6d70 6c65   "ActivityComple
+00005b50: 7465 6422 2c0a 2020 2020 2020 2020 2020  ted",.          
+00005b60: 2020 2020 2020 2265 6e61 626c 6564 223a        "enabled":
+00005b70: 2074 7275 652c 0a20 2020 2020 2020 2020   true,.         
+00005b80: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
+00005b90: 696f 6e22 3a20 2254 6865 2061 6374 6976  ion": "The activ
+00005ba0: 6974 6965 7320 636f 6d70 6c65 7465 6420  ities completed 
+00005bb0: 696e 2061 2067 6976 656e 2073 6573 7369  in a given sessi
+00005bc0: 6f6e 2e22 2c0a 2020 2020 2020 2020 2020  on.",.          
+00005bd0: 2020 2020 2020 2272 6574 7572 6e5f 7479        "return_ty
+00005be0: 7065 223a 2022 696e 7422 0a20 2020 2020  pe": "int".     
+00005bf0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00005c00: 2020 2020 2020 2241 6374 6976 6974 7944        "ActivityD
+00005c10: 7572 6174 696f 6e22 3a20 7b0a 2020 2020  uration": {.    
+00005c20: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
+00005c30: 6522 3a20 2241 6374 6976 6974 7944 7572  e": "ActivityDur
+00005c40: 6174 696f 6e22 2c0a 2020 2020 2020 2020  ation",.        
+00005c50: 2020 2020 2020 2020 2265 6e61 626c 6564          "enabled
+00005c60: 223a 2074 7275 652c 0a20 2020 2020 2020  ": true,.       
+00005c70: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
+00005c80: 7074 696f 6e22 3a20 2248 6f77 206c 6f6e  ption": "How lon
+00005c90: 6720 6163 7469 7669 7479 206c 6173 7420  g activity last 
+00005ca0: 666f 722e 222c 0a20 2020 2020 2020 2020  for.",.         
+00005cb0: 2020 2020 2020 2022 7265 7475 726e 5f74         "return_t
+00005cc0: 7970 6522 3a20 2269 6e74 220a 2020 2020  ype": "int".    
+00005cd0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00005ce0: 2020 2020 2020 2022 5265 6769 6f6e 7345         "RegionsE
+00005cf0: 6e63 6f75 6e74 6572 6564 223a 207b 0a20  ncountered": {. 
+00005d00: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00005d10: 7479 7065 223a 2022 5265 6769 6f6e 7345  type": "RegionsE
+00005d20: 6e63 6f75 6e74 6572 6564 222c 0a20 2020  ncountered",.   
+00005d30: 2020 2020 2020 2020 2020 2020 2022 656e               "en
+00005d40: 6162 6c65 6422 3a20 7472 7565 2c0a 2020  abled": true,.  
+00005d50: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+00005d60: 6573 6372 6970 7469 6f6e 223a 2022 5468  escription": "Th
+00005d70: 6520 7265 6769 6f6e 7320 656e 7465 7265  e regions entere
+00005d80: 6420 696e 2061 2067 6976 656e 2073 6573  d in a given ses
+00005d90: 7369 6f6e 2e22 2c0a 2020 2020 2020 2020  sion.",.        
+00005da0: 2020 2020 2020 2020 2272 6574 7572 6e5f          "return_
+00005db0: 7479 7065 223a 2022 696e 7422 0a20 2020  type": "int".   
+00005dc0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00005dd0: 2020 207d 0a20 2020 207d 2c0a 2020 2020     }.    },.    
+00005de0: 2263 6f6e 6669 6722 3a20 7b0a 2020 2020  "config": {.    
+00005df0: 2020 2020 2253 5550 504f 5254 4544 5f56      "SUPPORTED_V
+00005e00: 4552 5322 3a20 5b0a 2020 2020 2020 2020  ERS": [.        
+00005e10: 2020 2020 310a 2020 2020 2020 2020 5d0a      1.        ].
+00005e20: 2020 2020 7d0a 7d                            }.}
```

### Comparing `opengamedata-core-0.0.1/src/ogd/games/SHADOWSPECT/ShadowspectLoader.py` & `opengamedata_core-0.0.2/src/ogd/games/SHADOWSPECT/ShadowspectLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/SHADOWSPECT/features/FunnelByUser.py` & `opengamedata_core-0.0.2/src/ogd/games/SHADOWSPECT/features/FunnelByUser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # import libraries
 from typing import Any, List
 import json
-import pandas as pd
 # import locals
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 from ogd.core.schemas.Event import Event
 from ogd.core.schemas.ExtractionMode import ExtractionMode
 from ogd.core.schemas.FeatureData import FeatureData
```

### Comparing `opengamedata-core-0.0.1/src/ogd/games/SHADOWSPECT/features/LevelsOfDifficulty.py` & `opengamedata_core-0.0.2/src/ogd/games/SHADOWSPECT/features/LevelsOfDifficulty.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/SHADOWSPECT/features/MoveShapeCount.py` & `opengamedata_core-0.0.2/src/ogd/games/SHADOWSPECT/features/MoveShapeCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/SHADOWSPECT/features/SequenceBetweenPuzzles.py` & `opengamedata_core-0.0.2/src/ogd/games/SHADOWSPECT/features/SequenceBetweenPuzzles.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/SHADOWSPECT/features/SessionID.py` & `opengamedata_core-0.0.2/src/ogd/games/SHADOWSPECT/features/SessionID.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/SHADOWSPECT/schemas/SHADOWSPECT.json.template` & `opengamedata_core-0.0.2/src/ogd/games/SHADOWSPECT/schemas/SHADOWSPECT.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/SHIPWRECKS/ShipwrecksLoader.py` & `opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/ShipwrecksLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/SHIPWRECKS/features/ActiveJobs.py` & `opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/ActiveJobs.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/SHIPWRECKS/features/EventList.py` & `opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/EventList.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/SHIPWRECKS/features/EvidenceBoardCompleteCount.py` & `opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/EvidenceBoardCompleteCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/SHIPWRECKS/features/JobsAttempted.py` & `opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/JobsAttempted.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/SHIPWRECKS/features/JobsCompleted.py` & `opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/JobsCompleted.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/SHIPWRECKS/features/MissionDiveTime.py` & `opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/MissionDiveTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/SHIPWRECKS/features/MissionSonarTimeToComplete.py` & `opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/MissionSonarTimeToComplete.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/SHIPWRECKS/features/PlayerSummary.py` & `opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/PlayerSummary.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/SHIPWRECKS/features/PopulationSummary.py` & `opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/PopulationSummary.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/SHIPWRECKS/features/SessionDuration.py` & `opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/SessionDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/SHIPWRECKS/features/SessionID.py` & `opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/SessionID.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/SHIPWRECKS/features/TopJobCompletionDestinations.py` & `opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/TopJobCompletionDestinations.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/SHIPWRECKS/features/TopJobSwitchDestinations.py` & `opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/TopJobSwitchDestinations.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/SHIPWRECKS/features/TotalDiveTime.py` & `opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/TotalDiveTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/SHIPWRECKS/features/__init__.py` & `opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/__init__.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/SHIPWRECKS/schemas/SHIPWRECKS.json.template` & `opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/schemas/SHIPWRECKS.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/THERMOVR/ThermoVRLoader.py` & `opengamedata_core-0.0.2/src/ogd/games/THERMOVR/ThermoVRLoader.py`

 * *Files 19% similar despite different names*

```diff
@@ -65,14 +65,30 @@
         return features
 
     def _loadFeature(self, feature_type:str, extractor_params:GeneratorParameters, schema_args:Dict[str,Any]) -> Feature:
         ret_val : Feature
         # First run through aggregate features
         if extractor_params._count_index == None:
             match feature_type:
+                case "PhasesReached":
+                    ret_val = PhasesReached.PhasesReached(params=extractor_params)
+                case "PlayMode":
+                    ret_val = PlayMode.PlayMode(params=extractor_params)
+                case "TaskCompleteCount":
+                    ret_val = TaskCompleteCount.TaskCompleteCount(params=extractor_params)
+                case "LabCompleteCount":
+                    ret_val = LabCompleteCount.LabCompleteCount(params=extractor_params)
+                case "LeftHandMoves":
+                    ret_val = LeftHandMoves.LeftHandMoves(params=extractor_params)
+                case "RightHandMoves":
+                    ret_val = RightHandMoves.RightHandMoves(params=extractor_params)
+                case "ToolNudgeCount":
+                    ret_val = ToolNudgeCount.ToolNudgeCount(params=extractor_params)
+                case "ToolSliderTime":
+                    ret_val = ToolSliderTime.ToolSliderTime(params=extractor_params)
                 case _:
                     raise NotImplementedError(f"'{feature_type}' is not a valid aggregate feature type for ThermoVR.")
         # then run through per-count features.
         else:
             match feature_type:
                 case _:
                     raise NotImplementedError(f"'{feature_type}' is not a valid per-count feature type for ThermoVR.")
```

### Comparing `opengamedata-core-0.0.1/src/ogd/games/THERMOVR/features/TaskCompleteCount.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/MenuButtonCount.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,35 @@
-from typing import Any, List
+# import libraries
+from ogd.core.schemas import Event
+from typing import Any, List, Optional
+# import locals
+from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.generators.extractors.SessionFeature import SessionFeature
 from ogd.core.schemas.Event import Event
 from ogd.core.schemas.ExtractionMode import ExtractionMode
 from ogd.core.schemas.FeatureData import FeatureData
 
-class TaskCompleteCount(SessionFeature):
-
-    def __init__(self, params:GeneratorParameters, player_id:str):
-        self._player_id = player_id
-        super().__init__(params=params)
-        self._task_complete_count = 0
+class MenuButtonCount(PerLevelFeature):
+    def __init__(self, params:GeneratorParameters):
+        PerLevelFeature.__init__(self, params=params)
+        self._menu_btn_count = 0
 
+    # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["game_state"]
+        return ["CUSTOM.5"]
+        # "events": ["MENU_BUTTON"],
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
-    def _updateFromEvent(self, event: Event) -> None:
-        if event.UserID == self._player_id:
-            current_task = event.GameState.get('current_task', None)
-            if current_task and current_task.get('is_complete', False):
-                self._task_complete_count += 1
+    def _updateFromEvent(self, event:Event) -> None:
+        self._menu_btn_count += 1
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [self._task_complete_count]
+        return [self._menu_btn_count]
+
+    # *** Optionally override public functions. ***
```

### Comparing `opengamedata-core-0.0.1/src/ogd/games/THERMOVR/features/ToolNudegCount.py` & `opengamedata_core-0.0.2/src/ogd/games/THERMOVR/features/ToolNudgeCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/THERMOVR/schemas/THERMOVR.json.template` & `opengamedata_core-0.0.2/src/ogd/games/THERMOVR/schemas/THERMOVR.json.template`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'features'": "{'aggregate': {replace: OrderedDict([('LabCompleteCount', OrderedDict([('enabled', "*

 * *               "False), ('type', 'LabCompleteCount'), ('description', 'Count of number of labs "*

 * *               "completed'), ('return_type', 'int')])), ('LeftHandMoves', OrderedDict([('enabled', "*

 * *               "False), ('type', 'LabCompleteCount'), ('description', 'Count of number of Left "*

 * *               "hand moves'), ('return_type', 'int')])), ('RighHandMoves', "*

 * *               "OrderedDict([('enabled' […]*

```diff
@@ -833,15 +833,64 @@
                     "description": "The list of words available to be chosen from the bank.",
                     "type": "List[str]"
                 }
             }
         }
     },
     "features": {
-        "aggregate": {},
+        "aggregate": {
+            "LabCompleteCount": {
+                "description": "Count of number of labs completed",
+                "enabled": false,
+                "return_type": "int",
+                "type": "LabCompleteCount"
+            },
+            "LeftHandMoves": {
+                "description": "Count of number of Left hand moves",
+                "enabled": false,
+                "return_type": "int",
+                "type": "LabCompleteCount"
+            },
+            "PhasesReached": {
+                "description": "Phases Reached during a certain task",
+                "enabled": false,
+                "return_type": "dict",
+                "type": "PhasesReached"
+            },
+            "PlayMode": {
+                "description": "Play mode of the current instance",
+                "enabled": false,
+                "return_type": "str",
+                "type": "PlayMode"
+            },
+            "RighHandMoves": {
+                "description": "Count of number of right hand moves",
+                "enabled": false,
+                "return_type": "int",
+                "type": "RighHandMoves"
+            },
+            "TaskCompleteCount": {
+                "description": "Count of number of tasks completed",
+                "enabled": true,
+                "return_type": "int",
+                "type": "TaskCompleteCount"
+            },
+            "ToolNudegCount": {
+                "description": "Count of number of times a tool has been nudged",
+                "enabled": false,
+                "return_type": "dict",
+                "type": "ToolNudegCount"
+            },
+            "ToolSliderTime": {
+                "description": "Counts the total time the slider has been moved",
+                "enabled": false,
+                "return_type": "timedelta",
+                "type": "ToolSliderTime"
+            }
+        },
         "per_count": {}
     },
     "game_state": {
         "chamber_pressure_tool": {
             "description": "The state of the chamber/ambient pressure tool: the ambient pressure in kPa (the ambient pressure is always enabled).",
             "details": {
                 "enabled": "bool",
```

### Comparing `opengamedata-core-0.0.1/src/ogd/games/TRANSFORMATION_QUEST/DBExport.json` & `opengamedata_core-0.0.2/src/ogd/games/TRANSFORMATION_QUEST/DBExport.json`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/TRANSFORMATION_QUEST/schemas/TRANSFORMATION_QUEST.json.template` & `opengamedata_core-0.0.2/src/ogd/games/TRANSFORMATION_QUEST/schemas/TRANSFORMATION_QUEST.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/WaveLoader.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/WaveLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/AmplitudeGoodMoveCount.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/AmplitudeGoodMoveCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/AverageFails.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/AverageFails.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/AverageLevelTime.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/AverageLevelTime.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             Logger.Log(f"AverageLevelTime received an event which was not a BEGIN or a COMPLETE!", logging.WARN)
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
         if len(self._begin_times) < len(self._complete_times):
-            Logger.Log(f"Player began level {self.CountIndex} {len(self._begin_times)} times but completed it {len(self._complete_times)}.", logging.WARNING)
+            self.WarningMessage(f"Player began level {self.CountIndex} {len(self._begin_times)} times but completed it {len(self._complete_times)}.")
         _diffs      = []
         for level in self._levels_encountered:
             if level in self._begin_times.keys() and level in self._complete_times.keys():
                 _num_plays  = min(len(self._begin_times[level]), len(self._complete_times[level]))
                 _diffs += [(self._complete_times[level][i] - self._begin_times[level][i]).total_seconds() for i in range(_num_plays)]
             else:
                 if level not in self._begin_times.keys() and level in self._complete_times.keys():
```

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/AverageMoveTypeChanges.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/AverageMoveTypeChanges.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/AverageSliderMoves.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/AverageSliderMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/BeginCount.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/BeginCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/ClosenessIntercept.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/ClosenessIntercept.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/ClosenessR2.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/ClosenessR2.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/ClosenessSlope.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/ClosenessSlope.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/Completed.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/Completed.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/FirstMoveType.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/FirstMoveType.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/MenuButtonCount.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/TotalFails.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,34 @@
-# import libraries
 from ogd.core.schemas import Event
+import typing
 from typing import Any, List, Optional
 # import locals
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.schemas.Event import Event
 from ogd.core.schemas.ExtractionMode import ExtractionMode
 from ogd.core.schemas.FeatureData import FeatureData
 
-class MenuButtonCount(PerLevelFeature):
+class TotalFails(PerLevelFeature):
     def __init__(self, params:GeneratorParameters):
         PerLevelFeature.__init__(self, params=params)
-        self._menu_btn_count = 0
+        self._fail_count = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["CUSTOM.5"]
-        # "events": ["MENU_BUTTON"],
+        return ["FAIL.0"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
-        self._menu_btn_count += 1
+        self._fail_count += 1
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [self._menu_btn_count]
+        return [self._fail_count]
 
     # *** Optionally override public functions. ***
```

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/OffsetGoodMoveCount.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/OffsetGoodMoveCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/OverallPercentAmplitudeMoves.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/OverallPercentAmplitudeMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/OverallPercentOffsetMoves.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/OverallPercentOffsetMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/OverallPercentWavelengthMoves.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/OverallPercentWavelengthMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/OverallSliderAverageRange.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/OverallSliderAverageRange.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/OverallSliderAverageStandardDeviations.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/OverallSliderAverageStandardDeviations.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/PercentAmplitudeGoodMoves.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/PercentAmplitudeGoodMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/PercentAmplitudeMoves.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/PercentAmplitudeMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/PercentOffsetGoodMoves.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/PercentOffsetGoodMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/PercentOffsetMoves.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/PercentOffsetMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/PercentWavelengthGoodMoves.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/PercentWavelengthGoodMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/PercentWavelengthMoves.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/PercentWavelengthMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/PersistentSessionID.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/PersistentSessionID.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/QuestionAnswered.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/QuestionAnswered.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/QuestionCorrect.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/QuestionCorrect.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/RangeIntercept.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/RangeIntercept.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/RangeR2.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/RangeR2.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/RangeSlope.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/RangeSlope.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/SequenceLevel.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/SequenceLevel.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/SessionID.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/SessionID.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/SliderAverageRange.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/SliderAverageRange.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/SliderAverageStandardDeviations.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/SliderAverageStandardDeviations.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/SucceedCount.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/SucceedCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/TimeToAnswerMS.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/TimeToAnswerMS.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/TotalArrowMoves.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/TotalArrowMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/TotalFails.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/TotalResets.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,36 @@
+# import libraries
 from ogd.core.schemas import Event
 import typing
 from typing import Any, List, Optional
 # import locals
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.schemas.Event import Event
 from ogd.core.schemas.ExtractionMode import ExtractionMode
 from ogd.core.schemas.FeatureData import FeatureData
 
-class TotalFails(PerLevelFeature):
+class TotalResets(PerLevelFeature):
     def __init__(self, params:GeneratorParameters):
         PerLevelFeature.__init__(self, params=params)
-        self._fail_count = 0
+        self._reset_count = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["FAIL.0"]
+        return ["CUSTOM.4"]
+        # "events": ["RESET_BTN_PRESS"],
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
-        self._fail_count += 1
+        self._reset_count += 1
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [self._fail_count]
+        return [self._reset_count]
 
     # *** Optionally override public functions. ***
```

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/TotalLevelTime.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/TotalLevelTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/TotalMoveTypeChanges.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/TotalMoveTypeChanges.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/TotalResets.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/TotalSkips.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,32 +5,32 @@
 # import locals
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.schemas.Event import Event
 from ogd.core.schemas.ExtractionMode import ExtractionMode
 from ogd.core.schemas.FeatureData import FeatureData
 
-class TotalResets(PerLevelFeature):
+class TotalSkips(PerLevelFeature):
     def __init__(self, params:GeneratorParameters):
         PerLevelFeature.__init__(self, params=params)
-        self._reset_count = 0
+        self._skip_count = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["CUSTOM.4"]
-        # "events": ["RESET_BTN_PRESS"],
+        return ["CUSTOM.6"]
+        # "events": ["SKIP_BUTTON"],
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
-        self._reset_count += 1
+        self._skip_count += 1
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [self._reset_count]
+        return [self._skip_count]
 
     # *** Optionally override public functions. ***
```

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/TotalSliderMoves.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/TotalSliderMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/WavelengthGoodMoveCount.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/WavelengthGoodMoveCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/features/__init__.py` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/__init__.py`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WAVES/schemas/WAVES.json.template` & `opengamedata_core-0.0.2/src/ogd/games/WAVES/schemas/WAVES.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/ogd/games/WEATHER_STATION/schemas/WEATHER_STATION.json.template` & `opengamedata_core-0.0.2/src/ogd/games/WEATHER_STATION/schemas/WEATHER_STATION.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata-core-0.0.1/src/opengamedata_core.egg-info/PKG-INFO` & `opengamedata_core-0.0.2/src/opengamedata_core.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opengamedata-core
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for retrieving and processing event-based video game data. Additional authors: Nick Spevacek, Renee Li, John McCloskey, Zach Studdiford, Glenn Palmer, Haishuo Chen, Daus, Ameya Kshirsagar, Yunqing Xiao, Erik Harpstead, Manuel Jesus Gomez Moratilla
 Author-email: Luke Swanson <superscription58@gmail.com>, David Gagnon <djgagnon@wisc.edu>
 Project-URL: Homepage, https://github.com/opengamedata/opengamedata-core
 Project-URL: Bug Tracker, https://github.com/opengamedata/opengamedata-core/issues
 Project-URL: Documentation, https://opengamedata-doc.readthedocs.io/en/latest/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,29 +13,29 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Python3 implementation of the Open Game Gata feature extractor  
 
 This code pulls raw game data from a SQL database, BigQuery database, or export file; chooses appropiate features to extract based on the "game_id"; and writes results to a file for data mining.
 
-See http://fielddaylab.wisc.edu/opengamedata for exports of raw events and the features created by this code for a collection of education games.
-See https://www.youtube.com/watch?v=gelyDJjxIeg for a walkthorugh of the high-level code structure.
+See [http://fielddaylab.wisc.edu/opengamedata](http://fielddaylab.wisc.edu/opengamedata) for exports of raw events and the features created by this code for a collection of education games.
+See [https://www.youtube.com/watch?v=gelyDJjxIeg](https://www.youtube.com/watch?v=gelyDJjxIeg) for a walkthorugh of the high-level code structure.
 
 Please feel free to modify this code, add new features or games and share back to the authors. We will deploy improvements to the Open Game Data site.
 
 Setup:
 
 * Install python3 (could write a whole chapter on this)
 * Install python dependencies: "pip3 install -r requirements.txt"
 * Copy `config.py.template` to `config.py` and set server/authentication data
 * Download any authentication keys needed for BigQuery game data projects
 
 Running Data Exports:  
 
-```
+```none
 usage: <python> main.py <cmd> [<args>]
 
 <python> is your python command.
 <cmd>    is one of the available commands:
          - export
          - export-events
          - export-features
@@ -60,34 +60,40 @@
          - readme: game_id
              game_id    = id of game whose readme should be generated
          - help: *None*
 [<opt-args>] are option arguments, which affect certain commands:
          --file: specifies a file to export events or features
          --monthly: with this flag, specify dates by mm/yyyy instead of mm/dd/yyyy
 ```
+
 (you can see a similar printout directly from the system by running ```python3 main.py --help```)
 
 Example use:
-```
+
+```none
 python3 main.py export JOWILDER 1/1/2019 2/28/2019
 ```
+
 In the example above, all JOWILDER data from beginning of January to end of February (in 2019) is exported. This includes both the events and the processed session features.
 
-```
+```none
 python3 main.py export JOWILDER --monthly 1/2019
 ```
+
 In the example above, all JOWILDER data from the month of January 2019 is exported. This includes both the events and the processed session features.
 
-```
+```none
 python3 main.py export-events JOWILDER 1/1/2019 2/28/2019
 ```
+
 In the example above, only the events from the JOWILDER data during given date range are exported.
 
-```
+```none
 python3 main.py export-features JOWILDER 1/1/2019 2/28/2019
 ```
+
 In the example above, only the processed session/player/population features from the JOWILDER data during given date range are exported.
 
 <!-- ```
 python3 main.py export JOWILDER --file=C:\path\to\opengamedata-backend\data\JOWILDER\JOWILDER_20190101_to_20190228_1234abc_events.zip
 ```
 In the example above, events and processed session features are exported from the data at the specified file path. -->
```

### Comparing `opengamedata-core-0.0.1/src/opengamedata_core.egg-info/SOURCES.txt` & `opengamedata_core-0.0.2/src/opengamedata_core.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -69,17 +69,17 @@
 src/ogd/core/schemas/configs/IndexingSchema.py
 src/ogd/core/schemas/configs/LegacyConfigSchema.py
 src/ogd/core/schemas/configs/data_sources/BigQuerySourceSchema.py
 src/ogd/core/schemas/configs/data_sources/DataSourceSchema.py
 src/ogd/core/schemas/configs/data_sources/FileSourceSchema.py
 src/ogd/core/schemas/configs/data_sources/MySQLSourceSchema.py
 src/ogd/core/schemas/games/AggregateSchema.py
+src/ogd/core/schemas/games/DataElementSchema.py
 src/ogd/core/schemas/games/DetectorMapSchema.py
 src/ogd/core/schemas/games/DetectorSchema.py
-src/ogd/core/schemas/games/EventDataElementSchema.py
 src/ogd/core/schemas/games/EventSchema.py
 src/ogd/core/schemas/games/ExtractorSchema.py
 src/ogd/core/schemas/games/FeatureMapSchema.py
 src/ogd/core/schemas/games/FeatureSchema.py
 src/ogd/core/schemas/games/GameSchema.py
 src/ogd/core/schemas/games/GameStateSchema.py
 src/ogd/core/schemas/games/PerCountSchema.py
@@ -123,14 +123,15 @@
 src/ogd/games/AQUALAB/features/JobDiveSitesCount.py
 src/ogd/games/AQUALAB/features/JobDiveTime.py
 src/ogd/games/AQUALAB/features/JobExperimentationTime.py
 src/ogd/games/AQUALAB/features/JobGuideCount.py
 src/ogd/games/AQUALAB/features/JobHelpCount.py
 src/ogd/games/AQUALAB/features/JobLocationChanges.py
 src/ogd/games/AQUALAB/features/JobModelingTime.py
+src/ogd/games/AQUALAB/features/JobPlayTime.py
 src/ogd/games/AQUALAB/features/JobStartCount.py
 src/ogd/games/AQUALAB/features/JobTasksCompleted.py
 src/ogd/games/AQUALAB/features/JobTriesInArgument.py
 src/ogd/games/AQUALAB/features/JobsAttempted.py
 src/ogd/games/AQUALAB/features/JobsCompleted.py
 src/ogd/games/AQUALAB/features/ModelExportCount.py
 src/ogd/games/AQUALAB/features/ModelInterveneCount.py
@@ -155,14 +156,17 @@
 src/ogd/games/AQUALAB/features/UserAvgActiveTime.py
 src/ogd/games/AQUALAB/features/UserAvgSessionDuration.py
 src/ogd/games/AQUALAB/features/UserTotalSessionDuration.py
 src/ogd/games/AQUALAB/features/__init__.py
 src/ogd/games/AQUALAB/schemas/AQUALAB.json.template
 src/ogd/games/BACTERIA/schemas/BACTERIA.json.template
 src/ogd/games/BALLOON/schemas/BALLOON.json.template
+src/ogd/games/BLOOM/schemas/BLOOM.json.template
+src/ogd/games/CENSIO_SLIDE/schemas/CENSIO_SLIDE.json.template
+src/ogd/games/CENSIO_STACK/schemas/CENSIO_STACK.json.template
 src/ogd/games/CRUSH_STATION/schemas/CRUSH_STATION.json.template
 src/ogd/games/CRYSTAL/CrystalLoader.py
 src/ogd/games/CRYSTAL/features/CrystalExtractor.py
 src/ogd/games/CRYSTAL/features/__init__.py
 src/ogd/games/CRYSTAL/schemas/CRYSTAL.json.template
 src/ogd/games/CYCLE_CARBON/schemas/CYCLE_CARBON.json.template
 src/ogd/games/CYCLE_NITROGEN/schemas/CYCLE_NITROGEN.json.template
@@ -349,16 +353,21 @@
 src/ogd/games/SHIPWRECKS/features/__init__.py
 src/ogd/games/SHIPWRECKS/schemas/SHIPWRECKS.json.template
 src/ogd/games/THERMOVR/DBExport.json
 src/ogd/games/THERMOVR/ThermoVRLoader.py
 src/ogd/games/THERMOVR/__init__.py
 src/ogd/games/THERMOVR/detectors/__init__.py
 src/ogd/games/THERMOVR/features/LabCompleteCount.py
+src/ogd/games/THERMOVR/features/LeftHandMoves.py
+src/ogd/games/THERMOVR/features/PhasesReached.py
+src/ogd/games/THERMOVR/features/PlayMode.py
+src/ogd/games/THERMOVR/features/RightHandMoves.py
 src/ogd/games/THERMOVR/features/TaskCompleteCount.py
-src/ogd/games/THERMOVR/features/ToolNudegCount.py
+src/ogd/games/THERMOVR/features/ToolNudgeCount.py
+src/ogd/games/THERMOVR/features/ToolSliderTime.py
 src/ogd/games/THERMOVR/features/__init__.py
 src/ogd/games/THERMOVR/schemas/THERMOVR.json.template
 src/ogd/games/TRANSFORMATION_QUEST/DBExport.json
 src/ogd/games/TRANSFORMATION_QUEST/schemas/TRANSFORMATION_QUEST.json.template
 src/ogd/games/WAVES/WaveLoader.py
 src/ogd/games/WAVES/features/AmplitudeGoodMoveCount.py
 src/ogd/games/WAVES/features/AverageFails.py
```

### Comparing `opengamedata-core-0.0.1/tests/test_lakeland_models.py` & `opengamedata_core-0.0.2/tests/test_lakeland_models.py`

 * *Files identical despite different names*

