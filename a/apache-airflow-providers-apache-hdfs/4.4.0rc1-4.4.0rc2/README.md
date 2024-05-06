# Comparing `tmp/apache_airflow_providers_apache_hdfs-4.4.0rc1.tar.gz` & `tmp/apache_airflow_providers_apache_hdfs-4.4.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_apache_hdfs-4.4.0rc1.tar", last modified: Mon Jan 22 08:25:07 2024, max compression
+gzip compressed data, was "apache_airflow_providers_apache_hdfs-4.4.0rc2.tar", last modified: Tue Apr 30 11:13:10 2024, max compression
```

## Comparing `apache_airflow_providers_apache_hdfs-4.4.0rc1.tar` & `apache_airflow_providers_apache_hdfs-4.4.0rc2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     3332 2024-01-22 08:25:07.000000 apache_airflow_providers_apache_hdfs-4.4.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-01-22 08:25:07.000000 apache_airflow_providers_apache_hdfs-4.4.0rc1/airflow/providers/apache/hdfs/LICENSE
--rw-r--r--   0        0        0     1586 2024-01-22 08:25:07.000000 apache_airflow_providers_apache_hdfs-4.4.0rc1/airflow/providers/apache/hdfs/__init__.py
--rw-r--r--   0        0        0     3356 2024-01-22 08:25:07.000000 apache_airflow_providers_apache_hdfs-4.4.0rc1/airflow/providers/apache/hdfs/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-01-22 08:25:07.000000 apache_airflow_providers_apache_hdfs-4.4.0rc1/airflow/providers/apache/hdfs/hooks/__init__.py
--rw-r--r--   0        0        0     2309 2024-01-22 08:25:07.000000 apache_airflow_providers_apache_hdfs-4.4.0rc1/airflow/providers/apache/hdfs/hooks/hdfs.py
--rw-r--r--   0        0        0     6592 2024-01-22 08:25:07.000000 apache_airflow_providers_apache_hdfs-4.4.0rc1/airflow/providers/apache/hdfs/hooks/webhdfs.py
--rw-r--r--   0        0        0      785 2024-01-22 08:25:07.000000 apache_airflow_providers_apache_hdfs-4.4.0rc1/airflow/providers/apache/hdfs/log/__init__.py
--rw-r--r--   0        0        0     4251 2024-01-22 08:25:07.000000 apache_airflow_providers_apache_hdfs-4.4.0rc1/airflow/providers/apache/hdfs/log/hdfs_task_handler.py
--rw-r--r--   0        0        0      787 2024-01-22 08:25:07.000000 apache_airflow_providers_apache_hdfs-4.4.0rc1/airflow/providers/apache/hdfs/sensors/__init__.py
--rw-r--r--   0        0        0     2104 2024-01-22 08:25:07.000000 apache_airflow_providers_apache_hdfs-4.4.0rc1/airflow/providers/apache/hdfs/sensors/hdfs.py
--rw-r--r--   0        0        0     1653 2024-01-22 08:25:07.000000 apache_airflow_providers_apache_hdfs-4.4.0rc1/airflow/providers/apache/hdfs/sensors/web_hdfs.py
--rw-r--r--   0        0        0     2976 2024-01-22 08:25:07.000000 apache_airflow_providers_apache_hdfs-4.4.0rc1/pyproject.toml
--rw-r--r--   0        0        0     5020 1970-01-01 00:00:00.000000 apache_airflow_providers_apache_hdfs-4.4.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     3337 2024-04-30 11:13:10.000000 apache_airflow_providers_apache_hdfs-4.4.0rc2/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-30 11:13:10.000000 apache_airflow_providers_apache_hdfs-4.4.0rc2/airflow/providers/apache/hdfs/LICENSE
+-rw-r--r--   0        0        0     1586 2024-04-30 11:13:10.000000 apache_airflow_providers_apache_hdfs-4.4.0rc2/airflow/providers/apache/hdfs/__init__.py
+-rw-r--r--   0        0        0     3377 2024-04-30 11:13:10.000000 apache_airflow_providers_apache_hdfs-4.4.0rc2/airflow/providers/apache/hdfs/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:13:10.000000 apache_airflow_providers_apache_hdfs-4.4.0rc2/airflow/providers/apache/hdfs/hooks/__init__.py
+-rw-r--r--   0        0        0     2315 2024-04-30 11:13:10.000000 apache_airflow_providers_apache_hdfs-4.4.0rc2/airflow/providers/apache/hdfs/hooks/hdfs.py
+-rw-r--r--   0        0        0     6575 2024-04-30 11:13:10.000000 apache_airflow_providers_apache_hdfs-4.4.0rc2/airflow/providers/apache/hdfs/hooks/webhdfs.py
+-rw-r--r--   0        0        0      785 2024-04-30 11:13:10.000000 apache_airflow_providers_apache_hdfs-4.4.0rc2/airflow/providers/apache/hdfs/log/__init__.py
+-rw-r--r--   0        0        0     4251 2024-04-30 11:13:10.000000 apache_airflow_providers_apache_hdfs-4.4.0rc2/airflow/providers/apache/hdfs/log/hdfs_task_handler.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:13:10.000000 apache_airflow_providers_apache_hdfs-4.4.0rc2/airflow/providers/apache/hdfs/sensors/__init__.py
+-rw-r--r--   0        0        0     2141 2024-04-30 11:13:10.000000 apache_airflow_providers_apache_hdfs-4.4.0rc2/airflow/providers/apache/hdfs/sensors/hdfs.py
+-rw-r--r--   0        0        0     1653 2024-04-30 11:13:10.000000 apache_airflow_providers_apache_hdfs-4.4.0rc2/airflow/providers/apache/hdfs/sensors/web_hdfs.py
+-rw-r--r--   0        0        0     3020 2024-04-30 11:13:10.000000 apache_airflow_providers_apache_hdfs-4.4.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     5074 1970-01-01 00:00:00.000000 apache_airflow_providers_apache_hdfs-4.4.0rc2/PKG-INFO
```

### Comparing `apache_airflow_providers_apache_hdfs-4.4.0rc1/README.rst` & `apache_airflow_providers_apache_hdfs-4.4.0rc2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-apache-hdfs``
 
-Release: ``4.4.0.rc1``
+Release: ``4.4.0.rc2``
 
 
 `Hadoop Distributed File System (HDFS) <https://hadoop.apache.org/docs/r1.2.1/hdfs_design.html>`__
 and `WebHDFS <https://hadoop.apache.org/docs/current/hadoop-project-dist/hadoop-hdfs/WebHDFS.html>`__.
 
 
 Provider package
@@ -61,21 +61,21 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apache-hdfs``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 =================================  ==================
 PIP package                        Version required
 =================================  ==================
-``apache-airflow``                 ``>=2.6.0``
+``apache-airflow``                 ``>=2.7.0``
 ``hdfs[avro,dataframe,kerberos]``  ``>=2.0.4``
 =================================  ==================
 
 The changelog for the provider package can be found in the
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-apache-hdfs/4.4.0/changelog.html>`_.
```

### Comparing `apache_airflow_providers_apache_hdfs-4.4.0rc1/airflow/providers/apache/hdfs/LICENSE` & `apache_airflow_providers_apache_hdfs-4.4.0rc2/airflow/providers/apache/hdfs/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_hdfs-4.4.0rc1/airflow/providers/apache/hdfs/__init__.py` & `apache_airflow_providers_apache_hdfs-4.4.0rc2/airflow/providers/apache/hdfs/__init__.py`

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
-        f"The package `apache-airflow-providers-apache-hdfs:{__version__}` needs Apache Airflow 2.6.0+"
+        f"The package `apache-airflow-providers-apache-hdfs:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_apache_hdfs-4.4.0rc1/airflow/providers/apache/hdfs/get_provider_info.py` & `apache_airflow_providers_apache_hdfs-4.4.0rc2/airflow/providers/apache/hdfs/get_provider_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,17 +24,18 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-apache-hdfs",
         "name": "Apache HDFS",
         "description": "`Hadoop Distributed File System (HDFS) <https://hadoop.apache.org/docs/r1.2.1/hdfs_design.html>`__\nand `WebHDFS <https://hadoop.apache.org/docs/current/hadoop-project-dist/hadoop-hdfs/WebHDFS.html>`__.\n",
         "state": "ready",
-        "source-date-epoch": 1705911907,
+        "source-date-epoch": 1714475590,
         "versions": [
             "4.4.0",
+            "4.3.3",
             "4.3.2",
             "4.3.1",
             "4.3.0",
             "4.2.0",
             "4.1.1",
             "4.1.0",
             "4.0.0",
@@ -49,15 +50,15 @@
             "2.2.0",
             "2.1.1",
             "2.1.0",
             "2.0.0",
             "1.0.1",
             "1.0.0",
         ],
-        "dependencies": ["apache-airflow>=2.6.0", "hdfs[avro,dataframe,kerberos]>=2.0.4"],
+        "dependencies": ["apache-airflow>=2.7.0", "hdfs[avro,dataframe,kerberos]>=2.0.4"],
         "integrations": [
             {
                 "integration-name": "Hadoop Distributed File System (HDFS)",
                 "external-doc-url": "https://hadoop.apache.org/docs/r1.2.1/hdfs_design.html",
                 "logo": "/integration-logos/apache/hadoop.png",
                 "tags": ["apache"],
             },
```

### Comparing `apache_airflow_providers_apache_hdfs-4.4.0rc1/airflow/providers/apache/hdfs/hooks/__init__.py` & `apache_airflow_providers_apache_hdfs-4.4.0rc2/airflow/providers/apache/hdfs/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_hdfs-4.4.0rc1/airflow/providers/apache/hdfs/hooks/hdfs.py` & `apache_airflow_providers_apache_hdfs-4.4.0rc2/airflow/providers/apache/hdfs/hooks/hdfs.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,22 +34,22 @@
     Please convert your DAGs to use the WebHdfsHook or downgrade the provider
     to below 4.* if you want to continue using it. If you want to use earlier
     provider you can downgrade to latest released 3.* version using
     `pip install apache-airflow-providers-apache-hdfs==3.2.1` (no constraints).
     """
 
     def __init__(self, *args, **kwargs):
-        raise Exception(_EXCEPTION_MESSAGE)
+        raise RuntimeError(_EXCEPTION_MESSAGE)
 
 
 class HDFSHook(BaseHook):
     """
     This Hook has been removed and is not functional.
 
     Please convert your DAGs to use the WebHdfsHook or downgrade the provider
     to below 4.*. if you want to continue using it. If you want to use earlier
     provider you can downgrade to latest released 3.* version using
     `pip install apache-airflow-providers-apache-hdfs==3.2.1` (no constraints).
     """
 
     def __init__(self, *args, **kwargs):
-        raise Exception(_EXCEPTION_MESSAGE)
+        raise RuntimeError(_EXCEPTION_MESSAGE)
```

### Comparing `apache_airflow_providers_apache_hdfs-4.4.0rc1/airflow/providers/apache/hdfs/hooks/webhdfs.py` & `apache_airflow_providers_apache_hdfs-4.4.0rc2/airflow/providers/apache/hdfs/hooks/webhdfs.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """Hook for Web HDFS."""
+
 from __future__ import annotations
 
 import logging
 import socket
 from typing import Any
 
 import requests
@@ -53,16 +54,16 @@
     """
 
     conn_type = "webhdfs"
     conn_name_attr = "webhdfs_conn_id"
     default_conn_name = "webhdfs_default"
     hook_name = "Apache WebHDFS"
 
-    def __init__(self, webhdfs_conn_id: str = default_conn_name, proxy_user: str | None = None, **kwargs):
-        super().__init__(**kwargs)
+    def __init__(self, webhdfs_conn_id: str = default_conn_name, proxy_user: str | None = None):
+        super().__init__()
         self.webhdfs_conn_id = webhdfs_conn_id
         self.proxy_user = proxy_user
 
     def get_conn(self) -> Any:
         """
         Establish a connection depending on the security mode set via config or environment variable.
```

### Comparing `apache_airflow_providers_apache_hdfs-4.4.0rc1/airflow/providers/apache/hdfs/log/__init__.py` & `apache_airflow_providers_apache_hdfs-4.4.0rc2/airflow/providers/apache/hdfs/log/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_hdfs-4.4.0rc1/airflow/providers/apache/hdfs/log/hdfs_task_handler.py` & `apache_airflow_providers_apache_hdfs-4.4.0rc2/airflow/providers/apache/hdfs/log/hdfs_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_hdfs-4.4.0rc1/airflow/providers/apache/hdfs/sensors/__init__.py` & `apache_airflow_providers_apache_hdfs-4.4.0rc2/airflow/providers/apache/hdfs/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_hdfs-4.4.0rc1/airflow/providers/apache/hdfs/sensors/hdfs.py` & `apache_airflow_providers_apache_hdfs-4.4.0rc2/airflow/providers/apache/hdfs/sensors/hdfs.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 from airflow.sensors.base import BaseSensorOperator
 
+# Ignore missing docstring
+
 _EXCEPTION_MESSAGE = """The old HDFS Sensors have been removed in 4.0.0 version of the apache.hdfs provider.
 Please convert your DAGs to use the WebHdfsSensor or downgrade the provider to below 4.*
 if you want to continue using it.
 If you want to use earlier provider you can downgrade to latest released 3.* version
 using `pip install apache-airflow-providers-apache-hdfs==3.2.1` (no constraints)
 """
 
@@ -33,18 +35,18 @@
     Please convert your DAGs to use the WebHdfsSensor or downgrade the provider
     to below 4.* if you want to continue using it. If you want to use earlier
     provider you can downgrade to latest released 3.* version using
     `pip install apache-airflow-providers-apache-hdfs==3.2.1` (no constraints).
     """
 
     def __init__(self, *args, **kwargs):
-        raise Exception(_EXCEPTION_MESSAGE)
+        raise RuntimeError(_EXCEPTION_MESSAGE)
 
 
 class HdfsRegexSensor(HdfsSensor):  # noqa: D101 Ignore missing docstring
     def __init__(self, *args, **kwargs):
-        raise Exception(_EXCEPTION_MESSAGE)
+        raise RuntimeError(_EXCEPTION_MESSAGE)
 
 
 class HdfsFolderSensor(HdfsSensor):  # noqa: D101 Ignore missing docstring
     def __init__(self, *args, **kwargs):
-        raise Exception(_EXCEPTION_MESSAGE)
+        raise RuntimeError(_EXCEPTION_MESSAGE)
```

### Comparing `apache_airflow_providers_apache_hdfs-4.4.0rc1/airflow/providers/apache/hdfs/sensors/web_hdfs.py` & `apache_airflow_providers_apache_hdfs-4.4.0rc2/airflow/providers/apache/hdfs/sensors/web_hdfs.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_hdfs-4.4.0rc1/pyproject.toml` & `apache_airflow_providers_apache_hdfs-4.4.0rc2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-apache-hdfs"
-version = "4.4.0.rc1"
+version = "4.4.0.rc2"
 description = "Provider package apache-airflow-providers-apache-hdfs for Apache Airflow"
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
     "hdfs[avro,dataframe,kerberos]>=2.0.4",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-apache-hdfs/4.4.0"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-apache-hdfs/4.4.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
```

### Comparing `apache_airflow_providers_apache_hdfs-4.4.0rc1/PKG-INFO` & `apache_airflow_providers_apache_hdfs-4.4.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-hdfs
-Version: 4.4.0rc1
+Version: 4.4.0rc2
 Summary: Provider package apache-airflow-providers-apache-hdfs for Apache Airflow
 Keywords: airflow-provider,apache.hdfs,airflow,integration
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
 Requires-Dist: hdfs[avro,dataframe,kerberos]>=2.0.4
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-apache-hdfs/4.4.0/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-hdfs/4.4.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
@@ -70,15 +71,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-apache-hdfs``
 
-Release: ``4.4.0.rc1``
+Release: ``4.4.0.rc2``
 
 
 `Hadoop Distributed File System (HDFS) <https://hadoop.apache.org/docs/r1.2.1/hdfs_design.html>`__
 and `WebHDFS <https://hadoop.apache.org/docs/current/hadoop-project-dist/hadoop-hdfs/WebHDFS.html>`__.
 
 
 Provider package
@@ -93,21 +94,21 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apache-hdfs``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 =================================  ==================
 PIP package                        Version required
 =================================  ==================
-``apache-airflow``                 ``>=2.6.0``
+``apache-airflow``                 ``>=2.7.0``
 ``hdfs[avro,dataframe,kerberos]``  ``>=2.0.4``
 =================================  ==================
 
 The changelog for the provider package can be found in the
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-apache-hdfs/4.4.0/changelog.html>`_.
```

