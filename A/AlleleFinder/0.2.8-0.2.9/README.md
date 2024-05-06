# Comparing `tmp/allelefinder-0.2.8.tar.gz` & `tmp/allelefinder-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allelefinder-0.2.8.tar", last modified: Mon May  6 15:27:29 2024, max compression
+gzip compressed data, was "allelefinder-0.2.9.tar", last modified: Mon May  6 15:41:22 2024, max compression
```

## Comparing `allelefinder-0.2.8.tar` & `allelefinder-0.2.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:27:29.907987 allelefinder-0.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:27:29.907987 allelefinder-0.2.8/AlleleFinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-05-06 15:27:29.000000 allelefinder-0.2.8/AlleleFinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-06 15:27:29.000000 allelefinder-0.2.8/AlleleFinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 15:27:29.000000 allelefinder-0.2.8/AlleleFinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-06 15:27:29.000000 allelefinder-0.2.8/AlleleFinder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-06 15:27:29.000000 allelefinder-0.2.8/AlleleFinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-06 15:27:29.000000 allelefinder-0.2.8/AlleleFinder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-06 15:27:21.000000 allelefinder-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-06 15:27:21.000000 allelefinder-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-05-06 15:27:29.907987 allelefinder-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-05-06 15:27:21.000000 allelefinder-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:27:29.903987 allelefinder-0.2.8/allele_tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:27:21.000000 allelefinder-0.2.8/allele_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26836 2024-05-06 15:27:21.000000 allelefinder-0.2.8/allele_tools/allele_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    38776 2024-05-06 15:27:21.000000 allelefinder-0.2.8/allele_tools/allele_translate_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)    31560 2024-05-06 15:27:21.000000 allelefinder-0.2.8/allele_tools/allele_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)   121713 2024-05-06 15:27:21.000000 allelefinder-0.2.8/allele_tools/methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-05-06 15:27:21.000000 allelefinder-0.2.8/allele_tools/profile_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)    53101 2024-05-06 15:27:21.000000 allelefinder-0.2.8/allele_tools/stec.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-06 15:27:21.000000 allelefinder-0.2.8/allele_tools/version.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-06 15:27:21.000000 allelefinder-0.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 15:27:29.907987 allelefinder-0.2.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2298 2024-05-06 15:27:21.000000 allelefinder-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:27:29.903987 allelefinder-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:27:21.000000 allelefinder-0.2.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15501 2024-05-06 15:27:21.000000 allelefinder-0.2.8/tests/test_0_profile_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)    15193 2024-05-06 15:27:21.000000 allelefinder-0.2.8/tests/test_1_allele_translate_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)    15736 2024-05-06 15:27:21.000000 allelefinder-0.2.8/tests/test_2_allele_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-05-06 15:27:21.000000 allelefinder-0.2.8/tests/test_3_stec_profile_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-05-06 15:27:21.000000 allelefinder-0.2.8/tests/test_4_stec_allele_translate_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-05-06 15:27:21.000000 allelefinder-0.2.8/tests/test_5_stec_allele_find.py
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-05-06 15:27:21.000000 allelefinder-0.2.8/tests/test_6_stec_aa_allele_find.py
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-05-06 15:27:21.000000 allelefinder-0.2.8/tests/test_7_stec_allele_split.py
--rw-r--r--   0 runner    (1001) docker     (127)    17176 2024-05-06 15:27:21.000000 allelefinder-0.2.8/tests/test_8_stec_allele_concatenate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-05-06 15:27:21.000000 allelefinder-0.2.8/tests/test_9_stec_allele_translate_find.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:41:22.175762 allelefinder-0.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:41:22.175762 allelefinder-0.2.9/AlleleFinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-05-06 15:41:22.000000 allelefinder-0.2.9/AlleleFinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-06 15:41:22.000000 allelefinder-0.2.9/AlleleFinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 15:41:22.000000 allelefinder-0.2.9/AlleleFinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-06 15:41:22.000000 allelefinder-0.2.9/AlleleFinder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-06 15:41:22.000000 allelefinder-0.2.9/AlleleFinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-06 15:41:22.000000 allelefinder-0.2.9/AlleleFinder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-06 15:41:13.000000 allelefinder-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-06 15:41:13.000000 allelefinder-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-05-06 15:41:22.175762 allelefinder-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-05-06 15:41:13.000000 allelefinder-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:41:22.171762 allelefinder-0.2.9/allele_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:41:13.000000 allelefinder-0.2.9/allele_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26836 2024-05-06 15:41:13.000000 allelefinder-0.2.9/allele_tools/allele_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38776 2024-05-06 15:41:13.000000 allelefinder-0.2.9/allele_tools/allele_translate_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31560 2024-05-06 15:41:13.000000 allelefinder-0.2.9/allele_tools/allele_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)   121713 2024-05-06 15:41:13.000000 allelefinder-0.2.9/allele_tools/methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-05-06 15:41:13.000000 allelefinder-0.2.9/allele_tools/profile_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53101 2024-05-06 15:41:13.000000 allelefinder-0.2.9/allele_tools/stec.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-06 15:41:13.000000 allelefinder-0.2.9/allele_tools/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-06 15:41:13.000000 allelefinder-0.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 15:41:22.175762 allelefinder-0.2.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2298 2024-05-06 15:41:13.000000 allelefinder-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:41:22.175762 allelefinder-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:41:13.000000 allelefinder-0.2.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15501 2024-05-06 15:41:13.000000 allelefinder-0.2.9/tests/test_0_profile_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15193 2024-05-06 15:41:13.000000 allelefinder-0.2.9/tests/test_1_allele_translate_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15736 2024-05-06 15:41:13.000000 allelefinder-0.2.9/tests/test_2_allele_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-05-06 15:41:13.000000 allelefinder-0.2.9/tests/test_3_stec_profile_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-05-06 15:41:13.000000 allelefinder-0.2.9/tests/test_4_stec_allele_translate_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-05-06 15:41:13.000000 allelefinder-0.2.9/tests/test_5_stec_allele_find.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-05-06 15:41:13.000000 allelefinder-0.2.9/tests/test_6_stec_aa_allele_find.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-05-06 15:41:13.000000 allelefinder-0.2.9/tests/test_7_stec_allele_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17176 2024-05-06 15:41:13.000000 allelefinder-0.2.9/tests/test_8_stec_allele_concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-05-06 15:41:13.000000 allelefinder-0.2.9/tests/test_9_stec_allele_translate_find.py
```

### Comparing `allelefinder-0.2.8/AlleleFinder.egg-info/PKG-INFO` & `allelefinder-0.2.9/AlleleFinder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlleleFinder
-Version: 0.2.8
+Version: 0.2.9
 Home-page: https://github.com/OLC-Bioinformatics/AlleleFinder
 Author: Adam Koziol
 Author-email: adam.koziol@inspection.gc.ca
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `allelefinder-0.2.8/AlleleFinder.egg-info/SOURCES.txt` & `allelefinder-0.2.9/AlleleFinder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `allelefinder-0.2.8/LICENSE` & `allelefinder-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `allelefinder-0.2.8/PKG-INFO` & `allelefinder-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlleleFinder
-Version: 0.2.8
+Version: 0.2.9
 Home-page: https://github.com/OLC-Bioinformatics/AlleleFinder
 Author: Adam Koziol
 Author-email: adam.koziol@inspection.gc.ca
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `allelefinder-0.2.8/README.md` & `allelefinder-0.2.9/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -55,8 +55,8 @@
 
 ## Feedback
 
 We welcome your feedback. If you encounter any issues installing or running AlleleFinder, have feature requests, or need assistance, please [open an issue on GitHub](https://github.com/OLC-Bioinformatics/AlleleFinder/issues/new/choose).
 
 ## License
 
-AlleleFinder is licensed under the MIT License. See the [LICENSE](https://github.com/OLC-Bioinformatics/AlleleFinder/blob/main/LICENSE) file for more details.
+AlleleFinder is licensed under the MIT License. See the [LICENSE](https://github.com/OLC-Bioinformatics/AlleleFinder/blob/main/LICENSE) file for more details.
```

### Comparing `allelefinder-0.2.8/allele_tools/allele_profiler.py` & `allelefinder-0.2.9/allele_tools/allele_profiler.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.2.8/allele_tools/allele_translate_reduce.py` & `allelefinder-0.2.9/allele_tools/allele_translate_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.2.8/allele_tools/allele_updater.py` & `allelefinder-0.2.9/allele_tools/allele_updater.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.2.8/allele_tools/methods.py` & `allelefinder-0.2.9/allele_tools/methods.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.2.8/allele_tools/profile_reduce.py` & `allelefinder-0.2.9/allele_tools/profile_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.2.8/allele_tools/stec.py` & `allelefinder-0.2.9/allele_tools/stec.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.2.8/setup.py` & `allelefinder-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.2.8/tests/test_0_profile_reduce.py` & `allelefinder-0.2.9/tests/test_0_profile_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.2.8/tests/test_1_allele_translate_reduce.py` & `allelefinder-0.2.9/tests/test_1_allele_translate_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.2.8/tests/test_2_allele_updater.py` & `allelefinder-0.2.9/tests/test_2_allele_updater.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.2.8/tests/test_3_stec_profile_reduce.py` & `allelefinder-0.2.9/tests/test_3_stec_profile_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.2.8/tests/test_4_stec_allele_translate_reduce.py` & `allelefinder-0.2.9/tests/test_4_stec_allele_translate_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.2.8/tests/test_5_stec_allele_find.py` & `allelefinder-0.2.9/tests/test_5_stec_allele_find.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.2.8/tests/test_6_stec_aa_allele_find.py` & `allelefinder-0.2.9/tests/test_6_stec_aa_allele_find.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.2.8/tests/test_7_stec_allele_split.py` & `allelefinder-0.2.9/tests/test_7_stec_allele_split.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.2.8/tests/test_8_stec_allele_concatenate.py` & `allelefinder-0.2.9/tests/test_8_stec_allele_concatenate.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.2.8/tests/test_9_stec_allele_translate_find.py` & `allelefinder-0.2.9/tests/test_9_stec_allele_translate_find.py`

 * *Files identical despite different names*

