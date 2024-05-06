# Comparing `tmp/rotary_emb-0.4.4.tar.gz` & `tmp/rotary_emb-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rotary_emb-0.4.4.tar", last modified: Mon May  6 08:23:32 2024, max compression
+gzip compressed data, was "rotary_emb-0.4.5.tar", last modified: Mon May  6 08:47:39 2024, max compression
```

## Comparing `rotary_emb-0.4.4.tar` & `rotary_emb-0.4.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:21:35.586478 rotary_emb-0.4.4/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       54 2024-05-06 08:23:32.434807 rotary_emb-0.4.4/PKG-INFO
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1612 2024-05-06 07:30:03.000000 rotary_emb-0.4.4/rotary.cpp
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1791 2024-05-06 07:30:03.000000 rotary_emb-0.4.4/rotary_cuda.cu
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:21:35.578018 rotary_emb-0.4.4/rotary_emb.egg-info/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       54 2024-05-06 08:23:31.000000 rotary_emb-0.4.4/rotary_emb.egg-info/PKG-INFO
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      170 2024-05-06 08:23:32.000000 rotary_emb-0.4.4/rotary_emb.egg-info/SOURCES.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        1 2024-05-06 08:23:31.000000 rotary_emb-0.4.4/rotary_emb.egg-info/dependency_links.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       11 2024-05-06 08:23:31.000000 rotary_emb-0.4.4/rotary_emb.egg-info/top_level.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       38 2024-05-06 08:23:32.438091 rotary_emb-0.4.4/setup.cfg
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5493 2024-05-06 08:17:40.000000 rotary_emb-0.4.4/setup.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:45:42.974689 rotary_emb-0.4.5/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       54 2024-05-06 08:47:39.826362 rotary_emb-0.4.5/PKG-INFO
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1612 2024-05-06 07:30:03.000000 rotary_emb-0.4.5/rotary.cpp
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1791 2024-05-06 07:30:03.000000 rotary_emb-0.4.5/rotary_cuda.cu
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:45:42.966019 rotary_emb-0.4.5/rotary_emb.egg-info/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       54 2024-05-06 08:47:39.000000 rotary_emb-0.4.5/rotary_emb.egg-info/PKG-INFO
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      170 2024-05-06 08:47:39.000000 rotary_emb-0.4.5/rotary_emb.egg-info/SOURCES.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        1 2024-05-06 08:47:39.000000 rotary_emb-0.4.5/rotary_emb.egg-info/dependency_links.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       11 2024-05-06 08:47:39.000000 rotary_emb-0.4.5/rotary_emb.egg-info/top_level.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       38 2024-05-06 08:47:39.829829 rotary_emb-0.4.5/setup.cfg
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5579 2024-05-06 08:47:12.000000 rotary_emb-0.4.5/setup.py
```

### Comparing `rotary_emb-0.4.4/rotary.cpp` & `rotary_emb-0.4.5/rotary.cpp`

 * *Files identical despite different names*

### Comparing `rotary_emb-0.4.4/rotary_cuda.cu` & `rotary_emb-0.4.5/rotary_cuda.cu`

 * *Files identical despite different names*

### Comparing `rotary_emb-0.4.4/setup.py` & `rotary_emb-0.4.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -120,21 +120,26 @@
 def get_version():
     with open(os.path.join(pwd, 'version.txt'), 'r') as f:
         content = f.read().strip()
     return content
 
 proj_version = get_version()
 
+package_data = {
+    'rotary_emb': ['version.txt'],
+}
+
 class CustomBdistWheel(bdist_wheel):
     def finalize_options(self):
         bdist_wheel.finalize_options(self)
         self.plat_name = 'any'
 
 setup(
     name="rotary_emb",
     version=proj_version,
+    package_data=package_data,
     ext_modules=ext_modules,
     cmdclass={
         "build_ext": BuildExtension,
         "bdist_wheel": CustomBdistWheel
     },
 )
```

