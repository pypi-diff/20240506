# Comparing `tmp/apache_airflow_providers_atlassian_jira-2.6.0rc1.tar.gz` & `tmp/apache_airflow_providers_atlassian_jira-2.6.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_atlassian_jira-2.6.0rc1.tar", last modified: Mon Jan 22 08:25:55 2024, max compression
+gzip compressed data, was "apache_airflow_providers_atlassian_jira-2.6.0rc2.tar", last modified: Tue Apr 30 11:19:11 2024, max compression
```

## Comparing `apache_airflow_providers_atlassian_jira-2.6.0rc1.tar` & `apache_airflow_providers_atlassian_jira-2.6.0rc2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     3194 2024-01-22 08:25:55.000000 apache_airflow_providers_atlassian_jira-2.6.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-01-22 08:25:55.000000 apache_airflow_providers_atlassian_jira-2.6.0rc1/airflow/providers/atlassian/jira/LICENSE
--rw-r--r--   0        0        0     1589 2024-01-22 08:25:55.000000 apache_airflow_providers_atlassian_jira-2.6.0rc1/airflow/providers/atlassian/jira/__init__.py
--rw-r--r--   0        0        0     2919 2024-01-22 08:25:55.000000 apache_airflow_providers_atlassian_jira-2.6.0rc1/airflow/providers/atlassian/jira/get_provider_info.py
--rw-r--r--   0        0        0      785 2024-01-22 08:25:55.000000 apache_airflow_providers_atlassian_jira-2.6.0rc1/airflow/providers/atlassian/jira/hooks/__init__.py
--rw-r--r--   0        0        0     3634 2024-01-22 08:25:55.000000 apache_airflow_providers_atlassian_jira-2.6.0rc1/airflow/providers/atlassian/jira/hooks/jira.py
--rw-r--r--   0        0        0      785 2024-01-22 08:25:55.000000 apache_airflow_providers_atlassian_jira-2.6.0rc1/airflow/providers/atlassian/jira/notifications/__init__.py
--rw-r--r--   0        0        0     2720 2024-01-22 08:25:55.000000 apache_airflow_providers_atlassian_jira-2.6.0rc1/airflow/providers/atlassian/jira/notifications/jira.py
--rw-r--r--   0        0        0      785 2024-01-22 08:25:55.000000 apache_airflow_providers_atlassian_jira-2.6.0rc1/airflow/providers/atlassian/jira/operators/__init__.py
--rw-r--r--   0        0        0     3710 2024-01-22 08:25:55.000000 apache_airflow_providers_atlassian_jira-2.6.0rc1/airflow/providers/atlassian/jira/operators/jira.py
--rw-r--r--   0        0        0      785 2024-01-22 08:25:55.000000 apache_airflow_providers_atlassian_jira-2.6.0rc1/airflow/providers/atlassian/jira/sensors/__init__.py
--rw-r--r--   0        0        0     5192 2024-01-22 08:25:55.000000 apache_airflow_providers_atlassian_jira-2.6.0rc1/airflow/providers/atlassian/jira/sensors/jira.py
--rw-r--r--   0        0        0     3020 2024-01-22 08:25:55.000000 apache_airflow_providers_atlassian_jira-2.6.0rc1/pyproject.toml
--rw-r--r--   0        0        0     4928 1970-01-01 00:00:00.000000 apache_airflow_providers_atlassian_jira-2.6.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     3199 2024-04-30 11:19:11.000000 apache_airflow_providers_atlassian_jira-2.6.0rc2/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-30 11:19:11.000000 apache_airflow_providers_atlassian_jira-2.6.0rc2/airflow/providers/atlassian/jira/LICENSE
+-rw-r--r--   0        0        0     1589 2024-04-30 11:19:11.000000 apache_airflow_providers_atlassian_jira-2.6.0rc2/airflow/providers/atlassian/jira/__init__.py
+-rw-r--r--   0        0        0     2940 2024-04-30 11:19:11.000000 apache_airflow_providers_atlassian_jira-2.6.0rc2/airflow/providers/atlassian/jira/get_provider_info.py
+-rw-r--r--   0        0        0      785 2024-04-30 11:19:11.000000 apache_airflow_providers_atlassian_jira-2.6.0rc2/airflow/providers/atlassian/jira/hooks/__init__.py
+-rw-r--r--   0        0        0     3663 2024-04-30 11:19:11.000000 apache_airflow_providers_atlassian_jira-2.6.0rc2/airflow/providers/atlassian/jira/hooks/jira.py
+-rw-r--r--   0        0        0      785 2024-04-30 11:19:11.000000 apache_airflow_providers_atlassian_jira-2.6.0rc2/airflow/providers/atlassian/jira/notifications/__init__.py
+-rw-r--r--   0        0        0     2720 2024-04-30 11:19:11.000000 apache_airflow_providers_atlassian_jira-2.6.0rc2/airflow/providers/atlassian/jira/notifications/jira.py
+-rw-r--r--   0        0        0      785 2024-04-30 11:19:11.000000 apache_airflow_providers_atlassian_jira-2.6.0rc2/airflow/providers/atlassian/jira/operators/__init__.py
+-rw-r--r--   0        0        0     3710 2024-04-30 11:19:11.000000 apache_airflow_providers_atlassian_jira-2.6.0rc2/airflow/providers/atlassian/jira/operators/jira.py
+-rw-r--r--   0        0        0      785 2024-04-30 11:19:11.000000 apache_airflow_providers_atlassian_jira-2.6.0rc2/airflow/providers/atlassian/jira/sensors/__init__.py
+-rw-r--r--   0        0        0     5192 2024-04-30 11:19:11.000000 apache_airflow_providers_atlassian_jira-2.6.0rc2/airflow/providers/atlassian/jira/sensors/jira.py
+-rw-r--r--   0        0        0     3064 2024-04-30 11:19:11.000000 apache_airflow_providers_atlassian_jira-2.6.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     4982 1970-01-01 00:00:00.000000 apache_airflow_providers_atlassian_jira-2.6.0rc2/PKG-INFO
```

### Comparing `apache_airflow_providers_atlassian_jira-2.6.0rc1/README.rst` & `apache_airflow_providers_atlassian_jira-2.6.0rc2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-atlassian-jira``
 
-Release: ``2.6.0.rc1``
+Release: ``2.6.0.rc2``
 
 
 `Atlassian Jira <https://www.atlassian.com/software/jira/>`__
 
 
 Provider package
 ----------------
@@ -60,22 +60,22 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-atlassian-jira``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ========================  =====================
 PIP package               Version required
 ========================  =====================
-``apache-airflow``        ``>=2.6.0``
+``apache-airflow``        ``>=2.7.0``
 ``atlassian-python-api``  ``>=1.14.2,!=3.41.6``
 ``beautifulsoup4``
 ========================  =====================
 
 The changelog for the provider package can be found in the
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-atlassian-jira/2.6.0/changelog.html>`_.
```

### Comparing `apache_airflow_providers_atlassian_jira-2.6.0rc1/airflow/providers/atlassian/jira/LICENSE` & `apache_airflow_providers_atlassian_jira-2.6.0rc2/airflow/providers/atlassian/jira/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_atlassian_jira-2.6.0rc1/airflow/providers/atlassian/jira/__init__.py` & `apache_airflow_providers_atlassian_jira-2.6.0rc2/airflow/providers/atlassian/jira/__init__.py`

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
-        f"The package `apache-airflow-providers-atlassian-jira:{__version__}` needs Apache Airflow 2.6.0+"
+        f"The package `apache-airflow-providers-atlassian-jira:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_atlassian_jira-2.6.0rc1/airflow/providers/atlassian/jira/get_provider_info.py` & `apache_airflow_providers_atlassian_jira-2.6.0rc2/airflow/providers/atlassian/jira/get_provider_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,29 +24,30 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-atlassian-jira",
         "name": "Atlassian Jira",
         "description": "`Atlassian Jira <https://www.atlassian.com/software/jira/>`__\n",
         "state": "ready",
-        "source-date-epoch": 1705911955,
+        "source-date-epoch": 1714475951,
         "versions": [
             "2.6.0",
+            "2.5.1",
             "2.5.0",
             "2.4.0",
             "2.3.0",
             "2.2.0",
             "2.1.1",
             "2.1.0",
             "2.0.1",
             "2.0.0",
             "1.1.0",
             "1.0.0",
         ],
-        "dependencies": ["apache-airflow>=2.6.0", "atlassian-python-api>=1.14.2,!=3.41.6", "beautifulsoup4"],
+        "dependencies": ["apache-airflow>=2.7.0", "atlassian-python-api>=1.14.2,!=3.41.6", "beautifulsoup4"],
         "integrations": [
             {
                 "integration-name": "Atlassian Jira",
                 "external-doc-url": "https://www.atlassian.com/software/jira",
                 "logo": "/integration-logos/jira/Jira.png",
                 "tags": ["software"],
             }
```

### Comparing `apache_airflow_providers_atlassian_jira-2.6.0rc1/airflow/providers/atlassian/jira/hooks/__init__.py` & `apache_airflow_providers_atlassian_jira-2.6.0rc2/airflow/providers/atlassian/jira/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_atlassian_jira-2.6.0rc1/airflow/providers/atlassian/jira/hooks/jira.py` & `apache_airflow_providers_atlassian_jira-2.6.0rc2/airflow/providers/atlassian/jira/hooks/jira.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """Hook for JIRA."""
+
 from __future__ import annotations
 
 import warnings
 from typing import Any
 
 from atlassian import Jira
 
@@ -35,16 +36,16 @@
     """
 
     default_conn_name = "jira_default"
     conn_type = "jira"
     conn_name_attr = "jira_conn_id"
     hook_name = "JIRA"
 
-    def __init__(self, jira_conn_id: str = default_conn_name, proxies: Any | None = None, **kwargs) -> None:
-        super().__init__(**kwargs)
+    def __init__(self, jira_conn_id: str = default_conn_name, proxies: Any | None = None) -> None:
+        super().__init__()
         self.jira_conn_id = jira_conn_id
         self.proxies = proxies
         self.client: Jira | None = None
         self.get_conn()
 
     def get_conn(self) -> Jira:
         if not self.client:
@@ -81,22 +82,22 @@
                 proxies=self.proxies,
             )
 
         return self.client
 
     @classmethod
     def get_connection_form_widgets(cls) -> dict[str, Any]:
-        """Returns connection widgets to add to connection form."""
+        """Return connection widgets to add to Atlassian Jira Connection form."""
         from flask_babel import lazy_gettext
         from wtforms import BooleanField
 
         return {
             "verify": BooleanField(lazy_gettext("Verify SSL"), default=True),
         }
 
     @classmethod
     def get_ui_field_behaviour(cls) -> dict[str, Any]:
-        """Returns custom field behaviour."""
+        """Return custom UI field behaviour for Atlassian Jira Connection."""
         return {
             "hidden_fields": ["schema", "extra"],
             "relabeling": {},
         }
```

### Comparing `apache_airflow_providers_atlassian_jira-2.6.0rc1/airflow/providers/atlassian/jira/notifications/__init__.py` & `apache_airflow_providers_atlassian_jira-2.6.0rc2/airflow/providers/atlassian/jira/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_atlassian_jira-2.6.0rc1/airflow/providers/atlassian/jira/notifications/jira.py` & `apache_airflow_providers_atlassian_jira-2.6.0rc2/airflow/providers/atlassian/jira/notifications/jira.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_atlassian_jira-2.6.0rc1/airflow/providers/atlassian/jira/operators/__init__.py` & `apache_airflow_providers_atlassian_jira-2.6.0rc2/airflow/providers/atlassian/jira/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_atlassian_jira-2.6.0rc1/airflow/providers/atlassian/jira/operators/jira.py` & `apache_airflow_providers_atlassian_jira-2.6.0rc2/airflow/providers/atlassian/jira/operators/jira.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_atlassian_jira-2.6.0rc1/airflow/providers/atlassian/jira/sensors/__init__.py` & `apache_airflow_providers_atlassian_jira-2.6.0rc2/airflow/providers/atlassian/jira/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_atlassian_jira-2.6.0rc1/airflow/providers/atlassian/jira/sensors/jira.py` & `apache_airflow_providers_atlassian_jira-2.6.0rc2/airflow/providers/atlassian/jira/sensors/jira.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_atlassian_jira-2.6.0rc1/pyproject.toml` & `apache_airflow_providers_atlassian_jira-2.6.0rc2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-atlassian-jira"
-version = "2.6.0.rc1"
+version = "2.6.0.rc2"
 description = "Provider package apache-airflow-providers-atlassian-jira for Apache Airflow"
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
     "atlassian-python-api>=1.14.2,!=3.41.6",
     "beautifulsoup4",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-atlassian-jira/2.6.0"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-atlassian-jira/2.6.0/changelog.html"
```

### Comparing `apache_airflow_providers_atlassian_jira-2.6.0rc1/PKG-INFO` & `apache_airflow_providers_atlassian_jira-2.6.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-atlassian-jira
-Version: 2.6.0rc1
+Version: 2.6.0rc2
 Summary: Provider package apache-airflow-providers-atlassian-jira for Apache Airflow
 Keywords: airflow-provider,atlassian.jira,airflow,integration
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
 Requires-Dist: atlassian-python-api>=1.14.2,!=3.41.6
 Requires-Dist: beautifulsoup4
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-atlassian-jira/2.6.0/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-atlassian-jira/2.6.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
@@ -71,15 +72,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-atlassian-jira``
 
-Release: ``2.6.0.rc1``
+Release: ``2.6.0.rc2``
 
 
 `Atlassian Jira <https://www.atlassian.com/software/jira/>`__
 
 
 Provider package
 ----------------
@@ -93,22 +94,22 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-atlassian-jira``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ========================  =====================
 PIP package               Version required
 ========================  =====================
-``apache-airflow``        ``>=2.6.0``
+``apache-airflow``        ``>=2.7.0``
 ``atlassian-python-api``  ``>=1.14.2,!=3.41.6``
 ``beautifulsoup4``
 ========================  =====================
 
 The changelog for the provider package can be found in the
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-atlassian-jira/2.6.0/changelog.html>`_.
```

