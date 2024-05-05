# Comparing `tmp/dfa_sampler-0.1.0.tar.gz` & `tmp/dfa_sampler-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfa_sampler-0.1.0.tar", max compression
+gzip compressed data, was "dfa_sampler-0.1.1.tar", max compression
```

## Comparing `dfa_sampler-0.1.0.tar` & `dfa_sampler-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1082 2024-05-05 16:07:42.823033 dfa_sampler-0.1.0/LICENSE
--rw-r--r--   0        0        0       87 2024-05-05 16:07:42.823033 dfa_sampler-0.1.0/README.md
--rw-r--r--   0        0        0       38 2024-05-05 21:51:14.278477 dfa_sampler-0.1.0/dfa_sampler/__init__.py
--rw-r--r--   0        0        0     2054 2024-05-05 21:53:13.377254 dfa_sampler-0.1.0/dfa_sampler/dfa_sampler.py
--rw-r--r--   0        0        0      508 2024-05-05 16:19:36.978708 dfa_sampler-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      702 1970-01-01 00:00:00.000000 dfa_sampler-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-05-05 16:07:42.823033 dfa_sampler-0.1.1/LICENSE
+-rw-r--r--   0        0        0      936 2024-05-05 22:16:38.911473 dfa_sampler-0.1.1/README.md
+-rw-r--r--   0        0        0       38 2024-05-05 21:51:14.278477 dfa_sampler-0.1.1/dfa_sampler/__init__.py
+-rw-r--r--   0        0        0     2492 2024-05-05 22:21:16.232991 dfa_sampler-0.1.1/dfa_sampler/dfa_sampler.py
+-rw-r--r--   0        0        0      508 2024-05-05 22:24:17.264671 dfa_sampler-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1551 1970-01-01 00:00:00.000000 dfa_sampler-0.1.1/PKG-INFO
```

### Comparing `dfa_sampler-0.1.0/LICENSE` & `dfa_sampler-0.1.1/LICENSE`

 * *Files identical despite different names*

