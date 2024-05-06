# Comparing `tmp/apache_airflow_providers_grpc-3.5.0rc1.tar.gz` & `tmp/apache_airflow_providers_grpc-3.5.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_grpc-3.5.0rc1.tar", last modified: Mon Jan 22 08:28:33 2024, max compression
+gzip compressed data, was "apache_airflow_providers_grpc-3.5.0rc2.tar", last modified: Tue Apr 30 11:28:59 2024, max compression
```

## Comparing `apache_airflow_providers_grpc-3.5.0rc1.tar` & `apache_airflow_providers_grpc-3.5.0rc2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3146 2024-01-22 08:28:33.000000 apache_airflow_providers_grpc-3.5.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-01-22 08:28:33.000000 apache_airflow_providers_grpc-3.5.0rc1/airflow/providers/grpc/LICENSE
--rw-r--r--   0        0        0     1579 2024-01-22 08:28:33.000000 apache_airflow_providers_grpc-3.5.0rc1/airflow/providers/grpc/__init__.py
--rw-r--r--   0        0        0     2407 2024-01-22 08:28:33.000000 apache_airflow_providers_grpc-3.5.0rc1/airflow/providers/grpc/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-01-22 08:28:33.000000 apache_airflow_providers_grpc-3.5.0rc1/airflow/providers/grpc/hooks/__init__.py
--rw-r--r--   0        0        0     6873 2024-01-22 08:28:33.000000 apache_airflow_providers_grpc-3.5.0rc1/airflow/providers/grpc/hooks/grpc.py
--rw-r--r--   0        0        0      787 2024-01-22 08:28:33.000000 apache_airflow_providers_grpc-3.5.0rc1/airflow/providers/grpc/operators/__init__.py
--rw-r--r--   0        0        0     3800 2024-01-22 08:28:33.000000 apache_airflow_providers_grpc-3.5.0rc1/airflow/providers/grpc/operators/grpc.py
--rw-r--r--   0        0        0     2974 2024-01-22 08:28:33.000000 apache_airflow_providers_grpc-3.5.0rc1/pyproject.toml
--rw-r--r--   0        0        0     4862 1970-01-01 00:00:00.000000 apache_airflow_providers_grpc-3.5.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     3151 2024-04-30 11:28:59.000000 apache_airflow_providers_grpc-3.5.0rc2/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-30 11:28:59.000000 apache_airflow_providers_grpc-3.5.0rc2/airflow/providers/grpc/LICENSE
+-rw-r--r--   0        0        0     1579 2024-04-30 11:28:59.000000 apache_airflow_providers_grpc-3.5.0rc2/airflow/providers/grpc/__init__.py
+-rw-r--r--   0        0        0     2407 2024-04-30 11:28:59.000000 apache_airflow_providers_grpc-3.5.0rc2/airflow/providers/grpc/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:28:59.000000 apache_airflow_providers_grpc-3.5.0rc2/airflow/providers/grpc/hooks/__init__.py
+-rw-r--r--   0        0        0     6852 2024-04-30 11:28:59.000000 apache_airflow_providers_grpc-3.5.0rc2/airflow/providers/grpc/hooks/grpc.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:28:59.000000 apache_airflow_providers_grpc-3.5.0rc2/airflow/providers/grpc/operators/__init__.py
+-rw-r--r--   0        0        0     3800 2024-04-30 11:28:59.000000 apache_airflow_providers_grpc-3.5.0rc2/airflow/providers/grpc/operators/grpc.py
+-rw-r--r--   0        0        0     3018 2024-04-30 11:28:59.000000 apache_airflow_providers_grpc-3.5.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     4916 1970-01-01 00:00:00.000000 apache_airflow_providers_grpc-3.5.0rc2/PKG-INFO
```

### Comparing `apache_airflow_providers_grpc-3.5.0rc1/README.rst` & `apache_airflow_providers_grpc-3.5.0rc2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-grpc``
 
-Release: ``3.5.0.rc1``
+Release: ``3.5.0.rc2``
 
 
 `gRPC <https://grpc.io/>`__
 
 
 Provider package
 ----------------
@@ -60,23 +60,23 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-grpc``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ========================  ==================
 PIP package               Version required
 ========================  ==================
-``apache-airflow``        ``>=2.6.0``
+``apache-airflow``        ``>=2.7.0``
 ``google-auth``           ``>=1.0.0,<3.0.0``
 ``google-auth-httplib2``  ``>=0.0.1``
 ``grpcio``                ``>=1.15.0``
 ========================  ==================
 
 The changelog for the provider package can be found in the
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-grpc/3.5.0/changelog.html>`_.
```

### Comparing `apache_airflow_providers_grpc-3.5.0rc1/airflow/providers/grpc/LICENSE` & `apache_airflow_providers_grpc-3.5.0rc2/airflow/providers/grpc/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_grpc-3.5.0rc1/airflow/providers/grpc/__init__.py` & `apache_airflow_providers_grpc-3.5.0rc2/airflow/providers/grpc/__init__.py`

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
-        f"The package `apache-airflow-providers-grpc:{__version__}` needs Apache Airflow 2.6.0+"
+        f"The package `apache-airflow-providers-grpc:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_grpc-3.5.0rc1/airflow/providers/grpc/get_provider_info.py` & `apache_airflow_providers_grpc-3.5.0rc2/airflow/providers/grpc/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-grpc",
         "name": "gRPC",
         "description": "`gRPC <https://grpc.io/>`__\n",
         "state": "ready",
-        "source-date-epoch": 1705912113,
+        "source-date-epoch": 1714476539,
         "versions": [
             "3.5.0",
             "3.4.1",
             "3.4.0",
             "3.3.0",
             "3.2.2",
             "3.2.1",
@@ -45,15 +45,15 @@
             "2.0.1",
             "2.0.0",
             "1.1.0",
             "1.0.1",
             "1.0.0",
         ],
         "dependencies": [
-            "apache-airflow>=2.6.0",
+            "apache-airflow>=2.7.0",
             "google-auth>=1.0.0, <3.0.0",
             "google-auth-httplib2>=0.0.1",
             "grpcio>=1.15.0",
         ],
         "integrations": [
             {"integration-name": "gRPC", "external-doc-url": "https://grpc.io/", "tags": ["protocol"]}
         ],
```

### Comparing `apache_airflow_providers_grpc-3.5.0rc1/airflow/providers/grpc/hooks/__init__.py` & `apache_airflow_providers_grpc-3.5.0rc2/airflow/providers/grpc/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_grpc-3.5.0rc1/airflow/providers/grpc/hooks/grpc.py` & `apache_airflow_providers_grpc-3.5.0rc2/airflow/providers/grpc/hooks/grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """GRPC Hook."""
+
 from __future__ import annotations
 
 from typing import Any, Callable, Generator
 
 import grpc
 from google import auth as google_auth
 from google.auth import jwt as google_auth_jwt  # type: ignore[attr-defined]
@@ -49,15 +50,15 @@
     conn_name_attr = "grpc_conn_id"
     default_conn_name = "grpc_default"
     conn_type = "grpc"
     hook_name = "GRPC Connection"
 
     @classmethod
     def get_connection_form_widgets(cls) -> dict[str, Any]:
-        """Returns connection widgets to add to connection form."""
+        """Return connection widgets to add to GRPC connection form."""
         from flask_appbuilder.fieldwidgets import BS3TextFieldWidget
         from flask_babel import lazy_gettext
         from wtforms import StringField
 
         return {
             "auth_type": StringField(lazy_gettext("Grpc Auth Type"), widget=BS3TextFieldWidget()),
             "credential_pem_file": StringField(
@@ -67,17 +68,16 @@
         }
 
     def __init__(
         self,
         grpc_conn_id: str = default_conn_name,
         interceptors: list[Callable] | None = None,
         custom_connection_func: Callable | None = None,
-        **kwargs,
     ) -> None:
-        super().__init__(**kwargs)
+        super().__init__()
         self.grpc_conn_id = grpc_conn_id
         self.conn = self.get_connection(self.grpc_conn_id)
         self.extras = self.conn.extra_dejson
         self.interceptors = interceptors or []
         self.custom_connection_func = custom_connection_func
 
     def get_conn(self) -> grpc.Channel:
```

### Comparing `apache_airflow_providers_grpc-3.5.0rc1/airflow/providers/grpc/operators/__init__.py` & `apache_airflow_providers_grpc-3.5.0rc2/airflow/providers/grpc/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_grpc-3.5.0rc1/airflow/providers/grpc/operators/grpc.py` & `apache_airflow_providers_grpc-3.5.0rc2/airflow/providers/grpc/operators/grpc.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_grpc-3.5.0rc1/pyproject.toml` & `apache_airflow_providers_grpc-3.5.0rc2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-grpc"
-version = "3.5.0.rc1"
+version = "3.5.0.rc2"
 description = "Provider package apache-airflow-providers-grpc for Apache Airflow"
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
     "google-auth-httplib2>=0.0.1",
     "google-auth>=1.0.0, <3.0.0",
     "grpcio>=1.15.0",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-grpc/3.5.0"
```

### Comparing `apache_airflow_providers_grpc-3.5.0rc1/PKG-INFO` & `apache_airflow_providers_grpc-3.5.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-grpc
-Version: 3.5.0rc1
+Version: 3.5.0rc2
 Summary: Provider package apache-airflow-providers-grpc for Apache Airflow
 Keywords: airflow-provider,grpc,airflow,integration
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
 Requires-Dist: google-auth-httplib2>=0.0.1
 Requires-Dist: google-auth>=1.0.0, <3.0.0
 Requires-Dist: grpcio>=1.15.0
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-grpc/3.5.0/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-grpc/3.5.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
@@ -72,15 +73,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-grpc``
 
-Release: ``3.5.0.rc1``
+Release: ``3.5.0.rc2``
 
 
 `gRPC <https://grpc.io/>`__
 
 
 Provider package
 ----------------
@@ -94,23 +95,23 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-grpc``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ========================  ==================
 PIP package               Version required
 ========================  ==================
-``apache-airflow``        ``>=2.6.0``
+``apache-airflow``        ``>=2.7.0``
 ``google-auth``           ``>=1.0.0,<3.0.0``
 ``google-auth-httplib2``  ``>=0.0.1``
 ``grpcio``                ``>=1.15.0``
 ========================  ==================
 
 The changelog for the provider package can be found in the
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-grpc/3.5.0/changelog.html>`_.
```

