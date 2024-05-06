# Comparing `tmp/temper_syntax-0.1.1.tar.gz` & `tmp/temper_syntax-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "temper_syntax-0.1.1.tar", max compression
+gzip compressed data, was "temper_syntax-0.2.0.tar", max compression
```

## Comparing `temper_syntax-0.1.1.tar` & `temper_syntax-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,8 @@
--rw-r--r--   0        0        0      801 2023-08-04 17:21:36.942063 temper_syntax-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-04 17:21:36.937394 temper_syntax-0.1.1/temper_syntax/__init__.py
--rw-r--r--   0        0        0      126 2023-08-04 17:21:36.939912 temper_syntax-0.1.1/temper_syntax/__init__.py.map
--rw-r--r--   0        0        0       99 2023-08-04 17:21:36.939912 temper_syntax-0.1.1/temper_syntax/config.py
--rw-r--r--   0        0        0      799 2023-08-04 17:21:36.957566 temper_syntax-0.1.1/temper_syntax/config.py.map
--rw-r--r--   0        0        0     5095 2023-08-04 17:21:36.955569 temper_syntax-0.1.1/temper_syntax/pygments.py
--rw-r--r--   0        0        0     9472 2023-08-04 17:21:36.956566 temper_syntax-0.1.1/temper_syntax/pygments.py.map
--rw-r--r--   0        0        0       44 2023-08-04 17:21:36.939912 temper_syntax-0.1.1/temper_syntax/pygments__preface.py
--rw-r--r--   0        0        0     3046 2023-08-04 17:21:36.956566 temper_syntax-0.1.1/temper_syntax/pygments__preface.py.map
--rw-r--r--   0        0        0     6946 2023-08-04 17:21:36.958566 temper_syntax-0.1.1/temper_syntax/temper_pygments.py
--rw-r--r--   0        0        0    13736 2023-08-04 17:21:36.961574 temper_syntax-0.1.1/temper_syntax/temper_pygments.py.map
--rw-r--r--   0        0        0       44 2023-08-04 17:21:36.940911 temper_syntax-0.1.1/temper_syntax/temper_pygments__preface.py
--rw-r--r--   0        0        0     5120 2023-08-04 17:21:36.942063 temper_syntax-0.1.1/temper_syntax/temper_pygments__preface.py.map
--rw-r--r--   0        0        0     4049 2023-08-04 17:21:36.991575 temper_syntax-0.1.1/temper_syntax/tempermd_pygments.py
--rw-r--r--   0        0        0     6291 2023-08-04 17:21:36.992576 temper_syntax-0.1.1/temper_syntax/tempermd_pygments.py.map
--rw-r--r--   0        0        0       44 2023-08-04 17:21:36.952565 temper_syntax-0.1.1/temper_syntax/tempermd_pygments__preface.py
--rw-r--r--   0        0        0     1771 2023-08-04 17:21:36.953566 temper_syntax-0.1.1/temper_syntax/tempermd_pygments__preface.py.map
--rw-r--r--   0        0        0      382 1970-01-01 00:00:00.000000 temper_syntax-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      682 2024-05-06 17:02:14.991393 temper_syntax-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-06 17:02:14.991393 temper_syntax-0.2.0/temper_syntax/__init__.py
+-rw-r--r--   0        0        0      114 2024-05-06 17:02:14.991393 temper_syntax-0.2.0/temper_syntax/__init__.py.map
+-rw-r--r--   0        0        0     4606 2024-05-06 17:02:15.211393 temper_syntax-0.2.0/temper_syntax/pygments.py
+-rw-r--r--   0        0        0     1475 2024-05-06 17:02:15.211393 temper_syntax-0.2.0/temper_syntax/pygments.py.map
+-rw-r--r--   0        0        0     8803 2024-05-06 17:02:15.241393 temper_syntax-0.2.0/temper_syntax/temper_pygments.py
+-rw-r--r--   0        0        0     2493 2024-05-06 17:02:15.241393 temper_syntax-0.2.0/temper_syntax/temper_pygments.py.map
+-rw-r--r--   0        0        0      433 1970-01-01 00:00:00.000000 temper_syntax-0.2.0/PKG-INFO
```

