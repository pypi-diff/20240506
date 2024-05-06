# Comparing `tmp/psssodls-0.1.0.tar.gz` & `tmp/psssodls-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psssodls-0.1.0.tar", max compression
+gzip compressed data, was "dist/psssodls-0.3.tar", last modified: Mon Jun 29 14:06:18 2020, max compression
```

## Comparing `psssodls-0.1.0.tar` & `psssodls-0.3.tar`

### file list

```diff
@@ -1,7 +1,15 @@
--rwxr-xr-x   0        0        0     1076 2024-05-06 15:51:05.330045 psssodls-0.1.0/LICENSE
--rw-r--r--   0        0        0       49 2024-05-06 15:51:05.330045 psssodls-0.1.0/README.md
--rw-r--r--   0        0        0      397 2024-05-06 15:51:05.330045 psssodls-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      110 2024-05-06 15:51:05.330045 psssodls-0.1.0/src/psssodls/__init__.py
--rw-r--r--   0        0        0     1171 2024-05-06 15:51:05.330045 psssodls-0.1.0/src/psssodls/constraints.py
--rw-r--r--   0        0        0     2465 2024-05-06 15:51:05.330045 psssodls-0.1.0/src/psssodls/main.py
--rw-r--r--   0        0        0      558 1970-01-01 00:00:00.000000 psssodls-0.1.0/PKG-INFO
+drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2020-06-29 14:06:18.000000 psssodls-0.3/
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      667 2020-06-29 14:06:18.000000 psssodls-0.3/PKG-INFO
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      109 2020-06-29 13:34:57.000000 psssodls-0.3/README.md
+drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2020-06-29 14:06:18.000000 psssodls-0.3/bin/
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      392 2020-06-29 13:39:34.000000 psssodls-0.3/bin/psssodls
+drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2020-06-29 14:06:18.000000 psssodls-0.3/psssodls/
+-rwxr-xr-x   0 matthew   (1000) matthew   (1000)     3224 2020-06-29 13:37:21.000000 psssodls-0.3/psssodls/__init__.py
+drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2020-06-29 14:06:18.000000 psssodls-0.3/psssodls.egg-info/
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      667 2020-06-29 14:06:18.000000 psssodls-0.3/psssodls.egg-info/PKG-INFO
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      211 2020-06-29 14:06:18.000000 psssodls-0.3/psssodls.egg-info/SOURCES.txt
+-rw-r--r--   0 matthew   (1000) matthew   (1000)        1 2020-06-29 14:06:18.000000 psssodls-0.3/psssodls.egg-info/dependency_links.txt
+-rw-r--r--   0 matthew   (1000) matthew   (1000)        1 2020-06-29 14:06:18.000000 psssodls-0.3/psssodls.egg-info/not-zip-safe
+-rw-r--r--   0 matthew   (1000) matthew   (1000)        9 2020-06-29 14:06:18.000000 psssodls-0.3/psssodls.egg-info/top_level.txt
+-rw-r--r--   0 matthew   (1000) matthew   (1000)       38 2020-06-29 14:06:18.000000 psssodls-0.3/setup.cfg
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      770 2020-06-29 14:04:56.000000 psssodls-0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

