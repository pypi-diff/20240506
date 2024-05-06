# Comparing `tmp/apache_airflow_providers_apache_pinot-4.4.0rc1.tar.gz` & `tmp/apache_airflow_providers_apache_pinot-4.4.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_apache_pinot-4.4.0rc1.tar", last modified: Mon Jan 22 08:25:37 2024, max compression
+gzip compressed data, was "apache_airflow_providers_apache_pinot-4.4.0rc2.tar", last modified: Tue Apr 30 11:16:46 2024, max compression
```

## Comparing `apache_airflow_providers_apache_pinot-4.4.0rc1.tar` & `apache_airflow_providers_apache_pinot-4.4.0rc2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     4307 2024-01-22 08:25:37.000000 apache_airflow_providers_apache_pinot-4.4.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-01-22 08:25:37.000000 apache_airflow_providers_apache_pinot-4.4.0rc1/airflow/providers/apache/pinot/LICENSE
--rw-r--r--   0        0        0     1587 2024-01-22 08:25:37.000000 apache_airflow_providers_apache_pinot-4.4.0rc1/airflow/providers/apache/pinot/__init__.py
--rw-r--r--   0        0        0     2921 2024-01-22 08:25:37.000000 apache_airflow_providers_apache_pinot-4.4.0rc1/airflow/providers/apache/pinot/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-01-22 08:25:37.000000 apache_airflow_providers_apache_pinot-4.4.0rc1/airflow/providers/apache/pinot/hooks/__init__.py
--rw-r--r--   0        0        0    12127 2024-01-22 08:25:37.000000 apache_airflow_providers_apache_pinot-4.4.0rc1/airflow/providers/apache/pinot/hooks/pinot.py
--rw-r--r--   0        0        0     3109 2024-01-22 08:25:37.000000 apache_airflow_providers_apache_pinot-4.4.0rc1/pyproject.toml
--rw-r--r--   0        0        0     6142 1970-01-01 00:00:00.000000 apache_airflow_providers_apache_pinot-4.4.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     4313 2024-04-30 11:16:46.000000 apache_airflow_providers_apache_pinot-4.4.0rc2/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-30 11:16:46.000000 apache_airflow_providers_apache_pinot-4.4.0rc2/airflow/providers/apache/pinot/LICENSE
+-rw-r--r--   0        0        0     1587 2024-04-30 11:16:46.000000 apache_airflow_providers_apache_pinot-4.4.0rc2/airflow/providers/apache/pinot/__init__.py
+-rw-r--r--   0        0        0     2943 2024-04-30 11:16:46.000000 apache_airflow_providers_apache_pinot-4.4.0rc2/airflow/providers/apache/pinot/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:16:46.000000 apache_airflow_providers_apache_pinot-4.4.0rc2/airflow/providers/apache/pinot/hooks/__init__.py
+-rw-r--r--   0        0        0    12101 2024-04-30 11:16:46.000000 apache_airflow_providers_apache_pinot-4.4.0rc2/airflow/providers/apache/pinot/hooks/pinot.py
+-rw-r--r--   0        0        0     3152 2024-04-30 11:16:46.000000 apache_airflow_providers_apache_pinot-4.4.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     6196 1970-01-01 00:00:00.000000 apache_airflow_providers_apache_pinot-4.4.0rc2/PKG-INFO
```

### Comparing `apache_airflow_providers_apache_pinot-4.4.0rc1/README.rst` & `apache_airflow_providers_apache_pinot-4.4.0rc2/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-apache-pinot``
 
-Release: ``4.4.0.rc1``
+Release: ``4.4.0.rc2``
 
 
 `Apache Pinot <https://pinot.apache.org/>`__
 
 
 Provider package
 ----------------
@@ -60,25 +60,25 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apache-pinot``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
-``apache-airflow``                       ``>=2.6.0``
+``apache-airflow``                       ``>=2.7.0``
 ``apache-airflow-providers-common-sql``  ``>=1.3.1``
-``pinotdb``                              ``>0.4.7``
+``pinotdb``                              ``>=5.1.0``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
 Those are dependencies that might be needed in order to use all the features of the package.
 You need to install the specified provider packages in order to use them.
```

### Comparing `apache_airflow_providers_apache_pinot-4.4.0rc1/airflow/providers/apache/pinot/LICENSE` & `apache_airflow_providers_apache_pinot-4.4.0rc2/airflow/providers/apache/pinot/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_pinot-4.4.0rc1/airflow/providers/apache/pinot/__init__.py` & `apache_airflow_providers_apache_pinot-4.4.0rc2/airflow/providers/apache/pinot/__init__.py`

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
-        f"The package `apache-airflow-providers-apache-pinot:{__version__}` needs Apache Airflow 2.6.0+"
+        f"The package `apache-airflow-providers-apache-pinot:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_apache_pinot-4.4.0rc1/airflow/providers/apache/pinot/get_provider_info.py` & `apache_airflow_providers_apache_pinot-4.4.0rc2/airflow/providers/apache/pinot/get_provider_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,17 +24,18 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-apache-pinot",
         "name": "Apache Pinot",
         "description": "`Apache Pinot <https://pinot.apache.org/>`__\n",
         "state": "ready",
-        "source-date-epoch": 1705911937,
+        "source-date-epoch": 1714475806,
         "versions": [
             "4.4.0",
+            "4.3.1",
             "4.3.0",
             "4.2.0",
             "4.1.4",
             "4.1.3",
             "4.1.2",
             "4.1.1",
             "4.1.0",
@@ -49,17 +50,17 @@
             "2.0.2",
             "2.0.1",
             "2.0.0",
             "1.0.1",
             "1.0.0",
         ],
         "dependencies": [
-            "apache-airflow>=2.6.0",
+            "apache-airflow>=2.7.0",
             "apache-airflow-providers-common-sql>=1.3.1",
-            "pinotdb>0.4.7",
+            "pinotdb>=5.1.0",
         ],
         "integrations": [
             {
                 "integration-name": "Apache Pinot",
                 "external-doc-url": "https://pinot.apache.org/",
                 "logo": "/integration-logos/apache/pinot.png",
                 "tags": ["apache"],
```

### Comparing `apache_airflow_providers_apache_pinot-4.4.0rc1/airflow/providers/apache/pinot/hooks/__init__.py` & `apache_airflow_providers_apache_pinot-4.4.0rc2/airflow/providers/apache/pinot/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_pinot-4.4.0rc1/airflow/providers/apache/pinot/hooks/pinot.py` & `apache_airflow_providers_apache_pinot-4.4.0rc2/airflow/providers/apache/pinot/hooks/pinot.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,17 +64,16 @@
     hook_name = "Pinot Admin"
 
     def __init__(
         self,
         conn_id: str = "pinot_admin_default",
         cmd_path: str = "pinot-admin.sh",
         pinot_admin_system_exit: bool = False,
-        **kwargs,
     ) -> None:
-        super().__init__(**kwargs)
+        super().__init__()
         conn = self.get_connection(conn_id)
         self.host = conn.host
         self.port = str(conn.port)
         if cmd_path != "pinot-admin.sh":
             raise RuntimeError(
                 "In version 4.0.0 of the PinotAdminHook the cmd_path has been hard-coded to"
                 " pinot-admin.sh. In order to avoid accidental using of this parameter as"
```

### Comparing `apache_airflow_providers_apache_pinot-4.4.0rc1/pyproject.toml` & `apache_airflow_providers_apache_pinot-4.4.0rc2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-apache-pinot"
-version = "4.4.0.rc1"
+version = "4.4.0.rc2"
 description = "Provider package apache-airflow-providers-apache-pinot for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -47,21 +47,22 @@
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
-    "apache-airflow-providers-common-sql>=1.3.1.dev0",
-    "apache-airflow>=2.6.0.dev0",
-    "pinotdb>0.4.7",
+    "apache-airflow-providers-common-sql>=1.3.1rc0",
+    "apache-airflow>=2.7.0rc0",
+    "pinotdb>=5.1.0",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-apache-pinot/4.4.0"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-apache-pinot/4.4.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
```

### Comparing `apache_airflow_providers_apache_pinot-4.4.0rc1/PKG-INFO` & `apache_airflow_providers_apache_pinot-4.4.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-pinot
-Version: 4.4.0rc1
+Version: 4.4.0rc2
 Summary: Provider package apache-airflow-providers-apache-pinot for Apache Airflow
 Keywords: airflow-provider,apache.pinot,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,18 +15,19 @@
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Monitoring
-Requires-Dist: apache-airflow-providers-common-sql>=1.3.1.dev0
-Requires-Dist: apache-airflow>=2.6.0.dev0
-Requires-Dist: pinotdb>0.4.7
+Requires-Dist: apache-airflow-providers-common-sql>=1.3.1rc0
+Requires-Dist: apache-airflow>=2.7.0rc0
+Requires-Dist: pinotdb>=5.1.0
 Requires-Dist: apache-airflow-providers-common-sql ; extra == "common.sql"
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-apache-pinot/4.4.0/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-pinot/4.4.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
@@ -73,15 +74,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-apache-pinot``
 
-Release: ``4.4.0.rc1``
+Release: ``4.4.0.rc2``
 
 
 `Apache Pinot <https://pinot.apache.org/>`__
 
 
 Provider package
 ----------------
@@ -95,25 +96,25 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apache-pinot``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
-``apache-airflow``                       ``>=2.6.0``
+``apache-airflow``                       ``>=2.7.0``
 ``apache-airflow-providers-common-sql``  ``>=1.3.1``
-``pinotdb``                              ``>0.4.7``
+``pinotdb``                              ``>=5.1.0``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
 Those are dependencies that might be needed in order to use all the features of the package.
 You need to install the specified provider packages in order to use them.
```

