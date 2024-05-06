# Comparing `tmp/e2edge-0.1.2.tar.gz` & `tmp/e2edge-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2edge-0.1.2.tar", max compression
+gzip compressed data, was "e2edge-0.1.3.tar", max compression
```

## Comparing `e2edge-0.1.2.tar` & `e2edge-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      275 2024-05-06 06:13:06.465453 e2edge-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        6 2024-04-25 17:20:52.754953 e2edge-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-04-25 16:42:31.748713 e2edge-0.1.2/src/e2edge/__init__.py
--rw-r--r--   0        0        0      140 2024-05-06 06:12:50.258793 e2edge-0.1.2/src/e2edge/sample_module.py
--rw-r--r--   0        0        0      388 1970-01-01 00:00:00.000000 e2edge-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      275 2024-05-06 06:27:25.207337 e2edge-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        6 2024-04-25 17:20:52.754953 e2edge-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-25 16:42:31.748713 e2edge-0.1.3/src/e2edge/__init__.py
+-rw-r--r--   0        0        0      141 2024-05-06 06:27:29.621517 e2edge-0.1.3/src/e2edge/sample_module.py
+-rw-r--r--   0        0        0      388 1970-01-01 00:00:00.000000 e2edge-0.1.3/PKG-INFO
```

