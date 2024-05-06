# Comparing `tmp/rotary_emb-0.4.2.tar.gz` & `tmp/rotary_emb-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rotary_emb-0.4.2.tar", last modified: Mon May  6 07:52:41 2024, max compression
+gzip compressed data, was "rotary_emb-0.4.3.tar", last modified: Mon May  6 08:04:40 2024, max compression
```

## Comparing `rotary_emb-0.4.2.tar` & `rotary_emb-0.4.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 07:50:44.166748 rotary_emb-0.4.2/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       54 2024-05-06 07:52:40.993484 rotary_emb-0.4.2/PKG-INFO
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1612 2024-05-06 07:30:03.000000 rotary_emb-0.4.2/rotary.cpp
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1791 2024-05-06 07:30:03.000000 rotary_emb-0.4.2/rotary_cuda.cu
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 07:50:44.158268 rotary_emb-0.4.2/rotary_emb.egg-info/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       54 2024-05-06 07:52:40.000000 rotary_emb-0.4.2/rotary_emb.egg-info/PKG-INFO
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      170 2024-05-06 07:52:40.000000 rotary_emb-0.4.2/rotary_emb.egg-info/SOURCES.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        1 2024-05-06 07:52:40.000000 rotary_emb-0.4.2/rotary_emb.egg-info/dependency_links.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       11 2024-05-06 07:52:40.000000 rotary_emb-0.4.2/rotary_emb.egg-info/top_level.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       38 2024-05-06 07:52:40.996855 rotary_emb-0.4.2/setup.cfg
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5474 2024-05-06 07:48:10.000000 rotary_emb-0.4.2/setup.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:02:43.451446 rotary_emb-0.4.3/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       54 2024-05-06 08:04:40.298123 rotary_emb-0.4.3/PKG-INFO
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1612 2024-05-06 07:30:03.000000 rotary_emb-0.4.3/rotary.cpp
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1791 2024-05-06 07:30:03.000000 rotary_emb-0.4.3/rotary_cuda.cu
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:02:43.442659 rotary_emb-0.4.3/rotary_emb.egg-info/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       54 2024-05-06 08:04:39.000000 rotary_emb-0.4.3/rotary_emb.egg-info/PKG-INFO
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      170 2024-05-06 08:04:40.000000 rotary_emb-0.4.3/rotary_emb.egg-info/SOURCES.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        1 2024-05-06 08:04:39.000000 rotary_emb-0.4.3/rotary_emb.egg-info/dependency_links.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       11 2024-05-06 08:04:39.000000 rotary_emb-0.4.3/rotary_emb.egg-info/top_level.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       38 2024-05-06 08:04:40.302927 rotary_emb-0.4.3/setup.cfg
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5468 2024-05-06 08:04:10.000000 rotary_emb-0.4.3/setup.py
```

### Comparing `rotary_emb-0.4.2/rotary.cpp` & `rotary_emb-0.4.3/rotary.cpp`

 * *Files identical despite different names*

### Comparing `rotary_emb-0.4.2/rotary_cuda.cu` & `rotary_emb-0.4.3/rotary_cuda.cu`

 * *Files identical despite different names*

### Comparing `rotary_emb-0.4.2/setup.py` & `rotary_emb-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
                            }
     )
 )
 
 pwd = os.path.dirname(__file__)
 
 def get_version():
-    with open(os.path.join(pwd, '../../version.txt'), 'r') as f:
+    with open(os.path.join(pwd, 'version.txt'), 'r') as f:
         content = f.read()
     return content
 
 proj_version = get_version()
 
 class CustomBdistWheel(bdist_wheel):
     def finalize_options(self):
```

