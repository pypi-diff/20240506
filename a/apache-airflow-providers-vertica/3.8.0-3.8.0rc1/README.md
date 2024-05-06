# Comparing `tmp/apache_airflow_providers_vertica-3.8.0.tar.gz` & `tmp/apache_airflow_providers_vertica-3.8.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_vertica-3.8.0.tar", last modified: Tue Apr 30 11:48:59 2024, max compression
+gzip compressed data, was "apache_airflow_providers_vertica-3.8.0rc1.tar", last modified: Tue Apr 30 11:48:59 2024, max compression
```

## Comparing `apache_airflow_providers_vertica-3.8.0.tar` & `apache_airflow_providers_vertica-3.8.0rc1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     4268 2024-04-30 11:48:59.000000 apache_airflow_providers_vertica-3.8.0/README.rst
--rw-r--r--   0        0        0    13569 2024-04-30 11:48:59.000000 apache_airflow_providers_vertica-3.8.0/airflow/providers/vertica/LICENSE
--rw-r--r--   0        0        0     1582 2024-04-30 11:48:59.000000 apache_airflow_providers_vertica-3.8.0/airflow/providers/vertica/__init__.py
--rw-r--r--   0        0        0     2769 2024-04-30 11:48:59.000000 apache_airflow_providers_vertica-3.8.0/airflow/providers/vertica/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-04-30 11:48:59.000000 apache_airflow_providers_vertica-3.8.0/airflow/providers/vertica/hooks/__init__.py
--rw-r--r--   0        0        0     6123 2024-04-30 11:48:59.000000 apache_airflow_providers_vertica-3.8.0/airflow/providers/vertica/hooks/vertica.py
--rw-r--r--   0        0        0      787 2024-04-30 11:48:59.000000 apache_airflow_providers_vertica-3.8.0/airflow/providers/vertica/operators/__init__.py
--rw-r--r--   0        0        0     2033 2024-04-30 11:48:59.000000 apache_airflow_providers_vertica-3.8.0/airflow/providers/vertica/operators/vertica.py
--rw-r--r--   0        0        0     3114 2024-04-30 11:48:59.000000 apache_airflow_providers_vertica-3.8.0/pyproject.toml
--rw-r--r--   0        0        0     6124 1970-01-01 00:00:00.000000 apache_airflow_providers_vertica-3.8.0/PKG-INFO
+-rw-r--r--   0        0        0     4272 2024-04-30 11:48:59.000000 apache_airflow_providers_vertica-3.8.0rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-30 11:48:59.000000 apache_airflow_providers_vertica-3.8.0rc1/airflow/providers/vertica/LICENSE
+-rw-r--r--   0        0        0     1582 2024-04-30 11:48:59.000000 apache_airflow_providers_vertica-3.8.0rc1/airflow/providers/vertica/__init__.py
+-rw-r--r--   0        0        0     2769 2024-04-30 11:48:59.000000 apache_airflow_providers_vertica-3.8.0rc1/airflow/providers/vertica/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:48:59.000000 apache_airflow_providers_vertica-3.8.0rc1/airflow/providers/vertica/hooks/__init__.py
+-rw-r--r--   0        0        0     6123 2024-04-30 11:48:59.000000 apache_airflow_providers_vertica-3.8.0rc1/airflow/providers/vertica/hooks/vertica.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:48:59.000000 apache_airflow_providers_vertica-3.8.0rc1/airflow/providers/vertica/operators/__init__.py
+-rw-r--r--   0        0        0     2033 2024-04-30 11:48:59.000000 apache_airflow_providers_vertica-3.8.0rc1/airflow/providers/vertica/operators/vertica.py
+-rw-r--r--   0        0        0     3124 2024-04-30 11:48:59.000000 apache_airflow_providers_vertica-3.8.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     6137 1970-01-01 00:00:00.000000 apache_airflow_providers_vertica-3.8.0rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_vertica-3.8.0/README.rst` & `apache_airflow_providers_vertica-3.8.0rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-vertica``
 
-Release: ``3.8.0``
+Release: ``3.8.0.rc1``
 
 
 `Vertica <https://www.vertica.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache_airflow_providers_vertica-3.8.0/airflow/providers/vertica/LICENSE` & `apache_airflow_providers_vertica-3.8.0rc1/airflow/providers/vertica/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_vertica-3.8.0/airflow/providers/vertica/__init__.py` & `apache_airflow_providers_vertica-3.8.0rc1/airflow/providers/vertica/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_vertica-3.8.0/airflow/providers/vertica/get_provider_info.py` & `apache_airflow_providers_vertica-3.8.0rc1/airflow/providers/vertica/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_vertica-3.8.0/airflow/providers/vertica/hooks/__init__.py` & `apache_airflow_providers_vertica-3.8.0rc1/airflow/providers/vertica/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_vertica-3.8.0/airflow/providers/vertica/hooks/vertica.py` & `apache_airflow_providers_vertica-3.8.0rc1/airflow/providers/vertica/hooks/vertica.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_vertica-3.8.0/airflow/providers/vertica/operators/__init__.py` & `apache_airflow_providers_vertica-3.8.0rc1/airflow/providers/vertica/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_vertica-3.8.0/airflow/providers/vertica/operators/vertica.py` & `apache_airflow_providers_vertica-3.8.0rc1/airflow/providers/vertica/operators/vertica.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_vertica-3.8.0/pyproject.toml` & `apache_airflow_providers_vertica-3.8.0rc1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-vertica"
-version = "3.8.0"
+version = "3.8.0.rc1"
 description = "Provider package apache-airflow-providers-vertica for Apache Airflow"
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
     "vertica-python>=0.5.1",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-vertica/3.8.0"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-vertica/3.8.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
```

### Comparing `apache_airflow_providers_vertica-3.8.0/PKG-INFO` & `apache_airflow_providers_vertica-3.8.0rc1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-vertica
-Version: 3.8.0
+Version: 3.8.0rc1
 Summary: Provider package apache-airflow-providers-vertica for Apache Airflow
 Keywords: airflow-provider,vertica,airflow,integration
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
 Requires-Dist: vertica-python>=0.5.1
 Requires-Dist: apache-airflow-providers-common-sql ; extra == "common.sql"
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-vertica/3.8.0/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-vertica/3.8.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
@@ -74,15 +74,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-vertica``
 
-Release: ``3.8.0``
+Release: ``3.8.0.rc1``
 
 
 `Vertica <https://www.vertica.com/>`__
 
 
 Provider package
 ----------------
```

