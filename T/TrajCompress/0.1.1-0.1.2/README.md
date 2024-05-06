# Comparing `tmp/trajcompress-0.1.1.tar.gz` & `tmp/trajcompress-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trajcompress-0.1.1.tar", last modified: Mon May  6 15:08:46 2024, max compression
+gzip compressed data, was "trajcompress-0.1.2.tar", last modified: Mon May  6 15:18:51 2024, max compression
```

## Comparing `trajcompress-0.1.1.tar` & `trajcompress-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:08:46.883073 trajcompress-0.1.1/
--rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     1051 2024-05-06 09:10:18.000000 trajcompress-0.1.1/LICENSE
--rw-r--r--   0 chenghao  (1033) chenghao  (1034)      224 2024-05-06 15:08:46.883073 trajcompress-0.1.1/PKG-INFO
-drwxrwxr-x   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:08:46.859073 trajcompress-0.1.1/TrajCompress/
--rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     1348 2024-05-06 04:51:54.000000 trajcompress-0.1.1/TrajCompress/__init__.py
-drwxrwxr-x   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:08:46.883073 trajcompress-0.1.1/TrajCompress.egg-info/
--rw-r--r--   0 chenghao  (1033) chenghao  (1034)      224 2024-05-06 15:08:46.000000 trajcompress-0.1.1/TrajCompress.egg-info/PKG-INFO
--rw-rw-r--   0 chenghao  (1033) chenghao  (1034)      241 2024-05-06 15:08:46.000000 trajcompress-0.1.1/TrajCompress.egg-info/SOURCES.txt
--rw-rw-r--   0 chenghao  (1033) chenghao  (1034)        1 2024-05-06 15:08:46.000000 trajcompress-0.1.1/TrajCompress.egg-info/dependency_links.txt
--rw-rw-r--   0 chenghao  (1033) chenghao  (1034)       12 2024-05-06 15:08:46.000000 trajcompress-0.1.1/TrajCompress.egg-info/requires.txt
--rw-rw-r--   0 chenghao  (1033) chenghao  (1034)       13 2024-05-06 15:08:46.000000 trajcompress-0.1.1/TrajCompress.egg-info/top_level.txt
--rw-rw-r--   0 chenghao  (1033) chenghao  (1034)       38 2024-05-06 15:08:46.883073 trajcompress-0.1.1/setup.cfg
--rw-rw-r--   0 chenghao  (1033) chenghao  (1034)      433 2024-05-06 15:08:16.000000 trajcompress-0.1.1/setup.py
-drwxrwxr-x   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:08:46.871073 trajcompress-0.1.1/tests/
--rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     3692 2024-05-06 08:27:26.000000 trajcompress-0.1.1/tests/test_sample.py
+drwxrwxr-x   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:18:51.157646 trajcompress-0.1.2/
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     1051 2024-05-06 09:10:18.000000 trajcompress-0.1.2/LICENSE
+-rw-r--r--   0 chenghao  (1033) chenghao  (1034)      224 2024-05-06 15:18:51.157646 trajcompress-0.1.2/PKG-INFO
+drwxrwxr-x   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:18:51.153646 trajcompress-0.1.2/TrajCompress/
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     1348 2024-05-06 04:51:54.000000 trajcompress-0.1.2/TrajCompress/__init__.py
+drwxrwxr-x   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:18:51.157646 trajcompress-0.1.2/TrajCompress.egg-info/
+-rw-r--r--   0 chenghao  (1033) chenghao  (1034)      224 2024-05-06 15:18:51.000000 trajcompress-0.1.2/TrajCompress.egg-info/PKG-INFO
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)      241 2024-05-06 15:18:51.000000 trajcompress-0.1.2/TrajCompress.egg-info/SOURCES.txt
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)        1 2024-05-06 15:18:51.000000 trajcompress-0.1.2/TrajCompress.egg-info/dependency_links.txt
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)       12 2024-05-06 15:18:51.000000 trajcompress-0.1.2/TrajCompress.egg-info/requires.txt
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)       13 2024-05-06 15:18:51.000000 trajcompress-0.1.2/TrajCompress.egg-info/top_level.txt
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)       38 2024-05-06 15:18:51.157646 trajcompress-0.1.2/setup.cfg
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)      433 2024-05-06 15:18:32.000000 trajcompress-0.1.2/setup.py
+drwxrwxr-x   0 chenghao  (1033) chenghao  (1034)        0 2024-05-06 15:18:51.157646 trajcompress-0.1.2/tests/
+-rw-rw-r--   0 chenghao  (1033) chenghao  (1034)     3692 2024-05-06 08:27:26.000000 trajcompress-0.1.2/tests/test_sample.py
```

### Comparing `trajcompress-0.1.1/LICENSE` & `trajcompress-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trajcompress-0.1.1/TrajCompress/__init__.py` & `trajcompress-0.1.2/TrajCompress/__init__.py`

 * *Files identical despite different names*

### Comparing `trajcompress-0.1.1/tests/test_sample.py` & `trajcompress-0.1.2/tests/test_sample.py`

 * *Files identical despite different names*

