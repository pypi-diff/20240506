# Comparing `tmp/apache_airflow_providers_telegram-4.5.0.tar.gz` & `tmp/apache_airflow_providers_telegram-4.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_telegram-4.5.0.tar", last modified: Tue Apr 30 11:48:07 2024, max compression
+gzip compressed data, was "apache_airflow_providers_telegram-4.5.0rc1.tar", last modified: Tue Apr 30 11:48:07 2024, max compression
```

## Comparing `apache_airflow_providers_telegram-4.5.0.tar` & `apache_airflow_providers_telegram-4.5.0rc1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3089 2024-04-30 11:48:07.000000 apache_airflow_providers_telegram-4.5.0/README.rst
--rw-r--r--   0        0        0    13569 2024-04-30 11:48:07.000000 apache_airflow_providers_telegram-4.5.0/airflow/providers/telegram/LICENSE
--rw-r--r--   0        0        0     1583 2024-04-30 11:48:07.000000 apache_airflow_providers_telegram-4.5.0/airflow/providers/telegram/__init__.py
--rw-r--r--   0        0        0     2743 2024-04-30 11:48:07.000000 apache_airflow_providers_telegram-4.5.0/airflow/providers/telegram/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-04-30 11:48:07.000000 apache_airflow_providers_telegram-4.5.0/airflow/providers/telegram/hooks/__init__.py
--rw-r--r--   0        0        0     5746 2024-04-30 11:48:07.000000 apache_airflow_providers_telegram-4.5.0/airflow/providers/telegram/hooks/telegram.py
--rw-r--r--   0        0        0      787 2024-04-30 11:48:07.000000 apache_airflow_providers_telegram-4.5.0/airflow/providers/telegram/operators/__init__.py
--rw-r--r--   0        0        0     3014 2024-04-30 11:48:07.000000 apache_airflow_providers_telegram-4.5.0/airflow/providers/telegram/operators/telegram.py
--rw-r--r--   0        0        0     2981 2024-04-30 11:48:07.000000 apache_airflow_providers_telegram-4.5.0/pyproject.toml
--rw-r--r--   0        0        0     4794 1970-01-01 00:00:00.000000 apache_airflow_providers_telegram-4.5.0/PKG-INFO
+-rw-r--r--   0        0        0     3093 2024-04-30 11:48:07.000000 apache_airflow_providers_telegram-4.5.0rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-30 11:48:07.000000 apache_airflow_providers_telegram-4.5.0rc1/airflow/providers/telegram/LICENSE
+-rw-r--r--   0        0        0     1583 2024-04-30 11:48:07.000000 apache_airflow_providers_telegram-4.5.0rc1/airflow/providers/telegram/__init__.py
+-rw-r--r--   0        0        0     2743 2024-04-30 11:48:07.000000 apache_airflow_providers_telegram-4.5.0rc1/airflow/providers/telegram/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:48:07.000000 apache_airflow_providers_telegram-4.5.0rc1/airflow/providers/telegram/hooks/__init__.py
+-rw-r--r--   0        0        0     5746 2024-04-30 11:48:07.000000 apache_airflow_providers_telegram-4.5.0rc1/airflow/providers/telegram/hooks/telegram.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:48:07.000000 apache_airflow_providers_telegram-4.5.0rc1/airflow/providers/telegram/operators/__init__.py
+-rw-r--r--   0        0        0     3014 2024-04-30 11:48:07.000000 apache_airflow_providers_telegram-4.5.0rc1/airflow/providers/telegram/operators/telegram.py
+-rw-r--r--   0        0        0     2988 2024-04-30 11:48:07.000000 apache_airflow_providers_telegram-4.5.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     4804 1970-01-01 00:00:00.000000 apache_airflow_providers_telegram-4.5.0rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_telegram-4.5.0/README.rst` & `apache_airflow_providers_telegram-4.5.0rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-telegram``
 
-Release: ``4.5.0``
+Release: ``4.5.0.rc1``
 
 
 `Telegram <https://telegram.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache_airflow_providers_telegram-4.5.0/airflow/providers/telegram/LICENSE` & `apache_airflow_providers_telegram-4.5.0rc1/airflow/providers/telegram/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_telegram-4.5.0/airflow/providers/telegram/__init__.py` & `apache_airflow_providers_telegram-4.5.0rc1/airflow/providers/telegram/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_telegram-4.5.0/airflow/providers/telegram/get_provider_info.py` & `apache_airflow_providers_telegram-4.5.0rc1/airflow/providers/telegram/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_telegram-4.5.0/airflow/providers/telegram/hooks/__init__.py` & `apache_airflow_providers_telegram-4.5.0rc1/airflow/providers/telegram/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_telegram-4.5.0/airflow/providers/telegram/hooks/telegram.py` & `apache_airflow_providers_telegram-4.5.0rc1/airflow/providers/telegram/hooks/telegram.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_telegram-4.5.0/airflow/providers/telegram/operators/__init__.py` & `apache_airflow_providers_telegram-4.5.0rc1/airflow/providers/telegram/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_telegram-4.5.0/airflow/providers/telegram/operators/telegram.py` & `apache_airflow_providers_telegram-4.5.0rc1/airflow/providers/telegram/operators/telegram.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_telegram-4.5.0/pyproject.toml` & `apache_airflow_providers_telegram-4.5.0rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-telegram"
-version = "4.5.0"
+version = "4.5.0.rc1"
 description = "Provider package apache-airflow-providers-telegram for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -52,15 +52,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: System :: Monitoring",
 ]
 requires-python = "~=3.8"
 dependencies = [
-    "apache-airflow>=2.7.0",
+    "apache-airflow>=2.7.0rc0",
     "python-telegram-bot>=20.2",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-telegram/4.5.0"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-telegram/4.5.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
```

### Comparing `apache_airflow_providers_telegram-4.5.0/PKG-INFO` & `apache_airflow_providers_telegram-4.5.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-telegram
-Version: 4.5.0
+Version: 4.5.0rc1
 Summary: Provider package apache-airflow-providers-telegram for Apache Airflow
 Keywords: airflow-provider,telegram,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,15 +17,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Monitoring
-Requires-Dist: apache-airflow>=2.7.0
+Requires-Dist: apache-airflow>=2.7.0rc0
 Requires-Dist: python-telegram-bot>=20.2
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-telegram/4.5.0/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-telegram/4.5.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
@@ -71,15 +71,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-telegram``
 
-Release: ``4.5.0``
+Release: ``4.5.0.rc1``
 
 
 `Telegram <https://telegram.org/>`__
 
 
 Provider package
 ----------------
```

