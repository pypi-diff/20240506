# Comparing `tmp/aegis-tools-2.6.2.tar.gz` & `tmp/aegis-tools-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aegis-tools-2.6.2.tar", last modified: Tue Apr 30 18:57:09 2024, max compression
+gzip compressed data, was "aegis-tools-2.6.3.tar", last modified: Mon May  6 18:49:45 2024, max compression
```

## Comparing `aegis-tools-2.6.2.tar` & `aegis-tools-2.6.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-04-30 18:57:09.008497 aegis-tools-2.6.2/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1073 2022-10-24 18:25:55.000000 aegis-tools-2.6.2/LICENSE
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2022-10-24 18:25:55.000000 aegis-tools-2.6.2/MANIFEST.in
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2024-04-30 18:57:09.008497 aegis-tools-2.6.2/PKG-INFO
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      881 2022-10-24 18:25:55.000000 aegis-tools-2.6.2/README.md
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-04-30 18:57:08.996497 aegis-tools-2.6.2/aegis/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       57 2022-10-24 18:25:55.000000 aegis-tools-2.6.2/aegis/__init__.py
--rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    20802 2024-04-30 00:13:47.000000 aegis-tools-2.6.2/aegis/aegis_.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    19087 2024-04-30 00:19:28.000000 aegis-tools-2.6.2/aegis/build.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2831 2024-02-09 21:33:25.000000 aegis-tools-2.6.2/aegis/config.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    25607 2024-04-30 01:24:43.000000 aegis-tools-2.6.2/aegis/database.py
--rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    27302 2024-04-22 18:29:41.000000 aegis-tools-2.6.2/aegis/hydra.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     7559 2023-05-24 02:47:45.000000 aegis-tools-2.6.2/aegis/mailer.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    46062 2024-04-30 18:56:53.000000 aegis-tools-2.6.2/aegis/model.py
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-04-30 18:57:09.000497 aegis-tools-2.6.2/aegis/sql/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1089 2022-11-22 01:51:27.000000 aegis-tools-2.6.2/aegis/sql/auditing-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     4611 2024-01-31 22:04:42.000000 aegis-tools-2.6.2/aegis/sql/auditing-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1051 2022-10-24 18:25:55.000000 aegis-tools-2.6.2/aegis/sql/build-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1672 2022-11-16 03:24:54.000000 aegis-tools-2.6.2/aegis/sql/build-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      450 2022-10-24 18:25:55.000000 aegis-tools-2.6.2/aegis/sql/cache_system.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1839 2023-04-02 17:24:35.000000 aegis-tools-2.6.2/aegis/sql/email_system-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1252 2023-05-22 20:40:27.000000 aegis-tools-2.6.2/aegis/sql/google_signin.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3409 2022-10-24 18:25:55.000000 aegis-tools-2.6.2/aegis/sql/hydra-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3195 2022-10-24 18:25:55.000000 aegis-tools-2.6.2/aegis/sql/hydra-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1535 2022-10-24 18:25:55.000000 aegis-tools-2.6.2/aegis/sql/member_auth.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      616 2022-10-24 18:25:55.000000 aegis-tools-2.6.2/aegis/sql/monitor-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      579 2022-10-24 18:25:55.000000 aegis-tools-2.6.2/aegis/sql/reports.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    37012 2024-04-18 02:54:56.000000 aegis-tools-2.6.2/aegis/stdlib.py
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-04-30 18:57:09.008497 aegis-tools-2.6.2/aegis/templates/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3071 2023-09-30 03:49:20.000000 aegis-tools-2.6.2/aegis/templates/build.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1549 2023-03-11 00:57:54.000000 aegis-tools-2.6.2/aegis/templates/build_confirm.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1187 2023-03-11 00:57:33.000000 aegis-tools-2.6.2/aegis/templates/build_form.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1217 2023-03-11 01:00:56.000000 aegis-tools-2.6.2/aegis/templates/build_view.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      253 2022-10-24 18:25:55.000000 aegis-tools-2.6.2/aegis/templates/error_message.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3377 2023-08-14 03:31:20.000000 aegis-tools-2.6.2/aegis/templates/frame.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2238 2023-09-30 03:49:39.000000 aegis-tools-2.6.2/aegis/templates/hydra.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2652 2023-03-11 00:52:58.000000 aegis-tools-2.6.2/aegis/templates/hydra_form.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1857 2023-09-30 03:52:25.000000 aegis-tools-2.6.2/aegis/templates/hydra_queue.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      109 2023-03-11 01:02:04.000000 aegis-tools-2.6.2/aegis/templates/index.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1954 2023-03-26 04:27:55.000000 aegis-tools-2.6.2/aegis/templates/report.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1909 2023-03-20 03:03:26.000000 aegis-tools-2.6.2/aegis/templates/report_form.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      745 2023-03-20 02:52:01.000000 aegis-tools-2.6.2/aegis/templates/reports.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    23427 2023-03-11 00:09:55.000000 aegis-tools-2.6.2/aegis/templates/w3.css
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2681 2022-10-24 18:25:55.000000 aegis-tools-2.6.2/aegis/threadpool.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    78528 2024-04-30 00:13:28.000000 aegis-tools-2.6.2/aegis/webapp.py
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-04-30 18:57:09.008497 aegis-tools-2.6.2/aegis_tools.egg-info/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2024-04-30 18:57:08.000000 aegis-tools-2.6.2/aegis_tools.egg-info/PKG-INFO
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1176 2024-04-30 18:57:08.000000 aegis-tools-2.6.2/aegis_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        1 2024-04-30 18:57:08.000000 aegis-tools-2.6.2/aegis_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       45 2024-04-30 18:57:08.000000 aegis-tools-2.6.2/aegis_tools.egg-info/entry_points.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       85 2024-04-30 18:57:08.000000 aegis-tools-2.6.2/aegis_tools.egg-info/requires.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        6 2024-04-30 18:57:08.000000 aegis-tools-2.6.2/aegis_tools.egg-info/top_level.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2024-04-30 18:57:09.008497 aegis-tools-2.6.2/setup.cfg
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1716 2023-09-26 15:24:50.000000 aegis-tools-2.6.2/setup.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-05-06 18:49:45.329288 aegis-tools-2.6.3/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1073 2022-10-24 18:25:55.000000 aegis-tools-2.6.3/LICENSE
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2022-10-24 18:25:55.000000 aegis-tools-2.6.3/MANIFEST.in
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2024-05-06 18:49:45.329288 aegis-tools-2.6.3/PKG-INFO
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      881 2022-10-24 18:25:55.000000 aegis-tools-2.6.3/README.md
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-05-06 18:49:45.305288 aegis-tools-2.6.3/aegis/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       57 2022-10-24 18:25:55.000000 aegis-tools-2.6.3/aegis/__init__.py
+-rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    20802 2024-04-30 00:13:47.000000 aegis-tools-2.6.3/aegis/aegis_.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    19087 2024-04-30 00:19:28.000000 aegis-tools-2.6.3/aegis/build.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2831 2024-02-09 21:33:25.000000 aegis-tools-2.6.3/aegis/config.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    25607 2024-04-30 01:24:43.000000 aegis-tools-2.6.3/aegis/database.py
+-rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    27302 2024-04-22 18:29:41.000000 aegis-tools-2.6.3/aegis/hydra.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     7559 2023-05-24 02:47:45.000000 aegis-tools-2.6.3/aegis/mailer.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    46355 2024-05-06 18:46:46.000000 aegis-tools-2.6.3/aegis/model.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-05-06 18:49:45.321288 aegis-tools-2.6.3/aegis/sql/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1089 2022-11-22 01:51:27.000000 aegis-tools-2.6.3/aegis/sql/auditing-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     4611 2024-01-31 22:04:42.000000 aegis-tools-2.6.3/aegis/sql/auditing-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1051 2022-10-24 18:25:55.000000 aegis-tools-2.6.3/aegis/sql/build-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1672 2022-11-16 03:24:54.000000 aegis-tools-2.6.3/aegis/sql/build-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      450 2022-10-24 18:25:55.000000 aegis-tools-2.6.3/aegis/sql/cache_system.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1839 2023-04-02 17:24:35.000000 aegis-tools-2.6.3/aegis/sql/email_system-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1252 2023-05-22 20:40:27.000000 aegis-tools-2.6.3/aegis/sql/google_signin.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3409 2022-10-24 18:25:55.000000 aegis-tools-2.6.3/aegis/sql/hydra-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3195 2022-10-24 18:25:55.000000 aegis-tools-2.6.3/aegis/sql/hydra-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1535 2022-10-24 18:25:55.000000 aegis-tools-2.6.3/aegis/sql/member_auth.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      616 2022-10-24 18:25:55.000000 aegis-tools-2.6.3/aegis/sql/monitor-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      579 2022-10-24 18:25:55.000000 aegis-tools-2.6.3/aegis/sql/reports.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    37012 2024-04-18 02:54:56.000000 aegis-tools-2.6.3/aegis/stdlib.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-05-06 18:49:45.325288 aegis-tools-2.6.3/aegis/templates/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3071 2023-09-30 03:49:20.000000 aegis-tools-2.6.3/aegis/templates/build.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1549 2023-03-11 00:57:54.000000 aegis-tools-2.6.3/aegis/templates/build_confirm.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1187 2023-03-11 00:57:33.000000 aegis-tools-2.6.3/aegis/templates/build_form.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1217 2023-03-11 01:00:56.000000 aegis-tools-2.6.3/aegis/templates/build_view.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      253 2022-10-24 18:25:55.000000 aegis-tools-2.6.3/aegis/templates/error_message.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3377 2023-08-14 03:31:20.000000 aegis-tools-2.6.3/aegis/templates/frame.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2238 2023-09-30 03:49:39.000000 aegis-tools-2.6.3/aegis/templates/hydra.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2652 2023-03-11 00:52:58.000000 aegis-tools-2.6.3/aegis/templates/hydra_form.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1857 2023-09-30 03:52:25.000000 aegis-tools-2.6.3/aegis/templates/hydra_queue.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      109 2023-03-11 01:02:04.000000 aegis-tools-2.6.3/aegis/templates/index.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1954 2023-03-26 04:27:55.000000 aegis-tools-2.6.3/aegis/templates/report.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1909 2023-03-20 03:03:26.000000 aegis-tools-2.6.3/aegis/templates/report_form.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      745 2023-03-20 02:52:01.000000 aegis-tools-2.6.3/aegis/templates/reports.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    23427 2023-03-11 00:09:55.000000 aegis-tools-2.6.3/aegis/templates/w3.css
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2681 2022-10-24 18:25:55.000000 aegis-tools-2.6.3/aegis/threadpool.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    78528 2024-04-30 00:13:28.000000 aegis-tools-2.6.3/aegis/webapp.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-05-06 18:49:45.329288 aegis-tools-2.6.3/aegis_tools.egg-info/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2024-05-06 18:49:45.000000 aegis-tools-2.6.3/aegis_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1176 2024-05-06 18:49:45.000000 aegis-tools-2.6.3/aegis_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        1 2024-05-06 18:49:45.000000 aegis-tools-2.6.3/aegis_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       45 2024-05-06 18:49:45.000000 aegis-tools-2.6.3/aegis_tools.egg-info/entry_points.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       85 2024-05-06 18:49:45.000000 aegis-tools-2.6.3/aegis_tools.egg-info/requires.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        6 2024-05-06 18:49:45.000000 aegis-tools-2.6.3/aegis_tools.egg-info/top_level.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2024-05-06 18:49:45.329288 aegis-tools-2.6.3/setup.cfg
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1716 2023-09-26 15:24:50.000000 aegis-tools-2.6.3/setup.py
```

### Comparing `aegis-tools-2.6.2/LICENSE` & `aegis-tools-2.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.2/PKG-INFO` & `aegis-tools-2.6.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aegis-tools
-Version: 2.6.2
+Version: 2.6.3
 Summary: Aegis is a set of battle-tested tools and tricks to help everyone make better software
 Home-page: https://github.com/mdagosta/aegis
 Author: Michael D'Agosta
 Author-email: mdagosta@codebug.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aegis-tools-2.6.2/README.md` & `aegis-tools-2.6.3/README.md`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.2/aegis/aegis_.py` & `aegis-tools-2.6.3/aegis/aegis_.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.2/aegis/build.py` & `aegis-tools-2.6.3/aegis/build.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.2/aegis/config.py` & `aegis-tools-2.6.3/aegis/config.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.2/aegis/database.py` & `aegis-tools-2.6.3/aegis/database.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.2/aegis/hydra.py` & `aegis-tools-2.6.3/aegis/hydra.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.2/aegis/mailer.py` & `aegis-tools-2.6.3/aegis/mailer.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.2/aegis/model.py` & `aegis-tools-2.6.3/aegis/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -936,77 +936,80 @@
 class Cache(aegis.database.Row):
     table_name = 'cache'
     id_column = 'cache_id'
 
     # External Interface for simplified usage
     @classmethod
     def get_cache(cls, cache_key):
+        # It's important to make sure this only does SELECT. It can't UPDATE or DELETE to maintain the cache or can be surprising in real usage.
         cache_obj = cls.get_key(cache_key)
-        if cache_obj and type(cache_obj['cache_json']) is str:
+        if not cache_obj:
+            return None
+        if cache_obj['cache_expiry'] <= datetime.datetime.utcnow():
+            return False
+        if type(cache_obj['cache_json']) is str:
             return json.loads(cache_obj['cache_json'])
-        elif cache_obj:
+        else:
             return cache_obj['cache_json']
 
     @classmethod
-    def set_cache(cls, cache_key, cache_obj, duration_s):
-        cache_json = json.dumps(cache_obj, cls=aegis.stdlib.DateTimeEncoder)
-        cache_expiry = datetime.datetime.utcnow() + datetime.timedelta(seconds=duration_s) + datetime.timedelta(seconds=random.randint(0, duration_s))
-        cache_id = cls.set_key(cache_key, cache_json, cache_expiry)
+    def set_cache(cls, cache_key, cache_json_str, duration_s):
+        # INSERT or UPDATE to make sure that these values are what are in the cache and returned.
+        cache_json = json.dumps(cache_json_str, cls=aegis.stdlib.DateTimeEncoder)
+        cache_expiry = datetime.datetime.utcnow() + datetime.timedelta(seconds=duration_s) + datetime.timedelta(seconds=random.uniform(0, duration_s))
+        cls.set_key(cache_key, cache_json, cache_expiry)
         return cls.get_cache(cache_key)
 
     @staticmethod
+    def del_key(cache_key):
+        sql = "DELETE FROM cache WHERE cache_key=%s"
+        return db().execute(sql, cache_key)
+
+    @staticmethod
     def del_star(cache_key):
         cache_key = cache_key.replace('*', '%%')
         sql = "DELETE FROM cache WHERE cache_key LIKE '" + cache_key + "'"
         return db().execute_rowcount(sql)
 
     @staticmethod
-    def del_key(cache_key):
-        sql = "DELETE FROM cache WHERE cache_key=%s"
-        return db().execute(sql, cache_key)
-
-    @staticmethod
-    def purge_all():
+    def del_all():
         sql = "DELETE FROM cache"
         return db().execute(sql)
 
-    # Internal Interface
+    # Internal Interface. Use the existence of cache_key to choose INSERT or UPDATE.
     @classmethod
     def get_key(cls, cache_key):
-        sql = "SELECT * FROM cache WHERE cache_key=%s AND cache_expiry > NOW()"
+        sql = "SELECT * FROM cache WHERE cache_key=%s"
         return db().get(sql, cache_key, cls=cls)
 
     @classmethod
+    def set_key(cls, cache_key, cache_json, cache_expiry):
+        cache_obj = cls.get_key(cache_key)
+        if cache_obj:
+            cls.update_key(cache_key, cache_json, cache_expiry)
+        else:
+            cls.insert_key(cache_key, cache_json, cache_expiry)
+        cls.purge_expired()
+
+    @classmethod
     def insert_key(cls, cache_key, cache_json, cache_expiry):
         sql = "INSERT INTO cache (cache_key, cache_json, cache_expiry) VALUES (%s, %s, %s)"
         if type(db()) is aegis.database.PostgresConnection:
             sql += ' RETURNING cache_id'
         try:
             return db().execute(sql, cache_key, cache_json, cache_expiry)
         except (aegis.database.MysqlIntegrityError, aegis.database.PgsqlUniqueViolation) as ex:
             logging.warning("Ignoring duplicate key in cache: %s", cache_key)
 
     @classmethod
     def update_key(cls, cache_key, cache_json, cache_expiry):
-        sql = "UPDATE cache SET cache_json=%s, cache_expiry=%s WHERE cache_key=%s"
+        sql = "UPDATE cache SET cache_json=%s, cache_expiry=%s, delete_dttm=NULL WHERE cache_key=%s"
         return db().execute(sql, cache_json, cache_expiry, cache_key)
 
     @classmethod
-    def set_key(cls, cache_key, cache_json, cache_expiry):
-        cls.purge_expired()
-        cache_obj = cls.get_key(cache_key)
-        if cache_obj:
-            cls.update_key(cache_key, cache_json, cache_expiry)
-            cache_obj = cls.get_key(cache_key)
-        else:
-            cls.insert_key(cache_key, cache_json, cache_expiry)
-            cache_obj = cls.get_key(cache_key)
-        return cache_obj
-
-    @classmethod
     def purge_expired(cls):
         sql = "DELETE FROM cache WHERE cache_expiry < NOW()"
         return db().execute(sql)
 
 
 class AuditSession(aegis.database.Row):
     table_name = 'audit_session'
```

### Comparing `aegis-tools-2.6.2/aegis/sql/auditing-mysql.sql` & `aegis-tools-2.6.3/aegis/sql/auditing-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.2/aegis/sql/auditing-pgsql.sql` & `aegis-tools-2.6.3/aegis/sql/auditing-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.2/aegis/sql/build-mysql.sql` & `aegis-tools-2.6.3/aegis/sql/build-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.2/aegis/sql/build-pgsql.sql` & `aegis-tools-2.6.3/aegis/sql/build-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.2/aegis/sql/email_system-pgsql.sql` & `aegis-tools-2.6.3/aegis/sql/email_system-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.2/aegis/sql/google_signin.sql` & `aegis-tools-2.6.3/aegis/sql/google_signin.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.2/aegis/sql/hydra-mysql.sql` & `aegis-tools-2.6.3/aegis/sql/hydra-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.2/aegis/sql/hydra-pgsql.sql` & `aegis-tools-2.6.3/aegis/sql/hydra-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.2/aegis/sql/member_auth.sql` & `aegis-tools-2.6.3/aegis/sql/member_auth.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.2/aegis/sql/monitor-mysql.sql` & `aegis-tools-2.6.3/aegis/sql/monitor-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.2/aegis/sql/reports.sql` & `aegis-tools-2.6.3/aegis/sql/reports.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.2/aegis/stdlib.py` & `aegis-tools-2.6.3/aegis/stdlib.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.2/aegis/templates/build.html` & `aegis-tools-2.6.3/aegis/templates/build.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.2/aegis/templates/build_confirm.html` & `aegis-tools-2.6.3/aegis/templates/build_confirm.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.2/aegis/templates/build_form.html` & `aegis-tools-2.6.3/aegis/templates/build_form.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.2/aegis/templates/build_view.html` & `aegis-tools-2.6.3/aegis/templates/build_view.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.2/aegis/templates/frame.html` & `aegis-tools-2.6.3/aegis/templates/frame.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.2/aegis/templates/hydra.html` & `aegis-tools-2.6.3/aegis/templates/hydra.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.2/aegis/templates/hydra_form.html` & `aegis-tools-2.6.3/aegis/templates/hydra_form.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.2/aegis/templates/hydra_queue.html` & `aegis-tools-2.6.3/aegis/templates/hydra_queue.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.2/aegis/templates/report.html` & `aegis-tools-2.6.3/aegis/templates/report.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.2/aegis/templates/report_form.html` & `aegis-tools-2.6.3/aegis/templates/report_form.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.2/aegis/templates/reports.html` & `aegis-tools-2.6.3/aegis/templates/reports.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.2/aegis/templates/w3.css` & `aegis-tools-2.6.3/aegis/templates/w3.css`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.2/aegis/threadpool.py` & `aegis-tools-2.6.3/aegis/threadpool.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.2/aegis/webapp.py` & `aegis-tools-2.6.3/aegis/webapp.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.2/aegis_tools.egg-info/PKG-INFO` & `aegis-tools-2.6.3/aegis_tools.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aegis-tools
-Version: 2.6.2
+Version: 2.6.3
 Summary: Aegis is a set of battle-tested tools and tricks to help everyone make better software
 Home-page: https://github.com/mdagosta/aegis
 Author: Michael D'Agosta
 Author-email: mdagosta@codebug.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aegis-tools-2.6.2/aegis_tools.egg-info/SOURCES.txt` & `aegis-tools-2.6.3/aegis_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.2/setup.py` & `aegis-tools-2.6.3/setup.py`

 * *Files identical despite different names*

