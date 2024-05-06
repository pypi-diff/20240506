# Comparing `tmp/plone.app.linkintegrity-4.0.3.tar.gz` & `tmp/plone_app_linkintegrity-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.linkintegrity-4.0.3.tar", last modified: Fri Sep 29 12:04:28 2023, max compression
+gzip compressed data, was "plone_app_linkintegrity-4.0.4.tar", last modified: Mon May  6 12:50:20 2024, max compression
```

## Comparing `plone.app.linkintegrity-4.0.3.tar` & `plone_app_linkintegrity-4.0.4.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-09-29 12:04:28.684173 plone.app.linkintegrity-4.0.3/
--rw-r--r--   0 timo       (501) staff       (20)    18996 2023-09-29 12:04:27.000000 plone.app.linkintegrity-4.0.3/CHANGES.rst
--rw-r--r--   0 timo       (501) staff       (20)       70 2023-09-29 12:04:27.000000 plone.app.linkintegrity-4.0.3/CONTRIBUTING.rst
--rw-r--r--   0 timo       (501) staff       (20)      150 2023-09-29 12:04:27.000000 plone.app.linkintegrity-4.0.3/MANIFEST.in
--rw-r--r--   0 timo       (501) staff       (20)    24181 2023-09-29 12:04:28.683807 plone.app.linkintegrity-4.0.3/PKG-INFO
--rw-r--r--   0 timo       (501) staff       (20)     4032 2023-09-29 12:04:27.000000 plone.app.linkintegrity-4.0.3/README.rst
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-09-29 12:04:28.671205 plone.app.linkintegrity-4.0.3/docs/
--rw-r--r--   0 timo       (501) staff       (20)    15220 2023-09-29 12:04:27.000000 plone.app.linkintegrity-4.0.3/docs/LICENSE.GPL
--rw-r--r--   0 timo       (501) staff       (20)      685 2023-09-29 12:04:27.000000 plone.app.linkintegrity-4.0.3/docs/LICENSE.txt
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-09-29 12:04:28.671486 plone.app.linkintegrity-4.0.3/plone/
--rw-r--r--   0 timo       (501) staff       (20)       56 2023-09-29 12:04:27.000000 plone.app.linkintegrity-4.0.3/plone/__init__.py
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-09-29 12:04:28.674117 plone.app.linkintegrity-4.0.3/plone/app/
--rw-r--r--   0 timo       (501) staff       (20)       56 2023-09-29 12:04:27.000000 plone.app.linkintegrity-4.0.3/plone/app/__init__.py
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-09-29 12:04:28.677105 plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/
--rw-r--r--   0 timo       (501) staff       (20)        0 2023-09-29 12:04:27.000000 plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/__init__.py
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-09-29 12:04:28.678793 plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/browser/
--rw-r--r--   0 timo       (501) staff       (20)        0 2023-09-29 12:04:27.000000 plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/browser/__init__.py
--rw-r--r--   0 timo       (501) staff       (20)      498 2023-09-29 12:04:27.000000 plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/browser/configure.zcml
--rw-r--r--   0 timo       (501) staff       (20)     4158 2023-09-29 12:04:27.000000 plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/browser/delete_confirmation_info.pt
--rw-r--r--   0 timo       (501) staff       (20)     8053 2023-09-29 12:04:27.000000 plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/browser/info.py
--rw-r--r--   0 timo       (501) staff       (20)     1581 2023-09-29 12:04:27.000000 plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/browser/update.pt
--rw-r--r--   0 timo       (501) staff       (20)     2521 2023-09-29 12:04:27.000000 plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/browser/update.py
--rw-r--r--   0 timo       (501) staff       (20)     1593 2023-09-29 12:04:27.000000 plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/configure.zcml
--rw-r--r--   0 timo       (501) staff       (20)      599 2023-09-29 12:04:27.000000 plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/exceptions.py
--rw-r--r--   0 timo       (501) staff       (20)     6243 2023-09-29 12:04:27.000000 plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/handlers.py
--rw-r--r--   0 timo       (501) staff       (20)      174 2023-09-29 12:04:27.000000 plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/interfaces.py
--rw-r--r--   0 timo       (501) staff       (20)     1887 2023-09-29 12:04:27.000000 plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/parser.py
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-09-29 12:04:28.668130 plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/profiles/
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-09-29 12:04:28.680662 plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/profiles/default/
--rw-r--r--   0 timo       (501) staff       (20)      253 2023-09-29 12:04:27.000000 plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/profiles/default/metadata.xml
--rw-r--r--   0 timo       (501) staff       (20)        0 2023-09-29 12:04:27.000000 plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/profiles/default/ploneapplinkintegrity_default.txt
--rw-r--r--   0 timo       (501) staff       (20)     1533 2023-09-29 12:04:27.000000 plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/retriever.py
--rw-r--r--   0 timo       (501) staff       (20)     2965 2023-09-29 12:04:27.000000 plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/testing.py
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-09-29 12:04:28.683398 plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/tests/
--rw-r--r--   0 timo       (501) staff       (20)      201 2023-09-29 12:04:27.000000 plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/tests/__init__.py
--rw-r--r--   0 timo       (501) staff       (20)     4324 2023-09-29 12:04:27.000000 plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/tests/test_circular.py
--rw-r--r--   0 timo       (501) staff       (20)    17112 2023-09-29 12:04:27.000000 plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/tests/test_functional.py
--rw-r--r--   0 timo       (501) staff       (20)     2352 2023-09-29 12:04:27.000000 plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/tests/test_handlers.py
--rw-r--r--   0 timo       (501) staff       (20)     2467 2023-09-29 12:04:27.000000 plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/tests/test_imagescales.py
--rw-r--r--   0 timo       (501) staff       (20)     1451 2023-09-29 12:04:27.000000 plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/tests/test_info.py
--rw-r--r--   0 timo       (501) staff       (20)    10297 2023-09-29 12:04:27.000000 plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/tests/test_references.py
--rw-r--r--   0 timo       (501) staff       (20)      167 2023-09-29 12:04:27.000000 plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/tests/utils.py
--rw-r--r--   0 timo       (501) staff       (20)     2534 2023-09-29 12:04:27.000000 plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/utils.py
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-09-29 12:04:28.673844 plone.app.linkintegrity-4.0.3/plone.app.linkintegrity.egg-info/
--rw-r--r--   0 timo       (501) staff       (20)    24181 2023-09-29 12:04:28.000000 plone.app.linkintegrity-4.0.3/plone.app.linkintegrity.egg-info/PKG-INFO
--rw-r--r--   0 timo       (501) staff       (20)     1631 2023-09-29 12:04:28.000000 plone.app.linkintegrity-4.0.3/plone.app.linkintegrity.egg-info/SOURCES.txt
--rw-r--r--   0 timo       (501) staff       (20)        1 2023-09-29 12:04:28.000000 plone.app.linkintegrity-4.0.3/plone.app.linkintegrity.egg-info/dependency_links.txt
--rw-r--r--   0 timo       (501) staff       (20)       40 2023-09-29 12:04:28.000000 plone.app.linkintegrity-4.0.3/plone.app.linkintegrity.egg-info/entry_points.txt
--rw-r--r--   0 timo       (501) staff       (20)       16 2023-09-29 12:04:28.000000 plone.app.linkintegrity-4.0.3/plone.app.linkintegrity.egg-info/namespace_packages.txt
--rw-r--r--   0 timo       (501) staff       (20)        1 2023-09-29 12:04:28.000000 plone.app.linkintegrity-4.0.3/plone.app.linkintegrity.egg-info/not-zip-safe
--rw-r--r--   0 timo       (501) staff       (20)      300 2023-09-29 12:04:28.000000 plone.app.linkintegrity-4.0.3/plone.app.linkintegrity.egg-info/requires.txt
--rw-r--r--   0 timo       (501) staff       (20)        6 2023-09-29 12:04:28.000000 plone.app.linkintegrity-4.0.3/plone.app.linkintegrity.egg-info/top_level.txt
--rw-r--r--   0 timo       (501) staff       (20)     3803 2023-09-29 12:04:27.000000 plone.app.linkintegrity-4.0.3/pyproject.toml
--rw-r--r--   0 timo       (501) staff       (20)       38 2023-09-29 12:04:28.684274 plone.app.linkintegrity-4.0.3/setup.cfg
--rw-r--r--   0 timo       (501) staff       (20)     2206 2023-09-29 12:04:27.000000 plone.app.linkintegrity-4.0.3/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:50:20.053295 plone_app_linkintegrity-4.0.4/
+-rw-r--r--   0 maurits    (501) staff       (20)    19202 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      150 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    25020 2024-05-06 12:50:20.052895 plone_app_linkintegrity-4.0.4/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     4032 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:50:20.038930 plone_app_linkintegrity-4.0.4/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      685 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:50:20.039252 plone_app_linkintegrity-4.0.4/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:50:20.042878 plone_app_linkintegrity-4.0.4/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:50:20.045896 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:50:20.048072 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      498 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     4158 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/browser/delete_confirmation_info.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     6854 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/browser/info.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1581 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/browser/update.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2521 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/browser/update.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1593 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      599 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/exceptions.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6243 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/handlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)      174 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1887 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/parser.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:50:20.034179 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:50:20.048617 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      253 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/profiles/default/ploneapplinkintegrity_default.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1534 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/retriever.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2965 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:50:20.051535 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)      201 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4324 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/tests/test_circular.py
+-rw-r--r--   0 maurits    (501) staff       (20)    17114 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/tests/test_functional.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2352 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/tests/test_handlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2467 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/tests/test_imagescales.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1451 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/tests/test_info.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11261 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/tests/test_references.py
+-rw-r--r--   0 maurits    (501) staff       (20)      167 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/tests/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2534 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/utils.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:50:20.052098 plone_app_linkintegrity-4.0.4/plone.app.linkintegrity.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    25020 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone.app.linkintegrity.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1631 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone.app.linkintegrity.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone.app.linkintegrity.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone.app.linkintegrity.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone.app.linkintegrity.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone.app.linkintegrity.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      305 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone.app.linkintegrity.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone.app.linkintegrity.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4230 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2024-05-06 12:50:20.053374 plone_app_linkintegrity-4.0.4/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2222 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/setup.py
```

### Comparing `plone.app.linkintegrity-4.0.3/CHANGES.rst` & `plone_app_linkintegrity-4.0.4/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,26 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.4 (2024-05-06)
+------------------
+
+Bug fixes:
+
+
+- Improve performance for calculating breaches.
+  [pgrunewald] (#100)
+- Fix breaches reporting for documents with multiple links.
+  [pgrunewald] (#102)
+
+
 4.0.3 (2023-09-29)
 ------------------
 
 Bug fixes:
 
 
 - Report sources once per breach in delete_confirmation_info.
```

### Comparing `plone.app.linkintegrity-4.0.3/PKG-INFO` & `plone_app_linkintegrity-4.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.linkintegrity
-Version: 4.0.3
+Version: 4.0.4
 Summary: Manage link integrity in Plone.
 Home-page: https://github.com/plone/plone.app.linkintegrity
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: link integrity plone
 Platform: Any
@@ -21,15 +21,34 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management :: Link Checking
 Requires-Python: >=3.8
+Requires-Dist: setuptools
+Requires-Dist: plone.app.intid
+Requires-Dist: plone.app.relationfield
+Requires-Dist: plone.base
+Requires-Dist: plone.dexterity
+Requires-Dist: Products.GenericSetup
+Requires-Dist: Products.statusmessages
+Requires-Dist: plone.app.textfield
+Requires-Dist: plone.app.uuid
+Requires-Dist: plone.registry
+Requires-Dist: plone.uuid
+Requires-Dist: Zope
+Requires-Dist: z3c.relationfield
+Requires-Dist: zc.relation
+Requires-Dist: zope.intid
+Requires-Dist: zope.keyreference
 Provides-Extra: test
+Requires-Dist: plone.app.testing; extra == "test"
+Requires-Dist: plone.namedfile; extra == "test"
+Requires-Dist: plone.testing; extra == "test"
 
 plone.app.linkintegrity
 =======================
 
 Overview
 --------
 
@@ -146,14 +165,26 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.4 (2024-05-06)
+------------------
+
+Bug fixes:
+
+
+- Improve performance for calculating breaches.
+  [pgrunewald] (#100)
+- Fix breaches reporting for documents with multiple links.
+  [pgrunewald] (#102)
+
+
 4.0.3 (2023-09-29)
 ------------------
 
 Bug fixes:
 
 
 - Report sources once per breach in delete_confirmation_info.
```

### Comparing `plone.app.linkintegrity-4.0.3/README.rst` & `plone_app_linkintegrity-4.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.linkintegrity-4.0.3/docs/LICENSE.GPL` & `plone_app_linkintegrity-4.0.4/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.linkintegrity-4.0.3/docs/LICENSE.txt` & `plone_app_linkintegrity-4.0.4/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/browser/delete_confirmation_info.pt` & `plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/browser/delete_confirmation_info.pt`

 * *Files identical despite different names*

### Comparing `plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/browser/info.py` & `plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/browser/info.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from Acquisition import aq_inner
-from collections import defaultdict
 from OFS.interfaces import IFolder
 from plone.app.linkintegrity.utils import getIncomingLinks
 from plone.app.linkintegrity.utils import linkintegrity_enabled
 from plone.base import PloneMessageFactory as _
 from plone.base.interfaces import IPloneSiteRoot
 from plone.uuid.interfaces import IUUID
 from Products.CMFCore.permissions import AccessContentsInformation
 from Products.CMFCore.utils import _checkPermission
 from Products.CMFCore.utils import getToolByName
 from Products.Five import BrowserView
 from Products.Five.browser.pagetemplatefile import ViewPageTemplateFile
 from zope.i18n import translate
 
 import logging
+import warnings
 
 
 logger = logging.getLogger(__name__)
 
 
 class DeleteConfirmationInfo(BrowserView):
     template = ViewPageTemplateFile("delete_confirmation_info.pt")
@@ -46,127 +46,102 @@
         Breaches coming from objects in the list of items
         or their children (if a object is a folder) will be ignored.
         """
         if items is None:
             items = [self.context]
         catalog = getToolByName(self.context, "portal_catalog")
         results = []
-        uids_to_ignore = []
-        uids_visited = set()
+        uids_to_ignore = set()
         self.breach_count = {}
+        path2obj = dict()
+        path2brains = dict()
+
+        # build various helper structures
         for obj in items:
             obj_path = "/".join(obj.getPhysicalPath())
-            brains_to_delete = catalog(path={"query": obj_path})
+            path2obj[obj_path] = obj
+            path2brains[obj_path] = brains_to_delete = catalog(path={"query": obj_path})
             # add the current items uid and all its children's uids to the
             # list of uids that are ignored
-            uids_to_ignore.extend([i.UID for i in brains_to_delete])
+            uids_to_ignore.update([i.UID for i in brains_to_delete])
+
+        # determine breaches
+        for obj_path, obj in path2obj.items():
+            brains_to_delete = path2brains[obj_path]
             for brain_to_delete in brains_to_delete:
                 try:
                     obj_to_delete = brain_to_delete.getObject()  # noqa
                 except (AttributeError, KeyError):
                     logger.exception(
                         "No object found for %s! Skipping", brain_to_delete
                     )
                     continue
-                for breach in self.get_breaches_for_item(obj):
-                    add_breach = False
+                # look into potential breach
+                breach = self.check_object(
+                    obj=obj_to_delete, excluded_paths=set(path2obj.keys())
+                )
+                if breach:
                     for source in breach["sources"]:
                         # Only add the breach if one the sources is not in the
                         # list of items that are to be deleted.
-                        if (
-                            source["uid"] not in uids_to_ignore
-                            and source["uid"] not in uids_visited
-                        ):
-                            add_breach = True
-                            uids_visited.add(source["uid"])
+                        if source["uid"] not in uids_to_ignore:
+                            results.append(breach)
                             break
-                    if add_breach:
-                        results.append(breach)
+
             if IFolder.providedBy(obj):
                 count = len(catalog(path={"query": obj_path}))
                 count_dirs = len(catalog(path={"query": obj_path}, is_folderish=True))
                 count_public = len(
                     catalog(path={"query": obj_path}, review_state="published")
                 )
                 if count:
                     self.breach_count[obj_path] = [count, count_dirs, count_public]
 
-        # Cleanup: Some breaches where added before it was known
-        # that their source will be deleted too.
-        for result in results:
-            for source in result["sources"]:
-                if source["uid"] in uids_to_ignore:
-                    # Drop sources that are also being deleted
-                    result["sources"].remove(source)
-                    if not result["sources"]:
-                        # Remove the breach is there are no more sources
-                        # This check is necessary since there can be multiple
-                        # sources for a breach
-                        results.remove(result)
-
-        # De-duplicate targets * sources
-        uid_target = {}
-        uid_sources = defaultdict(list)
-        for result in results:
-            target_uid = result["target"]["uid"]
-            uid_target[target_uid] = result["target"]
-            sources = uid_sources[target_uid]
-            for source in result["sources"]:
-                if source not in sources:
-                    sources.append(source)
-
-        # List of breaches
-        return [
-            {"target": uid_target[uid], "sources": sources}
-            for uid, sources in uid_sources.items()
-        ]
+        return results
 
     def get_breaches_for_item(self, obj=None):
         """Get breaches for one object and its children.
 
         Breaches coming from the children of a folder are ignored by default.
         """
-        if obj is None:
-            obj = self.context
-        results = []
-        catalog = getToolByName(obj, "portal_catalog")
-        obj_path = "/".join(obj.getPhysicalPath())
+        # BBB: No direct usage is known, but keep this for backwards compatibility.
+        # Sooner or later, we should use only one method.
+        warnings.warn(
+            """Using `get_breaches_for_item` is deprecated. Use `get_breaches`
+                      instead.""",
+            DeprecationWarning,
+        )
+        if obj is not None:
+            obj = [obj]
+        return self.get_breaches(obj)
 
-        breaches = self.check_object(obj)
-        if breaches:
-            results.append(breaches)
-
-        if IFolder.providedBy(obj):
-            brains = catalog(path={"query": obj_path})
-            for brain in brains:
-                try:
-                    child = brain.getObject()
-                except (AttributeError, KeyError):
-                    continue
-                if child == obj:
-                    continue
-                breaches = self.check_object(obj=child, excluded_path=obj_path)
-                if breaches:
-                    results.append(breaches)
-        self.breaches = results
-        return results
-
-    def check_object(self, obj, excluded_path=None):
+    def check_object(self, obj, excluded_path=None, excluded_paths=None):
         """Check one object for breaches.
-        Breaches originating from excluded_path are ignored.
+        Breaches originating from excluded_paths are ignored.
         """
+        # BBB: Support old and new parameters likewise
+        if excluded_paths is None:
+            excluded_paths = set()
+        if excluded_path:
+            excluded_paths.add(excluded_path)
+
         breaches = {}
         direct_links = getIncomingLinks(obj, from_attribute=None)
         has_breaches = False
         for direct_link in direct_links:
             source_path = direct_link.from_path
             if not source_path:
                 # link is broken
                 continue
-            if excluded_path and source_path.startswith(excluded_path):
+            if any(
+                [
+                    source_path.startswith(excluded_path)
+                    for excluded_path in excluded_paths
+                ]
+            ):
                 # source is in excluded_path
                 continue
             source = direct_link.from_object
             if not breaches.get("sources"):
                 breaches["sources"] = []
             breaches["sources"].append(
                 {
```

### Comparing `plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/browser/update.pt` & `plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/browser/update.pt`

 * *Files identical despite different names*

### Comparing `plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/browser/update.py` & `plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/browser/update.py`

 * *Files identical despite different names*

### Comparing `plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/configure.zcml` & `plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/exceptions.py` & `plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/exceptions.py`

 * *Files identical despite different names*

### Comparing `plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/handlers.py` & `plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/handlers.py`

 * *Files identical despite different names*

### Comparing `plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/parser.py` & `plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/parser.py`

 * *Files identical despite different names*

### Comparing `plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/retriever.py` & `plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/retriever.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Link Integrity - link retriever methods.
 """
+
 from plone.app.linkintegrity.interfaces import IRetriever
 from plone.app.linkintegrity.parser import extractLinks
 from plone.app.textfield import RichText
 from plone.dexterity.interfaces import IDexterityContent
 from plone.dexterity.interfaces import IDexterityFTI
 from plone.dexterity.utils import getAdditionalSchemata
 from zope.component import adapter
```

### Comparing `plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/testing.py` & `plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/tests/test_circular.py` & `plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/tests/test_circular.py`

 * *Files identical despite different names*

### Comparing `plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/tests/test_functional.py` & `plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/tests/test_functional.py`

 * *Files 0% similar despite different names*

```diff
@@ -398,17 +398,17 @@
         transaction.commit()
         # Then we use a browser to try to delete the referenced
         # document. Before we can do this we need to prevent the test
         # framework from choking on the exception we intentionally throw.
         self.browser.handleErrors = True
 
         self.browser.open("http://nohost/plone/manage_main")
-        self.browser.getControl(name="ids:list").getControl(
-            value="doc2"
-        ).selected = True
+        self.browser.getControl(name="ids:list").getControl(value="doc2").selected = (
+            True
+        )
 
         self.browser.getControl("Delete").click()
         self.assertNotIn("doc2", self.portal.objectIds())
 
     def test_warn_about_content(self):
         folder1 = self.portal.folder1
         self.browser.open(
```

### Comparing `plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/tests/test_handlers.py` & `plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/tests/test_imagescales.py` & `plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/tests/test_imagescales.py`

 * *Files identical despite different names*

### Comparing `plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/tests/test_info.py` & `plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/tests/test_references.py` & `plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/tests/test_references.py`

 * *Files 4% similar despite different names*

```diff
@@ -255,7 +255,26 @@
 
         # Test, if delete_confirmation_info shows also other relations than
         # ``isReferencing``.
         info = img1.restrictedTraverse("@@delete_confirmation_info")
         breaches = info.get_breaches()
         self.assertEqual(len(breaches), 1)
         self.assertEqual(len(info.get_breaches()[0]["sources"]), 1)
+
+    def test_sources_with_multiple_links_can_appear_multiple_times(self):
+        """Test, if delete confirmation shows one document as source twice
+        if it links to two of our to-be-deleted documents.
+        """
+        from plone.app.linkintegrity.testing import create
+
+        doc1 = self.portal.doc1
+        doc2 = self.portal.doc2
+        # create a document and create links to two existing documents
+        doc5 = create(self.portal, "Document", id="doc5", title="Test Page 5")
+        set_text(doc5, '<a href="doc1">d1</a><a href="doc2">d2</a>')
+
+        doc5_breaches = {r.to_object for r in getOutgoingLinks(doc5)}
+        # the order of breaches is non-deterministic
+        self.assertEqual({doc1, doc2}, doc5_breaches)
+        view = self.portal.restrictedTraverse("@@delete_confirmation_info")
+        # deleting the two referenced document results in two reported breaches
+        self.assertEqual(len(view.get_breaches([doc1, doc2])), 2)
```

### Comparing `plone.app.linkintegrity-4.0.3/plone/app/linkintegrity/utils.py` & `plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.linkintegrity-4.0.3/plone.app.linkintegrity.egg-info/PKG-INFO` & `plone_app_linkintegrity-4.0.4/plone.app.linkintegrity.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.linkintegrity
-Version: 4.0.3
+Version: 4.0.4
 Summary: Manage link integrity in Plone.
 Home-page: https://github.com/plone/plone.app.linkintegrity
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: link integrity plone
 Platform: Any
@@ -21,15 +21,34 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management :: Link Checking
 Requires-Python: >=3.8
+Requires-Dist: setuptools
+Requires-Dist: plone.app.intid
+Requires-Dist: plone.app.relationfield
+Requires-Dist: plone.base
+Requires-Dist: plone.dexterity
+Requires-Dist: Products.GenericSetup
+Requires-Dist: Products.statusmessages
+Requires-Dist: plone.app.textfield
+Requires-Dist: plone.app.uuid
+Requires-Dist: plone.registry
+Requires-Dist: plone.uuid
+Requires-Dist: Zope
+Requires-Dist: z3c.relationfield
+Requires-Dist: zc.relation
+Requires-Dist: zope.intid
+Requires-Dist: zope.keyreference
 Provides-Extra: test
+Requires-Dist: plone.app.testing; extra == "test"
+Requires-Dist: plone.namedfile; extra == "test"
+Requires-Dist: plone.testing; extra == "test"
 
 plone.app.linkintegrity
 =======================
 
 Overview
 --------
 
@@ -146,14 +165,26 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.4 (2024-05-06)
+------------------
+
+Bug fixes:
+
+
+- Improve performance for calculating breaches.
+  [pgrunewald] (#100)
+- Fix breaches reporting for documents with multiple links.
+  [pgrunewald] (#102)
+
+
 4.0.3 (2023-09-29)
 ------------------
 
 Bug fixes:
 
 
 - Report sources once per breach in delete_confirmation_info.
```

### Comparing `plone.app.linkintegrity-4.0.3/plone.app.linkintegrity.egg-info/SOURCES.txt` & `plone_app_linkintegrity-4.0.4/plone.app.linkintegrity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.linkintegrity-4.0.3/pyproject.toml` & `plone_app_linkintegrity-4.0.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # Generated from:
-# https://github.com/plone/meta/tree/master/config/default
+# https://github.com/plone/meta/tree/main/config/default
 # See the inline comments on how to expand/tweak this configuration file
+[build-system]
+requires = ["setuptools>=68.2"]
+
 [tool.towncrier]
 directory = "news/"
 filename = "CHANGES.rst"
 title_format = "{version} ({project_date})"
 underlines = ["-", ""]
 
 [[tool.towncrier.type]]
@@ -33,20 +36,44 @@
 showcontent = true
 
 [[tool.towncrier.type]]
 directory = "tests"
 name = "Tests"
 showcontent = true
 
+##
+# Add extra configuration options in .meta.toml:
+#  [pyproject]
+#  towncrier_extra_lines = """
+#  extra_configuration
+#  """
+##
+
 [tool.isort]
 profile = "plone"
 
+##
+# Add extra configuration options in .meta.toml:
+#  [pyproject]
+#  isort_extra_lines = """
+#  extra_configuration
+#  """
+##
+
 [tool.black]
 target-version = ["py38"]
 
+##
+# Add extra configuration options in .meta.toml:
+#  [pyproject]
+#  black_extra_lines = """
+#  extra_configuration
+#  """
+##
+
 [tool.codespell]
 ignore-words-list = "discreet,"
 skip = "*.po,"
 ##
 # Add extra configuration options in .meta.toml:
 #  [pyproject]
 #  codespell_ignores = "foo,bar"
@@ -97,15 +124,14 @@
 # Add extra configuration options in .meta.toml:
 #  [pyproject]
 #  dependencies_ignores = "['zestreleaser.towncrier']"
 #  dependencies_mappings = [
 #    "gitpython = ['git']",
 #    "pygithub = ['github']",
 #  ]
-#  """
 ##
 
 [tool.check-manifest]
 ignore = [
     ".editorconfig",
     ".meta.toml",
     ".pre-commit-config.yaml",
```

### Comparing `plone.app.linkintegrity-4.0.3/setup.py` & `plone_app_linkintegrity-4.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "4.0.3"
+version = "4.0.4"
 
 setup(
     name="plone.app.linkintegrity",
     version=version,
     description="Manage link integrity in Plone.",
     long_description="\n\n".join(
         [
@@ -49,14 +49,15 @@
         "plone.dexterity",
         "Products.GenericSetup",
         "Products.statusmessages",
         "plone.app.textfield",
         "plone.app.uuid",
         "plone.registry",
         "plone.uuid",
+        "Zope",
         "z3c.relationfield",
         "zc.relation",
         "zope.intid",
         "zope.keyreference",
     ],
     extras_require={
         "test": [
```

