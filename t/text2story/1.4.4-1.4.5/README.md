# Comparing `tmp/text2story-1.4.4.tar.gz` & `tmp/text2story-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2story-1.4.4.tar", last modified: Wed Nov 22 10:01:09 2023, max compression
+gzip compressed data, was "text2story-1.4.5.tar", last modified: Mon May  6 10:05:49 2024, max compression
```

## Comparing `text2story-1.4.4.tar` & `text2story-1.4.5.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-11-22 10:01:09.544894 text2story-1.4.4/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    33470 2022-10-19 09:22:59.000000 text2story-1.4.4/LICENSE
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      559 2023-09-20 11:40:02.000000 text2story-1.4.4/MANIFEST.in
--rw-r--r--   0 evelinamorim  (1000) evelinamorim  (1000)    11572 2023-11-22 10:01:09.544894 text2story-1.4.4/PKG-INFO
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    10931 2023-11-22 09:50:23.000000 text2story-1.4.4/README.md
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      347 2023-11-08 10:34:23.000000 text2story-1.4.4/pyproject.toml
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      667 2023-11-22 10:01:09.544894 text2story-1.4.4/setup.cfg
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2023-09-11 13:50:06.000000 text2story-1.4.4/setup.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-11-22 10:01:09.528895 text2story-1.4.4/text2story/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      757 2022-10-19 09:12:42.000000 text2story-1.4.4/text2story/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       67 2022-10-19 09:12:42.000000 text2story-1.4.4/text2story/__main__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-11-22 10:01:09.528895 text2story-1.4.4/text2story/annotators/
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-11-22 10:01:09.528895 text2story-1.4.4/text2story/annotators/ALLENNLP/
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-11-22 10:01:09.524895 text2story-1.4.4/text2story/annotators/ALLENNLP/Models/
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-11-22 10:01:09.528895 text2story-1.4.4/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-11-22 10:01:09.528895 text2story-1.4.4/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      739 2022-10-13 08:54:40.000000 text2story-1.4.4/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/labels.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       14 2022-10-13 08:54:40.000000 text2story-1.4.4/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/non_padded_namespaces.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1343 2022-10-13 08:54:40.000000 text2story-1.4.4/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/config.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   265058 2022-10-13 08:54:40.000000 text2story-1.4.4/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/linear_layer.pt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    10386 2022-10-13 08:54:40.000000 text2story-1.4.4/text2story/annotators/ALLENNLP/PropBankBr.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6172 2023-11-08 10:19:59.000000 text2story-1.4.4/text2story/annotators/ALLENNLP/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    28375 2023-11-08 10:15:57.000000 text2story-1.4.4/text2story/annotators/ALLENNLP/allen_wrapper.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13691 2022-10-13 08:54:40.000000 text2story-1.4.4/text2story/annotators/ALLENNLP/my_model.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    20528 2023-09-20 15:37:16.000000 text2story-1.4.4/text2story/annotators/ALLENNLP/my_reader.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6217 2022-10-13 08:54:40.000000 text2story-1.4.4/text2story/annotators/ALLENNLP/preprocess.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9773 2023-09-18 13:41:19.000000 text2story-1.4.4/text2story/annotators/ALLENNLP/requirements.txt
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-11-22 10:01:09.532895 text2story-1.4.4/text2story/annotators/BERTNERPT/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)  2143882 2023-09-12 15:18:59.000000 text2story-1.4.4/text2story/annotators/BERTNERPT/POS_tagger_brill.pkl
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3160 2023-09-19 14:37:58.000000 text2story-1.4.4/text2story/annotators/BERTNERPT/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-11-22 10:01:09.532895 text2story-1.4.4/text2story/annotators/CUSTOMPT/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14794 2022-10-13 08:54:40.000000 text2story-1.4.4/text2story/annotators/CUSTOMPT/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   371646 2022-10-13 08:54:40.000000 text2story-1.4.4/text2story/annotators/CUSTOMPT/crf_v2.1.joblib
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    15093 2022-10-13 08:54:40.000000 text2story-1.4.4/text2story/annotators/CUSTOMPT/event_model.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13972 2022-10-13 08:54:40.000000 text2story-1.4.4/text2story/annotators/CUSTOMPT/feature_extractor.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-11-22 10:01:09.532895 text2story-1.4.4/text2story/annotators/NLTK/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2954 2023-09-13 10:57:45.000000 text2story-1.4.4/text2story/annotators/NLTK/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-11-22 10:01:09.536894 text2story-1.4.4/text2story/annotators/PY_HEIDELTIME/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1786 2023-10-11 13:29:55.000000 text2story-1.4.4/text2story/annotators/PY_HEIDELTIME/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-11-22 10:01:09.536894 text2story-1.4.4/text2story/annotators/SPACY/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1901 2023-09-21 09:23:20.000000 text2story-1.4.4/text2story/annotators/SPACY/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-11-22 10:01:09.536894 text2story-1.4.4/text2story/annotators/SPARKNLP/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9462 2022-10-26 12:28:21.000000 text2story-1.4.4/text2story/annotators/SPARKNLP/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-11-22 10:01:09.536894 text2story-1.4.4/text2story/annotators/SRLWeakLabeling/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3501 2023-09-11 13:50:06.000000 text2story-1.4.4/text2story/annotators/SRLWeakLabeling/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-11-22 10:01:09.536894 text2story-1.4.4/text2story/annotators/TEI2GO/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1623 2023-09-21 09:11:18.000000 text2story-1.4.4/text2story/annotators/TEI2GO/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     4557 2023-10-09 15:52:56.000000 text2story-1.4.4/text2story/annotators/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-11-22 10:01:09.536894 text2story-1.4.4/text2story/brat2viz/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      548 2022-10-19 09:12:42.000000 text2story-1.4.4/text2story/brat2viz/README.md
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2022-10-19 09:12:42.000000 text2story-1.4.4/text2story/brat2viz/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-11-22 10:01:09.536894 text2story-1.4.4/text2story/brat2viz/brat2drs/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       37 2022-10-19 09:12:42.000000 text2story-1.4.4/text2story/brat2viz/brat2drs/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    17359 2023-09-11 13:50:06.000000 text2story-1.4.4/text2story/brat2viz/brat2drs/brat2drs.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1059 2022-10-19 09:12:42.000000 text2story-1.4.4/text2story/brat2viz/brat2drs/files_monitor.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-11-22 10:01:09.536894 text2story-1.4.4/text2story/brat2viz/brat2json/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-10-24 13:54:25.000000 text2story-1.4.4/text2story/brat2viz/brat2json/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    45447 2023-10-24 14:47:12.000000 text2story-1.4.4/text2story/brat2viz/brat2json/brat2json.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-11-22 10:01:09.536894 text2story-1.4.4/text2story/brat2viz/drs2viz/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2022-10-19 09:12:42.000000 text2story-1.4.4/text2story/brat2viz/drs2viz/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2428 2022-10-19 09:12:42.000000 text2story-1.4.4/text2story/brat2viz/drs2viz/app.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13487 2022-10-19 09:12:42.000000 text2story-1.4.4/text2story/brat2viz/drs2viz/parser.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    10956 2023-09-13 14:10:19.000000 text2story-1.4.4/text2story/brat2viz/drs2viz/viz.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-11-22 10:01:09.540894 text2story-1.4.4/text2story/core/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-19 13:19:29.000000 text2story-1.4.4/text2story/core/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    12228 2023-09-19 12:37:09.000000 text2story-1.4.4/text2story/core/annotator.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3429 2023-10-09 14:49:24.000000 text2story-1.4.4/text2story/core/entity_structures.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1257 2023-09-12 15:18:59.000000 text2story-1.4.4/text2story/core/exceptions.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      546 2023-09-11 13:50:06.000000 text2story-1.4.4/text2story/core/graph_builder.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3343 2023-09-11 13:50:06.000000 text2story-1.4.4/text2story/core/link_structures.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    28477 2023-10-18 11:54:50.000000 text2story-1.4.4/text2story/core/narrative.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    11397 2023-10-06 10:45:23.000000 text2story-1.4.4/text2story/core/utils.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-11-22 10:01:09.540894 text2story-1.4.4/text2story/experiments/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-09-11 13:50:06.000000 text2story-1.4.4/text2story/experiments/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3918 2023-09-11 13:50:06.000000 text2story-1.4.4/text2story/experiments/compare_ann.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3713 2023-10-16 09:18:06.000000 text2story-1.4.4/text2story/experiments/cp_notlusa.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      882 2023-10-19 23:18:46.000000 text2story-1.4.4/text2story/experiments/evaluate_gpt.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    16957 2023-10-13 11:47:45.000000 text2story-1.4.4/text2story/experiments/evaluation.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      429 2022-10-13 08:54:40.000000 text2story-1.4.4/text2story/experiments/exp.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      205 2022-10-13 08:54:40.000000 text2story-1.4.4/text2story/experiments/exp_en_fn.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      601 2022-10-13 08:54:40.000000 text2story-1.4.4/text2story/experiments/exp_en_pb.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14456 2023-09-11 13:50:06.000000 text2story-1.4.4/text2story/experiments/metrics.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1453 2023-10-16 10:27:43.000000 text2story-1.4.4/text2story/experiments/run_experiments.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6423 2023-11-17 15:45:46.000000 text2story-1.4.4/text2story/experiments/stats.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-11-22 10:01:09.540894 text2story-1.4.4/text2story/readers/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-09-11 13:50:06.000000 text2story-1.4.4/text2story/readers/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      380 2022-10-13 08:54:40.000000 text2story-1.4.4/text2story/readers/fn-lirics.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   312656 2022-10-13 08:54:40.000000 text2story-1.4.4/text2story/readers/pb-vn2.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      547 2022-10-13 08:54:40.000000 text2story-1.4.4/text2story/readers/read.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14407 2023-10-18 07:53:38.000000 text2story-1.4.4/text2story/readers/read_ace.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    25543 2023-10-19 13:22:28.000000 text2story-1.4.4/text2story/readers/read_brat.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    17011 2023-10-06 10:45:23.000000 text2story-1.4.4/text2story/readers/read_ecb.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6081 2022-10-13 08:54:40.000000 text2story-1.4.4/text2story/readers/read_framenet.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    11525 2022-10-13 08:54:40.000000 text2story-1.4.4/text2story/readers/read_propbank.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1180 2023-03-27 13:07:12.000000 text2story-1.4.4/text2story/readers/token_corpus.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1221 2022-10-13 08:54:40.000000 text2story-1.4.4/text2story/readers/utils.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      353 2022-10-13 08:54:40.000000 text2story-1.4.4/text2story/readers/vn-lirics.json
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-11-22 10:01:09.540894 text2story-1.4.4/text2story/select/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      121 2023-03-27 13:07:12.000000 text2story-1.4.4/text2story/select/README.md
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-09-11 13:50:06.000000 text2story-1.4.4/text2story/select/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14728 2023-03-27 13:07:12.000000 text2story-1.4.4/text2story/select/bubble.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     5958 2023-11-21 15:17:41.000000 text2story-1.4.4/text2story/select/event.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1341 2023-11-21 16:20:00.000000 text2story-1.4.4/text2story/select/links.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-11-22 10:01:09.540894 text2story-1.4.4/text2story/text2viz/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     5371 2022-10-13 08:54:40.000000 text2story-1.4.4/text2story/text2viz/Text2Viz.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2022-10-13 08:54:40.000000 text2story-1.4.4/text2story/text2viz/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      699 2022-10-13 08:54:40.000000 text2story-1.4.4/text2story/text2viz/visualization.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-11-22 10:01:09.540894 text2story-1.4.4/text2story/training/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-09-11 13:50:06.000000 text2story-1.4.4/text2story/training/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14422 2023-09-11 13:50:06.000000 text2story-1.4.4/text2story/training/participant_concept.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-11-22 10:01:09.544894 text2story-1.4.4/text2story/viz/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-09-11 13:50:06.000000 text2story-1.4.4/text2story/viz/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    15162 2023-09-11 13:50:06.000000 text2story-1.4.4/text2story/viz/bubble_tikz.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-11-22 10:01:09.544894 text2story-1.4.4/text2story.egg-info/
--rw-r--r--   0 evelinamorim  (1000) evelinamorim  (1000)    11572 2023-11-22 10:01:09.000000 text2story-1.4.4/text2story.egg-info/PKG-INFO
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3360 2023-11-22 10:01:09.000000 text2story-1.4.4/text2story.egg-info/SOURCES.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-11-22 10:01:09.000000 text2story-1.4.4/text2story.egg-info/dependency_links.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      224 2023-11-22 10:01:09.000000 text2story-1.4.4/text2story.egg-info/requires.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       11 2023-11-22 10:01:09.000000 text2story-1.4.4/text2story.egg-info/top_level.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-05-26 15:56:54.000000 text2story-1.4.4/text2story.egg-info/zip-safe
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.613779 text2story-1.4.5/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    33470 2022-10-19 09:22:59.000000 text2story-1.4.5/LICENSE
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      559 2023-09-20 11:40:02.000000 text2story-1.4.5/MANIFEST.in
+-rw-r--r--   0 evelinamorim  (1000) evelinamorim  (1000)    10904 2024-05-06 10:05:49.613779 text2story-1.4.5/PKG-INFO
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    10263 2023-12-13 15:05:29.000000 text2story-1.4.5/README.md
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      417 2024-05-06 10:00:42.000000 text2story-1.4.5/pyproject.toml
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      601 2024-05-06 10:05:49.617780 text2story-1.4.5/setup.cfg
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2023-09-11 13:50:06.000000 text2story-1.4.5/setup.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.577779 text2story-1.4.5/text2story/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      757 2022-10-19 09:12:42.000000 text2story-1.4.5/text2story/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       67 2022-10-19 09:12:42.000000 text2story-1.4.5/text2story/__main__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.577779 text2story-1.4.5/text2story/annotators/
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.581780 text2story-1.4.5/text2story/annotators/ALLENNLP/
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.573779 text2story-1.4.5/text2story/annotators/ALLENNLP/Models/
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.581780 text2story-1.4.5/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.585780 text2story-1.4.5/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      739 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/labels.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       14 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/non_padded_namespaces.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1343 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/config.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   265058 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/linear_layer.pt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    10386 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/annotators/ALLENNLP/PropBankBr.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6172 2023-11-08 10:19:59.000000 text2story-1.4.5/text2story/annotators/ALLENNLP/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    28375 2023-11-08 10:15:57.000000 text2story-1.4.5/text2story/annotators/ALLENNLP/allen_wrapper.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13691 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/annotators/ALLENNLP/my_model.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    20528 2023-09-20 15:37:16.000000 text2story-1.4.5/text2story/annotators/ALLENNLP/my_reader.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6217 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/annotators/ALLENNLP/preprocess.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9718 2024-05-02 10:55:09.000000 text2story-1.4.5/text2story/annotators/ALLENNLP/requirements.txt
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.589779 text2story-1.4.5/text2story/annotators/BERTNERPT/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)  2143882 2023-09-12 15:18:59.000000 text2story-1.4.5/text2story/annotators/BERTNERPT/POS_tagger_brill.pkl
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3160 2023-09-19 14:37:58.000000 text2story-1.4.5/text2story/annotators/BERTNERPT/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.593779 text2story-1.4.5/text2story/annotators/CUSTOMPT/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14794 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/annotators/CUSTOMPT/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   371646 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/annotators/CUSTOMPT/crf_v2.1.joblib
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    15093 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/annotators/CUSTOMPT/event_model.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13972 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/annotators/CUSTOMPT/feature_extractor.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.593779 text2story-1.4.5/text2story/annotators/NLTK/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2954 2023-09-13 10:57:45.000000 text2story-1.4.5/text2story/annotators/NLTK/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.593779 text2story-1.4.5/text2story/annotators/PY_HEIDELTIME/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1786 2023-10-11 13:29:55.000000 text2story-1.4.5/text2story/annotators/PY_HEIDELTIME/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.593779 text2story-1.4.5/text2story/annotators/SPACY/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1901 2023-09-21 09:23:20.000000 text2story-1.4.5/text2story/annotators/SPACY/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.593779 text2story-1.4.5/text2story/annotators/SPARKNLP/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9462 2022-10-26 12:28:21.000000 text2story-1.4.5/text2story/annotators/SPARKNLP/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.597780 text2story-1.4.5/text2story/annotators/SRLWeakLabeling/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3501 2023-09-11 13:50:06.000000 text2story-1.4.5/text2story/annotators/SRLWeakLabeling/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.597780 text2story-1.4.5/text2story/annotators/TEI2GO/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1623 2023-09-21 09:11:18.000000 text2story-1.4.5/text2story/annotators/TEI2GO/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     4557 2024-05-06 09:48:38.000000 text2story-1.4.5/text2story/annotators/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.597780 text2story-1.4.5/text2story/brat2viz/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      548 2022-10-19 09:12:42.000000 text2story-1.4.5/text2story/brat2viz/README.md
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2022-10-19 09:12:42.000000 text2story-1.4.5/text2story/brat2viz/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.597780 text2story-1.4.5/text2story/brat2viz/brat2drs/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       37 2022-10-19 09:12:42.000000 text2story-1.4.5/text2story/brat2viz/brat2drs/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    17359 2023-09-11 13:50:06.000000 text2story-1.4.5/text2story/brat2viz/brat2drs/brat2drs.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1059 2022-10-19 09:12:42.000000 text2story-1.4.5/text2story/brat2viz/brat2drs/files_monitor.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.597780 text2story-1.4.5/text2story/brat2viz/brat2json/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-10-24 13:54:25.000000 text2story-1.4.5/text2story/brat2viz/brat2json/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    45447 2023-10-24 14:47:12.000000 text2story-1.4.5/text2story/brat2viz/brat2json/brat2json.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.601780 text2story-1.4.5/text2story/brat2viz/drs2viz/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2022-10-19 09:12:42.000000 text2story-1.4.5/text2story/brat2viz/drs2viz/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2428 2022-10-19 09:12:42.000000 text2story-1.4.5/text2story/brat2viz/drs2viz/app.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13487 2022-10-19 09:12:42.000000 text2story-1.4.5/text2story/brat2viz/drs2viz/parser.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    10956 2023-09-13 14:10:19.000000 text2story-1.4.5/text2story/brat2viz/drs2viz/viz.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.601780 text2story-1.4.5/text2story/core/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-19 13:19:29.000000 text2story-1.4.5/text2story/core/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    12228 2024-05-02 10:54:43.000000 text2story-1.4.5/text2story/core/annotator.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3429 2023-10-09 14:49:24.000000 text2story-1.4.5/text2story/core/entity_structures.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1257 2024-05-02 10:54:43.000000 text2story-1.4.5/text2story/core/exceptions.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      546 2023-09-11 13:50:06.000000 text2story-1.4.5/text2story/core/graph_builder.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3343 2023-09-11 13:50:06.000000 text2story-1.4.5/text2story/core/link_structures.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    28477 2024-05-02 10:54:43.000000 text2story-1.4.5/text2story/core/narrative.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    11397 2023-10-06 10:45:23.000000 text2story-1.4.5/text2story/core/utils.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.605780 text2story-1.4.5/text2story/experiments/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-09-11 13:50:06.000000 text2story-1.4.5/text2story/experiments/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3918 2023-09-11 13:50:06.000000 text2story-1.4.5/text2story/experiments/compare_ann.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3713 2023-10-16 09:18:06.000000 text2story-1.4.5/text2story/experiments/cp_notlusa.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      882 2023-10-19 23:18:46.000000 text2story-1.4.5/text2story/experiments/evaluate_gpt.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    16957 2024-01-31 16:04:58.000000 text2story-1.4.5/text2story/experiments/evaluation.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      429 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/experiments/exp.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      205 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/experiments/exp_en_fn.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      601 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/experiments/exp_en_pb.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14493 2024-05-02 10:54:43.000000 text2story-1.4.5/text2story/experiments/metrics.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1453 2024-01-31 16:03:53.000000 text2story-1.4.5/text2story/experiments/run_experiments.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     8912 2024-01-16 16:40:49.000000 text2story-1.4.5/text2story/experiments/stats.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.609779 text2story-1.4.5/text2story/readers/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-09-11 13:50:06.000000 text2story-1.4.5/text2story/readers/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      380 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/readers/fn-lirics.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   312656 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/readers/pb-vn2.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      547 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/readers/read.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14407 2023-10-18 07:53:38.000000 text2story-1.4.5/text2story/readers/read_ace.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    26882 2024-05-02 10:54:43.000000 text2story-1.4.5/text2story/readers/read_brat.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    17011 2023-10-06 10:45:23.000000 text2story-1.4.5/text2story/readers/read_ecb.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6081 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/readers/read_framenet.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    11525 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/readers/read_propbank.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1639 2024-01-09 13:08:04.000000 text2story-1.4.5/text2story/readers/token_corpus.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1221 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/readers/utils.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      353 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/readers/vn-lirics.json
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.613779 text2story-1.4.5/text2story/select/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      121 2023-03-27 13:07:12.000000 text2story-1.4.5/text2story/select/README.md
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-09-11 13:50:06.000000 text2story-1.4.5/text2story/select/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    15112 2024-01-18 13:01:37.000000 text2story-1.4.5/text2story/select/bubble.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    10207 2024-01-23 10:09:52.000000 text2story-1.4.5/text2story/select/event.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.613779 text2story-1.4.5/text2story/text2viz/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     5371 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/text2viz/Text2Viz.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/text2viz/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      699 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/text2viz/visualization.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.613779 text2story-1.4.5/text2story/training/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-09-11 13:50:06.000000 text2story-1.4.5/text2story/training/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14422 2023-09-11 13:50:06.000000 text2story-1.4.5/text2story/training/participant_concept.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.613779 text2story-1.4.5/text2story/viz/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-09-11 13:50:06.000000 text2story-1.4.5/text2story/viz/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    15649 2024-01-18 11:52:24.000000 text2story-1.4.5/text2story/viz/bubble_tikz.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2710 2024-01-19 15:14:06.000000 text2story-1.4.5/text2story/viz/msc.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.613779 text2story-1.4.5/text2story.egg-info/
+-rw-r--r--   0 evelinamorim  (1000) evelinamorim  (1000)    10904 2024-05-06 10:05:49.000000 text2story-1.4.5/text2story.egg-info/PKG-INFO
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3355 2024-05-06 10:05:49.000000 text2story-1.4.5/text2story.egg-info/SOURCES.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2024-05-06 10:05:49.000000 text2story-1.4.5/text2story.egg-info/dependency_links.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      224 2024-05-06 10:05:49.000000 text2story-1.4.5/text2story.egg-info/requires.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       11 2024-05-06 10:05:49.000000 text2story-1.4.5/text2story.egg-info/top_level.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-05-26 15:56:54.000000 text2story-1.4.5/text2story.egg-info/zip-safe
```

### Comparing `text2story-1.4.4/LICENSE` & `text2story-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/MANIFEST.in` & `text2story-1.4.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/PKG-INFO` & `text2story-1.4.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,22 @@
-Metadata-Version: 2.1
-Name: text2story
-Version: 1.4.4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: joblib
-Requires-Dist: spacy
-Requires-Dist: py-heideltime
-Requires-Dist: importlib_metadata
-Requires-Dist: pandas<2.0.0
-Requires-Dist: plantuml
-Requires-Dist: matplotlib
-Requires-Dist: networkx
-Requires-Dist: netgraph
-Requires-Dist: pytorch-crf
-Requires-Dist: transformers
-Requires-Dist: torch
-Requires-Dist: pdf2image
-Requires-Dist: latexcompiler
-Requires-Dist: nltk
-Requires-Dist: thinc
-Requires-Dist: beautifulsoup4
-Requires-Dist: streamlit==1.3.1
-Requires-Dist: altair==4.2.2
-Requires-Dist: protobuf==3.20
-
 # Text2Story main package
 The Text2Story main package contains the main classes and methods for the T2S pipeline: from text to formal representation to visualization or other representation.
 
 - **Relation to Brat2Viz**
-The Text2Story package is a generalization of Brat2Viz and should in fact contain all the functionalities and variants of the T2S project output.
+The Text2Story package is a generalization of Brat2Viz and should in fact contain all the funcionalities and variants of the T2S project output.
 
 ## Table of Contents
 
 1. [ Getting Start. ](#start)
 2. [ The Framework Structure. ](#structure)
 3. [ The Annotators. ](#annotators)
 4. [ Installation. ](#installation)
    - 4.1\. [ Linux Ubuntu ](#installationlinux)
    - 4.2\. [ Windows ](#installationwindows)
-
+5. [ The Web App. ](#webapp)
 
 <a name="start"></a>
 ## 1. Getting Started
 
 The main goal of the text2story is to extract narrative from raw text. The narrative 
 components comprise events, the participants (or participants) in the events, and the time expressions. 
 
@@ -181,33 +155,22 @@
 The installation requires graphviz software, the latex suite and the software poppler to convert pdf to png. 
 In Linux, to install these software open a terminal and type the following commands:
 
 ```
 sudo apt-get install graphviz libgraphviz-dev texlive-latex-base  texlive-latex-extra poppler-utils
 ```
 
-You will need a virtual environment as well. If you do not have venv, you can install it in linux by using the 
-apt-get command or pip command. Next, we demonstrate these two ways of install it.
-
-```
-sudo apt-get install python3-venv
-```
-
-```
-python3 -m pip install virtualenv
-```
-
-After that, you will be able to create a virtual environment using venv. For instance, 
+After that, create a virtual enviroment using venv or other tool of your preference. For instance, 
 using the following command in the prompt line:
 
 ```
 $ python3 -m venv venv
 ```
 
-Then, activate the virtual environment in the prompt line. Like, the following command:
+Then, activate the virtual enviroment in the prompt line. Like, the following command:
 
 ```
 $ source venv/bin/activate
 ```
 
 After that, you are ready to install 
 
@@ -215,44 +178,32 @@
 ### 4.2 Windows
 
 First, make sure you have Microsoft C++ Build Tools. Then install graphviz software by download one suitable version 
 in this [link](https://graphviz.org/download/#windows). Next, install the latex-suite like these 
 [tutorial](https://www.tug.org/texlive/windows.html#install) explains. Then, install Popple packed for windows, 
 which you download [here](https://github.com/oschwartz10612/poppler-windows).
 
-Finally, you can install text2story using pip. If it did not recognize the graphviz installation, then you can 
+Finnally, you can install text2story using pip. If it did not recognize the graphviz installation, then you can 
 use the following command for pip (tested in pip == 21.1.1).
 
 ```
 pip install text2story  --global-option=build_ext --global-option="-IC:\Program Files\Graphviz\include" --global-option="-LC:\Program Files\Graphviz\lib\"
 ```
 
 For newer version of pip (tested in pip == 23.1.2), you can type the following command:
 
 ```
 pip install --use-pep517  --config-setting="--global-option=build_ext"  --config-setting="--global-option=-IC:\Program Files\Graphviz\include" --config-setting="--global-option=-LC:\Program Files\Graphviz\lib"
 ```
 
-You need to make sure that venv is also installed in your environment. You can do this by using pip in you 
-PowerShell command line (or another similar shell). 
 
+<a name="webapp"></a>
+## Web App
 ```
-$ python3 -m pip install virtualenv
+#### Web app
+```ssh
+python backend.py
+streamlit run main.py
 ```
+and a page on your browser will open!
 
-Next, you will be able to create a virtual environment with the following command.
 
-```
-$ python3 -m venv venv
-```
-
-Then, activate the virtual environment in the prompt line. Like, the following command:
-
-```
-$ python3 -m venv venv
-```
-
-Then, activate the virtual environment in the prompt line. Like, the following command:
-
-```
-$ .\venv\Scripts\activate
-```
```

### Comparing `text2story-1.4.4/README.md` & `text2story-1.4.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,48 @@
+Metadata-Version: 2.1
+Name: text2story
+Version: 1.4.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: joblib
+Requires-Dist: spacy
+Requires-Dist: py-heideltime
+Requires-Dist: importlib_metadata
+Requires-Dist: pandas<2.0.0
+Requires-Dist: plantuml
+Requires-Dist: matplotlib
+Requires-Dist: networkx
+Requires-Dist: netgraph
+Requires-Dist: pytorch-crf
+Requires-Dist: transformers
+Requires-Dist: torch
+Requires-Dist: pdf2image
+Requires-Dist: latexcompiler
+Requires-Dist: nltk
+Requires-Dist: thinc
+Requires-Dist: beautifulsoup4
+Requires-Dist: streamlit==1.3.1
+Requires-Dist: altair==4.2.2
+Requires-Dist: protobuf==3.20
+
 # Text2Story main package
 The Text2Story main package contains the main classes and methods for the T2S pipeline: from text to formal representation to visualization or other representation.
 
 - **Relation to Brat2Viz**
-The Text2Story package is a generalization of Brat2Viz and should in fact contain all the functionalities and variants of the T2S project output.
+The Text2Story package is a generalization of Brat2Viz and should in fact contain all the funcionalities and variants of the T2S project output.
 
 ## Table of Contents
 
 1. [ Getting Start. ](#start)
 2. [ The Framework Structure. ](#structure)
 3. [ The Annotators. ](#annotators)
 4. [ Installation. ](#installation)
    - 4.1\. [ Linux Ubuntu ](#installationlinux)
    - 4.2\. [ Windows ](#installationwindows)
-
+5. [ The Web App. ](#webapp)
 
 <a name="start"></a>
 ## 1. Getting Started
 
 The main goal of the text2story is to extract narrative from raw text. The narrative 
 components comprise events, the participants (or participants) in the events, and the time expressions. 
 
@@ -155,33 +181,22 @@
 The installation requires graphviz software, the latex suite and the software poppler to convert pdf to png. 
 In Linux, to install these software open a terminal and type the following commands:
 
 ```
 sudo apt-get install graphviz libgraphviz-dev texlive-latex-base  texlive-latex-extra poppler-utils
 ```
 
-You will need a virtual environment as well. If you do not have venv, you can install it in linux by using the 
-apt-get command or pip command. Next, we demonstrate these two ways of install it.
-
-```
-sudo apt-get install python3-venv
-```
-
-```
-python3 -m pip install virtualenv
-```
-
-After that, you will be able to create a virtual environment using venv. For instance, 
+After that, create a virtual enviroment using venv or other tool of your preference. For instance, 
 using the following command in the prompt line:
 
 ```
 $ python3 -m venv venv
 ```
 
-Then, activate the virtual environment in the prompt line. Like, the following command:
+Then, activate the virtual enviroment in the prompt line. Like, the following command:
 
 ```
 $ source venv/bin/activate
 ```
 
 After that, you are ready to install 
 
@@ -189,44 +204,32 @@
 ### 4.2 Windows
 
 First, make sure you have Microsoft C++ Build Tools. Then install graphviz software by download one suitable version 
 in this [link](https://graphviz.org/download/#windows). Next, install the latex-suite like these 
 [tutorial](https://www.tug.org/texlive/windows.html#install) explains. Then, install Popple packed for windows, 
 which you download [here](https://github.com/oschwartz10612/poppler-windows).
 
-Finally, you can install text2story using pip. If it did not recognize the graphviz installation, then you can 
+Finnally, you can install text2story using pip. If it did not recognize the graphviz installation, then you can 
 use the following command for pip (tested in pip == 21.1.1).
 
 ```
 pip install text2story  --global-option=build_ext --global-option="-IC:\Program Files\Graphviz\include" --global-option="-LC:\Program Files\Graphviz\lib\"
 ```
 
 For newer version of pip (tested in pip == 23.1.2), you can type the following command:
 
 ```
 pip install --use-pep517  --config-setting="--global-option=build_ext"  --config-setting="--global-option=-IC:\Program Files\Graphviz\include" --config-setting="--global-option=-LC:\Program Files\Graphviz\lib"
 ```
 
-You need to make sure that venv is also installed in your environment. You can do this by using pip in you 
-PowerShell command line (or another similar shell). 
 
+<a name="webapp"></a>
+## Web App
 ```
-$ python3 -m pip install virtualenv
+#### Web app
+```ssh
+python backend.py
+streamlit run main.py
 ```
+and a page on your browser will open!
 
-Next, you will be able to create a virtual environment with the following command.
 
-```
-$ python3 -m venv venv
-```
-
-Then, activate the virtual environment in the prompt line. Like, the following command:
-
-```
-$ python3 -m venv venv
-```
-
-Then, activate the virtual environment in the prompt line. Like, the following command:
-
-```
-$ .\venv\Scripts\activate
-```
```

### Comparing `text2story-1.4.4/setup.cfg` & `text2story-1.4.5/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 description-file = README.md
 name = text2story
-version = 1.4.4
+version = 1.4.5
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
 packages = find:
 zip_safe = True
 include_package_data = True
@@ -28,14 +28,14 @@
 	thinc
 	beautifulsoup4
 	streamlit==1.3.1
 	altair==4.2.2
 	protobuf==3.20
 
 [options.package_data]
-example = *.joblib, *.json,annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/*.txt, *.pt
+example = *.joblib, *.json, *.pt
 * = README.md
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `text2story-1.4.4/text2story/__init__.py` & `text2story-1.4.5/text2story/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/labels.txt` & `text2story-1.4.5/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/labels.txt`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/config.json` & `text2story-1.4.5/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/config.json`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/linear_layer.pt` & `text2story-1.4.5/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/linear_layer.pt`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/annotators/ALLENNLP/PropBankBr.py` & `text2story-1.4.5/text2story/annotators/ALLENNLP/PropBankBr.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/annotators/ALLENNLP/__init__.py` & `text2story-1.4.5/text2story/annotators/ALLENNLP/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/annotators/ALLENNLP/allen_wrapper.py` & `text2story-1.4.5/text2story/annotators/ALLENNLP/allen_wrapper.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/annotators/ALLENNLP/my_model.py` & `text2story-1.4.5/text2story/annotators/ALLENNLP/my_model.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/annotators/ALLENNLP/my_reader.py` & `text2story-1.4.5/text2story/annotators/ALLENNLP/my_reader.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/annotators/ALLENNLP/preprocess.py` & `text2story-1.4.5/text2story/annotators/ALLENNLP/preprocess.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/annotators/ALLENNLP/requirements.txt` & `text2story-1.4.5/text2story/annotators/ALLENNLP/requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -307,16 +307,14 @@
     # via google-auth
 pydantic==1.8.2
     # via
     #   langchain
     #   openapi-schema-pydantic
     #   spacy
     #   thinc
-pygraphviz==1.10
-    # via text2story (pyproject.toml)
 pyparsing==3.0.9
     # via
     #   grandalf
     #   httplib2
     #   matplotlib
 pysocks==1.7.1
     # via requests
```

### Comparing `text2story-1.4.4/text2story/annotators/BERTNERPT/POS_tagger_brill.pkl` & `text2story-1.4.5/text2story/annotators/BERTNERPT/POS_tagger_brill.pkl`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/annotators/BERTNERPT/__init__.py` & `text2story-1.4.5/text2story/annotators/BERTNERPT/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/annotators/CUSTOMPT/__init__.py` & `text2story-1.4.5/text2story/annotators/CUSTOMPT/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/annotators/CUSTOMPT/crf_v2.1.joblib` & `text2story-1.4.5/text2story/annotators/CUSTOMPT/crf_v2.1.joblib`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/annotators/CUSTOMPT/event_model.py` & `text2story-1.4.5/text2story/annotators/CUSTOMPT/event_model.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/annotators/CUSTOMPT/feature_extractor.py` & `text2story-1.4.5/text2story/annotators/CUSTOMPT/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/annotators/NLTK/__init__.py` & `text2story-1.4.5/text2story/annotators/NLTK/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/annotators/PY_HEIDELTIME/__init__.py` & `text2story-1.4.5/text2story/annotators/PY_HEIDELTIME/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/annotators/SPACY/__init__.py` & `text2story-1.4.5/text2story/annotators/SPACY/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/annotators/SPARKNLP/__init__.py` & `text2story-1.4.5/text2story/annotators/SPARKNLP/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/annotators/SRLWeakLabeling/__init__.py` & `text2story-1.4.5/text2story/annotators/SRLWeakLabeling/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/annotators/TEI2GO/__init__.py` & `text2story-1.4.5/text2story/annotators/TEI2GO/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/annotators/__init__.py` & `text2story-1.4.5/text2story/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/brat2viz/README.md` & `text2story-1.4.5/text2story/brat2viz/README.md`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/brat2viz/brat2drs/brat2drs.py` & `text2story-1.4.5/text2story/brat2viz/brat2drs/brat2drs.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/brat2viz/brat2drs/files_monitor.py` & `text2story-1.4.5/text2story/brat2viz/brat2drs/files_monitor.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/brat2viz/brat2json/brat2json.py` & `text2story-1.4.5/text2story/brat2viz/brat2json/brat2json.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/brat2viz/drs2viz/app.py` & `text2story-1.4.5/text2story/brat2viz/drs2viz/app.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/brat2viz/drs2viz/parser.py` & `text2story-1.4.5/text2story/brat2viz/drs2viz/parser.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/brat2viz/drs2viz/viz.py` & `text2story-1.4.5/text2story/brat2viz/drs2viz/viz.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/core/annotator.py` & `text2story-1.4.5/text2story/core/annotator.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/core/entity_structures.py` & `text2story-1.4.5/text2story/core/entity_structures.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/core/exceptions.py` & `text2story-1.4.5/text2story/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/core/graph_builder.py` & `text2story-1.4.5/text2story/core/graph_builder.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/core/link_structures.py` & `text2story-1.4.5/text2story/core/link_structures.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/core/narrative.py` & `text2story-1.4.5/text2story/core/narrative.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/core/utils.py` & `text2story-1.4.5/text2story/core/utils.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/experiments/compare_ann.py` & `text2story-1.4.5/text2story/experiments/compare_ann.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/experiments/cp_notlusa.py` & `text2story-1.4.5/text2story/experiments/cp_notlusa.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/experiments/evaluate_gpt.py` & `text2story-1.4.5/text2story/experiments/evaluate_gpt.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/experiments/evaluation.py` & `text2story-1.4.5/text2story/experiments/evaluation.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/experiments/exp_en_pb.json` & `text2story-1.4.5/text2story/experiments/exp_en_pb.json`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/experiments/metrics.py` & `text2story-1.4.5/text2story/experiments/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from collections import Counter
+
+
 
 def partial_match(b1, e1, b2, e2):
     """
     Check if the interval (b1,e1) intersects
     with the interval (b2, e2)
 
     @param int: beginning of a interval
@@ -107,14 +110,15 @@
 
     @param dictionary: dictionary of annotations
 
     @return tuple list of integers
     """
 
     interval_lst = []
+
     for el in ann_lst:
         s1, e1 = el["offset1"]
         interval_lst.append((s1, e1, el["id"]))
         if "offset2" in el:
             s2, e2 = el["offset2"]
             interval_lst.append((s2, e2, el["id"]))
 
@@ -452,7 +456,9 @@
              else:
                  search_target[id_srlink] = None
         else:
             search_target[id_srlink] = None
 
     return search_pred, search_target
 
+
+
```

### Comparing `text2story-1.4.4/text2story/experiments/run_experiments.py` & `text2story-1.4.5/text2story/experiments/run_experiments.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/readers/pb-vn2.json` & `text2story-1.4.5/text2story/readers/pb-vn2.json`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/readers/read.py` & `text2story-1.4.5/text2story/readers/read.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/readers/read_ace.py` & `text2story-1.4.5/text2story/readers/read_ace.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/readers/read_brat.py` & `text2story-1.4.5/text2story/readers/read_brat.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,14 +250,38 @@
             #if "offset2_end" not in ann[ent_type]:
             #    print("-->", ann[ent_type])
             new_ann_ent = self.merge_span(ann[ent_type])
             new_ann[ent_type] = new_ann_ent
 
         return new_ann
 
+    def get_attribute_value(self, element_id, attr_name):
+        if attr_name in self.ann_ref:
+            if element_id in self.ann_ref[attr_name]:
+                return self.ann_ref[attr_name][element_id]
+
+    def get_relation(self, element_a, element_b):
+        """
+        Get the relation name between two entities (their ids)
+        @param element_a: String with the id of an entity
+        @param element_b: String with the id of an entity
+        @return: String with relation name, NOne if there is no relation between
+        elements A and B
+        """
+
+        annotation_types = list(self.ann_ref.keys())
+        annotation_links_types = [ann_type for ann_type in annotation_types if "LINK" in ann_type]
+
+        for relation_name in  annotation_links_types:
+            if element_a in self.ann_ref[relation_name]:
+                if element_b in self.ann_ref[relation_name][element_a]:
+                    return relation_name
+
+
+
     def read_annotation_file(self, file_ann, merge_entities=False):
         """
         It reads only the annotation file, then returns
         the processed tokens as TokenCorpus type
 
         @param string: path of data to gather and process
 
@@ -319,33 +343,39 @@
                             offset1_end = int(line_toks[3])
 
                             value = " ".join(line_toks[4:])
 
                             ann[ann_type].append({"id":line_toks[0],"offset1": (offset1_start, offset1_end), \
                                               "value": value})
                     elif line[0] == 'R':
+                        e1 = line_toks[2].split(":")[1]  # entity 1
+                        e2 = line_toks[3].split(":")[1]  # entity 2
+                        rel_id = line_toks[0]
                         if ann_type.startswith("SEMROLE") or ann_type.startswith("SRLINK"):
-                            e1 = line_toks[2].split(":")[1] # entity 1
-                            e2 = line_toks[3].split(":")[1] # entity 2
-                            ann["SRLINK"].append({"id":line_toks[0],"args":(e1, e2)})
+                            ann["SRLINK"].append({"id":rel_id,"args":(e1, e2)})
+
+
+                        if ann_type in self.ann_ref:
+                            if e1 in self.ann_ref[ann_type]:
+                                self.ann_ref[ann_type][e1].append(e2)
+                            else:
+                                self.ann_ref[ann_type][e1] = [e2]
+                        else:
+                            self.ann_ref[ann_type] = {e1: [e2]}
 
                     elif line[0] == 'A': # for now ignore attributes
 
-                        ref = line[2]
-                        attr_name = line[1]
-                        attr_value = line[3]
+                        ref = line_toks[2]
+                        attr_name = line_toks[1]
+                        attr_value = line_toks[3]
 
                         if ann_type in self.ann_ref:
-                            # ann_type keeps the last type of annotation
-                            if ref in self.ann_ref[ann_type]:
-                                self.ann_ref[ann_type][ref][attr_name] =  attr_value
-                            else:
-                                self.ann_ref[ann_type][ref] = {attr_name: attr_value}
+                            self.ann_ref[ann_type][ref] = attr_value
                         else:
-                            self.ann_ref[ann_type] = {ref:{attr_name:attr_value}}
+                            self.ann_ref[ann_type] = {ref:attr_value}
         if merge_entities:
             return self.merge_entity_span(ann)
         else:
             return ann
 
     def process(self, data_dir, split=None):
         """
@@ -373,15 +403,15 @@
                 if f.endswith(".ann"):
 
                     p = Path(f)
                     if split_lst != [] and not(p.stem + ".txt" in split_lst):
                         continue
                  
                     fullname = os.path.join(data_dir, p.stem)
-                    print("-->", fullname)
+                    #print("-->", fullname)
                     token_lst = self.process_file(fullname)
                     self.file_lst.append(fullname + ".txt")
 
                     if len(token_lst) > 0:
                         data_tokens.append(token_lst)
 
         return data_tokens
@@ -405,32 +435,37 @@
         """
         count = 0
         token_lst = []
         ref2tok = {}
 
     
         sent_id = -1
+        clause_id = 0
         for tok_idx, tok in enumerate(doc):
-
             if tok.is_sent_start:
                 sent_id += 1
 
+            # Check if the token marks the end of a clause
+            if tok.dep_ in ["punct", "mark"]:
+                clause_id += 1
+
             
             mytok = token_corpus.TokenCorpus()
             mytok.id = count
             mytok.text = tok.text
             mytok.lemma = tok.lemma_
             mytok.pos = tok.pos_
             mytok.dep = tok.dep_
             mytok.head = tok.head.text
             mytok.head_pos = tok.head.pos_
             mytok.head_lemma = tok.head.lemma_
             mytok.offset = tok.idx
             mytok.sent_id = sent_id
-
+            mytok.clause_id = clause_id
+            #print("-->",clause_id, sent_id)
 
 
             ans = self.search_all_idx(tok.idx, ann_idx)
 
             # TODO: it is necessary perform a more efficient search
             # a possible subtoken annotation
             # perform more than one search, and build a list of id's
```

### Comparing `text2story-1.4.4/text2story/readers/read_ecb.py` & `text2story-1.4.5/text2story/readers/read_ecb.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/readers/read_framenet.py` & `text2story-1.4.5/text2story/readers/read_framenet.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/readers/read_propbank.py` & `text2story-1.4.5/text2story/readers/read_propbank.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/readers/token_corpus.py` & `text2story-1.4.5/text2story/readers/token_corpus.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,25 +16,38 @@
         self.head = None
         self.head_pos = None
         self.head_lemma = None
         self.gov_verb = None
         self.gov_verb_idx = None
         self.srl = None
         self.sent_id = None
+        self.clause_id = None
 
         self.offset = None
         self.attr = []
 
         # a token can be annotated by more than one 
         # layer, therefore it can present more than one 
         # id
         self.id_ann = []
 
         # a list of items of type TokenRelation
-        self.relations = [] 
+        self.relations = []
+
+    def get_attr_value(self,attr_name, token_type=None):
+        for (type_, attr_map) in self.attr:
+            if token_type != None and type_ == token_type:
+                return attr_map.get(attr_name)
+            else:
+                return attr_map.get(attr_name)
+    def is_type(self, token_type):
+        for (type_, _) in self.attr:
+            if type_ == token_type:
+                return True
+        return False
 
 class TokenRelation:
     """
     Specifies a Relation between tokens
     """
     def __init__(self, rel_id, toks = [], rel_type = None, argn = None, arg_id = None):
         self.rel_id = rel_id
```

### Comparing `text2story-1.4.4/text2story/readers/utils.py` & `text2story-1.4.5/text2story/readers/utils.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/select/bubble.py` & `text2story-1.4.5/text2story/select/bubble.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-
 import json
 
 from dataclasses import dataclass, field
 from typing import List
 
 from text2story.readers.token_corpus import TokenCorpus
 from text2story.select.event import get_all_events, get_event_type
 from text2story.select.event import sieve_bbubbles_events, is_event
 
+
 def is_type_rel(type_rel, type_rel_lst):
+    for t in type_rel_lst:
+        if type_rel.startswith(t):
+            return True
+    return False
 
-        for t in type_rel_lst:
-            if type_rel.startswith(t):
-                return True
-        return False
 
 class Bubble:
 
-    def __init__(self, event = None):
-        #print("-->", event)
+    def __init__(self, event=None):
+        # print("-->", event)
         self.event_chain = []
         if isinstance(event, list):
 
             self.event = event[0]
             if len(event) > 1:
                 self.event_chain = event
         else:
-            self.event = event # event trigger as TokenCorpus
-        #if event is not None:
+            self.event = event  # event trigger as TokenCorpus
+        # if event is not None:
         #    print("-->", event.id_ann)
-        self.relations = [] # the edges to other bubbles (BubbleEdge)
-       
+        self.relations = []  # the edges to other bubbles (BubbleEdge)
+
         self.name = ""
         # a text span (type:[TokenCorpus]) that is connected 
         # by an SRLINK_agent to this event
-        self.agent = Agent() 
+        self.agent = Agent()
 
     def get_event_text(self):
         if self.event_chain == []:
             return self.event.text
         else:
             tok_txt = [tok.text for tok in self.event_chain]
             return " ".join(tok_txt)
@@ -53,37 +53,34 @@
         for bubble_rel in self.relations:
             if bubble_rel.edge_type in hist_rel:
                 hist_rel[bubble_rel.edge_type] += 1
             else:
                 hist_rel[bubble_rel.edge_type] = 1
         return hist_rel
 
-    def add_agent_relations(self, map_ann, relations_set, type_rel_lst = []):
+    def add_agent_relations(self, map_ann, relations_set, type_rel_lst=[]):
 
         # this bubble does not have an agent object
         if len(self.agent.span) == 0:
             return
 
-
         # iterate through the relations of the agent of
         # the event in the bubble
         current_agent = self.agent
         while current_agent != None:
 
-
             for rel in current_agent.span[0].relations:
 
                 for id_ann_rel in rel.toks[0].id_ann:
 
                     if rel.rel_type in type_rel_lst and rel.rel_id not in relations_set:
 
                         if id_ann_rel in map_ann:
                             object_rel = map_ann[id_ann_rel]
 
-
                             if isinstance(object_rel, Agent):
 
                                 relation = RelationsAgent(object_rel,
                                                           rel.rel_type,
                                                           rel.rel_id)
                                 relation.set_arg(rel.argn)
 
@@ -94,166 +91,169 @@
                                                                 rel.rel_id)
                                 relation.set_arg(rel.argn)
                                 current_agent.relations_bubbles.append(relation)
 
                             relations_set.add(rel.rel_id)
             current_agent = current_agent.next_agent
 
-    def add_relations(self, map_ann,  relations_set, type_rel_lst = []):
-
-
+    def add_relations(self, map_ann, relations_set, type_rel_lst=[]):
 
         for rel in self.event.relations:
             self_event_type = get_event_type(self.event)
 
             for idx_rel, id_ann_rel in enumerate(rel.toks[0].id_ann):
                 ann_type_rel, attr_rel = rel.toks[0].attr[idx_rel]
 
                 # getting the participant connected to this bubble
-                if "Reporting" in self_event_type and\
-                     (rel.rel_type.startswith("SRLINK")) and\
-                     ann_type_rel == "Participant" and\
-                     id_ann_rel == rel.arg_id and\
-                     rel.toks[0].sent_id == int(self.event.sent_id):
-                     # the last condition test if the id of this token chain if related
-                     # to the current relation
-
-
-                     agent_pointer = self.agent.add_agent(rel.toks)
-                     id_ann_agent = rel.toks[0].id_ann[0]
-                     map_ann[id_ann_agent] = agent_pointer
-
-                     #print("Agent %s Event %s ID REL %s %d %s" % (id_ann_agent, self.get_id_ann(), rel.rel_id, idx_rel, rel.arg_id))
-
-                if id_ann_rel in map_ann and\
-                 rel.rel_id not in relations_set and\
-                 is_type_rel(rel.rel_type, type_rel_lst):
-
-                     if not(isinstance(map_ann[id_ann_rel], Agent)):
-                         #print("Event %s ID REL %s %d %s %s" % (self.get_id_ann(), rel.rel_id, idx_rel, rel.arg_id, rel.rel_type))
-                         bubble_rel = map_ann[id_ann_rel]
-                         relation = BubbleRelation(rel.rel_type,\
-                                              bubble_rel,\
-                                              rel.argn)
-
-                         self.relations.append(relation)
-                         relations_set.add(rel.rel_id)
-
-                    #prnt("==>", rel.rel_type)
-                    #print("-->", rel.rel_id)
-                    #print("-->",rel.argn)
+                if "Reporting" in self_event_type and \
+                        (rel.rel_type.startswith("SRLINK")) and \
+                        ann_type_rel == "Participant" and \
+                        id_ann_rel == rel.arg_id and \
+                        rel.toks[0].sent_id == int(self.event.sent_id):
+                    # the last condition test if the id of this token chain if related
+                    # to the current relation
+
+                    agent_pointer = self.agent.add_agent(rel.toks)
+                    id_ann_agent = rel.toks[0].id_ann[0]
+                    map_ann[id_ann_agent] = agent_pointer
+
+                    # print("Agent %s Event %s ID REL %s %d %s" % (id_ann_agent, self.get_id_ann(), rel.rel_id, idx_rel, rel.arg_id))
+                # if it is a link between two reporting events, it ignores this link
+                event_arg2_class = get_event_type(rel.toks[0])
+                if "Reporting" in event_arg2_class and "Reporting" in self_event_type:
+                    continue
+
+                if id_ann_rel in map_ann and \
+                        rel.rel_id not in relations_set and \
+                        is_type_rel(rel.rel_type, type_rel_lst):
+
+                    if not (isinstance(map_ann[id_ann_rel], Agent)):
+                        #print("Event %s ID REL %s %d %s %s" % (self.get_id_ann(), rel.rel_id, idx_rel, rel.arg_id, rel.rel_type))
+                        bubble_rel = map_ann[id_ann_rel]
+                        relation = BubbleRelation(rel.rel_type, \
+                                                  bubble_rel, \
+                                                  rel.argn)
+
+                        self.relations.append(relation)
+                        relations_set.add(rel.rel_id)
+
+                # prnt("==>", rel.rel_type)
+                # print("-->", rel.rel_id)
+                # print("-->",rel.argn)
+
+
 @dataclass
 class Agent:
-
     span: [TokenCorpus] = field(default_factory=list)
-    relations_bubbles:['RelationsBubbleAgent'] = field(default_factory=list)
+    relations_bubbles: ['RelationsBubbleAgent'] = field(default_factory=list)
     relations_agent: List['RelationsAgent'] = field(default_factory=list)
     name: str = ""
     next_agent: 'Agent' = None
 
     def add_agent(self, toks: [TokenCorpus]):
         if self.span != []:
             current_agent = self
             while current_agent.next_agent != None:
                 current_agent = current_agent.next_agent
 
-            current_agent.next_agent = Agent(span = toks)
+            current_agent.next_agent = Agent(span=toks)
             return current_agent.next_agent
 
         else:
             self.span = toks
             return self
 
+
 @dataclass
 class RelationsBubbleAgent:
     bubble: Bubble
     rel_type: str
-    rel_id:str
+    rel_id: str
 
     def set_arg(self, argn):
 
         # if the relation starts with the agent pointer,
         # then its type is out
         if argn == "arg1":
             self.out = True
         else:
             self.out = False
+
+
 @dataclass
 class RelationsAgent:
     agent: Agent
     rel_type: str
-    rel_id:str
+    rel_id: str
 
     def set_arg(self, argn):
 
         # if the relation starts with the agent pointer,
         # then its type is out
         if argn == "arg1":
             self.out = True
         else:
             self.out = False
 
 
 class BigBubble:
 
-    def __init__(self, event = None):
-        #print("BigBubble")
+    def __init__(self, event=None):
+        # print("BigBubble")
         self.bubble_ = Bubble(event)
         self.little_bubbles = []
-        self.idx = 0 
+        self.idx = 0
 
     def add_bubble(self, event):
-        #print("add_bubble")
+        # print("add_bubble")
         self.bubble_ = Bubble(event)
 
         return self.bubble_
-        
-    def add_little_bubble(self, event_lst):
 
-        #print("add_little_bubble")
+    def add_little_bubble(self, event_lst):
+        # print("add_little_bubble")
         little_bubble = Bubble(event_lst)
         self.little_bubbles.append(little_bubble)
 
         return little_bubble
 
     def sort_by_offset(self):
         # sort little bubbles by offset
-        tmp_bubbles = [(b,b.event.offset) for b in self.little_bubbles]
-        tmp_bubbles = sorted(tmp_bubbles, key=lambda x:x[1])
+        tmp_bubbles = [(b, b.event.offset) for b in self.little_bubbles]
+        tmp_bubbles = sorted(tmp_bubbles, key=lambda x: x[1])
         self.little_bubbles = [b for (b, offset) in tmp_bubbles]
 
-    def create_relations(self, map_ann, relations_set, type_rel_lst = []):
-
+    def create_relations(self, map_ann, relations_set, type_rel_lst=[]):
         # add big bubble relations
-        self.bubble_.add_relations(map_ann,relations_set, type_rel_lst)
+        self.bubble_.add_relations(map_ann, relations_set, type_rel_lst)
 
-        
         # create relations for the little bubbles
         for bubble in self.little_bubbles:
             bubble.add_relations(map_ann, relations_set, type_rel_lst)
 
+
 class BubbleRelation:
     def __init__(self, edge_type, bubble, argn):
         self.edge_type = edge_type
         self.bubble_pointer = bubble
 
         # if the relation starts with bubble pointer,
         # then its type is out
         if argn == "arg1":
             self.out = True
         else:
             self.out = False
 
+
 class BubbleMap:
 
     def __init__(self):
-        self.map = {} # sent_id -> BigBubble
+        self.map = {}  # sent_id -> BigBubble
 
-
-    def collect_bubble_tokens(self,tok_lst, sent_id, map_ann):
+    def collect_bubble_tokens(self, tok_lst, sent_id, map_ann):
 
         bubble_toks = []
 
         for tok in tok_lst:
 
             # only events
             if is_event(tok):
@@ -269,24 +269,25 @@
                     bubble_toks.append(tok)
 
         return bubble_toks
 
     def build_map(self, tok_lst: [TokenCorpus], type_big_bubble: str, type_rel_lst: [str]) -> None:
 
         # for each id annotation get the related events
-        event_lst = get_all_events(tok_lst)
+        all_event_lst = get_all_events(tok_lst)
 
         # get only eligible big bubble events (with temporal links identity events)
-        event_lst, not_big_bubble_events = sieve_bbubbles_events(event_lst, type_big_bubble)
+        event_lst, not_big_bubble_events = sieve_bbubbles_events(all_event_lst, type_big_bubble)
 
         event_lst = [event_lst[id_ann] for id_ann in event_lst]
 
         # map the bubble by the id of annotations, 
         # then, after create the bubble, we create the bubble relations
-        map_ann = {} 
+        map_ann = {}
+        bubbles_ids = set()
 
         # create the big bubbles
         for event in event_lst:
 
             big_bubble = BigBubble(event)
             sent_id = event[0].sent_id
             id_ann = event[0].id_ann[0]
@@ -301,77 +302,76 @@
                     tok.sent_id = new_sent_id
 
                 self.map[new_sent_id] = big_bubble
             else:
                 self.map[sent_id] = big_bubble
 
             map_ann[id_ann] = big_bubble
-            
+            bubbles_ids.add(id_ann)
+
         for event in event_lst:
             id_ann = event[0].id_ann[0]
-            sent_id = event[0].sent_id    
-            
+            sent_id = event[0].sent_id
+
             for r in event[0].relations:
                 rel_sent_id = r.toks[0].sent_id
                 rel_id_ann = r.toks[0].id_ann[0]
 
                 # if the event related to the current event is in the same sentence,
-                # then add it as a little bubble. Otherwise it is a event that is big bubble,
-                # which was already created before or will be created as a little bubble of 
+                # then add it as a little bubble. Otherwise, it is an event that is big bubble,
+                # which was already created before or will be created as a little bubble
                 # of another big bubble
                 if int(rel_sent_id) == int(sent_id) and is_type_rel(r.rel_type, type_rel_lst):
 
                     # add little bubbles (only events)
                     bubble_toks = self.collect_bubble_tokens(r.toks, sent_id, map_ann)
 
-                
                     if len(bubble_toks) > 0:
                         bbubble = self.map[sent_id]
                         little_bubble = bbubble.add_little_bubble(bubble_toks)
                         lbubble_id_ann = bubble_toks[0].id_ann[0]
-                        
-                        map_ann[lbubble_id_ann] = little_bubble
-                        #print()
+                        bubbles_ids.add(lbubble_id_ann)
 
+                        map_ann[lbubble_id_ann] = little_bubble
+                        # print()
 
-        # events that can be little bubbles, but are not linked to big bubbles 
+        # events that can be little bubbles, but are not linked to big bubbles
         # TODO: mas nao deveriam so eventos que estivessem ligados por tlink?
         for id_ann in not_big_bubble_events:
 
-
             sent_id = not_big_bubble_events[id_ann][0].sent_id
             # it is an already created bubble AND
             if id_ann in map_ann:
                 continue
 
-            #...and there is no big bubble container, ignore this event
+            # ...and there is no big bubble container, ignore this event
             if sent_id not in self.map:
                 continue
-             
-            #print("-->", sent_id, id_ann, not_big_bubble_events[id_ann])
+
+            # print("-->", sent_id, id_ann, not_big_bubble_events[id_ann])
 
             bbubble = self.map[sent_id]
 
             little_bubble = bbubble.add_little_bubble(not_big_bubble_events[id_ann])
             map_ann[id_ann] = little_bubble
-   
-
+            bubbles_ids.add(id_ann)
 
         # keep track of the relations (id) already created
         relations_set = set()
         for sent_id in self.map:
             bbubble = self.map[sent_id]
-            bbubble.create_relations(map_ann, relations_set, type_rel_lst)    
+            bbubble.create_relations(map_ann, relations_set, type_rel_lst)
             bbubble.sort_by_offset()
 
         # now, add the relations regarding the agents
-        type_agent_rel = ["OLINK_objIdentity","OLINK_partOf","OLINK_memberOf","SRLINK_agent","SRLINK_medium"]
+        type_agent_rel = ["OLINK_objIdentity", "OLINK_partOf", "OLINK_memberOf", "SRLINK_agent", "SRLINK_medium"]
         for sent_id in self.map:
             bbubble = self.map[sent_id]
             bbubble.bubble_.add_agent_relations(map_ann, relations_set, type_agent_rel)
+        return  all_event_lst, bubbles_ids
 
     def to_json(self, output_file_name):
 
         data = {}
 
         for sent_id in self.map:
             data[sent_id] = {}
@@ -393,15 +393,16 @@
                 data[sent_id]["bubbles"]["bubble"]["value"] = lbubble.get_event_text()
 
                 for rel in lbubble.relations:
                     data[sent_id]["bubbles"]["bubble"]["relations"] = {}
                     if isinstance(rel.bubble_pointer, Bubble):
                         data[sent_id]["bubbles"]["bubble"]["relations"]["next"] = rel.bubble_pointer.event.id_ann[0]
                     else:
-                        data[sent_id]["bubbles"]["bubble"]["relations"]["next"] = rel.bubble_pointer.bubble_.event.id_ann[0]
+                        data[sent_id]["bubbles"]["bubble"]["relations"]["next"] = \
+                        rel.bubble_pointer.bubble_.event.id_ann[0]
                     data[sent_id]["bubbles"]["bubble"]["relations"]["type"] = rel.edge_type
                     data[sent_id]["bubbles"]["bubble"]["relations"]["out"] = rel.out
 
             # relations
             for rel in big_bubble.bubble_.relations:
                 data[sent_id]["relations"] = {}
 
@@ -411,10 +412,7 @@
                     data[sent_id]["relations"]["next"] = rel.bubble_pointer.bubble_.event.id_ann[0]
 
                 data[sent_id]["relations"]["type"] = rel.edge_type
                 data[sent_id]["relations"]["out"] = rel.out
 
         with open(output_file_name, "w") as fd:
             json.dump(data, fd, indent=4)
-
-
-
```

### Comparing `text2story-1.4.4/text2story/text2viz/Text2Viz.py` & `text2story-1.4.5/text2story/text2viz/Text2Viz.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/text2viz/visualization.py` & `text2story-1.4.5/text2story/text2viz/visualization.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/training/participant_concept.py` & `text2story-1.4.5/text2story/training/participant_concept.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.4/text2story/viz/bubble_tikz.py` & `text2story-1.4.5/text2story/viz/bubble_tikz.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,24 +75,24 @@
 def start_inside_angle(bubble_idx, nbubbles):
 
     
     angle_lst = compute_angles(nbubbles)
 
     bubble_angle = angle_lst[bubble_idx]
 
-    if bubble_angle > 0 and bubble_angle <= 90:
+    if bubble_angle > -45 and bubble_angle < 45:
         return 0
-    elif bubble_angle > -90 and bubble_angle <= 0:
+    elif bubble_angle > - 135 and bubble_angle <= -45:
         return -90
-    elif bubble_angle > -180 and bubble_angle <= -90:
+    elif bubble_angle > -280 and bubble_angle <= -135:
         return -180
     else:
         return -270
 
-def draw_big_bubble(big_bubble, type_event,  angle, map_id2nodes):
+def draw_big_bubble(big_bubble, type_event,  angle, map_id2nodes, has_agent):
 
     sent_id = big_bubble.bubble_.event.sent_id
 
     tikz_str = ""
     
     event_text = big_bubble.bubble_.get_event_text() 
     id_ann = big_bubble.bubble_.event.id_ann[0]
@@ -103,15 +103,15 @@
     name_node = "%s%s_%s" % (type_event.lower(), whole, frac[:1])
     map_id2nodes[id_ann] = name_node
     big_bubble.bubble_.name = name_node
 
     tikz_str += "\\node[report] (%s) at (A.%d) {\\footnotesize %s:%s};\n" % (name_node, angle, sent_id_text, event_text)
     tikz_str += "\n" 
 
-    if big_bubble.bubble_.agent.span != []:
+    if has_agent and big_bubble.bubble_.agent.span != []:
         # draw agents
         shift = 0.5
         current_agent = big_bubble.bubble_.agent
         idx_agent = 0
 
         while current_agent != None:
             name_agent_node = "agent%s_%s_%d" % (whole, frac[:1], idx_agent)
@@ -245,43 +245,45 @@
 
 
         if name_bubble2 not in inside_angle_map:
             inside_angle_map[name_bubble2] = start_inside_angle(bubble_idx, nevents)
 
         inside_angle = inside_angle_map[name_bubble2]
 
-        if rel.out: # arg1: bubble2 arg2: bubble1
-            rel_str = rel_str + "\n \\draw [<-, dashed, arrows = {-Latex[length=5mm, width=2mm]}] " 
-        else:
-            rel_str = rel_str + "\n \\draw [->, dashed, arrows = {-Latex[length=5mm, width=2mm]}] "
+        rel_str = rel_str + "\n \\draw [->, dashed, arrows = {-Latex[length=5mm, width=2mm]}] "
+
 
         if isinstance(bubble1, BigBubble):
             inside_angle1 = 0
             rel_str = rel_str + "(%s.center)" % name_bubble1
+            rel_str = rel_str + " edge [out=%d,in=%d] node[midway, fill=white, sloped] {\\footnotesize %s} (%s);" % (
+            inside_angle1, inside_angle, name_edge, name_bubble2)
+
         else:
             # TODO: testar com inside angle com o bubble1
             if name_bubble1 not in inside_angle_map:
                 # get the index number (a counter that is the index of the event inside a big bubble)
                 bubble_idx1 = int(re.match('.*?([0-9]+)$', name_bubble1).group(1))
                 inside_angle_map[name_bubble1] = start_inside_angle(bubble_idx1, nevents)
 
             inside_angle1 = inside_angle_map[name_bubble1]
-            inside_angle_map[name_bubble1] -= 60 
-            rel_str = rel_str + "(%s)" % name_bubble1
-
-
-        rel_str = rel_str + " edge [out=%d,in=%d] node[midway, fill=white, sloped] {\\footnotesize %s} (%s);" % (inside_angle1, inside_angle,name_edge,  name_bubble2)
+            #inside_angle_map[name_bubble1] -= 60
+            #rel_str = rel_str + "(%s)" % name_bubble1
+            if rel.out:
+                rel_str = rel_str + " (%s) edge [out=%d,in=%d] node[midway, fill=white, sloped] {\\footnotesize %s} (%s);" % \
+                          (name_bubble2, inside_angle1, inside_angle,name_edge,  name_bubble1)
+            else:
+                rel_str = rel_str + " (%s) edge [out=%d,in=%d] node[midway, fill=white, sloped] {\\footnotesize %s} (%s);" % \
+                          (name_bubble1, inside_angle1, inside_angle, name_edge, name_bubble2)
 
-        inside_angle_map[name_bubble2] -= 60
+        #inside_angle_map[name_bubble2] -= 60
                
     else:
-        if rel.out: # arg1:bubble2 arg2:bubble1:
-            rel_str = rel_str + "\n \\draw [<-, very thick, arrows = {-Latex[length=5mm, width=2mm]}] "
-        else:
-            rel_str = rel_str + "\n \\draw [->, very thick, arrows = {-Latex[length=5mm, width=2mm]}] "
+
+        rel_str = rel_str + "\n \\draw [->, very thick, arrows = {-Latex[length=5mm, width=2mm]}] "
 
         isbubble = re.match("r\d+", name_bubble1)
         if isbubble:
 
             sent_id1 = isbubble.group() # the sent id, if bubble 1 is not a big bubble
             sent_id2 = re.match("r\d+", name_bubble2) # the sent_id , if bubble 2 is not a big bubble
 
@@ -296,41 +298,48 @@
                         
                     inside_angle = inside_angle_map[name_bubble2]
                     rel_str = rel_str + "(%s) edge [out=0,in=%d] node[midway, fill=white, sloped] {\\footnotesize %s} (%s);" % (name_bubble1,inside_angle,name_edge,  name_bubble2)
 
                     inside_angle_map[name_bubble2] -= 60    
 
                 else:
-                    rel_str = rel_str + "(%s) -- (%s) node[midway,fill=white,sloped] {\\footnotesize %s};" % (name_bubble1, name_bubble2, name_edge)
+                    if rel.out:
+                        rel_str = rel_str + "(%s) -- (%s) node[midway,fill=white,sloped] {\\footnotesize %s};" % (
+                        name_bubble2, name_bubble1, name_edge)
+                    else:
+                        rel_str = rel_str + "(%s) -- (%s) node[midway,fill=white,sloped] {\\footnotesize %s};" % (name_bubble1, name_bubble2, name_edge)
             else:
                 rel_str = rel_str + "(%s) -- (%s) node[midway,fill=white,sloped] {\\footnotesize %s};" % (name_bubble1, name_bubble2, name_edge)
         else:
 
             rel_str = rel_str + "(%s) -- (%s) node[midway,fill=white,sloped] {\\footnotesize %s};" % (name_bubble1, name_bubble2, name_edge)
 
     
     return rel_str
 
 
-def build_fig(tok_lst, type_event = "Reporting", type_rel_lst = []):
+def build_fig(tok_lst, **kwargs):
+    type_event = kwargs["type_event"]
+    type_rel_lst = kwargs["type_rel_lst"]
+    has_agent = kwargs["has_agent"]
 
     tikz_str = tikz_doc + "\n" + bubble_header()
     
     bubble_map = BubbleMap()
     bubble_map.build_map(tok_lst, type_event, type_rel_lst)
 
     nevents =  len(bubble_map.map)
     angle_lst = compute_angles(nevents)
 
     map_id2nodes = {} # a map of id_ann to nodes id
     
     for idx, sent_id in enumerate(bubble_map.map.keys()):
 
         big_bubble = bubble_map.map[sent_id]
-        tikz_str = tikz_str + "\n" + draw_big_bubble(big_bubble, type_event, angle_lst[idx], map_id2nodes)    
+        tikz_str = tikz_str + "\n" + draw_big_bubble(big_bubble, type_event, angle_lst[idx], map_id2nodes,has_agent)
 
         tikz_str = tikz_str + "\n" + draw_little_bubbles(big_bubble, map_id2nodes)
 
     
     tikz_str = tikz_str + "\n"
 
     
@@ -344,16 +353,17 @@
         bubble_event_id = big_bubble.bubble_.event.id_ann[0]
 
 
         if bubble_event_id not in map_id2nodes:
             continue
 
         nevents = len(big_bubble.little_bubbles)
+
         # draw agent relations
-        if big_bubble.bubble_.agent.span != []:
+        if has_agent and big_bubble.bubble_.agent.span != []:
             current_agent = big_bubble.bubble_.agent
 
             while (current_agent != None):
                 rel_str = draw_agent_relation(current_agent)
                 if rel_str is not None:
                     tikz_str += rel_str
                 current_agent = current_agent.next_agent
@@ -367,47 +377,48 @@
             rel_str = draw_bubble_relation(big_bubble, rel, map_id2nodes, inside_angle_map, nevents)  
             if rel_str is not None:
                 tikz_str += rel_str
 
             
             tikz_str = tikz_str + "\n"
     
-            # draw relations of the little bubbles
-            for little_bubble in big_bubble.little_bubbles:
+         # draw relations of the little bubbles
+        for little_bubble in big_bubble.little_bubbles:
+
+            lbubble_event_id = little_bubble.event.id_ann[0]
+
+            if lbubble_event_id not in map_id2nodes:
+                continue
+
+            # is it in the same big bubble? adjust the angle inside
+            for rel in little_bubble.relations:
+                #print("-->", rel.bubble_pointer.event.id_ann)
+                #if rel.edge_type.startswith("TLINK") and rel.edge_type != "TLINK_identity":
+                #if rel.edge_type.startswith("TLINK"):
+                #    continue
+                rel_str = draw_bubble_relation(little_bubble, rel, map_id2nodes, inside_angle_map, nevents)
+                if rel_str is not None:
+                    tikz_str += rel_str
 
-                lbubble_event_id = little_bubble.event.id_ann[0]
-                #print("==>",lbubble_event_id)
-                #import pdb
-                #pdb.set_trace()
-
-                if lbubble_event_id not in map_id2nodes:
-                     continue
-
-                # is it in the same big bubble? adjust the angle inside
-                for rel in little_bubble.relations:
-                    #if rel.edge_type.startswith("TLINK") and rel.edge_type != "TLINK_identity":
-                    if rel.edge_type.startswith("TLINK"):
-                        continue
-                    rel_str = draw_bubble_relation(little_bubble, rel, map_id2nodes, inside_angle_map, nevents)  
-                    if rel_str is not None:
-                         tikz_str += rel_str
+            print()
 
                 
 
     tikz_str = tikz_str + "\n" + "\\end{tikzpicture}\n\\end{document}\n"
 
     return tikz_str, bubble_map
 
-def build_fig_ann(ann_file, output_dir):
+def build_fig_ann(ann_file, output_dir,**kwargs):
 
-    reader = ReadBrat()
+    lang = kwargs["lang"]
+    reader = ReadBrat(lang)
     data = reader.process_file(ann_file)
 
     #Serao apenas as relações temporais que nao envolvam reporting events ligado pelo TLINK identity.
-    tikz_str, bubble_map = build_fig(data, "Reporting", ["TLINK"])
+    tikz_str, bubble_map = build_fig(data, **kwargs)
 
     bubble_map.to_json(os.path.join(output_dir,"output.txt"))
 
     ann_file_base = os.path.basename(ann_file)
 
     output_file = os.path.join(output_dir, "%s.tex" % ann_file_base)
     with open(output_file, "w") as fd:
```

### Comparing `text2story-1.4.4/text2story.egg-info/PKG-INFO` & `text2story-1.4.5/text2story.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2story
-Version: 1.4.4
+Version: 1.4.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: joblib
 Requires-Dist: spacy
 Requires-Dist: py-heideltime
 Requires-Dist: importlib_metadata
 Requires-Dist: pandas<2.0.0
@@ -24,25 +24,25 @@
 Requires-Dist: altair==4.2.2
 Requires-Dist: protobuf==3.20
 
 # Text2Story main package
 The Text2Story main package contains the main classes and methods for the T2S pipeline: from text to formal representation to visualization or other representation.
 
 - **Relation to Brat2Viz**
-The Text2Story package is a generalization of Brat2Viz and should in fact contain all the functionalities and variants of the T2S project output.
+The Text2Story package is a generalization of Brat2Viz and should in fact contain all the funcionalities and variants of the T2S project output.
 
 ## Table of Contents
 
 1. [ Getting Start. ](#start)
 2. [ The Framework Structure. ](#structure)
 3. [ The Annotators. ](#annotators)
 4. [ Installation. ](#installation)
    - 4.1\. [ Linux Ubuntu ](#installationlinux)
    - 4.2\. [ Windows ](#installationwindows)
-
+5. [ The Web App. ](#webapp)
 
 <a name="start"></a>
 ## 1. Getting Started
 
 The main goal of the text2story is to extract narrative from raw text. The narrative 
 components comprise events, the participants (or participants) in the events, and the time expressions. 
 
@@ -181,33 +181,22 @@
 The installation requires graphviz software, the latex suite and the software poppler to convert pdf to png. 
 In Linux, to install these software open a terminal and type the following commands:
 
 ```
 sudo apt-get install graphviz libgraphviz-dev texlive-latex-base  texlive-latex-extra poppler-utils
 ```
 
-You will need a virtual environment as well. If you do not have venv, you can install it in linux by using the 
-apt-get command or pip command. Next, we demonstrate these two ways of install it.
-
-```
-sudo apt-get install python3-venv
-```
-
-```
-python3 -m pip install virtualenv
-```
-
-After that, you will be able to create a virtual environment using venv. For instance, 
+After that, create a virtual enviroment using venv or other tool of your preference. For instance, 
 using the following command in the prompt line:
 
 ```
 $ python3 -m venv venv
 ```
 
-Then, activate the virtual environment in the prompt line. Like, the following command:
+Then, activate the virtual enviroment in the prompt line. Like, the following command:
 
 ```
 $ source venv/bin/activate
 ```
 
 After that, you are ready to install 
 
@@ -215,44 +204,32 @@
 ### 4.2 Windows
 
 First, make sure you have Microsoft C++ Build Tools. Then install graphviz software by download one suitable version 
 in this [link](https://graphviz.org/download/#windows). Next, install the latex-suite like these 
 [tutorial](https://www.tug.org/texlive/windows.html#install) explains. Then, install Popple packed for windows, 
 which you download [here](https://github.com/oschwartz10612/poppler-windows).
 
-Finally, you can install text2story using pip. If it did not recognize the graphviz installation, then you can 
+Finnally, you can install text2story using pip. If it did not recognize the graphviz installation, then you can 
 use the following command for pip (tested in pip == 21.1.1).
 
 ```
 pip install text2story  --global-option=build_ext --global-option="-IC:\Program Files\Graphviz\include" --global-option="-LC:\Program Files\Graphviz\lib\"
 ```
 
 For newer version of pip (tested in pip == 23.1.2), you can type the following command:
 
 ```
 pip install --use-pep517  --config-setting="--global-option=build_ext"  --config-setting="--global-option=-IC:\Program Files\Graphviz\include" --config-setting="--global-option=-LC:\Program Files\Graphviz\lib"
 ```
 
-You need to make sure that venv is also installed in your environment. You can do this by using pip in you 
-PowerShell command line (or another similar shell). 
-
-```
-$ python3 -m pip install virtualenv
-```
-
-Next, you will be able to create a virtual environment with the following command.
-
-```
-$ python3 -m venv venv
-```
-
-Then, activate the virtual environment in the prompt line. Like, the following command:
 
+<a name="webapp"></a>
+## Web App
 ```
-$ python3 -m venv venv
+#### Web app
+```ssh
+python backend.py
+streamlit run main.py
 ```
+and a page on your browser will open!
 
-Then, activate the virtual environment in the prompt line. Like, the following command:
 
-```
-$ .\venv\Scripts\activate
-```
```

### Comparing `text2story-1.4.4/text2story.egg-info/SOURCES.txt` & `text2story-1.4.5/text2story.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 text2story/readers/token_corpus.py
 text2story/readers/utils.py
 text2story/readers/vn-lirics.json
 text2story/select/README.md
 text2story/select/__init__.py
 text2story/select/bubble.py
 text2story/select/event.py
-text2story/select/links.py
 text2story/text2viz/Text2Viz.py
 text2story/text2viz/__init__.py
 text2story/text2viz/visualization.py
 text2story/training/__init__.py
 text2story/training/participant_concept.py
 text2story/viz/__init__.py
-text2story/viz/bubble_tikz.py
+text2story/viz/bubble_tikz.py
+text2story/viz/msc.py
```

