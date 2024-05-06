# Comparing `tmp/imodelsx-1.0.2.tar.gz` & `tmp/imodelsx-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imodelsx-1.0.2.tar", last modified: Mon May  6 03:14:44 2024, max compression
+gzip compressed data, was "imodelsx-1.0.3.tar", last modified: Mon May  6 03:19:24 2024, max compression
```

## Comparing `imodelsx-1.0.2.tar` & `imodelsx-1.0.3.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 03:14:44.298455 imodelsx-1.0.2/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    12670 2024-05-06 03:14:44.298455 imodelsx-1.0.2/PKG-INFO
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 03:14:44.294455 imodelsx-1.0.2/imodelsx/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      561 2023-12-13 21:38:50.000000 imodelsx-1.0.2/imodelsx/__init__.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 03:14:44.294455 imodelsx-1.0.2/imodelsx/auglinear/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2022-10-04 23:40:44.000000 imodelsx-1.0.2/imodelsx/auglinear/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    17684 2024-02-13 16:34:50.000000 imodelsx-1.0.2/imodelsx/auglinear/auglinear.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     7082 2024-02-13 16:36:25.000000 imodelsx-1.0.2/imodelsx/auglinear/embed.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 03:14:44.294455 imodelsx-1.0.2/imodelsx/augtree/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-01-24 23:36:41.000000 imodelsx-1.0.2/imodelsx/augtree/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    11437 2023-04-07 17:36:23.000000 imodelsx-1.0.2/imodelsx/augtree/augtree.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1273 2023-11-02 14:39:42.000000 imodelsx-1.0.2/imodelsx/augtree/data.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6465 2023-11-02 14:40:10.000000 imodelsx-1.0.2/imodelsx/augtree/embed.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2234 2023-02-06 22:48:13.000000 imodelsx-1.0.2/imodelsx/augtree/ensemble.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2380 2023-04-07 16:31:41.000000 imodelsx-1.0.2/imodelsx/augtree/llm.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    16783 2023-04-07 05:20:42.000000 imodelsx-1.0.2/imodelsx/augtree/stump.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3260 2023-11-02 14:40:40.000000 imodelsx-1.0.2/imodelsx/augtree/utils.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2120 2024-03-24 12:39:14.000000 imodelsx-1.0.2/imodelsx/cache_save_utils.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 03:14:44.294455 imodelsx-1.0.2/imodelsx/d3/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2022-10-04 21:38:29.000000 imodelsx-1.0.2/imodelsx/d3/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4312 2023-04-07 05:02:55.000000 imodelsx-1.0.2/imodelsx/d3/d3.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     7246 2022-10-04 22:03:12.000000 imodelsx-1.0.2/imodelsx/d3/step1_get_extreme.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     7194 2022-10-04 22:27:59.000000 imodelsx-1.0.2/imodelsx/d3/step2_proposer.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8982 2022-10-04 22:12:36.000000 imodelsx-1.0.2/imodelsx/d3/step3_verifier.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6130 2023-07-28 21:36:15.000000 imodelsx-1.0.2/imodelsx/data.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      282 2023-02-16 23:25:53.000000 imodelsx-1.0.2/imodelsx/dummy_script.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2516 2023-09-13 00:14:38.000000 imodelsx-1.0.2/imodelsx/embeddings.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 03:14:44.294455 imodelsx-1.0.2/imodelsx/iprompt/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      195 2022-10-15 16:18:36.000000 imodelsx-1.0.2/imodelsx/iprompt/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    36551 2023-06-07 16:00:03.000000 imodelsx-1.0.2/imodelsx/iprompt/api.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    11285 2023-06-07 16:00:03.000000 imodelsx-1.0.2/imodelsx/iprompt/autoprompt.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      624 2023-02-07 19:15:27.000000 imodelsx-1.0.2/imodelsx/iprompt/data.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2371 2022-10-15 16:18:36.000000 imodelsx-1.0.2/imodelsx/iprompt/gumbel.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    14226 2023-05-25 18:26:24.000000 imodelsx-1.0.2/imodelsx/iprompt/hotflip.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    19376 2023-06-07 16:00:03.000000 imodelsx-1.0.2/imodelsx/iprompt/ipromptx.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    12909 2023-06-07 16:01:30.000000 imodelsx-1.0.2/imodelsx/iprompt/llm.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1751 2022-10-15 16:18:36.000000 imodelsx-1.0.2/imodelsx/iprompt/prompt_tune.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    24166 2023-02-14 20:42:53.000000 imodelsx-1.0.2/imodelsx/iprompt/utils.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    15635 2024-05-06 03:13:17.000000 imodelsx-1.0.2/imodelsx/kan.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8220 2024-04-22 20:35:21.000000 imodelsx-1.0.2/imodelsx/linear_finetune.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5618 2023-11-02 14:37:02.000000 imodelsx-1.0.2/imodelsx/linear_ngram.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    22977 2024-04-25 16:47:27.000000 imodelsx-1.0.2/imodelsx/llm.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1577 2023-04-24 18:43:24.000000 imodelsx-1.0.2/imodelsx/metrics.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6214 2024-05-05 15:40:12.000000 imodelsx-1.0.2/imodelsx/process_results.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 03:14:44.298455 imodelsx-1.0.2/imodelsx/sasc/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-05-15 21:34:39.000000 imodelsx-1.0.2/imodelsx/sasc/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5670 2023-06-27 00:56:11.000000 imodelsx-1.0.2/imodelsx/sasc/api.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4951 2023-05-15 20:33:55.000000 imodelsx-1.0.2/imodelsx/sasc/m1_ngrams.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4957 2023-06-27 00:10:16.000000 imodelsx-1.0.2/imodelsx/sasc/m2_summarize.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3543 2023-06-27 00:10:23.000000 imodelsx-1.0.2/imodelsx/sasc/m3_generate.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    14860 2024-05-05 12:34:12.000000 imodelsx-1.0.2/imodelsx/submit_utils.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 03:14:44.298455 imodelsx-1.0.2/imodelsx/treeprompt/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-08-30 17:20:13.000000 imodelsx-1.0.2/imodelsx/treeprompt/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    13430 2023-10-10 15:55:49.000000 imodelsx-1.0.2/imodelsx/treeprompt/stump.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6709 2024-04-15 14:14:26.000000 imodelsx-1.0.2/imodelsx/treeprompt/treeprompt.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6342 2023-12-14 18:21:43.000000 imodelsx-1.0.2/imodelsx/util.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8794 2024-01-19 23:29:14.000000 imodelsx-1.0.2/imodelsx/viz.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 03:14:44.294455 imodelsx-1.0.2/imodelsx.egg-info/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    12670 2024-05-06 03:14:44.000000 imodelsx-1.0.2/imodelsx.egg-info/PKG-INFO
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1578 2024-05-06 03:14:44.000000 imodelsx-1.0.2/imodelsx.egg-info/SOURCES.txt
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        1 2024-05-06 03:14:44.000000 imodelsx-1.0.2/imodelsx.egg-info/dependency_links.txt
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      114 2024-05-06 03:14:44.000000 imodelsx-1.0.2/imodelsx.egg-info/requires.txt
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        9 2024-05-06 03:14:44.000000 imodelsx-1.0.2/imodelsx.egg-info/top_level.txt
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)       38 2024-05-06 03:14:44.298455 imodelsx-1.0.2/setup.cfg
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1323 2024-05-06 03:13:38.000000 imodelsx-1.0.2/setup.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 03:14:44.298455 imodelsx-1.0.2/tests/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      146 2023-12-13 21:39:12.000000 imodelsx-1.0.2/tests/test_auglinear.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1685 2023-12-13 21:40:29.000000 imodelsx-1.0.2/tests/test_auglinear_pipeline.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5451 2023-04-07 16:34:10.000000 imodelsx-1.0.2/tests/test_augtree.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1099 2023-02-07 19:05:22.000000 imodelsx-1.0.2/tests/test_iprompt.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      917 2024-03-23 14:38:38.000000 imodelsx-1.0.2/tests/test_llm.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1451 2023-04-07 03:36:08.000000 imodelsx-1.0.2/tests/test_ngram_list.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      786 2023-05-15 21:35:21.000000 imodelsx-1.0.2/tests/test_sasc.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 03:19:24.814867 imodelsx-1.0.3/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    12670 2024-05-06 03:19:24.814867 imodelsx-1.0.3/PKG-INFO
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 03:19:24.810867 imodelsx-1.0.3/imodelsx/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      561 2023-12-13 21:38:50.000000 imodelsx-1.0.3/imodelsx/__init__.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 03:19:24.810867 imodelsx-1.0.3/imodelsx/auglinear/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2022-10-04 23:40:44.000000 imodelsx-1.0.3/imodelsx/auglinear/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    17684 2024-02-13 16:34:50.000000 imodelsx-1.0.3/imodelsx/auglinear/auglinear.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     7082 2024-02-13 16:36:25.000000 imodelsx-1.0.3/imodelsx/auglinear/embed.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 03:19:24.814867 imodelsx-1.0.3/imodelsx/augtree/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-01-24 23:36:41.000000 imodelsx-1.0.3/imodelsx/augtree/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    11437 2023-04-07 17:36:23.000000 imodelsx-1.0.3/imodelsx/augtree/augtree.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1273 2023-11-02 14:39:42.000000 imodelsx-1.0.3/imodelsx/augtree/data.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6465 2023-11-02 14:40:10.000000 imodelsx-1.0.3/imodelsx/augtree/embed.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2234 2023-02-06 22:48:13.000000 imodelsx-1.0.3/imodelsx/augtree/ensemble.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2380 2023-04-07 16:31:41.000000 imodelsx-1.0.3/imodelsx/augtree/llm.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    16783 2023-04-07 05:20:42.000000 imodelsx-1.0.3/imodelsx/augtree/stump.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3260 2023-11-02 14:40:40.000000 imodelsx-1.0.3/imodelsx/augtree/utils.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2120 2024-03-24 12:39:14.000000 imodelsx-1.0.3/imodelsx/cache_save_utils.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 03:19:24.814867 imodelsx-1.0.3/imodelsx/d3/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2022-10-04 21:38:29.000000 imodelsx-1.0.3/imodelsx/d3/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4312 2023-04-07 05:02:55.000000 imodelsx-1.0.3/imodelsx/d3/d3.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     7246 2022-10-04 22:03:12.000000 imodelsx-1.0.3/imodelsx/d3/step1_get_extreme.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     7194 2022-10-04 22:27:59.000000 imodelsx-1.0.3/imodelsx/d3/step2_proposer.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8982 2022-10-04 22:12:36.000000 imodelsx-1.0.3/imodelsx/d3/step3_verifier.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6130 2023-07-28 21:36:15.000000 imodelsx-1.0.3/imodelsx/data.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      282 2023-02-16 23:25:53.000000 imodelsx-1.0.3/imodelsx/dummy_script.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2516 2023-09-13 00:14:38.000000 imodelsx-1.0.3/imodelsx/embeddings.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 03:19:24.814867 imodelsx-1.0.3/imodelsx/iprompt/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      195 2022-10-15 16:18:36.000000 imodelsx-1.0.3/imodelsx/iprompt/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    36551 2023-06-07 16:00:03.000000 imodelsx-1.0.3/imodelsx/iprompt/api.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    11285 2023-06-07 16:00:03.000000 imodelsx-1.0.3/imodelsx/iprompt/autoprompt.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      624 2023-02-07 19:15:27.000000 imodelsx-1.0.3/imodelsx/iprompt/data.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2371 2022-10-15 16:18:36.000000 imodelsx-1.0.3/imodelsx/iprompt/gumbel.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    14226 2023-05-25 18:26:24.000000 imodelsx-1.0.3/imodelsx/iprompt/hotflip.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    19376 2023-06-07 16:00:03.000000 imodelsx-1.0.3/imodelsx/iprompt/ipromptx.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    12909 2023-06-07 16:01:30.000000 imodelsx-1.0.3/imodelsx/iprompt/llm.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1751 2022-10-15 16:18:36.000000 imodelsx-1.0.3/imodelsx/iprompt/prompt_tune.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    24166 2023-02-14 20:42:53.000000 imodelsx-1.0.3/imodelsx/iprompt/utils.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    15542 2024-05-06 03:18:57.000000 imodelsx-1.0.3/imodelsx/kan.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8220 2024-04-22 20:35:21.000000 imodelsx-1.0.3/imodelsx/linear_finetune.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5618 2023-11-02 14:37:02.000000 imodelsx-1.0.3/imodelsx/linear_ngram.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    22977 2024-04-25 16:47:27.000000 imodelsx-1.0.3/imodelsx/llm.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1577 2023-04-24 18:43:24.000000 imodelsx-1.0.3/imodelsx/metrics.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6214 2024-05-05 15:40:12.000000 imodelsx-1.0.3/imodelsx/process_results.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 03:19:24.814867 imodelsx-1.0.3/imodelsx/sasc/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-05-15 21:34:39.000000 imodelsx-1.0.3/imodelsx/sasc/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5670 2023-06-27 00:56:11.000000 imodelsx-1.0.3/imodelsx/sasc/api.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4951 2023-05-15 20:33:55.000000 imodelsx-1.0.3/imodelsx/sasc/m1_ngrams.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4957 2023-06-27 00:10:16.000000 imodelsx-1.0.3/imodelsx/sasc/m2_summarize.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3543 2023-06-27 00:10:23.000000 imodelsx-1.0.3/imodelsx/sasc/m3_generate.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    14860 2024-05-05 12:34:12.000000 imodelsx-1.0.3/imodelsx/submit_utils.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 03:19:24.814867 imodelsx-1.0.3/imodelsx/treeprompt/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-08-30 17:20:13.000000 imodelsx-1.0.3/imodelsx/treeprompt/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    13430 2023-10-10 15:55:49.000000 imodelsx-1.0.3/imodelsx/treeprompt/stump.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6709 2024-04-15 14:14:26.000000 imodelsx-1.0.3/imodelsx/treeprompt/treeprompt.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6342 2023-12-14 18:21:43.000000 imodelsx-1.0.3/imodelsx/util.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8794 2024-01-19 23:29:14.000000 imodelsx-1.0.3/imodelsx/viz.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 03:19:24.810867 imodelsx-1.0.3/imodelsx.egg-info/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    12670 2024-05-06 03:19:24.000000 imodelsx-1.0.3/imodelsx.egg-info/PKG-INFO
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1578 2024-05-06 03:19:24.000000 imodelsx-1.0.3/imodelsx.egg-info/SOURCES.txt
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        1 2024-05-06 03:19:24.000000 imodelsx-1.0.3/imodelsx.egg-info/dependency_links.txt
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      114 2024-05-06 03:19:24.000000 imodelsx-1.0.3/imodelsx.egg-info/requires.txt
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        9 2024-05-06 03:19:24.000000 imodelsx-1.0.3/imodelsx.egg-info/top_level.txt
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)       38 2024-05-06 03:19:24.814867 imodelsx-1.0.3/setup.cfg
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1323 2024-05-06 03:19:11.000000 imodelsx-1.0.3/setup.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 03:19:24.814867 imodelsx-1.0.3/tests/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      146 2023-12-13 21:39:12.000000 imodelsx-1.0.3/tests/test_auglinear.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1685 2023-12-13 21:40:29.000000 imodelsx-1.0.3/tests/test_auglinear_pipeline.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5451 2023-04-07 16:34:10.000000 imodelsx-1.0.3/tests/test_augtree.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1099 2023-02-07 19:05:22.000000 imodelsx-1.0.3/tests/test_iprompt.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      917 2024-03-23 14:38:38.000000 imodelsx-1.0.3/tests/test_llm.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1451 2023-04-07 03:36:08.000000 imodelsx-1.0.3/tests/test_ngram_list.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      786 2023-05-15 21:35:21.000000 imodelsx-1.0.3/tests/test_sasc.py
```

### Comparing `imodelsx-1.0.2/PKG-INFO` & `imodelsx-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imodelsx
-Version: 1.0.2
+Version: 1.0.3
 Summary: Library to explain a dataset in natural language.
 Home-page: https://github.com/csinva/imodelsX
 Author: Chandan Singh, John X. Morris, Armin Askari, Divyanshu Aggarwal, Aliyah Hsu, Yuntian Deng
 Author-email: chansingh@microsoft.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: imodelsx Version: 1.0.2 Summary: Library to explain
+Metadata-Version: 2.1 Name: imodelsx Version: 1.0.3 Summary: Library to explain
 a dataset in natural language. Home-page: https://github.com/csinva/imodelsX
 Author: Chandan Singh, John X. Morris, Armin Askari, Divyanshu Aggarwal, Aliyah
 Hsu, Yuntian Deng Author-email: chansingh@microsoft.com Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.9
 Description-Content-Type: text/markdown
   [https://microsoft.github.io/aug-models/embgam_gif.gif][https://csinva.io/
```

### Comparing `imodelsx-1.0.2/imodelsx/__init__.py` & `imodelsx-1.0.3/imodelsx/__init__.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx/auglinear/auglinear.py` & `imodelsx-1.0.3/imodelsx/auglinear/auglinear.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx/auglinear/embed.py` & `imodelsx-1.0.3/imodelsx/auglinear/embed.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx/augtree/augtree.py` & `imodelsx-1.0.3/imodelsx/augtree/augtree.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx/augtree/data.py` & `imodelsx-1.0.3/imodelsx/augtree/data.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx/augtree/embed.py` & `imodelsx-1.0.3/imodelsx/augtree/embed.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx/augtree/ensemble.py` & `imodelsx-1.0.3/imodelsx/augtree/ensemble.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx/augtree/llm.py` & `imodelsx-1.0.3/imodelsx/augtree/llm.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx/augtree/stump.py` & `imodelsx-1.0.3/imodelsx/augtree/stump.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx/augtree/utils.py` & `imodelsx-1.0.3/imodelsx/augtree/utils.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx/cache_save_utils.py` & `imodelsx-1.0.3/imodelsx/cache_save_utils.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx/d3/d3.py` & `imodelsx-1.0.3/imodelsx/d3/d3.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx/d3/step1_get_extreme.py` & `imodelsx-1.0.3/imodelsx/d3/step1_get_extreme.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx/d3/step2_proposer.py` & `imodelsx-1.0.3/imodelsx/d3/step2_proposer.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx/d3/step3_verifier.py` & `imodelsx-1.0.3/imodelsx/d3/step3_verifier.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx/data.py` & `imodelsx-1.0.3/imodelsx/data.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx/embeddings.py` & `imodelsx-1.0.3/imodelsx/embeddings.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx/iprompt/api.py` & `imodelsx-1.0.3/imodelsx/iprompt/api.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx/iprompt/autoprompt.py` & `imodelsx-1.0.3/imodelsx/iprompt/autoprompt.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx/iprompt/data.py` & `imodelsx-1.0.3/imodelsx/iprompt/data.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx/iprompt/gumbel.py` & `imodelsx-1.0.3/imodelsx/iprompt/gumbel.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx/iprompt/hotflip.py` & `imodelsx-1.0.3/imodelsx/iprompt/hotflip.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx/iprompt/ipromptx.py` & `imodelsx-1.0.3/imodelsx/iprompt/ipromptx.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx/iprompt/llm.py` & `imodelsx-1.0.3/imodelsx/iprompt/llm.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx/iprompt/prompt_tune.py` & `imodelsx-1.0.3/imodelsx/iprompt/prompt_tune.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx/iprompt/utils.py` & `imodelsx-1.0.3/imodelsx/iprompt/utils.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx/kan.py` & `imodelsx-1.0.3/imodelsx/kan.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,15 +314,15 @@
             Number of neurons in the hidden layer.
         '''
         self.hidden_layer_size = hidden_layer_size
         self.device = device
         self.regularize_activation = regularize_activation
         self.regularize_entropy = regularize_entropy
 
-    def fit(self, X, y, batch_size=512):
+    def fit(self, X, y, batch_size=512, lr=1e-3, weight_decay=1e-4, gamma=0.8):
         if isinstance(self, ClassifierMixin):
             check_classification_targets(y)
             self.classes_, y = np.unique(y, return_inverse=True)
             num_outputs = len(self.classes_)
             y = torch.tensor(y, dtype=torch.long)
         else:
             num_outputs = 1
@@ -341,16 +341,16 @@
         dset_tune = torch.utils.data.TensorDataset(X_tune, y_tune)
         loader_train = DataLoader(
             dset_train, batch_size=batch_size, shuffle=True)
         loader_tune = DataLoader(
             dset_tune, batch_size=batch_size, shuffle=False)
 
         optimizer = optim.AdamW(self.model.parameters(),
-                                lr=1e-3, weight_decay=1e-4)
-        scheduler = optim.lr_scheduler.ExponentialLR(optimizer, gamma=0.8)
+                                lr=lr, weight_decay=weight_decay)
+        scheduler = optim.lr_scheduler.ExponentialLR(optimizer, gamma=gamma)
 
         # Define loss
         if isinstance(self, ClassifierMixin):
             criterion = nn.CrossEntropyLoss()
         else:
             criterion = nn.MSELoss()
         tune_losses = []
@@ -374,22 +374,16 @@
                 for x, labs in loader_tune:
                     x = x.view(-1, num_features).to(self.device)
                     output = self.model(x).squeeze()
                     tune_loss += criterion(output,
                                            labs.to(self.device).squeeze()).item()
             tune_loss /= len(loader_tune)
             tune_losses.append(tune_loss)
-
-            # Update learning rate
             scheduler.step()
 
-            # print(
-            #     f"Epoch {epoch + 1}, Tune Loss: {val_loss:.4f}"
-            # )
-
             # apply early stopping
             if len(tune_losses) > 3 and tune_losses[-1] > tune_losses[-2]:
                 print("Early stopping")
                 return self
 
         return self
```

### Comparing `imodelsx-1.0.2/imodelsx/linear_finetune.py` & `imodelsx-1.0.3/imodelsx/linear_finetune.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx/linear_ngram.py` & `imodelsx-1.0.3/imodelsx/linear_ngram.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx/llm.py` & `imodelsx-1.0.3/imodelsx/llm.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx/metrics.py` & `imodelsx-1.0.3/imodelsx/metrics.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx/process_results.py` & `imodelsx-1.0.3/imodelsx/process_results.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx/sasc/api.py` & `imodelsx-1.0.3/imodelsx/sasc/api.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx/sasc/m1_ngrams.py` & `imodelsx-1.0.3/imodelsx/sasc/m1_ngrams.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx/sasc/m2_summarize.py` & `imodelsx-1.0.3/imodelsx/sasc/m2_summarize.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx/sasc/m3_generate.py` & `imodelsx-1.0.3/imodelsx/sasc/m3_generate.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx/submit_utils.py` & `imodelsx-1.0.3/imodelsx/submit_utils.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx/treeprompt/stump.py` & `imodelsx-1.0.3/imodelsx/treeprompt/stump.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx/treeprompt/treeprompt.py` & `imodelsx-1.0.3/imodelsx/treeprompt/treeprompt.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx/util.py` & `imodelsx-1.0.3/imodelsx/util.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx/viz.py` & `imodelsx-1.0.3/imodelsx/viz.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/imodelsx.egg-info/PKG-INFO` & `imodelsx-1.0.3/imodelsx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imodelsx
-Version: 1.0.2
+Version: 1.0.3
 Summary: Library to explain a dataset in natural language.
 Home-page: https://github.com/csinva/imodelsX
 Author: Chandan Singh, John X. Morris, Armin Askari, Divyanshu Aggarwal, Aliyah Hsu, Yuntian Deng
 Author-email: chansingh@microsoft.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: imodelsx Version: 1.0.2 Summary: Library to explain
+Metadata-Version: 2.1 Name: imodelsx Version: 1.0.3 Summary: Library to explain
 a dataset in natural language. Home-page: https://github.com/csinva/imodelsX
 Author: Chandan Singh, John X. Morris, Armin Askari, Divyanshu Aggarwal, Aliyah
 Hsu, Yuntian Deng Author-email: chansingh@microsoft.com Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.9
 Description-Content-Type: text/markdown
   [https://microsoft.github.io/aug-models/embgam_gif.gif][https://csinva.io/
```

### Comparing `imodelsx-1.0.2/imodelsx.egg-info/SOURCES.txt` & `imodelsx-1.0.3/imodelsx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/setup.py` & `imodelsx-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     # 'InstructorEmbedding', # embeddings for emb_diff_module
     # 'sentence-transformers', # embeddings for emb_diff_module
     # pdoc3 # for generating docs
 ]
 
 setuptools.setup(
     name="imodelsx",
-    version="1.0.2",
+    version="1.0.3",
     author="Chandan Singh, John X. Morris, Armin Askari, Divyanshu Aggarwal, Aliyah Hsu, Yuntian Deng",
     author_email="chansingh@microsoft.com",
     description="Library to explain a dataset in natural language.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/csinva/imodelsX",
     packages=setuptools.find_packages(
```

### Comparing `imodelsx-1.0.2/tests/test_auglinear_pipeline.py` & `imodelsx-1.0.3/tests/test_auglinear_pipeline.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/tests/test_augtree.py` & `imodelsx-1.0.3/tests/test_augtree.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/tests/test_iprompt.py` & `imodelsx-1.0.3/tests/test_iprompt.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/tests/test_llm.py` & `imodelsx-1.0.3/tests/test_llm.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/tests/test_ngram_list.py` & `imodelsx-1.0.3/tests/test_ngram_list.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.2/tests/test_sasc.py` & `imodelsx-1.0.3/tests/test_sasc.py`

 * *Files identical despite different names*

