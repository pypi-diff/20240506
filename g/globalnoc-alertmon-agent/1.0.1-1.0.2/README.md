# Comparing `tmp/globalnoc-alertmon-agent-1.0.1.tar.gz` & `tmp/globalnoc-alertmon-agent-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globalnoc-alertmon-agent-1.0.1.tar", last modified: Thu Jan 25 19:23:45 2024, max compression
+gzip compressed data, was "globalnoc-alertmon-agent-1.0.2.tar", last modified: Mon May  6 17:55:21 2024, max compression
```

## Comparing `globalnoc-alertmon-agent-1.0.1.tar` & `globalnoc-alertmon-agent-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,11 @@
-drwxr-xr-x   0 bengeels   (501) staff       (20)        0 2024-01-25 19:23:45.736740 globalnoc-alertmon-agent-1.0.1/
--rw-r--r--   0 bengeels   (501) staff       (20)    11356 2024-01-25 19:17:50.000000 globalnoc-alertmon-agent-1.0.1/LICENSE
--rw-r--r--   0 bengeels   (501) staff       (20)      604 2024-01-25 19:23:45.736307 globalnoc-alertmon-agent-1.0.1/PKG-INFO
--rw-r--r--   0 bengeels   (501) staff       (20)     1284 2024-01-25 19:17:50.000000 globalnoc-alertmon-agent-1.0.1/README.md
-drwxr-xr-x   0 bengeels   (501) staff       (20)        0 2024-01-25 19:23:45.733105 globalnoc-alertmon-agent-1.0.1/globalnoc_alertmon_agent/
--rw-r--r--   0 bengeels   (501) staff       (20)     7847 2024-01-25 19:17:50.000000 globalnoc-alertmon-agent-1.0.1/globalnoc_alertmon_agent/__init__.py
-drwxr-xr-x   0 bengeels   (501) staff       (20)        0 2024-01-25 19:23:45.735681 globalnoc-alertmon-agent-1.0.1/globalnoc_alertmon_agent.egg-info/
--rw-r--r--   0 bengeels   (501) staff       (20)      604 2024-01-25 19:23:45.000000 globalnoc-alertmon-agent-1.0.1/globalnoc_alertmon_agent.egg-info/PKG-INFO
--rw-r--r--   0 bengeels   (501) staff       (20)      302 2024-01-25 19:23:45.000000 globalnoc-alertmon-agent-1.0.1/globalnoc_alertmon_agent.egg-info/SOURCES.txt
--rw-r--r--   0 bengeels   (501) staff       (20)        1 2024-01-25 19:23:45.000000 globalnoc-alertmon-agent-1.0.1/globalnoc_alertmon_agent.egg-info/dependency_links.txt
--rw-r--r--   0 bengeels   (501) staff       (20)       35 2024-01-25 19:23:45.000000 globalnoc-alertmon-agent-1.0.1/globalnoc_alertmon_agent.egg-info/requires.txt
--rw-r--r--   0 bengeels   (501) staff       (20)       25 2024-01-25 19:23:45.000000 globalnoc-alertmon-agent-1.0.1/globalnoc_alertmon_agent.egg-info/top_level.txt
--rw-r--r--   0 bengeels   (501) staff       (20)       38 2024-01-25 19:23:45.736861 globalnoc-alertmon-agent-1.0.1/setup.cfg
--rw-r--r--   0 bengeels   (501) staff       (20)      643 2024-01-25 19:17:50.000000 globalnoc-alertmon-agent-1.0.1/setup.py
+drwxrwxr-x   0 saikappa (11202) saikappa (11202)        0 2024-05-06 17:55:21.177958 globalnoc-alertmon-agent-1.0.2/
+-rw-rw-r--   0 saikappa (11202) saikappa (11202)      556 2024-05-06 17:55:21.176958 globalnoc-alertmon-agent-1.0.2/PKG-INFO
+-rw-rw-r--   0 saikappa (11202) saikappa (11202)     1284 2024-05-06 17:13:52.000000 globalnoc-alertmon-agent-1.0.2/README.md
+drwxrwxr-x   0 saikappa (11202) saikappa (11202)        0 2024-05-06 17:55:21.176958 globalnoc-alertmon-agent-1.0.2/globalnoc_alertmon_agent.egg-info/
+-rw-rw-r--   0 saikappa (11202) saikappa (11202)      556 2024-05-06 17:55:21.000000 globalnoc-alertmon-agent-1.0.2/globalnoc_alertmon_agent.egg-info/PKG-INFO
+-rw-rw-r--   0 saikappa (11202) saikappa (11202)      257 2024-05-06 17:55:21.000000 globalnoc-alertmon-agent-1.0.2/globalnoc_alertmon_agent.egg-info/SOURCES.txt
+-rw-rw-r--   0 saikappa (11202) saikappa (11202)        1 2024-05-06 17:55:21.000000 globalnoc-alertmon-agent-1.0.2/globalnoc_alertmon_agent.egg-info/dependency_links.txt
+-rw-rw-r--   0 saikappa (11202) saikappa (11202)       35 2024-05-06 17:55:21.000000 globalnoc-alertmon-agent-1.0.2/globalnoc_alertmon_agent.egg-info/requires.txt
+-rw-rw-r--   0 saikappa (11202) saikappa (11202)        1 2024-05-06 17:55:21.000000 globalnoc-alertmon-agent-1.0.2/globalnoc_alertmon_agent.egg-info/top_level.txt
+-rw-rw-r--   0 saikappa (11202) saikappa (11202)       38 2024-05-06 17:55:21.177958 globalnoc-alertmon-agent-1.0.2/setup.cfg
+-rw-rw-r--   0 saikappa (11202) saikappa (11202)      643 2024-05-06 17:48:59.000000 globalnoc-alertmon-agent-1.0.2/setup.py
```

### Comparing `globalnoc-alertmon-agent-1.0.1/README.md` & `globalnoc-alertmon-agent-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `globalnoc-alertmon-agent-1.0.1/setup.py` & `globalnoc-alertmon-agent-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
   name="globalnoc-alertmon-agent",
-  version="1.0.1",
+  version="1.0.2",
   author="GlobalNOC Systems Engineering",
   author_email="syseng@globalnoc.iu.edu",
   python_requires='>=3.8.11, <4.0.0',
   description="Facilitates the process of submitting alerts to the GlobalNOC AlertMon system.",
   url="https://github.com/GlobalNOC/globalnoc-alertmon-agent",
   license="Apache License, Version 2.0 ",
   classifiers=[
```

