# Comparing `tmp/apache_airflow_providers_segment-3.5.0rc1.tar.gz` & `tmp/apache_airflow_providers_segment-3.5.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_segment-3.5.0rc1.tar", last modified: Mon Jan 22 08:30:47 2024, max compression
+gzip compressed data, was "apache_airflow_providers_segment-3.5.0rc2.tar", last modified: Tue Apr 30 11:44:12 2024, max compression
```

## Comparing `apache_airflow_providers_segment-3.5.0rc1.tar` & `apache_airflow_providers_segment-3.5.0rc2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3063 2024-01-22 08:30:47.000000 apache_airflow_providers_segment-3.5.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-01-22 08:30:47.000000 apache_airflow_providers_segment-3.5.0rc1/airflow/providers/segment/LICENSE
--rw-r--r--   0        0        0     1582 2024-01-22 08:30:47.000000 apache_airflow_providers_segment-3.5.0rc1/airflow/providers/segment/__init__.py
--rw-r--r--   0        0        0     2544 2024-01-22 08:30:47.000000 apache_airflow_providers_segment-3.5.0rc1/airflow/providers/segment/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-01-22 08:30:47.000000 apache_airflow_providers_segment-3.5.0rc1/airflow/providers/segment/hooks/__init__.py
--rw-r--r--   0        0        0     3459 2024-01-22 08:30:47.000000 apache_airflow_providers_segment-3.5.0rc1/airflow/providers/segment/hooks/segment.py
--rw-r--r--   0        0        0      787 2024-01-22 08:30:47.000000 apache_airflow_providers_segment-3.5.0rc1/airflow/providers/segment/operators/__init__.py
--rw-r--r--   0        0        0     2646 2024-01-22 08:30:47.000000 apache_airflow_providers_segment-3.5.0rc1/airflow/providers/segment/operators/segment_track_event.py
--rw-r--r--   0        0        0     2935 2024-01-22 08:30:47.000000 apache_airflow_providers_segment-3.5.0rc1/pyproject.toml
--rw-r--r--   0        0        0     4718 1970-01-01 00:00:00.000000 apache_airflow_providers_segment-3.5.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     3068 2024-04-30 11:44:12.000000 apache_airflow_providers_segment-3.5.0rc2/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-30 11:44:12.000000 apache_airflow_providers_segment-3.5.0rc2/airflow/providers/segment/LICENSE
+-rw-r--r--   0        0        0     1582 2024-04-30 11:44:12.000000 apache_airflow_providers_segment-3.5.0rc2/airflow/providers/segment/__init__.py
+-rw-r--r--   0        0        0     2544 2024-04-30 11:44:12.000000 apache_airflow_providers_segment-3.5.0rc2/airflow/providers/segment/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:44:12.000000 apache_airflow_providers_segment-3.5.0rc2/airflow/providers/segment/hooks/__init__.py
+-rw-r--r--   0        0        0     3428 2024-04-30 11:44:12.000000 apache_airflow_providers_segment-3.5.0rc2/airflow/providers/segment/hooks/segment.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:44:12.000000 apache_airflow_providers_segment-3.5.0rc2/airflow/providers/segment/operators/__init__.py
+-rw-r--r--   0        0        0     2646 2024-04-30 11:44:12.000000 apache_airflow_providers_segment-3.5.0rc2/airflow/providers/segment/operators/segment_track_event.py
+-rw-r--r--   0        0        0     2979 2024-04-30 11:44:12.000000 apache_airflow_providers_segment-3.5.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     4772 1970-01-01 00:00:00.000000 apache_airflow_providers_segment-3.5.0rc2/PKG-INFO
```

### Comparing `apache_airflow_providers_segment-3.5.0rc1/README.rst` & `apache_airflow_providers_segment-3.5.0rc2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-segment``
 
-Release: ``3.5.0.rc1``
+Release: ``3.5.0.rc2``
 
 
 `Segment <https://segment.com/>`__
 
 
 Provider package
 ----------------
@@ -60,21 +60,21 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-segment``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ====================  ==================
 PIP package           Version required
 ====================  ==================
-``apache-airflow``    ``>=2.6.0``
+``apache-airflow``    ``>=2.7.0``
 ``analytics-python``  ``>=1.2.9``
 ====================  ==================
 
 The changelog for the provider package can be found in the
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-segment/3.5.0/changelog.html>`_.
```

### Comparing `apache_airflow_providers_segment-3.5.0rc1/airflow/providers/segment/LICENSE` & `apache_airflow_providers_segment-3.5.0rc2/airflow/providers/segment/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_segment-3.5.0rc1/airflow/providers/segment/__init__.py` & `apache_airflow_providers_segment-3.5.0rc2/airflow/providers/segment/__init__.py`

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
-        f"The package `apache-airflow-providers-segment:{__version__}` needs Apache Airflow 2.6.0+"
+        f"The package `apache-airflow-providers-segment:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_segment-3.5.0rc1/airflow/providers/segment/get_provider_info.py` & `apache_airflow_providers_segment-3.5.0rc2/airflow/providers/segment/get_provider_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-segment",
         "name": "Segment",
         "description": "`Segment <https://segment.com/>`__\n",
         "state": "ready",
-        "source-date-epoch": 1705912247,
+        "source-date-epoch": 1714477452,
         "versions": [
             "3.5.0",
             "3.4.0",
             "3.3.0",
             "3.2.1",
             "3.2.0",
             "3.1.0",
@@ -41,15 +41,15 @@
             "2.0.3",
             "2.0.2",
             "2.0.1",
             "2.0.0",
             "1.0.1",
             "1.0.0",
         ],
-        "dependencies": ["apache-airflow>=2.6.0", "analytics-python>=1.2.9"],
+        "dependencies": ["apache-airflow>=2.7.0", "analytics-python>=1.2.9"],
         "integrations": [
             {
                 "integration-name": "Segment",
                 "external-doc-url": "https://segment.com/docs/",
                 "logo": "/integration-logos/segment/Segment.png",
                 "tags": ["service"],
             }
```

### Comparing `apache_airflow_providers_segment-3.5.0rc1/airflow/providers/segment/hooks/__init__.py` & `apache_airflow_providers_segment-3.5.0rc2/airflow/providers/segment/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_segment-3.5.0rc1/airflow/providers/segment/hooks/segment.py` & `apache_airflow_providers_segment-3.5.0rc2/airflow/providers/segment/hooks/segment.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 # under the License.
 """
 Connect to your Segment account, retrieve data from it or write to that file.
 
 NOTE:   this hook also relies on the Segment analytics package:
         https://github.com/segmentio/analytics-python
 """
+
 from __future__ import annotations
 
 import analytics
 
 from airflow.exceptions import AirflowException
 from airflow.hooks.base import BaseHook
 
@@ -53,15 +54,15 @@
     default_conn_name = "segment_default"
     conn_type = "segment"
     hook_name = "Segment"
 
     def __init__(
         self, segment_conn_id: str = "segment_default", segment_debug_mode: bool = False, *args, **kwargs
     ) -> None:
-        super().__init__(kwargs.pop("logger_name", None))
+        super().__init__()
         self.segment_conn_id = segment_conn_id
         self.segment_debug_mode = segment_debug_mode
         self._args = args
         self._kwargs = kwargs
 
         # get the connection parameters
         self.connection = self.get_connection(self.segment_conn_id)
@@ -76,10 +77,10 @@
         if self.segment_debug_mode:
             self.log.info("Setting Segment analytics connection to debug mode")
         analytics.on_error = self.on_error
         analytics.write_key = self.write_key
         return analytics
 
     def on_error(self, error: str, items: str) -> None:
-        """Handles error callbacks when using Segment with segment_debug_mode set to True."""
+        """Handle error callbacks when using Segment with segment_debug_mode set to True."""
         self.log.error("Encountered Segment error: %s with items: %s", error, items)
         raise AirflowException(f"Segment error: {error}")
```

### Comparing `apache_airflow_providers_segment-3.5.0rc1/airflow/providers/segment/operators/__init__.py` & `apache_airflow_providers_segment-3.5.0rc2/airflow/providers/segment/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_segment-3.5.0rc1/airflow/providers/segment/operators/segment_track_event.py` & `apache_airflow_providers_segment-3.5.0rc2/airflow/providers/segment/operators/segment_track_event.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_segment-3.5.0rc1/pyproject.toml` & `apache_airflow_providers_segment-3.5.0rc2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-segment"
-version = "3.5.0.rc1"
+version = "3.5.0.rc2"
 description = "Provider package apache-airflow-providers-segment for Apache Airflow"
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
     "analytics-python>=1.2.9",
-    "apache-airflow>=2.6.0.dev0",
+    "apache-airflow>=2.7.0rc0",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-segment/3.5.0"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-segment/3.5.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
```

### Comparing `apache_airflow_providers_segment-3.5.0rc1/PKG-INFO` & `apache_airflow_providers_segment-3.5.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-segment
-Version: 3.5.0rc1
+Version: 3.5.0rc2
 Summary: Provider package apache-airflow-providers-segment for Apache Airflow
 Keywords: airflow-provider,segment,airflow,integration
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
 Requires-Dist: analytics-python>=1.2.9
-Requires-Dist: apache-airflow>=2.6.0.dev0
+Requires-Dist: apache-airflow>=2.7.0rc0
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-segment/3.5.0/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-segment/3.5.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
@@ -70,15 +71,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-segment``
 
-Release: ``3.5.0.rc1``
+Release: ``3.5.0.rc2``
 
 
 `Segment <https://segment.com/>`__
 
 
 Provider package
 ----------------
@@ -92,21 +93,21 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-segment``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ====================  ==================
 PIP package           Version required
 ====================  ==================
-``apache-airflow``    ``>=2.6.0``
+``apache-airflow``    ``>=2.7.0``
 ``analytics-python``  ``>=1.2.9``
 ====================  ==================
 
 The changelog for the provider package can be found in the
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-segment/3.5.0/changelog.html>`_.
```

