# Comparing `tmp/chemdataextractor2-2.2.2.tar.gz` & `tmp/chemdataextractor2-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chemdataextractor2-2.2.2.tar", last modified: Thu Jan 18 12:39:06 2024, max compression
+gzip compressed data, was "chemdataextractor2-2.3.2.tar", last modified: Fri May  3 14:08:13 2024, max compression
```

## Comparing `chemdataextractor2-2.2.2.tar` & `chemdataextractor2-2.3.2.tar`

### file list

```diff
@@ -1,333 +1,268 @@
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/.github/
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/.github/workflows/
--rw-r--r--   0 Taketomo   (501) staff       (20)     1189 2023-09-24 07:25:38.000000 chemdataextractor2-2.2.2/.github/workflows/test-cde.yml
--rw-r--r--   0 Taketomo   (501) staff       (20)      628 2023-09-26 19:57:29.000000 chemdataextractor2-2.2.2/.gitignore
--rw-r--r--   0 Taketomo   (501) staff       (20)      545 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/.readthedocs.yml
--rw-r--r--   0 Taketomo   (501) staff       (20)        0 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/.travis.yml
--rw-r--r--   0 Taketomo   (501) staff       (20)     5452 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/CHANGELOG.md
--rw-r--r--   0 Taketomo   (501) staff       (20)    44569 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/Introduction.md
--rw-r--r--   0 Taketomo   (501) staff       (20)     2443 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/LICENSE
--rw-r--r--   0 Taketomo   (501) staff       (20)      311 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/MANIFEST.in
--rw-r--r--   0 Taketomo   (501) staff       (20)     2291 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/PKG-INFO
--rw-r--r--   0 Taketomo   (501) staff       (20)     1056 2023-09-24 07:25:38.000000 chemdataextractor2-2.2.2/README.md
--rw-r--r--   0 Taketomo   (501) staff       (20)      792 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/appveyor.yml
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/chemdataextractor/
--rw-r--r--   0 Taketomo   (501) staff       (20)      808 2024-01-18 12:26:54.000000 chemdataextractor2-2.2.2/chemdataextractor/__init__.py
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/chemdataextractor/biblio/
--rw-r--r--   0 Taketomo   (501) staff       (20)      350 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/biblio/__init__.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     7126 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/biblio/bibtex.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    11263 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/biblio/person.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     3455 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/biblio/xmp.py
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/chemdataextractor/cli/
--rw-r--r--   0 Taketomo   (501) staff       (20)     2528 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/cli/__init__.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     1068 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/cli/cem.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     4301 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/cli/chemdner.py
--rw-r--r--   0 Taketomo   (501) staff       (20)      973 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/cli/cluster.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     1504 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/cli/config.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     1377 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/cli/data.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    12236 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/cli/dict.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    13098 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/cli/evaluate.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    11566 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/cli/pos.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     3632 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/cli/tokenize.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     3584 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/config.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     7533 2024-01-18 12:22:26.000000 chemdataextractor2-2.2.2/chemdataextractor/data.py
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/chemdataextractor/doc/
--rw-r--r--   0 Taketomo   (501) staff       (20)      435 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/chemdataextractor/doc/__init__.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    35300 2023-09-26 19:57:29.000000 chemdataextractor2-2.2.2/chemdataextractor/doc/document.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     7817 2023-09-26 19:57:29.000000 chemdataextractor2-2.2.2/chemdataextractor/doc/document_cacher.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     9638 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/chemdataextractor/doc/element.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     4782 2023-09-26 19:57:29.000000 chemdataextractor2-2.2.2/chemdataextractor/doc/figure.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     2730 2022-03-14 11:57:07.000000 chemdataextractor2-2.2.2/chemdataextractor/doc/meta.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    15206 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/chemdataextractor/doc/table.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    54095 2024-01-18 12:22:26.000000 chemdataextractor2-2.2.2/chemdataextractor/doc/text.py
--rw-r--r--   0 Taketomo   (501) staff       (20)      529 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/errors.py
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/chemdataextractor/eval/
--rw-r--r--   0 Taketomo   (501) staff       (20)       66 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/eval/__init__.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    16523 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/eval/evaluation.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    15393 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/eval/sound.mp3
--rw-r--r--   0 Taketomo   (501) staff       (20)    22113 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/eval/sound_end.mp3
--rw-r--r--   0 Taketomo   (501) staff       (20)      666 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/chemdataextractor/fastner.py
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/chemdataextractor/model/
--rw-r--r--   0 Taketomo   (501) staff       (20)      447 2023-09-26 19:57:29.000000 chemdataextractor2-2.2.2/chemdataextractor/model/__init__.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    54750 2023-09-26 19:57:29.000000 chemdataextractor2-2.2.2/chemdataextractor/model/base.py
--rw-r--r--   0 Taketomo   (501) staff       (20)      511 2023-09-26 19:57:29.000000 chemdataextractor2-2.2.2/chemdataextractor/model/confidence_pooling.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     4552 2023-09-26 19:57:29.000000 chemdataextractor2-2.2.2/chemdataextractor/model/contextual_range.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    12150 2023-09-26 19:57:29.000000 chemdataextractor2-2.2.2/chemdataextractor/model/model.py
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/chemdataextractor/model/units/
--rw-r--r--   0 Taketomo   (501) staff       (20)      650 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/model/units/__init__.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     1583 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/model/units/angle.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     1337 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/model/units/charge.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     1574 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/model/units/current.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    12148 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/model/units/dimension.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     1418 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/model/units/electric_potential.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     2260 2022-05-26 05:41:16.000000 chemdataextractor2-2.2.2/chemdataextractor/model/units/energy.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     2824 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/model/units/length.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     2403 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/model/units/mass.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     1409 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/model/units/power.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    13431 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/chemdataextractor/model/units/quantity_model.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     1249 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/model/units/ratio.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     1946 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/model/units/substance_amount.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     2970 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/model/units/temperature.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     3252 2023-09-26 19:57:29.000000 chemdataextractor2-2.2.2/chemdataextractor/model/units/time.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    14038 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/model/units/unit.py
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/chemdataextractor/nlp/
--rw-r--r--   0 Taketomo   (501) staff       (20)      753 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/chemdataextractor/nlp/__init__.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    11866 2023-09-24 07:25:38.000000 chemdataextractor2-2.2.2/chemdataextractor/nlp/abbrev.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    14199 2023-09-26 19:57:29.000000 chemdataextractor2-2.2.2/chemdataextractor/nlp/allennlpwrapper.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    48838 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/chemdataextractor/nlp/cem.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     3651 2023-09-26 19:57:29.000000 chemdataextractor2-2.2.2/chemdataextractor/nlp/corenlp_dependency.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     6301 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/nlp/corpus.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     2137 2023-09-26 19:57:29.000000 chemdataextractor2-2.2.2/chemdataextractor/nlp/dependency.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    11562 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/chemdataextractor/nlp/finetuned_bert_crf_wrapper.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     7017 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/nlp/lexicon.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     1777 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/chemdataextractor/nlp/new_cem.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    12154 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/chemdataextractor/nlp/pos.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     1088 2023-09-26 19:57:29.000000 chemdataextractor2-2.2.2/chemdataextractor/nlp/spacy_dependency.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    14384 2023-09-26 19:57:29.000000 chemdataextractor2-2.2.2/chemdataextractor/nlp/subsentence.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    26351 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/chemdataextractor/nlp/tag.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    48612 2023-09-26 19:57:29.000000 chemdataextractor2-2.2.2/chemdataextractor/nlp/tokenize.py
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/chemdataextractor/parse/
--rw-r--r--   0 Taketomo   (501) staff       (20)      621 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/chemdataextractor/parse/__init__.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     2525 2023-09-26 19:57:29.000000 chemdataextractor2-2.2.2/chemdataextractor/parse/actions.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     2062 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/parse/apparatus.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    19643 2023-09-26 19:57:29.000000 chemdataextractor2-2.2.2/chemdataextractor/parse/auto.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    21946 2023-09-26 19:57:29.000000 chemdataextractor2-2.2.2/chemdataextractor/parse/auto_dependency.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     7051 2023-09-26 19:57:29.000000 chemdataextractor2-2.2.2/chemdataextractor/parse/base.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     1126 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/parse/category.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    12430 2023-09-26 19:57:29.000000 chemdataextractor2-2.2.2/chemdataextractor/parse/cem.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    38257 2023-09-26 19:57:29.000000 chemdataextractor2-2.2.2/chemdataextractor/parse/cem_factory.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     2068 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/parse/common.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     6304 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/parse/context.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     1203 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/parse/definitions.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    25562 2023-09-26 19:57:29.000000 chemdataextractor2-2.2.2/chemdataextractor/parse/elements.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     3593 2023-09-26 19:57:29.000000 chemdataextractor2-2.2.2/chemdataextractor/parse/ir.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     3695 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/parse/mp.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     3454 2023-09-26 19:57:29.000000 chemdataextractor2-2.2.2/chemdataextractor/parse/mp_new.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     4371 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/parse/new_parsers.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     7129 2024-01-18 12:38:37.000000 chemdataextractor2-2.2.2/chemdataextractor/parse/nmr.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    31981 2023-09-26 19:57:29.000000 chemdataextractor2-2.2.2/chemdataextractor/parse/quantity.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    30200 2023-09-26 19:57:29.000000 chemdataextractor2-2.2.2/chemdataextractor/parse/template.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     2812 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/chemdataextractor/parse/tg.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     2401 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/parse/uvvis.py
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/chemdataextractor/reader/
--rw-r--r--   0 Taketomo   (501) staff       (20)      874 2022-03-16 16:54:25.000000 chemdataextractor2-2.2.2/chemdataextractor/reader/__init__.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     1282 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/reader/acs.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     1197 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/reader/base.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     1418 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/reader/cssp.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    11557 2024-01-18 12:22:26.000000 chemdataextractor2-2.2.2/chemdataextractor/reader/elsevier.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    15061 2023-09-26 19:57:29.000000 chemdataextractor2-2.2.2/chemdataextractor/reader/markup.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     2158 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/reader/nlm.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     5902 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/reader/pdf.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     1010 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/reader/plaintext.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     3390 2023-09-26 19:57:29.000000 chemdataextractor2-2.2.2/chemdataextractor/reader/rsc.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     5500 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/reader/springer.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     3403 2022-03-16 16:54:25.000000 chemdataextractor2-2.2.2/chemdataextractor/reader/springer_jats.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     6337 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/reader/uspto.py
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/chemdataextractor/relex/
--rw-r--r--   0 Taketomo   (501) staff       (20)      875 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/relex/__init__.py
--rw-r--r--   0 Taketomo   (501) staff       (20)      953 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/relex/candidate_parser.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     9734 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/chemdataextractor/relex/cluster.py
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/chemdataextractor/relex/data/
--rw-r--r--   0 Taketomo   (501) staff       (20)    63336 2023-09-26 19:57:29.000000 chemdataextractor2-2.2.2/chemdataextractor/relex/data/CurieTemperature.pkl
--rw-r--r--   0 Taketomo   (501) staff       (20)      342 2023-09-26 17:44:55.000000 chemdataextractor2-2.2.2/chemdataextractor/relex/data/CurieTemperature_clusters.txt
--rw-r--r--   0 Taketomo   (501) staff       (20)      163 2023-09-26 17:44:55.000000 chemdataextractor2-2.2.2/chemdataextractor/relex/data/CurieTemperature_patterns.txt
--rw-r--r--   0 Taketomo   (501) staff       (20)      365 2023-09-26 17:44:55.000000 chemdataextractor2-2.2.2/chemdataextractor/relex/data/CurieTemperature_relations.txt
--rw-r--r--   0 Taketomo   (501) staff       (20)     2214 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/relex/entity.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     3100 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/relex/pattern.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     4662 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/relex/phrase.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     2153 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/relex/relationship.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    28456 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/chemdataextractor/relex/snowball.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     6237 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/relex/utils.py
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/chemdataextractor/scrape/
--rw-r--r--   0 Taketomo   (501) staff       (20)     1621 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/scrape/__init__.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     7800 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/scrape/base.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     9285 2024-01-18 12:22:26.000000 chemdataextractor2-2.2.2/chemdataextractor/scrape/clean.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     4832 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/scrape/csstranslator.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     7938 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/scrape/entity.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     4260 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/scrape/fields.py
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/chemdataextractor/scrape/pub/
--rw-r--r--   0 Taketomo   (501) staff       (20)      223 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/scrape/pub/__init__.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    10093 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/scrape/pub/elsevier.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     8662 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/scrape/pub/nlm.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    22045 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/scrape/pub/rsc.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     7041 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/scrape/pub/springer.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     4980 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/scrape/scraper.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     5871 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/scrape/selector.py
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/chemdataextractor/text/
--rw-r--r--   0 Taketomo   (501) staff       (20)    10401 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/text/__init__.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    12100 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/text/chem.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    49709 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/text/latex.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     8023 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/text/normalize.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     4804 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/text/processors.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     2523 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/chemdataextractor/utils.py
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/chemdataextractor2.egg-info/
--rw-r--r--   0 Taketomo   (501) staff       (20)     2291 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/chemdataextractor2.egg-info/PKG-INFO
--rw-r--r--   0 Taketomo   (501) staff       (20)     9581 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/chemdataextractor2.egg-info/SOURCES.txt
--rw-r--r--   0 Taketomo   (501) staff       (20)        1 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/chemdataextractor2.egg-info/dependency_links.txt
--rw-r--r--   0 Taketomo   (501) staff       (20)       51 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/chemdataextractor2.egg-info/entry_points.txt
--rw-r--r--   0 Taketomo   (501) staff       (20)        1 2022-02-25 17:18:32.000000 chemdataextractor2-2.2.2/chemdataextractor2.egg-info/not-zip-safe
--rw-r--r--   0 Taketomo   (501) staff       (20)      438 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/chemdataextractor2.egg-info/requires.txt
--rw-r--r--   0 Taketomo   (501) staff       (20)       27 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/chemdataextractor2.egg-info/top_level.txt
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/docs/
--rw-r--r--   0 Taketomo   (501) staff       (20)       26 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/docs/_config.yml
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/docs/_static/
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/docs/_static/css/
--rw-r--r--   0 Taketomo   (501) staff       (20)      515 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/docs/_static/css/custom.css
--rw-r--r--   0 Taketomo   (501) staff       (20)     4336 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/docs/_static/logo.png
--rw-r--r--   0 Taketomo   (501) staff       (20)     5313 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/docs/_static/logo.svg
--rw-r--r--   0 Taketomo   (501) staff       (20)    19026 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/docs/_static/logo2.png
--rw-r--r--   0 Taketomo   (501) staff       (20)       30 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/docs/changelog.rst
--rw-r--r--   0 Taketomo   (501) staff       (20)     2956 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/docs/code_documentation.rst
--rw-r--r--   0 Taketomo   (501) staff       (20)     7684 2024-01-18 12:26:54.000000 chemdataextractor2-2.2.2/docs/conf.py
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/docs/examples/
--rw-r--r--   0 Taketomo   (501) staff       (20)     6209 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/docs/examples/creating_taggers.rst
--rw-r--r--   0 Taketomo   (501) staff       (20)     6776 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/docs/examples/creating_units.rst
--rw-r--r--   0 Taketomo   (501) staff       (20)     3092 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/docs/examples/inferred_property.rst
--rw-r--r--   0 Taketomo   (501) staff       (20)      601 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/docs/examples.rst
--rw-r--r--   0 Taketomo   (501) staff       (20)     3806 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/docs/favicon.svg
--rw-r--r--   0 Taketomo   (501) staff       (20)     5618 2023-09-24 07:25:38.000000 chemdataextractor2-2.2.2/docs/getting_started.rst
--rw-r--r--   0 Taketomo   (501) staff       (20)     1042 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/docs/index.rst
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/docs/introduction/
--rw-r--r--   0 Taketomo   (501) staff       (20)     2608 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/docs/introduction/cli.rst
--rw-r--r--   0 Taketomo   (501) staff       (20)     6119 2023-09-04 20:45:57.000000 chemdataextractor2-2.2.2/docs/introduction/contributing.rst
--rw-r--r--   0 Taketomo   (501) staff       (20)     2038 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/docs/introduction/finding_records.rst
--rw-r--r--   0 Taketomo   (501) staff       (20)    17067 2023-09-24 07:25:38.000000 chemdataextractor2-2.2.2/docs/introduction/new_property.rst
--rw-r--r--   0 Taketomo   (501) staff       (20)     5039 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/docs/introduction/nlp.rst
--rw-r--r--   0 Taketomo   (501) staff       (20)     8432 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/docs/introduction/reading_docs.rst
--rw-r--r--   0 Taketomo   (501) staff       (20)     4790 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/docs/introduction/scraping.rst
--rw-r--r--   0 Taketomo   (501) staff       (20)     2420 2023-09-24 07:25:38.000000 chemdataextractor2-2.2.2/docs/license.rst
--rw-r--r--   0 Taketomo   (501) staff       (20)     3861 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/docs/logo.svg
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/docs/migration_guides/
--rw-r--r--   0 Taketomo   (501) staff       (20)      777 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/docs/migration_guides/index.rst
--rw-r--r--   0 Taketomo   (501) staff       (20)    32953 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/docs/migration_guides/migration_guide.rst
--rw-r--r--   0 Taketomo   (501) staff       (20)    19254 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/docs/migration_guides/migration_guide2.1.rst
--rw-r--r--   0 Taketomo   (501) staff       (20)      157 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/docs/requirements.txt
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/docs/source_code_docs/
--rw-r--r--   0 Taketomo   (501) staff       (20)      709 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/docs/source_code_docs/biblio.rst
--rw-r--r--   0 Taketomo   (501) staff       (20)      670 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/docs/source_code_docs/chemdataextractor.rst
--rw-r--r--   0 Taketomo   (501) staff       (20)     3403 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/docs/source_code_docs/cli.rst
--rw-r--r--   0 Taketomo   (501) staff       (20)     1250 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/docs/source_code_docs/doc.rst
--rw-r--r--   0 Taketomo   (501) staff       (20)      280 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/docs/source_code_docs/eval.rst
--rw-r--r--   0 Taketomo   (501) staff       (20)     1993 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/docs/source_code_docs/model.rst
--rw-r--r--   0 Taketomo   (501) staff       (20)     1516 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/docs/source_code_docs/nlp.rst
--rw-r--r--   0 Taketomo   (501) staff       (20)     2232 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/docs/source_code_docs/parse.rst
--rw-r--r--   0 Taketomo   (501) staff       (20)     1761 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/docs/source_code_docs/reader.rst
--rw-r--r--   0 Taketomo   (501) staff       (20)     1270 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/docs/source_code_docs/relex.rst
--rw-r--r--   0 Taketomo   (501) staff       (20)     1986 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/docs/source_code_docs/scrape.rst
--rw-r--r--   0 Taketomo   (501) staff       (20)      749 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/docs/source_code_docs/text.rst
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/examples/
--rw-r--r--   0 Taketomo   (501) staff       (20)        0 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/examples/__init__.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     4268 2022-03-16 16:54:25.000000 chemdataextractor2-2.2.2/examples/automatic_parsers.ipynb
--rw-r--r--   0 Taketomo   (501) staff       (20)     8252 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/examples/automatic_parsing_for_tables.ipynb
--rw-r--r--   0 Taketomo   (501) staff       (20)    18283 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/examples/automatic_parsing_of_complex_models.ipynb
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/examples/data/
--rw-r--r--   0 Taketomo   (501) staff       (20)      208 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/examples/data/table_example.csv
--rw-r--r--   0 Taketomo   (501) staff       (20)      501 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/examples/data/table_example_3.csv
--rw-r--r--   0 Taketomo   (501) staff       (20)     8166 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/examples/extracting_a_custom_property.ipynb
--rw-r--r--   0 Taketomo   (501) staff       (20)     2025 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/examples/searching_rsc.ipynb
--rw-r--r--   0 Taketomo   (501) staff       (20)     6176 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/examples/template_parsers.ipynb
--rw-r--r--   0 Taketomo   (501) staff       (20)     3911 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/examples/using_config_file.ipynb
--rw-r--r--   0 Taketomo   (501) staff       (20)    23786 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/examples/using_snowball.ipynb
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/requirements/
--rw-r--r--   0 Taketomo   (501) staff       (20)       76 2024-01-18 12:22:26.000000 chemdataextractor2-2.2.2/requirements/development.txt
--rw-r--r--   0 Taketomo   (501) staff       (20)      457 2024-01-18 12:22:26.000000 chemdataextractor2-2.2.2/requirements/production.txt
--rw-r--r--   0 Taketomo   (501) staff       (20)       31 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/requirements.txt
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/scripts/
--rw-r--r--   0 Taketomo   (501) staff       (20)      691 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/scripts/chemdner.sh
--rw-r--r--   0 Taketomo   (501) staff       (20)      554 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/scripts/cluster.sh
--rw-r--r--   0 Taketomo   (501) staff       (20)      204 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/scripts/dict.sh
--rw-r--r--   0 Taketomo   (501) staff       (20)    25451 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/scripts/melting_points_eval.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     4657 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/scripts/pos.sh
--rw-r--r--   0 Taketomo   (501) staff       (20)       38 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/setup.cfg
--rw-r--r--   0 Taketomo   (501) staff       (20)     2593 2024-01-18 12:26:54.000000 chemdataextractor2-2.2.2/setup.py
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/tests/
--rw-r--r--   0 Taketomo   (501) staff       (20)     6148 2022-12-09 07:59:27.000000 chemdataextractor2-2.2.2/tests/.DS_Store
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/tests/data/
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/tests/data/acs/
--rw-r--r--   0 Taketomo   (501) staff       (20)   440092 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/tests/data/acs/acs.jmedchem.6b00723.html
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/tests/data/elsevier/
--rw-r--r--   0 Taketomo   (501) staff       (20)   227028 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/tests/data/elsevier/j.jnoncrysol.2017.07.006.xml
--rw-r--r--   0 Taketomo   (501) staff       (20)   414742 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/tests/data/elsevier/j.jnoncrysol.2018.02.024.xml
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/tests/data/relex/
--rw-r--r--   0 Taketomo   (501) staff       (20)    15997 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/tests/data/relex/curie_temperatures.pkl
--rw-r--r--   0 Taketomo   (501) staff       (20)    29568 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/tests/data/relex/curie_temperatures_py2.pkl
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/tests/data/relex/curie_training_set/
--rw-r--r--   0 Taketomo   (501) staff       (20)   158180 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/tests/data/relex/curie_training_set/b806499g.html
--rw-r--r--   0 Taketomo   (501) staff       (20)   231958 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/tests/data/relex/curie_training_set/c1jm13879k.html
--rw-r--r--   0 Taketomo   (501) staff       (20)   177571 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/tests/data/relex/curie_training_set/c2jm33712f.html
--rw-r--r--   0 Taketomo   (501) staff       (20)   296700 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/tests/data/relex/curie_training_set/c2nr11767c.html
--rw-r--r--   0 Taketomo   (501) staff       (20)   114880 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/tests/data/relex/curie_training_set/c3nr33950e.html
--rw-r--r--   0 Taketomo   (501) staff       (20)   176637 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/tests/data/relex/curie_training_set/c6cp00375c.html
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/tests/data/rsc/
--rw-r--r--   0 Taketomo   (501) staff       (20)   100282 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/tests/data/rsc/10.1039_C6OB02074G.html
--rw-r--r--   0 Taketomo   (501) staff       (20)   185561 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/tests/data/rsc/searchresults.html
--rw-r--r--   0 Taketomo   (501) staff       (20)   110399 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/tests/data/rsc/test_paper.html
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/tests/data/springer/
--rw-r--r--   0 Taketomo   (501) staff       (20)   229930 2022-03-16 16:54:25.000000 chemdataextractor2-2.2.2/tests/data/springer/spr_test1.xml
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/tests/data/tables/
--rw-r--r--   0 Taketomo   (501) staff       (20)   515408 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/tests/data/tables/j.commatsci.2018.02.056.xml
--rw-r--r--   0 Taketomo   (501) staff       (20)   515384 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/tests/data/tables/j.commatsci.2018.02.056_2.xml
--rw-r--r--   0 Taketomo   (501) staff       (20)      190 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/tests/data/tables/table_example_1.csv
--rw-r--r--   0 Taketomo   (501) staff       (20)      240 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/tests/data/tables/table_example_2.csv
--rw-r--r--   0 Taketomo   (501) staff       (20)      465 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/tests/data/tables/table_example_3.csv
--rw-r--r--   0 Taketomo   (501) staff       (20)     4421 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/tests/data/tables/table_test.html
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/tests/data/test_cache/
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/tests/data/test_cache/test_cache/
--rw-r--r--   0 Taketomo   (501) staff       (20)      100 2023-09-26 17:42:56.000000 chemdataextractor2-2.2.2/tests/data/test_cache/test_cache/configuration.json
--rw-r--r--   0 Taketomo   (501) staff       (20)    20939 2023-09-26 17:43:24.000000 chemdataextractor2-2.2.2/tests/data/test_cache/test_cache/subsentences.txt
--rw-r--r--   0 Taketomo   (501) staff       (20)   131970 2023-09-26 17:43:14.000000 chemdataextractor2-2.2.2/tests/data/test_cache/test_cache/tag__ner_tag.txt
--rw-r--r--   0 Taketomo   (501) staff       (20)    93213 2023-09-26 17:43:14.000000 chemdataextractor2-2.2.2/tests/data/test_cache/test_cache/tag__pos_tag.txt
--rw-r--r--   0 Taketomo   (501) staff       (20)    59030 2023-09-26 17:42:56.000000 chemdataextractor2-2.2.2/tests/data/test_cache/test_cache/tag__start_end.txt
--rw-r--r--   0 Taketomo   (501) staff       (20)   100062 2023-09-26 17:42:56.000000 chemdataextractor2-2.2.2/tests/data/test_cache/test_cache/tokenizer__BertWordTokenizer.txt
--rw-r--r--   0 Taketomo   (501) staff       (20)      463 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/tests/data/test_config.yml
-drwxr-xr-x   0 Taketomo   (501) staff       (20)        0 2024-01-18 12:39:06.000000 chemdataextractor2-2.2.2/tests/data/uspto/
--rw-r--r--   0 Taketomo   (501) staff       (20)    85297 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/tests/data/uspto/US06840965B2.xml
--rw-r--r--   0 Taketomo   (501) staff       (20)     7750 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/tests/test_biblio.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     1846 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/tests/test_doc_cache.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     5132 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/tests/test_doc_document.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    39837 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/tests/test_doc_table.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    37909 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/tests/test_doc_table_2.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     4026 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/tests/test_doc_text.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     6523 2023-09-26 19:57:29.000000 chemdataextractor2-2.2.2/tests/test_extract.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    11815 2023-09-26 19:57:29.000000 chemdataextractor2-2.2.2/tests/test_model.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     7044 2023-09-26 19:57:29.000000 chemdataextractor2-2.2.2/tests/test_model_contextual_range.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    11515 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/tests/test_model_units.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     7570 2023-09-24 07:25:38.000000 chemdataextractor2-2.2.2/tests/test_nlp_abbrev.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     3206 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/tests/test_nlp_cem.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     2319 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/tests/test_nlp_pos.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     7474 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/tests/test_nlp_sentence.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     3459 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/tests/test_nlp_tag.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    55194 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/tests/test_nlp_tokenize.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     2300 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/tests/test_parse_apparatus.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     6544 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/tests/test_parse_auto.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     3120 2023-09-26 19:57:29.000000 chemdataextractor2-2.2.2/tests/test_parse_auto_dependency.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    21497 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/tests/test_parse_cem.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     7589 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/tests/test_parse_definitions.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     4068 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/tests/test_parse_ir.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    13006 2023-09-26 19:57:29.000000 chemdataextractor2-2.2.2/tests/test_parse_mp.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    20422 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/tests/test_parse_nmr.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     7259 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/tests/test_parse_quantity.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    10809 2023-09-26 19:57:29.000000 chemdataextractor2-2.2.2/tests/test_parse_template.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     3742 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/tests/test_parse_tg.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     1411 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/tests/test_parse_uvvis.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     1611 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/tests/test_reader_acs.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     3433 2024-01-18 12:22:26.000000 chemdataextractor2-2.2.2/tests/test_reader_elsevier.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     2199 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/tests/test_reader_markup.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     2544 2023-09-26 19:57:29.000000 chemdataextractor2-2.2.2/tests/test_reader_rsc.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     1564 2022-03-16 16:54:25.000000 chemdataextractor2-2.2.2/tests/test_reader_springer.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     1606 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/tests/test_reader_uspto.py
--rw-r--r--   0 Taketomo   (501) staff       (20)    13081 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/tests/test_reading_cell+fig.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     3913 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/tests/test_relex_cluster.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     2289 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/tests/test_relex_entity.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     4501 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/tests/test_relex_phrase.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     3169 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/tests/test_relex_relationship.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     6040 2022-09-21 10:28:43.000000 chemdataextractor2-2.2.2/tests/test_relex_snowball.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     2131 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/tests/test_relex_utils.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     8214 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/tests/test_scrape_clean.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     9220 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/tests/test_scrape_entity.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     2740 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/tests/test_scrape_fields.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     5614 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/tests/test_scrape_rsc.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     1723 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/tests/test_scrape_selector.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     4364 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/tests/test_text.py
--rw-r--r--   0 Taketomo   (501) staff       (20)     6328 2022-02-23 16:56:42.000000 chemdataextractor2-2.2.2/tests/test_text_chem.py
+drwxrwxr-x   0 dh582     (1000) dh582     (1000)        0 2024-05-03 14:08:13.673673 chemdataextractor2-2.3.2/
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     5452 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/CHANGELOG.md
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     2443 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/LICENSE
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)      311 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/MANIFEST.in
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     2271 2024-05-03 14:08:13.673673 chemdataextractor2-2.3.2/PKG-INFO
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     1056 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/README.md
+drwxrwxr-x   0 dh582     (1000) dh582     (1000)        0 2024-05-03 14:08:13.633673 chemdataextractor2-2.3.2/chemdataextractor/
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)      808 2024-05-03 14:04:23.000000 chemdataextractor2-2.3.2/chemdataextractor/__init__.py
+drwxrwxr-x   0 dh582     (1000) dh582     (1000)        0 2024-05-03 14:08:13.633673 chemdataextractor2-2.3.2/chemdataextractor/biblio/
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)      350 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/biblio/__init__.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     7126 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/biblio/bibtex.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    11263 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/biblio/person.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     3455 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/biblio/xmp.py
+drwxrwxr-x   0 dh582     (1000) dh582     (1000)        0 2024-05-03 14:08:13.637673 chemdataextractor2-2.3.2/chemdataextractor/cli/
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     2528 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/cli/__init__.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     1068 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/cli/cem.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     4301 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/cli/chemdner.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)      973 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/cli/cluster.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     1504 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/cli/config.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     1377 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/cli/data.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    12236 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/cli/dict.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    13098 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/cli/evaluate.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    11566 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/cli/pos.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     3632 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/cli/tokenize.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     3584 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/config.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     7533 2024-05-03 14:04:23.000000 chemdataextractor2-2.3.2/chemdataextractor/data.py
+drwxrwxr-x   0 dh582     (1000) dh582     (1000)        0 2024-05-03 14:08:13.637673 chemdataextractor2-2.3.2/chemdataextractor/doc/
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)      435 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/doc/__init__.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    38602 2024-05-03 14:04:23.000000 chemdataextractor2-2.3.2/chemdataextractor/doc/document.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     8182 2024-05-03 14:04:23.000000 chemdataextractor2-2.3.2/chemdataextractor/doc/document_cacher.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     9638 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/doc/element.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     4782 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/doc/figure.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     2730 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/doc/meta.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    15206 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/doc/table.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    54727 2024-05-03 14:04:23.000000 chemdataextractor2-2.3.2/chemdataextractor/doc/text.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)      529 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/errors.py
+drwxrwxr-x   0 dh582     (1000) dh582     (1000)        0 2024-05-03 14:08:13.637673 chemdataextractor2-2.3.2/chemdataextractor/eval/
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)       66 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/eval/__init__.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    16523 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/eval/evaluation.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)      666 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/fastner.py
+drwxrwxr-x   0 dh582     (1000) dh582     (1000)        0 2024-05-03 14:08:13.637673 chemdataextractor2-2.3.2/chemdataextractor/model/
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)      447 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/model/__init__.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    56671 2024-05-03 14:04:23.000000 chemdataextractor2-2.3.2/chemdataextractor/model/base.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)      511 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/model/confidence_pooling.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     4552 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/model/contextual_range.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    12150 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/model/model.py
+drwxrwxr-x   0 dh582     (1000) dh582     (1000)        0 2024-05-03 14:08:13.641673 chemdataextractor2-2.3.2/chemdataextractor/model/units/
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)      650 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/model/units/__init__.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     1583 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/model/units/angle.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     1337 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/model/units/charge.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     1574 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/model/units/current.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    12148 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/model/units/dimension.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     1418 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/model/units/electric_potential.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     2260 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/model/units/energy.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     2824 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/model/units/length.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     2403 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/model/units/mass.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     1409 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/model/units/power.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    13431 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/model/units/quantity_model.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     1249 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/model/units/ratio.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     1946 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/model/units/substance_amount.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     2970 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/model/units/temperature.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     3252 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/model/units/time.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    14038 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/model/units/unit.py
+drwxrwxr-x   0 dh582     (1000) dh582     (1000)        0 2024-05-03 14:08:13.645673 chemdataextractor2-2.3.2/chemdataextractor/nlp/
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)      753 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/nlp/__init__.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    11866 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/nlp/abbrev.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    14196 2024-05-03 14:04:23.000000 chemdataextractor2-2.3.2/chemdataextractor/nlp/allennlpwrapper.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    48838 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/nlp/cem.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     3651 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/nlp/corenlp_dependency.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     6301 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/nlp/corpus.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     2200 2024-05-03 14:04:23.000000 chemdataextractor2-2.3.2/chemdataextractor/nlp/dependency.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    11562 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/nlp/finetuned_bert_crf_wrapper.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     7017 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/nlp/lexicon.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     1777 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/nlp/new_cem.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    12154 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/nlp/pos.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     1088 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/nlp/spacy_dependency.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    14384 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/nlp/subsentence.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    26351 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/nlp/tag.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    48612 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/nlp/tokenize.py
+drwxrwxr-x   0 dh582     (1000) dh582     (1000)        0 2024-05-03 14:08:13.649673 chemdataextractor2-2.3.2/chemdataextractor/parse/
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)      621 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/parse/__init__.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     2525 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/parse/actions.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     2062 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/parse/apparatus.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    20635 2024-05-03 14:04:23.000000 chemdataextractor2-2.3.2/chemdataextractor/parse/auto.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    21946 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/parse/auto_dependency.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     7051 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/parse/base.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     1126 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/parse/category.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    12430 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/parse/cem.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    38257 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/parse/cem_factory.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     2068 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/parse/common.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     6304 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/parse/context.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     1203 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/parse/definitions.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    25562 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/parse/elements.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     3593 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/parse/ir.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     3695 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/parse/mp.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     3454 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/parse/mp_new.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    22995 2024-05-03 14:04:23.000000 chemdataextractor2-2.3.2/chemdataextractor/parse/multi_turn_qa.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     4371 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/parse/new_parsers.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     7129 2024-05-03 14:04:23.000000 chemdataextractor2-2.3.2/chemdataextractor/parse/nmr.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    31981 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/parse/quantity.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    30200 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/parse/template.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     2812 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/parse/tg.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     2401 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/parse/uvvis.py
+drwxrwxr-x   0 dh582     (1000) dh582     (1000)        0 2024-05-03 14:08:13.649673 chemdataextractor2-2.3.2/chemdataextractor/reader/
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)      874 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/reader/__init__.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     1282 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/reader/acs.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     1197 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/reader/base.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     1418 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/reader/cssp.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    11557 2024-05-03 14:04:23.000000 chemdataextractor2-2.3.2/chemdataextractor/reader/elsevier.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    15061 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/reader/markup.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     2158 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/reader/nlm.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     5902 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/reader/pdf.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     1010 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/reader/plaintext.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     3390 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/reader/rsc.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     5500 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/reader/springer.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     3403 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/reader/springer_jats.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     6337 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/reader/uspto.py
+drwxrwxr-x   0 dh582     (1000) dh582     (1000)        0 2024-05-03 14:08:13.649673 chemdataextractor2-2.3.2/chemdataextractor/relex/
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)      875 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/relex/__init__.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)      953 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/relex/candidate_parser.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     9734 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/relex/cluster.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     2214 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/relex/entity.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     3100 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/relex/pattern.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     4662 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/relex/phrase.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     2153 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/relex/relationship.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    28456 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/relex/snowball.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     6237 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/relex/utils.py
+drwxrwxr-x   0 dh582     (1000) dh582     (1000)        0 2024-05-03 14:08:13.649673 chemdataextractor2-2.3.2/chemdataextractor/scrape/
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     1621 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/scrape/__init__.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     7800 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/scrape/base.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     9285 2024-05-03 14:04:23.000000 chemdataextractor2-2.3.2/chemdataextractor/scrape/clean.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     4832 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/scrape/csstranslator.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     7938 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/scrape/entity.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     4260 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/scrape/fields.py
+drwxrwxr-x   0 dh582     (1000) dh582     (1000)        0 2024-05-03 14:08:13.653673 chemdataextractor2-2.3.2/chemdataextractor/scrape/pub/
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)      223 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/scrape/pub/__init__.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    10093 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/scrape/pub/elsevier.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     8662 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/scrape/pub/nlm.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    22045 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/scrape/pub/rsc.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     7041 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/scrape/pub/springer.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     4980 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/scrape/scraper.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     5871 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/scrape/selector.py
+drwxrwxr-x   0 dh582     (1000) dh582     (1000)        0 2024-05-03 14:08:13.653673 chemdataextractor2-2.3.2/chemdataextractor/text/
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    10401 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/text/__init__.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    12100 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/text/chem.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    49709 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/text/latex.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     8023 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/text/normalize.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     4804 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/text/processors.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     2523 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/chemdataextractor/utils.py
+drwxrwxr-x   0 dh582     (1000) dh582     (1000)        0 2024-05-03 14:08:13.653673 chemdataextractor2-2.3.2/chemdataextractor2.egg-info/
+-rw-r--r--   0 dh582     (1000) dh582     (1000)     2271 2024-05-03 14:08:13.000000 chemdataextractor2-2.3.2/chemdataextractor2.egg-info/PKG-INFO
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     8002 2024-05-03 14:08:13.000000 chemdataextractor2-2.3.2/chemdataextractor2.egg-info/SOURCES.txt
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)        1 2024-05-03 14:08:13.000000 chemdataextractor2-2.3.2/chemdataextractor2.egg-info/dependency_links.txt
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)       50 2024-05-03 14:08:13.000000 chemdataextractor2-2.3.2/chemdataextractor2.egg-info/entry_points.txt
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)        1 2023-10-18 10:44:53.000000 chemdataextractor2-2.3.2/chemdataextractor2.egg-info/not-zip-safe
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)      527 2024-05-03 14:08:13.000000 chemdataextractor2-2.3.2/chemdataextractor2.egg-info/requires.txt
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)       27 2024-05-03 14:08:13.000000 chemdataextractor2-2.3.2/chemdataextractor2.egg-info/top_level.txt
+drwxrwxr-x   0 dh582     (1000) dh582     (1000)        0 2024-05-03 14:08:13.653673 chemdataextractor2-2.3.2/examples/
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)        0 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/examples/__init__.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     4268 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/examples/automatic_parsers.ipynb
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     8252 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/examples/automatic_parsing_for_tables.ipynb
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    18283 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/examples/automatic_parsing_of_complex_models.ipynb
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     8166 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/examples/extracting_a_custom_property.ipynb
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     2025 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/examples/searching_rsc.ipynb
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     6176 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/examples/template_parsers.ipynb
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     3911 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/examples/using_config_file.ipynb
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    23786 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/examples/using_snowball.ipynb
+drwxrwxr-x   0 dh582     (1000) dh582     (1000)        0 2024-05-03 14:08:13.657673 chemdataextractor2-2.3.2/requirements/
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)       92 2024-05-03 14:04:23.000000 chemdataextractor2-2.3.2/requirements/development.txt
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)      496 2024-05-03 14:04:23.000000 chemdataextractor2-2.3.2/requirements/production.txt
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)       31 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/requirements.txt
+drwxrwxr-x   0 dh582     (1000) dh582     (1000)        0 2024-05-03 14:08:13.657673 chemdataextractor2-2.3.2/scripts/
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)      691 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/scripts/chemdner.sh
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)      554 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/scripts/cluster.sh
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)      204 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/scripts/dict.sh
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    25451 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/scripts/melting_points_eval.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     4657 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/scripts/pos.sh
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)       38 2024-05-03 14:08:13.673673 chemdataextractor2-2.3.2/setup.cfg
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     2691 2024-05-03 14:04:23.000000 chemdataextractor2-2.3.2/setup.py
+drwxrwxr-x   0 dh582     (1000) dh582     (1000)        0 2024-05-03 14:08:13.661673 chemdataextractor2-2.3.2/tests/
+drwxrwxr-x   0 dh582     (1000) dh582     (1000)        0 2024-05-03 14:08:13.661673 chemdataextractor2-2.3.2/tests/data/
+drwxrwxr-x   0 dh582     (1000) dh582     (1000)        0 2024-05-03 14:08:13.661673 chemdataextractor2-2.3.2/tests/data/acs/
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)   440092 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/data/acs/acs.jmedchem.6b00723.html
+drwxrwxr-x   0 dh582     (1000) dh582     (1000)        0 2024-05-03 14:08:13.665673 chemdataextractor2-2.3.2/tests/data/elsevier/
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)   227028 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/data/elsevier/j.jnoncrysol.2017.07.006.xml
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)   414742 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/data/elsevier/j.jnoncrysol.2018.02.024.xml
+drwxrwxr-x   0 dh582     (1000) dh582     (1000)        0 2024-05-03 14:08:13.665673 chemdataextractor2-2.3.2/tests/data/relex/
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    15997 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/data/relex/curie_temperatures.pkl
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    29568 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/data/relex/curie_temperatures_py2.pkl
+drwxrwxr-x   0 dh582     (1000) dh582     (1000)        0 2024-05-03 14:08:13.665673 chemdataextractor2-2.3.2/tests/data/relex/curie_training_set/
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)   158180 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/data/relex/curie_training_set/b806499g.html
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)   231958 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/data/relex/curie_training_set/c1jm13879k.html
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)   177571 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/data/relex/curie_training_set/c2jm33712f.html
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)   296700 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/data/relex/curie_training_set/c2nr11767c.html
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)   114880 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/data/relex/curie_training_set/c3nr33950e.html
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)   176637 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/data/relex/curie_training_set/c6cp00375c.html
+drwxrwxr-x   0 dh582     (1000) dh582     (1000)        0 2024-05-03 14:08:13.665673 chemdataextractor2-2.3.2/tests/data/rsc/
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)   100282 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/data/rsc/10.1039_C6OB02074G.html
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)   185561 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/data/rsc/searchresults.html
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)   110399 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/data/rsc/test_paper.html
+drwxrwxr-x   0 dh582     (1000) dh582     (1000)        0 2024-05-03 14:08:13.665673 chemdataextractor2-2.3.2/tests/data/springer/
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)   229930 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/data/springer/spr_test1.xml
+drwxrwxr-x   0 dh582     (1000) dh582     (1000)        0 2024-05-03 14:08:13.669673 chemdataextractor2-2.3.2/tests/data/tables/
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)   515408 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/data/tables/j.commatsci.2018.02.056.xml
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)   515384 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/data/tables/j.commatsci.2018.02.056_2.xml
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)      190 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/data/tables/table_example_1.csv
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)      240 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/data/tables/table_example_2.csv
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)      465 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/data/tables/table_example_3.csv
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     4421 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/data/tables/table_test.html
+drwxrwxr-x   0 dh582     (1000) dh582     (1000)        0 2024-05-03 14:08:13.633673 chemdataextractor2-2.3.2/tests/data/test_cache/
+drwxrwxr-x   0 dh582     (1000) dh582     (1000)        0 2024-05-03 14:08:13.673673 chemdataextractor2-2.3.2/tests/data/test_cache/test_cache/
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)      100 2023-10-18 10:54:51.000000 chemdataextractor2-2.3.2/tests/data/test_cache/test_cache/configuration.json
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    20939 2023-10-18 10:55:03.000000 chemdataextractor2-2.3.2/tests/data/test_cache/test_cache/subsentences.txt
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)   131970 2023-10-18 10:54:58.000000 chemdataextractor2-2.3.2/tests/data/test_cache/test_cache/tag__ner_tag.txt
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    93213 2023-10-18 10:54:58.000000 chemdataextractor2-2.3.2/tests/data/test_cache/test_cache/tag__pos_tag.txt
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    59030 2023-10-18 10:54:51.000000 chemdataextractor2-2.3.2/tests/data/test_cache/test_cache/tag__start_end.txt
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)   100062 2023-10-18 10:54:51.000000 chemdataextractor2-2.3.2/tests/data/test_cache/test_cache/tokenizer__BertWordTokenizer.txt
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)      463 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/data/test_config.yml
+drwxrwxr-x   0 dh582     (1000) dh582     (1000)        0 2024-05-03 14:08:13.673673 chemdataextractor2-2.3.2/tests/data/uspto/
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    85297 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/data/uspto/US06840965B2.xml
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     7750 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_biblio.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     1846 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_doc_cache.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     5132 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_doc_document.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    39837 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_doc_table.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    37909 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_doc_table_2.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     4026 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_doc_text.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     6523 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_extract.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    11815 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_model.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     7044 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_model_contextual_range.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    11515 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_model_units.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     7570 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_nlp_abbrev.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     3206 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_nlp_cem.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     2319 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_nlp_pos.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     7474 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_nlp_sentence.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     3459 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_nlp_tag.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    55194 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_nlp_tokenize.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     2300 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_parse_apparatus.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     6544 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_parse_auto.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     3120 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_parse_auto_dependency.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    21497 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_parse_cem.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     7589 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_parse_definitions.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     4068 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_parse_ir.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    13006 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_parse_mp.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    20422 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_parse_nmr.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     7259 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_parse_quantity.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    10809 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_parse_template.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     3742 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_parse_tg.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     1411 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_parse_uvvis.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     1611 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_reader_acs.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     3433 2024-05-03 14:04:23.000000 chemdataextractor2-2.3.2/tests/test_reader_elsevier.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     2199 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_reader_markup.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     2544 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_reader_rsc.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     1564 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_reader_springer.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     1606 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_reader_uspto.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)    13081 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_reading_cell+fig.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     3913 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_relex_cluster.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     2289 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_relex_entity.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     4501 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_relex_phrase.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     3169 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_relex_relationship.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     6040 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_relex_snowball.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     2131 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_relex_utils.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     8214 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_scrape_clean.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     9220 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_scrape_entity.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     2740 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_scrape_fields.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     5614 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_scrape_rsc.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     1723 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_scrape_selector.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     4364 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_text.py
+-rw-rw-r--   0 dh582     (1000) dh582     (1000)     6328 2023-10-18 10:34:42.000000 chemdataextractor2-2.3.2/tests/test_text_chem.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `chemdataextractor2-2.2.2/CHANGELOG.md` & `chemdataextractor2-2.3.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/LICENSE` & `chemdataextractor2-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/PKG-INFO` & `chemdataextractor2-2.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: chemdataextractor2
-Version: 2.2.2
+Version: 2.3.2
 Summary: A toolkit for extracting chemical information from the scientific literature.
 Home-page: https://github.com/CambridgeMolecularEngineering/ChemDataExtractor2
 Author: Matt Swain, Callum Court, Juraj Mavracic, Taketomo Isazawa, and contributors
 Author-email: m.swain@me.com, cc889@cam.ac.uk, jm2111@cam.ac.uk, ti250@cam.ac.uk
 License: MIT
 Keywords: text-mining mining chemistry cheminformatics nlp html xml science scientific
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
@@ -56,9 +55,7 @@
 License
 -------
 
 ChemDataExtractor v2 is licensed under the `MIT license`_, a permissive, business-friendly license for open source
 software.
 
 MIT license: https://github.com/CambridgeMolecularEngineering/ChemDataExtractor/blob/master/LICENSE
-
-
```

### Comparing `chemdataextractor2-2.2.2/README.md` & `chemdataextractor2-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/__init__.py` & `chemdataextractor2-2.3.2/chemdataextractor/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from __future__ import division
 from __future__ import print_function
 from __future__ import unicode_literals
 import logging
 
 
 __title__ = 'ChemDataExtractor'
-__version__ = '2.2.2'
+__version__ = '2.3.2'
 __author__ = 'Matt Swain, Callum Court, Edward Beard, Juraj Mavracic and Taketomo Isazawa'
 __email__ = 'm.swain@me.com, cc889@cam.ac.uk, ejb207@cam.ac.uk, jm2111@cam.ac.uk, ti250@cam.ac.uk'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2019 Matt Swain and contributors'
 
 log = logging.getLogger(__name__)
 log.addHandler(logging.NullHandler())
```

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/biblio/bibtex.py` & `chemdataextractor2-2.3.2/chemdataextractor/biblio/bibtex.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/biblio/person.py` & `chemdataextractor2-2.3.2/chemdataextractor/biblio/person.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/biblio/xmp.py` & `chemdataextractor2-2.3.2/chemdataextractor/biblio/xmp.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/cli/__init__.py` & `chemdataextractor2-2.3.2/chemdataextractor/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/cli/cem.py` & `chemdataextractor2-2.3.2/chemdataextractor/cli/cem.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/cli/chemdner.py` & `chemdataextractor2-2.3.2/chemdataextractor/cli/chemdner.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/cli/cluster.py` & `chemdataextractor2-2.3.2/chemdataextractor/cli/cluster.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/cli/config.py` & `chemdataextractor2-2.3.2/chemdataextractor/cli/config.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/cli/data.py` & `chemdataextractor2-2.3.2/chemdataextractor/cli/data.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/cli/dict.py` & `chemdataextractor2-2.3.2/chemdataextractor/cli/dict.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/cli/evaluate.py` & `chemdataextractor2-2.3.2/chemdataextractor/cli/evaluate.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/cli/pos.py` & `chemdataextractor2-2.3.2/chemdataextractor/cli/pos.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/cli/tokenize.py` & `chemdataextractor2-2.3.2/chemdataextractor/cli/tokenize.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/config.py` & `chemdataextractor2-2.3.2/chemdataextractor/config.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/data.py` & `chemdataextractor2-2.3.2/chemdataextractor/data.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/doc/document.py` & `chemdataextractor2-2.3.2/chemdataextractor/doc/document.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,24 +6,25 @@
 
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 from __future__ import unicode_literals
 
 from abc import ABCMeta, abstractproperty
+from operator import index
 from pprint import pprint
 import collections
 import io
 import json
 import logging
 import copy
 
 import six
 
-from ..utils import python_2_unicode_compatible
+from ..utils import memoized_property, python_2_unicode_compatible
 from .text import Paragraph, Citation, Footnote, Heading, Title, Caption, RichToken, Sentence, Cell
 from .element import CaptionedElement
 from .table import Table
 from .figure import Figure
 from .meta import MetaData
 from ..errors import ReaderError
 from ..model.base import ModelList
@@ -244,14 +245,16 @@
         last_product_record = None
         title_record = None # Records found in the title
         record_id_el_map = {} # A dictionary that tells what element each record ID came from. We use their IDs as the records themselves change as they are updated
 
         prev_records = []
         el_records = []
 
+        self._batch_parse_sentences()
+
         # Main loop, over all elements in the document
         for i, el in enumerate(self.elements):
 
             if type(el) in self.skip_elements:
                 continue
 
             log.debug("Element %d, type %s" %(i, str(type(el))))
@@ -526,14 +529,16 @@
                 model.reset_updatables()
 
         # Append contextual records if they've filled required fields
         # for record in contextual_records:
         #     if record.required_fulfilled:
         #         records.append(record)
 
+        self._clean_batch_parsed_records_dict()
+
         return cleaned_records
 
     def get_element_with_id(self, id):
         """
         Get element with the specified ID. If one is not found, None is returned.
 
         :param id: Identifier to search for.
@@ -704,26 +709,100 @@
         else:
             tag_results = tagger.batch_tag(all_tokens)
 
         for tag_result in tag_results:
             for token, tag in tag_result:
                 token._tags[tag_type] = tag
 
+    def _batch_parse_sentences(self):
+        sentences = self.sentences
+        self._batch_parsers = []
+        sentences_for_parser_at_index = []
+        for sentence in sentences:
+            for model in sentence._streamlined_models:
+                parsers = model.parsers
+                for parser in parsers:
+                    if hasattr(parser, "batch_parse_sentences"):
+                        if parser not in self._batch_parsers:
+                            self._batch_parsers.append(parser)
+                            sentences_for_parser_at_index.append([sentence])
+                        else:
+                            batch_parser_index = self._batch_parsers.index(parser)
+                            sentences_for_parser_at_index[batch_parser_index].append(sentence)
+        for parser, sentences in zip(self._batch_parsers, sentences_for_parser_at_index):
+            records_dict = parser.batch_parse_sentences(sentences)
+            parser._batch_parsed_records_dict = records_dict
+
+    def _clean_batch_parsed_records_dict(self):
+        for batch_parser in self._batch_parsers:
+            batch_parser._batch_parsed_records_dict = {}
+        self._batch_parsers = []
+
     @property
     def sentences(self):
         elements = copy.copy(self.elements)
 
         sentences = []
         for element in elements:
             if element.elements is not None:
                 elements.extend(element.elements)
             if isinstance(element, Sentence) and not isinstance(element, Cell):
                 sentences.append(element)
         return sentences
 
+    def heading_for_sentence(self, sentence):
+        # Note: By design, this returns None if we are passing in a sentence
+        # that's part of a heading
+        elements = copy.copy(self.elements)
+
+        elements_under_heading = []
+        current_heading = None
+        for element in elements:
+            if isinstance(element, Heading):
+                if self._sentence_in_elements(sentence, elements_under_heading):
+                    return current_heading
+                current_heading = element
+                elements_under_heading = []
+                continue
+            else:
+                elements_under_heading.append(element)
+        if self._sentence_in_elements(sentence, elements_under_heading):
+            return current_heading
+        return None
+
+    def _sentence_in_elements(self, sentence, elements):
+        # Warning: this method mutates the elements argument
+        for element in elements:
+            if element is sentence:
+                return True
+            elif element.elements is not None:
+                elements.extend(element.elements)
+        return False
+
+
+    def adjacent_sentences(self, sentence, num_adjacent=2):
+        sentences = self.sentences
+        sentence_index = sentences.index(sentence)
+        adjacent_sentences = sentences[max(0, sentence_index - num_adjacent): sentence_index + num_adjacent]
+        return adjacent_sentences
+
+
+    def preceding_sentences(self, sentence, num_preceding=2):
+        sentences = self.sentences
+        sentence_index = sentences.index(sentence)
+        adjacent_sentences = sentences[max(0, sentence_index - num_preceding): sentence_index]
+        return adjacent_sentences
+
+
+    def following_sentences(self, sentence, num_following=2):
+        sentences = self.sentences
+        sentence_index = sentences.index(sentence)
+        adjacent_sentences = sentences[sentence_index + 1: sentence_index + num_following + 1]
+        return adjacent_sentences
+
 
     def _element_distance(self, element_a, element_b):
         """
         This method works by getting the indices for the elements. The elements between are
         counted, with each heading in between being a section.
 
         Because of the way this works, the elements must be those directly contained by the document,
```

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/doc/document_cacher.py` & `chemdataextractor2-2.3.2/chemdataextractor/doc/document_cacher.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,14 +65,21 @@
         with open(self._document_subsentence_cache_path(cache_location_root), "w+") as f:
             for sentence in sentences:
                 indices = []
                 for subsentence in sentence.subsentences:
                     indices.append([token.index for token in subsentence.tokens])
                 f.write(str(indices) + "\n")
 
+        with open(self._document_subsentence_cache_path(cache_location_root), "w+") as f:
+            for sentence in sentences:
+                indices = []
+                for subsentence in sentence.subsentences:
+                    indices.append([token.index for token in subsentence.tokens])
+                f.write(str(indices) + "\n")
+
     def hydrate_document(self, document, document_id, tags=None):
         # Add in all the tags, tokenisation for a document.
         document_configuration = get_document_configuration(document)
         cache_location_root = os.path.join(self.cache_location, self._safe_document_id(document_id))
 
         # Check cache looks good
         if not os.path.isdir(cache_location_root):
@@ -140,15 +147,15 @@
                 if len(subsentences) == 1:
                     subsentences[0]._is_only_subsentence = True
                 sentence._subsentences = subsentences
 
         return document
 
     def _safe_document_id(self, document_id):
-        return document_id.replace(".", "🔥")
+        return document_id.replace(".", "🔥").replace("/", "😅")
 
     def _document_config_path(self, cache_location_root):
         return os.path.join(cache_location_root, "configuration.json")
 
     def _document_subsentence_cache_path(self, cache_location_root):
         return os.path.join(cache_location_root, "subsentences.txt")
```

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/doc/element.py` & `chemdataextractor2-2.3.2/chemdataextractor/doc/element.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/doc/figure.py` & `chemdataextractor2-2.3.2/chemdataextractor/doc/figure.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/doc/meta.py` & `chemdataextractor2-2.3.2/chemdataextractor/doc/meta.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/doc/table.py` & `chemdataextractor2-2.3.2/chemdataextractor/doc/table.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/doc/text.py` & `chemdataextractor2-2.3.2/chemdataextractor/doc/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 from ..model.model import Compound, NmrSpectrum, IrSpectrum, UvvisSpectrum, MeltingPoint, GlassTransition
 from ..model.contextual_range import SentenceRange
 
 
 
 log = logging.getLogger(__name__)
 cem_tagger = CemTagger()
+dep_tagger = DependencyTagger()
 
 
 @python_2_unicode_compatible
 class BaseText(BaseElement):
     """Abstract base class for a text Document Element."""
     taggers = []
     """
@@ -181,15 +182,15 @@
 class Text(collections.Sequence, BaseText):
     """A passage of text, comprising one or more sentences."""
 
     sentence_tokenizer = ChemSentenceTokenizer()
     word_tokenizer = BertWordTokenizer()
     lexicon = ChemLexicon()
     abbreviation_detector = ChemAbbreviationDetector()
-    taggers = [ChemCrfPosTagger(), cem_tagger, DependencyTagger()]
+    taggers = [ChemCrfPosTagger(), cem_tagger, dep_tagger]
     subsentence_extractor = None
 
     def __init__(self, text, sentence_tokenizer=None, word_tokenizer=None, lexicon=None, abbreviation_detector=None, pos_tagger=None, ner_tagger=None, parsers=None, **kwargs):
         """
         .. note::
 
             If intended as part of a :class:`~chemdataextractor.doc.document.Document`,
@@ -508,15 +509,15 @@
 class Sentence(BaseText):
     """A single sentence within a text passage."""
 
     word_tokenizer = BertWordTokenizer()
     lexicon = ChemLexicon()
     abbreviation_detector = ChemAbbreviationDetector()
     subsentence_extractor = SubsentenceExtractor()
-    taggers = [ChemCrfPosTagger(), cem_tagger, DependencyTagger()]
+    taggers = [ChemCrfPosTagger(), cem_tagger, dep_tagger]
     specifier_definition = specifier_definition
 
     def __init__(self, text, start=0, end=None, word_tokenizer=None, lexicon=None, abbreviation_detector=None, pos_tagger=None, ner_tagger=None, specifier_definition=None, subsentence_extractor=None, **kwargs):
         """
         .. note::
 
             If intended as part of a :class:`chemdataextractor.doc.document.Document`,
@@ -876,15 +877,15 @@
 
         i = 0
         length = len(records)
         while i < length:
             j = 0
             while j < length:
                 if i != j:
-                    records[j].merge_all(records[i])
+                    records[j].merge_all(records[i], distance=0*SentenceRange())
                 j += 1
             i += 1
 
         cleaned_records = []
         for record in records:
             record._clean(clean_contextual=False)
             if record.noncontextual_required_fulfilled:
@@ -912,14 +913,15 @@
                 ner_tagger=self.ner_tagger,
             )
             return merged
         return NotImplemented
 
 
 class Subsentence(Sentence):
+
     """
     A sub-sentence level logical division of text. Used to store clauses in CDE based on clause extraction as described
     in the paper Automated Construction of a Photocatalysis Dataset for Water-Splitting Applications
     (https://www.nature.com/articles/s41597-023-02511-6).
     An example of subsentences would be “A has quality α” and “A has quality β” from the sentence
     “A has quality α and quality β”. This enables rule-based and template-based parsing to adapt to a wider range
     of sentences.
@@ -942,18 +944,27 @@
         seen_labels = set()
         skip_parsers = self.document.skip_parsers if self.document is not None else []
 
         for model in self._streamlined_models:
             for parser in model.parsers:
                 if parser in skip_parsers:
                     continue
-                if hasattr(parser, 'parse_sentence'):
+                if hasattr(parser, 'parse_sentence') or hasattr(parser, "batch_parse_sentences"):
                     if (parser.parse_full_sentence != self.is_full_sentence) and not self._is_only_subsentence:
                         continue
-                    for record in parser.parse_sentence(self):
+                    parser_records = []
+                    # Add batch parsed records
+                    if (
+                        parser not in skip_parsers
+                        and hasattr(parser, "_batch_parsed_records_dict")
+                        and id(self.parent_sentence) in parser._batch_parsed_records_dict
+                    ):
+                        parser_records.extend(parser._batch_parsed_records_dict[id(self.parent_sentence)])
+                    parser_records.extend(parser.parse_sentence(self))
+                    for record in parser_records:
                         p = record.serialize()
                         if record.is_empty:  # TODO: Potential performance issues?
                             continue
                         # Skip duplicate records
                         if record in records:
                             continue
                         # Skip just labels that have already been seen (bit of a hack)
@@ -979,15 +990,15 @@
                         records.append(record)
         i = 0
         length = len(records)
         while i < length:
             j = 0
             while j < length:
                 if i != j:
-                    records[j].merge_all(records[i])
+                    records[j].merge_all(records[i], distance=0*SentenceRange())
                 j += 1
             i += 1
         return records
 
 
 class Cell(Sentence):
     """Data cell for tables. One row of the category table"""
```

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/errors.py` & `chemdataextractor2-2.3.2/chemdataextractor/errors.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/eval/evaluation.py` & `chemdataextractor2-2.3.2/chemdataextractor/eval/evaluation.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/fastner.py` & `chemdataextractor2-2.3.2/chemdataextractor/fastner.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/model/base.py` & `chemdataextractor2-2.3.2/chemdataextractor/model/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -383,22 +383,28 @@
             if key not in raw_data:
                 setattr(self, key, copy.copy(field.default))
         self._record_method = None
         self.was_updated = self._updated
         # Keep track of the number of times we've merged contextually.
         # This is then used to diminish the confidence if we've merged many times.
         self._contextual_merge_count = 0
+        self._no_merge_ranges = {}
 
     @classmethod
     def deserialize(cls, serialized):
         record = cls()
         flattened_serialized = cls._flatten_serialized(serialized)
         cleaned_serialized = [(cls._clean_key(key), value) for (key, value) in flattened_serialized]
         for key, value in cleaned_serialized:
-            record[key] = value
+            if isinstance(cls.fields[key[0]], ListType) and isinstance(cls.fields[key[0]].field, ModelType):
+                model = cls.fields[key[0]].field.model_class
+                value = [model.deserialize(val) for val in value]
+                record[key] = value
+            else:
+                record[key] = value
         return record
 
     @classmethod
     def _flatten_serialized(cls, serialized):
         flattened = []
         for key, value in serialized.items():
             if isinstance(value, dict):
@@ -575,15 +581,15 @@
                     self[key[0]] = created_attr
 
                 if len(key) == 1:
                     return attribute
                 else:
                     if isinstance(attribute, list):
                         attribute = attribute[0]
-                    return attribute[key[1:]]
+                    return attribute._get_item(key[1:], create_defaults=create_defaults)
         except AttributeError as e:
             pass
         raise KeyError(key)
 
     def __setitem__(self, key, value):
         """Redirect dictionary-style field setting to attribute-style."""
         if not isinstance(key, list):
@@ -854,45 +860,54 @@
                 for field_name, field in six.iteritems(self.fields):
                     if hasattr(field, 'field') and hasattr(field.field, 'model_class') and isinstance(other, field.field.model_class):
                         log.debug('model class list case')
                         # Basic merging in of lists/sets of models by just creating a list with one element
                         if (not field.never_merge
                             and field.contextual
                             and not self[field_name]
-                            and other and distance <= self.contextual_range(field_name)):
+                            and other
+                            and distance <= self.contextual_range(field_name)
+                            and distance > self.no_merge_range(field_name)
+                        ):
                             log.debug(field_name)
                             self[field_name] = [other]
                             # self.merge_confidence(other, field_name)
                             did_merge = True
                     elif hasattr(field, 'model_class') and isinstance(other, field.model_class) and not field.never_merge:
                         # Merging when there already exists a partial record
                         if (self[field_name] is not None
                             and field.contextual
                             and not self[field_name].contextual_fulfilled
-                            and distance <= self.contextual_range(field_name)):
+                            and distance <= self.contextual_range(field_name)
+                            and distance > self.no_merge_range(field_name)
+                        ):
                             log.debug('reconciling model classes')
                             if self[field_name].merge_contextual(other):
                                 did_merge = True
                         # Merging when there is no partial record
                         elif (field.contextual
                               and not self[field_name]
                               and other
-                              and distance <= self.contextual_range(field_name)):
+                              and distance <= self.contextual_range(field_name)
+                              and distance > self.no_merge_range(field_name)
+                            ):
                             log.debug(field_name)
                             self[field_name] = copy.copy(other)
                             # self.merge_confidence(other, field_name)
                             did_merge = True
             # Case when merging two records of the same type
             elif self._compatible(other):
                 for field_name, field in six.iteritems(self.fields):
                     if (field.contextual
                        and not field.never_merge
                        and not self[field_name]
                        and other.get(field_name, None)
-                       and distance <= self.contextual_range(field_name)):
+                       and distance <= self.contextual_range(field_name)
+                       and distance > self.no_merge_range(field_name)
+                    ):
                         self[field_name] = other[field_name]
                         self.merge_confidence(other, field_name)
                         did_merge = True
         self._consolidate_binding()
         if did_merge:
             self._contextual_merge_count += 1
             if 'self' in other._confidences:
@@ -907,15 +922,27 @@
 
         :param str field_name: The name of the field for which to calculate the contextual range
         :return: The contextual range for the field given the current record
         :rtype: ContextualRange
         """
         return self.fields[field_name].contextual_range
 
-    def merge_all(self, other, strict=True):
+    def no_merge_range(self, field_name):
+        """
+        A range within which the model should not be merging the field
+
+        :param str field_name: The name of the field for which to calculate the contextual range
+        :return: The contextual range within which the field should not be merged given the current record
+        :rtype: ContextualRange
+        """
+        if field_name in self._no_merge_ranges:
+            return self._no_merge_ranges[field_name]
+        return 0 * SentenceRange()
+
+    def merge_all(self, other, strict=True, distance=SentenceRange()):
         """
         Merges any properties between other and self, regardless of whether that field is contextual.
         Checks to make sure that there are no conflicts between the values contained in self and those in other.
 
         .. note::
 
             This method mutates the model it's called on **and** returns it.
@@ -935,38 +962,51 @@
                 if type(other) not in type(self).flatten():
                     # If the type of the other is not part of the flattened model,
                     # no point trying to merge
                     return False
                 for field_name, field in six.iteritems(self.fields):
                     if hasattr(field, 'field') and hasattr(field.field, 'model_class') and isinstance(other, field.field.model_class) and not field.never_merge:
                         log.debug('model list case')
-                        if self[field_name]:
+                        if (
+                            self[field_name]
+                            and distance > self.no_merge_range(field_name)
+                        ):
                             for el in self[field_name]:
                                 if el.merge_all(other):
                                     did_merge = True
                         elif (not self[field_name]
-                              and other):
+                              and other
+                              and distance > self.no_merge_range(field_name)):
                             log.debug(field_name)
                             self[field_name] = [copy.copy(other)]
                             did_merge = True
                     elif hasattr(field, 'model_class') and isinstance(other, field.model_class) and not field.never_merge:
                         log.debug('model class case')
-                        if self[field_name]:
+                        if (
+                            self[field_name]
+                            and distance > self.no_merge_range(field_name)
+                        ):
                             if self[field_name].merge_all(other):
                                 did_merge = True
-                        elif (not self[field_name]
-                              and other):
+                        elif (
+                            not self[field_name]
+                            and other
+                            and distance > self.no_merge_range(field_name)
+                        ):
                             log.debug(field_name)
                             self[field_name] = copy.copy(other)
                             did_merge = True
             elif self._compatible(other):
                 for field_name, field in six.iteritems(self.fields):
-                    if (not self[field_name]
-                      and other.get(field_name, None)
-                      and not field.never_merge):
+                    if (
+                        not self[field_name]
+                        and other.get(field_name, None)
+                        and not field.never_merge
+                        and distance > self.no_merge_range(field_name)
+                    ):
                         did_merge = True
                         self[field_name] = other[field_name]
                         self.merge_confidence(other, field_name)
         self._consolidate_binding()
         if did_merge:
             if 'self' in other._confidences:
                 self.merge_confidence(other, 'self')
```

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/model/contextual_range.py` & `chemdataextractor2-2.3.2/chemdataextractor/model/contextual_range.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/model/model.py` & `chemdataextractor2-2.3.2/chemdataextractor/model/model.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/model/units/__init__.py` & `chemdataextractor2-2.3.2/chemdataextractor/model/units/__init__.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/model/units/angle.py` & `chemdataextractor2-2.3.2/chemdataextractor/model/units/angle.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/model/units/charge.py` & `chemdataextractor2-2.3.2/chemdataextractor/model/units/charge.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/model/units/current.py` & `chemdataextractor2-2.3.2/chemdataextractor/model/units/current.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/model/units/dimension.py` & `chemdataextractor2-2.3.2/chemdataextractor/model/units/dimension.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/model/units/electric_potential.py` & `chemdataextractor2-2.3.2/chemdataextractor/model/units/electric_potential.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/model/units/energy.py` & `chemdataextractor2-2.3.2/chemdataextractor/model/units/energy.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/model/units/length.py` & `chemdataextractor2-2.3.2/chemdataextractor/model/units/length.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/model/units/mass.py` & `chemdataextractor2-2.3.2/chemdataextractor/model/units/mass.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/model/units/power.py` & `chemdataextractor2-2.3.2/chemdataextractor/model/units/power.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/model/units/quantity_model.py` & `chemdataextractor2-2.3.2/chemdataextractor/model/units/quantity_model.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/model/units/ratio.py` & `chemdataextractor2-2.3.2/chemdataextractor/model/units/ratio.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/model/units/substance_amount.py` & `chemdataextractor2-2.3.2/chemdataextractor/model/units/substance_amount.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/model/units/temperature.py` & `chemdataextractor2-2.3.2/chemdataextractor/model/units/temperature.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/model/units/time.py` & `chemdataextractor2-2.3.2/chemdataextractor/model/units/time.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/model/units/unit.py` & `chemdataextractor2-2.3.2/chemdataextractor/model/units/unit.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/nlp/__init__.py` & `chemdataextractor2-2.3.2/chemdataextractor/nlp/__init__.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/nlp/abbrev.py` & `chemdataextractor2-2.3.2/chemdataextractor/nlp/abbrev.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/nlp/allennlpwrapper.py` & `chemdataextractor2-2.3.2/chemdataextractor/nlp/allennlpwrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,22 +110,20 @@
         if archive_location is None:
             archive_location = find_data(self.model)
         self._weights_location = weights_location
         self._archive_location = archive_location
         self._predictor = None
         if self.overrides is None:
             self.overrides = {}
-
         self.min_batch_size = min_batch_size
         if min_batch_size is None:
-            self.min_batch_size = 100
-
+            self.min_batch_size = 50
         self.max_batch_size = max_batch_size
         if max_batch_size is None:
-            self.max_batch_size = 200
+            self.max_batch_size = 100
 
         self.max_allowed_length = max_allowed_length
         if max_allowed_length is None:
             self.max_allowed_length = 220
 
     def process(self, tag):
         """
```

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/nlp/cem.py` & `chemdataextractor2-2.3.2/chemdataextractor/nlp/cem.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/nlp/corenlp_dependency.py` & `chemdataextractor2-2.3.2/chemdataextractor/nlp/corenlp_dependency.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/nlp/corpus.py` & `chemdataextractor2-2.3.2/chemdataextractor/nlp/corpus.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/nlp/dependency.py` & `chemdataextractor2-2.3.2/chemdataextractor/nlp/dependency.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 class _DependencyTagger(BaseTagger):
 
     tag_type = "dependency"
 
     def __init__(self):
         try:
             self._nlp = stanza.Pipeline("en", tokenize_pretokenized=True, logging_level="ERROR")
-        except Exception:
+        except Exception as e:
+            print(f"Downloading stanza due to error {e}")
             stanza.download("en", resources_version="1.1.0")
             self._nlp = stanza.Pipeline("en", tokenize_pretokenized=True, logging_level="ERROR")
 
     def _tokens_to_stanza_tokens(self, tokens):
         return [token.text for token in tokens]
 
     def tag(self, tokens):
```

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/nlp/finetuned_bert_crf_wrapper.py` & `chemdataextractor2-2.3.2/chemdataextractor/nlp/finetuned_bert_crf_wrapper.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/nlp/lexicon.py` & `chemdataextractor2-2.3.2/chemdataextractor/nlp/lexicon.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/nlp/new_cem.py` & `chemdataextractor2-2.3.2/chemdataextractor/nlp/new_cem.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/nlp/pos.py` & `chemdataextractor2-2.3.2/chemdataextractor/nlp/pos.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/nlp/spacy_dependency.py` & `chemdataextractor2-2.3.2/chemdataextractor/nlp/spacy_dependency.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/nlp/subsentence.py` & `chemdataextractor2-2.3.2/chemdataextractor/nlp/subsentence.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/nlp/tag.py` & `chemdataextractor2-2.3.2/chemdataextractor/nlp/tag.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/nlp/tokenize.py` & `chemdataextractor2-2.3.2/chemdataextractor/nlp/tokenize.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/parse/__init__.py` & `chemdataextractor2-2.3.2/chemdataextractor/parse/__init__.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/parse/actions.py` & `chemdataextractor2-2.3.2/chemdataextractor/parse/actions.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/parse/apparatus.py` & `chemdataextractor2-2.3.2/chemdataextractor/parse/apparatus.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/parse/auto.py` & `chemdataextractor2-2.3.2/chemdataextractor/parse/auto.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,20 +33,25 @@
 
 from lxml.builder import E
 import xml.etree.ElementTree as etree
 
 log = logging.getLogger(__name__)
 
 
-def construct_unit_element(dimensions):
+def construct_unit_element(dimensions, max_power=None):
     """
     Construct an element for detecting units for the dimensions given.
     Any magnitude modifiers (e.g. kilo) will be automatically handled.
 
     :param Dimension dimensions: The dimensions that the element produced will look for.
+    :param int max_power: The maximum absolute value of the power that can be on any unit.
+        Default is None, where any power is allowed, but this can lead to false positives for things like GenericExtractor,
+        and it's actually unlikely that we'll ever get a unit to the power of 10 or something.
+        .. note::
+            This can only be a number between 2 and 9 due to how it has been implemented.
     :returns: An Element to look for units of given dimensions. If None or Dimensionless are passed in, returns None.
     :rtype: BaseParserElement or None
     """
     if not dimensions or not dimensions.units_dict:
         return None
     # Handle all the magnitudes
     units_regex = '^(('
@@ -57,16 +62,26 @@
     units_regex += '('
     # Case where we have a token that's just brackets
     units_regex += r'((\(|\[))|((\)|\]))|\-|'
     # Handle all the units
     for element in dimensions.units_dict:
         units_regex += '(' + element.pattern + ')|'
     units_regex += r'(\/)'
+    numbers_regex = r'\d+'
+    if max_power is not None:
+        if not isinstance(max_power, int):
+            raise TypeError(f"max_power should be an integer, not {type(max_power)}")
+        elif max_power <= 2:
+            raise ValueError(f"max_power should be greater than or equal to 2, not {max_power}")
+        elif max_power > 9:
+            raise ValueError(f"max_power should be less than or equal to 9 due to the implementation, not {max_power}")
+        else:
+            numbers_regex = f'[2-{max_power}]'
     # Case when we have powers, or one or more units
-    units_regex2 = units_regex + r'|([\+\-–−]?\d+(\.\d+)?)'
+    units_regex2 = units_regex + r'|([\+\-–−]?' + numbers_regex + r'(\.' + numbers_regex + ')?)'
     units_regex2 += '))+$'
     units_regex += '))+'
     units_regex += (units_regex2[1:-2] + '*')
     units_regex += '$'
     return (R(pattern=units_regex) + ZeroOrMore(R(pattern=units_regex) | R(pattern=units_regex2))).add_action(_clean_units_results)
```

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/parse/auto_dependency.py` & `chemdataextractor2-2.3.2/chemdataextractor/parse/auto_dependency.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/parse/base.py` & `chemdataextractor2-2.3.2/chemdataextractor/parse/base.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/parse/category.py` & `chemdataextractor2-2.3.2/chemdataextractor/parse/category.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/parse/cem.py` & `chemdataextractor2-2.3.2/chemdataextractor/parse/cem.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/parse/cem_factory.py` & `chemdataextractor2-2.3.2/chemdataextractor/parse/cem_factory.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/parse/common.py` & `chemdataextractor2-2.3.2/chemdataextractor/parse/common.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/parse/context.py` & `chemdataextractor2-2.3.2/chemdataextractor/parse/context.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/parse/definitions.py` & `chemdataextractor2-2.3.2/chemdataextractor/parse/definitions.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/parse/elements.py` & `chemdataextractor2-2.3.2/chemdataextractor/parse/elements.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/parse/ir.py` & `chemdataextractor2-2.3.2/chemdataextractor/parse/ir.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/parse/mp.py` & `chemdataextractor2-2.3.2/chemdataextractor/parse/mp.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/parse/mp_new.py` & `chemdataextractor2-2.3.2/chemdataextractor/parse/mp_new.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/parse/new_parsers.py` & `chemdataextractor2-2.3.2/chemdataextractor/parse/new_parsers.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/parse/nmr.py` & `chemdataextractor2-2.3.2/chemdataextractor/parse/nmr.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/parse/quantity.py` & `chemdataextractor2-2.3.2/chemdataextractor/parse/quantity.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/parse/template.py` & `chemdataextractor2-2.3.2/chemdataextractor/parse/template.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/parse/tg.py` & `chemdataextractor2-2.3.2/chemdataextractor/parse/tg.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/parse/uvvis.py` & `chemdataextractor2-2.3.2/chemdataextractor/parse/uvvis.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/reader/__init__.py` & `chemdataextractor2-2.3.2/chemdataextractor/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/reader/acs.py` & `chemdataextractor2-2.3.2/chemdataextractor/reader/acs.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/reader/base.py` & `chemdataextractor2-2.3.2/chemdataextractor/reader/base.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/reader/cssp.py` & `chemdataextractor2-2.3.2/chemdataextractor/reader/cssp.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/reader/elsevier.py` & `chemdataextractor2-2.3.2/chemdataextractor/reader/elsevier.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/reader/markup.py` & `chemdataextractor2-2.3.2/chemdataextractor/reader/markup.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/reader/nlm.py` & `chemdataextractor2-2.3.2/chemdataextractor/reader/nlm.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/reader/pdf.py` & `chemdataextractor2-2.3.2/chemdataextractor/reader/pdf.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/reader/plaintext.py` & `chemdataextractor2-2.3.2/chemdataextractor/reader/plaintext.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/reader/rsc.py` & `chemdataextractor2-2.3.2/chemdataextractor/reader/rsc.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/reader/springer.py` & `chemdataextractor2-2.3.2/chemdataextractor/reader/springer.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/reader/springer_jats.py` & `chemdataextractor2-2.3.2/chemdataextractor/reader/springer_jats.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/reader/uspto.py` & `chemdataextractor2-2.3.2/chemdataextractor/reader/uspto.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/relex/__init__.py` & `chemdataextractor2-2.3.2/chemdataextractor/relex/__init__.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/relex/candidate_parser.py` & `chemdataextractor2-2.3.2/chemdataextractor/relex/candidate_parser.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/relex/cluster.py` & `chemdataextractor2-2.3.2/chemdataextractor/relex/cluster.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/relex/entity.py` & `chemdataextractor2-2.3.2/chemdataextractor/relex/entity.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/relex/pattern.py` & `chemdataextractor2-2.3.2/chemdataextractor/relex/pattern.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/relex/phrase.py` & `chemdataextractor2-2.3.2/chemdataextractor/relex/phrase.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/relex/relationship.py` & `chemdataextractor2-2.3.2/chemdataextractor/relex/relationship.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/relex/snowball.py` & `chemdataextractor2-2.3.2/chemdataextractor/relex/snowball.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/relex/utils.py` & `chemdataextractor2-2.3.2/chemdataextractor/relex/utils.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/scrape/__init__.py` & `chemdataextractor2-2.3.2/chemdataextractor/scrape/__init__.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/scrape/base.py` & `chemdataextractor2-2.3.2/chemdataextractor/scrape/base.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/scrape/clean.py` & `chemdataextractor2-2.3.2/chemdataextractor/scrape/clean.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/scrape/csstranslator.py` & `chemdataextractor2-2.3.2/chemdataextractor/scrape/csstranslator.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/scrape/entity.py` & `chemdataextractor2-2.3.2/chemdataextractor/scrape/entity.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/scrape/fields.py` & `chemdataextractor2-2.3.2/chemdataextractor/scrape/fields.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/scrape/pub/elsevier.py` & `chemdataextractor2-2.3.2/chemdataextractor/scrape/pub/elsevier.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/scrape/pub/nlm.py` & `chemdataextractor2-2.3.2/chemdataextractor/scrape/pub/nlm.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/scrape/pub/rsc.py` & `chemdataextractor2-2.3.2/chemdataextractor/scrape/pub/rsc.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/scrape/pub/springer.py` & `chemdataextractor2-2.3.2/chemdataextractor/scrape/pub/springer.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/scrape/scraper.py` & `chemdataextractor2-2.3.2/chemdataextractor/scrape/scraper.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/scrape/selector.py` & `chemdataextractor2-2.3.2/chemdataextractor/scrape/selector.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/text/__init__.py` & `chemdataextractor2-2.3.2/chemdataextractor/text/__init__.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/text/chem.py` & `chemdataextractor2-2.3.2/chemdataextractor/text/chem.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/text/latex.py` & `chemdataextractor2-2.3.2/chemdataextractor/text/latex.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/text/normalize.py` & `chemdataextractor2-2.3.2/chemdataextractor/text/normalize.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/text/processors.py` & `chemdataextractor2-2.3.2/chemdataextractor/text/processors.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor/utils.py` & `chemdataextractor2-2.3.2/chemdataextractor/utils.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/chemdataextractor2.egg-info/PKG-INFO` & `chemdataextractor2-2.3.2/chemdataextractor2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: chemdataextractor2
-Version: 2.2.2
+Version: 2.3.2
 Summary: A toolkit for extracting chemical information from the scientific literature.
 Home-page: https://github.com/CambridgeMolecularEngineering/ChemDataExtractor2
 Author: Matt Swain, Callum Court, Juraj Mavracic, Taketomo Isazawa, and contributors
 Author-email: m.swain@me.com, cc889@cam.ac.uk, jm2111@cam.ac.uk, ti250@cam.ac.uk
 License: MIT
 Keywords: text-mining mining chemistry cheminformatics nlp html xml science scientific
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
@@ -56,9 +55,7 @@
 License
 -------
 
 ChemDataExtractor v2 is licensed under the `MIT license`_, a permissive, business-friendly license for open source
 software.
 
 MIT license: https://github.com/CambridgeMolecularEngineering/ChemDataExtractor/blob/master/LICENSE
-
-
```

### Comparing `chemdataextractor2-2.2.2/examples/automatic_parsers.ipynb` & `chemdataextractor2-2.3.2/examples/automatic_parsers.ipynb`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/examples/automatic_parsing_for_tables.ipynb` & `chemdataextractor2-2.3.2/examples/automatic_parsing_for_tables.ipynb`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/examples/automatic_parsing_of_complex_models.ipynb` & `chemdataextractor2-2.3.2/examples/automatic_parsing_of_complex_models.ipynb`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/examples/extracting_a_custom_property.ipynb` & `chemdataextractor2-2.3.2/examples/extracting_a_custom_property.ipynb`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/examples/searching_rsc.ipynb` & `chemdataextractor2-2.3.2/examples/searching_rsc.ipynb`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/examples/template_parsers.ipynb` & `chemdataextractor2-2.3.2/examples/template_parsers.ipynb`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/examples/using_config_file.ipynb` & `chemdataextractor2-2.3.2/examples/using_config_file.ipynb`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/examples/using_snowball.ipynb` & `chemdataextractor2-2.3.2/examples/using_snowball.ipynb`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/scripts/chemdner.sh` & `chemdataextractor2-2.3.2/scripts/chemdner.sh`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/scripts/cluster.sh` & `chemdataextractor2-2.3.2/scripts/cluster.sh`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/scripts/melting_points_eval.py` & `chemdataextractor2-2.3.2/scripts/melting_points_eval.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/scripts/pos.sh` & `chemdataextractor2-2.3.2/scripts/pos.sh`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/setup.py` & `chemdataextractor2-2.3.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if os.path.exists('README.md'):
     long_description = open('README.md').read()
 else:
     long_description = '''A toolkit for extracting chemical information from the scientific literature.'''
 
 setup(
     name='chemdataextractor2',
-    version='2.2.2',
+    version='2.3.2',
     author='Matt Swain, Callum Court, Juraj Mavracic, Taketomo Isazawa, and contributors',
     author_email='m.swain@me.com, cc889@cam.ac.uk, jm2111@cam.ac.uk, ti250@cam.ac.uk',
     license='MIT',
     url='https://github.com/CambridgeMolecularEngineering/ChemDataExtractor2',
     packages=find_packages(),
     description='A toolkit for extracting chemical information from the scientific literature.',
     long_description=long_description,
@@ -31,15 +31,16 @@
         'beautifulsoup4',
         'boto3==1.15.18',
         'botocore==1.18.18',
         'click==6.7',
         'cssselect',
         'lxml',
         'nltk',
-        'pdfminer.six',
+        'pdfminer.six ; python_version >= "3.8"',
+        'pdfminer.six >=20160614, <=20220524 ; python_version < "3.8"',
         'python-dateutil',
         'requests==2.21.0',
         'six',
         'python-crfsuite',
         'tabledataextractor',
         'DAWG-Patched; python_version >= "3.7.0"',
         'DAWG; python_version < "3.7.0"',
@@ -51,15 +52,15 @@
         # 'scipy',
         'yaspin',
         'deprecation',
         'allennlp==0.9.0',
         'tokenizers==0.12.1',
         'scikit-learn==0.22.1',
         'overrides==3.1.0',
-        'stanza==1.2.0',
+        'stanza==1.6.1',
     ],
     classifiers=[
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 2',
```

### Comparing `chemdataextractor2-2.2.2/tests/data/acs/acs.jmedchem.6b00723.html` & `chemdataextractor2-2.3.2/tests/data/acs/acs.jmedchem.6b00723.html`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/data/elsevier/j.jnoncrysol.2017.07.006.xml` & `chemdataextractor2-2.3.2/tests/data/elsevier/j.jnoncrysol.2017.07.006.xml`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/data/elsevier/j.jnoncrysol.2018.02.024.xml` & `chemdataextractor2-2.3.2/tests/data/elsevier/j.jnoncrysol.2018.02.024.xml`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/data/relex/curie_temperatures.pkl` & `chemdataextractor2-2.3.2/tests/data/relex/curie_temperatures.pkl`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/data/relex/curie_temperatures_py2.pkl` & `chemdataextractor2-2.3.2/tests/data/relex/curie_temperatures_py2.pkl`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/data/relex/curie_training_set/b806499g.html` & `chemdataextractor2-2.3.2/tests/data/relex/curie_training_set/b806499g.html`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/data/relex/curie_training_set/c1jm13879k.html` & `chemdataextractor2-2.3.2/tests/data/relex/curie_training_set/c1jm13879k.html`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/data/relex/curie_training_set/c2jm33712f.html` & `chemdataextractor2-2.3.2/tests/data/relex/curie_training_set/c2jm33712f.html`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/data/relex/curie_training_set/c2nr11767c.html` & `chemdataextractor2-2.3.2/tests/data/relex/curie_training_set/c2nr11767c.html`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/data/relex/curie_training_set/c3nr33950e.html` & `chemdataextractor2-2.3.2/tests/data/relex/curie_training_set/c3nr33950e.html`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/data/relex/curie_training_set/c6cp00375c.html` & `chemdataextractor2-2.3.2/tests/data/relex/curie_training_set/c6cp00375c.html`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/data/rsc/10.1039_C6OB02074G.html` & `chemdataextractor2-2.3.2/tests/data/rsc/10.1039_C6OB02074G.html`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/data/rsc/searchresults.html` & `chemdataextractor2-2.3.2/tests/data/rsc/searchresults.html`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/data/rsc/test_paper.html` & `chemdataextractor2-2.3.2/tests/data/rsc/test_paper.html`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/data/springer/spr_test1.xml` & `chemdataextractor2-2.3.2/tests/data/springer/spr_test1.xml`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/data/tables/j.commatsci.2018.02.056.xml` & `chemdataextractor2-2.3.2/tests/data/tables/j.commatsci.2018.02.056.xml`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/data/tables/j.commatsci.2018.02.056_2.xml` & `chemdataextractor2-2.3.2/tests/data/tables/j.commatsci.2018.02.056_2.xml`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/data/tables/table_test.html` & `chemdataextractor2-2.3.2/tests/data/tables/table_test.html`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/data/test_cache/test_cache/subsentences.txt` & `chemdataextractor2-2.3.2/tests/data/test_cache/test_cache/subsentences.txt`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/data/test_cache/test_cache/tag__ner_tag.txt` & `chemdataextractor2-2.3.2/tests/data/test_cache/test_cache/tag__ner_tag.txt`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/data/test_cache/test_cache/tag__pos_tag.txt` & `chemdataextractor2-2.3.2/tests/data/test_cache/test_cache/tag__pos_tag.txt`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/data/test_cache/test_cache/tag__start_end.txt` & `chemdataextractor2-2.3.2/tests/data/test_cache/test_cache/tag__start_end.txt`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/data/test_cache/test_cache/tokenizer__BertWordTokenizer.txt` & `chemdataextractor2-2.3.2/tests/data/test_cache/test_cache/tokenizer__BertWordTokenizer.txt`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/data/uspto/US06840965B2.xml` & `chemdataextractor2-2.3.2/tests/data/uspto/US06840965B2.xml`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_biblio.py` & `chemdataextractor2-2.3.2/tests/test_biblio.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_doc_cache.py` & `chemdataextractor2-2.3.2/tests/test_doc_cache.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_doc_document.py` & `chemdataextractor2-2.3.2/tests/test_doc_document.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_doc_table.py` & `chemdataextractor2-2.3.2/tests/test_doc_table.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_doc_table_2.py` & `chemdataextractor2-2.3.2/tests/test_doc_table_2.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_doc_text.py` & `chemdataextractor2-2.3.2/tests/test_doc_text.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_extract.py` & `chemdataextractor2-2.3.2/tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_model.py` & `chemdataextractor2-2.3.2/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_model_contextual_range.py` & `chemdataextractor2-2.3.2/tests/test_model_contextual_range.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_model_units.py` & `chemdataextractor2-2.3.2/tests/test_model_units.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_nlp_abbrev.py` & `chemdataextractor2-2.3.2/tests/test_nlp_abbrev.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_nlp_cem.py` & `chemdataextractor2-2.3.2/tests/test_nlp_cem.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_nlp_pos.py` & `chemdataextractor2-2.3.2/tests/test_nlp_pos.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_nlp_sentence.py` & `chemdataextractor2-2.3.2/tests/test_nlp_sentence.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_nlp_tag.py` & `chemdataextractor2-2.3.2/tests/test_nlp_tag.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_nlp_tokenize.py` & `chemdataextractor2-2.3.2/tests/test_nlp_tokenize.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_parse_apparatus.py` & `chemdataextractor2-2.3.2/tests/test_parse_apparatus.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_parse_auto.py` & `chemdataextractor2-2.3.2/tests/test_parse_auto.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_parse_auto_dependency.py` & `chemdataextractor2-2.3.2/tests/test_parse_auto_dependency.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_parse_cem.py` & `chemdataextractor2-2.3.2/tests/test_parse_cem.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_parse_definitions.py` & `chemdataextractor2-2.3.2/tests/test_parse_definitions.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_parse_ir.py` & `chemdataextractor2-2.3.2/tests/test_parse_ir.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_parse_mp.py` & `chemdataextractor2-2.3.2/tests/test_parse_mp.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_parse_nmr.py` & `chemdataextractor2-2.3.2/tests/test_parse_nmr.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_parse_quantity.py` & `chemdataextractor2-2.3.2/tests/test_parse_quantity.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_parse_template.py` & `chemdataextractor2-2.3.2/tests/test_parse_template.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_parse_tg.py` & `chemdataextractor2-2.3.2/tests/test_parse_tg.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_parse_uvvis.py` & `chemdataextractor2-2.3.2/tests/test_parse_uvvis.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_reader_acs.py` & `chemdataextractor2-2.3.2/tests/test_reader_acs.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_reader_elsevier.py` & `chemdataextractor2-2.3.2/tests/test_reader_elsevier.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_reader_markup.py` & `chemdataextractor2-2.3.2/tests/test_reader_markup.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_reader_rsc.py` & `chemdataextractor2-2.3.2/tests/test_reader_rsc.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_reader_springer.py` & `chemdataextractor2-2.3.2/tests/test_reader_springer.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_reader_uspto.py` & `chemdataextractor2-2.3.2/tests/test_reader_uspto.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_reading_cell+fig.py` & `chemdataextractor2-2.3.2/tests/test_reading_cell+fig.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_relex_cluster.py` & `chemdataextractor2-2.3.2/tests/test_relex_cluster.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_relex_entity.py` & `chemdataextractor2-2.3.2/tests/test_relex_entity.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_relex_phrase.py` & `chemdataextractor2-2.3.2/tests/test_relex_phrase.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_relex_relationship.py` & `chemdataextractor2-2.3.2/tests/test_relex_relationship.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_relex_snowball.py` & `chemdataextractor2-2.3.2/tests/test_relex_snowball.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_relex_utils.py` & `chemdataextractor2-2.3.2/tests/test_relex_utils.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_scrape_clean.py` & `chemdataextractor2-2.3.2/tests/test_scrape_clean.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_scrape_entity.py` & `chemdataextractor2-2.3.2/tests/test_scrape_entity.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_scrape_fields.py` & `chemdataextractor2-2.3.2/tests/test_scrape_fields.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_scrape_rsc.py` & `chemdataextractor2-2.3.2/tests/test_scrape_rsc.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_scrape_selector.py` & `chemdataextractor2-2.3.2/tests/test_scrape_selector.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_text.py` & `chemdataextractor2-2.3.2/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `chemdataextractor2-2.2.2/tests/test_text_chem.py` & `chemdataextractor2-2.3.2/tests/test_text_chem.py`

 * *Files identical despite different names*

