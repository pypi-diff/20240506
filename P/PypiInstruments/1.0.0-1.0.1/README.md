# Comparing `tmp/PypiInstruments-1.0.0.tar.gz` & `tmp/PypiInstruments-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PypiInstruments-1.0.0.tar", last modified: Mon May  6 09:44:51 2024, max compression
+gzip compressed data, was "PypiInstruments-1.0.1.tar", last modified: Mon May  6 09:55:53 2024, max compression
```

## Comparing `PypiInstruments-1.0.0.tar` & `PypiInstruments-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 09:44:51.203991 PypiInstruments-1.0.0/
--rw-rw-rw-   0        0        0       83 2024-05-06 09:44:51.202983 PypiInstruments-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-06 09:44:51.200460 PypiInstruments-1.0.0/PypiInstruments.egg-info/
--rw-rw-rw-   0        0        0       83 2024-05-06 09:44:51.000000 PypiInstruments-1.0.0/PypiInstruments.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2024-05-06 09:44:51.000000 PypiInstruments-1.0.0/PypiInstruments.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 09:44:51.000000 PypiInstruments-1.0.0/PypiInstruments.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-06 09:44:51.000000 PypiInstruments-1.0.0/PypiInstruments.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        4 2024-05-06 09:44:51.000000 PypiInstruments-1.0.0/PypiInstruments.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-06 09:44:51.201792 PypiInstruments-1.0.0/one/
--rw-rw-rw-   0        0        0        0 2024-05-04 13:27:09.000000 PypiInstruments-1.0.0/one/__init__.py
--rw-rw-rw-   0        0        0      104 2024-05-04 13:35:48.000000 PypiInstruments-1.0.0/one/hello.py
--rw-rw-rw-   0        0        0        0 2024-05-04 13:27:19.000000 PypiInstruments-1.0.0/one/main.py
--rw-rw-rw-   0        0        0       42 2024-05-06 09:44:51.203991 PypiInstruments-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      273 2024-05-06 09:44:44.000000 PypiInstruments-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:55:53.451472 PypiInstruments-1.0.1/
+-rw-rw-rw-   0        0        0       83 2024-05-06 09:55:53.451472 PypiInstruments-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-06 09:55:53.445052 PypiInstruments-1.0.1/PypiInstruments.egg-info/
+-rw-rw-rw-   0        0        0       83 2024-05-06 09:55:53.000000 PypiInstruments-1.0.1/PypiInstruments.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      436 2024-05-06 09:55:53.000000 PypiInstruments-1.0.1/PypiInstruments.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 09:55:53.000000 PypiInstruments-1.0.1/PypiInstruments.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-06 09:55:53.000000 PypiInstruments-1.0.1/PypiInstruments.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       16 2024-05-06 09:55:53.000000 PypiInstruments-1.0.1/PypiInstruments.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 09:55:53.448903 PypiInstruments-1.0.1/instruments/
+-rw-rw-rw-   0        0        0     2132 2024-04-29 07:50:25.000000 PypiInstruments-1.0.1/instruments/DP821A.py
+-rw-rw-rw-   0        0        0     3827 2024-05-06 09:48:58.000000 PypiInstruments-1.0.1/instruments/Multimemter.py
+-rw-rw-rw-   0        0        0      979 2024-04-30 09:41:34.000000 PypiInstruments-1.0.1/instruments/SMU_Examples.py
+-rw-rw-rw-   0        0        0      141 2024-05-06 09:53:39.000000 PypiInstruments-1.0.1/instruments/__init__.py
+-rw-rw-rw-   0        0        0      297 2024-04-28 10:28:19.000000 PypiInstruments-1.0.1/instruments/device_scan.py
+-rw-rw-rw-   0        0        0      740 2024-04-29 02:13:11.000000 PypiInstruments-1.0.1/instruments/instruments_name.py
+-rw-rw-rw-   0        0        0    11510 2024-05-06 09:48:58.000000 PypiInstruments-1.0.1/instruments/smu_keithley_2450.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:55:53.451472 PypiInstruments-1.0.1/one/
+-rw-rw-rw-   0        0        0        0 2024-05-06 09:46:19.000000 PypiInstruments-1.0.1/one/__init__.py
+-rw-rw-rw-   0        0        0      104 2024-05-04 13:35:48.000000 PypiInstruments-1.0.1/one/hello.py
+-rw-rw-rw-   0        0        0        0 2024-05-04 13:27:19.000000 PypiInstruments-1.0.1/one/main.py
+-rw-rw-rw-   0        0        0       42 2024-05-06 09:55:53.451472 PypiInstruments-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      273 2024-05-06 09:55:18.000000 PypiInstruments-1.0.1/setup.py
```

