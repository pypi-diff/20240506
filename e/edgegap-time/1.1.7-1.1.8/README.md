# Comparing `tmp/edgegap_time-1.1.7.tar.gz` & `tmp/edgegap_time-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_time-1.1.7.tar", max compression
+gzip compressed data, was "edgegap_time-1.1.8.tar", max compression
```

## Comparing `edgegap_time-1.1.7.tar` & `edgegap_time-1.1.8.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0        0 2024-05-04 02:09:59.790358 edgegap_time-1.1.7/README.md
--rw-r--r--   0        0        0       17 2024-05-04 02:09:59.790358 edgegap_time-1.1.7/edgegap_time/BUILD
--rw-r--r--   0        0        0       63 2024-05-04 02:09:59.790358 edgegap_time-1.1.7/edgegap_time/__init__.py
--rw-r--r--   0        0        0     1329 2024-05-04 02:09:59.790358 edgegap_time-1.1.7/edgegap_time/_duration.py
--rw-r--r--   0        0        0      493 2024-05-04 02:11:48.363172 edgegap_time-1.1.7/pyproject.toml
--rw-r--r--   0        0        0      490 1970-01-01 00:00:00.000000 edgegap_time-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-06 20:24:27.589271 edgegap_time-1.1.8/README.md
+-rw-r--r--   0        0        0       17 2024-05-06 20:24:27.589271 edgegap_time-1.1.8/edgegap_time/BUILD
+-rw-r--r--   0        0        0      147 2024-05-06 20:24:27.589271 edgegap_time-1.1.8/edgegap_time/__init__.py
+-rw-r--r--   0        0        0     1329 2024-05-06 20:24:27.589271 edgegap_time-1.1.8/edgegap_time/_duration.py
+-rw-r--r--   0        0        0     1999 2024-05-06 20:24:27.589271 edgegap_time-1.1.8/edgegap_time/_pydantic.py
+-rw-r--r--   0        0        0      493 2024-05-06 20:26:59.182139 edgegap_time-1.1.8/pyproject.toml
+-rw-r--r--   0        0        0      490 1970-01-01 00:00:00.000000 edgegap_time-1.1.8/PKG-INFO
```

### Comparing `edgegap_time-1.1.7/edgegap_time/_duration.py` & `edgegap_time-1.1.8/edgegap_time/_duration.py`

 * *Files identical despite different names*

