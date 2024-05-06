# Comparing `tmp/apache_airflow_providers_apache_kafka-1.4.0rc1.tar.gz` & `tmp/apache_airflow_providers_apache_kafka-1.4.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_apache_kafka-1.4.0rc1.tar", last modified: Mon Jan 22 08:25:26 2024, max compression
+gzip compressed data, was "apache_airflow_providers_apache_kafka-1.4.0rc2.tar", last modified: Tue Apr 30 11:15:04 2024, max compression
```

## Comparing `apache_airflow_providers_apache_kafka-1.4.0rc1.tar` & `apache_airflow_providers_apache_kafka-1.4.0rc2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     3110 2024-01-22 08:25:26.000000 apache_airflow_providers_apache_kafka-1.4.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-01-22 08:25:26.000000 apache_airflow_providers_apache_kafka-1.4.0rc1/airflow/providers/apache/kafka/LICENSE
--rw-r--r--   0        0        0     1587 2024-01-22 08:25:26.000000 apache_airflow_providers_apache_kafka-1.4.0rc1/airflow/providers/apache/kafka/__init__.py
--rw-r--r--   0        0        0     3152 2024-01-22 08:25:26.000000 apache_airflow_providers_apache_kafka-1.4.0rc1/airflow/providers/apache/kafka/get_provider_info.py
--rw-r--r--   0        0        0      785 2024-01-22 08:25:26.000000 apache_airflow_providers_apache_kafka-1.4.0rc1/airflow/providers/apache/kafka/hooks/__init__.py
--rw-r--r--   0        0        0     2745 2024-01-22 08:25:26.000000 apache_airflow_providers_apache_kafka-1.4.0rc1/airflow/providers/apache/kafka/hooks/base.py
--rw-r--r--   0        0        0     2352 2024-01-22 08:25:26.000000 apache_airflow_providers_apache_kafka-1.4.0rc1/airflow/providers/apache/kafka/hooks/client.py
--rw-r--r--   0        0        0     1675 2024-01-22 08:25:26.000000 apache_airflow_providers_apache_kafka-1.4.0rc1/airflow/providers/apache/kafka/hooks/consume.py
--rw-r--r--   0        0        0     1550 2024-01-22 08:25:26.000000 apache_airflow_providers_apache_kafka-1.4.0rc1/airflow/providers/apache/kafka/hooks/produce.py
--rw-r--r--   0        0        0      785 2024-01-22 08:25:26.000000 apache_airflow_providers_apache_kafka-1.4.0rc1/airflow/providers/apache/kafka/operators/__init__.py
--rw-r--r--   0        0        0     8091 2024-01-22 08:25:26.000000 apache_airflow_providers_apache_kafka-1.4.0rc1/airflow/providers/apache/kafka/operators/consume.py
--rw-r--r--   0        0        0     4949 2024-01-22 08:25:26.000000 apache_airflow_providers_apache_kafka-1.4.0rc1/airflow/providers/apache/kafka/operators/produce.py
--rw-r--r--   0        0        0      785 2024-01-22 08:25:26.000000 apache_airflow_providers_apache_kafka-1.4.0rc1/airflow/providers/apache/kafka/sensors/__init__.py
--rw-r--r--   0        0        0     8214 2024-01-22 08:25:26.000000 apache_airflow_providers_apache_kafka-1.4.0rc1/airflow/providers/apache/kafka/sensors/kafka.py
--rw-r--r--   0        0        0      785 2024-01-22 08:25:26.000000 apache_airflow_providers_apache_kafka-1.4.0rc1/airflow/providers/apache/kafka/triggers/__init__.py
--rw-r--r--   0        0        0     4978 2024-01-22 08:25:26.000000 apache_airflow_providers_apache_kafka-1.4.0rc1/airflow/providers/apache/kafka/triggers/await_message.py
--rw-r--r--   0        0        0     2984 2024-01-22 08:25:26.000000 apache_airflow_providers_apache_kafka-1.4.0rc1/pyproject.toml
--rw-r--r--   0        0        0     4812 1970-01-01 00:00:00.000000 apache_airflow_providers_apache_kafka-1.4.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     3115 2024-04-30 11:15:04.000000 apache_airflow_providers_apache_kafka-1.4.0rc2/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-30 11:15:04.000000 apache_airflow_providers_apache_kafka-1.4.0rc2/airflow/providers/apache/kafka/LICENSE
+-rw-r--r--   0        0        0     1587 2024-04-30 11:15:04.000000 apache_airflow_providers_apache_kafka-1.4.0rc2/airflow/providers/apache/kafka/__init__.py
+-rw-r--r--   0        0        0     3152 2024-04-30 11:15:04.000000 apache_airflow_providers_apache_kafka-1.4.0rc2/airflow/providers/apache/kafka/get_provider_info.py
+-rw-r--r--   0        0        0      785 2024-04-30 11:15:04.000000 apache_airflow_providers_apache_kafka-1.4.0rc2/airflow/providers/apache/kafka/hooks/__init__.py
+-rw-r--r--   0        0        0     2737 2024-04-30 11:15:04.000000 apache_airflow_providers_apache_kafka-1.4.0rc2/airflow/providers/apache/kafka/hooks/base.py
+-rw-r--r--   0        0        0     2352 2024-04-30 11:15:04.000000 apache_airflow_providers_apache_kafka-1.4.0rc2/airflow/providers/apache/kafka/hooks/client.py
+-rw-r--r--   0        0        0     1675 2024-04-30 11:15:04.000000 apache_airflow_providers_apache_kafka-1.4.0rc2/airflow/providers/apache/kafka/hooks/consume.py
+-rw-r--r--   0        0        0     1550 2024-04-30 11:15:04.000000 apache_airflow_providers_apache_kafka-1.4.0rc2/airflow/providers/apache/kafka/hooks/produce.py
+-rw-r--r--   0        0        0      785 2024-04-30 11:15:04.000000 apache_airflow_providers_apache_kafka-1.4.0rc2/airflow/providers/apache/kafka/operators/__init__.py
+-rw-r--r--   0        0        0     8091 2024-04-30 11:15:04.000000 apache_airflow_providers_apache_kafka-1.4.0rc2/airflow/providers/apache/kafka/operators/consume.py
+-rw-r--r--   0        0        0     4993 2024-04-30 11:15:04.000000 apache_airflow_providers_apache_kafka-1.4.0rc2/airflow/providers/apache/kafka/operators/produce.py
+-rw-r--r--   0        0        0      785 2024-04-30 11:15:04.000000 apache_airflow_providers_apache_kafka-1.4.0rc2/airflow/providers/apache/kafka/sensors/__init__.py
+-rw-r--r--   0        0        0     8214 2024-04-30 11:15:04.000000 apache_airflow_providers_apache_kafka-1.4.0rc2/airflow/providers/apache/kafka/sensors/kafka.py
+-rw-r--r--   0        0        0      785 2024-04-30 11:15:04.000000 apache_airflow_providers_apache_kafka-1.4.0rc2/airflow/providers/apache/kafka/triggers/__init__.py
+-rw-r--r--   0        0        0     4978 2024-04-30 11:15:04.000000 apache_airflow_providers_apache_kafka-1.4.0rc2/airflow/providers/apache/kafka/triggers/await_message.py
+-rw-r--r--   0        0        0     3028 2024-04-30 11:15:04.000000 apache_airflow_providers_apache_kafka-1.4.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     4866 1970-01-01 00:00:00.000000 apache_airflow_providers_apache_kafka-1.4.0rc2/PKG-INFO
```

### Comparing `apache_airflow_providers_apache_kafka-1.4.0rc1/README.rst` & `apache_airflow_providers_apache_kafka-1.4.0rc2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-apache-kafka``
 
-Release: ``1.4.0.rc1``
+Release: ``1.4.0.rc2``
 
 
 `Apache Kafka  <https://kafka.apache.org/>`__
 
 
 Provider package
 ----------------
@@ -60,22 +60,22 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apache-kafka``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ===================  ==================
 PIP package          Version required
 ===================  ==================
-``apache-airflow``   ``>=2.6.0``
+``apache-airflow``   ``>=2.7.0``
 ``asgiref``
 ``confluent-kafka``  ``>=1.8.2``
 ===================  ==================
 
 The changelog for the provider package can be found in the
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-apache-kafka/1.4.0/changelog.html>`_.
```

### Comparing `apache_airflow_providers_apache_kafka-1.4.0rc1/airflow/providers/apache/kafka/LICENSE` & `apache_airflow_providers_apache_kafka-1.4.0rc2/airflow/providers/apache/kafka/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_kafka-1.4.0rc1/airflow/providers/apache/kafka/__init__.py` & `apache_airflow_providers_apache_kafka-1.4.0rc2/airflow/providers/apache/kafka/__init__.py`

 * *Files 8% similar despite different names*

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
-        f"The package `apache-airflow-providers-apache-kafka:{__version__}` needs Apache Airflow 2.6.0+"
+        f"The package `apache-airflow-providers-apache-kafka:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_apache_kafka-1.4.0rc1/airflow/providers/apache/kafka/get_provider_info.py` & `apache_airflow_providers_apache_kafka-1.4.0rc2/airflow/providers/apache/kafka/get_provider_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,18 +23,18 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-apache-kafka",
         "name": "Apache Kafka",
         "state": "ready",
-        "source-date-epoch": 1705911926,
+        "source-date-epoch": 1714475704,
         "description": "`Apache Kafka  <https://kafka.apache.org/>`__\n",
         "versions": ["1.4.0", "1.3.1", "1.3.0", "1.2.0", "1.1.2", "1.1.1", "1.1.0", "1.0.0"],
-        "dependencies": ["apache-airflow>=2.6.0", "asgiref", "confluent-kafka>=1.8.2"],
+        "dependencies": ["apache-airflow>=2.7.0", "asgiref", "confluent-kafka>=1.8.2"],
         "integrations": [
             {
                 "integration-name": "Apache Kafka",
                 "external-doc-url": "https://kafka.apache.org/",
                 "logo": "/integration-logos/apache/kafka.svg",
                 "tags": ["apache"],
             }
```

### Comparing `apache_airflow_providers_apache_kafka-1.4.0rc1/airflow/providers/apache/kafka/hooks/__init__.py` & `apache_airflow_providers_apache_kafka-1.4.0rc2/airflow/providers/apache/kafka/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_kafka-1.4.0rc1/airflow/providers/apache/kafka/hooks/base.py` & `apache_airflow_providers_apache_kafka-1.4.0rc2/airflow/providers/apache/kafka/hooks/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     conn_name_attr = "kafka_config_id"
     default_conn_name = "kafka_default"
     conn_type = "kafka"
     hook_name = "Apache Kafka"
 
     def __init__(self, kafka_config_id=default_conn_name, *args, **kwargs):
         """Initialize our Base."""
-        super().__init__(**kwargs)
+        super().__init__()
         self.kafka_config_id = kafka_config_id
         self.get_conn
 
     @classmethod
     def get_ui_field_behaviour(cls) -> dict[str, Any]:
         """Return custom field behaviour."""
         return {
```

### Comparing `apache_airflow_providers_apache_kafka-1.4.0rc1/airflow/providers/apache/kafka/hooks/client.py` & `apache_airflow_providers_apache_kafka-1.4.0rc2/airflow/providers/apache/kafka/hooks/client.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_kafka-1.4.0rc1/airflow/providers/apache/kafka/hooks/consume.py` & `apache_airflow_providers_apache_kafka-1.4.0rc2/airflow/providers/apache/kafka/hooks/consume.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_kafka-1.4.0rc1/airflow/providers/apache/kafka/hooks/produce.py` & `apache_airflow_providers_apache_kafka-1.4.0rc2/airflow/providers/apache/kafka/hooks/produce.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_kafka-1.4.0rc1/airflow/providers/apache/kafka/operators/__init__.py` & `apache_airflow_providers_apache_kafka-1.4.0rc2/airflow/providers/apache/kafka/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_kafka-1.4.0rc1/airflow/providers/apache/kafka/operators/consume.py` & `apache_airflow_providers_apache_kafka-1.4.0rc2/airflow/providers/apache/kafka/operators/consume.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_kafka-1.4.0rc1/airflow/providers/apache/kafka/operators/produce.py` & `apache_airflow_providers_apache_kafka-1.4.0rc2/airflow/providers/apache/kafka/operators/produce.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,18 +26,21 @@
 from airflow.utils.module_loading import import_string
 
 local_logger = logging.getLogger("airflow")
 
 
 def acked(err, msg):
     if err is not None:
-        local_logger.error(f"Failed to deliver message: {err}")
+        local_logger.error("Failed to deliver message: %s", err)
     else:
         local_logger.info(
-            f"Produced record to topic {msg.topic()} partition [{msg.partition()}] @ offset {msg.offset()}"
+            "Produced record to topic %s, partition [%s] @ offset %s",
+            msg.topic(),
+            msg.partition(),
+            msg.offset(),
         )
 
 
 class ProduceToTopicOperator(BaseOperator):
     """An operator that produces messages to a Kafka topic.
 
     Registers a producer to a kafka topic and publishes messages to the log.
```

### Comparing `apache_airflow_providers_apache_kafka-1.4.0rc1/airflow/providers/apache/kafka/sensors/__init__.py` & `apache_airflow_providers_apache_kafka-1.4.0rc2/airflow/providers/apache/kafka/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_kafka-1.4.0rc1/airflow/providers/apache/kafka/sensors/kafka.py` & `apache_airflow_providers_apache_kafka-1.4.0rc2/airflow/providers/apache/kafka/sensors/kafka.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_kafka-1.4.0rc1/airflow/providers/apache/kafka/triggers/__init__.py` & `apache_airflow_providers_apache_kafka-1.4.0rc2/airflow/providers/apache/kafka/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_kafka-1.4.0rc1/airflow/providers/apache/kafka/triggers/await_message.py` & `apache_airflow_providers_apache_kafka-1.4.0rc2/airflow/providers/apache/kafka/triggers/await_message.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_kafka-1.4.0rc1/pyproject.toml` & `apache_airflow_providers_apache_kafka-1.4.0rc2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-apache-kafka"
-version = "1.4.0.rc1"
+version = "1.4.0.rc2"
 description = "Provider package apache-airflow-providers-apache-kafka for Apache Airflow"
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
     "asgiref",
     "confluent-kafka>=1.8.2",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-apache-kafka/1.4.0"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-apache-kafka/1.4.0/changelog.html"
```

### Comparing `apache_airflow_providers_apache_kafka-1.4.0rc1/PKG-INFO` & `apache_airflow_providers_apache_kafka-1.4.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-kafka
-Version: 1.4.0rc1
+Version: 1.4.0rc2
 Summary: Provider package apache-airflow-providers-apache-kafka for Apache Airflow
 Keywords: airflow-provider,apache.kafka,airflow,integration
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
 Requires-Dist: asgiref
 Requires-Dist: confluent-kafka>=1.8.2
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-apache-kafka/1.4.0/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-kafka/1.4.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
@@ -71,15 +72,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-apache-kafka``
 
-Release: ``1.4.0.rc1``
+Release: ``1.4.0.rc2``
 
 
 `Apache Kafka  <https://kafka.apache.org/>`__
 
 
 Provider package
 ----------------
@@ -93,22 +94,22 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apache-kafka``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ===================  ==================
 PIP package          Version required
 ===================  ==================
-``apache-airflow``   ``>=2.6.0``
+``apache-airflow``   ``>=2.7.0``
 ``asgiref``
 ``confluent-kafka``  ``>=1.8.2``
 ===================  ==================
 
 The changelog for the provider package can be found in the
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-apache-kafka/1.4.0/changelog.html>`_.
```

