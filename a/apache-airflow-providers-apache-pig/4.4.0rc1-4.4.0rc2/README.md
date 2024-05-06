# Comparing `tmp/apache_airflow_providers_apache_pig-4.4.0rc1.tar.gz` & `tmp/apache_airflow_providers_apache_pig-4.4.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_apache_pig-4.4.0rc1.tar", last modified: Mon Jan 22 08:25:34 2024, max compression
+gzip compressed data, was "apache_airflow_providers_apache_pig-4.4.0rc2.tar", last modified: Tue Apr 30 11:16:34 2024, max compression
```

## Comparing `apache_airflow_providers_apache_pig-4.4.0rc1.tar` & `apache_airflow_providers_apache_pig-4.4.0rc2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3043 2024-01-22 08:25:34.000000 apache_airflow_providers_apache_pig-4.4.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-01-22 08:25:34.000000 apache_airflow_providers_apache_pig-4.4.0rc1/airflow/providers/apache/pig/LICENSE
--rw-r--r--   0        0        0     1585 2024-01-22 08:25:34.000000 apache_airflow_providers_apache_pig-4.4.0rc1/airflow/providers/apache/pig/__init__.py
--rw-r--r--   0        0        0     2628 2024-01-22 08:25:34.000000 apache_airflow_providers_apache_pig-4.4.0rc1/airflow/providers/apache/pig/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-01-22 08:25:34.000000 apache_airflow_providers_apache_pig-4.4.0rc1/airflow/providers/apache/pig/hooks/__init__.py
--rw-r--r--   0        0        0     4151 2024-01-22 08:25:34.000000 apache_airflow_providers_apache_pig-4.4.0rc1/airflow/providers/apache/pig/hooks/pig.py
--rw-r--r--   0        0        0      787 2024-01-22 08:25:34.000000 apache_airflow_providers_apache_pig-4.4.0rc1/airflow/providers/apache/pig/operators/__init__.py
--rw-r--r--   0        0        0     2977 2024-01-22 08:25:34.000000 apache_airflow_providers_apache_pig-4.4.0rc1/airflow/providers/apache/pig/operators/pig.py
--rw-r--r--   0        0        0     2925 2024-01-22 08:25:34.000000 apache_airflow_providers_apache_pig-4.4.0rc1/pyproject.toml
--rw-r--r--   0        0        0     4674 1970-01-01 00:00:00.000000 apache_airflow_providers_apache_pig-4.4.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     3048 2024-04-30 11:16:34.000000 apache_airflow_providers_apache_pig-4.4.0rc2/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-30 11:16:34.000000 apache_airflow_providers_apache_pig-4.4.0rc2/airflow/providers/apache/pig/LICENSE
+-rw-r--r--   0        0        0     1585 2024-04-30 11:16:34.000000 apache_airflow_providers_apache_pig-4.4.0rc2/airflow/providers/apache/pig/__init__.py
+-rw-r--r--   0        0        0     2628 2024-04-30 11:16:34.000000 apache_airflow_providers_apache_pig-4.4.0rc2/airflow/providers/apache/pig/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:16:34.000000 apache_airflow_providers_apache_pig-4.4.0rc2/airflow/providers/apache/pig/hooks/__init__.py
+-rw-r--r--   0        0        0     4108 2024-04-30 11:16:34.000000 apache_airflow_providers_apache_pig-4.4.0rc2/airflow/providers/apache/pig/hooks/pig.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:16:34.000000 apache_airflow_providers_apache_pig-4.4.0rc2/airflow/providers/apache/pig/operators/__init__.py
+-rw-r--r--   0        0        0     2977 2024-04-30 11:16:34.000000 apache_airflow_providers_apache_pig-4.4.0rc2/airflow/providers/apache/pig/operators/pig.py
+-rw-r--r--   0        0        0     2969 2024-04-30 11:16:34.000000 apache_airflow_providers_apache_pig-4.4.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     4728 1970-01-01 00:00:00.000000 apache_airflow_providers_apache_pig-4.4.0rc2/PKG-INFO
```

### Comparing `apache_airflow_providers_apache_pig-4.4.0rc1/README.rst` & `apache_airflow_providers_apache_pig-4.4.0rc2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-apache-pig``
 
-Release: ``4.4.0.rc1``
+Release: ``4.4.0.rc2``
 
 
 `Apache Pig <https://pig.apache.org/>`__
 
 
 Provider package
 ----------------
@@ -60,20 +60,20 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apache-pig``
 
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
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-apache-pig/4.4.0/changelog.html>`_.
```

### Comparing `apache_airflow_providers_apache_pig-4.4.0rc1/airflow/providers/apache/pig/LICENSE` & `apache_airflow_providers_apache_pig-4.4.0rc2/airflow/providers/apache/pig/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_pig-4.4.0rc1/airflow/providers/apache/pig/__init__.py` & `apache_airflow_providers_apache_pig-4.4.0rc2/airflow/providers/apache/pig/__init__.py`

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
-        f"The package `apache-airflow-providers-apache-pig:{__version__}` needs Apache Airflow 2.6.0+"
+        f"The package `apache-airflow-providers-apache-pig:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_apache_pig-4.4.0rc1/airflow/providers/apache/pig/get_provider_info.py` & `apache_airflow_providers_apache_pig-4.4.0rc2/airflow/providers/apache/pig/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-apache-pig",
         "name": "Apache Pig",
         "description": "`Apache Pig <https://pig.apache.org/>`__\n",
         "state": "ready",
-        "source-date-epoch": 1705911934,
+        "source-date-epoch": 1714475794,
         "versions": [
             "4.4.0",
             "4.3.0",
             "4.2.0",
             "4.1.2",
             "4.1.1",
             "4.1.0",
@@ -42,15 +42,15 @@
             "2.0.3",
             "2.0.2",
             "2.0.1",
             "2.0.0",
             "1.0.1",
             "1.0.0",
         ],
-        "dependencies": ["apache-airflow>=2.6.0"],
+        "dependencies": ["apache-airflow>=2.7.0"],
         "integrations": [
             {
                 "integration-name": "Apache Pig",
                 "external-doc-url": "https://pig.apache.org/",
                 "how-to-guide": ["/docs/apache-airflow-providers-apache-pig/operators.rst"],
                 "logo": "/integration-logos/apache/pig.png",
                 "tags": ["apache"],
```

### Comparing `apache_airflow_providers_apache_pig-4.4.0rc1/airflow/providers/apache/pig/hooks/__init__.py` & `apache_airflow_providers_apache_pig-4.4.0rc2/airflow/providers/apache/pig/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_pig-4.4.0rc1/airflow/providers/apache/pig/hooks/pig.py` & `apache_airflow_providers_apache_pig-4.4.0rc2/airflow/providers/apache/pig/hooks/pig.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,20 +34,17 @@
 
     conn_name_attr = "pig_cli_conn_id"
     default_conn_name = "pig_cli_default"
     conn_type = "pig_cli"
     hook_name = "Pig Client Wrapper"
 
     def __init__(
-        self,
-        pig_cli_conn_id: str = default_conn_name,
-        pig_properties: list[str] | None = None,
-        **kwargs,
+        self, pig_cli_conn_id: str = default_conn_name, pig_properties: list[str] | None = None
     ) -> None:
-        super().__init__(**kwargs)
+        super().__init__()
         conn = self.get_connection(pig_cli_conn_id)
         conn_pig_properties = conn.extra_dejson.get("pig_properties")
         if conn_pig_properties:
             raise RuntimeError(
                 "The PigCliHook used to have possibility of passing `pig_properties` to the Hook,"
                 " however with the 4.0.0 version of `apache-pig` provider it has been removed. You should"
                 " use ``pig_opts`` (space separated string) or ``pig_properties`` (string list) in the"
```

### Comparing `apache_airflow_providers_apache_pig-4.4.0rc1/airflow/providers/apache/pig/operators/__init__.py` & `apache_airflow_providers_apache_pig-4.4.0rc2/airflow/providers/apache/pig/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_pig-4.4.0rc1/airflow/providers/apache/pig/operators/pig.py` & `apache_airflow_providers_apache_pig-4.4.0rc2/airflow/providers/apache/pig/operators/pig.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_pig-4.4.0rc1/pyproject.toml` & `apache_airflow_providers_apache_pig-4.4.0rc2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-apache-pig"
-version = "4.4.0.rc1"
+version = "4.4.0.rc2"
 description = "Provider package apache-airflow-providers-apache-pig for Apache Airflow"
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
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-apache-pig/4.4.0"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-apache-pig/4.4.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
```

### Comparing `apache_airflow_providers_apache_pig-4.4.0rc1/PKG-INFO` & `apache_airflow_providers_apache_pig-4.4.0rc2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-pig
-Version: 4.4.0rc1
+Version: 4.4.0rc2
 Summary: Provider package apache-airflow-providers-apache-pig for Apache Airflow
 Keywords: airflow-provider,apache.pig,airflow,integration
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
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-apache-pig/4.4.0/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-pig/4.4.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
@@ -69,15 +70,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-apache-pig``
 
-Release: ``4.4.0.rc1``
+Release: ``4.4.0.rc2``
 
 
 `Apache Pig <https://pig.apache.org/>`__
 
 
 Provider package
 ----------------
@@ -91,20 +92,20 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apache-pig``
 
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
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-apache-pig/4.4.0/changelog.html>`_.
```

