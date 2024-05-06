# Comparing `tmp/rotary_emb-0.4.3.tar.gz` & `tmp/rotary_emb-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rotary_emb-0.4.3.tar", last modified: Mon May  6 08:04:40 2024, max compression
+gzip compressed data, was "rotary_emb-0.4.4.tar", last modified: Mon May  6 08:23:32 2024, max compression
```

## Comparing `rotary_emb-0.4.3.tar` & `rotary_emb-0.4.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:02:43.451446 rotary_emb-0.4.3/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       54 2024-05-06 08:04:40.298123 rotary_emb-0.4.3/PKG-INFO
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1612 2024-05-06 07:30:03.000000 rotary_emb-0.4.3/rotary.cpp
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1791 2024-05-06 07:30:03.000000 rotary_emb-0.4.3/rotary_cuda.cu
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:02:43.442659 rotary_emb-0.4.3/rotary_emb.egg-info/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       54 2024-05-06 08:04:39.000000 rotary_emb-0.4.3/rotary_emb.egg-info/PKG-INFO
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      170 2024-05-06 08:04:40.000000 rotary_emb-0.4.3/rotary_emb.egg-info/SOURCES.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        1 2024-05-06 08:04:39.000000 rotary_emb-0.4.3/rotary_emb.egg-info/dependency_links.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       11 2024-05-06 08:04:39.000000 rotary_emb-0.4.3/rotary_emb.egg-info/top_level.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       38 2024-05-06 08:04:40.302927 rotary_emb-0.4.3/setup.cfg
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5468 2024-05-06 08:04:10.000000 rotary_emb-0.4.3/setup.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:21:35.586478 rotary_emb-0.4.4/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       54 2024-05-06 08:23:32.434807 rotary_emb-0.4.4/PKG-INFO
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1612 2024-05-06 07:30:03.000000 rotary_emb-0.4.4/rotary.cpp
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1791 2024-05-06 07:30:03.000000 rotary_emb-0.4.4/rotary_cuda.cu
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:21:35.578018 rotary_emb-0.4.4/rotary_emb.egg-info/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       54 2024-05-06 08:23:31.000000 rotary_emb-0.4.4/rotary_emb.egg-info/PKG-INFO
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      170 2024-05-06 08:23:32.000000 rotary_emb-0.4.4/rotary_emb.egg-info/SOURCES.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        1 2024-05-06 08:23:31.000000 rotary_emb-0.4.4/rotary_emb.egg-info/dependency_links.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       11 2024-05-06 08:23:31.000000 rotary_emb-0.4.4/rotary_emb.egg-info/top_level.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       38 2024-05-06 08:23:32.438091 rotary_emb-0.4.4/setup.cfg
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5493 2024-05-06 08:17:40.000000 rotary_emb-0.4.4/setup.py
```

### Comparing `rotary_emb-0.4.3/rotary.cpp` & `rotary_emb-0.4.4/rotary.cpp`

 * *Files identical despite different names*

### Comparing `rotary_emb-0.4.3/rotary_cuda.cu` & `rotary_emb-0.4.4/rotary_cuda.cu`

 * *Files identical despite different names*

### Comparing `rotary_emb-0.4.3/setup.py` & `rotary_emb-0.4.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,19 +111,19 @@
                             'nvcc': append_nvcc_threads([
                                 '-O3', '--use_fast_math', '--expt-extended-lambda'
                             ] + cc_flag)
                            }
     )
 )
 
-pwd = os.path.dirname(__file__)
+pwd = os.path.dirname(os.path.abspath(__file__))
 
 def get_version():
     with open(os.path.join(pwd, 'version.txt'), 'r') as f:
-        content = f.read()
+        content = f.read().strip()
     return content
 
 proj_version = get_version()
 
 class CustomBdistWheel(bdist_wheel):
     def finalize_options(self):
         bdist_wheel.finalize_options(self)
```

