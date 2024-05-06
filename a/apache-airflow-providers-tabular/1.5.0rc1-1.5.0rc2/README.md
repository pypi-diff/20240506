# Comparing `tmp/apache_airflow_providers_tabular-1.5.0rc1.tar.gz` & `tmp/apache_airflow_providers_tabular-1.5.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_tabular-1.5.0rc1.tar", last modified: Mon Jan 22 08:31:33 2024, max compression
+gzip compressed data, was "apache_airflow_providers_tabular-1.5.0rc2.tar", last modified: Tue Apr 30 11:47:40 2024, max compression
```

## Comparing `apache_airflow_providers_tabular-1.5.0rc1.tar` & `apache_airflow_providers_tabular-1.5.0rc2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     3018 2024-01-22 08:31:33.000000 apache_airflow_providers_tabular-1.5.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-01-22 08:31:33.000000 apache_airflow_providers_tabular-1.5.0rc1/airflow/providers/tabular/LICENSE
--rw-r--r--   0        0        0     1582 2024-01-22 08:31:33.000000 apache_airflow_providers_tabular-1.5.0rc1/airflow/providers/tabular/__init__.py
--rw-r--r--   0        0        0     2141 2024-01-22 08:31:33.000000 apache_airflow_providers_tabular-1.5.0rc1/airflow/providers/tabular/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-01-22 08:31:33.000000 apache_airflow_providers_tabular-1.5.0rc1/airflow/providers/tabular/hooks/__init__.py
--rw-r--r--   0        0        0     3356 2024-01-22 08:31:33.000000 apache_airflow_providers_tabular-1.5.0rc1/airflow/providers/tabular/hooks/tabular.py
--rw-r--r--   0        0        0     2904 2024-01-22 08:31:33.000000 apache_airflow_providers_tabular-1.5.0rc1/pyproject.toml
--rw-r--r--   0        0        0     4634 1970-01-01 00:00:00.000000 apache_airflow_providers_tabular-1.5.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     3023 2024-04-30 11:47:40.000000 apache_airflow_providers_tabular-1.5.0rc2/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-30 11:47:40.000000 apache_airflow_providers_tabular-1.5.0rc2/airflow/providers/tabular/LICENSE
+-rw-r--r--   0        0        0     1582 2024-04-30 11:47:40.000000 apache_airflow_providers_tabular-1.5.0rc2/airflow/providers/tabular/__init__.py
+-rw-r--r--   0        0        0     2141 2024-04-30 11:47:40.000000 apache_airflow_providers_tabular-1.5.0rc2/airflow/providers/tabular/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:47:40.000000 apache_airflow_providers_tabular-1.5.0rc2/airflow/providers/tabular/hooks/__init__.py
+-rw-r--r--   0        0        0     3363 2024-04-30 11:47:40.000000 apache_airflow_providers_tabular-1.5.0rc2/airflow/providers/tabular/hooks/tabular.py
+-rw-r--r--   0        0        0     2948 2024-04-30 11:47:40.000000 apache_airflow_providers_tabular-1.5.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     4688 1970-01-01 00:00:00.000000 apache_airflow_providers_tabular-1.5.0rc2/PKG-INFO
```

### Comparing `apache_airflow_providers_tabular-1.5.0rc1/README.rst` & `apache_airflow_providers_tabular-1.5.0rc2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-tabular``
 
-Release: ``1.5.0.rc1``
+Release: ``1.5.0.rc2``
 
 
 `Tabular <https://tabular.io/>`__
 
 
 Provider package
 ----------------
@@ -60,20 +60,20 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-tabular``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.6.0``
+``apache-airflow``  ``>=2.7.0``
 ==================  ==================
 
 The changelog for the provider package can be found in the
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-tabular/1.5.0/changelog.html>`_.
```

### Comparing `apache_airflow_providers_tabular-1.5.0rc1/airflow/providers/tabular/LICENSE` & `apache_airflow_providers_tabular-1.5.0rc2/airflow/providers/tabular/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_tabular-1.5.0rc1/airflow/providers/tabular/__init__.py` & `apache_airflow_providers_tabular-1.5.0rc2/airflow/providers/tabular/__init__.py`

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
-        f"The package `apache-airflow-providers-tabular:{__version__}` needs Apache Airflow 2.6.0+"
+        f"The package `apache-airflow-providers-tabular:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_tabular-1.5.0rc1/airflow/providers/tabular/get_provider_info.py` & `apache_airflow_providers_tabular-1.5.0rc2/airflow/providers/tabular/get_provider_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-tabular",
         "name": "Tabular",
         "description": "`Tabular <https://tabular.io/>`__\n",
         "state": "ready",
-        "source-date-epoch": 1705912293,
+        "source-date-epoch": 1714477660,
         "versions": ["1.5.0", "1.4.1", "1.4.0", "1.3.0", "1.2.1", "1.2.0", "1.1.0", "1.0.1", "1.0.0"],
-        "dependencies": ["apache-airflow>=2.6.0"],
+        "dependencies": ["apache-airflow>=2.7.0"],
         "devel-dependencies": ["pyiceberg>=0.5.0"],
         "integrations": [
             {
                 "integration-name": "Tabular",
                 "external-doc-url": "https://tabular.io/docs/",
                 "logo": "/integration-logos/tabular/tabular.jpeg",
                 "tags": ["software"],
```

### Comparing `apache_airflow_providers_tabular-1.5.0rc1/airflow/providers/tabular/hooks/__init__.py` & `apache_airflow_providers_tabular-1.5.0rc2/airflow/providers/tabular/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_tabular-1.5.0rc1/airflow/providers/tabular/hooks/tabular.py` & `apache_airflow_providers_tabular-1.5.0rc2/airflow/providers/tabular/hooks/tabular.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,31 +42,31 @@
     conn_name_attr = "tabular_conn_id"
     default_conn_name = "tabular_default"
     conn_type = "tabular"
     hook_name = "Tabular"
 
     @classmethod
     def get_ui_field_behaviour(cls) -> dict[str, Any]:
-        """Returns custom field behaviour."""
+        """Return custom UI field behaviour for Tabular connection."""
         return {
             "hidden_fields": ["schema", "port"],
             "relabeling": {
                 "host": "Base URL",
                 "login": "Client ID",
                 "password": "Client Secret",
             },
             "placeholders": {
                 "host": DEFAULT_TABULAR_URL,
                 "login": "client_id (token credentials auth)",
                 "password": "secret (token credentials auth)",
             },
         }
 
-    def __init__(self, tabular_conn_id: str = default_conn_name, **kwargs) -> None:
-        super().__init__(**kwargs)
+    def __init__(self, tabular_conn_id: str = default_conn_name) -> None:
+        super().__init__()
         self.conn_id = tabular_conn_id
 
     def test_connection(self) -> tuple[bool, str]:
         """Test the Tabular connection."""
         try:
             self.get_conn()
             return True, "Successfully fetched token from Tabular"
```

### Comparing `apache_airflow_providers_tabular-1.5.0rc1/pyproject.toml` & `apache_airflow_providers_tabular-1.5.0rc2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-tabular"
-version = "1.5.0.rc1"
+version = "1.5.0.rc2"
 description = "Provider package apache-airflow-providers-tabular for Apache Airflow"
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
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-tabular/1.5.0"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-tabular/1.5.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
```

### Comparing `apache_airflow_providers_tabular-1.5.0rc1/PKG-INFO` & `apache_airflow_providers_tabular-1.5.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-tabular
-Version: 1.5.0rc1
+Version: 1.5.0rc2
 Summary: Provider package apache-airflow-providers-tabular for Apache Airflow
 Keywords: airflow-provider,tabular,airflow,integration
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
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-tabular/1.5.0/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-tabular/1.5.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
@@ -69,15 +70,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-tabular``
 
-Release: ``1.5.0.rc1``
+Release: ``1.5.0.rc2``
 
 
 `Tabular <https://tabular.io/>`__
 
 
 Provider package
 ----------------
@@ -91,20 +92,20 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-tabular``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.6.0``
+``apache-airflow``  ``>=2.7.0``
 ==================  ==================
 
 The changelog for the provider package can be found in the
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-tabular/1.5.0/changelog.html>`_.
```

