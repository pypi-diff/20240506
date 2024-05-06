# Comparing `tmp/apache_airflow_providers_redis-3.7.0rc1.tar.gz` & `tmp/apache_airflow_providers_redis-3.7.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_redis-3.7.0rc1.tar", last modified: Mon Jan 22 08:30:35 2024, max compression
+gzip compressed data, was "apache_airflow_providers_redis-3.7.0rc2.tar", last modified: Tue Apr 30 11:43:11 2024, max compression
```

## Comparing `apache_airflow_providers_redis-3.7.0rc1.tar` & `apache_airflow_providers_redis-3.7.0rc2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     3073 2024-01-22 08:30:35.000000 apache_airflow_providers_redis-3.7.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-01-22 08:30:35.000000 apache_airflow_providers_redis-3.7.0rc1/airflow/providers/redis/LICENSE
--rw-r--r--   0        0        0     1580 2024-01-22 08:30:35.000000 apache_airflow_providers_redis-3.7.0rc1/airflow/providers/redis/__init__.py
--rw-r--r--   0        0        0     2916 2024-01-22 08:30:35.000000 apache_airflow_providers_redis-3.7.0rc1/airflow/providers/redis/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-01-22 08:30:35.000000 apache_airflow_providers_redis-3.7.0rc1/airflow/providers/redis/hooks/__init__.py
--rw-r--r--   0        0        0     5795 2024-01-22 08:30:35.000000 apache_airflow_providers_redis-3.7.0rc1/airflow/providers/redis/hooks/redis.py
--rw-r--r--   0        0        0      787 2024-01-22 08:30:35.000000 apache_airflow_providers_redis-3.7.0rc1/airflow/providers/redis/log/__init__.py
--rw-r--r--   0        0        0     3677 2024-01-22 08:30:35.000000 apache_airflow_providers_redis-3.7.0rc1/airflow/providers/redis/log/redis_task_handler.py
--rw-r--r--   0        0        0      787 2024-01-22 08:30:35.000000 apache_airflow_providers_redis-3.7.0rc1/airflow/providers/redis/operators/__init__.py
--rw-r--r--   0        0        0     2096 2024-01-22 08:30:35.000000 apache_airflow_providers_redis-3.7.0rc1/airflow/providers/redis/operators/redis_publish.py
--rw-r--r--   0        0        0      787 2024-01-22 08:30:35.000000 apache_airflow_providers_redis-3.7.0rc1/airflow/providers/redis/sensors/__init__.py
--rw-r--r--   0        0        0     1585 2024-01-22 08:30:35.000000 apache_airflow_providers_redis-3.7.0rc1/airflow/providers/redis/sensors/redis_key.py
--rw-r--r--   0        0        0     2672 2024-01-22 08:30:35.000000 apache_airflow_providers_redis-3.7.0rc1/airflow/providers/redis/sensors/redis_pub_sub.py
--rw-r--r--   0        0        0     2925 2024-01-22 08:30:35.000000 apache_airflow_providers_redis-3.7.0rc1/pyproject.toml
--rw-r--r--   0        0        0     4722 1970-01-01 00:00:00.000000 apache_airflow_providers_redis-3.7.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     3082 2024-04-30 11:43:11.000000 apache_airflow_providers_redis-3.7.0rc2/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-30 11:43:11.000000 apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/LICENSE
+-rw-r--r--   0        0        0     1580 2024-04-30 11:43:11.000000 apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/__init__.py
+-rw-r--r--   0        0        0     2938 2024-04-30 11:43:11.000000 apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:43:11.000000 apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/hooks/__init__.py
+-rw-r--r--   0        0        0     5804 2024-04-30 11:43:11.000000 apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/hooks/redis.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:43:11.000000 apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/log/__init__.py
+-rw-r--r--   0        0        0     3677 2024-04-30 11:43:11.000000 apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/log/redis_task_handler.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:43:11.000000 apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/operators/__init__.py
+-rw-r--r--   0        0        0     2096 2024-04-30 11:43:11.000000 apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/operators/redis_publish.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:43:11.000000 apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/sensors/__init__.py
+-rw-r--r--   0        0        0     1585 2024-04-30 11:43:11.000000 apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/sensors/redis_key.py
+-rw-r--r--   0        0        0     2672 2024-04-30 11:43:11.000000 apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/sensors/redis_pub_sub.py
+-rw-r--r--   0        0        0     2970 2024-04-30 11:43:11.000000 apache_airflow_providers_redis-3.7.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     4781 1970-01-01 00:00:00.000000 apache_airflow_providers_redis-3.7.0rc2/PKG-INFO
```

### Comparing `apache_airflow_providers_redis-3.7.0rc1/README.rst` & `apache_airflow_providers_redis-3.7.0rc2/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-redis``
 
-Release: ``3.7.0.rc1``
+Release: ``3.7.0.rc2``
 
 
 `Redis <https://redis.io/>`__
 
 
 Provider package
 ----------------
@@ -60,21 +60,21 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-redis``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
-==================  ==========================
+==================  ===========================
 PIP package         Version required
-==================  ==========================
-``apache-airflow``  ``>=2.6.0``
-``redis``           ``>=4.5.2,!=4.5.5,<5.0.0``
-==================  ==========================
+==================  ===========================
+``apache-airflow``  ``>=2.7.0``
+``redis``           ``>=4.5.2,!=4.5.5,!=5.0.2``
+==================  ===========================
 
 The changelog for the provider package can be found in the
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-redis/3.7.0/changelog.html>`_.
```

### Comparing `apache_airflow_providers_redis-3.7.0rc1/airflow/providers/redis/LICENSE` & `apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_redis-3.7.0rc1/airflow/providers/redis/__init__.py` & `apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/__init__.py`

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
-        f"The package `apache-airflow-providers-redis:{__version__}` needs Apache Airflow 2.6.0+"
+        f"The package `apache-airflow-providers-redis:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_redis-3.7.0rc1/airflow/providers/redis/get_provider_info.py` & `apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/get_provider_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,17 +24,18 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-redis",
         "name": "Redis",
         "description": "`Redis <https://redis.io/>`__\n",
         "state": "ready",
-        "source-date-epoch": 1705912235,
+        "source-date-epoch": 1714477391,
         "versions": [
             "3.7.0",
+            "3.6.1",
             "3.6.0",
             "3.5.0",
             "3.4.1",
             "3.4.0",
             "3.3.2",
             "3.3.1",
             "3.3.0",
@@ -46,15 +47,15 @@
             "2.0.3",
             "2.0.2",
             "2.0.1",
             "2.0.0",
             "1.0.1",
             "1.0.0",
         ],
-        "dependencies": ["apache-airflow>=2.6.0", "redis>=4.5.2,<5.0.0,!=4.5.5"],
+        "dependencies": ["apache-airflow>=2.7.0", "redis>=4.5.2,!=4.5.5,!=5.0.2"],
         "integrations": [
             {
                 "integration-name": "Redis",
                 "external-doc-url": "https://redis.io/",
                 "logo": "/integration-logos/redis/Redis.png",
                 "tags": ["software"],
             }
```

### Comparing `apache_airflow_providers_redis-3.7.0rc1/airflow/providers/redis/hooks/__init__.py` & `apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_redis-3.7.0rc1/airflow/providers/redis/hooks/redis.py` & `apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/hooks/redis.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """RedisHook module."""
+
 from __future__ import annotations
 
 import warnings
 from typing import Any
 
 from redis import Redis
 
@@ -40,32 +41,32 @@
     """
 
     conn_name_attr = "redis_conn_id"
     default_conn_name = "redis_default"
     conn_type = "redis"
     hook_name = "Redis"
 
-    def __init__(self, redis_conn_id: str = default_conn_name, **kwargs) -> None:
+    def __init__(self, redis_conn_id: str = default_conn_name) -> None:
         """
-        Prepares hook to connect to a Redis database.
+        Prepare hook to connect to a Redis database.
 
         :param conn_id:     the name of the connection that has the parameters
                             we need to connect to Redis.
         """
-        super().__init__(**kwargs)
+        super().__init__()
         self.redis_conn_id = redis_conn_id
         self.redis = None
         self.host = None
         self.port = None
         self.username = None
         self.password = None
         self.db = None
 
     def get_conn(self):
-        """Returns a Redis connection."""
+        """Return a Redis connection."""
         conn = self.get_connection(self.redis_conn_id)
         self.host = conn.host
         self.port = conn.port
         self.username = conn.login
         self.password = None if str(conn.password).lower() in ["none", "false", ""] else conn.password
         self.db = conn.extra_dejson.get("db")
 
@@ -107,23 +108,23 @@
                 **ssl_args,
             )
 
         return self.redis
 
     @classmethod
     def get_ui_field_behaviour(cls) -> dict[str, Any]:
-        """Returns custom field behaviour."""
+        """Return custom UI field behaviour for Redis connection."""
         return {
             "hidden_fields": ["schema", "extra"],
             "relabeling": {},
         }
 
     @classmethod
     def get_connection_form_widgets(cls) -> dict[str, Any]:
-        """Returns connection widgets to add to connection form."""
+        """Return connection widgets to add to Redis connection form."""
         from flask_appbuilder.fieldwidgets import BS3TextFieldWidget
         from flask_babel import lazy_gettext
         from wtforms import BooleanField, IntegerField, StringField
         from wtforms.validators import Optional, any_of
 
         return {
             "db": IntegerField(lazy_gettext("DB"), widget=BS3TextFieldWidget(), default=0),
```

### Comparing `apache_airflow_providers_redis-3.7.0rc1/airflow/providers/redis/log/__init__.py` & `apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/log/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_redis-3.7.0rc1/airflow/providers/redis/log/redis_task_handler.py` & `apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/log/redis_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_redis-3.7.0rc1/airflow/providers/redis/operators/__init__.py` & `apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_redis-3.7.0rc1/airflow/providers/redis/operators/redis_publish.py` & `apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/operators/redis_publish.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_redis-3.7.0rc1/airflow/providers/redis/sensors/__init__.py` & `apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_redis-3.7.0rc1/airflow/providers/redis/sensors/redis_key.py` & `apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/sensors/redis_key.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_redis-3.7.0rc1/airflow/providers/redis/sensors/redis_pub_sub.py` & `apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/sensors/redis_pub_sub.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_redis-3.7.0rc1/pyproject.toml` & `apache_airflow_providers_redis-3.7.0rc2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-redis"
-version = "3.7.0.rc1"
+version = "3.7.0.rc2"
 description = "Provider package apache-airflow-providers-redis for Apache Airflow"
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
-    "redis>=4.5.2,<5.0.0,!=4.5.5",
+    "apache-airflow>=2.7.0rc0",
+    "redis>=4.5.2,!=4.5.5,!=5.0.2",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-redis/3.7.0"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-redis/3.7.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
```

### Comparing `apache_airflow_providers_redis-3.7.0rc1/PKG-INFO` & `apache_airflow_providers_redis-3.7.0rc2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-redis
-Version: 3.7.0rc1
+Version: 3.7.0rc2
 Summary: Provider package apache-airflow-providers-redis for Apache Airflow
 Keywords: airflow-provider,redis,airflow,integration
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
-Requires-Dist: redis>=4.5.2,<5.0.0,!=4.5.5
+Requires-Dist: apache-airflow>=2.7.0rc0
+Requires-Dist: redis>=4.5.2,!=4.5.5,!=5.0.2
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-redis/3.7.0/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-redis/3.7.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
@@ -70,15 +71,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-redis``
 
-Release: ``3.7.0.rc1``
+Release: ``3.7.0.rc2``
 
 
 `Redis <https://redis.io/>`__
 
 
 Provider package
 ----------------
@@ -92,21 +93,21 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-redis``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
-==================  ==========================
+==================  ===========================
 PIP package         Version required
-==================  ==========================
-``apache-airflow``  ``>=2.6.0``
-``redis``           ``>=4.5.2,!=4.5.5,<5.0.0``
-==================  ==========================
+==================  ===========================
+``apache-airflow``  ``>=2.7.0``
+``redis``           ``>=4.5.2,!=4.5.5,!=5.0.2``
+==================  ===========================
 
 The changelog for the provider package can be found in the
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-redis/3.7.0/changelog.html>`_.
```

