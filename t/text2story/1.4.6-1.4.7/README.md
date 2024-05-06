# Comparing `tmp/text2story-1.4.6.tar.gz` & `tmp/text2story-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2story-1.4.6.tar", last modified: Mon May  6 11:06:21 2024, max compression
+gzip compressed data, was "text2story-1.4.7.tar", last modified: Mon May  6 12:35:44 2024, max compression
```

## Comparing `text2story-1.4.6.tar` & `text2story-1.4.7.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.475712 text2story-1.4.6/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    33470 2022-10-19 09:22:59.000000 text2story-1.4.6/LICENSE
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      559 2023-09-20 11:40:02.000000 text2story-1.4.6/MANIFEST.in
--rw-r--r--   0 evelinamorim  (1000) evelinamorim  (1000)    10904 2024-05-06 11:06:21.475712 text2story-1.4.6/PKG-INFO
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    10263 2023-12-13 15:05:29.000000 text2story-1.4.6/README.md
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      417 2024-05-06 11:01:40.000000 text2story-1.4.6/pyproject.toml
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      601 2024-05-06 11:06:21.475712 text2story-1.4.6/setup.cfg
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2023-09-11 13:50:06.000000 text2story-1.4.6/setup.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.451712 text2story-1.4.6/text2story/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      757 2022-10-19 09:12:42.000000 text2story-1.4.6/text2story/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       67 2022-10-19 09:12:42.000000 text2story-1.4.6/text2story/__main__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.451712 text2story-1.4.6/text2story/annotators/
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.451712 text2story-1.4.6/text2story/annotators/ALLENNLP/
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.447712 text2story-1.4.6/text2story/annotators/ALLENNLP/Models/
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.451712 text2story-1.4.6/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.455712 text2story-1.4.6/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      739 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/labels.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       14 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/non_padded_namespaces.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1343 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/config.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   265058 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/linear_layer.pt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    10386 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/annotators/ALLENNLP/PropBankBr.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6172 2023-11-08 10:19:59.000000 text2story-1.4.6/text2story/annotators/ALLENNLP/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    28375 2023-11-08 10:15:57.000000 text2story-1.4.6/text2story/annotators/ALLENNLP/allen_wrapper.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13691 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/annotators/ALLENNLP/my_model.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    20528 2023-09-20 15:37:16.000000 text2story-1.4.6/text2story/annotators/ALLENNLP/my_reader.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6217 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/annotators/ALLENNLP/preprocess.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9718 2024-05-06 11:03:00.000000 text2story-1.4.6/text2story/annotators/ALLENNLP/requirements.txt
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.459712 text2story-1.4.6/text2story/annotators/BERTNERPT/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)  2143882 2023-09-12 15:18:59.000000 text2story-1.4.6/text2story/annotators/BERTNERPT/POS_tagger_brill.pkl
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3160 2023-09-19 14:37:58.000000 text2story-1.4.6/text2story/annotators/BERTNERPT/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.459712 text2story-1.4.6/text2story/annotators/CUSTOMPT/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14794 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/annotators/CUSTOMPT/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   371646 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/annotators/CUSTOMPT/crf_v2.1.joblib
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    15093 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/annotators/CUSTOMPT/event_model.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13972 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/annotators/CUSTOMPT/feature_extractor.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.459712 text2story-1.4.6/text2story/annotators/DBPEDIA/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3178 2024-05-06 11:02:12.000000 text2story-1.4.6/text2story/annotators/DBPEDIA/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.459712 text2story-1.4.6/text2story/annotators/NLTK/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2954 2023-09-13 10:57:45.000000 text2story-1.4.6/text2story/annotators/NLTK/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.459712 text2story-1.4.6/text2story/annotators/PY_HEIDELTIME/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1786 2023-10-11 13:29:55.000000 text2story-1.4.6/text2story/annotators/PY_HEIDELTIME/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.459712 text2story-1.4.6/text2story/annotators/SPACY/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1901 2023-09-21 09:23:20.000000 text2story-1.4.6/text2story/annotators/SPACY/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.463712 text2story-1.4.6/text2story/annotators/SPARKNLP/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9462 2022-10-26 12:28:21.000000 text2story-1.4.6/text2story/annotators/SPARKNLP/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.463712 text2story-1.4.6/text2story/annotators/SRL/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    19653 2024-05-06 11:02:12.000000 text2story-1.4.6/text2story/annotators/SRL/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.463712 text2story-1.4.6/text2story/annotators/SRLWeakLabeling/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3501 2023-09-11 13:50:06.000000 text2story-1.4.6/text2story/annotators/SRLWeakLabeling/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.463712 text2story-1.4.6/text2story/annotators/TEI2GO/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1623 2023-09-21 09:11:18.000000 text2story-1.4.6/text2story/annotators/TEI2GO/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     5372 2024-05-06 11:05:42.000000 text2story-1.4.6/text2story/annotators/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.463712 text2story-1.4.6/text2story/brat2viz/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      548 2022-10-19 09:12:42.000000 text2story-1.4.6/text2story/brat2viz/README.md
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2022-10-19 09:12:42.000000 text2story-1.4.6/text2story/brat2viz/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.463712 text2story-1.4.6/text2story/brat2viz/brat2drs/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       37 2022-10-19 09:12:42.000000 text2story-1.4.6/text2story/brat2viz/brat2drs/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    17359 2023-09-11 13:50:06.000000 text2story-1.4.6/text2story/brat2viz/brat2drs/brat2drs.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1059 2022-10-19 09:12:42.000000 text2story-1.4.6/text2story/brat2viz/brat2drs/files_monitor.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.463712 text2story-1.4.6/text2story/brat2viz/brat2json/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-10-24 13:54:25.000000 text2story-1.4.6/text2story/brat2viz/brat2json/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    45447 2023-10-24 14:47:12.000000 text2story-1.4.6/text2story/brat2viz/brat2json/brat2json.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.463712 text2story-1.4.6/text2story/brat2viz/drs2viz/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2022-10-19 09:12:42.000000 text2story-1.4.6/text2story/brat2viz/drs2viz/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2428 2022-10-19 09:12:42.000000 text2story-1.4.6/text2story/brat2viz/drs2viz/app.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13487 2022-10-19 09:12:42.000000 text2story-1.4.6/text2story/brat2viz/drs2viz/parser.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    10956 2023-09-13 14:10:19.000000 text2story-1.4.6/text2story/brat2viz/drs2viz/viz.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.467712 text2story-1.4.6/text2story/core/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-19 13:19:29.000000 text2story-1.4.6/text2story/core/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    12476 2024-05-06 11:02:12.000000 text2story-1.4.6/text2story/core/annotator.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3429 2023-10-09 14:49:24.000000 text2story-1.4.6/text2story/core/entity_structures.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1472 2024-05-06 11:02:12.000000 text2story-1.4.6/text2story/core/exceptions.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      546 2023-09-11 13:50:06.000000 text2story-1.4.6/text2story/core/graph_builder.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3343 2023-09-11 13:50:06.000000 text2story-1.4.6/text2story/core/link_structures.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    28491 2024-05-06 11:02:12.000000 text2story-1.4.6/text2story/core/narrative.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    11397 2023-10-06 10:45:23.000000 text2story-1.4.6/text2story/core/utils.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.467712 text2story-1.4.6/text2story/experiments/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-09-11 13:50:06.000000 text2story-1.4.6/text2story/experiments/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3918 2023-09-11 13:50:06.000000 text2story-1.4.6/text2story/experiments/compare_ann.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3713 2023-10-16 09:18:06.000000 text2story-1.4.6/text2story/experiments/cp_notlusa.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      882 2023-10-19 23:18:46.000000 text2story-1.4.6/text2story/experiments/evaluate_gpt.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    16957 2024-01-31 16:04:58.000000 text2story-1.4.6/text2story/experiments/evaluation.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      429 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/experiments/exp.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      205 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/experiments/exp_en_fn.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      601 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/experiments/exp_en_pb.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    17812 2024-05-06 11:02:12.000000 text2story-1.4.6/text2story/experiments/metrics.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1453 2024-01-31 16:03:53.000000 text2story-1.4.6/text2story/experiments/run_experiments.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     8912 2024-01-16 16:40:49.000000 text2story-1.4.6/text2story/experiments/stats.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.471712 text2story-1.4.6/text2story/readers/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-09-11 13:50:06.000000 text2story-1.4.6/text2story/readers/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      380 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/readers/fn-lirics.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   312656 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/readers/pb-vn2.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      547 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/readers/read.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14407 2023-10-18 07:53:38.000000 text2story-1.4.6/text2story/readers/read_ace.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    27190 2024-05-06 11:02:12.000000 text2story-1.4.6/text2story/readers/read_brat.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1799 2024-05-06 11:02:12.000000 text2story-1.4.6/text2story/readers/read_csv.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    17011 2023-10-06 10:45:23.000000 text2story-1.4.6/text2story/readers/read_ecb.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6081 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/readers/read_framenet.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    11525 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/readers/read_propbank.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1639 2024-01-09 13:08:04.000000 text2story-1.4.6/text2story/readers/token_corpus.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1221 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/readers/utils.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      353 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/readers/vn-lirics.json
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.475712 text2story-1.4.6/text2story/select/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      121 2023-03-27 13:07:12.000000 text2story-1.4.6/text2story/select/README.md
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-09-11 13:50:06.000000 text2story-1.4.6/text2story/select/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    15112 2024-01-18 13:01:37.000000 text2story-1.4.6/text2story/select/bubble.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    10207 2024-01-23 10:09:52.000000 text2story-1.4.6/text2story/select/event.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.475712 text2story-1.4.6/text2story/text2viz/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     5371 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/text2viz/Text2Viz.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/text2viz/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      699 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/text2viz/visualization.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.475712 text2story-1.4.6/text2story/training/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-09-11 13:50:06.000000 text2story-1.4.6/text2story/training/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14422 2023-09-11 13:50:06.000000 text2story-1.4.6/text2story/training/participant_concept.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.475712 text2story-1.4.6/text2story/viz/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-09-11 13:50:06.000000 text2story-1.4.6/text2story/viz/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    15649 2024-01-18 11:52:24.000000 text2story-1.4.6/text2story/viz/bubble_tikz.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2710 2024-01-19 15:14:06.000000 text2story-1.4.6/text2story/viz/msc.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.475712 text2story-1.4.6/text2story.egg-info/
--rw-r--r--   0 evelinamorim  (1000) evelinamorim  (1000)    10904 2024-05-06 11:06:21.000000 text2story-1.4.6/text2story.egg-info/PKG-INFO
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3466 2024-05-06 11:06:21.000000 text2story-1.4.6/text2story.egg-info/SOURCES.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2024-05-06 11:06:21.000000 text2story-1.4.6/text2story.egg-info/dependency_links.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      224 2024-05-06 11:06:21.000000 text2story-1.4.6/text2story.egg-info/requires.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       11 2024-05-06 11:06:21.000000 text2story-1.4.6/text2story.egg-info/top_level.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-05-26 15:56:54.000000 text2story-1.4.6/text2story.egg-info/zip-safe
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 12:35:44.756725 text2story-1.4.7/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    33470 2022-10-19 09:22:59.000000 text2story-1.4.7/LICENSE
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      559 2023-09-20 11:40:02.000000 text2story-1.4.7/MANIFEST.in
+-rw-r--r--   0 evelinamorim  (1000) evelinamorim  (1000)    10904 2024-05-06 12:35:44.756725 text2story-1.4.7/PKG-INFO
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    10263 2023-12-13 15:05:29.000000 text2story-1.4.7/README.md
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      417 2024-05-06 12:34:22.000000 text2story-1.4.7/pyproject.toml
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      601 2024-05-06 12:35:44.756725 text2story-1.4.7/setup.cfg
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2023-09-11 13:50:06.000000 text2story-1.4.7/setup.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 12:35:44.720725 text2story-1.4.7/text2story/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      757 2022-10-19 09:12:42.000000 text2story-1.4.7/text2story/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       67 2022-10-19 09:12:42.000000 text2story-1.4.7/text2story/__main__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 12:35:44.720725 text2story-1.4.7/text2story/annotators/
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 12:35:44.724725 text2story-1.4.7/text2story/annotators/ALLENNLP/
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 12:35:44.716725 text2story-1.4.7/text2story/annotators/ALLENNLP/Models/
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 12:35:44.724725 text2story-1.4.7/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 12:35:44.724725 text2story-1.4.7/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      739 2022-10-13 08:54:40.000000 text2story-1.4.7/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/labels.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       14 2022-10-13 08:54:40.000000 text2story-1.4.7/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/non_padded_namespaces.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1343 2022-10-13 08:54:40.000000 text2story-1.4.7/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/config.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   265058 2022-10-13 08:54:40.000000 text2story-1.4.7/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/linear_layer.pt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    10386 2022-10-13 08:54:40.000000 text2story-1.4.7/text2story/annotators/ALLENNLP/PropBankBr.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6172 2023-11-08 10:19:59.000000 text2story-1.4.7/text2story/annotators/ALLENNLP/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    28394 2024-05-06 12:34:04.000000 text2story-1.4.7/text2story/annotators/ALLENNLP/allen_wrapper.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13691 2022-10-13 08:54:40.000000 text2story-1.4.7/text2story/annotators/ALLENNLP/my_model.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    20528 2023-09-20 15:37:16.000000 text2story-1.4.7/text2story/annotators/ALLENNLP/my_reader.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6217 2022-10-13 08:54:40.000000 text2story-1.4.7/text2story/annotators/ALLENNLP/preprocess.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9718 2024-05-06 11:03:00.000000 text2story-1.4.7/text2story/annotators/ALLENNLP/requirements.txt
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 12:35:44.732725 text2story-1.4.7/text2story/annotators/BERTNERPT/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)  2143882 2023-09-12 15:18:59.000000 text2story-1.4.7/text2story/annotators/BERTNERPT/POS_tagger_brill.pkl
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3160 2023-09-19 14:37:58.000000 text2story-1.4.7/text2story/annotators/BERTNERPT/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 12:35:44.736725 text2story-1.4.7/text2story/annotators/CUSTOMPT/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14794 2022-10-13 08:54:40.000000 text2story-1.4.7/text2story/annotators/CUSTOMPT/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   371646 2022-10-13 08:54:40.000000 text2story-1.4.7/text2story/annotators/CUSTOMPT/crf_v2.1.joblib
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    15093 2022-10-13 08:54:40.000000 text2story-1.4.7/text2story/annotators/CUSTOMPT/event_model.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13972 2022-10-13 08:54:40.000000 text2story-1.4.7/text2story/annotators/CUSTOMPT/feature_extractor.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 12:35:44.736725 text2story-1.4.7/text2story/annotators/DBPEDIA/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3178 2024-05-06 11:02:12.000000 text2story-1.4.7/text2story/annotators/DBPEDIA/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 12:35:44.736725 text2story-1.4.7/text2story/annotators/NLTK/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2954 2023-09-13 10:57:45.000000 text2story-1.4.7/text2story/annotators/NLTK/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 12:35:44.736725 text2story-1.4.7/text2story/annotators/PY_HEIDELTIME/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1786 2023-10-11 13:29:55.000000 text2story-1.4.7/text2story/annotators/PY_HEIDELTIME/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 12:35:44.736725 text2story-1.4.7/text2story/annotators/SPACY/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1901 2023-09-21 09:23:20.000000 text2story-1.4.7/text2story/annotators/SPACY/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 12:35:44.740725 text2story-1.4.7/text2story/annotators/SPARKNLP/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9462 2022-10-26 12:28:21.000000 text2story-1.4.7/text2story/annotators/SPARKNLP/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 12:35:44.740725 text2story-1.4.7/text2story/annotators/SRL/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    19677 2024-05-06 12:32:29.000000 text2story-1.4.7/text2story/annotators/SRL/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 12:35:44.740725 text2story-1.4.7/text2story/annotators/SRLWeakLabeling/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3501 2023-09-11 13:50:06.000000 text2story-1.4.7/text2story/annotators/SRLWeakLabeling/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 12:35:44.740725 text2story-1.4.7/text2story/annotators/TEI2GO/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1623 2023-09-21 09:11:18.000000 text2story-1.4.7/text2story/annotators/TEI2GO/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     5372 2024-05-06 11:05:42.000000 text2story-1.4.7/text2story/annotators/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 12:35:44.740725 text2story-1.4.7/text2story/brat2viz/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      548 2022-10-19 09:12:42.000000 text2story-1.4.7/text2story/brat2viz/README.md
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2022-10-19 09:12:42.000000 text2story-1.4.7/text2story/brat2viz/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 12:35:44.740725 text2story-1.4.7/text2story/brat2viz/brat2drs/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       37 2022-10-19 09:12:42.000000 text2story-1.4.7/text2story/brat2viz/brat2drs/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    17359 2023-09-11 13:50:06.000000 text2story-1.4.7/text2story/brat2viz/brat2drs/brat2drs.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1059 2022-10-19 09:12:42.000000 text2story-1.4.7/text2story/brat2viz/brat2drs/files_monitor.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 12:35:44.740725 text2story-1.4.7/text2story/brat2viz/brat2json/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-10-24 13:54:25.000000 text2story-1.4.7/text2story/brat2viz/brat2json/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    45447 2023-10-24 14:47:12.000000 text2story-1.4.7/text2story/brat2viz/brat2json/brat2json.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 12:35:44.744725 text2story-1.4.7/text2story/brat2viz/drs2viz/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2022-10-19 09:12:42.000000 text2story-1.4.7/text2story/brat2viz/drs2viz/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2428 2022-10-19 09:12:42.000000 text2story-1.4.7/text2story/brat2viz/drs2viz/app.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13487 2022-10-19 09:12:42.000000 text2story-1.4.7/text2story/brat2viz/drs2viz/parser.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    10956 2023-09-13 14:10:19.000000 text2story-1.4.7/text2story/brat2viz/drs2viz/viz.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 12:35:44.744725 text2story-1.4.7/text2story/core/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-19 13:19:29.000000 text2story-1.4.7/text2story/core/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    12476 2024-05-06 11:02:12.000000 text2story-1.4.7/text2story/core/annotator.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3429 2023-10-09 14:49:24.000000 text2story-1.4.7/text2story/core/entity_structures.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1472 2024-05-06 11:02:12.000000 text2story-1.4.7/text2story/core/exceptions.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      546 2023-09-11 13:50:06.000000 text2story-1.4.7/text2story/core/graph_builder.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3343 2023-09-11 13:50:06.000000 text2story-1.4.7/text2story/core/link_structures.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    28491 2024-05-06 11:02:12.000000 text2story-1.4.7/text2story/core/narrative.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    11397 2023-10-06 10:45:23.000000 text2story-1.4.7/text2story/core/utils.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 12:35:44.748725 text2story-1.4.7/text2story/experiments/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-09-11 13:50:06.000000 text2story-1.4.7/text2story/experiments/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3918 2023-09-11 13:50:06.000000 text2story-1.4.7/text2story/experiments/compare_ann.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3713 2023-10-16 09:18:06.000000 text2story-1.4.7/text2story/experiments/cp_notlusa.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      882 2023-10-19 23:18:46.000000 text2story-1.4.7/text2story/experiments/evaluate_gpt.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    16957 2024-01-31 16:04:58.000000 text2story-1.4.7/text2story/experiments/evaluation.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      429 2022-10-13 08:54:40.000000 text2story-1.4.7/text2story/experiments/exp.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      205 2022-10-13 08:54:40.000000 text2story-1.4.7/text2story/experiments/exp_en_fn.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      601 2022-10-13 08:54:40.000000 text2story-1.4.7/text2story/experiments/exp_en_pb.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    17812 2024-05-06 11:02:12.000000 text2story-1.4.7/text2story/experiments/metrics.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1453 2024-01-31 16:03:53.000000 text2story-1.4.7/text2story/experiments/run_experiments.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     8912 2024-01-16 16:40:49.000000 text2story-1.4.7/text2story/experiments/stats.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 12:35:44.752725 text2story-1.4.7/text2story/readers/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-09-11 13:50:06.000000 text2story-1.4.7/text2story/readers/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      380 2022-10-13 08:54:40.000000 text2story-1.4.7/text2story/readers/fn-lirics.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   312656 2022-10-13 08:54:40.000000 text2story-1.4.7/text2story/readers/pb-vn2.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      547 2022-10-13 08:54:40.000000 text2story-1.4.7/text2story/readers/read.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14407 2023-10-18 07:53:38.000000 text2story-1.4.7/text2story/readers/read_ace.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    27190 2024-05-06 11:02:12.000000 text2story-1.4.7/text2story/readers/read_brat.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1799 2024-05-06 11:02:12.000000 text2story-1.4.7/text2story/readers/read_csv.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    17011 2023-10-06 10:45:23.000000 text2story-1.4.7/text2story/readers/read_ecb.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6081 2022-10-13 08:54:40.000000 text2story-1.4.7/text2story/readers/read_framenet.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    11525 2022-10-13 08:54:40.000000 text2story-1.4.7/text2story/readers/read_propbank.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1639 2024-01-09 13:08:04.000000 text2story-1.4.7/text2story/readers/token_corpus.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1221 2022-10-13 08:54:40.000000 text2story-1.4.7/text2story/readers/utils.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      353 2022-10-13 08:54:40.000000 text2story-1.4.7/text2story/readers/vn-lirics.json
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 12:35:44.756725 text2story-1.4.7/text2story/select/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      121 2023-03-27 13:07:12.000000 text2story-1.4.7/text2story/select/README.md
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-09-11 13:50:06.000000 text2story-1.4.7/text2story/select/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    15112 2024-01-18 13:01:37.000000 text2story-1.4.7/text2story/select/bubble.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    10207 2024-01-23 10:09:52.000000 text2story-1.4.7/text2story/select/event.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 12:35:44.756725 text2story-1.4.7/text2story/text2viz/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     5371 2022-10-13 08:54:40.000000 text2story-1.4.7/text2story/text2viz/Text2Viz.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2022-10-13 08:54:40.000000 text2story-1.4.7/text2story/text2viz/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      699 2022-10-13 08:54:40.000000 text2story-1.4.7/text2story/text2viz/visualization.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 12:35:44.756725 text2story-1.4.7/text2story/training/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-09-11 13:50:06.000000 text2story-1.4.7/text2story/training/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14422 2023-09-11 13:50:06.000000 text2story-1.4.7/text2story/training/participant_concept.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 12:35:44.756725 text2story-1.4.7/text2story/viz/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-09-11 13:50:06.000000 text2story-1.4.7/text2story/viz/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    15649 2024-01-18 11:52:24.000000 text2story-1.4.7/text2story/viz/bubble_tikz.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2710 2024-01-19 15:14:06.000000 text2story-1.4.7/text2story/viz/msc.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 12:35:44.756725 text2story-1.4.7/text2story.egg-info/
+-rw-r--r--   0 evelinamorim  (1000) evelinamorim  (1000)    10904 2024-05-06 12:35:44.000000 text2story-1.4.7/text2story.egg-info/PKG-INFO
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3466 2024-05-06 12:35:44.000000 text2story-1.4.7/text2story.egg-info/SOURCES.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2024-05-06 12:35:44.000000 text2story-1.4.7/text2story.egg-info/dependency_links.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      224 2024-05-06 12:35:44.000000 text2story-1.4.7/text2story.egg-info/requires.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       11 2024-05-06 12:35:44.000000 text2story-1.4.7/text2story.egg-info/top_level.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-05-26 15:56:54.000000 text2story-1.4.7/text2story.egg-info/zip-safe
```

### Comparing `text2story-1.4.6/LICENSE` & `text2story-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/MANIFEST.in` & `text2story-1.4.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/PKG-INFO` & `text2story-1.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2story
-Version: 1.4.6
+Version: 1.4.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: joblib
 Requires-Dist: spacy
 Requires-Dist: py-heideltime
 Requires-Dist: importlib_metadata
 Requires-Dist: pandas<2.0.0
```

### Comparing `text2story-1.4.6/README.md` & `text2story-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/setup.cfg` & `text2story-1.4.7/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 description-file = README.md
 name = text2story
-version = 1.4.6
+version = 1.4.7
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
 packages = find:
 zip_safe = True
 include_package_data = True
```

### Comparing `text2story-1.4.6/text2story/__init__.py` & `text2story-1.4.7/text2story/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/labels.txt` & `text2story-1.4.7/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/labels.txt`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/config.json` & `text2story-1.4.7/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/config.json`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/linear_layer.pt` & `text2story-1.4.7/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/linear_layer.pt`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/annotators/ALLENNLP/PropBankBr.py` & `text2story-1.4.7/text2story/annotators/ALLENNLP/PropBankBr.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/annotators/ALLENNLP/__init__.py` & `text2story-1.4.7/text2story/annotators/ALLENNLP/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/annotators/ALLENNLP/allen_wrapper.py` & `text2story-1.4.7/text2story/annotators/ALLENNLP/allen_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -554,43 +554,43 @@
        span of that participant, the second elements is the POS tag, anf third
        element is the NER tag, if it is a entity
     """
     participant_lst = sorted(participant_lst, key=lambda x:x[0])
     tagged_participants = {}
 
     doc = pipeline[lang](text)
-
+    tagged_participants_lst = []
     for tok in doc:
         pos = bsearch_tuplelist(tok.idx, participant_lst)
 
         if pos != -1:
 
             # only update the tag value with the lexical head of the
             # participant
 
             if pos not in tagged_participants:
                 offset_participant = participant_lst[pos]
                 if tok.ent_type_ == '':
-                    tagged_participants[pos] = (offset_participant, tok.pos_, 'UNDEF')
+                    tagged_participants[pos] = (offset_participant, tok.pos_, 'Arg')
                 else:
                     tagged_participants[pos] = (offset_participant, tok.pos_,tok.ent_type_.lower().capitalize())
             else:
                 # if there is a token inside the text span that  has a NER tag, then replace the ner tag with more specific than UNDEF
                 offset_participant, pos_tag, ner_tag = tagged_participants[pos]
-                if ner_tag == 'UNDEF' and tok.ent_type_ != '':
+                if ner_tag == 'Arg' and tok.ent_type_ != '':
                     tagged_participants[pos] = (offset_participant, tok.pos_, tok.ent_type_.lower().capitalize())
+        else:
 
+            tagged_participants_lst.append(((tok.idx, tok.idx + len(tok.text)),tok.pos_,"UNDEF"))
 
-    tagged_participants_lst = []
     # it is possible that some participant was not found by the bsearch?
     for idx in range(len(participant_lst)):
-        if idx not in tagged_participants:
-            tagged_participants_lst.append((participant_lst[idx],"UNDEF","UNDEF"))
-        else:
-            tagged_participants_lst.append(tagged_participants[idx])
+        tagged_participants_lst.append(tagged_participants[idx])
+
+    tagged_participants_lst.sort(key=lambda x:x[0][0])
 
     return tagged_participants_lst
 
 def extract_participants(lang, text):
     """
     Main function that applies the SRL pipeline to extract participant entities from each sentence.
```

### Comparing `text2story-1.4.6/text2story/annotators/ALLENNLP/my_model.py` & `text2story-1.4.7/text2story/annotators/ALLENNLP/my_model.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/annotators/ALLENNLP/my_reader.py` & `text2story-1.4.7/text2story/annotators/ALLENNLP/my_reader.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/annotators/ALLENNLP/preprocess.py` & `text2story-1.4.7/text2story/annotators/ALLENNLP/preprocess.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/annotators/ALLENNLP/requirements.txt` & `text2story-1.4.7/text2story/annotators/ALLENNLP/requirements.txt`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/annotators/BERTNERPT/POS_tagger_brill.pkl` & `text2story-1.4.7/text2story/annotators/BERTNERPT/POS_tagger_brill.pkl`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/annotators/BERTNERPT/__init__.py` & `text2story-1.4.7/text2story/annotators/BERTNERPT/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/annotators/CUSTOMPT/__init__.py` & `text2story-1.4.7/text2story/annotators/CUSTOMPT/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/annotators/CUSTOMPT/crf_v2.1.joblib` & `text2story-1.4.7/text2story/annotators/CUSTOMPT/crf_v2.1.joblib`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/annotators/CUSTOMPT/event_model.py` & `text2story-1.4.7/text2story/annotators/CUSTOMPT/event_model.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/annotators/CUSTOMPT/feature_extractor.py` & `text2story-1.4.7/text2story/annotators/CUSTOMPT/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/annotators/DBPEDIA/__init__.py` & `text2story-1.4.7/text2story/annotators/DBPEDIA/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/annotators/NLTK/__init__.py` & `text2story-1.4.7/text2story/annotators/NLTK/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/annotators/PY_HEIDELTIME/__init__.py` & `text2story-1.4.7/text2story/annotators/PY_HEIDELTIME/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/annotators/SPACY/__init__.py` & `text2story-1.4.7/text2story/annotators/SPACY/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/annotators/SPARKNLP/__init__.py` & `text2story-1.4.7/text2story/annotators/SPARKNLP/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/annotators/SRL/__init__.py` & `text2story-1.4.7/text2story/annotators/SRL/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import transformers
 import pandas as pd
 import numpy as np
 
 import nltk
 from nltk.tokenize import sent_tokenize
 
+nltk.download('punkt')
+
 from itertools import zip_longest
 
 from text2story.core.utils import bsearch_tuplelist
 
 ### Global Variables ###
 
 SRL_TYPE_MAPPING = {
```

### Comparing `text2story-1.4.6/text2story/annotators/SRLWeakLabeling/__init__.py` & `text2story-1.4.7/text2story/annotators/SRLWeakLabeling/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/annotators/TEI2GO/__init__.py` & `text2story-1.4.7/text2story/annotators/TEI2GO/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/annotators/__init__.py` & `text2story-1.4.7/text2story/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/brat2viz/README.md` & `text2story-1.4.7/text2story/brat2viz/README.md`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/brat2viz/brat2drs/brat2drs.py` & `text2story-1.4.7/text2story/brat2viz/brat2drs/brat2drs.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/brat2viz/brat2drs/files_monitor.py` & `text2story-1.4.7/text2story/brat2viz/brat2drs/files_monitor.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/brat2viz/brat2json/brat2json.py` & `text2story-1.4.7/text2story/brat2viz/brat2json/brat2json.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/brat2viz/drs2viz/app.py` & `text2story-1.4.7/text2story/brat2viz/drs2viz/app.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/brat2viz/drs2viz/parser.py` & `text2story-1.4.7/text2story/brat2viz/drs2viz/parser.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/brat2viz/drs2viz/viz.py` & `text2story-1.4.7/text2story/brat2viz/drs2viz/viz.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/core/annotator.py` & `text2story-1.4.7/text2story/core/annotator.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/core/entity_structures.py` & `text2story-1.4.7/text2story/core/entity_structures.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/core/exceptions.py` & `text2story-1.4.7/text2story/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/core/graph_builder.py` & `text2story-1.4.7/text2story/core/graph_builder.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/core/link_structures.py` & `text2story-1.4.7/text2story/core/link_structures.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/core/narrative.py` & `text2story-1.4.7/text2story/core/narrative.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/core/utils.py` & `text2story-1.4.7/text2story/core/utils.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/experiments/compare_ann.py` & `text2story-1.4.7/text2story/experiments/compare_ann.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/experiments/cp_notlusa.py` & `text2story-1.4.7/text2story/experiments/cp_notlusa.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/experiments/evaluate_gpt.py` & `text2story-1.4.7/text2story/experiments/evaluate_gpt.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/experiments/evaluation.py` & `text2story-1.4.7/text2story/experiments/evaluation.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/experiments/exp_en_pb.json` & `text2story-1.4.7/text2story/experiments/exp_en_pb.json`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/experiments/metrics.py` & `text2story-1.4.7/text2story/experiments/metrics.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/experiments/run_experiments.py` & `text2story-1.4.7/text2story/experiments/run_experiments.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/experiments/stats.py` & `text2story-1.4.7/text2story/experiments/stats.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/readers/pb-vn2.json` & `text2story-1.4.7/text2story/readers/pb-vn2.json`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/readers/read.py` & `text2story-1.4.7/text2story/readers/read.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/readers/read_ace.py` & `text2story-1.4.7/text2story/readers/read_ace.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/readers/read_brat.py` & `text2story-1.4.7/text2story/readers/read_brat.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/readers/read_csv.py` & `text2story-1.4.7/text2story/readers/read_csv.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/readers/read_ecb.py` & `text2story-1.4.7/text2story/readers/read_ecb.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/readers/read_framenet.py` & `text2story-1.4.7/text2story/readers/read_framenet.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/readers/read_propbank.py` & `text2story-1.4.7/text2story/readers/read_propbank.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/readers/token_corpus.py` & `text2story-1.4.7/text2story/readers/token_corpus.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/readers/utils.py` & `text2story-1.4.7/text2story/readers/utils.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/select/bubble.py` & `text2story-1.4.7/text2story/select/bubble.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/select/event.py` & `text2story-1.4.7/text2story/select/event.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/text2viz/Text2Viz.py` & `text2story-1.4.7/text2story/text2viz/Text2Viz.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/text2viz/visualization.py` & `text2story-1.4.7/text2story/text2viz/visualization.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/training/participant_concept.py` & `text2story-1.4.7/text2story/training/participant_concept.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/viz/bubble_tikz.py` & `text2story-1.4.7/text2story/viz/bubble_tikz.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story/viz/msc.py` & `text2story-1.4.7/text2story/viz/msc.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.6/text2story.egg-info/PKG-INFO` & `text2story-1.4.7/text2story.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2story
-Version: 1.4.6
+Version: 1.4.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: joblib
 Requires-Dist: spacy
 Requires-Dist: py-heideltime
 Requires-Dist: importlib_metadata
 Requires-Dist: pandas<2.0.0
```

### Comparing `text2story-1.4.6/text2story.egg-info/SOURCES.txt` & `text2story-1.4.7/text2story.egg-info/SOURCES.txt`

 * *Files identical despite different names*
