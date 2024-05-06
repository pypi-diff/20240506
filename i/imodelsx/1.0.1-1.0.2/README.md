# Comparing `tmp/imodelsx-1.0.1.tar.gz` & `tmp/imodelsx-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imodelsx-1.0.1.tar", last modified: Sat Apr 20 00:17:00 2024, max compression
+gzip compressed data, was "imodelsx-1.0.2.tar", last modified: Mon May  6 03:14:44 2024, max compression
```

## Comparing `imodelsx-1.0.1.tar` & `imodelsx-1.0.2.tar`

### file list

```diff
@@ -1,72 +1,73 @@
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-04-20 00:17:00.121135 imodelsx-1.0.1/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    12670 2024-04-20 00:17:00.121135 imodelsx-1.0.1/PKG-INFO
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-04-20 00:17:00.117134 imodelsx-1.0.1/imodelsx/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      561 2023-12-13 21:38:50.000000 imodelsx-1.0.1/imodelsx/__init__.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-04-20 00:17:00.117134 imodelsx-1.0.1/imodelsx/auglinear/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2022-10-04 23:40:44.000000 imodelsx-1.0.1/imodelsx/auglinear/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    17684 2024-02-13 16:34:50.000000 imodelsx-1.0.1/imodelsx/auglinear/auglinear.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     7082 2024-02-13 16:36:25.000000 imodelsx-1.0.1/imodelsx/auglinear/embed.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-04-20 00:17:00.117134 imodelsx-1.0.1/imodelsx/augtree/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-01-24 23:36:41.000000 imodelsx-1.0.1/imodelsx/augtree/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    11437 2023-04-07 17:36:23.000000 imodelsx-1.0.1/imodelsx/augtree/augtree.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1273 2023-11-02 14:39:42.000000 imodelsx-1.0.1/imodelsx/augtree/data.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6465 2023-11-02 14:40:10.000000 imodelsx-1.0.1/imodelsx/augtree/embed.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2234 2023-02-06 22:48:13.000000 imodelsx-1.0.1/imodelsx/augtree/ensemble.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2380 2023-04-07 16:31:41.000000 imodelsx-1.0.1/imodelsx/augtree/llm.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    16783 2023-04-07 05:20:42.000000 imodelsx-1.0.1/imodelsx/augtree/stump.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3260 2023-11-02 14:40:40.000000 imodelsx-1.0.1/imodelsx/augtree/utils.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2120 2024-03-24 12:39:14.000000 imodelsx-1.0.1/imodelsx/cache_save_utils.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-04-20 00:17:00.117134 imodelsx-1.0.1/imodelsx/d3/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2022-10-04 21:38:29.000000 imodelsx-1.0.1/imodelsx/d3/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4312 2023-04-07 05:02:55.000000 imodelsx-1.0.1/imodelsx/d3/d3.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     7246 2022-10-04 22:03:12.000000 imodelsx-1.0.1/imodelsx/d3/step1_get_extreme.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     7194 2022-10-04 22:27:59.000000 imodelsx-1.0.1/imodelsx/d3/step2_proposer.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8982 2022-10-04 22:12:36.000000 imodelsx-1.0.1/imodelsx/d3/step3_verifier.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6130 2023-07-28 21:36:15.000000 imodelsx-1.0.1/imodelsx/data.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      282 2023-02-16 23:25:53.000000 imodelsx-1.0.1/imodelsx/dummy_script.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2516 2023-09-13 00:14:38.000000 imodelsx-1.0.1/imodelsx/embeddings.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-04-20 00:17:00.121135 imodelsx-1.0.1/imodelsx/iprompt/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      195 2022-10-15 16:18:36.000000 imodelsx-1.0.1/imodelsx/iprompt/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    36551 2023-06-07 16:00:03.000000 imodelsx-1.0.1/imodelsx/iprompt/api.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    11285 2023-06-07 16:00:03.000000 imodelsx-1.0.1/imodelsx/iprompt/autoprompt.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      624 2023-02-07 19:15:27.000000 imodelsx-1.0.1/imodelsx/iprompt/data.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2371 2022-10-15 16:18:36.000000 imodelsx-1.0.1/imodelsx/iprompt/gumbel.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    14226 2023-05-25 18:26:24.000000 imodelsx-1.0.1/imodelsx/iprompt/hotflip.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    19376 2023-06-07 16:00:03.000000 imodelsx-1.0.1/imodelsx/iprompt/ipromptx.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    12909 2023-06-07 16:01:30.000000 imodelsx-1.0.1/imodelsx/iprompt/llm.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1751 2022-10-15 16:18:36.000000 imodelsx-1.0.1/imodelsx/iprompt/prompt_tune.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    24166 2023-02-14 20:42:53.000000 imodelsx-1.0.1/imodelsx/iprompt/utils.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8181 2024-04-12 13:28:41.000000 imodelsx-1.0.1/imodelsx/linear_finetune.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5618 2023-11-02 14:37:02.000000 imodelsx-1.0.1/imodelsx/linear_ngram.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    22658 2024-04-20 00:15:34.000000 imodelsx-1.0.1/imodelsx/llm.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1577 2023-04-24 18:43:24.000000 imodelsx-1.0.1/imodelsx/metrics.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6148 2024-04-19 21:47:37.000000 imodelsx-1.0.1/imodelsx/process_results.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-04-20 00:17:00.121135 imodelsx-1.0.1/imodelsx/sasc/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-05-15 21:34:39.000000 imodelsx-1.0.1/imodelsx/sasc/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5670 2023-06-27 00:56:11.000000 imodelsx-1.0.1/imodelsx/sasc/api.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4951 2023-05-15 20:33:55.000000 imodelsx-1.0.1/imodelsx/sasc/m1_ngrams.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4957 2023-06-27 00:10:16.000000 imodelsx-1.0.1/imodelsx/sasc/m2_summarize.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3543 2023-06-27 00:10:23.000000 imodelsx-1.0.1/imodelsx/sasc/m3_generate.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    14826 2024-04-03 15:01:50.000000 imodelsx-1.0.1/imodelsx/submit_utils.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-04-20 00:17:00.121135 imodelsx-1.0.1/imodelsx/treeprompt/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-08-30 17:20:13.000000 imodelsx-1.0.1/imodelsx/treeprompt/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    13430 2023-10-10 15:55:49.000000 imodelsx-1.0.1/imodelsx/treeprompt/stump.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6709 2024-04-15 14:14:26.000000 imodelsx-1.0.1/imodelsx/treeprompt/treeprompt.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6342 2023-12-14 18:21:43.000000 imodelsx-1.0.1/imodelsx/util.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8794 2024-01-19 23:29:14.000000 imodelsx-1.0.1/imodelsx/viz.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-04-20 00:17:00.117134 imodelsx-1.0.1/imodelsx.egg-info/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    12670 2024-04-20 00:17:00.000000 imodelsx-1.0.1/imodelsx.egg-info/PKG-INFO
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1562 2024-04-20 00:17:00.000000 imodelsx-1.0.1/imodelsx.egg-info/SOURCES.txt
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        1 2024-04-20 00:17:00.000000 imodelsx-1.0.1/imodelsx.egg-info/dependency_links.txt
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      114 2024-04-20 00:17:00.000000 imodelsx-1.0.1/imodelsx.egg-info/requires.txt
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        9 2024-04-20 00:17:00.000000 imodelsx-1.0.1/imodelsx.egg-info/top_level.txt
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)       38 2024-04-20 00:17:00.121135 imodelsx-1.0.1/setup.cfg
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1323 2024-04-20 00:16:12.000000 imodelsx-1.0.1/setup.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-04-20 00:17:00.121135 imodelsx-1.0.1/tests/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      146 2023-12-13 21:39:12.000000 imodelsx-1.0.1/tests/test_auglinear.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1685 2023-12-13 21:40:29.000000 imodelsx-1.0.1/tests/test_auglinear_pipeline.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5451 2023-04-07 16:34:10.000000 imodelsx-1.0.1/tests/test_augtree.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1099 2023-02-07 19:05:22.000000 imodelsx-1.0.1/tests/test_iprompt.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      917 2024-03-23 14:38:38.000000 imodelsx-1.0.1/tests/test_llm.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1451 2023-04-07 03:36:08.000000 imodelsx-1.0.1/tests/test_ngram_list.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      786 2023-05-15 21:35:21.000000 imodelsx-1.0.1/tests/test_sasc.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 03:14:44.298455 imodelsx-1.0.2/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    12670 2024-05-06 03:14:44.298455 imodelsx-1.0.2/PKG-INFO
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 03:14:44.294455 imodelsx-1.0.2/imodelsx/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      561 2023-12-13 21:38:50.000000 imodelsx-1.0.2/imodelsx/__init__.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 03:14:44.294455 imodelsx-1.0.2/imodelsx/auglinear/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2022-10-04 23:40:44.000000 imodelsx-1.0.2/imodelsx/auglinear/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    17684 2024-02-13 16:34:50.000000 imodelsx-1.0.2/imodelsx/auglinear/auglinear.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     7082 2024-02-13 16:36:25.000000 imodelsx-1.0.2/imodelsx/auglinear/embed.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 03:14:44.294455 imodelsx-1.0.2/imodelsx/augtree/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-01-24 23:36:41.000000 imodelsx-1.0.2/imodelsx/augtree/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    11437 2023-04-07 17:36:23.000000 imodelsx-1.0.2/imodelsx/augtree/augtree.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1273 2023-11-02 14:39:42.000000 imodelsx-1.0.2/imodelsx/augtree/data.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6465 2023-11-02 14:40:10.000000 imodelsx-1.0.2/imodelsx/augtree/embed.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2234 2023-02-06 22:48:13.000000 imodelsx-1.0.2/imodelsx/augtree/ensemble.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2380 2023-04-07 16:31:41.000000 imodelsx-1.0.2/imodelsx/augtree/llm.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    16783 2023-04-07 05:20:42.000000 imodelsx-1.0.2/imodelsx/augtree/stump.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3260 2023-11-02 14:40:40.000000 imodelsx-1.0.2/imodelsx/augtree/utils.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2120 2024-03-24 12:39:14.000000 imodelsx-1.0.2/imodelsx/cache_save_utils.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 03:14:44.294455 imodelsx-1.0.2/imodelsx/d3/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2022-10-04 21:38:29.000000 imodelsx-1.0.2/imodelsx/d3/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4312 2023-04-07 05:02:55.000000 imodelsx-1.0.2/imodelsx/d3/d3.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     7246 2022-10-04 22:03:12.000000 imodelsx-1.0.2/imodelsx/d3/step1_get_extreme.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     7194 2022-10-04 22:27:59.000000 imodelsx-1.0.2/imodelsx/d3/step2_proposer.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8982 2022-10-04 22:12:36.000000 imodelsx-1.0.2/imodelsx/d3/step3_verifier.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6130 2023-07-28 21:36:15.000000 imodelsx-1.0.2/imodelsx/data.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      282 2023-02-16 23:25:53.000000 imodelsx-1.0.2/imodelsx/dummy_script.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2516 2023-09-13 00:14:38.000000 imodelsx-1.0.2/imodelsx/embeddings.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 03:14:44.294455 imodelsx-1.0.2/imodelsx/iprompt/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      195 2022-10-15 16:18:36.000000 imodelsx-1.0.2/imodelsx/iprompt/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    36551 2023-06-07 16:00:03.000000 imodelsx-1.0.2/imodelsx/iprompt/api.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    11285 2023-06-07 16:00:03.000000 imodelsx-1.0.2/imodelsx/iprompt/autoprompt.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      624 2023-02-07 19:15:27.000000 imodelsx-1.0.2/imodelsx/iprompt/data.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2371 2022-10-15 16:18:36.000000 imodelsx-1.0.2/imodelsx/iprompt/gumbel.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    14226 2023-05-25 18:26:24.000000 imodelsx-1.0.2/imodelsx/iprompt/hotflip.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    19376 2023-06-07 16:00:03.000000 imodelsx-1.0.2/imodelsx/iprompt/ipromptx.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    12909 2023-06-07 16:01:30.000000 imodelsx-1.0.2/imodelsx/iprompt/llm.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1751 2022-10-15 16:18:36.000000 imodelsx-1.0.2/imodelsx/iprompt/prompt_tune.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    24166 2023-02-14 20:42:53.000000 imodelsx-1.0.2/imodelsx/iprompt/utils.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    15635 2024-05-06 03:13:17.000000 imodelsx-1.0.2/imodelsx/kan.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8220 2024-04-22 20:35:21.000000 imodelsx-1.0.2/imodelsx/linear_finetune.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5618 2023-11-02 14:37:02.000000 imodelsx-1.0.2/imodelsx/linear_ngram.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    22977 2024-04-25 16:47:27.000000 imodelsx-1.0.2/imodelsx/llm.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1577 2023-04-24 18:43:24.000000 imodelsx-1.0.2/imodelsx/metrics.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6214 2024-05-05 15:40:12.000000 imodelsx-1.0.2/imodelsx/process_results.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 03:14:44.298455 imodelsx-1.0.2/imodelsx/sasc/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-05-15 21:34:39.000000 imodelsx-1.0.2/imodelsx/sasc/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5670 2023-06-27 00:56:11.000000 imodelsx-1.0.2/imodelsx/sasc/api.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4951 2023-05-15 20:33:55.000000 imodelsx-1.0.2/imodelsx/sasc/m1_ngrams.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4957 2023-06-27 00:10:16.000000 imodelsx-1.0.2/imodelsx/sasc/m2_summarize.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3543 2023-06-27 00:10:23.000000 imodelsx-1.0.2/imodelsx/sasc/m3_generate.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    14860 2024-05-05 12:34:12.000000 imodelsx-1.0.2/imodelsx/submit_utils.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 03:14:44.298455 imodelsx-1.0.2/imodelsx/treeprompt/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-08-30 17:20:13.000000 imodelsx-1.0.2/imodelsx/treeprompt/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    13430 2023-10-10 15:55:49.000000 imodelsx-1.0.2/imodelsx/treeprompt/stump.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6709 2024-04-15 14:14:26.000000 imodelsx-1.0.2/imodelsx/treeprompt/treeprompt.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6342 2023-12-14 18:21:43.000000 imodelsx-1.0.2/imodelsx/util.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8794 2024-01-19 23:29:14.000000 imodelsx-1.0.2/imodelsx/viz.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 03:14:44.294455 imodelsx-1.0.2/imodelsx.egg-info/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    12670 2024-05-06 03:14:44.000000 imodelsx-1.0.2/imodelsx.egg-info/PKG-INFO
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1578 2024-05-06 03:14:44.000000 imodelsx-1.0.2/imodelsx.egg-info/SOURCES.txt
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        1 2024-05-06 03:14:44.000000 imodelsx-1.0.2/imodelsx.egg-info/dependency_links.txt
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      114 2024-05-06 03:14:44.000000 imodelsx-1.0.2/imodelsx.egg-info/requires.txt
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        9 2024-05-06 03:14:44.000000 imodelsx-1.0.2/imodelsx.egg-info/top_level.txt
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)       38 2024-05-06 03:14:44.298455 imodelsx-1.0.2/setup.cfg
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1323 2024-05-06 03:13:38.000000 imodelsx-1.0.2/setup.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 03:14:44.298455 imodelsx-1.0.2/tests/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      146 2023-12-13 21:39:12.000000 imodelsx-1.0.2/tests/test_auglinear.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1685 2023-12-13 21:40:29.000000 imodelsx-1.0.2/tests/test_auglinear_pipeline.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5451 2023-04-07 16:34:10.000000 imodelsx-1.0.2/tests/test_augtree.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1099 2023-02-07 19:05:22.000000 imodelsx-1.0.2/tests/test_iprompt.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      917 2024-03-23 14:38:38.000000 imodelsx-1.0.2/tests/test_llm.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1451 2023-04-07 03:36:08.000000 imodelsx-1.0.2/tests/test_ngram_list.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      786 2023-05-15 21:35:21.000000 imodelsx-1.0.2/tests/test_sasc.py
```

### Comparing `imodelsx-1.0.1/PKG-INFO` & `imodelsx-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imodelsx
-Version: 1.0.1
+Version: 1.0.2
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
-Metadata-Version: 2.1 Name: imodelsx Version: 1.0.1 Summary: Library to explain
+Metadata-Version: 2.1 Name: imodelsx Version: 1.0.2 Summary: Library to explain
 a dataset in natural language. Home-page: https://github.com/csinva/imodelsX
 Author: Chandan Singh, John X. Morris, Armin Askari, Divyanshu Aggarwal, Aliyah
 Hsu, Yuntian Deng Author-email: chansingh@microsoft.com Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.9
 Description-Content-Type: text/markdown
   [https://microsoft.github.io/aug-models/embgam_gif.gif][https://csinva.io/
```

### Comparing `imodelsx-1.0.1/imodelsx/__init__.py` & `imodelsx-1.0.2/imodelsx/__init__.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/imodelsx/auglinear/auglinear.py` & `imodelsx-1.0.2/imodelsx/auglinear/auglinear.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/imodelsx/auglinear/embed.py` & `imodelsx-1.0.2/imodelsx/auglinear/embed.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/imodelsx/augtree/augtree.py` & `imodelsx-1.0.2/imodelsx/augtree/augtree.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/imodelsx/augtree/data.py` & `imodelsx-1.0.2/imodelsx/augtree/data.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/imodelsx/augtree/embed.py` & `imodelsx-1.0.2/imodelsx/augtree/embed.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/imodelsx/augtree/ensemble.py` & `imodelsx-1.0.2/imodelsx/augtree/ensemble.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/imodelsx/augtree/llm.py` & `imodelsx-1.0.2/imodelsx/augtree/llm.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/imodelsx/augtree/stump.py` & `imodelsx-1.0.2/imodelsx/augtree/stump.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/imodelsx/augtree/utils.py` & `imodelsx-1.0.2/imodelsx/augtree/utils.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/imodelsx/cache_save_utils.py` & `imodelsx-1.0.2/imodelsx/cache_save_utils.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/imodelsx/d3/d3.py` & `imodelsx-1.0.2/imodelsx/d3/d3.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/imodelsx/d3/step1_get_extreme.py` & `imodelsx-1.0.2/imodelsx/d3/step1_get_extreme.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/imodelsx/d3/step2_proposer.py` & `imodelsx-1.0.2/imodelsx/d3/step2_proposer.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/imodelsx/d3/step3_verifier.py` & `imodelsx-1.0.2/imodelsx/d3/step3_verifier.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/imodelsx/data.py` & `imodelsx-1.0.2/imodelsx/data.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/imodelsx/embeddings.py` & `imodelsx-1.0.2/imodelsx/embeddings.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/imodelsx/iprompt/api.py` & `imodelsx-1.0.2/imodelsx/iprompt/api.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/imodelsx/iprompt/autoprompt.py` & `imodelsx-1.0.2/imodelsx/iprompt/autoprompt.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/imodelsx/iprompt/data.py` & `imodelsx-1.0.2/imodelsx/iprompt/data.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/imodelsx/iprompt/gumbel.py` & `imodelsx-1.0.2/imodelsx/iprompt/gumbel.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/imodelsx/iprompt/hotflip.py` & `imodelsx-1.0.2/imodelsx/iprompt/hotflip.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/imodelsx/iprompt/ipromptx.py` & `imodelsx-1.0.2/imodelsx/iprompt/ipromptx.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/imodelsx/iprompt/llm.py` & `imodelsx-1.0.2/imodelsx/iprompt/llm.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/imodelsx/iprompt/prompt_tune.py` & `imodelsx-1.0.2/imodelsx/iprompt/prompt_tune.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/imodelsx/iprompt/utils.py` & `imodelsx-1.0.2/imodelsx/iprompt/utils.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/imodelsx/linear_finetune.py` & `imodelsx-1.0.2/imodelsx/linear_finetune.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,26 +17,25 @@
 import os.path
 import warnings
 import pickle as pkl
 import torch
 import torch.nn
 from sklearn.exceptions import ConvergenceWarning
 
-device = "cuda" if torch.cuda.is_available() else "cpu"
-
 
 class LinearFinetune(BaseEstimator):
     def __init__(
         self,
         checkpoint: str = "bert-base-uncased",
         layer: str = "last_hidden_state",
         random_state=None,
         normalize_embs=False,
         cache_embs_dir: str = None,
         verbose: int = 0,
+        device="cuda" if torch.cuda.is_available() else "cpu"
     ):
         """LinearFinetune Class - use either LinearFinetuneClassifier or LinearFinetuneRegressor rather than initializing this class directly.
 
         Parameters
         ----------
         checkpoint: str
             Name of model checkpoint (i.e. to be fetch by huggingface)
@@ -75,19 +74,20 @@
         """
         self.checkpoint = checkpoint
         self.layer = layer
         self.random_state = random_state
         self.normalize_embs = normalize_embs
         self.cache_embs_dir = cache_embs_dir
         self.verbose = verbose
+        self.device = device
         self._initialize_checkpoint_and_tokenizer()
 
     def _initialize_checkpoint_and_tokenizer(self):
         self.model = transformers.AutoModel.from_pretrained(
-            self.checkpoint).to(device)
+            self.checkpoint).to(self.device)
         self.tokenizer = transformers.AutoTokenizer.from_pretrained(
             self.checkpoint)
 
     def fit(
         self,
         X_text: ArrayLike,
         y: ArrayLike,
```

### Comparing `imodelsx-1.0.1/imodelsx/linear_ngram.py` & `imodelsx-1.0.2/imodelsx/linear_ngram.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/imodelsx/llm.py` & `imodelsx-1.0.2/imodelsx/llm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from copy import deepcopy
 import json
 from transformers import (
     T5ForConditionalGeneration,
 )
+from datasets import Dataset
 import transformers
 from transformers import AutoConfig, AutoModel, AutoTokenizer, AutoModelForCausalLM
 import re
 from transformers import LlamaForCausalLM, LlamaTokenizer
 from typing import Any, Dict, List, Mapping, Optional, Union
 import numpy as np
 import os.path
@@ -57,15 +58,15 @@
         LLM_CONFIG["LLM_REPEAT_DELAY"] = repeat_delay
 
     """Get an LLM with a call function and caching capabilities"""
     if checkpoint.startswith("text-da"):
         return LLM_OpenAI(checkpoint, seed=seed, CACHE_DIR=CACHE_DIR)
     elif checkpoint.startswith("gpt-3") or checkpoint.startswith("gpt-4"):
         return LLM_Chat(checkpoint, seed, role, CACHE_DIR)
-    elif 'Meta-Llama-3-8B' in checkpoint and 'Instruct' in checkpoint:
+    elif 'Meta-Llama-3' in checkpoint and 'Instruct' in checkpoint:
         return LLM_HF_Pipeline(checkpoint, CACHE_DIR)
     else:
         # warning: this sets torch.manual_seed(seed)
         return LLM_HF(checkpoint, seed=seed, CACHE_DIR=CACHE_DIR, LLAMA_DIR=LLAMA_DIR)
 
 
 def repeatedly_call_with_delay(llm_call):
@@ -319,25 +320,30 @@
 
 class LLM_HF_Pipeline:
     def __init__(self, checkpoint, CACHE_DIR):
 
         self.pipeline_ = transformers.pipeline(
             "text-generation",
             model=checkpoint,
-            model_kwargs={"torch_dtype": torch.bfloat16},
+            # model_kwargs={"torch_dtype": torch.bfloat16},
+            # , 'device_map': "auto"},
+            model_kwargs={'torch_dtype': torch.float16},
             device_map="auto"
         )
+        self.pipeline_.tokenizer.pad_token_id = self.pipeline_.tokenizer.eos_token_id
+        self.pipeline_.tokenizer.padding_side = 'left'
         self.cache_dir = join(CACHE_DIR)
 
     def __call__(
         self,
         prompt: Union[str, List[str]],
         max_new_tokens=20,
         use_cache=True,
         verbose=False,
+        batch_size=64,
     ):
 
         if use_cache:
             os.makedirs(self.cache_dir, exist_ok=True)
             hash_str = hashlib.sha256(str(prompt).encode()).hexdigest()
             cache_file = join(
                 self.cache_dir, f"{hash_str}__num_tok={max_new_tokens}.pkl"
@@ -351,16 +357,17 @@
                 except:
                     print('failed to load cache so rerunning...')
             if verbose:
                 print("not cached...")
         outputs = self.pipeline_(
             prompt,
             max_new_tokens=max_new_tokens,
+            batch_size=batch_size,
+            do_sample=False,
         )
-        print('outs', outputs)
         if isinstance(prompt, str):
             texts = outputs[0]["generated_text"][len(prompt):]
         else:
             texts = [outputs[i][0]['generated_text']
                      [len(prompt[i]):] for i in range(len(outputs))]
 
         if use_cache:
@@ -385,15 +392,15 @@
         max_new_tokens=20,
         do_sample=False,
         use_cache=True,
         verbose=False,
         return_next_token_prob_scores=False,
         target_token_strs: List[str] = None,
         return_top_target_token_str: bool = False,
-        # batch_size=1,
+        batch_size=1,
     ) -> Union[str, List[str]]:
         """Warning: stop is used posthoc but not during generation.
         Be careful, caching can take up a lot of memory....
 
         Example mistral-instruct prompt: "<s>[INST]'Input text: {example}\nQuestion: {question} Answer yes or no.[/INST]"
```

### Comparing `imodelsx-1.0.1/imodelsx/metrics.py` & `imodelsx-1.0.2/imodelsx/metrics.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/imodelsx/process_results.py` & `imodelsx-1.0.2/imodelsx/process_results.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,17 +83,19 @@
     parser = train_script.add_main_args(argparse.ArgumentParser())
     parser = train_script.add_computational_args(parser)
     args = parser.parse_args([])
     args_dict = vars(args)
     for k, v in args_dict.items():
         if k not in df.columns:
             df[k] = v
-        if v is None:
-            v = "None"
-        df[k] = df[k].fillna(v)
+        else:
+            if v is None:
+                df[k] = df[k].fillna(np.nan)
+            else:
+                df[k] = df[k].fillna(v)
     return df
 
 
 def delete_runs_in_dataframe(
     df: pd.DataFrame, actually_delete=False,
     directory_key="save_dir_unique",
     # save_dir_prefix_replace=('/mntv1', '/home/chansingh/mntv1')
```

### Comparing `imodelsx-1.0.1/imodelsx/sasc/api.py` & `imodelsx-1.0.2/imodelsx/sasc/api.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/imodelsx/sasc/m1_ngrams.py` & `imodelsx-1.0.2/imodelsx/sasc/m1_ngrams.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/imodelsx/sasc/m2_summarize.py` & `imodelsx-1.0.2/imodelsx/sasc/m2_summarize.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/imodelsx/sasc/m3_generate.py` & `imodelsx-1.0.2/imodelsx/sasc/m3_generate.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/imodelsx/submit_utils.py` & `imodelsx-1.0.2/imodelsx/submit_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     args_list: List[Dict[str, Any]],
     cmd_python: str = 'python',
     script_name: str = '02_train_suffix.py',
     actually_run: bool = True,
     debug_mode: bool = False,
     shuffle: bool = False,
     reverse: bool = False,
-    unique_seeds: bool = False,
+    unique_seeds: str = None,
     n_cpus: int = 1,
     gpu_ids: Union[List[int], List[List[int]]] = [],
     repeat_failed_jobs: bool = False,
     slurm: bool = False,
     slurm_kwargs: Optional[Dict] = None,
     amlt_kwargs: Optional[Dict] = None,
 ):
@@ -46,16 +46,16 @@
         Whether to actually run the script (otherwise just print the command)
     debug_mode: bool
         Whether to open debugger after failure (stops all parallelilization) 
     shuffle: bool
         Whether to shuffle the order of the script calls
     reverse: bool
         Whether to reverse the order of the script calls
-    unique_seeds: bool
-        Whether to assign random, unique seeds to each run
+    unique_seeds: str
+        Whether to assign random, unique values to each parameter with this value
     n_cpus: int
         Number of cpus to use (if >1, parallelizes over local machine)
     gpu_ids: List[int], List[List[int]]
         Ids of GPUs to run on (e.g. [0, 1] for 2 gpus)
         If List[List[int]], then each inner list is a group of GPUs to run on, e.g. [[0, 1], [2, 3]] for 2 groups of 2 GPUs
     repeat_failed_jobs: bool
         Whether to repeatedly run failed jobs
@@ -85,15 +85,15 @@
             print('\n###\n### Debug mode, setting n_cpus=1 and n_gpus=0 ###\n###\n')
             n_cpus = 1
             n_gpus = 0
 
     # assign unique seeds
     if unique_seeds:
         for i, args in enumerate(args_list):
-            args_list[i]['seed'] = random.randint(1, int(1e6))
+            args_list[i]['seed_stories'] = random.randint(1, int(1e6))
 
     # construct commands
     param_str_list = [_param_str_from_args(
         args, cmd_python, script_name) for args in args_list]
 
     # just print and exit
     if not actually_run:
@@ -137,15 +137,15 @@
   sku: {sku}
   command:
   - {param_str}'''
         out_file = join(logs_dir, sha256({'s': str(param_str_list)}) + '.yaml')
         s = amlt_text
         for i, param_str in enumerate(param_str_list):
             job_text = job_template.format(
-                name=f'job_{i}',
+                name=f'{sku}_job_{i}',
                 process_count_per_node=process_count_per_node,
                 sku=sku,
                 param_str=param_str
             )
             s = s + job_text
         s = s.replace('$CONFIG_DIR', '$CONFIG_DIR/..')
         with open(out_file, 'w') as f:
```

### Comparing `imodelsx-1.0.1/imodelsx/treeprompt/stump.py` & `imodelsx-1.0.2/imodelsx/treeprompt/stump.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/imodelsx/treeprompt/treeprompt.py` & `imodelsx-1.0.2/imodelsx/treeprompt/treeprompt.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/imodelsx/util.py` & `imodelsx-1.0.2/imodelsx/util.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/imodelsx/viz.py` & `imodelsx-1.0.2/imodelsx/viz.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/imodelsx.egg-info/PKG-INFO` & `imodelsx-1.0.2/imodelsx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imodelsx
-Version: 1.0.1
+Version: 1.0.2
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
-Metadata-Version: 2.1 Name: imodelsx Version: 1.0.1 Summary: Library to explain
+Metadata-Version: 2.1 Name: imodelsx Version: 1.0.2 Summary: Library to explain
 a dataset in natural language. Home-page: https://github.com/csinva/imodelsX
 Author: Chandan Singh, John X. Morris, Armin Askari, Divyanshu Aggarwal, Aliyah
 Hsu, Yuntian Deng Author-email: chansingh@microsoft.com Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.9
 Description-Content-Type: text/markdown
   [https://microsoft.github.io/aug-models/embgam_gif.gif][https://csinva.io/
```

### Comparing `imodelsx-1.0.1/imodelsx.egg-info/SOURCES.txt` & `imodelsx-1.0.2/imodelsx.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 setup.py
 imodelsx/__init__.py
 imodelsx/cache_save_utils.py
 imodelsx/data.py
 imodelsx/dummy_script.py
 imodelsx/embeddings.py
+imodelsx/kan.py
 imodelsx/linear_finetune.py
 imodelsx/linear_ngram.py
 imodelsx/llm.py
 imodelsx/metrics.py
 imodelsx/process_results.py
 imodelsx/submit_utils.py
 imodelsx/util.py
```

### Comparing `imodelsx-1.0.1/setup.py` & `imodelsx-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     # 'InstructorEmbedding', # embeddings for emb_diff_module
     # 'sentence-transformers', # embeddings for emb_diff_module
     # pdoc3 # for generating docs
 ]
 
 setuptools.setup(
     name="imodelsx",
-    version="1.0.1",
+    version="1.0.2",
     author="Chandan Singh, John X. Morris, Armin Askari, Divyanshu Aggarwal, Aliyah Hsu, Yuntian Deng",
     author_email="chansingh@microsoft.com",
     description="Library to explain a dataset in natural language.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/csinva/imodelsX",
     packages=setuptools.find_packages(
```

### Comparing `imodelsx-1.0.1/tests/test_auglinear_pipeline.py` & `imodelsx-1.0.2/tests/test_auglinear_pipeline.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/tests/test_augtree.py` & `imodelsx-1.0.2/tests/test_augtree.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/tests/test_iprompt.py` & `imodelsx-1.0.2/tests/test_iprompt.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/tests/test_llm.py` & `imodelsx-1.0.2/tests/test_llm.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/tests/test_ngram_list.py` & `imodelsx-1.0.2/tests/test_ngram_list.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.1/tests/test_sasc.py` & `imodelsx-1.0.2/tests/test_sasc.py`

 * *Files identical despite different names*

