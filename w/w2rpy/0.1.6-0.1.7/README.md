# Comparing `tmp/w2rpy-0.1.6.tar.gz` & `tmp/w2rpy-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "w2rpy-0.1.6.tar", last modified: Mon May  6 19:37:18 2024, max compression
+gzip compressed data, was "w2rpy-0.1.7.tar", last modified: Mon May  6 19:46:42 2024, max compression
```

## Comparing `w2rpy-0.1.6.tar` & `w2rpy-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 19:37:18.800166 w2rpy-0.1.6/
--rw-rw-rw-   0        0        0     1062 2024-05-01 20:18:19.000000 w2rpy-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      416 2024-05-06 19:37:18.800166 w2rpy-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0        7 2024-05-01 21:03:28.000000 w2rpy-0.1.6/README.md
--rw-rw-rw-   0        0        0       86 2024-05-06 19:37:18.801175 w2rpy-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      722 2024-05-06 19:36:37.000000 w2rpy-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 19:37:18.789167 w2rpy-0.1.6/w2rpy/
--rw-rw-rw-   0        0        0      114 2024-05-01 21:04:56.000000 w2rpy-0.1.6/w2rpy/__init__.py
--rw-rw-rw-   0        0        0    28193 2024-05-06 19:30:27.000000 w2rpy-0.1.6/w2rpy/w2rpy.py
-drwxrwxrwx   0        0        0        0 2024-05-06 19:37:18.799171 w2rpy-0.1.6/w2rpy.egg-info/
--rw-rw-rw-   0        0        0      416 2024-05-06 19:37:18.000000 w2rpy-0.1.6/w2rpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2024-05-06 19:37:18.000000 w2rpy-0.1.6/w2rpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 19:37:18.000000 w2rpy-0.1.6/w2rpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-06 19:37:18.000000 w2rpy-0.1.6/w2rpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-06 19:37:18.000000 w2rpy-0.1.6/w2rpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 19:46:42.609265 w2rpy-0.1.7/
+-rw-rw-rw-   0        0        0     1062 2024-05-01 20:18:19.000000 w2rpy-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0      379 2024-05-06 19:46:42.608260 w2rpy-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2024-05-01 21:03:28.000000 w2rpy-0.1.7/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-06 19:46:42.610260 w2rpy-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      640 2024-05-06 19:44:23.000000 w2rpy-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 19:46:42.608260 w2rpy-0.1.7/w2rpy.egg-info/
+-rw-rw-rw-   0        0        0      379 2024-05-06 19:46:42.000000 w2rpy-0.1.7/w2rpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2024-05-06 19:46:42.000000 w2rpy-0.1.7/w2rpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 19:46:42.000000 w2rpy-0.1.7/w2rpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-06 19:46:42.000000 w2rpy-0.1.7/w2rpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-06 19:46:42.000000 w2rpy-0.1.7/w2rpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    28193 2024-05-06 19:30:27.000000 w2rpy-0.1.7/w2rpy.py
```

### Comparing `w2rpy-0.1.6/LICENSE` & `w2rpy-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `w2rpy-0.1.6/w2rpy/w2rpy.py` & `w2rpy-0.1.7/w2rpy.py`

 * *Files identical despite different names*

