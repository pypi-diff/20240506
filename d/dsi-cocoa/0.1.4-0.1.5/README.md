# Comparing `tmp/dsi_cocoa-0.1.4.tar.gz` & `tmp/dsi_cocoa-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsi_cocoa-0.1.4.tar", last modified: Mon May  6 18:00:11 2024, max compression
+gzip compressed data, was "dsi_cocoa-0.1.5.tar", last modified: Mon May  6 18:06:46 2024, max compression
```

## Comparing `dsi_cocoa-0.1.4.tar` & `dsi_cocoa-0.1.5.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:00:11.228889 dsi_cocoa-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-06 18:00:06.000000 dsi_cocoa-0.1.4/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:00:11.224889 dsi_cocoa-0.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:00:11.224889 dsi_cocoa-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-06 18:00:06.000000 dsi_cocoa-0.1.4/.github/workflows/increment.workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-06 18:00:06.000000 dsi_cocoa-0.1.4/.github/workflows/main.workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-06 18:00:06.000000 dsi_cocoa-0.1.4/.github/workflows/publish.workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-06 18:00:06.000000 dsi_cocoa-0.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-06 18:00:06.000000 dsi_cocoa-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-06 18:00:11.228889 dsi_cocoa-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-06 18:00:06.000000 dsi_cocoa-0.1.4/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-05-06 18:00:06.000000 dsi_cocoa-0.1.4/eval-repo.sh
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-06 18:00:06.000000 dsi_cocoa-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-06 18:00:06.000000 dsi_cocoa-0.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-06 18:00:11.228889 dsi_cocoa-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:00:11.224889 dsi_cocoa-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:00:11.228889 dsi_cocoa-0.1.4/src/cocoa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 18:00:06.000000 dsi_cocoa-0.1.4/src/cocoa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-06 18:00:06.000000 dsi_cocoa-0.1.4/src/cocoa/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-06 18:00:06.000000 dsi_cocoa-0.1.4/src/cocoa/evaluate_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8865 2024-05-06 18:00:06.000000 dsi_cocoa-0.1.4/src/cocoa/linting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-06 18:00:06.000000 dsi_cocoa-0.1.4/src/cocoa/notebooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-05-06 18:00:06.000000 dsi_cocoa-0.1.4/src/cocoa/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-06 18:00:06.000000 dsi_cocoa-0.1.4/src/cocoa/spring2024.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:00:11.228889 dsi_cocoa-0.1.4/src/dsi_cocoa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-06 18:00:11.000000 dsi_cocoa-0.1.4/src/dsi_cocoa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-06 18:00:11.000000 dsi_cocoa-0.1.4/src/dsi_cocoa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 18:00:11.000000 dsi_cocoa-0.1.4/src/dsi_cocoa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-06 18:00:11.000000 dsi_cocoa-0.1.4/src/dsi_cocoa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-06 18:00:11.000000 dsi_cocoa-0.1.4/src/dsi_cocoa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-06 18:00:11.000000 dsi_cocoa-0.1.4/src/dsi_cocoa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:06:46.053252 dsi_cocoa-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-06 18:06:34.000000 dsi_cocoa-0.1.5/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:06:46.045252 dsi_cocoa-0.1.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:06:46.049252 dsi_cocoa-0.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-06 18:06:34.000000 dsi_cocoa-0.1.5/.github/workflows/main.workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-06 18:06:34.000000 dsi_cocoa-0.1.5/.github/workflows/publish.workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-06 18:06:34.000000 dsi_cocoa-0.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-06 18:06:34.000000 dsi_cocoa-0.1.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-06 18:06:46.053252 dsi_cocoa-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-06 18:06:34.000000 dsi_cocoa-0.1.5/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-05-06 18:06:34.000000 dsi_cocoa-0.1.5/eval-repo.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-06 18:06:34.000000 dsi_cocoa-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-06 18:06:34.000000 dsi_cocoa-0.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-06 18:06:46.053252 dsi_cocoa-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:06:46.045252 dsi_cocoa-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:06:46.049252 dsi_cocoa-0.1.5/src/cocoa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 18:06:34.000000 dsi_cocoa-0.1.5/src/cocoa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-06 18:06:34.000000 dsi_cocoa-0.1.5/src/cocoa/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-06 18:06:34.000000 dsi_cocoa-0.1.5/src/cocoa/evaluate_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8865 2024-05-06 18:06:34.000000 dsi_cocoa-0.1.5/src/cocoa/linting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-06 18:06:34.000000 dsi_cocoa-0.1.5/src/cocoa/notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-05-06 18:06:34.000000 dsi_cocoa-0.1.5/src/cocoa/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-06 18:06:34.000000 dsi_cocoa-0.1.5/src/cocoa/spring2024.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:06:46.053252 dsi_cocoa-0.1.5/src/dsi_cocoa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-06 18:06:46.000000 dsi_cocoa-0.1.5/src/dsi_cocoa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-06 18:06:46.000000 dsi_cocoa-0.1.5/src/dsi_cocoa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 18:06:46.000000 dsi_cocoa-0.1.5/src/dsi_cocoa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-06 18:06:46.000000 dsi_cocoa-0.1.5/src/dsi_cocoa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-06 18:06:46.000000 dsi_cocoa-0.1.5/src/dsi_cocoa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-06 18:06:46.000000 dsi_cocoa-0.1.5/src/dsi_cocoa.egg-info/top_level.txt
```

### Comparing `dsi_cocoa-0.1.4/.github/workflows/main.workflow.yml` & `dsi_cocoa-0.1.5/.github/workflows/main.workflow.yml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.4/.github/workflows/publish.workflow.yml` & `dsi_cocoa-0.1.5/.github/workflows/publish.workflow.yml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.4/.gitignore` & `dsi_cocoa-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.4/.pre-commit-config.yaml` & `dsi_cocoa-0.1.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.4/PKG-INFO` & `dsi_cocoa-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsi-cocoa
-Version: 0.1.4
+Version: 0.1.5
 Summary: Clinic Opinionated Codebase Oversight and Analysis
 Author-email: Nick Ross <tspread@uchicago.edu>, Trevor Spreadbury <tspread@uchicago.edu>
 Maintainer: Nick Ross, Trevor Spreadbury
 Keywords: codebase analysis,uchicago dsi
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `dsi_cocoa-0.1.4/README.md` & `dsi_cocoa-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.4/pyproject.toml` & `dsi_cocoa-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.4/src/cocoa/evaluate_repo.py` & `dsi_cocoa-0.1.5/src/cocoa/evaluate_repo.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.4/src/cocoa/linting.py` & `dsi_cocoa-0.1.5/src/cocoa/linting.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.4/src/cocoa/notebooks.py` & `dsi_cocoa-0.1.5/src/cocoa/notebooks.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.4/src/cocoa/repo.py` & `dsi_cocoa-0.1.5/src/cocoa/repo.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.4/src/cocoa/spring2024.py` & `dsi_cocoa-0.1.5/src/cocoa/spring2024.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.4/src/dsi_cocoa.egg-info/PKG-INFO` & `dsi_cocoa-0.1.5/src/dsi_cocoa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsi-cocoa
-Version: 0.1.4
+Version: 0.1.5
 Summary: Clinic Opinionated Codebase Oversight and Analysis
 Author-email: Nick Ross <tspread@uchicago.edu>, Trevor Spreadbury <tspread@uchicago.edu>
 Maintainer: Nick Ross, Trevor Spreadbury
 Keywords: codebase analysis,uchicago dsi
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `dsi_cocoa-0.1.4/src/dsi_cocoa.egg-info/SOURCES.txt` & `dsi_cocoa-0.1.5/src/dsi_cocoa.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 .gitignore
 .pre-commit-config.yaml
 README.md
 eval-repo.sh
 pyproject.toml
 requirements.txt
 setup.cfg
-.github/workflows/increment.workflow.yml
 .github/workflows/main.workflow.yml
 .github/workflows/publish.workflow.yml
 src/cocoa/__init__.py
 src/cocoa/constants.py
 src/cocoa/evaluate_repo.py
 src/cocoa/linting.py
 src/cocoa/notebooks.py
```

