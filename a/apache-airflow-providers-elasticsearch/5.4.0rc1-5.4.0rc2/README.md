# Comparing `tmp/apache_airflow_providers_elasticsearch-5.4.0rc1.tar.gz` & `tmp/apache_airflow_providers_elasticsearch-5.4.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_elasticsearch-5.4.0rc1.tar", last modified: Mon Jan 22 08:27:50 2024, max compression
+gzip compressed data, was "apache_airflow_providers_elasticsearch-5.4.0rc2.tar", last modified: Tue Apr 30 11:25:11 2024, max compression
```

## Comparing `apache_airflow_providers_elasticsearch-5.4.0rc1.tar` & `apache_airflow_providers_elasticsearch-5.4.0rc2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     4329 2024-01-22 08:27:50.000000 apache_airflow_providers_elasticsearch-5.4.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-01-22 08:27:50.000000 apache_airflow_providers_elasticsearch-5.4.0rc1/airflow/providers/elasticsearch/LICENSE
--rw-r--r--   0        0        0     1588 2024-01-22 08:27:50.000000 apache_airflow_providers_elasticsearch-5.4.0rc1/airflow/providers/elasticsearch/__init__.py
--rw-r--r--   0        0        0     7878 2024-01-22 08:27:50.000000 apache_airflow_providers_elasticsearch-5.4.0rc1/airflow/providers/elasticsearch/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-01-22 08:27:50.000000 apache_airflow_providers_elasticsearch-5.4.0rc1/airflow/providers/elasticsearch/hooks/__init__.py
--rw-r--r--   0        0        0     6448 2024-01-22 08:27:50.000000 apache_airflow_providers_elasticsearch-5.4.0rc1/airflow/providers/elasticsearch/hooks/elasticsearch.py
--rw-r--r--   0        0        0      785 2024-01-22 08:27:50.000000 apache_airflow_providers_elasticsearch-5.4.0rc1/airflow/providers/elasticsearch/log/__init__.py
--rw-r--r--   0        0        0     1640 2024-01-22 08:27:50.000000 apache_airflow_providers_elasticsearch-5.4.0rc1/airflow/providers/elasticsearch/log/es_json_formatter.py
--rw-r--r--   0        0        0     5428 2024-01-22 08:27:50.000000 apache_airflow_providers_elasticsearch-5.4.0rc1/airflow/providers/elasticsearch/log/es_response.py
--rw-r--r--   0        0        0    25257 2024-01-22 08:27:50.000000 apache_airflow_providers_elasticsearch-5.4.0rc1/airflow/providers/elasticsearch/log/es_task_handler.py
--rw-r--r--   0        0        0     3125 2024-01-22 08:27:50.000000 apache_airflow_providers_elasticsearch-5.4.0rc1/pyproject.toml
--rw-r--r--   0        0        0     6178 1970-01-01 00:00:00.000000 apache_airflow_providers_elasticsearch-5.4.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     4334 2024-04-30 11:25:11.000000 apache_airflow_providers_elasticsearch-5.4.0rc2/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-30 11:25:11.000000 apache_airflow_providers_elasticsearch-5.4.0rc2/airflow/providers/elasticsearch/LICENSE
+-rw-r--r--   0        0        0     1588 2024-04-30 11:25:11.000000 apache_airflow_providers_elasticsearch-5.4.0rc2/airflow/providers/elasticsearch/__init__.py
+-rw-r--r--   0        0        0     7941 2024-04-30 11:25:11.000000 apache_airflow_providers_elasticsearch-5.4.0rc2/airflow/providers/elasticsearch/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:25:11.000000 apache_airflow_providers_elasticsearch-5.4.0rc2/airflow/providers/elasticsearch/hooks/__init__.py
+-rw-r--r--   0        0        0     6362 2024-04-30 11:25:11.000000 apache_airflow_providers_elasticsearch-5.4.0rc2/airflow/providers/elasticsearch/hooks/elasticsearch.py
+-rw-r--r--   0        0        0      785 2024-04-30 11:25:11.000000 apache_airflow_providers_elasticsearch-5.4.0rc2/airflow/providers/elasticsearch/log/__init__.py
+-rw-r--r--   0        0        0     1796 2024-04-30 11:25:11.000000 apache_airflow_providers_elasticsearch-5.4.0rc2/airflow/providers/elasticsearch/log/es_json_formatter.py
+-rw-r--r--   0        0        0     6037 2024-04-30 11:25:11.000000 apache_airflow_providers_elasticsearch-5.4.0rc2/airflow/providers/elasticsearch/log/es_response.py
+-rw-r--r--   0        0        0    25310 2024-04-30 11:25:11.000000 apache_airflow_providers_elasticsearch-5.4.0rc2/airflow/providers/elasticsearch/log/es_task_handler.py
+-rw-r--r--   0        0        0     3167 2024-04-30 11:25:11.000000 apache_airflow_providers_elasticsearch-5.4.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     6230 1970-01-01 00:00:00.000000 apache_airflow_providers_elasticsearch-5.4.0rc2/PKG-INFO
```

### Comparing `apache_airflow_providers_elasticsearch-5.4.0rc1/README.rst` & `apache_airflow_providers_elasticsearch-5.4.0rc2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-elasticsearch``
 
-Release: ``5.4.0.rc1``
+Release: ``5.4.0.rc2``
 
 
 `Elasticsearch <https://www.elastic.co/elasticsearch>`__
 
 
 Provider package
 ----------------
@@ -60,23 +60,23 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-elasticsearch``
 
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
 ``elasticsearch``                        ``>=8.10,<9``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
```

### Comparing `apache_airflow_providers_elasticsearch-5.4.0rc1/airflow/providers/elasticsearch/LICENSE` & `apache_airflow_providers_elasticsearch-5.4.0rc2/airflow/providers/elasticsearch/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_elasticsearch-5.4.0rc1/airflow/providers/elasticsearch/__init__.py` & `apache_airflow_providers_elasticsearch-5.4.0rc2/airflow/providers/elasticsearch/__init__.py`

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
-        f"The package `apache-airflow-providers-elasticsearch:{__version__}` needs Apache Airflow 2.6.0+"
+        f"The package `apache-airflow-providers-elasticsearch:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_elasticsearch-5.4.0rc1/airflow/providers/elasticsearch/get_provider_info.py` & `apache_airflow_providers_elasticsearch-5.4.0rc2/airflow/providers/elasticsearch/get_provider_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,17 +24,20 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-elasticsearch",
         "name": "Elasticsearch",
         "description": "`Elasticsearch <https://www.elastic.co/elasticsearch>`__\n",
         "state": "ready",
-        "source-date-epoch": 1705912070,
+        "source-date-epoch": 1714476311,
         "versions": [
             "5.4.0",
+            "5.3.4",
+            "5.3.3",
+            "5.3.2",
             "5.3.1",
             "5.3.0",
             "5.2.0",
             "5.1.1",
             "5.1.0",
             "5.0.2",
             "5.0.1",
@@ -62,15 +65,15 @@
             "1.0.4",
             "1.0.3",
             "1.0.2",
             "1.0.1",
             "1.0.0",
         ],
         "dependencies": [
-            "apache-airflow>=2.6.0",
+            "apache-airflow>=2.7.0",
             "apache-airflow-providers-common-sql>=1.3.1",
             "elasticsearch>=8.10,<9",
         ],
         "integrations": [
             {
                 "integration-name": "Elasticsearch",
                 "external-doc-url": "https://www.elastic.co/elasticsearch",
```

### Comparing `apache_airflow_providers_elasticsearch-5.4.0rc1/airflow/providers/elasticsearch/hooks/__init__.py` & `apache_airflow_providers_elasticsearch-5.4.0rc2/airflow/providers/elasticsearch/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_elasticsearch-5.4.0rc1/airflow/providers/elasticsearch/hooks/elasticsearch.py` & `apache_airflow_providers_elasticsearch-5.4.0rc2/airflow/providers/elasticsearch/hooks/elasticsearch.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
-import warnings
 from functools import cached_property
 from typing import TYPE_CHECKING, Any
 from urllib import parse
 
+from deprecated import deprecated
 from elasticsearch import Elasticsearch
 
 from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.hooks.base import BaseHook
 from airflow.providers.common.sql.hooks.sql import DbApiHook
 
 if TYPE_CHECKING:
@@ -134,42 +134,40 @@
 
             if extras_length:
                 uri += "&"
 
         return uri
 
 
+@deprecated(
+    reason="Please use `airflow.providers.elasticsearch.hooks.elasticsearch.ElasticsearchSQLHook`.",
+    category=AirflowProviderDeprecationWarning,
+)
 class ElasticsearchHook(ElasticsearchSQLHook):
     """
     This class is deprecated and was renamed to ElasticsearchSQLHook.
 
     Please use :class:`airflow.providers.elasticsearch.hooks.elasticsearch.ElasticsearchSQLHook`.
     """
 
     def __init__(self, *args, **kwargs):
-        warnings.warn(
-            """This class is deprecated.
-            Please use `airflow.providers.elasticsearch.hooks.elasticsearch.ElasticsearchSQLHook`.""",
-            AirflowProviderDeprecationWarning,
-            stacklevel=3,
-        )
         super().__init__(*args, **kwargs)
 
 
 class ElasticsearchPythonHook(BaseHook):
     """
     Interacts with Elasticsearch. This hook uses the official Elasticsearch Python Client.
 
     :param hosts: list: A list of a single or many Elasticsearch instances. Example: ["http://localhost:9200"]
     :param es_conn_args: dict: Additional arguments you might need to enter to connect to Elasticsearch.
                                 Example: {"ca_cert":"/path/to/cert", "basic_auth": "(user, pass)"}
     """
 
-    def __init__(self, hosts: list[Any], es_conn_args: dict | None = None, **kwargs):
-        super().__init__(**kwargs)
+    def __init__(self, hosts: list[Any], es_conn_args: dict | None = None):
+        super().__init__()
         self.hosts = hosts
         self.es_conn_args = es_conn_args or {}
 
     def _get_elastic_connection(self):
         """Return the Elasticsearch client."""
         client = Elasticsearch(self.hosts, **self.es_conn_args)
```

### Comparing `apache_airflow_providers_elasticsearch-5.4.0rc1/airflow/providers/elasticsearch/log/__init__.py` & `apache_airflow_providers_elasticsearch-5.4.0rc2/airflow/providers/elasticsearch/log/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_elasticsearch-5.4.0rc1/airflow/providers/elasticsearch/log/es_json_formatter.py` & `apache_airflow_providers_elasticsearch-5.4.0rc2/airflow/providers/elasticsearch/log/es_json_formatter.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,28 +12,32 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
+from datetime import datetime
+
 import pendulum
 
 from airflow.utils.log.json_formatter import JSONFormatter
 
 
 class ElasticsearchJSONFormatter(JSONFormatter):
     """Convert a log record to JSON with ISO 8601 date and time format."""
 
     default_time_format = "%Y-%m-%dT%H:%M:%S"
     default_msec_format = "%s.%03d"
     default_tz_format = "%z"
 
     def formatTime(self, record, datefmt=None):
         """Return the creation time of the LogRecord in ISO 8601 date/time format in the local time zone."""
-        dt = pendulum.from_timestamp(record.created, tz=pendulum.local_timezone())
+        # TODO: Use airflow.utils.timezone.from_timestamp(record.created, tz="local")
+        #  as soon as min Airflow 2.9.0
+        dt = datetime.fromtimestamp(record.created, tz=pendulum.local_timezone())
         s = dt.strftime(datefmt or self.default_time_format)
         if self.default_msec_format:
             s = self.default_msec_format % (s, record.msecs)
         if self.default_tz_format:
             s += dt.strftime(self.default_tz_format)
         return s
```

### Comparing `apache_airflow_providers_elasticsearch-5.4.0rc1/airflow/providers/elasticsearch/log/es_response.py` & `apache_airflow_providers_elasticsearch-5.4.0rc2/airflow/providers/elasticsearch/log/es_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,39 +30,44 @@
 
     def __init__(self, _list):
         if not isinstance(_list, list):
             _list = list(_list)
         self._l_ = _list
 
     def __getitem__(self, k):
+        """Retrieve an item or a slice from the list. If the item is a dictionary, it is wrapped in an AttributeDict."""
         val = self._l_[k]
         if isinstance(val, slice):
             return AttributeList(val)
         return _wrap(val)
 
     def __iter__(self):
+        """Provide an iterator for the list or the dictionary."""
         return (_wrap(i) for i in self._l_)
 
     def __bool__(self):
+        """Check if the list is non-empty."""
         return bool(self._l_)
 
 
 class AttributeDict:
     """Helper class to provide attribute like access to Dictionary objects."""
 
     def __init__(self, d):
         super().__setattr__("_d_", d)
 
     def __getattr__(self, attr_name):
+        """Retrieve an item as an attribute from the dictionary."""
         try:
             return self.__getitem__(attr_name)
         except KeyError:
             raise AttributeError(f"{self.__class__.__name__!r} object has no attribute {attr_name!r}")
 
     def __getitem__(self, key):
+        """Retrieve an item using a key from the dictionary."""
         return _wrap(self._d_[key])
 
     def to_dict(self):
         return self._d_
 
 
 class Hit(AttributeDict):
@@ -116,22 +121,25 @@
 
     def __init__(self, search, response, doc_class=None):
         super().__setattr__("_search", search)
         super().__setattr__("_doc_class", doc_class)
         super().__init__(response)
 
     def __iter__(self) -> Iterator[Hit]:
+        """Provide an iterator over the hits in the Elasticsearch response."""
         return iter(self.hits)
 
     def __getitem__(self, key):
+        """Retrieve a specific hit or a slice of hits from the Elasticsearch response."""
         if isinstance(key, (slice, int)):
             return self.hits[key]
         return super().__getitem__(key)
 
     def __bool__(self):
+        """Evaluate the presence of hits in the Elasticsearch response."""
         return bool(self.hits)
 
     @property
     def hits(self) -> list[Hit]:
         """
         This property provides access to the hits (i.e., the results) of the Elasticsearch response.
```

### Comparing `apache_airflow_providers_elasticsearch-5.4.0rc1/airflow/providers/elasticsearch/log/es_task_handler.py` & `apache_airflow_providers_elasticsearch-5.4.0rc2/airflow/providers/elasticsearch/log/es_task_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,14 +221,16 @@
                 ti = _ensure_ti(ti, session)
             dag_run = ti.get_dagrun(session=session)
             if USE_PER_RUN_LOG_ID:
                 log_id_template = dag_run.get_log_template(session=session).elasticsearch_id
             else:
                 log_id_template = self.log_id_template
 
+        if TYPE_CHECKING:
+            assert ti.task
         try:
             dag = ti.task.dag
         except AttributeError:  # ti.task is not always set.
             data_interval = (dag_run.data_interval_start, dag_run.data_interval_end)
         else:
             if TYPE_CHECKING:
                 assert dag is not None
```

### Comparing `apache_airflow_providers_elasticsearch-5.4.0rc1/pyproject.toml` & `apache_airflow_providers_elasticsearch-5.4.0rc2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-elasticsearch"
-version = "5.4.0.rc1"
+version = "5.4.0.rc2"
 description = "Provider package apache-airflow-providers-elasticsearch for Apache Airflow"
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
-    "apache-airflow-providers-common-sql>=1.3.1.dev0",
-    "apache-airflow>=2.6.0.dev0",
+    "apache-airflow-providers-common-sql>=1.3.1rc0",
+    "apache-airflow>=2.7.0rc0",
     "elasticsearch>=8.10,<9",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-elasticsearch/5.4.0"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-elasticsearch/5.4.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
```

### Comparing `apache_airflow_providers_elasticsearch-5.4.0rc1/PKG-INFO` & `apache_airflow_providers_elasticsearch-5.4.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-elasticsearch
-Version: 5.4.0rc1
+Version: 5.4.0rc2
 Summary: Provider package apache-airflow-providers-elasticsearch for Apache Airflow
 Keywords: airflow-provider,elasticsearch,airflow,integration
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
-Requires-Dist: apache-airflow-providers-common-sql>=1.3.1.dev0
-Requires-Dist: apache-airflow>=2.6.0.dev0
+Requires-Dist: apache-airflow-providers-common-sql>=1.3.1rc0
+Requires-Dist: apache-airflow>=2.7.0rc0
 Requires-Dist: elasticsearch>=8.10,<9
 Requires-Dist: apache-airflow-providers-common-sql ; extra == "common.sql"
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-elasticsearch/5.4.0/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-elasticsearch/5.4.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
@@ -73,15 +74,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-elasticsearch``
 
-Release: ``5.4.0.rc1``
+Release: ``5.4.0.rc2``
 
 
 `Elasticsearch <https://www.elastic.co/elasticsearch>`__
 
 
 Provider package
 ----------------
@@ -95,23 +96,23 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-elasticsearch``
 
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
 ``elasticsearch``                        ``>=8.10,<9``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
```

