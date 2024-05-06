# Comparing `tmp/trajcompress-0.1.3.tar.gz` & `tmp/trajcompress-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trajcompress-0.1.3.tar", last modified: Mon May  6 15:23:34 2024, max compression
+gzip compressed data, was "trajcompress-0.1.4.tar", last modified: Mon May  6 15:33:21 2024, max compression
```

## Comparing `trajcompress-0.1.3.tar` & `trajcompress-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,27 @@
-drwxrwxr-x   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:23:34.855091 trajcompress-0.1.3/
--rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     1051 2024-05-06 09:10:18.000000 trajcompress-0.1.3/LICENSE
--rw-r--r--   0 chenghao  (1033) chenghao  (1034)      224 2024-05-06 15:23:34.855091 trajcompress-0.1.3/PKG-INFO
-drwxrwxr-x   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:23:34.851091 trajcompress-0.1.3/TrajCompress/
--rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     1348 2024-05-06 04:51:54.000000 trajcompress-0.1.3/TrajCompress/__init__.py
-drwxrwxr-x   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:23:34.851091 trajcompress-0.1.3/TrajCompress.egg-info/
--rw-r--r--   0 chenghao  (1033) chenghao  (1034)      224 2024-05-06 15:23:34.000000 trajcompress-0.1.3/TrajCompress.egg-info/PKG-INFO
--rw-rw-r--   0 chenghao  (1033) chenghao  (1034)      241 2024-05-06 15:23:34.000000 trajcompress-0.1.3/TrajCompress.egg-info/SOURCES.txt
--rw-rw-r--   0 chenghao  (1033) chenghao  (1034)        1 2024-05-06 15:23:34.000000 trajcompress-0.1.3/TrajCompress.egg-info/dependency_links.txt
--rw-rw-r--   0 chenghao  (1033) chenghao  (1034)       12 2024-05-06 15:23:34.000000 trajcompress-0.1.3/TrajCompress.egg-info/requires.txt
--rw-rw-r--   0 chenghao  (1033) chenghao  (1034)        1 2024-05-06 15:23:34.000000 trajcompress-0.1.3/TrajCompress.egg-info/top_level.txt
--rw-rw-r--   0 chenghao  (1033) chenghao  (1034)       38 2024-05-06 15:23:34.855091 trajcompress-0.1.3/setup.cfg
--rw-rw-r--   0 chenghao  (1033) chenghao  (1034)      447 2024-05-06 15:23:28.000000 trajcompress-0.1.3/setup.py
-drwxrwxr-x   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:23:34.851091 trajcompress-0.1.3/tests/
--rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     3692 2024-05-06 08:27:26.000000 trajcompress-0.1.3/tests/test_sample.py
+drwxrwxr-x   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:33:21.965791 trajcompress-0.1.4/
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     1051 2024-05-06 09:10:18.000000 trajcompress-0.1.4/LICENSE
+-rw-r--r--   0 chenghao  (1033) chenghao  (1034)      224 2024-05-06 15:33:21.965791 trajcompress-0.1.4/PKG-INFO
+drwxrwxr-x   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:33:21.905792 trajcompress-0.1.4/TrajCompress/
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     1348 2024-05-06 04:51:54.000000 trajcompress-0.1.4/TrajCompress/__init__.py
+drwxrwxr-x   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:33:21.925792 trajcompress-0.1.4/TrajCompress/src/
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     8669 2024-05-06 05:10:32.000000 trajcompress-0.1.4/TrajCompress/src/List_Points_2_List_Points.py
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:30:46.000000 trajcompress-0.1.4/TrajCompress/src/__init__.py
+drwxrwxr-x   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:33:21.949791 trajcompress-0.1.4/TrajCompress/src/basic_notion/
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     5324 2024-05-06 04:52:23.000000 trajcompress-0.1.4/TrajCompress/src/basic_notion/DistFunc.py
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     2560 2024-05-06 04:53:38.000000 trajcompress-0.1.4/TrajCompress/src/basic_notion/LineSimplify.py
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     1455 2024-05-06 03:47:23.000000 trajcompress-0.1.4/TrajCompress/src/basic_notion/Point.py
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)       71 2024-05-06 03:47:22.000000 trajcompress-0.1.4/TrajCompress/src/basic_notion/__init__.py
+drwxrwxr-x   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:33:21.965791 trajcompress-0.1.4/TrajCompress/utils/
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:31:05.000000 trajcompress-0.1.4/TrajCompress/utils/__init__.py
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)      635 2024-05-06 07:00:24.000000 trajcompress-0.1.4/TrajCompress/utils/get_sample.py
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 04:11:45.000000 trajcompress-0.1.4/TrajCompress/utils/read_data.py
+drwxrwxr-x   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:33:21.965791 trajcompress-0.1.4/TrajCompress.egg-info/
+-rw-r--r--   0 chenghao  (1033) chenghao  (1034)      224 2024-05-06 15:33:21.000000 trajcompress-0.1.4/TrajCompress.egg-info/PKG-INFO
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)      581 2024-05-06 15:33:21.000000 trajcompress-0.1.4/TrajCompress.egg-info/SOURCES.txt
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)        1 2024-05-06 15:33:21.000000 trajcompress-0.1.4/TrajCompress.egg-info/dependency_links.txt
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)       12 2024-05-06 15:33:21.000000 trajcompress-0.1.4/TrajCompress.egg-info/requires.txt
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)       13 2024-05-06 15:33:21.000000 trajcompress-0.1.4/TrajCompress.egg-info/top_level.txt
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)       38 2024-05-06 15:33:21.965791 trajcompress-0.1.4/setup.cfg
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)      479 2024-05-06 15:33:11.000000 trajcompress-0.1.4/setup.py
+drwxrwxr-x   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:33:21.965791 trajcompress-0.1.4/tests/
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     3692 2024-05-06 08:27:26.000000 trajcompress-0.1.4/tests/test_sample.py
```

### Comparing `trajcompress-0.1.3/LICENSE` & `trajcompress-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `trajcompress-0.1.3/TrajCompress/__init__.py` & `trajcompress-0.1.4/TrajCompress/__init__.py`

 * *Files identical despite different names*

### Comparing `trajcompress-0.1.3/tests/test_sample.py` & `trajcompress-0.1.4/tests/test_sample.py`

 * *Files identical despite different names*

