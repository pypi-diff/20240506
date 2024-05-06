# Comparing `tmp/apache_airflow_providers_trino-5.7.0.tar.gz` & `tmp/apache_airflow_providers_trino-5.7.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_trino-5.7.0.tar", last modified: Tue Apr 30 11:48:43 2024, max compression
+gzip compressed data, was "apache_airflow_providers_trino-5.7.0rc1.tar", last modified: Tue Apr 30 11:48:43 2024, max compression
```

## Comparing `apache_airflow_providers_trino-5.7.0.tar` & `apache_airflow_providers_trino-5.7.0rc1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     4569 2024-04-30 11:48:43.000000 apache_airflow_providers_trino-5.7.0/README.rst
--rw-r--r--   0        0        0    13569 2024-04-30 11:48:43.000000 apache_airflow_providers_trino-5.7.0/airflow/providers/trino/LICENSE
--rw-r--r--   0        0        0     1580 2024-04-30 11:48:43.000000 apache_airflow_providers_trino-5.7.0/airflow/providers/trino/__init__.py
--rw-r--r--   0        0        0      785 2024-04-30 11:48:43.000000 apache_airflow_providers_trino-5.7.0/airflow/providers/trino/datasets/__init__.py
--rw-r--r--   0        0        0     1371 2024-04-30 11:48:43.000000 apache_airflow_providers_trino-5.7.0/airflow/providers/trino/datasets/trino.py
--rw-r--r--   0        0        0     3509 2024-04-30 11:48:43.000000 apache_airflow_providers_trino-5.7.0/airflow/providers/trino/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-04-30 11:48:43.000000 apache_airflow_providers_trino-5.7.0/airflow/providers/trino/hooks/__init__.py
--rw-r--r--   0        0        0    10835 2024-04-30 11:48:43.000000 apache_airflow_providers_trino-5.7.0/airflow/providers/trino/hooks/trino.py
--rw-r--r--   0        0        0      785 2024-04-30 11:48:43.000000 apache_airflow_providers_trino-5.7.0/airflow/providers/trino/operators/__init__.py
--rw-r--r--   0        0        0     3346 2024-04-30 11:48:43.000000 apache_airflow_providers_trino-5.7.0/airflow/providers/trino/operators/trino.py
--rw-r--r--   0        0        0      787 2024-04-30 11:48:43.000000 apache_airflow_providers_trino-5.7.0/airflow/providers/trino/transfers/__init__.py
--rw-r--r--   0        0        0     5000 2024-04-30 11:48:43.000000 apache_airflow_providers_trino-5.7.0/airflow/providers/trino/transfers/gcs_to_trino.py
--rw-r--r--   0        0        0     3237 2024-04-30 11:48:43.000000 apache_airflow_providers_trino-5.7.0/pyproject.toml
--rw-r--r--   0        0        0     6637 1970-01-01 00:00:00.000000 apache_airflow_providers_trino-5.7.0/PKG-INFO
+-rw-r--r--   0        0        0     4573 2024-04-30 11:48:43.000000 apache_airflow_providers_trino-5.7.0rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-30 11:48:43.000000 apache_airflow_providers_trino-5.7.0rc1/airflow/providers/trino/LICENSE
+-rw-r--r--   0        0        0     1580 2024-04-30 11:48:43.000000 apache_airflow_providers_trino-5.7.0rc1/airflow/providers/trino/__init__.py
+-rw-r--r--   0        0        0      785 2024-04-30 11:48:43.000000 apache_airflow_providers_trino-5.7.0rc1/airflow/providers/trino/datasets/__init__.py
+-rw-r--r--   0        0        0     1371 2024-04-30 11:48:43.000000 apache_airflow_providers_trino-5.7.0rc1/airflow/providers/trino/datasets/trino.py
+-rw-r--r--   0        0        0     3509 2024-04-30 11:48:43.000000 apache_airflow_providers_trino-5.7.0rc1/airflow/providers/trino/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:48:43.000000 apache_airflow_providers_trino-5.7.0rc1/airflow/providers/trino/hooks/__init__.py
+-rw-r--r--   0        0        0    10835 2024-04-30 11:48:43.000000 apache_airflow_providers_trino-5.7.0rc1/airflow/providers/trino/hooks/trino.py
+-rw-r--r--   0        0        0      785 2024-04-30 11:48:43.000000 apache_airflow_providers_trino-5.7.0rc1/airflow/providers/trino/operators/__init__.py
+-rw-r--r--   0        0        0     3346 2024-04-30 11:48:43.000000 apache_airflow_providers_trino-5.7.0rc1/airflow/providers/trino/operators/trino.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:48:43.000000 apache_airflow_providers_trino-5.7.0rc1/airflow/providers/trino/transfers/__init__.py
+-rw-r--r--   0        0        0     5000 2024-04-30 11:48:43.000000 apache_airflow_providers_trino-5.7.0rc1/airflow/providers/trino/transfers/gcs_to_trino.py
+-rw-r--r--   0        0        0     3247 2024-04-30 11:48:43.000000 apache_airflow_providers_trino-5.7.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     6650 1970-01-01 00:00:00.000000 apache_airflow_providers_trino-5.7.0rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_trino-5.7.0/README.rst` & `apache_airflow_providers_trino-5.7.0rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-trino``
 
-Release: ``5.7.0``
+Release: ``5.7.0.rc1``
 
 
 `Trino <https://trino.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache_airflow_providers_trino-5.7.0/airflow/providers/trino/LICENSE` & `apache_airflow_providers_trino-5.7.0rc1/airflow/providers/trino/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_trino-5.7.0/airflow/providers/trino/__init__.py` & `apache_airflow_providers_trino-5.7.0rc1/airflow/providers/trino/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_trino-5.7.0/airflow/providers/trino/datasets/__init__.py` & `apache_airflow_providers_trino-5.7.0rc1/airflow/providers/trino/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_trino-5.7.0/airflow/providers/trino/datasets/trino.py` & `apache_airflow_providers_trino-5.7.0rc1/airflow/providers/trino/datasets/trino.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_trino-5.7.0/airflow/providers/trino/get_provider_info.py` & `apache_airflow_providers_trino-5.7.0rc1/airflow/providers/trino/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_trino-5.7.0/airflow/providers/trino/hooks/__init__.py` & `apache_airflow_providers_trino-5.7.0rc1/airflow/providers/trino/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_trino-5.7.0/airflow/providers/trino/hooks/trino.py` & `apache_airflow_providers_trino-5.7.0rc1/airflow/providers/trino/hooks/trino.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_trino-5.7.0/airflow/providers/trino/operators/__init__.py` & `apache_airflow_providers_trino-5.7.0rc1/airflow/providers/trino/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_trino-5.7.0/airflow/providers/trino/operators/trino.py` & `apache_airflow_providers_trino-5.7.0rc1/airflow/providers/trino/operators/trino.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_trino-5.7.0/airflow/providers/trino/transfers/__init__.py` & `apache_airflow_providers_trino-5.7.0rc1/airflow/providers/trino/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_trino-5.7.0/airflow/providers/trino/transfers/gcs_to_trino.py` & `apache_airflow_providers_trino-5.7.0rc1/airflow/providers/trino/transfers/gcs_to_trino.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_trino-5.7.0/pyproject.toml` & `apache_airflow_providers_trino-5.7.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-trino"
-version = "5.7.0"
+version = "5.7.0.rc1"
 description = "Provider package apache-airflow-providers-trino for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -52,16 +52,16 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: System :: Monitoring",
 ]
 requires-python = "~=3.8"
 dependencies = [
-    "apache-airflow-providers-common-sql>=1.3.1",
-    "apache-airflow>=2.7.0",
+    "apache-airflow-providers-common-sql>=1.3.1rc0",
+    "apache-airflow>=2.7.0rc0",
     "pandas>=1.2.5,<2.2",
     "trino>=0.318.0",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-trino/5.7.0"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-trino/5.7.0/changelog.html"
```

### Comparing `apache_airflow_providers_trino-5.7.0/PKG-INFO` & `apache_airflow_providers_trino-5.7.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-trino
-Version: 5.7.0
+Version: 5.7.0rc1
 Summary: Provider package apache-airflow-providers-trino for Apache Airflow
 Keywords: airflow-provider,trino,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,16 +17,16 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Monitoring
-Requires-Dist: apache-airflow-providers-common-sql>=1.3.1
-Requires-Dist: apache-airflow>=2.7.0
+Requires-Dist: apache-airflow-providers-common-sql>=1.3.1rc0
+Requires-Dist: apache-airflow>=2.7.0rc0
 Requires-Dist: pandas>=1.2.5,<2.2
 Requires-Dist: trino>=0.318.0
 Requires-Dist: apache-airflow-providers-common-sql ; extra == "common.sql"
 Requires-Dist: apache-airflow-providers-google ; extra == "google"
 Requires-Dist: apache-airflow-providers-openlineage ; extra == "openlineage"
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-trino/5.7.0/changelog.html
@@ -79,15 +79,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-trino``
 
-Release: ``5.7.0``
+Release: ``5.7.0.rc1``
 
 
 `Trino <https://trino.io/>`__
 
 
 Provider package
 ----------------
```

