# Comparing `tmp/test_nvf_builds-0.0.1.tar.gz` & `tmp/test_nvf_builds-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_nvf_builds-0.0.1.tar", last modified: Mon May  6 08:17:23 2024, max compression
+gzip compressed data, was "test_nvf_builds-0.0.2.tar", last modified: Mon May  6 15:42:05 2024, max compression
```

## Comparing `test_nvf_builds-0.0.1.tar` & `test_nvf_builds-0.0.2.tar`

### file list

```diff
@@ -1,45 +1,42 @@
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 08:17:23.893809 test_nvf_builds-0.0.1/
--rw-r--r--   0 mostafa    (501) staff       (20)      438 2024-05-06 08:17:23.893748 test_nvf_builds-0.0.1/PKG-INFO
--rw-r--r--   0 mostafa    (501) staff       (20)       85 2024-05-06 07:53:59.000000 test_nvf_builds-0.0.1/README.md
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 08:17:23.887852 test_nvf_builds-0.0.1/oasysnow/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:25.000000 test_nvf_builds-0.0.1/oasysnow/__init__.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 08:17:23.887991 test_nvf_builds-0.0.1/oasysnow/nvflare/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:50:57.000000 test_nvf_builds-0.0.1/oasysnow/nvflare/__init__.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 08:17:23.888108 test_nvf_builds-0.0.1/oasysnow/nvflare/client/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:25:11.000000 test_nvf_builds-0.0.1/oasysnow/nvflare/client/__init__.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 08:17:23.888794 test_nvf_builds-0.0.1/oasysnow/nvflare/client/filters/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:35.000000 test_nvf_builds-0.0.1/oasysnow/nvflare/client/filters/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)     3468 2024-05-02 11:52:22.000000 test_nvf_builds-0.0.1/oasysnow/nvflare/client/filters/filter_data.py
--rw-r--r--   0 mostafa    (501) staff       (20)     2471 2024-05-02 11:52:22.000000 test_nvf_builds-0.0.1/oasysnow/nvflare/client/filters/filter_results.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 08:17:23.889343 test_nvf_builds-0.0.1/oasysnow/nvflare/client/trainer/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:41.000000 test_nvf_builds-0.0.1/oasysnow/nvflare/client/trainer/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)     5232 2024-05-02 13:52:34.000000 test_nvf_builds-0.0.1/oasysnow/nvflare/client/trainer/trainer.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 08:17:23.890139 test_nvf_builds-0.0.1/oasysnow/nvflare/model/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:36:02.000000 test_nvf_builds-0.0.1/oasysnow/nvflare/model/__init__.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 08:17:23.890781 test_nvf_builds-0.0.1/oasysnow/nvflare/model/data/
--rw-r--r--   0 mostafa    (501) staff       (20)     1136 2024-05-02 13:27:01.000000 test_nvf_builds-0.0.1/oasysnow/nvflare/model/data/SNP_gene_mask.npz
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 14:12:08.000000 test_nvf_builds-0.0.1/oasysnow/nvflare/model/data/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)     2460 2024-05-02 13:22:42.000000 test_nvf_builds-0.0.1/oasysnow/nvflare/model/gennet_model.py
--rw-r--r--   0 mostafa    (501) staff       (20)     1928 2024-05-02 13:26:14.000000 test_nvf_builds-0.0.1/oasysnow/nvflare/model/global_model.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 08:17:23.890905 test_nvf_builds-0.0.1/oasysnow/nvflare/server/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:44:11.000000 test_nvf_builds-0.0.1/oasysnow/nvflare/server/__init__.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 08:17:23.891481 test_nvf_builds-0.0.1/oasysnow/nvflare/server/filters/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:44:45.000000 test_nvf_builds-0.0.1/oasysnow/nvflare/server/filters/__init__.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 08:17:23.892090 test_nvf_builds-0.0.1/oasysnow/nvflare/server/filters/attestation_service/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-03 14:56:34.000000 test_nvf_builds-0.0.1/oasysnow/nvflare/server/filters/attestation_service/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-03 14:46:21.000000 test_nvf_builds-0.0.1/oasysnow/nvflare/server/filters/attestation_service/server.py
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-03 14:56:28.000000 test_nvf_builds-0.0.1/oasysnow/nvflare/server/filters/attestation_service/verification.py
--rw-r--r--   0 mostafa    (501) staff       (20)     4442 2024-05-03 13:51:03.000000 test_nvf_builds-0.0.1/oasysnow/nvflare/server/filters/filter_data.py
--rw-r--r--   0 mostafa    (501) staff       (20)     2475 2024-04-19 21:41:54.000000 test_nvf_builds-0.0.1/oasysnow/nvflare/server/filters/filter_results.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 08:17:23.892329 test_nvf_builds-0.0.1/oasysnow/nvflare/server/model_runner/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:45:46.000000 test_nvf_builds-0.0.1/oasysnow/nvflare/server/model_runner/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)     5422 2024-05-02 14:00:51.000000 test_nvf_builds-0.0.1/oasysnow/nvflare/server/model_runner/model_runner.py
--rw-r--r--   0 mostafa    (501) staff       (20)       57 2024-05-06 08:08:28.000000 test_nvf_builds-0.0.1/requirements.txt
--rw-r--r--   0 mostafa    (501) staff       (20)      435 2024-05-06 08:17:23.894057 test_nvf_builds-0.0.1/setup.cfg
--rw-r--r--   0 mostafa    (501) staff       (20)      314 2024-05-02 14:15:15.000000 test_nvf_builds-0.0.1/setup.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 08:17:23.893504 test_nvf_builds-0.0.1/test_nvf_builds.egg-info/
--rw-r--r--   0 mostafa    (501) staff       (20)      438 2024-05-06 08:17:23.000000 test_nvf_builds-0.0.1/test_nvf_builds.egg-info/PKG-INFO
--rw-r--r--   0 mostafa    (501) staff       (20)     1225 2024-05-06 08:17:23.000000 test_nvf_builds-0.0.1/test_nvf_builds.egg-info/SOURCES.txt
--rw-r--r--   0 mostafa    (501) staff       (20)        1 2024-05-06 08:17:23.000000 test_nvf_builds-0.0.1/test_nvf_builds.egg-info/dependency_links.txt
--rw-r--r--   0 mostafa    (501) staff       (20)       57 2024-05-06 08:17:23.000000 test_nvf_builds-0.0.1/test_nvf_builds.egg-info/requires.txt
--rw-r--r--   0 mostafa    (501) staff       (20)        9 2024-05-06 08:17:23.000000 test_nvf_builds-0.0.1/test_nvf_builds.egg-info/top_level.txt
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 15:42:05.659165 test_nvf_builds-0.0.2/
+-rw-r--r--   0 mostafa    (501) staff       (20)      402 2024-05-06 15:42:05.659096 test_nvf_builds-0.0.2/PKG-INFO
+-rw-r--r--   0 mostafa    (501) staff       (20)       85 2024-05-06 07:53:59.000000 test_nvf_builds-0.0.2/README.md
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 15:42:05.654161 test_nvf_builds-0.0.2/oasysnow/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:25.000000 test_nvf_builds-0.0.2/oasysnow/__init__.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 15:42:05.654263 test_nvf_builds-0.0.2/oasysnow/nvflare/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:50:57.000000 test_nvf_builds-0.0.2/oasysnow/nvflare/__init__.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 15:42:05.654359 test_nvf_builds-0.0.2/oasysnow/nvflare/client/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:25:11.000000 test_nvf_builds-0.0.2/oasysnow/nvflare/client/__init__.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 15:42:05.654996 test_nvf_builds-0.0.2/oasysnow/nvflare/client/filters/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:35.000000 test_nvf_builds-0.0.2/oasysnow/nvflare/client/filters/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     3468 2024-05-02 11:52:22.000000 test_nvf_builds-0.0.2/oasysnow/nvflare/client/filters/filter_data.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     2471 2024-05-02 11:52:22.000000 test_nvf_builds-0.0.2/oasysnow/nvflare/client/filters/filter_results.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 15:42:05.655504 test_nvf_builds-0.0.2/oasysnow/nvflare/client/trainer/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:41.000000 test_nvf_builds-0.0.2/oasysnow/nvflare/client/trainer/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     5232 2024-05-02 13:52:34.000000 test_nvf_builds-0.0.2/oasysnow/nvflare/client/trainer/trainer.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 15:42:05.656214 test_nvf_builds-0.0.2/oasysnow/nvflare/model/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:36:02.000000 test_nvf_builds-0.0.2/oasysnow/nvflare/model/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     2460 2024-05-02 13:22:42.000000 test_nvf_builds-0.0.2/oasysnow/nvflare/model/gennet_model.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     1928 2024-05-02 13:26:14.000000 test_nvf_builds-0.0.2/oasysnow/nvflare/model/global_model.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 15:42:05.656458 test_nvf_builds-0.0.2/oasysnow/nvflare/server/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:44:11.000000 test_nvf_builds-0.0.2/oasysnow/nvflare/server/__init__.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 15:42:05.656961 test_nvf_builds-0.0.2/oasysnow/nvflare/server/filters/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:44:45.000000 test_nvf_builds-0.0.2/oasysnow/nvflare/server/filters/__init__.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 15:42:05.657457 test_nvf_builds-0.0.2/oasysnow/nvflare/server/filters/attestation_service/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-03 14:56:34.000000 test_nvf_builds-0.0.2/oasysnow/nvflare/server/filters/attestation_service/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-03 14:46:21.000000 test_nvf_builds-0.0.2/oasysnow/nvflare/server/filters/attestation_service/server.py
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-03 14:56:28.000000 test_nvf_builds-0.0.2/oasysnow/nvflare/server/filters/attestation_service/verification.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     4442 2024-05-03 13:51:03.000000 test_nvf_builds-0.0.2/oasysnow/nvflare/server/filters/filter_data.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     2475 2024-04-19 21:41:54.000000 test_nvf_builds-0.0.2/oasysnow/nvflare/server/filters/filter_results.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 15:42:05.657669 test_nvf_builds-0.0.2/oasysnow/nvflare/server/model_runner/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:45:46.000000 test_nvf_builds-0.0.2/oasysnow/nvflare/server/model_runner/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     5422 2024-05-02 14:00:51.000000 test_nvf_builds-0.0.2/oasysnow/nvflare/server/model_runner/model_runner.py
+-rw-r--r--   0 mostafa    (501) staff       (20)       36 2024-05-06 15:40:29.000000 test_nvf_builds-0.0.2/requirements.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)      435 2024-05-06 15:42:05.659415 test_nvf_builds-0.0.2/setup.cfg
+-rw-r--r--   0 mostafa    (501) staff       (20)      322 2024-05-06 15:10:01.000000 test_nvf_builds-0.0.2/setup.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-06 15:42:05.658849 test_nvf_builds-0.0.2/test_nvf_builds.egg-info/
+-rw-r--r--   0 mostafa    (501) staff       (20)      402 2024-05-06 15:42:05.000000 test_nvf_builds-0.0.2/test_nvf_builds.egg-info/PKG-INFO
+-rw-r--r--   0 mostafa    (501) staff       (20)     1139 2024-05-06 15:42:05.000000 test_nvf_builds-0.0.2/test_nvf_builds.egg-info/SOURCES.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)        1 2024-05-06 15:42:05.000000 test_nvf_builds-0.0.2/test_nvf_builds.egg-info/dependency_links.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)       36 2024-05-06 15:42:05.000000 test_nvf_builds-0.0.2/test_nvf_builds.egg-info/requires.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)        9 2024-05-06 15:42:05.000000 test_nvf_builds-0.0.2/test_nvf_builds.egg-info/top_level.txt
```

### Comparing `test_nvf_builds-0.0.1/oasysnow/nvflare/client/filters/filter_data.py` & `test_nvf_builds-0.0.2/oasysnow/nvflare/client/filters/filter_data.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.1/oasysnow/nvflare/client/filters/filter_results.py` & `test_nvf_builds-0.0.2/oasysnow/nvflare/client/filters/filter_results.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.1/oasysnow/nvflare/client/trainer/trainer.py` & `test_nvf_builds-0.0.2/oasysnow/nvflare/client/trainer/trainer.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.1/oasysnow/nvflare/model/gennet_model.py` & `test_nvf_builds-0.0.2/oasysnow/nvflare/model/gennet_model.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.1/oasysnow/nvflare/model/global_model.py` & `test_nvf_builds-0.0.2/oasysnow/nvflare/model/global_model.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.1/oasysnow/nvflare/server/filters/filter_data.py` & `test_nvf_builds-0.0.2/oasysnow/nvflare/server/filters/filter_data.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.1/oasysnow/nvflare/server/filters/filter_results.py` & `test_nvf_builds-0.0.2/oasysnow/nvflare/server/filters/filter_results.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.1/oasysnow/nvflare/server/model_runner/model_runner.py` & `test_nvf_builds-0.0.2/oasysnow/nvflare/server/model_runner/model_runner.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.1/test_nvf_builds.egg-info/SOURCES.txt` & `test_nvf_builds-0.0.2/test_nvf_builds.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 oasysnow/nvflare/client/filters/filter_data.py
 oasysnow/nvflare/client/filters/filter_results.py
 oasysnow/nvflare/client/trainer/__init__.py
 oasysnow/nvflare/client/trainer/trainer.py
 oasysnow/nvflare/model/__init__.py
 oasysnow/nvflare/model/gennet_model.py
 oasysnow/nvflare/model/global_model.py
-oasysnow/nvflare/model/data/SNP_gene_mask.npz
-oasysnow/nvflare/model/data/__init__.py
 oasysnow/nvflare/server/__init__.py
 oasysnow/nvflare/server/filters/__init__.py
 oasysnow/nvflare/server/filters/filter_data.py
 oasysnow/nvflare/server/filters/filter_results.py
 oasysnow/nvflare/server/filters/attestation_service/__init__.py
 oasysnow/nvflare/server/filters/attestation_service/server.py
 oasysnow/nvflare/server/filters/attestation_service/verification.py
```

