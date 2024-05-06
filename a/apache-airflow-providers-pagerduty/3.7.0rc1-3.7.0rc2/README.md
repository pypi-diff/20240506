# Comparing `tmp/apache_airflow_providers_pagerduty-3.7.0rc1.tar.gz` & `tmp/apache_airflow_providers_pagerduty-3.7.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_pagerduty-3.7.0rc1.tar", last modified: Mon Jan 22 08:30:10 2024, max compression
+gzip compressed data, was "apache_airflow_providers_pagerduty-3.7.0rc2.tar", last modified: Tue Apr 30 11:39:07 2024, max compression
```

## Comparing `apache_airflow_providers_pagerduty-3.7.0rc1.tar` & `apache_airflow_providers_pagerduty-3.7.0rc2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     3071 2024-01-22 08:30:10.000000 apache_airflow_providers_pagerduty-3.7.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-01-22 08:30:10.000000 apache_airflow_providers_pagerduty-3.7.0rc1/airflow/providers/pagerduty/LICENSE
--rw-r--r--   0        0        0     1584 2024-01-22 08:30:10.000000 apache_airflow_providers_pagerduty-3.7.0rc1/airflow/providers/pagerduty/__init__.py
--rw-r--r--   0        0        0     2902 2024-01-22 08:30:10.000000 apache_airflow_providers_pagerduty-3.7.0rc1/airflow/providers/pagerduty/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-01-22 08:30:10.000000 apache_airflow_providers_pagerduty-3.7.0rc1/airflow/providers/pagerduty/hooks/__init__.py
--rw-r--r--   0        0        0     7887 2024-01-22 08:30:10.000000 apache_airflow_providers_pagerduty-3.7.0rc1/airflow/providers/pagerduty/hooks/pagerduty.py
--rw-r--r--   0        0        0    12336 2024-01-22 08:30:10.000000 apache_airflow_providers_pagerduty-3.7.0rc1/airflow/providers/pagerduty/hooks/pagerduty_events.py
--rw-r--r--   0        0        0      785 2024-01-22 08:30:10.000000 apache_airflow_providers_pagerduty-3.7.0rc1/airflow/providers/pagerduty/notifications/__init__.py
--rw-r--r--   0        0        0     5108 2024-01-22 08:30:10.000000 apache_airflow_providers_pagerduty-3.7.0rc1/airflow/providers/pagerduty/notifications/pagerduty.py
--rw-r--r--   0        0        0     2940 2024-01-22 08:30:10.000000 apache_airflow_providers_pagerduty-3.7.0rc1/pyproject.toml
--rw-r--r--   0        0        0     4727 1970-01-01 00:00:00.000000 apache_airflow_providers_pagerduty-3.7.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     3076 2024-04-30 11:39:07.000000 apache_airflow_providers_pagerduty-3.7.0rc2/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-30 11:39:07.000000 apache_airflow_providers_pagerduty-3.7.0rc2/airflow/providers/pagerduty/LICENSE
+-rw-r--r--   0        0        0     1584 2024-04-30 11:39:07.000000 apache_airflow_providers_pagerduty-3.7.0rc2/airflow/providers/pagerduty/__init__.py
+-rw-r--r--   0        0        0     2944 2024-04-30 11:39:07.000000 apache_airflow_providers_pagerduty-3.7.0rc2/airflow/providers/pagerduty/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:39:07.000000 apache_airflow_providers_pagerduty-3.7.0rc2/airflow/providers/pagerduty/hooks/__init__.py
+-rw-r--r--   0        0        0     7880 2024-04-30 11:39:07.000000 apache_airflow_providers_pagerduty-3.7.0rc2/airflow/providers/pagerduty/hooks/pagerduty.py
+-rw-r--r--   0        0        0    12306 2024-04-30 11:39:07.000000 apache_airflow_providers_pagerduty-3.7.0rc2/airflow/providers/pagerduty/hooks/pagerduty_events.py
+-rw-r--r--   0        0        0      785 2024-04-30 11:39:07.000000 apache_airflow_providers_pagerduty-3.7.0rc2/airflow/providers/pagerduty/notifications/__init__.py
+-rw-r--r--   0        0        0     5033 2024-04-30 11:39:07.000000 apache_airflow_providers_pagerduty-3.7.0rc2/airflow/providers/pagerduty/notifications/pagerduty.py
+-rw-r--r--   0        0        0     2984 2024-04-30 11:39:07.000000 apache_airflow_providers_pagerduty-3.7.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     4781 1970-01-01 00:00:00.000000 apache_airflow_providers_pagerduty-3.7.0rc2/PKG-INFO
```

### Comparing `apache_airflow_providers_pagerduty-3.7.0rc1/README.rst` & `apache_airflow_providers_pagerduty-3.7.0rc2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-pagerduty``
 
-Release: ``3.7.0.rc1``
+Release: ``3.7.0.rc2``
 
 
 `Pagerduty <https://www.pagerduty.com/>`__
 
 
 Provider package
 ----------------
@@ -60,21 +60,21 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-pagerduty``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.6.0``
+``apache-airflow``  ``>=2.7.0``
 ``pdpyras``         ``>=4.1.2``
 ==================  ==================
 
 The changelog for the provider package can be found in the
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.7.0/changelog.html>`_.
```

### Comparing `apache_airflow_providers_pagerduty-3.7.0rc1/airflow/providers/pagerduty/LICENSE` & `apache_airflow_providers_pagerduty-3.7.0rc2/airflow/providers/pagerduty/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_pagerduty-3.7.0rc1/airflow/providers/pagerduty/__init__.py` & `apache_airflow_providers_pagerduty-3.7.0rc2/airflow/providers/pagerduty/__init__.py`

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
-        f"The package `apache-airflow-providers-pagerduty:{__version__}` needs Apache Airflow 2.6.0+"
+        f"The package `apache-airflow-providers-pagerduty:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_pagerduty-3.7.0rc1/airflow/providers/pagerduty/get_provider_info.py` & `apache_airflow_providers_pagerduty-3.7.0rc2/airflow/providers/pagerduty/get_provider_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,17 +24,19 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-pagerduty",
         "name": "Pagerduty",
         "description": "`Pagerduty <https://www.pagerduty.com/>`__\n",
         "state": "ready",
-        "source-date-epoch": 1705912210,
+        "source-date-epoch": 1714477147,
         "versions": [
             "3.7.0",
+            "3.6.2",
+            "3.6.1",
             "3.6.0",
             "3.5.1",
             "3.5.0",
             "3.4.0",
             "3.3.1",
             "3.3.0",
             "3.2.0",
@@ -45,15 +47,15 @@
             "2.1.1",
             "2.1.0",
             "2.0.1",
             "2.0.0",
             "1.0.1",
             "1.0.0",
         ],
-        "dependencies": ["apache-airflow>=2.6.0", "pdpyras>=4.1.2"],
+        "dependencies": ["apache-airflow>=2.7.0", "pdpyras>=4.1.2"],
         "integrations": [
             {
                 "integration-name": "Pagerduty",
                 "external-doc-url": "https://www.pagerduty.com/",
                 "logo": "/integration-logos/pagerduty/PagerDuty.png",
                 "tags": ["service"],
             }
```

### Comparing `apache_airflow_providers_pagerduty-3.7.0rc1/airflow/providers/pagerduty/hooks/__init__.py` & `apache_airflow_providers_pagerduty-3.7.0rc2/airflow/providers/pagerduty/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_pagerduty-3.7.0rc1/airflow/providers/pagerduty/hooks/pagerduty.py` & `apache_airflow_providers_pagerduty-3.7.0rc2/airflow/providers/pagerduty/hooks/pagerduty.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,20 +12,21 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """Hook for sending or receiving data from PagerDuty as well as creating PagerDuty incidents."""
+
 from __future__ import annotations
 
-import warnings
 from typing import Any
 
 import pdpyras
+from deprecated import deprecated
 
 from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.hooks.base import BaseHook
 from airflow.providers.pagerduty.hooks.pagerduty_events import PagerdutyEventsHook
 
 
 class PagerdutyHook(BaseHook):
@@ -48,41 +49,41 @@
     conn_name_attr = "pagerduty_conn_id"
     default_conn_name = "pagerduty_default"
     conn_type = "pagerduty"
     hook_name = "Pagerduty"
 
     @classmethod
     def get_ui_field_behaviour(cls) -> dict[str, Any]:
-        """Returns custom field behaviour."""
+        """Return custom field behaviour."""
         return {
             "hidden_fields": ["port", "login", "schema", "host", "extra"],
             "relabeling": {
                 "password": "Pagerduty API token",
             },
         }
 
     @classmethod
     def get_connection_form_widgets(cls) -> dict[str, Any]:
-        """Returns connection widgets to add to connection form."""
+        """Return connection widgets to add to connection form."""
         from flask_appbuilder.fieldwidgets import BS3PasswordFieldWidget
         from flask_babel import lazy_gettext
         from wtforms import PasswordField
         from wtforms.validators import Optional
 
         return {
             "routing_key": PasswordField(
                 lazy_gettext("Routing Key"),
                 widget=BS3PasswordFieldWidget(),
                 validators=[Optional()],
                 default=None,
             ),
         }
 
-    def __init__(self, token: str | None = None, pagerduty_conn_id: str | None = None, **kwargs) -> None:
-        super().__init__(**kwargs)
+    def __init__(self, token: str | None = None, pagerduty_conn_id: str | None = None) -> None:
+        super().__init__()
         self.routing_key = None
         self._session = None
 
         if pagerduty_conn_id is not None:
             conn = self.get_connection(pagerduty_conn_id)
             self.token = conn.get_password()
 
@@ -94,25 +95,32 @@
             self.token = token
 
         if self.token is None:
             raise AirflowException("Cannot get token: No valid api token nor pagerduty_conn_id supplied.")
 
     def get_session(self) -> pdpyras.APISession:
         """
-        Returns `pdpyras.APISession` for use with sending or receiving data through the PagerDuty REST API.
+        Return `pdpyras.APISession` for use with sending or receiving data through the PagerDuty REST API.
 
         The `pdpyras` library supplies a class `pdpyras.APISession` extending `requests.Session` from the
         Requests HTTP library.
 
         Documentation on how to use the `APISession` class can be found at:
         https://pagerduty.github.io/pdpyras/#data-access-abstraction
         """
         self._session = pdpyras.APISession(self.token)
         return self._session
 
+    @deprecated(
+        reason=(
+            "This method will be deprecated. Please use the "
+            "`airflow.providers.pagerduty.hooks.PagerdutyEventsHook` to interact with the Events API"
+        ),
+        category=AirflowProviderDeprecationWarning,
+    )
     def create_event(
         self,
         summary: str,
         severity: str,
         source: str = "airflow",
         action: str = "trigger",
         routing_key: str | None = None,
@@ -150,21 +158,14 @@
             `alt`: [Optional] Alternative text for the image.
         :param links: List of links to include. Each dictionary in the list accepts the following keys:
             `href`: URL of the link to be attached.
             `text`: [Optional] Plain text that describes the purpose of the link, and can be used as the
             link's text.
         :return: PagerDuty Events API v2 response.
         """
-        warnings.warn(
-            "This method will be deprecated. Please use the "
-            "`airflow.providers.pagerduty.hooks.PagerdutyEventsHook` to interact with the Events API",
-            AirflowProviderDeprecationWarning,
-            stacklevel=2,
-        )
-
         routing_key = routing_key or self.routing_key
 
         return PagerdutyEventsHook(integration_key=routing_key).create_event(
             summary=summary,
             severity=severity,
             source=source,
             action=action,
```

### Comparing `apache_airflow_providers_pagerduty-3.7.0rc1/airflow/providers/pagerduty/hooks/pagerduty_events.py` & `apache_airflow_providers_pagerduty-3.7.0rc2/airflow/providers/pagerduty/hooks/pagerduty_events.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,20 +12,21 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """Hook for sending or receiving data from PagerDuty as well as creating PagerDuty incidents."""
+
 from __future__ import annotations
 
-import warnings
 from typing import TYPE_CHECKING, Any
 
 import pdpyras
+from deprecated import deprecated
 
 from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.hooks.base import BaseHook
 
 if TYPE_CHECKING:
     from datetime import datetime
 
@@ -45,29 +46,26 @@
     conn_name_attr = "pagerduty_events_conn_id"
     default_conn_name = "pagerduty_events_default"
     conn_type = "pagerduty_events"
     hook_name = "Pagerduty Events"
 
     @classmethod
     def get_ui_field_behaviour(cls) -> dict[str, Any]:
-        """Returns custom field behaviour."""
+        """Return custom field behaviour."""
         return {
             "hidden_fields": ["port", "login", "schema", "host", "extra"],
             "relabeling": {
                 "password": "Pagerduty Integration key",
             },
         }
 
     def __init__(
-        self,
-        integration_key: str | None = None,
-        pagerduty_events_conn_id: str | None = None,
-        **kwargs,
+        self, integration_key: str | None = None, pagerduty_events_conn_id: str | None = None
     ) -> None:
-        super().__init__(**kwargs)
+        super().__init__()
         self.integration_key = None
         self._session = None
 
         if pagerduty_events_conn_id is not None:
             conn = self.get_connection(pagerduty_events_conn_id)
             self.integration_key = conn.get_password()
 
@@ -75,14 +73,21 @@
             self.integration_key = integration_key
 
         if self.integration_key is None:
             raise AirflowException(
                 "Cannot get token: No valid integration key nor pagerduty_events_conn_id supplied."
             )
 
+    @deprecated(
+        reason=(
+            "This method will be deprecated. Please use the "
+            "`PagerdutyEventsHook.send_event` to interact with the Events API"
+        ),
+        category=AirflowProviderDeprecationWarning,
+    )
     def create_event(
         self,
         summary: str,
         severity: str,
         source: str = "airflow",
         action: str = "trigger",
         dedup_key: str | None = None,
@@ -117,21 +122,14 @@
             `alt`: [Optional] Alternative text for the image.
         :param links: List of links to include. Each dictionary in the list accepts the following keys:
             `href`: URL of the link to be attached.
             `text`: [Optional] Plain text that describes the purpose of the link, and can be used as the
             link's text.
         :return: PagerDuty Events API v2 response.
         """
-        warnings.warn(
-            "This method will be deprecated. Please use the "
-            "`PagerdutyEventsHook.send_event` to interact with the Events API",
-            AirflowProviderDeprecationWarning,
-            stacklevel=2,
-        )
-
         data = PagerdutyEventsHook.prepare_event_data(
             summary=summary,
             severity=severity,
             source=source,
             custom_details=custom_details,
             component=component,
             group=group,
```

### Comparing `apache_airflow_providers_pagerduty-3.7.0rc1/airflow/providers/pagerduty/notifications/__init__.py` & `apache_airflow_providers_pagerduty-3.7.0rc2/airflow/providers/pagerduty/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_pagerduty-3.7.0rc1/airflow/providers/pagerduty/notifications/pagerduty.py` & `apache_airflow_providers_pagerduty-3.7.0rc2/airflow/providers/pagerduty/notifications/pagerduty.py`

 * *Files 9% similar despite different names*

```diff
@@ -80,31 +80,29 @@
         dedup_key: str | None = None,
         custom_details: Any | None = None,
         group: str | None = None,
         component: str | None = None,
         class_type: str | None = None,
         images: list[Any] | None = None,
         links: list[Any] | None = None,
-        pagerduty_events_conn_id: str = "pagerduty_events_default",
+        pagerduty_events_conn_id: str | None = "pagerduty_events_default",
         integration_key: str | None = None,
     ):
         super().__init__()
         self.pagerduty_events_conn_id = pagerduty_events_conn_id
         self.integration_key = integration_key
         self.summary = summary
         self.severity = severity
         self.source = source
         self.action = action
         self.dedup_key = dedup_key
         self.custom_details = custom_details
-        self.custom_details = custom_details
         self.group = group
         self.component = component
         self.class_type = class_type
-        self.class_type = class_type
         self.images = images
         self.links = links
 
     @cached_property
     def hook(self) -> PagerdutyEventsHook:
         """Pagerduty Events Hook."""
         return PagerdutyEventsHook(
```

### Comparing `apache_airflow_providers_pagerduty-3.7.0rc1/pyproject.toml` & `apache_airflow_providers_pagerduty-3.7.0rc2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-pagerduty"
-version = "3.7.0.rc1"
+version = "3.7.0.rc2"
 description = "Provider package apache-airflow-providers-pagerduty for Apache Airflow"
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
     "pdpyras>=4.1.2",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.7.0"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.7.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
```

### Comparing `apache_airflow_providers_pagerduty-3.7.0rc1/PKG-INFO` & `apache_airflow_providers_pagerduty-3.7.0rc2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-pagerduty
-Version: 3.7.0rc1
+Version: 3.7.0rc2
 Summary: Provider package apache-airflow-providers-pagerduty for Apache Airflow
 Keywords: airflow-provider,pagerduty,airflow,integration
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
 Requires-Dist: pdpyras>=4.1.2
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.7.0/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.7.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
@@ -70,15 +71,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-pagerduty``
 
-Release: ``3.7.0.rc1``
+Release: ``3.7.0.rc2``
 
 
 `Pagerduty <https://www.pagerduty.com/>`__
 
 
 Provider package
 ----------------
@@ -92,21 +93,21 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-pagerduty``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.6.0``
+``apache-airflow``  ``>=2.7.0``
 ``pdpyras``         ``>=4.1.2``
 ==================  ==================
 
 The changelog for the provider package can be found in the
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.7.0/changelog.html>`_.
```

