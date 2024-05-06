# Comparing `tmp/lifton-1.0.0.tar.gz` & `tmp/lifton-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifton-1.0.0.tar", last modified: Thu Apr 25 19:31:45 2024, max compression
+gzip compressed data, was "lifton-1.0.1.tar", last modified: Mon May  6 01:24:29 2024, max compression
```

## Comparing `lifton-1.0.0.tar` & `lifton-1.0.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwsr-x   0 kh.chao   (3822) salzberg_ifx  (5042)        0 2024-04-25 19:31:45.271436 lifton-1.0.0/
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    34599 2024-01-03 20:18:51.000000 lifton-1.0.0/LICENSE
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    27871 2024-04-25 19:31:45.259436 lifton-1.0.0/PKG-INFO
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    27543 2024-04-25 19:31:21.000000 lifton-1.0.0/README.md
-drwxrwsr-x   0 kh.chao   (3822) salzberg_ifx  (5042)        0 2024-04-25 19:31:44.231434 lifton-1.0.0/lifton/
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)       23 2024-04-25 19:16:25.000000 lifton-1.0.0/lifton/__init__.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     8659 2024-04-19 19:09:42.000000 lifton-1.0.0/lifton/align.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     6640 2024-04-25 19:14:34.000000 lifton-1.0.0/lifton/annotation.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     2620 2024-04-21 18:41:09.000000 lifton-1.0.0/lifton/extract_sequence.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     1823 2024-04-21 18:41:11.000000 lifton-1.0.0/lifton/get_id_fraction.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      578 2024-04-19 19:16:38.000000 lifton-1.0.0/lifton/intervals.py
-drwxrwsr-x   0 kh.chao   (3822) salzberg_ifx  (5042)        0 2024-04-25 19:31:45.088436 lifton-1.0.0/lifton/liftoff/
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)        0 2023-12-24 02:47:54.000000 lifton-1.0.0/lifton/liftoff/__init__.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    13175 2023-12-24 03:45:20.000000 lifton-1.0.0/lifton/liftoff/align_features.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      597 2023-12-24 03:45:20.000000 lifton-1.0.0/lifton/liftoff/aligned_seg.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    10276 2023-12-24 03:45:20.000000 lifton-1.0.0/lifton/liftoff/extract_features.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      190 2023-12-24 03:45:20.000000 lifton-1.0.0/lifton/liftoff/feature_hierarchy.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    19044 2023-12-24 03:45:20.000000 lifton-1.0.0/lifton/liftoff/find_best_mapping.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     9361 2023-12-24 03:45:20.000000 lifton-1.0.0/lifton/liftoff/fix_overlapping_features.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     5664 2023-12-24 03:45:20.000000 lifton-1.0.0/lifton/liftoff/lift_features.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    15486 2024-02-12 19:50:40.000000 lifton-1.0.0/lifton/liftoff/liftoff_main.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     4032 2023-12-24 03:45:20.000000 lifton-1.0.0/lifton/liftoff/liftoff_utils.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     5206 2023-12-24 03:45:20.000000 lifton-1.0.0/lifton/liftoff/liftover_types.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     3945 2023-12-24 03:45:20.000000 lifton-1.0.0/lifton/liftoff/merge_lifted_features.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      372 2023-12-24 03:45:20.000000 lifton-1.0.0/lifton/liftoff/new_feature.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    14008 2023-12-24 03:45:20.000000 lifton-1.0.0/lifton/liftoff/polish.py
-drwxrwsr-x   0 kh.chao   (3822) salzberg_ifx  (5042)        0 2024-04-25 19:31:45.210436 lifton-1.0.0/lifton/liftoff/tests/
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)        1 2023-12-24 03:45:20.000000 lifton-1.0.0/lifton/liftoff/tests/__init__.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     2058 2023-12-24 03:45:19.000000 lifton-1.0.0/lifton/liftoff/tests/test_advanced.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     1895 2023-12-24 03:45:19.000000 lifton-1.0.0/lifton/liftoff/tests/test_basic.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     5428 2023-12-24 03:45:20.000000 lifton-1.0.0/lifton/liftoff/write_new_gff.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    20402 2024-04-24 11:32:28.000000 lifton-1.0.0/lifton/lifton.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    34533 2024-04-21 22:08:34.000000 lifton-1.0.0/lifton/lifton_class.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    20597 2024-04-24 11:32:28.000000 lifton-1.0.0/lifton/lifton_utils.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      233 2024-01-24 15:32:08.000000 lifton-1.0.0/lifton/logger.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     7585 2024-04-21 00:36:04.000000 lifton-1.0.0/lifton/protein_maximization.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     5764 2024-04-21 23:00:23.000000 lifton-1.0.0/lifton/run_evaluation.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     9031 2024-04-24 11:32:28.000000 lifton-1.0.0/lifton/run_liftoff.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     6507 2024-04-24 11:32:28.000000 lifton-1.0.0/lifton/run_miniprot.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     5595 2024-04-21 21:25:50.000000 lifton-1.0.0/lifton/stats.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     4191 2024-04-21 22:07:42.000000 lifton-1.0.0/lifton/variants.py
-drwxrwsr-x   0 kh.chao   (3822) salzberg_ifx  (5042)        0 2024-04-25 19:31:44.479434 lifton-1.0.0/lifton.egg-info/
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    27871 2024-04-25 19:31:43.000000 lifton-1.0.0/lifton.egg-info/PKG-INFO
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     1154 2024-04-25 19:31:43.000000 lifton-1.0.0/lifton.egg-info/SOURCES.txt
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)        1 2024-04-25 19:31:43.000000 lifton-1.0.0/lifton.egg-info/dependency_links.txt
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)       46 2024-04-25 19:31:43.000000 lifton-1.0.0/lifton.egg-info/entry_points.txt
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      168 2024-04-25 19:31:43.000000 lifton-1.0.0/lifton.egg-info/requires.txt
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)        7 2024-04-25 19:31:43.000000 lifton-1.0.0/lifton.egg-info/top_level.txt
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)       38 2024-04-25 19:31:45.280436 lifton-1.0.0/setup.cfg
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      865 2024-04-25 19:17:04.000000 lifton-1.0.0/setup.py
+drwxrwsr-x   0 kh.chao   (3822) salzberg_ifx  (5042)        0 2024-05-06 01:24:29.460955 lifton-1.0.1/
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    34599 2024-01-03 20:18:51.000000 lifton-1.0.1/LICENSE
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    27871 2024-05-06 01:24:29.449955 lifton-1.0.1/PKG-INFO
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    27543 2024-05-06 01:23:28.000000 lifton-1.0.1/README.md
+drwxrwsr-x   0 kh.chao   (3822) salzberg_ifx  (5042)        0 2024-05-06 01:24:28.146952 lifton-1.0.1/lifton/
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)       23 2024-05-06 01:22:29.000000 lifton-1.0.1/lifton/__init__.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     8659 2024-04-19 19:09:42.000000 lifton-1.0.1/lifton/align.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     6640 2024-04-25 19:14:34.000000 lifton-1.0.1/lifton/annotation.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     2620 2024-04-21 18:41:09.000000 lifton-1.0.1/lifton/extract_sequence.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     1823 2024-04-21 18:41:11.000000 lifton-1.0.1/lifton/get_id_fraction.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      578 2024-04-19 19:16:38.000000 lifton-1.0.1/lifton/intervals.py
+drwxrwsr-x   0 kh.chao   (3822) salzberg_ifx  (5042)        0 2024-05-06 01:24:29.253954 lifton-1.0.1/lifton/liftoff/
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)        0 2023-12-24 02:47:54.000000 lifton-1.0.1/lifton/liftoff/__init__.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    13175 2023-12-24 03:45:20.000000 lifton-1.0.1/lifton/liftoff/align_features.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      597 2023-12-24 03:45:20.000000 lifton-1.0.1/lifton/liftoff/aligned_seg.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    10276 2023-12-24 03:45:20.000000 lifton-1.0.1/lifton/liftoff/extract_features.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      190 2023-12-24 03:45:20.000000 lifton-1.0.1/lifton/liftoff/feature_hierarchy.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    19044 2023-12-24 03:45:20.000000 lifton-1.0.1/lifton/liftoff/find_best_mapping.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     9361 2023-12-24 03:45:20.000000 lifton-1.0.1/lifton/liftoff/fix_overlapping_features.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     5664 2023-12-24 03:45:20.000000 lifton-1.0.1/lifton/liftoff/lift_features.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    15486 2024-02-12 19:50:40.000000 lifton-1.0.1/lifton/liftoff/liftoff_main.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     4032 2023-12-24 03:45:20.000000 lifton-1.0.1/lifton/liftoff/liftoff_utils.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     5206 2023-12-24 03:45:20.000000 lifton-1.0.1/lifton/liftoff/liftover_types.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     3945 2023-12-24 03:45:20.000000 lifton-1.0.1/lifton/liftoff/merge_lifted_features.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      372 2023-12-24 03:45:20.000000 lifton-1.0.1/lifton/liftoff/new_feature.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    14008 2023-12-24 03:45:20.000000 lifton-1.0.1/lifton/liftoff/polish.py
+drwxrwsr-x   0 kh.chao   (3822) salzberg_ifx  (5042)        0 2024-05-06 01:24:29.394955 lifton-1.0.1/lifton/liftoff/tests/
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)        1 2023-12-24 03:45:20.000000 lifton-1.0.1/lifton/liftoff/tests/__init__.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     2058 2023-12-24 03:45:19.000000 lifton-1.0.1/lifton/liftoff/tests/test_advanced.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     1895 2023-12-24 03:45:19.000000 lifton-1.0.1/lifton/liftoff/tests/test_basic.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     5428 2023-12-24 03:45:20.000000 lifton-1.0.1/lifton/liftoff/write_new_gff.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    20403 2024-05-06 01:23:50.000000 lifton-1.0.1/lifton/lifton.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    34486 2024-05-06 01:21:50.000000 lifton-1.0.1/lifton/lifton_class.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    20597 2024-04-24 11:32:28.000000 lifton-1.0.1/lifton/lifton_utils.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      233 2024-01-24 15:32:08.000000 lifton-1.0.1/lifton/logger.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     7585 2024-05-04 23:05:47.000000 lifton-1.0.1/lifton/protein_maximization.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     5764 2024-04-21 23:00:23.000000 lifton-1.0.1/lifton/run_evaluation.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     9031 2024-05-06 01:01:57.000000 lifton-1.0.1/lifton/run_liftoff.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     6350 2024-05-05 21:10:16.000000 lifton-1.0.1/lifton/run_miniprot.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     5595 2024-04-21 21:25:50.000000 lifton-1.0.1/lifton/stats.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     4191 2024-04-21 22:07:42.000000 lifton-1.0.1/lifton/variants.py
+drwxrwsr-x   0 kh.chao   (3822) salzberg_ifx  (5042)        0 2024-05-06 01:24:28.384953 lifton-1.0.1/lifton.egg-info/
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    27871 2024-05-06 01:24:26.000000 lifton-1.0.1/lifton.egg-info/PKG-INFO
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     1154 2024-05-06 01:24:26.000000 lifton-1.0.1/lifton.egg-info/SOURCES.txt
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)        1 2024-05-06 01:24:26.000000 lifton-1.0.1/lifton.egg-info/dependency_links.txt
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)       46 2024-05-06 01:24:26.000000 lifton-1.0.1/lifton.egg-info/entry_points.txt
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      168 2024-05-06 01:24:26.000000 lifton-1.0.1/lifton.egg-info/requires.txt
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)        7 2024-05-06 01:24:26.000000 lifton-1.0.1/lifton.egg-info/top_level.txt
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)       38 2024-05-06 01:24:29.470955 lifton-1.0.1/setup.cfg
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      865 2024-05-06 01:22:42.000000 lifton-1.0.1/setup.py
```

### Comparing `lifton-1.0.0/LICENSE` & `lifton-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lifton-1.0.0/PKG-INFO` & `lifton-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifton
-Version: 1.0.0
+Version: 1.0.1
 Summary: Combining DNA and protein alignments to improve genome annotation with LiftOn
 Home-page: https://github.com/Kuanhao-Chao/Lifton
 Author: Kuan-Hao Chao
 Author-email: kh.chao@cs.jhu.edu
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -181,15 +181,15 @@
 </li>
 <li class="toctree-l1"><a class="reference internal" href="https://ccb.jhu.edu/lifton/content/how_to_page.html">FAQ ...</a></li>
 <li class="toctree-l1"><a class="reference internal" href="https://ccb.jhu.edu/lifton/content/function_manual.html">User Manual</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="https://ccb.jhu.edu/lifton/content/function_manual.html#lifton">LiftOn</a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="https://ccb.jhu.edu/lifton/content/changelog.html">Changelog</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="https://ccb.jhu.edu/lifton/content/changelog.html#v1-0-0">v1.0.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="https://ccb.jhu.edu/lifton/content/changelog.html#v1-0-0">v1.0.1</a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="https://ccb.jhu.edu/lifton/content/license.html">License</a></li>
 <li class="toctree-l1"><a class="reference internal" href="https://ccb.jhu.edu/lifton/content/contact.html">Contact</a></li>
 </ul>
 </div>
 <div class="line-block">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lifton Version: 1.0.0 Summary: Combining DNA and
+Metadata-Version: 2.1 Name: lifton Version: 1.0.1 Summary: Combining DNA and
 protein alignments to improve genome annotation with LiftOn Home-page: https://
 github.com/Kuanhao-Chao/Lifton Author: Kuan-Hao Chao Author-email:
 kh.chao@cs.jhu.edu Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE[My Logo]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_G_P_L_v_3_-_y_e_l_l_o_w_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _b_a_d_g_e_/_v_e_r_s_i_o_n_-_v_._0_._0_._1_-_b_l_u_e_]_[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_p_e_r_s_o_n_a_l_i_z_e_d_-_b_a_d_g_e_/
 _l_i_f_t_o_n_?_p_e_r_i_o_d_=_t_o_t_a_l_&_u_n_i_t_s_=_a_b_b_r_e_v_i_a_t_i_o_n_&_l_e_f_t___c_o_l_o_r_=_g_r_e_y_&_r_i_g_h_t___c_o_l_o_r_=_b_l_u_e_&_l_e_f_t___t_e_x_t_=_P_y_P_i_%_2_0_d_o_w_n_l_o_a_d_s_]
@@ -139,15 +139,15 @@
           o _P_r_o_t_e_i_n_-_m_a_x_i_m_i_z_a_t_i_o_n_ _a_l_g_o_r_i_t_h_m
           o _M_u_t_a_t_i_o_n_ _r_e_p_o_r_t
           o _R_e_f_e_r_e_n_c_e
     * _F_A_Q_ _._._.
     * _U_s_e_r_ _M_a_n_u_a_l
           o _L_i_f_t_O_n
     * _C_h_a_n_g_e_l_o_g
-          o _v_1_._0_._0
+          o _v_1_._0_._1
     * _L_i_c_e_n_s_e
     * _C_o_n_t_a_c_t
 
 ********** LLiiffttOOnn''ss lliimmiittaattiioonn_## **********
 LiftOn's cchhaaiinniinngg aallggoorriitthhmm currently only utilizes miniprot alignment results
 to fix the Liftoff annotation. However, it can be extended to chain together
 multiple DNA- and protein-based annotation files or aasembled RNA-Seq
```

### Comparing `lifton-1.0.0/README.md` & `lifton-1.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,15 @@
 </li>
 <li class="toctree-l1"><a class="reference internal" href="https://ccb.jhu.edu/lifton/content/how_to_page.html">FAQ ...</a></li>
 <li class="toctree-l1"><a class="reference internal" href="https://ccb.jhu.edu/lifton/content/function_manual.html">User Manual</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="https://ccb.jhu.edu/lifton/content/function_manual.html#lifton">LiftOn</a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="https://ccb.jhu.edu/lifton/content/changelog.html">Changelog</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="https://ccb.jhu.edu/lifton/content/changelog.html#v1-0-0">v1.0.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="https://ccb.jhu.edu/lifton/content/changelog.html#v1-0-0">v1.0.1</a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="https://ccb.jhu.edu/lifton/content/license.html">License</a></li>
 <li class="toctree-l1"><a class="reference internal" href="https://ccb.jhu.edu/lifton/content/contact.html">Contact</a></li>
 </ul>
 </div>
 <div class="line-block">
```

#### html2text {}

```diff
@@ -135,15 +135,15 @@
           o _P_r_o_t_e_i_n_-_m_a_x_i_m_i_z_a_t_i_o_n_ _a_l_g_o_r_i_t_h_m
           o _M_u_t_a_t_i_o_n_ _r_e_p_o_r_t
           o _R_e_f_e_r_e_n_c_e
     * _F_A_Q_ _._._.
     * _U_s_e_r_ _M_a_n_u_a_l
           o _L_i_f_t_O_n
     * _C_h_a_n_g_e_l_o_g
-          o _v_1_._0_._0
+          o _v_1_._0_._1
     * _L_i_c_e_n_s_e
     * _C_o_n_t_a_c_t
 
 ********** LLiiffttOOnn''ss lliimmiittaattiioonn_## **********
 LiftOn's cchhaaiinniinngg aallggoorriitthhmm currently only utilizes miniprot alignment results
 to fix the Liftoff annotation. However, it can be extended to chain together
 multiple DNA- and protein-based annotation files or aasembled RNA-Seq
```

### Comparing `lifton-1.0.0/lifton/align.py` & `lifton-1.0.1/lifton/align.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.0/lifton/annotation.py` & `lifton-1.0.1/lifton/annotation.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.0/lifton/extract_sequence.py` & `lifton-1.0.1/lifton/extract_sequence.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.0/lifton/get_id_fraction.py` & `lifton-1.0.1/lifton/get_id_fraction.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.0/lifton/intervals.py` & `lifton-1.0.1/lifton/intervals.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.0/lifton/liftoff/align_features.py` & `lifton-1.0.1/lifton/liftoff/align_features.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.0/lifton/liftoff/aligned_seg.py` & `lifton-1.0.1/lifton/liftoff/aligned_seg.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.0/lifton/liftoff/extract_features.py` & `lifton-1.0.1/lifton/liftoff/extract_features.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.0/lifton/liftoff/find_best_mapping.py` & `lifton-1.0.1/lifton/liftoff/find_best_mapping.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.0/lifton/liftoff/fix_overlapping_features.py` & `lifton-1.0.1/lifton/liftoff/fix_overlapping_features.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.0/lifton/liftoff/lift_features.py` & `lifton-1.0.1/lifton/liftoff/lift_features.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.0/lifton/liftoff/liftoff_main.py` & `lifton-1.0.1/lifton/liftoff/liftoff_main.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.0/lifton/liftoff/liftoff_utils.py` & `lifton-1.0.1/lifton/liftoff/liftoff_utils.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.0/lifton/liftoff/liftover_types.py` & `lifton-1.0.1/lifton/liftoff/liftover_types.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.0/lifton/liftoff/merge_lifted_features.py` & `lifton-1.0.1/lifton/liftoff/merge_lifted_features.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.0/lifton/liftoff/polish.py` & `lifton-1.0.1/lifton/liftoff/polish.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.0/lifton/liftoff/tests/test_advanced.py` & `lifton-1.0.1/lifton/liftoff/tests/test_advanced.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.0/lifton/liftoff/tests/test_basic.py` & `lifton-1.0.1/lifton/liftoff/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.0/lifton/liftoff/write_new_gff.py` & `lifton-1.0.1/lifton/liftoff/write_new_gff.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.0/lifton/lifton.py` & `lifton-1.0.1/lifton/lifton.py`

 * *Files 1% similar despite different names*

```diff
@@ -292,15 +292,15 @@
     
     ################################
     # Step 7: Process Liftoff genes & transcripts
     #     structure 1: gene -> transcript -> exon
     #     structure 2: transcript -> exon
     ################################
     for feature in features:#CP132235.1:34100723-34103135
-        for locus in l_feature_db.features_of_type(feature):#, limit=("CP132235.1", 34100723, 34303135)):
+        for locus in l_feature_db.features_of_type(feature):#, limit=("NC_051336.1", 29333544, 29357000)):
             lifton_gene = run_liftoff.process_liftoff(None, locus, ref_db.db_connection, l_feature_db, ref_id_2_m_id_trans_dict, m_feature_db, tree_dict, tgt_fai, ref_proteins, ref_trans, ref_features_dict, fw_score, fw_chain, args, ENTRY_FEATURE=True)
             if lifton_gene is None or lifton_gene.ref_gene_id is None:
                 continue
             lifton_gene.write_entry(fw,transcripts_stats_dict)
             if processed_features % 20 == 0:
                 sys.stdout.write("\r>> LiftOn processed: %i features." % processed_features)
             processed_features += 1
```

### Comparing `lifton-1.0.0/lifton/lifton_class.py` & `lifton-1.0.1/lifton/lifton_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -467,32 +467,30 @@
                     cdss_lens.append(exon.cds.entry.end - exon.cds.entry.start + 1)
         return coding_seq, cds_children, cdss_lens
 
     def get_coding_trans_seq(self, fai):
         trans_seq = ""
         coding_seq = ""
         accum_cds_length = 0
-        for exon in self.exons:
+        lcl_exons = []
+        lcl_exons = self.exons
+        if len(self.exons) > 0 and self.exons[0].entry.strand == '-':
+            lcl_exons = self.exons[::-1]
+        for exon in lcl_exons:
             # Chaining the exon features
             p_trans_seq = exon.entry.sequence(fai)
             p_trans_seq = Seq(p_trans_seq).upper()
-            if exon.entry.strand == '-':
-                trans_seq = p_trans_seq + trans_seq
-            elif exon.entry.strand == '+':
-                trans_seq = trans_seq + p_trans_seq
+            trans_seq = trans_seq + p_trans_seq
             if exon.cds is not None:
                 # Updating CDS frame
                 exon.cds.entry.frame = str(self.__get_cds_frame(accum_cds_length))
-                accum_cds_length = exon.cds.entry.end - exon.cds.entry.start + 1
+                accum_cds_length += (exon.cds.entry.end - exon.cds.entry.start + 1)
                 # Chaining the CDS features
                 p_seq = exon.cds.entry.sequence(fai)
-                if exon.cds.entry.strand == '-':
-                    coding_seq = p_seq + coding_seq
-                elif exon.cds.entry.strand == '+':
-                    coding_seq = coding_seq + p_seq
+                coding_seq = coding_seq + p_seq
         if trans_seq != None:
             trans_seq = str(trans_seq).upper()
         if coding_seq != None:
             coding_seq = str(coding_seq).upper()
         return coding_seq, trans_seq
 
     def translate_coding_seq(self, coding_seq):
@@ -611,16 +609,18 @@
         for exon_idx, exon in enumerate(exons):
             curr_exon_len = exon.entry.end - exon.entry.start + 1
             if accum_exon_length <= final_orf.start:
                 if final_orf.start < accum_exon_length+curr_exon_len:
                     # Create first partial CDS
                     if exon.cds is not None:
                         if strand == "+":
+                            exon.cds.entry.end = exon.entry.end
                             exon.cds.entry.start = exon.entry.start + (final_orf.start - accum_exon_length)
                         elif strand == "-":
+                            exon.cds.entry.start = exon.entry.start 
                             exon.cds.entry.end = exon.entry.end - (final_orf.start - accum_exon_length)
                     else:
                         if strand == "+":
                             exon.add_novel_lifton_cds(exon.entry, exon.entry.start + (final_orf.start - accum_exon_length), exon.entry.end)
                         elif strand == "-":
                             exon.add_novel_lifton_cds(exon.entry, exon.entry.start, exon.entry.end - (final_orf.start - accum_exon_length))
                     exon.cds.entry.frame = str(self.__get_cds_frame(accum_cds_length))
@@ -629,32 +629,32 @@
                     # No CDS should be created
                     exon.cds = None
             elif final_orf.start < accum_exon_length and accum_exon_length < final_orf.end:
                 if final_orf.end <= accum_exon_length+curr_exon_len:
                     # Create the last partial CDS
                     if exon.cds is not None:
                         if strand == "+":
+                            exon.cds.entry.start = exon.entry.start
                             exon.cds.entry.end = exon.entry.start + (final_orf.end - accum_exon_length)-1
                         elif strand == "-":
+                            exon.cds.entry.end = exon.entry.end
                             exon.cds.entry.start = exon.entry.end - (final_orf.end - accum_exon_length)+1
                     else:
                         if strand == "+":
                             exon.add_novel_lifton_cds(exon.entry, exon.entry.start, exon.entry.start + (final_orf.end - accum_exon_length)-1)
                         elif strand == "-":
                             exon.add_novel_lifton_cds(exon.entry, exon.entry.end - (final_orf.end - accum_exon_length)+1, exon.entry.end)
-                    exon.cds.entry.frame = str(self.__get_cds_frame(accum_cds_length))
-                    accum_cds_length += (exon.cds.entry.end - exon.cds.entry.start + 1)
                 else:
                     # Keep the original full CDS / extend the CDS to full exon length
                     if exon.cds is None:
                         exon.add_novel_lifton_cds(exon.entry, exon.entry.start, exon.entry.end)
                     else:
                         exon.cds.update_CDS_info(exon.entry.start, exon.entry.end)
-                    exon.cds.entry.frame = str(self.__get_cds_frame(accum_cds_length))
-                    accum_cds_length += (exon.cds.entry.end - exon.cds.entry.start + 1)
+                exon.cds.entry.frame = str(self.__get_cds_frame(accum_cds_length))
+                accum_cds_length += (exon.cds.entry.end - exon.cds.entry.start + 1)
             elif final_orf.end <= accum_exon_length:
                 # No CDS should be created
                 exon.cds = None
             accum_exon_length += curr_exon_len
 
     def __get_cds_frame(self, accum_cds_length):
         return (3 - accum_cds_length%3)%3
```

### Comparing `lifton-1.0.0/lifton/lifton_utils.py` & `lifton-1.0.1/lifton/lifton_utils.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.0/lifton/protein_maximization.py` & `lifton-1.0.1/lifton/protein_maximization.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.0/lifton/run_evaluation.py` & `lifton-1.0.1/lifton/run_evaluation.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.0/lifton/run_liftoff.py` & `lifton-1.0.1/lifton/run_liftoff.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.0/lifton/run_miniprot.py` & `lifton-1.0.1/lifton/run_miniprot.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,14 @@
         lifton_gene.add_cds(Lifton_trans.entry.id, cds_copy)
     # Update LiftOn status
     lifton_status = lifton_class.Lifton_Status()                
     m_entry = m_feature_db[mtrans_id]
     m_lifton_aln = align.lifton_parasail_align(Lifton_trans, m_entry, tgt_fai, ref_proteins, ref_trans_id)
     lifton_status.annotation =  "miniprot"
     lifton_status.lifton_aa = m_lifton_aln.identity
-    # lifton_trans_aln, lifton_aa_aln = lifton_gene.orf_search_protein(Lifton_trans.entry.id, ref_trans_id, tgt_fai, ref_proteins, ref_trans, lifton_status)
     return lifton_gene, Lifton_trans, Lifton_trans.entry.id, lifton_status
 
 
 def process_miniprot(mtrans, ref_db, m_feature_db, tree_dict, tgt_fai, ref_proteins, ref_trans, ref_features_dict, fw_score, m_id_2_ref_id_trans_dict, ref_features_len_dict, ref_trans_exon_num_dict, ref_features_reverse_dict, args):
     mtrans_id = mtrans.attributes["ID"][0]
     mtrans_interval = Interval(mtrans.start, mtrans.end, mtrans_id)
     is_overlapped = lifton_utils.check_ovps_ratio(mtrans, mtrans_interval, args.overlap, tree_dict)
```

### Comparing `lifton-1.0.0/lifton/stats.py` & `lifton-1.0.1/lifton/stats.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.0/lifton/variants.py` & `lifton-1.0.1/lifton/variants.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.0/lifton.egg-info/PKG-INFO` & `lifton-1.0.1/lifton.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifton
-Version: 1.0.0
+Version: 1.0.1
 Summary: Combining DNA and protein alignments to improve genome annotation with LiftOn
 Home-page: https://github.com/Kuanhao-Chao/Lifton
 Author: Kuan-Hao Chao
 Author-email: kh.chao@cs.jhu.edu
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -181,15 +181,15 @@
 </li>
 <li class="toctree-l1"><a class="reference internal" href="https://ccb.jhu.edu/lifton/content/how_to_page.html">FAQ ...</a></li>
 <li class="toctree-l1"><a class="reference internal" href="https://ccb.jhu.edu/lifton/content/function_manual.html">User Manual</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="https://ccb.jhu.edu/lifton/content/function_manual.html#lifton">LiftOn</a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="https://ccb.jhu.edu/lifton/content/changelog.html">Changelog</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="https://ccb.jhu.edu/lifton/content/changelog.html#v1-0-0">v1.0.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="https://ccb.jhu.edu/lifton/content/changelog.html#v1-0-0">v1.0.1</a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="https://ccb.jhu.edu/lifton/content/license.html">License</a></li>
 <li class="toctree-l1"><a class="reference internal" href="https://ccb.jhu.edu/lifton/content/contact.html">Contact</a></li>
 </ul>
 </div>
 <div class="line-block">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lifton Version: 1.0.0 Summary: Combining DNA and
+Metadata-Version: 2.1 Name: lifton Version: 1.0.1 Summary: Combining DNA and
 protein alignments to improve genome annotation with LiftOn Home-page: https://
 github.com/Kuanhao-Chao/Lifton Author: Kuan-Hao Chao Author-email:
 kh.chao@cs.jhu.edu Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE[My Logo]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_G_P_L_v_3_-_y_e_l_l_o_w_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _b_a_d_g_e_/_v_e_r_s_i_o_n_-_v_._0_._0_._1_-_b_l_u_e_]_[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_p_e_r_s_o_n_a_l_i_z_e_d_-_b_a_d_g_e_/
 _l_i_f_t_o_n_?_p_e_r_i_o_d_=_t_o_t_a_l_&_u_n_i_t_s_=_a_b_b_r_e_v_i_a_t_i_o_n_&_l_e_f_t___c_o_l_o_r_=_g_r_e_y_&_r_i_g_h_t___c_o_l_o_r_=_b_l_u_e_&_l_e_f_t___t_e_x_t_=_P_y_P_i_%_2_0_d_o_w_n_l_o_a_d_s_]
@@ -139,15 +139,15 @@
           o _P_r_o_t_e_i_n_-_m_a_x_i_m_i_z_a_t_i_o_n_ _a_l_g_o_r_i_t_h_m
           o _M_u_t_a_t_i_o_n_ _r_e_p_o_r_t
           o _R_e_f_e_r_e_n_c_e
     * _F_A_Q_ _._._.
     * _U_s_e_r_ _M_a_n_u_a_l
           o _L_i_f_t_O_n
     * _C_h_a_n_g_e_l_o_g
-          o _v_1_._0_._0
+          o _v_1_._0_._1
     * _L_i_c_e_n_s_e
     * _C_o_n_t_a_c_t
 
 ********** LLiiffttOOnn''ss lliimmiittaattiioonn_## **********
 LiftOn's cchhaaiinniinngg aallggoorriitthhmm currently only utilizes miniprot alignment results
 to fix the Liftoff annotation. However, it can be extended to chain together
 multiple DNA- and protein-based annotation files or aasembled RNA-Seq
```

### Comparing `lifton-1.0.0/lifton.egg-info/SOURCES.txt` & `lifton-1.0.1/lifton.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lifton-1.0.0/setup.py` & `lifton-1.0.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 from pathlib import Path
 
 this_directory = Path(__file__).resolve().parent
 long_description = (this_directory / "./README.md").read_text()
 setuptools.setup(
 	name="lifton",
-	version="1.0.0",
+	version="1.0.1",
 	author="Kuan-Hao Chao",
 	author_email="kh.chao@cs.jhu.edu",
 	description="Combining DNA and protein alignments to improve genome annotation with LiftOn",
 	url="https://github.com/Kuanhao-Chao/Lifton",
 	install_requires=['numpy>= 1.22.0', "biopython>=1.76", "cigar>=0.1.3", "parasail>=1.2.4", 'intervaltree>=3.1.0', 'interlap>=0.2.6', 'networkx>=2.4', 'pyfaidx>=0.5.8', 'pysam>=0.19.1', 'gffutils>=0.10.1', 'ujson>=3.2.0'],
 	python_requires='>=3.6',
 	packages=setuptools.find_packages(),
```

