# Comparing `tmp/neolibrary-0.4.2b1.tar.gz` & `tmp/neolibrary-0.4.3b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neolibrary-0.4.2b1.tar", max compression
+gzip compressed data, was "neolibrary-0.4.3b1.tar", max compression
```

## Comparing `neolibrary-0.4.2b1.tar` & `neolibrary-0.4.3b1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2024-02-27 15:43:19.055512 neolibrary-0.4.2b1/LICENSE
--rw-r--r--   0        0        0     3284 2024-02-27 15:43:19.055512 neolibrary-0.4.2b1/README.md
--rw-r--r--   0        0        0     1889 2024-02-27 15:43:19.059512 neolibrary-0.4.2b1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-27 15:43:19.059512 neolibrary-0.4.2b1/src/neolibrary/__init__.py
--rw-r--r--   0        0        0      696 2024-02-27 15:43:19.059512 neolibrary-0.4.2b1/src/neolibrary/decorators.py
--rw-r--r--   0        0        0        0 2024-02-27 15:43:19.059512 neolibrary-0.4.2b1/src/neolibrary/monitoring/__init__.py
--rw-r--r--   0        0        0      770 2024-02-27 15:43:19.059512 neolibrary-0.4.2b1/src/neolibrary/monitoring/config/config.py
--rw-r--r--   0        0        0     8365 2024-02-27 15:43:19.059512 neolibrary-0.4.2b1/src/neolibrary/monitoring/logger.py
--rw-r--r--   0        0        0      144 2024-02-27 15:43:19.059512 neolibrary-0.4.2b1/src/neolibrary/preproc.py
--rw-r--r--   0        0        0    26817 2024-02-27 15:43:19.059512 neolibrary-0.4.2b1/src/neolibrary/thumbnail_creator.py
--rw-r--r--   0        0        0     8628 2024-02-27 15:43:19.059512 neolibrary-0.4.2b1/src/neolibrary/utils.py
--rw-r--r--   0        0        0     4151 1970-01-01 00:00:00.000000 neolibrary-0.4.2b1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-06 12:58:22.221624 neolibrary-0.4.3b1/LICENSE
+-rw-r--r--   0        0        0     3284 2024-05-06 12:58:22.221624 neolibrary-0.4.3b1/README.md
+-rw-r--r--   0        0        0     1889 2024-05-06 12:58:22.225625 neolibrary-0.4.3b1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-06 12:58:22.225625 neolibrary-0.4.3b1/src/neolibrary/__init__.py
+-rw-r--r--   0        0        0      696 2024-05-06 12:58:22.225625 neolibrary-0.4.3b1/src/neolibrary/decorators.py
+-rw-r--r--   0        0        0        0 2024-05-06 12:58:22.225625 neolibrary-0.4.3b1/src/neolibrary/monitoring/__init__.py
+-rw-r--r--   0        0        0      770 2024-05-06 12:58:22.225625 neolibrary-0.4.3b1/src/neolibrary/monitoring/config/config.py
+-rw-r--r--   0        0        0     8365 2024-05-06 12:58:22.225625 neolibrary-0.4.3b1/src/neolibrary/monitoring/logger.py
+-rw-r--r--   0        0        0      144 2024-05-06 12:58:22.225625 neolibrary-0.4.3b1/src/neolibrary/preproc.py
+-rw-r--r--   0        0        0    26817 2024-05-06 12:58:22.225625 neolibrary-0.4.3b1/src/neolibrary/thumbnail_creator.py
+-rw-r--r--   0        0        0     8628 2024-05-06 12:58:22.225625 neolibrary-0.4.3b1/src/neolibrary/utils.py
+-rw-r--r--   0        0        0     4151 1970-01-01 00:00:00.000000 neolibrary-0.4.3b1/PKG-INFO
```

### Comparing `neolibrary-0.4.2b1/LICENSE` & `neolibrary-0.4.3b1/LICENSE`

 * *Files identical despite different names*

### Comparing `neolibrary-0.4.2b1/README.md` & `neolibrary-0.4.3b1/README.md`

 * *Files identical despite different names*

### Comparing `neolibrary-0.4.2b1/pyproject.toml` & `neolibrary-0.4.3b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = 'neolibrary'
-version = "v0.4.2b1"
+version = "v0.4.3b1"
 description = 'The general utils library for neomedsys development'
 authors = ['Martin Soria Røvang <martinrovang@gmail.com>']
 license = 'Apache-2.0 license'
 readme = 'README.md'
 
 [tool.poetry.dependencies]
 python = '^3.9'
 colorlog = '^6.7.0'
 blosc = '^1.11.1'
 numpy = '^1.25.2'
 arrow = "^1.2.3"
 nibabel = "^5.1.0"
-simpleitk = "^2.3.1"
+simpleitk = "^2.0.0"
 scikit-image = "^0.22.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = '^7.4.0'
 nox = '^2023.4.22'
 coverage = "^7.2.7"
```

### Comparing `neolibrary-0.4.2b1/src/neolibrary/decorators.py` & `neolibrary-0.4.3b1/src/neolibrary/decorators.py`

 * *Files identical despite different names*

### Comparing `neolibrary-0.4.2b1/src/neolibrary/monitoring/config/config.py` & `neolibrary-0.4.3b1/src/neolibrary/monitoring/config/config.py`

 * *Files identical despite different names*

### Comparing `neolibrary-0.4.2b1/src/neolibrary/monitoring/logger.py` & `neolibrary-0.4.3b1/src/neolibrary/monitoring/logger.py`

 * *Files identical despite different names*

### Comparing `neolibrary-0.4.2b1/src/neolibrary/thumbnail_creator.py` & `neolibrary-0.4.3b1/src/neolibrary/thumbnail_creator.py`

 * *Files identical despite different names*

### Comparing `neolibrary-0.4.2b1/src/neolibrary/utils.py` & `neolibrary-0.4.3b1/src/neolibrary/utils.py`

 * *Files identical despite different names*

### Comparing `neolibrary-0.4.2b1/PKG-INFO` & `neolibrary-0.4.3b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neolibrary
-Version: 0.4.2b1
+Version: 0.4.3b1
 Summary: The general utils library for neomedsys development
 License: Apache-2.0 license
 Author: Martin Soria Røvang
 Author-email: martinrovang@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: arrow (>=1.2.3,<2.0.0)
 Requires-Dist: blosc (>=1.11.1,<2.0.0)
 Requires-Dist: colorlog (>=6.7.0,<7.0.0)
 Requires-Dist: nibabel (>=5.1.0,<6.0.0)
 Requires-Dist: numpy (>=1.25.2,<2.0.0)
 Requires-Dist: scikit-image (>=0.22.0,<0.23.0)
-Requires-Dist: simpleitk (>=2.3.1,<3.0.0)
+Requires-Dist: simpleitk (>=2.0.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 
 
 <img align="right" width="200" alt="20200907_104224" src="./images/neolibcone.png">
 
 # NeoLibrary 🍦
```

