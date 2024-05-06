# Comparing `tmp/rotary_emb-0.4.0.dev20240403.tar.gz` & `tmp/rotary_emb-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rotary_emb-0.4.0.dev20240403.tar", last modified: Mon May  6 07:48:36 2024, max compression
+gzip compressed data, was "rotary_emb-0.4.2.tar", last modified: Mon May  6 07:52:41 2024, max compression
```

## Comparing `rotary_emb-0.4.0.dev20240403.tar` & `rotary_emb-0.4.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 07:46:39.272165 rotary_emb-0.4.0.dev20240403/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       66 2024-05-06 07:48:36.098324 rotary_emb-0.4.0.dev20240403/PKG-INFO
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1612 2024-05-06 07:30:03.000000 rotary_emb-0.4.0.dev20240403/rotary.cpp
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1791 2024-05-06 07:30:03.000000 rotary_emb-0.4.0.dev20240403/rotary_cuda.cu
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 07:46:39.263200 rotary_emb-0.4.0.dev20240403/rotary_emb.egg-info/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       66 2024-05-06 07:48:35.000000 rotary_emb-0.4.0.dev20240403/rotary_emb.egg-info/PKG-INFO
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      170 2024-05-06 07:48:35.000000 rotary_emb-0.4.0.dev20240403/rotary_emb.egg-info/SOURCES.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        1 2024-05-06 07:48:35.000000 rotary_emb-0.4.0.dev20240403/rotary_emb.egg-info/dependency_links.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       11 2024-05-06 07:48:35.000000 rotary_emb-0.4.0.dev20240403/rotary_emb.egg-info/top_level.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       38 2024-05-06 07:48:36.101715 rotary_emb-0.4.0.dev20240403/setup.cfg
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5474 2024-05-06 07:48:10.000000 rotary_emb-0.4.0.dev20240403/setup.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 07:50:44.166748 rotary_emb-0.4.2/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       54 2024-05-06 07:52:40.993484 rotary_emb-0.4.2/PKG-INFO
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1612 2024-05-06 07:30:03.000000 rotary_emb-0.4.2/rotary.cpp
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1791 2024-05-06 07:30:03.000000 rotary_emb-0.4.2/rotary_cuda.cu
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 07:50:44.158268 rotary_emb-0.4.2/rotary_emb.egg-info/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       54 2024-05-06 07:52:40.000000 rotary_emb-0.4.2/rotary_emb.egg-info/PKG-INFO
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      170 2024-05-06 07:52:40.000000 rotary_emb-0.4.2/rotary_emb.egg-info/SOURCES.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        1 2024-05-06 07:52:40.000000 rotary_emb-0.4.2/rotary_emb.egg-info/dependency_links.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       11 2024-05-06 07:52:40.000000 rotary_emb-0.4.2/rotary_emb.egg-info/top_level.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       38 2024-05-06 07:52:40.996855 rotary_emb-0.4.2/setup.cfg
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5474 2024-05-06 07:48:10.000000 rotary_emb-0.4.2/setup.py
```

### Comparing `rotary_emb-0.4.0.dev20240403/rotary.cpp` & `rotary_emb-0.4.2/rotary.cpp`

 * *Files identical despite different names*

### Comparing `rotary_emb-0.4.0.dev20240403/rotary_cuda.cu` & `rotary_emb-0.4.2/rotary_cuda.cu`

 * *Files identical despite different names*

### Comparing `rotary_emb-0.4.0.dev20240403/setup.py` & `rotary_emb-0.4.2/setup.py`

 * *Files identical despite different names*

