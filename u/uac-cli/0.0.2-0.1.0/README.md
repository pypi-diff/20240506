# Comparing `tmp/uac-cli-0.0.2.tar.gz` & `tmp/uac-cli-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uac-cli-0.0.2.tar", last modified: Sat May  4 05:46:02 2024, max compression
+gzip compressed data, was "uac-cli-0.1.0.tar", last modified: Sun May  5 22:53:30 2024, max compression
```

## Comparing `uac-cli-0.0.2.tar` & `uac-cli-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,58 @@
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-04 05:46:02.643201 uac-cli-0.0.2/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      476 2024-05-04 05:46:02.643016 uac-cli-0.0.2/PKG-INFO
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       66 2024-04-26 03:43:37.000000 uac-cli-0.0.2/README.md
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-26 03:38:30.000000 uac-cli-0.0.2/pyproject.toml
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       38 2024-05-04 05:46:02.643242 uac-cli-0.0.2/setup.cfg
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1233 2024-04-26 06:07:27.000000 uac-cli-0.0.2/setup.py
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-04 05:46:02.640403 uac-cli-0.0.2/uac_cli/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       21 2024-05-01 16:03:14.000000 uac-cli-0.0.2/uac_cli/__init__.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)   129020 2024-05-03 20:46:53.000000 uac-cli-0.0.2/uac_cli/uac.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1939 2024-05-01 07:02:37.000000 uac-cli-0.0.2/uac_cli/utils.py
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-04 05:46:02.642696 uac-cli-0.0.2/uac_cli.egg-info/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      476 2024-05-04 05:46:02.000000 uac-cli-0.0.2/uac_cli.egg-info/PKG-INFO
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      273 2024-05-04 05:46:02.000000 uac-cli-0.0.2/uac_cli.egg-info/SOURCES.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        1 2024-05-04 05:46:02.000000 uac-cli-0.0.2/uac_cli.egg-info/dependency_links.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       40 2024-05-04 05:46:02.000000 uac-cli-0.0.2/uac_cli.egg-info/entry_points.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       96 2024-05-04 05:46:02.000000 uac-cli-0.0.2/uac_cli.egg-info/requires.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        8 2024-05-04 05:46:02.000000 uac-cli-0.0.2/uac_cli.egg-info/top_level.txt
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-05 22:53:30.390833 uac-cli-0.1.0/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    10667 2024-05-05 22:53:30.390587 uac-cli-0.1.0/PKG-INFO
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    10256 2024-05-05 22:51:52.000000 uac-cli-0.1.0/README.md
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-26 03:38:30.000000 uac-cli-0.1.0/pyproject.toml
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       38 2024-05-05 22:53:30.390888 uac-cli-0.1.0/setup.cfg
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1256 2024-05-05 22:48:41.000000 uac-cli-0.1.0/setup.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-05 22:53:30.369281 uac-cli-0.1.0/uac_cli/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       21 2024-05-05 22:52:20.000000 uac-cli-0.1.0/uac_cli/__init__.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-05 22:53:30.388217 uac-cli-0.1.0/uac_cli/commands/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-05 17:55:51.000000 uac-cli-0.1.0/uac_cli/commands/__init__.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5200 2024-05-05 18:06:52.000000 uac-cli-0.1.0/uac_cli/commands/agent.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5924 2024-05-05 18:08:29.000000 uac-cli-0.1.0/uac_cli/commands/agent_cluster.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      857 2024-05-05 18:19:43.000000 uac-cli-0.1.0/uac_cli/commands/audit.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     8955 2024-05-05 18:23:19.000000 uac-cli-0.1.0/uac_cli/commands/bundle.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2849 2024-05-05 18:20:29.000000 uac-cli-0.1.0/uac_cli/commands/business_service.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5107 2024-05-05 18:20:47.000000 uac-cli-0.1.0/uac_cli/commands/calendar.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1106 2024-05-05 18:21:02.000000 uac-cli-0.1.0/uac_cli/commands/cluster_node.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2143 2024-05-05 22:45:19.000000 uac-cli-0.1.0/uac_cli/commands/config.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    11376 2024-05-05 18:32:10.000000 uac-cli-0.1.0/uac_cli/commands/connection.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3688 2024-05-05 18:21:16.000000 uac-cli-0.1.0/uac_cli/commands/credential.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3268 2024-05-05 18:21:37.000000 uac-cli-0.1.0/uac_cli/commands/custom_day.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2784 2024-05-05 18:22:02.000000 uac-cli-0.1.0/uac_cli/commands/email_template.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1409 2024-05-05 18:22:13.000000 uac-cli-0.1.0/uac_cli/commands/ldap.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      695 2024-05-05 18:41:31.000000 uac-cli-0.1.0/uac_cli/commands/metric.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2809 2024-05-05 18:22:39.000000 uac-cli-0.1.0/uac_cli/commands/oauth_client.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2878 2024-05-05 18:22:58.000000 uac-cli-0.1.0/uac_cli/commands/oms_server.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1484 2024-05-05 18:23:54.000000 uac-cli-0.1.0/uac_cli/commands/property.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      897 2024-05-05 18:24:18.000000 uac-cli-0.1.0/uac_cli/commands/report.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2382 2024-05-05 18:24:34.000000 uac-cli-0.1.0/uac_cli/commands/script.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1075 2024-05-05 18:24:50.000000 uac-cli-0.1.0/uac_cli/commands/server_operation.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2848 2024-05-05 18:25:03.000000 uac-cli-0.1.0/uac_cli/commands/simulation.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      665 2024-05-05 22:30:41.000000 uac-cli-0.1.0/uac_cli/commands/system.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     8273 2024-05-05 18:26:39.000000 uac-cli-0.1.0/uac_cli/commands/task.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    17677 2024-05-05 18:25:56.000000 uac-cli-0.1.0/uac_cli/commands/task_instance.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6121 2024-05-05 22:53:03.000000 uac-cli-0.1.0/uac_cli/commands/trigger.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1396 2024-05-05 18:28:59.000000 uac-cli-0.1.0/uac_cli/commands/universal_event.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2939 2024-05-05 18:28:56.000000 uac-cli-0.1.0/uac_cli/commands/universal_event_template.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6110 2024-05-05 18:29:19.000000 uac-cli-0.1.0/uac_cli/commands/universal_template.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4487 2024-05-05 18:29:46.000000 uac-cli-0.1.0/uac_cli/commands/user.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2533 2024-05-05 18:29:32.000000 uac-cli-0.1.0/uac_cli/commands/user_group.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3308 2024-05-05 18:30:07.000000 uac-cli-0.1.0/uac_cli/commands/variable.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3504 2024-05-05 18:30:22.000000 uac-cli-0.1.0/uac_cli/commands/virtual_resource.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4000 2024-05-05 18:30:39.000000 uac-cli-0.1.0/uac_cli/commands/webhook.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4934 2024-05-05 18:30:54.000000 uac-cli-0.1.0/uac_cli/commands/workflow.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4761 2024-05-05 22:31:55.000000 uac-cli-0.1.0/uac_cli/main.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6236 2024-05-05 20:12:30.000000 uac-cli-0.1.0/uac_cli/uac.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-05 22:53:30.390215 uac-cli-0.1.0/uac_cli/utils/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-05 17:56:14.000000 uac-cli-0.1.0/uac_cli/utils/__init__.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2922 2024-05-05 22:04:40.000000 uac-cli-0.1.0/uac_cli/utils/config.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      460 2024-05-05 18:06:43.000000 uac-cli-0.1.0/uac_cli/utils/options.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1939 2024-05-05 17:56:49.000000 uac-cli-0.1.0/uac_cli/utils/process.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-05 22:53:30.371931 uac-cli-0.1.0/uac_cli.egg-info/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    10667 2024-05-05 22:53:30.000000 uac-cli-0.1.0/uac_cli.egg-info/PKG-INFO
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1448 2024-05-05 22:53:30.000000 uac-cli-0.1.0/uac_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        1 2024-05-05 22:53:30.000000 uac-cli-0.1.0/uac_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       41 2024-05-05 22:53:30.000000 uac-cli-0.1.0/uac_cli.egg-info/entry_points.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      103 2024-05-05 22:53:30.000000 uac-cli-0.1.0/uac_cli.egg-info/requires.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        8 2024-05-05 22:53:30.000000 uac-cli-0.1.0/uac_cli.egg-info/top_level.txt
```

### Comparing `uac-cli-0.0.2/setup.py` & `uac-cli-0.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,21 +14,22 @@
         include_package_data=True,
         install_requires=[
             "uac-api",
             "colorama >= 0.4.4",
             "setuptools >= 44.1.1",
             "python-dotenv == 1.0.1",
             "click == 8.1.6",
-            "jsonpath-ng == 1.5.3"
+            "jsonpath-ng == 1.5.3",
+            "PyYAML"
         ],
         author='Stonebranch',
         description='A CLI tool for executing commands against the Stonebranch UAC API',
         entry_points={
             'console_scripts': [
-                'uac=uac_cli.uac:run'
+                'uac=uac_cli.main:run'
             ]
         },
         python_requires='>=3.7',
         classifiers=[
             "Programming Language :: Python :: 3",
             "License :: OSI Approved :: MIT License",
             "Operating System :: OS Independent",
```

### Comparing `uac-cli-0.0.2/uac_cli/utils.py` & `uac-cli-0.1.0/uac_cli/utils/process.py`

 * *Files identical despite different names*

