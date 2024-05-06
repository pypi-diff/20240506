# Comparing `tmp/aidot-0.1.0.tar.gz` & `tmp/aidot-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aidot-0.1.0.tar", last modified: Mon May  6 02:51:41 2024, max compression
+gzip compressed data, was "aidot-0.1.1.tar", last modified: Mon May  6 03:56:56 2024, max compression
```

## Comparing `aidot-0.1.0.tar` & `aidot-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 02:51:41.810066 aidot-0.1.0/
--rw-rw-rw-   0        0        0     1141 2024-02-23 09:09:51.000000 aidot-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      488 2024-05-06 02:51:41.776063 aidot-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       84 2024-05-06 02:35:01.000000 aidot-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 02:51:41.744063 aidot-0.1.0/aidot/
--rw-rw-rw-   0        0        0        0 2024-05-06 01:51:06.000000 aidot-0.1.0/aidot/__init__.py
--rw-rw-rw-   0        0        0      950 2024-05-06 01:51:06.000000 aidot-0.1.0/aidot/aes_utils.py
--rw-rw-rw-   0        0        0     2359 2024-05-06 01:51:06.000000 aidot-0.1.0/aidot/discover.py
--rw-rw-rw-   0        0        0     9527 2024-05-06 01:51:06.000000 aidot-0.1.0/aidot/lan.py
--rw-rw-rw-   0        0        0      436 2024-05-06 01:51:06.000000 aidot-0.1.0/aidot/login_const.py
--rw-rw-rw-   0        0        0     5610 2024-05-06 01:51:06.000000 aidot-0.1.0/aidot/login_control.py
--rw-rw-rw-   0        0        0      351 2024-05-06 01:51:06.000000 aidot-0.1.0/aidot/login_data.py
-drwxrwxrwx   0        0        0        0 2024-05-06 02:51:41.773064 aidot-0.1.0/aidot.egg-info/
--rw-rw-rw-   0        0        0      488 2024-05-06 02:51:41.000000 aidot-0.1.0/aidot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      344 2024-05-06 02:51:41.000000 aidot-0.1.0/aidot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 02:51:41.000000 aidot-0.1.0/aidot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-05-06 02:51:41.000000 aidot-0.1.0/aidot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2024-05-06 02:51:41.000000 aidot-0.1.0/aidot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-06 02:51:41.000000 aidot-0.1.0/aidot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-05-06 02:51:41.817067 aidot-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      750 2024-05-06 02:48:18.000000 aidot-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:56:56.307393 aidot-0.1.1/
+-rw-rw-rw-   0        0        0     1141 2024-02-23 09:09:51.000000 aidot-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      488 2024-05-06 03:56:56.275971 aidot-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       84 2024-05-06 02:35:01.000000 aidot-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 03:56:56.241941 aidot-0.1.1/aidot/
+-rw-rw-rw-   0        0        0        0 2024-05-06 01:51:06.000000 aidot-0.1.1/aidot/__init__.py
+-rw-rw-rw-   0        0        0      950 2024-05-06 01:51:06.000000 aidot-0.1.1/aidot/aes_utils.py
+-rw-rw-rw-   0        0        0     2359 2024-05-06 01:51:06.000000 aidot-0.1.1/aidot/discover.py
+-rw-rw-rw-   0        0        0     9527 2024-05-06 01:51:06.000000 aidot-0.1.1/aidot/lan.py
+-rw-rw-rw-   0        0        0      436 2024-05-06 01:51:06.000000 aidot-0.1.1/aidot/login_const.py
+-rw-rw-rw-   0        0        0     5610 2024-05-06 01:51:06.000000 aidot-0.1.1/aidot/login_control.py
+-rw-rw-rw-   0        0        0      351 2024-05-06 01:51:06.000000 aidot-0.1.1/aidot/login_data.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:56:56.272561 aidot-0.1.1/aidot.egg-info/
+-rw-rw-rw-   0        0        0      488 2024-05-06 03:56:55.000000 aidot-0.1.1/aidot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2024-05-06 03:56:56.000000 aidot-0.1.1/aidot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 03:56:55.000000 aidot-0.1.1/aidot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-05-06 03:56:55.000000 aidot-0.1.1/aidot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-06 03:56:55.000000 aidot-0.1.1/aidot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-05-06 03:56:56.311427 aidot-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      635 2024-05-06 03:56:09.000000 aidot-0.1.1/setup.py
```

### Comparing `aidot-0.1.0/LICENSE` & `aidot-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aidot-0.1.0/aidot/aes_utils.py` & `aidot-0.1.1/aidot/aes_utils.py`

 * *Files identical despite different names*

### Comparing `aidot-0.1.0/aidot/discover.py` & `aidot-0.1.1/aidot/discover.py`

 * *Files identical despite different names*

### Comparing `aidot-0.1.0/aidot/lan.py` & `aidot-0.1.1/aidot/lan.py`

 * *Files identical despite different names*

### Comparing `aidot-0.1.0/aidot/login_control.py` & `aidot-0.1.1/aidot/login_control.py`

 * *Files identical despite different names*

