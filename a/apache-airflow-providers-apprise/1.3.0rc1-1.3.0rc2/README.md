# Comparing `tmp/apache_airflow_providers_apprise-1.3.0rc1.tar.gz` & `tmp/apache_airflow_providers_apprise-1.3.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_apprise-1.3.0rc1.tar", last modified: Mon Jan 22 08:25:45 2024, max compression
+gzip compressed data, was "apache_airflow_providers_apprise-1.3.0rc2.tar", last modified: Tue Apr 30 11:17:54 2024, max compression
```

## Comparing `apache_airflow_providers_apprise-1.3.0rc1.tar` & `apache_airflow_providers_apprise-1.3.0rc2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3044 2024-01-22 08:25:45.000000 apache_airflow_providers_apprise-1.3.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-01-22 08:25:45.000000 apache_airflow_providers_apprise-1.3.0rc1/airflow/providers/apprise/LICENSE
--rw-r--r--   0        0        0     1582 2024-01-22 08:25:45.000000 apache_airflow_providers_apprise-1.3.0rc1/airflow/providers/apprise/__init__.py
--rw-r--r--   0        0        0     2132 2024-01-22 08:25:45.000000 apache_airflow_providers_apprise-1.3.0rc1/airflow/providers/apprise/get_provider_info.py
--rw-r--r--   0        0        0     1053 2024-01-22 08:25:45.000000 apache_airflow_providers_apprise-1.3.0rc1/airflow/providers/apprise/hooks/__init__.py
--rw-r--r--   0        0        0     5231 2024-01-22 08:25:45.000000 apache_airflow_providers_apprise-1.3.0rc1/airflow/providers/apprise/hooks/apprise.py
--rw-r--r--   0        0        0     1053 2024-01-22 08:25:45.000000 apache_airflow_providers_apprise-1.3.0rc1/airflow/providers/apprise/notifications/__init__.py
--rw-r--r--   0        0        0     3477 2024-01-22 08:25:45.000000 apache_airflow_providers_apprise-1.3.0rc1/airflow/providers/apprise/notifications/apprise.py
--rw-r--r--   0        0        0     2919 2024-01-22 08:25:45.000000 apache_airflow_providers_apprise-1.3.0rc1/pyproject.toml
--rw-r--r--   0        0        0     4683 1970-01-01 00:00:00.000000 apache_airflow_providers_apprise-1.3.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     3049 2024-04-30 11:17:54.000000 apache_airflow_providers_apprise-1.3.0rc2/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-30 11:17:54.000000 apache_airflow_providers_apprise-1.3.0rc2/airflow/providers/apprise/LICENSE
+-rw-r--r--   0        0        0     1582 2024-04-30 11:17:54.000000 apache_airflow_providers_apprise-1.3.0rc2/airflow/providers/apprise/__init__.py
+-rw-r--r--   0        0        0     2141 2024-04-30 11:17:54.000000 apache_airflow_providers_apprise-1.3.0rc2/airflow/providers/apprise/get_provider_info.py
+-rw-r--r--   0        0        0     1053 2024-04-30 11:17:54.000000 apache_airflow_providers_apprise-1.3.0rc2/airflow/providers/apprise/hooks/__init__.py
+-rw-r--r--   0        0        0     5276 2024-04-30 11:17:54.000000 apache_airflow_providers_apprise-1.3.0rc2/airflow/providers/apprise/hooks/apprise.py
+-rw-r--r--   0        0        0     1053 2024-04-30 11:17:54.000000 apache_airflow_providers_apprise-1.3.0rc2/airflow/providers/apprise/notifications/__init__.py
+-rw-r--r--   0        0        0     3477 2024-04-30 11:17:54.000000 apache_airflow_providers_apprise-1.3.0rc2/airflow/providers/apprise/notifications/apprise.py
+-rw-r--r--   0        0        0     2963 2024-04-30 11:17:54.000000 apache_airflow_providers_apprise-1.3.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     4737 1970-01-01 00:00:00.000000 apache_airflow_providers_apprise-1.3.0rc2/PKG-INFO
```

### Comparing `apache_airflow_providers_apprise-1.3.0rc1/README.rst` & `apache_airflow_providers_apprise-1.3.0rc2/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-apprise``
 
-Release: ``1.3.0.rc1``
+Release: ``1.3.0.rc2``
 
 
 `Apprise <https://github.com/caronc/apprise>`__
 
 
 Provider package
 ----------------
@@ -60,21 +60,21 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apprise``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.6.0``
+``apache-airflow``  ``>=2.7.0``
 ``apprise``
 ==================  ==================
 
 The changelog for the provider package can be found in the
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-apprise/1.3.0/changelog.html>`_.
```

### Comparing `apache_airflow_providers_apprise-1.3.0rc1/airflow/providers/apprise/LICENSE` & `apache_airflow_providers_apprise-1.3.0rc2/airflow/providers/apprise/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apprise-1.3.0rc1/airflow/providers/apprise/__init__.py` & `apache_airflow_providers_apprise-1.3.0rc2/airflow/providers/apprise/__init__.py`

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
-        f"The package `apache-airflow-providers-apprise:{__version__}` needs Apache Airflow 2.6.0+"
+        f"The package `apache-airflow-providers-apprise:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_apprise-1.3.0rc1/airflow/providers/apprise/get_provider_info.py` & `apache_airflow_providers_apprise-1.3.0rc2/airflow/providers/apprise/get_provider_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,24 +24,24 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-apprise",
         "name": "Apprise",
         "description": "`Apprise <https://github.com/caronc/apprise>`__\n",
         "state": "ready",
-        "source-date-epoch": 1705911945,
-        "versions": ["1.3.0", "1.2.1", "1.2.0", "1.1.0", "1.0.2", "1.0.1", "1.0.0"],
+        "source-date-epoch": 1714475874,
+        "versions": ["1.3.0", "1.2.2", "1.2.1", "1.2.0", "1.1.0", "1.0.2", "1.0.1", "1.0.0"],
         "integrations": [
             {
                 "integration-name": "Apprise",
                 "external-doc-url": "https://github.com/caronc/apprise",
                 "tags": ["software"],
             }
         ],
-        "dependencies": ["apache-airflow>=2.6.0", "apprise"],
+        "dependencies": ["apache-airflow>=2.7.0", "apprise"],
         "hooks": [
             {"integration-name": "Apprise", "python-modules": ["airflow.providers.apprise.hooks.apprise"]}
         ],
         "connection-types": [
             {
                 "hook-class-name": "airflow.providers.apprise.hooks.apprise.AppriseHook",
                 "connection-type": "apprise",
```

### Comparing `apache_airflow_providers_apprise-1.3.0rc1/airflow/providers/apprise/hooks/__init__.py` & `apache_airflow_providers_apprise-1.3.0rc2/airflow/providers/apprise/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apprise-1.3.0rc1/airflow/providers/apprise/hooks/apprise.py` & `apache_airflow_providers_apprise-1.3.0rc2/airflow/providers/apprise/hooks/apprise.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,21 +38,22 @@
     """
 
     conn_name_attr = "apprise_conn_id"
     default_conn_name = "apprise_default"
     conn_type = "apprise"
     hook_name = "Apprise"
 
-    def __init__(self, apprise_conn_id: str = default_conn_name, **kwargs) -> None:
-        super().__init__(**kwargs)
+    def __init__(self, apprise_conn_id: str = default_conn_name) -> None:
+        super().__init__()
         self.apprise_conn_id = apprise_conn_id
 
     def get_config_from_conn(self):
         conn = self.get_connection(self.apprise_conn_id)
-        return json.loads(conn.extra_dejson["config"])
+        config = conn.extra_dejson["config"]
+        return json.loads(config) if isinstance(config, str) else config
 
     def set_config_from_conn(self, apprise_obj: apprise.Apprise):
         """Set config from connection to apprise object."""
         config_object = self.get_config_from_conn()
         if isinstance(config_object, list):
             for config in config_object:
                 apprise_obj.add(config["path"], tag=config.get("tag", None))
```

### Comparing `apache_airflow_providers_apprise-1.3.0rc1/airflow/providers/apprise/notifications/__init__.py` & `apache_airflow_providers_apprise-1.3.0rc2/airflow/providers/apprise/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apprise-1.3.0rc1/airflow/providers/apprise/notifications/apprise.py` & `apache_airflow_providers_apprise-1.3.0rc2/airflow/providers/apprise/notifications/apprise.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apprise-1.3.0rc1/pyproject.toml` & `apache_airflow_providers_apprise-1.3.0rc2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-apprise"
-version = "1.3.0.rc1"
+version = "1.3.0.rc2"
 description = "Provider package apache-airflow-providers-apprise for Apache Airflow"
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
     "apprise",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-apprise/1.3.0"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-apprise/1.3.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
```

### Comparing `apache_airflow_providers_apprise-1.3.0rc1/PKG-INFO` & `apache_airflow_providers_apprise-1.3.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apprise
-Version: 1.3.0rc1
+Version: 1.3.0rc2
 Summary: Provider package apache-airflow-providers-apprise for Apache Airflow
 Keywords: airflow-provider,apprise,airflow,integration
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
 Requires-Dist: apprise
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-apprise/1.3.0/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apprise/1.3.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
@@ -70,15 +71,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-apprise``
 
-Release: ``1.3.0.rc1``
+Release: ``1.3.0.rc2``
 
 
 `Apprise <https://github.com/caronc/apprise>`__
 
 
 Provider package
 ----------------
@@ -92,21 +93,21 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apprise``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.6.0``
+``apache-airflow``  ``>=2.7.0``
 ``apprise``
 ==================  ==================
 
 The changelog for the provider package can be found in the
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-apprise/1.3.0/changelog.html>`_.
```

