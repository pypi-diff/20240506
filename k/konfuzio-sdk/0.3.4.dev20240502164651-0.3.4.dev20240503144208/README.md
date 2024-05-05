# Comparing `tmp/konfuzio_sdk-0.3.4.dev20240502164651.tar.gz` & `tmp/konfuzio_sdk-0.3.4.dev20240503144208.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "konfuzio_sdk-0.3.4.dev20240502164651.tar", last modified: Fri May  3 03:29:52 2024, max compression
+gzip compressed data, was "konfuzio_sdk-0.3.4.dev20240503144208.tar", last modified: Sat May  4 03:27:47 2024, max compression
```

## Comparing `konfuzio_sdk-0.3.4.dev20240502164651.tar` & `konfuzio_sdk-0.3.4.dev20240503144208.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:29:52.530389 konfuzio_sdk-0.3.4.dev20240502164651/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-05-03 03:29:52.530389 konfuzio_sdk-0.3.4.dev20240502164651/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:29:52.518389 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33566 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)   207592 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    44747 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/extras.py
--rw-r--r--   0 runner    (1001) docker     (127)    27450 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/regex.py
--rw-r--r--   0 runner    (1001) docker     (127)    27029 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/settings_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:29:52.522389 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/tokenizer/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/tokenizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13180 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/tokenizer/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15231 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/tokenizer/paragraph_and_sentence.py
--rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/tokenizer/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:29:52.522389 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11655 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/trainer/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    75617 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/trainer/document_categorization.py
--rw-r--r--   0 runner    (1001) docker     (127)    51309 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/trainer/file_splitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/trainer/image.py
--rw-r--r--   0 runner    (1001) docker     (127)   101643 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/trainer/information_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/trainer/tokenization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/trainer/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    37377 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:29:52.526389 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-05-03 03:29:52.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-03 03:29:52.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 03:29:52.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-03 03:29:52.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-03 03:29:52.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-03 03:29:52.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 03:29:52.530389 konfuzio_sdk-0.3.4.dev20240502164651/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:29:52.526389 konfuzio_sdk-0.3.4.dev20240502164651/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    23504 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)   168877 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    80271 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/tests/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/tests/test_extras.py
--rw-r--r--   0 runner    (1001) docker     (127)    10164 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/tests/test_normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)    41449 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/tests/test_regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/tests/test_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/tests/test_urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    20678 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:27:47.015671 konfuzio_sdk-0.3.4.dev20240503144208/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-05-04 03:27:47.011671 konfuzio_sdk-0.3.4.dev20240503144208/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:27:47.003671 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33566 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)   207592 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44747 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27450 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27029 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/settings_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:27:47.007670 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/tokenizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13180 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/tokenizer/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15231 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/tokenizer/paragraph_and_sentence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/tokenizer/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:27:47.007670 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11655 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/trainer/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75617 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/trainer/document_categorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51309 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/trainer/file_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/trainer/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)   102313 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/trainer/information_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/trainer/tokenization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/trainer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37377 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:27:47.011671 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-05-04 03:27:46.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-04 03:27:46.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 03:27:46.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-04 03:27:46.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-04 03:27:46.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-04 03:27:46.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 03:27:47.015671 konfuzio_sdk-0.3.4.dev20240503144208/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:27:47.011671 konfuzio_sdk-0.3.4.dev20240503144208/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    23504 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)   168877 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80271 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/tests/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/tests/test_extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10164 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/tests/test_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41449 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/tests/test_regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/tests/test_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/tests/test_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20678 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/tests/test_utils.py
```

### Comparing `konfuzio_sdk-0.3.4.dev20240502164651/LICENSE.md` & `konfuzio_sdk-0.3.4.dev20240503144208/LICENSE.md`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240502164651/PKG-INFO` & `konfuzio_sdk-0.3.4.dev20240503144208/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konfuzio_sdk
-Version: 0.3.4.dev20240502164651
+Version: 0.3.4.dev20240503144208
 Summary: Konfuzio Software Development Kit
 Home-page: https://github.com/konfuzio-ai/konfuzio-sdk/
 Author: Helm & Nagel GmbH
 Author-email: info@helm-nagel.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: certifi==2023.7.22
```

### Comparing `konfuzio_sdk-0.3.4.dev20240502164651/README.md` & `konfuzio_sdk-0.3.4.dev20240503144208/README.md`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/api.py` & `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/api.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/cli.py` & `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/cli.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/data.py` & `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/data.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/evaluate.py` & `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/evaluate.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/extras.py` & `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/extras.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/normalize.py` & `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/normalize.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/regex.py` & `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/regex.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/samples.py` & `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/samples.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/settings_importer.py` & `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/settings_importer.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/tokenizer/base.py` & `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/tokenizer/base.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/tokenizer/paragraph_and_sentence.py` & `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/tokenizer/paragraph_and_sentence.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/tokenizer/regex.py` & `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/tokenizer/regex.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/trainer/base.py` & `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/trainer/base.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/trainer/document_categorization.py` & `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/trainer/document_categorization.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/trainer/file_splitting.py` & `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/trainer/file_splitting.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/trainer/image.py` & `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/trainer/image.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/trainer/information_extraction.py` & `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/trainer/information_extraction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1154,17 +1154,17 @@
 
 
 class GroupAnnotationSets:
     """Groups Annotation into Annotation Sets."""
 
     def __init__(self):
         """Initialize TemplateClf."""
-        self.n_nearest_template = 5
-        self.max_depth = 100
-        self.n_estimators = 100
+        self.label_set_max_depth = 100
+        self.label_set_n_estimators = 100
+        self.label_set_n_nearest_template = 5
         self.label_set_clf = None
 
     def fit_label_set_clf(self) -> Tuple[Optional[object], Optional[List['str']]]:
         """
         Fit classifier to predict start lines of Sections.
 
         :param documents:
@@ -1193,16 +1193,15 @@
             # todo check for NO_LABEL_SET if we should keep it
             return None
         logger.info('Start training of Multi-class Label Set Classifier.')
         # ignores the section count as it actually worsens results
         # todo check if no category labels should be ignored
         self.template_feature_list = list(self.clf.classes_)  # list of label classifier targets
         # logger.warning("template_feature_list:", self.template_feature_list)
-        n_nearest = self.n_nearest_template  # if hasattr(self, 'n_nearest_template') else 0
-
+        n_nearest = self.label_set_n_nearest_template
         # Pretty long feature generation
         df_train_label = self.df_train
 
         df_train_label_list = list(df_train_label.groupby('document_id'))
 
         df_train_template_list = []
         df_train_ground_truth_list = []
@@ -1236,15 +1235,15 @@
         if x_train.empty:
             logger.error(
                 'No features available to train template classifier, ' 'probably because there are no annotations.'
             )
             return None, None
 
         label_set_clf = RandomForestClassifier(
-            n_estimators=self.n_estimators, max_depth=self.max_depth, random_state=420
+            n_estimators=self.label_set_n_estimators, max_depth=self.label_set_max_depth, random_state=420
         )
         label_set_clf.fit(x_train, y_train)
 
         self.label_set_clf = label_set_clf
         return self.label_set_clf, self.template_feature_list
 
     def generate_relative_line_features(self, n_nearest: int, df_features: pandas.DataFrame) -> pandas.DataFrame:
@@ -1412,15 +1411,19 @@
 
     def extract_template_with_clf(self, text, res_dict):
         """Run LabelSet classifier to find AnnotationSets."""
         logger.info('Extract AnnotationSets.')
         if not res_dict:
             logger.warning('res_dict is empty')
             return res_dict
-        n_nearest = self.n_nearest_template if hasattr(self, 'n_nearest_template') else 0
+        n_nearest = (
+            self.label_set_n_nearest_template
+            if hasattr(self, 'label_set_n_nearest_template')
+            else (self.n_nearest_template if hasattr(self, 'n_nearest_template') else 0)
+        )
         feature_df = self.build_document_template_feature_X(text, self.dict_to_dataframe(res_dict)).filter(
             self.template_feature_list, axis=1
         )
         feature_df = feature_df.reindex(columns=self.template_feature_list).fillna(0)
         feature_df = self.generate_relative_line_features(n_nearest, feature_df)
 
         res_series = self.label_set_clf.predict(feature_df)
@@ -1566,22 +1569,30 @@
         logger.info(f'{n_nearest=}')
         logger.info(f'{first_word=}')
         logger.info(f'{max_depth=}')
         logger.info(f'{n_estimators=}')
         logger.info(f'{no_label_limit=}')
         logger.info(f'{n_nearest_across_lines=}')
 
-        self.use_separate_labels = use_separate_labels
         self.n_nearest = n_nearest
-        self.first_word = first_word
         self.max_depth = max_depth
         self.n_estimators = n_estimators
+        self.use_separate_labels = use_separate_labels
         self.no_label_limit = no_label_limit
+        self.first_word = first_word
         self.n_nearest_across_lines = n_nearest_across_lines
 
+        # label set clf hyperparameters
+        self.label_set_n_nearest_template = kwargs.get('label_set_n_nearest_template', 5)
+        self.label_set_max_depth = kwargs.get('label_set_max_depth', 100)
+        self.label_set_n_estimators = kwargs.get('label_set_n_estimators', 100)
+        logger.info(f'label_set_n_nearest_template={self.label_set_n_nearest_template}')
+        logger.info(f'label_set_max_depth={self.label_set_max_depth}')
+        logger.info(f'label_set_n_estimators={self.label_set_n_estimators}')
+
         self.tokenizer = tokenizer
         logger.info(f'{tokenizer=}')
 
         self.clf = None
 
         self.no_label_set_name = None
         self.no_label_name = None
```

### Comparing `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/trainer/tokenization.py` & `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/trainer/tokenization.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/trainer/utils.py` & `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/trainer/utils.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/urls.py` & `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/urls.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/utils.py` & `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk.egg-info/PKG-INFO` & `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konfuzio_sdk
-Version: 0.3.4.dev20240502164651
+Version: 0.3.4.dev20240503144208
 Summary: Konfuzio Software Development Kit
 Home-page: https://github.com/konfuzio-ai/konfuzio-sdk/
 Author: Helm & Nagel GmbH
 Author-email: info@helm-nagel.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: certifi==2023.7.22
```

### Comparing `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk.egg-info/SOURCES.txt` & `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk.egg-info/requires.txt` & `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240502164651/setup.py` & `konfuzio_sdk-0.3.4.dev20240503144208/setup.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240502164651/tests/test_api.py` & `konfuzio_sdk-0.3.4.dev20240503144208/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240502164651/tests/test_cli.py` & `konfuzio_sdk-0.3.4.dev20240503144208/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240502164651/tests/test_data.py` & `konfuzio_sdk-0.3.4.dev20240503144208/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240502164651/tests/test_evaluate.py` & `konfuzio_sdk-0.3.4.dev20240503144208/tests/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240502164651/tests/test_extras.py` & `konfuzio_sdk-0.3.4.dev20240503144208/tests/test_extras.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240502164651/tests/test_normalize.py` & `konfuzio_sdk-0.3.4.dev20240503144208/tests/test_normalize.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240502164651/tests/test_regex.py` & `konfuzio_sdk-0.3.4.dev20240503144208/tests/test_regex.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240502164651/tests/test_samples.py` & `konfuzio_sdk-0.3.4.dev20240503144208/tests/test_samples.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240502164651/tests/test_urls.py` & `konfuzio_sdk-0.3.4.dev20240503144208/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240502164651/tests/test_utils.py` & `konfuzio_sdk-0.3.4.dev20240503144208/tests/test_utils.py`

 * *Files identical despite different names*

