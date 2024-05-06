# Comparing `tmp/ATH-0.5.0.tar.gz` & `tmp/ATH-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ATH-0.5.0.tar", last modified: Mon May  6 15:42:15 2024, max compression
+gzip compressed data, was "ATH-0.5.1.tar", last modified: Mon May  6 15:53:38 2024, max compression
```

## Comparing `ATH-0.5.0.tar` & `ATH-0.5.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 15:42:15.045108 ATH-0.5.0/
-drwxrwxrwx   0        0        0        0 2024-05-06 15:42:15.023615 ATH-0.5.0/ATH/
--rw-rw-rw-   0        0        0     1287 2024-03-03 12:52:16.000000 ATH-0.5.0/ATH/DB_read.py
--rw-rw-rw-   0        0        0      914 2024-03-02 12:38:15.000000 ATH-0.5.0/ATH/DB_send.py
--rw-rw-rw-   0        0        0      440 2024-04-27 18:54:21.000000 ATH-0.5.0/ATH/__init__.py
--rw-rw-rw-   0        0        0      172 2024-03-16 15:51:41.000000 ATH-0.5.0/ATH/abc123_2.py
--rw-rw-rw-   0        0        0      125 2024-03-01 17:00:39.000000 ATH-0.5.0/ATH/arithmetic_average.py
--rw-rw-rw-   0        0        0      528 2024-03-07 17:24:38.000000 ATH-0.5.0/ATH/calculator.py
--rw-rw-rw-   0        0        0      196 2024-03-05 13:23:48.000000 ATH-0.5.0/ATH/env.py
--rw-rw-rw-   0        0        0      368 2024-03-03 20:21:14.000000 ATH-0.5.0/ATH/get_current_time.py
--rw-rw-rw-   0        0        0       73 2024-02-29 15:44:39.000000 ATH-0.5.0/ATH/owl.py
--rw-rw-rw-   0        0        0      347 2024-03-07 15:18:29.000000 ATH-0.5.0/ATH/qr.py
--rw-rw-rw-   0        0        0      430 2024-02-29 15:58:56.000000 ATH-0.5.0/ATH/safe.py
--rw-rw-rw-   0        0        0      113 2024-02-28 18:40:56.000000 ATH-0.5.0/ATH/scr_shot.py
--rw-rw-rw-   0        0        0      312 2024-03-03 17:45:47.000000 ATH-0.5.0/ATH/scr_shot_telegram.py
--rw-rw-rw-   0        0        0      212 2024-04-16 17:22:17.000000 ATH-0.5.0/ATH/singed.py
--rw-rw-rw-   0        0        0       96 2024-02-29 13:36:04.000000 ATH-0.5.0/ATH/sq_root.py
--rw-rw-rw-   0        0        0      167 2024-04-16 15:53:44.000000 ATH-0.5.0/ATH/telegram.py
--rw-rw-rw-   0        0        0      571 2024-05-06 15:41:13.000000 ATH-0.5.0/ATH/tts.py
--rw-rw-rw-   0        0        0       58 2024-03-03 20:32:05.000000 ATH-0.5.0/ATH/wait.py
--rw-rw-rw-   0        0        0       78 2024-03-06 13:59:40.000000 ATH-0.5.0/ATH/write.py
-drwxrwxrwx   0        0        0        0 2024-05-06 15:42:15.042568 ATH-0.5.0/ATH.egg-info/
--rw-rw-rw-   0        0        0      479 2024-05-06 15:42:14.000000 ATH-0.5.0/ATH.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      438 2024-05-06 15:42:14.000000 ATH-0.5.0/ATH.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 15:42:14.000000 ATH-0.5.0/ATH.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      137 2024-05-06 15:42:14.000000 ATH-0.5.0/ATH.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-06 15:42:14.000000 ATH-0.5.0/ATH.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      479 2024-05-06 15:42:15.043596 ATH-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-06 15:42:15.045108 ATH-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0      423 2024-05-06 15:41:47.000000 ATH-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 15:53:38.756553 ATH-0.5.1/
+drwxrwxrwx   0        0        0        0 2024-05-06 15:53:38.731964 ATH-0.5.1/ATH/
+-rw-rw-rw-   0        0        0     1287 2024-03-03 12:52:16.000000 ATH-0.5.1/ATH/DB_read.py
+-rw-rw-rw-   0        0        0      914 2024-03-02 12:38:15.000000 ATH-0.5.1/ATH/DB_send.py
+-rw-rw-rw-   0        0        0      440 2024-04-27 18:54:21.000000 ATH-0.5.1/ATH/__init__.py
+-rw-rw-rw-   0        0        0      172 2024-03-16 15:51:41.000000 ATH-0.5.1/ATH/abc123_2.py
+-rw-rw-rw-   0        0        0      125 2024-03-01 17:00:39.000000 ATH-0.5.1/ATH/arithmetic_average.py
+-rw-rw-rw-   0        0        0      528 2024-03-07 17:24:38.000000 ATH-0.5.1/ATH/calculator.py
+-rw-rw-rw-   0        0        0      196 2024-03-05 13:23:48.000000 ATH-0.5.1/ATH/env.py
+-rw-rw-rw-   0        0        0      368 2024-03-03 20:21:14.000000 ATH-0.5.1/ATH/get_current_time.py
+-rw-rw-rw-   0        0        0       73 2024-02-29 15:44:39.000000 ATH-0.5.1/ATH/owl.py
+-rw-rw-rw-   0        0        0      347 2024-03-07 15:18:29.000000 ATH-0.5.1/ATH/qr.py
+-rw-rw-rw-   0        0        0      430 2024-02-29 15:58:56.000000 ATH-0.5.1/ATH/safe.py
+-rw-rw-rw-   0        0        0      113 2024-02-28 18:40:56.000000 ATH-0.5.1/ATH/scr_shot.py
+-rw-rw-rw-   0        0        0      312 2024-03-03 17:45:47.000000 ATH-0.5.1/ATH/scr_shot_telegram.py
+-rw-rw-rw-   0        0        0      212 2024-04-16 17:22:17.000000 ATH-0.5.1/ATH/singed.py
+-rw-rw-rw-   0        0        0       96 2024-02-29 13:36:04.000000 ATH-0.5.1/ATH/sq_root.py
+-rw-rw-rw-   0        0        0      167 2024-04-16 15:53:44.000000 ATH-0.5.1/ATH/telegram.py
+-rw-rw-rw-   0        0        0      486 2024-05-06 15:53:19.000000 ATH-0.5.1/ATH/tts.py
+-rw-rw-rw-   0        0        0       58 2024-03-03 20:32:05.000000 ATH-0.5.1/ATH/wait.py
+-rw-rw-rw-   0        0        0       78 2024-03-06 13:59:40.000000 ATH-0.5.1/ATH/write.py
+drwxrwxrwx   0        0        0        0 2024-05-06 15:53:38.754759 ATH-0.5.1/ATH.egg-info/
+-rw-rw-rw-   0        0        0      479 2024-05-06 15:53:38.000000 ATH-0.5.1/ATH.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      438 2024-05-06 15:53:38.000000 ATH-0.5.1/ATH.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 15:53:38.000000 ATH-0.5.1/ATH.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      137 2024-05-06 15:53:38.000000 ATH-0.5.1/ATH.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-06 15:53:38.000000 ATH-0.5.1/ATH.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      479 2024-05-06 15:53:38.754759 ATH-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-06 15:53:38.757948 ATH-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      423 2024-05-06 15:53:37.000000 ATH-0.5.1/setup.py
```

### Comparing `ATH-0.5.0/ATH/DB_read.py` & `ATH-0.5.1/ATH/DB_read.py`

 * *Files identical despite different names*

### Comparing `ATH-0.5.0/ATH/DB_send.py` & `ATH-0.5.1/ATH/DB_send.py`

 * *Files identical despite different names*

### Comparing `ATH-0.5.0/ATH/calculator.py` & `ATH-0.5.1/ATH/calculator.py`

 * *Files identical despite different names*

