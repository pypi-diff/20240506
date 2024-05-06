# Comparing `tmp/mteb-1.7.9.tar.gz` & `tmp/mteb-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mteb-1.7.9.tar", last modified: Tue Apr 23 07:43:09 2024, max compression
+gzip compressed data, was "mteb-1.8.0.tar", last modified: Sun May  5 20:39:02 2024, max compression
```

## Comparing `mteb-1.7.9.tar` & `mteb-1.8.0.tar`

### file list

```diff
@@ -1,772 +1,1114 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.191770 mteb-1.7.9/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-04-23 07:43:04.000000 mteb-1.7.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)    23583 2024-04-23 07:43:09.187770 mteb-1.7.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9185 2024-04-23 07:43:04.000000 mteb-1.7.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.043770 mteb-1.7.9/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.063770 mteb-1.7.9/docs/mmteb/
--rw-r--r--   0 root         (0) root         (0)     1143 2024-04-23 07:43:04.000000 mteb-1.7.9/docs/mmteb/create_points_table.py
--rw-r--r--   0 root         (0) root         (0)     2108 2024-04-23 07:43:04.000000 mteb-1.7.9/docs/mmteb/validate_points.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.063770 mteb-1.7.9/mteb/
--rw-r--r--   0 root         (0) root         (0)     2273 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.067770 mteb-1.7.9/mteb/abstasks/
--rw-r--r--   0 root         (0) root         (0)     2284 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/abstasks/AbsTask.py
--rw-r--r--   0 root         (0) root         (0)     3058 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/abstasks/AbsTaskBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     5876 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/abstasks/AbsTaskClassification.py
--rw-r--r--   0 root         (0) root         (0)     2384 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/abstasks/AbsTaskClustering.py
--rw-r--r--   0 root         (0) root         (0)    24826 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/abstasks/AbsTaskInstructionRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2537 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/abstasks/AbsTaskPairClassification.py
--rw-r--r--   0 root         (0) root         (0)     1115 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/abstasks/AbsTaskReranking.py
--rw-r--r--   0 root         (0) root         (0)    13352 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/abstasks/AbsTaskRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2002 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/abstasks/AbsTaskSTS.py
--rw-r--r--   0 root         (0) root         (0)     2291 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/abstasks/AbsTaskSummarization.py
--rw-r--r--   0 root         (0) root         (0)      862 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/abstasks/CrosslingualTask.py
--rw-r--r--   0 root         (0) root         (0)     2831 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/abstasks/LangMapping.py
--rw-r--r--   0 root         (0) root         (0)     1013 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/abstasks/MultilingualTask.py
--rw-r--r--   0 root         (0) root         (0)     9810 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/abstasks/TaskMetadata.py
--rw-r--r--   0 root         (0) root         (0)      465 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/abstasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7082 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/abstasks/iso_15924_to_script.json
--rw-r--r--   0 root         (0) root         (0)   193114 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/abstasks/iso_639_3_to_language.json
--rw-r--r--   0 root         (0) root         (0)      541 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/abstasks/languages.py
--rw-r--r--   0 root         (0) root         (0)     5225 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.071770 mteb-1.7.9/mteb/evaluation/
--rw-r--r--   0 root         (0) root         (0)    13004 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/evaluation/MTEB.py
--rw-r--r--   0 root         (0) root         (0)       56 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/evaluation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.071770 mteb-1.7.9/mteb/evaluation/evaluators/
--rw-r--r--   0 root         (0) root         (0)     5840 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/evaluation/evaluators/BitextMiningEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     8927 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/evaluation/evaluators/ClassificationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1463 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/evaluation/evaluators/ClusteringEvaluator.py
--rw-r--r--   0 root         (0) root         (0)      730 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/evaluation/evaluators/Evaluator.py
--rw-r--r--   0 root         (0) root         (0)      789 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/evaluation/evaluators/InstructionRetrievalEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     7126 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/evaluation/evaluators/PairClassificationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     9554 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/evaluation/evaluators/RerankingEvaluator.py
--rw-r--r--   0 root         (0) root         (0)    13983 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/evaluation/evaluators/RetrievalEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     2394 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/evaluation/evaluators/STSEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     4841 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/evaluation/evaluators/SummarizationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)      324 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/evaluation/evaluators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7469 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/evaluation/evaluators/utils.py
--rw-r--r--   0 root         (0) root         (0)      820 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.071770 mteb-1.7.9/mteb/tasks/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.071770 mteb-1.7.9/mteb/tasks/BitextMining/
--rw-r--r--   0 root         (0) root         (0)      567 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/BitextMining/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.071770 mteb-1.7.9/mteb/tasks/BitextMining/dan/
--rw-r--r--   0 root         (0) root         (0)     1443 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/BitextMining/dan/BornholmskBitextMining.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/BitextMining/dan/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.075770 mteb-1.7.9/mteb/tasks/BitextMining/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1199 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     2263 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     5951 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     4585 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/BitextMining/multilingual/IN22ConvBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     3552 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/BitextMining/multilingual/IN22GenBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     1423 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     1830 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/BitextMining/multilingual/RomaTalesBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     5709 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/BitextMining/multilingual/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1363 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/BitextMining/multilingual/norwegian_courts_bitext_mining.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.075770 mteb-1.7.9/mteb/tasks/BitextMining/vie/
--rw-r--r--   0 root         (0) root         (0)     2889 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/BitextMining/vie/VieMedEVBitextMining.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/BitextMining/vie/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.075770 mteb-1.7.9/mteb/tasks/Classification/
--rw-r--r--   0 root         (0) root         (0)     3171 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.075770 mteb-1.7.9/mteb/tasks/Classification/ara/
--rw-r--r--   0 root         (0) root         (0)     1725 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ara/HotelReviewSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)     1852 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ara/RestaurantReviewSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)     1913 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ara/TweetEmotionClassification.py
--rw-r--r--   0 root         (0) root         (0)     3161 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ara/TweetSarcasmClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ara/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.075770 mteb-1.7.9/mteb/tasks/Classification/bam/
--rw-r--r--   0 root         (0) root         (0)     1969 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/bam/BambaraSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/bam/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.075770 mteb-1.7.9/mteb/tasks/Classification/ben/
--rw-r--r--   0 root         (0) root         (0)     1793 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ben/BengaliHateSpeechClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ben/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.079770 mteb-1.7.9/mteb/tasks/Classification/bul/
--rw-r--r--   0 root         (0) root         (0)     2031 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/bul/BulgarianSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)     1947 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/bul/BulgarianStoreReviewSentimentClassfication.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/bul/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.079770 mteb-1.7.9/mteb/tasks/Classification/ces/
--rw-r--r--   0 root         (0) root         (0)     1704 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ces/CzechSubjectivityClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ces/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.079770 mteb-1.7.9/mteb/tasks/Classification/dan/
--rw-r--r--   0 root         (0) root         (0)     1322 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/dan/AngryTweetsClassification.py
--rw-r--r--   0 root         (0) root         (0)     1621 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/dan/DKHateClassification.py
--rw-r--r--   0 root         (0) root         (0)     2502 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/dan/DalajClassification.py
--rw-r--r--   0 root         (0) root         (0)     1616 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/dan/DanishPoliticalCommentsClassification.py
--rw-r--r--   0 root         (0) root         (0)     2943 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/dan/DdiscoCohesionClassification.py
--rw-r--r--   0 root         (0) root         (0)     1261 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/dan/LccSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/dan/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.079770 mteb-1.7.9/mteb/tasks/Classification/ell/
--rw-r--r--   0 root         (0) root         (0)     2172 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ell/GreekLegalCodeClassification.py
--rw-r--r--   0 root         (0) root         (0)     2192 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ell/GreekSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ell/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.083770 mteb-1.7.9/mteb/tasks/Classification/eng/
--rw-r--r--   0 root         (0) root         (0)     1041 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/eng/AmazonPolarityClassification.py
--rw-r--r--   0 root         (0) root         (0)     1054 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/eng/Banking77Classification.py
--rw-r--r--   0 root         (0) root         (0)     1374 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/eng/EmotionClassification.py
--rw-r--r--   0 root         (0) root         (0)      990 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/eng/ImdbClassification.py
--rw-r--r--   0 root         (0) root         (0)     1085 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/eng/NewsClassification.py
--rw-r--r--   0 root         (0) root         (0)     1406 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/eng/ToxicConversationsClassification.py
--rw-r--r--   0 root         (0) root         (0)     1281 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/eng/TweetSentimentExtractionClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.083770 mteb-1.7.9/mteb/tasks/Classification/est/
--rw-r--r--   0 root         (0) root         (0)     2407 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/est/estonian_valence.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.083770 mteb-1.7.9/mteb/tasks/Classification/fas/
--rw-r--r--   0 root         (0) root         (0)     1874 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/fas/PersianFoodSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/fas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.083770 mteb-1.7.9/mteb/tasks/Classification/fil/
--rw-r--r--   0 root         (0) root         (0)     2085 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/fil/FilipinoHateSpeechClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/fil/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.083770 mteb-1.7.9/mteb/tasks/Classification/fra/
--rw-r--r--   0 root         (0) root         (0)     1905 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/fra/MovieReviewSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/fra/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.083770 mteb-1.7.9/mteb/tasks/Classification/guj/
--rw-r--r--   0 root         (0) root         (0)     1285 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/guj/GujaratiNewsClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/guj/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.083770 mteb-1.7.9/mteb/tasks/Classification/hin/
--rw-r--r--   0 root         (0) root         (0)     2195 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/hin/HindiDiscourseClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/hin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.083770 mteb-1.7.9/mteb/tasks/Classification/hrv/
--rw-r--r--   0 root         (0) root         (0)     2028 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/hrv/CroatianSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/hrv/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.083770 mteb-1.7.9/mteb/tasks/Classification/ind/
--rw-r--r--   0 root         (0) root         (0)     2881 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ind/IndonesianIdClickbaitClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ind/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.083770 mteb-1.7.9/mteb/tasks/Classification/ita/
--rw-r--r--   0 root         (0) root         (0)     4105 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ita/ItaHateClassification.py
--rw-r--r--   0 root         (0) root         (0)     2188 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ita/ItalianLinguistAcceptabilityClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ita/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.083770 mteb-1.7.9/mteb/tasks/Classification/jpn/
--rw-r--r--   0 root         (0) root         (0)     3550 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/jpn/WRIMEClassification.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.087770 mteb-1.7.9/mteb/tasks/Classification/kur/
--rw-r--r--   0 root         (0) root         (0)     1544 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/kur/KurdishSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/kur/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.087770 mteb-1.7.9/mteb/tasks/Classification/mkd/
--rw-r--r--   0 root         (0) root         (0)     1768 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/mkd/MacedonianTweetSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/mkd/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.087770 mteb-1.7.9/mteb/tasks/Classification/mlt/
--rw-r--r--   0 root         (0) root         (0)     2023 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/mlt/MalteseSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/mlt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.087770 mteb-1.7.9/mteb/tasks/Classification/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1575 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py
--rw-r--r--   0 root         (0) root         (0)     1377 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py
--rw-r--r--   0 root         (0) root         (0)     3286 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/multilingual/IndicSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)     1275 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py
--rw-r--r--   0 root         (0) root         (0)     1275 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py
--rw-r--r--   0 root         (0) root         (0)     1627 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py
--rw-r--r--   0 root         (0) root         (0)     2537 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py
--rw-r--r--   0 root         (0) root         (0)     2543 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py
--rw-r--r--   0 root         (0) root         (0)     1611 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/multilingual/NordicLangClassification.py
--rw-r--r--   0 root         (0) root         (0)     6099 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/multilingual/ScalaClassification.py
--rw-r--r--   0 root         (0) root         (0)     3358 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/multilingual/ToxicChatClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.087770 mteb-1.7.9/mteb/tasks/Classification/nld/
--rw-r--r--   0 root         (0) root         (0)     1749 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/nld/DutchBookReviewSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/nld/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.091770 mteb-1.7.9/mteb/tasks/Classification/nob/
--rw-r--r--   0 root         (0) root         (0)     1121 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/nob/NoRecClassification.py
--rw-r--r--   0 root         (0) root         (0)     1173 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/nob/NorwegianParliamentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/nob/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.091770 mteb-1.7.9/mteb/tasks/Classification/pol/
--rw-r--r--   0 root         (0) root         (0)     4922 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/pol/PolishClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/pol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.091770 mteb-1.7.9/mteb/tasks/Classification/ron/
--rw-r--r--   0 root         (0) root         (0)     1587 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ron/RomanianSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ron/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.091770 mteb-1.7.9/mteb/tasks/Classification/slk/
--rw-r--r--   0 root         (0) root         (0)     2078 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/slk/SlovakSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/slk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.091770 mteb-1.7.9/mteb/tasks/Classification/ssw/
--rw-r--r--   0 root         (0) root         (0)     1632 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ssw/SiswatiNewsClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/ssw/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.091770 mteb-1.7.9/mteb/tasks/Classification/swe/
--rw-r--r--   0 root         (0) root         (0)     1043 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/swe/SweRecClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/swe/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.091770 mteb-1.7.9/mteb/tasks/Classification/tur/
--rw-r--r--   0 root         (0) root         (0)     1518 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/tur/TurkishMovieSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)     1525 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/tur/TurkishProductSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/tur/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.091770 mteb-1.7.9/mteb/tasks/Classification/uig/
--rw-r--r--   0 root         (0) root         (0)     1966 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/uig/UyghurSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/uig/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.091770 mteb-1.7.9/mteb/tasks/Classification/vie/
--rw-r--r--   0 root         (0) root         (0)     3368 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/vie/VieStudentFeedbackClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/vie/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.095770 mteb-1.7.9/mteb/tasks/Classification/zho/
--rw-r--r--   0 root         (0) root         (0)     6571 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/zho/CMTEBClassification.py
--rw-r--r--   0 root         (0) root         (0)     1729 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/zho/YueOpenriceReviewClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/zho/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.095770 mteb-1.7.9/mteb/tasks/Classification/zul/
--rw-r--r--   0 root         (0) root         (0)     1632 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/zul/IsiZuluNewsClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Classification/zul/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.095770 mteb-1.7.9/mteb/tasks/Clustering/
--rw-r--r--   0 root         (0) root         (0)     1319 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.095770 mteb-1.7.9/mteb/tasks/Clustering/deu/
--rw-r--r--   0 root         (0) root         (0)     1132 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/deu/BlurbsClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1124 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/deu/BlurbsClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1100 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/deu/TenKGnadClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1080 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/deu/TenKGnadClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/deu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.099770 mteb-1.7.9/mteb/tasks/Clustering/eng/
--rw-r--r--   0 root         (0) root         (0)     1101 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/eng/ArxivClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1087 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/eng/ArxivClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1128 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/eng/BigPatentClustering.py
--rw-r--r--   0 root         (0) root         (0)     1071 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/eng/BiorxivClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1061 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/eng/BiorxivClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1072 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/eng/MedrxivClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1062 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/eng/MedrxivClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1102 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/eng/RedditClustering.py
--rw-r--r--   0 root         (0) root         (0)     1091 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/eng/RedditClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1127 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/eng/StackExchangeClustering.py
--rw-r--r--   0 root         (0) root         (0)     1115 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/eng/StackExchangeClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1084 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/eng/TwentyNewsgroupsClustering.py
--rw-r--r--   0 root         (0) root         (0)     1135 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/eng/WikiCitiesClustering.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.099770 mteb-1.7.9/mteb/tasks/Clustering/fra/
--rw-r--r--   0 root         (0) root         (0)     1893 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/fra/AlloProfClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1739 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/fra/AlloProfClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1607 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/fra/HALClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     2406 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/fra/MLSUMClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     2221 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/fra/MLSUMClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/fra/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.099770 mteb-1.7.9/mteb/tasks/Clustering/multilingual/
--rw-r--r--   0 root         (0) root         (0)     2687 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     2701 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1676 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/multilingual/WikiClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.099770 mteb-1.7.9/mteb/tasks/Clustering/nob/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/nob/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3442 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/nob/snl_clustering.py
--rw-r--r--   0 root         (0) root         (0)     3596 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/nob/vg_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.099770 mteb-1.7.9/mteb/tasks/Clustering/pol/
--rw-r--r--   0 root         (0) root         (0)     1137 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/pol/PolishClustering.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/pol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.103770 mteb-1.7.9/mteb/tasks/Clustering/rom/
--rw-r--r--   0 root         (0) root         (0)     1089 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/rom/RomaniBibleClustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.103770 mteb-1.7.9/mteb/tasks/Clustering/spa/
--rw-r--r--   0 root         (0) root         (0)     1042 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/spa/FloresClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1060 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/spa/SpanishNewsClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/spa/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.103770 mteb-1.7.9/mteb/tasks/Clustering/swe/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/swe/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3917 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/swe/swedn_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.103770 mteb-1.7.9/mteb/tasks/Clustering/zho/
--rw-r--r--   0 root         (0) root         (0)     3639 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/zho/CMTEBClustering.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Clustering/zho/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.103770 mteb-1.7.9/mteb/tasks/InstructionRetrieval/
--rw-r--r--   0 root         (0) root         (0)      176 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/InstructionRetrieval/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.103770 mteb-1.7.9/mteb/tasks/InstructionRetrieval/eng/
--rw-r--r--   0 root         (0) root         (0)     1548 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/InstructionRetrieval/eng/Core17InstructionRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1547 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/InstructionRetrieval/eng/News21InstructionRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1555 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/InstructionRetrieval/eng/Robust04InstructionRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/InstructionRetrieval/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.103770 mteb-1.7.9/mteb/tasks/PairClassification/
--rw-r--r--   0 root         (0) root         (0)      344 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/PairClassification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.103770 mteb-1.7.9/mteb/tasks/PairClassification/deu/
--rw-r--r--   0 root         (0) root         (0)     2862 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/PairClassification/deu/FalseFriendsDeEnPC.py
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/PairClassification/deu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.107770 mteb-1.7.9/mteb/tasks/PairClassification/eng/
--rw-r--r--   0 root         (0) root         (0)     1152 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/PairClassification/eng/SprintDuplicateQuestionsPC.py
--rw-r--r--   0 root         (0) root         (0)     1086 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/PairClassification/eng/TwitterSemEval2015PC.py
--rw-r--r--   0 root         (0) root         (0)     1040 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/PairClassification/eng/TwitterURLCorpusPC.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/PairClassification/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.107770 mteb-1.7.9/mteb/tasks/PairClassification/multilingual/
--rw-r--r--   0 root         (0) root         (0)     2780 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py
--rw-r--r--   0 root         (0) root         (0)     1768 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/PairClassification/multilingual/PawsX.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/PairClassification/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.107770 mteb-1.7.9/mteb/tasks/PairClassification/pol/
--rw-r--r--   0 root         (0) root         (0)     3577 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/PairClassification/pol/PolishPC.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/PairClassification/pol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.107770 mteb-1.7.9/mteb/tasks/PairClassification/zho/
--rw-r--r--   0 root         (0) root         (0)     1849 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/PairClassification/zho/CMTEBPairClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/PairClassification/zho/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.107770 mteb-1.7.9/mteb/tasks/Reranking/
--rw-r--r--   0 root         (0) root         (0)      346 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Reranking/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.107770 mteb-1.7.9/mteb/tasks/Reranking/eng/
--rw-r--r--   0 root         (0) root         (0)     1118 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Reranking/eng/AskUbuntuDupQuestions.py
--rw-r--r--   0 root         (0) root         (0)     1103 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Reranking/eng/MindSmallReranking.py
--rw-r--r--   0 root         (0) root         (0)     3054 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Reranking/eng/SciDocsReranking.py
--rw-r--r--   0 root         (0) root         (0)     1137 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Reranking/eng/StackOverflowDupQuestions.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Reranking/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.107770 mteb-1.7.9/mteb/tasks/Reranking/fra/
--rw-r--r--   0 root         (0) root         (0)     1195 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Reranking/fra/AlloprofReranking.py
--rw-r--r--   0 root         (0) root         (0)     1065 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Reranking/fra/SyntecReranking.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Reranking/fra/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.111770 mteb-1.7.9/mteb/tasks/Reranking/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1269 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Reranking/multilingual/MIRACLReranking.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Reranking/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.111770 mteb-1.7.9/mteb/tasks/Reranking/zho/
--rw-r--r--   0 root         (0) root         (0)     3528 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Reranking/zho/CMTEBReranking.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Reranking/zho/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.111770 mteb-1.7.9/mteb/tasks/Retrieval/
--rw-r--r--   0 root         (0) root         (0)     3435 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.111770 mteb-1.7.9/mteb/tasks/Retrieval/code/
--rw-r--r--   0 root         (0) root         (0)     3377 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/code/CodeSearchNetRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/code/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.111770 mteb-1.7.9/mteb/tasks/Retrieval/dan/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/dan/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3785 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/dan/dan_fever.py
--rw-r--r--   0 root         (0) root         (0)     2574 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/dan/t2nord_retrieval.py
--rw-r--r--   0 root         (0) root         (0)     3139 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/dan/twitterhjerne.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.111770 mteb-1.7.9/mteb/tasks/Retrieval/deu/
--rw-r--r--   0 root         (0) root         (0)     2048 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/deu/GerDaLIRRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1228 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/deu/GerDaLIRSmallRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2891 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/deu/GermanDPRRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2127 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/deu/GermanQuADRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1052 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/deu/LegalQuADRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/deu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.119770 mteb-1.7.9/mteb/tasks/Retrieval/eng/
--rw-r--r--   0 root         (0) root         (0)     1118 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/AILACasedocsRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1086 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/AILAStatutesRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1011 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/ArguAnaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1065 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackAndroidRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1065 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackEnglishRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1062 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackGamingRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1053 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackGisRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1077 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackMathematicaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1065 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackPhysicsRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1077 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackProgrammersRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1059 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackStatsRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1053 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackTexRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1056 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackUnixRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1074 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackWebmastersRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1071 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackWordpressRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1095 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/ClimateFEVERRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1031 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/DBPediaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1175 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/FEVERRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      983 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/FiQA2018Retrieval.py
--rw-r--r--   0 root         (0) root         (0)     3668 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/HagridRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1151 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/HotpotQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3022 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/LEMBNarrativeQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3296 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/LEMBNeedleRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3289 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/LEMBPasskeyRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3391 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/LEMBQMSumRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3050 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/LEMBSummScreenFDRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2526 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/LEMBWikimQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1146 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/LegalBenchConsumerContractsQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1150 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/LegalBenchCorporateLobbyingRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1147 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/LegalSummarizationRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1009 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/MSMARCORetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1039 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/MSMARCOv2Retrieval.py
--rw-r--r--   0 root         (0) root         (0)     1650 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/MedicalQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1024 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/NFCorpusRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      999 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/NQRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1991 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/NarrativeQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1155 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/QuoraRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1114 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/SCIDOCSRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1046 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/SciFactRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1069 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/TRECCOVIDRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1009 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/Touche2020Retrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.119770 mteb-1.7.9/mteb/tasks/Retrieval/est/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/est/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1596 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/est/estqa.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.123770 mteb-1.7.9/mteb/tasks/Retrieval/fra/
--rw-r--r--   0 root         (0) root         (0)     2144 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/fra/AlloprofRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2475 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/fra/BSARDRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3184 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/fra/FQuADRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2148 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/fra/SyntecRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/fra/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.123770 mteb-1.7.9/mteb/tasks/Retrieval/hun/
--rw-r--r--   0 root         (0) root         (0)     2589 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/hun/HunSum2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.123770 mteb-1.7.9/mteb/tasks/Retrieval/jpn/
--rw-r--r--   0 root         (0) root         (0)     2853 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/jpn/JaQuADRetrieval.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.123770 mteb-1.7.9/mteb/tasks/Retrieval/kor/
--rw-r--r--   0 root         (0) root         (0)      906 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/kor/KoMiracl.py
--rw-r--r--   0 root         (0) root         (0)      922 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/kor/KoStrategyQA.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/kor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.123770 mteb-1.7.9/mteb/tasks/Retrieval/multilingual/
--rw-r--r--   0 root         (0) root         (0)     3277 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3052 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3432 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3731 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/multilingual/NeuCLIR2022Retrieval.py
--rw-r--r--   0 root         (0) root         (0)     3771 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/multilingual/NeuCLIR2023Retrieval.py
--rw-r--r--   0 root         (0) root         (0)     2979 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3145 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.123770 mteb-1.7.9/mteb/tasks/Retrieval/nob/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/nob/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3943 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/nob/norquad.py
--rw-r--r--   0 root         (0) root         (0)     2699 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/nob/snl_retrieval.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.127770 mteb-1.7.9/mteb/tasks/Retrieval/pol/
--rw-r--r--   0 root         (0) root         (0)      967 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/pol/ArguAnaPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1040 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/pol/DBPediaPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      984 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/pol/FiQAPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1112 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/pol/HotpotQAPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1009 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/pol/MSMARCOPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1040 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/pol/NFCorpusPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      997 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/pol/NQPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1130 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/pol/QuoraPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1091 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/pol/SCIDOCSPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1053 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/pol/SciFactPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1085 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/pol/TRECCOVIDPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/pol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.127770 mteb-1.7.9/mteb/tasks/Retrieval/spa/
--rw-r--r--   0 root         (0) root         (0)     2125 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2P.py
--rw-r--r--   0 root         (0) root         (0)     2056 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/spa/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.127770 mteb-1.7.9/mteb/tasks/Retrieval/swe/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/swe/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3210 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/swe/swedn_retrieval.py
--rw-r--r--   0 root         (0) root         (0)     2610 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/swe/swefaq_retrieval.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.127770 mteb-1.7.9/mteb/tasks/Retrieval/vie/
--rw-r--r--   0 root         (0) root         (0)     3798 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/vie/VieQuADRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/vie/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.127770 mteb-1.7.9/mteb/tasks/Retrieval/zho/
--rw-r--r--   0 root         (0) root         (0)    10384 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/zho/CMTEBRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1121 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/zho/LeCaRDv2Retrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Retrieval/zho/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.131770 mteb-1.7.9/mteb/tasks/STS/
--rw-r--r--   0 root         (0) root         (0)      708 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.131770 mteb-1.7.9/mteb/tasks/STS/deu/
--rw-r--r--   0 root         (0) root         (0)     1370 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/deu/GermanSTSBenchmarkSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/deu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.131770 mteb-1.7.9/mteb/tasks/STS/eng/
--rw-r--r--   0 root         (0) root         (0)     1184 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/eng/BiossesSTS.py
--rw-r--r--   0 root         (0) root         (0)     1153 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/eng/STS12STS.py
--rw-r--r--   0 root         (0) root         (0)     1150 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/eng/STS13STS.py
--rw-r--r--   0 root         (0) root         (0)     1184 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/eng/STS14STS.py
--rw-r--r--   0 root         (0) root         (0)     1148 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/eng/STS15STS.py
--rw-r--r--   0 root         (0) root         (0)     1148 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/eng/STS16STS.py
--rw-r--r--   0 root         (0) root         (0)     1208 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/eng/STSBenchmarkSTS.py
--rw-r--r--   0 root         (0) root         (0)     1185 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/eng/SickrSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.131770 mteb-1.7.9/mteb/tasks/STS/fin/
--rw-r--r--   0 root         (0) root         (0)     3422 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/fin/FinParaSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/fin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.131770 mteb-1.7.9/mteb/tasks/STS/fra/
--rw-r--r--   0 root         (0) root         (0)     1472 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/fra/SickFrSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/fra/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.131770 mteb-1.7.9/mteb/tasks/STS/jpn/
--rw-r--r--   0 root         (0) root         (0)     3034 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/jpn/JSTS.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.131770 mteb-1.7.9/mteb/tasks/STS/kor/
--rw-r--r--   0 root         (0) root         (0)     2504 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/kor/KlueSTS.py
--rw-r--r--   0 root         (0) root         (0)     1634 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/kor/KorSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/kor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.135770 mteb-1.7.9/mteb/tasks/STS/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1600 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py
--rw-r--r--   0 root         (0) root         (0)     1832 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py
--rw-r--r--   0 root         (0) root         (0)     2712 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.135770 mteb-1.7.9/mteb/tasks/STS/pol/
--rw-r--r--   0 root         (0) root         (0)     2268 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/pol/PolishSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/pol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.135770 mteb-1.7.9/mteb/tasks/STS/ron/
--rw-r--r--   0 root         (0) root         (0)     1896 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/ron/RonSTS.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.135770 mteb-1.7.9/mteb/tasks/STS/spa/
--rw-r--r--   0 root         (0) root         (0)     1486 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/spa/STSES.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/spa/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.135770 mteb-1.7.9/mteb/tasks/STS/zho/
--rw-r--r--   0 root         (0) root         (0)     7122 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/zho/CMTEBSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/STS/zho/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.135770 mteb-1.7.9/mteb/tasks/Summarization/
--rw-r--r--   0 root         (0) root         (0)      124 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Summarization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.135770 mteb-1.7.9/mteb/tasks/Summarization/eng/
--rw-r--r--   0 root         (0) root         (0)     1243 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Summarization/eng/SummEvalSummarization.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Summarization/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.135770 mteb-1.7.9/mteb/tasks/Summarization/fra/
--rw-r--r--   0 root         (0) root         (0)     1304 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Summarization/fra/SummEvalFrSummarization.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/Summarization/fra/__init__.py
--rw-r--r--   0 root         (0) root         (0)      288 2024-04-23 07:43:04.000000 mteb-1.7.9/mteb/tasks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.187770 mteb-1.7.9/mteb.egg-info/
--rw-r--r--   0 root         (0) root         (0)    23583 2024-04-23 07:43:08.000000 mteb-1.7.9/mteb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    36394 2024-04-23 07:43:09.000000 mteb-1.7.9/mteb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 07:43:08.000000 mteb-1.7.9/mteb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2024-04-23 07:43:08.000000 mteb-1.7.9/mteb.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      241 2024-04-23 07:43:08.000000 mteb-1.7.9/mteb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-04-23 07:43:08.000000 mteb-1.7.9/mteb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2728 2024-04-23 07:43:05.000000 mteb-1.7.9/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.059770 mteb-1.7.9/results/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.135770 mteb-1.7.9/results/GritLM__GritLM-7B/
--rw-r--r--   0 root         (0) root         (0)     2342 2024-04-23 07:43:04.000000 mteb-1.7.9/results/GritLM__GritLM-7B/Core17InstructionRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     2381 2024-04-23 07:43:04.000000 mteb-1.7.9/results/GritLM__GritLM-7B/News21InstructionRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     2384 2024-04-23 07:43:04.000000 mteb-1.7.9/results/GritLM__GritLM-7B/Robust04InstructionRetrieval.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.059770 mteb-1.7.9/results/dangvantuan/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.143770 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/
--rw-r--r--   0 root         (0) root         (0)      308 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/AlloProfClusteringP2P.json
--rw-r--r--   0 root         (0) root         (0)      308 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/AlloProfClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)      250 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/AlloprofReranking.json
--rw-r--r--   0 root         (0) root         (0)     1165 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/AlloprofRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      634 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/AmazonReviewsClassification.json
--rw-r--r--   0 root         (0) root         (0)     1042 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/BSARDRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      305 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/HALClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)      308 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/MLSUMClusteringP2P.json
--rw-r--r--   0 root         (0) root         (0)      305 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/MLSUMClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)      675 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/MTOPDomainClassification.json
--rw-r--r--   0 root         (0) root         (0)      676 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/MTOPIntentClassification.json
--rw-r--r--   0 root         (0) root         (0)      411 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/MasakhaNEWSClassification.json
--rw-r--r--   0 root         (0) root         (0)      332 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/MasakhaNEWSClusteringP2P.json
--rw-r--r--   0 root         (0) root         (0)      335 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/MasakhaNEWSClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)      679 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/MassiveIntentClassification.json
--rw-r--r--   0 root         (0) root         (0)      679 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/MassiveScenarioClassification.json
--rw-r--r--   0 root         (0) root         (0)     1242 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/MintakaRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     2992 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/OpusparcusPC.json
--rw-r--r--   0 root         (0) root         (0)     2801 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/PawsX.json
--rw-r--r--   0 root         (0) root         (0)      820 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/SICKFr.json
--rw-r--r--   0 root         (0) root         (0)      511 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/STS22.json
--rw-r--r--   0 root         (0) root         (0)      921 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/STSBenchmarkMultilingualSTS.json
--rw-r--r--   0 root         (0) root         (0)      371 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/SummEvalFr.json
--rw-r--r--   0 root         (0) root         (0)      221 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/SyntecReranking.json
--rw-r--r--   0 root         (0) root         (0)     1099 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/SyntecRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1245 2024-04-23 07:43:04.000000 mteb-1.7.9/results/dangvantuan/sentence-camembert-base/XPQARetrieval.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.059770 mteb-1.7.9/results/intfloat/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.143770 mteb-1.7.9/results/intfloat/multilingual-e5-small/
--rw-r--r--   0 root         (0) root         (0)      384 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat/multilingual-e5-small/BengaliHateSpeechClassification.json
--rw-r--r--   0 root         (0) root         (0)      378 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat/multilingual-e5-small/GujaratiNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      448 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat/multilingual-e5-small/IndonesianIdClickbaitClassification.json
--rw-r--r--   0 root         (0) root         (0)      453 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat/multilingual-e5-small/SlovakSentimentClassification.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.143770 mteb-1.7.9/results/intfloat__e5-small/
--rw-r--r--   0 root         (0) root         (0)      439 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__e5-small/TurkishProductSentimentClassification.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.143770 mteb-1.7.9/results/intfloat__e5-small-v2/
--rw-r--r--   0 root         (0) root         (0)     2512 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__e5-small-v2/Core17InstructionRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     2540 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__e5-small-v2/News21InstructionRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     2550 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__e5-small-v2/Robust04InstructionRetrieval.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.147770 mteb-1.7.9/results/intfloat__multilingual-e5-base/
--rw-r--r--   0 root         (0) root         (0)      758 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-base/CroatianSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      733 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-base/CzechSubjectivityClassification.json
--rw-r--r--   0 root         (0) root         (0)      464 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-base/DutchBookReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      382 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-base/HotelReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      384 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-base/IsiZuluNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      757 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-base/MalteseSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      453 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-base/RestaurantReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      447 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-base/RomanianSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      356 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-base/SiswatiNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      376 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-base/TweetEmotionClassification.json
--rw-r--r--   0 root         (0) root         (0)      452 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-base/TweetSarcasmClassification.json
--rw-r--r--   0 root         (0) root         (0)      452 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-base/UyghurSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)       65 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-base/model_meta.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.159770 mteb-1.7.9/results/intfloat__multilingual-e5-small/
--rw-r--r--   0 root         (0) root         (0)      451 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/BambaraSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      760 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/BulgarianSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      397 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/BulgarianStoreReviewSentimentClassfication.json
--rw-r--r--   0 root         (0) root         (0)     5524 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/CodeSearchNetRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      760 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/CroatianSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      738 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/CzechSubjectivityClassification.json
--rw-r--r--   0 root         (0) root         (0)     1016 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/DanFEVER.json
--rw-r--r--   0 root         (0) root         (0)      463 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/DutchBookReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1125 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/EstQA.json
--rw-r--r--   0 root         (0) root         (0)      387 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/EstonianValenceClassification.json
--rw-r--r--   0 root         (0) root         (0)     2105 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/FQuADRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      742 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/FilipinoHateSpeechClassification.json
--rw-r--r--   0 root         (0) root         (0)      827 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/FinParaSTS.json
--rw-r--r--   0 root         (0) root         (0)     1150 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/GermanDPR.json
--rw-r--r--   0 root         (0) root         (0)      606 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/GreekLegalCodeClassification.json
--rw-r--r--   0 root         (0) root         (0)      761 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/GreekSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      380 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/HotelReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1034 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/HunSum2AbstractiveRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1289 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/IN22ConvBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      604 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/IN22GenBitextMining.json
--rw-r--r--   0 root         (0) root         (0)     3924 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/IndicSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      384 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/IsiZuluNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      445 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/ItaHateClassification.json
--rw-r--r--   0 root         (0) root         (0)      431 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/Itacola.json
--rw-r--r--   0 root         (0) root         (0)      475 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/JSTS.json
--rw-r--r--   0 root         (0) root         (0)     1027 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/JaQuADRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      479 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/KLUE-STS.json
--rw-r--r--   0 root         (0) root         (0)      469 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/KorSTS.json
--rw-r--r--   0 root         (0) root         (0)      452 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/KurdishSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1163 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/LEMBNarrativeQARetrieval.json
--rw-r--r--   0 root         (0) root         (0)     7814 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/LEMBNeedleRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     7703 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/LEMBPasskeyRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1153 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/LEMBQMSumRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1169 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/LEMBSummScreenFDRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1149 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/LEMBWikimQARetrieval.json
--rw-r--r--   0 root         (0) root         (0)      394 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/MacedonianTweetSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      760 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/MalteseSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1025 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/MedicalQARetrieval.json
--rw-r--r--   0 root         (0) root         (0)      745 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/MovieReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     3386 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/NeuCLIR2022Retrieval.json
--rw-r--r--   0 root         (0) root         (0)     3392 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/NeuCLIR2023Retrieval.json
--rw-r--r--   0 root         (0) root         (0)      371 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/NewsClassification.json
--rw-r--r--   0 root         (0) root         (0)     1021 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/NorQuadRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      374 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/NorwegianCourtsBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      744 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/PersianFoodSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      454 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/RestaurantReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      403 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/RomaTalesBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      306 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/RomaniBibleClustering.json
--rw-r--r--   0 root         (0) root         (0)      447 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/RomanianSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      472 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/RonSTS.json
--rw-r--r--   0 root         (0) root         (0)      298 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/SNLClustering.json
--rw-r--r--   0 root         (0) root         (0)     1023 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/SNLRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      384 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/SiswatiNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)     1015 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/SweFaqRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      304 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/SwednClustering.json
--rw-r--r--   0 root         (0) root         (0)     1023 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/SwednRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1116 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/SyntecRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1021 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/TV2Nordretrieval.json
--rw-r--r--   0 root         (0) root         (0)      445 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/ToxicChatClassification.json
--rw-r--r--   0 root         (0) root         (0)      459 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/TurkishMovieSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      372 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/TweetEmotionClassification.json
--rw-r--r--   0 root         (0) root         (0)      451 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/TweetSarcasmClassification.json
--rw-r--r--   0 root         (0) root         (0)     1034 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/TwitterHjerneRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      451 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/UyghurSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      303 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/VGClustering.json
--rw-r--r--   0 root         (0) root         (0)      351 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/VieMedEVBitextMining.json
--rw-r--r--   0 root         (0) root         (0)     1028 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/VieQuADRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      377 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/VieStudentFeedbackClassification.json
--rw-r--r--   0 root         (0) root         (0)      364 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/WRIMEClassification.json
--rw-r--r--   0 root         (0) root         (0)     2184 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/WikiClusteringP2P.json
--rw-r--r--   0 root         (0) root         (0)      387 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/YueOpenriceReviewClassification.json
--rw-r--r--   0 root         (0) root         (0)       66 2024-04-23 07:43:04.000000 mteb-1.7.9/results/intfloat__multilingual-e5-small/model_meta.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.159770 mteb-1.7.9/results/sentence-transformers/
--rw-r--r--   0 root         (0) root         (0)      446 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers/ToxicChatClassification.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.163770 mteb-1.7.9/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/
--rw-r--r--   0 root         (0) root         (0)      380 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/BengaliHateSpeechClassification.json
--rw-r--r--   0 root         (0) root         (0)      381 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/GujaratiNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      452 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/IndonesianIdClickbaitClassification.json
--rw-r--r--   0 root         (0) root         (0)      452 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/SlovakSentimentClassification.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.163770 mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/
--rw-r--r--   0 root         (0) root         (0)      385 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/Banking77Classification.json
--rw-r--r--   0 root         (0) root         (0)      340 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/BornholmBitextMining.json
--rw-r--r--   0 root         (0) root         (0)     1020 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/DanFEVER.json
--rw-r--r--   0 root         (0) root         (0)     1027 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/NorQuadRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      374 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/NorwegianCourtsBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      303 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/SNLClustering.json
--rw-r--r--   0 root         (0) root         (0)     1021 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/SNLRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1014 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/SweFaqRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      306 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/SwednClustering.json
--rw-r--r--   0 root         (0) root         (0)     1025 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/SwednRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1021 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/TV2Nordretrieval.json
--rw-r--r--   0 root         (0) root         (0)     1034 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/TwitterHjerneRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      302 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/VGClustering.json
--rw-r--r--   0 root         (0) root         (0)      194 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/model.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.179770 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/
--rw-r--r--   0 root         (0) root         (0)     1001 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BUCC.json
--rw-r--r--   0 root         (0) root         (0)      454 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BambaraSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      344 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BornholmBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      762 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BulgarianSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      398 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BulgarianStoreReviewSentimentClassfication.json
--rw-r--r--   0 root         (0) root         (0)     5535 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CodeSearchNetRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      759 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CroatianSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      758 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CzechSubjectivityClassification.json
--rw-r--r--   0 root         (0) root         (0)     1020 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DanFEVER.json
--rw-r--r--   0 root         (0) root         (0)      603 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DiaBlaBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      464 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DutchBookReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1139 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/EstQA.json
--rw-r--r--   0 root         (0) root         (0)      385 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/EstonianValenceClassification.json
--rw-r--r--   0 root         (0) root         (0)     2108 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FQuADRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      746 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FilipinoHateSpeechClassification.json
--rw-r--r--   0 root         (0) root         (0)      835 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FinParaSTS.json
--rw-r--r--   0 root         (0) root         (0)      291 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FloresClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)     1020 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GerDaLIR.json
--rw-r--r--   0 root         (0) root         (0)      610 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GreekLegalCodeClassification.json
--rw-r--r--   0 root         (0) root         (0)      758 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GreekSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      380 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HotelReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1032 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HunSum2AbstractiveRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1317 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IN22ConvBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      605 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IN22GenBitextMining.json
--rw-r--r--   0 root         (0) root         (0)     3921 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      385 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IsiZuluNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      442 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ItaHateClassification.json
--rw-r--r--   0 root         (0) root         (0)      430 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Itacola.json
--rw-r--r--   0 root         (0) root         (0)      475 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JSTS.json
--rw-r--r--   0 root         (0) root         (0)     1025 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JaQuADRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      479 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/KLUE-STS.json
--rw-r--r--   0 root         (0) root         (0)      470 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/KorSTS.json
--rw-r--r--   0 root         (0) root         (0)      452 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/KurdishSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1167 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBNarrativeQARetrieval.json
--rw-r--r--   0 root         (0) root         (0)     7839 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBNeedleRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     7915 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBPasskeyRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1153 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBQMSumRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1153 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBSummScreenFDRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1152 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBWikimQARetrieval.json
--rw-r--r--   0 root         (0) root         (0)      394 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MacedonianTweetSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      756 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MalteseSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1021 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MedicalQARetrieval.json
--rw-r--r--   0 root         (0) root         (0)      736 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MovieReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     3382 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NeuCLIR2022Retrieval.json
--rw-r--r--   0 root         (0) root         (0)     3376 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NeuCLIR2023Retrieval.json
--rw-r--r--   0 root         (0) root         (0)      370 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NewsClassification.json
--rw-r--r--   0 root         (0) root         (0)     1027 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NorQuadRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      374 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NorwegianCourtsBitextMining.json
--rw-r--r--   0 root         (0) root         (0)    16669 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/OpusparcusPC.json
--rw-r--r--   0 root         (0) root         (0)    18247 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PawsX.json
--rw-r--r--   0 root         (0) root         (0)      741 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PersianFoodSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      455 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RestaurantReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      404 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RomaTalesBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      308 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RomaniBibleClustering.json
--rw-r--r--   0 root         (0) root         (0)      442 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RomanianSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      471 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RonSTS.json
--rw-r--r--   0 root         (0) root         (0)      300 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SNLClustering.json
--rw-r--r--   0 root         (0) root         (0)     1011 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SNLRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      380 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SiswatiNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)     1021 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SweFaqRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      303 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednClustering.json
--rw-r--r--   0 root         (0) root         (0)     1022 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1027 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TV2Nordretrieval.json
--rw-r--r--   0 root         (0) root         (0)      460 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TurkishMovieSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      440 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TurkishProductSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      376 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TweetEmotionClassification.json
--rw-r--r--   0 root         (0) root         (0)      450 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TweetSarcasmClassification.json
--rw-r--r--   0 root         (0) root         (0)     1035 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TwitterHjerneRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      453 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/UyghurSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      300 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VGClustering.json
--rw-r--r--   0 root         (0) root         (0)      351 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieMedEVBitextMining.json
--rw-r--r--   0 root         (0) root         (0)     1029 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieQuADRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      376 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieStudentFeedbackClassification.json
--rw-r--r--   0 root         (0) root         (0)      366 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WRIMEClassification.json
--rw-r--r--   0 root         (0) root         (0)      294 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WikiCitiesClustering.json
--rw-r--r--   0 root         (0) root         (0)     2186 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WikiClusteringP2P.json
--rw-r--r--   0 root         (0) root         (0)      387 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/YueOpenriceReviewClassification.json
--rw-r--r--   0 root         (0) root         (0)      176 2024-04-23 07:43:04.000000 mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/model_meta.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.183770 mteb-1.7.9/scripts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.183770 mteb-1.7.9/scripts/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.183770 mteb-1.7.9/scripts/data/amazon_polarity/
--rw-r--r--   0 root         (0) root         (0)      842 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/amazon_polarity/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.183770 mteb-1.7.9/scripts/data/amazon_reviews_multi/
--rw-r--r--   0 root         (0) root         (0)     1379 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/amazon_reviews_multi/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.183770 mteb-1.7.9/scripts/data/arxiv/
--rw-r--r--   0 root         (0) root         (0)     3146 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/arxiv/script_clustering.py
--rw-r--r--   0 root         (0) root         (0)     1450 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/arxiv/script_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.183770 mteb-1.7.9/scripts/data/biorxiv/
--rw-r--r--   0 root         (0) root         (0)     1781 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/biorxiv/script_clustering.py
--rw-r--r--   0 root         (0) root         (0)     1672 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/biorxiv/script_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.183770 mteb-1.7.9/scripts/data/bucc/
--rw-r--r--   0 root         (0) root         (0)     1171 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/bucc/create_data.py
--rw-r--r--   0 root         (0) root         (0)     5924 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/create_task_table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.183770 mteb-1.7.9/scripts/data/germanquad/
--rw-r--r--   0 root         (0) root         (0)     2133 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/germanquad/process_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.183770 mteb-1.7.9/scripts/data/hal/
--rw-r--r--   0 root         (0) root         (0)     1512 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/hal/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.183770 mteb-1.7.9/scripts/data/imdb/
--rw-r--r--   0 root         (0) root         (0)      682 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/imdb/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.183770 mteb-1.7.9/scripts/data/medicalqaretrieval/
--rw-r--r--   0 root         (0) root         (0)     1884 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/medicalqaretrieval/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.183770 mteb-1.7.9/scripts/data/medrxiv/
--rw-r--r--   0 root         (0) root         (0)     1780 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/medrxiv/script_clustering.py
--rw-r--r--   0 root         (0) root         (0)     1615 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/medrxiv/script_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.183770 mteb-1.7.9/scripts/data/mind/
--rw-r--r--   0 root         (0) root         (0)     1377 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/mind/prepare_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.183770 mteb-1.7.9/scripts/data/redditp2p/
--rw-r--r--   0 root         (0) root         (0)     1880 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/redditp2p/script_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.183770 mteb-1.7.9/scripts/data/stackexchangep2p/
--rw-r--r--   0 root         (0) root         (0)     1627 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/stackexchangep2p/script_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.187770 mteb-1.7.9/scripts/data/sts22-crosslingual-sts/
--rw-r--r--   0 root         (0) root         (0)     2435 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/sts22-crosslingual-sts/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.187770 mteb-1.7.9/scripts/data/summeval_fr/
--rw-r--r--   0 root         (0) root         (0)     1692 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/summeval_fr/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.187770 mteb-1.7.9/scripts/data/toxic_conversations_50k/
--rw-r--r--   0 root         (0) root         (0)     1151 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/data/toxic_conversations_50k/create_data.py
--rw-r--r--   0 root         (0) root         (0)     2515 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/merge_cqadupstack.py
--rw-r--r--   0 root         (0) root         (0)     5216 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/mteb_meta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.063770 mteb-1.7.9/scripts/results/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.187770 mteb-1.7.9/scripts/results/intfloat__multilingual-e5-small/
--rw-r--r--   0 root         (0) root         (0)      376 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/results/intfloat__multilingual-e5-small/HindiDiscourseClassification.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.187770 mteb-1.7.9/scripts/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/
--rw-r--r--   0 root         (0) root         (0)      376 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HindiDiscourseClassification.json
--rw-r--r--   0 root         (0) root         (0)      673 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/run_mteb_chinese.py
--rw-r--r--   0 root         (0) root         (0)     2819 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/run_mteb_english.py
--rw-r--r--   0 root         (0) root         (0)     1689 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/run_mteb_french.py
--rw-r--r--   0 root         (0) root         (0)     1334 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/run_mteb_german.py
--rw-r--r--   0 root         (0) root         (0)     1008 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/run_mteb_korean.py
--rw-r--r--   0 root         (0) root         (0)      876 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/run_mteb_law.py
--rw-r--r--   0 root         (0) root         (0)      975 2024-04-23 07:43:04.000000 mteb-1.7.9/scripts/run_mteb_polish.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 07:43:09.191770 mteb-1.7.9/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:43:09.187770 mteb-1.7.9/tests/
--rw-r--r--   0 root         (0) root         (0)      632 2024-04-23 07:43:04.000000 mteb-1.7.9/tests/test_ClusteringEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1418 2024-04-23 07:43:04.000000 mteb-1.7.9/tests/test_InstructionRetrievalEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1560 2024-04-23 07:43:04.000000 mteb-1.7.9/tests/test_PairClassificationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1129 2024-04-23 07:43:04.000000 mteb-1.7.9/tests/test_RerankingEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1112 2024-04-23 07:43:04.000000 mteb-1.7.9/tests/test_RetrievalEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     3715 2024-04-23 07:43:04.000000 mteb-1.7.9/tests/test_TaskMetadata.py
--rw-r--r--   0 root         (0) root         (0)     2404 2024-04-23 07:43:04.000000 mteb-1.7.9/tests/test_all_abstasks.py
--rw-r--r--   0 root         (0) root         (0)     1390 2024-04-23 07:43:04.000000 mteb-1.7.9/tests/test_mteb.py
--rw-r--r--   0 root         (0) root         (0)      278 2024-04-23 07:43:04.000000 mteb-1.7.9/tests/test_retrieval_abstask.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.767204 mteb-1.8.0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-05-05 20:38:58.000000 mteb-1.8.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    24072 2024-05-05 20:39:02.767204 mteb-1.8.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9642 2024-05-05 20:38:58.000000 mteb-1.8.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.571203 mteb-1.8.0/docs/
+-rw-r--r--   0 root         (0) root         (0)     2651 2024-05-05 20:38:58.000000 mteb-1.8.0/docs/create_tasks_table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.575203 mteb-1.8.0/docs/mmteb/
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-05-05 20:38:58.000000 mteb-1.8.0/docs/mmteb/create_points_table.py
+-rw-r--r--   0 root         (0) root         (0)     2108 2024-05-05 20:38:58.000000 mteb-1.8.0/docs/mmteb/validate_points.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.575203 mteb-1.8.0/mteb/
+-rw-r--r--   0 root         (0) root         (0)      443 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.579203 mteb-1.8.0/mteb/abstasks/
+-rw-r--r--   0 root         (0) root         (0)     6404 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/abstasks/AbsTask.py
+-rw-r--r--   0 root         (0) root         (0)     3058 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/abstasks/AbsTaskBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     5876 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/abstasks/AbsTaskClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2410 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/abstasks/AbsTaskClustering.py
+-rw-r--r--   0 root         (0) root         (0)     7433 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/abstasks/AbsTaskClusteringFast.py
+-rw-r--r--   0 root         (0) root         (0)    24968 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/abstasks/AbsTaskInstructionRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2537 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/abstasks/AbsTaskPairClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1115 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/abstasks/AbsTaskReranking.py
+-rw-r--r--   0 root         (0) root         (0)    13422 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/abstasks/AbsTaskRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2002 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/abstasks/AbsTaskSTS.py
+-rw-r--r--   0 root         (0) root         (0)     2291 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/abstasks/AbsTaskSummarization.py
+-rw-r--r--   0 root         (0) root         (0)      562 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/abstasks/CrosslingualTask.py
+-rw-r--r--   0 root         (0) root         (0)     2831 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/abstasks/LangMapping.py
+-rw-r--r--   0 root         (0) root         (0)     1897 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/abstasks/MultiSubsetLoader.py
+-rw-r--r--   0 root         (0) root         (0)      653 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/abstasks/MultilingualTask.py
+-rw-r--r--   0 root         (0) root         (0)    10326 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/abstasks/TaskMetadata.py
+-rw-r--r--   0 root         (0) root         (0)      465 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/abstasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7082 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/abstasks/iso_15924_to_script.json
+-rw-r--r--   0 root         (0) root         (0)   193114 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/abstasks/iso_639_3_to_language.json
+-rw-r--r--   0 root         (0) root         (0)      541 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/abstasks/languages.py
+-rw-r--r--   0 root         (0) root         (0)     2101 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/benchmarks.py
+-rw-r--r--   0 root         (0) root         (0)     5225 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/cmd.py
+-rw-r--r--   0 root         (0) root         (0)     1702 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/encoder_interface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.579203 mteb-1.8.0/mteb/evaluation/
+-rw-r--r--   0 root         (0) root         (0)    13258 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/evaluation/MTEB.py
+-rw-r--r--   0 root         (0) root         (0)       56 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/evaluation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.583203 mteb-1.8.0/mteb/evaluation/evaluators/
+-rw-r--r--   0 root         (0) root         (0)     5840 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/evaluation/evaluators/BitextMiningEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     8927 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/evaluation/evaluators/ClassificationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1463 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/evaluation/evaluators/ClusteringEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)      730 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/evaluation/evaluators/Evaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/evaluation/evaluators/InstructionRetrievalEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     7126 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/evaluation/evaluators/PairClassificationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     9554 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/evaluation/evaluators/RerankingEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)    19805 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/evaluation/evaluators/RetrievalEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     2394 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/evaluation/evaluators/STSEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     4841 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/evaluation/evaluators/SummarizationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)      324 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/evaluation/evaluators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7965 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/evaluation/evaluators/utils.py
+-rw-r--r--   0 root         (0) root         (0)      820 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/logging.py
+-rw-r--r--   0 root         (0) root         (0)     6530 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/overview.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.583203 mteb-1.8.0/mteb/tasks/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.583203 mteb-1.8.0/mteb/tasks/BitextMining/
+-rw-r--r--   0 root         (0) root         (0)      750 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/BitextMining/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.583203 mteb-1.8.0/mteb/tasks/BitextMining/dan/
+-rw-r--r--   0 root         (0) root         (0)     2246 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/BitextMining/dan/BornholmskBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/BitextMining/dan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.583203 mteb-1.8.0/mteb/tasks/BitextMining/kat/
+-rw-r--r--   0 root         (0) root         (0)     2147 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/BitextMining/kat/TbilisiCityHallBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/BitextMining/kat/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.587203 mteb-1.8.0/mteb/tasks/BitextMining/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1199 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)    29308 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/BitextMining/multilingual/BibleNLPBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     2263 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     5951 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     4585 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/BitextMining/multilingual/IN22ConvBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     3552 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/BitextMining/multilingual/IN22GenBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)    13482 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/BitextMining/multilingual/NTREXBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     1423 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     1830 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/BitextMining/multilingual/RomaTalesBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     5733 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/BitextMining/multilingual/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1363 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/BitextMining/multilingual/norwegian_courts_bitext_mining.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.587203 mteb-1.8.0/mteb/tasks/BitextMining/srn/
+-rw-r--r--   0 root         (0) root         (0)     2610 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/BitextMining/srn/SRNCorpusBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/BitextMining/srn/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.587203 mteb-1.8.0/mteb/tasks/BitextMining/vie/
+-rw-r--r--   0 root         (0) root         (0)     2889 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/BitextMining/vie/VieMedEVBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/BitextMining/vie/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.587203 mteb-1.8.0/mteb/tasks/Classification/
+-rw-r--r--   0 root         (0) root         (0)     4775 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.591203 mteb-1.8.0/mteb/tasks/Classification/ara/
+-rw-r--r--   0 root         (0) root         (0)     1598 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/ara/AJGT.py
+-rw-r--r--   0 root         (0) root         (0)     1719 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/ara/HotelReviewSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/ara/RestaurantReviewSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1907 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/ara/TweetEmotionClassification.py
+-rw-r--r--   0 root         (0) root         (0)     3161 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/ara/TweetSarcasmClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/ara/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.591203 mteb-1.8.0/mteb/tasks/Classification/ben/
+-rw-r--r--   0 root         (0) root         (0)     1840 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/ben/BengaliHateSpeechClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/ben/BengaliSentimentAnalysis.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/ben/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.591203 mteb-1.8.0/mteb/tasks/Classification/bul/
+-rw-r--r--   0 root         (0) root         (0)     1947 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/bul/BulgarianStoreReviewSentimentClassfication.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/bul/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.591203 mteb-1.8.0/mteb/tasks/Classification/ces/
+-rw-r--r--   0 root         (0) root         (0)     1704 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/ces/CzechSubjectivityClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/ces/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.591203 mteb-1.8.0/mteb/tasks/Classification/dan/
+-rw-r--r--   0 root         (0) root         (0)     1750 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/dan/AngryTweetsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     4348 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/dan/DKHateClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1616 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/dan/DanishPoliticalCommentsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2943 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/dan/DdiscoCohesionClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2435 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/dan/LccSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/dan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.591203 mteb-1.8.0/mteb/tasks/Classification/deu/
+-rw-r--r--   0 root         (0) root         (0)     2374 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/deu/GermanPoliticiansTwitterSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/deu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.591203 mteb-1.8.0/mteb/tasks/Classification/ell/
+-rw-r--r--   0 root         (0) root         (0)     2172 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/ell/GreekLegalCodeClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/ell/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.595203 mteb-1.8.0/mteb/tasks/Classification/eng/
+-rw-r--r--   0 root         (0) root         (0)     1041 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/eng/AmazonPolarityClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1468 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/eng/ArxivClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1054 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/eng/Banking77Classification.py
+-rw-r--r--   0 root         (0) root         (0)     2072 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/eng/DBpediaClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1374 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/eng/EmotionClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1735 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/eng/FinancialPhrasebankClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1447 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/eng/FrenkEnClassification.py
+-rw-r--r--   0 root         (0) root         (0)      990 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/eng/ImdbClassification.py
+-rw-r--r--   0 root         (0) root         (0)   127090 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/eng/LegalBenchClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1085 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/eng/NewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     3186 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/eng/PatentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2842 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/eng/ToxicChatClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1560 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/eng/ToxicConversationsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1281 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/eng/TweetSentimentExtractionClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2290 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/eng/TweetTopicSingleClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1806 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/eng/YahooAnswersTopicsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2151 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/eng/YelpReviewFullClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.595203 mteb-1.8.0/mteb/tasks/Classification/est/
+-rw-r--r--   0 root         (0) root         (0)     2407 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/est/estonian_valence.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.599203 mteb-1.8.0/mteb/tasks/Classification/fas/
+-rw-r--r--   0 root         (0) root         (0)     1714 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/fas/PersianFoodSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/fas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.599203 mteb-1.8.0/mteb/tasks/Classification/fil/
+-rw-r--r--   0 root         (0) root         (0)     1925 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/fil/FilipinoHateSpeechClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2040 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/fil/FilipinoShopeeReviewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/fil/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.599203 mteb-1.8.0/mteb/tasks/Classification/fin/
+-rw-r--r--   0 root         (0) root         (0)     2562 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/fin/FinToxicityClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/fin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.599203 mteb-1.8.0/mteb/tasks/Classification/fra/
+-rw-r--r--   0 root         (0) root         (0)     1777 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/fra/MovieReviewSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/fra/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.599203 mteb-1.8.0/mteb/tasks/Classification/guj/
+-rw-r--r--   0 root         (0) root         (0)     1285 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/guj/GujaratiNewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/guj/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.599203 mteb-1.8.0/mteb/tasks/Classification/hin/
+-rw-r--r--   0 root         (0) root         (0)     2242 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/hin/HindiDiscourseClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1755 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/hin/SentimentAnalysisHindi.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/hin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.599203 mteb-1.8.0/mteb/tasks/Classification/hrv/
+-rw-r--r--   0 root         (0) root         (0)     1447 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/hrv/FrenkHrClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/hrv/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.599203 mteb-1.8.0/mteb/tasks/Classification/ind/
+-rw-r--r--   0 root         (0) root         (0)     2928 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/ind/IndonesianIdClickbaitClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/ind/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.599203 mteb-1.8.0/mteb/tasks/Classification/ita/
+-rw-r--r--   0 root         (0) root         (0)     2188 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/ita/ItalianLinguistAcceptabilityClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/ita/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.603203 mteb-1.8.0/mteb/tasks/Classification/jav/
+-rw-r--r--   0 root         (0) root         (0)     1871 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/jav/JavaneseIMDBClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/jav/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.603203 mteb-1.8.0/mteb/tasks/Classification/jpn/
+-rw-r--r--   0 root         (0) root         (0)     3402 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/jpn/WRIMEClassification.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.603203 mteb-1.8.0/mteb/tasks/Classification/kan/
+-rw-r--r--   0 root         (0) root         (0)     1676 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/kan/KannadaNewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/kan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.603203 mteb-1.8.0/mteb/tasks/Classification/kat/
+-rw-r--r--   0 root         (0) root         (0)     3016 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/kat/GeorgianSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/kat/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.603203 mteb-1.8.0/mteb/tasks/Classification/kor/
+-rw-r--r--   0 root         (0) root         (0)     2428 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/kor/KlueTC.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.603203 mteb-1.8.0/mteb/tasks/Classification/kur/
+-rw-r--r--   0 root         (0) root         (0)     1544 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/kur/KurdishSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/kur/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.603203 mteb-1.8.0/mteb/tasks/Classification/mal/
+-rw-r--r--   0 root         (0) root         (0)     1293 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/mal/MalayalamNewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/mal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.603203 mteb-1.8.0/mteb/tasks/Classification/mkd/
+-rw-r--r--   0 root         (0) root         (0)     1768 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/mkd/MacedonianTweetSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/mkd/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.607203 mteb-1.8.0/mteb/tasks/Classification/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     2313 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/multilingual/AfriSentiLangClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1377 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     3360 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/multilingual/CataloniaTweetClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2638 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/multilingual/HinDialectClassification.py
+-rw-r--r--   0 root         (0) root         (0)     5163 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/multilingual/IndicLangClassification.py
+-rw-r--r--   0 root         (0) root         (0)     3286 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/multilingual/IndicSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1627 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2537 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2543 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py
+-rw-r--r--   0 root         (0) root         (0)     6431 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/multilingual/MultiHateClassification.py
+-rw-r--r--   0 root         (0) root         (0)     3839 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/multilingual/MultilingualSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1586 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/multilingual/NordicLangClassification.py
+-rw-r--r--   0 root         (0) root         (0)     8376 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/multilingual/SIB200Classification.py
+-rw-r--r--   0 root         (0) root         (0)     6099 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/multilingual/ScalaClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1744 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/multilingual/SouthAfricanLangClassification.py
+-rw-r--r--   0 root         (0) root         (0)     3264 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/multilingual/TweetSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.607203 mteb-1.8.0/mteb/tasks/Classification/nep/
+-rw-r--r--   0 root         (0) root         (0)     2770 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/nep/NepaliNewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/nep/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.607203 mteb-1.8.0/mteb/tasks/Classification/nld/
+-rw-r--r--   0 root         (0) root         (0)     1751 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/nld/DutchBookReviewSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/nld/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.611203 mteb-1.8.0/mteb/tasks/Classification/nob/
+-rw-r--r--   0 root         (0) root         (0)     1121 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/nob/NoRecClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1173 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/nob/NorwegianParliamentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/nob/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.611203 mteb-1.8.0/mteb/tasks/Classification/ory/
+-rw-r--r--   0 root         (0) root         (0)     1306 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/ory/OdiaNewsClassification.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.611203 mteb-1.8.0/mteb/tasks/Classification/pan/
+-rw-r--r--   0 root         (0) root         (0)     1336 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/pan/PunjabiNewsClassification.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.611203 mteb-1.8.0/mteb/tasks/Classification/pol/
+-rw-r--r--   0 root         (0) root         (0)     4922 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/pol/PolishClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/pol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.611203 mteb-1.8.0/mteb/tasks/Classification/por/
+-rw-r--r--   0 root         (0) root         (0)     2307 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/por/HateSpeechPortugueseClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/por/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.611203 mteb-1.8.0/mteb/tasks/Classification/ron/
+-rw-r--r--   0 root         (0) root         (0)     1579 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/ron/RomanianSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/ron/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.611203 mteb-1.8.0/mteb/tasks/Classification/san/
+-rw-r--r--   0 root         (0) root         (0)     2851 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/san/SanskritShlokasClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/san/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.611203 mteb-1.8.0/mteb/tasks/Classification/sin/
+-rw-r--r--   0 root         (0) root         (0)     2271 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/sin/SinhalaNewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/sin/SinhalaNewsSourceClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/sin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.611203 mteb-1.8.0/mteb/tasks/Classification/slv/
+-rw-r--r--   0 root         (0) root         (0)     1680 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/slv/FrenkSlClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/slv/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.611203 mteb-1.8.0/mteb/tasks/Classification/spa/
+-rw-r--r--   0 root         (0) root         (0)     2218 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/spa/SpanishSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/spa/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.611203 mteb-1.8.0/mteb/tasks/Classification/ssw/
+-rw-r--r--   0 root         (0) root         (0)     1632 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/ssw/SiswatiNewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/ssw/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.615203 mteb-1.8.0/mteb/tasks/Classification/swe/
+-rw-r--r--   0 root         (0) root         (0)     2834 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/swe/DalajClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1043 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/swe/SweRecClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/swe/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.615203 mteb-1.8.0/mteb/tasks/Classification/tam/
+-rw-r--r--   0 root         (0) root         (0)     1408 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/tam/TamilNewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/tam/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.615203 mteb-1.8.0/mteb/tasks/Classification/tel/
+-rw-r--r--   0 root         (0) root         (0)     1382 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/tel/TeluguAndhraJyotiNewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/tel/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.615203 mteb-1.8.0/mteb/tasks/Classification/tha/
+-rw-r--r--   0 root         (0) root         (0)     2106 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/tha/WisesightSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/tha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.615203 mteb-1.8.0/mteb/tasks/Classification/tur/
+-rw-r--r--   0 root         (0) root         (0)     1640 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/tur/TurkishMovieSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1493 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/tur/TurkishProductSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/tur/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.615203 mteb-1.8.0/mteb/tasks/Classification/ukr/
+-rw-r--r--   0 root         (0) root         (0)     2485 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/ukr/UkrFormalityClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/ukr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.615203 mteb-1.8.0/mteb/tasks/Classification/urd/
+-rw-r--r--   0 root         (0) root         (0)     1739 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/urd/UrduRomanSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/urd/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.615203 mteb-1.8.0/mteb/tasks/Classification/vie/
+-rw-r--r--   0 root         (0) root         (0)     1872 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/vie/VieStudentFeedbackClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/vie/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.619203 mteb-1.8.0/mteb/tasks/Classification/zho/
+-rw-r--r--   0 root         (0) root         (0)     6571 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/zho/CMTEBClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1883 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/zho/YueOpenriceReviewClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/zho/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.619203 mteb-1.8.0/mteb/tasks/Classification/zul/
+-rw-r--r--   0 root         (0) root         (0)     1632 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/zul/IsiZuluNewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Classification/zul/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.619203 mteb-1.8.0/mteb/tasks/Clustering/
+-rw-r--r--   0 root         (0) root         (0)     1644 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.619203 mteb-1.8.0/mteb/tasks/Clustering/deu/
+-rw-r--r--   0 root         (0) root         (0)     1179 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/deu/BlurbsClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     2007 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/deu/BlurbsClusteringP2PFast.py
+-rw-r--r--   0 root         (0) root         (0)     1171 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/deu/BlurbsClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1984 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/deu/BlurbsClusteringS2SFast.py
+-rw-r--r--   0 root         (0) root         (0)     1149 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/deu/TenKGnadClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1477 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/deu/TenKGnadClusteringP2PFast.py
+-rw-r--r--   0 root         (0) root         (0)     1129 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/deu/TenKGnadClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/deu/TenKGnadClusteringS2SFast.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/deu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.623203 mteb-1.8.0/mteb/tasks/Clustering/eng/
+-rw-r--r--   0 root         (0) root         (0)     1147 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/eng/ArxivClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1579 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/eng/ArxivClusteringP2PFast.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/eng/ArxivClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/eng/BigPatentClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/eng/BiorxivClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1061 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/eng/BiorxivClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1072 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/eng/MedrxivClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1062 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/eng/MedrxivClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/eng/RedditClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1091 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/eng/RedditClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1127 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/eng/StackExchangeClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1115 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/eng/StackExchangeClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1084 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/eng/TwentyNewsgroupsClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1135 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/eng/WikiCitiesClustering.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.623203 mteb-1.8.0/mteb/tasks/Clustering/fra/
+-rw-r--r--   0 root         (0) root         (0)     1893 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/fra/AlloProfClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1739 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/fra/AlloProfClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1607 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/fra/HALClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/fra/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.623203 mteb-1.8.0/mteb/tasks/Clustering/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     3055 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/multilingual/IndicReviewsClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     3202 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/multilingual/MLSUMClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     3009 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/multilingual/MLSUMClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     2687 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     2701 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/multilingual/WikiClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.627203 mteb-1.8.0/mteb/tasks/Clustering/nob/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/nob/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3442 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/nob/snl_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     3596 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/nob/vg_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.627203 mteb-1.8.0/mteb/tasks/Clustering/pol/
+-rw-r--r--   0 root         (0) root         (0)     3352 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/pol/PolishClustering.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/pol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.627203 mteb-1.8.0/mteb/tasks/Clustering/rom/
+-rw-r--r--   0 root         (0) root         (0)     1089 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/rom/RomaniBibleClustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.627203 mteb-1.8.0/mteb/tasks/Clustering/spa/
+-rw-r--r--   0 root         (0) root         (0)     1042 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/spa/FloresClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1060 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/spa/SpanishNewsClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/spa/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.627203 mteb-1.8.0/mteb/tasks/Clustering/swe/
+-rw-r--r--   0 root         (0) root         (0)     4765 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/swe/SwednClustering.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/swe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4094 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/swe/swedn_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.627203 mteb-1.8.0/mteb/tasks/Clustering/zho/
+-rw-r--r--   0 root         (0) root         (0)     3639 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/zho/CMTEBClustering.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Clustering/zho/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.627203 mteb-1.8.0/mteb/tasks/InstructionRetrieval/
+-rw-r--r--   0 root         (0) root         (0)      176 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/InstructionRetrieval/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.627203 mteb-1.8.0/mteb/tasks/InstructionRetrieval/eng/
+-rw-r--r--   0 root         (0) root         (0)     1547 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/InstructionRetrieval/eng/Core17InstructionRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1547 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/InstructionRetrieval/eng/News21InstructionRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1556 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/InstructionRetrieval/eng/Robust04InstructionRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/InstructionRetrieval/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.627203 mteb-1.8.0/mteb/tasks/PairClassification/
+-rw-r--r--   0 root         (0) root         (0)      449 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/PairClassification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.631203 mteb-1.8.0/mteb/tasks/PairClassification/deu/
+-rw-r--r--   0 root         (0) root         (0)     2862 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/PairClassification/deu/FalseFriendsDeEnPC.py
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/PairClassification/deu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.631203 mteb-1.8.0/mteb/tasks/PairClassification/eng/
+-rw-r--r--   0 root         (0) root         (0)     4517 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/PairClassification/eng/LegalBenchPC.py
+-rw-r--r--   0 root         (0) root         (0)     1152 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/PairClassification/eng/SprintDuplicateQuestionsPC.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/PairClassification/eng/TwitterSemEval2015PC.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/PairClassification/eng/TwitterURLCorpusPC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/PairClassification/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.631203 mteb-1.8.0/mteb/tasks/PairClassification/hye/
+-rw-r--r--   0 root         (0) root         (0)     1439 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/PairClassification/hye/ArmenianParaphrasePC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/PairClassification/hye/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.631203 mteb-1.8.0/mteb/tasks/PairClassification/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     2780 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/PairClassification/multilingual/PawsX.py
+-rw-r--r--   0 root         (0) root         (0)     3290 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/PairClassification/multilingual/XNLI.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/PairClassification/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.631203 mteb-1.8.0/mteb/tasks/PairClassification/pol/
+-rw-r--r--   0 root         (0) root         (0)     3577 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/PairClassification/pol/PolishPC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/PairClassification/pol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.631203 mteb-1.8.0/mteb/tasks/PairClassification/zho/
+-rw-r--r--   0 root         (0) root         (0)     1849 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/PairClassification/zho/CMTEBPairClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/PairClassification/zho/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.631203 mteb-1.8.0/mteb/tasks/Reranking/
+-rw-r--r--   0 root         (0) root         (0)      346 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Reranking/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.635203 mteb-1.8.0/mteb/tasks/Reranking/eng/
+-rw-r--r--   0 root         (0) root         (0)     1118 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Reranking/eng/AskUbuntuDupQuestions.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Reranking/eng/MindSmallReranking.py
+-rw-r--r--   0 root         (0) root         (0)     3054 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Reranking/eng/SciDocsReranking.py
+-rw-r--r--   0 root         (0) root         (0)     1137 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Reranking/eng/StackOverflowDupQuestions.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Reranking/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.635203 mteb-1.8.0/mteb/tasks/Reranking/fra/
+-rw-r--r--   0 root         (0) root         (0)     1195 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Reranking/fra/AlloprofReranking.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Reranking/fra/SyntecReranking.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Reranking/fra/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.635203 mteb-1.8.0/mteb/tasks/Reranking/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1269 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Reranking/multilingual/MIRACLReranking.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Reranking/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.635203 mteb-1.8.0/mteb/tasks/Reranking/zho/
+-rw-r--r--   0 root         (0) root         (0)     3528 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Reranking/zho/CMTEBReranking.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Reranking/zho/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.635203 mteb-1.8.0/mteb/tasks/Retrieval/
+-rw-r--r--   0 root         (0) root         (0)     3751 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.635203 mteb-1.8.0/mteb/tasks/Retrieval/code/
+-rw-r--r--   0 root         (0) root         (0)     3275 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/code/CodeEditSearchRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3377 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/code/CodeSearchNetRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/code/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.635203 mteb-1.8.0/mteb/tasks/Retrieval/dan/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/dan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3785 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/dan/dan_fever.py
+-rw-r--r--   0 root         (0) root         (0)     2574 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/dan/t2nord_retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3139 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/dan/twitterhjerne.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.639203 mteb-1.8.0/mteb/tasks/Retrieval/deu/
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/deu/GerDaLIRRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/deu/GerDaLIRSmallRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2891 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/deu/GermanDPRRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2127 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/deu/GermanQuADRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1052 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/deu/LegalQuADRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/deu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.639203 mteb-1.8.0/mteb/tasks/Retrieval/ell/
+-rw-r--r--   0 root         (0) root         (0)     2683 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/ell/GreekCivicsQA.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/ell/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.647203 mteb-1.8.0/mteb/tasks/Retrieval/eng/
+-rw-r--r--   0 root         (0) root         (0)     1118 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/AILACasedocsRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/AILAStatutesRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1011 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/ArguAnaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/CQADupstackAndroidRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/CQADupstackEnglishRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1062 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/CQADupstackGamingRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/CQADupstackGisRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1077 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/CQADupstackMathematicaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/CQADupstackPhysicsRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1077 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/CQADupstackProgrammersRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/CQADupstackStatsRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/CQADupstackTexRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/CQADupstackUnixRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1074 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/CQADupstackWebmastersRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/CQADupstackWordpressRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/ClimateFEVERRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/DBPediaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1175 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/FEVERRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      983 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/FiQA2018Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3668 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/HagridRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1151 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/HotpotQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3022 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/LEMBNarrativeQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3648 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/LEMBNeedleRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3641 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/LEMBPasskeyRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3391 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/LEMBQMSumRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3050 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/LEMBSummScreenFDRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2526 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/LEMBWikimQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/LegalBenchConsumerContractsQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1150 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/LegalBenchCorporateLobbyingRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/LegalSummarizationRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/MSMARCORetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1039 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/MSMARCOv2Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1650 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/MedicalQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1024 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/NFCorpusRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      999 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/NQRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1991 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/NarrativeQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1155 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/QuoraRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1114 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/SCIDOCSRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1046 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/SciFactRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1069 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/TRECCOVIDRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/Touche2020Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.647203 mteb-1.8.0/mteb/tasks/Retrieval/est/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/est/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1596 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/est/estqa.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.647203 mteb-1.8.0/mteb/tasks/Retrieval/fra/
+-rw-r--r--   0 root         (0) root         (0)     2144 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/fra/AlloprofRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2481 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/fra/BSARDRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3184 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/fra/FQuADRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2148 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/fra/SyntecRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/fra/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.647203 mteb-1.8.0/mteb/tasks/Retrieval/hun/
+-rw-r--r--   0 root         (0) root         (0)     2589 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/hun/HunSum2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.647203 mteb-1.8.0/mteb/tasks/Retrieval/jpn/
+-rw-r--r--   0 root         (0) root         (0)     2853 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/jpn/JaQuADRetrieval.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.651203 mteb-1.8.0/mteb/tasks/Retrieval/kat/
+-rw-r--r--   0 root         (0) root         (0)     2568 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/kat/GeorgianFAQRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/kat/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.651203 mteb-1.8.0/mteb/tasks/Retrieval/kor/
+-rw-r--r--   0 root         (0) root         (0)      906 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/kor/KoMiracl.py
+-rw-r--r--   0 root         (0) root         (0)      922 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/kor/KoStrategyQA.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/kor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.651203 mteb-1.8.0/mteb/tasks/Retrieval/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     3776 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/multilingual/IndicQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3277 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     6239 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/multilingual/MLQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3052 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3432 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3731 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/multilingual/NeuCLIR2022Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3771 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/multilingual/NeuCLIR2023Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2979 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3145 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     4217 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/multilingual/XQuADRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.651203 mteb-1.8.0/mteb/tasks/Retrieval/nob/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/nob/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3943 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/nob/norquad.py
+-rw-r--r--   0 root         (0) root         (0)     2699 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/nob/snl_retrieval.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.655203 mteb-1.8.0/mteb/tasks/Retrieval/pol/
+-rw-r--r--   0 root         (0) root         (0)      967 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/pol/ArguAnaPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/pol/DBPediaPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      984 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/pol/FiQAPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1112 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/pol/HotpotQAPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/pol/MSMARCOPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/pol/NFCorpusPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      997 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/pol/NQPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/pol/QuoraPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1091 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/pol/SCIDOCSPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/pol/SciFactPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1085 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/pol/TRECCOVIDPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/pol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.655203 mteb-1.8.0/mteb/tasks/Retrieval/slk/
+-rw-r--r--   0 root         (0) root         (0)     2891 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/slk/SlovakSumRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/slk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.655203 mteb-1.8.0/mteb/tasks/Retrieval/spa/
+-rw-r--r--   0 root         (0) root         (0)     2125 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2P.py
+-rw-r--r--   0 root         (0) root         (0)     2056 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/spa/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.655203 mteb-1.8.0/mteb/tasks/Retrieval/swe/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/swe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3210 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/swe/swedn_retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2610 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/swe/swefaq_retrieval.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.659203 mteb-1.8.0/mteb/tasks/Retrieval/tur/
+-rw-r--r--   0 root         (0) root         (0)     3883 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/tur/TurHistQuad.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/tur/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.659203 mteb-1.8.0/mteb/tasks/Retrieval/vie/
+-rw-r--r--   0 root         (0) root         (0)     3798 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/vie/VieQuADRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/vie/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.659203 mteb-1.8.0/mteb/tasks/Retrieval/zho/
+-rw-r--r--   0 root         (0) root         (0)    10384 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/zho/CMTEBRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1121 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/zho/LeCaRDv2Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Retrieval/zho/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.659203 mteb-1.8.0/mteb/tasks/STS/
+-rw-r--r--   0 root         (0) root         (0)      757 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/STS/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.659203 mteb-1.8.0/mteb/tasks/STS/deu/
+-rw-r--r--   0 root         (0) root         (0)     1370 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/STS/deu/GermanSTSBenchmarkSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/STS/deu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.659203 mteb-1.8.0/mteb/tasks/STS/eng/
+-rw-r--r--   0 root         (0) root         (0)     1184 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/STS/eng/BiossesSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1153 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/STS/eng/STS12STS.py
+-rw-r--r--   0 root         (0) root         (0)     1150 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/STS/eng/STS13STS.py
+-rw-r--r--   0 root         (0) root         (0)     1184 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/STS/eng/STS14STS.py
+-rw-r--r--   0 root         (0) root         (0)     1148 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/STS/eng/STS15STS.py
+-rw-r--r--   0 root         (0) root         (0)     1148 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/STS/eng/STS16STS.py
+-rw-r--r--   0 root         (0) root         (0)     1208 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/STS/eng/STSBenchmarkSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1185 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/STS/eng/SickrSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/STS/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.663203 mteb-1.8.0/mteb/tasks/STS/fin/
+-rw-r--r--   0 root         (0) root         (0)     3422 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/STS/fin/FinParaSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/STS/fin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.663203 mteb-1.8.0/mteb/tasks/STS/fra/
+-rw-r--r--   0 root         (0) root         (0)     1472 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/STS/fra/SickFrSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/STS/fra/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.663203 mteb-1.8.0/mteb/tasks/STS/jpn/
+-rw-r--r--   0 root         (0) root         (0)     3034 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/STS/jpn/JSTS.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.663203 mteb-1.8.0/mteb/tasks/STS/kor/
+-rw-r--r--   0 root         (0) root         (0)     2504 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/STS/kor/KlueSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1634 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/STS/kor/KorSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/STS/kor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.663203 mteb-1.8.0/mteb/tasks/STS/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     4131 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/STS/multilingual/IndicCrosslingualSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1600 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1832 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py
+-rw-r--r--   0 root         (0) root         (0)     2712 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/STS/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.663203 mteb-1.8.0/mteb/tasks/STS/pol/
+-rw-r--r--   0 root         (0) root         (0)     2268 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/STS/pol/PolishSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/STS/pol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.663203 mteb-1.8.0/mteb/tasks/STS/ron/
+-rw-r--r--   0 root         (0) root         (0)     1896 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/STS/ron/RonSTS.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.663203 mteb-1.8.0/mteb/tasks/STS/spa/
+-rw-r--r--   0 root         (0) root         (0)     1486 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/STS/spa/STSES.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/STS/spa/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.667203 mteb-1.8.0/mteb/tasks/STS/zho/
+-rw-r--r--   0 root         (0) root         (0)     7122 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/STS/zho/CMTEBSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/STS/zho/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.667203 mteb-1.8.0/mteb/tasks/Summarization/
+-rw-r--r--   0 root         (0) root         (0)      124 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Summarization/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.667203 mteb-1.8.0/mteb/tasks/Summarization/eng/
+-rw-r--r--   0 root         (0) root         (0)     1243 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Summarization/eng/SummEvalSummarization.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Summarization/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.667203 mteb-1.8.0/mteb/tasks/Summarization/fra/
+-rw-r--r--   0 root         (0) root         (0)     1304 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Summarization/fra/SummEvalFrSummarization.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/Summarization/fra/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      288 2024-05-05 20:38:58.000000 mteb-1.8.0/mteb/tasks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.767204 mteb-1.8.0/mteb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    24072 2024-05-05 20:39:02.000000 mteb-1.8.0/mteb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    62388 2024-05-05 20:39:02.000000 mteb-1.8.0/mteb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 20:39:02.000000 mteb-1.8.0/mteb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2024-05-05 20:39:02.000000 mteb-1.8.0/mteb.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      258 2024-05-05 20:39:02.000000 mteb-1.8.0/mteb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-05 20:39:02.000000 mteb-1.8.0/mteb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2752 2024-05-05 20:38:59.000000 mteb-1.8.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.567203 mteb-1.8.0/results/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.667203 mteb-1.8.0/results/GritLM__GritLM-7B/
+-rw-r--r--   0 root         (0) root         (0)     2342 2024-05-05 20:38:58.000000 mteb-1.8.0/results/GritLM__GritLM-7B/Core17InstructionRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     2381 2024-05-05 20:38:58.000000 mteb-1.8.0/results/GritLM__GritLM-7B/News21InstructionRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     2384 2024-05-05 20:38:58.000000 mteb-1.8.0/results/GritLM__GritLM-7B/Robust04InstructionRetrieval.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.667203 mteb-1.8.0/results/cross_encoder__ms-marco-TinyBERT-L-2-v2/
+-rw-r--r--   0 root         (0) root         (0)     1154 2024-05-05 20:38:58.000000 mteb-1.8.0/results/cross_encoder__ms-marco-TinyBERT-L-2-v2/NFCorpus.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.567203 mteb-1.8.0/results/dangvantuan/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.671203 mteb-1.8.0/results/dangvantuan/sentence-camembert-base/
+-rw-r--r--   0 root         (0) root         (0)      308 2024-05-05 20:38:58.000000 mteb-1.8.0/results/dangvantuan/sentence-camembert-base/AlloProfClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)      308 2024-05-05 20:38:58.000000 mteb-1.8.0/results/dangvantuan/sentence-camembert-base/AlloProfClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      250 2024-05-05 20:38:58.000000 mteb-1.8.0/results/dangvantuan/sentence-camembert-base/AlloprofReranking.json
+-rw-r--r--   0 root         (0) root         (0)     1165 2024-05-05 20:38:58.000000 mteb-1.8.0/results/dangvantuan/sentence-camembert-base/AlloprofRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      634 2024-05-05 20:38:58.000000 mteb-1.8.0/results/dangvantuan/sentence-camembert-base/AmazonReviewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      305 2024-05-05 20:38:58.000000 mteb-1.8.0/results/dangvantuan/sentence-camembert-base/HALClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      308 2024-05-05 20:38:58.000000 mteb-1.8.0/results/dangvantuan/sentence-camembert-base/MLSUMClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)      305 2024-05-05 20:38:58.000000 mteb-1.8.0/results/dangvantuan/sentence-camembert-base/MLSUMClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      675 2024-05-05 20:38:58.000000 mteb-1.8.0/results/dangvantuan/sentence-camembert-base/MTOPDomainClassification.json
+-rw-r--r--   0 root         (0) root         (0)      676 2024-05-05 20:38:58.000000 mteb-1.8.0/results/dangvantuan/sentence-camembert-base/MTOPIntentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      411 2024-05-05 20:38:58.000000 mteb-1.8.0/results/dangvantuan/sentence-camembert-base/MasakhaNEWSClassification.json
+-rw-r--r--   0 root         (0) root         (0)      332 2024-05-05 20:38:58.000000 mteb-1.8.0/results/dangvantuan/sentence-camembert-base/MasakhaNEWSClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)      335 2024-05-05 20:38:58.000000 mteb-1.8.0/results/dangvantuan/sentence-camembert-base/MasakhaNEWSClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      679 2024-05-05 20:38:58.000000 mteb-1.8.0/results/dangvantuan/sentence-camembert-base/MassiveIntentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      679 2024-05-05 20:38:58.000000 mteb-1.8.0/results/dangvantuan/sentence-camembert-base/MassiveScenarioClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1242 2024-05-05 20:38:58.000000 mteb-1.8.0/results/dangvantuan/sentence-camembert-base/MintakaRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     2992 2024-05-05 20:38:58.000000 mteb-1.8.0/results/dangvantuan/sentence-camembert-base/OpusparcusPC.json
+-rw-r--r--   0 root         (0) root         (0)     2801 2024-05-05 20:38:58.000000 mteb-1.8.0/results/dangvantuan/sentence-camembert-base/PawsX.json
+-rw-r--r--   0 root         (0) root         (0)      820 2024-05-05 20:38:58.000000 mteb-1.8.0/results/dangvantuan/sentence-camembert-base/SICKFr.json
+-rw-r--r--   0 root         (0) root         (0)      511 2024-05-05 20:38:58.000000 mteb-1.8.0/results/dangvantuan/sentence-camembert-base/STS22.json
+-rw-r--r--   0 root         (0) root         (0)      921 2024-05-05 20:38:58.000000 mteb-1.8.0/results/dangvantuan/sentence-camembert-base/STSBenchmarkMultilingualSTS.json
+-rw-r--r--   0 root         (0) root         (0)      371 2024-05-05 20:38:58.000000 mteb-1.8.0/results/dangvantuan/sentence-camembert-base/SummEvalFr.json
+-rw-r--r--   0 root         (0) root         (0)      221 2024-05-05 20:38:58.000000 mteb-1.8.0/results/dangvantuan/sentence-camembert-base/SyntecReranking.json
+-rw-r--r--   0 root         (0) root         (0)     1099 2024-05-05 20:38:58.000000 mteb-1.8.0/results/dangvantuan/sentence-camembert-base/SyntecRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1245 2024-05-05 20:38:58.000000 mteb-1.8.0/results/dangvantuan/sentence-camembert-base/XPQARetrieval.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.567203 mteb-1.8.0/results/intfloat/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.675203 mteb-1.8.0/results/intfloat/multilingual-e5-small/
+-rw-r--r--   0 root         (0) root         (0)      380 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat/multilingual-e5-small/HinDialectClassification.json
+-rw-r--r--   0 root         (0) root         (0)      382 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat/multilingual-e5-small/MalayalamNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      366 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat/multilingual-e5-small/OdiaNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      369 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat/multilingual-e5-small/SouthAfricanLangClassification.json
+-rw-r--r--   0 root         (0) root         (0)      367 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat/multilingual-e5-small/TamilNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      383 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat/multilingual-e5-small/TeluguAndhraJyotiNewsClassification.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.675203 mteb-1.8.0/results/intfloat__e5-small/
+-rw-r--r--   0 root         (0) root         (0)      439 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__e5-small/TurkishProductSentimentClassification.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.675203 mteb-1.8.0/results/intfloat__e5-small-v2/
+-rw-r--r--   0 root         (0) root         (0)     2512 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__e5-small-v2/Core17InstructionRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     2540 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__e5-small-v2/News21InstructionRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     2550 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__e5-small-v2/Robust04InstructionRetrieval.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.679203 mteb-1.8.0/results/intfloat__multilingual-e5-base/
+-rw-r--r--   0 root         (0) root         (0)      758 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-base/CroatianSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      733 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-base/CzechSubjectivityClassification.json
+-rw-r--r--   0 root         (0) root         (0)      464 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-base/DutchBookReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      382 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-base/HotelReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      384 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-base/IsiZuluNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      757 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-base/MalteseSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      453 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-base/RestaurantReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      447 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-base/RomanianSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      356 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-base/SiswatiNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      376 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-base/TweetEmotionClassification.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-base/TweetSarcasmClassification.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-base/UyghurSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-base/model_meta.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.715204 mteb-1.8.0/results/intfloat__multilingual-e5-small/
+-rw-r--r--   0 root         (0) root         (0)      405 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/AJGT.json
+-rw-r--r--   0 root         (0) root         (0)      375 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/AfriSentiLangClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1422 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/ArmenianParaphrasePC.json
+-rw-r--r--   0 root         (0) root         (0)      376 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/ArxivClassification.json
+-rw-r--r--   0 root         (0) root         (0)      517 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/ArxivClusteringP2P.v2.json
+-rw-r--r--   0 root         (0) root         (0)     1161 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/BSARDRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      380 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/BengaliHateSpeechClassification.json
+-rw-r--r--   0 root         (0) root         (0)      446 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/BengaliSentimentAnalysis.json
+-rw-r--r--   0 root         (0) root         (0)   336719 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/BibleNLPBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)     1083 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/BlurbsClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)     1081 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/BlurbsClusteringS2S.v2.json
+-rw-r--r--   0 root         (0) root         (0)      397 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/BulgarianStoreReviewSentimentClassfication.json
+-rw-r--r--   0 root         (0) root         (0)      445 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/CUADAffiliateLicenseLicenseeLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      426 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/CUADAffiliateLicenseLicensorLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      454 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/CUADAntiAssignmentLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/CUADAuditRightsLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      455 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/CUADCapOnLiabilityLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      414 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/CUADChangeOfControlLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      433 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/CUADCompetitiveRestrictionExceptionLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      436 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/CUADCovenantNotToSueLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      434 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/CUADEffectiveDateLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/CUADExclusivityLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      433 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/CUADExpirationDateLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/CUADGoverningLawLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      460 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/CUADIPOwnershipAssignmentLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      468 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/CUADInsuranceLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      449 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/CUADIrrevocableOrPerpetualLicenseLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      418 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/CUADJointIPOwnershipLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      434 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/CUADLicenseGrantLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      438 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/CUADLiquidatedDamagesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      437 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/CUADMinimumCommitmentLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      396 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/CUADMostFavoredNationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      441 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/CUADNoSolicitOfCustomersLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      460 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/CUADNoSolicitOfEmployeesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      429 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/CUADNonCompeteLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      424 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/CUADNonDisparagementLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      425 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/CUADNonTransferableLicenseLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      431 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/CUADNoticePeriodToTerminateRenewalLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      445 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/CUADPostTerminationServicesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      457 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/CUADPriceRestrictionsLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      386 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/CanadaTaxCourtOutcomesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      616 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/CataloniaTweetClassification.json
+-rw-r--r--   0 root         (0) root         (0)    13681 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/CodeEditSearchRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     5524 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/CodeSearchNetRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      492 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/ContractNLIConfidentialityOfAgreementLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      449 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/ContractNLIExplicitIdentificationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      483 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/ContractNLIInclusionOfVerballyConveyedInformationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      438 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/ContractNLILimitedUseLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      439 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/ContractNLINoLicensingLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      492 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/ContractNLINoticeOnCompelledDisclosureLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      470 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/ContractNLIPermissibleAcquirementOfSimilarInformationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      422 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/ContractNLIPermissibleCopyLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      470 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/ContractNLIPermissibleDevelopmentOfSimilarInformationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      461 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/ContractNLIPermissiblePostAgreementPossessionLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      478 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/ContractNLIReturnOfConfidentialInformationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      428 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/ContractNLISharingWithEmployeesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      469 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/ContractNLISharingWithThirdPartiesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      430 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/ContractNLISurvivalOfObligationsLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/CorporateLobbyingLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      738 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/CzechSubjectivityClassification.json
+-rw-r--r--   0 root         (0) root         (0)      369 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/DBpediaClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1016 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/DanFEVER.json
+-rw-r--r--   0 root         (0) root         (0)      463 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/DutchBookReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/EstQA.json
+-rw-r--r--   0 root         (0) root         (0)      387 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/EstonianValenceClassification.json
+-rw-r--r--   0 root         (0) root         (0)     2105 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/FQuADRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      733 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/FilipinoHateSpeechClassification.json
+-rw-r--r--   0 root         (0) root         (0)      611 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/FilipinoShopeeReviewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      827 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/FinParaSTS.json
+-rw-r--r--   0 root         (0) root         (0)      443 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/FinToxicityClassification.json
+-rw-r--r--   0 root         (0) root         (0)      389 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/FinancialPhrasebankClassification.json
+-rw-r--r--   0 root         (0) root         (0)      446 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/FrenkEnClassification.json
+-rw-r--r--   0 root         (0) root         (0)      445 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/FrenkHrClassification.json
+-rw-r--r--   0 root         (0) root         (0)      438 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/FrenkSlClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1168 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/GeorgianFAQRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      453 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/GeorgianSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1150 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/GermanDPR.json
+-rw-r--r--   0 root         (0) root         (0)      401 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/GermanPoliticiansTwitterSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1150 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/GreekCivicsQA.json
+-rw-r--r--   0 root         (0) root         (0)      606 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/GreekLegalCodeClassification.json
+-rw-r--r--   0 root         (0) root         (0)      378 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/GujaratiNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      451 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/HateSpeechPortugueseClassification.json
+-rw-r--r--   0 root         (0) root         (0)      377 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/HindiDiscourseClassification.json
+-rw-r--r--   0 root         (0) root         (0)      381 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/HotelReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/HunSum2AbstractiveRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1289 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/IN22ConvBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      604 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/IN22GenBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)     4319 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/IndicCrosslingualSTS.json
+-rw-r--r--   0 root         (0) root         (0)      377 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/IndicLangClassification.json
+-rw-r--r--   0 root         (0) root         (0)    11798 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/IndicQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     4273 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/IndicReviewsClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)     3924 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/IndicSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      454 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/IndonesianIdClickbaitClassification.json
+-rw-r--r--   0 root         (0) root         (0)      384 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/IsiZuluNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      431 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/Itacola.json
+-rw-r--r--   0 root         (0) root         (0)      475 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/JSTS.json
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/JaQuADRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      431 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/JavaneseIMDBClassification.json
+-rw-r--r--   0 root         (0) root         (0)      479 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/KLUE-STS.json
+-rw-r--r--   0 root         (0) root         (0)      359 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/KLUE-TC.json
+-rw-r--r--   0 root         (0) root         (0)      371 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/KannadaNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      469 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/KorSTS.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/KurdishSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1163 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/LEMBNarrativeQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     7814 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/LEMBNeedleRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     7703 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/LEMBPasskeyRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1153 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/LEMBQMSumRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1169 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/LEMBSummScreenFDRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1149 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/LEMBWikimQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1411 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/LegalBenchPC.json
+-rw-r--r--   0 root         (0) root         (0)     2360 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/MLQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     3894 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/MLSUMClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)     1153 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/MLSUMClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      394 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/MacedonianTweetSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/MedicalQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      749 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/MovieReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     3151 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/MultiHateClassification.json
+-rw-r--r--   0 root         (0) root         (0)     8513 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/MultilingualSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)   417235 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/NTREXBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      373 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/NepaliNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)     3386 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/NeuCLIR2022Retrieval.json
+-rw-r--r--   0 root         (0) root         (0)     3392 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/NeuCLIR2023Retrieval.json
+-rw-r--r--   0 root         (0) root         (0)      371 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/NewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/NorQuadRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      381 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/NordicLangClassification.json
+-rw-r--r--   0 root         (0) root         (0)      374 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/NorwegianCourtsBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      359 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/PatentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      745 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/PersianFoodSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      514 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/PlscClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)      513 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/PlscClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      447 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/PunjabiNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      454 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/RestaurantReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      403 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/RomaTalesBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      306 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/RomaniBibleClustering.json
+-rw-r--r--   0 root         (0) root         (0)      445 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/RomanianSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      472 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/RonSTS.json
+-rw-r--r--   0 root         (0) root         (0)    42700 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/SIB200Classification.json
+-rw-r--r--   0 root         (0) root         (0)      298 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/SNLClustering.json
+-rw-r--r--   0 root         (0) root         (0)     1023 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/SNLRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      584 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/SRNCorpusBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      592 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/SanskritShlokasClassification.json
+-rw-r--r--   0 root         (0) root         (0)      374 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/SentimentAnalysisHindi.json
+-rw-r--r--   0 root         (0) root         (0)      370 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/SinhalaNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      381 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/SinhalaNewsSourceClassification.json
+-rw-r--r--   0 root         (0) root         (0)      384 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/SiswatiNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      453 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/SlovakSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/SlovakSumRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      430 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/SpanishSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1015 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/SweFaqRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      304 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/SwednClustering.json
+-rw-r--r--   0 root         (0) root         (0)      893 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/SwednClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)      524 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/SwednClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)     1023 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/SwednRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1116 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/SyntecRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/TV2Nordretrieval.json
+-rw-r--r--   0 root         (0) root         (0)      629 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/TbilisiCityHallBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      597 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/TenKGnadClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      522 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/TenKGnadClusteringS2S.v2.json
+-rw-r--r--   0 root         (0) root         (0)      448 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/ToxicChatClassification.json
+-rw-r--r--   0 root         (0) root         (0)      446 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/ToxicConversationsClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1166 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/TurHistQuadRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      459 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/TurkishMovieSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      459 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/TurkishProductSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      374 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/TweetEmotionClassification.json
+-rw-r--r--   0 root         (0) root         (0)      451 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/TweetSarcasmClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1827 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/TweetSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      391 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/TweetTopicSingleClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/TwitterHjerneRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      734 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/UkrFormalityClassification.json
+-rw-r--r--   0 root         (0) root         (0)      383 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/UrduRomanSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      303 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/VGClustering.json
+-rw-r--r--   0 root         (0) root         (0)      351 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/VieMedEVBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)     1028 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/VieQuADRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      378 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/VieStudentFeedbackClassification.json
+-rw-r--r--   0 root         (0) root         (0)      368 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/WRIMEClassification.json
+-rw-r--r--   0 root         (0) root         (0)     2184 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/WikiClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)      388 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/WisesightSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)    38759 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/XNLI.json
+-rw-r--r--   0 root         (0) root         (0)    12839 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/XQuADRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      377 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/YahooAnswersTopicsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      378 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/YelpReviewFullClassification.json
+-rw-r--r--   0 root         (0) root         (0)      380 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/YueOpenriceReviewClassification.json
+-rw-r--r--   0 root         (0) root         (0)       66 2024-05-05 20:38:58.000000 mteb-1.8.0/results/intfloat__multilingual-e5-small/model_meta.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.567203 mteb-1.8.0/results/sentence-transformers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.715204 mteb-1.8.0/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/
+-rw-r--r--   0 root         (0) root         (0)      380 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/HinDialectClassification.json
+-rw-r--r--   0 root         (0) root         (0)      380 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/MalayalamNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      364 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/OdiaNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      377 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/SouthAfricanLangClassification.json
+-rw-r--r--   0 root         (0) root         (0)      370 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/TamilNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)    21290 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/Tatoeba_fast.json
+-rw-r--r--   0 root         (0) root         (0)    21291 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/Tatoeba_slow.json
+-rw-r--r--   0 root         (0) root         (0)      382 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/TeluguAndhraJyotiNewsClassification.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.719204 mteb-1.8.0/results/sentence-transformers__all-MiniLM-L6-v2/
+-rw-r--r--   0 root         (0) root         (0)      385 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__all-MiniLM-L6-v2/Banking77Classification.json
+-rw-r--r--   0 root         (0) root         (0)      340 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__all-MiniLM-L6-v2/BornholmBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__all-MiniLM-L6-v2/DanFEVER.json
+-rw-r--r--   0 root         (0) root         (0)   387673 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__all-MiniLM-L6-v2/NTREXBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__all-MiniLM-L6-v2/NorQuadRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      374 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__all-MiniLM-L6-v2/NorwegianCourtsBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      303 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__all-MiniLM-L6-v2/SNLClustering.json
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__all-MiniLM-L6-v2/SNLRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1014 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__all-MiniLM-L6-v2/SweFaqRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      306 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__all-MiniLM-L6-v2/SwednClustering.json
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__all-MiniLM-L6-v2/SwednRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__all-MiniLM-L6-v2/TV2Nordretrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__all-MiniLM-L6-v2/TwitterHjerneRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      302 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__all-MiniLM-L6-v2/VGClustering.json
+-rw-r--r--   0 root         (0) root         (0)      194 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__all-MiniLM-L6-v2/model.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.755204 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/
+-rw-r--r--   0 root         (0) root         (0)      428 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/AJGT.json
+-rw-r--r--   0 root         (0) root         (0)      376 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/AfriSentiLangClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1452 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ArmenianParaphrasePC.json
+-rw-r--r--   0 root         (0) root         (0)      355 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ArxivClassification.json
+-rw-r--r--   0 root         (0) root         (0)      520 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ArxivClusteringP2P.v2.json
+-rw-r--r--   0 root         (0) root         (0)     1160 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BSARDRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1001 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BUCC.json
+-rw-r--r--   0 root         (0) root         (0)      454 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BambaraSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      384 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BengaliHateSpeechClassification.json
+-rw-r--r--   0 root         (0) root         (0)      444 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BengaliSentimentAnalysis.json
+-rw-r--r--   0 root         (0) root         (0)   338028 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BibleNLPBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)     1086 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BlurbsClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)     1088 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BlurbsClusteringS2S.v2.json
+-rw-r--r--   0 root         (0) root         (0)      344 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BornholmBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      398 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BulgarianStoreReviewSentimentClassfication.json
+-rw-r--r--   0 root         (0) root         (0)      462 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADAffiliateLicenseLicenseeLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      381 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADAffiliateLicenseLicensorLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      435 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADAntiAssignmentLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      432 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADAuditRightsLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      416 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADCapOnLiabilityLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      455 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADChangeOfControlLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      471 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADCompetitiveRestrictionExceptionLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      456 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADCovenantNotToSueLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      434 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADEffectiveDateLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      431 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADExclusivityLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      435 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADExpirationDateLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      451 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADGoverningLawLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      423 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADIPOwnershipAssignmentLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      430 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADInsuranceLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      469 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADIrrevocableOrPerpetualLicenseLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      394 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADJointIPOwnershipLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      415 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADLicenseGrantLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      388 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADLiquidatedDamagesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      457 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADMinimumCommitmentLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      365 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADMostFavoredNationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      411 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADNoSolicitOfCustomersLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      441 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADNoSolicitOfEmployeesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADNonCompeteLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      390 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADNonDisparagementLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      442 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADNonTransferableLicenseLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      449 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADNoticePeriodToTerminateRenewalLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      444 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADPostTerminationServicesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      438 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADPriceRestrictionsLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      387 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CanadaTaxCourtOutcomesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      641 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CataloniaTweetClassification.json
+-rw-r--r--   0 root         (0) root         (0)    13663 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CodeEditSearchRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     5535 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CodeSearchNetRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      472 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIConfidentialityOfAgreementLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      450 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIExplicitIdentificationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      449 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIInclusionOfVerballyConveyedInformationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      414 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLILimitedUseLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      439 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLINoLicensingLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      474 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLINoticeOnCompelledDisclosureLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      469 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIPermissibleAcquirementOfSimilarInformationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      443 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIPermissibleCopyLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      442 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIPermissibleDevelopmentOfSimilarInformationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      464 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIPermissiblePostAgreementPossessionLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      456 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIReturnOfConfidentialInformationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      426 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLISharingWithEmployeesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      450 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLISharingWithThirdPartiesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      449 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLISurvivalOfObligationsLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      435 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CorporateLobbyingLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      758 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CzechSubjectivityClassification.json
+-rw-r--r--   0 root         (0) root         (0)      369 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DBpediaClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DanFEVER.json
+-rw-r--r--   0 root         (0) root         (0)      603 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DiaBlaBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      464 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DutchBookReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1139 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/EstQA.json
+-rw-r--r--   0 root         (0) root         (0)      385 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/EstonianValenceClassification.json
+-rw-r--r--   0 root         (0) root         (0)     2108 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FQuADRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      746 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FilipinoHateSpeechClassification.json
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FilipinoShopeeReviewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      835 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FinParaSTS.json
+-rw-r--r--   0 root         (0) root         (0)      441 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FinToxicityClassification.json
+-rw-r--r--   0 root         (0) root         (0)      389 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FinancialPhrasebankClassification.json
+-rw-r--r--   0 root         (0) root         (0)      291 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FloresClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      443 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FrenkEnClassification.json
+-rw-r--r--   0 root         (0) root         (0)      445 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FrenkHrClassification.json
+-rw-r--r--   0 root         (0) root         (0)      433 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FrenkSlClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1165 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GeorgianFAQRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      454 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GeorgianSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GerDaLIR.json
+-rw-r--r--   0 root         (0) root         (0)      405 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GermanPoliticiansTwitterSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1157 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GreekCivicsQA.json
+-rw-r--r--   0 root         (0) root         (0)      610 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GreekLegalCodeClassification.json
+-rw-r--r--   0 root         (0) root         (0)      381 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GujaratiNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      448 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HateSpeechPortugueseClassification.json
+-rw-r--r--   0 root         (0) root         (0)      372 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HindiDiscourseClassification.json
+-rw-r--r--   0 root         (0) root         (0)      380 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HotelReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1032 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HunSum2AbstractiveRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1317 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IN22ConvBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      605 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IN22GenBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)     4370 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicCrosslingualSTS.json
+-rw-r--r--   0 root         (0) root         (0)      380 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicLangClassification.json
+-rw-r--r--   0 root         (0) root         (0)    11833 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     4276 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicReviewsClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)     3921 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      456 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndonesianIdClickbaitClassification.json
+-rw-r--r--   0 root         (0) root         (0)      385 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IsiZuluNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      430 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Itacola.json
+-rw-r--r--   0 root         (0) root         (0)      475 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JSTS.json
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JaQuADRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      441 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JavaneseIMDBClassification.json
+-rw-r--r--   0 root         (0) root         (0)      479 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/KLUE-STS.json
+-rw-r--r--   0 root         (0) root         (0)      358 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/KLUE-TC.json
+-rw-r--r--   0 root         (0) root         (0)      369 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/KannadaNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      470 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/KorSTS.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/KurdishSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1167 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBNarrativeQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     7839 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBNeedleRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     7915 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBPasskeyRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1153 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBQMSumRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1153 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBSummScreenFDRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1152 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBWikimQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1454 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LegalBenchPC.json
+-rw-r--r--   0 root         (0) root         (0)   104611 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MLQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     3877 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MLSUMClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)     3884 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MLSUMClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      394 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MacedonianTweetSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MedicalQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      748 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MovieReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     3151 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MultiHateClassification.json
+-rw-r--r--   0 root         (0) root         (0)     8537 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MultilingualSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)   421556 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NTREXBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      365 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NepaliNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)     3382 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NeuCLIR2022Retrieval.json
+-rw-r--r--   0 root         (0) root         (0)     3376 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NeuCLIR2023Retrieval.json
+-rw-r--r--   0 root         (0) root         (0)      370 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NorQuadRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      383 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NordicLangClassification.json
+-rw-r--r--   0 root         (0) root         (0)      374 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NorwegianCourtsBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)    16669 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/OpusparcusPC.json
+-rw-r--r--   0 root         (0) root         (0)      369 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PatentClassification.json
+-rw-r--r--   0 root         (0) root         (0)    18247 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PawsX.json
+-rw-r--r--   0 root         (0) root         (0)      741 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PersianFoodSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      511 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PlscClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)      517 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PlscClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      448 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PunjabiNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RestaurantReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      404 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RomaTalesBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      308 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RomaniBibleClustering.json
+-rw-r--r--   0 root         (0) root         (0)      441 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RomanianSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      471 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RonSTS.json
+-rw-r--r--   0 root         (0) root         (0)    42635 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SIB200Classification.json
+-rw-r--r--   0 root         (0) root         (0)      300 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SNLClustering.json
+-rw-r--r--   0 root         (0) root         (0)     1011 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SNLRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      599 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SRNCorpusBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      620 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SanskritShlokasClassification.json
+-rw-r--r--   0 root         (0) root         (0)      373 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SentimentAnalysisHindi.json
+-rw-r--r--   0 root         (0) root         (0)      373 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SinhalaNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      378 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SinhalaNewsSourceClassification.json
+-rw-r--r--   0 root         (0) root         (0)      380 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SiswatiNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1149 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SlovakSumRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      454 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SpanishSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SweFaqRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      303 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednClustering.json
+-rw-r--r--   0 root         (0) root         (0)      898 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)      523 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)     1022 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TV2Nordretrieval.json
+-rw-r--r--   0 root         (0) root         (0)      637 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TbilisiCityHallBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      605 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TenKGnadClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      523 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TenKGnadClusteringS2S.v2.json
+-rw-r--r--   0 root         (0) root         (0)      446 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ToxicChatClassification.json
+-rw-r--r--   0 root         (0) root         (0)      447 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ToxicConversationsClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1165 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TurHistQuadRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      451 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TurkishMovieSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      440 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TurkishProductSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      373 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TweetEmotionClassification.json
+-rw-r--r--   0 root         (0) root         (0)      450 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TweetSarcasmClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1822 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TweetSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      388 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TweetTopicSingleClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1035 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TwitterHjerneRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      727 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/UkrFormalityClassification.json
+-rw-r--r--   0 root         (0) root         (0)      385 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/UrduRomanSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      300 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VGClustering.json
+-rw-r--r--   0 root         (0) root         (0)      351 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieMedEVBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)     1029 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieQuADRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      370 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieStudentFeedbackClassification.json
+-rw-r--r--   0 root         (0) root         (0)      363 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WRIMEClassification.json
+-rw-r--r--   0 root         (0) root         (0)      294 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WikiCitiesClustering.json
+-rw-r--r--   0 root         (0) root         (0)     2186 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WikiClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)      384 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WisesightSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)    38547 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/XNLI.json
+-rw-r--r--   0 root         (0) root         (0)    12890 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/XQuADRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      378 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/YahooAnswersTopicsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      378 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/YelpReviewFullClassification.json
+-rw-r--r--   0 root         (0) root         (0)      377 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/YueOpenriceReviewClassification.json
+-rw-r--r--   0 root         (0) root         (0)      176 2024-05-05 20:38:58.000000 mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/model_meta.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.759204 mteb-1.8.0/scripts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.759204 mteb-1.8.0/scripts/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.759204 mteb-1.8.0/scripts/data/amazon_polarity/
+-rw-r--r--   0 root         (0) root         (0)      842 2024-05-05 20:38:58.000000 mteb-1.8.0/scripts/data/amazon_polarity/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.759204 mteb-1.8.0/scripts/data/amazon_reviews_multi/
+-rw-r--r--   0 root         (0) root         (0)     1379 2024-05-05 20:38:58.000000 mteb-1.8.0/scripts/data/amazon_reviews_multi/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.759204 mteb-1.8.0/scripts/data/arxiv/
+-rw-r--r--   0 root         (0) root         (0)     3146 2024-05-05 20:38:58.000000 mteb-1.8.0/scripts/data/arxiv/script_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     1450 2024-05-05 20:38:58.000000 mteb-1.8.0/scripts/data/arxiv/script_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.759204 mteb-1.8.0/scripts/data/biorxiv/
+-rw-r--r--   0 root         (0) root         (0)     1781 2024-05-05 20:38:58.000000 mteb-1.8.0/scripts/data/biorxiv/script_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     1672 2024-05-05 20:38:58.000000 mteb-1.8.0/scripts/data/biorxiv/script_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.759204 mteb-1.8.0/scripts/data/bucc/
+-rw-r--r--   0 root         (0) root         (0)     1171 2024-05-05 20:38:58.000000 mteb-1.8.0/scripts/data/bucc/create_data.py
+-rw-r--r--   0 root         (0) root         (0)     5924 2024-05-05 20:38:58.000000 mteb-1.8.0/scripts/data/create_task_table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.759204 mteb-1.8.0/scripts/data/germanquad/
+-rw-r--r--   0 root         (0) root         (0)     2133 2024-05-05 20:38:58.000000 mteb-1.8.0/scripts/data/germanquad/process_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.759204 mteb-1.8.0/scripts/data/hal/
+-rw-r--r--   0 root         (0) root         (0)     1512 2024-05-05 20:38:58.000000 mteb-1.8.0/scripts/data/hal/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.759204 mteb-1.8.0/scripts/data/imdb/
+-rw-r--r--   0 root         (0) root         (0)      682 2024-05-05 20:38:58.000000 mteb-1.8.0/scripts/data/imdb/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.759204 mteb-1.8.0/scripts/data/medicalqaretrieval/
+-rw-r--r--   0 root         (0) root         (0)     1884 2024-05-05 20:38:58.000000 mteb-1.8.0/scripts/data/medicalqaretrieval/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.763204 mteb-1.8.0/scripts/data/medrxiv/
+-rw-r--r--   0 root         (0) root         (0)     1780 2024-05-05 20:38:58.000000 mteb-1.8.0/scripts/data/medrxiv/script_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     1615 2024-05-05 20:38:58.000000 mteb-1.8.0/scripts/data/medrxiv/script_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.763204 mteb-1.8.0/scripts/data/mind/
+-rw-r--r--   0 root         (0) root         (0)     1377 2024-05-05 20:38:58.000000 mteb-1.8.0/scripts/data/mind/prepare_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.763204 mteb-1.8.0/scripts/data/multilingual_sentiment_classification/
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-05-05 20:38:58.000000 mteb-1.8.0/scripts/data/multilingual_sentiment_classification/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.763204 mteb-1.8.0/scripts/data/redditp2p/
+-rw-r--r--   0 root         (0) root         (0)     1880 2024-05-05 20:38:58.000000 mteb-1.8.0/scripts/data/redditp2p/script_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.763204 mteb-1.8.0/scripts/data/stackexchangep2p/
+-rw-r--r--   0 root         (0) root         (0)     1627 2024-05-05 20:38:58.000000 mteb-1.8.0/scripts/data/stackexchangep2p/script_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.763204 mteb-1.8.0/scripts/data/sts22-crosslingual-sts/
+-rw-r--r--   0 root         (0) root         (0)     2435 2024-05-05 20:38:58.000000 mteb-1.8.0/scripts/data/sts22-crosslingual-sts/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.763204 mteb-1.8.0/scripts/data/summeval_fr/
+-rw-r--r--   0 root         (0) root         (0)     1692 2024-05-05 20:38:58.000000 mteb-1.8.0/scripts/data/summeval_fr/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.763204 mteb-1.8.0/scripts/data/toxic_conversations_50k/
+-rw-r--r--   0 root         (0) root         (0)     1151 2024-05-05 20:38:58.000000 mteb-1.8.0/scripts/data/toxic_conversations_50k/create_data.py
+-rw-r--r--   0 root         (0) root         (0)     2515 2024-05-05 20:38:58.000000 mteb-1.8.0/scripts/merge_cqadupstack.py
+-rw-r--r--   0 root         (0) root         (0)     5216 2024-05-05 20:38:58.000000 mteb-1.8.0/scripts/mteb_meta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.571203 mteb-1.8.0/scripts/results/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.763204 mteb-1.8.0/scripts/results/intfloat__multilingual-e5-small/
+-rw-r--r--   0 root         (0) root         (0)      376 2024-05-05 20:38:58.000000 mteb-1.8.0/scripts/results/intfloat__multilingual-e5-small/HindiDiscourseClassification.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.763204 mteb-1.8.0/scripts/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/
+-rw-r--r--   0 root         (0) root         (0)      376 2024-05-05 20:38:58.000000 mteb-1.8.0/scripts/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HindiDiscourseClassification.json
+-rw-r--r--   0 root         (0) root         (0)      673 2024-05-05 20:38:58.000000 mteb-1.8.0/scripts/run_mteb_chinese.py
+-rw-r--r--   0 root         (0) root         (0)     2819 2024-05-05 20:38:58.000000 mteb-1.8.0/scripts/run_mteb_english.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2024-05-05 20:38:58.000000 mteb-1.8.0/scripts/run_mteb_french.py
+-rw-r--r--   0 root         (0) root         (0)     1334 2024-05-05 20:38:58.000000 mteb-1.8.0/scripts/run_mteb_german.py
+-rw-r--r--   0 root         (0) root         (0)     1017 2024-05-05 20:38:58.000000 mteb-1.8.0/scripts/run_mteb_korean.py
+-rw-r--r--   0 root         (0) root         (0)      876 2024-05-05 20:38:58.000000 mteb-1.8.0/scripts/run_mteb_law.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2024-05-05 20:38:58.000000 mteb-1.8.0/scripts/run_mteb_polish.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-05 20:39:02.767204 mteb-1.8.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:39:02.763204 mteb-1.8.0/tests/
+-rw-r--r--   0 root         (0) root         (0)      632 2024-05-05 20:38:58.000000 mteb-1.8.0/tests/test_ClusteringEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1418 2024-05-05 20:38:58.000000 mteb-1.8.0/tests/test_InstructionRetrievalEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1560 2024-05-05 20:38:58.000000 mteb-1.8.0/tests/test_PairClassificationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1129 2024-05-05 20:38:58.000000 mteb-1.8.0/tests/test_RerankingEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1112 2024-05-05 20:38:58.000000 mteb-1.8.0/tests/test_RetrievalEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)    11651 2024-05-05 20:38:58.000000 mteb-1.8.0/tests/test_TaskMetadata.py
+-rw-r--r--   0 root         (0) root         (0)     2602 2024-05-05 20:38:58.000000 mteb-1.8.0/tests/test_all_abstasks.py
+-rw-r--r--   0 root         (0) root         (0)      598 2024-05-05 20:38:58.000000 mteb-1.8.0/tests/test_encoder_interfaces.py
+-rw-r--r--   0 root         (0) root         (0)     1390 2024-05-05 20:38:58.000000 mteb-1.8.0/tests/test_mteb.py
+-rw-r--r--   0 root         (0) root         (0)     7159 2024-05-05 20:38:58.000000 mteb-1.8.0/tests/test_mteb_rerank.py
+-rw-r--r--   0 root         (0) root         (0)     3013 2024-05-05 20:38:58.000000 mteb-1.8.0/tests/test_overview.py
+-rw-r--r--   0 root         (0) root         (0)      278 2024-05-05 20:38:58.000000 mteb-1.8.0/tests/test_retrieval_abstask.py
```

### Comparing `mteb-1.7.9/LICENSE` & `mteb-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/PKG-INFO` & `mteb-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mteb
-Version: 1.7.9
+Version: 1.8.0
 Summary: Massive Text Embedding Benchmark
 Author-email: MTEB Contributors <niklas@huggingface.co>, nouamane@huggingface.co, info@nils-reimers.de
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -215,28 +215,29 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: datasets>=2.2.0
+Requires-Dist: datasets>=2.19.0
 Requires-Dist: jsonlines
 Requires-Dist: numpy
 Requires-Dist: requests>=2.26.0
 Requires-Dist: scikit_learn>=1.0.2
 Requires-Dist: scipy
 Requires-Dist: sentence_transformers>=2.2.0
 Requires-Dist: torch
 Requires-Dist: tqdm
 Requires-Dist: rich
 Requires-Dist: pytrec-eval-terrier>=0.5.6
 Requires-Dist: pydantic>=2.0.0
 Requires-Dist: typing_extensions
 Requires-Dist: eval_type_backport
+Requires-Dist: polars>=0.20.22
 Provides-Extra: dev
 Requires-Dist: ruff>=0.0.254; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
 
 <h1 align="center">Massive Text Embedding Benchmark</h1>
 
@@ -369,23 +370,26 @@
 
 ### Using a custom model
 
 Models should implement the following interface, implementing an `encode` function taking as inputs a list of sentences, and returning a list of embeddings (embeddings can be `np.array`, `torch.tensor`, etc.). For inspiration, you can look at the [mteb/mtebscripts repo](https://github.com/embeddings-benchmark/mtebscripts) used for running diverse models via SLURM scripts for the paper.
 
 ```python
 class MyModel():
-    def encode(self, sentences: list[str], **kwargs) -> list[np.ndarray] | list[torch.Tensor]:
-        """
-        Returns a list of embeddings for the given sentences.
-        
+    def encode(
+        self, sentences: list[str], prompt: str, **kwargs: Any
+    ) -> torch.Tensor | np.ndarray:
+        """Encodes the given sentences using the encoder.
+
         Args:
-            sentences: List of sentences to encode
+            sentences: The sentences to encode.
+            prompt: The prompt to use. Useful for prompt-based models.
+            **kwargs: Additional arguments to pass to the encoder.
 
         Returns:
-            List of embeddings for the given sentences
+            The encoded sentences.
         """
         pass
 
 model = MyModel()
 evaluation = MTEB(tasks=["Banking77Classification"])
 evaluation.run(model)
 ```
@@ -444,21 +448,23 @@
 
 | Documentation                          |                        |
 | ------------------------------ | ---------------------- |
 | 📋 [Tasks] | Overview of available tasks |
 | 📈 [Leaderboard] | The interactive leaderboard of the benchmark |
 | 🤖 [Adding a model] | Information related to how to submit a model to the leaderboard |
 | 👩‍💻 [Adding a dataset] | How to add a new task/dataset to MTEB | 
+| 👩‍💻 [Adding a leaderboard tab] | How to add a new leaderboard tab to MTEB | 
 | 🤝  [Contributing] | How to contribute to MTEB and set it up for development |
 <!-- | 🌐 [MMTEB] | An open-source effort to extend MTEB to cover a broad set of languages |   -->
 
 [Tasks]: docs/tasks.md
 [Contributing]: CONTRIBUTING.md
 [Adding a model]: docs/adding_a_model.md
 [Adding a dataset]: docs/adding_a_dataset.md
+[Adding a leaderboard tab]: docs/adding_a_leaderboard_tab.md
 [Leaderboard]: https://huggingface.co/spaces/mteb/leaderboard
 [MMTEB]: docs/mmteb/readme.md
 
 ## Citing
 
 MTEB was introduced in "[MTEB: Massive Text Embedding Benchmark](https://arxiv.org/abs/2210.07316)", feel free to cite:
 
@@ -474,9 +480,10 @@
 }
 ```
 
 You may also want to read and cite the amazing work that has extended MTEB & integrated new datasets:
 - Shitao Xiao, Zheng Liu, Peitian Zhang, Niklas Muennighoff. "[C-Pack: Packaged Resources To Advance General Chinese Embedding](https://arxiv.org/abs/2309.07597)" arXiv 2023
 - Michael Günther, Jackmin Ong, Isabelle Mohr, Alaeddine Abdessalem, Tanguy Abel, Mohammad Kalim Akram, Susana Guzman, Georgios Mastrapas, Saba Sturua, Bo Wang, Maximilian Werk, Nan Wang, Han Xiao. "[Jina Embeddings 2: 8192-Token General-Purpose Text Embeddings for Long Documents](https://arxiv.org/abs/2310.19923)" arXiv 2023
 - Silvan Wehrli, Bert Arnrich, Christopher Irrgang. "[German Text Embedding Clustering Benchmark](https://arxiv.org/abs/2401.02709)" arXiv 2024
+- Dawei Zhu, Liang Wang, Nan Yang, Yifan Song, Wenhao Wu, Furu Wei, and Sujian Li. "[LongEmbed: Extending Embedding Models for Long Context Retrieval](https://arxiv.org/abs/2404.12096)" arXiv 2024
 
 For works that have used MTEB for benchmarking, you can find them on the [leaderboard](https://huggingface.co/spaces/mteb/leaderboard).
```

### Comparing `mteb-1.7.9/README.md` & `mteb-1.8.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -129,23 +129,26 @@
 
 ### Using a custom model
 
 Models should implement the following interface, implementing an `encode` function taking as inputs a list of sentences, and returning a list of embeddings (embeddings can be `np.array`, `torch.tensor`, etc.). For inspiration, you can look at the [mteb/mtebscripts repo](https://github.com/embeddings-benchmark/mtebscripts) used for running diverse models via SLURM scripts for the paper.
 
 ```python
 class MyModel():
-    def encode(self, sentences: list[str], **kwargs) -> list[np.ndarray] | list[torch.Tensor]:
-        """
-        Returns a list of embeddings for the given sentences.
-        
+    def encode(
+        self, sentences: list[str], prompt: str, **kwargs: Any
+    ) -> torch.Tensor | np.ndarray:
+        """Encodes the given sentences using the encoder.
+
         Args:
-            sentences: List of sentences to encode
+            sentences: The sentences to encode.
+            prompt: The prompt to use. Useful for prompt-based models.
+            **kwargs: Additional arguments to pass to the encoder.
 
         Returns:
-            List of embeddings for the given sentences
+            The encoded sentences.
         """
         pass
 
 model = MyModel()
 evaluation = MTEB(tasks=["Banking77Classification"])
 evaluation.run(model)
 ```
@@ -204,21 +207,23 @@
 
 | Documentation                          |                        |
 | ------------------------------ | ---------------------- |
 | 📋 [Tasks] | Overview of available tasks |
 | 📈 [Leaderboard] | The interactive leaderboard of the benchmark |
 | 🤖 [Adding a model] | Information related to how to submit a model to the leaderboard |
 | 👩‍💻 [Adding a dataset] | How to add a new task/dataset to MTEB | 
+| 👩‍💻 [Adding a leaderboard tab] | How to add a new leaderboard tab to MTEB | 
 | 🤝  [Contributing] | How to contribute to MTEB and set it up for development |
 <!-- | 🌐 [MMTEB] | An open-source effort to extend MTEB to cover a broad set of languages |   -->
 
 [Tasks]: docs/tasks.md
 [Contributing]: CONTRIBUTING.md
 [Adding a model]: docs/adding_a_model.md
 [Adding a dataset]: docs/adding_a_dataset.md
+[Adding a leaderboard tab]: docs/adding_a_leaderboard_tab.md
 [Leaderboard]: https://huggingface.co/spaces/mteb/leaderboard
 [MMTEB]: docs/mmteb/readme.md
 
 ## Citing
 
 MTEB was introduced in "[MTEB: Massive Text Embedding Benchmark](https://arxiv.org/abs/2210.07316)", feel free to cite:
 
@@ -234,9 +239,10 @@
 }
 ```
 
 You may also want to read and cite the amazing work that has extended MTEB & integrated new datasets:
 - Shitao Xiao, Zheng Liu, Peitian Zhang, Niklas Muennighoff. "[C-Pack: Packaged Resources To Advance General Chinese Embedding](https://arxiv.org/abs/2309.07597)" arXiv 2023
 - Michael Günther, Jackmin Ong, Isabelle Mohr, Alaeddine Abdessalem, Tanguy Abel, Mohammad Kalim Akram, Susana Guzman, Georgios Mastrapas, Saba Sturua, Bo Wang, Maximilian Werk, Nan Wang, Han Xiao. "[Jina Embeddings 2: 8192-Token General-Purpose Text Embeddings for Long Documents](https://arxiv.org/abs/2310.19923)" arXiv 2023
 - Silvan Wehrli, Bert Arnrich, Christopher Irrgang. "[German Text Embedding Clustering Benchmark](https://arxiv.org/abs/2401.02709)" arXiv 2024
+- Dawei Zhu, Liang Wang, Nan Yang, Yifan Song, Wenhao Wu, Furu Wei, and Sujian Li. "[LongEmbed: Extending Embedding Models for Long Context Retrieval](https://arxiv.org/abs/2404.12096)" arXiv 2024
 
 For works that have used MTEB for benchmarking, you can find them on the [leaderboard](https://huggingface.co/spaces/mteb/leaderboard).
```

### Comparing `mteb-1.7.9/docs/mmteb/create_points_table.py` & `mteb-1.8.0/docs/mmteb/create_points_table.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/docs/mmteb/validate_points.py` & `mteb-1.8.0/docs/mmteb/validate_points.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/__init__.py` & `mteb-1.8.0/scripts/run_mteb_english.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,95 +1,120 @@
+"""Example script for benchmarking all datasets constituting the MTEB English leaderboard & average scores"""
+
 from __future__ import annotations
 
-from importlib.metadata import version
+import logging
+
+from sentence_transformers import SentenceTransformer
 
-from mteb.evaluation import *
+from mteb import MTEB
 
-__version__ = version("mteb")  # fetch version from install metadata
+logging.basicConfig(level=logging.INFO)
 
+logger = logging.getLogger("main")
 
-MTEB_MAIN_EN = [
+TASK_LIST_CLASSIFICATION = [
     "AmazonCounterfactualClassification",
     "AmazonPolarityClassification",
     "AmazonReviewsClassification",
-    "ArguAna",
+    "Banking77Classification",
+    "EmotionClassification",
+    "ImdbClassification",
+    "MassiveIntentClassification",
+    "MassiveScenarioClassification",
+    "MTOPDomainClassification",
+    "MTOPIntentClassification",
+    "ToxicConversationsClassification",
+    "TweetSentimentExtractionClassification",
+]
+
+TASK_LIST_CLUSTERING = [
     "ArxivClusteringP2P",
     "ArxivClusteringS2S",
-    "AskUbuntuDupQuestions",
-    "BIOSSES",
-    "Banking77Classification",
     "BiorxivClusteringP2P",
     "BiorxivClusteringS2S",
+    "MedrxivClusteringP2P",
+    "MedrxivClusteringS2S",
+    "RedditClustering",
+    "RedditClusteringP2P",
+    "StackExchangeClustering",
+    "StackExchangeClusteringP2P",
+    "TwentyNewsgroupsClustering",
+]
+
+TASK_LIST_PAIR_CLASSIFICATION = [
+    "SprintDuplicateQuestions",
+    "TwitterSemEval2015",
+    "TwitterURLCorpus",
+]
+
+TASK_LIST_RERANKING = [
+    "AskUbuntuDupQuestions",
+    "MindSmallReranking",
+    "SciDocsRR",
+    "StackOverflowDupQuestions",
+]
+
+TASK_LIST_RETRIEVAL = [
+    "ArguAna",
+    "ClimateFEVER",
     "CQADupstackAndroidRetrieval",
     "CQADupstackEnglishRetrieval",
     "CQADupstackGamingRetrieval",
     "CQADupstackGisRetrieval",
     "CQADupstackMathematicaRetrieval",
     "CQADupstackPhysicsRetrieval",
     "CQADupstackProgrammersRetrieval",
     "CQADupstackStatsRetrieval",
     "CQADupstackTexRetrieval",
     "CQADupstackUnixRetrieval",
     "CQADupstackWebmastersRetrieval",
     "CQADupstackWordpressRetrieval",
-    "ClimateFEVER",
     "DBPedia",
-    "EmotionClassification",
     "FEVER",
     "FiQA2018",
     "HotpotQA",
-    "ImdbClassification",
     "MSMARCO",
-    "MTOPDomainClassification",
-    "MTOPIntentClassification",
-    "MassiveIntentClassification",
-    "MassiveScenarioClassification",
-    "MedrxivClusteringP2P",
-    "MedrxivClusteringS2S",
-    "MindSmallReranking",
     "NFCorpus",
     "NQ",
     "QuoraRetrieval",
-    "RedditClustering",
-    "RedditClusteringP2P",
     "SCIDOCS",
+    "SciFact",
+    "Touche2020",
+    "TRECCOVID",
+]
+
+TASK_LIST_STS = [
+    "BIOSSES",
     "SICK-R",
     "STS12",
     "STS13",
     "STS14",
     "STS15",
     "STS16",
     "STS17",
     "STS22",
     "STSBenchmark",
-    "SciDocsRR",
-    "SciFact",
-    "SprintDuplicateQuestions",
-    "StackExchangeClustering",
-    "StackExchangeClusteringP2P",
-    "StackOverflowDupQuestions",
     "SummEval",
-    "TRECCOVID",
-    "Touche2020",
-    "ToxicConversationsClassification",
-    "TweetSentimentExtractionClassification",
-    "TwentyNewsgroupsClustering",
-    "TwitterSemEval2015",
-    "TwitterURLCorpus",
-]
-
-MTEB_RETRIEVAL_WITH_INSTRUCTIONS = [
-    "RobustInstructionRetrieval",
-    "NewsInstructionRetrieval",
-    "CoreInstructionRetrieval",
 ]
 
-MTEB_RETRIEVAL_LAW = [
-    "LegalSummarization",
-    "LegalBenchConsumerContractsQA",
-    "LegalBenchCorporateLobbying",
-    "AILACasedocs",
-    "AILAStatutes",
-    "LeCaRDv2",
-    "LegalQuAD",
-    "GerDaLIRSmall",
-]
+TASK_LIST = (
+    TASK_LIST_CLASSIFICATION
+    + TASK_LIST_CLUSTERING
+    + TASK_LIST_PAIR_CLASSIFICATION
+    + TASK_LIST_RERANKING
+    + TASK_LIST_RETRIEVAL
+    + TASK_LIST_STS
+)
+
+model_name = "average_word_embeddings_komninos"
+model = SentenceTransformer(model_name)
+
+for task in TASK_LIST:
+    logger.info(f"Running task: {task}")
+    eval_splits = ["dev"] if task == "MSMARCO" else ["test"]
+    evaluation = MTEB(
+        tasks=[task], task_langs=["en"]
+    )  # Remove "en" for running all languages
+    evaluation.run(
+        model, output_folder=f"results/{model_name}", eval_splits=eval_splits
+    )
```

### Comparing `mteb-1.7.9/mteb/abstasks/AbsTask.py` & `mteb-1.8.0/mteb/abstasks/AbsTaskSummarization.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,74 +1,71 @@
 from __future__ import annotations
 
-import random
-from abc import ABC, abstractmethod
+import logging
 
-import datasets
 import numpy as np
-import torch
 
-from mteb.abstasks.TaskMetadata import TaskMetadata
+from ..evaluation.evaluators import SummarizationEvaluator
+from .AbsTask import AbsTask
 
+logger = logging.getLogger(__name__)
 
-class AbsTask(ABC):
-    metadata: TaskMetadata
 
-    def __init__(self, seed=42, **kwargs):
-        self.dataset = None
-        self.data_loaded = False
-        self.is_multilingual = False
-        self.is_crosslingual = False
-        self.save_suffix = kwargs.get("save_suffix", "")
-
-        self.seed = seed
-        random.seed(self.seed)
-        np.random.seed(self.seed)
-        torch.manual_seed(self.seed)
-        torch.cuda.manual_seed_all(self.seed)
-
-    def dataset_transform(self):
-        """Transform operations applied to the dataset after loading.
-        Override this method if your dataset requires any transformation.
-        """
-        pass
-
-    def load_data(self, **kwargs):
-        """Load dataset from HuggingFace hub"""
-        if self.data_loaded:
-            return
-        self.dataset = datasets.load_dataset(**self.metadata_dict["dataset"])
-        self.dataset_transform()
-        self.data_loaded = True
+class AbsTaskSummarization(AbsTask):
+    """Abstract class for summarization experiments.
+
+    self.load_data() must generate a huggingface dataset with a split matching self.metadata_dict["eval_splits"], and assign it to self.dataset. It must contain the following columns:
+        text: str
+        human_summaries: list[str]
+        machine_summaries: list[str]
+        relevance: list[float] (the score of the machine generated summaries)
+    """
+
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
 
     @property
-    def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = dict(self.metadata)
-        return metadata_dict
-
-    @abstractmethod
-    def evaluate(self, model, split="test"):
-        """Evaluates a Sentence Embedding Model on the task.
-        Returns a dict (that can be serialized to json).
-        :param model: Sentence embedding method. Implements a encode(sentences) method, that encodes sentences
-        and returns a numpy matrix with the sentence embeddings
-        :param split: Which datasplit to be used.
-        """
-        raise NotImplementedError
+    def min_score(self):
+        return self.metadata_dict["min_score"]
 
     @property
-    def languages(self) -> set[str]:
-        """Returns the languages of the task"""
-        return self.metadata.languages
-
-    def __repr__(self) -> str:
-        """Format the representation of the task such that it appears as:
-
-        TaskObjectName(name='{name}', languages={lang1, lang2, ...})
-        """
-        langs = self.languages
-        if len(langs) > 3:
-            langs = list(langs)[:3]
-            langs.append("...")
-        return (
-            f"{self.__class__.__name__}(name='{self.metadata.name}', languages={langs})"
+    def max_score(self):
+        return self.metadata_dict["max_score"]
+
+    def evaluate(self, model, split, **kwargs):
+        if not self.data_loaded:
+            self.load_data()
+
+        if self.is_crosslingual:
+            scores = {}
+            for lang in self.dataset:
+                logger.info(
+                    f"\nTask: {self.metadata_dict['name']}, split: {split}, language: {lang}. Running..."
+                )
+                data_split = self.dataset[lang][split]
+                scores[lang] = self._evaluate_split(model, data_split, **kwargs)
+        else:
+            logger.info(
+                f"\nTask: {self.metadata_dict['name']}, split: {split}. Running..."
+            )
+            data_split = self.dataset[split]
+            scores = self._evaluate_split(model, data_split, **kwargs)
+
+        return scores
+
+    def _evaluate_split(self, model, data_split, **kwargs):
+        normalized_scores = list(
+            map(
+                lambda x: (np.array(x) - self.min_score)
+                / (self.max_score - self.min_score),
+                data_split["relevance"],
+            )
+        )
+        evaluator = SummarizationEvaluator(
+            machine_summaries=data_split["machine_summaries"],
+            human_summaries=data_split["human_summaries"],
+            texts=data_split["text"],
+            gold_scores=normalized_scores,
+            **kwargs,
         )
+        metrics = evaluator(model)
+        return metrics
```

### Comparing `mteb-1.7.9/mteb/abstasks/AbsTaskBitextMining.py` & `mteb-1.8.0/mteb/abstasks/AbsTaskBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/abstasks/AbsTaskClassification.py` & `mteb-1.8.0/mteb/abstasks/AbsTaskClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/abstasks/AbsTaskClustering.py` & `mteb-1.8.0/mteb/abstasks/AbsTaskClustering.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,8 +61,8 @@
                 cluster_set["sentences"], cluster_set["labels"], **kwargs
             )
             metrics = evaluator(model)
             v_measures.append(metrics["v_measure"])
 
         v_mean = np.mean(v_measures)
         v_std = np.std(v_measures)
-        return {"v_measure": v_mean, "v_measure_std": v_std}
+        return {"v_measure": v_mean, "v_measure_std": v_std, "v_measures": v_measures}
```

### Comparing `mteb-1.7.9/mteb/abstasks/AbsTaskInstructionRetrieval.py` & `mteb-1.8.0/mteb/abstasks/AbsTaskInstructionRetrieval.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,14 +241,16 @@
         qrels_file: str = "",
         streaming: bool = False,
         keep_in_memory: bool = False,
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.do_length_ablation = kwargs.get("do_length_ablation", False)
+        if self.do_length_ablation:
+            logger.info("Running length ablation also...")
 
     def load_data(self, **kwargs):
         if self.data_loaded:
             return
         self.corpus, self.queries, self.og_relevant_docs, self.changed_relevant_docs = (
             {},
             {},
@@ -282,24 +284,24 @@
             ]
             og_instructions = {
                 query["text"]: query["instruction_og"] for query in queries
             }
             changed_instructions = {
                 query["text"]: query["instruction_changed"] for query in queries
             }
-            queries = {query["id"]: query["text"] for query in queries}
-            corpus = {
-                doc["id"]: {"title": doc["title"], "text": doc["text"]}
-                for doc in corpus
-            }
             if self.do_length_ablation:
                 keywords = {query["text"]: query["keywords"] for query in queries}
                 short_instructions = {
                     query["text"]: query["short_query"] for query in queries
                 }
+            queries = {query["id"]: query["text"] for query in queries}
+            corpus = {
+                doc["id"]: {"title": doc["title"], "text": doc["text"]}
+                for doc in corpus
+            }
             assert (
                 len(top_ranked) == len(queries)
             ), f"Top ranked not loaded properly! Expected {len(self.queries)} but got {len(self.top_ranked)}."
 
             (
                 self.corpus[split],
                 self.queries[split],
@@ -467,15 +469,14 @@
             overall_changed_scores = utils.evaluate_change(
                 results_og, results_changed, newly_irrelevant_qrels
             )
 
             overall_changed_scores["individual"] = {
                 "original": scores_og,
                 "changed": scores_changed,
-                "base": scores_base,
             }
 
             if self.do_length_ablation:
                 keywords, short_instructions = (
                     self.keywords[split],
                     self.short_instructions[split],
                 )
@@ -532,15 +533,15 @@
         lang=None,
         **kwargs,
     ):
         start_time = time()
 
         # do the results by query and relevant docs only
         all_results = []
-        for query_id in tqdm.tqdm(list(queries.keys()), leave=True):
+        for query_id in tqdm.tqdm(list(queries.keys()), leave=False, desc="Retrieving"):
             cur_queries = {query_id: queries[query_id]}
             cur_instructions = {queries[query_id]: instructions[queries[query_id]]}
             cur_docs = {
                 key: value
                 for (key, value) in corpus.items()
                 if key in top_ranked[query_id]
             }
@@ -555,15 +556,15 @@
         results = {k: v for d in all_results for k, v in d.items()}
 
         end_time = time()
         logger.info(
             "Time taken to retrieve: {:.2f} seconds".format(end_time - start_time)
         )
 
-        if kwargs.get("save_qrels", False):
+        if kwargs.get("save_predictions", False):
             output_folder = kwargs.get("output_folder", "results")
             if not os.path.isdir(output_folder):
                 os.makedirs(output_folder)
             top_k = kwargs.get("top_k", None)
             if top_k is not None:
                 for qid in list(results.keys()):
                     doc_ids = set(
@@ -572,20 +573,18 @@
                         )[:top_k]
                     )
                     results[qid] = {
                         k: v for k, v in results[qid].items() if k in doc_ids
                     }
             if lang is None:
                 qrels_save_path = (
-                    f"{output_folder}/{self.metadata_dict['name']}_qrels.json"
+                    f"{output_folder}/{self.metadata_dict['name']}_predictions.json"
                 )
             else:
-                qrels_save_path = (
-                    f"{output_folder}/{self.metadata_dict['name']}_{lang}_qrels.json"
-                )
+                qrels_save_path = f"{output_folder}/{self.metadata_dict['name']}_{lang}_predictions.json"
 
             with open(qrels_save_path, "w") as f:
                 json.dump(results, f)
 
         ndcg, _map, recall, precision = retriever.evaluate(
             relevant_docs,
             results,
@@ -655,12 +654,15 @@
 def calculate_length_and_count(relevant_docs, queries, corpus, instructions):
     total_length = 0
     num_pairs = 0
     for query_id, docs in relevant_docs.items():
         query = queries[query_id]
         query += " " + instructions[query]
         for doc_id in docs:
+            # not relevant
+            if docs[doc_id] == 0:
+                continue
             doc = corpus[doc_id]
             doc_text = doc["title"] + doc["text"]
             total_length += len(query) + len(doc_text)
             num_pairs += 1
     return total_length, num_pairs
```

### Comparing `mteb-1.7.9/mteb/abstasks/AbsTaskPairClassification.py` & `mteb-1.8.0/mteb/abstasks/AbsTaskPairClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/abstasks/AbsTaskReranking.py` & `mteb-1.8.0/mteb/abstasks/AbsTaskReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/abstasks/AbsTaskRetrieval.py` & `mteb-1.8.0/mteb/abstasks/AbsTaskRetrieval.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,47 +242,47 @@
 
         self.data_loaded = True
 
     def evaluate(self, model, split="test", **kwargs):
         retriever = RetrievalEvaluator(model, **kwargs)
 
         scores = {}
-        if self.is_multilingual:
+        if self.is_crosslingual or self.is_multilingual:
             for lang in self.langs:
                 logger.info(f"Language: {lang}")
                 corpus, queries, relevant_docs = (
                     self.corpus[lang][split],
                     self.queries[lang][split],
                     self.relevant_docs[lang][split],
                 )
-                scores[lang] = self._evaluate_monolingual(
+                scores[lang] = self._evaluate_split(
                     retriever, corpus, queries, relevant_docs, lang, **kwargs
                 )
         else:
             corpus, queries, relevant_docs = (
                 self.corpus[split],
                 self.queries[split],
                 self.relevant_docs[split],
             )
-            scores = self._evaluate_monolingual(
+            scores = self._evaluate_split(
                 retriever, corpus, queries, relevant_docs, None, **kwargs
             )
         return scores
 
-    def _evaluate_monolingual(
+    def _evaluate_split(
         self, retriever, corpus, queries, relevant_docs, lang=None, **kwargs
     ):
         start_time = time()
         results = retriever(corpus, queries)
         end_time = time()
         logger.info(
             "Time taken to retrieve: {:.2f} seconds".format(end_time - start_time)
         )
 
-        if kwargs.get("save_qrels", False):
+        if kwargs.get("save_predictions", False):
             output_folder = kwargs.get("output_folder", "results")
             if not os.path.isdir(output_folder):
                 os.makedirs(output_folder)
             top_k = kwargs.get("top_k", None)
             if top_k is not None:
                 for qid in list(results.keys()):
                     doc_ids = set(
@@ -291,20 +291,18 @@
                         )[:top_k]
                     )
                     results[qid] = {
                         k: v for k, v in results[qid].items() if k in doc_ids
                     }
             if lang is None:
                 qrels_save_path = (
-                    f"{output_folder}/{self.metadata_dict['name']}_qrels.json"
+                    f"{output_folder}/{self.metadata_dict['name']}_predictions.json"
                 )
             else:
-                qrels_save_path = (
-                    f"{output_folder}/{self.metadata_dict['name']}_{lang}_qrels.json"
-                )
+                qrels_save_path = f"{output_folder}/{self.metadata_dict['name']}_{lang}_predictions.json"
 
             with open(qrels_save_path, "w") as f:
                 json.dump(results, f)
 
         ndcg, _map, recall, precision = retriever.evaluate(
             relevant_docs,
             results,
@@ -353,12 +351,15 @@
 
 def calculate_length_and_count(relevant_docs, queries, corpus):
     total_length = 0
     num_pairs = 0
     for query_id, docs in relevant_docs.items():
         query = queries[query_id]
         for doc_id in docs:
+            # not relevant
+            if docs[doc_id] == 0:
+                continue
             doc = corpus[doc_id]
             doc_text = doc["title"] + doc["text"]
             total_length += len(query) + len(doc_text)
             num_pairs += 1
     return total_length, num_pairs
```

### Comparing `mteb-1.7.9/mteb/abstasks/AbsTaskSTS.py` & `mteb-1.8.0/mteb/abstasks/AbsTaskSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/abstasks/AbsTaskSummarization.py` & `mteb-1.8.0/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,71 +1,96 @@
 from __future__ import annotations
 
-import logging
+import datasets
 
-import numpy as np
+from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ..evaluation.evaluators import SummarizationEvaluator
-from .AbsTask import AbsTask
+from ....abstasks import AbsTaskSTS, MultilingualTask
 
-logger = logging.getLogger(__name__)
-
-
-class AbsTaskSummarization(AbsTask):
-    """Abstract class for summarization experiments.
-
-    self.load_data() must generate a huggingface dataset with a split matching self.metadata_dict["eval_splits"], and assign it to self.dataset. It must contain the following columns:
-        text: str
-        human_summaries: list[str]
-        machine_summaries: list[str]
-        relevance: list[float] (the score of the machine generated summaries)
-    """
-
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-
-    @property
-    def min_score(self):
-        return self.metadata_dict["min_score"]
+_LANGUAGES = {
+    "en": ["eng-Latn"],
+    "de": ["deu-Latn"],
+    "es": ["spa-Latn"],
+    "fr": ["fra-Latn"],
+    "it": ["ita-Latn"],
+    "nl": ["nld-Latn"],
+    "pl": ["pol-Latn"],
+    "pt": ["por-Latn"],
+    "ru": ["rus-Cyrl"],
+    "zh": ["cmn-Hans"],
+}
+
+_SPLITS = ["dev", "test"]
+
+
+class STSBenchmarkMultilingualSTS(AbsTaskSTS, MultilingualTask):
+    metadata = TaskMetadata(
+        name="STSBenchmarkMultilingualSTS",
+        dataset={
+            "path": "PhilipMay/stsb_multi_mt",
+            "revision": "93d57ef91790589e3ce9c365164337a8a78b7632",
+        },
+        description=(
+            "Semantic Textual Similarity Benchmark (STSbenchmark) dataset,"
+            "but translated using DeepL API."
+        ),
+        reference="https://github.com/PhilipMay/stsb-multi-mt/",
+        type="STS",
+        category="s2s",
+        eval_splits=_SPLITS,
+        eval_langs=_LANGUAGES,
+        main_score="cosine_spearman",
+        date=None,
+        form=None,
+        domains=None,
+        task_subtypes=None,
+        license=None,
+        socioeconomic_status=None,
+        annotations_creators=None,
+        dialect=None,
+        text_creation=None,
+        bibtex_citation=None,
+        n_samples=None,
+        avg_character_length=None,
+    )
 
     @property
-    def max_score(self):
-        return self.metadata_dict["max_score"]
-
-    def evaluate(self, model, split, **kwargs):
-        if not self.data_loaded:
-            self.load_data()
-
-        if self.is_crosslingual:
-            scores = {}
-            for lang in self.dataset:
-                logger.info(
-                    f"\nTask: {self.metadata_dict['name']}, split: {split}, language: {lang}. Running..."
+    def metadata_dict(self) -> dict[str, str]:
+        metadata_dict = super().metadata_dict
+        metadata_dict["min_score"] = 0
+        metadata_dict["max_score"] = 5
+        return metadata_dict
+
+    def load_data(self, **kwargs):
+        if self.data_loaded:
+            return
+
+        def get_dataset_subset(lang: str):
+            """For a specified subset (=language)
+            only get the splits listed in _SPLIT
+            and rename column "score"
+
+            Args:
+                lang (str): _description_
+
+            Returns:
+                datasets.DatasetDict: the dataset of the specified language
+            """
+            subset = datasets.DatasetDict(
+                **dict(
+                    zip(
+                        _SPLITS,
+                        datasets.load_dataset(
+                            name=lang,
+                            split=_SPLITS,
+                            **self.metadata_dict["dataset"],
+                        ),
+                    )
                 )
-                data_split = self.dataset[lang][split]
-                scores[lang] = self._evaluate_split(model, data_split, **kwargs)
-        else:
-            logger.info(
-                f"\nTask: {self.metadata_dict['name']}, split: {split}. Running..."
             )
-            data_split = self.dataset[split]
-            scores = self._evaluate_split(model, data_split, **kwargs)
-
-        return scores
+            return subset.rename_column("similarity_score", "score")
 
-    def _evaluate_split(self, model, data_split, **kwargs):
-        normalized_scores = list(
-            map(
-                lambda x: (np.array(x) - self.min_score)
-                / (self.max_score - self.min_score),
-                data_split["relevance"],
-            )
+        self.dataset = datasets.DatasetDict(
+            **dict(zip(self.langs, [get_dataset_subset(lang) for lang in self.langs]))
         )
-        evaluator = SummarizationEvaluator(
-            machine_summaries=data_split["machine_summaries"],
-            human_summaries=data_split["human_summaries"],
-            texts=data_split["text"],
-            gold_scores=normalized_scores,
-            **kwargs,
-        )
-        metrics = evaluator(model)
-        return metrics
+
+        self.data_loaded = True
```

### Comparing `mteb-1.7.9/mteb/abstasks/LangMapping.py` & `mteb-1.8.0/mteb/abstasks/LangMapping.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/abstasks/TaskMetadata.py` & `mteb-1.8.0/mteb/abstasks/TaskMetadata.py`

 * *Files 8% similar despite different names*

```diff
@@ -106,15 +106,29 @@
 ]  # Allows the type to be a string, but ensures that the string is a valid date
 
 SPLIT_NAME = str
 # a 3-letter ISO 639-3 language code followed by a 4-letter ISO 15924 script code (e.g. "eng-Latn")
 ISO_LANGUAGE_SCRIPT = str
 LANGUAGES = Union[List[ISO_LANGUAGE_SCRIPT], Mapping[str, List[ISO_LANGUAGE_SCRIPT]]]
 
-PROGRAMMING_LANGS = ["python", "javascript", "go", "ruby", "java", "php"]
+PROGRAMMING_LANGS = [
+    "python",
+    "javascript",
+    "typescript",
+    "go",
+    "ruby",
+    "java",
+    "php",
+    "c",
+    "c++",
+    "rust",
+    "swift",
+    "scala",
+    "shell",
+]
 
 logger = logging.getLogger(__name__)
 
 
 class TaskMetadata(BaseModel):
     """Metadata for a task.
 
@@ -137,18 +151,18 @@
         domains: The domains of the data. These includes "Non-fiction", "Social", "Fiction", "News", "Academic", "Blog", "Encyclopaedic",
             "Government", "Legal", "Medical", "Poetry", "Religious", "Reviews", "Web", "Spoken". A dataset can belong to multiple domains.
         task_subtypes: The subtypes of the task. E.g. includes "Sentiment/Hate speech", "Thematic Clustering". Feel free to update the list as needed.
         license: The license of the data.
         socioeconomic_status: The socioeconomic status of the data. Includes "high", "medium", "low", "mixed".
         annotations_creators: The type of the annotators. Includes "expert-annotated" (annotated by experts), "human-annotated" (annotated e.g. by
             mturkers), "derived" (derived from structure in the data).
-        dialect: The dialect of the data, if applicable. Ideally specified as a BCP-47 language tag.
+        dialect: The dialect of the data, if applicable. Ideally specified as a BCP-47 language tag. Empty list if no dialects are present.
         text_creation: The method of text creation. Includes "found", "created", "machine-translated", "machine-translated and verified", and
             "machine-translated and localized".
-        bibtex_citation: The BibTeX citation for the dataset.
+        bibtex_citation: The BibTeX citation for the dataset. Should be an empty string if no citation is available.
         n_samples: The number of samples in the dataset. This should only be for the splits evaluated on. For retrieval tasks, this should be the
             number of query-document pairs.
         avg_character_length: The average character length of the samples in the dataset. This should only be for the splits evaluated on. For
             retrieval tasks, this should be the average character length of the query-document pairs.
     """
 
     dataset: dict
@@ -231,31 +245,41 @@
             )
         if script not in ISO_TO_SCRIPT:
             raise ValueError(
                 f"Invalid script code: {script}, you can find valid ISO 15924 codes in {path_to_lang_scripts}"
             )
 
     @property
-    def languages(self) -> set[str]:
+    def languages(self) -> list[str]:
         """Return the languages of the dataset as iso639-3 codes."""
 
         def get_lang(lang: str) -> str:
             return lang.split("-")[0]
 
         if isinstance(self.eval_langs, dict):
-            return set(
-                get_lang(lang) for langs in self.eval_langs.values() for lang in langs
+            return sorted(
+                set(
+                    get_lang(lang)
+                    for langs in self.eval_langs.values()
+                    for lang in langs
+                )
             )
-        return set(get_lang(lang) for lang in self.eval_langs)
+        return sorted(set([get_lang(lang) for lang in self.eval_langs]))
 
     @property
     def scripts(self) -> set[str]:
         """Return the scripts of the dataset as iso15924 codes."""
 
         def get_script(lang: str) -> str:
             return lang.split("-")[1]
 
         if isinstance(self.eval_langs, dict):
             return set(
                 get_script(lang) for langs in self.eval_langs.values() for lang in langs
             )
         return set(get_script(lang) for lang in self.eval_langs)
+
+    def is_filled(self) -> bool:
+        """Check if all the metadata fields are filled."""
+        return all(
+            getattr(self, field_name) is not None for field_name in self.model_fields
+        )
```

### Comparing `mteb-1.7.9/mteb/abstasks/iso_15924_to_script.json` & `mteb-1.8.0/mteb/abstasks/iso_15924_to_script.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/abstasks/iso_639_3_to_language.json` & `mteb-1.8.0/mteb/abstasks/iso_639_3_to_language.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/abstasks/languages.py` & `mteb-1.8.0/mteb/abstasks/languages.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/cmd.py` & `mteb-1.8.0/mteb/cmd.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/evaluation/MTEB.py` & `mteb-1.8.0/mteb/evaluation/MTEB.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,14 +253,17 @@
         if output_folder is not None:
             pathlib.Path(output_folder).mkdir(parents=True, exist_ok=True)
 
         # Run selected tasks
         logger.info(f"\n\n## Evaluating {len(self.tasks)} tasks:")
         self.print_selected_tasks()
         evaluation_results = {}
+        original_tasks = (
+            self.tasks.copy()
+        )  # save them in case we re-use the object (e.g. for reranking)
         while len(self.tasks) > 0:
             task = self.tasks[0]
             logger.info(
                 f"\n\n********************** Evaluating {task.metadata_dict['name']} **********************"
             )
 
             # skip evaluation if results folder exists and overwrite_results is False
@@ -281,14 +284,15 @@
                     eval_splits
                     if eval_splits is not None
                     else task.metadata_dict.get("eval_splits", [])
                 )
 
                 # load data
                 logger.info(f"Loading dataset for {task.metadata_dict['name']}")
+                task.check_if_dataset_is_superseeded()
                 task.load_data(eval_splits=task_eval_splits, **kwargs)
 
                 # run evaluation
                 task_results = {
                     "mteb_version": version("mteb"),  # noqa: F405
                     "dataset_revision": task.metadata_dict["dataset"].get(
                         "revision", None
@@ -329,8 +333,10 @@
                     f_out.write(f"{datetime.now()} >>> {task.metadata_dict['name']}\n")
                     f_out.write(traceback.format_exc())
                     f_out.write("\n\n")
 
             # empty memory
             del self.tasks[0]
 
+        # restore original tasks
+        self.tasks = original_tasks
         return evaluation_results
```

### Comparing `mteb-1.7.9/mteb/evaluation/evaluators/BitextMiningEvaluator.py` & `mteb-1.8.0/mteb/evaluation/evaluators/BitextMiningEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/evaluation/evaluators/ClassificationEvaluator.py` & `mteb-1.8.0/mteb/evaluation/evaluators/ClassificationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/evaluation/evaluators/ClusteringEvaluator.py` & `mteb-1.8.0/mteb/evaluation/evaluators/ClusteringEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/evaluation/evaluators/Evaluator.py` & `mteb-1.8.0/mteb/evaluation/evaluators/Evaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/evaluation/evaluators/InstructionRetrievalEvaluator.py` & `mteb-1.8.0/mteb/evaluation/evaluators/InstructionRetrievalEvaluator.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,15 +15,21 @@
         corpus: Dict[str, Dict[str, str]],
         queries: Dict[str, str],
         instructions: Dict[str, str],
         **kwargs,
     ) -> Dict[str, Dict[str, float]]:
         if not self.retriever:
             raise ValueError("Model/Technique has not been provided!")
-        return self.retriever.search(
-            corpus,
-            queries,
-            self.top_k,
-            self.score_function,
-            instructions=instructions,
-            **kwargs,
-        )
+
+        if self.is_cross_encoder:
+            return self.retriever.search_cross_encoder(
+                corpus, queries, self.top_k, instructions=instructions, **kwargs
+            )
+        else:
+            return self.retriever.search(
+                corpus,
+                queries,
+                self.top_k,
+                self.score_function,
+                instructions=instructions,
+                **kwargs,
+            )
```

### Comparing `mteb-1.7.9/mteb/evaluation/evaluators/PairClassificationEvaluator.py` & `mteb-1.8.0/mteb/evaluation/evaluators/PairClassificationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/evaluation/evaluators/RerankingEvaluator.py` & `mteb-1.8.0/mteb/evaluation/evaluators/RerankingEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/evaluation/evaluators/RetrievalEvaluator.py` & `mteb-1.8.0/mteb/evaluation/evaluators/RetrievalEvaluator.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,62 @@
 from __future__ import annotations
 
 import heapq
+import json
 import logging
+import os
 from collections import defaultdict
 from typing import Dict, List, Tuple
 
 import pytrec_eval
 import torch
-from sentence_transformers import SentenceTransformer
+import tqdm
+from sentence_transformers import CrossEncoder, SentenceTransformer
 from sentence_transformers.models import Transformer, WordEmbeddings
 
 from .Evaluator import Evaluator
-from .utils import cos_sim, dot_score, hole, mrr, recall_cap, top_k_accuracy
+from .utils import cos_sim, dot_score, download, hole, mrr, recall_cap, top_k_accuracy
 
 logger = logging.getLogger(__name__)
 
 
 # Adapted from https://github.com/beir-cellar/beir/blob/f062f038c4bfd19a8ca942a9910b1e0d218759d4/beir/retrieval/search/dense/exact_search.py#L12
 class DenseRetrievalExactSearch:
     def __init__(
-        self, model, batch_size: int = 128, corpus_chunk_size: int = 50000, **kwargs
+        self,
+        model,
+        batch_size: int = 128,
+        corpus_chunk_size: int = 50000,
+        previous_results: str = None,
+        **kwargs,
     ):
         # Model is class that provides encode_corpus() and encode_queries()
         self.model = model
         self.batch_size = batch_size
         self.score_functions = {"cos_sim": cos_sim, "dot": dot_score}
         self.score_function_desc = {
             "cos_sim": "Cosine Similarity",
             "dot": "Dot Product",
         }
         self.corpus_chunk_size = corpus_chunk_size
+        self.previous_results = previous_results
         self.show_progress_bar = kwargs.get("show_progress_bar", True)
         self.convert_to_tensor = kwargs.get("convert_to_tensor", True)
         self.save_corpus_embeddings = kwargs.get("save_corpus_embeddings", False)
         self.corpus_embeddings = defaultdict(list)
         self.results = {}
 
+        if self.previous_results is not None:
+            self.previous_results = self.load_results_file()
+
+        if isinstance(self.model, CrossEncoder):
+            # load the predict instance from the CrossEncoder
+            # custom functions can be used by extending the DenseRetrievalExactSearch class
+            self.predict = self.model.predict
+
     def search(
         self,
         corpus: dict[str, dict[str, str]],
         queries: dict[str, str],
         top_k: int,
         score_function: str,
         return_sorted: bool = False,
@@ -64,15 +81,14 @@
             batch_size=self.batch_size,
             show_progress_bar=self.show_progress_bar,
             convert_to_tensor=self.convert_to_tensor,
             **kwargs,
         )
 
         logger.info("Sorting Corpus by document length (Longest first)...")
-
         corpus_ids = sorted(
             corpus,
             key=lambda k: len(corpus[k].get("title", "") + corpus[k].get("text", "")),
             reverse=True,
         )
         corpus = [corpus[cid] for cid in corpus_ids]
 
@@ -150,130 +166,260 @@
 
         for qid in result_heaps:
             for score, corpus_id in result_heaps[qid]:
                 self.results[qid][corpus_id] = score
 
         return self.results
 
+    def load_results_file(self):
+        # load the first stage results from file in format {qid: {doc_id: score}}
+        if "https://" in self.previous_results:
+            # download the file
+            if not os.path.exists(self.previous_results):
+                url_descriptor = self.previous_results.split("https://")[-1].replace(
+                    "/", "--"
+                )
+                dest_file = os.path.join(
+                    "results", f"cached_predictions--{url_descriptor}"
+                )
+                os.makedirs(os.path.dirname(os.path.abspath(dest_file)), exist_ok=True)
+                download(self.previous_results, dest_file)
+                logger.info(
+                    f"Downloaded the previous results at {self.previous_results} to {dest_file}"
+                )
+            self.previous_results = dest_file
+
+        with open(self.previous_results, "r") as f:
+            previous_results = json.load(f)
+        assert isinstance(previous_results, dict)
+        assert isinstance(previous_results[list(previous_results.keys())[0]], dict)
+        return previous_results
+
+    def search_cross_encoder(
+        self,
+        corpus: Dict[str, Dict[str, str]],
+        queries: Dict[str, str],
+        top_k: int,
+        instructions: Dict[str, str] | None = None,
+        **kwargs,
+    ) -> Dict[str, Dict[str, float]]:
+        """This function provides support for reranker (or cross-encoder) models that encoder query and document at the same time (typically with attention).
+        Some notable examples include MonoBERT, MonoT5, RankLlama, etc.
+        Note: you must provide the path to the results to rerank to the __init__ function as `previous_results`
+        """
+        pairs = []  # create the pairs for reranking
+        for qid in queries.keys():
+            q_results = self.previous_results[qid]
+            # take the top-k only
+            q_results_sorted = {
+                k: v
+                for k, v in sorted(
+                    q_results.items(), key=lambda item: item[1], reverse=True
+                )
+            }
+            top_n = [k for k, v in list(q_results_sorted.items())[:top_k]]
+            query = queries[qid]
+            for doc_id in top_n:
+                corpus_item = (
+                    corpus[doc_id].get("title", "") + " " + corpus[doc_id]["text"]
+                ).strip()
+                pairs.append(
+                    (
+                        query,
+                        corpus_item,
+                        instructions[query] if instructions is not None else None,
+                        qid,
+                        doc_id,
+                    )
+                )
+
+        logger.info(f"Reranking the top {top_k} in batches... This might take a while!")
+        itr = range(0, len(pairs), self.batch_size)
+
+        results = {qid: {} for qid in queries.keys()}
+        for batch_num, corpus_start_idx in enumerate(
+            tqdm.tqdm(itr, leave=False, disable=not self.show_progress_bar)
+        ):
+            corpus_end_idx = min(corpus_start_idx + self.batch_size, len(pairs))
+            cur_batch = pairs[corpus_start_idx:corpus_end_idx]
+
+            (
+                queries_in_pair,
+                corpus_in_pair,
+                instructions_in_pair,
+                query_ids,
+                corpus_ids,
+            ) = zip(*cur_batch)
+
+            assert (
+                len(queries_in_pair) == len(corpus_in_pair) == len(instructions_in_pair)
+            )
+
+            if isinstance(self.model, CrossEncoder):
+                # can't take instructions, so add them here
+                queries_in_pair = [
+                    f"{q} {i}".strip()
+                    for i, q in zip(instructions_in_pair, queries_in_pair)
+                ]
+                scores = self.model.predict(list(zip(queries_in_pair, corpus_in_pair)))
+            else:
+                # may use the instructions in a unique way, so give them also
+                scores = self.model.predict(
+                    list(zip(queries_in_pair, corpus_in_pair, instructions_in_pair))
+                )
+
+            for i, score in enumerate(scores):
+                results[query_ids[i]][corpus_ids[i]] = float(score)
+
+        return results
+
+    def predict(self, queries, passages, **kwargs):
+        raise NotImplementedError(
+            "You must implement a predict method for your reranker model"
+        )
+
 
 class DRESModel:
     """Dense Retrieval Exact Search (DRES) requires an encode_queries & encode_corpus method.
     This class converts a model with just an .encode method into DRES format.
     """
 
-    def __init__(self, model, sep=" ", **kwargs):
+    def __init__(self, model, **kwargs):
         self.model = model
-        self.sep = sep
         self.use_sbert_model = isinstance(model, SentenceTransformer)
         self.save_corpus_embeddings = kwargs.get("save_corpus_embeddings", False)
         self.corpus_embeddings = {}
 
     def encode_queries(self, queries: List[str], batch_size: int, **kwargs):
         if self.use_sbert_model:
             if isinstance(self.model._first_module(), Transformer):
                 logger.info(
                     f"Queries will be truncated to {self.model.get_max_seq_length()} tokens."
                 )
             elif isinstance(self.model._first_module(), WordEmbeddings):
                 logger.warning(
                     "Queries will not be truncated. This could lead to memory issues. In that case please lower the batch_size."
                 )
-        return self.model.encode(queries, batch_size=batch_size, **kwargs)
+
+        if "instructions" in kwargs:
+            if kwargs["instructions"] is not None:
+                queries = [
+                    (query + " " + kwargs["instructions"][query]).strip()
+                    for query in queries
+                ]
+            new_kwargs = {
+                k: v for k, v in kwargs.items() if k not in ["instructions", "qid"]
+            }
+        else:
+            # can't just delete, cuz assign by reference on kwargs
+            new_kwargs = kwargs
+
+        return self.model.encode(queries, batch_size=batch_size, **new_kwargs)
 
     def encode_corpus(self, corpus: List[Dict[str, str]], batch_size: int, **kwargs):
         if (
             "qid" in kwargs
             and self.save_corpus_embeddings
             and len(self.corpus_embeddings) > 0
         ):
             return self.corpus_embeddings[kwargs["qid"]]
 
         if isinstance(corpus, dict):
             sentences = [
-                (corpus["title"][i] + self.sep + corpus["text"][i]).strip()
+                (corpus["title"][i] + " " + corpus["text"][i]).strip()
                 if "title" in corpus
                 else corpus["text"][i].strip()
                 for i in range(len(corpus["text"]))
             ]
         else:
             sentences = [
-                (doc["title"] + self.sep + doc["text"]).strip()
+                (doc["title"] + " " + doc["text"]).strip()
                 if "title" in doc
                 else doc["text"].strip()
                 for doc in corpus
             ]
 
+        if "instructions" in kwargs:  # not used on the doc side
+            new_kwargs = {
+                k: v for k, v in kwargs.items() if k not in ["instructions", "qid"]
+            }
+        else:
+            # can't just delete, cuz assign by reference on kwargs
+            new_kwargs = kwargs
+
         corpus_embeddings = self.model.encode(
-            sentences, batch_size=batch_size, **kwargs
+            sentences, batch_size=batch_size, **new_kwargs
         )
         if self.save_corpus_embeddings and "qid" in kwargs:
-            if type(corpus_embeddings) == torch.tensor:
+            if isinstance(corpus_embeddings, torch.tensor):
                 corpus_embeddings = corpus_embeddings.cpu().detach()
             self.corpus_embeddings[kwargs["qid"]] = corpus_embeddings
         return corpus_embeddings
 
+    def encode(self, sentences: List[str], **kwargs):
+        return self.model.encode(sentences, **kwargs)
+
 
 def is_dres_compatible(model):
     for method in ["encode_queries", "encode_corpus"]:
         op = getattr(model, method, None)
         if not (callable(op)):
             return False
     return True
 
 
+def is_cross_encoder_compatible(model):
+    op = getattr(model, "predict", None)
+    if not (callable(op)):
+        return False
+    return True
+
+
 # Adapted from https://github.com/beir-cellar/beir/blob/f062f038c4bfd19a8ca942a9910b1e0d218759d4/beir/retrieval/evaluation.py#L9
 class RetrievalEvaluator(Evaluator):
     def __init__(
         self,
         retriever=None,
         k_values: List[int] = [1, 3, 5, 10, 20, 100, 1000],
         score_function: str = "cos_sim",
         **kwargs,
     ):
         super().__init__(**kwargs)
-        if is_dres_compatible(retriever):
+        self.is_cross_encoder = False
+        if is_cross_encoder_compatible(retriever):
+            logger.info(
+                "The custom predict function of the model will be used if not a SentenceTransformer CrossEncoder"
+            )
+            self.retriever = DenseRetrievalExactSearch(retriever, **kwargs)
+            self.is_cross_encoder = True
+        elif is_dres_compatible(retriever):
             logger.info(
                 "The custom encode_queries and encode_corpus functions of the model will be used"
             )
             self.retriever = DenseRetrievalExactSearch(retriever, **kwargs)
         else:
             self.retriever = DenseRetrievalExactSearch(DRESModel(retriever), **kwargs)
         self.k_values = k_values
-        self.top_k = max(k_values)
+        self.top_k = (
+            max(k_values) if "top_k" not in kwargs else kwargs["top_k"]
+        )  # can lower it if reranking
         self.score_function = score_function
 
     def __call__(
-        self, corpus: dict[str, dict[str, str]], queries: dict[str, str], **kwargs
+        self, corpus: dict[str, dict[str, str]], queries: dict[str, str]
     ) -> dict[str, dict[str, float]]:
         if not self.retriever:
             raise ValueError("Model/Technique has not been provided!")
-        return self.retriever.search(
-            corpus, queries, self.top_k, self.score_function, **kwargs
-        )
 
-    def rerank(
-        self,
-        corpus: dict[str, dict[str, str]],
-        queries: dict[str, str],
-        results: dict[str, dict[str, float]],
-        top_k: int,
-    ) -> dict[str, dict[str, float]]:
-        new_corpus = {}
-
-        for query_id in results:
-            if len(results[query_id]) > top_k:
-                for doc_id, _ in sorted(
-                    results[query_id].items(), key=lambda item: item[1], reverse=True
-                )[:top_k]:
-                    new_corpus[doc_id] = corpus[doc_id]
-            else:
-                for doc_id in results[query_id]:
-                    new_corpus[doc_id] = corpus[doc_id]
-
-        return self.retriever.search(new_corpus, queries, top_k, self.score_function)
+        if self.is_cross_encoder:
+            return self.retriever.search_cross_encoder(corpus, queries, self.top_k)
+        else:
+            return self.retriever.search(
+                corpus, queries, self.top_k, self.score_function
+            )
 
     @staticmethod
     def evaluate(
         qrels: dict[str, dict[str, int]],
         results: dict[str, dict[str, float]],
         k_values: List[int],
         ignore_identical_ids: bool = True,
```

### Comparing `mteb-1.7.9/mteb/evaluation/evaluators/STSEvaluator.py` & `mteb-1.8.0/mteb/evaluation/evaluators/STSEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/evaluation/evaluators/SummarizationEvaluator.py` & `mteb-1.8.0/mteb/evaluation/evaluators/SummarizationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/evaluation/evaluators/utils.py` & `mteb-1.8.0/mteb/evaluation/evaluators/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 
 import logging
 from typing import Dict, List, Tuple
 
 import pandas as pd
+import requests
 import torch
+import tqdm
 
 
 def cos_sim(a, b):
     """Computes the cosine similarity cos_sim(a[i], b[j]) for all i and j.
 
     Return:
         Matrix with res[i][j]  = cos_sim(a[i], b[j])
@@ -242,7 +244,23 @@
 
 
 def rank_score(x: dict[str, float]) -> float:
     if x["og_rank"] >= x["new_rank"]:
         return ((1 / x["og_rank"]) / (1 / x["new_rank"])) - 1
     else:
         return 1 - ((1 / x["new_rank"]) / (1 / x["og_rank"]))
+
+
+# https://stackoverflow.com/a/62113293
+def download(url: str, fname: str):
+    resp = requests.get(url, stream=True)
+    total = int(resp.headers.get("content-length", 0))
+    with open(fname, "wb") as file, tqdm.tqdm(
+        desc=fname,
+        total=total,
+        unit="iB",
+        unit_scale=True,
+        unit_divisor=1024,
+    ) as bar:
+        for data in resp.iter_content(chunk_size=1024):
+            size = file.write(data)
+            bar.update(size)
```

### Comparing `mteb-1.7.9/mteb/logging.py` & `mteb-1.8.0/mteb/logging.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/BitextMining/__init__.py` & `mteb-1.8.0/mteb/tasks/BitextMining/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from __future__ import annotations
 
 from .dan.BornholmskBitextMining import *
+from .kat.TbilisiCityHallBitextMining import *
+from .multilingual.BibleNLPBitextMining import *
 from .multilingual.BUCCBitextMining import *
 from .multilingual.DiaBLaBitextMining import *
 from .multilingual.FloresBitextMining import *
 from .multilingual.IN22ConvBitextMining import *
 from .multilingual.IN22GenBitextMining import *
 from .multilingual.norwegian_courts_bitext_mining import *
 from .multilingual.NorwegianCourtsBitextMining import *
+from .multilingual.NTREXBitextMining import *
 from .multilingual.RomaTalesBitextMining import *
 from .multilingual.TatoebaBitextMining import *
+from .srn.SRNCorpusBitextMining import *
 from .vie.VieMedEVBitextMining import *
```

### Comparing `mteb-1.7.9/mteb/tasks/BitextMining/dan/BornholmskBitextMining.py` & `mteb-1.8.0/mteb/tasks/BitextMining/multilingual/norwegian_courts_bitext_mining.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-from __future__ import annotations
-
 from mteb.abstasks import AbsTaskBitextMining
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 
-class BornholmBitextMining(AbsTaskBitextMining):
+class NorwegianCourtsBitextMining(AbsTaskBitextMining):
     metadata = TaskMetadata(
-        name="BornholmBitextMining",
+        name="NorwegianCourtsBitextMining",
         dataset={
-            "path": "strombergnlp/bornholmsk_parallel",
-            "revision": "3bc5cfb4ec514264fe2db5615fac9016f7251552",
-            "trust_remote_code": True,
+            "path": "kardosdrur/norwegian-courts",
+            "revision": "d79af07e969a6678fcbbe819956840425816468f",
         },
-        description="Danish Bornholmsk Parallel Corpus. Bornholmsk is a Danish dialect spoken on the island of Bornholm, Denmark. Historically it is a part of east Danish which was also spoken in Scania and Halland, Sweden.",
-        reference="https://aclanthology.org/W19-6138/",
+        description="Nynorsk and Bokmål parallel corpus from Norwegian courts. ",
+        reference="https://opus.nlpl.eu/ELRC-Courts_Norway-v1.php",
         type="BitextMining",
         category="s2s",
         eval_splits=["test"],
-        eval_langs=["dan-Latn"],
-        main_score="f1",
-        date=None,
-        form=None,
-        domains=None,
-        license=None,
-        task_subtypes=None,
-        socioeconomic_status=None,
-        annotations_creators=None,
-        dialect=["da-dan-bornholm"],
-        text_creation=None,
+        eval_langs=["nno-Latn", "nob-Latn"],
+        main_score="accuracy",
+        date=("2000-01-01", "2020-12-31"),  # approximate guess
+        form=["spoken"],
+        domains=["Spoken", "Legal"],
+        task_subtypes=["Dialect pairing"],
+        license="openUnder-PSI",
+        socioeconomic_status="high",
+        annotations_creators="derived",  # best guess
+        dialect=[],
+        text_creation="found",
         bibtex_citation=None,
-        avg_character_length={"test": 89.7},
-        n_samples={"test": 500},
+        n_samples={"test": 456},
+        avg_character_length={"test": 82.11},
     )
 
-    def dataset_transform(self):
+    def dataset_transform(self) -> None:
         # Convert to standard format
-        self.dataset = self.dataset.rename_column("da", "sentence1")
-        self.dataset = self.dataset.rename_column("da_bornholm", "sentence2")
+        self.dataset = self.dataset.rename_column("nb", "sentence1")
+        self.dataset = self.dataset.rename_column("nn", "sentence2")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mteb-1.7.9/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py` & `mteb-1.8.0/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py` & `mteb-1.8.0/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py` & `mteb-1.8.0/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/BitextMining/multilingual/IN22ConvBitextMining.py` & `mteb-1.8.0/mteb/tasks/BitextMining/multilingual/IN22ConvBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/BitextMining/multilingual/IN22GenBitextMining.py` & `mteb-1.8.0/mteb/tasks/BitextMining/multilingual/IN22GenBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py` & `mteb-1.8.0/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/BitextMining/multilingual/RomaTalesBitextMining.py` & `mteb-1.8.0/mteb/tasks/BitextMining/multilingual/RomaTalesBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py` & `mteb-1.8.0/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,19 +117,20 @@
     "fin-eng": ["fin-Latn", "eng-Latn"],
     "tha-eng": ["tha-Thai", "eng-Latn"],
     "wuu-eng": ["wuu-Hans", "eng-Latn"],
 }
 
 
 class TatoebaBitextMining(AbsTaskBitextMining, CrosslingualTask):
+    fast_loading = True
     metadata = TaskMetadata(
         name="Tatoeba",
         dataset={
             "path": "mteb/tatoeba-bitext-mining",
-            "revision": "9080400076fbadbb4c4dcb136ff4eddc40b42553",
+            "revision": "69e8f12da6e31d59addadda9a9c8a2e601a0e282",
         },
         description="1,000 English-aligned sentence pairs for each language based on the Tatoeba corpus",
         reference="https://github.com/facebookresearch/LASER/tree/main/data/tatoeba/v1",
         type="BitextMining",
         category="s2s",
         eval_splits=["test"],
         eval_langs=_LANGUAGES,
```

### Comparing `mteb-1.7.9/mteb/tasks/BitextMining/multilingual/norwegian_courts_bitext_mining.py` & `mteb-1.8.0/mteb/tasks/Classification/pan/PunjabiNewsClassification.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,38 @@
-from mteb.abstasks import AbsTaskBitextMining
+from __future__ import annotations
+
+from mteb.abstasks import AbsTaskClassification
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 
-class NorwegianCourtsBitextMining(AbsTaskBitextMining):
+class PunjabiNewsClassification(AbsTaskClassification):
     metadata = TaskMetadata(
-        name="NorwegianCourtsBitextMining",
+        name="PunjabiNewsClassification",
+        description="A Punjabi dataset for 2-class classification of Punjabi news articles",
+        reference="https://github.com/goru001/nlp-for-punjabi/",
         dataset={
-            "path": "kardosdrur/norwegian-courts",
-            "revision": "d79af07e969a6678fcbbe819956840425816468f",
+            "path": "mlexplorer008/punjabi_news_classification",
+            "revision": "cec3923e16519efe51d535497e711932b8f1dc44",
         },
-        description="Nynorsk and Bokmål parallel corpus from Norwegian courts. ",
-        reference="https://opus.nlpl.eu/ELRC-Courts_Norway-v1.php",
-        type="BitextMining",
+        type="Classification",
         category="s2s",
+        date=("2014-01-01", "2018-01-01"),
         eval_splits=["test"],
-        eval_langs=["nno-Latn", "nob-Latn"],
+        eval_langs=["pan-Guru"],
         main_score="accuracy",
-        date=("2000-01-01", "2020-12-31"),  # approximate guess
-        form=["spoken"],
-        domains=["Spoken", "Legal"],
-        task_subtypes=["Dialect pairing"],
-        license="openUnder-PSI",
-        socioeconomic_status="high",
-        annotations_creators="derived",  # best guess
+        form=["written"],
+        domains=["News"],
+        task_subtypes=["Topic classification"],
+        license="MIT",
+        socioeconomic_status="mixed",
+        annotations_creators="derived",
         dialect=[],
         text_creation="found",
         bibtex_citation=None,
-        n_samples={"test": 456},
-        avg_character_length={"test": 82.11},
+        n_samples={"train": 627, "test": 157},
+        avg_character_length={"train": 4222.22, "test": 4115.14},
     )
 
-    def dataset_transform(self) -> None:
-        # Convert to standard format
-        self.dataset = self.dataset.rename_column("nb", "sentence1")
-        self.dataset = self.dataset.rename_column("nn", "sentence2")
+    def dataset_transform(self):
+        self.dataset = self.dataset.rename_columns(
+            {"article": "text", "is_about_politics": "label"}
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mteb-1.7.9/mteb/tasks/BitextMining/vie/VieMedEVBitextMining.py` & `mteb-1.8.0/mteb/tasks/BitextMining/vie/VieMedEVBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Classification/ara/HotelReviewSentimentClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/ara/HotelReviewSentimentClassification.py`

 * *Files 11% similar despite different names*

```diff
@@ -40,10 +40,10 @@
 }
 """,
         n_samples={"train": N_SAMPLES},
         avg_character_length={"train": 137.2},
     )
 
     def dataset_transform(self):
-        self.dataset["train"] = (
-            self.dataset["train"].shuffle(seed=self.seed).select(range(N_SAMPLES))
+        self.dataset = self.stratified_subsampling(
+            self.dataset, seed=self.seed, splits=["train"]
         )
```

### Comparing `mteb-1.7.9/mteb/tasks/Classification/ara/RestaurantReviewSentimentClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/ara/RestaurantReviewSentimentClassification.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,10 +42,10 @@
         n_samples={"train": N_SAMPLES},
         avg_character_length={"train": 231.4},
     )
 
     def dataset_transform(self):
         # labels: 0 negative, 1 positive
         self.dataset = self.dataset.rename_column("polarity", "label")
-        self.dataset["train"] = (
-            self.dataset["train"].shuffle(seed=self.seed).select(range(N_SAMPLES))
+        self.dataset = self.stratified_subsampling(
+            self.dataset, seed=self.seed, splits=["train"]
         )
```

### Comparing `mteb-1.7.9/mteb/tasks/Classification/ara/TweetEmotionClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/ara/TweetEmotionClassification.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,10 +41,10 @@
 """,
         n_samples={"train": N_SAMPLES},
         avg_character_length={"train": 78.8},
     )
 
     def dataset_transform(self):
         self.dataset = self.dataset.rename_column("tweet", "text")
-        self.dataset["train"] = (
-            self.dataset["train"].shuffle(seed=self.seed).select(range(N_SAMPLES))
+        self.dataset = self.stratified_subsampling(
+            self.dataset, seed=self.seed, splits=["train"]
         )
```

### Comparing `mteb-1.7.9/mteb/tasks/Classification/ara/TweetSarcasmClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/ara/TweetSarcasmClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Classification/bam/BambaraSentimentClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/kat/GeorgianSentimentClassification.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,61 @@
 from __future__ import annotations
 
 from mteb.abstasks import AbsTaskClassification
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 
-class BambaraSentimentClassification(AbsTaskClassification):
+class GeorgianSentimentClassification(AbsTaskClassification):
     metadata = TaskMetadata(
-        name="BambaraSentimentClassification",
-        description="An Bambara dataset for sentiment classification.",
-        reference="https://arxiv.org/abs/2009.08712",
+        name="GeorgianSentimentClassification",
+        description="Goergian Sentiment Dataset",
+        reference="https://aclanthology.org/2022.lrec-1.173",
         dataset={
-            "path": "sepidmnorozy/Bambara_sentiment",
-            "revision": "abdd077d23df1170c9fa1098cf93c83f6ae1217c",
+            "path": "asparius/Georgian-Sentiment",
+            "revision": "d4fb68dff38e89c42406080737b8431ea48fa866",
         },
         type="Classification",
         category="s2s",
-        date=("2022-01-01", "2022-01-01"),
         eval_splits=["test"],
-        eval_langs=["mlt-Latn"],
+        eval_langs=["kat-Geor"],
         main_score="accuracy",
+        date=("2022-01-01", "2022-06-25"),
         form=["written"],
         domains=["Reviews"],
         task_subtypes=["Sentiment/Hate speech"],
-        license="Not specified",
+        license="CC BY 4.0",
         socioeconomic_status="mixed",
-        annotations_creators="human-annotated",
+        annotations_creators="derived",
         dialect=[],
         text_creation="found",
-        bibtex_citation="""@inproceedings{mollanorozy-etal-2023-cross,
-    title = "Cross-lingual Transfer Learning with \{P\}ersian",
-    author = "Mollanorozy, Sepideh  and
-      Tanti, Marc  and
-      Nissim, Malvina",
-    editor = "Beinborn, Lisa  and
-      Goswami, Koustava  and
-      Murado{\\u{g}}lu, Saliha  and
-      Sorokin, Alexey  and
-      Kumar, Ritesh  and
-      Shcherbakov, Andreas  and
-      Ponti, Edoardo M.  and
-      Cotterell, Ryan  and
-      Vylomova, Ekaterina",
-    booktitle = "Proceedings of the 5th Workshop on Research in Computational Linguistic Typology and Multilingual NLP",
-    month = may,
-    year = "2023",
-    address = "Dubrovnik, Croatia",
-    publisher = "Association for Computational Linguistics",
-    url = "https://aclanthology.org/2023.sigtyp-1.9",
-    doi = "10.18653/v1/2023.sigtyp-1.9",
-    pages = "89--95",
+        bibtex_citation="""
+        @inproceedings{stefanovitch-etal-2022-resources,
+    title = "Resources and Experiments on Sentiment Classification for {G}eorgian",
+    author = "Stefanovitch, Nicolas  and
+      Piskorski, Jakub  and
+      Kharazi, Sopho",
+    editor = "Calzolari, Nicoletta  and
+      B{\'e}chet, Fr{\'e}d{\'e}ric  and
+      Blache, Philippe  and
+      Choukri, Khalid  and
+      Cieri, Christopher  and
+      Declerck, Thierry  and
+      Goggi, Sara  and
+      Isahara, Hitoshi  and
+      Maegaard, Bente  and
+      Mariani, Joseph  and
+      Mazo, H{\'e}l{\`e}ne  and
+      Odijk, Jan  and
+      Piperidis, Stelios",
+    booktitle = "Proceedings of the Thirteenth Language Resources and Evaluation Conference",
+    month = jun,
+    year = "2022",
+    address = "Marseille, France",
+    publisher = "European Language Resources Association",
+    url = "https://aclanthology.org/2022.lrec-1.173",
+    pages = "1613--1621",
+    abstract = "This paper presents, to the best of our knowledge, the first ever publicly available annotated dataset for sentiment classification and semantic polarity dictionary for Georgian. The characteristics of these resources and the process of their creation are described in detail. The results of various experiments on the performance of both lexicon- and machine learning-based models for Georgian sentiment classification are also reported. Both 3-label (positive, neutral, negative) and 4-label settings (same labels + mixed) are considered. The machine learning models explored include, i.a., logistic regression, SVMs, and transformed-based models. We also explore transfer learning- and translation-based (to a well-supported language) approaches. The obtained results for Georgian are on par with the state-of-the-art results in sentiment classification for well studied languages when using training data of comparable size.",
 }
-""",
-        n_samples={"test": 673},
-        avg_character_length={"test": 29.4},
+        """,
+        n_samples={"train": 330, "test": 1200},
+        avg_character_length={"train": 114.26, "test": 118.06},
     )
```

### Comparing `mteb-1.7.9/mteb/tasks/Classification/ben/BengaliHateSpeechClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/ben/BengaliHateSpeechClassification.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,8 +36,10 @@
 }
 """,
         n_samples={"train": 3418},
         avg_character_length={"train": 103.42},
     )
 
     def dataset_transform(self):
-        self.dataset["train"] = self.dataset["train"].select(range(2048))
+        self.dataset = self.stratified_subsampling(
+            self.dataset, seed=self.seed, splits=["train"]
+        )
```

### Comparing `mteb-1.7.9/mteb/tasks/Classification/bul/BulgarianSentimentClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/spa/SpanishSentimentClassification.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 from __future__ import annotations
 
 from mteb.abstasks import AbsTaskClassification
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 
-class BulgarianSentimentClassification(AbsTaskClassification):
+class SpanishSentimentClassification(AbsTaskClassification):
     metadata = TaskMetadata(
-        name="BulgarianSentimentClassification",
-        description="An Bulgarian dataset for sentiment classification.",
-        reference="https://arxiv.org/abs/2009.08712",
+        name="SpanishSentimentClassification",
+        description="A Spanish dataset for sentiment classification.",
+        reference="https://huggingface.co/datasets/sepidmnorozy/Spanish_sentiment",
         dataset={
-            "path": "sepidmnorozy/Bulgarian_sentiment",
-            "revision": "c0d5c781a115d570b8acceb14928ffb99543bb74",
+            "path": "sepidmnorozy/Spanish_sentiment",
+            "revision": "2a6e340e4b59b7c0a78c03a0b79ac27e1b4a2662",
         },
         type="Classification",
         category="s2s",
-        date=("2022-01-01", "2022-01-01"),
+        date=("2022-08-16", "2022-08-16"),
         eval_splits=["validation", "test"],
-        eval_langs=["bul-Cyrl"],
+        eval_langs=["spa-Latn"],
         main_score="accuracy",
         form=["written"],
         domains=["Reviews"],
         task_subtypes=["Sentiment/Hate speech"],
         license="Not specified",
         socioeconomic_status="mixed",
-        annotations_creators="human-annotated",
+        annotations_creators="derived",
         dialect=[],
         text_creation="found",
-        bibtex_citation="""@inproceedings{mollanorozy-etal-2023-cross,
-    title = "Cross-lingual Transfer Learning with \{P\}ersian",
-    author = "Mollanorozy, Sepideh  and
-      Tanti, Marc  and
-      Nissim, Malvina",
-    editor = "Beinborn, Lisa  and
-      Goswami, Koustava  and
-      Murado{\\u{g}}lu, Saliha  and
-      Sorokin, Alexey  and
-      Kumar, Ritesh  and
-      Shcherbakov, Andreas  and
-      Ponti, Edoardo M.  and
-      Cotterell, Ryan  and
-      Vylomova, Ekaterina",
-    booktitle = "Proceedings of the 5th Workshop on Research in Computational Linguistic Typology and Multilingual NLP",
-    month = may,
-    year = "2023",
-    address = "Dubrovnik, Croatia",
-    publisher = "Association for Computational Linguistics",
-    url = "https://aclanthology.org/2023.sigtyp-1.9",
-    doi = "10.18653/v1/2023.sigtyp-1.9",
-    pages = "89--95",
-}
-""",
-        n_samples={"validation": 838, "test": 1673},
-        avg_character_length={"validation": 43.3, "test": 46.3},
+        bibtex_citation="""
+        @inproceedings{mollanorozy-etal-2023-cross,
+            title = "Cross-lingual Transfer Learning with \{P\}ersian",
+            author = "Mollanorozy, Sepideh  and
+            Tanti, Marc  and
+            Nissim, Malvina",
+            editor = "Beinborn, Lisa  and
+            Goswami, Koustava  and
+            Murado{\\u{g}}lu, Saliha  and
+            Sorokin, Alexey  and
+            Kumar, Ritesh  and
+            Shcherbakov, Andreas  and
+            Ponti, Edoardo M.  and
+            Cotterell, Ryan  and
+            Vylomova, Ekaterina",
+            booktitle = "Proceedings of the 5th Workshop on Research in Computational Linguistic Typology and Multilingual NLP",
+            month = may,
+            year = "2023",
+            address = "Dubrovnik, Croatia",
+            publisher = "Association for Computational Linguistics",
+            url = "https://aclanthology.org/2023.sigtyp-1.9",
+            doi = "10.18653/v1/2023.sigtyp-1.9",
+            pages = "89--95",
+        }
+        """,
+        n_samples={"validation": 147, "test": 296},
+        avg_character_length={"validation": 85.02, "test": 87.91},
     )
```

### Comparing `mteb-1.7.9/mteb/tasks/Classification/bul/BulgarianStoreReviewSentimentClassfication.py` & `mteb-1.8.0/mteb/tasks/Classification/bul/BulgarianStoreReviewSentimentClassfication.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Classification/ces/CzechSubjectivityClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/ces/CzechSubjectivityClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Classification/dan/AngryTweetsClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/eng/ToxicConversationsClassification.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,46 @@
 from __future__ import annotations
 
-from mteb.abstasks.AbsTaskClassification import AbsTaskClassification
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
+from ....abstasks import AbsTaskClassification
 
-class AngryTweetsClassification(AbsTaskClassification):
+
+class ToxicConversationsClassification(AbsTaskClassification):
     metadata = TaskMetadata(
-        name="AngryTweetsClassification",
+        name="ToxicConversationsClassification",
+        description="Collection of comments from the Civil Comments platform together with annotations if the comment is toxic or not.",
+        reference="https://www.kaggle.com/competitions/jigsaw-unintended-bias-in-toxicity-classification/overview",
         dataset={
-            "path": "DDSC/angry-tweets",
-            "revision": "20b0e6081892e78179356fada741b7afa381443d",
+            "path": "mteb/toxic_conversations_50k",
+            "revision": "edfaf9da55d3dd50d43143d90c1ac476895ae6de",
         },
-        description="A sentiment dataset with 3 classes (positiv, negativ, neutral) for Danish tweets",
-        reference="https://aclanthology.org/2021.nodalida-main.53/",
         type="Classification",
         category="s2s",
         eval_splits=["test"],
-        eval_langs=["dan-Latn"],
+        eval_langs=["eng-Latn"],
         main_score="accuracy",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples={"test": 1050},
-        avg_character_length={"test": 156.1},
+        n_samples={"test": 50000},
+        avg_character_length={"test": 296.6},
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
         metadata_dict = super().metadata_dict
         metadata_dict["n_experiments"] = 10
         metadata_dict["samples_per_label"] = 16
         return metadata_dict
+
+    def dataset_transform(self):
+        self.dataset = self.stratified_subsampling(
+            self.dataset, seed=self.seed, splits=["test"]
+        )
```

### Comparing `mteb-1.7.9/mteb/tasks/Classification/dan/DKHateClassification.py` & `mteb-1.8.0/mteb/tasks/STS/eng/STS14STS.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,41 @@
 from __future__ import annotations
 
-from mteb.abstasks.AbsTaskClassification import AbsTaskClassification
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
+from ....abstasks.AbsTaskSTS import AbsTaskSTS
 
-class DKHateClassification(AbsTaskClassification):
+
+class STS14STS(AbsTaskSTS):
     metadata = TaskMetadata(
-        name="DKHateClassification",
+        name="STS14",
         dataset={
-            "path": "DDSC/dkhate",
-            "revision": "59d12749a3c91a186063c7d729ec392fda94681c",
+            "path": "mteb/sts14-sts",
+            "revision": "6031580fec1f6af667f0bd2da0a551cf4f0b2375",
         },
-        description="Danish Tweets annotated for Hate Speech either being Offensive or not",
-        reference="https://aclanthology.org/2020.lrec-1.430/",
-        type="Classification",
+        description="SemEval STS 2014 dataset. Currently only the English dataset",
+        reference="https://www.aclweb.org/anthology/S14-1002",
+        type="STS",
         category="s2s",
         eval_splits=["test"],
-        eval_langs=["dan-Latn"],
-        main_score="accuracy",
+        eval_langs=["eng-Latn"],
+        main_score="cosine_spearman",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples={"test": 329},
-        avg_character_length={"test": 104.0},
+        n_samples=None,
+        avg_character_length=None,
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = dict(self.metadata)
-        metadata_dict["n_experiments"] = 10
-        metadata_dict["samples_per_label"] = 16
+        metadata_dict = super().metadata_dict
+        metadata_dict["min_score"] = 0
+        metadata_dict["max_score"] = 5
         return metadata_dict
-
-    def dataset_transform(self):
-        # convert label to a 0/1 label
-        labels = self.dataset["train"]["label"]  # type: ignore
-        lab2idx = {lab: idx for idx, lab in enumerate(set(labels))}
-        self.dataset = self.dataset.map(
-            lambda x: {"label": lab2idx[x["label"]]}, remove_columns=["label"]
-        )
```

### Comparing `mteb-1.7.9/mteb/tasks/Classification/dan/DalajClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/eng/ToxicChatClassification.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,68 +1,67 @@
-# SuperLIM tasks
 from __future__ import annotations
 
 from mteb.abstasks import AbsTaskClassification
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
+_EVAL_SPLITS = ["test"]
 
-class DalajClassification(AbsTaskClassification):
+
+class ToxicChatClassification(AbsTaskClassification):
     metadata = TaskMetadata(
-        name="DalajClassification",
+        name="ToxicChatClassification",
+        description="""This dataset contains toxicity annotations on 10K user
+            prompts collected from the Vicuna online demo. We utilize a human-AI
+            collaborative annotation framework to guarantee the quality of annotation
+            while maintaining a feasible annotation workload. The details of data
+            collection, pre-processing, and annotation can be found in our paper.
+            We believe that ToxicChat can be a valuable resource to drive further
+            advancements toward building a safe and healthy environment for user-AI
+            interactions.
+            Only human annotated samples are selected here.""",
+        reference="https://aclanthology.org/2023.findings-emnlp.311/",
         dataset={
-            "path": "AI-Sweden/SuperLim",
-            "revision": "7ebf0b4caa7b2ae39698a889de782c09e6f5ee56",
-            "name": "dalaj",
+            "path": "lmsys/toxic-chat",
+            "name": "toxicchat0124",
+            "revision": "3e0319203c7162b9c9f8015b594441f979c199bc",
         },
-        description="A Swedish dataset for linguistic acceptability. Available as a part of Superlim.",
-        reference="https://spraakbanken.gu.se/en/resources/superlim",
         type="Classification",
         category="s2s",
-        eval_splits=["test"],
-        eval_langs=["dan-Latn"],
+        eval_splits=_EVAL_SPLITS,
+        eval_langs=["eng-Latn"],
         main_score="accuracy",
-        date=None,
-        form=None,
-        domains=None,
-        task_subtypes=None,
-        license=None,
-        socioeconomic_status=None,
-        annotations_creators=None,
-        dialect=None,
-        text_creation=None,
-        bibtex_citation=None,
-        n_samples={"test": 444},
-        avg_character_length={"test": 243.8},
+        date=("2023-10-26", "2024-01-31"),
+        form=["written"],
+        domains=["Constructed"],
+        task_subtypes=["Sentiment/Hate speech"],
+        license="cc-by-4.0",
+        socioeconomic_status="high",
+        annotations_creators="expert-annotated",
+        dialect=[],
+        text_creation="found",
+        bibtex_citation="""@misc{lin2023toxicchat,
+            title={ToxicChat: Unveiling Hidden Challenges of Toxicity Detection in Real-World User-AI Conversation},
+            author={Zi Lin and Zihan Wang and Yongqi Tong and Yangkun Wang and Yuxin Guo and Yujia Wang and Jingbo Shang},
+            year={2023},
+            eprint={2310.17389},
+            archivePrefix={arXiv},
+            primaryClass={cs.CL}
+        }""",
+        n_samples={"test": 1427},
+        avg_character_length={"test": 189.4},
     )
 
-    @property
-    def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = super().metadata_dict
-        metadata_dict["n_experiments"] = 10
-        metadata_dict["samples_per_label"] = 16
-        return metadata_dict
-
     def dataset_transform(self):
-        """This dataset consist of two columns of relevance, "original_sentence" and "corrected_sentence".
-        We will use the original sentence as we "wrong" sentence and the corrected sentence as the "correct" sentence
-        """
-
-        def __convert_sample_to_classification(sample):
-            text = sample["original_sentence"] + sample["corrected_sentence"]
-            label = [1] * len(sample["original_sentence"]) + [0] * len(
-                sample["corrected_sentence"]
-            )
-            return {"text": text, "label": label}
-
-        columns_to_keep = ["original_sentence", "corrected_sentence"]
-        for split in self.dataset:
-            columns_names = self.dataset[split].column_names  # type: ignore
-            columns_to_remove = [
-                col for col in columns_names if col not in columns_to_keep
-            ]
-            self.dataset[split] = self.dataset[split].remove_columns(columns_to_remove)  # type: ignore
-
-        self.dataset = self.dataset.map(
-            __convert_sample_to_classification,
-            batched=True,
-            remove_columns=columns_to_keep,
+        keep_cols = ["user_input", "toxicity"]
+        rename_dict = dict(zip(keep_cols, ["text", "label"]))
+        remove_cols = [
+            col
+            for col in self.dataset[_EVAL_SPLITS[0]].column_names
+            if col not in keep_cols
+        ]
+        self.dataset = self.dataset.rename_columns(rename_dict)
+        self.dataset = self.stratified_subsampling(
+            self.dataset, seed=self.seed, splits=["test"]
         )
+        # only use human-annotated data
+        self.dataset = self.dataset.filter(lambda x: x["human_annotation"])
+        self.dataset = self.dataset.remove_columns(remove_cols)
```

### Comparing `mteb-1.7.9/mteb/tasks/Classification/dan/DanishPoliticalCommentsClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/dan/DanishPoliticalCommentsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Classification/dan/DdiscoCohesionClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/dan/DdiscoCohesionClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Classification/dan/LccSentimentClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/eng/EmotionClassification.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 from __future__ import annotations
 
-from mteb.abstasks import AbsTaskClassification
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
+from ....abstasks import AbsTaskClassification
 
-class LccSentimentClassification(AbsTaskClassification):
+
+class EmotionClassification(AbsTaskClassification):
     metadata = TaskMetadata(
-        name="LccSentimentClassification",
+        name="EmotionClassification",
+        description="Emotion is a dataset of English Twitter messages with six basic emotions: anger, fear, joy, love, sadness, and surprise.",
+        reference="https://www.aclweb.org/anthology/D18-1404",
         dataset={
-            "path": "DDSC/lcc",
-            "revision": "de7ba3406ee55ea2cc52a0a41408fa6aede6d3c6",
+            "path": "mteb/emotion",
+            "revision": "4f58c6b202a23cf9a4da393831edf4f9183cad37",
         },
-        description="The leipzig corpora collection, annotated for sentiment",
-        reference="https://github.com/fnielsen/lcc-sentiment",
         type="Classification",
         category="s2s",
-        eval_splits=["test"],
-        eval_langs=["dan-Latn"],
+        eval_splits=["validation", "test"],
+        eval_langs=["eng-Latn"],
         main_score="accuracy",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples={"test": 150},
-        avg_character_length={"test": 118.7},
+        n_samples={"validation": 2000, "test": 2000},
+        avg_character_length={"validation": 95.3, "test": 95.6},
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
         metadata_dict = super().metadata_dict
         metadata_dict["n_experiments"] = 10
         metadata_dict["samples_per_label"] = 16
```

### Comparing `mteb-1.7.9/mteb/tasks/Classification/ell/GreekLegalCodeClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/ell/GreekLegalCodeClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Classification/ell/GreekSentimentClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/eng/TweetTopicSingleClassification.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 from __future__ import annotations
 
 from mteb.abstasks import AbsTaskClassification
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 
-class GreekSentimentClassification(AbsTaskClassification):
+class TweetTopicSingleClassification(AbsTaskClassification):
     metadata = TaskMetadata(
-        name="GreekSentimentClassification",
+        name="TweetTopicSingleClassification",
+        description="""Topic classification dataset on Twitter with 6 labels. Each instance of
+        TweetTopic comes with a timestamp which distributes from September 2019 to August 2021.
+        Tweets were preprocessed before the annotation to normalize some artifacts, converting
+        URLs into a special token {{URL}} and non-verified usernames into {{USERNAME}}. For verified
+        usernames, we replace its display name (or account name) with symbols {@}.
+        """,
         dataset={
-            "path": "sepidmnorozy/Greek_sentiment",
-            "revision": "94b245f3ccdf8e8b2cbf8f13f55eee820b70eccf",
+            "path": "cardiffnlp/tweet_topic_single",
+            "revision": "87b7a0d1c402dbb481db649569c556d9aa27ac05",
         },
-        description="Greek sentiment analysis dataset.",
-        reference="https://huggingface.co/datasets/sepidmnorozy/Greek_sentiment",
+        reference="https://arxiv.org/abs/2209.09824",
         type="Classification",
         category="s2s",
-        eval_splits=["validation", "test"],
-        eval_langs=["ell-Grek"],
+        eval_splits=["test_2021"],
+        eval_langs=["eng-Latn"],
         main_score="accuracy",
-        date=("2022-08-01", "2022-08-01"),
+        date=("2019-09-01", "2021-08-31"),
         form=["written"],
-        domains=["Reviews"],
-        task_subtypes=["Sentiment/Hate speech"],
-        license="Not specified",
-        socioeconomic_status="mixed",
-        annotations_creators="derived",
+        domains=["Social", "News"],
+        task_subtypes=["Topic classification"],
+        license="Other",
+        socioeconomic_status="medium",
+        annotations_creators="expert-annotated",
         dialect=[],
         text_creation="found",
         bibtex_citation="""
-        @inproceedings{mollanorozy-etal-2023-cross,
-            title = "Cross-lingual Transfer Learning with \{P\}ersian",
-            author = "Mollanorozy, Sepideh  and
-            Tanti, Marc  and
-            Nissim, Malvina",
-            editor = "Beinborn, Lisa  and
-            Goswami, Koustava  and
-            Murado{\\u{g}}lu, Saliha  and
-            Sorokin, Alexey  and
-            Kumar, Ritesh  and
-            Shcherbakov, Andreas  and
-            Ponti, Edoardo M.  and
-            Cotterell, Ryan  and
-            Vylomova, Ekaterina",
-            booktitle = "Proceedings of the 5th Workshop on Research in Computational Linguistic Typology and Multilingual NLP",
-            month = may,
-            year = "2023",
-            address = "Dubrovnik, Croatia",
-            publisher = "Association for Computational Linguistics",
-            url = "https://aclanthology.org/2023.sigtyp-1.9",
-            doi = "10.18653/v1/2023.sigtyp-1.9",
-            pages = "89--95",
+        @inproceedings{dimosthenis-etal-2022-twitter,
+            title = "{T}witter {T}opic {C}lassification",
+            author = "Antypas, Dimosthenis  and
+            Ushio, Asahi  and
+            Camacho-Collados, Jose  and
+            Neves, Leonardo  and
+            Silva, Vitor  and
+            Barbieri, Francesco",
+            booktitle = "Proceedings of the 29th International Conference on Computational Linguistics",
+            month = oct,
+            year = "2022",
+            address = "Gyeongju, Republic of Korea",
+            publisher = "International Committee on Computational Linguistics"
         }
         """,
-        n_samples={"validation": 383, "test": 767},
-        avg_character_length={"validation": 208, "test": 206},
+        n_samples={"test_2021": 1693},
+        avg_character_length={"test_2021": 167.66},
     )
+
+    def dataset_transform(self):
+        self.dataset["train"] = self.dataset["train_2021"]
```

### Comparing `mteb-1.7.9/mteb/tasks/Classification/eng/AmazonPolarityClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/eng/AmazonPolarityClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Classification/eng/Banking77Classification.py` & `mteb-1.8.0/mteb/tasks/Classification/eng/Banking77Classification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Classification/eng/EmotionClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/nob/NorwegianParliamentClassification.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,34 @@
 from __future__ import annotations
 
+from mteb.abstasks import AbsTaskClassification
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks import AbsTaskClassification
 
-
-class EmotionClassification(AbsTaskClassification):
+class NorwegianParliamentClassification(AbsTaskClassification):
     metadata = TaskMetadata(
-        name="EmotionClassification",
-        description="Emotion is a dataset of English Twitter messages with six basic emotions: anger, fear, joy, love, sadness, and surprise.",
-        reference="https://www.aclweb.org/anthology/D18-1404",
+        name="NorwegianParliamentClassification",
+        description="Norwegian parliament speeches annotated for sentiment",
+        reference="https://huggingface.co/datasets/NbAiLab/norwegian_parliament",
         dataset={
-            "path": "mteb/emotion",
-            "revision": "4f58c6b202a23cf9a4da393831edf4f9183cad37",
+            "path": "NbAiLab/norwegian_parliament",
+            "revision": "f7393532774c66312378d30b197610b43d751972",
         },
         type="Classification",
         category="s2s",
-        eval_splits=["validation", "test"],
-        eval_langs=["eng-Latn"],
+        eval_splits=["test", "validation"],
+        eval_langs=["nob-Latn"],
+        # assumed to be bokmål
         main_score="accuracy",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples={"validation": 2000, "test": 2000},
-        avg_character_length={"validation": 95.3, "test": 95.6},
+        n_samples={"test": 1200, "validation": 1200},
+        avg_character_length={"test": 1884.0, "validation": 1911.0},
     )
-
-    @property
-    def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = super().metadata_dict
-        metadata_dict["n_experiments"] = 10
-        metadata_dict["samples_per_label"] = 16
-        return metadata_dict
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mteb-1.7.9/mteb/tasks/Classification/eng/ImdbClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/eng/ImdbClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Classification/eng/NewsClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/eng/NewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Classification/eng/ToxicConversationsClassification.py` & `mteb-1.8.0/mteb/tasks/STS/eng/BiossesSTS.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks import AbsTaskClassification
+from ....abstasks.AbsTaskSTS import AbsTaskSTS
 
 
-class ToxicConversationsClassification(AbsTaskClassification):
+class BiossesSTS(AbsTaskSTS):
     metadata = TaskMetadata(
-        name="ToxicConversationsClassification",
-        description="Collection of comments from the Civil Comments platform together with annotations if the comment is toxic or not.",
-        reference="https://www.kaggle.com/competitions/jigsaw-unintended-bias-in-toxicity-classification/overview",
+        name="BIOSSES",
         dataset={
-            "path": "mteb/toxic_conversations_50k",
-            "revision": "edfaf9da55d3dd50d43143d90c1ac476895ae6de",
+            "path": "mteb/biosses-sts",
+            "revision": "d3fb88f8f02e40887cd149695127462bbcf29b4a",
         },
-        type="Classification",
+        description="Biomedical Semantic Similarity Estimation.",
+        reference="https://tabilab.cmpe.boun.edu.tr/BIOSSES/DataSet.html",
+        type="STS",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["eng-Latn"],
-        main_score="accuracy",
+        main_score="cosine_spearman",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples={"test": 50000},
-        avg_character_length={"test": 296.6},
+        n_samples=None,
+        avg_character_length=None,
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
         metadata_dict = super().metadata_dict
-        metadata_dict["n_experiments"] = 10
-        metadata_dict["samples_per_label"] = 16
+        metadata_dict["min_score"] = 0
+        metadata_dict["max_score"] = 5
         return metadata_dict
```

### Comparing `mteb-1.7.9/mteb/tasks/Classification/eng/TweetSentimentExtractionClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/eng/TweetSentimentExtractionClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Classification/est/estonian_valence.py` & `mteb-1.8.0/mteb/tasks/Classification/est/estonian_valence.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Classification/fas/PersianFoodSentimentClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/fas/PersianFoodSentimentClassification.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,15 +39,10 @@
         }
         """,
         n_samples={"validation": TEST_SAMPLES, "test": TEST_SAMPLES},
         avg_character_length={"validation": 90.37, "test": 90.58},
     )
 
     def dataset_transform(self):
-        self.dataset["validation"] = (
-            self.dataset["validation"]
-            .shuffle(seed=self.seed)
-            .select(range(TEST_SAMPLES))
-        )
-        self.dataset["test"] = (
-            self.dataset["test"].shuffle(seed=self.seed).select(range(TEST_SAMPLES))
+        self.dataset = self.stratified_subsampling(
+            self.dataset, seed=self.seed, splits=["validation", "test"]
         )
```

### Comparing `mteb-1.7.9/mteb/tasks/Classification/fil/FilipinoHateSpeechClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/fil/FilipinoHateSpeechClassification.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,15 +41,10 @@
         }
         """,
         n_samples={"validation": TEST_SAMPLES, "test": TEST_SAMPLES},
         avg_character_length={"validation": 88.1, "test": 87.4},
     )
 
     def dataset_transform(self):
-        self.dataset["validation"] = (
-            self.dataset["validation"]
-            .shuffle(seed=self.seed)
-            .select(range(TEST_SAMPLES))
-        )
-        self.dataset["test"] = (
-            self.dataset["test"].shuffle(seed=self.seed).select(range(TEST_SAMPLES))
+        self.dataset = self.stratified_subsampling(
+            self.dataset, seed=self.seed, splits=["validation", "test"]
         )
```

### Comparing `mteb-1.7.9/mteb/tasks/Classification/fra/MovieReviewSentimentClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/fra/MovieReviewSentimentClassification.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,13 +39,10 @@
 """,
         n_samples={"validation": N_SAMPLES, "test": N_SAMPLES},
         avg_character_length={"validation": 550.3, "test": 558.1},
     )
 
     def dataset_transform(self):
         self.dataset = self.dataset.rename_column("review", "text")
-        self.dataset["validation"] = (
-            self.dataset["validation"].shuffle(seed=self.seed).select(range(N_SAMPLES))
-        )
-        self.dataset["test"] = (
-            self.dataset["test"].shuffle(seed=self.seed).select(range(N_SAMPLES))
+        self.dataset = self.stratified_subsampling(
+            self.dataset, seed=self.seed, splits=["validation", "test"]
         )
```

### Comparing `mteb-1.7.9/mteb/tasks/Classification/guj/GujaratiNewsClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/guj/GujaratiNewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Classification/hin/HindiDiscourseClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/hin/HindiDiscourseClassification.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,8 +54,10 @@
         avg_character_length={"train": 79.23828125},
     )
 
     def dataset_transform(self):
         self.dataset = self.dataset.rename_columns(
             {"Sentence": "text", "Discourse Mode": "label"}
         ).remove_columns(["Story_no"])
-        self.dataset["train"] = self.dataset["train"].select(range(2048))
+        self.dataset = self.stratified_subsampling(
+            self.dataset, seed=self.seed, splits=["train"]
+        )
```

### Comparing `mteb-1.7.9/mteb/tasks/Classification/hrv/CroatianSentimentClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/san/SanskritShlokasClassification.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 from __future__ import annotations
 
 from mteb.abstasks import AbsTaskClassification
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 
-class CroatianSentimentClassification(AbsTaskClassification):
+class SanskritShlokasClassification(AbsTaskClassification):
     metadata = TaskMetadata(
-        name="CroatianSentimentClassification",
-        description="An Croatian dataset for sentiment classification.",
-        reference="https://arxiv.org/abs/2009.08712",
+        name="SanskritShlokasClassification",
+        description="This data set contains ~500 Shlokas  ",
+        reference="https://github.com/goru001/nlp-for-sanskrit",
         dataset={
-            "path": "sepidmnorozy/Croatian_sentiment",
-            "revision": "255da5c6b54c95faf74aba6d6cad9b2e176bf90a",
+            "path": "bpHigh/iNLTK_Sanskrit_Shlokas_Dataset",
+            "revision": "5a79d6472db143690c7ce6e974995d3610eee7f0",
         },
         type="Classification",
         category="s2s",
-        date=("2022-01-01", "2022-01-01"),
-        eval_splits=["validation", "test"],
-        eval_langs=["hrv-Latn"],
+        date=("2019-01-01", "2020-01-01"),
+        eval_splits=["train", "validation"],
+        eval_langs=["san-Deva"],
         main_score="accuracy",
         form=["written"],
-        domains=["Reviews"],
-        task_subtypes=["Sentiment/Hate speech"],
-        license="Not specified",
+        domains=["Religious"],
+        task_subtypes=["Topic classification"],
+        license="CC BY-SA 4.0",
         socioeconomic_status="mixed",
-        annotations_creators="human-annotated",
+        annotations_creators="derived",
         dialect=[],
         text_creation="found",
-        bibtex_citation="""@inproceedings{mollanorozy-etal-2023-cross,
-    title = "Cross-lingual Transfer Learning with \{P\}ersian",
-    author = "Mollanorozy, Sepideh  and
-      Tanti, Marc  and
-      Nissim, Malvina",
-    editor = "Beinborn, Lisa  and
-      Goswami, Koustava  and
-      Murado{\\u{g}}lu, Saliha  and
-      Sorokin, Alexey  and
-      Kumar, Ritesh  and
-      Shcherbakov, Andreas  and
-      Ponti, Edoardo M.  and
-      Cotterell, Ryan  and
-      Vylomova, Ekaterina",
-    booktitle = "Proceedings of the 5th Workshop on Research in Computational Linguistic Typology and Multilingual NLP",
-    month = may,
-    year = "2023",
-    address = "Dubrovnik, Croatia",
-    publisher = "Association for Computational Linguistics",
-    url = "https://aclanthology.org/2023.sigtyp-1.9",
-    doi = "10.18653/v1/2023.sigtyp-1.9",
-    pages = "89--95",
-}
-""",
-        n_samples={"validation": 214, "test": 437},
-        avg_character_length={"validation": 166.9, "test": 151.4},
+        bibtex_citation="""
+               @inproceedings{arora-2020-inltk,
+           title = "i{NLTK}: Natural Language Toolkit for Indic Languages",
+           author = "Arora, Gaurav",
+           editor = "Park, Eunjeong L.  and
+             Hagiwara, Masato  and
+             Milajevs, Dmitrijs  and
+             Liu, Nelson F.  and
+             Chauhan, Geeticka  and
+             Tan, Liling",
+           booktitle = "Proceedings of Second Workshop for NLP Open Source Software (NLP-OSS)",
+           month = nov,
+           year = "2020",
+           address = "Online",
+           publisher = "Association for Computational Linguistics",
+           url = "https://aclanthology.org/2020.nlposs-1.10",
+           doi = "10.18653/v1/2020.nlposs-1.10",
+           pages = "66--71",
+           abstract = "We present iNLTK, an open-source NLP library consisting of pre-trained language models and out-of-the-box support for Data Augmentation, Textual Similarity, Sentence Embeddings, Word Embeddings, Tokenization and Text Generation in 13 Indic Languages. By using pre-trained models from iNLTK for text classification on publicly available datasets, we significantly outperform previously reported results. On these datasets, we also show that by using pre-trained models and data augmentation from iNLTK, we can achieve more than 95{\%} of the previous best performance by using less than 10{\%} of the training data. iNLTK is already being widely used by the community and has 40,000+ downloads, 600+ stars and 100+ forks on GitHub.",
+           }
+           """,
+        n_samples={"train": 383, "validation": 96},
+        avg_character_length={"train": 98.415, "validation": 96.635},
     )
+
+    def dataset_transform(self):
+        self.dataset = self.dataset.rename_columns({"Sloka": "text", "Class": "label"})
```

### Comparing `mteb-1.7.9/mteb/tasks/Classification/ind/IndonesianIdClickbaitClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/ind/IndonesianIdClickbaitClassification.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,8 +48,10 @@
         avg_character_length={"train": 64.28},
     )
 
     def dataset_transform(self):
         self.dataset = self.dataset.remove_columns(["label"]).rename_columns(
             {"title": "text", "label_score": "label"}
         )
-        self.dataset["train"] = self.dataset["train"].select(range(2048))
+        self.dataset = self.stratified_subsampling(
+            self.dataset, seed=self.seed, splits=["train"]
+        )
```

### Comparing `mteb-1.7.9/mteb/tasks/Classification/ita/ItaHateClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/multilingual/MultiHateClassification.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,77 @@
 from __future__ import annotations
 
-from mteb.abstasks.AbsTaskClassification import AbsTaskClassification
+from mteb.abstasks import AbsTaskClassification, MultilingualTask
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
+_LANGUAGES = {
+    "ara": ["ara-Arab"],
+    "cmn": ["cmn-Hans"],
+    "eng": ["eng-Latn"],
+    "deu": ["deu-Latn"],
+    "fra": ["fra-Latn"],
+    "hin": ["hin-Deva"],
+    "ita": ["ita-Latn"],
+    "nld": ["nld-Latn"],
+    "pol": ["pol-Latn"],
+    "por": ["por-Latn"],
+    "spa": ["spa-Latn"],
+}
 
-class ItaHateClassification(AbsTaskClassification):
+
+class MultiHateClassification(MultilingualTask, AbsTaskClassification):
     metadata = TaskMetadata(
-        name="ItaHateClassification",
+        name="MultiHateClassification",
         dataset={
-            "path": "Paul/hatecheck-italian",
-            "revision": "21e3d5c827cb60619a89988b24979850a7af85a5",
+            "path": "mteb/multi-hatecheck",
+            "revision": "ef137ea2b7c719183f8f60edf536b50f56d1365b",
         },
         description="""Hate speech detection dataset with binary
                        (hateful vs non-hateful) labels. Includes 25+ distinct types of hate
-                       and challenging non-hate. Multilingual datase released as 10 unilingual models
+                       and challenging non-hate, and 11 languages.
                      """,
         reference="https://aclanthology.org/2022.woah-1.15/",
         type="Classification",
         category="s2s",
         eval_splits=["test"],
-        eval_langs=["ita-Latn"],
+        eval_langs=_LANGUAGES,
         main_score="accuracy",
-        date=("2021-11-01", "2022-02-28"),
+        date=("2020-11-23", "2022-02-28"),
         form=["written"],
         domains=["Constructed"],
         task_subtypes=["Sentiment/Hate speech"],
         license="cc-by-4.0",
         socioeconomic_status="high",
         annotations_creators="expert-annotated",
         dialect=[],
         text_creation="created",
         bibtex_citation="""
+        @inproceedings{rottger-etal-2021-hatecheck,
+            title = "{H}ate{C}heck: Functional Tests for Hate Speech Detection Models",
+            author = {R{\"o}ttger, Paul  and
+            Vidgen, Bertie  and
+            Nguyen, Dong  and
+            Waseem, Zeerak  and
+            Margetts, Helen  and
+            Pierrehumbert, Janet},
+            editor = "Zong, Chengqing  and
+            Xia, Fei  and
+            Li, Wenjie  and
+            Navigli, Roberto",
+            booktitle = "Proceedings of the 59th Annual Meeting of the Association for Computational Linguistics and the 11th International Joint Conference on Natural Language Processing (Volume 1: Long Papers)",
+            month = aug,
+            year = "2021",
+            address = "Online",
+            publisher = "Association for Computational Linguistics",
+            url = "https://aclanthology.org/2021.acl-long.4",
+            doi = "10.18653/v1/2021.acl-long.4",
+            pages = "41--58",
+            abstract = "Detecting online hate is a difficult task that even state-of-the-art models struggle with. Typically, hate speech detection models are evaluated by measuring their performance on held-out test data using metrics such as accuracy and F1 score. However, this approach makes it difficult to identify specific model weak points. It also risks overestimating generalisable model performance due to increasingly well-evidenced systematic gaps and biases in hate speech datasets. To enable more targeted diagnostic insights, we introduce HateCheck, a suite of functional tests for hate speech detection models. We specify 29 model functionalities motivated by a review of previous research and a series of interviews with civil society stakeholders. We craft test cases for each functionality and validate their quality through a structured annotation process. To illustrate HateCheck{'}s utility, we test near-state-of-the-art transformer models as well as two popular commercial models, revealing critical model weaknesses.",
+        }
+
         @inproceedings{rottger-etal-2022-multilingual,
             title = "Multilingual {H}ate{C}heck: Functional Tests for Multilingual Hate Speech Detection Models",
             author = {R{\"o}ttger, Paul  and
             Seelawi, Haitham  and
             Nozza, Debora  and
             Talat, Zeerak  and
             Vidgen, Bertie},
@@ -50,24 +87,26 @@
             publisher = "Association for Computational Linguistics",
             url = "https://aclanthology.org/2022.woah-1.15",
             doi = "10.18653/v1/2022.woah-1.15",
             pages = "154--169",
             abstract = "Hate speech detection models are typically evaluated on held-out test sets. However, this risks painting an incomplete and potentially misleading picture of model performance because of increasingly well-documented systematic gaps and biases in hate speech datasets. To enable more targeted diagnostic insights, recent research has thus introduced functional tests for hate speech detection models. However, these tests currently only exist for English-language content, which means that they cannot support the development of more effective models in other languages spoken by billions across the world. To help address this issue, we introduce Multilingual HateCheck (MHC), a suite of functional tests for multilingual hate speech detection models. MHC covers 34 functionalities across ten languages, which is more languages than any other hate speech dataset. To illustrate MHC{'}s utility, we train and test a high-performing multilingual hate speech detection model, and reveal critical model weaknesses for monolingual and cross-lingual applications.",
         }
         """,
-        n_samples={"test": 1845},
-        avg_character_length={"test": 50.4},
+        n_samples={"test": 10000},
+        avg_character_length={"test": 45.9},
     )
 
     def dataset_transform(self):
-        keep_cols = ["test_case", "label_gold"]
-        rename_dict = dict(zip(keep_cols, ["text", "label"]))
-        remove_cols = [
-            col for col in self.dataset["test"].column_names if col not in keep_cols
-        ]
-        self.dataset = self.dataset.rename_columns(rename_dict)
-        self.dataset = self.dataset.class_encode_column("label")
-        self.dataset = self.dataset.class_encode_column("functionality")
-        self.dataset = self.dataset["test"].train_test_split(
-            test_size=0.5, seed=42, stratify_by_column="functionality"
-        )  # balanced sampling across types of hate speech
-        self.dataset = self.dataset.remove_columns(remove_cols)
+        # for each language perform some transforms
+        for lang in self.dataset.keys():
+            _dataset = self.dataset[lang]
+            _dataset = _dataset.rename_columns({"is_hateful": "label"})
+            for label in ["label", "functionality"]:
+                _dataset = _dataset.class_encode_column(label)
+            _dataset = _dataset["test"].train_test_split(
+                train_size=1000,
+                test_size=1000,
+                seed=self.seed,
+                stratify_by_column="functionality",
+            )  # balanced sampling across types of hate speech
+            _dataset = _dataset.remove_columns(["functionality"])
+            self.dataset[lang] = _dataset
```

### Comparing `mteb-1.7.9/mteb/tasks/Classification/ita/ItalianLinguistAcceptabilityClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/ita/ItalianLinguistAcceptabilityClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Classification/jpn/WRIMEClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/jpn/WRIMEClassification.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,13 +58,13 @@
         avg_character_length={"test": 47.78},
     )
 
     def dataset_transform(self):
         self.dataset = self.dataset.flatten().select_columns(
             ["sentence", "avg_readers.sentiment"]
         )
-        self.dataset = self.dataset.rename_column("sentence", "text")
-        self.dataset = self.dataset.rename_column("avg_readers.sentiment", "label")
-        # random downsample to 2048
-        self.dataset["test"] = self.dataset["test"].shuffle(seed=42)
-        max_samples = min(2048, len(self.dataset["test"]))
-        self.dataset["test"] = self.dataset["test"].select(range(max_samples))
+        self.dataset = self.dataset.rename_columns(
+            {"sentence": "text", "avg_readers.sentiment": "label"}
+        )
+        self.dataset = self.stratified_subsampling(
+            self.dataset, seed=self.seed, splits=["test"]
+        )
```

### Comparing `mteb-1.7.9/mteb/tasks/Classification/kur/KurdishSentimentClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/kur/KurdishSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Classification/mkd/MacedonianTweetSentimentClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/mkd/MacedonianTweetSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Classification/mlt/MalteseSentimentClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/dan/LccSentimentClassification.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,59 @@
 from __future__ import annotations
 
 from mteb.abstasks import AbsTaskClassification
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 
-class MalteseSentimentClassification(AbsTaskClassification):
+class LccSentimentClassification(AbsTaskClassification):
     metadata = TaskMetadata(
-        name="MalteseSentimentClassification",
-        description="An Maltese dataset for sentiment classification.",
-        reference="https://arxiv.org/abs/2009.08712",
+        name="LccSentimentClassification",
         dataset={
-            "path": "sepidmnorozy/Maltese_sentiment",
-            "revision": "fd47b916f9ebb5d27b0e583de9d2b2db39f7dda2",
+            "path": "DDSC/lcc",
+            "revision": "de7ba3406ee55ea2cc52a0a41408fa6aede6d3c6",
         },
+        description="The leipzig corpora collection, annotated for sentiment",
+        reference="https://github.com/fnielsen/lcc-sentiment",
         type="Classification",
         category="s2s",
-        date=("2022-01-01", "2022-01-01"),
-        eval_splits=["validation", "test"],
-        eval_langs=["mlt-Latn"],
+        eval_splits=["test"],
+        eval_langs=["dan-Latn"],
         main_score="accuracy",
+        date=("2006-01-01", "2006-12-31"),
         form=["written"],
-        domains=["Reviews"],
+        domains=["News", "Web"],
         task_subtypes=["Sentiment/Hate speech"],
-        license="Not specified",
+        license="CC-BY-4.0",
         socioeconomic_status="mixed",
-        annotations_creators="human-annotated",
+        annotations_creators="expert-annotated",
         dialect=[],
         text_creation="found",
-        bibtex_citation="""@inproceedings{mollanorozy-etal-2023-cross,
-    title = "Cross-lingual Transfer Learning with \{P\}ersian",
-    author = "Mollanorozy, Sepideh  and
-      Tanti, Marc  and
-      Nissim, Malvina",
-    editor = "Beinborn, Lisa  and
-      Goswami, Koustava  and
-      Murado{\\u{g}}lu, Saliha  and
-      Sorokin, Alexey  and
-      Kumar, Ritesh  and
-      Shcherbakov, Andreas  and
-      Ponti, Edoardo M.  and
-      Cotterell, Ryan  and
-      Vylomova, Ekaterina",
-    booktitle = "Proceedings of the 5th Workshop on Research in Computational Linguistic Typology and Multilingual NLP",
+        bibtex_citation="""@inproceedings{quasthoff-etal-2006-corpus,
+    title = "Corpus Portal for Search in Monolingual Corpora",
+    author = "Quasthoff, Uwe  and
+      Richter, Matthias  and
+      Biemann, Christian",
+    editor = "Calzolari, Nicoletta  and
+      Choukri, Khalid  and
+      Gangemi, Aldo  and
+      Maegaard, Bente  and
+      Mariani, Joseph  and
+      Odijk, Jan  and
+      Tapias, Daniel",
+    booktitle = "Proceedings of the Fifth International Conference on Language Resources and Evaluation ({LREC}{'}06)",
     month = may,
-    year = "2023",
-    address = "Dubrovnik, Croatia",
-    publisher = "Association for Computational Linguistics",
-    url = "https://aclanthology.org/2023.sigtyp-1.9",
-    doi = "10.18653/v1/2023.sigtyp-1.9",
-    pages = "89--95",
-}
-""",
-        n_samples={"validation": 85, "test": 171},
-        avg_character_length={"validation": 119.7, "test": 132.4},
+    year = "2006",
+    address = "Genoa, Italy",
+    publisher = "European Language Resources Association (ELRA)",
+    url = "http://www.lrec-conf.org/proceedings/lrec2006/pdf/641_pdf.pdf",
+    abstract = "A simple and flexible schema for storing and presenting monolingual language resources is proposed. In this format, data for 18 different languages is already available in various sizes. The data is provided free of charge for online use and download. The main target is to ease the application of algorithms for monolingual and interlingual studies.",
+}""",
+        n_samples={"test": 150},
+        avg_character_length={"test": 118.7},
     )
+
+    @property
+    def metadata_dict(self) -> dict[str, str]:
+        metadata_dict = super().metadata_dict
+        metadata_dict["n_experiments"] = 10
+        metadata_dict["samples_per_label"] = 16
+        return metadata_dict
```

### Comparing `mteb-1.7.9/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Classification/multilingual/IndicSentimentClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/multilingual/IndicSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Classification/multilingual/NordicLangClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/multilingual/NordicLangClassification.py`

 * *Files 13% similar despite different names*

```diff
@@ -44,9 +44,10 @@
     def metadata_dict(self) -> dict[str, str]:
         metadata_dict = super().metadata_dict
         metadata_dict["n_experiments"] = 10
         metadata_dict["samples_per_label"] = 32
         return metadata_dict
 
     def dataset_transform(self):
-        self.dataset = self.dataset.rename_column("sentence", "text")
-        self.dataset = self.dataset.rename_column("language", "label")
+        self.dataset = self.dataset.rename_columns(
+            {"sentence": "text", "language": "label"}
+        )
```

### Comparing `mteb-1.7.9/mteb/tasks/Classification/multilingual/ScalaClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/multilingual/ScalaClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Classification/nld/DutchBookReviewSentimentClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/nld/DutchBookReviewSentimentClassification.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,16 @@
         task_subtypes=["Sentiment/Hate speech"],
         license="CC BY-NC-SA 4.0",
         socioeconomic_status="mixed",
         annotations_creators="derived",
         dialect=[],
         text_creation="found",
         bibtex_citation="""@article{DBLP:journals/corr/abs-1910-00896,
-  author    = {Benjamin van der Burgh and
-               Suzan Verberne},
+  author    = {Benjamin, van der Burgh and
+               Suzan, Verberne},
   title     = {The merits of Universal Language Model Fine-tuning for Small Datasets
                - a case with Dutch book reviews},
   journal   = {CoRR},
   volume    = {abs/1910.00896},
   year      = {2019},
   url       = {http://arxiv.org/abs/1910.00896},
   archivePrefix = {arXiv},
```

### Comparing `mteb-1.7.9/mteb/tasks/Classification/nob/NoRecClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/nob/NoRecClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Classification/nob/NorwegianParliamentClassification.py` & `mteb-1.8.0/mteb/tasks/PairClassification/eng/TwitterSemEval2015PC.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from __future__ import annotations
 
-from mteb.abstasks import AbsTaskClassification
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
+from ....abstasks.AbsTaskPairClassification import AbsTaskPairClassification
 
-class NorwegianParliamentClassification(AbsTaskClassification):
+
+class TwitterSemEval2015PC(AbsTaskPairClassification):
     metadata = TaskMetadata(
-        name="NorwegianParliamentClassification",
-        description="Norwegian parliament speeches annotated for sentiment",
-        reference="https://huggingface.co/datasets/NbAiLab/norwegian_parliament",
+        name="TwitterSemEval2015",
         dataset={
-            "path": "NbAiLab/norwegian_parliament",
-            "revision": "f7393532774c66312378d30b197610b43d751972",
+            "path": "mteb/twittersemeval2015-pairclassification",
+            "revision": "70970daeab8776df92f5ea462b6173c0b46fd2d1",
         },
-        type="Classification",
+        description="Paraphrase-Pairs of Tweets from the SemEval 2015 workshop.",
+        reference="https://alt.qcri.org/semeval2015/task1/",
         category="s2s",
-        eval_splits=["test", "validation"],
-        eval_langs=["nob-Latn"],
-        # assumed to be bokmål
-        main_score="accuracy",
+        type="PairClassification",
+        eval_splits=["test"],
+        eval_langs=["eng-Latn"],
+        main_score="ap",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples={"test": 1200, "validation": 1200},
-        avg_character_length={"test": 1884.0, "validation": 1911.0},
+        n_samples={"test": 16777},
+        avg_character_length={"test": 38.3},
     )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mteb-1.7.9/mteb/tasks/Classification/pol/PolishClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/pol/PolishClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Classification/ron/RomanianSentimentClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/ron/RomanianSentimentClassification.py`

 * *Files 13% similar despite different names*

```diff
@@ -38,10 +38,10 @@
 """,
         n_samples={"test": TEST_SAMPLES},
         avg_character_length={"test": 67.6},
     )
 
     def dataset_transform(self):
         self.dataset = self.dataset.rename_column("sentence", "text")
-        self.dataset["test"] = (
-            self.dataset["test"].shuffle(seed=self.seed).select(range(TEST_SAMPLES))
+        self.dataset = self.stratified_subsampling(
+            self.dataset, seed=self.seed, splits=["test"]
         )
```

### Comparing `mteb-1.7.9/mteb/tasks/Classification/slk/SlovakSentimentClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/ben/BengaliSentimentAnalysis.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,44 @@
 from __future__ import annotations
 
-from mteb.abstasks import AbsTaskClassification
+from mteb.abstasks.AbsTaskClassification import AbsTaskClassification
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-N_SAMPLES = 2800
 
-
-class SlovakSentimentClassification(AbsTaskClassification):
+class BengaliSentimentAnalysis(AbsTaskClassification):
     metadata = TaskMetadata(
-        name="SlovakSentimentClassification",
-        description="Slovak Sentiment Classification Dataset",
-        reference="https://huggingface.co/datasets/sepidmnorozy/Slovak_sentiment",
+        name="BengaliSentimentAnalysis",
+        description="dataset contains 3307 Negative reviews and 8500 Positive reviews collected and manually annotated from Youtube Bengali drama.",
+        reference="https://data.mendeley.com/datasets/p6zc7krs37/4",
         dataset={
-            "path": "sepidmnorozy/Slovak_sentiment",
-            "revision": "e698d1df52766d73ae1cc569dfc622527c329a08",
+            "path": "Akash190104/bengali_sentiment_analysis",
+            "revision": "a4b3685b1854cc26c554dda4c7cb918a36a6fb6c",
         },
         type="Classification",
         category="s2s",
-        eval_splits=["validation", "test"],
-        eval_langs=["slk-Latn"],
-        main_score="accuracy",
-        date=("2022-08-01", "2022-08-01"),
+        eval_splits=["train"],
+        eval_langs=["ben-Beng"],
+        main_score="f1",
+        date=("2020-06-24", "2020-11-26"),
         form=["written"],
+        dialect=[],
         domains=["Reviews"],
         task_subtypes=["Sentiment/Hate speech"],
-        license="Not specified",
-        socioeconomic_status="medium",
+        license="CC BY 4.0",
+        socioeconomic_status="mixed",
         annotations_creators="human-annotated",
-        dialect=[],
         text_creation="found",
-        bibtex_citation="""
-        @inproceedings{mollanorozy-etal-2023-cross,
-    title = "Cross-lingual Transfer Learning with \{P\}ersian",
-    author = "Mollanorozy, Sepideh  and
-      Tanti, Marc  and
-      Nissim, Malvina",
-    editor = "Beinborn, Lisa  and
-      Goswami, Koustava  and
-      Murado{\\u{g}}lu, Saliha  and
-      Sorokin, Alexey  and
-      Kumar, Ritesh  and
-      Shcherbakov, Andreas  and
-      Ponti, Edoardo M.  and
-      Cotterell, Ryan  and
-      Vylomova, Ekaterina",
-    booktitle = "Proceedings of the 5th Workshop on Research in Computational Linguistic Typology and Multilingual NLP",
-    month = may,
-    year = "2023",
-    address = "Dubrovnik, Croatia",
-    publisher = "Association for Computational Linguistics",
-    url = "https://aclanthology.org/2023.sigtyp-1.9",
-    doi = "10.18653/v1/2023.sigtyp-1.9",
-    pages = "89--95",
-}
-        """,
-        n_samples={"validation": 522, "test": 1040},
-        avg_character_length={"validation": 84.96, "test": 91.95},
+        bibtex_citation="""@inproceedings{sazzed2020cross,
+        title={Cross-lingual sentiment classification in low-resource Bengali language},
+        author={Sazzed, Salim},
+        booktitle={Proceedings of the Sixth Workshop on Noisy User-generated Text (W-NUT 2020)},
+        pages={50--60},
+        year={2020}
+        }""",
+        n_samples={"train": 11807},
+        avg_character_length={"train": 69.66},
     )
+
+    def dataset_transform(self):
+        self.dataset = self.stratified_subsampling(
+            self.dataset, seed=self.seed, splits=["train"]
+        )
```

### Comparing `mteb-1.7.9/mteb/tasks/Classification/ssw/SiswatiNewsClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/ssw/SiswatiNewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Classification/swe/SweRecClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/swe/SweRecClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Classification/tur/TurkishMovieSentimentClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/mal/MalayalamNewsClassification.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,36 @@
 from __future__ import annotations
 
 from mteb.abstasks import AbsTaskClassification
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 
-class TurkishMovieSentimentClassification(AbsTaskClassification):
+class MalayalamNewsClassification(AbsTaskClassification):
     metadata = TaskMetadata(
-        name="TurkishMovieSentimentClassification",
-        description="Turkish Movie Review Dataset",
-        reference="https://www.win.tue.nl/~mpechen/publications/pubs/MT_WISDOM2013.pdf",
+        name="MalayalamNewsClassification",
+        description="A Malayalam dataset for 3-class classification of Malayalam news articles",
+        reference="https://github.com/goru001/nlp-for-malyalam",
         dataset={
-            "path": "asparius/Turkish-Movie-Review",
-            "revision": "409a4415cce5f6bcfca6d5f3ca3c408211ca00b3",
+            "path": "mlexplorer008/malayalam_news_classification",
+            "revision": "666f63bba2387456d8f846ea4d0565181bd47b81",
         },
         type="Classification",
         category="s2s",
+        date=("2014-01-01", "2018-01-01"),
         eval_splits=["test"],
-        eval_langs=["tur-Latn"],
+        eval_langs=["mal-Mlym"],
         main_score="accuracy",
-        date=("2013-01-01", "2013-08-11"),
         form=["written"],
-        domains=["Reviews"],
-        task_subtypes=["Sentiment/Hate speech"],
-        license="Not specified",
+        domains=["News"],
+        task_subtypes=["Topic classification"],
+        license="MIT",
         socioeconomic_status="mixed",
         annotations_creators="derived",
         dialect=[],
         text_creation="found",
-        bibtex_citation="""
-        @inproceedings{Demirtas2013CrosslingualPD,
-            title={Cross-lingual polarity detection with machine translation},
-            author={Erkin Demirtas and Mykola Pechenizkiy},
-            booktitle={wisdom},
-            year={2013},
-            url={https://api.semanticscholar.org/CorpusID:3912960}
-        }
-        """,
-        n_samples={"train": 7972, "test": 2644},
-        avg_character_length={"train": 141.03, "test": 141.50},
+        bibtex_citation=None,
+        n_samples={"train": 5036, "test": 1260},
+        avg_character_length={"train": 79.48, "test": 80.44},
     )
+
+    def dataset_transform(self):
+        self.dataset = self.dataset.rename_columns({"headings": "text"})
```

### Comparing `mteb-1.7.9/mteb/tasks/Classification/tur/TurkishProductSentimentClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/tur/TurkishProductSentimentClassification.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,10 +32,10 @@
             title={Cross-lingual polarity detection with machine translation},
             author={Erkin Demirtas and Mykola Pechenizkiy},
             booktitle={wisdom},
             year={2013},
             url={https://api.semanticscholar.org/CorpusID:3912960}
         }
         """,
-        n_samples={"train": 4800, "test": 800},
-        avg_character_length={"train": 247.75, "test": 246.85},
+        n_samples={"test": 800},
+        avg_character_length={"test": 246.85},
     )
```

### Comparing `mteb-1.7.9/mteb/tasks/Classification/uig/UyghurSentimentClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/eng/PatentClassification.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,55 @@
 from __future__ import annotations
 
 from mteb.abstasks import AbsTaskClassification
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 
-class UyghurSentimentClassification(AbsTaskClassification):
+class PatentClassification(AbsTaskClassification):
     metadata = TaskMetadata(
-        name="UyghurSentimentClassification",
-        description="An Uyghur dataset for sentiment classification.",
-        reference="https://arxiv.org/abs/2009.08712",
+        name="PatentClassification",
+        description="Classification Dataset of Patents and Abstract",
         dataset={
-            "path": "sepidmnorozy/Uyghur_sentiment",
-            "revision": "f859e1cdf823b3b27aa27b0f0fd4cef1d66f4b38",
+            "path": "ccdv/patent-classification",
+            "revision": "2f38a1dfdecfacee0184d74eaeafd3c0fb49d2a6",
         },
+        reference="https://aclanthology.org/P19-1212.pdf",
         type="Classification",
         category="s2s",
-        date=("2022-01-01", "2022-01-01"),
         eval_splits=["test"],
-        eval_langs=["uig-Arab"],
+        eval_langs=["eng-Latn"],
         main_score="accuracy",
+        date=("2021-11-05", "2022-10-22"),
         form=["written"],
-        domains=["Reviews"],
-        task_subtypes=["Sentiment/Hate speech"],
+        domains=["Legal"],
+        task_subtypes=["Topic classification"],
         license="Not specified",
-        socioeconomic_status="mixed",
-        annotations_creators="human-annotated",
+        socioeconomic_status="high",
+        annotations_creators="derived",
         dialect=[],
         text_creation="found",
-        bibtex_citation="""@inproceedings{mollanorozy-etal-2023-cross,
-    title = "Cross-lingual Transfer Learning with \{P\}ersian",
-    author = "Mollanorozy, Sepideh  and
-      Tanti, Marc  and
-      Nissim, Malvina",
-    editor = "Beinborn, Lisa  and
-      Goswami, Koustava  and
-      Murado{\\u{g}}lu, Saliha  and
-      Sorokin, Alexey  and
-      Kumar, Ritesh  and
-      Shcherbakov, Andreas  and
-      Ponti, Edoardo M.  and
-      Cotterell, Ryan  and
-      Vylomova, Ekaterina",
-    booktitle = "Proceedings of the 5th Workshop on Research in Computational Linguistic Typology and Multilingual NLP",
-    month = may,
-    year = "2023",
-    address = "Dubrovnik, Croatia",
-    publisher = "Association for Computational Linguistics",
-    url = "https://aclanthology.org/2023.sigtyp-1.9",
-    doi = "10.18653/v1/2023.sigtyp-1.9",
-    pages = "89--95",
-}
-""",
-        n_samples={"test": 841},
-        avg_character_length={"test": 245.2},
+        bibtex_citation="""@inproceedings{sharma-etal-2019-bigpatent,
+            title = "{BIGPATENT}: A Large-Scale Dataset for Abstractive and Coherent Summarization",
+            author = "Sharma, Eva  and
+            Li, Chen  and
+            Wang, Lu",
+            editor = "Korhonen, Anna  and
+            Traum, David  and
+            M{\`a}rquez, Llu{\'\i}s",
+            booktitle = "Proceedings of the 57th Annual Meeting of the Association for Computational Linguistics",
+            month = jul,
+            year = "2019",
+            address = "Florence, Italy",
+            publisher = "Association for Computational Linguistics",
+            url = "https://aclanthology.org/P19-1212",
+            doi = "10.18653/v1/P19-1212",
+            pages = "2204--2213",
+            abstract = "Most existing text summarization datasets are compiled from the news domain, where summaries have a flattened discourse structure. In such datasets, summary-worthy content often appears in the beginning of input articles. Moreover, large segments from input articles are present verbatim in their respective summaries. These issues impede the learning and evaluation of systems that can understand an article{'}s global content structure as well as produce abstractive summaries with high compression ratio. In this work, we present a novel dataset, BIGPATENT, consisting of 1.3 million records of U.S. patent documents along with human written abstractive summaries. Compared to existing summarization datasets, BIGPATENT has the following properties: i) summaries contain a richer discourse structure with more recurring entities, ii) salient content is evenly distributed in the input, and iii) lesser and shorter extractive fragments are present in the summaries. Finally, we train and evaluate baselines and popular learning models on BIGPATENT to shed light on new challenges and motivate future directions for summarization research.",
+        }""",
+        n_samples={"test": 5000},
+        avg_character_length={"test": 18620.44},
     )
+
+    def dataset_transform(self):
+        self.dataset = self.stratified_subsampling(
+            self.dataset, seed=self.seed, splits=["test"]
+        )
```

### Comparing `mteb-1.7.9/mteb/tasks/Classification/vie/VieStudentFeedbackClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/swe/DalajClassification.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,86 +1,73 @@
+# SuperLIM tasks
 from __future__ import annotations
 
-import random
-from collections import Counter
-
 from mteb.abstasks import AbsTaskClassification
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-TEST_SAMPLES = 2048
-
 
-class VieStudentFeedbackClassification(AbsTaskClassification):
+class DalajClassification(AbsTaskClassification):
     metadata = TaskMetadata(
-        name="VieStudentFeedbackClassification",
-        description="A Vietnamese dataset for classification of student feedback",
-        reference="https://ieeexplore.ieee.org/document/8573337",
+        name="DalajClassification",
         dataset={
-            "path": "uitnlp/vietnamese_students_feedback",
-            "revision": "7b56c6cb1c9c8523249f407044c838660df3811a",
+            "path": "AI-Sweden/SuperLim",
+            "revision": "7ebf0b4caa7b2ae39698a889de782c09e6f5ee56",
+            "name": "dalaj",
         },
+        description="A Swedish dataset for linguistic acceptability. Available as a part of Superlim.",
+        reference="https://spraakbanken.gu.se/en/resources/superlim",
         type="Classification",
         category="s2s",
         eval_splits=["test"],
-        eval_langs=["vie-Latn"],
+        eval_langs=["swe-Latn"],
         main_score="accuracy",
-        date=("2021-12-26", "2021-12-26"),
+        date=("2017-01-01", "2020-12-31"),
         form=["written"],
-        domains=["Reviews"],
-        task_subtypes=["Sentiment/Hate speech"],
-        license="MIT",
-        socioeconomic_status="medium",
-        annotations_creators="human-annotated",
+        domains=["Non-fiction"],
+        task_subtypes=["Linguistic acceptability"],
+        license="CC-BY-4.0",
+        socioeconomic_status="mixed",
+        annotations_creators="expert-annotated",
         dialect=[],
         text_creation="created",
-        bibtex_citation="""@InProceedings{8573337,
-  author={Nguyen, Kiet Van and Nguyen, Vu Duc and Nguyen, Phu X. V. and Truong, Tham T. H. and Nguyen, Ngan Luu-Thuy},
-  booktitle={2018 10th International Conference on Knowledge and Systems Engineering (KSE)},
-  title={UIT-VSFC: Vietnamese Students’ Feedback Corpus for Sentiment Analysis},
-  year={2018},
-  volume={},
-  number={},
-  pages={19-24},
-  doi={10.1109/KSE.2018.8573337}
+        bibtex_citation="""@misc{2105.06681,
+Author = {Elena Volodina and Yousuf Ali Mohammed and Julia Klezl},
+Title = {DaLAJ - a dataset for linguistic acceptability judgments for Swedish: Format, baseline, sharing},
+Year = {2021},
+Eprint = {arXiv:2105.06681},
 }""",
-        n_samples={"test": TEST_SAMPLES},
-        avg_character_length={"test": 14.22},
+        n_samples={"test": 444},
+        avg_character_length={"test": 243.8},
     )
 
+    @property
+    def metadata_dict(self) -> dict[str, str]:
+        metadata_dict = super().metadata_dict
+        metadata_dict["n_experiments"] = 10
+        metadata_dict["samples_per_label"] = 16
+        return metadata_dict
+
     def dataset_transform(self):
-        seed = 42
-        random.seed(seed)
-        self.dataset = self.dataset.rename_column("sentence", "text")
-        self.dataset = self.dataset.rename_column("sentiment", "label")
-
-        for split in ["test"]:
-            ds = self.dataset[split]
-            # Determine number of classes and samples per class
-            class_count = Counter([sample["label"] for sample in ds])
-            num_classes = len(class_count)
-            total_samples = min(TEST_SAMPLES, len(ds))
-            samples_per_class = total_samples // num_classes
-
-            # Try to maintain class balance
-            balanced_samples = []
-            for label, count in class_count.items():
-                indices = [i for i, sample in enumerate(ds) if sample["label"] == label]
-                if count <= samples_per_class:
-                    balanced_samples.extend(indices)
-                else:
-                    balanced_samples.extend(random.sample(indices, samples_per_class))
-
-            # Add missing quantity since minority classes might have too few
-            if len(balanced_samples) < total_samples:
-                extra_samples_needed = total_samples - len(balanced_samples)
-                remaining_indices = [
-                    i for i in range(len(ds)) if i not in balanced_samples
-                ]
-                balanced_samples.extend(
-                    random.sample(remaining_indices, extra_samples_needed)
-                )
-
-            test_data = ds.select(balanced_samples)
-            self.dataset["test"] = test_data
-            assert (
-                len(test_data) == TEST_SAMPLES
-            ), f"Exceeded {TEST_SAMPLES} samples for 'test' split."
+        """This dataset consist of two columns of relevance, "original_sentence" and "corrected_sentence".
+        We will use the original sentence as we "wrong" sentence and the corrected sentence as the "correct" sentence
+        """
+
+        def __convert_sample_to_classification(sample):
+            text = sample["original_sentence"] + sample["corrected_sentence"]
+            label = [1] * len(sample["original_sentence"]) + [0] * len(
+                sample["corrected_sentence"]
+            )
+            return {"text": text, "label": label}
+
+        columns_to_keep = ["original_sentence", "corrected_sentence"]
+        for split in self.dataset:
+            columns_names = self.dataset[split].column_names  # type: ignore
+            columns_to_remove = [
+                col for col in columns_names if col not in columns_to_keep
+            ]
+            self.dataset[split] = self.dataset[split].remove_columns(columns_to_remove)  # type: ignore
+
+        self.dataset = self.dataset.map(
+            __convert_sample_to_classification,
+            batched=True,
+            remove_columns=columns_to_keep,
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mteb-1.7.9/mteb/tasks/Classification/zho/CMTEBClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/zho/CMTEBClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Classification/zho/YueOpenriceReviewClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/zho/YueOpenriceReviewClassification.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,7 +41,12 @@
 
     @property
     def metadata_dict(self) -> dict[str, str]:
         metadata_dict = super().metadata_dict
         metadata_dict["n_experiments"] = 10
         metadata_dict["samples_per_label"] = 32
         return metadata_dict
+
+    def dataset_transform(self):
+        self.dataset = self.stratified_subsampling(
+            self.dataset, seed=self.seed, splits=["test"]
+        )
```

### Comparing `mteb-1.7.9/mteb/tasks/Classification/zul/IsiZuluNewsClassification.py` & `mteb-1.8.0/mteb/tasks/Classification/zul/IsiZuluNewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Clustering/__init__.py` & `mteb-1.8.0/mteb/tasks/Clustering/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 from __future__ import annotations
 
 from .deu.BlurbsClusteringP2P import *
+from .deu.BlurbsClusteringP2PFast import *
 from .deu.BlurbsClusteringS2S import *
+from .deu.BlurbsClusteringS2SFast import *
 from .deu.TenKGnadClusteringP2P import *
+from .deu.TenKGnadClusteringP2PFast import *
 from .deu.TenKGnadClusteringS2S import *
+from .deu.TenKGnadClusteringS2SFast import *
 from .eng.ArxivClusteringP2P import *
+from .eng.ArxivClusteringP2PFast import *
 from .eng.ArxivClusteringS2S import *
 from .eng.BigPatentClustering import *
 from .eng.BiorxivClusteringP2P import *
 from .eng.BiorxivClusteringS2S import *
 from .eng.MedrxivClusteringP2P import *
 from .eng.MedrxivClusteringS2S import *
 from .eng.RedditClustering import *
@@ -16,19 +21,21 @@
 from .eng.StackExchangeClustering import *
 from .eng.StackExchangeClusteringP2P import *
 from .eng.TwentyNewsgroupsClustering import *
 from .eng.WikiCitiesClustering import *
 from .fra.AlloProfClusteringP2P import *
 from .fra.AlloProfClusteringS2S import *
 from .fra.HALClusteringS2S import *
-from .fra.MLSUMClusteringP2P import *
-from .fra.MLSUMClusteringS2S import *
+from .multilingual.IndicReviewsClusteringP2P import *
 from .multilingual.MasakhaNEWSClusteringP2P import *
 from .multilingual.MasakhaNEWSClusteringS2S import *
+from .multilingual.MLSUMClusteringP2P import *
+from .multilingual.MLSUMClusteringS2S import *
 from .nob.snl_clustering import *
 from .nob.vg_clustering import *
 from .pol.PolishClustering import *
 from .rom.RomaniBibleClustering import *
 from .spa.FloresClusteringS2S import *
 from .spa.SpanishNewsClusteringP2P import *
 from .swe.swedn_clustering import *
+from .swe.SwednClustering import *
 from .zho.CMTEBClustering import *
```

### Comparing `mteb-1.7.9/mteb/tasks/Clustering/deu/BlurbsClusteringP2P.py` & `mteb-1.8.0/mteb/tasks/Clustering/deu/BlurbsClusteringP2P.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 
 from mteb.abstasks.AbsTaskClustering import AbsTaskClustering
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 
 class BlurbsClusteringP2P(AbsTaskClustering):
+    superseeded_by = "BlurbsClusteringP2P.v2"
+
     metadata = TaskMetadata(
         name="BlurbsClusteringP2P",
         description="Clustering of book titles+blurbs. Clustering of 28 sets, either on the main or secondary genre.",
         reference="https://www.inf.uni-hamburg.de/en/inst/ab/lt/resources/data/germeval-2019-hmc.html",
         dataset={
             "path": "slvnwhrl/blurbs-clustering-p2p",
             "revision": "a2dd5b02a77de3466a3eaa98ae586b5610314496",
```

### Comparing `mteb-1.7.9/mteb/tasks/Clustering/deu/BlurbsClusteringS2S.py` & `mteb-1.8.0/mteb/tasks/Clustering/deu/BlurbsClusteringS2S.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskClustering import AbsTaskClustering
 
 
 class BlurbsClusteringS2S(AbsTaskClustering):
+    superseeded_by = "BlurbsClusteringS2S.v2"
+
     metadata = TaskMetadata(
         name="BlurbsClusteringS2S",
         description="Clustering of book titles. Clustering of 28 sets, either on the main or secondary genre.",
         reference="https://www.inf.uni-hamburg.de/en/inst/ab/lt/resources/data/germeval-2019-hmc.html",
         dataset={
             "path": "slvnwhrl/blurbs-clustering-s2s",
             "revision": "22793b6a6465bf00120ad525e38c51210858132c",
```

### Comparing `mteb-1.7.9/mteb/tasks/Clustering/deu/TenKGnadClusteringP2P.py` & `mteb-1.8.0/mteb/tasks/Clustering/deu/TenKGnadClusteringP2P.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskClustering import AbsTaskClustering
 
 
 class TenKGnadClusteringP2P(AbsTaskClustering):
+    superseeded_by = "TenKGnadClusteringP2P.v2"
+
     metadata = TaskMetadata(
         name="TenKGnadClusteringP2P",
         description="Clustering of news article titles+subheadings+texts. Clustering of 10 splits on the news article category.",
         reference="https://tblock.github.io/10kGNAD/",
         dataset={
             "path": "slvnwhrl/tenkgnad-clustering-p2p",
             "revision": "5c59e41555244b7e45c9a6be2d720ab4bafae558",
```

### Comparing `mteb-1.7.9/mteb/tasks/Clustering/deu/TenKGnadClusteringS2S.py` & `mteb-1.8.0/mteb/tasks/Clustering/deu/TenKGnadClusteringS2S.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskClustering import AbsTaskClustering
 
 
 class TenKGnadClusteringS2S(AbsTaskClustering):
+    superseeded_by = "TenKGnadClusteringS2S.v2"
+
     metadata = TaskMetadata(
         name="TenKGnadClusteringS2S",
         description="Clustering of news article titles. Clustering of 10 splits on the news article category.",
         reference="https://tblock.github.io/10kGNAD/",
         dataset={
             "path": "slvnwhrl/tenkgnad-clustering-s2s",
             "revision": "6cddbe003f12b9b140aec477b583ac4191f01786",
```

### Comparing `mteb-1.7.9/mteb/tasks/Clustering/eng/ArxivClusteringP2P.py` & `mteb-1.8.0/mteb/tasks/Clustering/eng/ArxivClusteringS2S.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskClustering import AbsTaskClustering
 
 
-class ArxivClusteringP2P(AbsTaskClustering):
+class ArxivClusteringS2S(AbsTaskClustering):
     metadata = TaskMetadata(
-        name="ArxivClusteringP2P",
-        description="Clustering of titles+abstract from arxiv. Clustering of 30 sets, either on the main or secondary category",
+        name="ArxivClusteringS2S",
+        description="Clustering of titles from arxiv. Clustering of 30 sets, either on the main or secondary category",
         reference="https://www.kaggle.com/Cornell-University/arxiv",
         dataset={
-            "path": "mteb/arxiv-clustering-p2p",
-            "revision": "a122ad7f3f0291bf49cc6f4d32aa80929df69d5d",
+            "path": "mteb/arxiv-clustering-s2s",
+            "revision": "f910caf1a6075f7329cdf8c1a6135696f37dbd53",
         },
         type="Clustering",
-        category="p2p",
+        category="s2s",
         eval_splits=["test"],
         eval_langs=["eng-Latn"],
         main_score="v_measure",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
         n_samples={"test": 732723},
-        avg_character_length={"test": 1009.98},
+        avg_character_length={"test": 74},
     )
```

### Comparing `mteb-1.7.9/mteb/tasks/Clustering/eng/ArxivClusteringS2S.py` & `mteb-1.8.0/mteb/tasks/Clustering/eng/BiorxivClusteringP2P.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 from __future__ import annotations
 
+from mteb.abstasks.AbsTaskClustering import AbsTaskClustering
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks.AbsTaskClustering import AbsTaskClustering
 
-
-class ArxivClusteringS2S(AbsTaskClustering):
+class BiorxivClusteringP2P(AbsTaskClustering):
     metadata = TaskMetadata(
-        name="ArxivClusteringS2S",
-        description="Clustering of titles from arxiv. Clustering of 30 sets, either on the main or secondary category",
-        reference="https://www.kaggle.com/Cornell-University/arxiv",
+        name="BiorxivClusteringP2P",
+        description="Clustering of titles+abstract from biorxiv. Clustering of 10 sets, based on the main category.",
+        reference="https://api.biorxiv.org/",
         dataset={
-            "path": "mteb/arxiv-clustering-s2s",
-            "revision": "f910caf1a6075f7329cdf8c1a6135696f37dbd53",
+            "path": "mteb/biorxiv-clustering-p2p",
+            "revision": "65b79d1d13f80053f67aca9498d9402c2d9f1f40",
         },
         type="Clustering",
-        category="s2s",
+        category="p2p",
         eval_splits=["test"],
         eval_langs=["eng-Latn"],
         main_score="v_measure",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples={"test": 732723},
-        avg_character_length={"test": 74},
+        n_samples={"test": 75000},
+        avg_character_length={"test": 1666.2},
     )
```

### Comparing `mteb-1.7.9/mteb/tasks/Clustering/eng/BigPatentClustering.py` & `mteb-1.8.0/mteb/tasks/Clustering/eng/BigPatentClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Clustering/eng/BiorxivClusteringP2P.py` & `mteb-1.8.0/mteb/tasks/Clustering/eng/StackExchangeClusteringP2P.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from __future__ import annotations
 
-from mteb.abstasks.AbsTaskClustering import AbsTaskClustering
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
+from ....abstasks.AbsTaskClustering import AbsTaskClustering
 
-class BiorxivClusteringP2P(AbsTaskClustering):
+
+class StackExchangeClusteringP2P(AbsTaskClustering):
     metadata = TaskMetadata(
-        name="BiorxivClusteringP2P",
-        description="Clustering of titles+abstract from biorxiv. Clustering of 10 sets, based on the main category.",
-        reference="https://api.biorxiv.org/",
+        name="StackExchangeClusteringP2P",
+        description="Clustering of title+body from stackexchange. Clustering of 5 sets of 10k paragraphs and 5 sets of 5k paragraphs.",
+        reference="https://arxiv.org/abs/2104.07081",
         dataset={
-            "path": "mteb/biorxiv-clustering-p2p",
-            "revision": "65b79d1d13f80053f67aca9498d9402c2d9f1f40",
+            "path": "mteb/stackexchange-clustering-p2p",
+            "revision": "815ca46b2622cec33ccafc3735d572c266efdb44",
         },
         type="Clustering",
         category="p2p",
         eval_splits=["test"],
         eval_langs=["eng-Latn"],
         main_score="v_measure",
         date=None,
@@ -25,9 +26,9 @@
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
         n_samples={"test": 75000},
-        avg_character_length={"test": 1666.2},
+        avg_character_length={"test": 1090.7},
     )
```

### Comparing `mteb-1.7.9/mteb/tasks/Clustering/eng/BiorxivClusteringS2S.py` & `mteb-1.8.0/mteb/tasks/Clustering/eng/BiorxivClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Clustering/eng/MedrxivClusteringP2P.py` & `mteb-1.8.0/mteb/tasks/Clustering/eng/MedrxivClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Clustering/eng/MedrxivClusteringS2S.py` & `mteb-1.8.0/mteb/tasks/Clustering/eng/MedrxivClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Clustering/eng/RedditClustering.py` & `mteb-1.8.0/mteb/tasks/Clustering/eng/RedditClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Clustering/eng/RedditClusteringP2P.py` & `mteb-1.8.0/mteb/tasks/Clustering/eng/RedditClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Clustering/eng/StackExchangeClustering.py` & `mteb-1.8.0/mteb/tasks/Clustering/eng/StackExchangeClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Clustering/eng/StackExchangeClusteringP2P.py` & `mteb-1.8.0/mteb/tasks/Clustering/eng/ArxivClusteringP2P.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskClustering import AbsTaskClustering
 
 
-class StackExchangeClusteringP2P(AbsTaskClustering):
+class ArxivClusteringP2P(AbsTaskClustering):
+    superseeded_by = "ArxivClusteringP2P.v2"
+
     metadata = TaskMetadata(
-        name="StackExchangeClusteringP2P",
-        description="Clustering of title+body from stackexchange. Clustering of 5 sets of 10k paragraphs and 5 sets of 5k paragraphs.",
-        reference="https://arxiv.org/abs/2104.07081",
+        name="ArxivClusteringP2P",
+        description="Clustering of titles+abstract from arxiv. Clustering of 30 sets, either on the main or secondary category",
+        reference="https://www.kaggle.com/Cornell-University/arxiv",
         dataset={
-            "path": "mteb/stackexchange-clustering-p2p",
-            "revision": "815ca46b2622cec33ccafc3735d572c266efdb44",
+            "path": "mteb/arxiv-clustering-p2p",
+            "revision": "a122ad7f3f0291bf49cc6f4d32aa80929df69d5d",
         },
         type="Clustering",
         category="p2p",
         eval_splits=["test"],
         eval_langs=["eng-Latn"],
         main_score="v_measure",
         date=None,
@@ -25,10 +27,10 @@
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples={"test": 75000},
-        avg_character_length={"test": 1090.7},
+        n_samples={"test": 732723},
+        avg_character_length={"test": 1009.98},
     )
```

### Comparing `mteb-1.7.9/mteb/tasks/Clustering/eng/TwentyNewsgroupsClustering.py` & `mteb-1.8.0/mteb/tasks/Clustering/eng/TwentyNewsgroupsClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Clustering/eng/WikiCitiesClustering.py` & `mteb-1.8.0/mteb/tasks/Clustering/eng/WikiCitiesClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Clustering/fra/AlloProfClusteringP2P.py` & `mteb-1.8.0/mteb/tasks/Clustering/fra/AlloProfClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Clustering/fra/AlloProfClusteringS2S.py` & `mteb-1.8.0/mteb/tasks/Clustering/fra/AlloProfClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Clustering/fra/HALClusteringS2S.py` & `mteb-1.8.0/mteb/tasks/Clustering/fra/HALClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Clustering/fra/MLSUMClusteringP2P.py` & `mteb-1.8.0/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,51 @@
 from __future__ import annotations
 
 import datasets
 import numpy as np
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks.AbsTaskClustering import AbsTaskClustering
+from ....abstasks import AbsTaskClustering, MultilingualTask
 
+_LANGUAGES = {
+    "amh": ["amh-Ethi"],
+    "eng": ["eng-Latn"],
+    "fra": ["fra-Latn"],
+    "hau": ["hau-Latn"],
+    "ibo": ["ibo-Latn"],
+    "lin": ["lin-Latn"],
+    "lug": ["lug-Latn"],
+    "orm": ["orm-Ethi"],
+    "pcm": ["pcm-Latn"],
+    "run": ["run-Latn"],
+    "sna": ["sna-Latn"],
+    "som": ["som-Latn"],
+    "swa": ["swa-Latn"],
+    "tir": ["tir-Ethi"],
+    "xho": ["xho-Latn"],
+    "yor": ["yor-Latn"],
+}
 
-class MLSUMClusteringP2P(AbsTaskClustering):
+
+class MasakhaNEWSClusteringS2S(AbsTaskClustering, MultilingualTask):
     metadata = TaskMetadata(
-        name="MLSUMClusteringP2P",
-        description="Clustering of newspaper article contents and titles from MLSUM dataset. Clustering of 10 sets on the newpaper article topics.",
-        reference="https://huggingface.co/datasets/mlsum",
+        name="MasakhaNEWSClusteringS2S",
         dataset={
-            "path": "mlsum",
-            "revision": "b5d54f8f3b61ae17845046286940f03c6bc79bc7",
-            "name": "fr",
-            "trust_remote_code": True,
+            "path": "masakhane/masakhanews",
+            "revision": "8ccc72e69e65f40c70e117d8b3c08306bb788b60",
         },
+        description=(
+            "Clustering of news article headlines from MasakhaNEWS dataset. Clustering of 10 sets on the news article label."
+        ),
+        reference="https://huggingface.co/datasets/masakhane/masakhanews",
         type="Clustering",
-        category="p2p",
+        category="s2s",
         eval_splits=["test"],
-        eval_langs=["fra-Latn"],
+        eval_langs=_LANGUAGES,
         main_score="v_measure",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
@@ -38,33 +57,31 @@
         avg_character_length=None,
     )
 
     def load_data(self, **kwargs):
         """Load dataset from HuggingFace hub and convert it to the standard format."""
         if self.data_loaded:
             return
-        self.dataset = datasets.load_dataset(
-            self.metadata.dataset["path"],
-            self.metadata.dataset["name"],
-            split=self.metadata.eval_splits[0],
-            revision=self.metadata.dataset["revision"],
-        )
-        self.dataset_transform()
+        self.dataset = {}
+        for lang in self.langs:
+            self.dataset[lang] = datasets.load_dataset(
+                name=lang,
+                **self.metadata_dict["dataset"],
+            )
+            self.dataset_transform(lang)
         self.data_loaded = True
 
-    def create_description(self, example):
-        example["text"] = example["title"] + " " + example["text"]
-        return example
-
-    def dataset_transform(self):
+    def dataset_transform(self, lang):
         """Convert to standard format"""
-        self.dataset = self.dataset.map(self.create_description)
-        self.dataset = self.dataset.remove_columns(["summary", "url", "date", "title"])
-        texts = self.dataset["text"]
-        topics = self.dataset["topic"]
+        self.dataset[lang].pop("train")
+        self.dataset[lang].pop("validation")
+
+        self.dataset[lang] = self.dataset[lang].remove_columns(
+            ["url", "text", "headline_text"]
+        )
+        texts = self.dataset[lang]["test"]["headline"]
+        labels = self.dataset[lang]["test"]["label"]
         new_format = {
-            "sentences": [split.tolist() for split in np.array_split(texts, 10)],
-            "labels": [split.tolist() for split in np.array_split(topics, 10)],
-        }
-        self.dataset = {
-            self.metadata_dict["eval_splits"][0]: datasets.Dataset.from_dict(new_format)
+            "sentences": [split.tolist() for split in np.array_split(texts, 5)],
+            "labels": [split.tolist() for split in np.array_split(labels, 5)],
         }
+        self.dataset[lang]["test"] = datasets.Dataset.from_dict(new_format)
```

### Comparing `mteb-1.7.9/mteb/tasks/Clustering/fra/MLSUMClusteringS2S.py` & `mteb-1.8.0/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2S.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 from __future__ import annotations
 
 import datasets
-import numpy as np
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks.AbsTaskClustering import AbsTaskClustering
+from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class MLSUMClusteringS2S(AbsTaskClustering):
+class SpanishPassageRetrievalS2S(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="MLSUMClusteringS2S",
-        description="Clustering of newspaper article contents and titles from MLSUM dataset. Clustering of 10 sets on the newpaper article topics.",
-        reference="https://huggingface.co/datasets/mlsum",
+        name="SpanishPassageRetrievalS2S",
+        description="Test collection for passage retrieval from health-related Web resources in Spanish.",
+        reference="https://mklab.iti.gr/results/spanish-passage-retrieval-dataset/",
         dataset={
-            "path": "mlsum",
-            "revision": "b5d54f8f3b61ae17845046286940f03c6bc79bc7",
-            "name": "fr",
+            "path": "jinaai/spanish_passage_retrieval",
+            "revision": "9cddf2ce5209ade52c2115ccfa00eb22c6d3a837",
             "trust_remote_code": True,
         },
-        type="Clustering",
+        type="Retrieval",
         category="s2s",
         eval_splits=["test"],
-        eval_langs=["fra-Latn"],
-        main_score="v_measure",
+        eval_langs=["spa-Latn"],
+        main_score="ndcg_at_10",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -35,33 +33,35 @@
         text_creation=None,
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
     def load_data(self, **kwargs):
-        """Load dataset from HuggingFace hub and convert it to the standard format."""
         if self.data_loaded:
             return
-        self.dataset = datasets.load_dataset(
-            self.metadata.dataset["path"],
-            self.metadata.dataset["name"],
-            split=self.metadata.eval_splits[0],
-            revision=self.metadata.dataset["revision"],
+
+        query_rows = datasets.load_dataset(
+            name="queries",
+            split="test",
+            **self.metadata_dict["dataset"],
+        )
+        corpus_rows = datasets.load_dataset(
+            name="corpus.sentences",
+            split="test",
+            **self.metadata_dict["dataset"],
+        )
+        qrels_rows = datasets.load_dataset(
+            name="qrels.s2s",
+            split="test",
+            **self.metadata_dict["dataset"],
         )
-        self.dataset_transform()
-        self.data_loaded = True
 
-    def dataset_transform(self):
-        """Convert to standard format"""
-        self.dataset = self.dataset.remove_columns(["summary", "text", "url", "date"])
-        new_format = {
-            "sentences": [
-                split.tolist() for split in np.array_split(self.dataset["title"], 10)
-            ],
-            "labels": [
-                split.tolist() for split in np.array_split(self.dataset["topic"], 10)
-            ],
-        }
-        self.dataset = {
-            self.metadata_dict["eval_splits"][0]: datasets.Dataset.from_dict(new_format)
+        self.queries = {"test": {row["_id"]: row["text"] for row in query_rows}}
+        self.corpus = {"test": {row["_id"]: row for row in corpus_rows}}
+        self.relevant_docs = {
+            "test": {
+                row["_id"]: {v: 1 for v in row["text"].split(" ")} for row in qrels_rows
+            }
         }
+
+        self.data_loaded = True
```

### Comparing `mteb-1.7.9/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py` & `mteb-1.8.0/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py` & `mteb-1.8.0/mteb/tasks/Retrieval/deu/GermanQuADRetrieval.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,50 @@
 from __future__ import annotations
 
-import datasets
-import numpy as np
+from collections import defaultdict
+
+from datasets import DatasetDict, load_dataset
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks import AbsTaskClustering, MultilingualTask
+from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
+
+
+def load_retrieval_data(dataset_path, eval_splits):
+    eval_split = eval_splits[0]
+    corpus_dataset = load_dataset(dataset_path, "corpus")
+    queries_dataset = load_dataset(dataset_path, "queries")
+    qrels = load_dataset(dataset_path + "-qrels")[eval_split]
+
+    corpus = {e["_id"]: {"text": e["text"]} for e in corpus_dataset["corpus"]}
+    queries = {e["_id"]: e["text"] for e in queries_dataset["queries"]}
+    relevant_docs = defaultdict(dict)
+    for e in qrels:
+        relevant_docs[e["query-id"]][e["corpus-id"]] = e["score"]
 
-_LANGUAGES = {
-    "amh": ["amh-Ethi"],
-    "eng": ["eng-Latn"],
-    "fra": ["fra-Latn"],
-    "hau": ["hau-Latn"],
-    "ibo": ["ibo-Latn"],
-    "lin": ["lin-Latn"],
-    "lug": ["lug-Latn"],
-    "orm": ["orm-Ethi"],
-    "pcm": ["pcm-Latn"],
-    "run": ["run-Latn"],
-    "sna": ["sna-Latn"],
-    "som": ["som-Latn"],
-    "swa": ["swa-Latn"],
-    "tir": ["tir-Ethi"],
-    "xho": ["xho-Latn"],
-    "yor": ["yor-Latn"],
-}
+    corpus = DatasetDict({eval_split: corpus})
+    queries = DatasetDict({eval_split: queries})
+    relevant_docs = DatasetDict({eval_split: relevant_docs})
+    return corpus, queries, relevant_docs
 
 
-class MasakhaNEWSClusteringS2S(AbsTaskClustering, MultilingualTask):
+class GermanQuADRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="MasakhaNEWSClusteringS2S",
+        name="GermanQuAD-Retrieval",
+        description="Context Retrieval for German Question Answering",
+        reference="https://www.kaggle.com/datasets/GermanQuAD",
         dataset={
-            "path": "masakhane/masakhanews",
-            "revision": "8ccc72e69e65f40c70e117d8b3c08306bb788b60",
+            "path": "mteb/germanquad-retrieval",
+            "revision": "f5c87ae5a2e7a5106606314eef45255f03151bb3",
         },
-        description=(
-            "Clustering of news article headlines from MasakhaNEWS dataset. Clustering of 10 sets on the news article label."
-        ),
-        reference="https://huggingface.co/datasets/masakhane/masakhanews",
-        type="Clustering",
-        category="s2s",
+        type="Retrieval",
+        category="s2p",
         eval_splits=["test"],
-        eval_langs=_LANGUAGES,
-        main_score="v_measure",
+        eval_langs=["deu-Latn"],
+        main_score="mrr_at_5",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -54,34 +52,14 @@
         text_creation=None,
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
     def load_data(self, **kwargs):
-        """Load dataset from HuggingFace hub and convert it to the standard format."""
         if self.data_loaded:
             return
-        self.dataset = {}
-        for lang in self.langs:
-            self.dataset[lang] = datasets.load_dataset(
-                name=lang,
-                **self.metadata_dict["dataset"],
-            )
-            self.dataset_transform(lang)
-        self.data_loaded = True
-
-    def dataset_transform(self, lang):
-        """Convert to standard format"""
-        self.dataset[lang].pop("train")
-        self.dataset[lang].pop("validation")
 
-        self.dataset[lang] = self.dataset[lang].remove_columns(
-            ["url", "text", "headline_text"]
+        self.corpus, self.queries, self.relevant_docs = load_retrieval_data(
+            self.metadata_dict["dataset"]["path"], self.metadata_dict["eval_splits"]
         )
-        texts = self.dataset[lang]["test"]["headline"]
-        labels = self.dataset[lang]["test"]["label"]
-        new_format = {
-            "sentences": [split.tolist() for split in np.array_split(texts, 5)],
-            "labels": [split.tolist() for split in np.array_split(labels, 5)],
-        }
-        self.dataset[lang]["test"] = datasets.Dataset.from_dict(new_format)
+        self.data_loaded = True
```

### Comparing `mteb-1.7.9/mteb/tasks/Clustering/multilingual/WikiClusteringP2P.py` & `mteb-1.8.0/mteb/tasks/Clustering/multilingual/WikiClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Clustering/nob/snl_clustering.py` & `mteb-1.8.0/mteb/tasks/Clustering/nob/snl_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Clustering/nob/vg_clustering.py` & `mteb-1.8.0/mteb/tasks/Clustering/nob/vg_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Clustering/pol/PolishClustering.py` & `mteb-1.8.0/mteb/tasks/Clustering/spa/FloresClusteringS2S.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskClustering import AbsTaskClustering
 
 
-class EightTagsClustering(AbsTaskClustering):
+class FloresClusteringS2S(AbsTaskClustering):
     metadata = TaskMetadata(
-        name="EightTagsClustering",
-        description="Clustering of headlines from social media posts in Polish belonging to 8 categories: film, history, "
-        "food, medicine, motorization, work, sport and technology.",
-        reference="https://aclanthology.org/2020.lrec-1.207.pdf",
+        name="FloresClusteringS2S",
+        description="Clustering of sentences from various web articles, 32 topics in total.",
+        reference="https://huggingface.co/datasets/facebook/flores",
         dataset={
-            "path": "PL-MTEB/8tags-clustering",
-            "revision": "78b962b130c6690659c65abf67bf1c2f030606b6",
+            "path": "jinaai/flores_clustering",
+            "revision": "97faaf98d7ef21869d176115e669e2a4286513bf",
         },
         type="Clustering",
         category="s2s",
         eval_splits=["test"],
-        eval_langs=["pol-Latn"],
+        eval_langs=["spa-Latn"],
         main_score="v_measure",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
```

### Comparing `mteb-1.7.9/mteb/tasks/Clustering/rom/RomaniBibleClustering.py` & `mteb-1.8.0/mteb/tasks/Clustering/rom/RomaniBibleClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Clustering/spa/FloresClusteringS2S.py` & `mteb-1.8.0/mteb/tasks/Clustering/spa/SpanishNewsClusteringP2P.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskClustering import AbsTaskClustering
 
 
-class FloresClusteringS2S(AbsTaskClustering):
+class SpanishNewsClusteringP2P(AbsTaskClustering):
     metadata = TaskMetadata(
-        name="FloresClusteringS2S",
-        description="Clustering of sentences from various web articles, 32 topics in total.",
-        reference="https://huggingface.co/datasets/facebook/flores",
+        name="SpanishNewsClusteringP2P",
+        description="Clustering of news articles, 7 topics in total.",
+        reference="https://www.kaggle.com/datasets/kevinmorgado/spanish-news-classification",
         dataset={
-            "path": "jinaai/flores_clustering",
-            "revision": "97faaf98d7ef21869d176115e669e2a4286513bf",
+            "path": "jinaai/spanish_news_clustering",
+            "revision": "bf8ca8ddc5b7da4f7004720ddf99bbe0483480e6",
         },
         type="Clustering",
-        category="s2s",
+        category="p2p",
         eval_splits=["test"],
         eval_langs=["spa-Latn"],
         main_score="v_measure",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
```

### Comparing `mteb-1.7.9/mteb/tasks/Clustering/spa/SpanishNewsClusteringP2P.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/CQADupstackGisRetrieval.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks.AbsTaskClustering import AbsTaskClustering
+from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class SpanishNewsClusteringP2P(AbsTaskClustering):
+class CQADupstackGisRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="SpanishNewsClusteringP2P",
-        description="Clustering of news articles, 7 topics in total.",
-        reference="https://www.kaggle.com/datasets/kevinmorgado/spanish-news-classification",
+        name="CQADupstackGisRetrieval",
+        description="CQADupStack: A Benchmark Data Set for Community Question-Answering Research",
+        reference="http://nlp.cis.unimelb.edu.au/resources/cqadupstack/",
         dataset={
-            "path": "jinaai/spanish_news_clustering",
-            "revision": "bf8ca8ddc5b7da4f7004720ddf99bbe0483480e6",
+            "path": "mteb/cqadupstack-gis",
+            "revision": "5003b3064772da1887988e05400cf3806fe491f2",
         },
-        type="Clustering",
-        category="p2p",
+        type="Retrieval",
+        category="s2p",
         eval_splits=["test"],
-        eval_langs=["spa-Latn"],
-        main_score="v_measure",
+        eval_langs=["eng-Latn"],
+        main_score="ndcg_at_10",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.7.9/mteb/tasks/Clustering/swe/swedn_clustering.py` & `mteb-1.8.0/mteb/tasks/Clustering/swe/swedn_clustering.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,16 @@
         raise ValueError("n must be at least one")
     it = iter(iterable)
     while batch := tuple(islice(it, n)):
         yield batch
 
 
 class SwednClustering(AbsTaskClustering):
+    superseeded_by = "SwednClusteringP2P"
+
     metadata = TaskMetadata(
         name="SwednClustering",
         dataset={
             "path": "sbx/superlim-2",
             "revision": "ef1661775d746e0844b299164773db733bdc0bf6",
             "name": "swedn",
         },
@@ -62,37 +64,39 @@
         splits = ["train", "validation"]
         # performance of sample models with test set: 8.74, 2.43 -removing test-> 11.26, 4.27
         # this is due to the test set only having 1 cluster which is "other"
 
         headlines = []
         summaries = []
         articles = []
-        labels = []
+        headline_labels = []
+        sammary_labels = []
+        article_labels = []
         label_col = "article_category"
 
         for split in splits:
             ds_split = self.dataset[split]
             headlines.extend(ds_split["headline"])
-            labels.extend(ds_split[label_col])
+            headline_labels.extend(ds_split[label_col])
 
             summaries.extend(ds_split["summary"])
-            labels.extend(ds_split[label_col])
+            sammary_labels.extend(ds_split[label_col])
 
             articles.extend(ds_split["article"])
-            labels.extend(ds_split[label_col])
+            article_labels.extend(ds_split[label_col])
 
         rng = random.Random(42)  # local only seed
 
         clusters_text = []
         clusters_labels = []
-        doc_types = [summaries, articles]
+        doc_types = [(summaries, sammary_labels), (articles, article_labels)]
         # Note that headlines is excluded:
         # Scores of sample models with headlines: 11.26, 4.27 -removing headlines-> 16.43, 4.31
         # as headlines are soo short it is hard to meaningfully cluster them even for humans.
-        for text in doc_types:
+        for text, labels in doc_types:
             pairs = list(zip(text, labels))
             rng.shuffle(pairs)
             # reduce size of dataset to not have too large datasets in the clustering task
             pairs_batched = list(batched(pairs, 512))
             texts1, labels2 = list(zip(*pairs_batched[0]))
             texts2, labels2 = list(zip(*pairs_batched[1]))
```

### Comparing `mteb-1.7.9/mteb/tasks/Clustering/zho/CMTEBClustering.py` & `mteb-1.8.0/mteb/tasks/Clustering/zho/CMTEBClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/InstructionRetrieval/eng/Core17InstructionRetrieval.py` & `mteb-1.8.0/mteb/tasks/InstructionRetrieval/eng/News21InstructionRetrieval.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskInstructionRetrieval import AbsTaskInstructionRetrieval
 
 
-class Core17InstructionRetrieval(AbsTaskInstructionRetrieval):
+class News21InstructionRetrieval(AbsTaskInstructionRetrieval):
     metadata = TaskMetadata(
-        name="Core17InstructionRetrieval",
-        description="Measuring retrieval instruction following ability on Core17 narratives.",
+        name="News21InstructionRetrieval",
+        description="Measuring retrieval instruction following ability on News21 narratives.",
         reference="https://arxiv.org/abs/2403.15246",
         dataset={
-            "path": "jhu-clsp/core17-instructions",
-            "revision": "e783a88ec6bc4bbdc1ba998edd85edeaf3d820f7",
+            "path": "jhu-clsp/news21-instructions",
+            "revision": "e0144086b45fe31ac125e9ac1a83b6a409bb6ca6",
         },
         type="InstructionRetrieval",
         category="s2p",
         eval_splits=["test"],
         eval_langs=["eng-Latn"],
         main_score="p-MRR",
         date=("2023-08-01", "2024-04-01"),
@@ -32,10 +32,10 @@
       title={FollowIR: Evaluating and Teaching Information Retrieval Models to Follow Instructions}, 
       author={Orion Weller and Benjamin Chang and Sean MacAvaney and Kyle Lo and Arman Cohan and Benjamin Van Durme and Dawn Lawrie and Luca Soldaini},
       year={2024},
       eprint={2403.15246},
       archivePrefix={arXiv},
       primaryClass={cs.IR}
 }""",
-        n_samples={"eng": 19735 * 2},
-        avg_character_length={"eng": 2747.2883966244726},
+        n_samples={"eng": 30953 * 2},
+        avg_character_length={"eng": 2983.724665391969},
     )
```

### Comparing `mteb-1.7.9/mteb/tasks/InstructionRetrieval/eng/News21InstructionRetrieval.py` & `mteb-1.8.0/mteb/tasks/InstructionRetrieval/eng/Robust04InstructionRetrieval.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskInstructionRetrieval import AbsTaskInstructionRetrieval
 
 
-class News21InstructionRetrieval(AbsTaskInstructionRetrieval):
+class Robust04InstructionRetrieval(AbsTaskInstructionRetrieval):
     metadata = TaskMetadata(
-        name="News21InstructionRetrieval",
-        description="Measuring retrieval instruction following ability on News21 narratives.",
+        name="Robust04InstructionRetrieval",
+        description="Measuring retrieval instruction following ability on Robust04 narratives.",
         reference="https://arxiv.org/abs/2403.15246",
         dataset={
-            "path": "jhu-clsp/news21-instructions",
-            "revision": "fae860d870141ee0f34fbab67314c65f41921943",
+            "path": "jhu-clsp/robust04-instructions",
+            "revision": "a5a1c4fe2bc528ac12e83f8cdf82178da85d2f1d",
         },
         type="InstructionRetrieval",
         category="s2p",
         eval_splits=["test"],
         eval_langs=["eng-Latn"],
         main_score="p-MRR",
         date=("2023-08-01", "2024-04-01"),
@@ -32,10 +32,10 @@
       title={FollowIR: Evaluating and Teaching Information Retrieval Models to Follow Instructions}, 
       author={Orion Weller and Benjamin Chang and Sean MacAvaney and Kyle Lo and Arman Cohan and Benjamin Van Durme and Dawn Lawrie and Luca Soldaini},
       year={2024},
       eprint={2403.15246},
       archivePrefix={arXiv},
       primaryClass={cs.IR}
 }""",
-        n_samples={"eng": 30129 * 2},
-        avg_character_length={"eng": 2331.381203215969},
+        n_samples={"eng": 47544 * 2},
+        avg_character_length={"eng": 2471.0398058252426},
     )
```

### Comparing `mteb-1.7.9/mteb/tasks/InstructionRetrieval/eng/Robust04InstructionRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/deu/GerDaLIRSmallRetrieval.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,34 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks.AbsTaskInstructionRetrieval import AbsTaskInstructionRetrieval
+from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class Robust04InstructionRetrieval(AbsTaskInstructionRetrieval):
+class GerDaLIRSmall(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="Robust04InstructionRetrieval",
-        description="Measuring retrieval instruction following ability on Robust04 narratives.",
-        reference="https://arxiv.org/abs/2403.15246",
+        name="GerDaLIRSmall",
+        description="The dataset consists of documents, passages and relevance labels in German. In contrast to the original dataset, only documents that have corresponding queries in the query set are chosen to create a smaller corpus for evaluation purposes.",
+        reference="https://github.com/lavis-nlp/GerDaLIR",
         dataset={
-            "path": "jhu-clsp/robust04-instructions",
-            "revision": "d25e82647b09251f4feaaf5462c9a18445072ba6",
+            "path": "mteb/GerDaLIRSmall",
+            "revision": "48327de6ee192e9610f3069789719788957c7abd",
         },
-        type="InstructionRetrieval",
-        category="s2p",
+        type="Retrieval",
+        category="p2p",
         eval_splits=["test"],
-        eval_langs=["eng-Latn"],
-        main_score="p-MRR",
-        date=("2023-08-01", "2024-04-01"),
+        eval_langs=["deu-Latn"],
+        main_score="ndcg_at_10",
+        date=None,
         form=["written"],
-        domains=["News"],
-        task_subtypes=[],
-        license="MIT",
-        socioeconomic_status="medium",
+        domains=["Legal"],
+        task_subtypes=["Article retrieval"],
+        license="MIT license",
+        socioeconomic_status="high",
         annotations_creators="derived",
-        dialect=[],
+        dialect=None,
         text_creation="found",
-        bibtex_citation="""@misc{weller2024followir,
-      title={FollowIR: Evaluating and Teaching Information Retrieval Models to Follow Instructions}, 
-      author={Orion Weller and Benjamin Chang and Sean MacAvaney and Kyle Lo and Arman Cohan and Benjamin Van Durme and Dawn Lawrie and Luca Soldaini},
-      year={2024},
-      eprint={2403.15246},
-      archivePrefix={arXiv},
-      primaryClass={cs.IR}
-}""",
-        n_samples={"eng": 42645 * 2},
-        avg_character_length={"eng": 2680.043891349965},
+        bibtex_citation=None,
+        n_samples=None,
+        avg_character_length=None,
     )
```

### Comparing `mteb-1.7.9/mteb/tasks/PairClassification/deu/FalseFriendsDeEnPC.py` & `mteb-1.8.0/mteb/tasks/PairClassification/deu/FalseFriendsDeEnPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/PairClassification/eng/SprintDuplicateQuestionsPC.py` & `mteb-1.8.0/mteb/tasks/PairClassification/eng/SprintDuplicateQuestionsPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/PairClassification/eng/TwitterSemEval2015PC.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/MSMARCORetrieval.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks.AbsTaskPairClassification import AbsTaskPairClassification
+from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class TwitterSemEval2015PC(AbsTaskPairClassification):
+class MSMARCO(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="TwitterSemEval2015",
+        name="MSMARCO",
         dataset={
-            "path": "mteb/twittersemeval2015-pairclassification",
-            "revision": "70970daeab8776df92f5ea462b6173c0b46fd2d1",
+            "path": "mteb/msmarco",
+            "revision": "c5a29a104738b98a9e76336939199e264163d4a0",
         },
-        description="Paraphrase-Pairs of Tweets from the SemEval 2015 workshop.",
-        reference="https://alt.qcri.org/semeval2015/task1/",
-        category="s2s",
-        type="PairClassification",
-        eval_splits=["test"],
+        description="MS MARCO is a collection of datasets focused on deep learning in search",
+        reference="https://microsoft.github.io/msmarco/",
+        type="Retrieval",
+        category="s2p",
+        eval_splits=["train", "dev", "test"],
         eval_langs=["eng-Latn"],
-        main_score="ap",
+        main_score="ndcg_at_10",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples={"test": 16777},
-        avg_character_length={"test": 38.3},
+        n_samples=None,
+        avg_character_length=None,
     )
```

### Comparing `mteb-1.7.9/mteb/tasks/PairClassification/eng/TwitterURLCorpusPC.py` & `mteb-1.8.0/mteb/tasks/PairClassification/eng/TwitterURLCorpusPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py` & `mteb-1.8.0/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/PairClassification/multilingual/PawsX.py` & `mteb-1.8.0/mteb/tasks/PairClassification/multilingual/PawsX.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/PairClassification/pol/PolishPC.py` & `mteb-1.8.0/mteb/tasks/PairClassification/pol/PolishPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/PairClassification/zho/CMTEBPairClassification.py` & `mteb-1.8.0/mteb/tasks/PairClassification/zho/CMTEBPairClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Reranking/eng/AskUbuntuDupQuestions.py` & `mteb-1.8.0/mteb/tasks/Reranking/eng/AskUbuntuDupQuestions.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Reranking/eng/MindSmallReranking.py` & `mteb-1.8.0/mteb/tasks/Reranking/eng/MindSmallReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Reranking/eng/SciDocsReranking.py` & `mteb-1.8.0/mteb/tasks/Reranking/eng/SciDocsReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Reranking/eng/StackOverflowDupQuestions.py` & `mteb-1.8.0/mteb/tasks/Reranking/eng/StackOverflowDupQuestions.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Reranking/fra/AlloprofReranking.py` & `mteb-1.8.0/mteb/tasks/Reranking/fra/AlloprofReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Reranking/fra/SyntecReranking.py` & `mteb-1.8.0/mteb/tasks/Reranking/fra/SyntecReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Reranking/multilingual/MIRACLReranking.py` & `mteb-1.8.0/mteb/tasks/Reranking/multilingual/MIRACLReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Reranking/zho/CMTEBReranking.py` & `mteb-1.8.0/mteb/tasks/Reranking/zho/CMTEBReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/__init__.py` & `mteb-1.8.0/mteb/tasks/Retrieval/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from __future__ import annotations
 
+from .code.CodeEditSearchRetrieval import *
 from .code.CodeSearchNetRetrieval import *
 from .dan.dan_fever import *
 from .dan.t2nord_retrieval import *
 from .dan.twitterhjerne import *
 from .deu.GerDaLIRRetrieval import *
 from .deu.GerDaLIRSmallRetrieval import *
 from .deu.GermanDPRRetrieval import *
 from .deu.GermanQuADRetrieval import *
 from .deu.LegalQuADRetrieval import *
+from .ell.GreekCivicsQA import *
 from .eng.AILACasedocsRetrieval import *
 from .eng.AILAStatutesRetrieval import *
 from .eng.ArguAnaRetrieval import *
 from .eng.ClimateFEVERRetrieval import *
 from .eng.CQADupstackAndroidRetrieval import *
 from .eng.CQADupstackEnglishRetrieval import *
 from .eng.CQADupstackGamingRetrieval import *
@@ -53,36 +55,42 @@
 from .est.estqa import *
 from .fra.AlloprofRetrieval import *
 from .fra.BSARDRetrieval import *
 from .fra.FQuADRetrieval import *
 from .fra.SyntecRetrieval import *
 from .hun.HunSum2 import *
 from .jpn.JaQuADRetrieval import *
+from .kat.GeorgianFAQRetrieval import *
 from .kor.KoMiracl import *
 from .kor.KoStrategyQA import *
+from .multilingual.IndicQARetrieval import *
 from .multilingual.MintakaRetrieval import *
 from .multilingual.MIRACLRetrieval import *
+from .multilingual.MLQARetrieval import *
 from .multilingual.MultiLongDocRetrieval import *
 from .multilingual.NeuCLIR2022Retrieval import *
 from .multilingual.NeuCLIR2023Retrieval import *
 from .multilingual.XMarketRetrieval import *
 from .multilingual.XPQARetrieval import *
+from .multilingual.XQuADRetrieval import *
 from .nob.norquad import *
 from .nob.snl_retrieval import *
 from .pol.ArguAnaPLRetrieval import *
 from .pol.DBPediaPLRetrieval import *
 from .pol.FiQAPLRetrieval import *
 from .pol.HotpotQAPLRetrieval import *
 from .pol.MSMARCOPLRetrieval import *
 from .pol.NFCorpusPLRetrieval import *
 from .pol.NQPLRetrieval import *
 from .pol.QuoraPLRetrieval import *
 from .pol.SCIDOCSPLRetrieval import *
 from .pol.SciFactPLRetrieval import *
 from .pol.TRECCOVIDPLRetrieval import *
+from .slk.SlovakSumRetrieval import *
 from .spa.SpanishPassageRetrievalS2P import *
 from .spa.SpanishPassageRetrievalS2S import *
 from .swe.swedn_retrieval import *
 from .swe.swefaq_retrieval import *
+from .tur.TurHistQuad import *
 from .vie.VieQuADRetrieval import *
 from .zho.CMTEBRetrieval import *
 from .zho.LeCaRDv2Retrieval import *
```

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/code/CodeSearchNetRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/code/CodeSearchNetRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/dan/dan_fever.py` & `mteb-1.8.0/mteb/tasks/Retrieval/dan/dan_fever.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/dan/t2nord_retrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/dan/t2nord_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/dan/twitterhjerne.py` & `mteb-1.8.0/mteb/tasks/Retrieval/dan/twitterhjerne.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/deu/GerDaLIRRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/deu/GerDaLIRRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/deu/GerDaLIRSmallRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/zho/LeCaRDv2Retrieval.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class GerDaLIRSmall(AbsTaskRetrieval):
+class LeCaRDv2(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="GerDaLIRSmall",
-        description="The dataset consists of documents, passages and relevance labels in German. In contrast to the original dataset, only documents that have corresponding queries in the query set are chosen to create a smaller corpus for evaluation purposes.",
-        reference="https://github.com/lavis-nlp/GerDaLIR",
+        name="LeCaRDv2",
+        description="The task involves identifying and retrieving the case document that best matches or is most relevant to the scenario described in each of the provided queries.",
+        reference="https://github.com/THUIR/LeCaRDv2",
         dataset={
-            "path": "mteb/GerDaLIRSmall",
-            "revision": "48327de6ee192e9610f3069789719788957c7abd",
+            "path": "mteb/LeCaRDv2",
+            "revision": "b78e18688c3d012a33dc3676597c1d1b2243ce1c",
         },
         type="Retrieval",
         category="p2p",
         eval_splits=["test"],
-        eval_langs=["deu-Latn"],
+        eval_langs=["zho-Hans"],
         main_score="ndcg_at_10",
         date=None,
         form=["written"],
         domains=["Legal"],
         task_subtypes=["Article retrieval"],
-        license="MIT license",
+        license="MIT",
         socioeconomic_status="high",
         annotations_creators="derived",
         dialect=None,
         text_creation="found",
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
```

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/deu/GermanDPRRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/deu/GermanDPRRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/deu/GermanQuADRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/fra/SyntecRetrieval.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,65 +1,71 @@
 from __future__ import annotations
 
-from collections import defaultdict
-
-from datasets import DatasetDict, load_dataset
+import datasets
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-def load_retrieval_data(dataset_path, eval_splits):
-    eval_split = eval_splits[0]
-    corpus_dataset = load_dataset(dataset_path, "corpus")
-    queries_dataset = load_dataset(dataset_path, "queries")
-    qrels = load_dataset(dataset_path + "-qrels")[eval_split]
-
-    corpus = {e["_id"]: {"text": e["text"]} for e in corpus_dataset["corpus"]}
-    queries = {e["_id"]: e["text"] for e in queries_dataset["queries"]}
-    relevant_docs = defaultdict(dict)
-    for e in qrels:
-        relevant_docs[e["query-id"]][e["corpus-id"]] = e["score"]
-
-    corpus = DatasetDict({eval_split: corpus})
-    queries = DatasetDict({eval_split: queries})
-    relevant_docs = DatasetDict({eval_split: relevant_docs})
-    return corpus, queries, relevant_docs
-
+class SyntecRetrieval(AbsTaskRetrieval):
+    _EVAL_SPLITS = ["test"]
 
-class GermanQuADRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="GermanQuAD-Retrieval",
-        description="Context Retrieval for German Question Answering",
-        reference="https://www.kaggle.com/datasets/GermanQuAD",
+        name="SyntecRetrieval",
+        description="This dataset has been built from the Syntec Collective bargaining agreement.",
+        reference="https://huggingface.co/datasets/lyon-nlp/mteb-fr-retrieval-syntec-s2p",
         dataset={
-            "path": "mteb/germanquad-retrieval",
-            "revision": "f5c87ae5a2e7a5106606314eef45255f03151bb3",
+            "path": "lyon-nlp/mteb-fr-retrieval-syntec-s2p",
+            "revision": "19661ccdca4dfc2d15122d776b61685f48c68ca9",
         },
         type="Retrieval",
         category="s2p",
-        eval_splits=["test"],
-        eval_langs=["deu-Latn"],
-        main_score="mrr_at_5",
+        eval_splits=_EVAL_SPLITS,
+        eval_langs=["fra-Latn"],
+        main_score="map",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
-        dialect=None,
+        dialect=[],
         text_creation=None,
         bibtex_citation=None,
-        n_samples=None,
-        avg_character_length=None,
+        n_samples={"test": 90},
+        avg_character_length={"test": 62},
     )
 
     def load_data(self, **kwargs):
         if self.data_loaded:
             return
-
-        self.corpus, self.queries, self.relevant_docs = load_retrieval_data(
-            self.metadata_dict["dataset"]["path"], self.metadata_dict["eval_splits"]
+        # fetch both subsets of the dataset
+        corpus_raw = datasets.load_dataset(
+            name="documents",
+            **self.metadata_dict["dataset"],
         )
+        queries_raw = datasets.load_dataset(
+            name="queries",
+            **self.metadata_dict["dataset"],
+        )
+
+        eval_split = self.metadata_dict["eval_splits"][0]
+        self.queries = {
+            eval_split: {
+                str(i): q["Question"] for i, q in enumerate(queries_raw[eval_split])
+            }
+        }
+
+        corpus_raw = corpus_raw[eval_split]
+        corpus_raw = corpus_raw.rename_column("content", "text")
+        self.corpus = {eval_split: {str(row["id"]): row for row in corpus_raw}}
+
+        self.relevant_docs = {
+            eval_split: {
+                str(i): {str(q["Article"]): 1}
+                for i, q in enumerate(queries_raw[eval_split])
+            }
+        }
+
         self.data_loaded = True
```

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/deu/LegalQuADRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/deu/LegalQuADRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/AILACasedocsRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/AILACasedocsRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/AILAStatutesRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/AILAStatutesRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/ArguAnaRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/ArguAnaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackAndroidRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/CQADupstackAndroidRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackEnglishRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/CQADupstackEnglishRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackGamingRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/CQADupstackGamingRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackGisRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/CQADupstackUnixRetrieval.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class CQADupstackGisRetrieval(AbsTaskRetrieval):
+class CQADupstackUnixRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="CQADupstackGisRetrieval",
+        name="CQADupstackUnixRetrieval",
         description="CQADupStack: A Benchmark Data Set for Community Question-Answering Research",
         reference="http://nlp.cis.unimelb.edu.au/resources/cqadupstack/",
         dataset={
-            "path": "mteb/cqadupstack-gis",
-            "revision": "5003b3064772da1887988e05400cf3806fe491f2",
+            "path": "mteb/cqadupstack-unix",
+            "revision": "6c6430d3a6d36f8d2a829195bc5dc94d7e063e53",
         },
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
         eval_langs=["eng-Latn"],
         main_score="ndcg_at_10",
         date=None,
```

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackMathematicaRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/CQADupstackMathematicaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackPhysicsRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/CQADupstackPhysicsRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackProgrammersRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/CQADupstackProgrammersRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackStatsRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/CQADupstackStatsRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackTexRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/CQADupstackTexRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackUnixRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/CQADupstackWordpressRetrieval.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class CQADupstackUnixRetrieval(AbsTaskRetrieval):
+class CQADupstackWordpressRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="CQADupstackUnixRetrieval",
-        description="CQADupStack: A Benchmark Data Set for Community Question-Answering Research",
-        reference="http://nlp.cis.unimelb.edu.au/resources/cqadupstack/",
+        name="CQADupstackWordpressRetrieval",
         dataset={
-            "path": "mteb/cqadupstack-unix",
-            "revision": "6c6430d3a6d36f8d2a829195bc5dc94d7e063e53",
+            "path": "mteb/cqadupstack-wordpress",
+            "revision": "4ffe81d471b1924886b33c7567bfb200e9eec5c4",
         },
+        description="CQADupStack: A Benchmark Data Set for Community Question-Answering Research",
+        reference="http://nlp.cis.unimelb.edu.au/resources/cqadupstack/",
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
         eval_langs=["eng-Latn"],
         main_score="ndcg_at_10",
         date=None,
         form=None,
```

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackWebmastersRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/CQADupstackWebmastersRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/CQADupstackWordpressRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/pol/NQPLRetrieval.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class CQADupstackWordpressRetrieval(AbsTaskRetrieval):
+class NQPL(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="CQADupstackWordpressRetrieval",
+        name="NQ-PL",
+        description="Natural Questions: A Benchmark for Question Answering Research",
+        reference="https://ai.google.com/research/NaturalQuestions/",
         dataset={
-            "path": "mteb/cqadupstack-wordpress",
-            "revision": "4ffe81d471b1924886b33c7567bfb200e9eec5c4",
+            "path": "clarin-knext/nq-pl",
+            "revision": "f171245712cf85dd4700b06bef18001578d0ca8d",
         },
-        description="CQADupStack: A Benchmark Data Set for Community Question-Answering Research",
-        reference="http://nlp.cis.unimelb.edu.au/resources/cqadupstack/",
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
-        eval_langs=["eng-Latn"],
+        eval_langs=["pol-Latn"],
         main_score="ndcg_at_10",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
```

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/ClimateFEVERRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/ClimateFEVERRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/DBPediaRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/DBPediaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/FEVERRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/FEVERRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/FiQA2018Retrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/FiQA2018Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/HagridRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/HagridRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/HotpotQARetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/HotpotQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/LEMBNarrativeQARetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/LEMBNarrativeQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/LEMBNeedleRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/LEMBNeedleRetrieval.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,15 +36,22 @@
         domains=["Academic", "Blog"],
         task_subtypes=["Article retrieval"],
         license="Not specified",
         socioeconomic_status="high",
         annotations_creators="derived",
         dialect=[],
         text_creation="found",
-        bibtex_citation=None,
+        bibtex_citation="""
+            @article{zhu2024longembed,
+            title={LongEmbed: Extending Embedding Models for Long Context Retrieval},
+            author={Zhu, Dawei and Wang, Liang and Yang, Nan and Song, Yifan and Wu, Wenhao and Wei, Furu and Li, Sujian},
+            journal={arXiv preprint arXiv:2404.12096},
+            year={2024}
+            }
+        """,
         n_samples={
             "test_256": 150,
             "test_512": 150,
             "test_1024": 150,
             "test_2048": 150,
             "test_4096": 150,
             "test_8192": 150,
```

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/LEMBPasskeyRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/LEMBPasskeyRetrieval.py`

 * *Files 20% similar despite different names*

```diff
@@ -36,15 +36,22 @@
         domains=["Fiction"],
         task_subtypes=["Article retrieval"],
         license="Not specified",
         socioeconomic_status="low",
         annotations_creators="derived",
         dialect=[],
         text_creation="found",
-        bibtex_citation=None,
+        bibtex_citation="""
+            @article{zhu2024longembed,
+            title={LongEmbed: Extending Embedding Models for Long Context Retrieval},
+            author={Zhu, Dawei and Wang, Liang and Yang, Nan and Song, Yifan and Wu, Wenhao and Wei, Furu and Li, Sujian},
+            journal={arXiv preprint arXiv:2404.12096},
+            year={2024}
+            }
+        """,
         n_samples={
             "test_256": 150,
             "test_512": 150,
             "test_1024": 150,
             "test_2048": 150,
             "test_4096": 150,
             "test_8192": 150,
```

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/LEMBQMSumRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/LEMBQMSumRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/LEMBSummScreenFDRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/LEMBSummScreenFDRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/LEMBWikimQARetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/LEMBWikimQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/LegalBenchConsumerContractsQARetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/LegalBenchConsumerContractsQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/LegalBenchCorporateLobbyingRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/LegalBenchCorporateLobbyingRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/LegalSummarizationRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/LegalSummarizationRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/MSMARCORetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/MSMARCOv2Retrieval.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class MSMARCO(AbsTaskRetrieval):
+class MSMARCOv2(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="MSMARCO",
+        name="MSMARCOv2",
         dataset={
-            "path": "mteb/msmarco",
-            "revision": "c5a29a104738b98a9e76336939199e264163d4a0",
+            "path": "mteb/msmarco-v2",
+            "revision": "b1663124850d305ab7c470bb0548acf8e2e7ea43",
         },
         description="MS MARCO is a collection of datasets focused on deep learning in search",
-        reference="https://microsoft.github.io/msmarco/",
+        reference="https://microsoft.github.io/msmarco/TREC-Deep-Learning.html",
         type="Retrieval",
         category="s2p",
-        eval_splits=["train", "dev", "test"],
+        eval_splits=["train", "dev", "dev2"],
         eval_langs=["eng-Latn"],
         main_score="ndcg_at_10",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
```

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/MSMARCOv2Retrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/pol/MSMARCOPLRetrieval.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class MSMARCOv2(AbsTaskRetrieval):
+class MSMARCOPL(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="MSMARCOv2",
+        name="MSMARCO-PL",
+        description="MS MARCO is a collection of datasets focused on deep learning in search",
+        reference="https://microsoft.github.io/msmarco/",
         dataset={
-            "path": "mteb/msmarco-v2",
-            "revision": "b1663124850d305ab7c470bb0548acf8e2e7ea43",
+            "path": "clarin-knext/msmarco-pl",
+            "revision": "8634c07806d5cce3a6138e260e59b81760a0a640",
         },
-        description="MS MARCO is a collection of datasets focused on deep learning in search",
-        reference="https://microsoft.github.io/msmarco/TREC-Deep-Learning.html",
         type="Retrieval",
         category="s2p",
-        eval_splits=["train", "dev", "dev2"],
-        eval_langs=["eng-Latn"],
+        eval_splits=["test"],
+        eval_langs=["pol-Latn"],
         main_score="ndcg_at_10",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
```

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/MedicalQARetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/MedicalQARetrieval.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         task_subtypes=["Article retrieval"],
         license="CC0 1.0 Universal",
         socioeconomic_status="medium",
         annotations_creators="derived",
         dialect=[],
         text_creation="found",
         bibtex_citation="""@ARTICLE{BenAbacha-BMC-2019,
-            author    = {Asma {Ben Abacha} and Dina Demner{-}Fushman},
+            author    = {Asma, Ben Abacha and Dina, Demner{-}Fushman},
             title     = {A Question-Entailment Approach to Question Answering},
             journal = {{BMC} Bioinform.},
             volume    = {20},
             number    = {1},
             pages     = {511:1--511:23},
             year      = {2019},
             url       = {https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-019-3119-4}
```

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/NFCorpusRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/NFCorpusRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/NQRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/NQRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/NarrativeQARetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/NarrativeQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/QuoraRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/QuoraRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/SCIDOCSRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/SCIDOCSRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/SciFactRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/SciFactRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/TRECCOVIDRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/TRECCOVIDRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/eng/Touche2020Retrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/eng/Touche2020Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/est/estqa.py` & `mteb-1.8.0/mteb/tasks/Retrieval/est/estqa.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/fra/AlloprofRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/fra/AlloprofRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/fra/BSARDRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/fra/BSARDRetrieval.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,15 @@
             "path": "maastrichtlawtech/bsard",
             "revision": "5effa1b9b5fa3b0f9e12523e6e43e5f86a6e6d59",
         },
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
         eval_langs=["fra-Latn"],
-        main_score="ndcg_at_100",
+        main_score="recall_at_100",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -48,15 +48,15 @@
             name="questions",
             split=self.metadata.eval_splits[0],
             **self.metadata_dict["dataset"],
         )
 
         self.queries = {
             self.metadata.eval_splits[0]: {
-                str(q["id"]): " ".join((q["question"] + q["extra_description"]))
+                str(q["id"]): (q["question"] + " " + q["extra_description"]).strip()
                 for q in queries_raw
             }
         }
 
         self.corpus = {
             self.metadata.eval_splits[0]: {
                 str(d["id"]): {"text": d["article"]} for d in corpus_raw
```

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/fra/FQuADRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/fra/FQuADRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/fra/SyntecRetrieval.py` & `mteb-1.8.0/mteb/tasks/STS/fra/SickFrSTS.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,71 +1,51 @@
 from __future__ import annotations
 
-import datasets
-
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
-
+from ....abstasks.AbsTaskSTS import AbsTaskSTS
 
-class SyntecRetrieval(AbsTaskRetrieval):
-    _EVAL_SPLITS = ["test"]
 
+class SickFrSTS(AbsTaskSTS):
     metadata = TaskMetadata(
-        name="SyntecRetrieval",
-        description="This dataset has been built from the Syntec Collective bargaining agreement.",
-        reference="https://huggingface.co/datasets/lyon-nlp/mteb-fr-retrieval-syntec-s2p",
+        name="SICKFr",
         dataset={
-            "path": "lyon-nlp/mteb-fr-retrieval-syntec-s2p",
-            "revision": "19661ccdca4dfc2d15122d776b61685f48c68ca9",
+            "path": "Lajavaness/SICK-fr",
+            "revision": "e077ab4cf4774a1e36d86d593b150422fafd8e8a",
         },
-        type="Retrieval",
-        category="s2p",
-        eval_splits=_EVAL_SPLITS,
+        description="SICK dataset french version",
+        reference="https://huggingface.co/datasets/Lajavaness/SICK-fr",
+        type="STS",
+        category="s2s",
+        eval_splits=["validation", "test"],
         eval_langs=["fra-Latn"],
-        main_score="map",
+        main_score="cosine_spearman",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
-        dialect=[],
+        dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples={"test": 90},
-        avg_character_length={"test": 62},
+        n_samples=None,
+        avg_character_length=None,
     )
 
-    def load_data(self, **kwargs):
-        if self.data_loaded:
-            return
-        # fetch both subsets of the dataset
-        corpus_raw = datasets.load_dataset(
-            name="documents",
-            **self.metadata_dict["dataset"],
-        )
-        queries_raw = datasets.load_dataset(
-            name="queries",
-            **self.metadata_dict["dataset"],
-        )
-
-        eval_split = self.metadata_dict["eval_splits"][0]
-        self.queries = {
-            eval_split: {
-                str(i): q["Question"] for i, q in enumerate(queries_raw[eval_split])
+    @property
+    def metadata_dict(self) -> dict[str, str]:
+        metadata_dict = super().metadata_dict
+        metadata_dict["min_score"] = 0
+        metadata_dict["max_score"] = 5
+        return metadata_dict
+
+    def dataset_transform(self):
+        self.dataset = self.dataset.rename_columns(
+            {
+                "sentence_A": "sentence1",
+                "sentence_B": "sentence2",
+                "relatedness_score": "score",
+                "Unnamed: 0": "id",
             }
-        }
-
-        corpus_raw = corpus_raw[eval_split]
-        corpus_raw = corpus_raw.rename_column("content", "text")
-        self.corpus = {eval_split: {str(row["id"]): row for row in corpus_raw}}
-
-        self.relevant_docs = {
-            eval_split: {
-                str(i): {str(q["Article"]): 1}
-                for i, q in enumerate(queries_raw[eval_split])
-            }
-        }
-
-        self.data_loaded = True
+        )
```

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/hun/HunSum2.py` & `mteb-1.8.0/mteb/tasks/Retrieval/hun/HunSum2.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/jpn/JaQuADRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/jpn/JaQuADRetrieval.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         },
         description="Human-annotated question-answer pairs for Japanese wikipedia pages.",
         reference="https://arxiv.org/abs/2202.01764",
         type="Retrieval",
         category="p2p",
         eval_splits=["validation"],
         eval_langs=["jpn-Jpan"],
-        main_score="ncdg_at_10",
+        main_score="ndcg_at_10",
         date=("2022-01-01", "2022-12-31"),  # approximate guess
         form=["written"],
         domains=["Encyclopaedic", "Non-fiction"],
         task_subtypes=["Question answering"],
         license="CC-BY-SA-3.0",
         socioeconomic_status="high",
         annotations_creators="human-annotated",
```

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/kor/KoMiracl.py` & `mteb-1.8.0/mteb/tasks/Retrieval/kor/KoMiracl.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/kor/KoStrategyQA.py` & `mteb-1.8.0/mteb/tasks/Retrieval/kor/KoStrategyQA.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/multilingual/NeuCLIR2022Retrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/multilingual/NeuCLIR2022Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/multilingual/NeuCLIR2023Retrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/multilingual/NeuCLIR2023Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/nob/norquad.py` & `mteb-1.8.0/mteb/tasks/Retrieval/nob/norquad.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/nob/snl_retrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/nob/snl_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/pol/ArguAnaPLRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/pol/ArguAnaPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/pol/DBPediaPLRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/pol/DBPediaPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/pol/FiQAPLRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/pol/FiQAPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/pol/HotpotQAPLRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/pol/HotpotQAPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/pol/MSMARCOPLRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/pol/SciFactPLRetrieval.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class MSMARCOPL(AbsTaskRetrieval):
+class SciFactPL(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="MSMARCO-PL",
-        description="MS MARCO is a collection of datasets focused on deep learning in search",
-        reference="https://microsoft.github.io/msmarco/",
+        name="SciFact-PL",
+        description="SciFact verifies scientific claims using evidence from the research literature containing scientific paper abstracts.",
+        reference="https://github.com/allenai/scifact",
         dataset={
-            "path": "clarin-knext/msmarco-pl",
-            "revision": "8634c07806d5cce3a6138e260e59b81760a0a640",
+            "path": "clarin-knext/scifact-pl",
+            "revision": "47932a35f045ef8ed01ba82bf9ff67f6e109207e",
         },
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
         eval_langs=["pol-Latn"],
         main_score="ndcg_at_10",
         date=None,
```

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/pol/NFCorpusPLRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/pol/NFCorpusPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/pol/NQPLRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/pol/QuoraPLRetrieval.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class NQPL(AbsTaskRetrieval):
+class QuoraPLRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="NQ-PL",
-        description="Natural Questions: A Benchmark for Question Answering Research",
-        reference="https://ai.google.com/research/NaturalQuestions/",
+        name="Quora-PL",
+        description="QuoraRetrieval is based on questions that are marked as duplicates on the Quora platform. Given a question, find other (duplicate) questions.",
+        reference="https://quoradata.quora.com/First-Quora-Dataset-Release-Question-Pairs",
         dataset={
-            "path": "clarin-knext/nq-pl",
-            "revision": "f171245712cf85dd4700b06bef18001578d0ca8d",
+            "path": "clarin-knext/quora-pl",
+            "revision": "0be27e93455051e531182b85e85e425aba12e9d4",
         },
         type="Retrieval",
-        category="s2p",
-        eval_splits=["test"],
+        category="s2s",
+        eval_splits=["validation", "test"],
         eval_langs=["pol-Latn"],
         main_score="ndcg_at_10",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
```

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/pol/QuoraPLRetrieval.py` & `mteb-1.8.0/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,55 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
+from ....abstasks import AbsTaskSTS, CrosslingualTask
 
+_LANGUAGES = {
+    "ko-ko": ["kor-Hang"],
+    "ar-ar": ["ara-Arab"],
+    "en-ar": ["eng-Latn", "ara-Arab"],
+    "en-de": ["eng-Latn", "deu-Latn"],
+    "en-en": ["eng-Latn"],
+    "en-tr": ["eng-Latn", "tur-Latn"],
+    "es-en": ["spa-Latn", "eng-Latn"],
+    "es-es": ["spa-Latn"],
+    "fr-en": ["fra-Latn", "eng-Latn"],
+    "it-en": ["ita-Latn", "eng-Latn"],
+    "nl-en": ["nld-Latn", "eng-Latn"],
+}
 
-class QuoraPLRetrieval(AbsTaskRetrieval):
+
+class STS17Crosslingual(AbsTaskSTS, CrosslingualTask):
     metadata = TaskMetadata(
-        name="Quora-PL",
-        description="QuoraRetrieval is based on questions that are marked as duplicates on the Quora platform. Given a question, find other (duplicate) questions.",
-        reference="https://quoradata.quora.com/First-Quora-Dataset-Release-Question-Pairs",
+        name="STS17",
         dataset={
-            "path": "clarin-knext/quora-pl",
-            "revision": "0be27e93455051e531182b85e85e425aba12e9d4",
+            "path": "mteb/sts17-crosslingual-sts",
+            "revision": "af5e6fb845001ecf41f4c1e033ce921939a2a68d",
         },
-        type="Retrieval",
+        description="STS 2017 dataset",
+        reference="http://alt.qcri.org/semeval2016/task1/",
+        type="STS",
         category="s2s",
-        eval_splits=["validation", "test"],
-        eval_langs=["pol-Latn"],
-        main_score="ndcg_at_10",
+        eval_splits=["test"],
+        eval_langs=_LANGUAGES,
+        main_score="cosine_spearman",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples=None,
-        avg_character_length=None,
+        n_samples={"test": 500},
+        avg_character_length={"test": 43.3},
     )
+
+    @property
+    def metadata_dict(self) -> dict[str, str]:
+        metadata_dict = super().metadata_dict
+        metadata_dict["min_score"] = 0
+        metadata_dict["max_score"] = 5
+        return metadata_dict
```

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/pol/SCIDOCSPLRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/pol/SCIDOCSPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/pol/SciFactPLRetrieval.py` & `mteb-1.8.0/mteb/tasks/STS/eng/STS16STS.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
+from ....abstasks.AbsTaskSTS import AbsTaskSTS
 
 
-class SciFactPL(AbsTaskRetrieval):
+class STS16STS(AbsTaskSTS):
     metadata = TaskMetadata(
-        name="SciFact-PL",
-        description="SciFact verifies scientific claims using evidence from the research literature containing scientific paper abstracts.",
-        reference="https://github.com/allenai/scifact",
+        name="STS16",
         dataset={
-            "path": "clarin-knext/scifact-pl",
-            "revision": "47932a35f045ef8ed01ba82bf9ff67f6e109207e",
+            "path": "mteb/sts16-sts",
+            "revision": "4d8694f8f0e0100860b497b999b3dbed754a0513",
         },
-        type="Retrieval",
-        category="s2p",
+        description="SemEval STS 2016 dataset",
+        reference="https://www.aclweb.org/anthology/S16-1001",
+        type="STS",
+        category="s2s",
         eval_splits=["test"],
-        eval_langs=["pol-Latn"],
-        main_score="ndcg_at_10",
+        eval_langs=["eng-Latn"],
+        main_score="cosine_spearman",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
+
+    @property
+    def metadata_dict(self) -> dict[str, str]:
+        metadata_dict = super().metadata_dict
+        metadata_dict["min_score"] = 0
+        metadata_dict["max_score"] = 5
+        return metadata_dict
```

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/pol/TRECCOVIDPLRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/pol/TRECCOVIDPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2P.py` & `mteb-1.8.0/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2S.py` & `mteb-1.8.0/mteb/tasks/Clustering/deu/TenKGnadClusteringS2SFast.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,40 @@
 from __future__ import annotations
 
-import datasets
-
+from mteb.abstasks.AbsTaskClusteringFast import AbsTaskClusteringFast, convert_to_fast
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
-
 
-class SpanishPassageRetrievalS2S(AbsTaskRetrieval):
+class TenKGnadClusteringS2S(AbsTaskClusteringFast):
     metadata = TaskMetadata(
-        name="SpanishPassageRetrievalS2S",
-        description="Test collection for passage retrieval from health-related Web resources in Spanish.",
-        reference="https://mklab.iti.gr/results/spanish-passage-retrieval-dataset/",
+        name="TenKGnadClusteringS2S.v2",
+        description="Clustering of news article titles. Clustering of 10 splits on the news article category.",
+        reference="https://tblock.github.io/10kGNAD/",
         dataset={
-            "path": "jinaai/spanish_passage_retrieval",
-            "revision": "9cddf2ce5209ade52c2115ccfa00eb22c6d3a837",
-            "trust_remote_code": True,
+            "path": "slvnwhrl/tenkgnad-clustering-s2s",
+            "revision": "6cddbe003f12b9b140aec477b583ac4191f01786",
         },
-        type="Retrieval",
+        type="Clustering",
         category="s2s",
         eval_splits=["test"],
-        eval_langs=["spa-Latn"],
-        main_score="ndcg_at_10",
-        date=None,
-        form=None,
-        domains=None,
+        eval_langs=["deu-Latn"],
+        main_score="v_measure",
+        date=(
+            "2000-01-01",
+            "2020-12-31",
+        ),  # since it is news it is guessed that it is from 2000 to 2020
+        form=["written"],
+        domains=["News", "Non-fiction"],
         task_subtypes=None,
-        license=None,
-        socioeconomic_status=None,
-        annotations_creators=None,
-        dialect=None,
-        text_creation=None,
-        bibtex_citation=None,
-        n_samples=None,
-        avg_character_length=None,
+        license="cc-by-sa-4.0",
+        socioeconomic_status="medium",
+        annotations_creators="derived",
+        dialect=[],
+        text_creation="found",
+        bibtex_citation=None,  # none found
+        n_samples={"test": 10275},  # due to duplicates
+        avg_character_length={"test": 50.96},
     )
 
-    def load_data(self, **kwargs):
-        if self.data_loaded:
-            return
-
-        query_rows = datasets.load_dataset(
-            name="queries",
-            split="test",
-            **self.metadata_dict["dataset"],
-        )
-        corpus_rows = datasets.load_dataset(
-            name="corpus.sentences",
-            split="test",
-            **self.metadata_dict["dataset"],
-        )
-        qrels_rows = datasets.load_dataset(
-            name="qrels.s2s",
-            split="test",
-            **self.metadata_dict["dataset"],
-        )
-
-        self.queries = {"test": {row["_id"]: row["text"] for row in query_rows}}
-        self.corpus = {"test": {row["_id"]: row for row in corpus_rows}}
-        self.relevant_docs = {
-            "test": {
-                row["_id"]: {v: 1 for v in row["text"].split(" ")} for row in qrels_rows
-            }
-        }
-
-        self.data_loaded = True
+    def dataset_transform(self) -> None:
+        ds = convert_to_fast(self.dataset, self.seed)  # type: ignore
+        self.dataset = ds
```

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/swe/swedn_retrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/swe/swedn_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/swe/swefaq_retrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/swe/swefaq_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/vie/VieQuADRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/vie/VieQuADRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/zho/CMTEBRetrieval.py` & `mteb-1.8.0/mteb/tasks/Retrieval/zho/CMTEBRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Retrieval/zho/LeCaRDv2Retrieval.py` & `mteb-1.8.0/mteb/tasks/Summarization/fra/SummEvalFrSummarization.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 from __future__ import annotations
 
+from mteb.abstasks import AbsTaskSummarization
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
-
-class LeCaRDv2(AbsTaskRetrieval):
+class SummEvalFrSummarization(AbsTaskSummarization):
     metadata = TaskMetadata(
-        name="LeCaRDv2",
-        description="The task involves identifying and retrieving the case document that best matches or is most relevant to the scenario described in each of the provided queries.",
-        reference="https://github.com/THUIR/LeCaRDv2",
+        name="SummEvalFr",
+        description="News Article Summary Semantic Similarity Estimation translated from english to french with DeepL.",
+        reference="https://github.com/Yale-LILY/SummEval",
         dataset={
-            "path": "mteb/LeCaRDv2",
-            "revision": "b78e18688c3d012a33dc3676597c1d1b2243ce1c",
+            "path": "lyon-nlp/summarization-summeval-fr-p2p",
+            "revision": "b385812de6a9577b6f4d0f88c6a6e35395a94054",
         },
-        type="Retrieval",
+        type="Summarization",
         category="p2p",
         eval_splits=["test"],
-        eval_langs=["zho-Hans"],
-        main_score="ndcg_at_10",
+        eval_langs=["fra-Latn"],
+        main_score="cosine_spearman",
         date=None,
         form=["written"],
-        domains=["Legal"],
-        task_subtypes=["Article retrieval"],
-        license="MIT",
-        socioeconomic_status="high",
-        annotations_creators="derived",
+        domains=None,
+        task_subtypes=None,
+        license=None,
+        socioeconomic_status=None,
+        annotations_creators=None,
         dialect=None,
-        text_creation="found",
+        text_creation="machine-translated",
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
+
+    @property
+    def metadata_dict(self) -> dict[str, str]:
+        metadata_dict = super().metadata_dict
+        metadata_dict["min_score"] = 0
+        metadata_dict["max_score"] = 5
+
+        return metadata_dict
```

### Comparing `mteb-1.7.9/mteb/tasks/STS/__init__.py` & `mteb-1.8.0/mteb/tasks/STS/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from .eng.STS16STS import *
 from .eng.STSBenchmarkSTS import *
 from .fin.FinParaSTS import *
 from .fra.SickFrSTS import *
 from .jpn.JSTS import *
 from .kor.KlueSTS import *
 from .kor.KorSTS import *
+from .multilingual.IndicCrosslingualSTS import *
 from .multilingual.STS17CrosslingualSTS import *
 from .multilingual.STS22CrosslingualSTS import *
 from .multilingual.STSBenchmarkMultilingualSTS import *
 from .pol.PolishSTS import *
 from .ron.RonSTS import *
 from .spa.STSES import *
 from .zho.CMTEBSTS import *
```

### Comparing `mteb-1.7.9/mteb/tasks/STS/deu/GermanSTSBenchmarkSTS.py` & `mteb-1.8.0/mteb/tasks/STS/deu/GermanSTSBenchmarkSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/STS/eng/BiossesSTS.py` & `mteb-1.8.0/mteb/tasks/STS/spa/STSES.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskSTS import AbsTaskSTS
 
+_EVAL_SPLIT = "test"
 
-class BiossesSTS(AbsTaskSTS):
+
+class STSES(AbsTaskSTS):
     metadata = TaskMetadata(
-        name="BIOSSES",
+        name="STSES",
         dataset={
-            "path": "mteb/biosses-sts",
-            "revision": "d3fb88f8f02e40887cd149695127462bbcf29b4a",
+            "path": "PlanTL-GOB-ES/sts-es",
+            "revision": "0912bb6c9393c76d62a7c5ee81c4c817ff47c9f4",
+            "trust_remote_code": True,
         },
-        description="Biomedical Semantic Similarity Estimation.",
-        reference="https://tabilab.cmpe.boun.edu.tr/BIOSSES/DataSet.html",
+        description="Spanish test sets from SemEval-2014 (Agirre et al., 2014) and SemEval-2015 (Agirre et al., 2015)",
+        reference="https://huggingface.co/datasets/PlanTL-GOB-ES/sts-es",
         type="STS",
         category="s2s",
-        eval_splits=["test"],
-        eval_langs=["eng-Latn"],
+        eval_splits=[_EVAL_SPLIT],
+        eval_langs=["spa-Latn"],
         main_score="cosine_spearman",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
@@ -35,7 +38,12 @@
 
     @property
     def metadata_dict(self) -> dict[str, str]:
         metadata_dict = super().metadata_dict
         metadata_dict["min_score"] = 0
         metadata_dict["max_score"] = 5
         return metadata_dict
+
+    def dataset_transform(self):
+        data = self.dataset[_EVAL_SPLIT]
+        data = data.add_column("score", [d["label"] for d in data])
+        self.dataset = {_EVAL_SPLIT: data}
```

### Comparing `mteb-1.7.9/mteb/tasks/STS/eng/STS12STS.py` & `mteb-1.8.0/mteb/tasks/STS/eng/STS12STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/STS/eng/STS13STS.py` & `mteb-1.8.0/mteb/tasks/STS/eng/STS13STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/STS/eng/STS14STS.py` & `mteb-1.8.0/mteb/tasks/STS/eng/STS15STS.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskSTS import AbsTaskSTS
 
 
-class STS14STS(AbsTaskSTS):
+class STS15STS(AbsTaskSTS):
     metadata = TaskMetadata(
-        name="STS14",
+        name="STS15",
         dataset={
-            "path": "mteb/sts14-sts",
-            "revision": "6031580fec1f6af667f0bd2da0a551cf4f0b2375",
+            "path": "mteb/sts15-sts",
+            "revision": "ae752c7c21bf194d8b67fd573edf7ae58183cbe3",
         },
-        description="SemEval STS 2014 dataset. Currently only the English dataset",
-        reference="https://www.aclweb.org/anthology/S14-1002",
+        description="SemEval STS 2015 dataset",
+        reference="https://www.aclweb.org/anthology/S15-2010",
         type="STS",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["eng-Latn"],
         main_score="cosine_spearman",
         date=None,
         form=None,
```

### Comparing `mteb-1.7.9/mteb/tasks/STS/eng/STS15STS.py` & `mteb-1.8.0/mteb/tasks/STS/eng/SickrSTS.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskSTS import AbsTaskSTS
 
 
-class STS15STS(AbsTaskSTS):
+class SickrSTS(AbsTaskSTS):
     metadata = TaskMetadata(
-        name="STS15",
+        name="SICK-R",
         dataset={
-            "path": "mteb/sts15-sts",
-            "revision": "ae752c7c21bf194d8b67fd573edf7ae58183cbe3",
+            "path": "mteb/sickr-sts",
+            "revision": "20a6d6f312dd54037fe07a32d58e5e168867909d",
         },
-        description="SemEval STS 2015 dataset",
-        reference="https://www.aclweb.org/anthology/S15-2010",
+        description="Semantic Textual Similarity SICK-R dataset as described here:",
+        reference="https://aclanthology.org/2020.lrec-1.207",
         type="STS",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["eng-Latn"],
         main_score="cosine_spearman",
         date=None,
         form=None,
```

### Comparing `mteb-1.7.9/mteb/tasks/STS/eng/STS16STS.py` & `mteb-1.8.0/mteb/tasks/STS/eng/STSBenchmarkSTS.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskSTS import AbsTaskSTS
 
 
-class STS16STS(AbsTaskSTS):
+class STSBenchmarkSTS(AbsTaskSTS):
     metadata = TaskMetadata(
-        name="STS16",
+        name="STSBenchmark",
         dataset={
-            "path": "mteb/sts16-sts",
-            "revision": "4d8694f8f0e0100860b497b999b3dbed754a0513",
+            "path": "mteb/stsbenchmark-sts",
+            "revision": "b0fddb56ed78048fa8b90373c8a3cfc37b684831",
         },
-        description="SemEval STS 2016 dataset",
-        reference="https://www.aclweb.org/anthology/S16-1001",
+        description="Semantic Textual Similarity Benchmark (STSbenchmark) dataset.",
+        reference="https://github.com/PhilipMay/stsb-multi-mt/",
         type="STS",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["eng-Latn"],
         main_score="cosine_spearman",
         date=None,
         form=None,
```

### Comparing `mteb-1.7.9/mteb/tasks/STS/eng/STSBenchmarkSTS.py` & `mteb-1.8.0/mteb/tasks/Summarization/eng/SummEvalSummarization.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks.AbsTaskSTS import AbsTaskSTS
+from ....abstasks import AbsTaskSummarization
 
 
-class STSBenchmarkSTS(AbsTaskSTS):
+class SummEvalSummarization(AbsTaskSummarization):
     metadata = TaskMetadata(
-        name="STSBenchmark",
+        name="SummEval",
+        description="News Article Summary Semantic Similarity Estimation.",
+        reference="https://tabilab.cmpe.boun.edu.tr/BIOSSES/DataSet.html",
         dataset={
-            "path": "mteb/stsbenchmark-sts",
-            "revision": "b0fddb56ed78048fa8b90373c8a3cfc37b684831",
+            "path": "mteb/summeval",
+            "revision": "cda12ad7615edc362dbf25a00fdd61d3b1eaf93c",
         },
-        description="Semantic Textual Similarity Benchmark (STSbenchmark) dataset.",
-        reference="https://github.com/PhilipMay/stsb-multi-mt/",
-        type="STS",
-        category="s2s",
+        type="Summarization",
+        category="p2p",
         eval_splits=["test"],
         eval_langs=["eng-Latn"],
         main_score="cosine_spearman",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples=None,
-        avg_character_length=None,
+        n_samples={"test": 2800},
+        avg_character_length={"test": 359.8},
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
         metadata_dict = super().metadata_dict
         metadata_dict["min_score"] = 0
         metadata_dict["max_score"] = 5
```

### Comparing `mteb-1.7.9/mteb/tasks/STS/eng/SickrSTS.py` & `mteb-1.8.0/mteb/tasks/PairClassification/hye/ArmenianParaphrasePC.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 from __future__ import annotations
 
+from mteb.abstasks.AbsTaskPairClassification import AbsTaskPairClassification
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks.AbsTaskSTS import AbsTaskSTS
 
-
-class SickrSTS(AbsTaskSTS):
+class ArmenianParaphrasePC(AbsTaskPairClassification):
     metadata = TaskMetadata(
-        name="SICK-R",
+        name="ArmenianParaphrasePC",
+        description="asparius/Armenian-Paraphrase-PC",
+        reference="https://github.com/ivannikov-lab/arpa-paraphrase-corpus",
         dataset={
-            "path": "mteb/sickr-sts",
-            "revision": "20a6d6f312dd54037fe07a32d58e5e168867909d",
+            "path": "asparius/Armenian-Paraphrase-PC",
+            "revision": "f43b4f32987048043a8b31e5e26be4d360c2438f",
         },
-        description="Semantic Textual Similarity SICK-R dataset as described here:",
-        reference="https://aclanthology.org/2020.lrec-1.207",
-        type="STS",
+        type="PairClassification",
         category="s2s",
         eval_splits=["test"],
-        eval_langs=["eng-Latn"],
-        main_score="cosine_spearman",
-        date=None,
-        form=None,
-        domains=None,
-        task_subtypes=None,
-        license=None,
-        socioeconomic_status=None,
-        annotations_creators=None,
-        dialect=None,
-        text_creation=None,
-        bibtex_citation=None,
-        n_samples=None,
-        avg_character_length=None,
+        eval_langs=["hye-Armn"],
+        main_score="ap",
+        date=("2021-01-01", "2022-04-06"),
+        form=["written"],
+        domains=["News"],
+        task_subtypes=[],
+        license="Apache-2.0",
+        socioeconomic_status="mixed",
+        annotations_creators="derived",
+        dialect=[],
+        text_creation="found",
+        bibtex_citation="""
+        @misc{malajyan2020arpa,
+      title={ARPA: Armenian Paraphrase Detection Corpus and Models}, 
+      author={Arthur Malajyan and Karen Avetisyan and Tsolak Ghukasyan},
+      year={2020},
+      eprint={2009.12615},
+      archivePrefix={arXiv},
+      primaryClass={cs.CL}
+}
+        """,
+        n_samples={"train": 4023, "test": 1470},
+        avg_character_length={"train": 243.81, "test": 241.37},
     )
-
-    @property
-    def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = super().metadata_dict
-        metadata_dict["min_score"] = 0
-        metadata_dict["max_score"] = 5
-        return metadata_dict
```

### Comparing `mteb-1.7.9/mteb/tasks/STS/fin/FinParaSTS.py` & `mteb-1.8.0/mteb/tasks/STS/fin/FinParaSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/STS/fra/SickFrSTS.py` & `mteb-1.8.0/mteb/tasks/Classification/ory/OdiaNewsClassification.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,37 @@
 from __future__ import annotations
 
+from mteb.abstasks import AbsTaskClassification
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks.AbsTaskSTS import AbsTaskSTS
 
-
-class SickFrSTS(AbsTaskSTS):
+class OdiaNewsClassification(AbsTaskClassification):
     metadata = TaskMetadata(
-        name="SICKFr",
+        name="OdiaNewsClassification",
+        description="A Odia dataset for 3-class classification of Odia news articles",
+        reference="https://github.com/goru001/nlp-for-odia",
         dataset={
-            "path": "Lajavaness/SICK-fr",
-            "revision": "e077ab4cf4774a1e36d86d593b150422fafd8e8a",
+            "path": "mlexplorer008/odia_news_classification",
+            "revision": "ffb8a34c9637fb20256e8c7be02504d16af4bd6b",
         },
-        description="SICK dataset french version",
-        reference="https://huggingface.co/datasets/Lajavaness/SICK-fr",
-        type="STS",
+        type="Classification",
         category="s2s",
-        eval_splits=["validation", "test"],
-        eval_langs=["fra-Latn"],
-        main_score="cosine_spearman",
-        date=None,
-        form=None,
-        domains=None,
-        task_subtypes=None,
-        license=None,
-        socioeconomic_status=None,
-        annotations_creators=None,
-        dialect=None,
-        text_creation=None,
-        bibtex_citation=None,
-        n_samples=None,
-        avg_character_length=None,
+        date=("2014-01-01", "2018-01-01"),
+        eval_splits=["test"],
+        eval_langs=["ory-Orya"],
+        main_score="f1",
+        form=["written"],
+        domains=["News"],
+        task_subtypes=["Topic classification"],
+        license="MIT",
+        socioeconomic_status="mixed",
+        annotations_creators="derived",
+        dialect=[],
+        text_creation="found",
+        bibtex_citation="",
+        n_samples={"test": 2048},
+        avg_character_length={"test": 49.24},
     )
 
-    @property
-    def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = super().metadata_dict
-        metadata_dict["min_score"] = 0
-        metadata_dict["max_score"] = 5
-        return metadata_dict
-
     def dataset_transform(self):
-        self.dataset = self.dataset.rename_columns(
-            {
-                "sentence_A": "sentence1",
-                "sentence_B": "sentence2",
-                "relatedness_score": "score",
-                "Unnamed: 0": "id",
-            }
-        )
+        self.dataset = self.dataset.rename_columns({"headings": "text"})
+        self.dataset = self.stratified_subsampling(self.dataset, seed=self.seed)
```

### Comparing `mteb-1.7.9/mteb/tasks/STS/jpn/JSTS.py` & `mteb-1.8.0/mteb/tasks/STS/jpn/JSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/STS/kor/KlueSTS.py` & `mteb-1.8.0/mteb/tasks/STS/kor/KlueSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/STS/kor/KorSTS.py` & `mteb-1.8.0/mteb/tasks/STS/kor/KorSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py` & `mteb-1.8.0/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,62 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks import AbsTaskSTS, CrosslingualTask
 
 _LANGUAGES = {
-    "ko-ko": ["kor-Hang"],
-    "ar-ar": ["ara-Arab"],
-    "en-ar": ["eng-Latn", "ara-Arab"],
-    "en-de": ["eng-Latn", "deu-Latn"],
-    "en-en": ["eng-Latn"],
-    "en-tr": ["eng-Latn", "tur-Latn"],
+    "en": ["eng-Latn"],
+    "de": ["deu-Latn"],
+    "es": ["spa-Latn"],
+    "pl": ["pol-Latn"],
+    "tr": ["tur-Latn"],
+    "ar": ["ara-Arab"],
+    "ru": ["rus-Cyrl"],
+    "zh": ["cmn-Hans"],
+    "fr": ["fra-Latn"],
+    "de-en": ["deu-Latn", "eng-Latn"],
     "es-en": ["spa-Latn", "eng-Latn"],
-    "es-es": ["spa-Latn"],
-    "fr-en": ["fra-Latn", "eng-Latn"],
-    "it-en": ["ita-Latn", "eng-Latn"],
-    "nl-en": ["nld-Latn", "eng-Latn"],
+    "it": ["ita-Latn"],
+    "pl-en": ["pol-Latn", "eng-Latn"],
+    "zh-en": ["cmn-Hans", "eng-Latn"],
+    "es-it": ["spa-Latn", "ita-Latn"],
+    "de-fr": ["deu-Latn", "fra-Latn"],
+    "de-pl": ["deu-Latn", "pol-Latn"],
+    "fr-pl": ["fra-Latn", "pol-Latn"],
 }
 
 
-class STS17Crosslingual(AbsTaskSTS, CrosslingualTask):
+class STS22CrosslingualSTS(AbsTaskSTS, CrosslingualTask):
     metadata = TaskMetadata(
-        name="STS17",
+        name="STS22",
         dataset={
-            "path": "mteb/sts17-crosslingual-sts",
-            "revision": "af5e6fb845001ecf41f4c1e033ce921939a2a68d",
+            "path": "mteb/sts22-crosslingual-sts",
+            "revision": "eea2b4fe26a775864c896887d910b76a8098ad3f",
         },
-        description="STS 2017 dataset",
-        reference="http://alt.qcri.org/semeval2016/task1/",
+        description="SemEval 2022 Task 8: Multilingual News Article Similarity",
+        reference="https://competitions.codalab.org/competitions/33835",
         type="STS",
-        category="s2s",
+        category="p2p",
         eval_splits=["test"],
         eval_langs=_LANGUAGES,
         main_score="cosine_spearman",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples={"test": 500},
-        avg_character_length={"test": 43.3},
+        n_samples={"test": 8060},
+        avg_character_length={"train": 1992.8},
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
         metadata_dict = super().metadata_dict
-        metadata_dict["min_score"] = 0
-        metadata_dict["max_score"] = 5
+        metadata_dict["min_score"] = 1
+        metadata_dict["max_score"] = 4
         return metadata_dict
```

### Comparing `mteb-1.7.9/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py` & `mteb-1.8.0/mteb/tasks/Classification/multilingual/AfriSentiLangClassification.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,96 +1,60 @@
 from __future__ import annotations
 
-import datasets
-
+from mteb.abstasks import AbsTaskClassification
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks import AbsTaskSTS, MultilingualTask
-
-_LANGUAGES = {
-    "en": ["eng-Latn"],
-    "de": ["deu-Latn"],
-    "es": ["spa-Latn"],
-    "fr": ["fra-Latn"],
-    "it": ["ita-Latn"],
-    "nl": ["nld-Latn"],
-    "pl": ["pol-Latn"],
-    "pt": ["por-Latn"],
-    "ru": ["rus-Cyrl"],
-    "zh": ["cmn-Hans"],
-}
-
-_SPLITS = ["dev", "test"]
 
-
-class STSBenchmarkMultilingualSTS(AbsTaskSTS, MultilingualTask):
+class AfriSentiLangClassification(AbsTaskClassification):
     metadata = TaskMetadata(
-        name="STSBenchmarkMultilingualSTS",
+        name="AfriSentiLangClassification",
+        description="AfriSentiLID is the largest LID classification dataset for African Languages.",
         dataset={
-            "path": "PhilipMay/stsb_multi_mt",
-            "revision": "93d57ef91790589e3ce9c365164337a8a78b7632",
+            "path": "HausaNLP/afrisenti-lid-data",
+            "revision": "f17cb5f3ec522ac604601fd09db9fd644ac66ca5",
         },
-        description=(
-            "Semantic Textual Similarity Benchmark (STSbenchmark) dataset,"
-            "but translated using DeepL API."
-        ),
-        reference="https://github.com/PhilipMay/stsb-multi-mt/",
-        type="STS",
+        reference="https://huggingface.co/datasets/HausaNLP/afrisenti-lid-data/",
+        type="Classification",
         category="s2s",
-        eval_splits=_SPLITS,
-        eval_langs=_LANGUAGES,
-        main_score="cosine_spearman",
-        date=None,
-        form=None,
-        domains=None,
-        task_subtypes=None,
-        license=None,
-        socioeconomic_status=None,
-        annotations_creators=None,
-        dialect=None,
-        text_creation=None,
-        bibtex_citation=None,
-        n_samples=None,
-        avg_character_length=None,
+        eval_splits=["test"],
+        eval_langs=[
+            "amh-Ethi",  # Amharic (Ethiopic script)
+            "arq-Arab",
+            "ary-Arab",  # Moroccan Arabic, Standard Arabic (Arabic script)
+            "hau-Latn",  # Hausa (Latin script), additional script if written in Ajami (Arabic script)
+            "ibo-Latn",  # Igbo (Latin script)
+            "kin-Latn",  # Kinyarwanda (Latin script)
+            "por-Latn",  # Portuguese (Latin script)
+            "pcm-Latn",  # Nigerian Pidgin (Latin script)
+            "swa-Latn",  # Swahili (macrolanguage) (Latin script)
+            "twi-Latn",  # Twi (Latin script)
+            "tso-Latn",  # Tsonga (Latin script)
+            "yor-Latn",  # Yoruba (Latin script)
+        ],
+        main_score="accuracy",
+        date=("2023-07-04", "2023-08-04"),
+        form=["written"],
+        domains=["Social"],
+        task_subtypes=["Language identification"],
+        license="cc-by-nc-sa-4.0",
+        socioeconomic_status="low",
+        annotations_creators="derived",
+        dialect=[],
+        text_creation="found",
+        bibtex_citation="""
+        """,
+        n_samples={"test": 5754},
+        avg_character_length={"test": 77.84},
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
         metadata_dict = super().metadata_dict
-        metadata_dict["min_score"] = 0
-        metadata_dict["max_score"] = 5
+        metadata_dict["n_experiments"] = 10
+        metadata_dict["samples_per_label"] = 32
         return metadata_dict
 
-    def load_data(self, **kwargs):
-        if self.data_loaded:
-            return
-
-        def get_dataset_subset(lang: str):
-            """For a specified subset (=language)
-            only get the splits listed in _SPLIT
-            and rename column "score"
-
-            Args:
-                lang (str): _description_
-
-            Returns:
-                datasets.DatasetDict: the dataset of the specified language
-            """
-            subset = datasets.DatasetDict(
-                **dict(
-                    zip(
-                        _SPLITS,
-                        datasets.load_dataset(
-                            name=lang,
-                            split=_SPLITS,
-                            **self.metadata_dict["dataset"],
-                        ),
-                    )
-                )
-            )
-            return subset.rename_column("similarity_score", "score")
-
-        self.dataset = datasets.DatasetDict(
-            **dict(zip(self.langs, [get_dataset_subset(lang) for lang in self.langs]))
+    def dataset_transform(self):
+        self.dataset = self.dataset.rename_column("tweet", "text")
+        self.dataset = self.stratified_subsampling(
+            self.dataset, seed=self.seed, splits=["test"]
         )
-
-        self.data_loaded = True
```

### Comparing `mteb-1.7.9/mteb/tasks/STS/pol/PolishSTS.py` & `mteb-1.8.0/mteb/tasks/STS/pol/PolishSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/STS/ron/RonSTS.py` & `mteb-1.8.0/mteb/tasks/STS/ron/RonSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/STS/spa/STSES.py` & `mteb-1.8.0/mteb/tasks/Classification/kan/KannadaNewsClassification.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,40 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks.AbsTaskSTS import AbsTaskSTS
+from ....abstasks import AbsTaskClassification
 
-_EVAL_SPLIT = "test"
 
-
-class STSES(AbsTaskSTS):
+class KannadaNewsClassification(AbsTaskClassification):
     metadata = TaskMetadata(
-        name="STSES",
+        name="KannadaNewsClassification",
+        description="The Kannada news dataset contains only the headlines of news article in three categories: Entertainment, Tech, and Sports. The data set contains around 6300 news article headlines which are collected from Kannada news websites. The data set has been cleaned and contains train and test set using which can be used to benchmark topic classification models in Kannada.",
         dataset={
-            "path": "PlanTL-GOB-ES/sts-es",
-            "revision": "0912bb6c9393c76d62a7c5ee81c4c817ff47c9f4",
-            "trust_remote_code": True,
+            "path": "Akash190104/kannada_news_classification",
+            "revision": "a470711069906ac0a559defec3b89cb3725601bd",
         },
-        description="Spanish test sets from SemEval-2014 (Agirre et al., 2014) and SemEval-2015 (Agirre et al., 2015)",
-        reference="https://huggingface.co/datasets/PlanTL-GOB-ES/sts-es",
-        type="STS",
+        reference="https://github.com/goru001/nlp-for-kannada",
+        type="Classification",
         category="s2s",
-        eval_splits=[_EVAL_SPLIT],
-        eval_langs=["spa-Latn"],
-        main_score="cosine_spearman",
-        date=None,
-        form=None,
-        domains=None,
-        task_subtypes=None,
-        license=None,
-        socioeconomic_status=None,
-        annotations_creators=None,
-        dialect=None,
-        text_creation=None,
+        eval_splits=["train"],
+        eval_langs=["kan-Knda"],
+        main_score="accuracy",
+        date=("2019-03-17", "2020-08-06"),
+        form=["written"],
+        domains=["News"],
+        task_subtypes=["Topic classification"],
+        license="CC-BY-SA-4.0",
+        socioeconomic_status="mixed",
+        annotations_creators="derived",
+        dialect=[],
+        text_creation="found",
         bibtex_citation=None,
-        n_samples=None,
-        avg_character_length=None,
+        n_samples={"train": 6460},
+        avg_character_length={"train": 65.88},
     )
 
-    @property
-    def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = super().metadata_dict
-        metadata_dict["min_score"] = 0
-        metadata_dict["max_score"] = 5
-        return metadata_dict
-
     def dataset_transform(self):
-        data = self.dataset[_EVAL_SPLIT]
-        data = data.add_column("score", [d["label"] for d in data])
-        self.dataset = {_EVAL_SPLIT: data}
+        self.dataset = self.dataset.rename_column("headline", "text")
+        self.dataset = self.stratified_subsampling(
+            self.dataset, seed=self.seed, splits=["train"]
+        )
```

### Comparing `mteb-1.7.9/mteb/tasks/STS/zho/CMTEBSTS.py` & `mteb-1.8.0/mteb/tasks/STS/zho/CMTEBSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/mteb/tasks/Summarization/eng/SummEvalSummarization.py` & `mteb-1.8.0/mteb/tasks/Classification/vie/VieStudentFeedbackClassification.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,52 @@
 from __future__ import annotations
 
+from mteb.abstasks import AbsTaskClassification
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks import AbsTaskSummarization
+TEST_SAMPLES = 2048
 
 
-class SummEvalSummarization(AbsTaskSummarization):
+class VieStudentFeedbackClassification(AbsTaskClassification):
     metadata = TaskMetadata(
-        name="SummEval",
-        description="News Article Summary Semantic Similarity Estimation.",
-        reference="https://tabilab.cmpe.boun.edu.tr/BIOSSES/DataSet.html",
+        name="VieStudentFeedbackClassification",
+        description="A Vietnamese dataset for classification of student feedback",
+        reference="https://ieeexplore.ieee.org/document/8573337",
         dataset={
-            "path": "mteb/summeval",
-            "revision": "cda12ad7615edc362dbf25a00fdd61d3b1eaf93c",
+            "path": "uitnlp/vietnamese_students_feedback",
+            "revision": "7b56c6cb1c9c8523249f407044c838660df3811a",
         },
-        type="Summarization",
-        category="p2p",
+        type="Classification",
+        category="s2s",
         eval_splits=["test"],
-        eval_langs=["eng-Latn"],
-        main_score="cosine_spearman",
-        date=None,
-        form=None,
-        domains=None,
-        task_subtypes=None,
-        license=None,
-        socioeconomic_status=None,
-        annotations_creators=None,
-        dialect=None,
-        text_creation=None,
-        bibtex_citation=None,
-        n_samples={"test": 2800},
-        avg_character_length={"test": 359.8},
+        eval_langs=["vie-Latn"],
+        main_score="accuracy",
+        date=("2021-12-26", "2021-12-26"),
+        form=["written"],
+        domains=["Reviews"],
+        task_subtypes=["Sentiment/Hate speech"],
+        license="MIT",
+        socioeconomic_status="medium",
+        annotations_creators="human-annotated",
+        dialect=[],
+        text_creation="created",
+        bibtex_citation="""@InProceedings{8573337,
+  author={Nguyen, Kiet Van and Nguyen, Vu Duc and Nguyen, Phu X. V. and Truong, Tham T. H. and Nguyen, Ngan Luu-Thuy},
+  booktitle={2018 10th International Conference on Knowledge and Systems Engineering (KSE)},
+  title={UIT-VSFC: Vietnamese Students’ Feedback Corpus for Sentiment Analysis},
+  year={2018},
+  volume={},
+  number={},
+  pages={19-24},
+  doi={10.1109/KSE.2018.8573337}
+}""",
+        n_samples={"test": TEST_SAMPLES},
+        avg_character_length={"test": 14.22},
     )
 
-    @property
-    def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = super().metadata_dict
-        metadata_dict["min_score"] = 0
-        metadata_dict["max_score"] = 5
-        return metadata_dict
+    def dataset_transform(self):
+        self.dataset = self.dataset.rename_columns(
+            {"sentence": "text", "sentiment": "label"}
+        )
+        self.dataset = self.stratified_subsampling(
+            self.dataset, seed=self.seed, splits=["test"]
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mteb-1.7.9/mteb/tasks/Summarization/fra/SummEvalFrSummarization.py` & `mteb-1.8.0/mteb/tasks/Classification/slv/FrenkSlClassification.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 from __future__ import annotations
 
-from mteb.abstasks import AbsTaskSummarization
+from mteb.abstasks import AbsTaskClassification
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 
-class SummEvalFrSummarization(AbsTaskSummarization):
+class FrenkSlClassification(AbsTaskClassification):
     metadata = TaskMetadata(
-        name="SummEvalFr",
-        description="News Article Summary Semantic Similarity Estimation translated from english to french with DeepL.",
-        reference="https://github.com/Yale-LILY/SummEval",
+        name="FrenkSlClassification",
+        description="Slovenian subset of the FRENK dataset. Also available on HuggingFace dataset hub: English subset, Croatian subset.",
         dataset={
-            "path": "lyon-nlp/summarization-summeval-fr-p2p",
-            "revision": "b385812de6a9577b6f4d0f88c6a6e35395a94054",
+            "path": "classla/FRENK-hate-sl",
+            "revision": "37c8b42c63d4eb75f549679158a85eb5bd984caa",
         },
-        type="Summarization",
-        category="p2p",
+        reference="https://arxiv.org/pdf/1906.02045",
+        type="Classification",
+        category="s2s",
         eval_splits=["test"],
-        eval_langs=["fra-Latn"],
-        main_score="cosine_spearman",
-        date=None,
+        eval_langs=["slv-Latn"],
+        main_score="accuracy",
+        date=("2021-05-28", "2021-05-28"),
         form=["written"],
-        domains=None,
-        task_subtypes=None,
-        license=None,
-        socioeconomic_status=None,
-        annotations_creators=None,
-        dialect=None,
-        text_creation="machine-translated",
-        bibtex_citation=None,
-        n_samples=None,
-        avg_character_length=None,
+        domains=["Social"],
+        task_subtypes=["Sentiment/Hate speech"],
+        license="Not specified",
+        socioeconomic_status="low",
+        annotations_creators="derived",
+        dialect=[],
+        text_creation="found",
+        bibtex_citation="""@misc{ljubešić2019frenk,
+        title={The FRENK Datasets of Socially Unacceptable Discourse in Slovene and English}, 
+        author={Nikola Ljubešić and Darja Fišer and Tomaž Erjavec},
+        year={2019},
+        eprint={1906.02045},
+        archivePrefix={arXiv},
+        primaryClass={cs.CL},
+        url={https://arxiv.org/abs/1906.02045}
+        }""",
+        n_samples={"test": 2177},
+        avg_character_length={"test": 136.61},
     )
 
-    @property
-    def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = super().metadata_dict
-        metadata_dict["min_score"] = 0
-        metadata_dict["max_score"] = 5
-
-        return metadata_dict
+    def dataset_transform(self):
+        self.dataset = self.stratified_subsampling(
+            self.dataset, seed=self.seed, splits=["test"]
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mteb-1.7.9/mteb.egg-info/PKG-INFO` & `mteb-1.8.0/mteb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mteb
-Version: 1.7.9
+Version: 1.8.0
 Summary: Massive Text Embedding Benchmark
 Author-email: MTEB Contributors <niklas@huggingface.co>, nouamane@huggingface.co, info@nils-reimers.de
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -215,28 +215,29 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: datasets>=2.2.0
+Requires-Dist: datasets>=2.19.0
 Requires-Dist: jsonlines
 Requires-Dist: numpy
 Requires-Dist: requests>=2.26.0
 Requires-Dist: scikit_learn>=1.0.2
 Requires-Dist: scipy
 Requires-Dist: sentence_transformers>=2.2.0
 Requires-Dist: torch
 Requires-Dist: tqdm
 Requires-Dist: rich
 Requires-Dist: pytrec-eval-terrier>=0.5.6
 Requires-Dist: pydantic>=2.0.0
 Requires-Dist: typing_extensions
 Requires-Dist: eval_type_backport
+Requires-Dist: polars>=0.20.22
 Provides-Extra: dev
 Requires-Dist: ruff>=0.0.254; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
 
 <h1 align="center">Massive Text Embedding Benchmark</h1>
 
@@ -369,23 +370,26 @@
 
 ### Using a custom model
 
 Models should implement the following interface, implementing an `encode` function taking as inputs a list of sentences, and returning a list of embeddings (embeddings can be `np.array`, `torch.tensor`, etc.). For inspiration, you can look at the [mteb/mtebscripts repo](https://github.com/embeddings-benchmark/mtebscripts) used for running diverse models via SLURM scripts for the paper.
 
 ```python
 class MyModel():
-    def encode(self, sentences: list[str], **kwargs) -> list[np.ndarray] | list[torch.Tensor]:
-        """
-        Returns a list of embeddings for the given sentences.
-        
+    def encode(
+        self, sentences: list[str], prompt: str, **kwargs: Any
+    ) -> torch.Tensor | np.ndarray:
+        """Encodes the given sentences using the encoder.
+
         Args:
-            sentences: List of sentences to encode
+            sentences: The sentences to encode.
+            prompt: The prompt to use. Useful for prompt-based models.
+            **kwargs: Additional arguments to pass to the encoder.
 
         Returns:
-            List of embeddings for the given sentences
+            The encoded sentences.
         """
         pass
 
 model = MyModel()
 evaluation = MTEB(tasks=["Banking77Classification"])
 evaluation.run(model)
 ```
@@ -444,21 +448,23 @@
 
 | Documentation                          |                        |
 | ------------------------------ | ---------------------- |
 | 📋 [Tasks] | Overview of available tasks |
 | 📈 [Leaderboard] | The interactive leaderboard of the benchmark |
 | 🤖 [Adding a model] | Information related to how to submit a model to the leaderboard |
 | 👩‍💻 [Adding a dataset] | How to add a new task/dataset to MTEB | 
+| 👩‍💻 [Adding a leaderboard tab] | How to add a new leaderboard tab to MTEB | 
 | 🤝  [Contributing] | How to contribute to MTEB and set it up for development |
 <!-- | 🌐 [MMTEB] | An open-source effort to extend MTEB to cover a broad set of languages |   -->
 
 [Tasks]: docs/tasks.md
 [Contributing]: CONTRIBUTING.md
 [Adding a model]: docs/adding_a_model.md
 [Adding a dataset]: docs/adding_a_dataset.md
+[Adding a leaderboard tab]: docs/adding_a_leaderboard_tab.md
 [Leaderboard]: https://huggingface.co/spaces/mteb/leaderboard
 [MMTEB]: docs/mmteb/readme.md
 
 ## Citing
 
 MTEB was introduced in "[MTEB: Massive Text Embedding Benchmark](https://arxiv.org/abs/2210.07316)", feel free to cite:
 
@@ -474,9 +480,10 @@
 }
 ```
 
 You may also want to read and cite the amazing work that has extended MTEB & integrated new datasets:
 - Shitao Xiao, Zheng Liu, Peitian Zhang, Niklas Muennighoff. "[C-Pack: Packaged Resources To Advance General Chinese Embedding](https://arxiv.org/abs/2309.07597)" arXiv 2023
 - Michael Günther, Jackmin Ong, Isabelle Mohr, Alaeddine Abdessalem, Tanguy Abel, Mohammad Kalim Akram, Susana Guzman, Georgios Mastrapas, Saba Sturua, Bo Wang, Maximilian Werk, Nan Wang, Han Xiao. "[Jina Embeddings 2: 8192-Token General-Purpose Text Embeddings for Long Documents](https://arxiv.org/abs/2310.19923)" arXiv 2023
 - Silvan Wehrli, Bert Arnrich, Christopher Irrgang. "[German Text Embedding Clustering Benchmark](https://arxiv.org/abs/2401.02709)" arXiv 2024
+- Dawei Zhu, Liang Wang, Nan Yang, Yifan Song, Wenhao Wu, Furu Wei, and Sujian Li. "[LongEmbed: Extending Embedding Models for Long Context Retrieval](https://arxiv.org/abs/2404.12096)" arXiv 2024
 
 For works that have used MTEB for benchmarking, you can find them on the [leaderboard](https://huggingface.co/spaces/mteb/leaderboard).
```

### Comparing `mteb-1.7.9/pyproject.toml` & `mteb-1.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mteb"
-version = "1.7.9"
+version = "1.8.0"
 description = "Massive Text Embedding Benchmark"
 readme = "README.md"
 authors = [
     { name = "MTEB Contributors", email = "niklas@huggingface.co" },
     { email = "nouamane@huggingface.co" },
     { email = "info@nils-reimers.de" },
 ]
@@ -21,28 +21,29 @@
     "Intended Audience :: Information Technology",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
 ]
 requires-python = ">=3.8"
 dependencies = [
-    "datasets>=2.2.0",
+    "datasets>=2.19.0",
     "jsonlines",
     "numpy",
     "requests>=2.26.0",
     "scikit_learn>=1.0.2",
     "scipy",
     "sentence_transformers>=2.2.0",
     "torch",
     "tqdm",
     "rich",
     "pytrec-eval-terrier>=0.5.6",
     "pydantic>=2.0.0",
     "typing_extensions",
     "eval_type_backport",
+    "polars>=0.20.22",
 ]
 
 
 [project.urls]
 homepage = "https://github.com/embeddings-benchmark/mteb"
 "Huggingface Organization" = "https://huggingface.co/mteb"
 "Source Code" = "https://github.com/embeddings-benchmark/mteb"
```

### Comparing `mteb-1.7.9/results/GritLM__GritLM-7B/Core17InstructionRetrieval.json` & `mteb-1.8.0/results/GritLM__GritLM-7B/Core17InstructionRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/GritLM__GritLM-7B/News21InstructionRetrieval.json` & `mteb-1.8.0/results/GritLM__GritLM-7B/News21InstructionRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/GritLM__GritLM-7B/Robust04InstructionRetrieval.json` & `mteb-1.8.0/results/GritLM__GritLM-7B/Robust04InstructionRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/dangvantuan/sentence-camembert-base/AlloprofRetrieval.json` & `mteb-1.8.0/results/dangvantuan/sentence-camembert-base/AlloprofRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/dangvantuan/sentence-camembert-base/AmazonReviewsClassification.json` & `mteb-1.8.0/results/dangvantuan/sentence-camembert-base/AmazonReviewsClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/dangvantuan/sentence-camembert-base/BSARDRetrieval.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-small/TurHistQuadRetrieval.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5625%*

 * *Differences: {"'dataset_revision'": "'2a2b8ddecf1189f530676244d0751e1d0a569e03'",*

 * * "'mteb_dataset_name'": "'TurHistQuadRetrieval'",*

 * * "'mteb_version'": "'1.6.8'",*

 * * "'test'": "{'evaluation_time': 47.25, 'map_at_1': 0.21924, 'map_at_10': 0.32851, 'map_at_100': "*

 * *           "0.34157, 'map_at_1000': 0.34355, 'map_at_20': 0.33563, 'map_at_3': 0.29777, "*

 * *           "'map_at_5': 0.31447, 'mrr_at_1': 0.44336, 'mrr_at_10': 0.57768, 'mrr_at_100': 0.58363, "*

 * *           "'mrr_at_1000': 0.58379, 'mrr_at_20': 0.5814, 'mrr_at_3': 0.550 […]*

```diff
@@ -1,43 +1,43 @@
 {
-    "dataset_revision": "5effa1b9b5fa3b0f9e12523e6e43e5f86a6e6d59",
-    "mteb_dataset_name": "BSARDRetrieval",
-    "mteb_version": "1.6.16",
+    "dataset_revision": "2a2b8ddecf1189f530676244d0751e1d0a569e03",
+    "mteb_dataset_name": "TurHistQuadRetrieval",
+    "mteb_version": "1.6.8",
     "test": {
-        "evaluation_time": 419.28,
-        "map_at_1": 0.0,
-        "map_at_10": 0.0,
-        "map_at_100": 0.0,
-        "map_at_1000": 0.00017,
-        "map_at_20": 0.0,
-        "map_at_3": 0.0,
-        "map_at_5": 0.0,
-        "mrr_at_1": 0.0,
-        "mrr_at_10": 0.0,
-        "mrr_at_100": 0.0,
-        "mrr_at_1000": 0.00017,
-        "mrr_at_20": 0.0,
-        "mrr_at_3": 0.0,
-        "mrr_at_5": 0.0,
-        "ndcg_at_1": 0.0,
-        "ndcg_at_10": 0.0,
-        "ndcg_at_100": 0.0,
-        "ndcg_at_1000": 0.00809,
-        "ndcg_at_20": 0.0,
-        "ndcg_at_3": 0.0,
-        "ndcg_at_5": 0.0,
-        "precision_at_1": 0.0,
-        "precision_at_10": 0.0,
-        "precision_at_100": 0.0,
-        "precision_at_1000": 7e-05,
-        "precision_at_20": 0.0,
-        "precision_at_3": 0.0,
-        "precision_at_5": 0.0,
-        "recall_at_1": 0.0,
-        "recall_at_10": 0.0,
-        "recall_at_100": 0.0,
-        "recall_at_1000": 0.07207,
-        "recall_at_20": 0.0,
-        "recall_at_3": 0.0,
-        "recall_at_5": 0.0
+        "evaluation_time": 47.25,
+        "map_at_1": 0.21924,
+        "map_at_10": 0.32851,
+        "map_at_100": 0.34157,
+        "map_at_1000": 0.34355,
+        "map_at_20": 0.33563,
+        "map_at_3": 0.29777,
+        "map_at_5": 0.31447,
+        "mrr_at_1": 0.44336,
+        "mrr_at_10": 0.57768,
+        "mrr_at_100": 0.58363,
+        "mrr_at_1000": 0.58379,
+        "mrr_at_20": 0.5814,
+        "mrr_at_3": 0.55078,
+        "mrr_at_5": 0.5667,
+        "ndcg_at_1": 0.43848,
+        "ndcg_at_10": 0.43286,
+        "ndcg_at_100": 0.48571,
+        "ndcg_at_1000": 0.52601,
+        "ndcg_at_20": 0.45296,
+        "ndcg_at_3": 0.37663,
+        "ndcg_at_5": 0.40394,
+        "precision_at_1": 0.43848,
+        "precision_at_10": 0.09902,
+        "precision_at_100": 0.01413,
+        "precision_at_1000": 0.00196,
+        "precision_at_20": 0.05601,
+        "precision_at_3": 0.24544,
+        "precision_at_5": 0.16895,
+        "recall_at_1": 0.21924,
+        "recall_at_10": 0.49512,
+        "recall_at_100": 0.70654,
+        "recall_at_1000": 0.97754,
+        "recall_at_20": 0.56006,
+        "recall_at_3": 0.36816,
+        "recall_at_5": 0.42236
     }
 }
```

### Comparing `mteb-1.7.9/results/dangvantuan/sentence-camembert-base/MTOPDomainClassification.json` & `mteb-1.8.0/results/dangvantuan/sentence-camembert-base/MTOPDomainClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/dangvantuan/sentence-camembert-base/MTOPIntentClassification.json` & `mteb-1.8.0/results/dangvantuan/sentence-camembert-base/MTOPIntentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/dangvantuan/sentence-camembert-base/MassiveIntentClassification.json` & `mteb-1.8.0/results/dangvantuan/sentence-camembert-base/MassiveIntentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/dangvantuan/sentence-camembert-base/MassiveScenarioClassification.json` & `mteb-1.8.0/results/dangvantuan/sentence-camembert-base/MassiveScenarioClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/dangvantuan/sentence-camembert-base/MintakaRetrieval.json` & `mteb-1.8.0/results/dangvantuan/sentence-camembert-base/MintakaRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/dangvantuan/sentence-camembert-base/OpusparcusPC.json` & `mteb-1.8.0/results/dangvantuan/sentence-camembert-base/OpusparcusPC.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/dangvantuan/sentence-camembert-base/PawsX.json` & `mteb-1.8.0/results/dangvantuan/sentence-camembert-base/PawsX.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/dangvantuan/sentence-camembert-base/SICKFr.json` & `mteb-1.8.0/results/dangvantuan/sentence-camembert-base/SICKFr.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/dangvantuan/sentence-camembert-base/STSBenchmarkMultilingualSTS.json` & `mteb-1.8.0/results/dangvantuan/sentence-camembert-base/STSBenchmarkMultilingualSTS.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/dangvantuan/sentence-camembert-base/SyntecRetrieval.json` & `mteb-1.8.0/results/dangvantuan/sentence-camembert-base/SyntecRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/dangvantuan/sentence-camembert-base/XPQARetrieval.json` & `mteb-1.8.0/results/dangvantuan/sentence-camembert-base/XPQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/intfloat__e5-small-v2/Core17InstructionRetrieval.json` & `mteb-1.8.0/results/intfloat__e5-small-v2/Core17InstructionRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/intfloat__e5-small-v2/News21InstructionRetrieval.json` & `mteb-1.8.0/results/intfloat__e5-small-v2/News21InstructionRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/intfloat__e5-small-v2/Robust04InstructionRetrieval.json` & `mteb-1.8.0/results/intfloat__e5-small-v2/Robust04InstructionRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-base/CroatianSentimentClassification.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-base/CroatianSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-base/CzechSubjectivityClassification.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-base/CzechSubjectivityClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-base/MalteseSentimentClassification.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-base/MalteseSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-small/BulgarianSentimentClassification.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-small/MovieReviewSentimentClassification.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6%*

 * *Differences: {"'dataset_revision'": "'a4654f4896408912913a62ace89614879a549287'",*

 * * "'mteb_dataset_name'": "'MovieReviewSentimentClassification'",*

 * * "'mteb_version'": "'1.7.14'",*

 * * "'test'": "{'accuracy': 0.716650390625, 'accuracy_stderr': 0.028154865937927428, 'ap': "*

 * *           "0.6393496969615753, 'ap_stderr': 0.02855983599862856, 'evaluation_time': 27.35, 'f1': "*

 * *           "0.7140562409393475, 'f1_stderr': 0.027686299045850998, 'main_score': 0.716650390625}",*

 * * "'validation'": "{'accuracy': 0.715576171875, 'accuracy_st […]*

```diff
@@ -1,25 +1,25 @@
 {
-    "dataset_revision": "c0d5c781a115d570b8acceb14928ffb99543bb74",
-    "mteb_dataset_name": "BulgarianSentimentClassification",
-    "mteb_version": "1.6.12",
+    "dataset_revision": "a4654f4896408912913a62ace89614879a549287",
+    "mteb_dataset_name": "MovieReviewSentimentClassification",
+    "mteb_version": "1.7.14",
     "test": {
-        "accuracy": 0.7251046025104604,
-        "accuracy_stderr": 0.03945502514001783,
-        "ap": 0.8839028389202893,
-        "ap_stderr": 0.01775102786465037,
-        "evaluation_time": 3.3,
-        "f1": 0.6649167482675631,
-        "f1_stderr": 0.03895081321852516,
-        "main_score": 0.7251046025104604
+        "accuracy": 0.716650390625,
+        "accuracy_stderr": 0.028154865937927428,
+        "ap": 0.6393496969615753,
+        "ap_stderr": 0.02855983599862856,
+        "evaluation_time": 27.35,
+        "f1": 0.7140562409393475,
+        "f1_stderr": 0.027686299045850998,
+        "main_score": 0.716650390625
     },
     "validation": {
-        "accuracy": 0.7316229116945108,
-        "accuracy_stderr": 0.040909907906665426,
-        "ap": 0.9371518735025541,
-        "ap_stderr": 0.008238480175131136,
-        "evaluation_time": 5.48,
-        "f1": 0.6300379798171928,
-        "f1_stderr": 0.03474752659073286,
-        "main_score": 0.7316229116945108
+        "accuracy": 0.715576171875,
+        "accuracy_stderr": 0.033350896182165246,
+        "ap": 0.6466619388918061,
+        "ap_stderr": 0.03281559658058928,
+        "evaluation_time": 27.54,
+        "f1": 0.7133101647112581,
+        "f1_stderr": 0.0333552288626829,
+        "main_score": 0.715576171875
     }
 }
```

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-small/CodeSearchNetRetrieval.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-small/CodeSearchNetRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-small/CroatianSentimentClassification.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-small/FilipinoHateSpeechClassification.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6%*

 * *Differences: {"'dataset_revision'": "'1994e9bb7f3ec07518e3f0d9e870cb293e234686'",*

 * * "'mteb_dataset_name'": "'FilipinoHateSpeechClassification'",*

 * * "'mteb_version'": "'1.7.14'",*

 * * "'test'": "{'accuracy': 0.58359375, 'accuracy_stderr': 0.04045951590625083, 'ap': "*

 * *           "0.5183748795941082, 'ap_stderr': 0.026155224372107547, 'evaluation_time': 7.17, 'f1': "*

 * *           "0.576893865333713, 'f1_stderr': 0.04030538689824078, 'main_score': 0.58359375}",*

 * * "'validation'": "{'accuracy': 0.57998046875, 'accuracy_stderr': 0.04052 […]*

```diff
@@ -1,25 +1,25 @@
 {
-    "dataset_revision": "255da5c6b54c95faf74aba6d6cad9b2e176bf90a",
-    "mteb_dataset_name": "CroatianSentimentClassification",
-    "mteb_version": "1.6.12",
+    "dataset_revision": "1994e9bb7f3ec07518e3f0d9e870cb293e234686",
+    "mteb_dataset_name": "FilipinoHateSpeechClassification",
+    "mteb_version": "1.7.14",
     "test": {
-        "accuracy": 0.799771167048055,
-        "accuracy_stderr": 0.046977682903828685,
-        "ap": 0.9001937067150981,
-        "ap_stderr": 0.018403106906389386,
-        "evaluation_time": 3.33,
-        "f1": 0.7477748016816385,
-        "f1_stderr": 0.04572549702814684,
-        "main_score": 0.799771167048055
+        "accuracy": 0.58359375,
+        "accuracy_stderr": 0.04045951590625083,
+        "ap": 0.5183748795941082,
+        "ap_stderr": 0.026155224372107547,
+        "evaluation_time": 7.17,
+        "f1": 0.576893865333713,
+        "f1_stderr": 0.04030538689824078,
+        "main_score": 0.58359375
     },
     "validation": {
-        "accuracy": 0.8214953271028037,
-        "accuracy_stderr": 0.036244335382552006,
-        "ap": 0.9109813285666689,
-        "ap_stderr": 0.010190251621120913,
-        "evaluation_time": 5.61,
-        "f1": 0.7657761043142386,
-        "f1_stderr": 0.03510624637316594,
-        "main_score": 0.8214953271028037
+        "accuracy": 0.57998046875,
+        "accuracy_stderr": 0.04052722609169668,
+        "ap": 0.5067390857072789,
+        "ap_stderr": 0.02591176836681942,
+        "evaluation_time": 8.38,
+        "f1": 0.5733334721155943,
+        "f1_stderr": 0.03945981336363871,
+        "main_score": 0.57998046875
     }
 }
```

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-small/CzechSubjectivityClassification.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-small/CzechSubjectivityClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-small/DanFEVER.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-small/DanFEVER.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-small/EstQA.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-small/EstQA.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-small/FQuADRetrieval.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-small/FQuADRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-small/FilipinoHateSpeechClassification.json` & `mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/UkrFormalityClassification.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.375%*

 * *Differences: {"'dataset_revision'": "'671d1e6bbf45a74ef21af351fd4ef7b32b7856f8'",*

 * * "'mteb_dataset_name'": "'UkrFormalityClassification'",*

 * * "'mteb_version'": "'1.6.37'",*

 * * "'test'": "{'accuracy': 0.528076171875, 'accuracy_stderr': 0.030777409502741826, 'ap': "*

 * *           "0.4423356000929221, 'ap_stderr': 0.010210226392447973, 'evaluation_time': 5.95, 'f1': "*

 * *           "0.5084647911438317, 'f1_stderr': 0.022028997054790573, 'main_score': 0.528076171875}",*

 * * "'train'": "OrderedDict([('accuracy', 0.515625), ('accuracy_stderr […]*

```diff
@@ -1,25 +1,25 @@
 {
-    "dataset_revision": "1994e9bb7f3ec07518e3f0d9e870cb293e234686",
-    "mteb_dataset_name": "FilipinoHateSpeechClassification",
-    "mteb_version": "1.7.0",
+    "dataset_revision": "671d1e6bbf45a74ef21af351fd4ef7b32b7856f8",
+    "mteb_dataset_name": "UkrFormalityClassification",
+    "mteb_version": "1.6.37",
     "test": {
-        "accuracy": 0.588623046875,
-        "accuracy_stderr": 0.04424121838518151,
-        "ap": 0.5235485680653846,
-        "ap_stderr": 0.0292128856610349,
-        "evaluation_time": 3.28,
-        "f1": 0.5815646745354887,
-        "f1_stderr": 0.04485825288601201,
-        "main_score": 0.588623046875
+        "accuracy": 0.528076171875,
+        "accuracy_stderr": 0.030777409502741826,
+        "ap": 0.4423356000929221,
+        "ap_stderr": 0.010210226392447973,
+        "evaluation_time": 5.95,
+        "f1": 0.5084647911438317,
+        "f1_stderr": 0.022028997054790573,
+        "main_score": 0.528076171875
     },
-    "validation": {
-        "accuracy": 0.57958984375,
-        "accuracy_stderr": 0.042122005910901344,
-        "ap": 0.49819582657111905,
-        "ap_stderr": 0.02577058528891724,
-        "evaluation_time": 4.19,
-        "f1": 0.5716219492625749,
-        "f1_stderr": 0.042080406267862754,
-        "main_score": 0.57958984375
+    "train": {
+        "accuracy": 0.515625,
+        "accuracy_stderr": 0.017610646998202893,
+        "ap": 0.5087213333014945,
+        "ap_stderr": 0.009644894062476045,
+        "evaluation_time": 10.27,
+        "f1": 0.5019099055689374,
+        "f1_stderr": 0.014889799683856533,
+        "main_score": 0.515625
     }
 }
```

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-small/FinParaSTS.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-small/FinParaSTS.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-small/GermanDPR.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-small/GermanDPR.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-small/GreekLegalCodeClassification.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-small/GreekLegalCodeClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-small/GreekSentimentClassification.json` & `mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GreekLegalCodeClassification.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.575%*

 * *Differences: {"'dataset_revision'": "'de0fdb34424f07d1ac6f0ede23ee0ed44bd9f5d1'",*

 * * "'mteb_dataset_name'": "'GreekLegalCodeClassification'",*

 * * "'mteb_version'": "'1.6.36'",*

 * * "'test'": "{'accuracy': 0.290380859375, 'accuracy_stderr': 0.00819978191737022, "*

 * *           "'evaluation_time': 88.71, 'f1': 0.23772795241695582, 'f1_stderr': "*

 * *           "0.008730309299456626, 'main_score': 0.290380859375, delete: ['ap', 'ap_stderr']}",*

 * * "'validation'": "{'accuracy': 0.303564453125, 'accuracy_stderr': 0.010601551885184904, "*

 * *       […]*

```diff
@@ -1,25 +1,21 @@
 {
-    "dataset_revision": "94b245f3ccdf8e8b2cbf8f13f55eee820b70eccf",
-    "mteb_dataset_name": "GreekSentimentClassification",
-    "mteb_version": "1.6.38",
+    "dataset_revision": "de0fdb34424f07d1ac6f0ede23ee0ed44bd9f5d1",
+    "mteb_dataset_name": "GreekLegalCodeClassification",
+    "mteb_version": "1.6.36",
     "test": {
-        "accuracy": 0.8250325945241201,
-        "accuracy_stderr": 0.024390114548052354,
-        "ap": 0.7900660680219003,
-        "ap_stderr": 0.023034664377022326,
-        "evaluation_time": 38.04,
-        "f1": 0.8189927893165387,
-        "f1_stderr": 0.028510112712501045,
-        "main_score": 0.8250325945241201
+        "accuracy": 0.290380859375,
+        "accuracy_stderr": 0.00819978191737022,
+        "evaluation_time": 88.71,
+        "f1": 0.23772795241695582,
+        "f1_stderr": 0.008730309299456626,
+        "main_score": 0.290380859375
     },
     "validation": {
-        "accuracy": 0.829242819843342,
-        "accuracy_stderr": 0.030002260934147727,
-        "ap": 0.8002567395633753,
-        "ap_stderr": 0.030296552949220703,
-        "evaluation_time": 31.08,
-        "f1": 0.8243223776179838,
-        "f1_stderr": 0.033820296975630666,
-        "main_score": 0.829242819843342
+        "accuracy": 0.303564453125,
+        "accuracy_stderr": 0.010601551885184904,
+        "evaluation_time": 89.06,
+        "f1": 0.23970657874134466,
+        "f1_stderr": 0.008710551186652492,
+        "main_score": 0.303564453125
     }
 }
```

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-small/HunSum2AbstractiveRetrieval.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-small/HunSum2AbstractiveRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-small/IN22ConvBitextMining.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-small/IN22ConvBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-small/IN22GenBitextMining.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-small/IN22GenBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-small/IndicSentimentClassification.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-small/IndicSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-small/JaQuADRetrieval.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-small/JaQuADRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-small/LEMBNarrativeQARetrieval.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-small/LEMBNarrativeQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-small/LEMBNeedleRetrieval.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-small/LEMBNeedleRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-small/LEMBPasskeyRetrieval.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-small/LEMBPasskeyRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-small/LEMBQMSumRetrieval.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-small/LEMBQMSumRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-small/LEMBSummScreenFDRetrieval.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-small/LEMBSummScreenFDRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-small/LEMBWikimQARetrieval.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-small/LEMBWikimQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-small/MalteseSentimentClassification.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-small/SanskritShlokasClassification.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.3645833333333333%*

 * *Differences: {"'dataset_revision'": "'5a79d6472db143690c7ce6e974995d3610eee7f0'",*

 * * "'mteb_dataset_name'": "'SanskritShlokasClassification'",*

 * * "'mteb_version'": "'1.7.6'",*

 * * "'train'": "OrderedDict([('accuracy', 0.7861618798955614), ('accuracy_stderr', "*

 * *            "0.03234754078233619), ('evaluation_time', 5.71), ('f1', 0.785558565911011), "*

 * *            "('f1_stderr', 0.0311303300468244), ('main_score', 0.7861618798955614)])",*

 * * "'validation'": "{'accuracy': 0.775, 'accuracy_stderr': 0.0489028941429396, 'evaluation_time' […]*

```diff
@@ -1,25 +1,21 @@
 {
-    "dataset_revision": "fd47b916f9ebb5d27b0e583de9d2b2db39f7dda2",
-    "mteb_dataset_name": "MalteseSentimentClassification",
-    "mteb_version": "1.6.12",
-    "test": {
-        "accuracy": 0.5871345029239766,
-        "accuracy_stderr": 0.04752339100329834,
-        "ap": 0.40215222812168305,
-        "ap_stderr": 0.02713279956287242,
-        "evaluation_time": 3.08,
-        "f1": 0.5685613616801592,
-        "f1_stderr": 0.040561161547649084,
-        "main_score": 0.5871345029239766
+    "dataset_revision": "5a79d6472db143690c7ce6e974995d3610eee7f0",
+    "mteb_dataset_name": "SanskritShlokasClassification",
+    "mteb_version": "1.7.6",
+    "train": {
+        "accuracy": 0.7861618798955614,
+        "accuracy_stderr": 0.03234754078233619,
+        "evaluation_time": 5.71,
+        "f1": 0.785558565911011,
+        "f1_stderr": 0.0311303300468244,
+        "main_score": 0.7861618798955614
     },
     "validation": {
-        "accuracy": 0.6188235294117647,
-        "accuracy_stderr": 0.05523150397320236,
-        "ap": 0.4226946899300195,
-        "ap_stderr": 0.03816783230056503,
-        "evaluation_time": 5.06,
-        "f1": 0.6017270223460253,
-        "f1_stderr": 0.050922496714521905,
-        "main_score": 0.6188235294117647
+        "accuracy": 0.775,
+        "accuracy_stderr": 0.0489028941429396,
+        "evaluation_time": 1.43,
+        "f1": 0.7820968680935053,
+        "f1_stderr": 0.046782872469135026,
+        "main_score": 0.775
     }
 }
```

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-small/MedicalQARetrieval.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-small/MedicalQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-small/MovieReviewSentimentClassification.json` & `mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PersianFoodSentimentClassification.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6%*

 * *Differences: {"'dataset_revision'": "'92ba517dfd22f6334111ad84154d16a2890f5b1d'",*

 * * "'mteb_dataset_name'": "'PersianFoodSentimentClassification'",*

 * * "'mteb_version'": "'1.6.23'",*

 * * "'test'": "{'accuracy': 0.7462890625, 'accuracy_stderr': 0.04373713712975096, 'ap': "*

 * *           "0.6931826089298969, 'ap_stderr': 0.05202952761316073, 'evaluation_time': 11.52, 'f1': "*

 * *           "0.7412118753251911, 'f1_stderr': 0.050463894100974196, 'main_score': 0.7462890625}",*

 * * "'validation'": "{'accuracy': 0.7244140625, 'accuracy_stderr':  […]*

```diff
@@ -1,25 +1,25 @@
 {
-    "dataset_revision": "a4654f4896408912913a62ace89614879a549287",
-    "mteb_dataset_name": "MovieReviewSentimentClassification",
-    "mteb_version": "1.6.3",
+    "dataset_revision": "92ba517dfd22f6334111ad84154d16a2890f5b1d",
+    "mteb_dataset_name": "PersianFoodSentimentClassification",
+    "mteb_version": "1.6.23",
     "test": {
-        "accuracy": 0.71259765625,
-        "accuracy_stderr": 0.02655118813595098,
-        "ap": 0.6368737342492778,
-        "ap_stderr": 0.025522744681666484,
-        "evaluation_time": 251.07,
-        "f1": 0.7098389153838554,
-        "f1_stderr": 0.025949581387596135,
-        "main_score": 0.71259765625
+        "accuracy": 0.7462890625,
+        "accuracy_stderr": 0.04373713712975096,
+        "ap": 0.6931826089298969,
+        "ap_stderr": 0.05202952761316073,
+        "evaluation_time": 11.52,
+        "f1": 0.7412118753251911,
+        "f1_stderr": 0.050463894100974196,
+        "main_score": 0.7462890625
     },
     "validation": {
-        "accuracy": 0.70693359375,
-        "accuracy_stderr": 0.03255177408707274,
-        "ap": 0.6209567664315121,
-        "ap_stderr": 0.030557991003544345,
-        "evaluation_time": 261.1,
-        "f1": 0.7039163223038187,
-        "f1_stderr": 0.0322207234055602,
-        "main_score": 0.70693359375
+        "accuracy": 0.7244140625,
+        "accuracy_stderr": 0.042048472453164475,
+        "ap": 0.6658035802345703,
+        "ap_stderr": 0.04752832021439103,
+        "evaluation_time": 21.96,
+        "f1": 0.7191473875821562,
+        "f1_stderr": 0.04639202898224792,
+        "main_score": 0.7244140625
     }
 }
```

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-small/NeuCLIR2022Retrieval.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-small/NeuCLIR2022Retrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-small/NeuCLIR2023Retrieval.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-small/NeuCLIR2023Retrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-small/NorQuadRetrieval.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-small/NorQuadRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-small/PersianFoodSentimentClassification.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-small/PersianFoodSentimentClassification.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8%*

 * *Differences: {"'mteb_version'": "'1.7.13'",*

 * * "'test'": "{'accuracy': 0.743701171875, 'accuracy_stderr': 0.027541356633721408, 'ap': "*

 * *           "0.6905292631479201, 'ap_stderr': 0.02991974545843889, 'evaluation_time': 7.49, 'f1': "*

 * *           "0.740601460820036, 'f1_stderr': 0.029892432663399013, 'main_score': 0.743701171875}",*

 * * "'validation'": "{'accuracy': 0.753564453125, 'accuracy_stderr': 0.032625848225642, 'ap': "*

 * *                 "0.7008866195287176, 'ap_stderr': 0.034855399642854494, 'evaluation_time': 8.44, "*

 * *  […]*

```diff
@@ -1,25 +1,25 @@
 {
     "dataset_revision": "92ba517dfd22f6334111ad84154d16a2890f5b1d",
     "mteb_dataset_name": "PersianFoodSentimentClassification",
-    "mteb_version": "1.6.23",
+    "mteb_version": "1.7.13",
     "test": {
-        "accuracy": 0.76162109375,
-        "accuracy_stderr": 0.029608370076944144,
-        "ap": 0.7107301145647525,
-        "ap_stderr": 0.034055419244529754,
-        "evaluation_time": 12.65,
-        "f1": 0.7591600296974221,
-        "f1_stderr": 0.03217369721760639,
-        "main_score": 0.76162109375
+        "accuracy": 0.743701171875,
+        "accuracy_stderr": 0.027541356633721408,
+        "ap": 0.6905292631479201,
+        "ap_stderr": 0.02991974545843889,
+        "evaluation_time": 7.49,
+        "f1": 0.740601460820036,
+        "f1_stderr": 0.029892432663399013,
+        "main_score": 0.743701171875
     },
     "validation": {
-        "accuracy": 0.7482421875,
-        "accuracy_stderr": 0.027419676950723386,
-        "ap": 0.6907767680040339,
-        "ap_stderr": 0.03010830629103603,
-        "evaluation_time": 19.97,
-        "f1": 0.745168999799412,
-        "f1_stderr": 0.029181618331629827,
-        "main_score": 0.7482421875
+        "accuracy": 0.753564453125,
+        "accuracy_stderr": 0.032625848225642,
+        "ap": 0.7008866195287176,
+        "ap_stderr": 0.034855399642854494,
+        "evaluation_time": 8.44,
+        "f1": 0.7510130825181032,
+        "f1_stderr": 0.03460891571546719,
+        "main_score": 0.753564453125
     }
 }
```

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-small/SNLRetrieval.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-small/SNLRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-small/SweFaqRetrieval.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-small/SweFaqRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-small/SwednRetrieval.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-small/SwednRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-small/SyntecRetrieval.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-small/SyntecRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-small/TV2Nordretrieval.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-small/TV2Nordretrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-small/TwitterHjerneRetrieval.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-small/TwitterHjerneRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-small/VieQuADRetrieval.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-small/VieQuADRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/intfloat__multilingual-e5-small/WikiClusteringP2P.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-small/WikiClusteringP2P.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/DanFEVER.json` & `mteb-1.8.0/results/sentence-transformers__all-MiniLM-L6-v2/DanFEVER.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/NorQuadRetrieval.json` & `mteb-1.8.0/results/sentence-transformers__all-MiniLM-L6-v2/NorQuadRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/SNLRetrieval.json` & `mteb-1.8.0/results/sentence-transformers__all-MiniLM-L6-v2/SNLRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/SweFaqRetrieval.json` & `mteb-1.8.0/results/sentence-transformers__all-MiniLM-L6-v2/SweFaqRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/SwednRetrieval.json` & `mteb-1.8.0/results/sentence-transformers__all-MiniLM-L6-v2/SwednRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/TV2Nordretrieval.json` & `mteb-1.8.0/results/sentence-transformers__all-MiniLM-L6-v2/TV2Nordretrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__all-MiniLM-L6-v2/TwitterHjerneRetrieval.json` & `mteb-1.8.0/results/sentence-transformers__all-MiniLM-L6-v2/TwitterHjerneRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BUCC.json` & `mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BUCC.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BulgarianSentimentClassification.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-small/FilipinoShopeeReviewsClassification.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.575%*

 * *Differences: {"'dataset_revision'": "'d096f402fdc76886458c0cfb5dedc829bea2b935'",*

 * * "'mteb_dataset_name'": "'FilipinoShopeeReviewsClassification'",*

 * * "'mteb_version'": "'1.7.58'",*

 * * "'test'": "{'accuracy': 0.335791015625, 'accuracy_stderr': 0.024496005063450725, "*

 * *           "'evaluation_time': 4.45, 'f1': 0.32046860152589846, 'f1_stderr': 0.02309877466734575, "*

 * *           "'main_score': 0.335791015625, delete: ['ap', 'ap_stderr']}",*

 * * "'validation'": "{'accuracy': 0.33779296875, 'accuracy_stderr': 0.0267342791129198, "*

 * *    […]*

```diff
@@ -1,25 +1,21 @@
 {
-    "dataset_revision": "c0d5c781a115d570b8acceb14928ffb99543bb74",
-    "mteb_dataset_name": "BulgarianSentimentClassification",
-    "mteb_version": "1.6.12",
+    "dataset_revision": "d096f402fdc76886458c0cfb5dedc829bea2b935",
+    "mteb_dataset_name": "FilipinoShopeeReviewsClassification",
+    "mteb_version": "1.7.58",
     "test": {
-        "accuracy": 0.7785415421398685,
-        "accuracy_stderr": 0.06046594589367263,
-        "ap": 0.9138203738562648,
-        "ap_stderr": 0.016358122993814245,
-        "evaluation_time": 3.34,
-        "f1": 0.7279047189447724,
-        "f1_stderr": 0.055918407384301656,
-        "main_score": 0.7785415421398685
+        "accuracy": 0.335791015625,
+        "accuracy_stderr": 0.024496005063450725,
+        "evaluation_time": 4.45,
+        "f1": 0.32046860152589846,
+        "f1_stderr": 0.02309877466734575,
+        "main_score": 0.335791015625
     },
     "validation": {
-        "accuracy": 0.7890214797136038,
-        "accuracy_stderr": 0.06444753768326883,
-        "ap": 0.9570004694941152,
-        "ap_stderr": 0.010189851245946924,
-        "evaluation_time": 5.38,
-        "f1": 0.6974774929981921,
-        "f1_stderr": 0.06102218982582699,
-        "main_score": 0.7890214797136038
+        "accuracy": 0.33779296875,
+        "accuracy_stderr": 0.0267342791129198,
+        "evaluation_time": 6.34,
+        "f1": 0.32315488500253814,
+        "f1_stderr": 0.024768921377316615,
+        "main_score": 0.33779296875
     }
 }
```

### Comparing `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CodeSearchNetRetrieval.json` & `mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CodeSearchNetRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CroatianSentimentClassification.json` & `mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CataloniaTweetClassification.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.40499999999999997%*

 * *Differences: {"'dataset_revision'": "'cf24d44e517efa534f048e5fc5981f399ed25bee'",*

 * * "'mteb_dataset_name'": "'CataloniaTweetClassification'",*

 * * "'mteb_version'": "'1.6.37'",*

 * * "'test'": "{'evaluation_time': 42.22, 'catalan': OrderedDict([('accuracy', 0.43019999999999997), "*

 * *           "('accuracy_stderr', 0.04952888046382634), ('f1', 0.4126601099708986), ('f1_stderr', "*

 * *           "0.04601771378692479), ('main_score', 0.43019999999999997)]), 'spanish': "*

 * *           "OrderedDict([('accuracy', 0.42794999999999994), ('accuracy […]*

```diff
@@ -1,25 +1,22 @@
 {
-    "dataset_revision": "255da5c6b54c95faf74aba6d6cad9b2e176bf90a",
-    "mteb_dataset_name": "CroatianSentimentClassification",
-    "mteb_version": "1.6.12",
+    "dataset_revision": "cf24d44e517efa534f048e5fc5981f399ed25bee",
+    "mteb_dataset_name": "CataloniaTweetClassification",
+    "mteb_version": "1.6.37",
     "test": {
-        "accuracy": 0.7574370709382152,
-        "accuracy_stderr": 0.08020913236290611,
-        "ap": 0.8729234268997568,
-        "ap_stderr": 0.020946310829743606,
-        "evaluation_time": 3.16,
-        "f1": 0.6974335840131225,
-        "f1_stderr": 0.06862893318583979,
-        "main_score": 0.7574370709382152
-    },
-    "validation": {
-        "accuracy": 0.7654205607476635,
-        "accuracy_stderr": 0.08125468200059124,
-        "ap": 0.8786303620485129,
-        "ap_stderr": 0.017943015164604906,
-        "evaluation_time": 5.24,
-        "f1": 0.697347626855364,
-        "f1_stderr": 0.06520009834529593,
-        "main_score": 0.7654205607476635
+        "catalan": {
+            "accuracy": 0.43019999999999997,
+            "accuracy_stderr": 0.04952888046382634,
+            "f1": 0.4126601099708986,
+            "f1_stderr": 0.04601771378692479,
+            "main_score": 0.43019999999999997
+        },
+        "evaluation_time": 42.22,
+        "spanish": {
+            "accuracy": 0.42794999999999994,
+            "accuracy_stderr": 0.03462979208716101,
+            "f1": 0.42401316490609303,
+            "f1_stderr": 0.040485644702449405,
+            "main_score": 0.42794999999999994
+        }
     }
 }
```

### Comparing `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CzechSubjectivityClassification.json` & `mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CzechSubjectivityClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DanFEVER.json` & `mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DanFEVER.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DiaBlaBitextMining.json` & `mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DiaBlaBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/EstQA.json` & `mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/EstQA.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FQuADRetrieval.json` & `mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FQuADRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FilipinoHateSpeechClassification.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-small/CataloniaTweetClassification.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.40499999999999997%*

 * *Differences: {"'dataset_revision'": "'cf24d44e517efa534f048e5fc5981f399ed25bee'",*

 * * "'mteb_dataset_name'": "'CataloniaTweetClassification'",*

 * * "'mteb_version'": "'1.6.37'",*

 * * "'test'": "{'evaluation_time': 51.82, 'catalan': OrderedDict([('accuracy', 0.43600000000000005), "*

 * *           "('accuracy_stderr', 0.042004761634843256), ('f1', 0.4299942765198441), ('f1_stderr', "*

 * *           "0.04020665730650639), ('main_score', 0.43600000000000005)]), 'spanish': "*

 * *           "OrderedDict([('accuracy', 0.4932), ('accuracy_stderr', 0. […]*

```diff
@@ -1,25 +1,22 @@
 {
-    "dataset_revision": "1994e9bb7f3ec07518e3f0d9e870cb293e234686",
-    "mteb_dataset_name": "FilipinoHateSpeechClassification",
-    "mteb_version": "1.7.0",
+    "dataset_revision": "cf24d44e517efa534f048e5fc5981f399ed25bee",
+    "mteb_dataset_name": "CataloniaTweetClassification",
+    "mteb_version": "1.6.37",
     "test": {
-        "accuracy": 0.567236328125,
-        "accuracy_stderr": 0.03547762318671813,
-        "ap": 0.5091777339451248,
-        "ap_stderr": 0.022233974890613212,
-        "evaluation_time": 3.36,
-        "f1": 0.5601208748473766,
-        "f1_stderr": 0.039086309149307844,
-        "main_score": 0.567236328125
-    },
-    "validation": {
-        "accuracy": 0.560693359375,
-        "accuracy_stderr": 0.03873646284341647,
-        "ap": 0.48755526872683486,
-        "ap_stderr": 0.023538058050392732,
-        "evaluation_time": 4.12,
-        "f1": 0.553488267995188,
-        "f1_stderr": 0.044553263170545844,
-        "main_score": 0.560693359375
+        "catalan": {
+            "accuracy": 0.43600000000000005,
+            "accuracy_stderr": 0.042004761634843256,
+            "f1": 0.4299942765198441,
+            "f1_stderr": 0.04020665730650639,
+            "main_score": 0.43600000000000005
+        },
+        "evaluation_time": 51.82,
+        "spanish": {
+            "accuracy": 0.4932,
+            "accuracy_stderr": 0.021022844717116667,
+            "f1": 0.5019986248830843,
+            "f1_stderr": 0.025770061238838564,
+            "main_score": 0.4932
+        }
     }
 }
```

### Comparing `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FinParaSTS.json` & `mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FinParaSTS.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GerDaLIR.json` & `mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GerDaLIR.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GreekLegalCodeClassification.json` & `mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FilipinoHateSpeechClassification.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.575%*

 * *Differences: {"'dataset_revision'": "'1994e9bb7f3ec07518e3f0d9e870cb293e234686'",*

 * * "'mteb_dataset_name'": "'FilipinoHateSpeechClassification'",*

 * * "'mteb_version'": "'1.7.16'",*

 * * "'test'": "{'accuracy': 0.560986328125, 'accuracy_stderr': 0.0348712473938904, 'evaluation_time': "*

 * *           "24.91, 'f1': 0.5536573846297469, 'f1_stderr': 0.038059572332273875, 'main_score': "*

 * *           "0.560986328125, 'ap': 0.5039842907879104, 'ap_stderr': 0.02157794017691428}",*

 * * "'validation'": "{'accuracy': 0.565478515625, 'accuracy_stderr […]*

```diff
@@ -1,21 +1,25 @@
 {
-    "dataset_revision": "de0fdb34424f07d1ac6f0ede23ee0ed44bd9f5d1",
-    "mteb_dataset_name": "GreekLegalCodeClassification",
-    "mteb_version": "1.6.36",
+    "dataset_revision": "1994e9bb7f3ec07518e3f0d9e870cb293e234686",
+    "mteb_dataset_name": "FilipinoHateSpeechClassification",
+    "mteb_version": "1.7.16",
     "test": {
-        "accuracy": 0.290380859375,
-        "accuracy_stderr": 0.00819978191737022,
-        "evaluation_time": 88.71,
-        "f1": 0.23772795241695582,
-        "f1_stderr": 0.008730309299456626,
-        "main_score": 0.290380859375
+        "accuracy": 0.560986328125,
+        "accuracy_stderr": 0.0348712473938904,
+        "ap": 0.5039842907879104,
+        "ap_stderr": 0.02157794017691428,
+        "evaluation_time": 24.91,
+        "f1": 0.5536573846297469,
+        "f1_stderr": 0.038059572332273875,
+        "main_score": 0.560986328125
     },
     "validation": {
-        "accuracy": 0.303564453125,
-        "accuracy_stderr": 0.010601551885184904,
-        "evaluation_time": 89.06,
-        "f1": 0.23970657874134466,
-        "f1_stderr": 0.008710551186652492,
-        "main_score": 0.303564453125
+        "accuracy": 0.565478515625,
+        "accuracy_stderr": 0.03724049742672737,
+        "ap": 0.4988523504858809,
+        "ap_stderr": 0.023410641459661194,
+        "evaluation_time": 27.67,
+        "f1": 0.5582113131675175,
+        "f1_stderr": 0.04244987733223218,
+        "main_score": 0.565478515625
     }
 }
```

### Comparing `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GreekSentimentClassification.json` & `mteb-1.8.0/results/intfloat__multilingual-e5-small/UkrFormalityClassification.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.375%*

 * *Differences: {"'dataset_revision'": "'671d1e6bbf45a74ef21af351fd4ef7b32b7856f8'",*

 * * "'mteb_dataset_name'": "'UkrFormalityClassification'",*

 * * "'mteb_version'": "'1.6.37'",*

 * * "'test'": "{'accuracy': 0.531884765625, 'accuracy_stderr': 0.042682624460272475, 'ap': "*

 * *           "0.4519191811919496, 'ap_stderr': 0.023030098181090915, 'evaluation_time': 6.41, 'f1': "*

 * *           "0.5232694350569594, 'f1_stderr': 0.04149209518186783, 'main_score': 0.531884765625}",*

 * * "'train'": "OrderedDict([('accuracy', 0.53310546875), ('accuracy_st […]*

```diff
@@ -1,25 +1,25 @@
 {
-    "dataset_revision": "94b245f3ccdf8e8b2cbf8f13f55eee820b70eccf",
-    "mteb_dataset_name": "GreekSentimentClassification",
-    "mteb_version": "1.6.38",
+    "dataset_revision": "671d1e6bbf45a74ef21af351fd4ef7b32b7856f8",
+    "mteb_dataset_name": "UkrFormalityClassification",
+    "mteb_version": "1.6.37",
     "test": {
-        "accuracy": 0.7928292046936114,
-        "accuracy_stderr": 0.04926308383023319,
-        "ap": 0.7464210448969635,
-        "ap_stderr": 0.06379787177325662,
-        "evaluation_time": 22.93,
-        "f1": 0.786914648411039,
-        "f1_stderr": 0.049789628985373494,
-        "main_score": 0.7928292046936114
+        "accuracy": 0.531884765625,
+        "accuracy_stderr": 0.042682624460272475,
+        "ap": 0.4519191811919496,
+        "ap_stderr": 0.023030098181090915,
+        "evaluation_time": 6.41,
+        "f1": 0.5232694350569594,
+        "f1_stderr": 0.04149209518186783,
+        "main_score": 0.531884765625
     },
-    "validation": {
-        "accuracy": 0.7861618798955614,
-        "accuracy_stderr": 0.048894827362188927,
-        "ap": 0.7440403569139288,
-        "ap_stderr": 0.0620835985607011,
-        "evaluation_time": 16.98,
-        "f1": 0.7810197844405813,
-        "f1_stderr": 0.048885004677465003,
-        "main_score": 0.7861618798955614
+    "train": {
+        "accuracy": 0.53310546875,
+        "accuracy_stderr": 0.03355227727082908,
+        "ap": 0.5188855107501925,
+        "ap_stderr": 0.018712669478063233,
+        "evaluation_time": 11.28,
+        "f1": 0.5264433232444724,
+        "f1_stderr": 0.03228714969033335,
+        "main_score": 0.53310546875
     }
 }
```

### Comparing `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HunSum2AbstractiveRetrieval.json` & `mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HunSum2AbstractiveRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IN22ConvBitextMining.json` & `mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IN22ConvBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IN22GenBitextMining.json` & `mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IN22GenBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicSentimentClassification.json` & `mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JaQuADRetrieval.json` & `mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JaQuADRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBNarrativeQARetrieval.json` & `mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBNarrativeQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBNeedleRetrieval.json` & `mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBNeedleRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBPasskeyRetrieval.json` & `mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBPasskeyRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBQMSumRetrieval.json` & `mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBQMSumRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBSummScreenFDRetrieval.json` & `mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBSummScreenFDRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBWikimQARetrieval.json` & `mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBWikimQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MedicalQARetrieval.json` & `mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MedicalQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NeuCLIR2022Retrieval.json` & `mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NeuCLIR2022Retrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NeuCLIR2023Retrieval.json` & `mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NeuCLIR2023Retrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NorQuadRetrieval.json` & `mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NorQuadRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/OpusparcusPC.json` & `mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/OpusparcusPC.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PawsX.json` & `mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PawsX.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SNLRetrieval.json` & `mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SNLRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SweFaqRetrieval.json` & `mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SweFaqRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednRetrieval.json` & `mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TV2Nordretrieval.json` & `mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TV2Nordretrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TwitterHjerneRetrieval.json` & `mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TwitterHjerneRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieQuADRetrieval.json` & `mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieQuADRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WikiClusteringP2P.json` & `mteb-1.8.0/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WikiClusteringP2P.json`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/scripts/data/amazon_polarity/create_data.py` & `mteb-1.8.0/scripts/data/amazon_polarity/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/scripts/data/amazon_reviews_multi/create_data.py` & `mteb-1.8.0/scripts/data/amazon_reviews_multi/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/scripts/data/arxiv/script_clustering.py` & `mteb-1.8.0/scripts/data/arxiv/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/scripts/data/arxiv/script_raw.py` & `mteb-1.8.0/scripts/data/arxiv/script_raw.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/scripts/data/biorxiv/script_clustering.py` & `mteb-1.8.0/scripts/data/biorxiv/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/scripts/data/biorxiv/script_raw.py` & `mteb-1.8.0/scripts/data/biorxiv/script_raw.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/scripts/data/bucc/create_data.py` & `mteb-1.8.0/scripts/data/bucc/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/scripts/data/create_task_table.py` & `mteb-1.8.0/scripts/data/create_task_table.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/scripts/data/germanquad/process_data.py` & `mteb-1.8.0/scripts/data/germanquad/process_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/scripts/data/hal/create_data.py` & `mteb-1.8.0/scripts/data/hal/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/scripts/data/imdb/create_data.py` & `mteb-1.8.0/scripts/data/imdb/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/scripts/data/medicalqaretrieval/create_data.py` & `mteb-1.8.0/scripts/data/medicalqaretrieval/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/scripts/data/medrxiv/script_clustering.py` & `mteb-1.8.0/scripts/data/medrxiv/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/scripts/data/medrxiv/script_raw.py` & `mteb-1.8.0/scripts/data/medrxiv/script_raw.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/scripts/data/mind/prepare_data.py` & `mteb-1.8.0/scripts/data/mind/prepare_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/scripts/data/redditp2p/script_clustering.py` & `mteb-1.8.0/scripts/data/redditp2p/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/scripts/data/stackexchangep2p/script_clustering.py` & `mteb-1.8.0/scripts/data/stackexchangep2p/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/scripts/data/sts22-crosslingual-sts/create_data.py` & `mteb-1.8.0/scripts/data/sts22-crosslingual-sts/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/scripts/data/summeval_fr/create_data.py` & `mteb-1.8.0/scripts/data/summeval_fr/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/scripts/data/toxic_conversations_50k/create_data.py` & `mteb-1.8.0/scripts/data/toxic_conversations_50k/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/scripts/merge_cqadupstack.py` & `mteb-1.8.0/scripts/merge_cqadupstack.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/scripts/mteb_meta.py` & `mteb-1.8.0/scripts/mteb_meta.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/scripts/run_mteb_chinese.py` & `mteb-1.8.0/scripts/run_mteb_chinese.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/scripts/run_mteb_english.py` & `mteb-1.8.0/scripts/run_mteb_french.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,120 +1,69 @@
-"""Example script for benchmarking all datasets constituting the MTEB English leaderboard & average scores"""
+"""Example script for benchmarking all datasets constituting the MTEB French leaderboard & average scores"""
 
 from __future__ import annotations
 
 import logging
 
 from sentence_transformers import SentenceTransformer
 
 from mteb import MTEB
 
 logging.basicConfig(level=logging.INFO)
 
 logger = logging.getLogger("main")
 
 TASK_LIST_CLASSIFICATION = [
-    "AmazonCounterfactualClassification",
-    "AmazonPolarityClassification",
     "AmazonReviewsClassification",
-    "Banking77Classification",
-    "EmotionClassification",
-    "ImdbClassification",
+    "MasakhaNEWSClassification",
     "MassiveIntentClassification",
     "MassiveScenarioClassification",
     "MTOPDomainClassification",
     "MTOPIntentClassification",
-    "ToxicConversationsClassification",
-    "TweetSentimentExtractionClassification",
 ]
 
 TASK_LIST_CLUSTERING = [
-    "ArxivClusteringP2P",
-    "ArxivClusteringS2S",
-    "BiorxivClusteringP2P",
-    "BiorxivClusteringS2S",
-    "MedrxivClusteringP2P",
-    "MedrxivClusteringS2S",
-    "RedditClustering",
-    "RedditClusteringP2P",
-    "StackExchangeClustering",
-    "StackExchangeClusteringP2P",
-    "TwentyNewsgroupsClustering",
+    "AlloProfClusteringP2P",
+    "AlloProfClusteringS2S",
+    "HALClusteringS2S",
+    "MasakhaNEWSClusteringP2P",
+    "MasakhaNEWSClusteringS2S",
+    "MLSUMClusteringP2P",
+    "MLSUMClusteringS2S",
 ]
 
 TASK_LIST_PAIR_CLASSIFICATION = [
-    "SprintDuplicateQuestions",
-    "TwitterSemEval2015",
-    "TwitterURLCorpus",
+    "OpusparcusPC",
+    "PawsX",
 ]
 
-TASK_LIST_RERANKING = [
-    "AskUbuntuDupQuestions",
-    "MindSmallReranking",
-    "SciDocsRR",
-    "StackOverflowDupQuestions",
-]
+TASK_LIST_RERANKING = ["SyntecReranking", "AlloprofReranking"]
 
 TASK_LIST_RETRIEVAL = [
-    "ArguAna",
-    "ClimateFEVER",
-    "CQADupstackAndroidRetrieval",
-    "CQADupstackEnglishRetrieval",
-    "CQADupstackGamingRetrieval",
-    "CQADupstackGisRetrieval",
-    "CQADupstackMathematicaRetrieval",
-    "CQADupstackPhysicsRetrieval",
-    "CQADupstackProgrammersRetrieval",
-    "CQADupstackStatsRetrieval",
-    "CQADupstackTexRetrieval",
-    "CQADupstackUnixRetrieval",
-    "CQADupstackWebmastersRetrieval",
-    "CQADupstackWordpressRetrieval",
-    "DBPedia",
-    "FEVER",
-    "FiQA2018",
-    "HotpotQA",
-    "MSMARCO",
-    "NFCorpus",
-    "NQ",
-    "QuoraRetrieval",
-    "SCIDOCS",
-    "SciFact",
-    "Touche2020",
-    "TRECCOVID",
+    "AlloprofRetrieval",
+    "BSARDRetrieval",
+    "SyntecRetrieval",
+    "XPQARetrieval",
+    "MintakaRetrieval",
 ]
 
-TASK_LIST_STS = [
-    "BIOSSES",
-    "SICK-R",
-    "STS12",
-    "STS13",
-    "STS14",
-    "STS15",
-    "STS16",
-    "STS17",
-    "STS22",
-    "STSBenchmark",
-    "SummEval",
-]
+TASK_LIST_STS = ["SummEvalFr", "STSBenchmarkMultilingualSTS", "STS22", "SICKFr"]
 
 TASK_LIST = (
     TASK_LIST_CLASSIFICATION
     + TASK_LIST_CLUSTERING
     + TASK_LIST_PAIR_CLASSIFICATION
     + TASK_LIST_RERANKING
     + TASK_LIST_RETRIEVAL
     + TASK_LIST_STS
 )
 
-model_name = "average_word_embeddings_komninos"
+model_name = "dangvantuan/sentence-camembert-base"
 model = SentenceTransformer(model_name)
 
+logger.info(f"Task list : {TASK_LIST}")
 for task in TASK_LIST:
     logger.info(f"Running task: {task}")
-    eval_splits = ["dev"] if task == "MSMARCO" else ["test"]
     evaluation = MTEB(
-        tasks=[task], task_langs=["en"]
-    )  # Remove "en" for running all languages
-    evaluation.run(
-        model, output_folder=f"results/{model_name}", eval_splits=eval_splits
-    )
+        tasks=[task], task_langs=["fr"]
+    )  # Remove "fr" for running all languages
+    evaluation.run(model, output_folder=f"results/{model_name}")
```

### Comparing `mteb-1.7.9/scripts/run_mteb_french.py` & `mteb-1.8.0/scripts/run_mteb_german.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,69 +1,55 @@
-"""Example script for benchmarking all datasets constituting the MTEB French leaderboard & average scores"""
+"""Example script for benchmarking German Context models."""
 
 from __future__ import annotations
 
 import logging
 
 from sentence_transformers import SentenceTransformer
 
 from mteb import MTEB
 
 logging.basicConfig(level=logging.INFO)
-
 logger = logging.getLogger("main")
 
 TASK_LIST_CLASSIFICATION = [
+    "AmazonCounterfactualClassification",
     "AmazonReviewsClassification",
-    "MasakhaNEWSClassification",
-    "MassiveIntentClassification",
-    "MassiveScenarioClassification",
     "MTOPDomainClassification",
     "MTOPIntentClassification",
+    "MassiveIntentClassification",
+    "MassiveScenarioClassification",
 ]
 
 TASK_LIST_CLUSTERING = [
-    "AlloProfClusteringP2P",
-    "AlloProfClusteringS2S",
-    "HALClusteringS2S",
-    "MasakhaNEWSClusteringP2P",
-    "MasakhaNEWSClusteringS2S",
-    "MLSUMClusteringP2P",
-    "MLSUMClusteringS2S",
+    "BlurbsClusteringP2P",
+    "BlurbsClusteringS2S",
+    "TenKGnadClusteringP2P",
+    "TenKGnadClusteringS2S",
 ]
 
-TASK_LIST_PAIR_CLASSIFICATION = [
-    "OpusparcusPC",
-    "PawsX",
-]
+TASK_LIST_PAIR_CLASSIFICATION = ["FalseFriendsGermanEnglish", "PawsX"]
 
-TASK_LIST_RERANKING = ["SyntecReranking", "AlloprofReranking"]
+TASK_LIST_RERANKING = ["MIRACL"]
 
-TASK_LIST_RETRIEVAL = [
-    "AlloprofRetrieval",
-    "BSARDRetrieval",
-    "SyntecRetrieval",
-    "XPQARetrieval",
-    "MintakaRetrieval",
-]
+TASK_LIST_RETRIEVAL = ["GermanQuAD-Retrieval", "GermanDPR", "XMarketDE", "GerDaLIR"]
 
-TASK_LIST_STS = ["SummEvalFr", "STSBenchmarkMultilingualSTS", "STS22", "SICKFr"]
+TASK_LIST_STS = ["GermanSTSBenchmark", "STS22"]
 
 TASK_LIST = (
     TASK_LIST_CLASSIFICATION
     + TASK_LIST_CLUSTERING
     + TASK_LIST_PAIR_CLASSIFICATION
     + TASK_LIST_RERANKING
     + TASK_LIST_RETRIEVAL
     + TASK_LIST_STS
 )
 
-model_name = "dangvantuan/sentence-camembert-base"
+model_name = "intfloat/multilingual-e5-small"
 model = SentenceTransformer(model_name)
 
-logger.info(f"Task list : {TASK_LIST}")
-for task in TASK_LIST:
-    logger.info(f"Running task: {task}")
-    evaluation = MTEB(
-        tasks=[task], task_langs=["fr"]
-    )  # Remove "fr" for running all languages
-    evaluation.run(model, output_folder=f"results/{model_name}")
+evaluation = MTEB(tasks=TASK_LIST, task_langs=["de"])
+evaluation.run(
+    model,
+    overwrite_results=True,
+    output_folder=f"results/de/{model_name.split('/')[-1]}",
+)
```

### Comparing `mteb-1.7.9/scripts/run_mteb_korean.py` & `mteb-1.8.0/scripts/run_mteb_korean.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from mteb import MTEB
 
 logging.basicConfig(level=logging.INFO)
 
 logger = logging.getLogger("main")
 
-TASK_LIST_CLASSIFICATION = []
+TASK_LIST_CLASSIFICATION = ["KLUE-TC"]
 
 TASK_LIST_CLUSTERING = []
 
 TASK_LIST_PAIR_CLASSIFICATION = []
 
 TASK_LIST_RERANKING = []
```

### Comparing `mteb-1.7.9/scripts/run_mteb_law.py` & `mteb-1.8.0/scripts/run_mteb_law.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/scripts/run_mteb_polish.py` & `mteb-1.8.0/scripts/run_mteb_polish.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-"""Example script for benchmarking all datasets constituting the MTEB Polish leaderboard & average scores"""
+"""Example script for benchmarking all datasets constituting the MTEB Polish leaderboard & average scores.
+For a more elaborate evaluation, we refer to https://github.com/rafalposwiata/pl-mteb.
+"""
 
 from __future__ import annotations
 
 import logging
 
 from sentence_transformers import SentenceTransformer
 
@@ -17,19 +19,19 @@
     "PolEmo2.0-OUT",
     "AllegroReviews",
     "PAC",
     "MassiveIntentClassification",
     "MassiveScenarioClassification",
 ]
 
-clustering_tasks = ["8TagsClustering"]
+clustering_tasks = ["EightTagsClustering", "PlscClusteringS2S", "PlscClusteringP2P"]
 
 pair_classification_tasks = ["SICK-E-PL", "PPC", "CDSC-E", "PSC"]
 
-sts_tasks = ["SICK-R-PL", "CDSC-R", "STS22"]
+sts_tasks = ["SICK-R-PL", "CDSC-R", "STS22", "STSBenchmarkMultilingualSTS"]
 
 tasks = classification_tasks + clustering_tasks + pair_classification_tasks + sts_tasks
 
 model_name = "sdadas/st-polish-paraphrase-from-distilroberta"
 model = SentenceTransformer(model_name)
 
 evaluation = MTEB(tasks=tasks, task_langs=["pl"])
```

### Comparing `mteb-1.7.9/tests/test_ClusteringEvaluator.py` & `mteb-1.8.0/tests/test_ClusteringEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/tests/test_InstructionRetrievalEvaluator.py` & `mteb-1.8.0/tests/test_InstructionRetrievalEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/tests/test_PairClassificationEvaluator.py` & `mteb-1.8.0/tests/test_PairClassificationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/tests/test_RerankingEvaluator.py` & `mteb-1.8.0/tests/test_RerankingEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/tests/test_RetrievalEvaluator.py` & `mteb-1.8.0/tests/test_RetrievalEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.7.9/tests/test_all_abstasks.py` & `mteb-1.8.0/tests/test_all_abstasks.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,24 +7,30 @@
 import aiohttp
 import pytest
 
 from mteb import MTEB
 from mteb.abstasks import AbsTask
 from mteb.abstasks.AbsTaskInstructionRetrieval import AbsTaskInstructionRetrieval
 from mteb.abstasks.AbsTaskRetrieval import AbsTaskRetrieval
+from mteb.abstasks.MultiSubsetLoader import MultiSubsetLoader
 
 logging.basicConfig(level=logging.INFO)
 
 
 @pytest.mark.parametrize("task", MTEB().tasks_cls)
 @patch("datasets.load_dataset")
-def test_load_data(mock_load_dataset: Mock, task: AbsTask):
+@patch("datasets.concatenate_datasets")
+def test_load_data(
+    mock_concatenate_datasets: Mock, mock_load_dataset: Mock, task: AbsTask
+):
     # TODO: We skip because this load_data is completely different.
-    if isinstance(task, AbsTaskRetrieval) or isinstance(
-        task, AbsTaskInstructionRetrieval
+    if (
+        isinstance(task, AbsTaskRetrieval)
+        or isinstance(task, AbsTaskInstructionRetrieval)
+        or isinstance(task, MultiSubsetLoader)
     ):
         pytest.skip()
     with patch.object(task, "dataset_transform") as mock_dataset_transform:
         task.load_data()
         mock_load_dataset.assert_called()
 
         # They don't yet but should they so they can be expanded more easily?
```

### Comparing `mteb-1.7.9/tests/test_mteb.py` & `mteb-1.8.0/tests/test_mteb.py`

 * *Files identical despite different names*

