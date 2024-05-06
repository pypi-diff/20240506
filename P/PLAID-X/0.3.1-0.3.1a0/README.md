# Comparing `tmp/PLAID-X-0.3.1.tar.gz` & `tmp/plaid_x-0.3.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PLAID-X-0.3.1.tar", last modified: Tue Feb 27 23:23:51 2024, max compression
+gzip compressed data, was "plaid_x-0.3.1a0.tar", last modified: Mon May  6 03:41:50 2024, max compression
```

## Comparing `PLAID-X-0.3.1.tar` & `plaid_x-0.3.1a0.tar`

### file list

```diff
@@ -1,113 +1,114 @@
-drwxr-xr-x   0 eyang     (1795) staff    (20063)        0 2024-02-27 23:24:03.013878 PLAID-X-0.3.1/
--rw-r--r--   0 eyang     (1795) staff    (20063)     1091 2023-12-28 04:23:43.000000 PLAID-X-0.3.1/LICENSE
--rw-r--r--   0 eyang     (1795) staff    (20063)      196 2024-02-14 22:46:32.000000 PLAID-X-0.3.1/MANIFEST.in
--rw-r--r--   0 eyang     (1795) staff    (20063)     5559 2024-02-27 23:24:02.931850 PLAID-X-0.3.1/PKG-INFO
-drwxr-xr-x   0 eyang     (1795) staff    (20063)        0 2024-02-27 23:24:02.928850 PLAID-X-0.3.1/PLAID_X.egg-info/
--rw-r--r--   0 eyang     (1795) staff    (20063)     5559 2024-02-27 23:24:01.000000 PLAID-X-0.3.1/PLAID_X.egg-info/PKG-INFO
--rw-r--r--   0 eyang     (1795) staff    (20063)     2850 2024-02-27 23:24:01.000000 PLAID-X-0.3.1/PLAID_X.egg-info/SOURCES.txt
--rw-r--r--   0 eyang     (1795) staff    (20063)        1 2024-02-27 23:24:01.000000 PLAID-X-0.3.1/PLAID_X.egg-info/dependency_links.txt
--rw-r--r--   0 eyang     (1795) staff    (20063)      148 2024-02-27 23:24:01.000000 PLAID-X-0.3.1/PLAID_X.egg-info/requires.txt
--rw-r--r--   0 eyang     (1795) staff    (20063)        8 2024-02-27 23:24:01.000000 PLAID-X-0.3.1/PLAID_X.egg-info/top_level.txt
--rw-r--r--   0 eyang     (1795) staff    (20063)     4810 2024-02-27 22:50:01.000000 PLAID-X-0.3.1/README.md
-drwxr-xr-x   0 eyang     (1795) staff    (20063)        0 2024-02-27 23:24:02.153867 PLAID-X-0.3.1/colbert/
--rw-r--r--   0 eyang     (1795) staff    (20063)      174 2023-12-28 04:23:43.000000 PLAID-X-0.3.1/colbert/__init__.py
-drwxr-xr-x   0 eyang     (1795) staff    (20063)        0 2024-02-27 23:24:02.209862 PLAID-X-0.3.1/colbert/data/
--rw-r--r--   0 eyang     (1795) staff    (20063)       97 2023-12-28 04:23:43.000000 PLAID-X-0.3.1/colbert/data/__init__.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     3358 2024-02-14 22:45:42.000000 PLAID-X-0.3.1/colbert/data/collection.py
--rw-r--r--   0 eyang     (1795) staff    (20063)      421 2023-12-28 04:23:43.000000 PLAID-X-0.3.1/colbert/data/dataset.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     3598 2024-02-27 21:39:56.000000 PLAID-X-0.3.1/colbert/data/examples.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     4397 2024-02-14 22:45:42.000000 PLAID-X-0.3.1/colbert/data/queries.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     2774 2024-02-14 22:46:32.000000 PLAID-X-0.3.1/colbert/data/ranking.py
-drwxr-xr-x   0 eyang     (1795) staff    (20063)        0 2024-02-27 23:24:02.269859 PLAID-X-0.3.1/colbert/evaluation/
--rw-r--r--   0 eyang     (1795) staff    (20063)        0 2023-12-28 04:23:43.000000 PLAID-X-0.3.1/colbert/evaluation/__init__.py
--rw-r--r--   0 eyang     (1795) staff    (20063)      919 2023-12-28 04:23:43.000000 PLAID-X-0.3.1/colbert/evaluation/load_model.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     6650 2024-02-14 22:45:43.000000 PLAID-X-0.3.1/colbert/evaluation/loaders.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     4304 2023-12-28 04:23:43.000000 PLAID-X-0.3.1/colbert/evaluation/metrics.py
--rw-r--r--   0 eyang     (1795) staff    (20063)      286 2023-12-28 04:23:43.000000 PLAID-X-0.3.1/colbert/index.py
--rw-r--r--   0 eyang     (1795) staff    (20063)    20069 2023-12-28 04:23:43.000000 PLAID-X-0.3.1/colbert/index_updater.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     4640 2024-02-14 22:45:43.000000 PLAID-X-0.3.1/colbert/indexer.py
-drwxr-xr-x   0 eyang     (1795) staff    (20063)        0 2024-02-27 23:24:02.330862 PLAID-X-0.3.1/colbert/indexing/
--rw-r--r--   0 eyang     (1795) staff    (20063)        0 2023-12-28 04:23:43.000000 PLAID-X-0.3.1/colbert/indexing/__init__.py
-drwxr-xr-x   0 eyang     (1795) staff    (20063)        0 2024-02-27 23:24:02.433860 PLAID-X-0.3.1/colbert/indexing/codecs/
--rw-r--r--   0 eyang     (1795) staff    (20063)        0 2023-12-28 04:23:43.000000 PLAID-X-0.3.1/colbert/indexing/codecs/__init__.py
--rw-r--r--   0 eyang     (1795) staff    (20063)      982 2023-12-28 04:23:43.000000 PLAID-X-0.3.1/colbert/indexing/codecs/decompress_residuals.cpp
--rw-r--r--   0 eyang     (1795) staff    (20063)     3014 2023-12-28 04:23:43.000000 PLAID-X-0.3.1/colbert/indexing/codecs/decompress_residuals.cu
--rw-r--r--   0 eyang     (1795) staff    (20063)      284 2023-12-28 04:23:43.000000 PLAID-X-0.3.1/colbert/indexing/codecs/packbits.cpp
--rw-r--r--   0 eyang     (1795) staff    (20063)     1558 2023-12-28 04:23:43.000000 PLAID-X-0.3.1/colbert/indexing/codecs/packbits.cu
--rw-r--r--   0 eyang     (1795) staff    (20063)    10915 2023-12-28 04:23:43.000000 PLAID-X-0.3.1/colbert/indexing/codecs/residual.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     3192 2023-12-28 04:23:43.000000 PLAID-X-0.3.1/colbert/indexing/codecs/residual_embeddings.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     1735 2023-12-28 04:23:43.000000 PLAID-X-0.3.1/colbert/indexing/codecs/residual_embeddings_strided.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     1823 2023-12-28 04:23:43.000000 PLAID-X-0.3.1/colbert/indexing/collection_encoder.py
--rw-r--r--   0 eyang     (1795) staff    (20063)    33008 2024-02-14 22:45:43.000000 PLAID-X-0.3.1/colbert/indexing/collection_indexer.py
--rw-r--r--   0 eyang     (1795) staff    (20063)      878 2023-12-28 04:23:43.000000 PLAID-X-0.3.1/colbert/indexing/index_manager.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     2900 2023-12-28 04:23:43.000000 PLAID-X-0.3.1/colbert/indexing/index_saver.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     1995 2023-12-28 04:23:43.000000 PLAID-X-0.3.1/colbert/indexing/loaders.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     1826 2023-12-28 04:23:43.000000 PLAID-X-0.3.1/colbert/indexing/utils.py
-drwxr-xr-x   0 eyang     (1795) staff    (20063)        0 2024-02-27 23:24:02.484853 PLAID-X-0.3.1/colbert/infra/
--rw-r--r--   0 eyang     (1795) staff    (20063)       40 2023-12-28 04:23:43.000000 PLAID-X-0.3.1/colbert/infra/__init__.py
-drwxr-xr-x   0 eyang     (1795) staff    (20063)        0 2024-02-27 23:24:02.546856 PLAID-X-0.3.1/colbert/infra/config/
--rw-r--r--   0 eyang     (1795) staff    (20063)       45 2023-12-28 04:23:43.000000 PLAID-X-0.3.1/colbert/infra/config/__init__.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     4131 2024-02-14 22:46:32.000000 PLAID-X-0.3.1/colbert/infra/config/base_config.py
--rw-r--r--   0 eyang     (1795) staff    (20063)      364 2023-12-28 04:23:43.000000 PLAID-X-0.3.1/colbert/infra/config/config.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     2222 2024-02-14 22:46:32.000000 PLAID-X-0.3.1/colbert/infra/config/core_config.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     5273 2024-02-14 22:45:43.000000 PLAID-X-0.3.1/colbert/infra/config/settings.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     4611 2023-12-28 04:23:43.000000 PLAID-X-0.3.1/colbert/infra/launcher.py
--rw-r--r--   0 eyang     (1795) staff    (20063)      932 2023-12-28 04:23:43.000000 PLAID-X-0.3.1/colbert/infra/provenance.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     2555 2024-02-14 22:45:43.000000 PLAID-X-0.3.1/colbert/infra/run.py
-drwxr-xr-x   0 eyang     (1795) staff    (20063)        0 2024-02-27 23:24:02.559861 PLAID-X-0.3.1/colbert/modeling/
--rw-r--r--   0 eyang     (1795) staff    (20063)        0 2023-12-28 04:23:43.000000 PLAID-X-0.3.1/colbert/modeling/__init__.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     3747 2024-02-14 22:45:43.000000 PLAID-X-0.3.1/colbert/modeling/base_colbert.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     5284 2023-12-28 04:23:43.000000 PLAID-X-0.3.1/colbert/modeling/checkpoint.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     8619 2024-02-14 22:45:43.000000 PLAID-X-0.3.1/colbert/modeling/colbert.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     6873 2023-12-28 04:23:43.000000 PLAID-X-0.3.1/colbert/modeling/hf_colbert.py
-drwxr-xr-x   0 eyang     (1795) staff    (20063)        0 2024-02-27 23:24:02.591862 PLAID-X-0.3.1/colbert/modeling/reranker/
--rw-r--r--   0 eyang     (1795) staff    (20063)        0 2023-12-28 04:23:43.000000 PLAID-X-0.3.1/colbert/modeling/reranker/__init__.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     1272 2023-12-28 04:23:43.000000 PLAID-X-0.3.1/colbert/modeling/reranker/electra.py
--rw-r--r--   0 eyang     (1795) staff    (20063)      608 2023-12-28 04:23:43.000000 PLAID-X-0.3.1/colbert/modeling/reranker/tokenizer.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     2782 2023-12-28 04:23:43.000000 PLAID-X-0.3.1/colbert/modeling/segmented_maxsim.cpp
-drwxr-xr-x   0 eyang     (1795) staff    (20063)        0 2024-02-27 23:24:02.601851 PLAID-X-0.3.1/colbert/modeling/tokenization/
--rw-r--r--   0 eyang     (1795) staff    (20063)      190 2023-12-28 04:23:43.000000 PLAID-X-0.3.1/colbert/modeling/tokenization/__init__.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     2460 2023-12-28 04:23:43.000000 PLAID-X-0.3.1/colbert/modeling/tokenization/doc_tokenization.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     3976 2023-12-28 04:23:43.000000 PLAID-X-0.3.1/colbert/modeling/tokenization/query_tokenization.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     3499 2024-02-14 22:45:43.000000 PLAID-X-0.3.1/colbert/modeling/tokenization/utils.py
--rw-r--r--   0 eyang     (1795) staff    (20063)      551 2024-02-14 22:45:43.000000 PLAID-X-0.3.1/colbert/parameters.py
-drwxr-xr-x   0 eyang     (1795) staff    (20063)        0 2024-02-27 23:24:02.603863 PLAID-X-0.3.1/colbert/ranking/
--rw-r--r--   0 eyang     (1795) staff    (20063)        0 2023-12-28 04:23:44.000000 PLAID-X-0.3.1/colbert/ranking/__init__.py
-drwxr-xr-x   0 eyang     (1795) staff    (20063)        0 2024-02-27 23:24:02.644857 PLAID-X-0.3.1/colbert/scripts/
--rw-r--r--   0 eyang     (1795) staff    (20063)        0 2024-02-27 19:59:32.000000 PLAID-X-0.3.1/colbert/scripts/__init__.py
--rw-r--r--   0 eyang     (1795) staff    (20063)    11349 2024-02-27 22:02:39.000000 PLAID-X-0.3.1/colbert/scripts/collection_utils.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     4415 2024-02-27 20:47:27.000000 PLAID-X-0.3.1/colbert/scripts/index.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     4744 2024-02-27 20:47:46.000000 PLAID-X-0.3.1/colbert/scripts/search.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     4835 2024-02-27 21:34:52.000000 PLAID-X-0.3.1/colbert/scripts/train.py
-drwxr-xr-x   0 eyang     (1795) staff    (20063)        0 2024-02-27 23:24:02.723860 PLAID-X-0.3.1/colbert/search/
--rw-r--r--   0 eyang     (1795) staff    (20063)        0 2023-12-28 04:23:44.000000 PLAID-X-0.3.1/colbert/search/__init__.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     1984 2023-12-28 04:23:44.000000 PLAID-X-0.3.1/colbert/search/candidate_generation.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     5844 2023-12-28 04:23:44.000000 PLAID-X-0.3.1/colbert/search/decompress_residuals.cpp
--rw-r--r--   0 eyang     (1795) staff    (20063)     5678 2023-12-28 04:23:44.000000 PLAID-X-0.3.1/colbert/search/filter_pids.cpp
--rw-r--r--   0 eyang     (1795) staff    (20063)     2950 2023-12-28 04:23:44.000000 PLAID-X-0.3.1/colbert/search/index_loader.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     7915 2024-02-14 22:45:43.000000 PLAID-X-0.3.1/colbert/search/index_storage.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     4455 2023-12-28 04:23:44.000000 PLAID-X-0.3.1/colbert/search/segmented_lookup.cpp
--rw-r--r--   0 eyang     (1795) staff    (20063)     7058 2023-12-28 04:23:44.000000 PLAID-X-0.3.1/colbert/search/strided_tensor.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     4157 2023-12-28 04:23:44.000000 PLAID-X-0.3.1/colbert/search/strided_tensor_core.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     4633 2024-02-14 22:45:43.000000 PLAID-X-0.3.1/colbert/searcher.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     1346 2024-02-14 22:45:43.000000 PLAID-X-0.3.1/colbert/trainer.py
-drwxr-xr-x   0 eyang     (1795) staff    (20063)        0 2024-02-27 23:24:02.880854 PLAID-X-0.3.1/colbert/training/
--rw-r--r--   0 eyang     (1795) staff    (20063)        0 2023-12-28 04:23:44.000000 PLAID-X-0.3.1/colbert/training/__init__.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     2018 2023-12-28 04:23:44.000000 PLAID-X-0.3.1/colbert/training/eager_batcher.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     5570 2024-02-14 22:45:43.000000 PLAID-X-0.3.1/colbert/training/lazy_batcher.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     5920 2024-02-14 22:45:43.000000 PLAID-X-0.3.1/colbert/training/legacy_training.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     2610 2023-12-28 04:23:44.000000 PLAID-X-0.3.1/colbert/training/rerank_batcher.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     9156 2024-02-27 21:10:53.000000 PLAID-X-0.3.1/colbert/training/training.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     3414 2024-02-14 22:45:43.000000 PLAID-X-0.3.1/colbert/training/utils.py
-drwxr-xr-x   0 eyang     (1795) staff    (20063)        0 2024-02-27 23:24:02.925868 PLAID-X-0.3.1/colbert/utils/
--rw-r--r--   0 eyang     (1795) staff    (20063)        0 2023-12-28 04:23:44.000000 PLAID-X-0.3.1/colbert/utils/__init__.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     1058 2023-12-28 04:23:44.000000 PLAID-X-0.3.1/colbert/utils/amp.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     1050 2023-12-28 04:23:44.000000 PLAID-X-0.3.1/colbert/utils/distributed.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     3315 2023-12-28 04:23:44.000000 PLAID-X-0.3.1/colbert/utils/logging.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     5380 2023-12-28 04:23:44.000000 PLAID-X-0.3.1/colbert/utils/parser.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     3467 2023-12-28 04:23:44.000000 PLAID-X-0.3.1/colbert/utils/runs.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     1930 2024-02-14 22:46:32.000000 PLAID-X-0.3.1/colbert/utils/save_metadata.py
--rw-r--r--   0 eyang     (1795) staff    (20063)     8371 2024-02-27 21:21:23.000000 PLAID-X-0.3.1/colbert/utils/utils.py
--rw-r--r--   0 eyang     (1795) staff    (20063)      147 2024-02-27 20:56:48.000000 PLAID-X-0.3.1/requirements.txt
--rw-r--r--   0 eyang     (1795) staff    (20063)       38 2024-02-27 23:24:03.014877 PLAID-X-0.3.1/setup.cfg
--rw-r--r--   0 eyang     (1795) staff    (20063)      650 2024-02-27 23:22:57.000000 PLAID-X-0.3.1/setup.py
+drwxr-xr-x   0 eyang     (1795) staff    (20063)        0 2024-05-06 03:42:04.660933 plaid_x-0.3.1a0/
+-rw-r--r--   0 eyang     (1795) staff    (20063)     1091 2023-12-28 04:23:43.000000 plaid_x-0.3.1a0/LICENSE
+-rw-r--r--   0 eyang     (1795) staff    (20063)      191 2024-05-06 03:30:30.000000 plaid_x-0.3.1a0/MANIFEST.in
+-rw-r--r--   0 eyang     (1795) staff    (20063)     7539 2024-05-06 03:42:04.634933 plaid_x-0.3.1a0/PKG-INFO
+drwxr-xr-x   0 eyang     (1795) staff    (20063)        0 2024-05-06 03:42:04.630938 plaid_x-0.3.1a0/PLAID_X.egg-info/
+-rw-r--r--   0 eyang     (1795) staff    (20063)     7539 2024-05-06 03:42:03.000000 plaid_x-0.3.1a0/PLAID_X.egg-info/PKG-INFO
+-rw-r--r--   0 eyang     (1795) staff    (20063)     2798 2024-05-06 03:42:03.000000 plaid_x-0.3.1a0/PLAID_X.egg-info/SOURCES.txt
+-rw-r--r--   0 eyang     (1795) staff    (20063)        1 2024-05-06 03:42:03.000000 plaid_x-0.3.1a0/PLAID_X.egg-info/dependency_links.txt
+-rw-r--r--   0 eyang     (1795) staff    (20063)      148 2024-05-06 03:42:03.000000 plaid_x-0.3.1a0/PLAID_X.egg-info/requires.txt
+-rw-r--r--   0 eyang     (1795) staff    (20063)        7 2024-05-06 03:42:03.000000 plaid_x-0.3.1a0/PLAID_X.egg-info/top_level.txt
+-rw-r--r--   0 eyang     (1795) staff    (20063)     6787 2024-05-06 03:31:02.000000 plaid_x-0.3.1a0/README.md
+drwxr-xr-x   0 eyang     (1795) staff    (20063)        0 2024-05-06 03:42:03.927945 plaid_x-0.3.1a0/plaidx/
+-rw-r--r--   0 eyang     (1795) staff    (20063)      199 2024-05-06 03:30:01.000000 plaid_x-0.3.1a0/plaidx/__init__.py
+drwxr-xr-x   0 eyang     (1795) staff    (20063)        0 2024-05-06 03:42:03.957942 plaid_x-0.3.1a0/plaidx/data/
+-rw-r--r--   0 eyang     (1795) staff    (20063)       97 2023-12-28 04:23:43.000000 plaid_x-0.3.1a0/plaidx/data/__init__.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     3356 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/data/collection.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)      421 2023-12-28 04:23:43.000000 plaid_x-0.3.1a0/plaidx/data/dataset.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     3594 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/data/examples.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     4395 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/data/queries.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     2770 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/data/ranking.py
+drwxr-xr-x   0 eyang     (1795) staff    (20063)        0 2024-05-06 03:42:03.977945 plaid_x-0.3.1a0/plaidx/evaluation/
+-rw-r--r--   0 eyang     (1795) staff    (20063)        0 2023-12-28 04:23:43.000000 plaid_x-0.3.1a0/plaidx/evaluation/__init__.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)      916 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/evaluation/load_model.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     6645 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/evaluation/loaders.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     4303 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/evaluation/metrics.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)      286 2023-12-28 04:23:43.000000 plaid_x-0.3.1a0/plaidx/index.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)    20056 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/index_updater.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     4635 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/indexer.py
+drwxr-xr-x   0 eyang     (1795) staff    (20063)        0 2024-05-06 03:42:04.058941 plaid_x-0.3.1a0/plaidx/indexing/
+-rw-r--r--   0 eyang     (1795) staff    (20063)        0 2023-12-28 04:23:43.000000 plaid_x-0.3.1a0/plaidx/indexing/__init__.py
+drwxr-xr-x   0 eyang     (1795) staff    (20063)        0 2024-05-06 03:42:04.108942 plaid_x-0.3.1a0/plaidx/indexing/codecs/
+-rw-r--r--   0 eyang     (1795) staff    (20063)        0 2023-12-28 04:23:43.000000 plaid_x-0.3.1a0/plaidx/indexing/codecs/__init__.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)      982 2023-12-28 04:23:43.000000 plaid_x-0.3.1a0/plaidx/indexing/codecs/decompress_residuals.cpp
+-rw-r--r--   0 eyang     (1795) staff    (20063)     3014 2023-12-28 04:23:43.000000 plaid_x-0.3.1a0/plaidx/indexing/codecs/decompress_residuals.cu
+-rw-r--r--   0 eyang     (1795) staff    (20063)      284 2023-12-28 04:23:43.000000 plaid_x-0.3.1a0/plaidx/indexing/codecs/packbits.cpp
+-rw-r--r--   0 eyang     (1795) staff    (20063)     1558 2023-12-28 04:23:43.000000 plaid_x-0.3.1a0/plaidx/indexing/codecs/packbits.cu
+-rw-r--r--   0 eyang     (1795) staff    (20063)    10912 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/indexing/codecs/residual.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     3190 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/indexing/codecs/residual_embeddings.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     1732 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/indexing/codecs/residual_embeddings_strided.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     1821 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/indexing/collection_encoder.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)    32996 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/indexing/collection_indexer.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)      878 2023-12-28 04:23:43.000000 plaid_x-0.3.1a0/plaidx/indexing/index_manager.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     2898 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/indexing/index_saver.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     1995 2023-12-28 04:23:43.000000 plaid_x-0.3.1a0/plaidx/indexing/loaders.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     1824 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/indexing/utils.py
+drwxr-xr-x   0 eyang     (1795) staff    (20063)        0 2024-05-06 03:42:04.124942 plaid_x-0.3.1a0/plaidx/infra/
+-rw-r--r--   0 eyang     (1795) staff    (20063)       40 2023-12-28 04:23:43.000000 plaid_x-0.3.1a0/plaidx/infra/__init__.py
+drwxr-xr-x   0 eyang     (1795) staff    (20063)        0 2024-05-06 03:42:04.157947 plaid_x-0.3.1a0/plaidx/infra/config/
+-rw-r--r--   0 eyang     (1795) staff    (20063)       45 2023-12-28 04:23:43.000000 plaid_x-0.3.1a0/plaidx/infra/config/__init__.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     4129 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/infra/config/base_config.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)      364 2023-12-28 04:23:43.000000 plaid_x-0.3.1a0/plaidx/infra/config/config.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     2221 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/infra/config/core_config.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     5272 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/infra/config/settings.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     4607 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/infra/launcher.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)      932 2023-12-28 04:23:43.000000 plaid_x-0.3.1a0/plaidx/infra/provenance.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     2553 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/infra/run.py
+drwxr-xr-x   0 eyang     (1795) staff    (20063)        0 2024-05-06 03:42:04.188939 plaid_x-0.3.1a0/plaidx/modeling/
+-rw-r--r--   0 eyang     (1795) staff    (20063)        0 2023-12-28 04:23:43.000000 plaid_x-0.3.1a0/plaidx/modeling/__init__.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     3741 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/modeling/base_colbert.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     5281 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/modeling/checkpoint.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     8615 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/modeling/colbert.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     6871 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/modeling/hf_colbert.py
+drwxr-xr-x   0 eyang     (1795) staff    (20063)        0 2024-05-06 03:42:04.210943 plaid_x-0.3.1a0/plaidx/modeling/reranker/
+-rw-r--r--   0 eyang     (1795) staff    (20063)        0 2023-12-28 04:23:43.000000 plaid_x-0.3.1a0/plaidx/modeling/reranker/__init__.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     1272 2023-12-28 04:23:43.000000 plaid_x-0.3.1a0/plaidx/modeling/reranker/electra.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)      608 2023-12-28 04:23:43.000000 plaid_x-0.3.1a0/plaidx/modeling/reranker/tokenizer.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     2782 2023-12-28 04:23:43.000000 plaid_x-0.3.1a0/plaidx/modeling/segmented_maxsim.cpp
+drwxr-xr-x   0 eyang     (1795) staff    (20063)        0 2024-05-06 03:42:04.239940 plaid_x-0.3.1a0/plaidx/modeling/tokenization/
+-rw-r--r--   0 eyang     (1795) staff    (20063)      187 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/modeling/tokenization/__init__.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     2457 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/modeling/tokenization/doc_tokenization.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     3972 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/modeling/tokenization/query_tokenization.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     3499 2024-02-14 22:45:43.000000 plaid_x-0.3.1a0/plaidx/modeling/tokenization/utils.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)      551 2024-02-14 22:45:43.000000 plaid_x-0.3.1a0/plaidx/parameters.py
+drwxr-xr-x   0 eyang     (1795) staff    (20063)        0 2024-05-06 03:42:04.334937 plaid_x-0.3.1a0/plaidx/ranking/
+-rw-r--r--   0 eyang     (1795) staff    (20063)        0 2023-12-28 04:23:44.000000 plaid_x-0.3.1a0/plaidx/ranking/__init__.py
+drwxr-xr-x   0 eyang     (1795) staff    (20063)        0 2024-05-06 03:42:04.407939 plaid_x-0.3.1a0/plaidx/scripts/
+-rw-r--r--   0 eyang     (1795) staff    (20063)        0 2024-03-05 03:46:59.000000 plaid_x-0.3.1a0/plaidx/scripts/__init__.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)    14342 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/scripts/collection_utils.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     4489 2024-05-06 03:28:01.000000 plaid_x-0.3.1a0/plaidx/scripts/index.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     5067 2024-05-06 03:28:07.000000 plaid_x-0.3.1a0/plaidx/scripts/search.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     3360 2024-04-30 21:06:24.000000 plaid_x-0.3.1a0/plaidx/scripts/shirttt_utils.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     5780 2024-05-06 03:28:11.000000 plaid_x-0.3.1a0/plaidx/scripts/train.py
+drwxr-xr-x   0 eyang     (1795) staff    (20063)        0 2024-05-06 03:42:04.462937 plaid_x-0.3.1a0/plaidx/search/
+-rw-r--r--   0 eyang     (1795) staff    (20063)        0 2023-12-28 04:23:44.000000 plaid_x-0.3.1a0/plaidx/search/__init__.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     1983 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/search/candidate_generation.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     5844 2023-12-28 04:23:44.000000 plaid_x-0.3.1a0/plaidx/search/decompress_residuals.cpp
+-rw-r--r--   0 eyang     (1795) staff    (20063)     5678 2023-12-28 04:23:44.000000 plaid_x-0.3.1a0/plaidx/search/filter_pids.cpp
+-rw-r--r--   0 eyang     (1795) staff    (20063)     2946 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/search/index_loader.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     7909 2024-05-06 03:17:18.000000 plaid_x-0.3.1a0/plaidx/search/index_storage.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     4455 2023-12-28 04:23:44.000000 plaid_x-0.3.1a0/plaidx/search/segmented_lookup.cpp
+-rw-r--r--   0 eyang     (1795) staff    (20063)     7057 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/search/strided_tensor.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     4156 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/search/strided_tensor_core.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     4626 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/searcher.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     1341 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/trainer.py
+drwxr-xr-x   0 eyang     (1795) staff    (20063)        0 2024-05-06 03:42:04.569936 plaid_x-0.3.1a0/plaidx/training/
+-rw-r--r--   0 eyang     (1795) staff    (20063)        0 2023-12-28 04:23:44.000000 plaid_x-0.3.1a0/plaidx/training/__init__.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     2015 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/training/eager_batcher.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     5562 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/training/lazy_batcher.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     5912 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/training/legacy_training.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     2603 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/training/rerank_batcher.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     9147 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/training/training.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     3409 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/training/utils.py
+drwxr-xr-x   0 eyang     (1795) staff    (20063)        0 2024-05-06 03:42:04.628934 plaid_x-0.3.1a0/plaidx/utils/
+-rw-r--r--   0 eyang     (1795) staff    (20063)        0 2023-12-28 04:23:44.000000 plaid_x-0.3.1a0/plaidx/utils/__init__.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     1057 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/utils/amp.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     1050 2023-12-28 04:23:44.000000 plaid_x-0.3.1a0/plaidx/utils/distributed.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     3314 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/utils/logging.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     5377 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/utils/parser.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     3464 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/utils/runs.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     1929 2024-05-06 02:59:36.000000 plaid_x-0.3.1a0/plaidx/utils/save_metadata.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)     8371 2024-03-05 03:46:59.000000 plaid_x-0.3.1a0/plaidx/utils/utils.py
+-rw-r--r--   0 eyang     (1795) staff    (20063)      147 2024-03-05 03:46:59.000000 plaid_x-0.3.1a0/requirements.txt
+-rw-r--r--   0 eyang     (1795) staff    (20063)       38 2024-05-06 03:42:04.661934 plaid_x-0.3.1a0/setup.cfg
+-rw-r--r--   0 eyang     (1795) staff    (20063)      926 2024-05-06 03:30:23.000000 plaid_x-0.3.1a0/setup.py
```

### Comparing `PLAID-X-0.3.1/LICENSE` & `plaid_x-0.3.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `PLAID-X-0.3.1/PKG-INFO` & `plaid_x-0.3.1a0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PLAID-X
-Version: 0.3.1
+Version: 0.3.1a0
 Summary: Efficient and Effective Passage Search via Contextualized Late Interaction over BERT and XLM-RoBERTa
 Home-page: https://github.com/hltcoe/ColBERT-X/tree/plaid-x
 Author: Eugene Yang
 Author-email: eugene.yang@jhu.edu
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -21,19 +21,26 @@
 Requires-Dist: tqdm
 Requires-Dist: transformers
 Requires-Dist: ujson
 Requires-Dist: more_itertools
 Requires-Dist: ir_datasets
 Requires-Dist: ir_measures
 
+This is the alpha branch for changing the namespace of the package from `colbert` to `plaidx`. 
+
 # PLAID-X
 
 This is a generalized version of [PLAID](https://github.com/stanford-futuredata/ColBERT) and the previous ColBERT-X for CLIR.
 The codebase supports models trained with the original ColBERT-X scripts, which are not compatible with the PLAID codebase released from the Stadford Futuredata Group. 
 
+## Resources
+
+We release a set of CLIR models in our [Translate-Distill Huggingface Space](https://huggingface.co/collections/eugene-yang/translate-distill-658ccc3b38672a848bd53d74). 
+Feel free to try it out! 
+
 ## Installation
 
 PLAID-X is available on PyPi. You can install it through
 ```bash
 pip install PLAID-X
 ```
 
@@ -48,45 +55,48 @@
 The following provides a series of CLI commands for running a larger scale. 
 
 ### Training Models
 
 The following command starts the training process using the `t53b-monot5-msmarco-engeng.jsonl.gz` triple file on the Huggingface Dataset repository [`hltcoe/tdist-msmarco-scores`](https://huggingface.co/datasets/hltcoe/tdist-msmarco-scores) with English queries and translated Chinese passages from [neuMARCO](https://ir-datasets.com/neumarco.html).
 
 ```bash
-python -m colbert.scripts.train \
+python -m plaidx.scripts.train \
 --model_name xlm-roberta-large \
 --training_triples hltcoe/tdist-msmarco-scores:t53b-monot5-msmarco-engeng.jsonl.gz \
 --training_irds_id neumarco/zh/train \
 --maxsteps 200000 \
 --learning_rate 5e-6 \
 --kd_loss KLD \
 --only_top \
 --per_device_batch_size 8 \
 --nway 6 \
 --run_tag test \
 --experiment test
 ```
 
+For training MLIR models using Multilingual Translate-Distill, pass more multiple dataset ids to `--training_irds_id` flag along with a `--training_collection_mixing` for the mixing strategies (one of `entries`, `passages`, or `round-robin`). 
+For more details, please read our paper **Distillation for Multilingual Information Retrieval**(arxiv link TBD).
+
 ### Indexing 
 
 Since PLAID-X is a passage retrieval engine, you need to create passage collections if you are intended to search a document collection.
 The following command creates a passage collection for the NeuCLIR1 Chinese corpus (file implicitly downloaded from Huggingface). 
 
 ```bash
-python -m colbert.scripts.collection_utils create_passage_collection \
+python -m plaidx.scripts.collection_utils create_passage_collection \
 --root ./test_coll/ --corpus neuclir/neuclir1:data/zho-00000-of-00001.jsonl.gz
 ```
 
 The indexing processes is broken into **three** steps. 
 This is changed from the last version where we have two steps and also different from the original Stanford codebase where they combines everything into one Python call.
 Separating the steps provides better allocation for the computation resources and avoid bad GPU reservation deadlocks between Pytorch and FAISS.
 
 ```bash
 for step in prepare encode finalize; do
-python -m colbert.scripts.index \
+python -m plaidx.scripts.index \
 --coll_dir ./test_coll \
 --index_name test_index \
 --dataset_name test_coll \
 --nbits 1 \
 --step $step \
 --checkpoint eugene-yang/plaidx-xlmr-large-mlir-neuclir \
 --experiment test 
@@ -95,23 +105,33 @@
 Note that the `--checkpoint` flag accept ColBERT-X and ColBERT models stored on Huggingface Models.
 
 ### Searching 
 
 Finally, the following command searches the collection with a query `.tsv` file where the first column is the query id and the second column contains the query text. 
 
 ```bash
-python -m colbert.scripts.search \
+python -m plaidx.scripts.search \
 --index_name neuclir-zho.1bits \
 --passage_mapping ./test_coll/mapping.tsv \
 --query_file query.tsv \
 --metrics nDCG@20 MAP R@100 R@1000 Judged@10 \
 --qrel qrels.txt \
 --experiment test
 ```
 
+### PLAID SHIRTTT Indexing
+
+For replicating PLAID SHIRTTT experiments, we have released the 
+[date of each document in NeuCLIR1 and ClueWeb09 on Huggingface](https://huggingface.co/datasets/hltcoe/plaid-shirttt-doc-date). 
+To combine the ranks lists from each shard, you can use the following utility script to do so. 
+
+```bash
+python -m plaidx.scripts.shirttt_utils --input {ranking files from each shard} --output {file to write} --topn 50 
+```
+
 ## Citation and Credit
 
 Please cite the following paper if you use the CLIR generalization of ColBERT.
 ```bibtex
 @inproceedings{ecir2022colbert-x,
 	author = {Suraj Nair and Eugene Yang and Dawn Lawrie and Kevin Duh and Paul McNamee and Kenton Murray and James Mayfield and Douglas W. Oard},
 	title = {Transfer Learning Approaches for Building Cross-Language Dense Retrieval Models},
@@ -138,7 +158,27 @@
   author = {Eugene Yang and Dawn Lawrie and James Mayfield and Douglas W. Oard and Scott Miller},
   title = {Translate-Distill: Learning Cross-Language Dense Retrieval by Translation and Distillation},
   booktitle = {Proceedings of the 46th European Conference on Information Retrieval (ECIR)},
   year = {2024},
   url = {https://arxiv.org/abs/2401.04810}
 }
 ```
+
+Please cite the following paper if you use **Multilingual Translate-Distill** to train MLIR model. 
+```bibtex
+@inproceedings{sigir2024shirttt,
+  author = {Eugene Yang and Dawn Lawrie and James Mayfield},
+  title = {Distillation for Multilingual Information Retrieval},
+  booktitle = {Proceedings of the 47th International ACM SIGIR Conference on Research and Development in Information Retrieval (SIGIR ’24)},
+  year = {2024}
+}
+```
+
+Please cite the following paper if you use PLAID SHIRTTT. 
+```bibtex
+@inproceedings{sigir2024shirttt,
+  author = {Dawn Lawrie and Efsun Kayi and Eugene Yang and James Mayfield and Douglas W. Oard},
+  title = {PLAID SHIRTTT for Large-Scale Streaming Dense Retrieval},
+  booktitle = {Proceedings of the 47th International ACM SIGIR Conference on Research and Development in Information Retrieval (SIGIR ’24)},
+  year = {2024}
+}
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `PLAID-X-0.3.1/PLAID_X.egg-info/PKG-INFO` & `plaid_x-0.3.1a0/PLAID_X.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PLAID-X
-Version: 0.3.1
+Version: 0.3.1a0
 Summary: Efficient and Effective Passage Search via Contextualized Late Interaction over BERT and XLM-RoBERTa
 Home-page: https://github.com/hltcoe/ColBERT-X/tree/plaid-x
 Author: Eugene Yang
 Author-email: eugene.yang@jhu.edu
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -21,19 +21,26 @@
 Requires-Dist: tqdm
 Requires-Dist: transformers
 Requires-Dist: ujson
 Requires-Dist: more_itertools
 Requires-Dist: ir_datasets
 Requires-Dist: ir_measures
 
+This is the alpha branch for changing the namespace of the package from `colbert` to `plaidx`. 
+
 # PLAID-X
 
 This is a generalized version of [PLAID](https://github.com/stanford-futuredata/ColBERT) and the previous ColBERT-X for CLIR.
 The codebase supports models trained with the original ColBERT-X scripts, which are not compatible with the PLAID codebase released from the Stadford Futuredata Group. 
 
+## Resources
+
+We release a set of CLIR models in our [Translate-Distill Huggingface Space](https://huggingface.co/collections/eugene-yang/translate-distill-658ccc3b38672a848bd53d74). 
+Feel free to try it out! 
+
 ## Installation
 
 PLAID-X is available on PyPi. You can install it through
 ```bash
 pip install PLAID-X
 ```
 
@@ -48,45 +55,48 @@
 The following provides a series of CLI commands for running a larger scale. 
 
 ### Training Models
 
 The following command starts the training process using the `t53b-monot5-msmarco-engeng.jsonl.gz` triple file on the Huggingface Dataset repository [`hltcoe/tdist-msmarco-scores`](https://huggingface.co/datasets/hltcoe/tdist-msmarco-scores) with English queries and translated Chinese passages from [neuMARCO](https://ir-datasets.com/neumarco.html).
 
 ```bash
-python -m colbert.scripts.train \
+python -m plaidx.scripts.train \
 --model_name xlm-roberta-large \
 --training_triples hltcoe/tdist-msmarco-scores:t53b-monot5-msmarco-engeng.jsonl.gz \
 --training_irds_id neumarco/zh/train \
 --maxsteps 200000 \
 --learning_rate 5e-6 \
 --kd_loss KLD \
 --only_top \
 --per_device_batch_size 8 \
 --nway 6 \
 --run_tag test \
 --experiment test
 ```
 
+For training MLIR models using Multilingual Translate-Distill, pass more multiple dataset ids to `--training_irds_id` flag along with a `--training_collection_mixing` for the mixing strategies (one of `entries`, `passages`, or `round-robin`). 
+For more details, please read our paper **Distillation for Multilingual Information Retrieval**(arxiv link TBD).
+
 ### Indexing 
 
 Since PLAID-X is a passage retrieval engine, you need to create passage collections if you are intended to search a document collection.
 The following command creates a passage collection for the NeuCLIR1 Chinese corpus (file implicitly downloaded from Huggingface). 
 
 ```bash
-python -m colbert.scripts.collection_utils create_passage_collection \
+python -m plaidx.scripts.collection_utils create_passage_collection \
 --root ./test_coll/ --corpus neuclir/neuclir1:data/zho-00000-of-00001.jsonl.gz
 ```
 
 The indexing processes is broken into **three** steps. 
 This is changed from the last version where we have two steps and also different from the original Stanford codebase where they combines everything into one Python call.
 Separating the steps provides better allocation for the computation resources and avoid bad GPU reservation deadlocks between Pytorch and FAISS.
 
 ```bash
 for step in prepare encode finalize; do
-python -m colbert.scripts.index \
+python -m plaidx.scripts.index \
 --coll_dir ./test_coll \
 --index_name test_index \
 --dataset_name test_coll \
 --nbits 1 \
 --step $step \
 --checkpoint eugene-yang/plaidx-xlmr-large-mlir-neuclir \
 --experiment test 
@@ -95,23 +105,33 @@
 Note that the `--checkpoint` flag accept ColBERT-X and ColBERT models stored on Huggingface Models.
 
 ### Searching 
 
 Finally, the following command searches the collection with a query `.tsv` file where the first column is the query id and the second column contains the query text. 
 
 ```bash
-python -m colbert.scripts.search \
+python -m plaidx.scripts.search \
 --index_name neuclir-zho.1bits \
 --passage_mapping ./test_coll/mapping.tsv \
 --query_file query.tsv \
 --metrics nDCG@20 MAP R@100 R@1000 Judged@10 \
 --qrel qrels.txt \
 --experiment test
 ```
 
+### PLAID SHIRTTT Indexing
+
+For replicating PLAID SHIRTTT experiments, we have released the 
+[date of each document in NeuCLIR1 and ClueWeb09 on Huggingface](https://huggingface.co/datasets/hltcoe/plaid-shirttt-doc-date). 
+To combine the ranks lists from each shard, you can use the following utility script to do so. 
+
+```bash
+python -m plaidx.scripts.shirttt_utils --input {ranking files from each shard} --output {file to write} --topn 50 
+```
+
 ## Citation and Credit
 
 Please cite the following paper if you use the CLIR generalization of ColBERT.
 ```bibtex
 @inproceedings{ecir2022colbert-x,
 	author = {Suraj Nair and Eugene Yang and Dawn Lawrie and Kevin Duh and Paul McNamee and Kenton Murray and James Mayfield and Douglas W. Oard},
 	title = {Transfer Learning Approaches for Building Cross-Language Dense Retrieval Models},
@@ -138,7 +158,27 @@
   author = {Eugene Yang and Dawn Lawrie and James Mayfield and Douglas W. Oard and Scott Miller},
   title = {Translate-Distill: Learning Cross-Language Dense Retrieval by Translation and Distillation},
   booktitle = {Proceedings of the 46th European Conference on Information Retrieval (ECIR)},
   year = {2024},
   url = {https://arxiv.org/abs/2401.04810}
 }
 ```
+
+Please cite the following paper if you use **Multilingual Translate-Distill** to train MLIR model. 
+```bibtex
+@inproceedings{sigir2024shirttt,
+  author = {Eugene Yang and Dawn Lawrie and James Mayfield},
+  title = {Distillation for Multilingual Information Retrieval},
+  booktitle = {Proceedings of the 47th International ACM SIGIR Conference on Research and Development in Information Retrieval (SIGIR ’24)},
+  year = {2024}
+}
+```
+
+Please cite the following paper if you use PLAID SHIRTTT. 
+```bibtex
+@inproceedings{sigir2024shirttt,
+  author = {Dawn Lawrie and Efsun Kayi and Eugene Yang and James Mayfield and Douglas W. Oard},
+  title = {PLAID SHIRTTT for Large-Scale Streaming Dense Retrieval},
+  booktitle = {Proceedings of the 47th International ACM SIGIR Conference on Research and Development in Information Retrieval (SIGIR ’24)},
+  year = {2024}
+}
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `PLAID-X-0.3.1/README.md` & `plaid_x-0.3.1a0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,19 @@
+This is the alpha branch for changing the namespace of the package from `colbert` to `plaidx`. 
+
 # PLAID-X
 
 This is a generalized version of [PLAID](https://github.com/stanford-futuredata/ColBERT) and the previous ColBERT-X for CLIR.
 The codebase supports models trained with the original ColBERT-X scripts, which are not compatible with the PLAID codebase released from the Stadford Futuredata Group. 
 
+## Resources
+
+We release a set of CLIR models in our [Translate-Distill Huggingface Space](https://huggingface.co/collections/eugene-yang/translate-distill-658ccc3b38672a848bd53d74). 
+Feel free to try it out! 
+
 ## Installation
 
 PLAID-X is available on PyPi. You can install it through
 ```bash
 pip install PLAID-X
 ```
 
@@ -21,45 +28,48 @@
 The following provides a series of CLI commands for running a larger scale. 
 
 ### Training Models
 
 The following command starts the training process using the `t53b-monot5-msmarco-engeng.jsonl.gz` triple file on the Huggingface Dataset repository [`hltcoe/tdist-msmarco-scores`](https://huggingface.co/datasets/hltcoe/tdist-msmarco-scores) with English queries and translated Chinese passages from [neuMARCO](https://ir-datasets.com/neumarco.html).
 
 ```bash
-python -m colbert.scripts.train \
+python -m plaidx.scripts.train \
 --model_name xlm-roberta-large \
 --training_triples hltcoe/tdist-msmarco-scores:t53b-monot5-msmarco-engeng.jsonl.gz \
 --training_irds_id neumarco/zh/train \
 --maxsteps 200000 \
 --learning_rate 5e-6 \
 --kd_loss KLD \
 --only_top \
 --per_device_batch_size 8 \
 --nway 6 \
 --run_tag test \
 --experiment test
 ```
 
+For training MLIR models using Multilingual Translate-Distill, pass more multiple dataset ids to `--training_irds_id` flag along with a `--training_collection_mixing` for the mixing strategies (one of `entries`, `passages`, or `round-robin`). 
+For more details, please read our paper **Distillation for Multilingual Information Retrieval**(arxiv link TBD).
+
 ### Indexing 
 
 Since PLAID-X is a passage retrieval engine, you need to create passage collections if you are intended to search a document collection.
 The following command creates a passage collection for the NeuCLIR1 Chinese corpus (file implicitly downloaded from Huggingface). 
 
 ```bash
-python -m colbert.scripts.collection_utils create_passage_collection \
+python -m plaidx.scripts.collection_utils create_passage_collection \
 --root ./test_coll/ --corpus neuclir/neuclir1:data/zho-00000-of-00001.jsonl.gz
 ```
 
 The indexing processes is broken into **three** steps. 
 This is changed from the last version where we have two steps and also different from the original Stanford codebase where they combines everything into one Python call.
 Separating the steps provides better allocation for the computation resources and avoid bad GPU reservation deadlocks between Pytorch and FAISS.
 
 ```bash
 for step in prepare encode finalize; do
-python -m colbert.scripts.index \
+python -m plaidx.scripts.index \
 --coll_dir ./test_coll \
 --index_name test_index \
 --dataset_name test_coll \
 --nbits 1 \
 --step $step \
 --checkpoint eugene-yang/plaidx-xlmr-large-mlir-neuclir \
 --experiment test 
@@ -68,23 +78,33 @@
 Note that the `--checkpoint` flag accept ColBERT-X and ColBERT models stored on Huggingface Models.
 
 ### Searching 
 
 Finally, the following command searches the collection with a query `.tsv` file where the first column is the query id and the second column contains the query text. 
 
 ```bash
-python -m colbert.scripts.search \
+python -m plaidx.scripts.search \
 --index_name neuclir-zho.1bits \
 --passage_mapping ./test_coll/mapping.tsv \
 --query_file query.tsv \
 --metrics nDCG@20 MAP R@100 R@1000 Judged@10 \
 --qrel qrels.txt \
 --experiment test
 ```
 
+### PLAID SHIRTTT Indexing
+
+For replicating PLAID SHIRTTT experiments, we have released the 
+[date of each document in NeuCLIR1 and ClueWeb09 on Huggingface](https://huggingface.co/datasets/hltcoe/plaid-shirttt-doc-date). 
+To combine the ranks lists from each shard, you can use the following utility script to do so. 
+
+```bash
+python -m plaidx.scripts.shirttt_utils --input {ranking files from each shard} --output {file to write} --topn 50 
+```
+
 ## Citation and Credit
 
 Please cite the following paper if you use the CLIR generalization of ColBERT.
 ```bibtex
 @inproceedings{ecir2022colbert-x,
 	author = {Suraj Nair and Eugene Yang and Dawn Lawrie and Kevin Duh and Paul McNamee and Kenton Murray and James Mayfield and Douglas W. Oard},
 	title = {Transfer Learning Approaches for Building Cross-Language Dense Retrieval Models},
@@ -111,7 +131,27 @@
   author = {Eugene Yang and Dawn Lawrie and James Mayfield and Douglas W. Oard and Scott Miller},
   title = {Translate-Distill: Learning Cross-Language Dense Retrieval by Translation and Distillation},
   booktitle = {Proceedings of the 46th European Conference on Information Retrieval (ECIR)},
   year = {2024},
   url = {https://arxiv.org/abs/2401.04810}
 }
 ```
+
+Please cite the following paper if you use **Multilingual Translate-Distill** to train MLIR model. 
+```bibtex
+@inproceedings{sigir2024shirttt,
+  author = {Eugene Yang and Dawn Lawrie and James Mayfield},
+  title = {Distillation for Multilingual Information Retrieval},
+  booktitle = {Proceedings of the 47th International ACM SIGIR Conference on Research and Development in Information Retrieval (SIGIR ’24)},
+  year = {2024}
+}
+```
+
+Please cite the following paper if you use PLAID SHIRTTT. 
+```bibtex
+@inproceedings{sigir2024shirttt,
+  author = {Dawn Lawrie and Efsun Kayi and Eugene Yang and James Mayfield and Douglas W. Oard},
+  title = {PLAID SHIRTTT for Large-Scale Streaming Dense Retrieval},
+  booktitle = {Proceedings of the 47th International ACM SIGIR Conference on Research and Development in Information Retrieval (SIGIR ’24)},
+  year = {2024}
+}
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `PLAID-X-0.3.1/colbert/data/collection.py` & `plaid_x-0.3.1a0/plaidx/data/collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 # I think it could be worth doing some kind of parallel reads too, if the file exceeds 1 GiBs.
 # Just need to use a datastructure that shares things across processes without too much pickling.
 # I think multiprocessing.Manager can do that!
 
 import os
 import itertools
 
-from colbert.evaluation.loaders import load_collection
-from colbert.infra.run import Run
+from plaidx.evaluation.loaders import load_collection
+from plaidx.infra.run import Run
 
 
 class Collection:
     def __init__(self, path=None, data=None):
         self.path = path
         self.data = data or self._load_file(path)
```

### Comparing `PLAID-X-0.3.1/colbert/data/examples.py` & `plaid_x-0.3.1a0/plaidx/data/examples.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from colbert.infra.run import Run
+from plaidx.infra.run import Run
 import os
 import gzip
 import ujson
 
 from huggingface_hub import hf_hub_download
 from huggingface_hub.utils import EntryNotFoundError
 
-from colbert.utils.utils import print_message, easy_pbar
-from colbert.utils.save_metadata import get_metadata_only
+from plaidx.utils.utils import print_message, easy_pbar
+from plaidx.utils.save_metadata import get_metadata_only
 
-from colbert.infra.provenance import Provenance
+from plaidx.infra.provenance import Provenance
 
 
 class Examples:
     def __init__(self, path=None, data=None, nway=None, provenance=None):
         self.__provenance = provenance or path or Provenance()
         self.nway = nway
         self.path = path
```

### Comparing `PLAID-X-0.3.1/colbert/data/queries.py` & `plaid_x-0.3.1a0/plaidx/data/queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from colbert.infra.run import Run
+from plaidx.infra.run import Run
 import os
 import ujson
 
-from colbert.evaluation.loaders import load_queries
+from plaidx.evaluation.loaders import load_queries
 
 # TODO: Look up path in some global [per-thread or thread-safe] list.
 # TODO: path could be a list of paths...? But then how can we tell it's not a list of queries..
 
 
 class Queries:
     def __init__(self, path=None, data=None):
```

### Comparing `PLAID-X-0.3.1/colbert/data/ranking.py` & `plaid_x-0.3.1a0/plaidx/data/ranking.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import tqdm
 import ujson
-from colbert.infra.provenance import Provenance
+from plaidx.infra.provenance import Provenance
 
-from colbert.infra.run import Run
-from colbert.utils.utils import print_message, groupby_first_item
-from colbert.utils.save_metadata import get_metadata_only
+from plaidx.infra.run import Run
+from plaidx.utils.utils import print_message, groupby_first_item
+from plaidx.utils.save_metadata import get_metadata_only
 
 
 def numericize(v):
     if '.' in v:
         return float(v)
 
     return int(v)
```

### Comparing `PLAID-X-0.3.1/colbert/evaluation/load_model.py` & `plaid_x-0.3.1a0/plaidx/evaluation/load_model.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 import ujson
 import torch
 import random
 
 from collections import defaultdict, OrderedDict
 
-from colbert.parameters import DEVICE
-from colbert.modeling.colbert import ColBERT
-from colbert.utils.utils import print_message, load_checkpoint
+from plaidx.parameters import DEVICE
+from plaidx.modeling.colbert import ColBERT
+from plaidx.utils.utils import print_message, load_checkpoint
 
 
 def load_model(args, do_print=True):
     colbert = ColBERT.from_pretrained('bert-base-uncased',
                                       query_maxlen=args.query_maxlen,
                                       doc_maxlen=args.doc_maxlen,
                                       dim=args.dim,
```

### Comparing `PLAID-X-0.3.1/colbert/evaluation/loaders.py` & `plaid_x-0.3.1a0/plaidx/evaluation/loaders.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
 import ujson
 import torch
 import random
 
 from collections import defaultdict, OrderedDict
 
-from colbert.parameters import DEVICE
-from colbert.modeling.colbert import ColBERT
-from colbert.utils.utils import print_message, load_checkpoint
-from colbert.evaluation.load_model import load_model
-from colbert.utils.runs import Run
+from plaidx.parameters import DEVICE
+from plaidx.modeling.colbert import ColBERT
+from plaidx.utils.utils import print_message, load_checkpoint
+from plaidx.evaluation.load_model import load_model
+from plaidx.utils.runs import Run
 
 
 def load_queries(queries_path):
     queries = OrderedDict()
 
     print_message("#> Loading the queries from", queries_path, "...")
```

### Comparing `PLAID-X-0.3.1/colbert/evaluation/metrics.py` & `plaid_x-0.3.1a0/plaidx/evaluation/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import ujson
 
 from collections import defaultdict
-from colbert.utils.runs import Run
+from plaidx.utils.runs import Run
 
 
 class Metrics:
     def __init__(self, mrr_depths: set, recall_depths: set, success_depths: set, total_queries=None):
         self.results = {}
         self.mrr_sums = {depth: 0.0 for depth in mrr_depths}
         self.recall_sums = {depth: 0.0 for depth in recall_depths}
```

### Comparing `PLAID-X-0.3.1/colbert/index_updater.py` & `plaid_x-0.3.1a0/plaidx/index_updater.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import os
 import ujson
 import torch
 import numpy as np
 import tqdm
 
-from colbert.search.index_loader import IndexLoader
-from colbert.indexing.index_saver import IndexSaver
-from colbert.indexing.collection_encoder import CollectionEncoder
-
-from colbert.utils.utils import lengths2offsets, print_message, dotdict, flatten
-from colbert.indexing.codecs.residual import ResidualCodec
-from colbert.indexing.utils import optimize_ivf
-from colbert.search.strided_tensor import StridedTensor
-from colbert.modeling.checkpoint import Checkpoint
-from colbert.utils.utils import print_message, batch
-from colbert.data import Collection
-from colbert.indexing.codecs.residual_embeddings import ResidualEmbeddings
-from colbert.indexing.codecs.residual_embeddings_strided import (
+from plaidx.search.index_loader import IndexLoader
+from plaidx.indexing.index_saver import IndexSaver
+from plaidx.indexing.collection_encoder import CollectionEncoder
+
+from plaidx.utils.utils import lengths2offsets, print_message, dotdict, flatten
+from plaidx.indexing.codecs.residual import ResidualCodec
+from plaidx.indexing.utils import optimize_ivf
+from plaidx.search.strided_tensor import StridedTensor
+from plaidx.modeling.checkpoint import Checkpoint
+from plaidx.utils.utils import print_message, batch
+from plaidx.data import Collection
+from plaidx.indexing.codecs.residual_embeddings import ResidualEmbeddings
+from plaidx.indexing.codecs.residual_embeddings_strided import (
     ResidualEmbeddingsStrided,
 )
-from colbert.indexing.utils import optimize_ivf
+from plaidx.indexing.utils import optimize_ivf
 
 # For testing writing into new chunks, can set DEFAULT_CHUNKSIZE smaller (e.g. 1 or 2)
 DEFAULT_CHUNKSIZE = 25000
 
 
 class IndexUpdater:
```

### Comparing `PLAID-X-0.3.1/colbert/indexer.py` & `plaid_x-0.3.1a0/plaidx/indexer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
 import time
 
 import torch.multiprocessing as mp
 
-from colbert.infra.run import Run
-from colbert.infra.config import ColBERTConfig, RunConfig
-from colbert.infra.launcher import Launcher
+from plaidx.infra.run import Run
+from plaidx.infra.config import ColBERTConfig, RunConfig
+from plaidx.infra.launcher import Launcher
 
-from colbert.utils.utils import create_directory, print_message
+from plaidx.utils.utils import create_directory, print_message
 
-from colbert.indexing.collection_indexer import reuse_prepare, sample, kmeans, encode, finalize
+from plaidx.indexing.collection_indexer import reuse_prepare, sample, kmeans, encode, finalize
 
 class Indexer:
     def __init__(self, checkpoint, config=None):
         """
            Use Run().context() to choose the run's configuration. They are NOT extracted from `config`.
         """
```

### Comparing `PLAID-X-0.3.1/colbert/indexing/codecs/decompress_residuals.cpp` & `plaid_x-0.3.1a0/plaidx/indexing/codecs/decompress_residuals.cpp`

 * *Files identical despite different names*

### Comparing `PLAID-X-0.3.1/colbert/indexing/codecs/decompress_residuals.cu` & `plaid_x-0.3.1a0/plaidx/indexing/codecs/decompress_residuals.cu`

 * *Files identical despite different names*

### Comparing `PLAID-X-0.3.1/colbert/indexing/codecs/packbits.cu` & `plaid_x-0.3.1a0/plaidx/indexing/codecs/packbits.cu`

 * *Files identical despite different names*

### Comparing `PLAID-X-0.3.1/colbert/indexing/codecs/residual.py` & `plaid_x-0.3.1a0/plaidx/indexing/codecs/residual.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 """
 
 import os
 import torch
 import numpy as np
 from itertools import product
 
-from colbert.infra.config import ColBERTConfig
-from colbert.indexing.codecs.residual_embeddings import ResidualEmbeddings
-from colbert.utils.utils import print_message
+from plaidx.infra.config import ColBERTConfig
+from plaidx.indexing.codecs.residual_embeddings import ResidualEmbeddings
+from plaidx.utils.utils import print_message
 
 import pathlib
 from torch.utils.cpp_extension import load
 
 
 class ResidualCodec:
     Embeddings = ResidualEmbeddings
```

### Comparing `PLAID-X-0.3.1/colbert/indexing/codecs/residual_embeddings.py` & `plaid_x-0.3.1a0/plaidx/indexing/codecs/residual_embeddings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import torch
 import ujson
 import tqdm
 
-from colbert.indexing.codecs.residual_embeddings_strided import ResidualEmbeddingsStrided
-from colbert.utils.utils import print_message
+from plaidx.indexing.codecs.residual_embeddings_strided import ResidualEmbeddingsStrided
+from plaidx.utils.utils import print_message
 
 
 class ResidualEmbeddings:
     Strided = ResidualEmbeddingsStrided
 
     def __init__(self, codes, residuals):
         """
```

### Comparing `PLAID-X-0.3.1/colbert/indexing/codecs/residual_embeddings_strided.py` & `plaid_x-0.3.1a0/plaidx/indexing/codecs/residual_embeddings_strided.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# from colbert.indexing.codecs.residual import ResidualCodec
-import colbert.indexing.codecs.residual_embeddings as residual_embeddings
+# from plaidx.indexing.codecs.residual import ResidualCodec
+import plaidx.indexing.codecs.residual_embeddings as residual_embeddings
 
-from colbert.search.strided_tensor import StridedTensor
+from plaidx.search.strided_tensor import StridedTensor
 
 """
 import line_profiler
 import atexit
 profile = line_profiler.LineProfiler()
 atexit.register(profile.print_stats)
 """
```

### Comparing `PLAID-X-0.3.1/colbert/indexing/collection_encoder.py` & `plaid_x-0.3.1a0/plaidx/indexing/collection_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch
 
-from colbert.infra.run import Run
-from colbert.utils.utils import print_message, batch
+from plaidx.infra.run import Run
+from plaidx.utils.utils import print_message, batch
 
 
 class CollectionEncoder():
     def __init__(self, config, checkpoint):
         self.config = config
         self.checkpoint = checkpoint
         self.use_gpu = self.config.total_visible_gpus > 0
```

### Comparing `PLAID-X-0.3.1/colbert/indexing/collection_indexer.py` & `plaid_x-0.3.1a0/plaidx/indexing/collection_indexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,30 +14,30 @@
 try:
     import faiss
 except ImportError as e:
     print("WARNING: faiss must be imported for indexing")
 
 import numpy as np
 import torch.multiprocessing as mp
-from colbert.infra.config.config import ColBERTConfig
+from plaidx.infra.config.config import ColBERTConfig
 
-import colbert.utils.distributed as distributed
+import plaidx.utils.distributed as distributed
 
-from colbert.infra.run import Run
-from colbert.infra.launcher import print_memory_stats
-from colbert.modeling.checkpoint import Checkpoint
-from colbert.data.collection import Collection
-
-from colbert.indexing.collection_encoder import CollectionEncoder
-from colbert.indexing.index_saver import IndexSaver
-from colbert.indexing.loaders import load_doclens
-from colbert.indexing.utils import optimize_ivf
-from colbert.utils.utils import flatten, print_message
+from plaidx.infra.run import Run
+from plaidx.infra.launcher import print_memory_stats
+from plaidx.modeling.checkpoint import Checkpoint
+from plaidx.data.collection import Collection
+
+from plaidx.indexing.collection_encoder import CollectionEncoder
+from plaidx.indexing.index_saver import IndexSaver
+from plaidx.indexing.loaders import load_doclens
+from plaidx.indexing.utils import optimize_ivf
+from plaidx.utils.utils import flatten, print_message
 
-from colbert.indexing.codecs.residual import ResidualCodec
+from plaidx.indexing.codecs.residual import ResidualCodec
 
 # Eugene: deprecated
 # def encode(config, collection, shared_lists, shared_queues):
 #     encoder = CollectionIndexer(config=config, collection=collection)
 #     encoder.run(shared_lists)
 
 def reuse_prepare(config, collection, shared_lists, shared_queues):
```

### Comparing `PLAID-X-0.3.1/colbert/indexing/index_manager.py` & `plaid_x-0.3.1a0/plaidx/indexing/index_manager.py`

 * *Files identical despite different names*

### Comparing `PLAID-X-0.3.1/colbert/indexing/index_saver.py` & `plaid_x-0.3.1a0/plaidx/indexing/index_saver.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 import queue
 import ujson
 import threading
 
 from contextlib import contextmanager
 
-from colbert.indexing.codecs.residual import ResidualCodec
+from plaidx.indexing.codecs.residual import ResidualCodec
 
-from colbert.utils.utils import print_message
+from plaidx.utils.utils import print_message
 
 
 class IndexSaver():
     def __init__(self, config):
         self.config = config
 
     def save_codec(self, codec):
```

### Comparing `PLAID-X-0.3.1/colbert/indexing/loaders.py` & `plaid_x-0.3.1a0/plaidx/indexing/loaders.py`

 * *Files identical despite different names*

### Comparing `PLAID-X-0.3.1/colbert/indexing/utils.py` & `plaid_x-0.3.1a0/plaidx/indexing/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import torch
 import tqdm
 
-from colbert.indexing.loaders import load_doclens
-from colbert.utils.utils import print_message, flatten
+from plaidx.indexing.loaders import load_doclens
+from plaidx.utils.utils import print_message, flatten
 
 def optimize_ivf(orig_ivf, orig_ivf_lengths, index_path):
     print_message("#> Optimizing IVF to store map from centroids to list of pids..")
 
     print_message("#> Building the emb2pid mapping..")
     all_doclens = load_doclens(index_path, flatten=False)
```

### Comparing `PLAID-X-0.3.1/colbert/infra/config/base_config.py` & `plaid_x-0.3.1a0/plaidx/infra/config/base_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 from huggingface_hub import hf_hub_download
 from huggingface_hub.utils import EntryNotFoundError
 
 from typing import Any
 from collections import defaultdict
 from dataclasses import dataclass, fields
-from colbert.utils.utils import timestamp, torch_load_dnn
+from plaidx.utils.utils import timestamp, torch_load_dnn
 
-from colbert.utils.save_metadata import get_metadata_only
+from plaidx.utils.save_metadata import get_metadata_only
 from .core_config import *
 
 
 @dataclass
 class BaseConfig(CoreConfig):
     @classmethod
     def from_existing(cls, *sources):
```

### Comparing `PLAID-X-0.3.1/colbert/infra/config/core_config.py` & `plaid_x-0.3.1a0/plaidx/infra/config/core_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import torch
 import ujson
 import dataclasses
 
 from typing import Any
 from collections import defaultdict
 from dataclasses import dataclass, fields
-from colbert.utils.utils import timestamp, torch_load_dnn
+from plaidx.utils.utils import timestamp, torch_load_dnn
 
 
 @dataclass
 class DefaultVal:
     val: Any
```

### Comparing `PLAID-X-0.3.1/colbert/infra/config/settings.py` & `plaid_x-0.3.1a0/plaidx/infra/config/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import torch
 
 import __main__
 from dataclasses import dataclass
-from colbert.utils.utils import timestamp
+from plaidx.utils.utils import timestamp
 
 from .core_config import DefaultVal
 
 
 @dataclass
 class RunSettings:
     """
```

### Comparing `PLAID-X-0.3.1/colbert/infra/launcher.py` & `plaid_x-0.3.1a0/plaidx/infra/launcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 import numpy as np
 
 try:
     mp.set_start_method('spawn', force=True)
 except RuntimeError:
     pass
 
-import colbert.utils.distributed as distributed
+import plaidx.utils.distributed as distributed
 
-from colbert.infra.run import Run
-from colbert.infra.config import BaseConfig, RunConfig, RunSettings
+from plaidx.infra.run import Run
+from plaidx.infra.config import BaseConfig, RunConfig, RunSettings
 
-from colbert.utils.utils import print_message
+from plaidx.utils.utils import print_message
 
 
 class Launcher:
     def __init__(self, callee, run_config=None, return_all=False):
         self.callee = callee
         self.return_all = return_all
```

### Comparing `PLAID-X-0.3.1/colbert/infra/provenance.py` & `plaid_x-0.3.1a0/plaidx/infra/provenance.py`

 * *Files identical despite different names*

### Comparing `PLAID-X-0.3.1/colbert/infra/run.py` & `plaid_x-0.3.1a0/plaidx/infra/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import atexit
 
-from colbert.utils.utils import create_directory, print_message, timestamp
+from plaidx.utils.utils import create_directory, print_message, timestamp
 from contextlib import contextmanager
 
-from colbert.infra.config import RunConfig
+from plaidx.infra.config import RunConfig
 
 
 class Run(object):
     _instance = None
 
     os.environ["TOKENIZERS_PARALLELISM"] = "true"  # NOTE: If a deadlock arises, switch to false!!
```

### Comparing `PLAID-X-0.3.1/colbert/modeling/base_colbert.py` & `plaid_x-0.3.1a0/plaidx/modeling/base_colbert.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 import torch
 import sys
 
-from colbert.utils.utils import torch_load_dnn
+from plaidx.utils.utils import torch_load_dnn
 
 from transformers import AutoTokenizer
-from colbert.modeling.hf_colbert import class_factory
-from colbert.infra.config import ColBERTConfig
-from colbert.infra.run import Run
+from plaidx.modeling.hf_colbert import class_factory
+from plaidx.infra.config import ColBERTConfig
+from plaidx.infra.run import Run
 
 
 class BaseColBERT(torch.nn.Module):
     """
     Shallow module that wraps the ColBERT parameters, custom configuration, and underlying tokenizer.
     This class provides direct instantiation and saving of the model/colbert_config/tokenizer package.
 
@@ -58,16 +58,16 @@
         self.colbert_config.save_for_checkpoint(path)
 
 
 if __name__ == '__main__':
     import random
     import numpy as np
 
-    from colbert.infra.run import Run
-    from colbert.infra.config import RunConfig
+    from plaidx.infra.run import Run
+    from plaidx.infra.config import RunConfig
 
     random.seed(12345)
     np.random.seed(12345)
     torch.manual_seed(12345)
 
     with Run().context(RunConfig(gpus=2)):
         m = BaseColBERT('bert-base-uncased', colbert_config=ColBERTConfig(Run().config, doc_maxlen=300, similarity='l2'))
```

### Comparing `PLAID-X-0.3.1/colbert/modeling/checkpoint.py` & `plaid_x-0.3.1a0/plaidx/modeling/checkpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import torch
 
 from tqdm import tqdm
 
-from colbert.modeling.tokenization import QueryTokenizer, DocTokenizer
-from colbert.utils.amp import MixedPrecisionManager
+from plaidx.modeling.tokenization import QueryTokenizer, DocTokenizer
+from plaidx.utils.amp import MixedPrecisionManager
 
-from colbert.modeling.colbert import ColBERT
+from plaidx.modeling.colbert import ColBERT
 
 
 class Checkpoint(ColBERT):
     """
         Easy inference with ColBERT.
 
         TODO: Add .cast() accepting [also] an object instance-of(Checkpoint) as first argument.
```

### Comparing `PLAID-X-0.3.1/colbert/modeling/colbert.py` & `plaid_x-0.3.1a0/plaidx/modeling/colbert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from colbert.infra.config.config import ColBERTConfig
-from colbert.search.strided_tensor import StridedTensor
-from colbert.utils.utils import print_message, flatten
-from colbert.modeling.base_colbert import BaseColBERT
+from plaidx.infra.config.config import ColBERTConfig
+from plaidx.search.strided_tensor import StridedTensor
+from plaidx.utils.utils import print_message, flatten
+from plaidx.modeling.base_colbert import BaseColBERT
 
 import torch
 import string
 
 import os
 import pathlib
 from torch.utils.cpp_extension import load
```

### Comparing `PLAID-X-0.3.1/colbert/modeling/hf_colbert.py` & `plaid_x-0.3.1a0/plaidx/modeling/hf_colbert.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import torch.nn as nn
 import transformers
 from transformers import BertPreTrainedModel, BertModel, AutoTokenizer, AutoModel, AutoConfig
 from transformers import RobertaModel, RobertaPreTrainedModel
 from transformers import XLMRobertaModel, XLMRobertaConfig
 from transformers import ElectraModel, ElectraPreTrainedModel
 from transformers import DebertaV2Model, DebertaV2PreTrainedModel
-from colbert.utils.utils import torch_load_dnn, print_message
-from colbert.infra import ColBERTConfig
+from plaidx.utils.utils import torch_load_dnn, print_message
+from plaidx.infra import ColBERTConfig
 
 class XLMRobertaPreTrainedModel(RobertaPreTrainedModel):
     """
     This class overrides [`RobertaModel`]. Please check the superclass for the appropriate documentation alongside
     usage examples.
     """
```

### Comparing `PLAID-X-0.3.1/colbert/modeling/reranker/electra.py` & `plaid_x-0.3.1a0/plaidx/modeling/reranker/electra.py`

 * *Files identical despite different names*

### Comparing `PLAID-X-0.3.1/colbert/modeling/reranker/tokenizer.py` & `plaid_x-0.3.1a0/plaidx/modeling/reranker/tokenizer.py`

 * *Files identical despite different names*

### Comparing `PLAID-X-0.3.1/colbert/modeling/segmented_maxsim.cpp` & `plaid_x-0.3.1a0/plaidx/modeling/segmented_maxsim.cpp`

 * *Files identical despite different names*

### Comparing `PLAID-X-0.3.1/colbert/modeling/tokenization/doc_tokenization.py` & `plaid_x-0.3.1a0/plaidx/modeling/tokenization/doc_tokenization.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import torch
 
 # from transformers import BertTokenizerFast
 
-from colbert.modeling.hf_colbert import class_factory
-from colbert.infra import ColBERTConfig
-from colbert.modeling.tokenization.utils import _split_into_batches, _sort_by_length
+from plaidx.modeling.hf_colbert import class_factory
+from plaidx.infra import ColBERTConfig
+from plaidx.modeling.tokenization.utils import _split_into_batches, _sort_by_length
 
 
 class DocTokenizer():
     def __init__(self, config: ColBERTConfig):
         HF_ColBERT = class_factory(config.model_name)
         self.tok = HF_ColBERT.raw_tokenizer_from_pretrained(config.checkpoint, colbert_config=config)
```

### Comparing `PLAID-X-0.3.1/colbert/modeling/tokenization/query_tokenization.py` & `plaid_x-0.3.1a0/plaidx/modeling/tokenization/query_tokenization.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch
 
-from colbert.modeling.hf_colbert import class_factory
-from colbert.infra import ColBERTConfig
-from colbert.modeling.tokenization.utils import _split_into_batches
-from colbert.utils.utils import batch
+from plaidx.modeling.hf_colbert import class_factory
+from plaidx.infra import ColBERTConfig
+from plaidx.modeling.tokenization.utils import _split_into_batches
+from plaidx.utils.utils import batch
 
 
 class QueryTokenizer():
     def __init__(self, config: ColBERTConfig):
         HF_ColBERT = class_factory(config.model_name)
         self.tok = HF_ColBERT.raw_tokenizer_from_pretrained(config.checkpoint, colbert_config=config)
```

### Comparing `PLAID-X-0.3.1/colbert/modeling/tokenization/utils.py` & `plaid_x-0.3.1a0/plaidx/modeling/tokenization/utils.py`

 * *Files identical despite different names*

### Comparing `PLAID-X-0.3.1/colbert/parameters.py` & `plaid_x-0.3.1a0/plaidx/parameters.py`

 * *Files identical despite different names*

### Comparing `PLAID-X-0.3.1/colbert/scripts/collection_utils.py` & `plaid_x-0.3.1a0/plaidx/scripts/collection_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from pathlib import Path
 from typing import Dict, List, Union
 
 import gzip
 import pickle
 import json
 from time import time
+import random
 import re
 from tqdm import tqdm
 
-from colbert.infra import Run, ColBERTConfig
-from colbert.utils.utils import print_message, easy_pbar
-from colbert.data import Queries, Collection, Examples
+from plaidx.infra import Run, ColBERTConfig
+from plaidx.utils.utils import print_message, easy_pbar
+from plaidx.data import Queries, Collection, Examples
 
 from huggingface_hub import hf_hub_download
 from huggingface_hub.utils import EntryNotFoundError
+
 import ir_datasets as irds
+import ir_measures as irms
 
 import logging
 
 _component_cls_map: Dict[str, Union[Examples, Queries, Collection]] = { 
     'docpairs': Examples, 'queries': Queries, 'docs': Collection 
 }
 
@@ -169,24 +172,103 @@
                 collection_path=c, 
                 offsetmap_path=str(p.parent / f"{p.name}.offsetmap"),
                 config=None
             )
     return Collection.cast(c)
 
 
-def load_irds_or_local(ds: str, component: str, mixing='elements', use_offsetmap=False) -> Union[Examples, Collection, Examples, str]:
+class MutliCollections(Collection):
+    def __init__(self, children, mixing='elements', load_now=False, use_offsetmap=False):
+        self.children = children
+        self.loaded = False
+        if load_now:
+            self.load_all_collections()
+
+        assert mixing in ['entries', 'elements', 'all']
+        self.strategy = mixing
+        print_message(f"Using {len(self.children)} collections with {self.strategy} mixing strategy.")
+
+        self.use_offsetmap = use_offsetmap
+    
+
+    def load_all_collections(self):
+        self.children = [ _load_single_collection(c, self.use_offsetmap) for c in self.children ]
+        assert all([ len(self.children[0]) == len(c) for c in self.children ])
+        self.loaded = True
+
+    def _choice(self, options):
+        # TODO: could be fancier
+        return random.choice(options)
+
+    def __getitem__(self, item):
+        assert self.loaded
+
+        # TODO: might need some checking
+        if self.strategy == 'entries':
+            assert isinstance(item, list)
+            return self._choice(self.children)[item]
+
+        elif self.strategy == 'elements':
+            if not isinstance(item, list):
+                return self._choice(self.children)[item]
+            return [ self._choice(self.children)[i] for i in item ]
+        
+        elif self.strategy == 'all':
+            selected = [ c[item] for c in self.children ]
+            if not isinstance(item, list):
+                return selected
+            # change to [ [i1l1, i1l2, ...], [i2l1, i2l2, ...] ]
+            return list(map(list, zip(*selected))) # transpose
+
+        raise ValueError(f"strategy {self.strategy} not supported.")
+        # return self._choice([ c[item] for c in self.children ])
+
+    def __iter__(self):
+        if self.strategy == 'elements':
+            yield from map(self._choice, zip(*self.children))
+        elif self.strategy == 'all':
+            yield from map(list, zip(*self.children))
+
+        raise ValueError(f"strategy {self.strategy} not supported.")
+
+    def __len__(self):
+        return len(self.children[0])
+
+    def provenance(self):
+        return f"Combination({self.strategy})[{'+'.join([ c.provenance() if isinstance(c, Collection) else str(c) for c in self.children ])}]"
+
+
+def load_irds_or_local(ds: Union[List[str],str], component: str, mixing='elements', use_offsetmap=False) -> Union[Examples, Collection, Examples, str]:
+    if isinstance(ds, list):
+        if len(ds) > 1:
+            # TODO: support queries or even examples
+            return MutliCollections([load_irds_or_local(d, component) for d in ds], mixing, use_offsetmap=use_offsetmap)
+        ds = ds[0]
+
     if ds in irds.registry:
         print_message(f"Use IRDS:{ds} for {component}")
+        if component == 'qrels':
+            return list(irds.load(ds).qrels_iter())
         return _component_cls_map[component](data=_irds_wrapper(ds, component), path=f"irds:{ds}:{component}")
     else:
-        print_message(f"Use local file (or hfhub if applicable):{ds} for {component}")
-        # assert Path(ds).exists(), f"File {ds} does not exists."
+        print_message(f"Use local file:{ds} for {component}")
+        assert Path(ds).exists(), f"File {ds} does not exists."
+
+        if component == 'qrels':
+            return list(irms.read_trec_qrels())
 
         # avoid materialize it in the main process if using raw file
-        return _load_single_collection(ds, use_offsetmap=True) if use_offsetmap else ds
+        if component == "docs":
+            return _load_single_collection(ds, use_offsetmap=True) if use_offsetmap else ds
+        return _component_cls_map[component](path=ds)
+
+def irds_contains(ds: Union[List[str], str], component: str):
+    if isinstance(ds, list):
+        return [ irds_contains(d, component) for d in ds ]
+    return ds in irds.registry and irds.load(ds).has(component)
 
 
 def _offsetmap_cache_cli(args):
     collection_path: Path = args.collection_path
     offsetmap_path = collection_path.parent / f"{collection_path.name}.offsetmap"
     print_message(collection_path)
     OffsetMapCollection(None, str(collection_path), offsetmap_path, build_offset=True)
```

### Comparing `PLAID-X-0.3.1/colbert/scripts/index.py` & `plaid_x-0.3.1a0/plaidx/scripts/index.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import argparse
 
-from colbert.infra import Run, RunConfig, ColBERTConfig
-from colbert import Indexer
+from plaidx.infra import Run, RunConfig, ColBERTConfig
+from plaidx import Indexer
 
-from colbert.scripts.collection_utils import load_irds_or_local
+from plaidx.scripts.collection_utils import load_irds_or_local
 
 def create_plaid_index(args):
 
     if args.n_gpus is None:
         import torch
         n_gpus = torch.cuda.device_count()
     else:
@@ -16,16 +16,17 @@
 
     # Provide v1 checkpoint configurations
     config = ColBERTConfig(
         doc_maxlen=args.doc_maxlen, nbits=args.nbits,
         max_sampled_pid=args.max_sampled_pid, max_num_partitions=args.max_num_partitions
     )
 
+    coll_file = str(os.path.join(args.coll_dir, 'collection_passages.tsv')) if os.path.isdir(args.coll_dir) else args.coll_dir
     collection = load_irds_or_local(
-        args.dataset_name if args.coll_dir is None else str(os.path.join(args.coll_dir, 'collection_passages.tsv')),
+        args.dataset_name if args.coll_dir is None else coll_file,
         component='docs', use_offsetmap=args.lazy_collection_loader
     )
     dataset_name = args.dataset_name.replace('/', '.')
 
     if args.base_model is not None:
         config.configure(model_name=args.base_model)
     if args.checkpoint.endswith('.dnn'):
```

### Comparing `PLAID-X-0.3.1/colbert/scripts/search.py` & `plaid_x-0.3.1a0/plaidx/scripts/search.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import argparse
 from pathlib import Path
 from typing import Dict, List, Tuple
-from colbert.infra import Run, RunConfig, ColBERTConfig
-from colbert.data.queries import Queries
-from colbert import Searcher
+from plaidx.infra import Run, RunConfig, ColBERTConfig
+from plaidx import Searcher
 
 from tqdm.auto import tqdm
 
 import ir_measures as irms
-from colbert.scripts.collection_utils import load_mapping
+from plaidx.scripts.collection_utils import load_mapping, load_irds_or_local, irds_contains
 
 def maxp(passage_triples: List[Tuple[str, int, float]], mapping: Dict[str, str]) -> Dict[str, float]:
     doc_score = {}
     for pid, _, score in passage_triples:
         doc_id = mapping[pid]
         if doc_id not in doc_score or doc_score[doc_id] < score:
             doc_score[doc_id] = score
@@ -26,20 +25,20 @@
 
 def main(args):
     output_fn = args.output or f"./{args.run_id}.{args.search_depth}.trec"
     if args.check_exists and Path(output_fn).exists():
         print(f"Found {output_fn} -- skip")
         return
 
-    queries = Queries(path=args.query_file)
+    queries = load_irds_or_local(args.queries, component='queries', use_offsetmap=False)
     mapping = load_mapping(args.passage_mapping, is_dummy=not args.maxp)
 
     if args.run_evel:
         metrics = [ irms.parse_measure(m) for m in args.metrics ]
-        qrels = list(irms.read_trec_qrels(args.qrel))
+        qrels = load_irds_or_local(args.qrels, component='qrels')
 
     with Run().context(RunConfig(nranks=args.n_gpus, root=args.root, experiment=args.experiment, index_root=args.index_root)):
         checkpoint = None
         if args.checkpoint_root is not None:
             checkpoint = args.checkpoint_root + "/" + ColBERTConfig.load_from_index( args.index_root + "/" + args.index_name ).checkpoint
         searcher = Searcher(index=args.index_name, checkpoint=checkpoint)
         searcher.config.configure(only_approx=args.only_approx, ignore_unrecognized=False)
@@ -58,24 +57,24 @@
         print( irms.calc_aggregate(metrics, qrels, doc_ranking) )
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
     parser.add_argument('--index_name', help="name of the index", type=str)
     parser.add_argument('--passage_mapping', help="mapping tsv file from passage to documents", type=str)
-    parser.add_argument('--query_file', help="query tsv file", type=str)
+    parser.add_argument('--query_file', '--query', '--queries', dest='queries', help="query tsv file or irds", type=str, required=True)
     parser.add_argument('--search_depth', help="k; depth of PLAID search", type=int, default=2500)
     parser.add_argument('--centroid_score_threshold', help="threshold for centroid cell filter", type=float, default=0.4)
 
     parser.add_argument('--maxp', action='store_true', default=False)
     parser.add_argument('--checkpoint_root', type=str, default=None)
 
     parser.add_argument('--metrics', help="evalutation metrics used after search, should be parsable by ir_measures", 
                         type=str, nargs='*', default=[])
-    parser.add_argument('--qrel', help="path to qrels file", type=str, default=None)
+    parser.add_argument('--qrel', '--qrels', dest='qrels', help="path to qrels file", type=str, default=None)
 
     parser.add_argument('--run_id', help="name of this run, will be used for the filename of the trec file", type=str, default=None)
     parser.add_argument('--output', help="output directory of the trec file", type=str, default=None)
 
     parser.add_argument('--index_root', help="root directory of the indexes", type=str, default=None)
     parser.add_argument('--experiment', help="name of the experiment for locating the index", type=str, default="default")
     parser.add_argument('--root', type=str, default=None)
@@ -91,17 +90,20 @@
     args = parser.parse_args()
 
     if args.n_gpus is None:
         import torch
         args.n_gpus = torch.cuda.device_count()
     
     if len(args.metrics) > 0:
-        assert args.qrel and Path(args.qrel).exists(), args.qrel
+        if args.qrels is None and irds_contains(args.queries, 'qrels'):
+            args.qrels = args.queries
+
+        assert args.qrels and (Path(args.qrels).exists() or irds_contains(args.qrels, 'qrels')), args.qrels
         args.run_evel = True
 
-    assert Path(args.query_file).exists(), args.query_file
+    assert Path(args.queries).exists() or irds_contains(args.queries, 'queries'), args.queries
 
     if args.run_id is None:
-        args.run_id = f"{args.experiment}.{args.index_name}.{Path(args.query_file).name}"
+        args.run_id = f"{args.experiment}.{args.index_name}.{Path(args.queries).name}"
         args.run_id = args.run_id.replace('/', '.')
 
     main(args)
```

### Comparing `PLAID-X-0.3.1/colbert/scripts/train.py` & `plaid_x-0.3.1a0/plaidx/scripts/train.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import argparse
+from plaidx.infra import Run, RunConfig, ColBERTConfig
+from plaidx import Trainer
+from plaidx.utils.utils import print_message
 
-from colbert.infra import Run, RunConfig, ColBERTConfig
-from colbert import Trainer
-from colbert.utils.utils import print_message
-
-from colbert.scripts.collection_utils import load_irds_or_local
+from plaidx.scripts.collection_utils import load_irds_or_local
 
 def main(args):
     bsize = args.per_device_batch_size*args.n_gpus
     exp_name = f"{args.run_tag}/{bsize}bat.{args.nway}way{'-ib' if args.ib_negatives else ''}"
 
     if args.use_local_full_triples:
         queries = None
@@ -18,33 +17,45 @@
         collection = load_irds_or_local(args.training_collection, 'docs', mixing=args.training_collection_mixing, use_offsetmap=args.use_offsetmap)
     else:
         queries = load_irds_or_local(args.training_irds_id, 'queries')
         collection = load_irds_or_local(args.training_irds_id, 'docs', use_offsetmap=args.use_offsetmap)
 
     triples = load_irds_or_local(args.training_triples, 'docpairs')
 
+    # parse other_args
+    other_args = {}
+    for k,v in map(lambda x: x.split('='), args.other_args):
+        try: 
+            other_args[k] = eval(v)
+        except:
+            other_args[k] = v
+        
     with Run().context(RunConfig(nranks=args.n_gpus, root=args.root, experiment=args.experiment, name=exp_name)):
         trainer = Trainer(
             triples=triples, queries=queries, collection=collection,
             config=ColBERTConfig(
                 bsize=bsize, 
                 checkpoint=args.checkpoint,
                 maxsteps=args.maxsteps, lr=args.learning_rate, nway=args.nway, 
+                accumsteps=args.accumsteps, 
                 model_name=args.model_name, 
                 similarity=args.similarity,
                 force_resize_embeddings=True,
+                doc_maxlen=args.doc_maxlen, 
                 use_ib_negatives=args.ib_negatives,
                 ignore_scores=(args.kd_loss == 'None'),
                 kd_loss=args.kd_loss, 
                 shuffle_passages=not args.only_top, 
                 sampling_max_beta=args.sampling_max_beta,
                 over_one_epoch=True,
                 resume=args.resume,
                 resume_optimizer=args.resume_optimizer,
-                fix_broken_optimizer_state=args.fix_broken_optimizer_state
+                fix_broken_optimizer_state=args.fix_broken_optimizer_state,
+                multilang=(args.training_collection_mixing == 'all'),
+                **other_args
             )
         )
 
         trainer.train()
 
         print_message(f"Best model: {trainer.best_checkpoint_path()}")
         
@@ -56,50 +67,59 @@
     
     parser.add_argument('--use_local_full_triples', action='store_true', default=False)
     parser.add_argument('--training_triples', type=str, required=True) # can be a irds id or path
     parser.add_argument('--training_irds_id', type=str, default='beir/msmarco/train')
     parser.add_argument('--training_queries', type=str, default=None)
     parser.add_argument('--training_collection', type=str, nargs='+', default=None)
 
+    parser.add_argument('--doc_maxlen', type=int, default=220)
     parser.add_argument('--use_offsetmap', action='store_true', default=False)
 
+    parser.add_argument('--training_collection_mixing', choices=['entries', 'passages', 'elements', 'all', 'round-robin'], default='elements')
     parser.add_argument('--similarity', choices=['l2', 'cosine'], default='cosine')
 
     parser.add_argument('--learning_rate', type=float, default=5e-6)
     parser.add_argument('--nway', type=int, default=8)
     parser.add_argument('--per_device_batch_size', type=int, default=8)
     parser.add_argument('--maxsteps', type=int, default=200_000)
     parser.add_argument('--ib_negatives', action='store_true', default=False)
+    parser.add_argument('--accumsteps', type=int, default=1)
 
     parser.add_argument('--kd_loss', choices=['KLD', 'MSE', 'None'], default='KLD')
 
     parser.add_argument('--only_top', action='store_true', default=False)
     parser.add_argument('--sampling_max_beta', type=float, default=1.0)
 
     parser.add_argument('--experiment', help="name of the experiment for locating the index", type=str, default=None)
     parser.add_argument('--root', type=str, default=None)
     parser.add_argument('--run_tag', type=str, default=None)
     parser.add_argument('--n_gpus', help="number of gpus to use, default all visible ones in CUDA_VISIBLE_DEVICES", type=int, default=None)
 
     parser.add_argument('--resume', action='store_true', default=False)
     parser.add_argument('--resume_optimizer', action='store_true', default=False)
     parser.add_argument('--fix_broken_optimizer_state', action='store_true', default=False)
+    parser.add_argument('--other_args', type=str, nargs='+', default=[])
 
     args = parser.parse_args()
 
     if args.n_gpus is None:
         import torch
         args.n_gpus = torch.cuda.device_count()
 
     # make sure when running distillation, the triple file is a jsonl file
-    # if args.kd_loss != 'None':
-    #     assert args.training_triples.endswith('.jsonl')
+    if args.kd_loss != 'None':
+        assert args.training_triples.endswith('.jsonl')
 
     if args.training_queries is not None or args.training_collection is not None:
         assert args.training_queries is not None
         assert args.training_collection is not None
         print_message(f"Use separate irds for training queries and documents.")
 
+    if args.training_collection_mixing == 'passages':
+        args.training_collection_mixing = 'elements'
+    elif args.training_collection_mixing == 'round-robin':
+        args.training_collection_mixing = 'all'
+
     args.run_tag = args.run_tag or f"{args.learning_rate}"
     args.experiment = args.experiment or f"plaid_{args.model_name.split('/')[-1]}"
 
     main(args)
```

### Comparing `PLAID-X-0.3.1/colbert/search/candidate_generation.py` & `plaid_x-0.3.1a0/plaidx/search/candidate_generation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import torch
 
-from colbert.search.strided_tensor import StridedTensor
+from plaidx.search.strided_tensor import StridedTensor
 from .strided_tensor_core import _create_mask, _create_view
 
 
 class CandidateGeneration:
 
     def __init__(self, use_gpu=True):
         self.use_gpu = use_gpu
```

### Comparing `PLAID-X-0.3.1/colbert/search/decompress_residuals.cpp` & `plaid_x-0.3.1a0/plaidx/search/decompress_residuals.cpp`

 * *Files identical despite different names*

### Comparing `PLAID-X-0.3.1/colbert/search/filter_pids.cpp` & `plaid_x-0.3.1a0/plaidx/search/filter_pids.cpp`

 * *Files identical despite different names*

### Comparing `PLAID-X-0.3.1/colbert/search/index_loader.py` & `plaid_x-0.3.1a0/plaidx/search/index_loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 import ujson
 import torch
 import numpy as np
 import tqdm
 
-from colbert.utils.utils import lengths2offsets, print_message, dotdict, flatten
-from colbert.indexing.codecs.residual import ResidualCodec
-from colbert.indexing.utils import optimize_ivf
-from colbert.search.strided_tensor import StridedTensor
+from plaidx.utils.utils import lengths2offsets, print_message, dotdict, flatten
+from plaidx.indexing.codecs.residual import ResidualCodec
+from plaidx.indexing.utils import optimize_ivf
+from plaidx.search.strided_tensor import StridedTensor
 
 
 class IndexLoader:
     def __init__(self, index_path, use_gpu=True):
         self.index_path = index_path
         self.use_gpu = use_gpu
```

### Comparing `PLAID-X-0.3.1/colbert/search/index_storage.py` & `plaid_x-0.3.1a0/plaidx/search/index_storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import torch
 
-from colbert.utils.utils import flatten, print_message
+from plaidx.utils.utils import flatten, print_message
 
-from colbert.indexing.loaders import load_doclens
-from colbert.indexing.codecs.residual_embeddings_strided import ResidualEmbeddingsStrided
+from plaidx.indexing.loaders import load_doclens
+from plaidx.indexing.codecs.residual_embeddings_strided import ResidualEmbeddingsStrided
 
-from colbert.search.strided_tensor import StridedTensor
-from colbert.search.candidate_generation import CandidateGeneration
+from plaidx.search.strided_tensor import StridedTensor
+from plaidx.search.candidate_generation import CandidateGeneration
 
 from .index_loader import IndexLoader
-from colbert.modeling.colbert import colbert_score, colbert_score_packed, colbert_score_reduce
+from plaidx.modeling.colbert import colbert_score, colbert_score_packed, colbert_score_reduce
 
 from math import ceil
 
 import os
 import pathlib
 from torch.utils.cpp_extension import load
```

### Comparing `PLAID-X-0.3.1/colbert/search/segmented_lookup.cpp` & `plaid_x-0.3.1a0/plaidx/search/segmented_lookup.cpp`

 * *Files identical despite different names*

### Comparing `PLAID-X-0.3.1/colbert/search/strided_tensor.py` & `plaid_x-0.3.1a0/plaidx/search/strided_tensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from struct import pack
 import torch
 from torch._C import device
 
-from colbert.utils.utils import flatten, print_message
+from plaidx.utils.utils import flatten, print_message
 
 from .strided_tensor_core import StridedTensorCore, _create_mask, _create_view
 
 import os
 import pathlib
 from torch.utils.cpp_extension import load
```

### Comparing `PLAID-X-0.3.1/colbert/search/strided_tensor_core.py` & `plaid_x-0.3.1a0/plaidx/search/strided_tensor_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch
 import random
 
 import numpy as np
 
-from colbert.utils.utils import flatten
+from plaidx.utils.utils import flatten
 
 
 """
 import line_profiler
 import atexit
 profile = line_profiler.LineProfiler()
 atexit.register(profile.print_stats)
```

### Comparing `PLAID-X-0.3.1/colbert/searcher.py` & `plaid_x-0.3.1a0/plaidx/searcher.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import os
 import torch
 
 from tqdm import tqdm
 from typing import Union
 
-from colbert.data import Collection, Queries, Ranking
+from plaidx.data import Collection, Queries, Ranking
 
-from colbert.modeling.checkpoint import Checkpoint
-from colbert.search.index_storage import IndexScorer
+from plaidx.modeling.checkpoint import Checkpoint
+from plaidx.search.index_storage import IndexScorer
 
-from colbert.infra.provenance import Provenance
-from colbert.infra.run import Run
-from colbert.infra.config import ColBERTConfig, RunConfig
-from colbert.infra.launcher import print_memory_stats
+from plaidx.infra.provenance import Provenance
+from plaidx.infra.run import Run
+from plaidx.infra.config import ColBERTConfig, RunConfig
+from plaidx.infra.launcher import print_memory_stats
 
 import time
 
 TextQueries = Union[str, 'list[str]', 'dict[int, str]', Queries]
 
 
 class Searcher:
```

### Comparing `PLAID-X-0.3.1/colbert/trainer.py` & `plaid_x-0.3.1a0/plaidx/trainer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from colbert.infra.run import Run
-from colbert.infra.launcher import Launcher
-from colbert.infra.config import ColBERTConfig, RunConfig
+from plaidx.infra.run import Run
+from plaidx.infra.launcher import Launcher
+from plaidx.infra.config import ColBERTConfig, RunConfig
 
-from colbert.training.training import train
-from colbert.training.legacy_training import train as v1_train
+from plaidx.training.training import train
+from plaidx.training.legacy_training import train as v1_train
 
 
 class Trainer:
     def __init__(self, triples, queries=None, collection=None, config=None):
         self.config = ColBERTConfig.from_existing(config, Run().config)
 
         self.triples = triples
```

### Comparing `PLAID-X-0.3.1/colbert/training/eager_batcher.py` & `plaid_x-0.3.1a0/plaidx/training/eager_batcher.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import ujson
 
 from functools import partial
-from colbert.utils.utils import print_message
-from colbert.modeling.tokenization import QueryTokenizer, DocTokenizer, tensorize_triples
+from plaidx.utils.utils import print_message
+from plaidx.modeling.tokenization import QueryTokenizer, DocTokenizer, tensorize_triples
 
-from colbert.utils.runs import Run
+from plaidx.utils.runs import Run
 
 
 class EagerBatcher():
     def __init__(self, args, rank=0, nranks=1):
         self.rank, self.nranks = rank, nranks
         self.bsize, self.accumsteps = args.bsize, args.accumsteps
```

### Comparing `PLAID-X-0.3.1/colbert/training/lazy_batcher.py` & `plaid_x-0.3.1a0/plaidx/training/lazy_batcher.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import os
 import ujson
 from random import shuffle
 from tqdm.auto import tqdm
 
 from functools import partial
-from colbert.infra.config.config import ColBERTConfig
-from colbert.utils.utils import print_message, zipstar
-from colbert.modeling.tokenization import QueryTokenizer, DocTokenizer, tensorize_triples
-from colbert.evaluation.loaders import load_collection
+from plaidx.infra.config.config import ColBERTConfig
+from plaidx.utils.utils import print_message, zipstar
+from plaidx.modeling.tokenization import QueryTokenizer, DocTokenizer, tensorize_triples
+from plaidx.evaluation.loaders import load_collection
 
-from colbert.data.collection import Collection
-from colbert.data.queries import Queries
-from colbert.data.examples import Examples
+from plaidx.data.collection import Collection
+from plaidx.data.queries import Queries
+from plaidx.data.examples import Examples
 
-from colbert.utils.runs import Run
+from plaidx.utils.runs import Run
 
 from scipy.stats import beta
 import numpy as np
 def sampling_on_beta(items, nway: int, step: int, max_step: int, max_beta: float):
     samp_dist: np.ndarray = beta(1.0, 1.+step/max_step*(max_beta-1.)).pdf(np.arange(len(items))/len(items))
     samp_dist = samp_dist / samp_dist.sum()
     idx = np.random.choice(len(items), size=nway, replace=False, p=samp_dist)
```

### Comparing `PLAID-X-0.3.1/colbert/training/legacy_training.py` & `plaid_x-0.3.1a0/plaidx/training/legacy_training.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 import random
 import time
 import torch
 import torch.nn as nn
 import numpy as np
 
 from transformers import AdamW
-from colbert.infra import ColBERTConfig, Run
-from colbert.utils.amp import MixedPrecisionManager
+from plaidx.infra import ColBERTConfig, Run
+from plaidx.utils.amp import MixedPrecisionManager
 
-from colbert.training.lazy_batcher import LazyBatcher
-from colbert.parameters import DEVICE
+from plaidx.training.lazy_batcher import LazyBatcher
+from plaidx.parameters import DEVICE
 
-from colbert.modeling.colbert import ColBERT
-from colbert.utils.utils import print_message
-from colbert.training.utils import print_progress, manage_checkpoints, find_last_checkpoint, load_checkpoint_misc
+from plaidx.modeling.colbert import ColBERT
+from plaidx.utils.utils import print_message
+from plaidx.training.utils import print_progress, manage_checkpoints, find_last_checkpoint, load_checkpoint_misc
 
 from functools import partial
-from colbert.modeling.tokenization.utils import legacy_tensorize_triples
+from plaidx.modeling.tokenization.utils import legacy_tensorize_triples
 
 def train(config: ColBERTConfig, triples, queries=None, collection=None):
     # lagacy training code is only compatible with
     assert config.nway == 2
 
     if config.resume:
         config.checkpoint = config.checkpoint or find_last_checkpoint(config.checkpoint_path_)
```

### Comparing `PLAID-X-0.3.1/colbert/training/rerank_batcher.py` & `plaid_x-0.3.1a0/plaidx/training/rerank_batcher.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import os
 import ujson
 
 from functools import partial
-from colbert.infra.config.config import ColBERTConfig
-from colbert.utils.utils import flatten, print_message, zipstar
-from colbert.modeling.reranker.tokenizer import RerankerTokenizer
+from plaidx.infra.config.config import ColBERTConfig
+from plaidx.utils.utils import flatten, print_message, zipstar
+from plaidx.modeling.reranker.tokenizer import RerankerTokenizer
 
-from colbert.data.collection import Collection
-from colbert.data.queries import Queries
-from colbert.data.examples import Examples
+from plaidx.data.collection import Collection
+from plaidx.data.queries import Queries
+from plaidx.data.examples import Examples
 
-# from colbert.utils.runs import Run
+# from plaidx.utils.runs import Run
 
 
 class RerankBatcher():
     def __init__(self, config: ColBERTConfig, triples, queries, collection, rank=0, nranks=1):
         self.bsize, self.accumsteps = config.bsize, config.accumsteps
         self.nway = config.nway
```

### Comparing `PLAID-X-0.3.1/colbert/training/training.py` & `plaid_x-0.3.1a0/plaidx/training/training.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 import torch
 import random
 import torch.nn as nn
 import torch.nn.functional as F
 import numpy as np
 
 from transformers import AdamW, get_linear_schedule_with_warmup
-from colbert.infra import ColBERTConfig
-from colbert.training.rerank_batcher import RerankBatcher
+from plaidx.infra import ColBERTConfig
+from plaidx.training.rerank_batcher import RerankBatcher
 
-from colbert.utils.amp import MixedPrecisionManager
-from colbert.training.lazy_batcher import LazyBatcher, MultiLangBatcher
-from colbert.parameters import DEVICE
+from plaidx.utils.amp import MixedPrecisionManager
+from plaidx.training.lazy_batcher import LazyBatcher, MultiLangBatcher
+from plaidx.parameters import DEVICE
 
-from colbert.modeling.colbert import ColBERT
-from colbert.modeling.reranker.electra import ElectraReranker
+from plaidx.modeling.colbert import ColBERT
+from plaidx.modeling.reranker.electra import ElectraReranker
 
-from colbert.utils.utils import print_message
-from colbert.training.utils import print_progress, manage_checkpoints, find_last_checkpoint, load_checkpoint_misc
+from plaidx.utils.utils import print_message
+from plaidx.training.utils import print_progress, manage_checkpoints, find_last_checkpoint, load_checkpoint_misc
 
 
 
 def train(config: ColBERTConfig, triples, queries=None, collection=None):
     if config.resume:
         config.checkpoint = config.checkpoint or find_last_checkpoint(config.checkpoint_path_)
     else:
```

### Comparing `PLAID-X-0.3.1/colbert/training/utils.py` & `plaid_x-0.3.1a0/plaidx/training/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import torch
 from pathlib import Path
 
-# from colbert.utils.runs import Run
-from colbert.infra import ColBERTConfig
-from colbert.utils.utils import print_message, save_checkpoint
-from colbert.parameters import SAVED_CHECKPOINTS
-# from colbert.infra.run import Run
+# from plaidx.utils.runs import Run
+from plaidx.infra import ColBERTConfig
+from plaidx.utils.utils import print_message, save_checkpoint
+from plaidx.parameters import SAVED_CHECKPOINTS
+# from plaidx.infra.run import Run
 
 def find_last_checkpoint(path: str):
     return str(Path(path) / "colbert")
 
 def print_progress(scores):
     positive_avg, negative_avg = round(scores[:, 0].mean().item(), 2), round(scores[:, 1].mean().item(), 2)
     print("#>>>   ", positive_avg, negative_avg, '\t\t|\t\t', positive_avg - negative_avg)
```

### Comparing `PLAID-X-0.3.1/colbert/utils/amp.py` & `plaid_x-0.3.1a0/plaidx/utils/amp.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch
 
 from contextlib import contextmanager
-from colbert.utils.utils import NullContextManager
+from plaidx.utils.utils import NullContextManager
 
 
 class MixedPrecisionManager():
     def __init__(self, activated):
         self.activated = activated
 
         if self.activated:
```

### Comparing `PLAID-X-0.3.1/colbert/utils/distributed.py` & `plaid_x-0.3.1a0/plaidx/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `PLAID-X-0.3.1/colbert/utils/logging.py` & `plaid_x-0.3.1a0/plaidx/utils/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import sys
 import ujson
 # import mlflow
 import traceback
 
 # from torch.utils.tensorboard import SummaryWriter
-from colbert.utils.utils import print_message, create_directory
+from plaidx.utils.utils import print_message, create_directory
 
 
 class Logger():
     def __init__(self, rank, run):
         self.rank = rank
         self.is_main = self.rank in [-1, 0]
         self.run = run
```

### Comparing `PLAID-X-0.3.1/colbert/utils/parser.py` & `plaid_x-0.3.1a0/plaidx/utils/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import copy
 import faiss
 
 from argparse import ArgumentParser
 
-import colbert.utils.distributed as distributed
-from colbert.utils.runs import Run
-from colbert.utils.utils import print_message, timestamp, create_directory
+import plaidx.utils.distributed as distributed
+from plaidx.utils.runs import Run
+from plaidx.utils.utils import print_message, timestamp, create_directory
 
 
 class Arguments():
     def __init__(self, description):
         self.parser = ArgumentParser(description=description)
         self.checks = []
```

### Comparing `PLAID-X-0.3.1/colbert/utils/runs.py` & `plaid_x-0.3.1a0/plaidx/utils/runs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
 import sys
 import time
 import __main__
 import traceback
 # import mlflow
 
-import colbert.utils.distributed as distributed
+import plaidx.utils.distributed as distributed
 
 from contextlib import contextmanager
-from colbert.utils.logging import Logger
-from colbert.utils.utils import timestamp, create_directory, print_message
+from plaidx.utils.logging import Logger
+from plaidx.utils.utils import timestamp, create_directory, print_message
 
 
 class _RunManager():
     def __init__(self):
         self.experiments_root = None
         self.experiment = None
         self.path = None
```

### Comparing `PLAID-X-0.3.1/colbert/utils/save_metadata.py` & `plaid_x-0.3.1a0/plaidx/utils/save_metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from colbert.utils.utils import dotdict
+from plaidx.utils.utils import dotdict
 import os
 import sys
 import git
 import time
 import copy
 import ujson
 import socket
```

### Comparing `PLAID-X-0.3.1/colbert/utils/utils.py` & `plaid_x-0.3.1a0/plaidx/utils/utils.py`

 * *Files identical despite different names*

