# Comparing `tmp/apache_airflow_providers_apache_kylin-3.6.0rc1.tar.gz` & `tmp/apache_airflow_providers_apache_kylin-3.6.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_apache_kylin-3.6.0rc1.tar", last modified: Mon Jan 22 08:25:31 2024, max compression
+gzip compressed data, was "apache_airflow_providers_apache_kylin-3.6.0rc2.tar", last modified: Tue Apr 30 11:15:39 2024, max compression
```

## Comparing `apache_airflow_providers_apache_kylin-3.6.0rc1.tar` & `apache_airflow_providers_apache_kylin-3.6.0rc2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3089 2024-01-22 08:25:31.000000 apache_airflow_providers_apache_kylin-3.6.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-01-22 08:25:31.000000 apache_airflow_providers_apache_kylin-3.6.0rc1/airflow/providers/apache/kylin/LICENSE
--rw-r--r--   0        0        0     1587 2024-01-22 08:25:31.000000 apache_airflow_providers_apache_kylin-3.6.0rc1/airflow/providers/apache/kylin/__init__.py
--rw-r--r--   0        0        0     2630 2024-01-22 08:25:31.000000 apache_airflow_providers_apache_kylin-3.6.0rc1/airflow/providers/apache/kylin/get_provider_info.py
--rw-r--r--   0        0        0      785 2024-01-22 08:25:31.000000 apache_airflow_providers_apache_kylin-3.6.0rc1/airflow/providers/apache/kylin/hooks/__init__.py
--rw-r--r--   0        0        0     2831 2024-01-22 08:25:31.000000 apache_airflow_providers_apache_kylin-3.6.0rc1/airflow/providers/apache/kylin/hooks/kylin.py
--rw-r--r--   0        0        0      785 2024-01-22 08:25:31.000000 apache_airflow_providers_apache_kylin-3.6.0rc1/airflow/providers/apache/kylin/operators/__init__.py
--rw-r--r--   0        0        0     7308 2024-01-22 08:25:31.000000 apache_airflow_providers_apache_kylin-3.6.0rc1/airflow/providers/apache/kylin/operators/kylin_cube.py
--rw-r--r--   0        0        0     2959 2024-01-22 08:25:31.000000 apache_airflow_providers_apache_kylin-3.6.0rc1/pyproject.toml
--rw-r--r--   0        0        0     4758 1970-01-01 00:00:00.000000 apache_airflow_providers_apache_kylin-3.6.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     3094 2024-04-30 11:15:39.000000 apache_airflow_providers_apache_kylin-3.6.0rc2/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-30 11:15:39.000000 apache_airflow_providers_apache_kylin-3.6.0rc2/airflow/providers/apache/kylin/LICENSE
+-rw-r--r--   0        0        0     1587 2024-04-30 11:15:39.000000 apache_airflow_providers_apache_kylin-3.6.0rc2/airflow/providers/apache/kylin/__init__.py
+-rw-r--r--   0        0        0     2630 2024-04-30 11:15:39.000000 apache_airflow_providers_apache_kylin-3.6.0rc2/airflow/providers/apache/kylin/get_provider_info.py
+-rw-r--r--   0        0        0      785 2024-04-30 11:15:39.000000 apache_airflow_providers_apache_kylin-3.6.0rc2/airflow/providers/apache/kylin/hooks/__init__.py
+-rw-r--r--   0        0        0     2805 2024-04-30 11:15:39.000000 apache_airflow_providers_apache_kylin-3.6.0rc2/airflow/providers/apache/kylin/hooks/kylin.py
+-rw-r--r--   0        0        0      785 2024-04-30 11:15:39.000000 apache_airflow_providers_apache_kylin-3.6.0rc2/airflow/providers/apache/kylin/operators/__init__.py
+-rw-r--r--   0        0        0     7308 2024-04-30 11:15:39.000000 apache_airflow_providers_apache_kylin-3.6.0rc2/airflow/providers/apache/kylin/operators/kylin_cube.py
+-rw-r--r--   0        0        0     3003 2024-04-30 11:15:39.000000 apache_airflow_providers_apache_kylin-3.6.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     4812 1970-01-01 00:00:00.000000 apache_airflow_providers_apache_kylin-3.6.0rc2/PKG-INFO
```

### Comparing `apache_airflow_providers_apache_kylin-3.6.0rc1/README.rst` & `apache_airflow_providers_apache_kylin-3.6.0rc2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-apache-kylin``
 
-Release: ``3.6.0.rc1``
+Release: ``3.6.0.rc2``
 
 
 `Apache Kylin <https://kylin.apache.org/>`__
 
 
 Provider package
 ----------------
@@ -60,21 +60,21 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apache-kylin``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.6.0``
+``apache-airflow``  ``>=2.7.0``
 ``kylinpy``         ``>=2.6``
 ==================  ==================
 
 The changelog for the provider package can be found in the
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-apache-kylin/3.6.0/changelog.html>`_.
```

### Comparing `apache_airflow_providers_apache_kylin-3.6.0rc1/airflow/providers/apache/kylin/LICENSE` & `apache_airflow_providers_apache_kylin-3.6.0rc2/airflow/providers/apache/kylin/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_kylin-3.6.0rc1/airflow/providers/apache/kylin/__init__.py` & `apache_airflow_providers_apache_kylin-3.6.0rc2/airflow/providers/apache/kylin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,12 +31,12 @@
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
-    "2.6.0"
+    "2.7.0"
 ):
     raise RuntimeError(
-        f"The package `apache-airflow-providers-apache-kylin:{__version__}` needs Apache Airflow 2.6.0+"
+        f"The package `apache-airflow-providers-apache-kylin:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_apache_kylin-3.6.0rc1/airflow/providers/apache/kylin/get_provider_info.py` & `apache_airflow_providers_apache_kylin-3.6.0rc2/airflow/providers/apache/kylin/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-apache-kylin",
         "name": "Apache Kylin",
         "description": "`Apache Kylin <https://kylin.apache.org/>`__\n",
         "state": "ready",
-        "source-date-epoch": 1705911931,
+        "source-date-epoch": 1714475739,
         "versions": [
             "3.6.0",
             "3.5.0",
             "3.4.0",
             "3.3.0",
             "3.2.1",
             "3.2.0",
@@ -42,15 +42,15 @@
             "2.0.3",
             "2.0.2",
             "2.0.1",
             "2.0.0",
             "1.0.1",
             "1.0.0",
         ],
-        "dependencies": ["apache-airflow>=2.6.0", "kylinpy>=2.6"],
+        "dependencies": ["apache-airflow>=2.7.0", "kylinpy>=2.6"],
         "integrations": [
             {
                 "integration-name": "Apache Kylin",
                 "external-doc-url": "https://kylin.apache.org/",
                 "logo": "/integration-logos/apache/kylin.png",
                 "tags": ["apache"],
             }
```

### Comparing `apache_airflow_providers_apache_kylin-3.6.0rc1/airflow/providers/apache/kylin/hooks/__init__.py` & `apache_airflow_providers_apache_kylin-3.6.0rc2/airflow/providers/apache/kylin/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_kylin-3.6.0rc1/airflow/providers/apache/kylin/hooks/kylin.py` & `apache_airflow_providers_apache_kylin-3.6.0rc2/airflow/providers/apache/kylin/hooks/kylin.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,17 +38,16 @@
     hook_name = "Apache Kylin"
 
     def __init__(
         self,
         kylin_conn_id: str = default_conn_name,
         project: str | None = None,
         dsn: str | None = None,
-        **kwargs,
     ):
-        super().__init__(**kwargs)
+        super().__init__()
         self.kylin_conn_id = kylin_conn_id
         self.project = project
         self.dsn = dsn
 
     def get_conn(self):
         conn = self.get_connection(self.kylin_conn_id)
         if self.dsn:
```

### Comparing `apache_airflow_providers_apache_kylin-3.6.0rc1/airflow/providers/apache/kylin/operators/__init__.py` & `apache_airflow_providers_apache_kylin-3.6.0rc2/airflow/providers/apache/kylin/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_kylin-3.6.0rc1/airflow/providers/apache/kylin/operators/kylin_cube.py` & `apache_airflow_providers_apache_kylin-3.6.0rc2/airflow/providers/apache/kylin/operators/kylin_cube.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_kylin-3.6.0rc1/pyproject.toml` & `apache_airflow_providers_apache_kylin-3.6.0rc2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-apache-kylin"
-version = "3.6.0.rc1"
+version = "3.6.0.rc2"
 description = "Provider package apache-airflow-providers-apache-kylin for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -47,19 +47,20 @@
     "Framework :: Apache Airflow",
     "Framework :: Apache Airflow :: Provider",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: System :: Monitoring",
 ]
 requires-python = "~=3.8"
 dependencies = [
-    "apache-airflow>=2.6.0.dev0",
+    "apache-airflow>=2.7.0rc0",
     "kylinpy>=2.6",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-apache-kylin/3.6.0"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-apache-kylin/3.6.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
```

### Comparing `apache_airflow_providers_apache_kylin-3.6.0rc1/PKG-INFO` & `apache_airflow_providers_apache_kylin-3.6.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-kylin
-Version: 3.6.0rc1
+Version: 3.6.0rc2
 Summary: Provider package apache-airflow-providers-apache-kylin for Apache Airflow
 Keywords: airflow-provider,apache.kylin,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,16 +15,17 @@
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Monitoring
-Requires-Dist: apache-airflow>=2.6.0.dev0
+Requires-Dist: apache-airflow>=2.7.0rc0
 Requires-Dist: kylinpy>=2.6
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-apache-kylin/3.6.0/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-kylin/3.6.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
@@ -70,15 +71,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-apache-kylin``
 
-Release: ``3.6.0.rc1``
+Release: ``3.6.0.rc2``
 
 
 `Apache Kylin <https://kylin.apache.org/>`__
 
 
 Provider package
 ----------------
@@ -92,21 +93,21 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apache-kylin``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.6.0``
+``apache-airflow``  ``>=2.7.0``
 ``kylinpy``         ``>=2.6``
 ==================  ==================
 
 The changelog for the provider package can be found in the
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-apache-kylin/3.6.0/changelog.html>`_.
```
