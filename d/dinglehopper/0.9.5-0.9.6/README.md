# Comparing `tmp/dinglehopper-0.9.5.tar.gz` & `tmp/dinglehopper-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dinglehopper-0.9.5.tar", last modified: Wed Mar 27 17:51:34 2024, max compression
+gzip compressed data, was "dinglehopper-0.9.6.tar", last modified: Mon May  6 15:50:52 2024, max compression
```

## Comparing `dinglehopper-0.9.5.tar` & `dinglehopper-0.9.6.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:51:34.034340 dinglehopper-0.9.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7208 2024-03-27 17:51:34.034340 dinglehopper-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/ocrd-tool.json
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 17:51:34.034340 dinglehopper-0.9.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:51:34.026340 dinglehopper-0.9.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:51:34.030340 dinglehopper-0.9.5/src/dinglehopper/
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/src/dinglehopper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/src/dinglehopper/align.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/src/dinglehopper/character_error_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/src/dinglehopper/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/src/dinglehopper/cli_extract.py
--rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/src/dinglehopper/cli_line_dirs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/src/dinglehopper/cli_summarize.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/src/dinglehopper/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/src/dinglehopper/edit_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)    12192 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/src/dinglehopper/extracted_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/src/dinglehopper/ocr_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/src/dinglehopper/ocrd-tool.json
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/src/dinglehopper/ocrd_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:51:34.030340 dinglehopper-0.9.5/src/dinglehopper/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/src/dinglehopper/templates/report.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/src/dinglehopper/templates/report.html.js
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/src/dinglehopper/templates/report.json.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/src/dinglehopper/templates/summary.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/src/dinglehopper/templates/summary.json.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:51:34.034340 dinglehopper-0.9.5/src/dinglehopper/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/src/dinglehopper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5089 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/src/dinglehopper/tests/extracted_text_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/src/dinglehopper/tests/test_align.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/src/dinglehopper/tests/test_character_error_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/src/dinglehopper/tests/test_edit_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/src/dinglehopper/tests/test_editops.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/src/dinglehopper/tests/test_integ_align.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/src/dinglehopper/tests/test_integ_bigger_texts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/src/dinglehopper/tests/test_integ_character_error_rate_ocr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/src/dinglehopper/tests/test_integ_cli_dir.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/src/dinglehopper/tests/test_integ_cli_valid_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/src/dinglehopper/tests/test_integ_differences.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/src/dinglehopper/tests/test_integ_edit_distance_ocr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/src/dinglehopper/tests/test_integ_ocrd_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/src/dinglehopper/tests/test_integ_summarize.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/src/dinglehopper/tests/test_integ_table_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/src/dinglehopper/tests/test_integ_word_error_rate_ocr.py
--rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/src/dinglehopper/tests/test_ocr_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/src/dinglehopper/tests/test_word_error_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/src/dinglehopper/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-03-27 17:51:25.000000 dinglehopper-0.9.5/src/dinglehopper/word_error_rate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:51:34.034340 dinglehopper-0.9.5/src/dinglehopper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7208 2024-03-27 17:51:34.000000 dinglehopper-0.9.5/src/dinglehopper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-03-27 17:51:34.000000 dinglehopper-0.9.5/src/dinglehopper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 17:51:34.000000 dinglehopper-0.9.5/src/dinglehopper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-27 17:51:34.000000 dinglehopper-0.9.5/src/dinglehopper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-27 17:51:34.000000 dinglehopper-0.9.5/src/dinglehopper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-27 17:51:34.000000 dinglehopper-0.9.5/src/dinglehopper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:50:52.034524 dinglehopper-0.9.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-05-06 15:50:52.034524 dinglehopper-0.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/ocrd-tool.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 15:50:52.034524 dinglehopper-0.9.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:50:52.022524 dinglehopper-0.9.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:50:52.026524 dinglehopper-0.9.6/src/dinglehopper/
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/align.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/character_error_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8996 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/cli_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/cli_line_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/cli_summarize.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/edit_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/extracted_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/ocr_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/ocrd-tool.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/ocrd_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:50:52.030524 dinglehopper-0.9.6/src/dinglehopper/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/templates/report.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/templates/report.html.js
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/templates/report.json.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/templates/summary.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/templates/summary.json.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:50:52.034524 dinglehopper-0.9.6/src/dinglehopper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5089 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/tests/extracted_text_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/tests/test_align.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/tests/test_character_error_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/tests/test_edit_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/tests/test_editops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/tests/test_integ_align.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/tests/test_integ_bigger_texts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/tests/test_integ_character_error_rate_ocr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/tests/test_integ_cli_dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/tests/test_integ_cli_valid_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/tests/test_integ_differences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/tests/test_integ_edit_distance_ocr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/tests/test_integ_empty_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/tests/test_integ_ocrd_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/tests/test_integ_summarize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/tests/test_integ_table_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/tests/test_integ_word_error_rate_ocr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/tests/test_ocr_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/tests/test_word_error_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-06 15:50:41.000000 dinglehopper-0.9.6/src/dinglehopper/word_error_rate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:50:52.034524 dinglehopper-0.9.6/src/dinglehopper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-05-06 15:50:52.000000 dinglehopper-0.9.6/src/dinglehopper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-06 15:50:52.000000 dinglehopper-0.9.6/src/dinglehopper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 15:50:52.000000 dinglehopper-0.9.6/src/dinglehopper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-06 15:50:52.000000 dinglehopper-0.9.6/src/dinglehopper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-06 15:50:52.000000 dinglehopper-0.9.6/src/dinglehopper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-06 15:50:52.000000 dinglehopper-0.9.6/src/dinglehopper.egg-info/top_level.txt
```

### Comparing `dinglehopper-0.9.5/LICENSE` & `dinglehopper-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.5/PKG-INFO` & `dinglehopper-0.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dinglehopper
-Version: 0.9.5
+Version: 0.9.6
 Summary: The OCR evaluation tool
 Author-email: Mike Gerber <mike.gerber@sbb.spk-berlin.de>, The QURATOR SPK Team <qurator@sbb.spk-berlin.de>
 Project-URL: Homepage, https://github.com/qurator-spk/dinglehopper
 Project-URL: Repository, https://github.com/qurator-spk/dinglehopper.git
 Keywords: qurator,ocr,evaluation,ocr-d
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -21,15 +21,15 @@
 Requires-Dist: click
 Requires-Dist: jinja2
 Requires-Dist: lxml
 Requires-Dist: uniseg>=0.8.0
 Requires-Dist: numpy
 Requires-Dist: colorama
 Requires-Dist: MarkupSafe
-Requires-Dist: ocrd>=2.20.1
+Requires-Dist: ocrd>=2.65.0
 Requires-Dist: attrs
 Requires-Dist: multimethod>=1.3
 Requires-Dist: tqdm
 Requires-Dist: rapidfuzz>=2.7.0
 Requires-Dist: chardet
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
@@ -141,19 +141,19 @@
 ~~~
 dinglehopper-summarize output_folder/
 ~~~
 This generates `summary.html` and `summary.json` in the same `output_folder`.
 
 If you are summarizing many reports and have used the `--differences` flag while
 generating them, it may be useful to limit the number of differences reported by using
-the `--occurences-threshold` parameter. This will reduce the size of the generated HTML
+the `--occurrences-threshold` parameter. This will reduce the size of the generated HTML
 report, making it easier to open and navigate. Note that the JSON report will still
 contain all differences. Example:
 ~~~
-dinglehopper-summarize output_folder/ --occurences-threshold 10
+dinglehopper-summarize output_folder/ --occurrences-threshold 10
 ~~~
 
 ### dinglehopper-line-dirs
 You also may want to compare a directory of GT text files (i.e. `gt/line0001.gt.txt`)
 with a directory of OCR text files (i.e. `ocr/line0001.some-ocr.txt`) with a separate
 CLI interface:
```

### Comparing `dinglehopper-0.9.5/README.md` & `dinglehopper-0.9.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -96,19 +96,19 @@
 ~~~
 dinglehopper-summarize output_folder/
 ~~~
 This generates `summary.html` and `summary.json` in the same `output_folder`.
 
 If you are summarizing many reports and have used the `--differences` flag while
 generating them, it may be useful to limit the number of differences reported by using
-the `--occurences-threshold` parameter. This will reduce the size of the generated HTML
+the `--occurrences-threshold` parameter. This will reduce the size of the generated HTML
 report, making it easier to open and navigate. Note that the JSON report will still
 contain all differences. Example:
 ~~~
-dinglehopper-summarize output_folder/ --occurences-threshold 10
+dinglehopper-summarize output_folder/ --occurrences-threshold 10
 ~~~
 
 ### dinglehopper-line-dirs
 You also may want to compare a directory of GT text files (i.e. `gt/line0001.gt.txt`)
 with a directory of OCR text files (i.e. `ocr/line0001.some-ocr.txt`) with a separate
 CLI interface:
```

### Comparing `dinglehopper-0.9.5/ocrd-tool.json` & `dinglehopper-0.9.6/ocrd-tool.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {"'version'": "'0.9.6'"}*

```diff
@@ -31,9 +31,9 @@
                 }
             },
             "steps": [
                 "recognition/text-recognition"
             ]
         }
     },
-    "version": "0.9.5"
+    "version": "0.9.6"
 }
```

### Comparing `dinglehopper-0.9.5/pyproject.toml` & `dinglehopper-0.9.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.5/src/dinglehopper/__init__.py` & `dinglehopper-0.9.6/src/dinglehopper/__init__.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.5/src/dinglehopper/align.py` & `dinglehopper-0.9.6/src/dinglehopper/align.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.5/src/dinglehopper/character_error_rate.py` & `dinglehopper-0.9.6/src/dinglehopper/character_error_rate.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.5/src/dinglehopper/cli.py` & `dinglehopper-0.9.6/src/dinglehopper/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,16 +183,23 @@
             differences=differences,
             diff_c=diff_c,
             diff_w=diff_w,
         ).dump(out_fn)
 
 
 def process_dir(
-    gt, ocr, report_prefix, reports_folder, metrics, differences, textequiv_level
-):
+    gt: str,
+    ocr: str,
+    report_prefix: str,
+    reports_folder: str = ".",
+    *,
+    metrics: bool = True,
+    differences: bool = False,
+    textequiv_level: str = "region",
+) -> None:
     for gt_file in os.listdir(gt):
         gt_file_path = os.path.join(gt, gt_file)
         ocr_file_path = os.path.join(ocr, gt_file)
 
         if os.path.isfile(gt_file_path) and os.path.isfile(ocr_file_path):
             process(
                 gt_file_path,
@@ -265,17 +272,17 @@
             )
         else:
             process_dir(
                 gt,
                 ocr,
                 report_prefix,
                 reports_folder,
-                metrics,
-                differences,
-                textequiv_level,
+                metrics=metrics,
+                differences=differences,
+                textequiv_level=textequiv_level,
             )
     else:
         process(
             gt,
             ocr,
             report_prefix,
             reports_folder,
```

### Comparing `dinglehopper-0.9.5/src/dinglehopper/cli_extract.py` & `dinglehopper-0.9.6/src/dinglehopper/cli_extract.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.5/src/dinglehopper/cli_line_dirs.py` & `dinglehopper-0.9.6/src/dinglehopper/cli_line_dirs.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.5/src/dinglehopper/cli_summarize.py` & `dinglehopper-0.9.6/src/dinglehopper/cli_summarize.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.5/src/dinglehopper/edit_distance.py` & `dinglehopper-0.9.6/src/dinglehopper/edit_distance.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.5/src/dinglehopper/extracted_text.py` & `dinglehopper-0.9.6/src/dinglehopper/extracted_text.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,15 +231,15 @@
             # This is frozen, so we have to jump through the hoop:
             object.__setattr__(self, "_segment_id_for_pos", segment_id_for_pos)
             assert self._segment_id_for_pos
 
         return self._segment_id_for_pos[pos]
 
     @classmethod
-    def from_text_segment(cls, text_segment, nsmap, textequiv_level="region"):
+    def from_text_segment(cls, text_segment, nsmap, *, textequiv_level="region"):
         """Build an ExtractedText from a PAGE content text element"""
 
         localname_for_textequiv_level = {"region": "TextRegion", "line": "TextLine"}
         textequiv_level_for_localname = invert_dict(localname_for_textequiv_level)
         children_for_localname = {"TextRegion": "TextLine"}
         joiner_for_textequiv_level = {"line": "\n"}
 
@@ -325,14 +325,14 @@
     return textequivs[index]
 
 
 def get_attr(te: Any, attr_name: str) -> float:
     """Extract the attribute for the given name.
 
     Note: currently only handles numeric values!
-    Other or non existend values are encoded as np.nan.
+    Other or non existent values are encoded as np.nan.
     """
     attr_value = te.attrib.get(attr_name)
     try:
         return float(attr_value)
     except TypeError:
         return np.nan
```

### Comparing `dinglehopper-0.9.5/src/dinglehopper/ocr_files.py` & `dinglehopper-0.9.6/src/dinglehopper/ocr_files.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.5/src/dinglehopper/ocrd-tool.json` & `dinglehopper-0.9.6/src/dinglehopper/ocrd-tool.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {"'version'": "'0.9.6'"}*

```diff
@@ -31,9 +31,9 @@
                 }
             },
             "steps": [
                 "recognition/text-recognition"
             ]
         }
     },
-    "version": "0.9.5"
+    "version": "0.9.6"
 }
```

### Comparing `dinglehopper-0.9.5/src/dinglehopper/ocrd_cli.py` & `dinglehopper-0.9.6/src/dinglehopper/ocrd_cli.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.5/src/dinglehopper/templates/report.html.j2` & `dinglehopper-0.9.6/src/dinglehopper/templates/report.html.j2`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.5/src/dinglehopper/templates/report.html.js` & `dinglehopper-0.9.6/src/dinglehopper/templates/report.html.js`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.5/src/dinglehopper/templates/summary.html.j2` & `dinglehopper-0.9.6/src/dinglehopper/templates/summary.html.j2`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.5/src/dinglehopper/tests/extracted_text_test.py` & `dinglehopper-0.9.6/src/dinglehopper/tests/extracted_text_test.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.5/src/dinglehopper/tests/test_align.py` & `dinglehopper-0.9.6/src/dinglehopper/tests/test_align.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.5/src/dinglehopper/tests/test_character_error_rate.py` & `dinglehopper-0.9.6/src/dinglehopper/tests/test_character_error_rate.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.5/src/dinglehopper/tests/test_edit_distance.py` & `dinglehopper-0.9.6/src/dinglehopper/tests/test_edit_distance.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.5/src/dinglehopper/tests/test_editops.py` & `dinglehopper-0.9.6/src/dinglehopper/tests/test_editops.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.5/src/dinglehopper/tests/test_integ_align.py` & `dinglehopper-0.9.6/src/dinglehopper/tests/test_integ_align.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.5/src/dinglehopper/tests/test_integ_bigger_texts.py` & `dinglehopper-0.9.6/src/dinglehopper/tests/test_integ_bigger_texts.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.5/src/dinglehopper/tests/test_integ_character_error_rate_ocr.py` & `dinglehopper-0.9.6/src/dinglehopper/tests/test_integ_character_error_rate_ocr.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.5/src/dinglehopper/tests/test_integ_cli_dir.py` & `dinglehopper-0.9.6/src/dinglehopper/tests/test_integ_cli_dir.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 
     initLogging()
     process_dir(
         os.path.join(data_dir, "directory-test", "gt"),
         os.path.join(data_dir, "directory-test", "ocr"),
         "report",
         str(tmp_path / "reports"),
-        False,
-        True,
-        "line",
+        metrics=False,
+        differences=True,
+        textequiv_level="line",
     )
 
     assert os.path.exists(tmp_path / "reports/1.xml-report.json")
     assert os.path.exists(tmp_path / "reports/1.xml-report.html")
     assert os.path.exists(tmp_path / "reports/2.xml-report.json")
     assert os.path.exists(tmp_path / "reports/2.xml-report.html")
 
@@ -41,13 +41,13 @@
 
     initLogging()
     process_dir(
         os.path.join(data_dir, "directory-test", "gt"),
         os.path.join(data_dir, "directory-test", "ocr"),
         "report",
         str(tmp_path / "reports"),
-        False,
-        True,
-        "line",
+        metrics=False,
+        differences=True,
+        textequiv_level="line",
     )
 
     assert len(os.listdir(tmp_path / "reports")) == 2 * 2
```

### Comparing `dinglehopper-0.9.5/src/dinglehopper/tests/test_integ_cli_valid_json.py` & `dinglehopper-0.9.6/src/dinglehopper/tests/test_integ_cli_valid_json.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.5/src/dinglehopper/tests/test_integ_differences.py` & `dinglehopper-0.9.6/src/dinglehopper/tests/test_integ_differences.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.5/src/dinglehopper/tests/test_integ_edit_distance_ocr.py` & `dinglehopper-0.9.6/src/dinglehopper/tests/test_integ_edit_distance_ocr.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.5/src/dinglehopper/tests/test_integ_ocrd_cli.py` & `dinglehopper-0.9.6/src/dinglehopper/tests/test_integ_ocrd_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,13 @@
             "-m",
             "mets.xml",
             "-I",
             "OCR-D-GT-PAGE,OCR-D-OCR-CALAMARI",
             "-O",
             "OCR-D-OCR-CALAMARI-EVAL",
         ]
-        sys.argv[1:] = (
-            args  # XXX Hack to satisfy ocrd_cli_wrap_processor() check for arguments
-        )
+        # Hack to satisfy ocrd_cli_wrap_processor() check for arguments
+        sys.argv[1:] = args
         result = runner.invoke(ocrd_dinglehopper, args)
     assert result.exit_code == 0
     result_json = list((test_workspace_dir / "OCR-D-OCR-CALAMARI-EVAL").glob("*.json"))
     assert json.load(open(str(result_json[0])))["cer"] < 0.03
```

### Comparing `dinglehopper-0.9.5/src/dinglehopper/tests/test_integ_summarize.py` & `dinglehopper-0.9.6/src/dinglehopper/tests/test_integ_summarize.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.5/src/dinglehopper/tests/test_integ_table_extraction.py` & `dinglehopper-0.9.6/src/dinglehopper/tests/test_integ_table_extraction.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.5/src/dinglehopper/tests/test_integ_word_error_rate_ocr.py` & `dinglehopper-0.9.6/src/dinglehopper/tests/test_integ_word_error_rate_ocr.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.5/src/dinglehopper/tests/test_ocr_files.py` & `dinglehopper-0.9.6/src/dinglehopper/tests/test_ocr_files.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.5/src/dinglehopper/tests/test_word_error_rate.py` & `dinglehopper-0.9.6/src/dinglehopper/tests/test_word_error_rate.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.5/src/dinglehopper/tests/util.py` & `dinglehopper-0.9.6/src/dinglehopper/tests/util.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.5/src/dinglehopper/word_error_rate.py` & `dinglehopper-0.9.6/src/dinglehopper/word_error_rate.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
         subcat = unicodedata.category(c)
         cat = subcat[0]
         return cat in unwanted_categories or subcat in unwanted_subcategories
 
     # We follow Unicode Standard Annex #29 on Unicode Text Segmentation here: Split on
     # word boundaries using uniseg.wordbreak.words() and ignore all "words" that contain
-    # only whitespace, punctation "or similar characters."
+    # only whitespace, punctuation "or similar characters."
     for word in uniseg.wordbreak.words(s):
         if all(unwanted(c) for c in word):
             pass
         else:
             yield word
```

### Comparing `dinglehopper-0.9.5/src/dinglehopper.egg-info/PKG-INFO` & `dinglehopper-0.9.6/src/dinglehopper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dinglehopper
-Version: 0.9.5
+Version: 0.9.6
 Summary: The OCR evaluation tool
 Author-email: Mike Gerber <mike.gerber@sbb.spk-berlin.de>, The QURATOR SPK Team <qurator@sbb.spk-berlin.de>
 Project-URL: Homepage, https://github.com/qurator-spk/dinglehopper
 Project-URL: Repository, https://github.com/qurator-spk/dinglehopper.git
 Keywords: qurator,ocr,evaluation,ocr-d
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -21,15 +21,15 @@
 Requires-Dist: click
 Requires-Dist: jinja2
 Requires-Dist: lxml
 Requires-Dist: uniseg>=0.8.0
 Requires-Dist: numpy
 Requires-Dist: colorama
 Requires-Dist: MarkupSafe
-Requires-Dist: ocrd>=2.20.1
+Requires-Dist: ocrd>=2.65.0
 Requires-Dist: attrs
 Requires-Dist: multimethod>=1.3
 Requires-Dist: tqdm
 Requires-Dist: rapidfuzz>=2.7.0
 Requires-Dist: chardet
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
@@ -141,19 +141,19 @@
 ~~~
 dinglehopper-summarize output_folder/
 ~~~
 This generates `summary.html` and `summary.json` in the same `output_folder`.
 
 If you are summarizing many reports and have used the `--differences` flag while
 generating them, it may be useful to limit the number of differences reported by using
-the `--occurences-threshold` parameter. This will reduce the size of the generated HTML
+the `--occurrences-threshold` parameter. This will reduce the size of the generated HTML
 report, making it easier to open and navigate. Note that the JSON report will still
 contain all differences. Example:
 ~~~
-dinglehopper-summarize output_folder/ --occurences-threshold 10
+dinglehopper-summarize output_folder/ --occurrences-threshold 10
 ~~~
 
 ### dinglehopper-line-dirs
 You also may want to compare a directory of GT text files (i.e. `gt/line0001.gt.txt`)
 with a directory of OCR text files (i.e. `ocr/line0001.some-ocr.txt`) with a separate
 CLI interface:
```

### Comparing `dinglehopper-0.9.5/src/dinglehopper.egg-info/SOURCES.txt` & `dinglehopper-0.9.6/src/dinglehopper.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 src/dinglehopper/tests/test_integ_align.py
 src/dinglehopper/tests/test_integ_bigger_texts.py
 src/dinglehopper/tests/test_integ_character_error_rate_ocr.py
 src/dinglehopper/tests/test_integ_cli_dir.py
 src/dinglehopper/tests/test_integ_cli_valid_json.py
 src/dinglehopper/tests/test_integ_differences.py
 src/dinglehopper/tests/test_integ_edit_distance_ocr.py
+src/dinglehopper/tests/test_integ_empty_files.py
 src/dinglehopper/tests/test_integ_ocrd_cli.py
 src/dinglehopper/tests/test_integ_summarize.py
 src/dinglehopper/tests/test_integ_table_extraction.py
 src/dinglehopper/tests/test_integ_word_error_rate_ocr.py
 src/dinglehopper/tests/test_ocr_files.py
 src/dinglehopper/tests/test_word_error_rate.py
 src/dinglehopper/tests/util.py
```

