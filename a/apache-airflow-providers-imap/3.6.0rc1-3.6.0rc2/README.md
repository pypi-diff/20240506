# Comparing `tmp/apache_airflow_providers_imap-3.6.0rc1.tar.gz` & `tmp/apache_airflow_providers_imap-3.6.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_imap-3.6.0rc1.tar", last modified: Mon Jan 22 08:28:57 2024, max compression
+gzip compressed data, was "apache_airflow_providers_imap-3.6.0rc2.tar", last modified: Tue Apr 30 11:30:25 2024, max compression
```

## Comparing `apache_airflow_providers_imap-3.6.0rc1.tar` & `apache_airflow_providers_imap-3.6.0rc2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3048 2024-01-22 08:28:57.000000 apache_airflow_providers_imap-3.6.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-01-22 08:28:57.000000 apache_airflow_providers_imap-3.6.0rc1/airflow/providers/imap/LICENSE
--rw-r--r--   0        0        0     1579 2024-01-22 08:28:57.000000 apache_airflow_providers_imap-3.6.0rc1/airflow/providers/imap/__init__.py
--rw-r--r--   0        0        0     4373 2024-01-22 08:28:57.000000 apache_airflow_providers_imap-3.6.0rc1/airflow/providers/imap/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-01-22 08:28:57.000000 apache_airflow_providers_imap-3.6.0rc1/airflow/providers/imap/hooks/__init__.py
--rw-r--r--   0        0        0    15294 2024-01-22 08:28:57.000000 apache_airflow_providers_imap-3.6.0rc1/airflow/providers/imap/hooks/imap.py
--rw-r--r--   0        0        0      787 2024-01-22 08:28:57.000000 apache_airflow_providers_imap-3.6.0rc1/airflow/providers/imap/sensors/__init__.py
--rw-r--r--   0        0        0     3054 2024-01-22 08:28:57.000000 apache_airflow_providers_imap-3.6.0rc1/airflow/providers/imap/sensors/imap_attachment.py
--rw-r--r--   0        0        0     2883 2024-01-22 08:28:57.000000 apache_airflow_providers_imap-3.6.0rc1/pyproject.toml
--rw-r--r--   0        0        0     4649 1970-01-01 00:00:00.000000 apache_airflow_providers_imap-3.6.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     3053 2024-04-30 11:30:25.000000 apache_airflow_providers_imap-3.6.0rc2/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-30 11:30:25.000000 apache_airflow_providers_imap-3.6.0rc2/airflow/providers/imap/LICENSE
+-rw-r--r--   0        0        0     1579 2024-04-30 11:30:25.000000 apache_airflow_providers_imap-3.6.0rc2/airflow/providers/imap/__init__.py
+-rw-r--r--   0        0        0     4373 2024-04-30 11:30:25.000000 apache_airflow_providers_imap-3.6.0rc2/airflow/providers/imap/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:30:25.000000 apache_airflow_providers_imap-3.6.0rc2/airflow/providers/imap/hooks/__init__.py
+-rw-r--r--   0        0        0    15277 2024-04-30 11:30:25.000000 apache_airflow_providers_imap-3.6.0rc2/airflow/providers/imap/hooks/imap.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:30:25.000000 apache_airflow_providers_imap-3.6.0rc2/airflow/providers/imap/sensors/__init__.py
+-rw-r--r--   0        0        0     3055 2024-04-30 11:30:25.000000 apache_airflow_providers_imap-3.6.0rc2/airflow/providers/imap/sensors/imap_attachment.py
+-rw-r--r--   0        0        0     2927 2024-04-30 11:30:25.000000 apache_airflow_providers_imap-3.6.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     4703 1970-01-01 00:00:00.000000 apache_airflow_providers_imap-3.6.0rc2/PKG-INFO
```

### Comparing `apache_airflow_providers_imap-3.6.0rc1/README.rst` & `apache_airflow_providers_imap-3.6.0rc2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-imap``
 
-Release: ``3.6.0.rc1``
+Release: ``3.6.0.rc2``
 
 
 `Internet Message Access Protocol (IMAP) <https://tools.ietf.org/html/rfc3501>`__
 
 
 Provider package
 ----------------
@@ -60,20 +60,20 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-imap``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.6.0``
+``apache-airflow``  ``>=2.7.0``
 ==================  ==================
 
 The changelog for the provider package can be found in the
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-imap/3.6.0/changelog.html>`_.
```

### Comparing `apache_airflow_providers_imap-3.6.0rc1/airflow/providers/imap/LICENSE` & `apache_airflow_providers_imap-3.6.0rc2/airflow/providers/imap/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_imap-3.6.0rc1/airflow/providers/imap/__init__.py` & `apache_airflow_providers_imap-3.6.0rc2/airflow/providers/imap/__init__.py`

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
-        f"The package `apache-airflow-providers-imap:{__version__}` needs Apache Airflow 2.6.0+"
+        f"The package `apache-airflow-providers-imap:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_imap-3.6.0rc1/airflow/providers/imap/get_provider_info.py` & `apache_airflow_providers_imap-3.6.0rc2/airflow/providers/imap/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-imap",
         "name": "Internet Message Access Protocol (IMAP)",
         "description": "`Internet Message Access Protocol (IMAP) <https://tools.ietf.org/html/rfc3501>`__\n",
         "state": "ready",
-        "source-date-epoch": 1705912137,
+        "source-date-epoch": 1714476625,
         "versions": [
             "3.6.0",
             "3.5.0",
             "3.4.0",
             "3.3.2",
             "3.3.1",
             "3.3.0",
@@ -48,15 +48,15 @@
             "2.2.0",
             "2.1.0",
             "2.0.1",
             "2.0.0",
             "1.0.1",
             "1.0.0",
         ],
-        "dependencies": ["apache-airflow>=2.6.0"],
+        "dependencies": ["apache-airflow>=2.7.0"],
         "integrations": [
             {
                 "integration-name": "Internet Message Access Protocol (IMAP)",
                 "external-doc-url": "https://tools.ietf.org/html/rfc3501",
                 "logo": "/integration-logos/imap/IMAP.png",
                 "tags": ["protocol"],
             }
```

### Comparing `apache_airflow_providers_imap-3.6.0rc1/airflow/providers/imap/hooks/__init__.py` & `apache_airflow_providers_imap-3.6.0rc2/airflow/providers/imap/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_imap-3.6.0rc1/airflow/providers/imap/hooks/imap.py` & `apache_airflow_providers_imap-3.6.0rc2/airflow/providers/imap/hooks/imap.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # specific language governing permissions and limitations
 # under the License.
 """
 This module provides everything to search mail for a specific attachment and download it.
 
 It uses the imaplib library that is already integrated in python 3.
 """
+
 from __future__ import annotations
 
 import email
 import imaplib
 import os
 import re
 import ssl
@@ -49,16 +50,16 @@
     """
 
     conn_name_attr = "imap_conn_id"
     default_conn_name = "imap_default"
     conn_type = "imap"
     hook_name = "IMAP"
 
-    def __init__(self, imap_conn_id: str = default_conn_name, **kwargs) -> None:
-        super().__init__(**kwargs)
+    def __init__(self, imap_conn_id: str = default_conn_name) -> None:
+        super().__init__()
         self.imap_conn_id = imap_conn_id
         self.mail_client: imaplib.IMAP4_SSL | imaplib.IMAP4 | None = None
 
     def __enter__(self) -> ImapHook:
         return self.get_conn()
 
     def __exit__(self, exc_type, exc_val, exc_tb):
@@ -116,15 +117,15 @@
 
         return mail_client
 
     def has_mail_attachment(
         self, name: str, *, check_regex: bool = False, mail_folder: str = "INBOX", mail_filter: str = "All"
     ) -> bool:
         """
-        Checks the mail folder for mails containing attachments with the given name.
+        Check the mail folder for mails containing attachments with the given name.
 
         :param name: The name of the attachment that will be searched for.
         :param check_regex: Checks the name for a regular expression.
         :param mail_folder: The mail folder where to look at.
         :param mail_filter: If set other than 'All' only specific mails will be checked.
             See :py:meth:`imaplib.IMAP4.search` for details.
         :returns: True if there is an attachment with the given name and False if not.
@@ -141,15 +142,15 @@
         check_regex: bool = False,
         latest_only: bool = False,
         mail_folder: str = "INBOX",
         mail_filter: str = "All",
         not_found_mode: str = "raise",
     ) -> list[tuple]:
         """
-        Retrieves mail's attachments in the mail folder by its name.
+        Retrieve mail's attachments in the mail folder by its name.
 
         :param name: The name of the attachment that will be downloaded.
         :param check_regex: Checks the name for a regular expression.
         :param latest_only: If set to True it will only retrieve the first matched attachment.
         :param mail_folder: The mail folder where to look at.
         :param mail_filter: If set other than 'All' only specific mails will be checked.
             See :py:meth:`imaplib.IMAP4.search` for details.
@@ -177,15 +178,15 @@
         check_regex: bool = False,
         latest_only: bool = False,
         mail_folder: str = "INBOX",
         mail_filter: str = "All",
         not_found_mode: str = "raise",
     ) -> None:
         """
-        Downloads mail's attachments in the mail folder by its name to the local directory.
+        Download mail's attachments in the mail folder by its name to the local directory.
 
         :param name: The name of the attachment that will be downloaded.
         :param local_output_directory: The output directory on the local machine
             where the files will be downloaded to.
         :param check_regex: Checks the name for a regular expression.
         :param latest_only: If set to True it will only download the first matched attachment.
         :param mail_folder: The mail folder where to look at.
@@ -214,15 +215,15 @@
         elif not_found_mode == "warn":
             self.log.warning("No mail attachments found!")
 
     def _retrieve_mails_attachments_by_name(
         self, name: str, check_regex: bool, latest_only: bool, mail_folder: str, mail_filter: str
     ) -> list:
         if not self.mail_client:
-            raise Exception("The 'mail_client' should be initialized before!")
+            raise RuntimeError("The 'mail_client' should be initialized before!")
 
         all_matching_attachments = []
 
         self.mail_client.select(mail_folder)
 
         for mail_id in self._list_mail_ids_desc(mail_filter):
             response_mail_body = self._fetch_mail_body(mail_id)
@@ -235,22 +236,22 @@
 
         self.mail_client.close()
 
         return all_matching_attachments
 
     def _list_mail_ids_desc(self, mail_filter: str) -> Iterable[str]:
         if not self.mail_client:
-            raise Exception("The 'mail_client' should be initialized before!")
+            raise RuntimeError("The 'mail_client' should be initialized before!")
         _, data = self.mail_client.search(None, mail_filter)
         mail_ids = data[0].split()
         return reversed(mail_ids)
 
     def _fetch_mail_body(self, mail_id: str) -> str:
         if not self.mail_client:
-            raise Exception("The 'mail_client' should be initialized before!")
+            raise RuntimeError("The 'mail_client' should be initialized before!")
         _, data = self.mail_client.fetch(mail_id, "(RFC822)")
         mail_body = data[0][1]  # type: ignore # The mail body is always in this specific location
         mail_body_str = mail_body.decode("utf-8")  # type: ignore
         return mail_body_str
 
     def _check_mail_body(
         self, response_mail_body: str, name: str, check_regex: bool, latest_only: bool
@@ -300,25 +301,25 @@
 
     def __init__(self, mail_body: str) -> None:
         super().__init__()
         self.mail = email.message_from_string(mail_body)
 
     def has_attachments(self) -> bool:
         """
-        Checks the mail for a attachments.
+        Check the mail for a attachments.
 
         :returns: True if it has attachments and False if not.
         """
         return self.mail.get_content_maintype() == "multipart"
 
     def get_attachments_by_name(
         self, name: str, check_regex: bool, find_first: bool = False
     ) -> list[tuple[Any, Any]]:
         """
-        Gets all attachments by name for the mail.
+        Get all attachments by name for the mail.
 
         :param name: The name of the attachment to look for.
         :param check_regex: Checks the name for a regular expression.
         :param find_first: If set to True it will only find the first match and then quit.
         :returns: a list of tuples each containing name and payload
             where the attachments name matches the given name.
         """
@@ -352,38 +353,38 @@
     """
 
     def __init__(self, part: Any) -> None:
         self.part = part
 
     def is_attachment(self) -> bool:
         """
-        Checks if the part is a valid mail attachment.
+        Check if the part is a valid mail attachment.
 
         :returns: True if it is an attachment and False if not.
         """
         return self.part.get_content_maintype() != "multipart" and self.part.get("Content-Disposition")
 
     def has_matching_name(self, name: str) -> tuple[Any, Any] | None:
         """
-        Checks if the given name matches the part's name.
+        Check if the given name matches the part's name.
 
         :param name: The name to look for.
         :returns: True if it matches the name (including regular expression).
         """
         return re.match(name, self.part.get_filename())  # type: ignore
 
     def has_equal_name(self, name: str) -> bool:
         """
-        Checks if the given name is equal to the part's name.
+        Check if the given name is equal to the part's name.
 
         :param name: The name to look for.
         :returns: True if it is equal to the given name.
         """
         return self.part.get_filename() == name
 
     def get_file(self) -> tuple:
         """
-        Gets the file including name and payload.
+        Get the file including name and payload.
 
         :returns: the part's name and payload.
         """
         return self.part.get_filename(), self.part.get_payload(decode=True)
```

### Comparing `apache_airflow_providers_imap-3.6.0rc1/airflow/providers/imap/sensors/__init__.py` & `apache_airflow_providers_imap-3.6.0rc2/airflow/providers/imap/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_imap-3.6.0rc1/airflow/providers/imap/sensors/imap_attachment.py` & `apache_airflow_providers_imap-3.6.0rc2/airflow/providers/imap/sensors/imap_attachment.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """This module allows you to poke for attachments on a mail server."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Sequence
 
 from airflow.providers.imap.hooks.imap import ImapHook
 from airflow.sensors.base import BaseSensorOperator
```

### Comparing `apache_airflow_providers_imap-3.6.0rc1/pyproject.toml` & `apache_airflow_providers_imap-3.6.0rc2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-imap"
-version = "3.6.0.rc1"
+version = "3.6.0.rc2"
 description = "Provider package apache-airflow-providers-imap for Apache Airflow"
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
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-imap/3.6.0"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-imap/3.6.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
```

### Comparing `apache_airflow_providers_imap-3.6.0rc1/PKG-INFO` & `apache_airflow_providers_imap-3.6.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-imap
-Version: 3.6.0rc1
+Version: 3.6.0rc2
 Summary: Provider package apache-airflow-providers-imap for Apache Airflow
 Keywords: airflow-provider,imap,airflow,integration
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
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-imap/3.6.0/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-imap/3.6.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
@@ -69,15 +70,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-imap``
 
-Release: ``3.6.0.rc1``
+Release: ``3.6.0.rc2``
 
 
 `Internet Message Access Protocol (IMAP) <https://tools.ietf.org/html/rfc3501>`__
 
 
 Provider package
 ----------------
@@ -91,20 +92,20 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-imap``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.6.0``
+``apache-airflow``  ``>=2.7.0``
 ==================  ==================
 
 The changelog for the provider package can be found in the
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-imap/3.6.0/changelog.html>`_.
```

