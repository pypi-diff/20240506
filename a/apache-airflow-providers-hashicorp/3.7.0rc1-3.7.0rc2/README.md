# Comparing `tmp/apache_airflow_providers_hashicorp-3.7.0rc1.tar.gz` & `tmp/apache_airflow_providers_hashicorp-3.7.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_hashicorp-3.7.0rc1.tar", last modified: Mon Jan 22 08:28:41 2024, max compression
+gzip compressed data, was "apache_airflow_providers_hashicorp-3.7.0rc2.tar", last modified: Tue Apr 30 11:29:25 2024, max compression
```

## Comparing `apache_airflow_providers_hashicorp-3.7.0rc1.tar` & `apache_airflow_providers_hashicorp-3.7.0rc2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     4074 2024-01-22 08:28:41.000000 apache_airflow_providers_hashicorp-3.7.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-01-22 08:28:41.000000 apache_airflow_providers_hashicorp-3.7.0rc1/airflow/providers/hashicorp/LICENSE
--rw-r--r--   0        0        0     1584 2024-01-22 08:28:41.000000 apache_airflow_providers_hashicorp-3.7.0rc1/airflow/providers/hashicorp/__init__.py
--rw-r--r--   0        0        0      785 2024-01-22 08:28:41.000000 apache_airflow_providers_hashicorp-3.7.0rc1/airflow/providers/hashicorp/_internal_client/__init__.py
--rw-r--r--   0        0        0    21372 2024-01-22 08:28:41.000000 apache_airflow_providers_hashicorp-3.7.0rc1/airflow/providers/hashicorp/_internal_client/vault_client.py
--rw-r--r--   0        0        0     2739 2024-01-22 08:28:41.000000 apache_airflow_providers_hashicorp-3.7.0rc1/airflow/providers/hashicorp/get_provider_info.py
--rw-r--r--   0        0        0      785 2024-01-22 08:28:41.000000 apache_airflow_providers_hashicorp-3.7.0rc1/airflow/providers/hashicorp/hooks/__init__.py
--rw-r--r--   0        0        0    18838 2024-01-22 08:28:41.000000 apache_airflow_providers_hashicorp-3.7.0rc1/airflow/providers/hashicorp/hooks/vault.py
--rw-r--r--   0        0        0      785 2024-01-22 08:28:41.000000 apache_airflow_providers_hashicorp-3.7.0rc1/airflow/providers/hashicorp/secrets/__init__.py
--rw-r--r--   0        0        0    11992 2024-01-22 08:28:41.000000 apache_airflow_providers_hashicorp-3.7.0rc1/airflow/providers/hashicorp/secrets/vault.py
--rw-r--r--   0        0        0     3023 2024-01-22 08:28:41.000000 apache_airflow_providers_hashicorp-3.7.0rc1/pyproject.toml
--rw-r--r--   0        0        0     5817 1970-01-01 00:00:00.000000 apache_airflow_providers_hashicorp-3.7.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     4079 2024-04-30 11:29:25.000000 apache_airflow_providers_hashicorp-3.7.0rc2/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-30 11:29:25.000000 apache_airflow_providers_hashicorp-3.7.0rc2/airflow/providers/hashicorp/LICENSE
+-rw-r--r--   0        0        0     1584 2024-04-30 11:29:25.000000 apache_airflow_providers_hashicorp-3.7.0rc2/airflow/providers/hashicorp/__init__.py
+-rw-r--r--   0        0        0      785 2024-04-30 11:29:25.000000 apache_airflow_providers_hashicorp-3.7.0rc2/airflow/providers/hashicorp/_internal_client/__init__.py
+-rw-r--r--   0        0        0    22534 2024-04-30 11:29:25.000000 apache_airflow_providers_hashicorp-3.7.0rc2/airflow/providers/hashicorp/_internal_client/vault_client.py
+-rw-r--r--   0        0        0     2887 2024-04-30 11:29:25.000000 apache_airflow_providers_hashicorp-3.7.0rc2/airflow/providers/hashicorp/get_provider_info.py
+-rw-r--r--   0        0        0      785 2024-04-30 11:29:25.000000 apache_airflow_providers_hashicorp-3.7.0rc2/airflow/providers/hashicorp/hooks/__init__.py
+-rw-r--r--   0        0        0    18790 2024-04-30 11:29:25.000000 apache_airflow_providers_hashicorp-3.7.0rc2/airflow/providers/hashicorp/hooks/vault.py
+-rw-r--r--   0        0        0      785 2024-04-30 11:29:25.000000 apache_airflow_providers_hashicorp-3.7.0rc2/airflow/providers/hashicorp/secrets/__init__.py
+-rw-r--r--   0        0        0    12245 2024-04-30 11:29:25.000000 apache_airflow_providers_hashicorp-3.7.0rc2/airflow/providers/hashicorp/secrets/vault.py
+-rw-r--r--   0        0        0     3102 2024-04-30 11:29:25.000000 apache_airflow_providers_hashicorp-3.7.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     5941 1970-01-01 00:00:00.000000 apache_airflow_providers_hashicorp-3.7.0rc2/PKG-INFO
```

### Comparing `apache_airflow_providers_hashicorp-3.7.0rc1/README.rst` & `apache_airflow_providers_hashicorp-3.7.0rc2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-hashicorp``
 
-Release: ``3.7.0.rc1``
+Release: ``3.7.0.rc2``
 
 
 Hashicorp including `Hashicorp Vault <https://www.vaultproject.io/>`__
 
 
 Provider package
 ----------------
@@ -60,23 +60,23 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-hashicorp``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.6.0``
+``apache-airflow``  ``>=2.7.0``
 ``hvac``            ``>=1.1.0``
 ==================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
 Those are dependencies that might be needed in order to use all the features of the package.
```

### Comparing `apache_airflow_providers_hashicorp-3.7.0rc1/airflow/providers/hashicorp/LICENSE` & `apache_airflow_providers_hashicorp-3.7.0rc2/airflow/providers/hashicorp/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_hashicorp-3.7.0rc1/airflow/providers/hashicorp/__init__.py` & `apache_airflow_providers_hashicorp-3.7.0rc2/airflow/providers/hashicorp/__init__.py`

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
-        f"The package `apache-airflow-providers-hashicorp:{__version__}` needs Apache Airflow 2.6.0+"
+        f"The package `apache-airflow-providers-hashicorp:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_hashicorp-3.7.0rc1/airflow/providers/hashicorp/_internal_client/__init__.py` & `apache_airflow_providers_hashicorp-3.7.0rc2/airflow/providers/hashicorp/_internal_client/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_hashicorp-3.7.0rc1/airflow/providers/hashicorp/_internal_client/vault_client.py` & `apache_airflow_providers_hashicorp-3.7.0rc2/airflow/providers/hashicorp/_internal_client/vault_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
+import os
 from functools import cached_property
 
 import hvac
 from hvac.api.auth_methods import Kubernetes
 from hvac.exceptions import InvalidPath, VaultError
 from requests import Response, Session
 from requests.adapters import HTTPAdapter
@@ -69,14 +70,17 @@
     :param token_path: path to file containing authentication token to include in requests sent to Vault
         (for ``token`` and ``github`` auth_type).
     :param username: Username for Authentication (for ``ldap`` and ``userpass`` auth_types).
     :param password: Password for Authentication (for ``ldap`` and ``userpass`` auth_types).
     :param key_id: Key ID for Authentication (for ``aws_iam`` and ''azure`` auth_type).
     :param secret_id: Secret ID for Authentication (for ``approle``, ``aws_iam`` and ``azure`` auth_types).
     :param role_id: Role ID for Authentication (for ``approle``, ``aws_iam`` auth_types).
+    :param assume_role_kwargs: AWS assume role param.
+        See AWS STS Docs:
+        https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts/client/assume_role.html
     :param kubernetes_role: Role for Authentication (for ``kubernetes`` auth_type).
     :param kubernetes_jwt_path: Path for kubernetes jwt token (for ``kubernetes`` auth_type, default:
         ``/var/run/secrets/kubernetes.io/serviceaccount/token``).
     :param gcp_key_path: Path to Google Cloud Service Account key file (JSON)  (for ``gcp`` auth_type).
            Mutually exclusive with gcp_keyfile_dict
     :param gcp_keyfile_dict: Dictionary of keyfile parameters. (for ``gcp`` auth_type).
            Mutually exclusive with gcp_key_path
@@ -98,14 +102,15 @@
         kv_engine_version: int | None = None,
         token: str | None = None,
         token_path: str | None = None,
         username: str | None = None,
         password: str | None = None,
         key_id: str | None = None,
         secret_id: str | None = None,
+        assume_role_kwargs: dict | None = None,
         role_id: str | None = None,
         kubernetes_role: str | None = None,
         kubernetes_jwt_path: str | None = "/var/run/secrets/kubernetes.io/serviceaccount/token",
         gcp_key_path: str | None = None,
         gcp_keyfile_dict: dict | None = None,
         gcp_scopes: str | None = None,
         azure_tenant_id: str | None = None,
@@ -121,15 +126,15 @@
                 f"The version is not supported: {kv_engine_version}. "
                 f"It should be one of {VALID_KV_VERSIONS}"
             )
         if auth_type not in VALID_AUTH_TYPES:
             raise VaultError(
                 f"The auth_type is not supported: {auth_type}. It should be one of {VALID_AUTH_TYPES}"
             )
-        if auth_type == "token" and not token and not token_path:
+        if auth_type == "token" and not token and not token_path and "VAULT_TOKEN" not in os.environ:
             raise VaultError("The 'token' authentication type requires 'token' or 'token_path'")
         if auth_type == "github" and not token and not token_path:
             raise VaultError("The 'github' authentication type requires 'token' or 'token_path'")
         if auth_type == "approle" and not role_id:
             raise VaultError("The 'approle' authentication type requires 'role_id'")
         if auth_type == "kubernetes":
             if not kubernetes_role:
@@ -147,23 +152,24 @@
             if not radius_secret:
                 raise VaultError("The 'radius' authentication type requires 'radius_secret'")
 
         self.kv_engine_version = kv_engine_version or 2
         self.url = url
         self.auth_type = auth_type
         self.kwargs = kwargs
-        self.token = token
+        self.token = token or os.getenv("VAULT_TOKEN", None)
         self.token_path = token_path
         self.auth_mount_point = auth_mount_point
         self.mount_point = mount_point
         self.username = username
         self.password = password
         self.key_id = key_id
         self.secret_id = secret_id
         self.role_id = role_id
+        self.assume_role_kwargs = assume_role_kwargs
         self.kubernetes_role = kubernetes_role
         self.kubernetes_jwt_path = kubernetes_jwt_path
         self.gcp_key_path = gcp_key_path
         self.gcp_keyfile_dict = gcp_keyfile_dict
         self.gcp_scopes = gcp_scopes
         self.azure_tenant_id = azure_tenant_id
         self.azure_resource = azure_resource
@@ -313,23 +319,44 @@
                 tenant_id=self.azure_tenant_id,
                 resource=self.azure_resource,
                 client_id=self.key_id,
                 client_secret=self.secret_id,
             )
 
     def _auth_aws_iam(self, _client: hvac.Client) -> None:
+        if self.key_id and self.secret_id:
+            auth_args = {
+                "access_key": self.key_id,
+                "secret_key": self.secret_id,
+                "role": self.role_id,
+            }
+        else:
+            import boto3
+
+            if self.assume_role_kwargs:
+                sts_client = boto3.client("sts")
+                credentials = sts_client.assume_role(**self.assume_role_kwargs)
+                auth_args = {
+                    "access_key": credentials["Credentials"]["AccessKeyId"],
+                    "secret_key": credentials["Credentials"]["SecretAccessKey"],
+                    "session_token": credentials["Credentials"]["SessionToken"],
+                }
+            else:
+                session = boto3.Session()
+                credentials = session.get_credentials()
+                auth_args = {
+                    "access_key": credentials.access_key,
+                    "secret_key": credentials.secret_key,
+                    "session_token": credentials.token,
+                }
+
         if self.auth_mount_point:
-            _client.auth.aws.iam_login(
-                access_key=self.key_id,
-                secret_key=self.secret_id,
-                role=self.role_id,
-                mount_point=self.auth_mount_point,
-            )
-        else:
-            _client.auth.aws.iam_login(access_key=self.key_id, secret_key=self.secret_id, role=self.role_id)
+            auth_args["mount_point"] = self.auth_mount_point
+
+        _client.auth.aws.iam_login(**auth_args)
 
     def _auth_approle(self, _client: hvac.Client) -> None:
         if self.auth_mount_point:
             _client.auth.approle.login(
                 role_id=self.role_id, secret_id=self.secret_id, mount_point=self.auth_mount_point
             )
         else:
@@ -383,15 +410,15 @@
             return None
 
         return_data = response["data"] if self.kv_engine_version == 1 else response["data"]["data"]
         return return_data
 
     def get_secret_metadata(self, secret_path: str) -> dict | None:
         """
-        Reads secret metadata (including versions) from the engine. It is only valid for KV version 2.
+        Read secret metadata (including versions) from the engine. It is only valid for KV version 2.
 
         :param secret_path: The path of the secret.
         :return: secret metadata. This is a Dict containing metadata for the secret.
 
                  See https://hvac.readthedocs.io/en/stable/usage/secrets_engines/kv_v2.html for details.
 
         """
@@ -405,15 +432,15 @@
             self.log.debug("Secret not found %s with mount point %s", secret_path, mount_point)
             return None
 
     def get_secret_including_metadata(
         self, secret_path: str, secret_version: int | None = None
     ) -> dict | None:
         """
-        Reads secret including metadata. It is only valid for KV version 2.
+        Read secret including metadata. It is only valid for KV version 2.
 
         See https://hvac.readthedocs.io/en/stable/usage/secrets_engines/kv_v2.html for details.
 
         :param secret_path: The path of the secret.
         :param secret_version: Specifies the version of Secret to return. If not set, the latest
             version is returned. (Can only be used in case of version 2 of KV).
         :return: The key info. This is a Dict with "data" mapping keeping secret
@@ -439,15 +466,15 @@
             )
             return None
 
     def create_or_update_secret(
         self, secret_path: str, secret: dict, method: str | None = None, cas: int | None = None
     ) -> Response:
         """
-        Creates or updates secret.
+        Create or updates secret.
 
         :param secret_path: The path of the secret.
         :param secret: Secret to create or update for the path specified
         :param method: Optional parameter to explicitly request a POST (create) or PUT (update) request to
             the selected kv secret engine. If no argument is provided for this parameter, hvac attempts to
             intelligently determine which method is appropriate. Only valid for KV engine version 1
         :param cas: Set the "cas" value to use a Check-And-Set operation. If not set the write will be
@@ -463,14 +490,14 @@
         if self.kv_engine_version == 2 and method:
             raise VaultError("The method parameter is only valid for version 1")
         if self.kv_engine_version == 1 and cas:
             raise VaultError("The cas parameter is only valid for version 2")
         mount_point, secret_path = self._parse_secret_path(secret_path)
         if self.kv_engine_version == 1:
             response = self.client.secrets.kv.v1.create_or_update_secret(
-                secret_path=secret_path, secret=secret, mount_point=mount_point, method=method
+                path=secret_path, secret=secret, mount_point=mount_point, method=method
             )
         else:
             response = self.client.secrets.kv.v2.create_or_update_secret(
-                secret_path=secret_path, secret=secret, mount_point=mount_point, cas=cas
+                path=secret_path, secret=secret, mount_point=mount_point, cas=cas
             )
         return response
```

### Comparing `apache_airflow_providers_hashicorp-3.7.0rc1/airflow/providers/hashicorp/get_provider_info.py` & `apache_airflow_providers_hashicorp-3.7.0rc2/airflow/providers/hashicorp/get_provider_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,17 +24,20 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-hashicorp",
         "name": "Hashicorp",
         "description": "Hashicorp including `Hashicorp Vault <https://www.vaultproject.io/>`__\n",
         "state": "ready",
-        "source-date-epoch": 1705912121,
+        "source-date-epoch": 1714476565,
         "versions": [
             "3.7.0",
+            "3.6.4",
+            "3.6.3",
+            "3.6.2",
             "3.6.1",
             "3.6.0",
             "3.5.0",
             "3.4.3",
             "3.4.2",
             "3.4.1",
             "3.4.0",
@@ -51,15 +54,15 @@
             "2.1.1",
             "2.1.0",
             "2.0.0",
             "1.0.2",
             "1.0.1",
             "1.0.0",
         ],
-        "dependencies": ["apache-airflow>=2.6.0", "hvac>=1.1.0"],
+        "dependencies": ["apache-airflow>=2.7.0", "hvac>=1.1.0"],
         "integrations": [
             {
                 "integration-name": "Hashicorp Vault",
                 "external-doc-url": "https://www.vaultproject.io/",
                 "logo": "/integration-logos/hashicorp/Hashicorp-Vault.png",
                 "tags": ["software"],
             }
@@ -73,8 +76,9 @@
         "connection-types": [
             {
                 "hook-class-name": "airflow.providers.hashicorp.hooks.vault.VaultHook",
                 "connection-type": "vault",
             }
         ],
         "secrets-backends": ["airflow.providers.hashicorp.secrets.vault.VaultBackend"],
+        "additional-extras": [{"name": "boto3", "dependencies": ["boto3>=1.33.0"]}],
     }
```

### Comparing `apache_airflow_providers_hashicorp-3.7.0rc1/airflow/providers/hashicorp/hooks/__init__.py` & `apache_airflow_providers_hashicorp-3.7.0rc2/airflow/providers/hashicorp/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_hashicorp-3.7.0rc1/airflow/providers/hashicorp/hooks/vault.py` & `apache_airflow_providers_hashicorp-3.7.0rc2/airflow/providers/hashicorp/hooks/vault.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """Hook for HashiCorp Vault."""
+
 from __future__ import annotations
 
 import json
 import warnings
 from typing import TYPE_CHECKING, Any
 
 from hvac.exceptions import VaultError
@@ -121,15 +122,15 @@
         gcp_scopes: str | None = None,
         azure_tenant_id: str | None = None,
         azure_resource: str | None = None,
         radius_host: str | None = None,
         radius_port: int | None = None,
         **kwargs,
     ):
-        super().__init__(logger_name=kwargs.pop("logger_name", None))
+        super().__init__()
         self.connection = self.get_connection(vault_conn_id)
 
         if not auth_type:
             auth_type = self.connection.extra_dejson.get("auth_type") or "token"
 
         if not auth_mount_point:
             auth_mount_point = self.connection.extra_dejson.get("auth_mount_point")
@@ -286,15 +287,15 @@
                     raise VaultError(f"Radius port was wrong: {radius_port_str}")
         if not radius_host:
             radius_host = self.connection.extra_dejson.get("radius_host")
         return radius_host, radius_port
 
     def get_conn(self) -> hvac.Client:
         """
-        Retrieves connection to Vault.
+        Retrieve connection to Vault.
 
         :return: connection used.
         """
         return self.vault_client.client
 
     def get_secret(self, secret_path: str, secret_version: int | None = None) -> dict | None:
         """
@@ -309,29 +310,29 @@
         :param secret_path: Path of the secret
         :return: secret stored in the vault as a dictionary
         """
         return self.vault_client.get_secret(secret_path=secret_path, secret_version=secret_version)
 
     def get_secret_metadata(self, secret_path: str) -> dict | None:
         """
-        Reads secret metadata (including versions) from the engine. It is only valid for KV version 2.
+        Read secret metadata (including versions) from the engine. It is only valid for KV version 2.
 
         :param secret_path: Path to read from
         :return: secret metadata. This is a Dict containing metadata for the secret.
 
         See https://hvac.readthedocs.io/en/stable/usage/secrets_engines/kv_v2.html for details.
 
         """
         return self.vault_client.get_secret_metadata(secret_path=secret_path)
 
     def get_secret_including_metadata(
         self, secret_path: str, secret_version: int | None = None
     ) -> dict | None:
         """
-        Reads secret including metadata. It is only valid for KV version 2.
+        Read secret including metadata. It is only valid for KV version 2.
 
         See https://hvac.readthedocs.io/en/stable/usage/secrets_engines/kv_v2.html for details.
 
         :param secret_path: Path of the secret
         :param secret_version: Optional version of key to read - can only be used in case of version 2 of KV
         :return: key info. This is a Dict with "data" mapping keeping secret
             and "metadata" mapping keeping metadata of the secret.
@@ -341,15 +342,15 @@
             secret_path=secret_path, secret_version=secret_version
         )
 
     def create_or_update_secret(
         self, secret_path: str, secret: dict, method: str | None = None, cas: int | None = None
     ) -> Response:
         """
-        Creates or updates secret.
+        Create or updates secret.
 
         :param secret_path: Path to read from
         :param secret: Secret to create or update for the path specified
         :param method: Optional parameter to explicitly request a POST (create) or PUT (update) request to
             the selected kv secret engine. If no argument is provided for this parameter, hvac attempts to
             intelligently determine which method is appropriate. Only valid for KV engine version 1
         :param cas: Set the "cas" value to use a Check-And-Set operation. If not set the write will be
@@ -364,15 +365,15 @@
         """
         return self.vault_client.create_or_update_secret(
             secret_path=secret_path, secret=secret, method=method, cas=cas
         )
 
     @classmethod
     def get_connection_form_widgets(cls) -> dict[str, Any]:
-        """Returns connection widgets to add to connection form."""
+        """Return connection widgets to add to connection form."""
         from flask_appbuilder.fieldwidgets import BS3TextFieldWidget
         from flask_babel import lazy_gettext
         from wtforms import BooleanField, IntegerField, StringField
         from wtforms.validators import NumberRange, Optional, any_of
 
         return {
             "auth_type": StringField(lazy_gettext("Auth type"), widget=BS3TextFieldWidget()),
@@ -401,15 +402,15 @@
                 validators=[Optional(), NumberRange(min=0)],
             ),
             "use_tls": BooleanField(lazy_gettext("Use TLS"), default=True),
         }
 
     @classmethod
     def get_ui_field_behaviour(cls) -> dict[str, Any]:
-        """Returns custom field behaviour."""
+        """Return custom field behaviour."""
         return {
             "hidden_fields": ["extra"],
             "relabeling": {},
         }
 
     def test_connection(self) -> tuple[bool, str]:
         """Test Vault connectivity from UI."""
```

### Comparing `apache_airflow_providers_hashicorp-3.7.0rc1/airflow/providers/hashicorp/secrets/__init__.py` & `apache_airflow_providers_hashicorp-3.7.0rc2/airflow/providers/hashicorp/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_hashicorp-3.7.0rc1/airflow/providers/hashicorp/secrets/vault.py` & `apache_airflow_providers_hashicorp-3.7.0rc2/airflow/providers/hashicorp/secrets/vault.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """Objects relating to sourcing connections & variables from Hashicorp Vault."""
+
 from __future__ import annotations
 
-import warnings
 from typing import TYPE_CHECKING
 
+from deprecated import deprecated
+
 from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.providers.hashicorp._internal_client.vault_client import _VaultClient
 from airflow.secrets import BaseSecretsBackend
 from airflow.utils.log.logging_mixin import LoggingMixin
 
 
 class VaultBackend(BaseSecretsBackend, LoggingMixin):
@@ -68,14 +70,17 @@
     :param token_path: path to file containing authentication token to include in requests sent to Vault
         (for ``token`` and ``github`` auth_type).
     :param username: Username for Authentication (for ``ldap`` and ``userpass`` auth_type).
     :param password: Password for Authentication (for ``ldap`` and ``userpass`` auth_type).
     :param key_id: Key ID for Authentication (for ``aws_iam`` and ''azure`` auth_type).
     :param secret_id: Secret ID for Authentication (for ``approle``, ``aws_iam`` and ``azure`` auth_types).
     :param role_id: Role ID for Authentication (for ``approle``, ``aws_iam`` auth_types).
+    :param assume_role_kwargs: AWS assume role param.
+        See AWS STS Docs:
+        https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts/client/assume_role.html
     :param kubernetes_role: Role for Authentication (for ``kubernetes`` auth_type).
     :param kubernetes_jwt_path: Path for kubernetes jwt token (for ``kubernetes`` auth_type, default:
         ``/var/run/secrets/kubernetes.io/serviceaccount/token``).
     :param gcp_key_path: Path to Google Cloud Service Account key file (JSON) (for ``gcp`` auth_type).
            Mutually exclusive with gcp_keyfile_dict.
     :param gcp_keyfile_dict: Dictionary of keyfile parameters. (for ``gcp`` auth_type).
            Mutually exclusive with gcp_key_path.
@@ -101,14 +106,15 @@
         token: str | None = None,
         token_path: str | None = None,
         username: str | None = None,
         password: str | None = None,
         key_id: str | None = None,
         secret_id: str | None = None,
         role_id: str | None = None,
+        assume_role_kwargs: dict | None = None,
         kubernetes_role: str | None = None,
         kubernetes_jwt_path: str = "/var/run/secrets/kubernetes.io/serviceaccount/token",
         gcp_key_path: str | None = None,
         gcp_keyfile_dict: dict | None = None,
         gcp_scopes: str | None = None,
         azure_tenant_id: str | None = None,
         azure_resource: str | None = None,
@@ -141,14 +147,15 @@
             token=token,
             token_path=token_path,
             username=username,
             password=password,
             key_id=key_id,
             secret_id=secret_id,
             role_id=role_id,
+            assume_role_kwargs=assume_role_kwargs,
             kubernetes_role=kubernetes_role,
             kubernetes_jwt_path=kubernetes_jwt_path,
             gcp_key_path=gcp_key_path,
             gcp_keyfile_dict=gcp_keyfile_dict,
             gcp_scopes=gcp_scopes,
             azure_tenant_id=azure_tenant_id,
             azure_resource=azure_resource,
@@ -180,29 +187,27 @@
             secret_path = conn_key
         else:
             secret_path = self.build_path(self.connections_path, conn_key)
         return self.vault_client.get_secret(
             secret_path=(mount_point + "/" if mount_point else "") + secret_path
         )
 
+    @deprecated(
+        reason="Method `VaultBackend.get_conn_uri` is deprecated and will be removed in a future release.",
+        category=AirflowProviderDeprecationWarning,
+    )
     def get_conn_uri(self, conn_id: str) -> str | None:
         """
         Get serialized representation of connection.
 
         :param conn_id: The connection id
         :return: The connection uri retrieved from the secret
         """
         # Since VaultBackend implements `get_connection`, `get_conn_uri` is not used. So we
         # don't need to implement (or direct users to use) method `get_conn_value` instead
-        warnings.warn(
-            f"Method `{self.__class__.__name__}.get_conn_uri` is deprecated and will be removed "
-            "in a future release.",
-            AirflowProviderDeprecationWarning,
-            stacklevel=2,
-        )
         response = self.get_response(conn_id)
         return response.get("conn_uri") if response else None
 
     # Make sure connection is imported this way for type checking, otherwise when importing
     # the backend it will get a circular dependency and fail
     if TYPE_CHECKING:
         from airflow.models.connection import Connection
```

### Comparing `apache_airflow_providers_hashicorp-3.7.0rc1/pyproject.toml` & `apache_airflow_providers_hashicorp-3.7.0rc2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-hashicorp"
-version = "3.7.0.rc1"
+version = "3.7.0.rc2"
 description = "Provider package apache-airflow-providers-hashicorp for Apache Airflow"
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
     "hvac>=1.1.0",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-hashicorp/3.7.0"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-hashicorp/3.7.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
@@ -70,10 +71,13 @@
 
 [project.entry-points."apache_airflow_provider"]
 provider_info = "airflow.providers.hashicorp.get_provider_info:get_provider_info"
 [project.optional-dependencies]
 "google" = [
     "apache-airflow-providers-google",
 ]
+"boto3" = [
+    "boto3>=1.33.0",
+]
 
 [tool.flit.module]
 name = "airflow.providers.hashicorp"
```

### Comparing `apache_airflow_providers_hashicorp-3.7.0rc1/PKG-INFO` & `apache_airflow_providers_hashicorp-3.7.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-hashicorp
-Version: 3.7.0rc1
+Version: 3.7.0rc2
 Summary: Provider package apache-airflow-providers-hashicorp for Apache Airflow
 Keywords: airflow-provider,hashicorp,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,25 +15,28 @@
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
 Requires-Dist: hvac>=1.1.0
+Requires-Dist: boto3>=1.33.0 ; extra == "boto3"
 Requires-Dist: apache-airflow-providers-google ; extra == "google"
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-hashicorp/3.7.0/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-hashicorp/3.7.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
+Provides-Extra: boto3
 Provides-Extra: google
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
    distributed with this work for additional information
    regarding copyright ownership.  The ASF licenses this file
@@ -72,15 +75,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-hashicorp``
 
-Release: ``3.7.0.rc1``
+Release: ``3.7.0.rc2``
 
 
 Hashicorp including `Hashicorp Vault <https://www.vaultproject.io/>`__
 
 
 Provider package
 ----------------
@@ -94,23 +97,23 @@
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-hashicorp``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.6.0``
+``apache-airflow``  ``>=2.7.0``
 ``hvac``            ``>=1.1.0``
 ==================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
 Those are dependencies that might be needed in order to use all the features of the package.
```

