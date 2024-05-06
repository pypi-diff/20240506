# Comparing `tmp/pih-rvw_auto-0.17.tar.gz` & `tmp/pih-rvw_auto-0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-rvw_auto-0.17.tar", last modified: Wed Apr 24 04:50:44 2024, max compression
+gzip compressed data, was "pih-rvw_auto-0.18.tar", last modified: Mon May  6 04:01:25 2024, max compression
```

## Comparing `pih-rvw_auto-0.17.tar` & `pih-rvw_auto-0.18.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 04:50:44.301414 pih-rvw_auto-0.17/
--rw-rw-rw-   0        0        0      282 2024-04-24 04:50:44.270167 pih-rvw_auto-0.17/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-24 04:50:43.879561 pih-rvw_auto-0.17/ReviewAutomationService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-rvw_auto-0.17/ReviewAutomationService/__init__.py
--rw-rw-rw-   0        0        0      158 2024-04-15 23:57:16.000000 pih-rvw_auto-0.17/ReviewAutomationService/__main__.py
--rw-rw-rw-   0        0        0     2476 2024-04-15 23:57:45.000000 pih-rvw_auto-0.17/ReviewAutomationService/api.py
--rw-rw-rw-   0        0        0      519 2024-04-24 04:48:56.000000 pih-rvw_auto-0.17/ReviewAutomationService/const.py
--rw-rw-rw-   0        0        0     8547 2024-04-24 04:33:37.000000 pih-rvw_auto-0.17/ReviewAutomationService/service.py
-drwxrwxrwx   0        0        0        0 2024-04-24 04:50:44.238922 pih-rvw_auto-0.17/pih_rvw_auto.egg-info/
--rw-rw-rw-   0        0        0      282 2024-04-24 04:50:43.000000 pih-rvw_auto-0.17/pih_rvw_auto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2024-04-24 04:50:43.000000 pih-rvw_auto-0.17/pih_rvw_auto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 04:50:43.000000 pih-rvw_auto-0.17/pih_rvw_auto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-04-24 04:50:43.000000 pih-rvw_auto-0.17/pih_rvw_auto.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-04-24 04:50:43.000000 pih-rvw_auto-0.17/pih_rvw_auto.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-04-24 04:50:43.000000 pih-rvw_auto-0.17/pih_rvw_auto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 04:50:44.301414 pih-rvw_auto-0.17/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-06 04:01:25.677923 pih-rvw_auto-0.18/
+-rw-rw-rw-   0        0        0      282 2024-05-06 04:01:25.646631 pih-rvw_auto-0.18/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-06 04:01:25.264028 pih-rvw_auto-0.18/ReviewAutomationService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-rvw_auto-0.18/ReviewAutomationService/__init__.py
+-rw-rw-rw-   0        0        0      158 2024-04-15 23:57:16.000000 pih-rvw_auto-0.18/ReviewAutomationService/__main__.py
+-rw-rw-rw-   0        0        0     2476 2024-04-15 23:57:45.000000 pih-rvw_auto-0.18/ReviewAutomationService/api.py
+-rw-rw-rw-   0        0        0      519 2024-05-06 04:00:59.000000 pih-rvw_auto-0.18/ReviewAutomationService/const.py
+-rw-rw-rw-   0        0        0     8565 2024-05-02 02:09:58.000000 pih-rvw_auto-0.18/ReviewAutomationService/service.py
+drwxrwxrwx   0        0        0        0 2024-05-06 04:01:25.599756 pih-rvw_auto-0.18/pih_rvw_auto.egg-info/
+-rw-rw-rw-   0        0        0      282 2024-05-06 04:01:24.000000 pih-rvw_auto-0.18/pih_rvw_auto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2024-05-06 04:01:24.000000 pih-rvw_auto-0.18/pih_rvw_auto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 04:01:24.000000 pih-rvw_auto-0.18/pih_rvw_auto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-05-06 04:01:24.000000 pih-rvw_auto-0.18/pih_rvw_auto.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-05-06 04:01:24.000000 pih-rvw_auto-0.18/pih_rvw_auto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-06 04:01:24.000000 pih-rvw_auto-0.18/pih_rvw_auto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 04:01:25.677923 pih-rvw_auto-0.18/setup.cfg
```

### Comparing `pih-rvw_auto-0.17/ReviewAutomationService/api.py` & `pih-rvw_auto-0.18/ReviewAutomationService/api.py`

 * *Files identical despite different names*

### Comparing `pih-rvw_auto-0.17/ReviewAutomationService/const.py` & `pih-rvw_auto-0.18/ReviewAutomationService/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pih.consts.hosts import Hosts
 from pih.collections.service import ServiceDescription
 
 NAME: str = "ReviewAutomation"
 
 HOST = Hosts.BACKUP_WORKER
 
-VERSION: str = "0.17"
+VERSION: str = "0.18"
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="Review automation service",
     host=HOST.NAME,
     use_standalone=True,
     version=VERSION,
```

### Comparing `pih-rvw_auto-0.17/ReviewAutomationService/service.py` & `pih-rvw_auto-0.18/ReviewAutomationService/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
                                                     )
                                                 )
 
                                             A.E.send(
                                                 A.CT_E.POLIBASE_PERSON_REVIEW_NOTIFICATION_WAS_ANSWERED,
                                                 (
                                                     nnt(person).pin,
-                                                    message_text,
+                                                    j((message_text.splitlines())),
                                                     int(answer_yes),
                                                 ),
                                             )
                                     else:
                                         pass
                             except NotFound as error:
                                 A.L.debug_bot(
```

