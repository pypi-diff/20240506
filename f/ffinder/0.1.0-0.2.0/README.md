# Comparing `tmp/ffinder-0.1.0.tar.gz` & `tmp/ffinder-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffinder-0.1.0.tar", max compression
+gzip compressed data, was "ffinder-0.2.0.tar", max compression
```

## Comparing `ffinder-0.1.0.tar` & `ffinder-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       14 2024-04-15 17:49:57.217301 ffinder-0.1.0/README.md
--rw-r--r--   0        0        0      276 2024-05-06 17:59:49.839537 ffinder-0.1.0/file_finder/cli.py
--rw-r--r--   0        0        0      231 2024-05-06 17:49:16.893628 ffinder-0.1.0/file_finder/constants.py
--rw-r--r--   0        0        0      153 2024-05-06 16:28:30.256612 ffinder-0.1.0/file_finder/exceptions.py
--rw-r--r--   0        0        0     2805 2024-05-06 17:52:45.256850 ffinder-0.1.0/file_finder/finder.py
--rw-r--r--   0        0        0     2384 2024-05-06 17:48:58.737702 ffinder-0.1.0/file_finder/utils.py
--rw-r--r--   0        0        0      400 2024-05-06 18:11:04.569791 ffinder-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      383 1970-01-01 00:00:00.000000 ffinder-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1559 2024-05-06 18:23:48.364593 ffinder-0.2.0/README.md
+-rw-r--r--   0        0        0      276 2024-05-06 17:59:49.839537 ffinder-0.2.0/file_finder/cli.py
+-rw-r--r--   0        0        0      231 2024-05-06 17:49:16.893628 ffinder-0.2.0/file_finder/constants.py
+-rw-r--r--   0        0        0      153 2024-05-06 16:28:30.256612 ffinder-0.2.0/file_finder/exceptions.py
+-rw-r--r--   0        0        0     2805 2024-05-06 17:52:45.256850 ffinder-0.2.0/file_finder/finder.py
+-rw-r--r--   0        0        0     2384 2024-05-06 17:48:58.737702 ffinder-0.2.0/file_finder/utils.py
+-rw-r--r--   0        0        0      400 2024-05-06 18:35:36.791439 ffinder-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1928 1970-01-01 00:00:00.000000 ffinder-0.2.0/PKG-INFO
```

### Comparing `ffinder-0.1.0/file_finder/finder.py` & `ffinder-0.2.0/file_finder/finder.py`

 * *Files identical despite different names*

### Comparing `ffinder-0.1.0/file_finder/utils.py` & `ffinder-0.2.0/file_finder/utils.py`

 * *Files identical despite different names*

