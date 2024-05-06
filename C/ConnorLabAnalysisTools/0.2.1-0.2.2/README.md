# Comparing `tmp/ConnorLabAnalysisTools-0.2.1.tar.gz` & `tmp/ConnorLabAnalysisTools-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ConnorLabAnalysisTools-0.2.1.tar", last modified: Mon Jan  8 22:26:34 2024, max compression
+gzip compressed data, was "ConnorLabAnalysisTools-0.2.2.tar", last modified: Mon May  6 14:38:10 2024, max compression
```

## Comparing `ConnorLabAnalysisTools-0.2.1.tar` & `ConnorLabAnalysisTools-0.2.2.tar`

### file list

```diff
@@ -1,59 +1,62 @@
-drwxrwxr-x   0 r2_allen  (1003) r2_allen  (1003)        0 2024-01-08 22:26:34.226883 ConnorLabAnalysisTools-0.2.1/
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)      281 2024-01-08 22:26:34.226883 ConnorLabAnalysisTools-0.2.1/PKG-INFO
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)       60 2023-10-17 19:04:46.000000 ConnorLabAnalysisTools-0.2.1/README.md
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)       38 2024-01-08 22:26:34.226883 ConnorLabAnalysisTools-0.2.1/setup.cfg
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)      583 2024-01-03 15:36:00.000000 ConnorLabAnalysisTools-0.2.1/setup.py
-drwxrwxr-x   0 r2_allen  (1003) r2_allen  (1003)        0 2024-01-08 22:26:34.218882 ConnorLabAnalysisTools-0.2.1/src/
-drwxrwxr-x   0 r2_allen  (1003) r2_allen  (1003)        0 2024-01-08 22:26:34.218882 ConnorLabAnalysisTools-0.2.1/src/ConnorLabAnalysisTools.egg-info/
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)      281 2024-01-08 22:26:34.000000 ConnorLabAnalysisTools-0.2.1/src/ConnorLabAnalysisTools.egg-info/PKG-INFO
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     1622 2024-01-08 22:26:34.000000 ConnorLabAnalysisTools-0.2.1/src/ConnorLabAnalysisTools.egg-info/SOURCES.txt
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)        1 2024-01-08 22:26:34.000000 ConnorLabAnalysisTools-0.2.1/src/ConnorLabAnalysisTools.egg-info/dependency_links.txt
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)      109 2024-01-08 22:26:34.000000 ConnorLabAnalysisTools-0.2.1/src/ConnorLabAnalysisTools.egg-info/requires.txt
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)        5 2024-01-08 22:26:34.000000 ConnorLabAnalysisTools-0.2.1/src/ConnorLabAnalysisTools.egg-info/top_level.txt
-drwxrwxr-x   0 r2_allen  (1003) r2_allen  (1003)        0 2024-01-08 22:26:34.218882 ConnorLabAnalysisTools-0.2.1/src/clat/
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)        0 2023-10-17 15:13:43.000000 ConnorLabAnalysisTools-0.2.1/src/clat/__init__.py
-drwxrwxr-x   0 r2_allen  (1003) r2_allen  (1003)        0 2024-01-08 22:26:34.218882 ConnorLabAnalysisTools-0.2.1/src/clat/compile/
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)        0 2023-10-03 18:07:38.000000 ConnorLabAnalysisTools-0.2.1/src/clat/compile/__init__.py
-drwxrwxr-x   0 r2_allen  (1003) r2_allen  (1003)        0 2024-01-08 22:26:34.222882 ConnorLabAnalysisTools-0.2.1/src/clat/compile/task/
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)        0 2023-10-03 18:07:38.000000 ConnorLabAnalysisTools-0.2.1/src/clat/compile/task/__init__.py
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     2464 2023-10-17 15:14:20.000000 ConnorLabAnalysisTools-0.2.1/src/clat/compile/task/base_database_fields.py
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     1841 2023-10-17 15:14:20.000000 ConnorLabAnalysisTools-0.2.1/src/clat/compile/task/compile_task_id.py
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     1305 2023-10-17 15:14:20.000000 ConnorLabAnalysisTools-0.2.1/src/clat/compile/task/matchstick_fields.py
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     2390 2024-01-08 17:15:14.000000 ConnorLabAnalysisTools-0.2.1/src/clat/compile/task/task_field.py
-drwxrwxr-x   0 r2_allen  (1003) r2_allen  (1003)        0 2024-01-08 22:26:34.222882 ConnorLabAnalysisTools-0.2.1/src/clat/compile/trial/
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)        0 2023-10-03 18:07:38.000000 ConnorLabAnalysisTools-0.2.1/src/clat/compile/trial/__init__.py
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     3240 2024-01-08 18:05:54.000000 ConnorLabAnalysisTools-0.2.1/src/clat/compile/trial/cached_fields.py
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     4336 2023-10-17 15:14:20.000000 ConnorLabAnalysisTools-0.2.1/src/clat/compile/trial/classic_database_fields.py
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     6012 2024-01-03 15:53:05.000000 ConnorLabAnalysisTools-0.2.1/src/clat/compile/trial/trial_collector.py
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     2062 2024-01-08 18:04:11.000000 ConnorLabAnalysisTools-0.2.1/src/clat/compile/trial/trial_field.py
-drwxrwxr-x   0 r2_allen  (1003) r2_allen  (1003)        0 2024-01-08 22:26:34.222882 ConnorLabAnalysisTools-0.2.1/src/clat/eyecal/
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)        0 2023-12-12 19:16:22.000000 ConnorLabAnalysisTools-0.2.1/src/clat/eyecal/__init__.py
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)      656 2023-12-18 21:10:41.000000 ConnorLabAnalysisTools-0.2.1/src/clat/eyecal/apply_eyecal.py
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     7360 2023-12-14 19:22:00.000000 ConnorLabAnalysisTools-0.2.1/src/clat/eyecal/params.py
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)    10907 2023-12-14 20:21:19.000000 ConnorLabAnalysisTools-0.2.1/src/clat/eyecal/plot_eyecal.py
-drwxrwxr-x   0 r2_allen  (1003) r2_allen  (1003)        0 2024-01-08 22:26:34.222882 ConnorLabAnalysisTools-0.2.1/src/clat/intan/
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)        0 2023-09-29 20:43:03.000000 ConnorLabAnalysisTools-0.2.1/src/clat/intan/__init__.py
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     4518 2023-10-17 15:52:02.000000 ConnorLabAnalysisTools-0.2.1/src/clat/intan/amplifiers.py
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     2690 2023-10-17 19:00:40.000000 ConnorLabAnalysisTools-0.2.1/src/clat/intan/channels.py
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     4861 2023-09-29 20:43:03.000000 ConnorLabAnalysisTools-0.2.1/src/clat/intan/livenotes.py
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     4477 2023-09-29 20:43:03.000000 ConnorLabAnalysisTools-0.2.1/src/clat/intan/marker_channels.py
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     1901 2023-10-17 16:01:05.000000 ConnorLabAnalysisTools-0.2.1/src/clat/intan/one_file_spike_parsing.py
-drwxrwxr-x   0 r2_allen  (1003) r2_allen  (1003)        0 2024-01-08 22:26:34.222882 ConnorLabAnalysisTools-0.2.1/src/clat/intan/rhd/
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)        0 2023-09-29 20:43:03.000000 ConnorLabAnalysisTools-0.2.1/src/clat/intan/rhd/__init__.py
-drwxrwxr-x   0 r2_allen  (1003) r2_allen  (1003)        0 2024-01-08 22:26:34.226883 ConnorLabAnalysisTools-0.2.1/src/clat/intan/rhd/intanutil/
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)        0 2023-09-29 20:43:03.000000 ConnorLabAnalysisTools-0.2.1/src/clat/intan/rhd/intanutil/__init__.py
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     2649 2023-09-29 20:43:03.000000 ConnorLabAnalysisTools-0.2.1/src/clat/intan/rhd/intanutil/data_to_result.py
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     1607 2023-09-29 20:43:03.000000 ConnorLabAnalysisTools-0.2.1/src/clat/intan/rhd/intanutil/get_bytes_per_data_block.py
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     1417 2023-09-29 20:43:03.000000 ConnorLabAnalysisTools-0.2.1/src/clat/intan/rhd/intanutil/notch_filter.py
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)      995 2023-09-29 20:43:03.000000 ConnorLabAnalysisTools-0.2.1/src/clat/intan/rhd/intanutil/qstring.py
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     6661 2023-10-17 15:57:41.000000 ConnorLabAnalysisTools-0.2.1/src/clat/intan/rhd/intanutil/read_header.py
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     3604 2023-09-29 20:43:03.000000 ConnorLabAnalysisTools-0.2.1/src/clat/intan/rhd/intanutil/read_one_data_block.py
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)    10280 2023-10-17 15:57:05.000000 ConnorLabAnalysisTools-0.2.1/src/clat/intan/rhd/load_intan_rhd_format.py
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     6565 2023-10-17 15:52:02.000000 ConnorLabAnalysisTools-0.2.1/src/clat/intan/spike_file.py
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     4106 2023-10-17 15:29:02.000000 ConnorLabAnalysisTools-0.2.1/src/clat/intan/stitch.py
-drwxrwxr-x   0 r2_allen  (1003) r2_allen  (1003)        0 2024-01-08 22:26:34.226883 ConnorLabAnalysisTools-0.2.1/src/clat/util/
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)        0 2023-10-03 18:07:38.000000 ConnorLabAnalysisTools-0.2.1/src/clat/util/__init__.py
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     3406 2023-12-13 20:32:24.000000 ConnorLabAnalysisTools-0.2.1/src/clat/util/connection.py
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     3482 2023-10-03 18:07:38.000000 ConnorLabAnalysisTools-0.2.1/src/clat/util/dictionary_util.py
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     3074 2023-10-17 15:14:20.000000 ConnorLabAnalysisTools-0.2.1/src/clat/util/table_util.py
--rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     3344 2024-01-03 20:12:22.000000 ConnorLabAnalysisTools-0.2.1/src/clat/util/time_util.py
+drwxrwxr-x   0 r2_allen  (1003) r2_allen  (1003)        0 2024-05-06 14:38:10.315781 ConnorLabAnalysisTools-0.2.2/
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)      281 2024-05-06 14:38:10.315781 ConnorLabAnalysisTools-0.2.2/PKG-INFO
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)       60 2023-10-17 19:04:46.000000 ConnorLabAnalysisTools-0.2.2/README.md
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)       38 2024-05-06 14:38:10.315781 ConnorLabAnalysisTools-0.2.2/setup.cfg
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)      583 2024-05-06 14:27:09.000000 ConnorLabAnalysisTools-0.2.2/setup.py
+drwxrwxr-x   0 r2_allen  (1003) r2_allen  (1003)        0 2024-05-06 14:38:10.307781 ConnorLabAnalysisTools-0.2.2/src/
+drwxrwxr-x   0 r2_allen  (1003) r2_allen  (1003)        0 2024-05-06 14:38:10.307781 ConnorLabAnalysisTools-0.2.2/src/ConnorLabAnalysisTools.egg-info/
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)      281 2024-05-06 14:38:10.000000 ConnorLabAnalysisTools-0.2.2/src/ConnorLabAnalysisTools.egg-info/PKG-INFO
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     1725 2024-05-06 14:38:10.000000 ConnorLabAnalysisTools-0.2.2/src/ConnorLabAnalysisTools.egg-info/SOURCES.txt
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)        1 2024-05-06 14:38:10.000000 ConnorLabAnalysisTools-0.2.2/src/ConnorLabAnalysisTools.egg-info/dependency_links.txt
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)      109 2024-05-06 14:38:10.000000 ConnorLabAnalysisTools-0.2.2/src/ConnorLabAnalysisTools.egg-info/requires.txt
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)        5 2024-05-06 14:38:10.000000 ConnorLabAnalysisTools-0.2.2/src/ConnorLabAnalysisTools.egg-info/top_level.txt
+drwxrwxr-x   0 r2_allen  (1003) r2_allen  (1003)        0 2024-05-06 14:38:10.307781 ConnorLabAnalysisTools-0.2.2/src/clat/
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)        0 2023-10-17 15:13:43.000000 ConnorLabAnalysisTools-0.2.2/src/clat/__init__.py
+drwxrwxr-x   0 r2_allen  (1003) r2_allen  (1003)        0 2024-05-06 14:38:10.307781 ConnorLabAnalysisTools-0.2.2/src/clat/compile/
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)        0 2023-10-03 18:07:38.000000 ConnorLabAnalysisTools-0.2.2/src/clat/compile/__init__.py
+drwxrwxr-x   0 r2_allen  (1003) r2_allen  (1003)        0 2024-05-06 14:38:10.311781 ConnorLabAnalysisTools-0.2.2/src/clat/compile/task/
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)        0 2023-10-03 18:07:38.000000 ConnorLabAnalysisTools-0.2.2/src/clat/compile/task/__init__.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     2464 2023-10-17 15:14:20.000000 ConnorLabAnalysisTools-0.2.2/src/clat/compile/task/base_database_fields.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     2947 2024-02-15 21:25:58.000000 ConnorLabAnalysisTools-0.2.2/src/clat/compile/task/cached_task_fields.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     1841 2023-10-17 15:14:20.000000 ConnorLabAnalysisTools-0.2.2/src/clat/compile/task/compile_task_id.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     1305 2023-10-17 15:14:20.000000 ConnorLabAnalysisTools-0.2.2/src/clat/compile/task/matchstick_fields.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     2712 2024-03-12 20:47:17.000000 ConnorLabAnalysisTools-0.2.2/src/clat/compile/task/task_field.py
+drwxrwxr-x   0 r2_allen  (1003) r2_allen  (1003)        0 2024-05-06 14:38:10.311781 ConnorLabAnalysisTools-0.2.2/src/clat/compile/trial/
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)        0 2023-10-03 18:07:38.000000 ConnorLabAnalysisTools-0.2.2/src/clat/compile/trial/__init__.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     4779 2024-03-04 20:42:57.000000 ConnorLabAnalysisTools-0.2.2/src/clat/compile/trial/cached_fields.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     4838 2024-03-04 17:15:52.000000 ConnorLabAnalysisTools-0.2.2/src/clat/compile/trial/classic_database_fields.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     7969 2024-01-17 16:44:09.000000 ConnorLabAnalysisTools-0.2.2/src/clat/compile/trial/trial_collector.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     2124 2024-02-15 17:04:18.000000 ConnorLabAnalysisTools-0.2.2/src/clat/compile/trial/trial_field.py
+drwxrwxr-x   0 r2_allen  (1003) r2_allen  (1003)        0 2024-05-06 14:38:10.311781 ConnorLabAnalysisTools-0.2.2/src/clat/eyecal/
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)        0 2023-12-12 19:16:22.000000 ConnorLabAnalysisTools-0.2.2/src/clat/eyecal/__init__.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)      656 2023-12-18 21:10:41.000000 ConnorLabAnalysisTools-0.2.2/src/clat/eyecal/apply_eyecal.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     7360 2023-12-14 19:22:00.000000 ConnorLabAnalysisTools-0.2.2/src/clat/eyecal/params.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)    11444 2024-04-17 16:25:57.000000 ConnorLabAnalysisTools-0.2.2/src/clat/eyecal/plot_eyecal.py
+drwxrwxr-x   0 r2_allen  (1003) r2_allen  (1003)        0 2024-05-06 14:38:10.311781 ConnorLabAnalysisTools-0.2.2/src/clat/intan/
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)        0 2023-09-29 20:43:03.000000 ConnorLabAnalysisTools-0.2.2/src/clat/intan/__init__.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     4518 2023-10-17 15:52:02.000000 ConnorLabAnalysisTools-0.2.2/src/clat/intan/amplifiers.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)      970 2024-02-29 20:02:42.000000 ConnorLabAnalysisTools-0.2.2/src/clat/intan/analogin.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     3090 2024-05-06 14:36:34.000000 ConnorLabAnalysisTools-0.2.2/src/clat/intan/channels.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     5549 2024-02-29 19:06:45.000000 ConnorLabAnalysisTools-0.2.2/src/clat/intan/livenotes.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     4477 2023-09-29 20:43:03.000000 ConnorLabAnalysisTools-0.2.2/src/clat/intan/marker_channels.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     1931 2024-05-05 16:07:19.000000 ConnorLabAnalysisTools-0.2.2/src/clat/intan/one_file_spike_parsing.py
+drwxrwxr-x   0 r2_allen  (1003) r2_allen  (1003)        0 2024-05-06 14:38:10.311781 ConnorLabAnalysisTools-0.2.2/src/clat/intan/rhd/
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)        0 2023-09-29 20:43:03.000000 ConnorLabAnalysisTools-0.2.2/src/clat/intan/rhd/__init__.py
+drwxrwxr-x   0 r2_allen  (1003) r2_allen  (1003)        0 2024-05-06 14:38:10.315781 ConnorLabAnalysisTools-0.2.2/src/clat/intan/rhd/intanutil/
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)        0 2023-09-29 20:43:03.000000 ConnorLabAnalysisTools-0.2.2/src/clat/intan/rhd/intanutil/__init__.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     2649 2023-09-29 20:43:03.000000 ConnorLabAnalysisTools-0.2.2/src/clat/intan/rhd/intanutil/data_to_result.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     1607 2023-09-29 20:43:03.000000 ConnorLabAnalysisTools-0.2.2/src/clat/intan/rhd/intanutil/get_bytes_per_data_block.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     1417 2023-09-29 20:43:03.000000 ConnorLabAnalysisTools-0.2.2/src/clat/intan/rhd/intanutil/notch_filter.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)      995 2023-09-29 20:43:03.000000 ConnorLabAnalysisTools-0.2.2/src/clat/intan/rhd/intanutil/qstring.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     6661 2023-10-17 15:57:41.000000 ConnorLabAnalysisTools-0.2.2/src/clat/intan/rhd/intanutil/read_header.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     3604 2023-09-29 20:43:03.000000 ConnorLabAnalysisTools-0.2.2/src/clat/intan/rhd/intanutil/read_one_data_block.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)    10280 2023-10-17 15:57:05.000000 ConnorLabAnalysisTools-0.2.2/src/clat/intan/rhd/load_intan_rhd_format.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     6565 2023-10-17 15:52:02.000000 ConnorLabAnalysisTools-0.2.2/src/clat/intan/spike_file.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     4106 2023-10-17 15:29:02.000000 ConnorLabAnalysisTools-0.2.2/src/clat/intan/stitch.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)      653 2024-02-29 19:56:37.000000 ConnorLabAnalysisTools-0.2.2/src/clat/intan/test_analogin.py
+drwxrwxr-x   0 r2_allen  (1003) r2_allen  (1003)        0 2024-05-06 14:38:10.315781 ConnorLabAnalysisTools-0.2.2/src/clat/util/
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)        0 2023-10-03 18:07:38.000000 ConnorLabAnalysisTools-0.2.2/src/clat/util/__init__.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     5558 2024-03-07 18:26:32.000000 ConnorLabAnalysisTools-0.2.2/src/clat/util/connection.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     3482 2023-10-03 18:07:38.000000 ConnorLabAnalysisTools-0.2.2/src/clat/util/dictionary_util.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     3074 2023-10-17 15:14:20.000000 ConnorLabAnalysisTools-0.2.2/src/clat/util/table_util.py
+-rw-rw-r--   0 r2_allen  (1003) r2_allen  (1003)     3526 2024-01-18 18:23:22.000000 ConnorLabAnalysisTools-0.2.2/src/clat/util/time_util.py
```

### Comparing `ConnorLabAnalysisTools-0.2.1/setup.py` & `ConnorLabAnalysisTools-0.2.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='ConnorLabAnalysisTools',
-    version='0.2.1',
+    version='0.2.2',
     description='Tools for analyzing data in the Connor Lab',
     # long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Allen Chen',
     author_email='allenmuhanchen@gmail.com',
     url='https://github.com/EdConnorLab/ConnorLabAnalysisTools',
     packages=find_packages(where="src"),
```

### Comparing `ConnorLabAnalysisTools-0.2.1/src/ConnorLabAnalysisTools.egg-info/SOURCES.txt` & `ConnorLabAnalysisTools-0.2.2/src/ConnorLabAnalysisTools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,34 +5,37 @@
 src/ConnorLabAnalysisTools.egg-info/dependency_links.txt
 src/ConnorLabAnalysisTools.egg-info/requires.txt
 src/ConnorLabAnalysisTools.egg-info/top_level.txt
 src/clat/__init__.py
 src/clat/compile/__init__.py
 src/clat/compile/task/__init__.py
 src/clat/compile/task/base_database_fields.py
+src/clat/compile/task/cached_task_fields.py
 src/clat/compile/task/compile_task_id.py
 src/clat/compile/task/matchstick_fields.py
 src/clat/compile/task/task_field.py
 src/clat/compile/trial/__init__.py
 src/clat/compile/trial/cached_fields.py
 src/clat/compile/trial/classic_database_fields.py
 src/clat/compile/trial/trial_collector.py
 src/clat/compile/trial/trial_field.py
 src/clat/eyecal/__init__.py
 src/clat/eyecal/apply_eyecal.py
 src/clat/eyecal/params.py
 src/clat/eyecal/plot_eyecal.py
 src/clat/intan/__init__.py
 src/clat/intan/amplifiers.py
+src/clat/intan/analogin.py
 src/clat/intan/channels.py
 src/clat/intan/livenotes.py
 src/clat/intan/marker_channels.py
 src/clat/intan/one_file_spike_parsing.py
 src/clat/intan/spike_file.py
 src/clat/intan/stitch.py
+src/clat/intan/test_analogin.py
 src/clat/intan/rhd/__init__.py
 src/clat/intan/rhd/load_intan_rhd_format.py
 src/clat/intan/rhd/intanutil/__init__.py
 src/clat/intan/rhd/intanutil/data_to_result.py
 src/clat/intan/rhd/intanutil/get_bytes_per_data_block.py
 src/clat/intan/rhd/intanutil/notch_filter.py
 src/clat/intan/rhd/intanutil/qstring.py
```

### Comparing `ConnorLabAnalysisTools-0.2.1/src/clat/compile/task/base_database_fields.py` & `ConnorLabAnalysisTools-0.2.2/src/clat/compile/task/base_database_fields.py`

 * *Files identical despite different names*

### Comparing `ConnorLabAnalysisTools-0.2.1/src/clat/compile/task/compile_task_id.py` & `ConnorLabAnalysisTools-0.2.2/src/clat/compile/task/compile_task_id.py`

 * *Files identical despite different names*

### Comparing `ConnorLabAnalysisTools-0.2.1/src/clat/compile/task/matchstick_fields.py` & `ConnorLabAnalysisTools-0.2.2/src/clat/compile/task/matchstick_fields.py`

 * *Files identical despite different names*

### Comparing `ConnorLabAnalysisTools-0.2.1/src/clat/compile/task/task_field.py` & `ConnorLabAnalysisTools-0.2.2/src/clat/compile/task/task_field.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,15 +27,16 @@
         """
         Given a list of task_ids, calls all the TaskFields to get the data for each task_id
         and returns a dataframe with the data
         """
         task_list = [Task(task_id, self) for task_id in task_ids]
         data = []
         for i, task in enumerate(task_list):
-            print("working on", i, "out of", len(task_list))
+            if i % 100 == 0:
+                print("working on", i, "out of", len(task_list))
             task.append_to_data(data)
         return pd.DataFrame(data)
 
     def append_to_data(self, data: pd.DataFrame):
         """ Creates a new dataframe from the triallist and appends it to the supplied dataframe
         This is used to add new columns (fields) to an existing dataframe"""
         # get first column
@@ -53,15 +54,23 @@
 
 class Task:
     def __init__(self, task_id: int, fields: TaskFieldList):
         self.task_id = task_id
         self.fields = fields
 
     def append_to_data(self, data):
-        field_values = [field.get(self.task_id) for field in self.fields]
+        field_values = []
+        for field in self.fields:
+            try:
+                field_value = field.get(self.task_id)
+            except Exception as e:
+                error = f"Error getting {field.name} for task_id {self.task_id}: {e}"
+                print(error)
+                field_value = "None"
+            field_values.append(field_value)
         names = self.fields.get_names()
         new_row = OrderedDict(zip(names, field_values))
         data.append(new_row)
 
 
 def get_data_from_tasks(fields: TaskFieldList, task_ids: list[int]) -> pd.DataFrame:
     task_list = [Task(task_id, fields) for task_id in task_ids]
```

### Comparing `ConnorLabAnalysisTools-0.2.1/src/clat/compile/trial/cached_fields.py` & `ConnorLabAnalysisTools-0.2.2/src/clat/compile/trial/cached_fields.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import ast
 from collections import OrderedDict
 
 import pandas as pd
 
 from clat.compile.trial.trial_field import DatabaseField, FieldList
 from clat.util.connection import Connection
 from clat.util.time_util import When
@@ -16,29 +17,51 @@
 
     Override get_cached_value and cache_value to change the caching logic.
 
     A subclass of a subclass of this class will still need to use super().get rather than
     super().get_and_cache() because the subclass will not have proper self.name (it is overriden).
     """
 
+    def __init__(self, conn: Connection,
+                 ):
+        self.conn = conn
+        super().__init__(conn, self.get_name())
+
+    def get_cached_super(self, when: When, super_type: CachedDatabaseField, *args, **kwargs):
+        # Dynamically get the superclass instance based on super_type
+        # Dynamically create an instance of the specified superclass
+        super_field = super_type(self.conn, *args, **kwargs)
 
+        # Attempt to retrieve cached value
+        cached_value = self._get_cached_value(super_field.get_name(), when)
+        if cached_value is not None:
+            return self.convert_from_string(cached_value)
 
-    def __init__(self, conn: Connection,
-                 name: str = None):
-        super().__init__(conn, name)
+        # Fetch data using the superclass's get method and cache it
+        data = super_field.get(when)
+        self._cache_value(super_field.get_name(), when, data)
+        converted_value = self.convert_from_string(self._get_cached_value(super_field.get_name(), when))
+        return converted_value
 
     def get_and_cache(self, name: str, when: When):
         cached_value = self._get_cached_value(name, when)
         if cached_value is not None:
-            return cached_value
+            return self.convert_from_string(cached_value)
 
         data = self.get(when)
         self._cache_value(name, when, data)
         # return the cached value rather than raw value to ensure same data-types are returned for all calls
-        return self._get_cached_value(name, when)
+        cached_value = self._get_cached_value(name, when)
+        return self.convert_from_string(cached_value)
+
+    def convert_from_string(self, cached_value):
+        try:
+            return ast.literal_eval(cached_value)
+        except ValueError:
+            return cached_value
 
     def _get_cached_value(self, name: str, when: When):
         # Implement the logic to query the TrialFieldCache table
         # to retrieve the cached value, if it exists and is still valid.
         query = "SELECT value FROM TrialFieldCache WHERE name = %s AND start = %s AND stop = %s;"
         self.conn.execute(query, params=(name, int(when.start), int(when.stop)))
         result = self.conn.fetch_all()
@@ -51,32 +74,42 @@
         query = """
         INSERT INTO TrialFieldCache (name, start, stop, value) 
         VALUES (%s, %s, %s, %s)
         ON DUPLICATE KEY UPDATE value = %s;
         """
         self.conn.execute(query, params=(name, int(when.start), int(when.stop), value, value))
 
+    def get_name(self):
+        raise NotImplementedError("Subclasses must implement get_name")
 
 class CachedFieldList(list[CachedDatabaseField]):
     def get_df(self):
         df = pd.DataFrame(columns=self.get_names())
         return df
 
     def get_names(self):
-        return [field.name for field in self]
+        return [field.get_name() for field in self]
 
-    def get_data(self, trial_tstamps: list[When]) -> pd.DataFrame:
+    def to_data(self, trial_tstamps: list[When]) -> pd.DataFrame:
         return self._get_data_from_trials(trial_tstamps)
 
     def _get_data_from_trials(self, trial_tstamps: list[When]) -> pd.DataFrame:
         data = []
         for i, when in enumerate(trial_tstamps):
             print("working on " + str(i) + " out of " + str(len(trial_tstamps)))
-            field_values = [field.get_and_cache(field.name, when) for field in self]
+            field_values = []
+            for field in self:
+                try:
+                    field_values.append(field.get_and_cache(field.name, when))
+                except Exception as e:
+                    print(f"Error fetching {field.name} at {when} for trial {i}: {e}")
+                    field_values.append(None)
+            field_values.insert(0, when)
             names = self.get_names()
+            names.insert(0, "TrialStartStop")
             new_row = OrderedDict(zip(names, field_values))
             data.append(new_row)
 
         return pd.DataFrame(data)
 
 
 """
```

### Comparing `ConnorLabAnalysisTools-0.2.1/src/clat/compile/trial/classic_database_fields.py` & `ConnorLabAnalysisTools-0.2.2/src/clat/compile/trial/classic_database_fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 import xmltodict
 
+from clat.compile.task.cached_task_fields import CachedTaskField
+from clat.compile.trial.cached_fields import CachedDatabaseField
 from clat.compile.trial.trial_field import DatabaseField
 from clat.util.connection import Connection
 from clat.util.time_util import When
 
 
 def get_stim_spec_id(conn: Connection, when: When) -> int:
-    conn.execute(
-        "SELECT msg from BehMsg WHERE "
-        "type = 'SlideOn' AND "
-        "tstamp >= %s AND tstamp <= %s",
-        params=(int(when.start), int(when.stop)))
-    trial_msg_xml = conn.fetch_one()
-    trial_msg_dict = xmltodict.parse(trial_msg_xml)
-    taskId = int(trial_msg_dict['SlideEvent']['taskId'])
-
-    conn.execute("SELECT stim_id from TaskToDo WHERE "
-                 "task_id = %s",
-                 params=(taskId,))
-    stim_spec_id = conn.fetch_one()
+    try:
+        conn.execute(
+            "SELECT msg from BehMsg WHERE "
+            "type = 'SlideOn' AND "
+            "tstamp >= %s AND tstamp <= %s",
+            params=(int(when.start), int(when.stop)))
+        trial_msg_xml = conn.fetch_one()
+        trial_msg_dict = xmltodict.parse(trial_msg_xml)
+        taskId = int(trial_msg_dict['SlideEvent']['taskId'])
+
+        conn.execute("SELECT stim_id from TaskToDo WHERE "
+                     "task_id = %s",
+                     params=(taskId,))
+        stim_spec_id = conn.fetch_one()
+    except:
+        return "None"
     return stim_spec_id
 
 
-class StimSpecIdField(DatabaseField):
+class StimSpecIdField(CachedDatabaseField):
     def get(self, when: When) -> int:
         return get_stim_spec_id(self.conn, when)
 
+    def get_name(self):
+        return "Id"
+
 
 class StimSpecDataField(StimSpecIdField):
     def get(self, when: When) -> dict:
         stim_spec_id = super().get(when)
         return get_stim_spec_data(self.conn, when, stim_spec_id)
 
 
@@ -68,41 +76,50 @@
 
     ga_name = conn.fetch_one()
     return ga_name
 
 
 class NewGaNameField(StimSpecIdField):
     def get(self, when: When) -> str:
-        stim_spec_id = super().get(when)
+        stim_spec_id = self.get_cached_super(when, StimSpecIdField)
         return get_new_ga_name_from_stim_spec_id(self.conn, stim_spec_id)
 
+    def get_name(self):
+        return "GaType"
+
 
 def get_new_ga_name_from_stim_spec_id(conn, stim_spec_id):
     conn.execute("SELECT ga_name FROM TaskToDo t WHERE"
                  " stim_id = %s",
                  params=(stim_spec_id,))
 
     ga_name = conn.fetch_one()
     return ga_name
 
 
 class NewGaLineageField(StimSpecIdField):
     def get(self, when: When) -> str:
-        stim_spec_id = super().get(when)
+        stim_spec_id = self.get_cached_super(when, StimSpecIdField)
         return get_new_ga_lineage_from_stim_spec_id(self.conn, stim_spec_id)
 
+    def get_name(self):
+        return "Lineage"
+
 
 class RegimeScoreField(NewGaLineageField):
     def get(self, when: When) -> str:
-        lineage_id = super().get(when)
+        lineage_id = self.get_cached_super(when, NewGaLineageField)
         return float(get_regime_score_from_lineage_id(self.conn, lineage_id))
 
+    def get_name(self):
+        return "RegimeScore"
+
 
 def get_regime_score_from_lineage_id(conn, lineage_id):
-    conn.execute("SELECT regime_score FROM LineageGaInfo WHERE lineage_id"
+    conn.execute("SELECT regime FROM LineageGaInfo WHERE lineage_id"
                  " = %s",
                  params=(lineage_id,))
     regime_score = conn.fetch_one()
     return regime_score
 
 
 def get_new_ga_lineage_from_stim_spec_id(conn, stim_spec_id):
```

### Comparing `ConnorLabAnalysisTools-0.2.1/src/clat/compile/trial/trial_field.py` & `ConnorLabAnalysisTools-0.2.2/src/clat/compile/trial/trial_field.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,27 +34,29 @@
 
     def get_data(self, trial_tstamps: list[When]) -> pd.DataFrame:
         return self._get_data_from_trials(self, trial_tstamps)
 
     def _get_data_from_trials(self, fields: FieldList, trial_tstamps: list[When]) -> pd.DataFrame:
         data = []
         for i, when in enumerate(trial_tstamps):
-            print("working on " + str(i) + " out of " + str(len(trial_tstamps)))
+            if i % 100 == 0:
+                print("working on " + str(i) + " out of " + str(len(trial_tstamps)))
             field_values = [field.get(when) for field in fields]
             names = fields.get_names()
             new_row = OrderedDict(zip(names, field_values))
             data.append(new_row)
 
         return pd.DataFrame(data)
 
 
 def get_data_from_trials(fields: FieldList, trial_tstamps: list[When]) -> pd.DataFrame:
     data = []
     for i, when in enumerate(trial_tstamps):
-        print("working on " + str(i) + " out of " + str(len(trial_tstamps)))
+        if i % 100 == 0:
+            print("working on " + str(i) + " out of " + str(len(trial_tstamps)))
         field_values = [field.get(when) for field in fields]
         names = fields.get_names()
         new_row = OrderedDict(zip(names, field_values))
         data.append(new_row)
 
     return pd.DataFrame(data)
```

### Comparing `ConnorLabAnalysisTools-0.2.1/src/clat/eyecal/apply_eyecal.py` & `ConnorLabAnalysisTools-0.2.2/src/clat/eyecal/apply_eyecal.py`

 * *Files identical despite different names*

### Comparing `ConnorLabAnalysisTools-0.2.1/src/clat/eyecal/params.py` & `ConnorLabAnalysisTools-0.2.2/src/clat/eyecal/params.py`

 * *Files identical despite different names*

### Comparing `ConnorLabAnalysisTools-0.2.1/src/clat/eyecal/plot_eyecal.py` & `ConnorLabAnalysisTools-0.2.2/src/clat/eyecal/plot_eyecal.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 from __future__ import annotations
 
+import ast
+from concurrent.futures import ThreadPoolExecutor
 from tkinter import filedialog
 import tkinter as tk
 import numpy as np
 import xmltodict
 
+from clat.compile.trial.cached_fields import CachedDatabaseField, CachedFieldList
 from clat.eyecal.params import EyeCalibrationParameters
 from clat.util import time_util
 
 from clat.compile.trial.trial_collector import TrialCollector
 from clat.compile.trial.trial_field import DatabaseField, FieldList, get_data_from_trials
 from clat.util.connection import Connection
 from clat.util.time_util import When
 from typing import Optional, Tuple, Any, List
 from datetime import datetime
 import matplotlib.pyplot as plt
 
 
 def main():
-    current_conn = Connection("allen_estimshape_train_231211")
+    current_conn = Connection("allen_estimshape_ga_dev_240207")
     trial_collector = TrialCollector(conn=current_conn, when=time_util.from_x_days_ago(0))
     calibration_trial_times = trial_collector.collect_calibration_trials()
     calibration_trial_times = filter_messages_after_experiment_start(current_conn, calibration_trial_times)
     print("calibration_trial_times: " + str(calibration_trial_times))
 
-    fields = FieldList()
+    fields = CachedFieldList()
     fields.append(CalibrationPointPositionField(current_conn))
     fields.append(SlideOnOffTimestampField(current_conn))
-    fields.append(VoltsField(current_conn))
     fields.append(AverageVoltsField(current_conn))
     fields.append(DegreesField(current_conn))
-    data = get_data_from_trials(fields, calibration_trial_times)
+    data = fields.to_data(calibration_trial_times)
 
     plot_average_volts(data)
 
     user_response = input("Do you want to serialize the current parameters? (yes/no): ").strip().lower()
     if user_response == 'yes':
         # Get the current parameters
         params = EyeCalibrationParameters.read_params(current_conn)
@@ -125,17 +127,20 @@
     axs[1, 1].set_ylabel('Y Position')
 
     # Show plot
     plt.tight_layout()
     plt.show()
 
 
-class CalibrationPointPositionField(DatabaseField):
-    def __init__(self, conn, name: str = "CalibrationPointPosition"):
-        super().__init__(conn, name)
+class CalibrationPointPositionField(CachedDatabaseField):
+    def __init__(self, conn):
+        super().__init__(conn)
+
+    def get_name(self):
+        return "CalibrationPointPosition"
 
     def get(self, when: When):
         return self.get_calibration_point_setup_msg(when.start, when.stop)
 
     def get_calibration_point_setup_msg(self, start_tstamp: datetime, end_tstamp: datetime) -> tuple[Any, Any]:
         query = """
             SELECT msg 
@@ -149,17 +154,20 @@
         msg = result[0][0] if result else None
         msg_dict = xmltodict.parse(msg)
         x = msg_dict['CalibrationPointSetupMessage']['fixationPosition']['x']
         y = msg_dict['CalibrationPointSetupMessage']['fixationPosition']['y']
         return (x, y)
 
 
-class SlideOnOffTimestampField(DatabaseField):
-    def __init__(self, conn, name: str = "SlideOnOffTimestamps"):
-        super().__init__(conn, name)
+class SlideOnOffTimestampField(CachedDatabaseField):
+    def __init__(self, conn):
+        super().__init__(conn)
+
+    def get_name(self):
+        return "SlideOnOffTimestamps"
 
     def get(self, when: When) -> Tuple[Optional[Any], Optional[Any]]:
         return self.get_slide_on_off_timestamps(when.start, when.stop)
 
     def get_slide_on_off_timestamps(self, start_tstamp: datetime, end_tstamp: datetime) -> Tuple[
         Optional[Any], Optional[Any]]:
         slide_on_query = """
@@ -189,63 +197,72 @@
         self.conn.execute(slide_off_query, params)
         result = self.conn.fetch_all()
         slide_off_timestamp = result[0][0] if result else None
 
         return slide_on_timestamp, slide_off_timestamp
 
 
-class VoltsField(DatabaseField):
-    def __init__(self, conn, name: str = "VoltsLeftRight"):
-        super().__init__(conn, name)
 
-    def get(self, when: When) -> Tuple[
-        List[Tuple[float, float]], List[Tuple[float, float]]]:
-        return self.get_eye_device_messages(when.start, when.stop)
+class AverageVoltsField(SlideOnOffTimestampField):
+    def __init__(self, conn):
+        super().__init__(conn)
+
+    def get_name(self):
+        return "AverageVoltsLeftRight"
+
+    def get(self, when: When) -> Tuple[Optional[Tuple[float, float]], Optional[Tuple[float, float]]]:
+        slide_on_off_timestamps = self.get_cached_super(when, SlideOnOffTimestampField)
+        left_eye_positions, right_eye_positions = self.get_eye_device_messages(slide_on_off_timestamps[0], slide_on_off_timestamps[1])
+        left_eye_positions_filtered = self.remove_outliers(left_eye_positions)
+        right_eye_positions_filtered = self.remove_outliers(right_eye_positions)
+
+        average_left = self.calculate_average(left_eye_positions_filtered)
+        average_right = self.calculate_average(right_eye_positions_filtered)
+
+        # self._cache_value(self.get_name(), when, (average_left, average_right))
+        return average_left, average_right
 
     def get_eye_device_messages(self, start_tstamp: datetime, end_tstamp: datetime) -> Tuple[
         List[Tuple[float, float]], List[Tuple[float, float]]]:
+
+
         query = """
-            SELECT msg 
-            FROM BehMsgEye 
-            WHERE type = 'EyeDeviceMessage' 
-            AND tstamp BETWEEN %s AND %s
+            SELECT msg
+                FROM BehMsgEye
+                WHERE type = 'EyeDeviceMessage' 
+                AND tstamp BETWEEN %s AND %s
         """
         params = (start_tstamp, end_tstamp)
         self.conn.execute(query, params)
         results = self.conn.fetch_all()
 
-        left_eye_positions = []
-        right_eye_positions = []
+        # Process results in parallel
+        with ThreadPoolExecutor() as executor:
+            processed_results = list(executor.map(self.process_message, results))
+
+        if not processed_results:
+            return ([(0,0), (0,0)], [(0,0), (0,0)])
+        left_eye_positions, right_eye_positions = zip(*processed_results)
+        return list(filter(None, left_eye_positions)), list(filter(None, right_eye_positions))
 
-        for row in results:
-            msg = row[0]
-            msg_dict = xmltodict.parse(msg)
-            eye_id = msg_dict['EyeDeviceMessage']['id']
-            volt_x = float(msg_dict['EyeDeviceMessage']['volt']['x'])
-            volt_y = float(msg_dict['EyeDeviceMessage']['volt']['y'])
-
-            if eye_id == 'leftIscan':
-                left_eye_positions.append((volt_x, volt_y))
-            elif eye_id == 'rightIscan':
-                right_eye_positions.append((volt_x, volt_y))
-
-        return left_eye_positions, right_eye_positions
-
-
-class AverageVoltsField(VoltsField):
-    def __init__(self, conn, name: str = "AverageVoltsLeftRight"):
-        super().__init__(conn, name)
-
-    def get(self, when: When) -> Tuple[Optional[Tuple[float, float]], Optional[Tuple[float, float]]]:
-        left_eye_positions, right_eye_positions = super().get(when)
-        left_eye_positions_filtered = self.remove_outliers(left_eye_positions)
-        right_eye_positions_filtered = self.remove_outliers(right_eye_positions)
-        return self.calculate_average(left_eye_positions_filtered), self.calculate_average(right_eye_positions_filtered)
 
     @staticmethod
+    def process_message(row):
+        msg = row[0]
+        msg_dict = xmltodict.parse(msg)
+        eye_id = msg_dict['EyeDeviceMessage']['id']
+        volt_x = float(msg_dict['EyeDeviceMessage']['volt']['x'])
+        volt_y = float(msg_dict['EyeDeviceMessage']['volt']['y'])
+
+        if eye_id == 'leftIscan':
+            return (volt_x, volt_y), None
+        elif eye_id == 'rightIscan':
+            return None, (volt_x, volt_y)
+        return None, None
+    @staticmethod
     def calculate_average(positions: List[Tuple[float, float]]) -> Optional[Tuple[float, float]]:
         if not positions:
             return None
 
         sum_x = sum(pos[0] for pos in positions)
         sum_y = sum(pos[1] for pos in positions)
         count = len(positions)
@@ -274,18 +291,21 @@
         iqr = q3 - q1
         lower_bound = median - 1.5 * iqr
         upper_bound = median + 1.5 * iqr
         return data[(data >= lower_bound) & (data <= upper_bound)]
 
 
 class DegreesField(AverageVoltsField):
-    def __init__(self, conn, name: str = "DegreesLeftRight"):
-        super().__init__(conn, name)
+    def get_name(self):
+        return "DegreesLeftRight"
+
+    def __init__(self, conn):
+        super().__init__(conn)
 
     def get(self, when: When):
         params = EyeCalibrationParameters.read_params(self.conn)
-        left_eye_positions, right_eye_positions = super().get(when)
+        left_eye_positions, right_eye_positions = self.get_cached_super(when, AverageVoltsField)
         return params.volt_to_degree((left_eye_positions, right_eye_positions))
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `ConnorLabAnalysisTools-0.2.1/src/clat/intan/amplifiers.py` & `ConnorLabAnalysisTools-0.2.2/src/clat/intan/amplifiers.py`

 * *Files identical despite different names*

### Comparing `ConnorLabAnalysisTools-0.2.1/src/clat/intan/livenotes.py` & `ConnorLabAnalysisTools-0.2.2/src/clat/intan/livenotes.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 import os
 from typing import Tuple, List, Dict
 
 
 def map_task_id_to_epochs_with_livenotes(livenotes_data: str,
-                                         marker_channel_time_indices: List[Tuple[int, int]]) -> Dict[
+                                         marker_channel_time_indices: List[Tuple[int, int]],
+                                         require_trial_complete=True) -> Dict[
     int, Tuple[int, int]]:
     """
+    If require_trial_complete is True:
     Map unique task IDs to epochs with a following 'Trial Complete' event,
     such that if there are repetitions of a task id in the livenotes, only the complete instance will
     be returned.
+
+    If require_trial_complete is False:
+    Map unique task IDs to epochs without requiring a following 'Trial Complete' event.
     """
     data = read_livenotes(livenotes_data)
     events = parse_livenotes_to_events(data)
     stim_ids = filter_for_stim_ids(events)
     stim_ids.sort()
 
     result = {}
@@ -25,15 +30,25 @@
         following_event = None
 
         idx = events.index((tstamp, str(stim_id)))  # Find the index of this stim_id in the original events list
         if idx < len(events) - 1:
             following_event = events[idx + 1][1]  # Get the following event
 
         # Only proceed if the following event is 'Trial Complete'
-        if following_event == 'Trial Complete':
+
+        if require_trial_complete:
+            if following_event == 'Trial Complete':
+                for start, end in marker_channel_time_indices:
+                    if closest_start is None or abs(tstamp - start) < abs(tstamp - closest_start):
+                        closest_start = start
+                        closest_end = end
+
+                if closest_start is not None and result.get(stim_id) is None:
+                    result[stim_id] = (closest_start, closest_end)
+        else:
             for start, end in marker_channel_time_indices:
                 if closest_start is None or abs(tstamp - start) < abs(tstamp - closest_start):
                     closest_start = start
                     closest_end = end
 
             if closest_start is not None and result.get(stim_id) is None:
                 result[stim_id] = (closest_start, closest_end)
```

### Comparing `ConnorLabAnalysisTools-0.2.1/src/clat/intan/marker_channels.py` & `ConnorLabAnalysisTools-0.2.2/src/clat/intan/marker_channels.py`

 * *Files identical despite different names*

### Comparing `ConnorLabAnalysisTools-0.2.1/src/clat/intan/one_file_spike_parsing.py` & `ConnorLabAnalysisTools-0.2.2/src/clat/intan/one_file_spike_parsing.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         spike_path = os.path.join(intan_file_path, "spike.dat")
         digital_in_path = os.path.join(intan_file_path, "digitalin.dat")
         notes_path = os.path.join(intan_file_path, "notes.txt")
 
         spike_tstamps_for_channels, sample_rate = fetch_spike_tstamps_from_file(spike_path)
         stim_epochs_from_markers = epoch_using_marker_channels(digital_in_path, false_negative_correction_duration=2)
         epochs_for_task_ids = map_task_id_to_epochs_with_livenotes(notes_path,
-                                                                          stim_epochs_from_markers)
+                                                                          stim_epochs_from_markers, require_trial_complete=False)
 
         filtered_spikes_for_channels_by_task_id = {}
         epoch_start_stop_times_by_task_id = {}
         for task_id, epoch in epochs_for_task_ids.items():
             filtered_spikes_for_channels = {}
             for channel, tstamps in spike_tstamps_for_channels.items():
                 passed_filter = []
```

### Comparing `ConnorLabAnalysisTools-0.2.1/src/clat/intan/rhd/intanutil/data_to_result.py` & `ConnorLabAnalysisTools-0.2.2/src/clat/intan/rhd/intanutil/data_to_result.py`

 * *Files identical despite different names*

### Comparing `ConnorLabAnalysisTools-0.2.1/src/clat/intan/rhd/intanutil/get_bytes_per_data_block.py` & `ConnorLabAnalysisTools-0.2.2/src/clat/intan/rhd/intanutil/get_bytes_per_data_block.py`

 * *Files identical despite different names*

### Comparing `ConnorLabAnalysisTools-0.2.1/src/clat/intan/rhd/intanutil/notch_filter.py` & `ConnorLabAnalysisTools-0.2.2/src/clat/intan/rhd/intanutil/notch_filter.py`

 * *Files identical despite different names*

### Comparing `ConnorLabAnalysisTools-0.2.1/src/clat/intan/rhd/intanutil/qstring.py` & `ConnorLabAnalysisTools-0.2.2/src/clat/intan/rhd/intanutil/qstring.py`

 * *Files identical despite different names*

### Comparing `ConnorLabAnalysisTools-0.2.1/src/clat/intan/rhd/intanutil/read_header.py` & `ConnorLabAnalysisTools-0.2.2/src/clat/intan/rhd/intanutil/read_header.py`

 * *Files identical despite different names*

### Comparing `ConnorLabAnalysisTools-0.2.1/src/clat/intan/rhd/intanutil/read_one_data_block.py` & `ConnorLabAnalysisTools-0.2.2/src/clat/intan/rhd/intanutil/read_one_data_block.py`

 * *Files identical despite different names*

### Comparing `ConnorLabAnalysisTools-0.2.1/src/clat/intan/rhd/load_intan_rhd_format.py` & `ConnorLabAnalysisTools-0.2.2/src/clat/intan/rhd/load_intan_rhd_format.py`

 * *Files identical despite different names*

### Comparing `ConnorLabAnalysisTools-0.2.1/src/clat/intan/spike_file.py` & `ConnorLabAnalysisTools-0.2.2/src/clat/intan/spike_file.py`

 * *Files identical despite different names*

### Comparing `ConnorLabAnalysisTools-0.2.1/src/clat/intan/stitch.py` & `ConnorLabAnalysisTools-0.2.2/src/clat/intan/stitch.py`

 * *Files identical despite different names*

### Comparing `ConnorLabAnalysisTools-0.2.1/src/clat/util/dictionary_util.py` & `ConnorLabAnalysisTools-0.2.2/src/clat/util/dictionary_util.py`

 * *Files identical despite different names*

### Comparing `ConnorLabAnalysisTools-0.2.1/src/clat/util/table_util.py` & `ConnorLabAnalysisTools-0.2.2/src/clat/util/table_util.py`

 * *Files identical despite different names*

### Comparing `ConnorLabAnalysisTools-0.2.1/src/clat/util/time_util.py` & `ConnorLabAnalysisTools-0.2.2/src/clat/util/time_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import time
 import datetime
 
 
+
+
 class When:
     def __init__(self, start, stop):
         self.start = start
         self.stop = stop
 
     def tuple(self):
         return (self.start, self.stop)
@@ -27,14 +29,20 @@
 def from_x_days_ago(x):
     start = to_unix(datetime.date.today() - datetime.timedelta(days=x))
     stop = now()
     when = When(start, stop)
     return when
 
 
+def from_date_to_now(year: int, month: int, day: int) -> When:
+    start = to_unix(datetime.date(year, month, day))
+    stop = now()
+    when = When(start, stop)
+    return when
+
 def all():
     when = When(0, to_unix(datetime.date.fromisoformat('3022-01-01')))
     return when
 
 
 def now():
     return round(time.time() * 1000000)
@@ -87,11 +95,12 @@
         # Default to the end of the day (23:59:59)
         end_datetime = datetime.datetime(year, month, day, 23, 59, 59)
     end = to_unix(end_datetime)
 
     return When(start, end)
 
 
+
 # Testing the new function with a start time and default end time
 test_start_time = "08:30:00"  # 8:30 AM
 when_for_date_time = on_date_and_time(2022, 7, 4, test_start_time)
 when_for_date_time
```

