# Comparing `tmp/text2story-1.4.5.tar.gz` & `tmp/text2story-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2story-1.4.5.tar", last modified: Mon May  6 10:05:49 2024, max compression
+gzip compressed data, was "text2story-1.4.6.tar", last modified: Mon May  6 11:06:21 2024, max compression
```

## Comparing `text2story-1.4.5.tar` & `text2story-1.4.6.tar`

### file list

```diff
@@ -1,120 +1,125 @@
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.613779 text2story-1.4.5/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    33470 2022-10-19 09:22:59.000000 text2story-1.4.5/LICENSE
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      559 2023-09-20 11:40:02.000000 text2story-1.4.5/MANIFEST.in
--rw-r--r--   0 evelinamorim  (1000) evelinamorim  (1000)    10904 2024-05-06 10:05:49.613779 text2story-1.4.5/PKG-INFO
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    10263 2023-12-13 15:05:29.000000 text2story-1.4.5/README.md
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      417 2024-05-06 10:00:42.000000 text2story-1.4.5/pyproject.toml
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      601 2024-05-06 10:05:49.617780 text2story-1.4.5/setup.cfg
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2023-09-11 13:50:06.000000 text2story-1.4.5/setup.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.577779 text2story-1.4.5/text2story/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      757 2022-10-19 09:12:42.000000 text2story-1.4.5/text2story/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       67 2022-10-19 09:12:42.000000 text2story-1.4.5/text2story/__main__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.577779 text2story-1.4.5/text2story/annotators/
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.581780 text2story-1.4.5/text2story/annotators/ALLENNLP/
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.573779 text2story-1.4.5/text2story/annotators/ALLENNLP/Models/
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.581780 text2story-1.4.5/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.585780 text2story-1.4.5/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      739 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/labels.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       14 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/non_padded_namespaces.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1343 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/config.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   265058 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/linear_layer.pt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    10386 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/annotators/ALLENNLP/PropBankBr.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6172 2023-11-08 10:19:59.000000 text2story-1.4.5/text2story/annotators/ALLENNLP/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    28375 2023-11-08 10:15:57.000000 text2story-1.4.5/text2story/annotators/ALLENNLP/allen_wrapper.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13691 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/annotators/ALLENNLP/my_model.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    20528 2023-09-20 15:37:16.000000 text2story-1.4.5/text2story/annotators/ALLENNLP/my_reader.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6217 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/annotators/ALLENNLP/preprocess.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9718 2024-05-02 10:55:09.000000 text2story-1.4.5/text2story/annotators/ALLENNLP/requirements.txt
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.589779 text2story-1.4.5/text2story/annotators/BERTNERPT/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)  2143882 2023-09-12 15:18:59.000000 text2story-1.4.5/text2story/annotators/BERTNERPT/POS_tagger_brill.pkl
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3160 2023-09-19 14:37:58.000000 text2story-1.4.5/text2story/annotators/BERTNERPT/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.593779 text2story-1.4.5/text2story/annotators/CUSTOMPT/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14794 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/annotators/CUSTOMPT/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   371646 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/annotators/CUSTOMPT/crf_v2.1.joblib
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    15093 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/annotators/CUSTOMPT/event_model.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13972 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/annotators/CUSTOMPT/feature_extractor.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.593779 text2story-1.4.5/text2story/annotators/NLTK/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2954 2023-09-13 10:57:45.000000 text2story-1.4.5/text2story/annotators/NLTK/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.593779 text2story-1.4.5/text2story/annotators/PY_HEIDELTIME/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1786 2023-10-11 13:29:55.000000 text2story-1.4.5/text2story/annotators/PY_HEIDELTIME/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.593779 text2story-1.4.5/text2story/annotators/SPACY/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1901 2023-09-21 09:23:20.000000 text2story-1.4.5/text2story/annotators/SPACY/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.593779 text2story-1.4.5/text2story/annotators/SPARKNLP/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9462 2022-10-26 12:28:21.000000 text2story-1.4.5/text2story/annotators/SPARKNLP/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.597780 text2story-1.4.5/text2story/annotators/SRLWeakLabeling/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3501 2023-09-11 13:50:06.000000 text2story-1.4.5/text2story/annotators/SRLWeakLabeling/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.597780 text2story-1.4.5/text2story/annotators/TEI2GO/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1623 2023-09-21 09:11:18.000000 text2story-1.4.5/text2story/annotators/TEI2GO/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     4557 2024-05-06 09:48:38.000000 text2story-1.4.5/text2story/annotators/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.597780 text2story-1.4.5/text2story/brat2viz/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      548 2022-10-19 09:12:42.000000 text2story-1.4.5/text2story/brat2viz/README.md
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2022-10-19 09:12:42.000000 text2story-1.4.5/text2story/brat2viz/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.597780 text2story-1.4.5/text2story/brat2viz/brat2drs/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       37 2022-10-19 09:12:42.000000 text2story-1.4.5/text2story/brat2viz/brat2drs/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    17359 2023-09-11 13:50:06.000000 text2story-1.4.5/text2story/brat2viz/brat2drs/brat2drs.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1059 2022-10-19 09:12:42.000000 text2story-1.4.5/text2story/brat2viz/brat2drs/files_monitor.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.597780 text2story-1.4.5/text2story/brat2viz/brat2json/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-10-24 13:54:25.000000 text2story-1.4.5/text2story/brat2viz/brat2json/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    45447 2023-10-24 14:47:12.000000 text2story-1.4.5/text2story/brat2viz/brat2json/brat2json.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.601780 text2story-1.4.5/text2story/brat2viz/drs2viz/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2022-10-19 09:12:42.000000 text2story-1.4.5/text2story/brat2viz/drs2viz/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2428 2022-10-19 09:12:42.000000 text2story-1.4.5/text2story/brat2viz/drs2viz/app.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13487 2022-10-19 09:12:42.000000 text2story-1.4.5/text2story/brat2viz/drs2viz/parser.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    10956 2023-09-13 14:10:19.000000 text2story-1.4.5/text2story/brat2viz/drs2viz/viz.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.601780 text2story-1.4.5/text2story/core/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-19 13:19:29.000000 text2story-1.4.5/text2story/core/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    12228 2024-05-02 10:54:43.000000 text2story-1.4.5/text2story/core/annotator.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3429 2023-10-09 14:49:24.000000 text2story-1.4.5/text2story/core/entity_structures.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1257 2024-05-02 10:54:43.000000 text2story-1.4.5/text2story/core/exceptions.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      546 2023-09-11 13:50:06.000000 text2story-1.4.5/text2story/core/graph_builder.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3343 2023-09-11 13:50:06.000000 text2story-1.4.5/text2story/core/link_structures.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    28477 2024-05-02 10:54:43.000000 text2story-1.4.5/text2story/core/narrative.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    11397 2023-10-06 10:45:23.000000 text2story-1.4.5/text2story/core/utils.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.605780 text2story-1.4.5/text2story/experiments/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-09-11 13:50:06.000000 text2story-1.4.5/text2story/experiments/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3918 2023-09-11 13:50:06.000000 text2story-1.4.5/text2story/experiments/compare_ann.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3713 2023-10-16 09:18:06.000000 text2story-1.4.5/text2story/experiments/cp_notlusa.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      882 2023-10-19 23:18:46.000000 text2story-1.4.5/text2story/experiments/evaluate_gpt.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    16957 2024-01-31 16:04:58.000000 text2story-1.4.5/text2story/experiments/evaluation.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      429 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/experiments/exp.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      205 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/experiments/exp_en_fn.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      601 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/experiments/exp_en_pb.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14493 2024-05-02 10:54:43.000000 text2story-1.4.5/text2story/experiments/metrics.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1453 2024-01-31 16:03:53.000000 text2story-1.4.5/text2story/experiments/run_experiments.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     8912 2024-01-16 16:40:49.000000 text2story-1.4.5/text2story/experiments/stats.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.609779 text2story-1.4.5/text2story/readers/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-09-11 13:50:06.000000 text2story-1.4.5/text2story/readers/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      380 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/readers/fn-lirics.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   312656 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/readers/pb-vn2.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      547 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/readers/read.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14407 2023-10-18 07:53:38.000000 text2story-1.4.5/text2story/readers/read_ace.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    26882 2024-05-02 10:54:43.000000 text2story-1.4.5/text2story/readers/read_brat.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    17011 2023-10-06 10:45:23.000000 text2story-1.4.5/text2story/readers/read_ecb.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6081 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/readers/read_framenet.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    11525 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/readers/read_propbank.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1639 2024-01-09 13:08:04.000000 text2story-1.4.5/text2story/readers/token_corpus.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1221 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/readers/utils.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      353 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/readers/vn-lirics.json
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.613779 text2story-1.4.5/text2story/select/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      121 2023-03-27 13:07:12.000000 text2story-1.4.5/text2story/select/README.md
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-09-11 13:50:06.000000 text2story-1.4.5/text2story/select/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    15112 2024-01-18 13:01:37.000000 text2story-1.4.5/text2story/select/bubble.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    10207 2024-01-23 10:09:52.000000 text2story-1.4.5/text2story/select/event.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.613779 text2story-1.4.5/text2story/text2viz/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     5371 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/text2viz/Text2Viz.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/text2viz/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      699 2022-10-13 08:54:40.000000 text2story-1.4.5/text2story/text2viz/visualization.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.613779 text2story-1.4.5/text2story/training/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-09-11 13:50:06.000000 text2story-1.4.5/text2story/training/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14422 2023-09-11 13:50:06.000000 text2story-1.4.5/text2story/training/participant_concept.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.613779 text2story-1.4.5/text2story/viz/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-09-11 13:50:06.000000 text2story-1.4.5/text2story/viz/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    15649 2024-01-18 11:52:24.000000 text2story-1.4.5/text2story/viz/bubble_tikz.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2710 2024-01-19 15:14:06.000000 text2story-1.4.5/text2story/viz/msc.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 10:05:49.613779 text2story-1.4.5/text2story.egg-info/
--rw-r--r--   0 evelinamorim  (1000) evelinamorim  (1000)    10904 2024-05-06 10:05:49.000000 text2story-1.4.5/text2story.egg-info/PKG-INFO
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3355 2024-05-06 10:05:49.000000 text2story-1.4.5/text2story.egg-info/SOURCES.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2024-05-06 10:05:49.000000 text2story-1.4.5/text2story.egg-info/dependency_links.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      224 2024-05-06 10:05:49.000000 text2story-1.4.5/text2story.egg-info/requires.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       11 2024-05-06 10:05:49.000000 text2story-1.4.5/text2story.egg-info/top_level.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-05-26 15:56:54.000000 text2story-1.4.5/text2story.egg-info/zip-safe
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.475712 text2story-1.4.6/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    33470 2022-10-19 09:22:59.000000 text2story-1.4.6/LICENSE
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      559 2023-09-20 11:40:02.000000 text2story-1.4.6/MANIFEST.in
+-rw-r--r--   0 evelinamorim  (1000) evelinamorim  (1000)    10904 2024-05-06 11:06:21.475712 text2story-1.4.6/PKG-INFO
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    10263 2023-12-13 15:05:29.000000 text2story-1.4.6/README.md
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      417 2024-05-06 11:01:40.000000 text2story-1.4.6/pyproject.toml
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      601 2024-05-06 11:06:21.475712 text2story-1.4.6/setup.cfg
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2023-09-11 13:50:06.000000 text2story-1.4.6/setup.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.451712 text2story-1.4.6/text2story/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      757 2022-10-19 09:12:42.000000 text2story-1.4.6/text2story/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       67 2022-10-19 09:12:42.000000 text2story-1.4.6/text2story/__main__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.451712 text2story-1.4.6/text2story/annotators/
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.451712 text2story-1.4.6/text2story/annotators/ALLENNLP/
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.447712 text2story-1.4.6/text2story/annotators/ALLENNLP/Models/
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.451712 text2story-1.4.6/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.455712 text2story-1.4.6/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      739 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/labels.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       14 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/non_padded_namespaces.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1343 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/config.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   265058 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/linear_layer.pt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    10386 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/annotators/ALLENNLP/PropBankBr.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6172 2023-11-08 10:19:59.000000 text2story-1.4.6/text2story/annotators/ALLENNLP/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    28375 2023-11-08 10:15:57.000000 text2story-1.4.6/text2story/annotators/ALLENNLP/allen_wrapper.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13691 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/annotators/ALLENNLP/my_model.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    20528 2023-09-20 15:37:16.000000 text2story-1.4.6/text2story/annotators/ALLENNLP/my_reader.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6217 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/annotators/ALLENNLP/preprocess.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9718 2024-05-06 11:03:00.000000 text2story-1.4.6/text2story/annotators/ALLENNLP/requirements.txt
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.459712 text2story-1.4.6/text2story/annotators/BERTNERPT/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)  2143882 2023-09-12 15:18:59.000000 text2story-1.4.6/text2story/annotators/BERTNERPT/POS_tagger_brill.pkl
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3160 2023-09-19 14:37:58.000000 text2story-1.4.6/text2story/annotators/BERTNERPT/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.459712 text2story-1.4.6/text2story/annotators/CUSTOMPT/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14794 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/annotators/CUSTOMPT/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   371646 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/annotators/CUSTOMPT/crf_v2.1.joblib
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    15093 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/annotators/CUSTOMPT/event_model.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13972 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/annotators/CUSTOMPT/feature_extractor.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.459712 text2story-1.4.6/text2story/annotators/DBPEDIA/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3178 2024-05-06 11:02:12.000000 text2story-1.4.6/text2story/annotators/DBPEDIA/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.459712 text2story-1.4.6/text2story/annotators/NLTK/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2954 2023-09-13 10:57:45.000000 text2story-1.4.6/text2story/annotators/NLTK/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.459712 text2story-1.4.6/text2story/annotators/PY_HEIDELTIME/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1786 2023-10-11 13:29:55.000000 text2story-1.4.6/text2story/annotators/PY_HEIDELTIME/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.459712 text2story-1.4.6/text2story/annotators/SPACY/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1901 2023-09-21 09:23:20.000000 text2story-1.4.6/text2story/annotators/SPACY/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.463712 text2story-1.4.6/text2story/annotators/SPARKNLP/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9462 2022-10-26 12:28:21.000000 text2story-1.4.6/text2story/annotators/SPARKNLP/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.463712 text2story-1.4.6/text2story/annotators/SRL/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    19653 2024-05-06 11:02:12.000000 text2story-1.4.6/text2story/annotators/SRL/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.463712 text2story-1.4.6/text2story/annotators/SRLWeakLabeling/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3501 2023-09-11 13:50:06.000000 text2story-1.4.6/text2story/annotators/SRLWeakLabeling/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.463712 text2story-1.4.6/text2story/annotators/TEI2GO/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1623 2023-09-21 09:11:18.000000 text2story-1.4.6/text2story/annotators/TEI2GO/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     5372 2024-05-06 11:05:42.000000 text2story-1.4.6/text2story/annotators/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.463712 text2story-1.4.6/text2story/brat2viz/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      548 2022-10-19 09:12:42.000000 text2story-1.4.6/text2story/brat2viz/README.md
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2022-10-19 09:12:42.000000 text2story-1.4.6/text2story/brat2viz/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.463712 text2story-1.4.6/text2story/brat2viz/brat2drs/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       37 2022-10-19 09:12:42.000000 text2story-1.4.6/text2story/brat2viz/brat2drs/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    17359 2023-09-11 13:50:06.000000 text2story-1.4.6/text2story/brat2viz/brat2drs/brat2drs.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1059 2022-10-19 09:12:42.000000 text2story-1.4.6/text2story/brat2viz/brat2drs/files_monitor.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.463712 text2story-1.4.6/text2story/brat2viz/brat2json/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-10-24 13:54:25.000000 text2story-1.4.6/text2story/brat2viz/brat2json/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    45447 2023-10-24 14:47:12.000000 text2story-1.4.6/text2story/brat2viz/brat2json/brat2json.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.463712 text2story-1.4.6/text2story/brat2viz/drs2viz/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2022-10-19 09:12:42.000000 text2story-1.4.6/text2story/brat2viz/drs2viz/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2428 2022-10-19 09:12:42.000000 text2story-1.4.6/text2story/brat2viz/drs2viz/app.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13487 2022-10-19 09:12:42.000000 text2story-1.4.6/text2story/brat2viz/drs2viz/parser.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    10956 2023-09-13 14:10:19.000000 text2story-1.4.6/text2story/brat2viz/drs2viz/viz.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.467712 text2story-1.4.6/text2story/core/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-19 13:19:29.000000 text2story-1.4.6/text2story/core/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    12476 2024-05-06 11:02:12.000000 text2story-1.4.6/text2story/core/annotator.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3429 2023-10-09 14:49:24.000000 text2story-1.4.6/text2story/core/entity_structures.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1472 2024-05-06 11:02:12.000000 text2story-1.4.6/text2story/core/exceptions.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      546 2023-09-11 13:50:06.000000 text2story-1.4.6/text2story/core/graph_builder.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3343 2023-09-11 13:50:06.000000 text2story-1.4.6/text2story/core/link_structures.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    28491 2024-05-06 11:02:12.000000 text2story-1.4.6/text2story/core/narrative.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    11397 2023-10-06 10:45:23.000000 text2story-1.4.6/text2story/core/utils.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.467712 text2story-1.4.6/text2story/experiments/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-09-11 13:50:06.000000 text2story-1.4.6/text2story/experiments/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3918 2023-09-11 13:50:06.000000 text2story-1.4.6/text2story/experiments/compare_ann.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3713 2023-10-16 09:18:06.000000 text2story-1.4.6/text2story/experiments/cp_notlusa.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      882 2023-10-19 23:18:46.000000 text2story-1.4.6/text2story/experiments/evaluate_gpt.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    16957 2024-01-31 16:04:58.000000 text2story-1.4.6/text2story/experiments/evaluation.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      429 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/experiments/exp.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      205 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/experiments/exp_en_fn.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      601 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/experiments/exp_en_pb.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    17812 2024-05-06 11:02:12.000000 text2story-1.4.6/text2story/experiments/metrics.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1453 2024-01-31 16:03:53.000000 text2story-1.4.6/text2story/experiments/run_experiments.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     8912 2024-01-16 16:40:49.000000 text2story-1.4.6/text2story/experiments/stats.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.471712 text2story-1.4.6/text2story/readers/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-09-11 13:50:06.000000 text2story-1.4.6/text2story/readers/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      380 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/readers/fn-lirics.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   312656 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/readers/pb-vn2.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      547 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/readers/read.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14407 2023-10-18 07:53:38.000000 text2story-1.4.6/text2story/readers/read_ace.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    27190 2024-05-06 11:02:12.000000 text2story-1.4.6/text2story/readers/read_brat.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1799 2024-05-06 11:02:12.000000 text2story-1.4.6/text2story/readers/read_csv.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    17011 2023-10-06 10:45:23.000000 text2story-1.4.6/text2story/readers/read_ecb.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6081 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/readers/read_framenet.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    11525 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/readers/read_propbank.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1639 2024-01-09 13:08:04.000000 text2story-1.4.6/text2story/readers/token_corpus.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1221 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/readers/utils.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      353 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/readers/vn-lirics.json
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.475712 text2story-1.4.6/text2story/select/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      121 2023-03-27 13:07:12.000000 text2story-1.4.6/text2story/select/README.md
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-09-11 13:50:06.000000 text2story-1.4.6/text2story/select/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    15112 2024-01-18 13:01:37.000000 text2story-1.4.6/text2story/select/bubble.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    10207 2024-01-23 10:09:52.000000 text2story-1.4.6/text2story/select/event.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.475712 text2story-1.4.6/text2story/text2viz/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     5371 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/text2viz/Text2Viz.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/text2viz/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      699 2022-10-13 08:54:40.000000 text2story-1.4.6/text2story/text2viz/visualization.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.475712 text2story-1.4.6/text2story/training/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-09-11 13:50:06.000000 text2story-1.4.6/text2story/training/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14422 2023-09-11 13:50:06.000000 text2story-1.4.6/text2story/training/participant_concept.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.475712 text2story-1.4.6/text2story/viz/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-09-11 13:50:06.000000 text2story-1.4.6/text2story/viz/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    15649 2024-01-18 11:52:24.000000 text2story-1.4.6/text2story/viz/bubble_tikz.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2710 2024-01-19 15:14:06.000000 text2story-1.4.6/text2story/viz/msc.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2024-05-06 11:06:21.475712 text2story-1.4.6/text2story.egg-info/
+-rw-r--r--   0 evelinamorim  (1000) evelinamorim  (1000)    10904 2024-05-06 11:06:21.000000 text2story-1.4.6/text2story.egg-info/PKG-INFO
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3466 2024-05-06 11:06:21.000000 text2story-1.4.6/text2story.egg-info/SOURCES.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2024-05-06 11:06:21.000000 text2story-1.4.6/text2story.egg-info/dependency_links.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      224 2024-05-06 11:06:21.000000 text2story-1.4.6/text2story.egg-info/requires.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       11 2024-05-06 11:06:21.000000 text2story-1.4.6/text2story.egg-info/top_level.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-05-26 15:56:54.000000 text2story-1.4.6/text2story.egg-info/zip-safe
```

### Comparing `text2story-1.4.5/LICENSE` & `text2story-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/MANIFEST.in` & `text2story-1.4.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/PKG-INFO` & `text2story-1.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2story
-Version: 1.4.5
+Version: 1.4.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: joblib
 Requires-Dist: spacy
 Requires-Dist: py-heideltime
 Requires-Dist: importlib_metadata
 Requires-Dist: pandas<2.0.0
```

### Comparing `text2story-1.4.5/README.md` & `text2story-1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/setup.cfg` & `text2story-1.4.6/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 description-file = README.md
 name = text2story
-version = 1.4.5
+version = 1.4.6
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
 packages = find:
 zip_safe = True
 include_package_data = True
```

### Comparing `text2story-1.4.5/text2story/__init__.py` & `text2story-1.4.6/text2story/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/labels.txt` & `text2story-1.4.6/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/labels.txt`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/config.json` & `text2story-1.4.6/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/config.json`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/linear_layer.pt` & `text2story-1.4.6/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/linear_layer.pt`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/annotators/ALLENNLP/PropBankBr.py` & `text2story-1.4.6/text2story/annotators/ALLENNLP/PropBankBr.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/annotators/ALLENNLP/__init__.py` & `text2story-1.4.6/text2story/annotators/ALLENNLP/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/annotators/ALLENNLP/allen_wrapper.py` & `text2story-1.4.6/text2story/annotators/ALLENNLP/allen_wrapper.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/annotators/ALLENNLP/my_model.py` & `text2story-1.4.6/text2story/annotators/ALLENNLP/my_model.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/annotators/ALLENNLP/my_reader.py` & `text2story-1.4.6/text2story/annotators/ALLENNLP/my_reader.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/annotators/ALLENNLP/preprocess.py` & `text2story-1.4.6/text2story/annotators/ALLENNLP/preprocess.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/annotators/ALLENNLP/requirements.txt` & `text2story-1.4.6/text2story/annotators/ALLENNLP/requirements.txt`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/annotators/BERTNERPT/POS_tagger_brill.pkl` & `text2story-1.4.6/text2story/annotators/BERTNERPT/POS_tagger_brill.pkl`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/annotators/BERTNERPT/__init__.py` & `text2story-1.4.6/text2story/annotators/BERTNERPT/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/annotators/CUSTOMPT/__init__.py` & `text2story-1.4.6/text2story/annotators/CUSTOMPT/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/annotators/CUSTOMPT/crf_v2.1.joblib` & `text2story-1.4.6/text2story/annotators/CUSTOMPT/crf_v2.1.joblib`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/annotators/CUSTOMPT/event_model.py` & `text2story-1.4.6/text2story/annotators/CUSTOMPT/event_model.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/annotators/CUSTOMPT/feature_extractor.py` & `text2story-1.4.6/text2story/annotators/CUSTOMPT/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/annotators/NLTK/__init__.py` & `text2story-1.4.6/text2story/annotators/NLTK/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/annotators/PY_HEIDELTIME/__init__.py` & `text2story-1.4.6/text2story/annotators/PY_HEIDELTIME/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/annotators/SPACY/__init__.py` & `text2story-1.4.6/text2story/annotators/SPACY/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/annotators/SPARKNLP/__init__.py` & `text2story-1.4.6/text2story/annotators/SPARKNLP/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/annotators/SRLWeakLabeling/__init__.py` & `text2story-1.4.6/text2story/annotators/SRLWeakLabeling/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/annotators/TEI2GO/__init__.py` & `text2story-1.4.6/text2story/annotators/TEI2GO/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/annotators/__init__.py` & `text2story-1.4.6/text2story/annotators/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import sys
 import os
 from pathlib import Path
 
 sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
 
-from core.exceptions import InvalidTool
+from text2story.core.exceptions import InvalidTool
 
 
 from collections import ChainMap
 
 sys.path.insert(0, Path(__file__).parent)
 
-PARTICIPANT_EXTRACTION_TOOLS = {'spacy':['pt','en'], 'nltk':['en'], 'allennlp':["pt","en"],'bertnerpt':["pt"]}
+PARTICIPANT_EXTRACTION_TOOLS = {'spacy':['pt','en'], 'nltk':['en'], 'allennlp':['en'],'bertnerpt':['pt'], 'dbpedia':['pt','en'],'srl':['pt']}
 TIME_EXTRACTION_TOOLS = {'py_heideltime':['pt','en'], 'tei2go':['pt','en','it','de','es','fr']}
-EVENT_EXTRACTION_TOOLS = {'allennlp':['pt','en']}
-OBJECTAL_LINKS_RESOLUTION_TOOLS = {'allennlp':['pt','en']}
-SEMANTIC_ROLE_LABELLING_TOOLS = {'allennlp':['pt','en']}
+EVENT_EXTRACTION_TOOLS = {'allennlp':['en'],"srl":["pt"]}
+OBJECTAL_LINKS_RESOLUTION_TOOLS = {'allennlp':['en']}
+SEMANTIC_ROLE_LABELLING_TOOLS = {'allennlp':['en'],"srl":["pt"]}
 
 def get_tools():
     return dict(ChainMap(PARTICIPANT_EXTRACTION_TOOLS, TIME_EXTRACTION_TOOLS, \
              EVENT_EXTRACTION_TOOLS, OBJECTAL_LINKS_RESOLUTION_TOOLS, \
                          SEMANTIC_ROLE_LABELLING_TOOLS))
 
 def load(lang, tools=None):
@@ -53,14 +53,20 @@
         ALLENNLP.load(lang)
     if lang in tools["bertnerpt"] and "bertnerpt" in tools:
         from text2story.annotators import BERTNERPT
         BERTNERPT.load(lang)
     if lang in tools["tei2go"]  and "tei2go" in tools:
         from text2story.annotators import TEI2GO
         TEI2GO.load(lang)
+    if lang in tools["dbpedia"]  and "dbpedia" in tools:
+        from text2story.annotators import DBPEDIA
+        DBPEDIA.load(lang)
+    if lang in tools["srl"]  and "srl" in tools:
+        from text2story.annotators import SRL
+        SRL.load(lang)
 
 def get_available_tools():
     return PARTICIPANT_EXTRACTION_TOOLS.keys()+\
             TIME_EXTRACTION_TOOLS.keys()+\
             EVENT_EXTRACTION_TOOLS.keys()+\
             OBJECTAL_LINKS_RESOLUTION_TOOLS.keys()+\
             SEMANTIC_ROLE_LABELLING_TOOLS.keys()
@@ -73,28 +79,34 @@
 
 def get_event_tools():
     return EVENT_EXTRACTION_TOOLS
 
 def get_srlink_tools():
     return SEMANTIC_ROLE_LABELLING_TOOLS
 
-def extract_participants(tool, lang, text):
+def extract_participants(tool, lang, text, url=None):
 
     if tool == 'spacy':
         from text2story.annotators import SPACY
         return SPACY.extract_participants(lang, text)
     elif tool == 'nltk' and lang == "en":
         from text2story.annotators import NLTK
         return NLTK.extract_participants(lang, text)
     elif tool == 'allennlp':
         from text2story.annotators import ALLENNLP
         return ALLENNLP.extract_participants(lang, text)
     elif tool == 'bertnerpt':
         from text2story.annotators import BERTNERPT
         return BERTNERPT.extract_participants(lang, text)
+    elif tool == 'dbpedia':
+        from text2story.annotators import DBPEDIA
+        return DBPEDIA.extract_participants(text, lang, url)
+    if tool == 'srl':
+        from text2story.annotators import SRL
+        return SRL.extract_participants(lang, text)
     else:
         raise InvalidTool
 
 
 def extract_times(tool, lang, text, publication_time):
     if tool == 'py_heideltime':
         from text2story.annotators import PY_HEIDELTIME
@@ -118,17 +130,23 @@
 def extract_events(tool, lang, text):
     if tool == 'allennlp':
         from text2story.annotators import ALLENNLP
         return ALLENNLP.extract_events(lang, text)
     if tool == 'custompt':
         from text2story.annotators import CUSTOMPT
         return CUSTOMPT.extract_events(lang, text)
+    if tool == 'srl':
+        from text2story.annotators import SRL
+        return SRL.extract_events(lang, text)
 
     raise InvalidTool
 
 
 def extract_semantic_role_links(tool, lang, text):
     if tool == 'allennlp':
         from text2story.annotators import ALLENNLP
         return ALLENNLP.extract_semantic_role_links(lang, text)
+    if tool == 'srl':
+        from text2story.annotators import SRL
+        return SRL.extract_semantic_role_links(lang, text)
 
     raise InvalidTool
```

### Comparing `text2story-1.4.5/text2story/brat2viz/README.md` & `text2story-1.4.6/text2story/brat2viz/README.md`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/brat2viz/brat2drs/brat2drs.py` & `text2story-1.4.6/text2story/brat2viz/brat2drs/brat2drs.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/brat2viz/brat2drs/files_monitor.py` & `text2story-1.4.6/text2story/brat2viz/brat2drs/files_monitor.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/brat2viz/brat2json/brat2json.py` & `text2story-1.4.6/text2story/brat2viz/brat2json/brat2json.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/brat2viz/drs2viz/app.py` & `text2story-1.4.6/text2story/brat2viz/drs2viz/app.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/brat2viz/drs2viz/parser.py` & `text2story-1.4.6/text2story/brat2viz/drs2viz/parser.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/brat2viz/drs2viz/viz.py` & `text2story-1.4.6/text2story/brat2viz/drs2viz/viz.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/core/annotator.py` & `text2story-1.4.6/text2story/core/annotator.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         tools : list[str]
             the list of the annotators to be used; can be used any combination of them
             possible annotators are: 'spacy', 'nltk' and 'sparknlp'
         """
         self.tools = tools
 
 
-    def extract_participants(self, lang, text):
+    def extract_participants(self, lang, text, url=None):
         """
         Parameters
         ----------
         lang : str
             the language of the text
             current supported languages are: portuguese ('pt'); english ('en')
         text : str
@@ -77,21 +77,25 @@
         # For the NE IOB tag, we do the same, but we favor all labels versus the generic 'Other' label. That is, even if the label 'Other' is the most common, if we have a more specific one, we use that, instead.
 
         nr_tools = len(self.tools)
 
         # If no tool specified, use all
         if nr_tools == 0:
             self.tools = PARTICIPANT_EXTRACTION_TOOLS.keys()
+
             nr_tools = len(self.tools)
 
         # Gather the annotations made by the tools specified and combine the results
         annotations = []
         idxs = []
         for tool in self.tools:
-            annotations.append(extract_participants(tool, lang, text))
+            if url is not None:
+                annotations.append(extract_participants(tool, lang, text, url))
+            else:
+                annotations.append(extract_participants(tool, lang, text))
 
         final_annotation = []
 
         idxs = [0] * nr_tools # Current actor position from each tool
 
 
         while not(all([len(annotations[i]) == idxs[i] for i in range(nr_tools)])): # We finish when we consumed every actor identified by every tool
@@ -156,23 +160,24 @@
             rmv_undef_pos_tags = [ne for ne in actor_lexical_heads if ne != 'UNDEF']
             if rmv_undef_pos_tags:
                 actor_lexical_head = max(rmv_undef_pos_tags, key=rmv_undef_pos_tags.count)
             else:
                 continue # Discard the actor if it's lexical head isn't a 'Noun' or 'Pronoun'
 
             # For the NE, we also favor specifics NEs, in this case all labels versus the NE 'OTHER' and we take the most common.
-            rmv_other_ne = [ne for ne in actor_types if ne != 'Other']
+            rmv_other_ne = [ne for ne in actor_types if ne != 'Other' or ne != 'Arg']
             if rmv_other_ne:
                 actor_type = max(rmv_other_ne, key=rmv_other_ne.count)
             else:
                 actor_type = 'Other'
 
             # Discard entities with types other than 'Per', 'Org', 'Loc', 'Obj', 'Nat' & 'Other'.
+            # if it is Agr, it was an argument of an semantic role labeling event
             # Used, typically, to eliminate dates and durations incorrectly identified as an actor.
-            if actor_type in ['Per', 'Org', 'Loc', 'Obj', 'Nat', 'Other']:
+            if actor_type in ['Arg','Per', 'Org', 'Loc', 'Obj', 'Nat', 'Other']:
                 final_annotation.append(((actor_start_character_offset, actor_end_character_offset), actor_lexical_head, actor_type))
 
         return final_annotation
 
     def extract_times(self, lang, text, publication_time):
         """
         Parameters
```

### Comparing `text2story-1.4.5/text2story/core/entity_structures.py` & `text2story-1.4.6/text2story/core/entity_structures.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/core/exceptions.py` & `text2story-1.4.6/text2story/core/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,25 @@
 """
 	text2story.core.exceptions
 
 	All defined exceptions raised by the package.
 """
 
+
+class NoConnection(Exception):
+	"""
+	Raised if the user specified an invalid/unsupported language.
+	"""
+
+	def __init__(self):
+		description = ('No internet Connection detected.')
+
+		super().__init__(description)
+
+
 class InvalidLanguage(Exception):
 	"""
 	Raised if the user specified an invalid/unsupported language.
 	"""
 	def __init__(self, lang):
 		description = ('Invalid language :' + lang)
```

### Comparing `text2story-1.4.5/text2story/core/graph_builder.py` & `text2story-1.4.6/text2story/core/graph_builder.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/core/link_structures.py` & `text2story-1.4.6/text2story/core/link_structures.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/core/narrative.py` & `text2story-1.4.6/text2story/core/narrative.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,28 +235,28 @@
         narrativeSelf.participants = cls.participants
         narrativeSelf.events = cls.events
         narrativeSelf.times = cls.times
         narrativeSelf.spatial_relations = cls.spatial_relations
         narrativeSelf.links = cls.links
         return narrativeSelf
 
-    def extract_participants(self, *tools):
+    def extract_participants(self, *tools, url=None):
         """
         Parameters
         ----------
         tools : str, ...
                 the tools to be used in the annotation
 
         Returns
         -------
                 self.participants updated
         """
 
         participants = Annotator(tools).extract_participants(self.lang,
-                                                 self.text)  # annotations :: [(EntityStartOffset, EntityEndOffset, EntityPOSTag, EntityType)]
+                                                 self.text,url)  # annotations :: [(EntityStartOffset, EntityEndOffset, EntityPOSTag, EntityType)]
 
         for participant in participants:
             self.participants['T' + str(self._id)] = ParticipantEntity(self.text[participant[0][0]:participant[0][1]], participant[0], participant[1],
                                                            participant[2])
             self._id += 1
 
         return self.participants
```

### Comparing `text2story-1.4.5/text2story/core/utils.py` & `text2story-1.4.6/text2story/core/utils.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/experiments/compare_ann.py` & `text2story-1.4.6/text2story/experiments/compare_ann.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/experiments/cp_notlusa.py` & `text2story-1.4.6/text2story/experiments/cp_notlusa.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/experiments/evaluate_gpt.py` & `text2story-1.4.6/text2story/experiments/evaluate_gpt.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/experiments/evaluation.py` & `text2story-1.4.6/text2story/experiments/evaluation.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/experiments/exp_en_pb.json` & `text2story-1.4.6/text2story/experiments/exp_en_pb.json`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/experiments/metrics.py` & `text2story-1.4.6/text2story/experiments/metrics.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from collections import Counter
 
+import nltk
+from sklearn.metrics import cohen_kappa_score
 
 
 def partial_match(b1, e1, b2, e2):
     """
     Check if the interval (b1,e1) intersects
     with the interval (b2, e2)
 
@@ -456,9 +458,92 @@
              else:
                  search_target[id_srlink] = None
         else:
             search_target[id_srlink] = None
 
     return search_pred, search_target
 
+def compute_bleu_lines(data_lines1, data_lines2):
+
+    text_span_map = {}
+
+    for d1 in data_lines1:
+        t1 = nltk.word_tokenize(d1['text_span'])
+        span_id1 = d1['span_id']
+
+        for d2 in data_lines2:
+
+            t2 = nltk.word_tokenize(d2['text_span'])
+
+            bleu_score = nltk.translate.bleu([t1], t2, (1,))
+            if span_id1 in text_span_map:
+                maxb, span_id2 = text_span_map[span_id1]
+                if maxb < bleu_score:
+                    text_span_map[span_id1] = (bleu_score, d2['span_id'])
+            else:
+                 text_span_map[span_id1] = (bleu_score, d2['span_id'])
+
+    for span_id1 in text_span_map:
+        bleu, _ = text_span_map[span_id1]
+        if bleu < 0.8:
+            text_span_map[span_id1] = (0, None)
+    return text_span_map
+
+def compute_iaa_link(match_pred, reader1, reader2, link_type):
+
+    all_entities_pairs = []
+    for element_id_a in match_pred:
+        for element_id_b in match_pred:
+            all_entities_pairs.append((element_id_a, element_id_b))
+
+    links_lst = []
+    links_type_lst = []
+    for (element_id_a, element_id_b) in all_entities_pairs:
+        # check if annotator1 annotated some relation between event_a and event_b
+        relation1 = reader1.get_relation(element_id_a, element_id_b)
+        element_id_a_2 = match_pred[element_id_a]
+        element_id_b_2 = match_pred[element_id_b]
+
+        relation2 = reader2.get_relation(element_id_a_2, element_id_b_2)
+
+        if relation1 == None and relation2 == None:
+            links_lst.append(("none", "none"))
+            links_type_lst.append(("none", "none"))
+        else:
+            if relation1 == None:
+                if relation2.startswith(link_type):
+                    links_lst.append(("none", link_type.lower()))
+                    links_type_lst.append(("none", relation2))
+                else:
+                    links_lst.append(("none", "other"))
+                    links_type_lst.append(("none", "other"))
+            else:
+                if relation2 == None:
+                    if relation1.startswith(link_type):
+                        links_lst.append((link_type.lower(), "none"))
+                        links_type_lst.append((relation1, "none"))
+                    else:
+                        links_lst.append(("other", "none"))
+                        links_type_lst.append(("other", "none"))
+                else:
+                    if relation1.startswith(link_type) and relation2.startswith(link_type):
+                        links_lst.append((link_type.lower(), link_type.lower()))
+                        links_type_lst.append((relation1, relation2))
+                    else:
+                        links_lst.append(("other", "other"))
+                        links_type_lst.append(("other", "other"))
+
+    link_annotations1 = [link[0] for link in links_lst]
+    link_annotations2 = [link[1] for link in links_lst]
+
+    link_kappa = cohen_kappa_score(link_annotations1, link_annotations2)
+
+    link_type_annotations1 = [link[0] for link in links_type_lst]
+    link_type_annotations2 = [link[1] for link in links_type_lst]
+
+    link_type_kappa = cohen_kappa_score(link_type_annotations1, link_type_annotations2)
+
+    return link_kappa, link_type_kappa
+
+
```

### Comparing `text2story-1.4.5/text2story/experiments/run_experiments.py` & `text2story-1.4.6/text2story/experiments/run_experiments.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/experiments/stats.py` & `text2story-1.4.6/text2story/experiments/stats.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/readers/pb-vn2.json` & `text2story-1.4.6/text2story/readers/pb-vn2.json`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/readers/read.py` & `text2story-1.4.6/text2story/readers/read.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/readers/read_ace.py` & `text2story-1.4.6/text2story/readers/read_ace.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/readers/read_brat.py` & `text2story-1.4.6/text2story/readers/read_brat.py`

 * *Files 1% similar despite different names*

```diff
@@ -285,15 +285,15 @@
 
         @param string: path of data to gather and process
 
         @return dictionary: a dictionary of annotations
         """
 
         ann = {"Event": [], "Actor": [], "Time": [], "TIME_X3": [], \
-                "ACTOR": [], "Participant": [],"SRLINK":[]}
+                "ACTOR": [], "Participant": [],"SRLINK":[],"OLINK":[],"TLINK":[]}
 
         with open(file_ann, "r") as fd:
             last_line_type = None
             for line in fd:
                 ann_type = None
                 if line[0] != '#':
 
@@ -346,16 +346,18 @@
 
                             ann[ann_type].append({"id":line_toks[0],"offset1": (offset1_start, offset1_end), \
                                               "value": value})
                     elif line[0] == 'R':
                         e1 = line_toks[2].split(":")[1]  # entity 1
                         e2 = line_toks[3].split(":")[1]  # entity 2
                         rel_id = line_toks[0]
-                        if ann_type.startswith("SEMROLE") or ann_type.startswith("SRLINK"):
-                            ann["SRLINK"].append({"id":rel_id,"args":(e1, e2)})
+                        if ann_type in ann:
+                            ann[ann_type].append({"id":rel_id,"args":(e1, e2)})
+                        else:
+                            ann[ann_type] = [{"id": rel_id, "args": (e1, e2)}]
 
 
                         if ann_type in self.ann_ref:
                             if e1 in self.ann_ref[ann_type]:
                                 self.ann_ref[ann_type][e1].append(e2)
                             else:
                                 self.ann_ref[ann_type][e1] = [e2]
@@ -396,14 +398,15 @@
                 split_lst = fd.readlines()
                 split_lst = [line.replace("\n","") for line in split_lst]
 
         data_tokens = []
 
         for dirpath, dirnames, filenames in os.walk(data_dir):
             for f in filenames:
+
                 if f.endswith(".ann"):
 
                     p = Path(f)
                     if split_lst != [] and not(p.stem + ".txt" in split_lst):
                         continue
                  
                     fullname = os.path.join(data_dir, p.stem)
@@ -465,14 +468,15 @@
 
 
             ans = self.search_all_idx(tok.idx, ann_idx)
 
             # TODO: it is necessary perform a more efficient search
             # a possible subtoken annotation
             # perform more than one search, and build a list of id's
+
             ans_sub = self.search_subtoken(tok.idx, tok.idx + len(tok.text), \
                         ann_idx)
 
             ans = ans.union(ans_sub)
 
             if len(ans) != 0:
                 # annotations in token
@@ -646,16 +650,19 @@
 
                 for ref  in mytok.id_ann:
 
                     if ref in ann_rel: # if the current token has any relation, then...
 
                         # the relation for the reference ref
                         for rel_id, rel_type, ref_arg,argn in ann_rel[ref]:
-                            rel_obj = token_corpus.TokenRelation(rel_id, ref2tok[ref_arg], rel_type, argn, ref_arg)
-                            mytok.relations.append(rel_obj)
+                            try:
+                                rel_obj = token_corpus.TokenRelation(rel_id, ref2tok[ref_arg], rel_type, argn, ref_arg)
+                                mytok.relations.append(rel_obj)
+                            except KeyError:
+                                print(f"Warning: The {rel_id} was not included in the doc since {ref_arg} was not found as annotation.")
 
         return token_lst
 
     def search_all_idx(self, idx, idx_lst):
         """
         Since a token can be annotated with multiple id's, it is necessary 
         to perform multiple search for each one of these id's.
```

### Comparing `text2story-1.4.5/text2story/readers/read_ecb.py` & `text2story-1.4.6/text2story/readers/read_ecb.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/readers/read_framenet.py` & `text2story-1.4.6/text2story/readers/read_framenet.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/readers/read_propbank.py` & `text2story-1.4.6/text2story/readers/read_propbank.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/readers/token_corpus.py` & `text2story-1.4.6/text2story/readers/token_corpus.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/readers/utils.py` & `text2story-1.4.6/text2story/readers/utils.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/select/bubble.py` & `text2story-1.4.6/text2story/select/bubble.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/select/event.py` & `text2story-1.4.6/text2story/select/event.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/text2viz/Text2Viz.py` & `text2story-1.4.6/text2story/text2viz/Text2Viz.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/text2viz/visualization.py` & `text2story-1.4.6/text2story/text2viz/visualization.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/training/participant_concept.py` & `text2story-1.4.6/text2story/training/participant_concept.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/viz/bubble_tikz.py` & `text2story-1.4.6/text2story/viz/bubble_tikz.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story/viz/msc.py` & `text2story-1.4.6/text2story/viz/msc.py`

 * *Files identical despite different names*

### Comparing `text2story-1.4.5/text2story.egg-info/PKG-INFO` & `text2story-1.4.6/text2story.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2story
-Version: 1.4.5
+Version: 1.4.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: joblib
 Requires-Dist: spacy
 Requires-Dist: py-heideltime
 Requires-Dist: importlib_metadata
 Requires-Dist: pandas<2.0.0
```

### Comparing `text2story-1.4.5/text2story.egg-info/SOURCES.txt` & `text2story-1.4.6/text2story.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -26,18 +26,20 @@
 text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/non_padded_namespaces.txt
 text2story/annotators/BERTNERPT/POS_tagger_brill.pkl
 text2story/annotators/BERTNERPT/__init__.py
 text2story/annotators/CUSTOMPT/__init__.py
 text2story/annotators/CUSTOMPT/crf_v2.1.joblib
 text2story/annotators/CUSTOMPT/event_model.py
 text2story/annotators/CUSTOMPT/feature_extractor.py
+text2story/annotators/DBPEDIA/__init__.py
 text2story/annotators/NLTK/__init__.py
 text2story/annotators/PY_HEIDELTIME/__init__.py
 text2story/annotators/SPACY/__init__.py
 text2story/annotators/SPARKNLP/__init__.py
+text2story/annotators/SRL/__init__.py
 text2story/annotators/SRLWeakLabeling/__init__.py
 text2story/annotators/TEI2GO/__init__.py
 text2story/brat2viz/README.md
 text2story/brat2viz/__init__.py
 text2story/brat2viz/brat2drs/__init__.py
 text2story/brat2viz/brat2drs/brat2drs.py
 text2story/brat2viz/brat2drs/files_monitor.py
@@ -68,14 +70,15 @@
 text2story/experiments/stats.py
 text2story/readers/__init__.py
 text2story/readers/fn-lirics.json
 text2story/readers/pb-vn2.json
 text2story/readers/read.py
 text2story/readers/read_ace.py
 text2story/readers/read_brat.py
+text2story/readers/read_csv.py
 text2story/readers/read_ecb.py
 text2story/readers/read_framenet.py
 text2story/readers/read_propbank.py
 text2story/readers/token_corpus.py
 text2story/readers/utils.py
 text2story/readers/vn-lirics.json
 text2story/select/README.md
```

