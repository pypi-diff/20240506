# Comparing `tmp/deepllm-1.5.0.tar.gz` & `tmp/deepllm-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepllm-1.5.0.tar", last modified: Sun Apr 21 00:13:20 2024, max compression
+gzip compressed data, was "deepllm-1.5.1.tar", last modified: Sun May  5 23:25:42 2024, max compression
```

## Comparing `deepllm-1.5.0.tar` & `deepllm-1.5.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-21 00:13:20.575532 deepllm-1.5.0/
--rw-r--r--   0 tarau      (503) staff       (20)    35149 2023-06-23 23:27:38.000000 deepllm-1.5.0/LICENSE
--rw-r--r--   0 tarau      (503) staff       (20)     4651 2024-04-21 00:13:20.575225 deepllm-1.5.0/PKG-INFO
--rw-r--r--   0 tarau      (503) staff       (20)     4366 2023-07-18 14:36:48.000000 deepllm-1.5.0/README.md
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-21 00:13:20.553520 deepllm-1.5.0/deepllm/
--rw-r--r--   0 tarau      (503) staff       (20)       22 2024-04-20 15:13:25.000000 deepllm-1.5.0/deepllm/__init__.py
--rw-r--r--   0 tarau      (503) staff       (20)     2188 2024-03-22 05:04:24.000000 deepllm-1.5.0/deepllm/api.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-21 00:13:20.560501 deepllm-1.5.0/deepllm/apps/
--rw-r--r--   0 tarau      (503) staff       (20)       51 2023-07-08 16:25:29.000000 deepllm-1.5.0/deepllm/apps/README.md
--rw-r--r--   0 tarau      (503) staff       (20)     3615 2024-03-25 00:43:56.000000 deepllm-1.5.0/deepllm/apps/app.py
--rwxr-xr-x   0 tarau      (503) staff       (20)       21 2023-08-09 18:23:15.000000 deepllm-1.5.0/deepllm/apps/app.sh
--rwxr-xr-x   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-1.5.0/deepllm/apps/install.sh
--rw-r--r--   0 tarau      (503) staff       (20)   295587 2024-04-20 16:17:38.000000 deepllm-1.5.0/deepllm/apps/rel_graph.html
--rw-r--r--   0 tarau      (503) staff       (20)       18 2024-03-16 22:29:32.000000 deepllm-1.5.0/deepllm/apps/requirements.txt
--rw-r--r--   0 tarau      (503) staff       (20)      663 2024-01-01 16:38:49.000000 deepllm-1.5.0/deepllm/configurator.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-21 00:13:20.563022 deepllm-1.5.0/deepllm/demos/
--rw-r--r--   0 tarau      (503) staff       (20)       98 2023-07-10 19:44:29.000000 deepllm-1.5.0/deepllm/demos/README.md
--rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-1.5.0/deepllm/demos/__init__.py
--rw-r--r--   0 tarau      (503) staff       (20)     2151 2024-02-25 03:35:53.000000 deepllm-1.5.0/deepllm/demos/demo.py
--rwxr-xr-x   0 tarau      (503) staff       (20)       75 2024-01-02 02:47:22.000000 deepllm-1.5.0/deepllm/demos/install.sh
--rw-r--r--   0 tarau      (503) staff       (20)       44 2024-01-02 02:54:03.000000 deepllm-1.5.0/deepllm/demos/requirements.txt
--rw-r--r--   0 tarau      (503) staff       (20)     1951 2023-10-04 22:28:27.000000 deepllm-1.5.0/deepllm/demos/viz.py
--rw-r--r--   0 tarau      (503) staff       (20)     3825 2023-10-13 02:28:54.000000 deepllm-1.5.0/deepllm/horn_prover.py
--rw-r--r--   0 tarau      (503) staff       (20)    11151 2024-04-20 21:22:06.000000 deepllm-1.5.0/deepllm/interactors.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-21 00:13:20.566918 deepllm-1.5.0/deepllm/local_llms/
--rw-r--r--   0 tarau      (503) staff       (20)      108 2023-07-03 02:51:19.000000 deepllm-1.5.0/deepllm/local_llms/README.md
--rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-1.5.0/deepllm/local_llms/__init__.py
--rw-r--r--   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-1.5.0/deepllm/local_llms/install.sh
--rw-r--r--   0 tarau      (503) staff       (20)      727 2023-07-03 05:58:58.000000 deepllm-1.5.0/deepllm/local_llms/local_runs.py
--rw-r--r--   0 tarau      (503) staff       (20)        9 2023-07-03 02:40:19.000000 deepllm-1.5.0/deepllm/local_llms/requirements.txt
--rwxr-xr-x   0 tarau      (503) staff       (20)      205 2023-07-03 02:43:48.000000 deepllm-1.5.0/deepllm/local_llms/server.sh
--rw-r--r--   0 tarau      (503) staff       (20)     1005 2024-04-20 00:01:10.000000 deepllm-1.5.0/deepllm/local_llms/test_llama3.py
--rw-r--r--   0 tarau      (503) staff       (20)     1028 2023-08-12 16:50:59.000000 deepllm-1.5.0/deepllm/local_llms/test_vicuna.py
--rw-r--r--   0 tarau      (503) staff       (20)     3966 2024-04-20 23:33:01.000000 deepllm-1.5.0/deepllm/params.py
--rw-r--r--   0 tarau      (503) staff       (20)     9716 2024-04-07 21:18:58.000000 deepllm-1.5.0/deepllm/prompters.py
--rw-r--r--   0 tarau      (503) staff       (20)     4061 2024-02-26 23:53:37.000000 deepllm-1.5.0/deepllm/questmaker.py
--rw-r--r--   0 tarau      (503) staff       (20)    10784 2024-03-25 00:48:51.000000 deepllm-1.5.0/deepllm/recursors.py
--rw-r--r--   0 tarau      (503) staff       (20)     6758 2024-04-07 20:07:59.000000 deepllm-1.5.0/deepllm/refiners.py
--rw-r--r--   0 tarau      (503) staff       (20)       59 2024-03-22 20:57:32.000000 deepllm-1.5.0/deepllm/requirements.txt
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-21 00:13:20.574500 deepllm-1.5.0/deepllm/tests/
--rw-r--r--   0 tarau      (503) staff       (20)      126 2023-07-08 20:37:56.000000 deepllm-1.5.0/deepllm/tests/README.md
--rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-02 23:51:45.000000 deepllm-1.5.0/deepllm/tests/__init__.py
--rwxr-xr-x   0 tarau      (503) staff       (20)      596 2024-03-15 13:54:55.000000 deepllm-1.5.0/deepllm/tests/test_all.py
--rw-r--r--   0 tarau      (503) staff       (20)      906 2023-08-13 18:57:17.000000 deepllm-1.5.0/deepllm/tests/test_api.py
--rw-r--r--   0 tarau      (503) staff       (20)      381 2023-07-15 20:32:09.000000 deepllm-1.5.0/deepllm/tests/test_configurator.py
--rw-r--r--   0 tarau      (503) staff       (20)      526 2024-03-16 00:51:59.000000 deepllm-1.5.0/deepllm/tests/test_embedders.py
--rw-r--r--   0 tarau      (503) staff       (20)      100 2023-07-03 00:38:48.000000 deepllm-1.5.0/deepllm/tests/test_horn_prover.py
--rw-r--r--   0 tarau      (503) staff       (20)      499 2023-07-19 14:10:18.000000 deepllm-1.5.0/deepllm/tests/test_interactors.py
--rw-r--r--   0 tarau      (503) staff       (20)      294 2023-07-03 05:58:15.000000 deepllm-1.5.0/deepllm/tests/test_params.py
--rw-r--r--   0 tarau      (503) staff       (20)     1216 2024-01-29 22:45:46.000000 deepllm-1.5.0/deepllm/tests/test_recursors.py
--rw-r--r--   0 tarau      (503) staff       (20)     2284 2023-07-08 20:38:27.000000 deepllm-1.5.0/deepllm/tests/test_refiners.py
--rw-r--r--   0 tarau      (503) staff       (20)     1287 2023-12-28 01:58:47.000000 deepllm-1.5.0/deepllm/tools.py
--rw-r--r--   0 tarau      (503) staff       (20)      882 2024-03-22 20:43:06.000000 deepllm-1.5.0/deepllm/vis.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-21 00:13:20.555923 deepllm-1.5.0/deepllm.egg-info/
--rw-r--r--   0 tarau      (503) staff       (20)     4651 2024-04-21 00:13:20.000000 deepllm-1.5.0/deepllm.egg-info/PKG-INFO
--rw-r--r--   0 tarau      (503) staff       (20)     1353 2024-04-21 00:13:20.000000 deepllm-1.5.0/deepllm.egg-info/SOURCES.txt
--rw-r--r--   0 tarau      (503) staff       (20)        1 2024-04-21 00:13:20.000000 deepllm-1.5.0/deepllm.egg-info/dependency_links.txt
--rw-r--r--   0 tarau      (503) staff       (20)        1 2024-04-21 00:13:20.000000 deepllm-1.5.0/deepllm.egg-info/not-zip-safe
--rw-r--r--   0 tarau      (503) staff       (20)       59 2024-04-21 00:13:20.000000 deepllm-1.5.0/deepllm.egg-info/requires.txt
--rw-r--r--   0 tarau      (503) staff       (20)        8 2024-04-21 00:13:20.000000 deepllm-1.5.0/deepllm.egg-info/top_level.txt
--rw-r--r--   0 tarau      (503) staff       (20)       38 2024-04-21 00:13:20.575642 deepllm-1.5.0/setup.cfg
--rw-r--r--   0 tarau      (503) staff       (20)      967 2023-11-08 02:45:22.000000 deepllm-1.5.0/setup.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-05-05 23:25:42.153004 deepllm-1.5.1/
+-rw-r--r--   0 tarau      (503) staff       (20)    35149 2023-06-23 23:27:38.000000 deepllm-1.5.1/LICENSE
+-rw-r--r--   0 tarau      (503) staff       (20)     4651 2024-05-05 23:25:42.152689 deepllm-1.5.1/PKG-INFO
+-rw-r--r--   0 tarau      (503) staff       (20)     4366 2023-07-18 14:36:48.000000 deepllm-1.5.1/README.md
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-05-05 23:25:42.132518 deepllm-1.5.1/deepllm/
+-rw-r--r--   0 tarau      (503) staff       (20)       22 2024-05-05 23:23:47.000000 deepllm-1.5.1/deepllm/__init__.py
+-rw-r--r--   0 tarau      (503) staff       (20)     2180 2024-04-28 16:21:55.000000 deepllm-1.5.1/deepllm/api.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-05-05 23:25:42.137900 deepllm-1.5.1/deepllm/apps/
+-rw-r--r--   0 tarau      (503) staff       (20)       51 2023-07-08 16:25:29.000000 deepllm-1.5.1/deepllm/apps/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)     3615 2024-03-25 00:43:56.000000 deepllm-1.5.1/deepllm/apps/app.py
+-rwxr-xr-x   0 tarau      (503) staff       (20)       21 2023-08-09 18:23:15.000000 deepllm-1.5.1/deepllm/apps/app.sh
+-rwxr-xr-x   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-1.5.1/deepllm/apps/install.sh
+-rw-r--r--   0 tarau      (503) staff       (20)    24934 2024-05-04 19:56:14.000000 deepllm-1.5.1/deepllm/apps/rel_graph.html
+-rw-r--r--   0 tarau      (503) staff       (20)       18 2024-03-16 22:29:32.000000 deepllm-1.5.1/deepllm/apps/requirements.txt
+-rw-r--r--   0 tarau      (503) staff       (20)      663 2024-01-01 16:38:49.000000 deepllm-1.5.1/deepllm/configurator.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-05-05 23:25:42.140759 deepllm-1.5.1/deepllm/demos/
+-rw-r--r--   0 tarau      (503) staff       (20)       98 2023-07-10 19:44:29.000000 deepllm-1.5.1/deepllm/demos/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-1.5.1/deepllm/demos/__init__.py
+-rw-r--r--   0 tarau      (503) staff       (20)     2151 2024-02-25 03:35:53.000000 deepllm-1.5.1/deepllm/demos/demo.py
+-rwxr-xr-x   0 tarau      (503) staff       (20)       75 2024-01-02 02:47:22.000000 deepllm-1.5.1/deepllm/demos/install.sh
+-rw-r--r--   0 tarau      (503) staff       (20)       44 2024-01-02 02:54:03.000000 deepllm-1.5.1/deepllm/demos/requirements.txt
+-rw-r--r--   0 tarau      (503) staff       (20)     1951 2023-10-04 22:28:27.000000 deepllm-1.5.1/deepllm/demos/viz.py
+-rw-r--r--   0 tarau      (503) staff       (20)     3825 2023-10-13 02:28:54.000000 deepllm-1.5.1/deepllm/horn_prover.py
+-rw-r--r--   0 tarau      (503) staff       (20)    11151 2024-04-20 21:22:06.000000 deepllm-1.5.1/deepllm/interactors.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-05-05 23:25:42.145637 deepllm-1.5.1/deepllm/local_llms/
+-rw-r--r--   0 tarau      (503) staff       (20)      108 2023-07-03 02:51:19.000000 deepllm-1.5.1/deepllm/local_llms/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-1.5.1/deepllm/local_llms/__init__.py
+-rw-r--r--   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-1.5.1/deepllm/local_llms/install.sh
+-rw-r--r--   0 tarau      (503) staff       (20)      727 2023-07-03 05:58:58.000000 deepllm-1.5.1/deepllm/local_llms/local_runs.py
+-rw-r--r--   0 tarau      (503) staff       (20)        9 2023-07-03 02:40:19.000000 deepllm-1.5.1/deepllm/local_llms/requirements.txt
+-rwxr-xr-x   0 tarau      (503) staff       (20)      205 2023-07-03 02:43:48.000000 deepllm-1.5.1/deepllm/local_llms/server.sh
+-rw-r--r--   0 tarau      (503) staff       (20)     1005 2024-04-20 00:01:10.000000 deepllm-1.5.1/deepllm/local_llms/test_llama3.py
+-rw-r--r--   0 tarau      (503) staff       (20)     1028 2023-08-12 16:50:59.000000 deepllm-1.5.1/deepllm/local_llms/test_vicuna.py
+-rw-r--r--   0 tarau      (503) staff       (20)     3958 2024-04-28 16:22:31.000000 deepllm-1.5.1/deepllm/params.py
+-rw-r--r--   0 tarau      (503) staff       (20)    10685 2024-05-04 19:52:35.000000 deepllm-1.5.1/deepllm/prompters.py
+-rw-r--r--   0 tarau      (503) staff       (20)     4061 2024-02-26 23:53:37.000000 deepllm-1.5.1/deepllm/questmaker.py
+-rw-r--r--   0 tarau      (503) staff       (20)    11003 2024-04-28 19:31:54.000000 deepllm-1.5.1/deepllm/recursors.py
+-rw-r--r--   0 tarau      (503) staff       (20)     6758 2024-04-07 20:07:59.000000 deepllm-1.5.1/deepllm/refiners.py
+-rw-r--r--   0 tarau      (503) staff       (20)       59 2024-03-22 20:57:32.000000 deepllm-1.5.1/deepllm/requirements.txt
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-05-05 23:25:42.151995 deepllm-1.5.1/deepllm/tests/
+-rw-r--r--   0 tarau      (503) staff       (20)      126 2023-07-08 20:37:56.000000 deepllm-1.5.1/deepllm/tests/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-02 23:51:45.000000 deepllm-1.5.1/deepllm/tests/__init__.py
+-rwxr-xr-x   0 tarau      (503) staff       (20)      596 2024-03-15 13:54:55.000000 deepllm-1.5.1/deepllm/tests/test_all.py
+-rw-r--r--   0 tarau      (503) staff       (20)      906 2023-08-13 18:57:17.000000 deepllm-1.5.1/deepllm/tests/test_api.py
+-rw-r--r--   0 tarau      (503) staff       (20)      381 2023-07-15 20:32:09.000000 deepllm-1.5.1/deepllm/tests/test_configurator.py
+-rw-r--r--   0 tarau      (503) staff       (20)      526 2024-03-16 00:51:59.000000 deepllm-1.5.1/deepllm/tests/test_embedders.py
+-rw-r--r--   0 tarau      (503) staff       (20)      100 2023-07-03 00:38:48.000000 deepllm-1.5.1/deepllm/tests/test_horn_prover.py
+-rw-r--r--   0 tarau      (503) staff       (20)      499 2023-07-19 14:10:18.000000 deepllm-1.5.1/deepllm/tests/test_interactors.py
+-rw-r--r--   0 tarau      (503) staff       (20)      294 2023-07-03 05:58:15.000000 deepllm-1.5.1/deepllm/tests/test_params.py
+-rw-r--r--   0 tarau      (503) staff       (20)     1216 2024-01-29 22:45:46.000000 deepllm-1.5.1/deepllm/tests/test_recursors.py
+-rw-r--r--   0 tarau      (503) staff       (20)     2284 2023-07-08 20:38:27.000000 deepllm-1.5.1/deepllm/tests/test_refiners.py
+-rw-r--r--   0 tarau      (503) staff       (20)     1287 2023-12-28 01:58:47.000000 deepllm-1.5.1/deepllm/tools.py
+-rw-r--r--   0 tarau      (503) staff       (20)      882 2024-03-22 20:43:06.000000 deepllm-1.5.1/deepllm/vis.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-05-05 23:25:42.134650 deepllm-1.5.1/deepllm.egg-info/
+-rw-r--r--   0 tarau      (503) staff       (20)     4651 2024-05-05 23:25:42.000000 deepllm-1.5.1/deepllm.egg-info/PKG-INFO
+-rw-r--r--   0 tarau      (503) staff       (20)     1353 2024-05-05 23:25:42.000000 deepllm-1.5.1/deepllm.egg-info/SOURCES.txt
+-rw-r--r--   0 tarau      (503) staff       (20)        1 2024-05-05 23:25:42.000000 deepllm-1.5.1/deepllm.egg-info/dependency_links.txt
+-rw-r--r--   0 tarau      (503) staff       (20)        1 2024-05-05 23:25:42.000000 deepllm-1.5.1/deepllm.egg-info/not-zip-safe
+-rw-r--r--   0 tarau      (503) staff       (20)       59 2024-05-05 23:25:42.000000 deepllm-1.5.1/deepllm.egg-info/requires.txt
+-rw-r--r--   0 tarau      (503) staff       (20)        8 2024-05-05 23:25:42.000000 deepllm-1.5.1/deepllm.egg-info/top_level.txt
+-rw-r--r--   0 tarau      (503) staff       (20)       38 2024-05-05 23:25:42.153118 deepllm-1.5.1/setup.cfg
+-rw-r--r--   0 tarau      (503) staff       (20)      967 2023-11-08 02:45:22.000000 deepllm-1.5.1/setup.py
```

### Comparing `deepllm-1.5.0/LICENSE` & `deepllm-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.0/PKG-INFO` & `deepllm-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepllm
-Version: 1.5.0
+Version: 1.5.1
 Summary: Deep, recursive, goal-driven LLM explorer
 Home-page: https://github.com/ptarau/recursors.git
 Author: Paul Tarau
 Author-email: paul.tarau@gmail.com
 License: GPL-3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `deepllm-1.5.0/README.md` & `deepllm-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.0/deepllm/api.py` & `deepllm-1.5.1/deepllm/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     GPT_PARAMS['TO_SVOS']=False
     LOCAL_PARAMS['TO_SVOS'] = False
 
 
 def smarter_model():
     IS_LOCAL_LLM[0] = False
     #GPT_PARAMS['model'] = "gpt-4"
-    GPT_PARAMS['model'] ='gpt-4-turbo-preview'
+    GPT_PARAMS['model'] ='gpt-4-turbo'
     openai.api_base = GPT_PARAMS['API_BASE']
     GPT_PARAMS['ROOT'] = "./STATE_SMARTER/"
     PARAMS()
 
 
 def cheaper_model():
     IS_LOCAL_LLM[0] = False
```

### Comparing `deepllm-1.5.0/deepllm/apps/app.py` & `deepllm-1.5.1/deepllm/apps/app.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.0/deepllm/configurator.py` & `deepllm-1.5.1/deepllm/configurator.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.0/deepllm/demos/demo.py` & `deepllm-1.5.1/deepllm/demos/demo.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.0/deepllm/demos/viz.py` & `deepllm-1.5.1/deepllm/demos/viz.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.0/deepllm/horn_prover.py` & `deepllm-1.5.1/deepllm/horn_prover.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.0/deepllm/interactors.py` & `deepllm-1.5.1/deepllm/interactors.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.0/deepllm/local_llms/local_runs.py` & `deepllm-1.5.1/deepllm/local_llms/local_runs.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.0/deepllm/local_llms/test_llama3.py` & `deepllm-1.5.1/deepllm/local_llms/test_llama3.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.0/deepllm/local_llms/test_vicuna.py` & `deepllm-1.5.1/deepllm/local_llms/test_vicuna.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.0/deepllm/params.py` & `deepllm-1.5.1/deepllm/params.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     ROOT_="./STATE/",
     ROOT="./STATE_SMARTER/",
     CACHES="caches/",
     DATA="data/",
     OUT='out/',
     # model="gpt-3.5-turbo",
     # model="gpt-4",
-    model='gpt-4-turbo-preview',
+    model='gpt-4-turbo',
     emebedding_model="text-embedding-3-large",
     temperature=0.2,
     n=1,
     max_toks=12000,
     TOP_K=3,
     API_BASE="https://api.openai.com/v1",
     LOCAL_LLM=IS_LOCAL_LLM[0]
```

### Comparing `deepllm-1.5.0/deepllm/prompters.py` & `deepllm-1.5.1/deepllm/prompters.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,19 +63,38 @@
         Generate 2-3 alternative predictions citing facts that are likely to be consequences of "$g".
         Itemize your answer, one noun phrase per line.
          No explanations are needed, just the noun phrase, nothing else.
         Avoid starting your sentence with the word "Alternative".
         Your answer should not contain ":"."""
 )
 
+
+falsifier_prompter = dict(
+    name='explorer_of_negative_consequences',
+    and_p="""We strongly disaprove and need to refute that: "$context".
+        To help with this task, generate 1-2 noun phrases of 2-4 words 
+        with each alternative detailing undesirable consequences of "$g".
+        Itemize your answer, one consequence of "$g" per line.
+        No explanations needed, just the noun phrase, nothing else.
+        Avoid using the words "Noun phrases" in your answer.
+        Your answer should not contain ":".""",
+    or_p="""We strongly disaprove and need to refute that: "$context".
+        Generate 1-2 noun phrases of 2-4 words that together are undesirable consequences "$g".
+        Itemize your answer, one noun phrase per line.
+         No explanations are needed, just the noun phrase, nothing else.
+        Avoid starting your sentence with the word "Alternative".
+        Your answer should not contain ":"."""
+)
+
+
 sci_prompter = dict(
     name='scientific_concept_explorer',
     and_p="""The task we are exploring is: "$context"
         Generate 3-5 noun phrases of 2-4 words each that occur as keyphrases only
-        in scientific papers bout "$g".
+        in scientific papers about "$g".
         Itemize your answer, one noun phrase per line.
         No explanations needed, just the noun phrase, nothing else.
         """,
     or_p="""The topic we are exploring is: "$context"
         Generate 2-3 noun phrases describing details of "$g".
         Itemize your answer, one noun phrase per line.
         No explanations needed, just the noun phrase, nothing else.
@@ -215,15 +234,16 @@
 prompter_vars = [
     sci_prompter,
     conseq_prompter,
     causal_prompter,
     task_planning_prompter,
     recommendation_prompter,
     thesis_support_prompter,
-    cons_and_pros_prompter
+    cons_and_pros_prompter,
+    falsifier_prompter
 ]
 
 
 def prompter_dict():
     d = dict()
     for prompter in prompter_vars:
         name = prompter['name']
```

### Comparing `deepllm-1.5.0/deepllm/questmaker.py` & `deepllm-1.5.1/deepllm/questmaker.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.0/deepllm/recursors.py` & `deepllm-1.5.1/deepllm/recursors.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,15 +219,15 @@
     c1 = r.unf.or_.dollar_cost()
     c2 = r.unf.and_.dollar_cost()
     print('COSTS in $:', {'and': c1, 'or': c2, 'total': c1 + c2})
     return True
 
 
 def quote(x):
-    x=x.replace('\\','')
+    x=x.replace('\\','').replace("'","_")
     return "'" + x + "'"
 
 
 def show_clauses(clauses):
     buf = []
 
     def p(x):
@@ -336,26 +336,31 @@
 def to_prolog(clauses, fname, neck=":-", suf='.pro'):
     suf = '.nat' if neck == ":" else suf
 
     path = fname + suf
     ensure_path(path)
     with open(path, 'w') as f:
         print('% CLAUSES:', file=f)
+        rule_heads=set()
         for h, bss in clauses.items():
             for bs in bss:
                 if bs == [] or bs == ['fail']: continue
                 body = ',\n    '.join(map(quote, bs)) + "."
                 print(quote(h), neck + '\n    ' + body, file=f)
+                rule_heads.add(h)
         for h, bss in clauses.items():
             if bss == []:
+                if h in rule_heads: continue
                 print(quote(h) + ".", file=f)
             for bs in bss:
                 if bs == []:
+                    if h in rule_heads: continue
                     print(quote(h) + ".", file=f)
                 elif bs == ['fail']:
+                    if h in rule_heads: continue
                     print(quote(h), neck + ' ' + 'fail.', file=f)
 
 
 def to_context(trace, topgoal):
     if not trace: return topgoal
     context = ".\n".join(reversed(to_list(trace))) + ".\n"
     # print('!!!! CONTEXT:',context, '!!!!\n')
```

### Comparing `deepllm-1.5.0/deepllm/refiners.py` & `deepllm-1.5.1/deepllm/refiners.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.0/deepllm/tests/test_all.py` & `deepllm-1.5.1/deepllm/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.0/deepllm/tests/test_api.py` & `deepllm-1.5.1/deepllm/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.0/deepllm/tests/test_embedders.py` & `deepllm-1.5.1/deepllm/tests/test_embedders.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.0/deepllm/tests/test_recursors.py` & `deepllm-1.5.1/deepllm/tests/test_recursors.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.0/deepllm/tests/test_refiners.py` & `deepllm-1.5.1/deepllm/tests/test_refiners.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.0/deepllm/tools.py` & `deepllm-1.5.1/deepllm/tools.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.0/deepllm/vis.py` & `deepllm-1.5.1/deepllm/vis.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.0/deepllm.egg-info/PKG-INFO` & `deepllm-1.5.1/deepllm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepllm
-Version: 1.5.0
+Version: 1.5.1
 Summary: Deep, recursive, goal-driven LLM explorer
 Home-page: https://github.com/ptarau/recursors.git
 Author: Paul Tarau
 Author-email: paul.tarau@gmail.com
 License: GPL-3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `deepllm-1.5.0/deepllm.egg-info/SOURCES.txt` & `deepllm-1.5.1/deepllm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepllm-1.5.0/setup.py` & `deepllm-1.5.1/setup.py`

 * *Files identical despite different names*

