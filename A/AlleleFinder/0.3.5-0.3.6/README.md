# Comparing `tmp/allelefinder-0.3.5.tar.gz` & `tmp/allelefinder-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allelefinder-0.3.5.tar", last modified: Mon May  6 17:58:14 2024, max compression
+gzip compressed data, was "allelefinder-0.3.6.tar", last modified: Mon May  6 18:11:03 2024, max compression
```

## Comparing `allelefinder-0.3.5.tar` & `allelefinder-0.3.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:58:14.523997 allelefinder-0.3.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:58:14.523997 allelefinder-0.3.5/AlleleFinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-05-06 17:58:14.000000 allelefinder-0.3.5/AlleleFinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-06 17:58:14.000000 allelefinder-0.3.5/AlleleFinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 17:58:14.000000 allelefinder-0.3.5/AlleleFinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-06 17:58:14.000000 allelefinder-0.3.5/AlleleFinder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-06 17:58:14.000000 allelefinder-0.3.5/AlleleFinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-06 17:58:14.000000 allelefinder-0.3.5/AlleleFinder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-06 17:58:06.000000 allelefinder-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-06 17:58:06.000000 allelefinder-0.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-05-06 17:58:14.523997 allelefinder-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-05-06 17:58:06.000000 allelefinder-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:58:14.519997 allelefinder-0.3.5/allele_tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 17:58:06.000000 allelefinder-0.3.5/allele_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26836 2024-05-06 17:58:06.000000 allelefinder-0.3.5/allele_tools/allele_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    38776 2024-05-06 17:58:06.000000 allelefinder-0.3.5/allele_tools/allele_translate_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)    31560 2024-05-06 17:58:06.000000 allelefinder-0.3.5/allele_tools/allele_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)   121713 2024-05-06 17:58:06.000000 allelefinder-0.3.5/allele_tools/methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-05-06 17:58:06.000000 allelefinder-0.3.5/allele_tools/profile_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)    53101 2024-05-06 17:58:06.000000 allelefinder-0.3.5/allele_tools/stec.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-06 17:58:06.000000 allelefinder-0.3.5/allele_tools/version.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-06 17:58:06.000000 allelefinder-0.3.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 17:58:14.523997 allelefinder-0.3.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2298 2024-05-06 17:58:06.000000 allelefinder-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:58:14.523997 allelefinder-0.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 17:58:06.000000 allelefinder-0.3.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15501 2024-05-06 17:58:06.000000 allelefinder-0.3.5/tests/test_0_profile_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)    15193 2024-05-06 17:58:06.000000 allelefinder-0.3.5/tests/test_1_allele_translate_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)    15736 2024-05-06 17:58:06.000000 allelefinder-0.3.5/tests/test_2_allele_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-05-06 17:58:06.000000 allelefinder-0.3.5/tests/test_3_stec_profile_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-05-06 17:58:06.000000 allelefinder-0.3.5/tests/test_4_stec_allele_translate_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-05-06 17:58:06.000000 allelefinder-0.3.5/tests/test_5_stec_allele_find.py
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-05-06 17:58:06.000000 allelefinder-0.3.5/tests/test_6_stec_aa_allele_find.py
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-05-06 17:58:06.000000 allelefinder-0.3.5/tests/test_7_stec_allele_split.py
--rw-r--r--   0 runner    (1001) docker     (127)    17176 2024-05-06 17:58:06.000000 allelefinder-0.3.5/tests/test_8_stec_allele_concatenate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-05-06 17:58:06.000000 allelefinder-0.3.5/tests/test_9_stec_allele_translate_find.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:11:03.340044 allelefinder-0.3.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:11:03.340044 allelefinder-0.3.6/AlleleFinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-05-06 18:11:03.000000 allelefinder-0.3.6/AlleleFinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-06 18:11:03.000000 allelefinder-0.3.6/AlleleFinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 18:11:03.000000 allelefinder-0.3.6/AlleleFinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-06 18:11:03.000000 allelefinder-0.3.6/AlleleFinder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-06 18:11:03.000000 allelefinder-0.3.6/AlleleFinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-06 18:11:03.000000 allelefinder-0.3.6/AlleleFinder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-06 18:10:55.000000 allelefinder-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-06 18:10:55.000000 allelefinder-0.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-05-06 18:11:03.340044 allelefinder-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-05-06 18:10:55.000000 allelefinder-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:11:03.336044 allelefinder-0.3.6/allele_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 18:10:55.000000 allelefinder-0.3.6/allele_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26836 2024-05-06 18:10:55.000000 allelefinder-0.3.6/allele_tools/allele_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38776 2024-05-06 18:10:55.000000 allelefinder-0.3.6/allele_tools/allele_translate_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31560 2024-05-06 18:10:55.000000 allelefinder-0.3.6/allele_tools/allele_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)   121713 2024-05-06 18:10:55.000000 allelefinder-0.3.6/allele_tools/methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-05-06 18:10:55.000000 allelefinder-0.3.6/allele_tools/profile_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53101 2024-05-06 18:10:55.000000 allelefinder-0.3.6/allele_tools/stec.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-06 18:10:55.000000 allelefinder-0.3.6/allele_tools/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-06 18:10:55.000000 allelefinder-0.3.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 18:11:03.340044 allelefinder-0.3.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2298 2024-05-06 18:10:55.000000 allelefinder-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:11:03.340044 allelefinder-0.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 18:10:55.000000 allelefinder-0.3.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15501 2024-05-06 18:10:55.000000 allelefinder-0.3.6/tests/test_0_profile_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15193 2024-05-06 18:10:55.000000 allelefinder-0.3.6/tests/test_1_allele_translate_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15736 2024-05-06 18:10:55.000000 allelefinder-0.3.6/tests/test_2_allele_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-05-06 18:10:55.000000 allelefinder-0.3.6/tests/test_3_stec_profile_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-05-06 18:10:55.000000 allelefinder-0.3.6/tests/test_4_stec_allele_translate_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-05-06 18:10:55.000000 allelefinder-0.3.6/tests/test_5_stec_allele_find.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-05-06 18:10:55.000000 allelefinder-0.3.6/tests/test_6_stec_aa_allele_find.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-05-06 18:10:55.000000 allelefinder-0.3.6/tests/test_7_stec_allele_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17176 2024-05-06 18:10:55.000000 allelefinder-0.3.6/tests/test_8_stec_allele_concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-05-06 18:10:55.000000 allelefinder-0.3.6/tests/test_9_stec_allele_translate_find.py
```

### Comparing `allelefinder-0.3.5/AlleleFinder.egg-info/PKG-INFO` & `allelefinder-0.3.6/AlleleFinder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlleleFinder
-Version: 0.3.5
+Version: 0.3.6
 Home-page: https://github.com/OLC-Bioinformatics/AlleleFinder
 Author: Adam Koziol
 Author-email: adam.koziol@inspection.gc.ca
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `allelefinder-0.3.5/AlleleFinder.egg-info/SOURCES.txt` & `allelefinder-0.3.6/AlleleFinder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `allelefinder-0.3.5/LICENSE` & `allelefinder-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `allelefinder-0.3.5/PKG-INFO` & `allelefinder-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlleleFinder
-Version: 0.3.5
+Version: 0.3.6
 Home-page: https://github.com/OLC-Bioinformatics/AlleleFinder
 Author: Adam Koziol
 Author-email: adam.koziol@inspection.gc.ca
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `allelefinder-0.3.5/README.md` & `allelefinder-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `allelefinder-0.3.5/allele_tools/allele_profiler.py` & `allelefinder-0.3.6/allele_tools/allele_profiler.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.3.5/allele_tools/allele_translate_reduce.py` & `allelefinder-0.3.6/allele_tools/allele_translate_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.3.5/allele_tools/allele_updater.py` & `allelefinder-0.3.6/allele_tools/allele_updater.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.3.5/allele_tools/methods.py` & `allelefinder-0.3.6/allele_tools/methods.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.3.5/allele_tools/profile_reduce.py` & `allelefinder-0.3.6/allele_tools/profile_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.3.5/allele_tools/stec.py` & `allelefinder-0.3.6/allele_tools/stec.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.3.5/setup.py` & `allelefinder-0.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.3.5/tests/test_0_profile_reduce.py` & `allelefinder-0.3.6/tests/test_0_profile_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.3.5/tests/test_1_allele_translate_reduce.py` & `allelefinder-0.3.6/tests/test_1_allele_translate_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.3.5/tests/test_2_allele_updater.py` & `allelefinder-0.3.6/tests/test_2_allele_updater.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.3.5/tests/test_3_stec_profile_reduce.py` & `allelefinder-0.3.6/tests/test_3_stec_profile_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.3.5/tests/test_4_stec_allele_translate_reduce.py` & `allelefinder-0.3.6/tests/test_4_stec_allele_translate_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.3.5/tests/test_5_stec_allele_find.py` & `allelefinder-0.3.6/tests/test_5_stec_allele_find.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.3.5/tests/test_6_stec_aa_allele_find.py` & `allelefinder-0.3.6/tests/test_6_stec_aa_allele_find.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.3.5/tests/test_7_stec_allele_split.py` & `allelefinder-0.3.6/tests/test_7_stec_allele_split.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.3.5/tests/test_8_stec_allele_concatenate.py` & `allelefinder-0.3.6/tests/test_8_stec_allele_concatenate.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.3.5/tests/test_9_stec_allele_translate_find.py` & `allelefinder-0.3.6/tests/test_9_stec_allele_translate_find.py`

 * *Files identical despite different names*
