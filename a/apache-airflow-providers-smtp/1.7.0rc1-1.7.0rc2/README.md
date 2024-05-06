# Comparing `tmp/apache_airflow_providers_smtp-1.7.0rc1.tar.gz` & `tmp/apache_airflow_providers_smtp-1.7.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_smtp-1.7.0rc1.tar", last modified: Mon Jan 22 08:31:00 2024, max compression
+gzip compressed data, was "apache_airflow_providers_smtp-1.7.0rc2.tar", last modified: Tue Apr 30 11:45:54 2024, max compression
```

## Comparing `apache_airflow_providers_smtp-1.7.0rc1.tar` & `apache_airflow_providers_smtp-1.7.0rc2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     3045 2024-01-22 08:31:00.000000 apache_airflow_providers_smtp-1.7.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-01-22 08:31:00.000000 apache_airflow_providers_smtp-1.7.0rc1/airflow/providers/smtp/LICENSE
--rw-r--r--   0        0        0     1579 2024-01-22 08:31:00.000000 apache_airflow_providers_smtp-1.7.0rc1/airflow/providers/smtp/__init__.py
--rw-r--r--   0        0        0     4258 2024-01-22 08:31:00.000000 apache_airflow_providers_smtp-1.7.0rc1/airflow/providers/smtp/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-01-22 08:31:00.000000 apache_airflow_providers_smtp-1.7.0rc1/airflow/providers/smtp/hooks/__init__.py
--rw-r--r--   0        0        0    14881 2024-01-22 08:31:00.000000 apache_airflow_providers_smtp-1.7.0rc1/airflow/providers/smtp/hooks/smtp.py
--rw-r--r--   0        0        0      785 2024-01-22 08:31:00.000000 apache_airflow_providers_smtp-1.7.0rc1/airflow/providers/smtp/notifications/__init__.py
--rw-r--r--   0        0        0     4665 2024-01-22 08:31:00.000000 apache_airflow_providers_smtp-1.7.0rc1/airflow/providers/smtp/notifications/smtp.py
--rw-r--r--   0        0        0      785 2024-01-22 08:31:00.000000 apache_airflow_providers_smtp-1.7.0rc1/airflow/providers/smtp/notifications/templates/__init__.py
--rw-r--r--   0        0        0     1580 2024-01-22 08:31:00.000000 apache_airflow_providers_smtp-1.7.0rc1/airflow/providers/smtp/notifications/templates/email.html
--rw-r--r--   0        0        0      787 2024-01-22 08:31:00.000000 apache_airflow_providers_smtp-1.7.0rc1/airflow/providers/smtp/operators/__init__.py
--rw-r--r--   0        0        0     3509 2024-01-22 08:31:00.000000 apache_airflow_providers_smtp-1.7.0rc1/airflow/providers/smtp/operators/smtp.py
--rw-r--r--   0        0        0     2883 2024-01-22 08:31:00.000000 apache_airflow_providers_smtp-1.7.0rc1/pyproject.toml
--rw-r--r--   0        0        0     4646 1970-01-01 00:00:00.000000 apache_airflow_providers_smtp-1.7.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     3050 2024-04-30 11:45:54.000000 apache_airflow_providers_smtp-1.7.0rc2/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-30 11:45:54.000000 apache_airflow_providers_smtp-1.7.0rc2/airflow/providers/smtp/LICENSE
+-rw-r--r--   0        0        0     1579 2024-04-30 11:45:54.000000 apache_airflow_providers_smtp-1.7.0rc2/airflow/providers/smtp/__init__.py
+-rw-r--r--   0        0        0     5183 2024-04-30 11:45:54.000000 apache_airflow_providers_smtp-1.7.0rc2/airflow/providers/smtp/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-04-30 11:45:54.000000 apache_airflow_providers_smtp-1.7.0rc2/airflow/providers/smtp/hooks/__init__.py
+-rw-r--r--   0        0        0    14887 2024-04-30 11:45:54.000000 apache_airflow_providers_smtp-1.7.0rc2/airflow/providers/smtp/hooks/smtp.py
+-rw-r--r--   0        0        0      785 2024-04-30 11:45:54.000000 apache_airflow_providers_smtp-1.7.0rc2/airflow/providers/smtp/notifications/__init__.py
+-rw-r--r--   0        0        0     5155 2024-04-30 11:45:54.000000 apache_airflow_providers_smtp-1.7.0rc2/airflow/providers/smtp/notifications/smtp.py
+-rw-r--r--   0        0        0      785 2024-04-30 11:45:54.000000 apache_airflow_providers_smtp-1.7.0rc2/airflow/providers/smtp/notifications/templates/__init__.py
+-rw-r--r--   0        0        0     1580 2024-04-30 11:45:54.000000 apache_airflow_providers_smtp-1.7.0rc2/airflow/providers/smtp/notifications/templates/email.html
+-rw-r--r--   0        0        0      995 2024-04-30 11:45:54.000000 apache_airflow_providers_smtp-1.7.0rc2/airflow/providers/smtp/notifications/templates/email_subject.jinja2
+-rw-r--r--   0        0        0      787 2024-04-30 11:45:54.000000 apache_airflow_providers_smtp-1.7.0rc2/airflow/providers/smtp/operators/__init__.py
+-rw-r--r--   0        0        0     3509 2024-04-30 11:45:54.000000 apache_airflow_providers_smtp-1.7.0rc2/airflow/providers/smtp/operators/smtp.py
+-rw-r--r--   0        0        0     2927 2024-04-30 11:45:54.000000 apache_airflow_providers_smtp-1.7.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     4700 1970-01-01 00:00:00.000000 apache_airflow_providers_smtp-1.7.0rc2/PKG-INFO
```

### Comparing `apache_airflow_providers_smtp-1.7.0rc1/README.rst` & `apache_airflow_providers_smtp-1.7.0rc2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-smtp``
 
-Release: ``1.7.0.rc1``
+Release: ``1.7.0.rc2``
 
 
 `Simple Mail Transfer Protocol (SMTP) <https://tools.ietf.org/html/rfc5321>`__
 
 
 Provider package
 ----------------
@@ -60,20 +60,20 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-smtp``
 
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
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.7.0/changelog.html>`_.
```

### Comparing `apache_airflow_providers_smtp-1.7.0rc1/airflow/providers/smtp/LICENSE` & `apache_airflow_providers_smtp-1.7.0rc2/airflow/providers/smtp/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_smtp-1.7.0rc1/airflow/providers/smtp/__init__.py` & `apache_airflow_providers_smtp-1.7.0rc2/airflow/providers/smtp/__init__.py`

 * *Files 8% similar despite different names*

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
-        f"The package `apache-airflow-providers-smtp:{__version__}` needs Apache Airflow 2.6.0+"
+        f"The package `apache-airflow-providers-smtp:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_smtp-1.7.0rc1/airflow/providers/smtp/get_provider_info.py` & `apache_airflow_providers_smtp-1.7.0rc2/airflow/providers/smtp/get_provider_info.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,30 +24,31 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-smtp",
         "name": "Simple Mail Transfer Protocol (SMTP)",
         "description": "`Simple Mail Transfer Protocol (SMTP) <https://tools.ietf.org/html/rfc5321>`__\n",
         "state": "ready",
-        "source-date-epoch": 1705912260,
+        "source-date-epoch": 1714477554,
         "versions": [
             "1.7.0",
+            "1.6.1",
             "1.6.0",
             "1.5.0",
             "1.4.1",
             "1.4.0",
             "1.3.2",
             "1.3.1",
             "1.3.0",
             "1.2.0",
             "1.1.0",
             "1.0.1",
             "1.0.0",
         ],
-        "dependencies": ["apache-airflow>=2.6.0"],
+        "dependencies": ["apache-airflow>=2.7.0"],
         "integrations": [
             {
                 "integration-name": "Simple Mail Transfer Protocol (SMTP)",
                 "external-doc-url": "https://tools.ietf.org/html/rfc5321",
                 "logo": "/integration-logos/smtp/SMTP.png",
                 "tags": ["protocol"],
             }
@@ -74,12 +75,26 @@
                 "options": {
                     "ssl_context": {
                         "description": 'ssl context to use when using SMTP and IMAP SSL connections. By default, the context is "default"\nwhich sets it to ``ssl.create_default_context()`` which provides the right balance between\ncompatibility and security, it however requires that certificates in your operating system are\nupdated and that SMTP/IMAP servers of yours have valid certificates that have corresponding public\nkeys installed on your machines. You can switch it to "none" if you want to disable checking\nof the certificates, but it is not recommended as it allows MITM (man-in-the-middle) attacks\nif your infrastructure is not sufficiently secured. It should only be set temporarily while you\nare fixing your certificate configuration. This can be typically done by upgrading to newer\nversion of the operating system you run Airflow components on,by upgrading/refreshing proper\ncertificates in the OS or by updating certificates for your mail servers.\n\nIf you do not set this option explicitly, it will use Airflow "email.ssl_context" configuration,\nbut if this configuration is not present, it will use "default" value.\n',
                         "type": "string",
                         "version_added": "1.3.0",
                         "example": "default",
                         "default": None,
-                    }
+                    },
+                    "templated_email_subject_path": {
+                        "description": "Allows overriding of the standard templated email subject line when the SmtpNotifier is used.\nMust provide a path to the template.\n",
+                        "type": "string",
+                        "version_added": "1.6.1",
+                        "example": "path/to/override/email_subject.html",
+                        "default": None,
+                    },
+                    "templated_html_content_path": {
+                        "description": "Allows overriding of the standard templated email path when the SmtpNotifier is used. Must provide\na path to the template.\n",
+                        "type": "string",
+                        "version_added": "1.6.1",
+                        "example": "path/to/override/email.html",
+                        "default": None,
+                    },
                 },
             }
         },
     }
```

### Comparing `apache_airflow_providers_smtp-1.7.0rc1/airflow/providers/smtp/hooks/__init__.py` & `apache_airflow_providers_smtp-1.7.0rc2/airflow/providers/smtp/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_smtp-1.7.0rc1/airflow/providers/smtp/hooks/smtp.py` & `apache_airflow_providers_smtp-1.7.0rc2/airflow/providers/smtp/hooks/smtp.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # specific language governing permissions and limitations
 # under the License.
 """
 Search in emails for a specific attachment and also to download it.
 
 It uses the smtplib library that is already integrated in python 3.
 """
+
 from __future__ import annotations
 
 import collections.abc
 import os
 import re
 import smtplib
 import ssl
@@ -52,16 +53,16 @@
     """
 
     conn_name_attr = "smtp_conn_id"
     default_conn_name = "smtp_default"
     conn_type = "smtp"
     hook_name = "SMTP"
 
-    def __init__(self, smtp_conn_id: str = default_conn_name, **kwargs) -> None:
-        super().__init__(**kwargs)
+    def __init__(self, smtp_conn_id: str = default_conn_name) -> None:
+        super().__init__()
         self.smtp_conn_id = smtp_conn_id
         self.smtp_connection: Connection | None = None
         self.smtp_client: smtplib.SMTP_SSL | smtplib.SMTP | None = None
 
     def __enter__(self) -> SmtpHook:
         return self.get_conn()
 
@@ -132,15 +133,15 @@
                     f"be set to 'default' or 'none' and is '{ssl_context_string}'."
                 )
             smtp_kwargs["context"] = ssl_context
         return SMTP(**smtp_kwargs)
 
     @classmethod
     def get_connection_form_widgets(cls) -> dict[str, Any]:
-        """Returns connection widgets to add to connection form."""
+        """Return connection widgets to add to connection form."""
         from flask_appbuilder.fieldwidgets import BS3TextFieldWidget
         from flask_babel import lazy_gettext
         from wtforms import BooleanField, IntegerField, StringField
         from wtforms.validators import NumberRange
 
         return {
             "from_email": StringField(lazy_gettext("From email"), widget=BS3TextFieldWidget()),
@@ -271,15 +272,16 @@
         :return: A tuple containing the email as a MIMEMultipart object and
             a list of recipient email addresses.
         """
         to = self._get_email_address_list(to)
 
         msg = MIMEMultipart(mime_subtype)
         msg["Subject"] = subject
-        msg["From"] = mail_from
+        if mail_from:
+            msg["From"] = mail_from
         msg["To"] = ", ".join(to)
         recipients = to
         if cc:
             cc = self._get_email_address_list(cc)
             msg["CC"] = ", ".join(cc)
             recipients += cc
 
@@ -304,15 +306,15 @@
             for header_key, header_value in custom_headers.items():
                 msg[header_key] = header_value
 
         return msg, recipients
 
     def _get_email_address_list(self, addresses: str | Iterable[str]) -> list[str]:
         """
-        Returns a list of email addresses from the provided input.
+        Return a list of email addresses from the provided input.
 
         :param addresses: A string or iterable of strings containing email addresses.
         :return: A list of email addresses.
         :raises TypeError: If the input is not a string or iterable of strings.
         """
         if isinstance(addresses, str):
             return self._get_email_list_from_str(addresses)
@@ -376,12 +378,12 @@
 
     @property
     def use_ssl(self) -> bool:
         return not bool(self.conn.extra_dejson.get("disable_ssl", False))
 
     @classmethod
     def get_ui_field_behaviour(cls) -> dict[str, Any]:
-        """Returns custom field behaviour."""
+        """Return custom field behaviour."""
         return {
             "hidden_fields": ["schema", "extra"],
             "relabeling": {},
         }
```

### Comparing `apache_airflow_providers_smtp-1.7.0rc1/airflow/providers/smtp/notifications/__init__.py` & `apache_airflow_providers_smtp-1.7.0rc2/airflow/providers/smtp/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_smtp-1.7.0rc1/airflow/providers/smtp/notifications/smtp.py` & `apache_airflow_providers_smtp-1.7.0rc2/airflow/providers/smtp/notifications/smtp.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,30 +26,33 @@
 from airflow.providers.smtp.hooks.smtp import SmtpHook
 
 
 class SmtpNotifier(BaseNotifier):
     """
     SMTP Notifier.
 
-    Accepts keyword arguments. The only required argument is `to`. Examples:
+    Accepts keyword arguments. The only required arguments are `from_email` and `to`. Examples:
 
     .. code-block:: python
 
         EmptyOperator(task_id="task", on_failure_callback=SmtpNotifier(from_email=None, to="myemail@myemail.com"))
 
         EmptyOperator(
             task_id="task",
             on_failure_callback=SmtpNotifier(
                 from_email="myemail@myemail.com",
                 to="myemail@myemail.com",
                 subject="Task {{ ti.task_id }} failed",
             ),
         )
 
-    Default template is defined in airflow.settings but can be overridden in local_settings.py
+    Default template can be overridden via the following provider configuration data:
+        - templated_email_subject_path
+        - templated_html_content_path
+
 
     :param smtp_conn_id: The :ref:`smtp connection id <howto/connection:smtp>`
         that contains the information used to authenticate the client.
     """
 
     template_fields = (
         "from_email",
@@ -78,36 +81,46 @@
         mime_subtype: str = "mixed",
         mime_charset: str = "utf-8",
         custom_headers: dict[str, Any] | None = None,
         smtp_conn_id: str = SmtpHook.default_conn_name,
         *,
         template: str | None = None,
     ):
-        from airflow.settings import SMTP_DEFAULT_TEMPLATED_HTML_CONTENT_PATH, SMTP_DEFAULT_TEMPLATED_SUBJECT
-
         super().__init__()
         self.smtp_conn_id = smtp_conn_id
         self.from_email = from_email or conf.get("smtp", "smtp_mail_from")
         self.to = to
-        self.subject = subject or SMTP_DEFAULT_TEMPLATED_SUBJECT.replace("\n", "").strip()
         self.files = files
         self.cc = cc
         self.bcc = bcc
         self.mime_subtype = mime_subtype
         self.mime_charset = mime_charset
         self.custom_headers = custom_headers
 
+        smtp_default_templated_subject_path = conf.get(
+            "smtp",
+            "templated_email_subject_path",
+            fallback=(Path(__file__).parent / "templates" / "email_subject.jinja2").as_posix(),
+        )
+        self.subject = (
+            subject or Path(smtp_default_templated_subject_path).read_text().replace("\n", "").strip()
+        )
         # If html_content is passed, prioritize it. Otherwise, if template is passed, use
         # it to populate html_content. Else, fall back to defaults defined in settings
         if html_content is not None:
             self.html_content = html_content
         elif template is not None:
             self.html_content = Path(template).read_text()
         else:
-            self.html_content = Path(SMTP_DEFAULT_TEMPLATED_HTML_CONTENT_PATH).read_text()
+            smtp_default_templated_html_content_path = conf.get(
+                "smtp",
+                "templated_html_content_path",
+                fallback=(Path(__file__).parent / "templates" / "email.html").as_posix(),
+            )
+            self.html_content = Path(smtp_default_templated_html_content_path).read_text()
 
     @cached_property
     def hook(self) -> SmtpHook:
         """Smtp Events Hook."""
         return SmtpHook(smtp_conn_id=self.smtp_conn_id)
 
     def notify(self, context):
```

### Comparing `apache_airflow_providers_smtp-1.7.0rc1/airflow/providers/smtp/notifications/templates/__init__.py` & `apache_airflow_providers_smtp-1.7.0rc2/airflow/providers/smtp/notifications/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_smtp-1.7.0rc1/airflow/providers/smtp/notifications/templates/email.html` & `apache_airflow_providers_smtp-1.7.0rc2/airflow/providers/smtp/notifications/templates/email.html`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_smtp-1.7.0rc1/airflow/providers/smtp/operators/__init__.py` & `apache_airflow_providers_smtp-1.7.0rc2/airflow/providers/smtp/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_smtp-1.7.0rc1/airflow/providers/smtp/operators/smtp.py` & `apache_airflow_providers_smtp-1.7.0rc2/airflow/providers/smtp/operators/smtp.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_smtp-1.7.0rc1/pyproject.toml` & `apache_airflow_providers_smtp-1.7.0rc2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-smtp"
-version = "1.7.0.rc1"
+version = "1.7.0.rc2"
 description = "Provider package apache-airflow-providers-smtp for Apache Airflow"
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
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.7.0"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.7.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
```

### Comparing `apache_airflow_providers_smtp-1.7.0rc1/PKG-INFO` & `apache_airflow_providers_smtp-1.7.0rc2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-smtp
-Version: 1.7.0rc1
+Version: 1.7.0rc2
 Summary: Provider package apache-airflow-providers-smtp for Apache Airflow
 Keywords: airflow-provider,smtp,airflow,integration
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
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.7.0/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.7.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
@@ -69,15 +70,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-smtp``
 
-Release: ``1.7.0.rc1``
+Release: ``1.7.0.rc2``
 
 
 `Simple Mail Transfer Protocol (SMTP) <https://tools.ietf.org/html/rfc5321>`__
 
 
 Provider package
 ----------------
@@ -91,20 +92,20 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-smtp``
 
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
 `changelog <https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.7.0/changelog.html>`_.
```

