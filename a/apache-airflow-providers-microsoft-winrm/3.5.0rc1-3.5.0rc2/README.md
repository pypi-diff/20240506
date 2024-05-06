# Comparing `tmp/apache_airflow_providers_microsoft_winrm-3.5.0rc1.tar.gz` & `tmp/apache_airflow_providers_microsoft_winrm-3.5.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_microsoft_winrm-3.5.0rc1.tar", last modified: Mon Jan 22 08:29:22 2024, max compression
+gzip compressed data, was "apache_airflow_providers_microsoft_winrm-3.5.0rc2.tar", last modified: Tue Apr 30 11:33:42 2024, max compression
```

## Comparing `apache_airflow_providers_microsoft_winrm-3.5.0rc1.tar` & `apache_airflow_providers_microsoft_winrm-3.5.0rc2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3156 2024-01-22 08:29:22.000000 apache_airflow_providers_microsoft_winrm-3.5.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-01-22 08:29:22.000000 apache_airflow_providers_microsoft_winrm-3.5.0rc1/airflow/providers/microsoft/winrm/LICENSE
--rw-r--r--   0        0        0     1590 2024-01-22 08:29:22.000000 apache_airflow_providers_microsoft_winrm-3.5.0rc1/airflow/providers/microsoft/winrm/__init__.py
--rw-r--r--   0        0        0     2780 2024-01-22 08:29:22.000000 apache_airflow_providers_microsoft_winrm-3.5.0rc1/airflow/providers/microsoft/winrm/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-01-22 08:29:22.000000 apache_airflow_providers_microsoft_winrm-3.5.0rc1/airflow/providers/microsoft/winrm/hooks/__init__.py
--rw-r--r--   0        0        0    10549 2024-01-22 08:29:22.000000 apache_airflow_providers_microsoft_winrm-3.5.0rc1/airflow/providers/microsoft/winrm/hooks/winrm.py
--rw-r--r--   0        0        0      787 2024-01-22 08:29:22.000000 apache_airflow_providers_microsoft_winrm-3.5.0rc1/airflow/providers/microsoft/winrm/operators/__init__.py
--rw-r--r--   0        0        0     6493 2024-01-22 08:29:22.000000 apache_airflow_providers_microsoft_winrm-3.5.0rc1/airflow/providers/microsoft/winrm/operators/winrm.py
--rw-r--r--   0        0        0     2980 2024-01-22 08:29:22.000000 apache_airflow_providers_microsoft_winrm-3.5.0rc1/pyproject.toml
--rw-r--r--   0        0        0     4840 1970-01-01 00:00:00.000000 apache_airflow_providers_microsoft_winrm-3.5.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     3161 2024-04-30 11:33:42.000000 apache_airflow_providers_microsoft_winrm-3.5.0rc2/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-30 11:33:42.000000 apache_airflow_providers_microsoft_winrm-3.5.0rc2/airflow/providers/microsoft/winrm/LICENSE
+-rw-r--r--   0        0        0     1590 2024-04-30 11:33:42.000000 apache_airflow_providers_microsoft_winrm-3.5.0rc2/airflow/providers/microsoft/winrm/__init__.py
+-rw-r--r--   0        0        0     2780 2024-04-30 11:33:42.000000 apache_airflow_providers_microsoft_winrm-3.5.0rc2/airflow/providers/microsoft/winrm/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:33:42.000000 apache_airflow_providers_microsoft_winrm-3.5.0rc2/airflow/providers/microsoft/winrm/hooks/__init__.py
+-rw-r--r--   0        0        0    10524 2024-04-30 11:33:42.000000 apache_airflow_providers_microsoft_winrm-3.5.0rc2/airflow/providers/microsoft/winrm/hooks/winrm.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:33:42.000000 apache_airflow_providers_microsoft_winrm-3.5.0rc2/airflow/providers/microsoft/winrm/operators/__init__.py
+-rw-r--r--   0        0        0     6493 2024-04-30 11:33:42.000000 apache_airflow_providers_microsoft_winrm-3.5.0rc2/airflow/providers/microsoft/winrm/operators/winrm.py
+-rw-r--r--   0        0        0     3024 2024-04-30 11:33:42.000000 apache_airflow_providers_microsoft_winrm-3.5.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     4894 1970-01-01 00:00:00.000000 apache_airflow_providers_microsoft_winrm-3.5.0rc2/PKG-INFO
```

### Comparing `apache_airflow_providers_microsoft_winrm-3.5.0rc1/README.rst` & `apache_airflow_providers_microsoft_winrm-3.5.0rc2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-microsoft-winrm``
 
-Release: ``3.5.0.rc1``
+Release: ``3.5.0.rc2``
 
 
 `Windows Remote Management (WinRM) <https://docs.microsoft.com/windows/win32/winrm/portal>`__
 
 
 Provider package
 ----------------
@@ -60,21 +60,21 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-microsoft-winrm``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.6.0``
+``apache-airflow``  ``>=2.7.0``
 ``pywinrm``         ``>=0.4``
 ==================  ==================
 
 The changelog for the provider package can be found in the
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-winrm/3.5.0/changelog.html>`_.
```

### Comparing `apache_airflow_providers_microsoft_winrm-3.5.0rc1/airflow/providers/microsoft/winrm/LICENSE` & `apache_airflow_providers_microsoft_winrm-3.5.0rc2/airflow/providers/microsoft/winrm/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_winrm-3.5.0rc1/airflow/providers/microsoft/winrm/__init__.py` & `apache_airflow_providers_microsoft_winrm-3.5.0rc2/airflow/providers/microsoft/winrm/__init__.py`

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
-        f"The package `apache-airflow-providers-microsoft-winrm:{__version__}` needs Apache Airflow 2.6.0+"
+        f"The package `apache-airflow-providers-microsoft-winrm:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_microsoft_winrm-3.5.0rc1/airflow/providers/microsoft/winrm/get_provider_info.py` & `apache_airflow_providers_microsoft_winrm-3.5.0rc2/airflow/providers/microsoft/winrm/get_provider_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-microsoft-winrm",
         "name": "Windows Remote Management (WinRM)",
         "description": "`Windows Remote Management (WinRM) <https://docs.microsoft.com/windows/win32/winrm/portal>`__\n",
         "state": "ready",
-        "source-date-epoch": 1705912162,
+        "source-date-epoch": 1714476822,
         "versions": [
             "3.5.0",
             "3.4.0",
             "3.3.0",
             "3.2.2",
             "3.2.1",
             "3.2.0",
@@ -46,15 +46,15 @@
             "2.0.1",
             "2.0.0",
             "1.2.0",
             "1.1.0",
             "1.0.1",
             "1.0.0",
         ],
-        "dependencies": ["apache-airflow>=2.6.0", "pywinrm>=0.4"],
+        "dependencies": ["apache-airflow>=2.7.0", "pywinrm>=0.4"],
         "integrations": [
             {
                 "integration-name": "Windows Remote Management (WinRM)",
                 "external-doc-url": "https://docs.microsoft.com/en-us/windows/win32/winrm/portal",
                 "logo": "/integration-logos/winrm/WinRM.png",
                 "how-to-guide": ["/docs/apache-airflow-providers-microsoft-winrm/operators.rst"],
                 "tags": ["protocol"],
```

### Comparing `apache_airflow_providers_microsoft_winrm-3.5.0rc1/airflow/providers/microsoft/winrm/hooks/__init__.py` & `apache_airflow_providers_microsoft_winrm-3.5.0rc2/airflow/providers/microsoft/winrm/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_winrm-3.5.0rc1/airflow/providers/microsoft/winrm/hooks/winrm.py` & `apache_airflow_providers_microsoft_winrm-3.5.0rc2/airflow/providers/microsoft/winrm/hooks/winrm.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """Hook for winrm remote execution."""
+
 from __future__ import annotations
 
 from winrm.protocol import Protocol
 
 from airflow.exceptions import AirflowException
 from airflow.hooks.base import BaseHook
 from airflow.utils.platform import getuser
@@ -86,17 +87,16 @@
         kerberos_delegation: bool = False,
         read_timeout_sec: int = 30,
         operation_timeout_sec: int = 20,
         kerberos_hostname_override: str | None = None,
         message_encryption: str | None = "auto",
         credssp_disable_tlsv1_2: bool = False,
         send_cbt: bool = True,
-        **kwargs,
     ) -> None:
-        super().__init__(**kwargs)
+        super().__init__()
         self.ssh_conn_id = ssh_conn_id
         self.endpoint = endpoint
         self.remote_host = remote_host
         self.remote_port = remote_port
         self.transport = transport
         self.username = username
         self.password = password
```

### Comparing `apache_airflow_providers_microsoft_winrm-3.5.0rc1/airflow/providers/microsoft/winrm/operators/__init__.py` & `apache_airflow_providers_microsoft_winrm-3.5.0rc2/airflow/providers/microsoft/winrm/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_winrm-3.5.0rc1/airflow/providers/microsoft/winrm/operators/winrm.py` & `apache_airflow_providers_microsoft_winrm-3.5.0rc2/airflow/providers/microsoft/winrm/operators/winrm.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_winrm-3.5.0rc1/pyproject.toml` & `apache_airflow_providers_microsoft_winrm-3.5.0rc2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-microsoft-winrm"
-version = "3.5.0.rc1"
+version = "3.5.0.rc2"
 description = "Provider package apache-airflow-providers-microsoft-winrm for Apache Airflow"
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
     "pywinrm>=0.4",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-microsoft-winrm/3.5.0"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-microsoft-winrm/3.5.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
```

### Comparing `apache_airflow_providers_microsoft_winrm-3.5.0rc1/PKG-INFO` & `apache_airflow_providers_microsoft_winrm-3.5.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-microsoft-winrm
-Version: 3.5.0rc1
+Version: 3.5.0rc2
 Summary: Provider package apache-airflow-providers-microsoft-winrm for Apache Airflow
 Keywords: airflow-provider,microsoft.winrm,airflow,integration
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
 Requires-Dist: pywinrm>=0.4
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-winrm/3.5.0/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-winrm/3.5.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
@@ -70,15 +71,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-microsoft-winrm``
 
-Release: ``3.5.0.rc1``
+Release: ``3.5.0.rc2``
 
 
 `Windows Remote Management (WinRM) <https://docs.microsoft.com/windows/win32/winrm/portal>`__
 
 
 Provider package
 ----------------
@@ -92,21 +93,21 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-microsoft-winrm``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.6.0``
+``apache-airflow``  ``>=2.7.0``
 ``pywinrm``         ``>=0.4``
 ==================  ==================
 
 The changelog for the provider package can be found in the
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-winrm/3.5.0/changelog.html>`_.
```

