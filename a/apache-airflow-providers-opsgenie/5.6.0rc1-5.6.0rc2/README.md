# Comparing `tmp/apache_airflow_providers_opsgenie-5.6.0rc1.tar.gz` & `tmp/apache_airflow_providers_opsgenie-5.6.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_opsgenie-5.6.0rc1.tar", last modified: Mon Jan 22 08:29:57 2024, max compression
+gzip compressed data, was "apache_airflow_providers_opsgenie-5.6.0rc2.tar", last modified: Tue Apr 30 11:38:11 2024, max compression
```

## Comparing `apache_airflow_providers_opsgenie-5.6.0rc1.tar` & `apache_airflow_providers_opsgenie-5.6.0rc2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     3081 2024-01-22 08:29:57.000000 apache_airflow_providers_opsgenie-5.6.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-01-22 08:29:57.000000 apache_airflow_providers_opsgenie-5.6.0rc1/airflow/providers/opsgenie/LICENSE
--rw-r--r--   0        0        0     1583 2024-01-22 08:29:57.000000 apache_airflow_providers_opsgenie-5.6.0rc1/airflow/providers/opsgenie/__init__.py
--rw-r--r--   0        0        0     2898 2024-01-22 08:29:57.000000 apache_airflow_providers_opsgenie-5.6.0rc1/airflow/providers/opsgenie/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-01-22 08:29:57.000000 apache_airflow_providers_opsgenie-5.6.0rc1/airflow/providers/opsgenie/hooks/__init__.py
--rw-r--r--   0        0        0     6016 2024-01-22 08:29:57.000000 apache_airflow_providers_opsgenie-5.6.0rc1/airflow/providers/opsgenie/hooks/opsgenie.py
--rw-r--r--   0        0        0      785 2024-01-22 08:29:57.000000 apache_airflow_providers_opsgenie-5.6.0rc1/airflow/providers/opsgenie/notifications/__init__.py
--rw-r--r--   0        0        0     2626 2024-01-22 08:29:57.000000 apache_airflow_providers_opsgenie-5.6.0rc1/airflow/providers/opsgenie/notifications/opsgenie.py
--rw-r--r--   0        0        0      787 2024-01-22 08:29:57.000000 apache_airflow_providers_opsgenie-5.6.0rc1/airflow/providers/opsgenie/operators/__init__.py
--rw-r--r--   0        0        0     9793 2024-01-22 08:29:57.000000 apache_airflow_providers_opsgenie-5.6.0rc1/airflow/providers/opsgenie/operators/opsgenie.py
--rw-r--r--   0        0        0      785 2024-01-22 08:29:57.000000 apache_airflow_providers_opsgenie-5.6.0rc1/airflow/providers/opsgenie/typing/__init__.py
--rw-r--r--   0        0        0     2575 2024-01-22 08:29:57.000000 apache_airflow_providers_opsgenie-5.6.0rc1/airflow/providers/opsgenie/typing/opsgenie.py
--rw-r--r--   0        0        0     2938 2024-01-22 08:29:57.000000 apache_airflow_providers_opsgenie-5.6.0rc1/pyproject.toml
--rw-r--r--   0        0        0     4737 1970-01-01 00:00:00.000000 apache_airflow_providers_opsgenie-5.6.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     3086 2024-04-30 11:38:11.000000 apache_airflow_providers_opsgenie-5.6.0rc2/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-30 11:38:11.000000 apache_airflow_providers_opsgenie-5.6.0rc2/airflow/providers/opsgenie/LICENSE
+-rw-r--r--   0        0        0     1583 2024-04-30 11:38:11.000000 apache_airflow_providers_opsgenie-5.6.0rc2/airflow/providers/opsgenie/__init__.py
+-rw-r--r--   0        0        0     2898 2024-04-30 11:38:11.000000 apache_airflow_providers_opsgenie-5.6.0rc2/airflow/providers/opsgenie/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:38:11.000000 apache_airflow_providers_opsgenie-5.6.0rc2/airflow/providers/opsgenie/hooks/__init__.py
+-rw-r--r--   0        0        0     6024 2024-04-30 11:38:11.000000 apache_airflow_providers_opsgenie-5.6.0rc2/airflow/providers/opsgenie/hooks/opsgenie.py
+-rw-r--r--   0        0        0      785 2024-04-30 11:38:11.000000 apache_airflow_providers_opsgenie-5.6.0rc2/airflow/providers/opsgenie/notifications/__init__.py
+-rw-r--r--   0        0        0     2626 2024-04-30 11:38:11.000000 apache_airflow_providers_opsgenie-5.6.0rc2/airflow/providers/opsgenie/notifications/opsgenie.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:38:11.000000 apache_airflow_providers_opsgenie-5.6.0rc2/airflow/providers/opsgenie/operators/__init__.py
+-rw-r--r--   0        0        0     9793 2024-04-30 11:38:11.000000 apache_airflow_providers_opsgenie-5.6.0rc2/airflow/providers/opsgenie/operators/opsgenie.py
+-rw-r--r--   0        0        0      785 2024-04-30 11:38:11.000000 apache_airflow_providers_opsgenie-5.6.0rc2/airflow/providers/opsgenie/typing/__init__.py
+-rw-r--r--   0        0        0     2575 2024-04-30 11:38:11.000000 apache_airflow_providers_opsgenie-5.6.0rc2/airflow/providers/opsgenie/typing/opsgenie.py
+-rw-r--r--   0        0        0     2982 2024-04-30 11:38:11.000000 apache_airflow_providers_opsgenie-5.6.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     4791 1970-01-01 00:00:00.000000 apache_airflow_providers_opsgenie-5.6.0rc2/PKG-INFO
```

### Comparing `apache_airflow_providers_opsgenie-5.6.0rc1/README.rst` & `apache_airflow_providers_opsgenie-5.6.0rc2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-opsgenie``
 
-Release: ``5.6.0.rc1``
+Release: ``5.6.0.rc2``
 
 
 `Opsgenie <https://www.atlassian.com/software/opsgenie>`__
 
 
 Provider package
 ----------------
@@ -60,21 +60,21 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-opsgenie``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.6.0``
+``apache-airflow``  ``>=2.7.0``
 ``opsgenie-sdk``    ``>=2.1.5``
 ==================  ==================
 
 The changelog for the provider package can be found in the
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-opsgenie/5.6.0/changelog.html>`_.
```

### Comparing `apache_airflow_providers_opsgenie-5.6.0rc1/airflow/providers/opsgenie/LICENSE` & `apache_airflow_providers_opsgenie-5.6.0rc2/airflow/providers/opsgenie/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_opsgenie-5.6.0rc1/airflow/providers/opsgenie/__init__.py` & `apache_airflow_providers_opsgenie-5.6.0rc2/airflow/providers/opsgenie/__init__.py`

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
-        f"The package `apache-airflow-providers-opsgenie:{__version__}` needs Apache Airflow 2.6.0+"
+        f"The package `apache-airflow-providers-opsgenie:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_opsgenie-5.6.0rc1/airflow/providers/opsgenie/get_provider_info.py` & `apache_airflow_providers_opsgenie-5.6.0rc2/airflow/providers/opsgenie/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-opsgenie",
         "name": "Opsgenie",
         "description": "`Opsgenie <https://www.atlassian.com/software/opsgenie>`__\n",
         "state": "ready",
-        "source-date-epoch": 1705912197,
+        "source-date-epoch": 1714477091,
         "versions": [
             "5.6.0",
             "5.5.0",
             "5.4.0",
             "5.3.0",
             "5.2.0",
             "5.1.1",
@@ -46,15 +46,15 @@
             "3.0.0",
             "2.0.1",
             "2.0.0",
             "1.0.2",
             "1.0.1",
             "1.0.0",
         ],
-        "dependencies": ["apache-airflow>=2.6.0", "opsgenie-sdk>=2.1.5"],
+        "dependencies": ["apache-airflow>=2.7.0", "opsgenie-sdk>=2.1.5"],
         "integrations": [
             {
                 "integration-name": "Opsgenie",
                 "external-doc-url": "https://www.atlassian.com/software/opsgenie",
                 "how-to-guide": ["/docs/apache-airflow-providers-opsgenie/operators/opsgenie_alert.rst"],
                 "logo": "/integration-logos/opsgenie/Opsgenie.png",
                 "tags": ["service"],
```

### Comparing `apache_airflow_providers_opsgenie-5.6.0rc1/airflow/providers/opsgenie/hooks/__init__.py` & `apache_airflow_providers_opsgenie-5.6.0rc2/airflow/providers/opsgenie/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_opsgenie-5.6.0rc1/airflow/providers/opsgenie/hooks/opsgenie.py` & `apache_airflow_providers_opsgenie-5.6.0rc2/airflow/providers/opsgenie/hooks/opsgenie.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,16 +48,16 @@
     """
 
     conn_name_attr = "opsgenie_conn_id"
     default_conn_name = "opsgenie_default"
     conn_type = "opsgenie"
     hook_name = "Opsgenie"
 
-    def __init__(self, opsgenie_conn_id: str = "opsgenie_default", **kwargs) -> None:
-        super().__init__(**kwargs)  # type: ignore[misc]
+    def __init__(self, opsgenie_conn_id: str = "opsgenie_default") -> None:
+        super().__init__()  # type: ignore[misc]
         self.conn_id = opsgenie_conn_id
         configuration = Configuration()
         conn = self.get_connection(self.conn_id)
         configuration.api_key["Authorization"] = conn.password
         configuration.host = conn.host or "https://api.opsgenie.com"
         self.alert_api_instance = AlertApi(ApiClient(configuration))
 
@@ -157,12 +157,12 @@
             return api_response
         except OpenApiException as e:
             self.log.exception("Exception when calling AlertApi->delete_alert: %s\n", e)
             raise e
 
     @classmethod
     def get_ui_field_behaviour(cls) -> dict[str, Any]:
-        """Returns custom field behaviour."""
+        """Return custom UI field behaviour for Opsgenie connection."""
         return {
             "hidden_fields": ["port", "schema", "login", "extra"],
             "relabeling": {"password": "Opsgenie API Key"},
         }
```

### Comparing `apache_airflow_providers_opsgenie-5.6.0rc1/airflow/providers/opsgenie/notifications/__init__.py` & `apache_airflow_providers_opsgenie-5.6.0rc2/airflow/providers/opsgenie/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_opsgenie-5.6.0rc1/airflow/providers/opsgenie/notifications/opsgenie.py` & `apache_airflow_providers_opsgenie-5.6.0rc2/airflow/providers/opsgenie/notifications/opsgenie.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_opsgenie-5.6.0rc1/airflow/providers/opsgenie/operators/__init__.py` & `apache_airflow_providers_opsgenie-5.6.0rc2/airflow/providers/opsgenie/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_opsgenie-5.6.0rc1/airflow/providers/opsgenie/operators/opsgenie.py` & `apache_airflow_providers_opsgenie-5.6.0rc2/airflow/providers/opsgenie/operators/opsgenie.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_opsgenie-5.6.0rc1/airflow/providers/opsgenie/typing/__init__.py` & `apache_airflow_providers_opsgenie-5.6.0rc2/airflow/providers/opsgenie/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_opsgenie-5.6.0rc1/airflow/providers/opsgenie/typing/opsgenie.py` & `apache_airflow_providers_opsgenie-5.6.0rc2/airflow/providers/opsgenie/typing/opsgenie.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_opsgenie-5.6.0rc1/pyproject.toml` & `apache_airflow_providers_opsgenie-5.6.0rc2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-opsgenie"
-version = "5.6.0.rc1"
+version = "5.6.0.rc2"
 description = "Provider package apache-airflow-providers-opsgenie for Apache Airflow"
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
     "opsgenie-sdk>=2.1.5",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-opsgenie/5.6.0"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-opsgenie/5.6.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
```

### Comparing `apache_airflow_providers_opsgenie-5.6.0rc1/PKG-INFO` & `apache_airflow_providers_opsgenie-5.6.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-opsgenie
-Version: 5.6.0rc1
+Version: 5.6.0rc2
 Summary: Provider package apache-airflow-providers-opsgenie for Apache Airflow
 Keywords: airflow-provider,opsgenie,airflow,integration
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
 Requires-Dist: opsgenie-sdk>=2.1.5
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-opsgenie/5.6.0/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-opsgenie/5.6.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
@@ -70,15 +71,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-opsgenie``
 
-Release: ``5.6.0.rc1``
+Release: ``5.6.0.rc2``
 
 
 `Opsgenie <https://www.atlassian.com/software/opsgenie>`__
 
 
 Provider package
 ----------------
@@ -92,21 +93,21 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-opsgenie``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.6.0``
+``apache-airflow``  ``>=2.7.0``
 ``opsgenie-sdk``    ``>=2.1.5``
 ==================  ==================
 
 The changelog for the provider package can be found in the
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-opsgenie/5.6.0/changelog.html>`_.
```

