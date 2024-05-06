# Comparing `tmp/uac-api-0.3.1.tar.gz` & `tmp/uac-api-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uac-api-0.3.1.tar", last modified: Fri Apr 26 03:37:10 2024, max compression
+gzip compressed data, was "uac-api-0.4.0.tar", last modified: Mon May  6 14:27:59 2024, max compression
```

## Comparing `uac-api-0.3.1.tar` & `uac-api-0.4.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-26 03:37:10.430240 uac-api-0.3.1/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    17900 2024-04-26 03:37:10.430027 uac-api-0.3.1/PKG-INFO
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    17463 2024-04-26 03:34:02.000000 uac-api-0.3.1/README.md
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-26 03:33:40.000000 uac-api-0.3.1/pyproject.toml
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       38 2024-04-26 03:37:10.430280 uac-api-0.3.1/setup.cfg
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      973 2024-04-26 03:36:03.000000 uac-api-0.3.1/setup.py
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-26 03:37:10.427952 uac-api-0.3.1/uac_api/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     7184 2024-04-26 03:36:24.000000 uac-api-0.3.1/uac_api/__init__.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     8745 2024-04-26 03:33:40.000000 uac-api-0.3.1/uac_api/agents.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1192 2024-04-26 03:33:40.000000 uac-api-0.3.1/uac_api/audits.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    10234 2024-04-26 03:33:40.000000 uac-api-0.3.1/uac_api/bundles.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2068 2024-04-26 03:33:40.000000 uac-api-0.3.1/uac_api/business_services.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4997 2024-04-26 03:33:40.000000 uac-api-0.3.1/uac_api/calendars.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      402 2024-04-26 03:33:40.000000 uac-api-0.3.1/uac_api/cluster_nodes.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     8909 2024-04-26 03:33:40.000000 uac-api-0.3.1/uac_api/connections.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2953 2024-04-26 03:33:40.000000 uac-api-0.3.1/uac_api/credentials.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3398 2024-04-26 03:33:40.000000 uac-api-0.3.1/uac_api/custom_days.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1851 2024-04-26 03:33:40.000000 uac-api-0.3.1/uac_api/email_templates.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      536 2024-04-26 03:33:40.000000 uac-api-0.3.1/uac_api/ldap.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      216 2024-04-26 03:33:40.000000 uac-api-0.3.1/uac_api/metrics.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2059 2024-04-26 03:33:40.000000 uac-api-0.3.1/uac_api/oauth_clients.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1891 2024-04-26 03:33:40.000000 uac-api-0.3.1/uac_api/oms_servers.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3257 2024-04-26 03:33:40.000000 uac-api-0.3.1/uac_api/payload.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      818 2024-04-26 03:33:40.000000 uac-api-0.3.1/uac_api/properties.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      669 2024-04-26 03:33:40.000000 uac-api-0.3.1/uac_api/reports.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1746 2024-04-26 03:33:40.000000 uac-api-0.3.1/uac_api/scripts.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      722 2024-04-26 03:33:40.000000 uac-api-0.3.1/uac_api/server_operations.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2571 2024-04-26 03:33:40.000000 uac-api-0.3.1/uac_api/simulations.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      305 2024-04-26 03:33:40.000000 uac-api-0.3.1/uac_api/system.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    43174 2024-04-26 03:33:40.000000 uac-api-0.3.1/uac_api/task_instances.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    21888 2024-04-26 03:33:40.000000 uac-api-0.3.1/uac_api/tasks.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5587 2024-04-26 03:33:40.000000 uac-api-0.3.1/uac_api/triggers.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2471 2024-04-26 03:33:40.000000 uac-api-0.3.1/uac_api/universal_event_templates.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2233 2024-04-26 03:33:40.000000 uac-api-0.3.1/uac_api/universal_events.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4942 2024-04-26 03:33:40.000000 uac-api-0.3.1/uac_api/universal_templates.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1760 2024-04-26 03:33:40.000000 uac-api-0.3.1/uac_api/user_groups.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4091 2024-04-26 03:33:40.000000 uac-api-0.3.1/uac_api/users.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4588 2024-04-26 03:33:40.000000 uac-api-0.3.1/uac_api/utils.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3787 2024-04-26 03:33:40.000000 uac-api-0.3.1/uac_api/variables.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3208 2024-04-26 03:33:40.000000 uac-api-0.3.1/uac_api/virtual_resources.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4221 2024-04-26 03:33:40.000000 uac-api-0.3.1/uac_api/webhooks.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6115 2024-04-26 03:33:40.000000 uac-api-0.3.1/uac_api/workflows.py
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-26 03:37:10.429705 uac-api-0.3.1/uac_api.egg-info/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    17900 2024-04-26 03:37:10.000000 uac-api-0.3.1/uac_api.egg-info/PKG-INFO
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      972 2024-04-26 03:37:10.000000 uac-api-0.3.1/uac_api.egg-info/SOURCES.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        1 2024-04-26 03:37:10.000000 uac-api-0.3.1/uac_api.egg-info/dependency_links.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        9 2024-04-26 03:37:10.000000 uac-api-0.3.1/uac_api.egg-info/requires.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        8 2024-04-26 03:37:10.000000 uac-api-0.3.1/uac_api.egg-info/top_level.txt
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-06 14:27:59.695315 uac-api-0.4.0/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    18579 2024-05-06 14:27:59.695101 uac-api-0.4.0/PKG-INFO
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    18142 2024-05-04 05:41:22.000000 uac-api-0.4.0/README.md
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-26 03:33:40.000000 uac-api-0.4.0/pyproject.toml
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       38 2024-05-06 14:27:59.695364 uac-api-0.4.0/setup.cfg
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      985 2024-05-04 04:48:08.000000 uac-api-0.4.0/setup.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-06 14:27:59.692700 uac-api-0.4.0/uac_api/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     8136 2024-05-05 22:43:42.000000 uac-api-0.4.0/uac_api/__init__.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9357 2024-04-29 16:35:47.000000 uac-api-0.4.0/uac_api/agents.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1192 2024-04-26 03:33:40.000000 uac-api-0.4.0/uac_api/audits.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    10489 2024-04-29 13:49:08.000000 uac-api-0.4.0/uac_api/bundles.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2107 2024-04-29 17:20:04.000000 uac-api-0.4.0/uac_api/business_services.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4997 2024-04-26 03:33:40.000000 uac-api-0.4.0/uac_api/calendars.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      402 2024-04-26 03:33:40.000000 uac-api-0.4.0/uac_api/cluster_nodes.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9129 2024-04-29 13:50:56.000000 uac-api-0.4.0/uac_api/connections.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3014 2024-04-29 18:48:08.000000 uac-api-0.4.0/uac_api/credentials.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3442 2024-04-30 02:41:31.000000 uac-api-0.4.0/uac_api/custom_days.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1895 2024-04-29 13:46:36.000000 uac-api-0.4.0/uac_api/email_templates.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      558 2024-04-29 13:47:11.000000 uac-api-0.4.0/uac_api/ldap.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      238 2024-04-29 18:58:01.000000 uac-api-0.4.0/uac_api/metrics.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2103 2024-04-29 13:47:38.000000 uac-api-0.4.0/uac_api/oauth_clients.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1935 2024-04-29 13:48:02.000000 uac-api-0.4.0/uac_api/oms_servers.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    10301 2024-05-03 20:22:47.000000 uac-api-0.4.0/uac_api/payload.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1107 2024-05-01 04:54:15.000000 uac-api-0.4.0/uac_api/properties.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1375 2024-05-01 05:59:17.000000 uac-api-0.4.0/uac_api/reports.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1790 2024-04-29 13:50:06.000000 uac-api-0.4.0/uac_api/scripts.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      722 2024-04-26 03:33:40.000000 uac-api-0.4.0/uac_api/server_operations.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2615 2024-04-29 13:50:28.000000 uac-api-0.4.0/uac_api/simulations.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      305 2024-04-26 03:33:40.000000 uac-api-0.4.0/uac_api/system.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    45039 2024-05-03 19:21:36.000000 uac-api-0.4.0/uac_api/task_instances.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9639 2024-05-03 20:22:58.000000 uac-api-0.4.0/uac_api/tasks.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6774 2024-05-01 07:18:22.000000 uac-api-0.4.0/uac_api/triggers.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2493 2024-04-29 13:52:45.000000 uac-api-0.4.0/uac_api/universal_event_templates.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2233 2024-04-26 03:33:40.000000 uac-api-0.4.0/uac_api/universal_events.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4986 2024-04-29 13:53:10.000000 uac-api-0.4.0/uac_api/universal_templates.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1804 2024-04-29 13:53:42.000000 uac-api-0.4.0/uac_api/user_groups.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4312 2024-05-01 04:31:22.000000 uac-api-0.4.0/uac_api/users.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     7831 2024-05-05 22:44:01.000000 uac-api-0.4.0/uac_api/utils.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3831 2024-04-29 13:54:30.000000 uac-api-0.4.0/uac_api/variables.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3378 2024-05-01 06:36:43.000000 uac-api-0.4.0/uac_api/virtual_resources.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4287 2024-04-29 13:55:16.000000 uac-api-0.4.0/uac_api/webhooks.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    10350 2024-05-04 05:17:55.000000 uac-api-0.4.0/uac_api/workflows.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-06 14:27:59.694767 uac-api-0.4.0/uac_api.egg-info/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    18579 2024-05-06 14:27:59.000000 uac-api-0.4.0/uac_api.egg-info/PKG-INFO
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      972 2024-05-06 14:27:59.000000 uac-api-0.4.0/uac_api.egg-info/SOURCES.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        1 2024-05-06 14:27:59.000000 uac-api-0.4.0/uac_api.egg-info/dependency_links.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       18 2024-05-06 14:27:59.000000 uac-api-0.4.0/uac_api.egg-info/requires.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        8 2024-05-06 14:27:59.000000 uac-api-0.4.0/uac_api.egg-info/top_level.txt
```

### Comparing `uac-api-0.3.1/PKG-INFO` & `uac-api-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uac-api
-Version: 0.3.1
+Version: 0.4.0
 Summary: A Python wrapper for the Stonebranch UAC API
 Home-page: https://github.com/gomleksiz/uac-api
 Author: Stonebranch
 Author-email: huseyim@gmail.com
 License: CC BY-NC 4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -21,14 +21,16 @@
 - **Comprehensive API Coverage**: Enables interaction with a wide array of Stonebranch UAC functionalities through Python functions.
 - **Enhanced Task Management**: Simplify the creation, management, and monitoring of tasks and workflows.
 - **Agent and Cluster Operations**: Manage agents and agent clusters with functions for updates, deletions, and status checks.
 - **Advanced Scheduling Capabilities**: Utilize calendars, custom days, and triggers to precisely schedule tasks.
 - **Resource Management**: Handle connections, credentials, properties, and variables for full control over your automation environment.
 - **Audit and Reporting**: Access audit logs and generate reports for detailed insights into your automation activities.
 - **Customization and Extension**: Manage custom days, email templates, scripts, and more, allowing for extensive customization and functionality extension.
+- **Download Reports**: Download report in CSV, TSV, JSON, XML and PDF formats.
+
 
 ## Installation
 
 ```bash
 pip install uac-api
 ```
 
@@ -220,18 +222,18 @@
 - get_oms_server(self, query=None, **args)
 - update_oms_server(self, payload=None, **args)
 - create_oms_server(self, payload=None, **args)
 - delete_oms_server(self, query=None, **args)
 - list_oms_servers(self)
 ## Properties:
 - get_property(self, query=None, **args)
-- update_property(self, payload=None, **args)
+- update_property(self, payload=None, query=None, **args)
 - list_properties(self)
 ## Reports:
-- run_report(self, query=None, **args)
+- run_report(self, query=None, report_format="csv", **args)
 ## Scripts:
 - get_script(self, query=None, **args)
 - update_script(self, payload=None, **args)
 - create_script(self, payload=None, **args)
 - delete_script(self, query=None, **args)
 - list_scripts(self)
 ## ServerOperations:
@@ -267,14 +269,15 @@
 - task_instance_rerun(self, payload=None, **args)
 - task_instance_retrieve_output(self, query=None, **args)
 - task_instance_skip(self, payload=None, **args)
 - task_instance_skip_path(self, payload=None, **args)
 - task_instance_unskip(self, payload=None, **args)
 - list_status(self, payload=None, **args) - List Task Instances
 - wait_for_status(self, id, statuses=FINAL_STATUS, timeout=300, interval=10): Waits until the task instance reaches one of the given statuses.
+- set_complete(self, payload=None, **args)
 ## Tasks:
 - get_task(self, query=None, **args)
 - update_task(self, payload=None, **args)
 - create_task(self, payload=None, **args)
 - clone_task(self, task_name, new_task_name): Copy task with a new name
 - delete_task(self, query=None, **args)
 - list_tasks(self, payload=None, **args)
@@ -287,24 +290,29 @@
 - task_clear_timewait(self, payload=None, **args)
 - task_create_with_properties(self, payload=None, **args)
 - list_dependency_list_1(self, query=None, **args)
 - task_insert_1(self, payload=None, **args)
 - task_launch(self, payload=None, **args)
 - task_release(self, payload=None, **args)
 - task_set_timewait(self, payload=None, **args)
+- create_linux_task(self, name, agent, payload=None, command=None, script=None)
+- create_windows_task(self, name, agent, payload=None, command=None, script=None)
+- create_workflow(self, name, payload=None)
 ## Triggers:
 - list_qualifying_times(self, query=None, **args)
+- assign_execution_user_to_trigger(self, query=None, payload=None, **args)
 - unassign_execution_user(self, payload=None, **args)
 - create_temp_trigger(self, payload=None, **args)
 - get_trigger(self, query=None, **args)
 - update_trigger(self, payload=None, **args)
 - create_trigger(self, payload=None, **args)
 - delete_trigger(self, query=None, **args)
 - list_triggers(self, payload=None, **args)
 - list_triggers_advanced(self, query=None, **args)
+- enable_disable(self, payload=None, **args)
 ## UniversalEventTemplates:
 - get_universal_event_template(self, query=None, **args)
 - update_universal_event_template(self, payload=None, **args)
 - create_universal_event_template(self, payload=None, **args)
 - delete_universal_event_template(self, query=None, **args)
 - list_universal_event_templates(self, query=None, **args)
 ## UniversalEvents:
@@ -369,14 +377,16 @@
 - add_edge(self, payload=None, **args)
 - delete_edge(self, query=None, **args)
 - get_vertices(self, query=None, **args)
 - update_vertex(self, payload=None, **args)
 - add_vertex(self, payload=None, **args)
 - delete_vertices(self, query=None, **args)
 - get_forecast(self, query=None, **args)
+- add_child_vertex(self, workflow_name, task_name, parent_task_name=None, parent_vertex_id=None, vertex_id=None, auto_arrange=True)
+- auto_arrange_vertices(self, workflow_name=None, payload=None)
 
 # Classes
 - Agents
 - AgentClusters
 - Audits
 - Bundles
 - Calendars
```

### Comparing `uac-api-0.3.1/README.md` & `uac-api-0.4.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 - **Comprehensive API Coverage**: Enables interaction with a wide array of Stonebranch UAC functionalities through Python functions.
 - **Enhanced Task Management**: Simplify the creation, management, and monitoring of tasks and workflows.
 - **Agent and Cluster Operations**: Manage agents and agent clusters with functions for updates, deletions, and status checks.
 - **Advanced Scheduling Capabilities**: Utilize calendars, custom days, and triggers to precisely schedule tasks.
 - **Resource Management**: Handle connections, credentials, properties, and variables for full control over your automation environment.
 - **Audit and Reporting**: Access audit logs and generate reports for detailed insights into your automation activities.
 - **Customization and Extension**: Manage custom days, email templates, scripts, and more, allowing for extensive customization and functionality extension.
+- **Download Reports**: Download report in CSV, TSV, JSON, XML and PDF formats.
+
 
 ## Installation
 
 ```bash
 pip install uac-api
 ```
 
@@ -206,18 +208,18 @@
 - get_oms_server(self, query=None, **args)
 - update_oms_server(self, payload=None, **args)
 - create_oms_server(self, payload=None, **args)
 - delete_oms_server(self, query=None, **args)
 - list_oms_servers(self)
 ## Properties:
 - get_property(self, query=None, **args)
-- update_property(self, payload=None, **args)
+- update_property(self, payload=None, query=None, **args)
 - list_properties(self)
 ## Reports:
-- run_report(self, query=None, **args)
+- run_report(self, query=None, report_format="csv", **args)
 ## Scripts:
 - get_script(self, query=None, **args)
 - update_script(self, payload=None, **args)
 - create_script(self, payload=None, **args)
 - delete_script(self, query=None, **args)
 - list_scripts(self)
 ## ServerOperations:
@@ -253,14 +255,15 @@
 - task_instance_rerun(self, payload=None, **args)
 - task_instance_retrieve_output(self, query=None, **args)
 - task_instance_skip(self, payload=None, **args)
 - task_instance_skip_path(self, payload=None, **args)
 - task_instance_unskip(self, payload=None, **args)
 - list_status(self, payload=None, **args) - List Task Instances
 - wait_for_status(self, id, statuses=FINAL_STATUS, timeout=300, interval=10): Waits until the task instance reaches one of the given statuses.
+- set_complete(self, payload=None, **args)
 ## Tasks:
 - get_task(self, query=None, **args)
 - update_task(self, payload=None, **args)
 - create_task(self, payload=None, **args)
 - clone_task(self, task_name, new_task_name): Copy task with a new name
 - delete_task(self, query=None, **args)
 - list_tasks(self, payload=None, **args)
@@ -273,24 +276,29 @@
 - task_clear_timewait(self, payload=None, **args)
 - task_create_with_properties(self, payload=None, **args)
 - list_dependency_list_1(self, query=None, **args)
 - task_insert_1(self, payload=None, **args)
 - task_launch(self, payload=None, **args)
 - task_release(self, payload=None, **args)
 - task_set_timewait(self, payload=None, **args)
+- create_linux_task(self, name, agent, payload=None, command=None, script=None)
+- create_windows_task(self, name, agent, payload=None, command=None, script=None)
+- create_workflow(self, name, payload=None)
 ## Triggers:
 - list_qualifying_times(self, query=None, **args)
+- assign_execution_user_to_trigger(self, query=None, payload=None, **args)
 - unassign_execution_user(self, payload=None, **args)
 - create_temp_trigger(self, payload=None, **args)
 - get_trigger(self, query=None, **args)
 - update_trigger(self, payload=None, **args)
 - create_trigger(self, payload=None, **args)
 - delete_trigger(self, query=None, **args)
 - list_triggers(self, payload=None, **args)
 - list_triggers_advanced(self, query=None, **args)
+- enable_disable(self, payload=None, **args)
 ## UniversalEventTemplates:
 - get_universal_event_template(self, query=None, **args)
 - update_universal_event_template(self, payload=None, **args)
 - create_universal_event_template(self, payload=None, **args)
 - delete_universal_event_template(self, query=None, **args)
 - list_universal_event_templates(self, query=None, **args)
 ## UniversalEvents:
@@ -355,14 +363,16 @@
 - add_edge(self, payload=None, **args)
 - delete_edge(self, query=None, **args)
 - get_vertices(self, query=None, **args)
 - update_vertex(self, payload=None, **args)
 - add_vertex(self, payload=None, **args)
 - delete_vertices(self, query=None, **args)
 - get_forecast(self, query=None, **args)
+- add_child_vertex(self, workflow_name, task_name, parent_task_name=None, parent_vertex_id=None, vertex_id=None, auto_arrange=True)
+- auto_arrange_vertices(self, workflow_name=None, payload=None)
 
 # Classes
 - Agents
 - AgentClusters
 - Audits
 - Bundles
 - Calendars
```

### Comparing `uac-api-0.3.1/setup.py` & `uac-api-0.4.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         version=version,
         author_email="huseyim@gmail.com",
         license="CC BY-NC 4.0",
         url="https://github.com/gomleksiz/uac-api",
         packages=find_packages(),
         include_package_data=True,
         install_requires=[
-            "requests"
+            "requests", "networkx"
         ],
         author='Stonebranch',
         description='A Python wrapper for the Stonebranch UAC API',
         python_requires='>=3.7',
         classifiers=[
             "Programming Language :: Python :: 3",
             "License :: OSI Approved :: MIT License",
```

### Comparing `uac-api-0.3.1/uac_api/__init__.py` & `uac-api-0.4.0/uac_api/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import requests
 import sys
 import json
+import re
 
 from .server_operations import ServerOperations
 from .metrics import Metrics
 from .audits import Audits
 from .system import System
 from .ldap import Ldaps
 from .tasks import Tasks
@@ -31,36 +32,41 @@
 from .user_groups import UserGroups
 from .webhooks import Webhooks
 from .cluster_nodes import ClusterNodes
 from .email_templates import EmailTemplates
 from .oauth_clients import OAuthClients
 from .calendars import Calendars
 from .universal_templates import UniversalTemplates
-from .utils import strip_url
+from .utils import strip_url, filter_secrets
 import logging
 
-__version__ = "0.3.1"
+__version__ = "0.4.0"
 
 class UniversalController():
     def __init__(self, base_url, credential=None, token=None, ssl_verify=True, logger=None, headers=None) -> None:
         if logger is None:
             logger = logging.getLogger(__name__)
             logger.setLevel(logging.INFO)
             logger.addHandler(logging.StreamHandler())
             self.log = logger
         else:
             self.log = logger
         self.base_url = strip_url(base_url)
         self.token = token
         self.ssl_verify = ssl_verify
         self.cridential = credential
+        self.secrets = []
+        if token:
+            self.secrets.append(token)
+        else:
+            self.secrets.append(credential[1])
         if headers:
             self.headers = headers
         else:
-            self.headers = {"content-type": "application/json"}
+            self.headers = {"content-type": "application/json", "accept": "application/json"}
         self.server_operations = ServerOperations(self)
         self.metrics = Metrics(self)
         self.audits = Audits(self)
         self.system = System(self)
         self.ldap = Ldaps(self)
         self.tasks = Tasks(self)
         self.triggers = Triggers(self)
@@ -101,49 +107,51 @@
     def get(self, resource, query="", headers=None, parse_response=True):
         return self.call("GET", resource, query, headers, json_data=None, parse_response=parse_response)
 
     def delete(self, resource, query="", json_data=None, headers=None, parse_response=True):
         return self.call("DELETE", resource, query, headers, json_data, parse_response)
 
     def call(self, method, resource, query, headers, json_data, parse_response):
-        self.log.debug("uac_rest_call start")
+        self.log.debug(filter_secrets("uac_rest_call start", self.secrets))
         if headers:
             _headers = headers
         else:
             _headers = self.headers
         
         if self.token:
-            self.headers["Authorization"] = f"Bearer {self.token}"
+            _headers["Authorization"] = f"Bearer {self.token}"
 
+        self.log.debug(filter_secrets(f"HEADERS => {_headers}", self.secrets))
         if len(query) > 0:
             query = "?" + "&".join(query)
         else:
             query = ""
         uri = f"{self.base_url}{resource}{query}"
         self.log.info(f"URL = {uri}")
         try:
             if method == "GET":
                 response = requests.get(uri,
                                         headers=_headers,
                                         auth=self.cridential,
                                         verify=self.ssl_verify)
             elif method == "POST":
-                self.log.debug(f"Payload = {json_data}")
+                self.log.debug(filter_secrets(f"Payload = {json_data}", self.secrets))
                 response = requests.post(uri,
                                         headers=_headers,
                                         auth=self.cridential,
                                         json=json_data,
                                         verify=self.ssl_verify)
             elif method == "DELETE":
                 response = requests.delete(uri,
                                         headers=_headers,
                                         auth=self.cridential,
                                         json=json_data,
                                         verify=self.ssl_verify)
             elif method == "PUT":
+                self.log.debug(filter_secrets(f"Payload = {json_data}", self.secrets))
                 response = requests.put(uri,
                                         headers=_headers,
                                         auth=self.cridential,
                                         json=json_data,
                                         verify=self.ssl_verify)
             else:
                 self.log.error(f"Unknown method {method}")
@@ -152,29 +160,36 @@
             self.log.error(f"Error Calling{self.base_url} API {sys.exc_info()}")
             raise
         if response.ok:
             pass
         else:
             self.log.error(f"{uri} Response Code : {response.status_code}")
             self.log.error(f"Failed with reason : {response.text}")
+            response.raise_for_status()
             response = None
-            raise
         # if response:
-        #     self.log.debug("response: " + response.text)
+        #     self.log.debug(filter_secrets("response: " + response.text, self.secrets))
         resp_data = None
         try:
             if parse_response:
                 resp_data = response.json()
-                self.log.debug("received data: %s..." % json.dumps(resp_data))
+                self.log.debug(filter_secrets("received data: %s..." % json.dumps(resp_data), self.secrets))
             else:
-                resp_data = response.text
-                self.log.debug("received data: %s..." % resp_data)
+                resp_data = {"response": response.text}
+                # Match anything like UUID: 0f2bd3ea0fc34da08bb668ccceee8c5a
+                matched = re.search(r"([0-9a-f]{32})", response.text)
+                if matched:
+                    resp_data["sys_id"] = matched.group(0)
+
+                self.log.debug(filter_secrets("received data: %s..." % resp_data, self.secrets))
         except Exception as unknown_exception:
             # no XML returned
             self.log.error("Couldn't parse the response.")
             resp_data = response.text
-        self.log.debug("received data: %s..." % json.dumps(resp_data)[0:10])
-        self.log.debug("uac_rest_call end")
+        # self.log.debug(filter_secrets("received data: %s..." % json.dumps(resp_data)[0:10], self.secrets))
+        self.log.debug(filter_secrets("uac_rest_call end", self.secrets))
+        if _headers.get("Accept") in ["application/pdf", "image/png"]:
+            return response.content
         return resp_data
```

### Comparing `uac-api-0.3.1/uac_api/agents.py` & `uac-api-0.4.0/uac_api/agents.py`

 * *Files 9% similar despite different names*

```diff
@@ -173,28 +173,28 @@
         }
         parameters = prepare_query_params(query, field_mapping, args)
         return self.uc.get(url, query=parameters)
     
     def update_agent_cluster(self, payload=None, **args):
         url="/resources/agentcluster"
         _payload = payload
-        return self.uc.put(url, json_data=_payload)
+        return self.uc.put(url, json_data=_payload, parse_response=False)
 
     def create_agent_cluster(self, payload=None, **args):
         '''
         Arguments:
         - retainSysIds: retainSysIds 
             False will ignore sysIds in the payload and create a new task  
         '''
         url="/resources/agentcluster"
         field_mapping={
           "retainSysIds": "retainSysIds", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
-        return self.uc.post(url, json_data=_payload)
+        return self.uc.post(url, json_data=_payload, parse_response=False)
 
     def delete_agent_cluster(self, query=None, **args):
         '''
         Arguments:
         - agentclusterid: agentclusterid 
         - agentclustername: agentclustername 
         '''
@@ -238,24 +238,38 @@
             "ignoreexecutionlimit": "ignoreexecutionlimit", 
         }
         parameters = prepare_query_params(query, field_mapping, args)
         return self.uc.get(url, query=parameters)
 
     def resolve_cluster(self, payload=None, **args):
         url="/resources/agentcluster/resolve"
-        _payload = payload
+        field_mapping={
+          "agentClusterName": "agentClusterName", 
+        }
+        _payload = prepare_payload(payload, field_mapping, args)
         return self.uc.post(url, json_data=_payload)
 
     def resume_cluster(self, payload=None, **args):
         url="/resources/agentcluster/resume"
-        _payload = payload
+        field_mapping={
+          "agentClusterName": "agentClusterName", 
+        }
+        _payload = prepare_payload(payload, field_mapping, args)
         return self.uc.post(url, json_data=_payload)
 
     def set_cluster_task_execution_limit(self, payload=None, **args):
         url="/resources/agentcluster/taskexecutionlimit"
-        _payload = payload
+        field_mapping={
+          "agentClusterName": "agentClusterName", 
+          "limitType": "limitType", 
+          "limitAmount": "limitAmount"
+        }
+        _payload = prepare_payload(payload, field_mapping, args)
         return self.uc.post(url, json_data=_payload)
 
     def suspend_cluster(self, payload=None, **args):
         url="/resources/agentcluster/suspend"
-        _payload = payload
+        field_mapping={
+          "agentClusterName": "agentClusterName", 
+        }
+        _payload = prepare_payload(payload, field_mapping, args)
         return self.uc.post(url, json_data=_payload)
```

### Comparing `uac-api-0.3.1/uac_api/audits.py` & `uac-api-0.4.0/uac_api/audits.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.3.1/uac_api/bundles.py` & `uac-api-0.4.0/uac_api/bundles.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # - create_promotion_target(target_data)
 # - modify_promotion_target(target_id, **kwargs)
 # - list_promotion_targets()
 # - delete_promotion_target(target_id)
 # - read_promotion_target(target_id)
 # - refresh_target_agents(target_id)
 
-from .utils import prepare_payload, prepare_query_params
+from .utils import prepare_payload, prepare_query_params, prepare_query_payload
 
 class Bundles:
     def __init__(self, uc):
         self.log = uc.log
         self.headers = uc.headers
         self.uc = uc
 
@@ -72,28 +72,28 @@
         }
         parameters = prepare_query_params(query, field_mapping, args)
         return self.uc.get(url, query=parameters)
 
     def update_bundle(self, payload=None, **args):
         url="/resources/bundle"
         _payload = payload
-        return self.uc.put(url, json_data=_payload)
+        return self.uc.put(url, json_data=_payload, parse_response=False)
 
     def create_bundle(self, payload=None, **args):
         '''
         Arguments:
         - retainSysIds: retainSysIds 
             False will ignore sysIds in the payload and create a new task  
         '''
         url="/resources/bundle"
         field_mapping={
           "retainSysIds": "retainSysIds", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
-        return self.uc.post(url, json_data=_payload)
+        return self.uc.post(url, json_data=_payload, parse_response=False)
 
     def delete_bundle(self, query=None, **args):
         '''
         Arguments:
         - bundleid: bundleid 
         - bundlename: bundlename 
         '''
@@ -112,15 +112,15 @@
             False will ignore sysIds in the payload and create a new task  
         '''
         url="/resources/bundle/{a}"
         field_mapping={
           "retainSysIds": "retainSysIds", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
-        return self.uc.post(url, json_data=_payload)
+        return self.uc.post(url, json_data=_payload, parse_response=False)
 
     def get_bundle_report(self, query=None, **args):
         '''
         Arguments:
         - bundleid: bundleid 
         - bundlename: bundlename 
         '''
@@ -235,28 +235,28 @@
         }
         parameters = prepare_query_params(query, field_mapping, args)
         return self.uc.get(url, query=parameters)
 
     def update_promotion_target(self, payload=None, **args):
         url="/resources/promotiontarget"
         _payload = payload
-        return self.uc.put(url, json_data=_payload)
+        return self.uc.put(url, json_data=_payload, parse_response=False)
 
     def create_promotion_target(self, payload=None, **args):
         '''
         Arguments:
         - retainSysIds: retainSysIds 
             False will ignore sysIds in the payload and create a new task  
         '''
         url="/resources/promotiontarget"
         field_mapping={
           "retainSysIds": "retainSysIds", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
-        return self.uc.post(url, json_data=_payload)
+        return self.uc.post(url, json_data=_payload, parse_response=False)
 
     def delete_promotion_target(self, query=None, **args):
         '''
         Arguments:
         - targetname: targetname 
         - targetid: targetid 
         '''
@@ -277,27 +277,29 @@
         url="/resources/promotiontarget/list"
         field_mapping={
             "targetname": "targetname", 
             "businessServices": "businessServices", 
         }
         parameters = prepare_query_params(query, field_mapping, args)
         return self.uc.get(url, query=parameters)
-
-    def refresh_target_agents(self, payload=None, **args):
+    
+    def refresh_target_agents(self, query=None, payload=None, **args):
         '''
         Arguments:
         - targetname: targetname 
         - targetid: targetid 
         - username: username 
         - password: password 
         - token: token 
         '''
         url="/resources/promotiontarget/refreshtargetagents"
-        field_mapping={
+        query_fields={
           "targetname": "targetname", 
           "targetid": "targetid", 
+        }
+        payload_fields={
           "username": "username", 
           "password": "password", 
           "token": "token", 
         }
-        _payload = prepare_payload(payload, field_mapping, args)
-        return self.uc.post(url, json_data=_payload)
+        _query, _payload = prepare_query_payload(query, query_fields, payload, payload_fields, args)
+        return self.uc.post(url, query=_query, json_data=_payload, parse_response=False)
```

### Comparing `uac-api-0.3.1/uac_api/business_services.py` & `uac-api-0.4.0/uac_api/business_services.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .utils import prepare_query_params
+from .utils import prepare_query_params, prepare_payload
 
 # - create_business_service(service_data)
 # - delete_business_service(service_id)
 # - modify_business_service(service_id, **kwargs)
 # - read_business_service(service_id)
 
 class BusinessServices:
@@ -24,15 +24,15 @@
         }
         parameters = prepare_query_params(query, field_mapping, args)
         return self.uc.get(url, query=parameters)
 
     def update_business_service(self, payload=None, **args):
         url="/resources/businessservice"
         _payload = payload
-        return self.uc.put(url, json_data=_payload)
+        return self.uc.put(url, json_data=_payload, parse_response=False)
 
     def create_business_service(self, payload=None, **args):
         '''
         Arguments:
         - retainSysIds: retainSysIds 
             False will ignore sysIds in the payload and create a new task  
         '''
```

### Comparing `uac-api-0.3.1/uac_api/calendars.py` & `uac-api-0.4.0/uac_api/calendars.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.3.1/uac_api/connections.py` & `uac-api-0.4.0/uac_api/connections.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,28 +26,28 @@
         }
         parameters = prepare_query_params(query, field_mapping, args)
         return self.uc.get(url, query=parameters)
 
     def update_database_connection(self, payload=None, **args):
         url="/resources/databaseconnection"
         _payload = payload
-        return self.uc.put(url, json_data=_payload)
+        return self.uc.put(url, json_data=_payload, parse_response=False)
 
     def create_database_connection(self, payload=None, **args):
         '''
         Arguments:
         - retainSysIds: retainSysIds 
             False will ignore sysIds in the payload and create a new task  
         '''
         url="/resources/databaseconnection"
         field_mapping={
           "retainSysIds": "retainSysIds", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
-        return self.uc.post(url, json_data=_payload)
+        return self.uc.post(url, json_data=_payload, parse_response=False)
 
     def delete_database_connection(self, query=None, **args):
         '''
         Arguments:
         - connectionid: connectionid 
         - connectionname: connectionname 
         '''
@@ -76,28 +76,28 @@
         }
         parameters = prepare_query_params(query, field_mapping, args)
         return self.uc.get(url, query=parameters)
 
     def update_email_connection(self, payload=None, **args):
         url="/resources/emailconnection"
         _payload = payload
-        return self.uc.put(url, json_data=_payload)
+        return self.uc.put(url, json_data=_payload, parse_response=False)
 
     def create_email_connection(self, payload=None, **args):
         '''
         Arguments:
         - retainSysIds: retainSysIds 
             False will ignore sysIds in the payload and create a new task  
         '''
         url="/resources/emailconnection"
         field_mapping={
           "retainSysIds": "retainSysIds", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
-        return self.uc.post(url, json_data=_payload)
+        return self.uc.post(url, json_data=_payload, parse_response=False)
 
     def delete_email_connection(self, query=None, **args):
         '''
         Arguments:
         - connectionid: connectionid 
         - connectionname: connectionname 
         '''
@@ -126,28 +126,28 @@
         }
         parameters = prepare_query_params(query, field_mapping, args)
         return self.uc.get(url, query=parameters)
 
     def update_peoplesoft_connection(self, payload=None, **args):
         url="/resources/peoplesoftconnection"
         _payload = payload
-        return self.uc.put(url, json_data=_payload)
+        return self.uc.put(url, json_data=_payload, parse_response=False)
 
     def create_peoplesoft_connection(self, payload=None, **args):
         '''
         Arguments:
         - retainSysIds: retainSysIds 
             False will ignore sysIds in the payload and create a new task  
         '''
         url="/resources/peoplesoftconnection"
         field_mapping={
           "retainSysIds": "retainSysIds", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
-        return self.uc.post(url, json_data=_payload)
+        return self.uc.post(url, json_data=_payload, parse_response=False)
 
     def delete_peoplesoft_connection(self, query=None, **args):
         '''
         Arguments:
         - connectionid: connectionid 
         - connectionname: connectionname 
         '''
@@ -176,28 +176,28 @@
         }
         parameters = prepare_query_params(query, field_mapping, args)
         return self.uc.get(url, query=parameters)
 
     def update_sap_connection(self, payload=None, **args):
         url="/resources/sapconnection"
         _payload = payload
-        return self.uc.put(url, json_data=_payload)
+        return self.uc.put(url, json_data=_payload, parse_response=False)
 
     def create_sap_connection(self, payload=None, **args):
         '''
         Arguments:
         - retainSysIds: retainSysIds 
             False will ignore sysIds in the payload and create a new task  
         '''
         url="/resources/sapconnection"
         field_mapping={
           "retainSysIds": "retainSysIds", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
-        return self.uc.post(url, json_data=_payload)
+        return self.uc.post(url, json_data=_payload, parse_response=False)
 
     def delete_sap_connection(self, query=None, **args):
         '''
         Arguments:
         - connectionid: connectionid 
         - connectionname: connectionname 
         '''
@@ -226,28 +226,28 @@
         }
         parameters = prepare_query_params(query, field_mapping, args)
         return self.uc.get(url, query=parameters)
 
     def update_snmp_connection(self, payload=None, **args):
         url="/resources/snmpmanager"
         _payload = payload
-        return self.uc.put(url, json_data=_payload)
+        return self.uc.put(url, json_data=_payload, parse_response=False)
 
     def create_snmp_connection(self, payload=None, **args):
         '''
         Arguments:
         - retainSysIds: retainSysIds 
             False will ignore sysIds in the payload and create a new task  
         '''
         url="/resources/snmpmanager"
         field_mapping={
           "retainSysIds": "retainSysIds", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
-        return self.uc.post(url, json_data=_payload)
+        return self.uc.post(url, json_data=_payload, parse_response=False)
 
     def delete_snmp_connection(self, query=None, **args):
         '''
         Arguments:
         - managerid: managerid 
         - managername: managername 
         '''
```

### Comparing `uac-api-0.3.1/uac_api/credentials.py` & `uac-api-0.4.0/uac_api/credentials.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,28 +39,28 @@
         }
         parameters = prepare_query_params(query, field_mapping, args)
         return self.uc.get(url, query=parameters)
 
     def update_credential(self, payload=None, **args):
         url="/resources/credential"
         _payload = payload
-        return self.uc.put(url, json_data=_payload)
+        return self.uc.put(url, json_data=_payload, parse_response=False)
 
     def create_credential(self, payload=None, **args):
         '''
         Arguments:
         - retainSysIds: retainSysIds 
             False will ignore sysIds in the payload and create a new task  
         '''
         url="/resources/credential"
         field_mapping={
           "retainSysIds": "retainSysIds", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
-        return self.uc.post(url, json_data=_payload)
+        return self.uc.post(url, json_data=_payload, parse_response=False)
 
     def delete_credential(self, query=None, **args):
         '''
         Arguments:
         - credentialid: credentialid 
         - credentialname: credentialname 
         '''
@@ -72,20 +72,20 @@
         parameters = prepare_query_params(query, field_mapping, args)
         return self.uc.delete(url, query=parameters, parse_response=False)
 
     def list_credentials(self):
         url="/resources/credential/list"
         return self.uc.get(url)
 
-    def test_provider(self, payload=None, **args):
+    def test_provider(self, query=None, **args):
         '''
         Arguments:
         - credentialid: credentialid 
         - credentialname: credentialname 
         '''
         url="/resources/credential/testprovider"
         field_mapping={
           "credentialid": "credentialid", 
           "credentialname": "credentialname", 
         }
-        _payload = prepare_payload(payload, field_mapping, args)
-        return self.uc.post(url, json_data=_payload)
+        parameters = prepare_query_params(query, field_mapping, args)
+        return self.uc.post(url, query=parameters, json_data=None)
```

### Comparing `uac-api-0.3.1/uac_api/custom_days.py` & `uac-api-0.4.0/uac_api/custom_days.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,28 +27,28 @@
         }
         parameters = prepare_query_params(query, field_mapping, args)
         return self.uc.get(url, query=parameters)
 
     def update_custom_day(self, payload=None, **args):
         url="/resources/customday"
         _payload = payload
-        return self.uc.put(url, json_data=_payload)
+        return self.uc.put(url, json_data=_payload, parse_response=False)
 
     def create_custom_day(self, payload=None, **args):
         '''
         Arguments:
         - retainSysIds: retainSysIds 
             False will ignore sysIds in the payload and create a new task  
         '''
         url="/resources/customday"
         field_mapping={
           "retainSysIds": "retainSysIds", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
-        return self.uc.post(url, json_data=_payload)
+        return self.uc.post(url, json_data=_payload, parse_response=False)
 
     def delete_custom_day(self, query=None, **args):
         '''
         Arguments:
         - customdayid: customdayid 
         - customdayname: customdayname 
         '''
```

### Comparing `uac-api-0.3.1/uac_api/email_templates.py` & `uac-api-0.4.0/uac_api/email_templates.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,28 +19,28 @@
         }
         parameters = prepare_query_params(query, field_mapping, args)
         return self.uc.get(url, query=parameters)
 
     def update_email_template(self, payload=None, **args):
         url="/resources/emailtemplate"
         _payload = payload
-        return self.uc.put(url, json_data=_payload)
+        return self.uc.put(url, json_data=_payload, parse_response=False)
 
     def create_email_template(self, payload=None, **args):
         '''
         Arguments:
         - retainSysIds: retainSysIds 
             False will ignore sysIds in the payload and create a new task  
         '''
         url="/resources/emailtemplate"
         field_mapping={
           "retainSysIds": "retainSysIds", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
-        return self.uc.post(url, json_data=_payload)
+        return self.uc.post(url, json_data=_payload, parse_response=False)
 
     def delete_email_template(self, query=None, **args):
         '''
         Arguments:
         - templateid: templateid 
         - templatename: templatename 
         '''
```

### Comparing `uac-api-0.3.1/uac_api/ldap.py` & `uac-api-0.4.0/uac_api/ldap.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,8 +13,8 @@
     def get_ldap(self):
         url="/resources/ldap"
         return self.uc.get(url)
 
     def update_ldap(self, payload=None, **args):
         url="/resources/ldap"
         _payload = payload
-        return self.uc.put(url, json_data=_payload)
+        return self.uc.put(url, json_data=_payload, parse_response=False)
```

### Comparing `uac-api-0.3.1/uac_api/oauth_clients.py` & `uac-api-0.4.0/uac_api/oauth_clients.py`

 * *Files 21% similar despite different names*

```diff
@@ -25,28 +25,28 @@
         }
         parameters = prepare_query_params(query, field_mapping, args)
         return self.uc.get(url, query=parameters)
 
     def update_oauth_client(self, payload=None, **args):
         url="/resources/oauthclient"
         _payload = payload
-        return self.uc.put(url, json_data=_payload)
+        return self.uc.put(url, json_data=_payload, parse_response=False)
 
     def create_oauth_client(self, payload=None, **args):
         '''
         Arguments:
         - retainSysIds: retainSysIds 
             False will ignore sysIds in the payload and create a new task  
         '''
         url="/resources/oauthclient"
         field_mapping={
           "retainSysIds": "retainSysIds", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
-        return self.uc.post(url, json_data=_payload)
+        return self.uc.post(url, json_data=_payload, parse_response=False)
 
     def delete_oauth_client(self, query=None, **args):
         '''
         Arguments:
         - oauthclientid: oauthclientid 
         - oauthclientname: oauthclientname 
         '''
```

### Comparing `uac-api-0.3.1/uac_api/oms_servers.py` & `uac-api-0.4.0/uac_api/oms_servers.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,28 +24,28 @@
         }
         parameters = prepare_query_params(query, field_mapping, args)
         return self.uc.get(url, query=parameters)
 
     def update_oms_server(self, payload=None, **args):
         url="/resources/omsserver"
         _payload = payload
-        return self.uc.put(url, json_data=_payload)
+        return self.uc.put(url, json_data=_payload, parse_response=False)
 
     def create_oms_server(self, payload=None, **args):
         '''
         Arguments:
         - retainSysIds: retainSysIds 
             False will ignore sysIds in the payload and create a new task  
         '''
         url="/resources/omsserver"
         field_mapping={
           "retainSysIds": "retainSysIds", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
-        return self.uc.post(url, json_data=_payload)
+        return self.uc.post(url, json_data=_payload, parse_response=False)
 
     def delete_oms_server(self, query=None, **args):
         '''
         Arguments:
         - serveraddress: serveraddress 
         - serverid: serverid 
         '''
```

### Comparing `uac-api-0.3.1/uac_api/properties.py` & `uac-api-0.4.0/uac_api/properties.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .utils import prepare_payload, prepare_query_params
+from .utils import prepare_payload, prepare_query_params, prepare_query_payload
 
 class Properties:
     def __init__(self, uc):
         self.log = uc.log
         self.headers = uc.headers
         self.uc = uc
 
@@ -14,15 +14,21 @@
         url="/resources/property"
         field_mapping={
             "propertyname": "propertyname", 
         }
         parameters = prepare_query_params(query, field_mapping, args)
         return self.uc.get(url, query=parameters)
 
-    def update_property(self, payload=None, **args):
+    def update_property(self, payload=None, query=None, **args):
         url="/resources/property"
-        _payload = payload
-        return self.uc.put(url, json_data=_payload)
+        query_fields={
+            "propertyname": "propertyname", 
+            "value": "value"
+        }
+        payload_fields = {
+        }
+        _query, _payload = prepare_query_payload(query, query_fields, payload, payload_fields, args)
+        return self.uc.put(url, query=_query, json_data=_payload, parse_response=False)
 
     def list_properties(self):
         url="/resources/property/list"
         return self.uc.get(url)
```

### Comparing `uac-api-0.3.1/uac_api/scripts.py` & `uac-api-0.4.0/uac_api/scripts.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,28 +19,28 @@
         }
         parameters = prepare_query_params(query, field_mapping, args)
         return self.uc.get(url, query=parameters)
 
     def update_script(self, payload=None, **args):
         url="/resources/script"
         _payload = payload
-        return self.uc.put(url, json_data=_payload)
+        return self.uc.put(url, json_data=_payload, parse_response=False)
 
     def create_script(self, payload=None, **args):
         '''
         Arguments:
         - retainSysIds: retainSysIds 
             False will ignore sysIds in the payload and create a new task  
         '''
         url="/resources/script"
         field_mapping={
           "retainSysIds": "retainSysIds", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
-        return self.uc.post(url, json_data=_payload)
+        return self.uc.post(url, json_data=_payload, parse_response=False)
 
     def delete_script(self, query=None, **args):
         '''
         Arguments:
         - scriptid: scriptid 
         - scriptname: scriptname 
         '''
```

### Comparing `uac-api-0.3.1/uac_api/server_operations.py` & `uac-api-0.4.0/uac_api/server_operations.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.3.1/uac_api/simulations.py` & `uac-api-0.4.0/uac_api/simulations.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,28 +27,28 @@
         }
         parameters = prepare_query_params(query, field_mapping, args)
         return self.uc.get(url, query=parameters)
 
     def update_simulation(self, payload=None, **args):
         url="/resources/simulation"
         _payload = payload
-        return self.uc.put(url, json_data=_payload)
+        return self.uc.put(url, json_data=_payload, parse_response=False)
 
     def create_simulation(self, payload=None, **args):
         '''
         Arguments:
         - retainSysIds: retainSysIds 
             False will ignore sysIds in the payload and create a new task  
         '''
         url="/resources/simulation"
         field_mapping={
           "retainSysIds": "retainSysIds", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
-        return self.uc.post(url, json_data=_payload)
+        return self.uc.post(url, json_data=_payload, parse_response=False)
 
     def delete_simulation(self, query=None, **args):
         '''
         Arguments:
         - simulationid: simulationid 
         - taskname: taskname 
         - workflowname: workflowname
```

### Comparing `uac-api-0.3.1/uac_api/task_instances.py` & `uac-api-0.4.0/uac_api/task_instances.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,48 @@
 # - set_or_modify_wait_time_duration_for_task_instance(instance_id, wait_time)
 # - set_priority_for_task_instance(instance_id, priority)
 # - skip_task_instance(instance_id)
 # - skip_task_instance_path(instance_id)
 # - unskip_task_instance(instance_id)
 
 class TaskInstances:
-    FINAL_STATUS = ["SUCCESS", "FAILED", "CANCELLED", "SKIPPED", "FINISHED"]
+    class Status:
+      ACTION_REQUIRED=60
+      CANCEL_PENDING=99
+      CANCELLED=130
+      CONFIRMATION_REQUIRED=125
+      DEFINED=0
+      EXCLUSIVE_REQUESTED=22
+      EXCLUSIVE_WAIT=23
+      EXECUTION_WAIT=33
+      FAILED=140
+      FINISHED=190
+      HELD=20
+      IN_DOUBT=110
+      QUEUED=40
+      RESOURCE_REQUESTED=25
+      RESOURCE_WAIT=30
+      RUNNING=80
+      RUNNING_PROBLEMS=81
+      SKIPPED=180
+      START_FAILURE=120
+      STARTED=70
+      SUBMITTED=43
+      SUCCESS=200
+      TIME_WAIT=15
+      UNDELIVERABLE=35
+      WAITING=10
+    
+    FINAL_STATUS = ["SUCCESS", "SKIPPED", "FINISHED", "START_FAILURE", "UNDELIVERABLE", "FAILED", "CANCELLED", "RUNNING/PROBLEMS", "IN_DOUBT"]
+    FINAL_STATUS_ID = [Status.START_FAILURE, Status.SUCCESS, Status.UNDELIVERABLE, Status.RUNNING_PROBLEMS, 
+                       Status.SKIPPED, Status.IN_DOUBT, Status.FINISHED, Status.FAILED, Status.CANCELLED]
     SUCCESS_STATUS = ["SUCCESS", "FINISHED", "SKIPPED"]
-    FAILED_STATUS = ["FAILED", "CANCELLED"]
+    SUCCESS_STATUS_ID = [Status.SUCCESS, Status.FINISHED, Status.SKIPPED]
+    FAILED_STATUS = ["FINISHED", "START_FAILURE", "UNDELIVERABLE", "FAILED", "CANCELLED", "RUNNING/PROBLEMS", "IN_DOUBT"]
+    FAILED_STATUS_ID = [Status.FAILED, Status.CANCELLED, Status.RUNNING_PROBLEMS]
     def __init__(self, uc) -> None:
         self.log = uc.log
         self.headers = uc.headers
         self.uc = uc
         
     def delete_task_instance(self, query=None, **args):
         '''
@@ -99,20 +130,49 @@
             "workflowinstancename": "workflowinstancename", 
             "criteria": "criteria", 
             "fetchglobal": "fetchglobal", 
         }
         parameters = prepare_query_params(query, field_mapping, args)
         return self.uc.get(url, query=parameters)
 
-    def update_operational_memo(self, payload=None, **args):
+    def update_operational_memo(self, query=None, **args):
         url="/resources/taskinstance/updatememo"
-        _payload = payload
-        return self.uc.put(url, json_data=_payload)
+        field_mapping={
+            "taskinstancename": "taskinstancename", 
+            "taskinstanceid": "taskinstanceid", 
+            "workflowinstancename": "workflowinstancename", 
+            "criteria": "criteria"
+        }
+        parameters = prepare_query_params(query, field_mapping, args)
+        print(args)
+        payload = args.pop("memo", "")
+        return self.uc.put(url, json_data=payload, query=parameters, headers={"Content-Type": "text/plain", "Accept": "text/plain"}, parse_response=False)
+
+    def set_complete(self, payload=None, **args):
+        '''
+        Arguments:
+        - name
+        - id
+        - workflowInstanceName
+        - criteria
+        - operationalMemo
+        '''
+        url="/resources/taskinstance/setcompleted"
+        field_mapping={
+            "name": "name", 
+            "id": "id", 
+            "workflowInstanceName": "workflowInstanceName", 
+            "criteria": "criteria",
+            "operationalMemo": "operationalMemo"
+        }
+        _payload = prepare_payload(payload, field_mapping, args)
+        return self.uc.post(url, json_data=_payload)
+
 
-    def task_instance_set_priority(self, payload=None, **args):
+    def set_priority(self, payload=None, **args):
         '''
         Arguments:
         - name: name 
         - id: id 
         - criteria: criteria 
         - workflowInstanceName: workflowInstanceName 
         - resourceName: resourceName 
@@ -256,15 +316,15 @@
           "vertexX": "vertexX", 
           "vertexY": "vertexY", 
           "inheritTriggerTime": "inheritTriggerTime", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
         return self.uc.post(url, json_data=_payload)
 
-    def task_instance_cancel(self, payload=None, **args):
+    def cancel(self, payload=None, **args):
         '''
         Arguments:
         - name: name 
         - id: id 
         - criteria: criteria 
         - workflowInstanceName: workflowInstanceName 
         - resourceName: resourceName 
@@ -306,15 +366,15 @@
           "taskStatus": "taskStatus", 
           "operationalMemo": "operationalMemo", 
           "holdReason": "holdReason", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
         return self.uc.post(url, json_data=_payload)
 
-    def task_instance_clear_dependencies(self, payload=None, **args):
+    def clear_dependencies(self, payload=None, **args):
         '''
         Arguments:
         - name: name 
         - id: id 
         - criteria: criteria 
         - workflowInstanceName: workflowInstanceName 
         - resourceName: resourceName 
@@ -356,15 +416,15 @@
           "taskStatus": "taskStatus", 
           "operationalMemo": "operationalMemo", 
           "holdReason": "holdReason", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
         return self.uc.post(url, json_data=_payload)
 
-    def task_instance_clear_exclusive(self, payload=None, **args):
+    def clear_exclusive(self, payload=None, **args):
         '''
         Arguments:
         - name: name 
         - id: id 
         - criteria: criteria 
         - workflowInstanceName: workflowInstanceName 
         - resourceName: resourceName 
@@ -406,15 +466,15 @@
           "taskStatus": "taskStatus", 
           "operationalMemo": "operationalMemo", 
           "holdReason": "holdReason", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
         return self.uc.post(url, json_data=_payload)
 
-    def task_instance_clear_instance_wait(self, payload=None, **args):
+    def clear_instance_wait(self, payload=None, **args):
         '''
         Arguments:
         - name: name 
         - id: id 
         - criteria: criteria 
         - workflowInstanceName: workflowInstanceName 
         - resourceName: resourceName 
@@ -456,15 +516,15 @@
           "taskStatus": "taskStatus", 
           "operationalMemo": "operationalMemo", 
           "holdReason": "holdReason", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
         return self.uc.post(url, json_data=_payload)
 
-    def task_instance_clear_predecessors(self, payload=None, **args):
+    def clear_predecessors(self, payload=None, **args):
         '''
         Arguments:
         - name: name 
         - id: id 
         - criteria: criteria 
         - workflowInstanceName: workflowInstanceName 
         - resourceName: resourceName 
@@ -506,15 +566,15 @@
           "taskStatus": "taskStatus", 
           "operationalMemo": "operationalMemo", 
           "holdReason": "holdReason", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
         return self.uc.post(url, json_data=_payload)
 
-    def task_instance_clear_resources(self, payload=None, **args):
+    def clear_resources(self, payload=None, **args):
         '''
         Arguments:
         - name: name 
         - id: id 
         - criteria: criteria 
         - workflowInstanceName: workflowInstanceName 
         - resourceName: resourceName 
@@ -556,15 +616,15 @@
           "taskStatus": "taskStatus", 
           "operationalMemo": "operationalMemo", 
           "holdReason": "holdReason", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
         return self.uc.post(url, json_data=_payload)
 
-    def task_instance_clear_timewait(self, payload=None, **args):
+    def clear_timewait(self, payload=None, **args):
         '''
         Arguments:
         - name: name 
         - id: id 
         - criteria: criteria 
         - workflowInstanceName: workflowInstanceName 
         - resourceName: resourceName 
@@ -606,15 +666,15 @@
           "taskStatus": "taskStatus", 
           "operationalMemo": "operationalMemo", 
           "holdReason": "holdReason", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
         return self.uc.post(url, json_data=_payload)
 
-    def task_instance_force_finish(self, payload=None, **args):
+    def force_finish(self, payload=None, **args):
         '''
         Arguments:
         - name: name 
         - id: id 
         - criteria: criteria 
         - workflowInstanceName: workflowInstanceName 
         - resourceName: resourceName 
@@ -656,15 +716,15 @@
           "taskStatus": "taskStatus", 
           "operationalMemo": "operationalMemo", 
           "holdReason": "holdReason", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
         return self.uc.post(url, json_data=_payload)
 
-    def task_instance_force_finish_cancel(self, payload=None, **args):
+    def force_finish_cancel(self, payload=None, **args):
         '''
         Arguments:
         - name: name 
         - id: id 
         - criteria: criteria 
         - workflowInstanceName: workflowInstanceName 
         - resourceName: resourceName 
@@ -706,15 +766,15 @@
           "taskStatus": "taskStatus", 
           "operationalMemo": "operationalMemo", 
           "holdReason": "holdReason", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
         return self.uc.post(url, json_data=_payload)
 
-    def task_instance_hold(self, payload=None, **args):
+    def hold(self, payload=None, **args):
         '''
         Arguments:
         - name: name 
         - id: id 
         - criteria: criteria 
         - workflowInstanceName: workflowInstanceName 
         - resourceName: resourceName 
@@ -756,15 +816,15 @@
           "taskStatus": "taskStatus", 
           "operationalMemo": "operationalMemo", 
           "holdReason": "holdReason", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
         return self.uc.post(url, json_data=_payload)
 
-    def task_instance_release(self, payload=None, **args):
+    def release(self, payload=None, **args):
         '''
         Arguments:
         - name: name 
         - id: id 
         - criteria: criteria 
         - workflowInstanceName: workflowInstanceName 
         - resourceName: resourceName 
@@ -806,15 +866,15 @@
           "taskStatus": "taskStatus", 
           "operationalMemo": "operationalMemo", 
           "holdReason": "holdReason", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
         return self.uc.post(url, json_data=_payload)
 
-    def task_instance_rerun(self, payload=None, **args):
+    def rerun(self, payload=None, **args):
         '''
         Arguments:
         - name: name 
         - id: id 
         - criteria: criteria 
         - workflowInstanceName: workflowInstanceName 
         - resourceName: resourceName 
@@ -856,15 +916,15 @@
           "taskStatus": "taskStatus", 
           "operationalMemo": "operationalMemo", 
           "holdReason": "holdReason", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
         return self.uc.post(url, json_data=_payload)
 
-    def task_instance_retrieve_output(self, query=None, **args):
+    def retrieve_output(self, query=None, **args):
         '''
         Arguments:
         - taskinstancename: taskinstancename 
         - taskinstanceid: taskinstanceid 
         - workflowinstancename: workflowinstancename 
         - criteria: criteria 
         - outputtype: outputtype 
@@ -884,15 +944,15 @@
             "numlines": "numlines", 
             "scantext": "scantext", 
             "operationalMemo": "operationalMemo", 
         }
         parameters = prepare_query_params(query, field_mapping, args)
         return self.uc.get(url, query=parameters)
 
-    def task_instance_skip(self, payload=None, **args):
+    def skip(self, payload=None, **args):
         '''
         Arguments:
         - name: name 
         - id: id 
         - criteria: criteria 
         - workflowInstanceName: workflowInstanceName 
         - resourceName: resourceName 
@@ -934,15 +994,15 @@
           "taskStatus": "taskStatus", 
           "operationalMemo": "operationalMemo", 
           "holdReason": "holdReason", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
         return self.uc.post(url, json_data=_payload)
 
-    def task_instance_skip_path(self, payload=None, **args):
+    def skip_path(self, payload=None, **args):
         '''
         Arguments:
         - name: name 
         - id: id 
         - criteria: criteria 
         - workflowInstanceName: workflowInstanceName 
         - resourceName: resourceName 
@@ -984,15 +1044,15 @@
           "taskStatus": "taskStatus", 
           "operationalMemo": "operationalMemo", 
           "holdReason": "holdReason", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
         return self.uc.post(url, json_data=_payload)
 
-    def task_instance_unskip(self, payload=None, **args):
+    def unskip(self, payload=None, **args):
         '''
         Arguments:
         - name: name 
         - id: id 
         - criteria: criteria 
         - workflowInstanceName: workflowInstanceName 
         - resourceName: resourceName
```

### Comparing `uac-api-0.3.1/uac_api/triggers.py` & `uac-api-0.4.0/uac_api/triggers.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # - list_triggers()
 # - list_triggers_advanced()
 # - modify_trigger(trigger_id, **kwargs)
 # - modify_time_of_time_trigger(trigger_id, new_time)
 # - read_trigger(trigger_id)
 # - trigger_now(trigger_id)
 # - unassign_execution_user_from_trigger(trigger_id)
-from .utils import prepare_payload, prepare_query_params
+from .utils import prepare_payload, prepare_query_params, prepare_query_payload
 
 class Triggers:
     def __init__(self, uc):
         self.log = uc.log
         self.headers = uc.headers
         self.uc = uc
 
@@ -32,27 +32,46 @@
             "triggername": "triggername", 
             "count": "count", 
             "startdate": "startdate", 
         }
         parameters = prepare_query_params(query, field_mapping, args)
         return self.uc.get(url, query=parameters)
 
-    def unassign_execution_user(self, payload=None, **args):
+    def unassign_execution_user(self, query=None, **args):
         '''
         Arguments:
         - triggerid: triggerid 
         - triggername: triggername 
         '''
         url="/resources/trigger/unassignexecutionuser"
         field_mapping={
           "triggerid": "triggerid", 
           "triggername": "triggername", 
         }
-        _payload = prepare_payload(payload, field_mapping, args)
-        return self.uc.post(url, json_data=_payload)
+        _query = prepare_query_params(query, field_mapping, args)
+        return self.uc.post(url, query=_query, json_data=None, parse_response=False)
+
+    def assign_execution_user_to_trigger(self, query=None, payload=None, **args):
+        '''
+        Arguments:
+        - triggerid: triggerid 
+        - triggername: triggername 
+        '''
+        url="/resources/trigger/assignexecutionuser"
+        query_fields = {
+            "triggername": "triggername",
+            "triggerid": "triggerid"
+        }
+
+        payload_fields={
+          "username": "username", 
+          "username": "username", 
+        }
+        _query, _payload = prepare_query_payload(query, query_fields, payload, payload_fields, args)
+        return self.uc.post(url, query=_query, json_data=_payload, parse_response=False)
 
     def create_temp_trigger(self, payload=None, **args):
         '''
         Arguments:
         - retainSysIds: retainSysIds 
             False will ignore sysIds in the payload and create a new task  
         '''
@@ -75,29 +94,32 @@
             "triggername": "triggername", 
         }
         parameters = prepare_query_params(query, field_mapping, args)
         return self.uc.get(url, query=parameters)
 
     def update_trigger(self, payload=None, **args):
         url="/resources/trigger"
-        _payload = payload
-        return self.uc.put(url, json_data=_payload)
+        field_mapping={
+          "enabled": "enabled", 
+        }
+        _payload = prepare_payload(payload, field_mapping, args)
+        return self.uc.put(url, json_data=_payload, parse_response=False)
 
     def create_trigger(self, payload=None, **args):
         '''
         Arguments:
         - retainSysIds: retainSysIds 
             False will ignore sysIds in the payload and create a new task  
         '''
         url="/resources/trigger"
         field_mapping={
           "retainSysIds": "retainSysIds", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
-        return self.uc.post(url, json_data=_payload)
+        return self.uc.post(url, json_data=_payload, parse_response=False)
 
     def delete_trigger(self, query=None, **args):
         '''
         Arguments:
         - triggerid: triggerid 
         - triggername: triggername 
         '''
@@ -161,8 +183,17 @@
             "type": "type", 
             "businessServices": "businessServices", 
             "enabled": "enabled", 
             "tasks": "tasks", 
             "description": "description", 
         }
         parameters = prepare_query_params(query, field_mapping, args)
-        return self.uc.get(url, query=parameters)
+        return self.uc.get(url, query=parameters)
+    
+    def enable_disable(self, payload=None, **args):
+        url="/resources/trigger/ops-enable-disable-trigger"
+        field_mapping={
+          "enable": "enable", 
+          "name": "name", 
+        }
+        _payload = prepare_payload(payload, field_mapping, args)
+        return self.uc.post(url, json_data=_payload)
```

### Comparing `uac-api-0.3.1/uac_api/universal_event_templates.py` & `uac-api-0.4.0/uac_api/universal_event_templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             False will ignore sysIds in the payload and create a new task  
         '''
         url="/resources/universaleventtemplate"
         field_mapping={
           "retainSysIds": "retainSysIds", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
-        return self.uc.post(url, json_data=_payload)
+        return self.uc.post(url, json_data=_payload, parse_response=False)
 
     def delete_universal_event_template(self, query=None, **args):
         '''
         Arguments:
         - templateid: templateid 
         - templatename: templatename 
         '''
```

### Comparing `uac-api-0.3.1/uac_api/universal_events.py` & `uac-api-0.4.0/uac_api/universal_events.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.3.1/uac_api/universal_templates.py` & `uac-api-0.4.0/uac_api/universal_templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,28 +31,28 @@
         }
         parameters = prepare_query_params(query, field_mapping, args)
         return self.uc.get(url, query=parameters)
 
     def update_universal_template(self, payload=None, **args):
         url="/resources/universaltemplate"
         _payload = payload
-        return self.uc.put(url, json_data=_payload)
+        return self.uc.put(url, json_data=_payload, parse_response=False)
 
     def create_universal_template(self, payload=None, **args):
         '''
         Arguments:
         - retainSysIds: retainSysIds 
             False will ignore sysIds in the payload and create a new task  
         '''
         url="/resources/universaltemplate"
         field_mapping={
           "retainSysIds": "retainSysIds", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
-        return self.uc.post(url, json_data=_payload)
+        return self.uc.post(url, json_data=_payload, parse_response=False)
 
     def delete_universal_template(self, query=None, **args):
         '''
         Arguments:
         - templateid: templateid 
         - templatename: templatename 
         '''
```

### Comparing `uac-api-0.3.1/uac_api/user_groups.py` & `uac-api-0.4.0/uac_api/user_groups.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,28 +19,28 @@
         }
         parameters = prepare_query_params(query, field_mapping, args)
         return self.uc.get(url, query=parameters)
 
     def update_user_group(self, payload=None, **args):
         url="/resources/usergroup"
         _payload = payload
-        return self.uc.put(url, json_data=_payload)
+        return self.uc.put(url, json_data=_payload, parse_response=False)
 
     def create_user_group(self, payload=None, **args):
         '''
         Arguments:
         - retainSysIds: retainSysIds 
             False will ignore sysIds in the payload and create a new task  
         '''
         url="/resources/usergroup"
         field_mapping={
           "retainSysIds": "retainSysIds", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
-        return self.uc.post(url, json_data=_payload)
+        return self.uc.post(url, json_data=_payload, parse_response=False)
 
     def delete_user_group(self, query=None, **args):
         '''
         Arguments:
         - groupid: groupid 
         - groupname: groupname 
         '''
```

### Comparing `uac-api-0.3.1/uac_api/users.py` & `uac-api-0.4.0/uac_api/users.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         Arguments:
         - userId: userId 
         - newPassword: newPassword 
         '''
         url="/resources/user/changepassword"
         field_mapping={
           "userId": "userId", 
+          "name": "userId", 
           "newPassword": "newPassword", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
         return self.uc.post(url, json_data=_payload)
 
     def get_user(self, query=None, **args):
         '''
@@ -44,28 +45,28 @@
         }
         parameters = prepare_query_params(query, field_mapping, args)
         return self.uc.get(url, query=parameters)
 
     def update_user(self, payload=None, **args):
         url="/resources/user"
         _payload = payload
-        return self.uc.put(url, json_data=_payload)
+        return self.uc.put(url, json_data=_payload, parse_response=False)
 
     def create_user(self, payload=None, **args):
         '''
         Arguments:
         - retainSysIds: retainSysIds 
             False will ignore sysIds in the payload and create a new task  
         '''
         url="/resources/user"
         field_mapping={
           "retainSysIds": "retainSysIds", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
-        return self.uc.post(url, json_data=_payload)
+        return self.uc.post(url, json_data=_payload, parse_response=False)
 
     def delete_user(self, query=None, **args):
         '''
         Arguments:
         - userid: userid 
         - username: username 
         '''
@@ -82,17 +83,21 @@
         Arguments:
         - retainSysIds: retainSysIds 
             False will ignore sysIds in the payload and create a new task  
         '''
         url="/resources/user/token"
         field_mapping={
           "retainSysIds": "retainSysIds", 
+          "userId":'userId',
+          "userName": "userName",
+          "name": "name",
+          "expiration": "expiration"
         }
         _payload = prepare_payload(payload, field_mapping, args)
-        return self.uc.post(url, json_data=_payload)
+        return self.uc.post(url, json_data=_payload, parse_response=False)
 
     def revoke_user_token(self, query=None, **args):
         '''
         Arguments:
         - userid: userid 
         - username: username 
         - tokenname: tokenname
```

### Comparing `uac-api-0.3.1/uac_api/variables.py` & `uac-api-0.4.0/uac_api/variables.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,28 +28,28 @@
         }
         parameters = prepare_query_params(query, field_mapping, args)
         return self.uc.get(url, query=parameters)
 
     def update_variable(self, payload=None, **args):
         url="/resources/variable"
         _payload = payload
-        return self.uc.put(url, json_data=_payload)
+        return self.uc.put(url, json_data=_payload, parse_response=False)
 
     def create_variable(self, payload=None, **args):
         '''
         Arguments:
         - retainSysIds: retainSysIds 
             False will ignore sysIds in the payload and create a new task  
         '''
         url="/resources/variable"
         field_mapping={
           "retainSysIds": "retainSysIds", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
-        return self.uc.post(url, json_data=_payload)
+        return self.uc.post(url, json_data=_payload, parse_response=False)
 
     def delete_variable(self, query=None, **args):
         '''
         Arguments:
         - variableid: variableid 
         - variablename: variablename 
         '''
```

### Comparing `uac-api-0.3.1/uac_api/virtual_resources.py` & `uac-api-0.4.0/uac_api/virtual_resources.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,28 +26,28 @@
         }
         parameters = prepare_query_params(query, field_mapping, args)
         return self.uc.get(url, query=parameters)
 
     def update_virtual_resource(self, payload=None, **args):
         url="/resources/virtual"
         _payload = payload
-        return self.uc.put(url, json_data=_payload)
+        return self.uc.put(url, json_data=_payload, parse_response=False)
 
     def create_virtual_resource(self, payload=None, **args):
         '''
         Arguments:
         - retainSysIds: retainSysIds 
             False will ignore sysIds in the payload and create a new task  
         '''
         url="/resources/virtual"
         field_mapping={
           "retainSysIds": "retainSysIds", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
-        return self.uc.post(url, json_data=_payload)
+        return self.uc.post(url, json_data=_payload, parse_response=False)
 
     def delete_virtual_resource(self, query=None, **args):
         '''
         Arguments:
         - resourceid: resourceid 
         - resourcename: resourcename 
         '''
@@ -89,9 +89,13 @@
             "businessServices": "businessServices", 
         }
         parameters = prepare_query_params(query, field_mapping, args)
         return self.uc.get(url, query=parameters)
 
     def update_limit(self, payload=None, **args):
         url="/resources/virtual/ops-update-resource-limit"
-        _payload = payload
+        field_mapping={
+          "name": "name", 
+          "limit": "limit"
+        }
+        _payload = prepare_payload(payload, field_mapping, args)
         return self.uc.post(url, json_data=_payload)
```

### Comparing `uac-api-0.3.1/uac_api/webhooks.py` & `uac-api-0.4.0/uac_api/webhooks.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         '''
         url="/resources/webhook/unassignexecutionuser"
         field_mapping={
           "webhookid": "webhookid", 
           "webhookname": "webhookname", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
-        return self.uc.post(url, json_data=_payload)
+        return self.uc.post(url, json_data=_payload, parse_response=False)
 
     def get_webhook(self, query=None, **args):
         '''
         Arguments:
         - webhookid: webhookid 
         - webhookname: webhookname 
         '''
@@ -43,28 +43,28 @@
         }
         parameters = prepare_query_params(query, field_mapping, args)
         return self.uc.get(url, query=parameters)
 
     def update_webhook(self, payload=None, **args):
         url="/resources/webhook"
         _payload = payload
-        return self.uc.put(url, json_data=_payload)
+        return self.uc.put(url, json_data=_payload, parse_response=False)
 
     def create_webhook(self, payload=None, **args):
         '''
         Arguments:
         - retainSysIds: retainSysIds 
             False will ignore sysIds in the payload and create a new task  
         '''
         url="/resources/webhook"
         field_mapping={
           "retainSysIds": "retainSysIds", 
         }
         _payload = prepare_payload(payload, field_mapping, args)
-        return self.uc.post(url, json_data=_payload)
+        return self.uc.post(url, json_data=_payload, parse_response=False)
 
     def delete_webhook(self, query=None, **args):
         '''
         Arguments:
         - webhookid: webhookid 
         - webhookname: webhookname 
         '''
```

### Comparing `uac-api-0.3.1/uac_api.egg-info/PKG-INFO` & `uac-api-0.4.0/uac_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uac-api
-Version: 0.3.1
+Version: 0.4.0
 Summary: A Python wrapper for the Stonebranch UAC API
 Home-page: https://github.com/gomleksiz/uac-api
 Author: Stonebranch
 Author-email: huseyim@gmail.com
 License: CC BY-NC 4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -21,14 +21,16 @@
 - **Comprehensive API Coverage**: Enables interaction with a wide array of Stonebranch UAC functionalities through Python functions.
 - **Enhanced Task Management**: Simplify the creation, management, and monitoring of tasks and workflows.
 - **Agent and Cluster Operations**: Manage agents and agent clusters with functions for updates, deletions, and status checks.
 - **Advanced Scheduling Capabilities**: Utilize calendars, custom days, and triggers to precisely schedule tasks.
 - **Resource Management**: Handle connections, credentials, properties, and variables for full control over your automation environment.
 - **Audit and Reporting**: Access audit logs and generate reports for detailed insights into your automation activities.
 - **Customization and Extension**: Manage custom days, email templates, scripts, and more, allowing for extensive customization and functionality extension.
+- **Download Reports**: Download report in CSV, TSV, JSON, XML and PDF formats.
+
 
 ## Installation
 
 ```bash
 pip install uac-api
 ```
 
@@ -220,18 +222,18 @@
 - get_oms_server(self, query=None, **args)
 - update_oms_server(self, payload=None, **args)
 - create_oms_server(self, payload=None, **args)
 - delete_oms_server(self, query=None, **args)
 - list_oms_servers(self)
 ## Properties:
 - get_property(self, query=None, **args)
-- update_property(self, payload=None, **args)
+- update_property(self, payload=None, query=None, **args)
 - list_properties(self)
 ## Reports:
-- run_report(self, query=None, **args)
+- run_report(self, query=None, report_format="csv", **args)
 ## Scripts:
 - get_script(self, query=None, **args)
 - update_script(self, payload=None, **args)
 - create_script(self, payload=None, **args)
 - delete_script(self, query=None, **args)
 - list_scripts(self)
 ## ServerOperations:
@@ -267,14 +269,15 @@
 - task_instance_rerun(self, payload=None, **args)
 - task_instance_retrieve_output(self, query=None, **args)
 - task_instance_skip(self, payload=None, **args)
 - task_instance_skip_path(self, payload=None, **args)
 - task_instance_unskip(self, payload=None, **args)
 - list_status(self, payload=None, **args) - List Task Instances
 - wait_for_status(self, id, statuses=FINAL_STATUS, timeout=300, interval=10): Waits until the task instance reaches one of the given statuses.
+- set_complete(self, payload=None, **args)
 ## Tasks:
 - get_task(self, query=None, **args)
 - update_task(self, payload=None, **args)
 - create_task(self, payload=None, **args)
 - clone_task(self, task_name, new_task_name): Copy task with a new name
 - delete_task(self, query=None, **args)
 - list_tasks(self, payload=None, **args)
@@ -287,24 +290,29 @@
 - task_clear_timewait(self, payload=None, **args)
 - task_create_with_properties(self, payload=None, **args)
 - list_dependency_list_1(self, query=None, **args)
 - task_insert_1(self, payload=None, **args)
 - task_launch(self, payload=None, **args)
 - task_release(self, payload=None, **args)
 - task_set_timewait(self, payload=None, **args)
+- create_linux_task(self, name, agent, payload=None, command=None, script=None)
+- create_windows_task(self, name, agent, payload=None, command=None, script=None)
+- create_workflow(self, name, payload=None)
 ## Triggers:
 - list_qualifying_times(self, query=None, **args)
+- assign_execution_user_to_trigger(self, query=None, payload=None, **args)
 - unassign_execution_user(self, payload=None, **args)
 - create_temp_trigger(self, payload=None, **args)
 - get_trigger(self, query=None, **args)
 - update_trigger(self, payload=None, **args)
 - create_trigger(self, payload=None, **args)
 - delete_trigger(self, query=None, **args)
 - list_triggers(self, payload=None, **args)
 - list_triggers_advanced(self, query=None, **args)
+- enable_disable(self, payload=None, **args)
 ## UniversalEventTemplates:
 - get_universal_event_template(self, query=None, **args)
 - update_universal_event_template(self, payload=None, **args)
 - create_universal_event_template(self, payload=None, **args)
 - delete_universal_event_template(self, query=None, **args)
 - list_universal_event_templates(self, query=None, **args)
 ## UniversalEvents:
@@ -369,14 +377,16 @@
 - add_edge(self, payload=None, **args)
 - delete_edge(self, query=None, **args)
 - get_vertices(self, query=None, **args)
 - update_vertex(self, payload=None, **args)
 - add_vertex(self, payload=None, **args)
 - delete_vertices(self, query=None, **args)
 - get_forecast(self, query=None, **args)
+- add_child_vertex(self, workflow_name, task_name, parent_task_name=None, parent_vertex_id=None, vertex_id=None, auto_arrange=True)
+- auto_arrange_vertices(self, workflow_name=None, payload=None)
 
 # Classes
 - Agents
 - AgentClusters
 - Audits
 - Bundles
 - Calendars
```

### Comparing `uac-api-0.3.1/uac_api.egg-info/SOURCES.txt` & `uac-api-0.4.0/uac_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

