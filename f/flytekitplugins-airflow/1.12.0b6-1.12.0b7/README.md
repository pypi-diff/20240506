# Comparing `tmp/flytekitplugins_airflow-1.12.0b6.tar.gz` & `tmp/flytekitplugins_airflow-1.12.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins_airflow-1.12.0b6.tar", last modified: Wed Apr 24 18:30:31 2024, max compression
+gzip compressed data, was "flytekitplugins_airflow-1.12.0b7.tar", last modified: Fri Apr 26 22:22:35 2024, max compression
```

## Comparing `flytekitplugins_airflow-1.12.0b6.tar` & `flytekitplugins_airflow-1.12.0b7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:31.957186 flytekitplugins_airflow-1.12.0b6/
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-24 18:30:31.953186 flytekitplugins_airflow-1.12.0b6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-24 18:30:04.000000 flytekitplugins_airflow-1.12.0b6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:31.953186 flytekitplugins_airflow-1.12.0b6/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:31.953186 flytekitplugins_airflow-1.12.0b6/flytekitplugins/airflow/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-24 18:30:04.000000 flytekitplugins_airflow-1.12.0b6/flytekitplugins/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7959 2024-04-24 18:30:04.000000 flytekitplugins_airflow-1.12.0b6/flytekitplugins/airflow/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     9131 2024-04-24 18:30:04.000000 flytekitplugins_airflow-1.12.0b6/flytekitplugins/airflow/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:31.953186 flytekitplugins_airflow-1.12.0b6/flytekitplugins_airflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-24 18:30:31.000000 flytekitplugins_airflow-1.12.0b6/flytekitplugins_airflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-24 18:30:31.000000 flytekitplugins_airflow-1.12.0b6/flytekitplugins_airflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 18:30:31.000000 flytekitplugins_airflow-1.12.0b6/flytekitplugins_airflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-24 18:30:31.000000 flytekitplugins_airflow-1.12.0b6/flytekitplugins_airflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-24 18:30:31.000000 flytekitplugins_airflow-1.12.0b6/flytekitplugins_airflow.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-24 18:30:31.000000 flytekitplugins_airflow-1.12.0b6/flytekitplugins_airflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-24 18:30:31.000000 flytekitplugins_airflow-1.12.0b6/flytekitplugins_airflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 18:30:31.957186 flytekitplugins_airflow-1.12.0b6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-24 18:30:31.000000 flytekitplugins_airflow-1.12.0b6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:31.953186 flytekitplugins_airflow-1.12.0b6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-24 18:30:04.000000 flytekitplugins_airflow-1.12.0b6/tests/test_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-04-24 18:30:04.000000 flytekitplugins_airflow-1.12.0b6/tests/test_task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:22:35.854202 flytekitplugins_airflow-1.12.0b7/
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-26 22:22:35.854202 flytekitplugins_airflow-1.12.0b7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-26 22:22:12.000000 flytekitplugins_airflow-1.12.0b7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:22:35.850202 flytekitplugins_airflow-1.12.0b7/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:22:35.850202 flytekitplugins_airflow-1.12.0b7/flytekitplugins/airflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-26 22:22:12.000000 flytekitplugins_airflow-1.12.0b7/flytekitplugins/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7959 2024-04-26 22:22:12.000000 flytekitplugins_airflow-1.12.0b7/flytekitplugins/airflow/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9131 2024-04-26 22:22:12.000000 flytekitplugins_airflow-1.12.0b7/flytekitplugins/airflow/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:22:35.854202 flytekitplugins_airflow-1.12.0b7/flytekitplugins_airflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-26 22:22:35.000000 flytekitplugins_airflow-1.12.0b7/flytekitplugins_airflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-26 22:22:35.000000 flytekitplugins_airflow-1.12.0b7/flytekitplugins_airflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 22:22:35.000000 flytekitplugins_airflow-1.12.0b7/flytekitplugins_airflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-26 22:22:35.000000 flytekitplugins_airflow-1.12.0b7/flytekitplugins_airflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-26 22:22:35.000000 flytekitplugins_airflow-1.12.0b7/flytekitplugins_airflow.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-26 22:22:35.000000 flytekitplugins_airflow-1.12.0b7/flytekitplugins_airflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-26 22:22:35.000000 flytekitplugins_airflow-1.12.0b7/flytekitplugins_airflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 22:22:35.854202 flytekitplugins_airflow-1.12.0b7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-26 22:22:35.000000 flytekitplugins_airflow-1.12.0b7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:22:35.854202 flytekitplugins_airflow-1.12.0b7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-26 22:22:12.000000 flytekitplugins_airflow-1.12.0b7/tests/test_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-04-26 22:22:12.000000 flytekitplugins_airflow-1.12.0b7/tests/test_task.py
```

### Comparing `flytekitplugins_airflow-1.12.0b6/PKG-INFO` & `flytekitplugins_airflow-1.12.0b7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-airflow
-Version: 1.12.0b6
+Version: 1.12.0b7
 Summary: This package holds the Airflow plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins_airflow-1.12.0b6/README.md` & `flytekitplugins_airflow-1.12.0b7/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins_airflow-1.12.0b6/flytekitplugins/airflow/agent.py` & `flytekitplugins_airflow-1.12.0b7/flytekitplugins/airflow/agent.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins_airflow-1.12.0b6/flytekitplugins/airflow/task.py` & `flytekitplugins_airflow-1.12.0b7/flytekitplugins/airflow/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins_airflow-1.12.0b6/flytekitplugins_airflow.egg-info/PKG-INFO` & `flytekitplugins_airflow-1.12.0b7/flytekitplugins_airflow.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-airflow
-Version: 1.12.0b6
+Version: 1.12.0b7
 Summary: This package holds the Airflow plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins_airflow-1.12.0b6/setup.py` & `flytekitplugins_airflow-1.12.0b7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 plugin_requires = [
     "apache-airflow",
     "flytekit>1.10.7",
     "flyteidl>1.10.7",
 ]
 
-__version__ = "1.12.0b6"
+__version__ = "1.12.0b7"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package holds the Airflow plugins for flytekit",
```

### Comparing `flytekitplugins_airflow-1.12.0b6/tests/test_agent.py` & `flytekitplugins_airflow-1.12.0b7/tests/test_agent.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins_airflow-1.12.0b6/tests/test_task.py` & `flytekitplugins_airflow-1.12.0b7/tests/test_task.py`

 * *Files identical despite different names*

