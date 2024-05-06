# Comparing `tmp/apache_airflow_providers_zendesk-4.7.0rc1.tar.gz` & `tmp/apache_airflow_providers_zendesk-4.7.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_zendesk-4.7.0rc1.tar", last modified: Mon Jan 22 08:32:06 2024, max compression
+gzip compressed data, was "apache_airflow_providers_zendesk-4.7.0rc2.tar", last modified: Tue Apr 30 11:49:29 2024, max compression
```

## Comparing `apache_airflow_providers_zendesk-4.7.0rc1.tar` & `apache_airflow_providers_zendesk-4.7.0rc2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     3056 2024-01-22 08:32:06.000000 apache_airflow_providers_zendesk-4.7.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-01-22 08:32:06.000000 apache_airflow_providers_zendesk-4.7.0rc1/airflow/providers/zendesk/LICENSE
--rw-r--r--   0        0        0     1582 2024-01-22 08:32:06.000000 apache_airflow_providers_zendesk-4.7.0rc1/airflow/providers/zendesk/__init__.py
--rw-r--r--   0        0        0     2418 2024-01-22 08:32:06.000000 apache_airflow_providers_zendesk-4.7.0rc1/airflow/providers/zendesk/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-01-22 08:32:06.000000 apache_airflow_providers_zendesk-4.7.0rc1/airflow/providers/zendesk/hooks/__init__.py
--rw-r--r--   0        0        0     4862 2024-01-22 08:32:06.000000 apache_airflow_providers_zendesk-4.7.0rc1/airflow/providers/zendesk/hooks/zendesk.py
--rw-r--r--   0        0        0     2925 2024-01-22 08:32:06.000000 apache_airflow_providers_zendesk-4.7.0rc1/pyproject.toml
--rw-r--r--   0        0        0     4701 1970-01-01 00:00:00.000000 apache_airflow_providers_zendesk-4.7.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     3061 2024-04-30 11:49:29.000000 apache_airflow_providers_zendesk-4.7.0rc2/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-30 11:49:29.000000 apache_airflow_providers_zendesk-4.7.0rc2/airflow/providers/zendesk/LICENSE
+-rw-r--r--   0        0        0     1582 2024-04-30 11:49:29.000000 apache_airflow_providers_zendesk-4.7.0rc2/airflow/providers/zendesk/__init__.py
+-rw-r--r--   0        0        0     2418 2024-04-30 11:49:29.000000 apache_airflow_providers_zendesk-4.7.0rc2/airflow/providers/zendesk/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:49:29.000000 apache_airflow_providers_zendesk-4.7.0rc2/airflow/providers/zendesk/hooks/__init__.py
+-rw-r--r--   0        0        0     4844 2024-04-30 11:49:29.000000 apache_airflow_providers_zendesk-4.7.0rc2/airflow/providers/zendesk/hooks/zendesk.py
+-rw-r--r--   0        0        0     2969 2024-04-30 11:49:29.000000 apache_airflow_providers_zendesk-4.7.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     4755 1970-01-01 00:00:00.000000 apache_airflow_providers_zendesk-4.7.0rc2/PKG-INFO
```

### Comparing `apache_airflow_providers_zendesk-4.7.0rc1/README.rst` & `apache_airflow_providers_zendesk-4.7.0rc2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-zendesk``
 
-Release: ``4.7.0.rc1``
+Release: ``4.7.0.rc2``
 
 
 `Zendesk <https://www.zendesk.com/>`__
 
 
 Provider package
 ----------------
@@ -60,21 +60,21 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-zendesk``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.6.0``
-``zenpy``           ``>=2.0.24``
+``apache-airflow``  ``>=2.7.0``
+``zenpy``           ``>=2.0.40``
 ==================  ==================
 
 The changelog for the provider package can be found in the
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-zendesk/4.7.0/changelog.html>`_.
```

### Comparing `apache_airflow_providers_zendesk-4.7.0rc1/airflow/providers/zendesk/LICENSE` & `apache_airflow_providers_zendesk-4.7.0rc2/airflow/providers/zendesk/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_zendesk-4.7.0rc1/airflow/providers/zendesk/__init__.py` & `apache_airflow_providers_zendesk-4.7.0rc2/airflow/providers/zendesk/__init__.py`

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
-        f"The package `apache-airflow-providers-zendesk:{__version__}` needs Apache Airflow 2.6.0+"
+        f"The package `apache-airflow-providers-zendesk:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_zendesk-4.7.0rc1/airflow/providers/zendesk/get_provider_info.py` & `apache_airflow_providers_zendesk-4.7.0rc2/airflow/providers/zendesk/get_provider_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-zendesk",
         "name": "Zendesk",
         "description": "`Zendesk <https://www.zendesk.com/>`__\n",
         "state": "ready",
-        "source-date-epoch": 1705912326,
+        "source-date-epoch": 1714477769,
         "versions": [
             "4.7.0",
             "4.6.0",
             "4.5.0",
             "4.4.0",
             "4.3.2",
             "4.3.1",
@@ -45,15 +45,15 @@
             "3.0.1",
             "3.0.0",
             "2.0.1",
             "2.0.0",
             "1.0.1",
             "1.0.0",
         ],
-        "dependencies": ["apache-airflow>=2.6.0", "zenpy>=2.0.24"],
+        "dependencies": ["apache-airflow>=2.7.0", "zenpy>=2.0.40"],
         "integrations": [
             {
                 "integration-name": "Zendesk",
                 "external-doc-url": "https://www.zendesk.com/",
                 "logo": "/integration-logos/zendesk/Zendesk.png",
                 "tags": ["software"],
             }
```

### Comparing `apache_airflow_providers_zendesk-4.7.0rc1/airflow/providers/zendesk/hooks/__init__.py` & `apache_airflow_providers_zendesk-4.7.0rc2/airflow/providers/zendesk/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_zendesk-4.7.0rc1/airflow/providers/zendesk/hooks/zendesk.py` & `apache_airflow_providers_zendesk-4.7.0rc2/airflow/providers/zendesk/hooks/zendesk.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,16 @@
     @classmethod
     def get_ui_field_behaviour(cls) -> dict[str, Any]:
         return {
             "hidden_fields": ["schema", "port", "extra"],
             "relabeling": {"host": "Zendesk domain", "login": "Zendesk email"},
         }
 
-    def __init__(self, zendesk_conn_id: str = default_conn_name, **kwargs) -> None:
-        super().__init__(**kwargs)
+    def __init__(self, zendesk_conn_id: str = default_conn_name) -> None:
+        super().__init__()
         self.zendesk_conn_id = zendesk_conn_id
         self.base_api: BaseApi | None = None
         zenpy_client, url = self._init_conn()
         self.zenpy_client = zenpy_client
         self.__url = url
         self.get = self.zenpy_client.users._get
```

### Comparing `apache_airflow_providers_zendesk-4.7.0rc1/pyproject.toml` & `apache_airflow_providers_zendesk-4.7.0rc2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-zendesk"
-version = "4.7.0.rc1"
+version = "4.7.0.rc2"
 description = "Provider package apache-airflow-providers-zendesk for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -47,20 +47,21 @@
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
-    "zenpy>=2.0.24",
+    "apache-airflow>=2.7.0rc0",
+    "zenpy>=2.0.40",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-zendesk/4.7.0"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-zendesk/4.7.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
```

### Comparing `apache_airflow_providers_zendesk-4.7.0rc1/PKG-INFO` & `apache_airflow_providers_zendesk-4.7.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-zendesk
-Version: 4.7.0rc1
+Version: 4.7.0rc2
 Summary: Provider package apache-airflow-providers-zendesk for Apache Airflow
 Keywords: airflow-provider,zendesk,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,17 +15,18 @@
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
-Requires-Dist: zenpy>=2.0.24
+Requires-Dist: apache-airflow>=2.7.0rc0
+Requires-Dist: zenpy>=2.0.40
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-zendesk/4.7.0/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-zendesk/4.7.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
@@ -70,15 +71,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-zendesk``
 
-Release: ``4.7.0.rc1``
+Release: ``4.7.0.rc2``
 
 
 `Zendesk <https://www.zendesk.com/>`__
 
 
 Provider package
 ----------------
@@ -92,21 +93,21 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-zendesk``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.6.0``
-``zenpy``           ``>=2.0.24``
+``apache-airflow``  ``>=2.7.0``
+``zenpy``           ``>=2.0.40``
 ==================  ==================
 
 The changelog for the provider package can be found in the
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-zendesk/4.7.0/changelog.html>`_.
```

