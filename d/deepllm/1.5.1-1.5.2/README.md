# Comparing `tmp/deepllm-1.5.1.tar.gz` & `tmp/deepllm-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepllm-1.5.1.tar", last modified: Sun May  5 23:25:42 2024, max compression
+gzip compressed data, was "deepllm-1.5.2.tar", last modified: Mon May  6 01:08:38 2024, max compression
```

## Comparing `deepllm-1.5.1.tar` & `deepllm-1.5.2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-05-05 23:25:42.153004 deepllm-1.5.1/
--rw-r--r--   0 tarau      (503) staff       (20)    35149 2023-06-23 23:27:38.000000 deepllm-1.5.1/LICENSE
--rw-r--r--   0 tarau      (503) staff       (20)     4651 2024-05-05 23:25:42.152689 deepllm-1.5.1/PKG-INFO
--rw-r--r--   0 tarau      (503) staff       (20)     4366 2023-07-18 14:36:48.000000 deepllm-1.5.1/README.md
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-05-05 23:25:42.132518 deepllm-1.5.1/deepllm/
--rw-r--r--   0 tarau      (503) staff       (20)       22 2024-05-05 23:23:47.000000 deepllm-1.5.1/deepllm/__init__.py
--rw-r--r--   0 tarau      (503) staff       (20)     2180 2024-04-28 16:21:55.000000 deepllm-1.5.1/deepllm/api.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-05-05 23:25:42.137900 deepllm-1.5.1/deepllm/apps/
--rw-r--r--   0 tarau      (503) staff       (20)       51 2023-07-08 16:25:29.000000 deepllm-1.5.1/deepllm/apps/README.md
--rw-r--r--   0 tarau      (503) staff       (20)     3615 2024-03-25 00:43:56.000000 deepllm-1.5.1/deepllm/apps/app.py
--rwxr-xr-x   0 tarau      (503) staff       (20)       21 2023-08-09 18:23:15.000000 deepllm-1.5.1/deepllm/apps/app.sh
--rwxr-xr-x   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-1.5.1/deepllm/apps/install.sh
--rw-r--r--   0 tarau      (503) staff       (20)    24934 2024-05-04 19:56:14.000000 deepllm-1.5.1/deepllm/apps/rel_graph.html
--rw-r--r--   0 tarau      (503) staff       (20)       18 2024-03-16 22:29:32.000000 deepllm-1.5.1/deepllm/apps/requirements.txt
--rw-r--r--   0 tarau      (503) staff       (20)      663 2024-01-01 16:38:49.000000 deepllm-1.5.1/deepllm/configurator.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-05-05 23:25:42.140759 deepllm-1.5.1/deepllm/demos/
--rw-r--r--   0 tarau      (503) staff       (20)       98 2023-07-10 19:44:29.000000 deepllm-1.5.1/deepllm/demos/README.md
--rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-1.5.1/deepllm/demos/__init__.py
--rw-r--r--   0 tarau      (503) staff       (20)     2151 2024-02-25 03:35:53.000000 deepllm-1.5.1/deepllm/demos/demo.py
--rwxr-xr-x   0 tarau      (503) staff       (20)       75 2024-01-02 02:47:22.000000 deepllm-1.5.1/deepllm/demos/install.sh
--rw-r--r--   0 tarau      (503) staff       (20)       44 2024-01-02 02:54:03.000000 deepllm-1.5.1/deepllm/demos/requirements.txt
--rw-r--r--   0 tarau      (503) staff       (20)     1951 2023-10-04 22:28:27.000000 deepllm-1.5.1/deepllm/demos/viz.py
--rw-r--r--   0 tarau      (503) staff       (20)     3825 2023-10-13 02:28:54.000000 deepllm-1.5.1/deepllm/horn_prover.py
--rw-r--r--   0 tarau      (503) staff       (20)    11151 2024-04-20 21:22:06.000000 deepllm-1.5.1/deepllm/interactors.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-05-05 23:25:42.145637 deepllm-1.5.1/deepllm/local_llms/
--rw-r--r--   0 tarau      (503) staff       (20)      108 2023-07-03 02:51:19.000000 deepllm-1.5.1/deepllm/local_llms/README.md
--rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-1.5.1/deepllm/local_llms/__init__.py
--rw-r--r--   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-1.5.1/deepllm/local_llms/install.sh
--rw-r--r--   0 tarau      (503) staff       (20)      727 2023-07-03 05:58:58.000000 deepllm-1.5.1/deepllm/local_llms/local_runs.py
--rw-r--r--   0 tarau      (503) staff       (20)        9 2023-07-03 02:40:19.000000 deepllm-1.5.1/deepllm/local_llms/requirements.txt
--rwxr-xr-x   0 tarau      (503) staff       (20)      205 2023-07-03 02:43:48.000000 deepllm-1.5.1/deepllm/local_llms/server.sh
--rw-r--r--   0 tarau      (503) staff       (20)     1005 2024-04-20 00:01:10.000000 deepllm-1.5.1/deepllm/local_llms/test_llama3.py
--rw-r--r--   0 tarau      (503) staff       (20)     1028 2023-08-12 16:50:59.000000 deepllm-1.5.1/deepllm/local_llms/test_vicuna.py
--rw-r--r--   0 tarau      (503) staff       (20)     3958 2024-04-28 16:22:31.000000 deepllm-1.5.1/deepllm/params.py
--rw-r--r--   0 tarau      (503) staff       (20)    10685 2024-05-04 19:52:35.000000 deepllm-1.5.1/deepllm/prompters.py
--rw-r--r--   0 tarau      (503) staff       (20)     4061 2024-02-26 23:53:37.000000 deepllm-1.5.1/deepllm/questmaker.py
--rw-r--r--   0 tarau      (503) staff       (20)    11003 2024-04-28 19:31:54.000000 deepllm-1.5.1/deepllm/recursors.py
--rw-r--r--   0 tarau      (503) staff       (20)     6758 2024-04-07 20:07:59.000000 deepllm-1.5.1/deepllm/refiners.py
--rw-r--r--   0 tarau      (503) staff       (20)       59 2024-03-22 20:57:32.000000 deepllm-1.5.1/deepllm/requirements.txt
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-05-05 23:25:42.151995 deepllm-1.5.1/deepllm/tests/
--rw-r--r--   0 tarau      (503) staff       (20)      126 2023-07-08 20:37:56.000000 deepllm-1.5.1/deepllm/tests/README.md
--rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-02 23:51:45.000000 deepllm-1.5.1/deepllm/tests/__init__.py
--rwxr-xr-x   0 tarau      (503) staff       (20)      596 2024-03-15 13:54:55.000000 deepllm-1.5.1/deepllm/tests/test_all.py
--rw-r--r--   0 tarau      (503) staff       (20)      906 2023-08-13 18:57:17.000000 deepllm-1.5.1/deepllm/tests/test_api.py
--rw-r--r--   0 tarau      (503) staff       (20)      381 2023-07-15 20:32:09.000000 deepllm-1.5.1/deepllm/tests/test_configurator.py
--rw-r--r--   0 tarau      (503) staff       (20)      526 2024-03-16 00:51:59.000000 deepllm-1.5.1/deepllm/tests/test_embedders.py
--rw-r--r--   0 tarau      (503) staff       (20)      100 2023-07-03 00:38:48.000000 deepllm-1.5.1/deepllm/tests/test_horn_prover.py
--rw-r--r--   0 tarau      (503) staff       (20)      499 2023-07-19 14:10:18.000000 deepllm-1.5.1/deepllm/tests/test_interactors.py
--rw-r--r--   0 tarau      (503) staff       (20)      294 2023-07-03 05:58:15.000000 deepllm-1.5.1/deepllm/tests/test_params.py
--rw-r--r--   0 tarau      (503) staff       (20)     1216 2024-01-29 22:45:46.000000 deepllm-1.5.1/deepllm/tests/test_recursors.py
--rw-r--r--   0 tarau      (503) staff       (20)     2284 2023-07-08 20:38:27.000000 deepllm-1.5.1/deepllm/tests/test_refiners.py
--rw-r--r--   0 tarau      (503) staff       (20)     1287 2023-12-28 01:58:47.000000 deepllm-1.5.1/deepllm/tools.py
--rw-r--r--   0 tarau      (503) staff       (20)      882 2024-03-22 20:43:06.000000 deepllm-1.5.1/deepllm/vis.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-05-05 23:25:42.134650 deepllm-1.5.1/deepllm.egg-info/
--rw-r--r--   0 tarau      (503) staff       (20)     4651 2024-05-05 23:25:42.000000 deepllm-1.5.1/deepllm.egg-info/PKG-INFO
--rw-r--r--   0 tarau      (503) staff       (20)     1353 2024-05-05 23:25:42.000000 deepllm-1.5.1/deepllm.egg-info/SOURCES.txt
--rw-r--r--   0 tarau      (503) staff       (20)        1 2024-05-05 23:25:42.000000 deepllm-1.5.1/deepllm.egg-info/dependency_links.txt
--rw-r--r--   0 tarau      (503) staff       (20)        1 2024-05-05 23:25:42.000000 deepllm-1.5.1/deepllm.egg-info/not-zip-safe
--rw-r--r--   0 tarau      (503) staff       (20)       59 2024-05-05 23:25:42.000000 deepllm-1.5.1/deepllm.egg-info/requires.txt
--rw-r--r--   0 tarau      (503) staff       (20)        8 2024-05-05 23:25:42.000000 deepllm-1.5.1/deepllm.egg-info/top_level.txt
--rw-r--r--   0 tarau      (503) staff       (20)       38 2024-05-05 23:25:42.153118 deepllm-1.5.1/setup.cfg
--rw-r--r--   0 tarau      (503) staff       (20)      967 2023-11-08 02:45:22.000000 deepllm-1.5.1/setup.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-05-06 01:08:38.310905 deepllm-1.5.2/
+-rw-r--r--   0 tarau      (503) staff       (20)    35149 2023-06-23 23:27:38.000000 deepllm-1.5.2/LICENSE
+-rw-r--r--   0 tarau      (503) staff       (20)     4651 2024-05-06 01:08:38.310555 deepllm-1.5.2/PKG-INFO
+-rw-r--r--   0 tarau      (503) staff       (20)     4366 2023-07-18 14:36:48.000000 deepllm-1.5.2/README.md
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-05-06 01:08:38.295471 deepllm-1.5.2/deepllm/
+-rw-r--r--   0 tarau      (503) staff       (20)       22 2024-05-06 01:07:42.000000 deepllm-1.5.2/deepllm/__init__.py
+-rw-r--r--   0 tarau      (503) staff       (20)     2253 2024-05-06 01:04:29.000000 deepllm-1.5.2/deepllm/api.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-05-06 01:08:38.299642 deepllm-1.5.2/deepllm/apps/
+-rw-r--r--   0 tarau      (503) staff       (20)       51 2023-07-08 16:25:29.000000 deepllm-1.5.2/deepllm/apps/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)     3626 2024-05-06 01:07:42.000000 deepllm-1.5.2/deepllm/apps/app.py
+-rwxr-xr-x   0 tarau      (503) staff       (20)       21 2023-08-09 18:23:15.000000 deepllm-1.5.2/deepllm/apps/app.sh
+-rwxr-xr-x   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-1.5.2/deepllm/apps/install.sh
+-rw-r--r--   0 tarau      (503) staff       (20)    24934 2024-05-04 19:56:14.000000 deepllm-1.5.2/deepllm/apps/rel_graph.html
+-rw-r--r--   0 tarau      (503) staff       (20)       18 2024-03-16 22:29:32.000000 deepllm-1.5.2/deepllm/apps/requirements.txt
+-rw-r--r--   0 tarau      (503) staff       (20)      663 2024-01-01 16:38:49.000000 deepllm-1.5.2/deepllm/configurator.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-05-06 01:08:38.301793 deepllm-1.5.2/deepllm/demos/
+-rw-r--r--   0 tarau      (503) staff       (20)       98 2023-07-10 19:44:29.000000 deepllm-1.5.2/deepllm/demos/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-1.5.2/deepllm/demos/__init__.py
+-rw-r--r--   0 tarau      (503) staff       (20)     2151 2024-02-25 03:35:53.000000 deepllm-1.5.2/deepllm/demos/demo.py
+-rwxr-xr-x   0 tarau      (503) staff       (20)       75 2024-01-02 02:47:22.000000 deepllm-1.5.2/deepllm/demos/install.sh
+-rw-r--r--   0 tarau      (503) staff       (20)       44 2024-01-02 02:54:03.000000 deepllm-1.5.2/deepllm/demos/requirements.txt
+-rw-r--r--   0 tarau      (503) staff       (20)     1951 2023-10-04 22:28:27.000000 deepllm-1.5.2/deepllm/demos/viz.py
+-rw-r--r--   0 tarau      (503) staff       (20)     3825 2023-10-13 02:28:54.000000 deepllm-1.5.2/deepllm/horn_prover.py
+-rw-r--r--   0 tarau      (503) staff       (20)    11151 2024-04-20 21:22:06.000000 deepllm-1.5.2/deepllm/interactors.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-05-06 01:08:38.304418 deepllm-1.5.2/deepllm/local_llms/
+-rw-r--r--   0 tarau      (503) staff       (20)      108 2023-07-03 02:51:19.000000 deepllm-1.5.2/deepllm/local_llms/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-1.5.2/deepllm/local_llms/__init__.py
+-rw-r--r--   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-1.5.2/deepllm/local_llms/install.sh
+-rw-r--r--   0 tarau      (503) staff       (20)      727 2023-07-03 05:58:58.000000 deepllm-1.5.2/deepllm/local_llms/local_runs.py
+-rw-r--r--   0 tarau      (503) staff       (20)        9 2023-07-03 02:40:19.000000 deepllm-1.5.2/deepllm/local_llms/requirements.txt
+-rwxr-xr-x   0 tarau      (503) staff       (20)      205 2023-07-03 02:43:48.000000 deepllm-1.5.2/deepllm/local_llms/server.sh
+-rw-r--r--   0 tarau      (503) staff       (20)     1005 2024-04-20 00:01:10.000000 deepllm-1.5.2/deepllm/local_llms/test_llama3.py
+-rw-r--r--   0 tarau      (503) staff       (20)     1028 2023-08-12 16:50:59.000000 deepllm-1.5.2/deepllm/local_llms/test_vicuna.py
+-rw-r--r--   0 tarau      (503) staff       (20)     3958 2024-04-28 16:22:31.000000 deepllm-1.5.2/deepllm/params.py
+-rw-r--r--   0 tarau      (503) staff       (20)    10685 2024-05-04 19:52:35.000000 deepllm-1.5.2/deepllm/prompters.py
+-rw-r--r--   0 tarau      (503) staff       (20)     4061 2024-02-26 23:53:37.000000 deepllm-1.5.2/deepllm/questmaker.py
+-rw-r--r--   0 tarau      (503) staff       (20)    11003 2024-04-28 19:31:54.000000 deepllm-1.5.2/deepllm/recursors.py
+-rw-r--r--   0 tarau      (503) staff       (20)     6758 2024-04-07 20:07:59.000000 deepllm-1.5.2/deepllm/refiners.py
+-rw-r--r--   0 tarau      (503) staff       (20)       59 2024-03-22 20:57:32.000000 deepllm-1.5.2/deepllm/requirements.txt
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-05-06 01:08:38.309864 deepllm-1.5.2/deepllm/tests/
+-rw-r--r--   0 tarau      (503) staff       (20)      126 2023-07-08 20:37:56.000000 deepllm-1.5.2/deepllm/tests/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-02 23:51:45.000000 deepllm-1.5.2/deepllm/tests/__init__.py
+-rwxr-xr-x   0 tarau      (503) staff       (20)      596 2024-03-15 13:54:55.000000 deepllm-1.5.2/deepllm/tests/test_all.py
+-rw-r--r--   0 tarau      (503) staff       (20)      906 2023-08-13 18:57:17.000000 deepllm-1.5.2/deepllm/tests/test_api.py
+-rw-r--r--   0 tarau      (503) staff       (20)      381 2023-07-15 20:32:09.000000 deepllm-1.5.2/deepllm/tests/test_configurator.py
+-rw-r--r--   0 tarau      (503) staff       (20)      526 2024-03-16 00:51:59.000000 deepllm-1.5.2/deepllm/tests/test_embedders.py
+-rw-r--r--   0 tarau      (503) staff       (20)      100 2023-07-03 00:38:48.000000 deepllm-1.5.2/deepllm/tests/test_horn_prover.py
+-rw-r--r--   0 tarau      (503) staff       (20)      499 2023-07-19 14:10:18.000000 deepllm-1.5.2/deepllm/tests/test_interactors.py
+-rw-r--r--   0 tarau      (503) staff       (20)      294 2023-07-03 05:58:15.000000 deepllm-1.5.2/deepllm/tests/test_params.py
+-rw-r--r--   0 tarau      (503) staff       (20)     1216 2024-01-29 22:45:46.000000 deepllm-1.5.2/deepllm/tests/test_recursors.py
+-rw-r--r--   0 tarau      (503) staff       (20)     2284 2023-07-08 20:38:27.000000 deepllm-1.5.2/deepllm/tests/test_refiners.py
+-rw-r--r--   0 tarau      (503) staff       (20)     1287 2023-12-28 01:58:47.000000 deepllm-1.5.2/deepllm/tools.py
+-rw-r--r--   0 tarau      (503) staff       (20)      882 2024-03-22 20:43:06.000000 deepllm-1.5.2/deepllm/vis.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-05-06 01:08:38.297414 deepllm-1.5.2/deepllm.egg-info/
+-rw-r--r--   0 tarau      (503) staff       (20)     4651 2024-05-06 01:08:38.000000 deepllm-1.5.2/deepllm.egg-info/PKG-INFO
+-rw-r--r--   0 tarau      (503) staff       (20)     1353 2024-05-06 01:08:38.000000 deepllm-1.5.2/deepllm.egg-info/SOURCES.txt
+-rw-r--r--   0 tarau      (503) staff       (20)        1 2024-05-06 01:08:38.000000 deepllm-1.5.2/deepllm.egg-info/dependency_links.txt
+-rw-r--r--   0 tarau      (503) staff       (20)        1 2024-05-06 01:08:38.000000 deepllm-1.5.2/deepllm.egg-info/not-zip-safe
+-rw-r--r--   0 tarau      (503) staff       (20)       59 2024-05-06 01:08:38.000000 deepllm-1.5.2/deepllm.egg-info/requires.txt
+-rw-r--r--   0 tarau      (503) staff       (20)        8 2024-05-06 01:08:38.000000 deepllm-1.5.2/deepllm.egg-info/top_level.txt
+-rw-r--r--   0 tarau      (503) staff       (20)       38 2024-05-06 01:08:38.311054 deepllm-1.5.2/setup.cfg
+-rw-r--r--   0 tarau      (503) staff       (20)      967 2023-11-08 02:45:22.000000 deepllm-1.5.2/setup.py
```

### Comparing `deepllm-1.5.1/LICENSE` & `deepllm-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.1/PKG-INFO` & `deepllm-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepllm
-Version: 1.5.1
+Version: 1.5.2
 Summary: Deep, recursive, goal-driven LLM explorer
 Home-page: https://github.com/ptarau/recursors.git
 Author: Paul Tarau
 Author-email: paul.tarau@gmail.com
 License: GPL-3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `deepllm-1.5.1/README.md` & `deepllm-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.1/deepllm/api.py` & `deepllm-1.5.2/deepllm/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+from deepllm import __version__
 from deepllm.prompters import *
 from deepllm.params import *
 from deepllm.recursors import AndOrExplorer, show_clauses, show_model, show_svos,vis_svos
 from deepllm.vis import browse
 from deepllm.refiners import Advisor, Rater, TruthRater, AbstractMaker, SummaryMaker, PaperReviewer,RetrievalRefiner
 
-
+def get_version():
+    return __version__
 def activate_svos():
     GPT_PARAMS['TO_SVOS']=True
     LOCAL_PARAMS['TO_SVOS'] = True
 
 def deactivate_svos():
     GPT_PARAMS['TO_SVOS']=False
     LOCAL_PARAMS['TO_SVOS'] = False
```

### Comparing `deepllm-1.5.1/deepllm/apps/app.py` & `deepllm-1.5.2/deepllm/apps/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from deepllm.api import *
 
 print('Running DeepLLM as a streamlit app!')
 
 st.set_page_config(layout="wide")
 
-st.title('Streamlit-based [DeepLLM](https://github.com/ptarau/recursors) Demo Client')
+st.title('Streamlit-based [DeepLLM](https://github.com/ptarau/recursors) Client '+ get_version())
 
 prompters = prompter_dict()
 
 def clear_key():
     API_KEY[0]=""
 
 def collect_key():
```

### Comparing `deepllm-1.5.1/deepllm/apps/rel_graph.html` & `deepllm-1.5.2/deepllm/apps/rel_graph.html`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.1/deepllm/configurator.py` & `deepllm-1.5.2/deepllm/configurator.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.1/deepllm/demos/demo.py` & `deepllm-1.5.2/deepllm/demos/demo.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.1/deepllm/demos/viz.py` & `deepllm-1.5.2/deepllm/demos/viz.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.1/deepllm/horn_prover.py` & `deepllm-1.5.2/deepllm/horn_prover.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.1/deepllm/interactors.py` & `deepllm-1.5.2/deepllm/interactors.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.1/deepllm/local_llms/local_runs.py` & `deepllm-1.5.2/deepllm/local_llms/local_runs.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.1/deepllm/local_llms/test_llama3.py` & `deepllm-1.5.2/deepllm/local_llms/test_llama3.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.1/deepllm/local_llms/test_vicuna.py` & `deepllm-1.5.2/deepllm/local_llms/test_vicuna.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.1/deepllm/params.py` & `deepllm-1.5.2/deepllm/params.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.1/deepllm/prompters.py` & `deepllm-1.5.2/deepllm/prompters.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.1/deepllm/questmaker.py` & `deepllm-1.5.2/deepllm/questmaker.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.1/deepllm/recursors.py` & `deepllm-1.5.2/deepllm/recursors.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.1/deepllm/refiners.py` & `deepllm-1.5.2/deepllm/refiners.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.1/deepllm/tests/test_all.py` & `deepllm-1.5.2/deepllm/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.1/deepllm/tests/test_api.py` & `deepllm-1.5.2/deepllm/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.1/deepllm/tests/test_embedders.py` & `deepllm-1.5.2/deepllm/tests/test_embedders.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.1/deepllm/tests/test_recursors.py` & `deepllm-1.5.2/deepllm/tests/test_recursors.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.1/deepllm/tests/test_refiners.py` & `deepllm-1.5.2/deepllm/tests/test_refiners.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.1/deepllm/tools.py` & `deepllm-1.5.2/deepllm/tools.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.1/deepllm/vis.py` & `deepllm-1.5.2/deepllm/vis.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.1/deepllm.egg-info/PKG-INFO` & `deepllm-1.5.2/deepllm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepllm
-Version: 1.5.1
+Version: 1.5.2
 Summary: Deep, recursive, goal-driven LLM explorer
 Home-page: https://github.com/ptarau/recursors.git
 Author: Paul Tarau
 Author-email: paul.tarau@gmail.com
 License: GPL-3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `deepllm-1.5.1/deepllm.egg-info/SOURCES.txt` & `deepllm-1.5.2/deepllm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.1/setup.py` & `deepllm-1.5.2/setup.py`

 * *Files identical despite different names*

