# Comparing `tmp/apache_airflow_providers_salesforce-5.7.0rc1.tar.gz` & `tmp/apache_airflow_providers_salesforce-5.7.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_salesforce-5.7.0rc1.tar", last modified: Mon Jan 22 08:30:38 2024, max compression
+gzip compressed data, was "apache_airflow_providers_salesforce-5.7.0rc2.tar", last modified: Tue Apr 30 11:43:28 2024, max compression
```

## Comparing `apache_airflow_providers_salesforce-5.7.0rc1.tar` & `apache_airflow_providers_salesforce-5.7.0rc2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     3132 2024-01-22 08:30:38.000000 apache_airflow_providers_salesforce-5.7.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-01-22 08:30:38.000000 apache_airflow_providers_salesforce-5.7.0rc1/airflow/providers/salesforce/LICENSE
--rw-r--r--   0        0        0     1585 2024-01-22 08:30:38.000000 apache_airflow_providers_salesforce-5.7.0rc1/airflow/providers/salesforce/__init__.py
--rw-r--r--   0        0        0     3259 2024-01-22 08:30:38.000000 apache_airflow_providers_salesforce-5.7.0rc1/airflow/providers/salesforce/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-01-22 08:30:38.000000 apache_airflow_providers_salesforce-5.7.0rc1/airflow/providers/salesforce/hooks/__init__.py
--rw-r--r--   0        0        0    18149 2024-01-22 08:30:38.000000 apache_airflow_providers_salesforce-5.7.0rc1/airflow/providers/salesforce/hooks/salesforce.py
--rw-r--r--   0        0        0      785 2024-01-22 08:30:38.000000 apache_airflow_providers_salesforce-5.7.0rc1/airflow/providers/salesforce/operators/__init__.py
--rw-r--r--   0        0        0     4763 2024-01-22 08:30:38.000000 apache_airflow_providers_salesforce-5.7.0rc1/airflow/providers/salesforce/operators/bulk.py
--rw-r--r--   0        0        0     2555 2024-01-22 08:30:38.000000 apache_airflow_providers_salesforce-5.7.0rc1/airflow/providers/salesforce/operators/salesforce_apex_rest.py
--rw-r--r--   0        0        0     2978 2024-01-22 08:30:38.000000 apache_airflow_providers_salesforce-5.7.0rc1/pyproject.toml
--rw-r--r--   0        0        0     4832 1970-01-01 00:00:00.000000 apache_airflow_providers_salesforce-5.7.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     3142 2024-04-30 11:43:28.000000 apache_airflow_providers_salesforce-5.7.0rc2/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-30 11:43:28.000000 apache_airflow_providers_salesforce-5.7.0rc2/airflow/providers/salesforce/LICENSE
+-rw-r--r--   0        0        0     1585 2024-04-30 11:43:28.000000 apache_airflow_providers_salesforce-5.7.0rc2/airflow/providers/salesforce/__init__.py
+-rw-r--r--   0        0        0     3306 2024-04-30 11:43:28.000000 apache_airflow_providers_salesforce-5.7.0rc2/airflow/providers/salesforce/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:43:28.000000 apache_airflow_providers_salesforce-5.7.0rc2/airflow/providers/salesforce/hooks/__init__.py
+-rw-r--r--   0        0        0    18220 2024-04-30 11:43:28.000000 apache_airflow_providers_salesforce-5.7.0rc2/airflow/providers/salesforce/hooks/salesforce.py
+-rw-r--r--   0        0        0      785 2024-04-30 11:43:28.000000 apache_airflow_providers_salesforce-5.7.0rc2/airflow/providers/salesforce/operators/__init__.py
+-rw-r--r--   0        0        0     4894 2024-04-30 11:43:28.000000 apache_airflow_providers_salesforce-5.7.0rc2/airflow/providers/salesforce/operators/bulk.py
+-rw-r--r--   0        0        0     2554 2024-04-30 11:43:28.000000 apache_airflow_providers_salesforce-5.7.0rc2/airflow/providers/salesforce/operators/salesforce_apex_rest.py
+-rw-r--r--   0        0        0     3027 2024-04-30 11:43:28.000000 apache_airflow_providers_salesforce-5.7.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     4896 1970-01-01 00:00:00.000000 apache_airflow_providers_salesforce-5.7.0rc2/PKG-INFO
```

### Comparing `apache_airflow_providers_salesforce-5.7.0rc1/README.rst` & `apache_airflow_providers_salesforce-5.7.0rc2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-salesforce``
 
-Release: ``5.7.0.rc1``
+Release: ``5.7.0.rc2``
 
 
 `Salesforce <https://www.salesforce.com/>`__
 
 
 Provider package
 ----------------
@@ -60,22 +60,22 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-salesforce``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 =====================  ==================
 PIP package            Version required
 =====================  ==================
-``apache-airflow``     ``>=2.6.0``
+``apache-airflow``     ``>=2.7.0``
 ``simple-salesforce``  ``>=1.0.0``
-``pandas``             ``>=1.2.5``
+``pandas``             ``>=1.2.5,<2.2``
 =====================  ==================
 
 The changelog for the provider package can be found in the
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.7.0/changelog.html>`_.
```

### Comparing `apache_airflow_providers_salesforce-5.7.0rc1/airflow/providers/salesforce/LICENSE` & `apache_airflow_providers_salesforce-5.7.0rc2/airflow/providers/salesforce/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_salesforce-5.7.0rc1/airflow/providers/salesforce/__init__.py` & `apache_airflow_providers_salesforce-5.7.0rc2/airflow/providers/salesforce/__init__.py`

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
-        f"The package `apache-airflow-providers-salesforce:{__version__}` needs Apache Airflow 2.6.0+"
+        f"The package `apache-airflow-providers-salesforce:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_salesforce-5.7.0rc1/airflow/providers/salesforce/get_provider_info.py` & `apache_airflow_providers_salesforce-5.7.0rc2/airflow/providers/salesforce/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,19 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-salesforce",
         "name": "Salesforce",
         "description": "`Salesforce <https://www.salesforce.com/>`__\n",
         "state": "ready",
-        "source-date-epoch": 1705912238,
+        "source-date-epoch": 1714477408,
         "versions": [
             "5.7.0",
+            "5.6.3",
+            "5.6.2",
             "5.6.1",
             "5.6.0",
             "5.5.1",
             "5.5.0",
             "5.4.3",
             "5.4.2",
             "5.4.1",
@@ -53,15 +55,15 @@
             "3.2.0",
             "3.1.0",
             "3.0.0",
             "2.0.0",
             "1.0.1",
             "1.0.0",
         ],
-        "dependencies": ["apache-airflow>=2.6.0", "simple-salesforce>=1.0.0", "pandas>=1.2.5"],
+        "dependencies": ["apache-airflow>=2.7.0", "simple-salesforce>=1.0.0", "pandas>=1.2.5,<2.2"],
         "integrations": [
             {
                 "integration-name": "Salesforce",
                 "external-doc-url": "https://www.salesforce.com/",
                 "how-to-guide": [
                     "/docs/apache-airflow-providers-salesforce/operators/salesforce_apex_rest.rst",
                     "/docs/apache-airflow-providers-salesforce/operators/bulk.rst",
```

### Comparing `apache_airflow_providers_salesforce-5.7.0rc1/airflow/providers/salesforce/hooks/__init__.py` & `apache_airflow_providers_salesforce-5.7.0rc2/airflow/providers/salesforce/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_salesforce-5.7.0rc1/airflow/providers/salesforce/hooks/salesforce.py` & `apache_airflow_providers_salesforce-5.7.0rc2/airflow/providers/salesforce/hooks/salesforce.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,28 +17,30 @@
 # under the License.
 """
 Connect to your Salesforce instance, retrieve data from it, and write that data to a file for other uses.
 
 .. note:: this hook also relies on the simple_salesforce package:
       https://github.com/simple-salesforce/simple-salesforce
 """
+
 from __future__ import annotations
 
 import logging
 import time
 from functools import cached_property
-from typing import TYPE_CHECKING, Any, Iterable
+from typing import TYPE_CHECKING, Any, Iterable, cast
 
 from simple_salesforce import Salesforce, api
 
 from airflow.hooks.base import BaseHook
 
 if TYPE_CHECKING:
     import pandas as pd
     from requests import Session
+    from simple_salesforce.api import SFType
 
 log = logging.getLogger(__name__)
 
 
 class SalesforceHook(BaseHook):
     """
     Creates new connection to Salesforce and allows you to pull data out of SFDC and save it to a file.
@@ -68,17 +70,16 @@
     hook_name = "Salesforce"
 
     def __init__(
         self,
         salesforce_conn_id: str = default_conn_name,
         session_id: str | None = None,
         session: Session | None = None,
-        **kwargs,
     ) -> None:
-        super().__init__(**kwargs)
+        super().__init__()
         self.conn_id = salesforce_conn_id
         self.session_id = session_id
         self.session = session
 
     def _get_field(self, extras: dict, field_name: str):
         """Get field from extra, first checking short name, then for backcompat we check for prefixed name."""
         backcompat_prefix = "extra__salesforce__"
@@ -90,15 +91,15 @@
         if field_name in extras:
             return extras[field_name] or None
         prefixed_name = f"{backcompat_prefix}{field_name}"
         return extras.get(prefixed_name) or None
 
     @classmethod
     def get_connection_form_widgets(cls) -> dict[str, Any]:
-        """Returns connection widgets to add to connection form."""
+        """Return connection widgets to add to connection form."""
         from flask_appbuilder.fieldwidgets import BS3PasswordFieldWidget, BS3TextFieldWidget
         from flask_babel import lazy_gettext
         from wtforms import PasswordField, StringField
 
         return {
             "security_token": PasswordField(lazy_gettext("Security Token"), widget=BS3PasswordFieldWidget()),
             "domain": StringField(lazy_gettext("Domain"), widget=BS3TextFieldWidget()),
@@ -113,15 +114,15 @@
             "proxies": StringField(lazy_gettext("Proxies"), widget=BS3TextFieldWidget()),
             "version": StringField(lazy_gettext("API Version"), widget=BS3TextFieldWidget()),
             "client_id": StringField(lazy_gettext("Client ID"), widget=BS3TextFieldWidget()),
         }
 
     @classmethod
     def get_ui_field_behaviour(cls) -> dict[str, Any]:
-        """Returns custom field behaviour."""
+        """Return custom field behaviour."""
         return {
             "hidden_fields": ["schema", "port", "extra", "host"],
             "relabeling": {
                 "login": "Username",
             },
         }
 
@@ -151,15 +152,15 @@
             consumer_key=self._get_field(extras, "consumer_key") or None,
             privatekey_file=self._get_field(extras, "private_key_file_path") or None,
             privatekey=self._get_field(extras, "private_key") or None,
         )
         return conn
 
     def get_conn(self) -> api.Salesforce:
-        """Returns a Salesforce instance. (cached)."""
+        """Return a Salesforce instance. (cached)."""
         return self.conn
 
     def make_query(self, query: str, include_deleted: bool = False, query_params: dict | None = None) -> dict:
         """
         Make a query to Salesforce.
 
         :param query: The query to make to Salesforce.
@@ -186,16 +187,17 @@
         This description is the object's schema and
         some extra metadata that Salesforce stores for each object.
 
         :param obj: The name of the Salesforce object that we are getting a description of.
         :return: the description of the Salesforce object.
         """
         conn = self.get_conn()
+        sftype: SFType = cast("SFType", conn.__getattr__(obj))
 
-        return conn.__getattr__(obj).describe()
+        return sftype.describe()
 
     def get_available_fields(self, obj: str) -> list[str]:
         """
         Get a list of all available fields for an object.
 
         :param obj: The name of the Salesforce object that we are getting a description of.
         :return: the names of the fields.
```

### Comparing `apache_airflow_providers_salesforce-5.7.0rc1/airflow/providers/salesforce/operators/__init__.py` & `apache_airflow_providers_salesforce-5.7.0rc2/airflow/providers/salesforce/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_salesforce-5.7.0rc1/airflow/providers/salesforce/operators/bulk.py` & `apache_airflow_providers_salesforce-5.7.0rc2/airflow/providers/salesforce/operators/bulk.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,20 +12,21 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Iterable, cast
 
 from airflow.models import BaseOperator
 from airflow.providers.salesforce.hooks.salesforce import SalesforceHook
 
 if TYPE_CHECKING:
+    from simple_salesforce.bulk import SFBulkHandler
     from typing_extensions import Literal
 
     from airflow.utils.context import Context
 
 
 class SalesforceBulkOperator(BaseOperator):
     """
@@ -77,44 +78,45 @@
             raise ValueError(
                 f"Operation {self.operation!r} not found! "
                 f"Available operations are {self.available_operations}."
             )
 
     def execute(self, context: Context):
         """
-        Makes an HTTP request to Salesforce Bulk API.
+        Make an HTTP request to Salesforce Bulk API.
 
         :param context: The task context during execution.
         :return: API response if do_xcom_push is True
         """
         sf_hook = SalesforceHook(salesforce_conn_id=self.salesforce_conn_id)
         conn = sf_hook.get_conn()
+        bulk: SFBulkHandler = cast("SFBulkHandler", conn.__getattr__("bulk"))
 
-        result = []
+        result: Iterable = []
         if self.operation == "insert":
-            result = conn.bulk.__getattr__(self.object_name).insert(
+            result = bulk.__getattr__(self.object_name).insert(
                 data=self.payload, batch_size=self.batch_size, use_serial=self.use_serial
             )
         elif self.operation == "update":
-            result = conn.bulk.__getattr__(self.object_name).update(
+            result = bulk.__getattr__(self.object_name).update(
                 data=self.payload, batch_size=self.batch_size, use_serial=self.use_serial
             )
         elif self.operation == "upsert":
-            result = conn.bulk.__getattr__(self.object_name).upsert(
+            result = bulk.__getattr__(self.object_name).upsert(
                 data=self.payload,
                 external_id_field=self.external_id_field,
                 batch_size=self.batch_size,
                 use_serial=self.use_serial,
             )
         elif self.operation == "delete":
-            result = conn.bulk.__getattr__(self.object_name).delete(
+            result = bulk.__getattr__(self.object_name).delete(
                 data=self.payload, batch_size=self.batch_size, use_serial=self.use_serial
             )
         elif self.operation == "hard_delete":
-            result = conn.bulk.__getattr__(self.object_name).hard_delete(
+            result = bulk.__getattr__(self.object_name).hard_delete(
                 data=self.payload, batch_size=self.batch_size, use_serial=self.use_serial
             )
 
         if self.do_xcom_push and result:
             return result
 
         return None
```

### Comparing `apache_airflow_providers_salesforce-5.7.0rc1/airflow/providers/salesforce/operators/salesforce_apex_rest.py` & `apache_airflow_providers_salesforce-5.7.0rc2/airflow/providers/salesforce/operators/salesforce_apex_rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         self.endpoint = endpoint
         self.method = method
         self.payload = payload
         self.salesforce_conn_id = salesforce_conn_id
 
     def execute(self, context: Context) -> dict:
         """
-        Makes an HTTP request to an APEX REST endpoint and pushes results to xcom.
+        Make an HTTP request to an APEX REST endpoint and pushes results to xcom.
 
         :param context: The task context during execution.
         :return: Apex response
         """
         result: dict = {}
         sf_hook = SalesforceHook(salesforce_conn_id=self.salesforce_conn_id)
         conn = sf_hook.get_conn()
```

### Comparing `apache_airflow_providers_salesforce-5.7.0rc1/pyproject.toml` & `apache_airflow_providers_salesforce-5.7.0rc2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-salesforce"
-version = "5.7.0.rc1"
+version = "5.7.0.rc2"
 description = "Provider package apache-airflow-providers-salesforce for Apache Airflow"
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
-    "pandas>=1.2.5",
+    "apache-airflow>=2.7.0rc0",
+    "pandas>=1.2.5,<2.2",
     "simple-salesforce>=1.0.0",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.7.0"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.7.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
```

### Comparing `apache_airflow_providers_salesforce-5.7.0rc1/PKG-INFO` & `apache_airflow_providers_salesforce-5.7.0rc2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-salesforce
-Version: 5.7.0rc1
+Version: 5.7.0rc2
 Summary: Provider package apache-airflow-providers-salesforce for Apache Airflow
 Keywords: airflow-provider,salesforce,airflow,integration
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
-Requires-Dist: pandas>=1.2.5
+Requires-Dist: apache-airflow>=2.7.0rc0
+Requires-Dist: pandas>=1.2.5,<2.2
 Requires-Dist: simple-salesforce>=1.0.0
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.7.0/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.7.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
@@ -71,15 +72,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-salesforce``
 
-Release: ``5.7.0.rc1``
+Release: ``5.7.0.rc2``
 
 
 `Salesforce <https://www.salesforce.com/>`__
 
 
 Provider package
 ----------------
@@ -93,22 +94,22 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-salesforce``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 =====================  ==================
 PIP package            Version required
 =====================  ==================
-``apache-airflow``     ``>=2.6.0``
+``apache-airflow``     ``>=2.7.0``
 ``simple-salesforce``  ``>=1.0.0``
-``pandas``             ``>=1.2.5``
+``pandas``             ``>=1.2.5,<2.2``
 =====================  ==================
 
 The changelog for the provider package can be found in the
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.7.0/changelog.html>`_.
```

