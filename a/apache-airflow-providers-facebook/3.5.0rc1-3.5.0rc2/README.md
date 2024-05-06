# Comparing `tmp/apache_airflow_providers_facebook-3.5.0rc1.tar.gz` & `tmp/apache_airflow_providers_facebook-3.5.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_facebook-3.5.0rc1.tar", last modified: Mon Jan 22 08:28:11 2024, max compression
+gzip compressed data, was "apache_airflow_providers_facebook-3.5.0rc2.tar", last modified: Tue Apr 30 11:26:15 2024, max compression
```

## Comparing `apache_airflow_providers_facebook-3.5.0rc1.tar` & `apache_airflow_providers_facebook-3.5.0rc2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     3094 2024-01-22 08:28:11.000000 apache_airflow_providers_facebook-3.5.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-01-22 08:28:11.000000 apache_airflow_providers_facebook-3.5.0rc1/airflow/providers/facebook/LICENSE
--rw-r--r--   0        0        0     1583 2024-01-22 08:28:11.000000 apache_airflow_providers_facebook-3.5.0rc1/airflow/providers/facebook/__init__.py
--rw-r--r--   0        0        0      785 2024-01-22 08:28:11.000000 apache_airflow_providers_facebook-3.5.0rc1/airflow/providers/facebook/ads/__init__.py
--rw-r--r--   0        0        0      785 2024-01-22 08:28:11.000000 apache_airflow_providers_facebook-3.5.0rc1/airflow/providers/facebook/ads/hooks/__init__.py
--rw-r--r--   0        0        0     7864 2024-01-22 08:28:11.000000 apache_airflow_providers_facebook-3.5.0rc1/airflow/providers/facebook/ads/hooks/ads.py
--rw-r--r--   0        0        0     2557 2024-01-22 08:28:11.000000 apache_airflow_providers_facebook-3.5.0rc1/airflow/providers/facebook/get_provider_info.py
--rw-r--r--   0        0        0     2943 2024-01-22 08:28:11.000000 apache_airflow_providers_facebook-3.5.0rc1/pyproject.toml
--rw-r--r--   0        0        0     4755 1970-01-01 00:00:00.000000 apache_airflow_providers_facebook-3.5.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     3099 2024-04-30 11:26:15.000000 apache_airflow_providers_facebook-3.5.0rc2/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-30 11:26:15.000000 apache_airflow_providers_facebook-3.5.0rc2/airflow/providers/facebook/LICENSE
+-rw-r--r--   0        0        0     1583 2024-04-30 11:26:15.000000 apache_airflow_providers_facebook-3.5.0rc2/airflow/providers/facebook/__init__.py
+-rw-r--r--   0        0        0      785 2024-04-30 11:26:15.000000 apache_airflow_providers_facebook-3.5.0rc2/airflow/providers/facebook/ads/__init__.py
+-rw-r--r--   0        0        0      785 2024-04-30 11:26:15.000000 apache_airflow_providers_facebook-3.5.0rc2/airflow/providers/facebook/ads/hooks/__init__.py
+-rw-r--r--   0        0        0     7839 2024-04-30 11:26:15.000000 apache_airflow_providers_facebook-3.5.0rc2/airflow/providers/facebook/ads/hooks/ads.py
+-rw-r--r--   0        0        0     2557 2024-04-30 11:26:15.000000 apache_airflow_providers_facebook-3.5.0rc2/airflow/providers/facebook/get_provider_info.py
+-rw-r--r--   0        0        0     2987 2024-04-30 11:26:15.000000 apache_airflow_providers_facebook-3.5.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     4809 1970-01-01 00:00:00.000000 apache_airflow_providers_facebook-3.5.0rc2/PKG-INFO
```

### Comparing `apache_airflow_providers_facebook-3.5.0rc1/README.rst` & `apache_airflow_providers_facebook-3.5.0rc2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-facebook``
 
-Release: ``3.5.0.rc1``
+Release: ``3.5.0.rc2``
 
 
 `Facebook Ads <https://www.facebook.com/about/ads>`__
 
 
 Provider package
 ----------------
@@ -60,21 +60,21 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-facebook``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 =====================  ==================
 PIP package            Version required
 =====================  ==================
-``apache-airflow``     ``>=2.6.0``
+``apache-airflow``     ``>=2.7.0``
 ``facebook-business``  ``>=6.0.2``
 =====================  ==================
 
 The changelog for the provider package can be found in the
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-facebook/3.5.0/changelog.html>`_.
```

### Comparing `apache_airflow_providers_facebook-3.5.0rc1/airflow/providers/facebook/LICENSE` & `apache_airflow_providers_facebook-3.5.0rc2/airflow/providers/facebook/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_facebook-3.5.0rc1/airflow/providers/facebook/__init__.py` & `apache_airflow_providers_facebook-3.5.0rc2/airflow/providers/facebook/__init__.py`

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
-        f"The package `apache-airflow-providers-facebook:{__version__}` needs Apache Airflow 2.6.0+"
+        f"The package `apache-airflow-providers-facebook:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_facebook-3.5.0rc1/airflow/providers/facebook/ads/__init__.py` & `apache_airflow_providers_facebook-3.5.0rc2/airflow/providers/facebook/ads/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_facebook-3.5.0rc1/airflow/providers/facebook/ads/hooks/__init__.py` & `apache_airflow_providers_facebook-3.5.0rc2/airflow/providers/facebook/ads/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_facebook-3.5.0rc1/airflow/providers/facebook/ads/hooks/ads.py` & `apache_airflow_providers_facebook-3.5.0rc2/airflow/providers/facebook/ads/hooks/ads.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """This module contains Facebook Ads Reporting hooks."""
+
 from __future__ import annotations
 
 import time
 from enum import Enum
 from functools import cached_property
 from typing import TYPE_CHECKING, Any
 
@@ -62,17 +63,16 @@
     conn_type = "facebook_social"
     hook_name = "Facebook Ads"
 
     def __init__(
         self,
         facebook_conn_id: str = default_conn_name,
         api_version: str | None = None,
-        **kwargs,
     ) -> None:
-        super().__init__(**kwargs)
+        super().__init__()
         self.facebook_conn_id = facebook_conn_id
         self.api_version = api_version
         self.client_required_fields = ["app_id", "app_secret", "access_token", "account_id"]
 
     def _get_service(self) -> FacebookAdsApi:
         """Return Facebook Ads Client using a service account."""
         config = self.facebook_ads_config
```

### Comparing `apache_airflow_providers_facebook-3.5.0rc1/airflow/providers/facebook/get_provider_info.py` & `apache_airflow_providers_facebook-3.5.0rc2/airflow/providers/facebook/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-facebook",
         "name": "Facebook",
         "description": "`Facebook Ads <https://www.facebook.com/about/ads>`__\n",
         "state": "ready",
-        "source-date-epoch": 1705912091,
+        "source-date-epoch": 1714476375,
         "versions": [
             "3.5.0",
             "3.4.0",
             "3.3.0",
             "3.2.2",
             "3.2.1",
             "3.2.0",
@@ -46,15 +46,15 @@
             "2.1.0",
             "2.0.1",
             "2.0.0",
             "1.1.0",
             "1.0.1",
             "1.0.0",
         ],
-        "dependencies": ["apache-airflow>=2.6.0", "facebook-business>=6.0.2"],
+        "dependencies": ["apache-airflow>=2.7.0", "facebook-business>=6.0.2"],
         "integrations": [
             {
                 "integration-name": "Facebook Ads",
                 "external-doc-url": "https://business.facebook.com",
                 "logo": "/integration-logos/facebook/Facebook-Ads.png",
                 "tags": ["service"],
             }
```

### Comparing `apache_airflow_providers_facebook-3.5.0rc1/pyproject.toml` & `apache_airflow_providers_facebook-3.5.0rc2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-facebook"
-version = "3.5.0.rc1"
+version = "3.5.0.rc2"
 description = "Provider package apache-airflow-providers-facebook for Apache Airflow"
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
     "facebook-business>=6.0.2",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-facebook/3.5.0"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-facebook/3.5.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
```

### Comparing `apache_airflow_providers_facebook-3.5.0rc1/PKG-INFO` & `apache_airflow_providers_facebook-3.5.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-facebook
-Version: 3.5.0rc1
+Version: 3.5.0rc2
 Summary: Provider package apache-airflow-providers-facebook for Apache Airflow
 Keywords: airflow-provider,facebook,airflow,integration
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
 Requires-Dist: facebook-business>=6.0.2
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-facebook/3.5.0/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-facebook/3.5.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
@@ -70,15 +71,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-facebook``
 
-Release: ``3.5.0.rc1``
+Release: ``3.5.0.rc2``
 
 
 `Facebook Ads <https://www.facebook.com/about/ads>`__
 
 
 Provider package
 ----------------
@@ -92,21 +93,21 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-facebook``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 =====================  ==================
 PIP package            Version required
 =====================  ==================
-``apache-airflow``     ``>=2.6.0``
+``apache-airflow``     ``>=2.7.0``
 ``facebook-business``  ``>=6.0.2``
 =====================  ==================
 
 The changelog for the provider package can be found in the
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-facebook/3.5.0/changelog.html>`_.
```

