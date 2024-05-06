# Comparing `tmp/nanomotif-0.3.0.tar.gz` & `tmp/nanomotif-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanomotif-0.3.0.tar", last modified: Fri May  3 10:18:33 2024, max compression
+gzip compressed data, was "nanomotif-0.3.1.tar", last modified: Mon May  6 09:14:25 2024, max compression
```

## Comparing `nanomotif-0.3.0.tar` & `nanomotif-0.3.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-05-03 10:18:33.492056 nanomotif-0.3.0/
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     1084 2023-09-06 10:54:37.000000 nanomotif-0.3.0/LICENSE
--rw-r--r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     7350 2024-05-03 10:18:33.492056 nanomotif-0.3.0/PKG-INFO
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     6794 2024-05-03 10:10:14.000000 nanomotif-0.3.0/README.md
-drwxrwxr-x   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-05-03 10:18:32.380055 nanomotif-0.3.0/nanomotif/
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      278 2024-01-23 08:11:50.000000 nanomotif-0.3.0/nanomotif/__init__.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)       22 2024-05-03 10:10:32.000000 nanomotif-0.3.0/nanomotif/_version.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)    11018 2024-05-03 08:31:51.000000 nanomotif-0.3.0/nanomotif/argparser.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     6016 2024-02-20 08:34:47.000000 nanomotif-0.3.0/nanomotif/bin_consensus.py
-drwxrwxr-x   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-05-03 10:18:32.752055 nanomotif-0.3.0/nanomotif/binnary/
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-03-29 17:11:23.000000 nanomotif-0.3.0/nanomotif/binnary/__init__.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)    13167 2024-03-29 17:11:23.000000 nanomotif-0.3.0/nanomotif/binnary/analysis.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)    15629 2024-05-03 08:31:42.000000 nanomotif-0.3.0/nanomotif/binnary/data_processing.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     3729 2024-05-03 08:31:42.000000 nanomotif-0.3.0/nanomotif/binnary/detect_contamination.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     3014 2024-05-03 08:31:42.000000 nanomotif-0.3.0/nanomotif/binnary/include_contigs.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      890 2024-03-29 17:11:23.000000 nanomotif-0.3.0/nanomotif/binnary/logging.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     9127 2024-05-03 08:31:42.000000 nanomotif-0.3.0/nanomotif/binnary/scoring.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      522 2024-03-29 17:11:23.000000 nanomotif-0.3.0/nanomotif/binnary/utils.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)    14165 2024-02-07 10:11:10.000000 nanomotif-0.3.0/nanomotif/candidate.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     1078 2024-05-03 08:31:51.000000 nanomotif-0.3.0/nanomotif/constants.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     1698 2023-11-17 10:28:11.000000 nanomotif-0.3.0/nanomotif/dataload.py
-drwxrwxr-x   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-05-03 10:18:32.792055 nanomotif-0.3.0/nanomotif/datasets/
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)       27 2024-03-29 17:11:23.000000 nanomotif-0.3.0/nanomotif/datasets/geobacillus-contig-bin.tsv
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)   176247 2024-03-29 17:11:23.000000 nanomotif-0.3.0/nanomotif/datasets/geobacillus-plasmids.assembly.fasta
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164) 26479844 2024-03-29 17:11:23.000000 nanomotif-0.3.0/nanomotif/datasets/geobacillus-plasmids.pileup.bed
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     1106 2024-03-29 17:11:23.000000 nanomotif-0.3.0/nanomotif/datasets.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)    28603 2024-05-03 08:31:52.000000 nanomotif-0.3.0/nanomotif/evaluate.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      539 2023-10-03 09:15:12.000000 nanomotif-0.3.0/nanomotif/feature.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      321 2023-11-19 13:30:13.000000 nanomotif-0.3.0/nanomotif/logger.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)    19829 2024-05-03 08:31:52.000000 nanomotif-0.3.0/nanomotif/main.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     1037 2024-02-19 12:26:57.000000 nanomotif-0.3.0/nanomotif/model.py
-drwxrwxr-x   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-05-03 10:18:33.168056 nanomotif-0.3.0/nanomotif/mtase_linker/
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)       47 2024-05-03 08:31:42.000000 nanomotif-0.3.0/nanomotif/mtase_linker/__init__.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     5051 2024-05-03 08:31:42.000000 nanomotif-0.3.0/nanomotif/mtase_linker/command.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     3615 2024-05-03 08:31:42.000000 nanomotif-0.3.0/nanomotif/mtase_linker/dependencies.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     5639 2023-10-16 10:50:49.000000 nanomotif-0.3.0/nanomotif/old_search_method.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      850 2024-01-23 09:46:13.000000 nanomotif-0.3.0/nanomotif/parallel.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     6202 2024-02-07 10:11:10.000000 nanomotif-0.3.0/nanomotif/postprocess.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     7193 2024-01-23 11:48:10.000000 nanomotif-0.3.0/nanomotif/scoremotifs.py
--rw-r--r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      197 2024-01-23 07:18:32.000000 nanomotif-0.3.0/nanomotif/seed.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)    20090 2024-02-19 12:26:57.000000 nanomotif-0.3.0/nanomotif/seq.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     2677 2024-02-26 13:37:04.000000 nanomotif-0.3.0/nanomotif/utils.py
-drwxrwxr-x   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-05-03 10:18:33.488056 nanomotif-0.3.0/nanomotif.egg-info/
--rw-r--r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     7350 2024-05-03 10:18:32.000000 nanomotif-0.3.0/nanomotif.egg-info/PKG-INFO
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     1714 2024-05-03 10:18:32.000000 nanomotif-0.3.0/nanomotif.egg-info/SOURCES.txt
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        1 2024-05-03 10:18:32.000000 nanomotif-0.3.0/nanomotif.egg-info/dependency_links.txt
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)       50 2024-05-03 10:18:32.000000 nanomotif-0.3.0/nanomotif.egg-info/entry_points.txt
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        1 2023-09-07 09:00:46.000000 nanomotif-0.3.0/nanomotif.egg-info/not-zip-safe
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      150 2024-05-03 10:18:32.000000 nanomotif-0.3.0/nanomotif.egg-info/requires.txt
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)       16 2024-05-03 10:18:32.000000 nanomotif-0.3.0/nanomotif.egg-info/top_level.txt
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)       38 2024-05-03 10:18:33.492056 nanomotif-0.3.0/setup.cfg
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      947 2024-05-03 08:31:42.000000 nanomotif-0.3.0/setup.py
-drwxrwxr-x   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-05-03 10:18:33.252056 nanomotif-0.3.0/tests/
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2023-10-17 07:22:50.000000 nanomotif-0.3.0/tests/__init__.py
-drwxrwxr-x   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-05-03 10:18:33.456056 nanomotif-0.3.0/tests/binnary/
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-03-29 17:11:23.000000 nanomotif-0.3.0/tests/binnary/__init__.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     2089 2024-05-03 08:31:42.000000 nanomotif-0.3.0/tests/binnary/conftest.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     1019 2024-03-29 17:11:23.000000 nanomotif-0.3.0/tests/binnary/test_arg_parser.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)    11132 2024-05-03 08:31:42.000000 nanomotif-0.3.0/tests/binnary/test_cli_commands.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     6352 2024-03-29 17:11:23.000000 nanomotif-0.3.0/tests/binnary/test_data_processing_functions.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     2585 2024-03-29 17:11:23.000000 nanomotif-0.3.0/tests/binnary/test_detect_contamination.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     1404 2024-03-29 17:11:23.000000 nanomotif-0.3.0/tests/binnary/test_generate_output.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     2132 2024-03-29 17:11:23.000000 nanomotif-0.3.0/tests/binnary/test_include_contigs.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     3317 2024-05-03 08:31:42.000000 nanomotif-0.3.0/tests/binnary/test_scoring.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      744 2024-03-29 17:11:23.000000 nanomotif-0.3.0/tests/binnary/test_utils.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     5405 2024-05-03 08:31:42.000000 nanomotif-0.3.0/tests/binnary/test_write_bins.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     7236 2023-11-17 09:23:51.000000 nanomotif-0.3.0/tests/test_candidate.py
--rw-r--r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     1365 2024-01-23 08:24:14.000000 nanomotif-0.3.0/tests/test_dataload.py
--rw-r--r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     2933 2024-01-23 09:52:43.000000 nanomotif-0.3.0/tests/test_motif_find.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-05-02 08:30:14.000000 nanomotif-0.3.0/tests/test_motif_score.py
+drwxrwxr-x   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-05-06 09:14:25.588185 nanomotif-0.3.1/
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     1084 2023-09-06 10:54:37.000000 nanomotif-0.3.1/LICENSE
+-rw-r--r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     7384 2024-05-06 09:14:25.584185 nanomotif-0.3.1/PKG-INFO
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     6828 2024-05-06 09:04:24.000000 nanomotif-0.3.1/README.md
+drwxrwxr-x   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-05-06 09:14:25.424185 nanomotif-0.3.1/nanomotif/
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      278 2024-01-23 08:11:50.000000 nanomotif-0.3.1/nanomotif/__init__.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)       22 2024-05-06 09:12:23.000000 nanomotif-0.3.1/nanomotif/_version.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)    11018 2024-05-06 09:04:17.000000 nanomotif-0.3.1/nanomotif/argparser.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     6016 2024-02-20 08:34:47.000000 nanomotif-0.3.1/nanomotif/bin_consensus.py
+drwxrwxr-x   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-05-06 09:14:25.444185 nanomotif-0.3.1/nanomotif/binnary/
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-03-29 17:11:23.000000 nanomotif-0.3.1/nanomotif/binnary/__init__.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)    13167 2024-03-29 17:11:23.000000 nanomotif-0.3.1/nanomotif/binnary/analysis.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)    15629 2024-05-06 09:04:17.000000 nanomotif-0.3.1/nanomotif/binnary/data_processing.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     3729 2024-05-06 09:04:17.000000 nanomotif-0.3.1/nanomotif/binnary/detect_contamination.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     3014 2024-05-06 09:04:17.000000 nanomotif-0.3.1/nanomotif/binnary/include_contigs.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      890 2024-03-29 17:11:23.000000 nanomotif-0.3.1/nanomotif/binnary/logging.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     9127 2024-05-06 09:04:17.000000 nanomotif-0.3.1/nanomotif/binnary/scoring.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      522 2024-03-29 17:11:23.000000 nanomotif-0.3.1/nanomotif/binnary/utils.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)    14165 2024-02-07 10:11:10.000000 nanomotif-0.3.1/nanomotif/candidate.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     1078 2024-05-03 08:31:51.000000 nanomotif-0.3.1/nanomotif/constants.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     1698 2023-11-17 10:28:11.000000 nanomotif-0.3.1/nanomotif/dataload.py
+drwxrwxr-x   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-05-06 09:14:25.448185 nanomotif-0.3.1/nanomotif/datasets/
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)       27 2024-03-29 17:11:23.000000 nanomotif-0.3.1/nanomotif/datasets/geobacillus-contig-bin.tsv
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)   176247 2024-03-29 17:11:23.000000 nanomotif-0.3.1/nanomotif/datasets/geobacillus-plasmids.assembly.fasta
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164) 26479844 2024-03-29 17:11:23.000000 nanomotif-0.3.1/nanomotif/datasets/geobacillus-plasmids.pileup.bed
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     1106 2024-03-29 17:11:23.000000 nanomotif-0.3.1/nanomotif/datasets.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)    28603 2024-05-03 08:31:52.000000 nanomotif-0.3.1/nanomotif/evaluate.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      539 2023-10-03 09:15:12.000000 nanomotif-0.3.1/nanomotif/feature.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      321 2023-11-19 13:30:13.000000 nanomotif-0.3.1/nanomotif/logger.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)    19493 2024-05-06 09:04:24.000000 nanomotif-0.3.1/nanomotif/main.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     1037 2024-02-19 12:26:57.000000 nanomotif-0.3.1/nanomotif/model.py
+drwxrwxr-x   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-05-06 09:14:25.568185 nanomotif-0.3.1/nanomotif/mtase_linker/
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)       47 2024-05-06 09:04:17.000000 nanomotif-0.3.1/nanomotif/mtase_linker/__init__.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     5051 2024-05-06 09:04:17.000000 nanomotif-0.3.1/nanomotif/mtase_linker/command.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     3615 2024-05-06 09:04:17.000000 nanomotif-0.3.1/nanomotif/mtase_linker/dependencies.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     5639 2023-10-16 10:50:49.000000 nanomotif-0.3.1/nanomotif/old_search_method.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      850 2024-01-23 09:46:13.000000 nanomotif-0.3.1/nanomotif/parallel.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     6202 2024-02-07 10:11:10.000000 nanomotif-0.3.1/nanomotif/postprocess.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     7193 2024-01-23 11:48:10.000000 nanomotif-0.3.1/nanomotif/scoremotifs.py
+-rw-r--r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      197 2024-01-23 07:18:32.000000 nanomotif-0.3.1/nanomotif/seed.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)    20090 2024-02-19 12:26:57.000000 nanomotif-0.3.1/nanomotif/seq.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     2677 2024-02-26 13:37:04.000000 nanomotif-0.3.1/nanomotif/utils.py
+drwxrwxr-x   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-05-06 09:14:25.584185 nanomotif-0.3.1/nanomotif.egg-info/
+-rw-r--r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     7384 2024-05-06 09:14:25.000000 nanomotif-0.3.1/nanomotif.egg-info/PKG-INFO
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     1714 2024-05-06 09:14:25.000000 nanomotif-0.3.1/nanomotif.egg-info/SOURCES.txt
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        1 2024-05-06 09:14:25.000000 nanomotif-0.3.1/nanomotif.egg-info/dependency_links.txt
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)       50 2024-05-06 09:14:25.000000 nanomotif-0.3.1/nanomotif.egg-info/entry_points.txt
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        1 2023-09-07 09:00:46.000000 nanomotif-0.3.1/nanomotif.egg-info/not-zip-safe
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      150 2024-05-06 09:14:25.000000 nanomotif-0.3.1/nanomotif.egg-info/requires.txt
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)       16 2024-05-06 09:14:25.000000 nanomotif-0.3.1/nanomotif.egg-info/top_level.txt
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)       38 2024-05-06 09:14:25.588185 nanomotif-0.3.1/setup.cfg
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      947 2024-05-06 09:04:17.000000 nanomotif-0.3.1/setup.py
+drwxrwxr-x   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-05-06 09:14:25.576185 nanomotif-0.3.1/tests/
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2023-10-17 07:22:50.000000 nanomotif-0.3.1/tests/__init__.py
+drwxrwxr-x   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-05-06 09:14:25.584185 nanomotif-0.3.1/tests/binnary/
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-03-29 17:11:23.000000 nanomotif-0.3.1/tests/binnary/__init__.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     2089 2024-05-06 09:04:17.000000 nanomotif-0.3.1/tests/binnary/conftest.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     1019 2024-03-29 17:11:23.000000 nanomotif-0.3.1/tests/binnary/test_arg_parser.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)    11132 2024-05-06 09:04:17.000000 nanomotif-0.3.1/tests/binnary/test_cli_commands.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     6352 2024-03-29 17:11:23.000000 nanomotif-0.3.1/tests/binnary/test_data_processing_functions.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     2585 2024-03-29 17:11:23.000000 nanomotif-0.3.1/tests/binnary/test_detect_contamination.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     1404 2024-03-29 17:11:23.000000 nanomotif-0.3.1/tests/binnary/test_generate_output.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     2132 2024-03-29 17:11:23.000000 nanomotif-0.3.1/tests/binnary/test_include_contigs.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     3317 2024-05-06 09:04:17.000000 nanomotif-0.3.1/tests/binnary/test_scoring.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      744 2024-03-29 17:11:23.000000 nanomotif-0.3.1/tests/binnary/test_utils.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     5405 2024-05-06 09:04:17.000000 nanomotif-0.3.1/tests/binnary/test_write_bins.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     7236 2023-11-17 09:23:51.000000 nanomotif-0.3.1/tests/test_candidate.py
+-rw-r--r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     1365 2024-01-23 08:24:14.000000 nanomotif-0.3.1/tests/test_dataload.py
+-rw-r--r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     2933 2024-01-23 09:52:43.000000 nanomotif-0.3.1/tests/test_motif_find.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-05-02 08:30:14.000000 nanomotif-0.3.1/tests/test_motif_score.py
```

### Comparing `nanomotif-0.3.0/LICENSE` & `nanomotif-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/PKG-INFO` & `nanomotif-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanomotif
-Version: 0.3.0
+Version: 0.3.1
 Summary: Identifying methlyation motifs in nanopore data
 Author: AAU_DarkScience
 Author-email: shei@bio.aau.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: wheel
@@ -44,15 +44,15 @@
 Please see the [documentation](https://nanomotif.readthedocs.io) for detailed installation and usage instructions, descriptions of required files, and analysis examples.
 
 
 ## Skip the Documentation: Your Quickstart Guide to Nanomotif
 
 ### Installation
 
-Using Conda for managing your Python environments, you can create a new environment and install Nanomotif as follows:
+Nanomotif can easily be installed using Conda for managing your Python environments. You can create a new environment and install Nanomotif as follows:
 ```shell
 conda create -n nanomotif  python=3.9
 conda activate nanomotif
 conda install -c bioconda nanomotif
 ```
 
 #### Check installation
```

### Comparing `nanomotif-0.3.0/README.md` & `nanomotif-0.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 Please see the [documentation](https://nanomotif.readthedocs.io) for detailed installation and usage instructions, descriptions of required files, and analysis examples.
 
 
 ## Skip the Documentation: Your Quickstart Guide to Nanomotif
 
 ### Installation
 
-Using Conda for managing your Python environments, you can create a new environment and install Nanomotif as follows:
+Nanomotif can easily be installed using Conda for managing your Python environments. You can create a new environment and install Nanomotif as follows:
 ```shell
 conda create -n nanomotif  python=3.9
 conda activate nanomotif
 conda install -c bioconda nanomotif
 ```
 
 #### Check installation
```

### Comparing `nanomotif-0.3.0/nanomotif/argparser.py` & `nanomotif-0.3.1/nanomotif/argparser.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/nanomotif/bin_consensus.py` & `nanomotif-0.3.1/nanomotif/bin_consensus.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/nanomotif/binnary/analysis.py` & `nanomotif-0.3.1/nanomotif/binnary/analysis.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/nanomotif/binnary/data_processing.py` & `nanomotif-0.3.1/nanomotif/binnary/data_processing.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/nanomotif/binnary/detect_contamination.py` & `nanomotif-0.3.1/nanomotif/binnary/detect_contamination.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/nanomotif/binnary/include_contigs.py` & `nanomotif-0.3.1/nanomotif/binnary/include_contigs.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/nanomotif/binnary/logging.py` & `nanomotif-0.3.1/nanomotif/binnary/logging.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/nanomotif/binnary/scoring.py` & `nanomotif-0.3.1/nanomotif/binnary/scoring.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/nanomotif/binnary/utils.py` & `nanomotif-0.3.1/nanomotif/binnary/utils.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/nanomotif/candidate.py` & `nanomotif-0.3.1/nanomotif/candidate.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/nanomotif/constants.py` & `nanomotif-0.3.1/nanomotif/constants.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/nanomotif/dataload.py` & `nanomotif-0.3.1/nanomotif/dataload.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/nanomotif/datasets/geobacillus-plasmids.assembly.fasta` & `nanomotif-0.3.1/nanomotif/datasets/geobacillus-plasmids.assembly.fasta`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/nanomotif/datasets/geobacillus-plasmids.pileup.bed` & `nanomotif-0.3.1/nanomotif/datasets/geobacillus-plasmids.pileup.bed`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/nanomotif/datasets.py` & `nanomotif-0.3.1/nanomotif/datasets.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/nanomotif/evaluate.py` & `nanomotif-0.3.1/nanomotif/evaluate.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/nanomotif/feature.py` & `nanomotif-0.3.1/nanomotif/feature.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/nanomotif/main.py` & `nanomotif-0.3.1/nanomotif/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,15 +273,15 @@
 
     output = nm.postprocess.join_motif_complements(output)
 
     output = output.rename({"contig":"bin", "n_mod":"n_mod_bin", "n_nomod":"n_nomod_bin"})
     output = output.sort(["bin", "mod_type", "motif"])
     output.write_csv(args.out + "/bin-motifs.tsv", separator="\t")
 
-def metagenomic_workflow(args):
+def motif_discovery(args):
     # Check if output directory exists
     log.info("Loading required files")
     pileup = nm.load_pileup(args.pileup, threads = args.threads, min_fraction = args.threshold_methylation_general)
     assembly = nm.load_assembly(args.assembly)
 
     # Find motifs
     log.info("Finding motifs")
@@ -481,27 +481,17 @@
     parser = nm.argparser.create_parser()
     args = parser.parse_args()
     
     if args.command in ["detect_contamination", "include_contigs", "MTase-linker"]:
         args.verbose = False
         args.seed = 1
     
-    
-    if args.command == "find-motifs":
-        shared_setup(args, args.out)
-        find_motifs(args)
-    elif args.command == "score-motifs":
-        shared_setup(args, args.out)
-        score_motifs(args)
-    elif args.command == "bin-consensus":
-        shared_setup(args, args.out)
-        bin_consensus(args)
-    elif args.command == "complete-workflow":
+    if args.command == "find_motifs":
         shared_setup(args, args.out)
-        metagenomic_workflow(args)
+        motif_discovery(args)
     elif args.command == "check-installation":
         args.out = "nanomotif_install_check"
         shared_setup(args, args.out)
         check_install(args)
 
     elif args.command in ["detect_contamination", "include_contigs"]:
         shared_setup(args, args.out)
```

### Comparing `nanomotif-0.3.0/nanomotif/model.py` & `nanomotif-0.3.1/nanomotif/model.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/nanomotif/mtase_linker/command.py` & `nanomotif-0.3.1/nanomotif/mtase_linker/command.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/nanomotif/mtase_linker/dependencies.py` & `nanomotif-0.3.1/nanomotif/mtase_linker/dependencies.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/nanomotif/old_search_method.py` & `nanomotif-0.3.1/nanomotif/old_search_method.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/nanomotif/parallel.py` & `nanomotif-0.3.1/nanomotif/parallel.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/nanomotif/postprocess.py` & `nanomotif-0.3.1/nanomotif/postprocess.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/nanomotif/scoremotifs.py` & `nanomotif-0.3.1/nanomotif/scoremotifs.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/nanomotif/seq.py` & `nanomotif-0.3.1/nanomotif/seq.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/nanomotif/utils.py` & `nanomotif-0.3.1/nanomotif/utils.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/nanomotif.egg-info/PKG-INFO` & `nanomotif-0.3.1/nanomotif.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanomotif
-Version: 0.3.0
+Version: 0.3.1
 Summary: Identifying methlyation motifs in nanopore data
 Author: AAU_DarkScience
 Author-email: shei@bio.aau.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: wheel
@@ -44,15 +44,15 @@
 Please see the [documentation](https://nanomotif.readthedocs.io) for detailed installation and usage instructions, descriptions of required files, and analysis examples.
 
 
 ## Skip the Documentation: Your Quickstart Guide to Nanomotif
 
 ### Installation
 
-Using Conda for managing your Python environments, you can create a new environment and install Nanomotif as follows:
+Nanomotif can easily be installed using Conda for managing your Python environments. You can create a new environment and install Nanomotif as follows:
 ```shell
 conda create -n nanomotif  python=3.9
 conda activate nanomotif
 conda install -c bioconda nanomotif
 ```
 
 #### Check installation
```

### Comparing `nanomotif-0.3.0/nanomotif.egg-info/SOURCES.txt` & `nanomotif-0.3.1/nanomotif.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/setup.py` & `nanomotif-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/tests/binnary/conftest.py` & `nanomotif-0.3.1/tests/binnary/conftest.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/tests/binnary/test_arg_parser.py` & `nanomotif-0.3.1/tests/binnary/test_arg_parser.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/tests/binnary/test_cli_commands.py` & `nanomotif-0.3.1/tests/binnary/test_cli_commands.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/tests/binnary/test_data_processing_functions.py` & `nanomotif-0.3.1/tests/binnary/test_data_processing_functions.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/tests/binnary/test_detect_contamination.py` & `nanomotif-0.3.1/tests/binnary/test_detect_contamination.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/tests/binnary/test_generate_output.py` & `nanomotif-0.3.1/tests/binnary/test_generate_output.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/tests/binnary/test_include_contigs.py` & `nanomotif-0.3.1/tests/binnary/test_include_contigs.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/tests/binnary/test_scoring.py` & `nanomotif-0.3.1/tests/binnary/test_scoring.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/tests/binnary/test_utils.py` & `nanomotif-0.3.1/tests/binnary/test_utils.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/tests/binnary/test_write_bins.py` & `nanomotif-0.3.1/tests/binnary/test_write_bins.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/tests/test_candidate.py` & `nanomotif-0.3.1/tests/test_candidate.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/tests/test_dataload.py` & `nanomotif-0.3.1/tests/test_dataload.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.0/tests/test_motif_find.py` & `nanomotif-0.3.1/tests/test_motif_find.py`

 * *Files identical despite different names*

