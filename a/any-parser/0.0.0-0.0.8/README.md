# Comparing `tmp/any_parser-0.0.0.tar.gz` & `tmp/any_parser-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "any_parser-0.0.0.tar", max compression
+gzip compressed data, was "any_parser-0.0.8.tar", max compression
```

## Comparing `any_parser-0.0.0.tar` & `any_parser-0.0.8.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0        0 2024-05-01 06:42:02.758916 any_parser-0.0.0/README.md
--rw-r--r--   0        0        0        0 2024-05-01 06:42:02.758868 any_parser-0.0.0/any_parser/__init__.py
--rw-r--r--   0        0        0      367 2024-05-01 06:43:37.449437 any_parser-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 any_parser-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1882 2024-05-06 06:10:36.107663 any_parser-0.0.8/README.md
+-rw-r--r--   0        0        0       86 2024-05-06 06:10:36.107818 any_parser-0.0.8/any_parser/__init__.py
+-rw-r--r--   0        0        0     3481 2024-05-06 06:10:36.107942 any_parser-0.0.8/any_parser/base.py
+-rw-r--r--   0        0        0      388 2024-05-06 06:10:36.116825 any_parser-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2538 1970-01-01 00:00:00.000000 any_parser-0.0.8/PKG-INFO
```

