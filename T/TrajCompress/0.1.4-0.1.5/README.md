# Comparing `tmp/trajcompress-0.1.4.tar.gz` & `tmp/trajcompress-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trajcompress-0.1.4.tar", last modified: Mon May  6 15:33:21 2024, max compression
+gzip compressed data, was "trajcompress-0.1.5.tar", last modified: Mon May  6 15:39:43 2024, max compression
```

## Comparing `trajcompress-0.1.4.tar` & `trajcompress-0.1.5.tar`

### file list

```diff
@@ -1,27 +1,42 @@
-drwxrwxr-x   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:33:21.965791 trajcompress-0.1.4/
--rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     1051 2024-05-06 09:10:18.000000 trajcompress-0.1.4/LICENSE
--rw-r--r--   0 chenghao  (1033) chenghao  (1034)      224 2024-05-06 15:33:21.965791 trajcompress-0.1.4/PKG-INFO
-drwxrwxr-x   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:33:21.905792 trajcompress-0.1.4/TrajCompress/
--rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     1348 2024-05-06 04:51:54.000000 trajcompress-0.1.4/TrajCompress/__init__.py
-drwxrwxr-x   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:33:21.925792 trajcompress-0.1.4/TrajCompress/src/
--rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     8669 2024-05-06 05:10:32.000000 trajcompress-0.1.4/TrajCompress/src/List_Points_2_List_Points.py
--rw-rw-r--   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:30:46.000000 trajcompress-0.1.4/TrajCompress/src/__init__.py
-drwxrwxr-x   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:33:21.949791 trajcompress-0.1.4/TrajCompress/src/basic_notion/
--rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     5324 2024-05-06 04:52:23.000000 trajcompress-0.1.4/TrajCompress/src/basic_notion/DistFunc.py
--rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     2560 2024-05-06 04:53:38.000000 trajcompress-0.1.4/TrajCompress/src/basic_notion/LineSimplify.py
--rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     1455 2024-05-06 03:47:23.000000 trajcompress-0.1.4/TrajCompress/src/basic_notion/Point.py
--rw-rw-r--   0 chenghao  (1033) chenghao  (1034)       71 2024-05-06 03:47:22.000000 trajcompress-0.1.4/TrajCompress/src/basic_notion/__init__.py
-drwxrwxr-x   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:33:21.965791 trajcompress-0.1.4/TrajCompress/utils/
--rw-rw-r--   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:31:05.000000 trajcompress-0.1.4/TrajCompress/utils/__init__.py
--rw-rw-r--   0 chenghao  (1033) chenghao  (1034)      635 2024-05-06 07:00:24.000000 trajcompress-0.1.4/TrajCompress/utils/get_sample.py
--rw-rw-r--   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 04:11:45.000000 trajcompress-0.1.4/TrajCompress/utils/read_data.py
-drwxrwxr-x   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:33:21.965791 trajcompress-0.1.4/TrajCompress.egg-info/
--rw-r--r--   0 chenghao  (1033) chenghao  (1034)      224 2024-05-06 15:33:21.000000 trajcompress-0.1.4/TrajCompress.egg-info/PKG-INFO
--rw-rw-r--   0 chenghao  (1033) chenghao  (1034)      581 2024-05-06 15:33:21.000000 trajcompress-0.1.4/TrajCompress.egg-info/SOURCES.txt
--rw-rw-r--   0 chenghao  (1033) chenghao  (1034)        1 2024-05-06 15:33:21.000000 trajcompress-0.1.4/TrajCompress.egg-info/dependency_links.txt
--rw-rw-r--   0 chenghao  (1033) chenghao  (1034)       12 2024-05-06 15:33:21.000000 trajcompress-0.1.4/TrajCompress.egg-info/requires.txt
--rw-rw-r--   0 chenghao  (1033) chenghao  (1034)       13 2024-05-06 15:33:21.000000 trajcompress-0.1.4/TrajCompress.egg-info/top_level.txt
--rw-rw-r--   0 chenghao  (1033) chenghao  (1034)       38 2024-05-06 15:33:21.965791 trajcompress-0.1.4/setup.cfg
--rw-rw-r--   0 chenghao  (1033) chenghao  (1034)      479 2024-05-06 15:33:11.000000 trajcompress-0.1.4/setup.py
-drwxrwxr-x   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:33:21.965791 trajcompress-0.1.4/tests/
--rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     3692 2024-05-06 08:27:26.000000 trajcompress-0.1.4/tests/test_sample.py
+drwxrwxr-x   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:39:43.038551 trajcompress-0.1.5/
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     1051 2024-05-06 09:10:18.000000 trajcompress-0.1.5/LICENSE
+-rw-r--r--   0 chenghao  (1033) chenghao  (1034)      224 2024-05-06 15:39:43.038551 trajcompress-0.1.5/PKG-INFO
+drwxrwxr-x   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:39:42.930552 trajcompress-0.1.5/TrajCompress/
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     1348 2024-05-06 04:51:54.000000 trajcompress-0.1.5/TrajCompress/__init__.py
+drwxrwxr-x   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:39:42.930552 trajcompress-0.1.5/TrajCompress/src/
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     8669 2024-05-06 05:10:32.000000 trajcompress-0.1.5/TrajCompress/src/List_Points_2_List_Points.py
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:30:46.000000 trajcompress-0.1.5/TrajCompress/src/__init__.py
+drwxrwxr-x   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:39:43.018551 trajcompress-0.1.5/TrajCompress/src/algorithms/
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     3464 2024-05-06 05:03:48.000000 trajcompress-0.1.5/TrajCompress/src/algorithms/Angular_batch.py
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)    16689 2024-05-06 05:14:35.000000 trajcompress-0.1.5/TrajCompress/src/algorithms/DOTS_batch.py
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     5545 2024-05-06 03:54:21.000000 trajcompress-0.1.5/TrajCompress/src/algorithms/DP_batch.py
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     1546 2024-05-06 03:53:34.000000 trajcompress-0.1.5/TrajCompress/src/algorithms/Dead_Reckoning_batch.py
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)    10884 2024-05-06 03:54:21.000000 trajcompress-0.1.5/TrajCompress/src/algorithms/OPERB_batch.py
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     8654 2024-05-06 05:15:17.000000 trajcompress-0.1.5/TrajCompress/src/algorithms/OpeningWindow_batch.py
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)    10960 2024-05-06 05:16:49.000000 trajcompress-0.1.5/TrajCompress/src/algorithms/SQUISH_E_batch.py
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     5635 2024-05-06 05:15:34.000000 trajcompress-0.1.5/TrajCompress/src/algorithms/STTrace_batch.py
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     4212 2024-05-06 03:53:35.000000 trajcompress-0.1.5/TrajCompress/src/algorithms/TD_TR_batch.py
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     2592 2024-05-06 05:09:16.000000 trajcompress-0.1.5/TrajCompress/src/algorithms/Uniform_batch.py
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:39:03.000000 trajcompress-0.1.5/TrajCompress/src/algorithms/__init__.py
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     4376 2024-05-06 05:11:14.000000 trajcompress-0.1.5/TrajCompress/src/algorithms/bottom_up_batch.py
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     5546 2024-05-06 05:14:44.000000 trajcompress-0.1.5/TrajCompress/src/algorithms/interval_batch.py
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     4691 2024-05-06 05:17:34.000000 trajcompress-0.1.5/TrajCompress/src/algorithms/threshold_batch.py
+drwxrwxr-x   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:39:43.038551 trajcompress-0.1.5/TrajCompress/src/basic_notion/
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     5324 2024-05-06 04:52:23.000000 trajcompress-0.1.5/TrajCompress/src/basic_notion/DistFunc.py
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     2560 2024-05-06 04:53:38.000000 trajcompress-0.1.5/TrajCompress/src/basic_notion/LineSimplify.py
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     1455 2024-05-06 03:47:23.000000 trajcompress-0.1.5/TrajCompress/src/basic_notion/Point.py
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)       71 2024-05-06 03:47:22.000000 trajcompress-0.1.5/TrajCompress/src/basic_notion/__init__.py
+drwxrwxr-x   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:39:43.038551 trajcompress-0.1.5/TrajCompress/utils/
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:31:05.000000 trajcompress-0.1.5/TrajCompress/utils/__init__.py
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)      635 2024-05-06 07:00:24.000000 trajcompress-0.1.5/TrajCompress/utils/get_sample.py
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 04:11:45.000000 trajcompress-0.1.5/TrajCompress/utils/read_data.py
+drwxrwxr-x   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:39:43.038551 trajcompress-0.1.5/TrajCompress.egg-info/
+-rw-r--r--   0 chenghao  (1033) chenghao  (1034)      224 2024-05-06 15:39:42.000000 trajcompress-0.1.5/TrajCompress.egg-info/PKG-INFO
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     1213 2024-05-06 15:39:42.000000 trajcompress-0.1.5/TrajCompress.egg-info/SOURCES.txt
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)        1 2024-05-06 15:39:42.000000 trajcompress-0.1.5/TrajCompress.egg-info/dependency_links.txt
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)       12 2024-05-06 15:39:42.000000 trajcompress-0.1.5/TrajCompress.egg-info/requires.txt
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)       13 2024-05-06 15:39:42.000000 trajcompress-0.1.5/TrajCompress.egg-info/top_level.txt
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)       38 2024-05-06 15:39:43.038551 trajcompress-0.1.5/setup.cfg
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)      479 2024-05-06 15:39:35.000000 trajcompress-0.1.5/setup.py
+drwxrwxr-x   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:39:43.038551 trajcompress-0.1.5/tests/
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     3692 2024-05-06 08:27:26.000000 trajcompress-0.1.5/tests/test_sample.py
```

### Comparing `trajcompress-0.1.4/LICENSE` & `trajcompress-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `trajcompress-0.1.4/TrajCompress/__init__.py` & `trajcompress-0.1.5/TrajCompress/__init__.py`

 * *Files identical despite different names*

### Comparing `trajcompress-0.1.4/TrajCompress/src/List_Points_2_List_Points.py` & `trajcompress-0.1.5/TrajCompress/src/List_Points_2_List_Points.py`

 * *Files identical despite different names*

### Comparing `trajcompress-0.1.4/TrajCompress/src/basic_notion/DistFunc.py` & `trajcompress-0.1.5/TrajCompress/src/basic_notion/DistFunc.py`

 * *Files identical despite different names*

### Comparing `trajcompress-0.1.4/TrajCompress/src/basic_notion/LineSimplify.py` & `trajcompress-0.1.5/TrajCompress/src/basic_notion/LineSimplify.py`

 * *Files identical despite different names*

### Comparing `trajcompress-0.1.4/TrajCompress/src/basic_notion/Point.py` & `trajcompress-0.1.5/TrajCompress/src/basic_notion/Point.py`

 * *Files identical despite different names*

### Comparing `trajcompress-0.1.4/TrajCompress/utils/get_sample.py` & `trajcompress-0.1.5/TrajCompress/utils/get_sample.py`

 * *Files identical despite different names*

### Comparing `trajcompress-0.1.4/tests/test_sample.py` & `trajcompress-0.1.5/tests/test_sample.py`

 * *Files identical despite different names*

