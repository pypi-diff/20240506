# Comparing `tmp/apache_airflow_providers_tableau-4.5.0rc1.tar.gz` & `tmp/apache_airflow_providers_tableau-4.5.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_tableau-4.5.0rc1.tar", last modified: Mon Jan 22 08:31:30 2024, max compression
+gzip compressed data, was "apache_airflow_providers_tableau-4.5.0rc2.tar", last modified: Tue Apr 30 11:47:22 2024, max compression
```

## Comparing `apache_airflow_providers_tableau-4.5.0rc1.tar` & `apache_airflow_providers_tableau-4.5.0rc2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     3072 2024-01-22 08:31:30.000000 apache_airflow_providers_tableau-4.5.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-01-22 08:31:30.000000 apache_airflow_providers_tableau-4.5.0rc1/airflow/providers/tableau/LICENSE
--rw-r--r--   0        0        0     1582 2024-01-22 08:31:30.000000 apache_airflow_providers_tableau-4.5.0rc1/airflow/providers/tableau/__init__.py
--rw-r--r--   0        0        0     2862 2024-01-22 08:31:30.000000 apache_airflow_providers_tableau-4.5.0rc1/airflow/providers/tableau/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-01-22 08:31:30.000000 apache_airflow_providers_tableau-4.5.0rc1/airflow/providers/tableau/hooks/__init__.py
--rw-r--r--   0        0        0     7158 2024-01-22 08:31:30.000000 apache_airflow_providers_tableau-4.5.0rc1/airflow/providers/tableau/hooks/tableau.py
--rw-r--r--   0        0        0      785 2024-01-22 08:31:30.000000 apache_airflow_providers_tableau-4.5.0rc1/airflow/providers/tableau/operators/__init__.py
--rw-r--r--   0        0        0     5414 2024-01-22 08:31:30.000000 apache_airflow_providers_tableau-4.5.0rc1/airflow/providers/tableau/operators/tableau.py
--rw-r--r--   0        0        0      785 2024-01-22 08:31:30.000000 apache_airflow_providers_tableau-4.5.0rc1/airflow/providers/tableau/sensors/__init__.py
--rw-r--r--   0        0        0     2976 2024-01-22 08:31:30.000000 apache_airflow_providers_tableau-4.5.0rc1/airflow/providers/tableau/sensors/tableau.py
--rw-r--r--   0        0        0     2931 2024-01-22 08:31:30.000000 apache_airflow_providers_tableau-4.5.0rc1/pyproject.toml
--rw-r--r--   0        0        0     4723 1970-01-01 00:00:00.000000 apache_airflow_providers_tableau-4.5.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     3077 2024-04-30 11:47:22.000000 apache_airflow_providers_tableau-4.5.0rc2/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-30 11:47:22.000000 apache_airflow_providers_tableau-4.5.0rc2/airflow/providers/tableau/LICENSE
+-rw-r--r--   0        0        0     1582 2024-04-30 11:47:22.000000 apache_airflow_providers_tableau-4.5.0rc2/airflow/providers/tableau/__init__.py
+-rw-r--r--   0        0        0     2904 2024-04-30 11:47:22.000000 apache_airflow_providers_tableau-4.5.0rc2/airflow/providers/tableau/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:47:22.000000 apache_airflow_providers_tableau-4.5.0rc2/airflow/providers/tableau/hooks/__init__.py
+-rw-r--r--   0        0        0     7199 2024-04-30 11:47:22.000000 apache_airflow_providers_tableau-4.5.0rc2/airflow/providers/tableau/hooks/tableau.py
+-rw-r--r--   0        0        0      785 2024-04-30 11:47:22.000000 apache_airflow_providers_tableau-4.5.0rc2/airflow/providers/tableau/operators/__init__.py
+-rw-r--r--   0        0        0     5411 2024-04-30 11:47:22.000000 apache_airflow_providers_tableau-4.5.0rc2/airflow/providers/tableau/operators/tableau.py
+-rw-r--r--   0        0        0      785 2024-04-30 11:47:22.000000 apache_airflow_providers_tableau-4.5.0rc2/airflow/providers/tableau/sensors/__init__.py
+-rw-r--r--   0        0        0     2976 2024-04-30 11:47:22.000000 apache_airflow_providers_tableau-4.5.0rc2/airflow/providers/tableau/sensors/tableau.py
+-rw-r--r--   0        0        0     2975 2024-04-30 11:47:22.000000 apache_airflow_providers_tableau-4.5.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     4777 1970-01-01 00:00:00.000000 apache_airflow_providers_tableau-4.5.0rc2/PKG-INFO
```

### Comparing `apache_airflow_providers_tableau-4.5.0rc1/README.rst` & `apache_airflow_providers_tableau-4.5.0rc2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-tableau``
 
-Release: ``4.5.0.rc1``
+Release: ``4.5.0.rc2``
 
 
 `Tableau <https://www.tableau.com/>`__
 
 
 Provider package
 ----------------
@@ -60,21 +60,21 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-tableau``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 =======================  ==================
 PIP package              Version required
 =======================  ==================
-``apache-airflow``       ``>=2.6.0``
+``apache-airflow``       ``>=2.7.0``
 ``tableauserverclient``
 =======================  ==================
 
 The changelog for the provider package can be found in the
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-tableau/4.5.0/changelog.html>`_.
```

### Comparing `apache_airflow_providers_tableau-4.5.0rc1/airflow/providers/tableau/LICENSE` & `apache_airflow_providers_tableau-4.5.0rc2/airflow/providers/tableau/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_tableau-4.5.0rc1/airflow/providers/tableau/__init__.py` & `apache_airflow_providers_tableau-4.5.0rc2/airflow/providers/tableau/__init__.py`

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
-        f"The package `apache-airflow-providers-tableau:{__version__}` needs Apache Airflow 2.6.0+"
+        f"The package `apache-airflow-providers-tableau:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_tableau-4.5.0rc1/airflow/providers/tableau/get_provider_info.py` & `apache_airflow_providers_tableau-4.5.0rc2/airflow/providers/tableau/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,19 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-tableau",
         "name": "Tableau",
         "description": "`Tableau <https://www.tableau.com/>`__\n",
         "state": "ready",
-        "source-date-epoch": 1705912290,
+        "source-date-epoch": 1714477642,
         "versions": [
             "4.5.0",
+            "4.4.2",
+            "4.4.1",
             "4.4.0",
             "4.3.0",
             "4.2.2",
             "4.2.1",
             "4.2.0",
             "4.1.0",
             "4.0.0",
@@ -48,15 +50,15 @@
             "2.1.3",
             "2.1.2",
             "2.1.1",
             "2.1.0",
             "2.0.0",
             "1.0.0",
         ],
-        "dependencies": ["apache-airflow>=2.6.0", "tableauserverclient"],
+        "dependencies": ["apache-airflow>=2.7.0", "tableauserverclient"],
         "integrations": [
             {
                 "integration-name": "Tableau",
                 "external-doc-url": "https://www.tableau.com/",
                 "how-to-guide": ["/docs/apache-airflow-providers-tableau/operators.rst"],
                 "logo": "/integration-logos/tableau/tableau.png",
                 "tags": ["service"],
```

### Comparing `apache_airflow_providers_tableau-4.5.0rc1/airflow/providers/tableau/hooks/__init__.py` & `apache_airflow_providers_tableau-4.5.0rc2/airflow/providers/tableau/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_tableau-4.5.0rc1/airflow/providers/tableau/hooks/tableau.py` & `apache_airflow_providers_tableau-4.5.0rc2/airflow/providers/tableau/hooks/tableau.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import time
-import warnings
 from enum import Enum
 from typing import TYPE_CHECKING, Any
 
+from deprecated import deprecated
 from tableauserverclient import Pager, PersonalAccessTokenAuth, Server, TableauAuth
 
 from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.hooks.base import BaseHook
 
 if TYPE_CHECKING:
     from tableauserverclient.server import Auth
@@ -76,18 +76,16 @@
     """
 
     conn_name_attr = "tableau_conn_id"
     default_conn_name = "tableau_default"
     conn_type = "tableau"
     hook_name = "Tableau"
 
-    def __init__(
-        self, site_id: str | None = None, tableau_conn_id: str = default_conn_name, **kwargs
-    ) -> None:
-        super().__init__(**kwargs)
+    def __init__(self, site_id: str | None = None, tableau_conn_id: str = default_conn_name) -> None:
+        super().__init__()
         self.tableau_conn_id = tableau_conn_id
         self.conn = self.get_connection(self.tableau_conn_id)
         self.site_id = site_id or self.conn.extra_dejson.get("site_id", "")
         self.server = Server(self.conn.host)
         verify: Any = self.conn.extra_dejson.get("verify", True)
         if isinstance(verify, str):
             verify = parse_boolean(verify)
@@ -119,22 +117,26 @@
 
     def _auth_via_password(self) -> Auth.contextmgr:
         tableau_auth = TableauAuth(
             username=self.conn.login, password=self.conn.password, site_id=self.site_id
         )
         return self.server.auth.sign_in(tableau_auth)
 
-    def _auth_via_token(self) -> Auth.contextmgr:
-        """The method is deprecated. Please, use the authentication via password instead."""
-        warnings.warn(
+    @deprecated(
+        reason=(
             "Authentication via personal access token is deprecated. "
-            "Please, use the password authentication to avoid inconsistencies.",
-            AirflowProviderDeprecationWarning,
-            stacklevel=2,
-        )
+            "Please, use the password authentication to avoid inconsistencies."
+        ),
+        category=AirflowProviderDeprecationWarning,
+    )
+    def _auth_via_token(self) -> Auth.contextmgr:
+        """Authenticate via personal access token.
+
+        This method is deprecated. Please, use the authentication via password instead.
+        """
         tableau_auth = PersonalAccessTokenAuth(
             token_name=self.conn.extra_dejson["token_name"],
             personal_access_token=self.conn.extra_dejson["personal_access_token"],
             site_id=self.site_id,
         )
         return self.server.auth.sign_in_with_personal_access_token(tableau_auth)
```

### Comparing `apache_airflow_providers_tableau-4.5.0rc1/airflow/providers/tableau/operators/__init__.py` & `apache_airflow_providers_tableau-4.5.0rc2/airflow/providers/tableau/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_tableau-4.5.0rc1/airflow/providers/tableau/operators/tableau.py` & `apache_airflow_providers_tableau-4.5.0rc2/airflow/providers/tableau/operators/tableau.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         self.check_interval = check_interval
         self.site_id = site_id
         self.blocking_refresh = blocking_refresh
         self.tableau_conn_id = tableau_conn_id
 
     def execute(self, context: Context) -> str:
         """
-        Executes the Tableau API resource and pushes the job id or downloaded file URI to xcom.
+        Execute the Tableau API resource and push the job id or downloaded file URI to xcom.
 
         :param context: The task context during execution.
         :return: the id of the job that executes the extract refresh or downloaded file URI.
         """
         available_resources = RESOURCES_METHODS.keys()
         if self.resource not in available_resources:
             error_message = f"Resource not found! Available Resources: {available_resources}"
```

### Comparing `apache_airflow_providers_tableau-4.5.0rc1/airflow/providers/tableau/sensors/__init__.py` & `apache_airflow_providers_tableau-4.5.0rc2/airflow/providers/tableau/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_tableau-4.5.0rc1/airflow/providers/tableau/sensors/tableau.py` & `apache_airflow_providers_tableau-4.5.0rc2/airflow/providers/tableau/sensors/tableau.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_tableau-4.5.0rc1/pyproject.toml` & `apache_airflow_providers_tableau-4.5.0rc2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-tableau"
-version = "4.5.0.rc1"
+version = "4.5.0.rc2"
 description = "Provider package apache-airflow-providers-tableau for Apache Airflow"
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
     "tableauserverclient",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-tableau/4.5.0"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-tableau/4.5.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
```

### Comparing `apache_airflow_providers_tableau-4.5.0rc1/PKG-INFO` & `apache_airflow_providers_tableau-4.5.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-tableau
-Version: 4.5.0rc1
+Version: 4.5.0rc2
 Summary: Provider package apache-airflow-providers-tableau for Apache Airflow
 Keywords: airflow-provider,tableau,airflow,integration
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
 Requires-Dist: tableauserverclient
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-tableau/4.5.0/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-tableau/4.5.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
@@ -70,15 +71,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-tableau``
 
-Release: ``4.5.0.rc1``
+Release: ``4.5.0.rc2``
 
 
 `Tableau <https://www.tableau.com/>`__
 
 
 Provider package
 ----------------
@@ -92,21 +93,21 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-tableau``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 =======================  ==================
 PIP package              Version required
 =======================  ==================
-``apache-airflow``       ``>=2.6.0``
+``apache-airflow``       ``>=2.7.0``
 ``tableauserverclient``
 =======================  ==================
 
 The changelog for the provider package can be found in the
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-tableau/4.5.0/changelog.html>`_.
```

