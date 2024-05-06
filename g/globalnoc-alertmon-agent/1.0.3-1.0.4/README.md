# Comparing `tmp/globalnoc-alertmon-agent-1.0.3.tar.gz` & `tmp/globalnoc_alertmon_agent-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globalnoc-alertmon-agent-1.0.3.tar", last modified: Mon May  6 19:19:39 2024, max compression
+gzip compressed data, was "globalnoc_alertmon_agent-1.0.4.tar", last modified: Mon May  6 20:19:06 2024, max compression
```

## Comparing `globalnoc-alertmon-agent-1.0.3.tar` & `globalnoc_alertmon_agent-1.0.4.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxr-x   0 saikappa (11202) saikappa (11202)        0 2024-05-06 19:19:39.364147 globalnoc-alertmon-agent-1.0.3/
--rw-rw-r--   0 saikappa (11202) saikappa (11202)      556 2024-05-06 19:19:39.363147 globalnoc-alertmon-agent-1.0.3/PKG-INFO
--rw-rw-r--   0 saikappa (11202) saikappa (11202)     1284 2024-05-06 17:13:52.000000 globalnoc-alertmon-agent-1.0.3/README.md
-drwxrwxr-x   0 saikappa (11202) saikappa (11202)        0 2024-05-06 19:19:39.363147 globalnoc-alertmon-agent-1.0.3/globalnoc_alertmon_agent.egg-info/
--rw-rw-r--   0 saikappa (11202) saikappa (11202)      556 2024-05-06 19:19:39.000000 globalnoc-alertmon-agent-1.0.3/globalnoc_alertmon_agent.egg-info/PKG-INFO
--rw-rw-r--   0 saikappa (11202) saikappa (11202)      257 2024-05-06 19:19:39.000000 globalnoc-alertmon-agent-1.0.3/globalnoc_alertmon_agent.egg-info/SOURCES.txt
--rw-rw-r--   0 saikappa (11202) saikappa (11202)        1 2024-05-06 19:19:39.000000 globalnoc-alertmon-agent-1.0.3/globalnoc_alertmon_agent.egg-info/dependency_links.txt
--rw-rw-r--   0 saikappa (11202) saikappa (11202)       35 2024-05-06 19:19:39.000000 globalnoc-alertmon-agent-1.0.3/globalnoc_alertmon_agent.egg-info/requires.txt
--rw-rw-r--   0 saikappa (11202) saikappa (11202)        1 2024-05-06 19:19:39.000000 globalnoc-alertmon-agent-1.0.3/globalnoc_alertmon_agent.egg-info/top_level.txt
--rw-rw-r--   0 saikappa (11202) saikappa (11202)       38 2024-05-06 19:19:39.364147 globalnoc-alertmon-agent-1.0.3/setup.cfg
--rw-rw-r--   0 saikappa (11202) saikappa (11202)      643 2024-05-06 19:18:03.000000 globalnoc-alertmon-agent-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:19:06.658745 globalnoc_alertmon_agent-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-06 20:19:02.000000 globalnoc_alertmon_agent-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-06 20:19:06.658745 globalnoc_alertmon_agent-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-06 20:19:02.000000 globalnoc_alertmon_agent-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:19:06.654745 globalnoc_alertmon_agent-1.0.4/globalnoc_alertmon_agent/
+-rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-05-06 20:19:02.000000 globalnoc_alertmon_agent-1.0.4/globalnoc_alertmon_agent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:19:06.658745 globalnoc_alertmon_agent-1.0.4/globalnoc_alertmon_agent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-06 20:19:06.000000 globalnoc_alertmon_agent-1.0.4/globalnoc_alertmon_agent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-06 20:19:06.000000 globalnoc_alertmon_agent-1.0.4/globalnoc_alertmon_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 20:19:06.000000 globalnoc_alertmon_agent-1.0.4/globalnoc_alertmon_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-06 20:19:06.000000 globalnoc_alertmon_agent-1.0.4/globalnoc_alertmon_agent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-06 20:19:06.000000 globalnoc_alertmon_agent-1.0.4/globalnoc_alertmon_agent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 20:19:06.658745 globalnoc_alertmon_agent-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-06 20:19:02.000000 globalnoc_alertmon_agent-1.0.4/setup.py
```

### Comparing `globalnoc-alertmon-agent-1.0.3/README.md` & `globalnoc_alertmon_agent-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `globalnoc-alertmon-agent-1.0.3/setup.py` & `globalnoc_alertmon_agent-1.0.4/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from setuptools import setup
 
 setup(
   name="globalnoc-alertmon-agent",
-  version="1.0.3",
+  version="1.0.4",
   author="GlobalNOC Systems Engineering",
   author_email="syseng@globalnoc.iu.edu",
   python_requires='>=3.8.11, <4.0.0',
   description="Facilitates the process of submitting alerts to the GlobalNOC AlertMon system.",
+  long_description=open('README.md').read(),
+  long_description_content_type='text/markdown',
   url="https://github.com/GlobalNOC/globalnoc-alertmon-agent",
   license="Apache License, Version 2.0 ",
   classifiers=[
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3"
   ],
```

