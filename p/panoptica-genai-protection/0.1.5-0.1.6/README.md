# Comparing `tmp/panoptica_genai_protection-0.1.5.tar.gz` & `tmp/panoptica_genai_protection-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panoptica_genai_protection-0.1.5.tar", last modified: Thu May  2 14:42:34 2024, max compression
+gzip compressed data, was "panoptica_genai_protection-0.1.6.tar", last modified: Sun May  5 12:42:01 2024, max compression
```

## Comparing `panoptica_genai_protection-0.1.5.tar` & `panoptica_genai_protection-0.1.6.tar`

### file list

```diff
@@ -1,4 +1,4 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:42:34.657342 panoptica_genai_protection-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-05-02 14:42:34.657342 panoptica_genai_protection-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-02 14:42:23.000000 panoptica_genai_protection-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 14:42:34.657342 panoptica_genai_protection-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:42:01.842210 panoptica_genai_protection-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-05-05 12:42:01.842210 panoptica_genai_protection-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-05 12:41:51.000000 panoptica_genai_protection-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 12:42:01.842210 panoptica_genai_protection-0.1.6/setup.cfg
```

### Comparing `panoptica_genai_protection-0.1.5/PKG-INFO` & `panoptica_genai_protection-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panoptica_genai_protection
-Version: 0.1.5
+Version: 0.1.6
 Summary: Protecting GenAI from Prompt Injection
 Author: marvin-team@cisco.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `panoptica_genai_protection-0.1.5/README.md` & `panoptica_genai_protection-0.1.6/README.md`

 * *Files identical despite different names*

