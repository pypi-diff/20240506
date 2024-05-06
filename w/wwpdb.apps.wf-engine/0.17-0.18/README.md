# Comparing `tmp/wwpdb.apps.wf_engine-0.17.tar.gz` & `tmp/wwpdb_apps_wf_engine-0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.apps.wf_engine-0.17.tar", last modified: Mon Jun  6 10:55:06 2022, max compression
+gzip compressed data, was "wwpdb_apps_wf_engine-0.18.tar", last modified: Mon May  6 13:56:05 2024, max compression
```

## Comparing `wwpdb.apps.wf_engine-0.17.tar` & `wwpdb_apps_wf_engine-0.18.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-06 10:55:06.697952 wwpdb.apps.wf_engine-0.17/
--rw-r--r--   0 vsts      (1001) docker     (121)      732 2022-06-06 10:55:06.697952 wwpdb.apps.wf_engine-0.17/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)       54 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/README.md
--rw-r--r--   0 vsts      (1001) docker     (121)      108 2022-06-06 10:55:06.697952 wwpdb.apps.wf_engine-0.17/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (121)     2672 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-06 10:55:06.693952 wwpdb.apps.wf_engine-0.17/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (121)       65 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-06 10:55:06.693952 wwpdb.apps.wf_engine-0.17/wwpdb/apps/
--rw-r--r--   0 vsts      (1001) docker     (121)       65 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/apps/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-06 10:55:06.693952 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/
--rw-r--r--   0 vsts      (1001) docker     (121)      150 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-06 10:55:06.697952 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/engine/
--rw-r--r--   0 vsts      (1001) docker     (121)     4673 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/engine/CommandLineArgs.py
--rw-r--r--   0 vsts      (1001) docker     (121)    19112 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/engine/EngineUtils.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10424 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/engine/ExternalTask.py
--rw-r--r--   0 vsts      (1001) docker     (121)    13656 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/engine/InterpretDataObject.py
--rw-r--r--   0 vsts      (1001) docker     (121)    11954 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/engine/ProcessManager.py
--rw-r--r--   0 vsts      (1001) docker     (121)    54426 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/engine/ServerMonitor.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1587 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/engine/SwitchTask.py
--rw-r--r--   0 vsts      (1001) docker     (121)    44520 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/engine/WFEapplications.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5768 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/engine/WorkflowManager.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5850 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/engine/WorkflowSession.py
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/engine/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2395 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/engine/autorun.py
--rw-r--r--   0 vsts      (1001) docker     (121)    11376 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/engine/dbAPI.py
--rw-r--r--   0 vsts      (1001) docker     (121)    57880 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/engine/mainEngine.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-06 10:55:06.697952 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/reader/
--rw-r--r--   0 vsts      (1001) docker     (121)     5681 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/reader/TaskComparitor.py
--rw-r--r--   0 vsts      (1001) docker     (121)      720 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/reader/TaskParameter.py
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/reader/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7288 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/reader/dataReference.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1424 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/reader/metaDataObject.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1022 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/reader/parseTimeDelta.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6112 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/reader/parseXML.py
--rw-r--r--   0 vsts      (1001) docker     (121)    16353 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/reader/taskReference.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-06 10:55:06.697952 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/wf_engine_utils/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/wf_engine_utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-06 10:55:06.697952 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/wf_engine_utils/process/
--rw-r--r--   0 vsts      (1001) docker     (121)     9509 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/wf_engine_utils/process/ProcessUtils.py
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/wf_engine_utils/process/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-06 10:55:06.697952 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/wf_engine_utils/run/
--rw-r--r--   0 vsts      (1001) docker     (121)     1673 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/wf_engine_utils/run/MyLogger.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1950 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/wf_engine_utils/run/WFEngineRunner.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     4404 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/wf_engine_utils/run/WFEngineRunnerExec.py
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/wf_engine_utils/run/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-06 10:55:06.697952 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/wf_engine_utils/tasks/
--rw-r--r--   0 vsts      (1001) docker     (121)    10807 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/wf_engine_utils/tasks/WFTaskRequest.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)    27516 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/wf_engine_utils/tasks/WFTaskRequestExec.py
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/wf_engine_utils/tasks/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-06 10:55:06.697952 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/wf_engine_utils/test/
--rw-r--r--   0 vsts      (1001) docker     (121)      300 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/wf_engine_utils/test/test-bmrb-codes.ids
--rw-r--r--   0 vsts      (1001) docker     (121)      450 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/wf_engine_utils/test/test-emdb-codes.ids
--rw-r--r--   0 vsts      (1001) docker     (121)      250 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/wf_engine_utils/test/test-pdb-codes.ids
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-06 10:55:06.697952 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/wf_engine_utils/time/
--rwxr-xr-x   0 vsts      (1001) docker     (121)     4355 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/wf_engine_utils/time/TimeStamp.py
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-06-06 10:54:00.000000 wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/wf_engine_utils/time/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-06 10:55:06.693952 wwpdb.apps.wf_engine-0.17/wwpdb.apps.wf_engine.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)      732 2022-06-06 10:55:06.000000 wwpdb.apps.wf_engine-0.17/wwpdb.apps.wf_engine.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     2202 2022-06-06 10:55:06.000000 wwpdb.apps.wf_engine-0.17/wwpdb.apps.wf_engine.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-06-06 10:55:06.000000 wwpdb.apps.wf_engine-0.17/wwpdb.apps.wf_engine.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-06-06 10:54:28.000000 wwpdb.apps.wf_engine-0.17/wwpdb.apps.wf_engine.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (121)      172 2022-06-06 10:55:06.000000 wwpdb.apps.wf_engine-0.17/wwpdb.apps.wf_engine.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        6 2022-06-06 10:55:06.000000 wwpdb.apps.wf_engine-0.17/wwpdb.apps.wf_engine.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 13:56:05.615555 wwpdb_apps_wf_engine-0.18/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1102 2024-05-06 13:56:05.615555 wwpdb_apps_wf_engine-0.18/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)       54 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-05-06 13:56:05.619555 wwpdb_apps_wf_engine-0.18/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2672 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 13:56:05.603555 wwpdb_apps_wf_engine-0.18/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 13:56:05.607555 wwpdb_apps_wf_engine-0.18/wwpdb/apps/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/apps/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 13:56:05.607555 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/
+-rw-r--r--   0 vsts      (1001) docker     (127)      150 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 13:56:05.611555 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/engine/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4673 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/engine/CommandLineArgs.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19112 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/engine/EngineUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10424 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/engine/ExternalTask.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13656 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/engine/InterpretDataObject.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11954 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/engine/ProcessManager.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    54426 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/engine/ServerMonitor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1587 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/engine/SwitchTask.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    44221 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/engine/WFEapplications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5768 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/engine/WorkflowManager.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5850 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/engine/WorkflowSession.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/engine/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2395 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/engine/autorun.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11376 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/engine/dbAPI.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    57880 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/engine/mainEngine.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 13:56:05.615555 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/reader/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5681 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/reader/TaskComparitor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      720 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/reader/TaskParameter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/reader/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7288 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/reader/dataReference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1424 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/reader/metaDataObject.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1022 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/reader/parseTimeDelta.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6112 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/reader/parseXML.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16353 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/reader/taskReference.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 13:56:05.615555 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/wf_engine_utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/wf_engine_utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 13:56:05.615555 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/wf_engine_utils/process/
+-rw-r--r--   0 vsts      (1001) docker     (127)     9509 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/wf_engine_utils/process/ProcessUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/wf_engine_utils/process/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 13:56:05.615555 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/wf_engine_utils/run/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1673 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/wf_engine_utils/run/MyLogger.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1950 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/wf_engine_utils/run/WFEngineRunner.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     4404 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/wf_engine_utils/run/WFEngineRunnerExec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/wf_engine_utils/run/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 13:56:05.615555 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/wf_engine_utils/tasks/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10807 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/wf_engine_utils/tasks/WFTaskRequest.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)    27516 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/wf_engine_utils/tasks/WFTaskRequestExec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/wf_engine_utils/tasks/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 13:56:05.615555 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/wf_engine_utils/test/
+-rw-r--r--   0 vsts      (1001) docker     (127)      300 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/wf_engine_utils/test/test-bmrb-codes.ids
+-rw-r--r--   0 vsts      (1001) docker     (127)      450 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/wf_engine_utils/test/test-emdb-codes.ids
+-rw-r--r--   0 vsts      (1001) docker     (127)      250 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/wf_engine_utils/test/test-pdb-codes.ids
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 13:56:05.615555 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/wf_engine_utils/time/
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     4355 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/wf_engine_utils/time/TimeStamp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-06 13:54:44.000000 wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/wf_engine_utils/time/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 13:56:05.615555 wwpdb_apps_wf_engine-0.18/wwpdb.apps.wf_engine.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1102 2024-05-06 13:56:05.000000 wwpdb_apps_wf_engine-0.18/wwpdb.apps.wf_engine.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2202 2024-05-06 13:56:05.000000 wwpdb_apps_wf_engine-0.18/wwpdb.apps.wf_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-06 13:56:05.000000 wwpdb_apps_wf_engine-0.18/wwpdb.apps.wf_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-06 13:55:45.000000 wwpdb_apps_wf_engine-0.18/wwpdb.apps.wf_engine.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      172 2024-05-06 13:56:05.000000 wwpdb_apps_wf_engine-0.18/wwpdb.apps.wf_engine.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-06 13:56:05.000000 wwpdb_apps_wf_engine-0.18/wwpdb.apps.wf_engine.egg-info/top_level.txt
```

### Comparing `wwpdb.apps.wf_engine-0.17/setup.py` & `wwpdb_apps_wf_engine-0.18/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/engine/CommandLineArgs.py` & `wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/engine/CommandLineArgs.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/engine/EngineUtils.py` & `wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/engine/EngineUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/engine/ExternalTask.py` & `wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/engine/ExternalTask.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/engine/InterpretDataObject.py` & `wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/engine/InterpretDataObject.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/engine/ProcessManager.py` & `wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/engine/ProcessManager.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/engine/ServerMonitor.py` & `wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/engine/ServerMonitor.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/engine/SwitchTask.py` & `wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/engine/SwitchTask.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/engine/WFEapplications.py` & `wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/engine/WFEapplications.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,27 +54,14 @@
         fPath = os.path.join(storage_pickled_depositions, str(depSetId))
     else:
         fPath = storage_pickled_depositions
 
     return fPath
 
 
-def getNotesEmailAddr():
-    """Returns the email address for archiving messages"""
-    email = "wwpdb-da-system@rcsb.rutgers.edu"
-
-    siteid = getSiteId()
-    # Debugging at PDBe
-    if siteid == "PDBE_DEV":
-        cI = ConfigInfo()
-        email = cI.get("ANNOTATION_EMAIL")
-
-    return email
-
-
 def runOutOfBandWorkflow(DBstatusAPI, depSetId, classId, classFileName):
     """UPDATE status.communication SET  sender=%s, receiver=%s, wf_class_id=%s, wf_class_file=%s,
                                   command=%s, status=%s, actual_timestamp=%s, data_version=%s
                                   WHERE ( dep_set_id=%s);
 
     ['WFUTILS', 'WFE', 'PDBX2PDBX_DEP', 'wf_op_pdbx2pdbx_fs_deposit.xml',
      'runWF', 'PENDING', Decimal('492013055.527617'), 'latest',
```

### Comparing `wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/engine/WorkflowManager.py` & `wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/engine/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/engine/WorkflowSession.py` & `wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/engine/WorkflowSession.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/engine/autorun.py` & `wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/engine/autorun.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/engine/dbAPI.py` & `wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/engine/dbAPI.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/engine/mainEngine.py` & `wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/engine/mainEngine.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/reader/TaskComparitor.py` & `wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/reader/TaskComparitor.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/reader/TaskParameter.py` & `wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/reader/TaskParameter.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/reader/dataReference.py` & `wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/reader/dataReference.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/reader/metaDataObject.py` & `wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/reader/metaDataObject.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/reader/parseTimeDelta.py` & `wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/reader/parseTimeDelta.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/reader/parseXML.py` & `wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/reader/parseXML.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/reader/taskReference.py` & `wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/reader/taskReference.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/wf_engine_utils/process/ProcessUtils.py` & `wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/wf_engine_utils/process/ProcessUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/wf_engine_utils/run/MyLogger.py` & `wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/wf_engine_utils/run/MyLogger.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/wf_engine_utils/run/WFEngineRunner.py` & `wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/wf_engine_utils/run/WFEngineRunner.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/wf_engine_utils/run/WFEngineRunnerExec.py` & `wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/wf_engine_utils/run/WFEngineRunnerExec.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/wf_engine_utils/tasks/WFTaskRequest.py` & `wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/wf_engine_utils/tasks/WFTaskRequest.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/wf_engine_utils/tasks/WFTaskRequestExec.py` & `wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/wf_engine_utils/tasks/WFTaskRequestExec.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.wf_engine-0.17/wwpdb/apps/wf_engine/wf_engine_utils/time/TimeStamp.py` & `wwpdb_apps_wf_engine-0.18/wwpdb/apps/wf_engine/wf_engine_utils/time/TimeStamp.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.wf_engine-0.17/wwpdb.apps.wf_engine.egg-info/SOURCES.txt` & `wwpdb_apps_wf_engine-0.18/wwpdb.apps.wf_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

