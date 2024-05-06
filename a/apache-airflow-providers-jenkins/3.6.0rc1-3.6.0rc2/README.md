# Comparing `tmp/apache_airflow_providers_jenkins-3.6.0rc1.tar.gz` & `tmp/apache_airflow_providers_jenkins-3.6.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_jenkins-3.6.0rc1.tar", last modified: Mon Jan 22 08:29:09 2024, max compression
+gzip compressed data, was "apache_airflow_providers_jenkins-3.6.0rc2.tar", last modified: Tue Apr 30 11:31:53 2024, max compression
```

## Comparing `apache_airflow_providers_jenkins-3.6.0rc1.tar` & `apache_airflow_providers_jenkins-3.6.0rc2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     3050 2024-01-22 08:29:09.000000 apache_airflow_providers_jenkins-3.6.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-01-22 08:29:09.000000 apache_airflow_providers_jenkins-3.6.0rc1/airflow/providers/jenkins/LICENSE
--rw-r--r--   0        0        0     1582 2024-01-22 08:29:09.000000 apache_airflow_providers_jenkins-3.6.0rc1/airflow/providers/jenkins/__init__.py
--rw-r--r--   0        0        0     2866 2024-01-22 08:29:09.000000 apache_airflow_providers_jenkins-3.6.0rc1/airflow/providers/jenkins/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-01-22 08:29:09.000000 apache_airflow_providers_jenkins-3.6.0rc1/airflow/providers/jenkins/hooks/__init__.py
--rw-r--r--   0        0        0     3900 2024-01-22 08:29:09.000000 apache_airflow_providers_jenkins-3.6.0rc1/airflow/providers/jenkins/hooks/jenkins.py
--rw-r--r--   0        0        0      787 2024-01-22 08:29:09.000000 apache_airflow_providers_jenkins-3.6.0rc1/airflow/providers/jenkins/operators/__init__.py
--rw-r--r--   0        0        0    10811 2024-01-22 08:29:09.000000 apache_airflow_providers_jenkins-3.6.0rc1/airflow/providers/jenkins/operators/jenkins_job_trigger.py
--rw-r--r--   0        0        0      787 2024-01-22 08:29:09.000000 apache_airflow_providers_jenkins-3.6.0rc1/airflow/providers/jenkins/sensors/__init__.py
--rw-r--r--   0        0        0     3044 2024-01-22 08:29:09.000000 apache_airflow_providers_jenkins-3.6.0rc1/airflow/providers/jenkins/sensors/jenkins.py
--rw-r--r--   0        0        0     2933 2024-01-22 08:29:09.000000 apache_airflow_providers_jenkins-3.6.0rc1/pyproject.toml
--rw-r--r--   0        0        0     4703 1970-01-01 00:00:00.000000 apache_airflow_providers_jenkins-3.6.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     3055 2024-04-30 11:31:53.000000 apache_airflow_providers_jenkins-3.6.0rc2/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-30 11:31:53.000000 apache_airflow_providers_jenkins-3.6.0rc2/airflow/providers/jenkins/LICENSE
+-rw-r--r--   0        0        0     1582 2024-04-30 11:31:53.000000 apache_airflow_providers_jenkins-3.6.0rc2/airflow/providers/jenkins/__init__.py
+-rw-r--r--   0        0        0     2866 2024-04-30 11:31:53.000000 apache_airflow_providers_jenkins-3.6.0rc2/airflow/providers/jenkins/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:31:53.000000 apache_airflow_providers_jenkins-3.6.0rc2/airflow/providers/jenkins/hooks/__init__.py
+-rw-r--r--   0        0        0     3914 2024-04-30 11:31:53.000000 apache_airflow_providers_jenkins-3.6.0rc2/airflow/providers/jenkins/hooks/jenkins.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:31:53.000000 apache_airflow_providers_jenkins-3.6.0rc2/airflow/providers/jenkins/operators/__init__.py
+-rw-r--r--   0        0        0    10811 2024-04-30 11:31:53.000000 apache_airflow_providers_jenkins-3.6.0rc2/airflow/providers/jenkins/operators/jenkins_job_trigger.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:31:53.000000 apache_airflow_providers_jenkins-3.6.0rc2/airflow/providers/jenkins/sensors/__init__.py
+-rw-r--r--   0        0        0     3044 2024-04-30 11:31:53.000000 apache_airflow_providers_jenkins-3.6.0rc2/airflow/providers/jenkins/sensors/jenkins.py
+-rw-r--r--   0        0        0     2977 2024-04-30 11:31:53.000000 apache_airflow_providers_jenkins-3.6.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     4757 1970-01-01 00:00:00.000000 apache_airflow_providers_jenkins-3.6.0rc2/PKG-INFO
```

### Comparing `apache_airflow_providers_jenkins-3.6.0rc1/README.rst` & `apache_airflow_providers_jenkins-3.6.0rc2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-jenkins``
 
-Release: ``3.6.0.rc1``
+Release: ``3.6.0.rc2``
 
 
 `Jenkins <https://jenkins.io/>`__
 
 
 Provider package
 ----------------
@@ -60,21 +60,21 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-jenkins``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.6.0``
+``apache-airflow``  ``>=2.7.0``
 ``python-jenkins``  ``>=1.0.0``
 ==================  ==================
 
 The changelog for the provider package can be found in the
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-jenkins/3.6.0/changelog.html>`_.
```

### Comparing `apache_airflow_providers_jenkins-3.6.0rc1/airflow/providers/jenkins/LICENSE` & `apache_airflow_providers_jenkins-3.6.0rc2/airflow/providers/jenkins/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_jenkins-3.6.0rc1/airflow/providers/jenkins/__init__.py` & `apache_airflow_providers_jenkins-3.6.0rc2/airflow/providers/jenkins/__init__.py`

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
-        f"The package `apache-airflow-providers-jenkins:{__version__}` needs Apache Airflow 2.6.0+"
+        f"The package `apache-airflow-providers-jenkins:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_jenkins-3.6.0rc1/airflow/providers/jenkins/get_provider_info.py` & `apache_airflow_providers_jenkins-3.6.0rc2/airflow/providers/jenkins/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-jenkins",
         "name": "Jenkins",
         "description": "`Jenkins <https://jenkins.io/>`__\n",
         "state": "ready",
-        "source-date-epoch": 1705912149,
+        "source-date-epoch": 1714476713,
         "versions": [
             "3.6.0",
             "3.5.1",
             "3.5.0",
             "3.4.0",
             "3.3.2",
             "3.3.1",
@@ -50,15 +50,15 @@
             "2.0.2",
             "2.0.1",
             "2.0.0",
             "1.1.0",
             "1.0.1",
             "1.0.0",
         ],
-        "dependencies": ["apache-airflow>=2.6.0", "python-jenkins>=1.0.0"],
+        "dependencies": ["apache-airflow>=2.7.0", "python-jenkins>=1.0.0"],
         "integrations": [
             {
                 "integration-name": "Jenkins",
                 "external-doc-url": "https://jenkins.io/",
                 "logo": "/integration-logos/jenkins/Jenkins.png",
                 "tags": ["software"],
             }
```

### Comparing `apache_airflow_providers_jenkins-3.6.0rc1/airflow/providers/jenkins/hooks/__init__.py` & `apache_airflow_providers_jenkins-3.6.0rc2/airflow/providers/jenkins/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_jenkins-3.6.0rc1/airflow/providers/jenkins/hooks/jenkins.py` & `apache_airflow_providers_jenkins-3.6.0rc2/airflow/providers/jenkins/hooks/jenkins.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,41 +30,41 @@
     conn_name_attr = "conn_id"
     default_conn_name = "jenkins_default"
     conn_type = "jenkins"
     hook_name = "Jenkins"
 
     @classmethod
     def get_connection_form_widgets(cls) -> dict[str, Any]:
-        """Returns connection widgets to add to connection form."""
+        """Return connection widgets to add to Jenkins connection form."""
         from flask_babel import lazy_gettext
         from wtforms import BooleanField
 
         return {
             "use_https": BooleanField(
                 label=lazy_gettext("Use Https"),
                 description="Specifies whether to use https scheme. Defaults to http",
             ),
         }
 
     @classmethod
     def get_ui_field_behaviour(cls) -> dict[str, Any]:
-        """Returns custom field behaviour."""
+        """Return custom UI field behaviour for Jenkins connection."""
         return {
             "hidden_fields": ["schema", "extra"],
             "relabeling": {},
             "placeholders": {
                 "login": "Login for the Jenkins service you would like to connect to",
                 "password": "Password for the Jenkins service you would like to connect too",
                 "host": "Host for your Jenkins server. Should NOT contain scheme (http:// or https://)",
                 "port": "Specify a port number",
             },
         }
 
-    def __init__(self, conn_id: str = default_conn_name, **kwargs) -> None:
-        super().__init__(**kwargs)
+    def __init__(self, conn_id: str = default_conn_name) -> None:
+        super().__init__()
         connection = self.get_connection(conn_id)
         self.connection = connection
         connection_prefix = "http"
         # connection.extra contains info about using https (true) or http (false)
         if connection.extra_dejson.get("use_https"):
             connection_prefix = "https"
         url = f"{connection_prefix}://{connection.host}:{connection.port}/{connection.schema}"
```

### Comparing `apache_airflow_providers_jenkins-3.6.0rc1/airflow/providers/jenkins/operators/__init__.py` & `apache_airflow_providers_jenkins-3.6.0rc2/airflow/providers/jenkins/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_jenkins-3.6.0rc1/airflow/providers/jenkins/operators/jenkins_job_trigger.py` & `apache_airflow_providers_jenkins-3.6.0rc2/airflow/providers/jenkins/operators/jenkins_job_trigger.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_jenkins-3.6.0rc1/airflow/providers/jenkins/sensors/__init__.py` & `apache_airflow_providers_jenkins-3.6.0rc2/airflow/providers/jenkins/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_jenkins-3.6.0rc1/airflow/providers/jenkins/sensors/jenkins.py` & `apache_airflow_providers_jenkins-3.6.0rc2/airflow/providers/jenkins/sensors/jenkins.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_jenkins-3.6.0rc1/pyproject.toml` & `apache_airflow_providers_jenkins-3.6.0rc2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-jenkins"
-version = "3.6.0.rc1"
+version = "3.6.0.rc2"
 description = "Provider package apache-airflow-providers-jenkins for Apache Airflow"
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
     "python-jenkins>=1.0.0",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-jenkins/3.6.0"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-jenkins/3.6.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
```

### Comparing `apache_airflow_providers_jenkins-3.6.0rc1/PKG-INFO` & `apache_airflow_providers_jenkins-3.6.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-jenkins
-Version: 3.6.0rc1
+Version: 3.6.0rc2
 Summary: Provider package apache-airflow-providers-jenkins for Apache Airflow
 Keywords: airflow-provider,jenkins,airflow,integration
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
 Requires-Dist: python-jenkins>=1.0.0
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-jenkins/3.6.0/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-jenkins/3.6.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
@@ -70,15 +71,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-jenkins``
 
-Release: ``3.6.0.rc1``
+Release: ``3.6.0.rc2``
 
 
 `Jenkins <https://jenkins.io/>`__
 
 
 Provider package
 ----------------
@@ -92,21 +93,21 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-jenkins``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.6.0``
+``apache-airflow``  ``>=2.7.0``
 ``python-jenkins``  ``>=1.0.0``
 ==================  ==================
 
 The changelog for the provider package can be found in the
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-jenkins/3.6.0/changelog.html>`_.
```

