# Comparing `tmp/lab-8.1.tar.gz` & `tmp/lab-8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lab-8.1.tar", last modified: Wed Feb 28 07:29:46 2024, max compression
+gzip compressed data, was "lab-8.2.tar", last modified: Mon May  6 12:58:24 2024, max compression
```

## Comparing `lab-8.1.tar` & `lab-8.2.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxr-x   0 jendrik   (1000) jendrik   (1000)        0 2024-02-28 07:29:46.903721 lab-8.1/
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     1432 2023-04-26 08:24:22.000000 lab-8.1/INSTALL.rst
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)    35147 2022-08-24 16:48:45.000000 lab-8.1/LICENSE.txt
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)       40 2023-04-26 08:24:22.000000 lab-8.1/MANIFEST.in
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     3285 2024-02-28 07:29:46.903721 lab-8.1/PKG-INFO
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)      973 2023-04-26 08:24:22.000000 lab-8.1/README.rst
-drwxrwxr-x   0 jendrik   (1000) jendrik   (1000)        0 2024-02-28 07:29:46.899721 lab-8.1/downward/
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)        0 2023-10-21 09:52:30.000000 lab-8.1/downward/__init__.py
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     1730 2023-10-21 12:32:56.000000 lab-8.1/downward/cached_revision.py
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)    14223 2023-10-21 15:26:34.000000 lab-8.1/downward/experiment.py
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     3524 2023-10-21 09:52:30.000000 lab-8.1/downward/outcomes.py
-drwxrwxr-x   0 jendrik   (1000) jendrik   (1000)        0 2024-02-28 07:29:46.899721 lab-8.1/downward/parsers/
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)        0 2023-10-21 15:26:34.000000 lab-8.1/downward/parsers/__init__.py
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     2104 2023-10-21 15:26:34.000000 lab-8.1/downward/parsers/anytime_search_parser.py
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     1669 2023-10-21 15:26:34.000000 lab-8.1/downward/parsers/exitcode_parser.py
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     2856 2023-10-21 15:26:34.000000 lab-8.1/downward/parsers/planner_parser.py
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     5433 2023-10-21 15:26:34.000000 lab-8.1/downward/parsers/single_search_parser.py
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     2042 2023-10-21 15:26:34.000000 lab-8.1/downward/parsers/translator_parser.py
-drwxrwxr-x   0 jendrik   (1000) jendrik   (1000)        0 2024-02-28 07:29:46.899721 lab-8.1/downward/reports/
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)    11847 2023-12-20 12:51:01.000000 lab-8.1/downward/reports/__init__.py
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)    12881 2023-10-21 09:52:30.000000 lab-8.1/downward/reports/absolute.py
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     8589 2023-10-21 09:52:30.000000 lab-8.1/downward/reports/compare.py
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)    14962 2023-10-21 09:52:30.000000 lab-8.1/downward/reports/scatter.py
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     3834 2023-10-21 09:52:30.000000 lab-8.1/downward/reports/scatter_matplotlib.py
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     4059 2023-10-21 09:52:30.000000 lab-8.1/downward/reports/scatter_pgfplots.py
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     1732 2023-10-21 09:52:30.000000 lab-8.1/downward/reports/taskwise.py
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     4529 2023-10-21 09:52:30.000000 lab-8.1/downward/suites.py
-drwxrwxr-x   0 jendrik   (1000) jendrik   (1000)        0 2024-02-28 07:29:46.899721 lab-8.1/lab/
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)       90 2024-02-28 07:29:46.000000 lab-8.1/lab/__init__.py
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     5915 2023-10-21 12:32:56.000000 lab-8.1/lab/cached_revision.py
-drwxrwxr-x   0 jendrik   (1000) jendrik   (1000)        0 2024-02-28 07:29:46.899721 lab-8.1/lab/calls/
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)        0 2023-10-21 09:52:30.000000 lab-8.1/lab/calls/__init__.py
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     7995 2023-10-21 09:52:30.000000 lab-8.1/lab/calls/call.py
-drwxrwxr-x   0 jendrik   (1000) jendrik   (1000)        0 2024-02-28 07:29:46.903721 lab-8.1/lab/data/
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     2082 2023-04-26 08:24:22.000000 lab-8.1/lab/data/local-job.py.template
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)      546 2023-04-26 08:24:22.000000 lab-8.1/lab/data/run.py.template
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     1044 2023-04-26 08:24:22.000000 lab-8.1/lab/data/slurm-job-header.template
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     1413 2023-04-26 08:24:22.000000 lab-8.1/lab/data/slurm-run-job-body.template
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)       55 2023-04-26 08:24:22.000000 lab-8.1/lab/data/slurm-step-job-body.template
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)    17805 2023-10-21 12:32:56.000000 lab-8.1/lab/environments.py
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)    27224 2024-02-23 13:50:24.000000 lab-8.1/lab/experiment.py
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     6188 2023-12-20 12:51:01.000000 lab-8.1/lab/fetcher.py
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     6210 2024-02-23 13:16:30.000000 lab-8.1/lab/parser.py
-drwxrwxr-x   0 jendrik   (1000) jendrik   (1000)        0 2024-02-28 07:29:46.903721 lab-8.1/lab/reports/
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)    31073 2023-11-02 13:49:45.000000 lab-8.1/lab/reports/__init__.py
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)      724 2023-10-21 09:52:30.000000 lab-8.1/lab/reports/filter.py
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     7233 2024-02-24 20:08:44.000000 lab-8.1/lab/reports/markup.py
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     2554 2023-10-21 09:52:30.000000 lab-8.1/lab/steps.py
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)    18360 2023-10-21 17:46:46.000000 lab-8.1/lab/tools.py
-drwxrwxr-x   0 jendrik   (1000) jendrik   (1000)        0 2024-02-28 07:29:46.899721 lab-8.1/lab.egg-info/
--rw-r--r--   0 jendrik   (1000) jendrik   (1000)     3285 2024-02-28 07:29:46.000000 lab-8.1/lab.egg-info/PKG-INFO
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     1206 2024-02-28 07:29:46.000000 lab-8.1/lab.egg-info/SOURCES.txt
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)        1 2024-02-28 07:29:46.000000 lab-8.1/lab.egg-info/dependency_links.txt
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)       36 2024-02-28 07:29:46.000000 lab-8.1/lab.egg-info/requires.txt
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)       13 2024-02-28 07:29:46.000000 lab-8.1/lab.egg-info/top_level.txt
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)      985 2023-04-26 08:24:22.000000 lab-8.1/pyproject.toml
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)       38 2024-02-28 07:29:46.903721 lab-8.1/setup.cfg
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     1477 2023-10-21 15:26:34.000000 lab-8.1/setup.py
-drwxrwxr-x   0 jendrik   (1000) jendrik   (1000)        0 2024-02-28 07:29:46.903721 lab-8.1/tests/
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)      576 2023-10-21 09:52:30.000000 lab-8.1/tests/test_reports.py
--rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     1805 2023-10-21 09:52:30.000000 lab-8.1/tests/test_various.py
+drwxrwxr-x   0 jendrik   (1000) jendrik   (1000)        0 2024-05-06 12:58:24.579512 lab-8.2/
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     1432 2023-04-26 08:24:22.000000 lab-8.2/INSTALL.rst
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)    35147 2022-08-24 16:48:45.000000 lab-8.2/LICENSE.txt
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)       40 2023-04-26 08:24:22.000000 lab-8.2/MANIFEST.in
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     3285 2024-05-06 12:58:24.579512 lab-8.2/PKG-INFO
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)      973 2023-04-26 08:24:22.000000 lab-8.2/README.rst
+drwxrwxr-x   0 jendrik   (1000) jendrik   (1000)        0 2024-05-06 12:58:24.575512 lab-8.2/downward/
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)        0 2024-05-06 12:57:50.000000 lab-8.2/downward/__init__.py
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     1730 2024-05-06 12:57:50.000000 lab-8.2/downward/cached_revision.py
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)    14155 2024-05-06 12:57:50.000000 lab-8.2/downward/experiment.py
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     3524 2024-05-06 12:57:50.000000 lab-8.2/downward/outcomes.py
+drwxrwxr-x   0 jendrik   (1000) jendrik   (1000)        0 2024-05-06 12:58:24.575512 lab-8.2/downward/parsers/
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)        0 2024-05-06 12:57:50.000000 lab-8.2/downward/parsers/__init__.py
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     2104 2024-05-06 12:57:50.000000 lab-8.2/downward/parsers/anytime_search_parser.py
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     1669 2024-05-06 12:57:50.000000 lab-8.2/downward/parsers/exitcode_parser.py
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     2856 2024-05-06 12:57:50.000000 lab-8.2/downward/parsers/planner_parser.py
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     5433 2024-05-06 12:57:50.000000 lab-8.2/downward/parsers/single_search_parser.py
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     2042 2024-05-06 12:57:50.000000 lab-8.2/downward/parsers/translator_parser.py
+drwxrwxr-x   0 jendrik   (1000) jendrik   (1000)        0 2024-05-06 12:58:24.575512 lab-8.2/downward/reports/
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)    12386 2024-05-06 12:57:50.000000 lab-8.2/downward/reports/__init__.py
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)    12881 2024-05-06 12:57:50.000000 lab-8.2/downward/reports/absolute.py
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     8589 2024-05-06 12:57:50.000000 lab-8.2/downward/reports/compare.py
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)    14962 2024-05-06 12:57:51.000000 lab-8.2/downward/reports/scatter.py
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     3834 2024-05-06 12:57:51.000000 lab-8.2/downward/reports/scatter_matplotlib.py
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     4059 2024-05-06 12:57:51.000000 lab-8.2/downward/reports/scatter_pgfplots.py
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     1732 2024-05-06 12:57:51.000000 lab-8.2/downward/reports/taskwise.py
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     4529 2024-05-06 12:57:51.000000 lab-8.2/downward/suites.py
+drwxrwxr-x   0 jendrik   (1000) jendrik   (1000)        0 2024-05-06 12:58:24.575512 lab-8.2/lab/
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)       90 2024-05-06 12:58:23.000000 lab-8.2/lab/__init__.py
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     5915 2024-05-06 12:57:51.000000 lab-8.2/lab/cached_revision.py
+drwxrwxr-x   0 jendrik   (1000) jendrik   (1000)        0 2024-05-06 12:58:24.575512 lab-8.2/lab/calls/
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)        0 2024-05-06 12:57:51.000000 lab-8.2/lab/calls/__init__.py
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     8003 2024-05-06 12:57:51.000000 lab-8.2/lab/calls/call.py
+drwxrwxr-x   0 jendrik   (1000) jendrik   (1000)        0 2024-05-06 12:58:24.579512 lab-8.2/lab/data/
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     2082 2023-04-26 08:24:22.000000 lab-8.2/lab/data/local-job.py.template
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)      546 2024-03-30 20:00:54.000000 lab-8.2/lab/data/run.py.template
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     1044 2023-04-26 08:24:22.000000 lab-8.2/lab/data/slurm-job-header.template
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     1413 2023-04-26 08:24:22.000000 lab-8.2/lab/data/slurm-run-job-body.template
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)       55 2023-04-26 08:24:22.000000 lab-8.2/lab/data/slurm-step-job-body.template
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)    17805 2024-05-06 12:57:51.000000 lab-8.2/lab/environments.py
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)    27643 2024-05-06 12:57:51.000000 lab-8.2/lab/experiment.py
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     6137 2024-05-06 12:57:51.000000 lab-8.2/lab/fetcher.py
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     6407 2024-05-06 12:57:51.000000 lab-8.2/lab/parser.py
+drwxrwxr-x   0 jendrik   (1000) jendrik   (1000)        0 2024-05-06 12:58:24.579512 lab-8.2/lab/reports/
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)    31073 2024-05-06 12:57:51.000000 lab-8.2/lab/reports/__init__.py
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)      724 2024-05-06 12:57:51.000000 lab-8.2/lab/reports/filter.py
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     7233 2024-05-06 12:57:51.000000 lab-8.2/lab/reports/markup.py
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     2554 2024-05-06 12:57:51.000000 lab-8.2/lab/steps.py
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)    18078 2024-05-06 12:57:51.000000 lab-8.2/lab/tools.py
+drwxrwxr-x   0 jendrik   (1000) jendrik   (1000)        0 2024-05-06 12:58:24.575512 lab-8.2/lab.egg-info/
+-rw-r--r--   0 jendrik   (1000) jendrik   (1000)     3285 2024-05-06 12:58:24.000000 lab-8.2/lab.egg-info/PKG-INFO
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     1206 2024-05-06 12:58:24.000000 lab-8.2/lab.egg-info/SOURCES.txt
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)        1 2024-05-06 12:58:24.000000 lab-8.2/lab.egg-info/dependency_links.txt
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)       36 2024-05-06 12:58:24.000000 lab-8.2/lab.egg-info/requires.txt
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)       13 2024-05-06 12:58:24.000000 lab-8.2/lab.egg-info/top_level.txt
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)      985 2024-05-06 12:55:53.000000 lab-8.2/pyproject.toml
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)       38 2024-05-06 12:58:24.579512 lab-8.2/setup.cfg
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     1477 2024-05-06 12:57:51.000000 lab-8.2/setup.py
+drwxrwxr-x   0 jendrik   (1000) jendrik   (1000)        0 2024-05-06 12:58:24.579512 lab-8.2/tests/
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)      576 2024-05-06 12:57:51.000000 lab-8.2/tests/test_reports.py
+-rw-rw-r--   0 jendrik   (1000) jendrik   (1000)     1805 2024-05-06 12:57:51.000000 lab-8.2/tests/test_various.py
```

### Comparing `lab-8.1/INSTALL.rst` & `lab-8.2/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `lab-8.1/LICENSE.txt` & `lab-8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lab-8.1/PKG-INFO` & `lab-8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lab
-Version: 8.1
+Version: 8.2
 Summary: Benchmark your code
 Home-page: https://github.com/aibasel/lab
 Author: Jendrik Seipp
 Author-email: jendrikseipp@gmail.com
 License: GPL3+
 Keywords: benchmarks cluster grid
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `lab-8.1/README.rst` & `lab-8.2/README.rst`

 * *Files identical despite different names*

### Comparing `lab-8.1/downward/cached_revision.py` & `lab-8.2/downward/cached_revision.py`

 * *Files identical despite different names*

### Comparing `lab-8.1/downward/experiment.py` & `lab-8.2/downward/experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -331,19 +331,15 @@
             if algorithm == algo:
                 logging.critical(
                     f"Algorithms {algo.name} and {algorithm.name} are identical."
                 )
         self._algorithms[name] = algorithm
 
     def build(self, **kwargs):
-        """Add Fast Downward code, runs and write everything to disk.
-
-        This method is called by the second experiment step.
-
-        """
+        """Add Fast Downward code and runs, and write everything to disk."""
         if not self._algorithms:
             logging.critical("You must add at least one algorithm.")
 
         # We convert the problems in suites to strings to avoid errors when
         # converting properties to JSON later. The clean but more complex
         # solution would be to add a method to the JSONEncoder that recognizes
         # and correctly serializes the Path and Task classes.
```

### Comparing `lab-8.1/downward/outcomes.py` & `lab-8.2/downward/outcomes.py`

 * *Files identical despite different names*

### Comparing `lab-8.1/downward/parsers/anytime_search_parser.py` & `lab-8.2/downward/parsers/anytime_search_parser.py`

 * *Files identical despite different names*

### Comparing `lab-8.1/downward/parsers/exitcode_parser.py` & `lab-8.2/downward/parsers/exitcode_parser.py`

 * *Files identical despite different names*

### Comparing `lab-8.1/downward/parsers/planner_parser.py` & `lab-8.2/downward/parsers/planner_parser.py`

 * *Files identical despite different names*

### Comparing `lab-8.1/downward/parsers/single_search_parser.py` & `lab-8.2/downward/parsers/single_search_parser.py`

 * *Files identical despite different names*

### Comparing `lab-8.1/downward/parsers/translator_parser.py` & `lab-8.2/downward/parsers/translator_parser.py`

 * *Files identical despite different names*

### Comparing `lab-8.1/downward/reports/__init__.py` & `lab-8.2/downward/reports/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,17 +46,17 @@
         "build_options",
         "driver_options",
         "component_options",
     ]
 
     #: Attributes shown in the unexplained-errors table.
     ERROR_ATTRIBUTES = [
+        "algorithm",
         "domain",
         "problem",
-        "algorithm",
         "unexplained_errors",
         "error",
         "planner_wall_clock_time",
         "raw_memory",
         "node",
     ]
 
@@ -137,16 +137,15 @@
             self.runs[(domain, problem, algo)] = run
         for domain, problem in problems:
             self.domains[domain].append(problem)
 
         self.algorithms = self._get_algorithm_order()
 
         num_unexplained_errors = sum(
-            int(bool(tools.get_unexplained_errors_message(run)))
-            for run in self.runs.values()
+            int(tools.has_unexplained_error(run)) for run in self.runs.values()
         )
         func = logging.info if num_unexplained_errors == 0 else logging.warning
         func(
             f"Report contains {num_unexplained_errors} runs with unexplained"
             f" errors."
         )
 
@@ -193,82 +192,97 @@
 
     def _format_unexplained_errors(self, errors):
         """
         Preserve line breaks and white space. If text has more than
         ERROR_LOG_MAX_LINES lines, omit lines in the middle of the text.
         """
         linebreak = "\\\\"
-        text = f"''{errors}''".replace("\\n", linebreak).replace(
-            " ", markup.ESCAPE_WHITESPACE
+        text = (
+            str(errors).replace("\\n", linebreak).replace(" ", markup.ESCAPE_WHITESPACE)
         )
         lines = text.split(linebreak)
         if len(lines) <= self.ERROR_LOG_MAX_LINES:
             return text
         index = (self.ERROR_LOG_MAX_LINES - 2) // 2
         text = linebreak.join(lines[:index] + ["", "[...]", ""] + lines[-index:])
-        assert text.startswith("''") and text.endswith("''"), text
         return text
 
     def _get_warnings_text_and_table(self):
-        """
-        Return a :py:class:`Table <lab.reports.Table>` containing one line for
-        each run where an unexplained error occured.
-        """
-        if not self.ERROR_ATTRIBUTES:
-            logging.critical("The list of error attributes must not be empty.")
-
-        table = reports.Table(title="Unexplained errors")
-        table.set_column_order(self.ERROR_ATTRIBUTES)
+        errors = []
 
         wrote_to_slurm_err = any(
             "output-to-slurm.err" in run.get("unexplained_errors", [])
             for run in self.runs.values()
         )
-
-        for run in self.runs.values():
-            error_message = tools.get_unexplained_errors_message(run)
-            if error_message:
-                run_dir = run["run_dir"]
-                for attr in self.ERROR_ATTRIBUTES:
-                    value = run.get(attr, "?")
-                    if attr == "unexplained_errors":
-                        value = self._format_unexplained_errors(value)
-                        # Use formatted value as-is.
-                        table.cell_formatters[run_dir][attr] = reports.CellFormatter()
-                    table.add_cell(run_dir, attr, value)
-
-        errors = []
-
         if wrote_to_slurm_err:
             src_dir = self.eval_dir.rstrip("/")[: -len("-eval")]
             slurm_err_file = src_dir + "-grid-steps/slurm.err"
             try:
                 slurm_err_content = tools.get_slurm_err_content(src_dir)
             except FileNotFoundError:
                 slurm_err_file = "*-grid-steps/slurm.err"
                 errors.append(
                     f"There was output to {slurm_err_file}, but the file was missing "
                     f"when this report was made."
                 )
             else:
                 slurm_err_content = tools.filter_slurm_err_content(slurm_err_content)
                 errors.append(
-                    f"There was output to {slurm_err_file}. Below is the output without"
-                    f'"memory cg" errors:\n```\n{slurm_err_content}\n```'
+                    f"There was output to {slurm_err_file}:\n"
+                    f"```\n{slurm_err_content}\n```"
                 )
             logging.warning(f"There was output to {slurm_err_file}.")
 
-        if table:
-            errors.append(str(table))
+        unique_error_messages = defaultdict(list)
+        for run in self.runs.values():
+            if tools.has_unexplained_error(run):
+                msg = self._format_unexplained_errors(
+                    run.get("unexplained_errors", "?")
+                )
+                unique_error_messages[msg].append(run)
+        if unique_error_messages:
+            logging.info(f"Unique unexplained errors: {len(unique_error_messages)}")
+
+        if self.output_format == "html":
+            error_atributes = [
+                attr for attr in self.ERROR_ATTRIBUTES if attr != "unexplained_errors"
+            ]
+            if "run_dir" not in self.ERROR_ATTRIBUTES:
+                error_atributes.append("run_dir")
+
+            def get_row(run):
+                return " ".join(
+                    f"<td>{run.get(attr, '?')}</td>" for attr in error_atributes
+                )
 
-        infai_1_nodes = {f"ase{i:02d}.cluster.bc2.ch" for i in range(1, 25)}
-        infai_2_nodes = {f"ase{i:02d}.cluster.bc2.ch" for i in range(31, 55)}
-        nodes = self._get_node_names()
-        if nodes & infai_1_nodes and nodes & infai_2_nodes:
-            errors.append("Report combines runs from infai_1 and infai_2 partitions.")
+            table = [
+                '<button type="button" class="toggle-table" '
+                'onclick="toggle_table(this)">Show table</button><p></p>',
+                '<table class="tableborder" style="display:none">',
+                "<tr>",
+                "<th>Unexplained errors</th> "
+                + " ".join(f"<th>{attr}</th>" for attr in error_atributes),
+                "</tr>",
+            ]
+            for msg, runs in sorted(
+                unique_error_messages.items(), key=lambda x: len(x[0])
+            ):
+                runs.sort(
+                    key=lambda run: (run["algorithm"], run["domain"], run["problem"])
+                )
+                table.append("<tr>")
+                table.append(f'<td rowspan="{len(runs)}">{msg}</td>')
+                table.append(get_row(runs[0]))
+                table.append("</tr>")
+                for run in runs[1:]:
+                    table.append(f"<tr>{get_row(run)}</tr>")
+            table.append("</table>")
+            errors.append("\n'''\n" + "\n".join(table) + "\n'''")
+        elif unique_error_messages:
+            errors.append("There were unexplained errors. See HTML report for details.")
 
         return "\n".join(errors)
 
     def _get_algorithm_order(self):
         """
         Return a list of algorithms in the order determined by the user.
```

### Comparing `lab-8.1/downward/reports/absolute.py` & `lab-8.2/downward/reports/absolute.py`

 * *Files identical despite different names*

### Comparing `lab-8.1/downward/reports/compare.py` & `lab-8.2/downward/reports/compare.py`

 * *Files identical despite different names*

### Comparing `lab-8.1/downward/reports/scatter.py` & `lab-8.2/downward/reports/scatter.py`

 * *Files identical despite different names*

### Comparing `lab-8.1/downward/reports/scatter_matplotlib.py` & `lab-8.2/downward/reports/scatter_matplotlib.py`

 * *Files identical despite different names*

### Comparing `lab-8.1/downward/reports/scatter_pgfplots.py` & `lab-8.2/downward/reports/scatter_pgfplots.py`

 * *Files identical despite different names*

### Comparing `lab-8.1/downward/reports/taskwise.py` & `lab-8.2/downward/reports/taskwise.py`

 * *Files identical despite different names*

### Comparing `lab-8.1/downward/suites.py` & `lab-8.2/downward/suites.py`

 * *Files identical despite different names*

### Comparing `lab-8.1/lab/cached_revision.py` & `lab-8.2/lab/cached_revision.py`

 * *Files identical despite different names*

### Comparing `lab-8.1/lab/calls/call.py` & `lab-8.2/lab/calls/call.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,16 +179,16 @@
         for fd, outfile in fd_to_outfile.items():
             # Ignore streams that exceeded the hard limit.
             if outfile is not None:
                 soft_limit, _ = fd_to_limits[fd]
                 bytes_written = fd_to_bytes[fd]
                 if soft_limit is not None and bytes_written > soft_limit:
                     logging.error(
-                        f"{self.name} finished and wrote {bytes_written / 1024} KiB "
-                        f"to {outfile.name} (soft limit: {soft_limit / 1024} KiB)"
+                        f"{self.name} finished and wrote {bytes_written / 1024:.2f} KiB "
+                        f"to {outfile.name} (soft limit: {soft_limit / 1024:.2f} KiB)"
                     )
 
     def wait(self):
         wall_clock_start_time = time.time()
         self._redirect_streams()
         retcode = self.process.wait()
         for stream, _ in self.redirected_streams_and_limits.values():
```

### Comparing `lab-8.1/lab/data/local-job.py.template` & `lab-8.2/lab/data/local-job.py.template`

 * *Files identical despite different names*

### Comparing `lab-8.1/lab/data/run.py.template` & `lab-8.2/lab/data/run.py.template`

 * *Files identical despite different names*

### Comparing `lab-8.1/lab/data/slurm-job-header.template` & `lab-8.2/lab/data/slurm-job-header.template`

 * *Files identical despite different names*

### Comparing `lab-8.1/lab/data/slurm-run-job-body.template` & `lab-8.2/lab/data/slurm-run-job-body.template`

 * *Files identical despite different names*

### Comparing `lab-8.1/lab/environments.py` & `lab-8.2/lab/environments.py`

 * *Files identical despite different names*

### Comparing `lab-8.1/lab/experiment.py` & `lab-8.2/lab/experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Main module for creating experiments."""
 
 from collections import OrderedDict
 import logging
 import os
 from pathlib import Path
+import re
 import sys
 
 from lab import environments, tools
 from lab.fetcher import Fetcher
 from lab.parser import Parser
 from lab.steps import get_step, get_steps_text, Step
 
@@ -245,21 +246,30 @@
             logging.critical(f"Command names must be unique: {name}")
 
         if not isinstance(command, list):
             logging.critical(f"The command for {name} is not a list: {command}")
         if not command:
             logging.critical(f'Command "{name}" must not be empty')
 
-        # Raise an error if the command calls a Python script directly.
-        msg = (
-            'Command "{name}" calls the Python script "{part}" directly. '
-            "To make sure the script uses the right Python interpreter, "
-            'please use "[sys.executable, "{part}", ...] instead.'
-        )
-        if command[0].endswith(".py"):
+        # Raise an error if the command calls Python directly.
+        if re.match(r"^python[0-9\.]*$", command[0]):
+            msg = (
+                'Command "{name}" calls Python directly. '
+                "To make sure the command uses the correct Python interpreter, "
+                "please use {part} instead."
+            )
+            raise ValueError(
+                msg.format(name=name, part=["sys.executable"] + command[1:])
+            )
+        elif command[0].endswith(".py"):
+            msg = (
+                'Command "{name}" calls the Python script "{part}" directly. '
+                "To make sure the script uses the correct Python interpreter, "
+                'please use "[sys.executable, "{part}", ...] instead.'
+            )
             raise ValueError(msg.format(name=name, part=command[0]))
 
         if "stdin" in kwargs:
             logging.critical("redirecting stdin is not supported")
         kwargs["time_limit"] = time_limit
         kwargs["memory_limit"] = memory_limit
         kwargs["soft_stdout_limit"] = soft_stdout_limit
```

### Comparing `lab-8.1/lab/fetcher.py` & `lab-8.2/lab/fetcher.py`

 * *Files 5% similar despite different names*

```diff
@@ -153,16 +153,15 @@
                     loglevel, f"Collected {index:6d}/{num_dirs} properties files"
                 )
             run_filter.apply(new_props)
             combined_props.update(new_props)
 
         unexplained_errors = 0
         for props in combined_props.values():
-            error_message = tools.get_unexplained_errors_message(props)
-            if error_message:
+            if tools.has_unexplained_error(props):
                 unexplained_errors += 1
 
         tools.makedirs(eval_dir)
         combined_props.write()
         func = logging.info if unexplained_errors == 0 else logging.warning
         func(
             f"Wrote properties file. It contains {unexplained_errors} "
```

### Comparing `lab-8.1/lab/parser.py` & `lab-8.2/lab/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,22 +20,24 @@
 """
 
 from collections import defaultdict
 import logging
 from pathlib import Path
 import re
 
+from lab import tools
+
 
 def _get_pattern_flags(s):
     flags = 0
     for char in s:
         try:
             flags |= getattr(re, char)
         except AttributeError:
-            logging.critical(f"Unknown pattern flag: {char}")
+            raise ValueError(f"Unknown pattern flag: {char}")
     return flags
 
 
 class _Function:
     def __init__(self, function, filename):
         self.function = function
         self.filename = filename
@@ -47,30 +49,33 @@
         self.type_ = type_
         self.required = required
         self.group = 1
 
         flags = _get_pattern_flags(flags)
         self.regex = re.compile(regex, flags)
 
-    def search(self, content, filename):
+    def search(self, filename, content, props):
         found_props = {}
         match = self.regex.search(content)
         if match:
             try:
                 value = match.group(self.group)
             except IndexError:
-                logging.error(
+                tools.add_unexplained_error(
+                    props,
                     f"Attribute {self.attribute} not found for pattern {self} in "
-                    f"file {filename}."
+                    f"file {filename}.",
                 )
             else:
                 value = self.type_(value)
                 found_props[self.attribute] = value
         elif self.required:
-            logging.error(f'Pattern "{self}" not found in {filename}')
+            tools.add_unexplained_error(
+                props, f'Pattern "{self}" not found in {filename}'
+            )
         return found_props
 
     def __str__(self):
         return self.regex.pattern
 
 
 class _FileParser:
@@ -82,15 +87,15 @@
         self.patterns = []
 
     def add_pattern(self, pattern):
         self.patterns.append(pattern)
 
     def search_patterns(self, filename, content, props):
         for pattern in self.patterns:
-            props.update(pattern.search(content, filename))
+            props.update(pattern.search(filename, content, props))
 
 
 class Parser:
     """
     Parse logs or files in a given directory and write results into the
     ``properties`` file.
     """
@@ -181,15 +186,17 @@
 
         for filename, file_parser in self.file_parsers.items():
             # If filename is absolute, path is set to filename.
             path = run_dir / filename
             content = get_content(path)
             if content is None:
                 if any(pattern.required for pattern in file_parser.patterns):
-                    logging.error(f'Required file "{path}" is missing.')
+                    tools.add_unexplained_error(
+                        props, f'Required file "{path}" is missing.'
+                    )
             else:
                 file_parser.search_patterns(str(path), content, props)
 
         for function in self.functions:
             path = run_dir / function.filename
             # Call function with empty string if file is missing.
             content = get_content(path) or ""
```

### Comparing `lab-8.1/lab/reports/__init__.py` & `lab-8.2/lab/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `lab-8.1/lab/reports/filter.py` & `lab-8.2/lab/reports/filter.py`

 * *Files identical despite different names*

### Comparing `lab-8.1/lab/reports/markup.py` & `lab-8.2/lab/reports/markup.py`

 * *Files identical despite different names*

### Comparing `lab-8.1/lab/steps.py` & `lab-8.2/lab/steps.py`

 * *Files identical despite different names*

### Comparing `lab-8.1/lab/tools.py` & `lab-8.2/lab/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 
 DEFAULT_ENCODING = "utf-8"
 
 
 def get_string(s):
     if isinstance(s, bytes):
-        return s.decode(DEFAULT_ENCODING)
+        return s.decode(DEFAULT_ENCODING, errors="replace")
     else:
         raise ValueError("tools.get_string() only accepts byte strings")
 
 
 def get_bytes(s):
     if isinstance(s, str):
         return s.encode(DEFAULT_ENCODING)
@@ -515,41 +515,31 @@
     return prod
 
 
 def rgb_fractions_to_html_color(r, g, b):
     return f"rgb({int(r * 255)},{int(g * 255)},{int(b * 255)})"
 
 
-def get_unexplained_errors_message(run):
+def has_unexplained_error(run):
     """
-    Return an error message if an unexplained error occured in the given run,
-    otherwise return None.
+    Return whether the run has an unexplained error apart from Slurm writing to stderr.
     """
     unexplained_errors = run.get("unexplained_errors", [])
-    if not unexplained_errors or unexplained_errors == ["output-to-slurm.err"]:
-        return ""
-    else:
-        return f"Unexplained error(s) in {run['run_dir']}: {unexplained_errors}"
+    return bool(unexplained_errors) and unexplained_errors != ["output-to-slurm.err"]
 
 
 def get_slurm_err_content(src_dir):
     grid_steps_dir = str(src_dir).rstrip("/") + "-grid-steps"
     slurm_err_filename = os.path.join(grid_steps_dir, "slurm.err")
     with open(slurm_err_filename) as f:
         return f.read()
 
 
 def filter_slurm_err_content(content):
-    filtered = re.sub(
-        r"slurmstepd: error: task/cgroup: unable to add task\[pid=\d+\]"
-        r" to memory cg '\(null\)'\n",
-        "",
-        content,
-    )
-    filtered = re.sub(r"\x00", "", filtered)
+    filtered = re.sub(r"\x00", "", content)
     return "\n".join(line for line in filtered.splitlines() if line.strip())
 
 
 class RawAndDefaultsHelpFormatter(argparse.HelpFormatter):
     """
     Help message formatter which preserves the description format and adds
     default values to argument help messages.
```

### Comparing `lab-8.1/lab.egg-info/PKG-INFO` & `lab-8.2/lab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lab
-Version: 8.1
+Version: 8.2
 Summary: Benchmark your code
 Home-page: https://github.com/aibasel/lab
 Author: Jendrik Seipp
 Author-email: jendrikseipp@gmail.com
 License: GPL3+
 Keywords: benchmarks cluster grid
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `lab-8.1/lab.egg-info/SOURCES.txt` & `lab-8.2/lab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lab-8.1/pyproject.toml` & `lab-8.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lab-8.1/setup.py` & `lab-8.2/setup.py`

 * *Files identical despite different names*

### Comparing `lab-8.1/tests/test_reports.py` & `lab-8.2/tests/test_reports.py`

 * *Files identical despite different names*

### Comparing `lab-8.1/tests/test_various.py` & `lab-8.2/tests/test_various.py`

 * *Files identical despite different names*

