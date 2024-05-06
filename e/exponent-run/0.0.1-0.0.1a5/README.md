# Comparing `tmp/exponent_run-0.0.1.tar.gz` & `tmp/exponent_run-0.0.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "exponent_run-0.0.1a5.tar", max compression
```

## Comparing `exponent_run-0.0.1.tar` & `exponent_run-0.0.1a5.tar`

### file list

```diff
@@ -1,5 +1,10 @@
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 exponent_run-0.0.1/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 exponent_run-0.0.1/src/exponent_run/__init__.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 exponent_run-0.0.1/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 exponent_run-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 exponent_run-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       57 2024-05-03 23:47:20.021413 exponent_run-0.0.1a5/exponent/__init__.py
+-rw-r--r--   0        0        0     3099 2024-05-04 21:27:55.629978 exponent_run-0.0.1a5/exponent/cli.py
+-rw-r--r--   0        0        0      501 2024-05-04 21:27:55.630193 exponent_run-0.0.1a5/exponent/core/config.py
+-rw-r--r--   0        0        0     2435 2024-05-04 21:27:55.630339 exponent_run-0.0.1a5/exponent/core/remote_execution/client.py
+-rw-r--r--   0        0        0      747 2024-05-04 21:27:55.630473 exponent_run-0.0.1a5/exponent/core/remote_execution/types.py
+-rw-r--r--   0        0        0        0 2024-05-03 23:47:19.960349 exponent_run-0.0.1a5/exponent/tests/__init__.py
+-rw-r--r--   0        0        0      718 2024-05-04 21:27:55.630751 exponent_run-0.0.1a5/exponent/tests/conftest.py
+-rw-r--r--   0        0        0      464 2024-05-04 21:27:55.630962 exponent_run-0.0.1a5/exponent/tests/test_cli.py
+-rw-r--r--   0        0        0     1422 2024-05-06 21:32:49.919856 exponent_run-0.0.1a5/pyproject.toml
+-rw-r--r--   0        0        0      516 1970-01-01 00:00:00.000000 exponent_run-0.0.1a5/PKG-INFO
```

