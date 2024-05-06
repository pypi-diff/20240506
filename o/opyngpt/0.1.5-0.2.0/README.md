# Comparing `tmp/opyngpt-0.1.5.tar.gz` & `tmp/opyngpt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opyngpt-0.1.5.tar", last modified: Fri Dec 15 11:13:04 2023, max compression
+gzip compressed data, was "opyngpt-0.2.0.tar", last modified: Mon May  6 17:46:34 2024, max compression
```

## Comparing `opyngpt-0.1.5.tar` & `opyngpt-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-12-15 11:13:04.667737 opyngpt-0.1.5/
--rw-rw-rw-   0        0        0     1893 2023-12-15 11:13:04.667737 opyngpt-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1668 2023-12-10 07:46:17.000000 opyngpt-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-12-15 11:13:04.661254 opyngpt-0.1.5/opyngpt/
--rw-rw-rw-   0        0        0       26 2023-12-01 17:52:45.000000 opyngpt-0.1.5/opyngpt/__init__.py
--rw-rw-rw-   0        0        0    35266 2023-12-15 11:12:18.000000 opyngpt-0.1.5/opyngpt/chat.py
-drwxrwxrwx   0        0        0        0 2023-12-15 11:13:04.666288 opyngpt-0.1.5/opyngpt.egg-info/
--rw-rw-rw-   0        0        0     1893 2023-12-15 11:13:04.000000 opyngpt-0.1.5/opyngpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2023-12-15 11:13:04.000000 opyngpt-0.1.5/opyngpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-15 11:13:04.000000 opyngpt-0.1.5/opyngpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-12-15 11:13:04.000000 opyngpt-0.1.5/opyngpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-12-15 11:13:04.000000 opyngpt-0.1.5/opyngpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-12-15 11:13:04.667737 opyngpt-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     2054 2023-12-15 11:12:28.000000 opyngpt-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 17:46:34.733947 opyngpt-0.2.0/
+-rw-rw-rw-   0        0        0     3429 2024-05-06 17:46:34.732941 opyngpt-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3102 2024-05-06 17:44:38.000000 opyngpt-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 17:46:34.727637 opyngpt-0.2.0/opyngpt/
+-rw-rw-rw-   0        0        0       26 2024-05-06 17:12:53.000000 opyngpt-0.2.0/opyngpt/__init__.py
+-rw-rw-rw-   0        0        0     1626 2024-05-06 17:27:21.000000 opyngpt-0.2.0/opyngpt/chat.py
+drwxrwxrwx   0        0        0        0 2024-05-06 17:46:34.731506 opyngpt-0.2.0/opyngpt.egg-info/
+-rw-rw-rw-   0        0        0     3429 2024-05-06 17:46:34.000000 opyngpt-0.2.0/opyngpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2024-05-06 17:46:34.000000 opyngpt-0.2.0/opyngpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 17:46:34.000000 opyngpt-0.2.0/opyngpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-06 17:46:34.000000 opyngpt-0.2.0/opyngpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-06 17:46:34.000000 opyngpt-0.2.0/opyngpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 17:46:34.733947 opyngpt-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     3615 2024-05-06 17:42:24.000000 opyngpt-0.2.0/setup.py
```

