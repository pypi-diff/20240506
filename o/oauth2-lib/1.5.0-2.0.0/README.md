# Comparing `tmp/oauth2_lib-1.5.0.tar.gz` & `tmp/oauth2_lib-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oauth2_lib-1.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "oauth2_lib-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `oauth2_lib-1.5.0.tar` & `oauth2_lib-2.0.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      364 2024-01-19 10:25:41.166876 oauth2_lib-1.5.0/.bumpversion.cfg
--rw-r--r--   0        0        0      502 2024-01-19 10:25:41.166876 oauth2_lib-1.5.0/.github/workflows/dependabot.yml
--rw-r--r--   0        0        0      550 2024-01-19 10:25:41.166876 oauth2_lib-1.5.0/.github/workflows/publish-release.yml
--rw-r--r--   0        0        0      389 2024-01-19 10:25:41.166876 oauth2_lib-1.5.0/.github/workflows/pull-request.yml
--rw-r--r--   0        0        0     1894 2024-01-19 10:25:41.166876 oauth2_lib-1.5.0/.github/workflows/scheduled-build.yml
--rw-r--r--   0        0        0     1649 2024-01-19 10:25:41.166876 oauth2_lib-1.5.0/.github/workflows/test-package.yml
--rw-r--r--   0        0        0     1115 2024-01-19 10:25:41.166876 oauth2_lib-1.5.0/.gitignore
--rw-r--r--   0        0        0     1790 2024-01-19 10:25:41.166876 oauth2_lib-1.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1150 2024-01-19 10:25:41.166876 oauth2_lib-1.5.0/.stignore
--rw-r--r--   0        0        0    11358 2024-01-19 10:25:41.166876 oauth2_lib-1.5.0/LICENSE
--rw-r--r--   0        0        0     1848 2024-01-19 10:25:41.166876 oauth2_lib-1.5.0/README.md
--rwxr-xr-x   0        0        0      150 2024-01-19 10:25:41.166876 oauth2_lib-1.5.0/fmt_code.sh
--rw-r--r--   0        0        0      671 2024-01-19 10:25:41.166876 oauth2_lib-1.5.0/oauth2_lib/__init__.py
--rw-r--r--   0        0        0     5285 2024-01-19 10:25:41.166876 oauth2_lib-1.5.0/oauth2_lib/async_api_client.py
--rw-r--r--   0        0        0    15803 2024-01-19 10:25:41.166876 oauth2_lib-1.5.0/oauth2_lib/fastapi.py
--rw-r--r--   0        0        0        0 2024-01-19 10:25:41.166876 oauth2_lib-1.5.0/oauth2_lib/py.typed
--rw-r--r--   0        0        0     1240 2024-01-19 10:25:41.166876 oauth2_lib-1.5.0/oauth2_lib/settings.py
--rw-r--r--   0        0        0     8504 2024-01-19 10:25:41.166876 oauth2_lib-1.5.0/oauth2_lib/strawberry.py
--rw-r--r--   0        0        0     2868 2024-01-19 10:25:41.166876 oauth2_lib-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     1203 2024-01-19 10:25:41.166876 oauth2_lib-1.5.0/setup.cfg
--rw-r--r--   0        0        0        0 2024-01-19 10:25:41.166876 oauth2_lib-1.5.0/tests/__init__.py
--rw-r--r--   0        0        0     1540 2024-01-19 10:25:41.166876 oauth2_lib-1.5.0/tests/conftest.py
--rw-r--r--   0        0        0     2783 2024-01-19 10:25:41.166876 oauth2_lib-1.5.0/tests/strawberry/conftest.py
--rw-r--r--   0        0        0     1541 2024-01-19 10:25:41.166876 oauth2_lib-1.5.0/tests/strawberry/test_authenticated_federated_field.py
--rw-r--r--   0        0        0     2360 2024-01-19 10:25:41.166876 oauth2_lib-1.5.0/tests/strawberry/test_authenticated_field.py
--rw-r--r--   0        0        0     3052 2024-01-19 10:25:41.166876 oauth2_lib-1.5.0/tests/strawberry/test_authenticated_mutation_field.py
--rw-r--r--   0        0        0     5708 2024-01-19 10:25:41.166876 oauth2_lib-1.5.0/tests/test_async_api_client.py
--rw-r--r--   0        0        0    15923 2024-01-19 10:25:41.170876 oauth2_lib-1.5.0/tests/test_fastapi.py
--rw-r--r--   0        0        0     6695 2024-01-19 10:25:41.170876 oauth2_lib-1.5.0/tests/test_opa_decision.py
--rw-r--r--   0        0        0     5243 2024-01-19 10:25:41.170876 oauth2_lib-1.5.0/tests/test_opa_graphql_decision.py
--rw-r--r--   0        0        0     4172 1970-01-01 00:00:00.000000 oauth2_lib-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0      364 2024-05-06 07:49:34.717384 oauth2_lib-2.0.0/.bumpversion.cfg
+-rw-r--r--   0        0        0      502 2024-05-06 07:49:34.717384 oauth2_lib-2.0.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      550 2024-05-06 07:49:34.717384 oauth2_lib-2.0.0/.github/workflows/publish-release.yml
+-rw-r--r--   0        0        0      389 2024-05-06 07:49:34.717384 oauth2_lib-2.0.0/.github/workflows/pull-request.yml
+-rw-r--r--   0        0        0     1894 2024-05-06 07:49:34.717384 oauth2_lib-2.0.0/.github/workflows/scheduled-build.yml
+-rw-r--r--   0        0        0     2302 2024-05-06 07:49:34.717384 oauth2_lib-2.0.0/.github/workflows/test-package.yml
+-rw-r--r--   0        0        0     1115 2024-05-06 07:49:34.717384 oauth2_lib-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1790 2024-05-06 07:49:34.717384 oauth2_lib-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1150 2024-05-06 07:49:34.717384 oauth2_lib-2.0.0/.stignore
+-rw-r--r--   0        0        0    11358 2024-05-06 07:49:34.717384 oauth2_lib-2.0.0/LICENSE
+-rw-r--r--   0        0        0     2004 2024-05-06 07:49:34.717384 oauth2_lib-2.0.0/README.md
+-rwxr-xr-x   0        0        0      150 2024-05-06 07:49:34.717384 oauth2_lib-2.0.0/fmt_code.sh
+-rw-r--r--   0        0        0      671 2024-05-06 07:49:34.717384 oauth2_lib-2.0.0/oauth2_lib/__init__.py
+-rw-r--r--   0        0        0     5285 2024-05-06 07:49:34.717384 oauth2_lib-2.0.0/oauth2_lib/async_api_client.py
+-rw-r--r--   0        0        0    16732 2024-05-06 07:49:34.717384 oauth2_lib-2.0.0/oauth2_lib/fastapi.py
+-rw-r--r--   0        0        0        0 2024-05-06 07:49:34.717384 oauth2_lib-2.0.0/oauth2_lib/py.typed
+-rw-r--r--   0        0        0     1433 2024-05-06 07:49:34.717384 oauth2_lib-2.0.0/oauth2_lib/settings.py
+-rw-r--r--   0        0        0     8450 2024-05-06 07:49:34.717384 oauth2_lib-2.0.0/oauth2_lib/strawberry.py
+-rw-r--r--   0        0        0     2823 2024-05-06 07:49:34.717384 oauth2_lib-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1203 2024-05-06 07:49:34.717384 oauth2_lib-2.0.0/setup.cfg
+-rw-r--r--   0        0        0        0 2024-05-06 07:49:34.717384 oauth2_lib-2.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     5118 2024-05-06 07:49:34.717384 oauth2_lib-2.0.0/tests/conftest.py
+-rw-r--r--   0        0        0     2950 2024-05-06 07:49:34.721384 oauth2_lib-2.0.0/tests/strawberry/conftest.py
+-rw-r--r--   0        0        0     2502 2024-05-06 07:49:34.721384 oauth2_lib-2.0.0/tests/strawberry/test_authenticated_federated_field.py
+-rw-r--r--   0        0        0     4185 2024-05-06 07:49:34.721384 oauth2_lib-2.0.0/tests/strawberry/test_authenticated_field.py
+-rw-r--r--   0        0        0     3316 2024-05-06 07:49:34.721384 oauth2_lib-2.0.0/tests/strawberry/test_authenticated_mutation_field.py
+-rw-r--r--   0        0        0     5708 2024-05-06 07:49:34.721384 oauth2_lib-2.0.0/tests/test_async_api_client.py
+-rw-r--r--   0        0        0    11434 2024-05-06 07:49:34.721384 oauth2_lib-2.0.0/tests/test_fastapi.py
+-rw-r--r--   0        0        0     8043 2024-05-06 07:49:34.721384 oauth2_lib-2.0.0/tests/test_opa_decision.py
+-rw-r--r--   0        0        0     6712 2024-05-06 07:49:34.721384 oauth2_lib-2.0.0/tests/test_opa_graphql_decision.py
+-rw-r--r--   0        0        0     4257 1970-01-01 00:00:00.000000 oauth2_lib-2.0.0/PKG-INFO
```

### Comparing `oauth2_lib-1.5.0/.github/workflows/publish-release.yml` & `oauth2_lib-2.0.0/.github/workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.5.0/.github/workflows/scheduled-build.yml` & `oauth2_lib-2.0.0/.github/workflows/scheduled-build.yml`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.5.0/.github/workflows/test-package.yml` & `oauth2_lib-2.0.0/.github/workflows/test-package.yml`

 * *Files 18% similar despite different names*

```diff
@@ -11,15 +11,14 @@
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ['3.9', '3.10', '3.11', '3.12']
         pydantic-version: ['1.*', '2.*']
       fail-fast: false
-
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
@@ -37,15 +36,41 @@
         run: |
           mypy -p oauth2_lib
       - name: License headers
         run: |
           apache-license-check --copyright "2019-`date +%Y` SURF" oauth2_lib
       - name: Test with pytest
         run: |
-          pytest -vvv --cov-branch --cov-fail-under=80 --cov=oauth2_lib --cov-config=.coveragerc --junitxml=report-pytest-${{ matrix.python-version }}.xml
+          pytest -vvv --cov-branch --cov-fail-under=80 --cov=oauth2_lib --cov-config=.coveragerc
+        env:
+          COVERAGE_FILE: reports/.coverage.${{ matrix.python-version }}
       - name: Upload pytest test results
         uses: actions/upload-artifact@v2
         with:
-          name: pytest-results-${{ matrix.python-version }}
-          path: report-pytest-${{ matrix.python-version }}.xml
+          name: reports
+          path: reports
         # Use always() to always run this step to publish test results when there are test failures
         if: ${{ matrix.pydantic-version == '2.*' }} && ${{ always() }}
+  coverage-combine:
+    needs: [build]
+    runs-on: ubuntu-latest
+    steps:
+      - uses: actions/checkout@v3
+      - uses: actions/setup-python@v5
+        with:
+          python-version: '3.8'
+      - name: Get coverage files
+        uses: actions/download-artifact@v3
+        with:
+          name: reports
+          path: reports
+      - run: pip install coverage[toml]
+      - run: ls -la reports
+      - run: coverage combine reports
+      - run: coverage report
+      - run: coverage xml
+      - name: "Upload coverage to Codecov"
+        uses: codecov/codecov-action@v3
+        with:
+          token: ${{ secrets.CODECOV_TOKEN }}
+          fail_ci_if_error: true
+          files: ./coverage.xml
```

### Comparing `oauth2_lib-1.5.0/.gitignore` & `oauth2_lib-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.5.0/.pre-commit-config.yaml` & `oauth2_lib-2.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.5.0/.stignore` & `oauth2_lib-2.0.0/.stignore`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.5.0/LICENSE` & `oauth2_lib-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.5.0/README.md` & `oauth2_lib-2.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # OAuth2-lib
 
 [![pypi_version](https://img.shields.io/pypi/v/oauth2-lib?color=%2334D058&label=pypi%20package)](https://pypi.org/project/oauth2-lib)
 [![Supported python versions](https://img.shields.io/pypi/pyversions/oauth2-lib.svg?color=%2334D058)](https://pypi.org/project/oauth2-lib)
+[![codecov](https://codecov.io/gh/workfloworchestrator/oauth2-lib/graph/badge.svg?token=JDMMBBOVM4)](https://codecov.io/gh/workfloworchestrator/oauth2-lib)
 
 This Project contains a Mixin class that wraps an openapi-codegen python client, to inject Opentelemetry spans
 and api call retries. It also contains a number of FastAPI dependencies which enables Policy enforcement offloading
 to Open Policy Agent.
 
 The project contains a number of OIDC classes that are tailored to the SURF environment.
```

### Comparing `oauth2_lib-1.5.0/oauth2_lib/__init__.py` & `oauth2_lib-2.0.0/oauth2_lib/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """This is the SURF Oauth2 module that interfaces with the oauth2 setup."""
 
-__version__ = "1.5.0"
+__version__ = "2.0.0"
```

### Comparing `oauth2_lib-1.5.0/oauth2_lib/async_api_client.py` & `oauth2_lib-2.0.0/oauth2_lib/async_api_client.py`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.5.0/oauth2_lib/fastapi.py` & `oauth2_lib-2.0.0/oauth2_lib/fastapi.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import re
 import ssl
-from collections.abc import AsyncGenerator, Awaitable, Mapping
+from abc import ABC, abstractmethod
+from collections.abc import Awaitable, Mapping
 from http import HTTPStatus
 from json import JSONDecodeError
 from typing import Any, Callable, Optional, Union, cast
 
-from fastapi.exceptions import HTTPException
-from fastapi.param_functions import Depends
+from fastapi import HTTPException
 from fastapi.requests import Request
 from fastapi.security.http import HTTPBearer
-from httpx import AsyncClient, BasicAuth, NetworkError
+from httpx import AsyncClient, NetworkError
 from pydantic import BaseModel
-from starlette.requests import ClientDisconnect
+from starlette.requests import ClientDisconnect, HTTPConnection
+from starlette.websockets import WebSocket
 from structlog import get_logger
 
 from oauth2_lib.settings import oauth2lib_settings
 
 logger = get_logger(__name__)
 
 HTTPX_SSL_CONTEXT = ssl.create_default_context()  # https://github.com/encode/httpx/issues/838
@@ -67,87 +67,31 @@
         try:
             return object.__getattribute__(self, key)
         except AttributeError as error:
             if key in self.REGISTERED_CLAIMS:
                 return self.get(key)
             raise error
 
-    """
-    Below this line are SURFnet specific properties that are used often in code to either display or check on.
-    """
-
     @property
     def user_name(self) -> str:
-        if "user_name" in self.keys():
-            return cast(str, self["user_name"])
-        if "unspecified_id" in self.keys():
-            return cast(str, self["unspecified_id"])
         return ""
 
-    @property
-    def display_name(self) -> str:
-        return self.get("display_name", "")  # type: ignore
-
-    @property
-    def principal_name(self) -> str:
-        return self.get("eduperson_principal_name", "")  # type: ignore
-
-    @property
-    def memberships(self) -> list[str]:
-        return self.get("edumember_is_member_of", [])  # type: ignore
-
-    @property
-    def teams(self) -> set[str]:
-        prefix = "urn:collab:group:surfteams.nl:nl:surfnet:diensten:"
-        length = len(prefix)
-        return {urn[length:] for urn in self.memberships if urn.startswith(prefix)}
-
-    @property
-    def entitlements(self) -> list[str]:
-        return self.get("eduperson_entitlement", [])  # type: ignore
-
-    @property
-    def roles(self) -> set[str]:
-        prefix = "urn:mace:surfnet.nl:surfnet.nl:sab:role:"
-        length = len(prefix)
-        return {urn[length:] for urn in self.entitlements if urn.startswith(prefix)}
-
-    @property
-    def organization_codes(self) -> set[str]:
-        prefix = "urn:mace:surfnet.nl:surfnet.nl:sab:organizationCode:"
-        length = len(prefix)
-        return {urn[length:] for urn in self.entitlements if urn.startswith(prefix)}
 
-    @property
-    def organization_guids(self) -> set[str]:
-        prefix = "urn:mace:surfnet.nl:surfnet.nl:sab:organizationGUID:"
-        length = len(prefix)
-        return {urn[length:] for urn in self.entitlements if urn.startswith(prefix)}
+RequestPath = str
+AuthenticationFunc = Callable[[HTTPConnection, Optional[str]], Awaitable[Optional[dict]]]
+AuthorizationFunc = Callable[[HTTPConnection, OIDCUserModel], Awaitable[bool]]
+GraphqlAuthorizationFunc = Callable[[RequestPath, OIDCUserModel], Awaitable[Optional[bool]]]
 
-    @property
-    def scopes(self) -> set[str]:
-        if isinstance(self.get("scope"), list):
-            return set(self.get("scope"))  # type: ignore
-        return set(re.split("[ ,]", self.get("scope", "")))
-
-    @property
-    def is_resource_server(self) -> bool:
-        return self.get("is_resource_server", False)  # type: ignore
 
-    @property
-    def surf_crm_id(self) -> str:
-        return self.get("surf-crm-id", "")  # type: ignore
-
-
-async def _make_async_client() -> AsyncGenerator[AsyncClient, None]:
-    async with AsyncClient(http1=True, verify=HTTPX_SSL_CONTEXT) as client:
-        yield client
+class OIDCConfig(BaseModel):
+    """Holds OpenID Connect provider configuration.
 
+    Details include endpoints, supported features, and various supported specifications.
+    """
 
-class OIDCConfig(BaseModel):
     issuer: str
     authorization_endpoint: str
     token_endpoint: str
     userinfo_endpoint: str
     introspect_endpoint: Optional[str] = None
     introspection_endpoint: Optional[str] = None
     jwks_uri: str
@@ -161,194 +105,235 @@
     claims_supported: list[str]
     claims_parameter_supported: bool
     request_parameter_supported: bool
     code_challenge_methods_supported: list[str]
 
 
 class OPAResult(BaseModel):
+    """Represents an OPA decision result.
+
+    Contains the decision outcome and an associated decision ID.
+    """
+
     result: bool = False
     decision_id: str
 
 
-class OIDCUser(HTTPBearer):
-    """OIDCUser class extends the HTTPBearer class to do extra verification.
+class Authentication(ABC):
+    """Abstract base for authentication mechanisms.
+
+    Requires an async authenticate method implementation.
+    """
+
+    @abstractmethod
+    async def authenticate(self, request: HTTPConnection, token: Optional[str] = None) -> Optional[dict]:
+        """Authenticate the user."""
+        pass
+
+
+class IdTokenExtractor(ABC):
+    """Abstract base for ID token extraction.
+
+    Must implement an async method to extract the token from requests.
+    """
+
+    @abstractmethod
+    async def extract(self, request: Request) -> Optional[str]:
+        pass
+
+
+class HttpBearerExtractor(IdTokenExtractor):
+    """Extracts bearer tokens using FastAPI's HTTPBearer.
 
-    The class will act as follows:
-        1. Validate the Credentials at SURFconext by calling the UserInfo endpoint
-        2. When receiving an active token it will enrich the response through the database roles
+    Specifically designed for HTTP Authorization header token extraction.
     """
 
-    openid_config: Union[OIDCConfig, None] = None
-    openid_url: str
-    resource_server_id: str
-    resource_server_secret: str
+    async def extract(self, request: Request) -> Optional[str]:
+        http_bearer = HTTPBearer(auto_error=True)
+        credential = await http_bearer(request)
+
+        return credential.credentials if credential else None
+
+
+class OIDCAuth(Authentication):
+    """Implements OIDC authentication.
+
+    Manages token extraction and user information retrieval based on OIDC standards.
+    """
 
     def __init__(
         self,
         openid_url: str,
+        openid_config_url: str,
         resource_server_id: str,
         resource_server_secret: str,
-        auto_error: bool = True,
-        scheme_name: Union[str, None] = None,
+        oidc_user_model_cls: type[OIDCUserModel],
+        id_token_extractor: Optional[IdTokenExtractor] = None,
     ):
-        super().__init__(auto_error=auto_error)
+        if not id_token_extractor:
+            self.id_token_extractor = HttpBearerExtractor()
+
         self.openid_url = openid_url
+        self.openid_config_url = openid_config_url
         self.resource_server_id = resource_server_id
         self.resource_server_secret = resource_server_secret
-        self.scheme_name = scheme_name or self.__class__.__name__
+        self.user_model_cls = oidc_user_model_cls
 
-    async def __call__(self, request: Request, token: Union[str, None] = None) -> Union[OIDCUserModel, None]:  # type: ignore
+        self.openid_config: Optional[OIDCConfig] = None
+
+    async def authenticate(self, request: HTTPConnection, token: Optional[str] = None) -> Optional[OIDCUserModel]:
         """Return the OIDC user from OIDC introspect endpoint.
 
         This is used as a security module in Fastapi projects
 
         Args:
-            request: Starlette request method.
+            request: Starlette request/websocket method.
             token: Optional value to directly pass a token.
 
         Returns:
             OIDCUserModel object.
 
         """
         if not oauth2lib_settings.OAUTH2_ACTIVE:
             return None
 
-        async with AsyncClient(http1=True, verify=HTTPX_SSL_CONTEXT) as async_request:
-            await self.check_openid_config(async_request)
+        async with AsyncClient(http1=True, verify=HTTPX_SSL_CONTEXT) as async_client:
+            await self.check_openid_config(async_client)
 
-            if token is None:
-                credentials = await super().__call__(request)
-                if not credentials:
-                    return None
-                token_or_credentials = credentials.credentials
+            # Handle WebSocket requests separately only to check for token presence.
+            if isinstance(request, WebSocket):
+                if token is None:
+                    raise HTTPException(
+                        status_code=HTTPStatus.FORBIDDEN,
+                        detail="Not authenticated",
+                    )
+                token_or_extracted_id_token = token
             else:
-                token_or_credentials = token
-
-            user_info = await self.introspect_token(async_request, token_or_credentials)
-
-            if "active" not in user_info:
-                logger.error("Token doesn't have the mandatory 'active' key, probably caused by a caching problem")
-                raise HTTPException(status_code=HTTPStatus.UNAUTHORIZED, detail="Missing active key")
-            if not user_info.get("active", False):
-                logger.info("User is not active", url=request.url, user_info=user_info)
-                raise HTTPException(status_code=HTTPStatus.UNAUTHORIZED, detail="User is not active")
+                request = cast(Request, request)
+                if token is None:
+                    extracted_id_token = await self.id_token_extractor.extract(request)
+                    if not extracted_id_token:
+                        return None
+                    token_or_extracted_id_token = extracted_id_token
+                elif await self.is_bypassable_request(request):
+                    return None
+                else:
+                    token_or_extracted_id_token = token
 
+            user_info: OIDCUserModel = await self.userinfo(async_client, token_or_extracted_id_token)
             logger.debug("OIDCUserModel object.", user_info=user_info)
             return user_info
 
-    async def check_openid_config(self, async_request: AsyncClient) -> None:
+    @staticmethod
+    async def is_bypassable_request(request: Request) -> bool:
+        """By default no request is bypassable."""
+        return False
+
+    async def userinfo(self, async_request: AsyncClient, token: str) -> OIDCUserModel:
+        """Get the userinfo from the openid server.
+
+        :param AsyncClient async_request: The async request
+        :param str token: the access_token
+        :return: OIDCUserModel dict: OIDC user model from openid server
+
+        """
+        raise NotImplementedError()
+
+    async def check_openid_config(self, async_client: AsyncClient) -> None:
         """Check of openid config is loaded and load if not."""
         if self.openid_config is not None:
             return
 
-        response = await async_request.get(self.openid_url + "/.well-known/openid-configuration")
+        response = await async_client.get(self.openid_config_url)
+        if response.status_code != HTTPStatus.OK:
+            raise HTTPException(
+                status_code=HTTPStatus.SERVICE_UNAVAILABLE,
+                detail=f"Could not load openid config from {self.openid_config_url}",
+            )
         self.openid_config = OIDCConfig.parse_obj(response.json())
 
-    async def introspect_token(self, async_request: AsyncClient, token: str) -> OIDCUserModel:
-        """Introspect the access token to retrieve the user info.
 
-        Args:
-            async_request: The async request
-            token: the access_token
-
-        Returns:
-            OIDCUserModel from openid server
+class Authorization(ABC):
+    """Defines the authorization logic interface.
 
-        """
-        await self.check_openid_config(async_request)
-        assert self.openid_config
-
-        endpoint = self.openid_config.introspect_endpoint or self.openid_config.introspection_endpoint or ""
-        response = await async_request.post(
-            endpoint,
-            params={"token": token},
-            data={"token": token},
-            auth=BasicAuth(self.resource_server_id, self.resource_server_secret),
-            headers={"Content-Type": "application/x-www-form-urlencoded"},
-        )
+    Implementations must provide an async method to authorize based on request and user info.
+    """
 
-        try:
-            data = dict(response.json())
-        except JSONDecodeError:
-            logger.debug(
-                "Unable to parse introspect response",
-                detail=response.text,
-                resource_server_id=self.resource_server_id,
-                openid_url=self.openid_url,
-            )
-            raise HTTPException(status_code=HTTPStatus.UNAUTHORIZED, detail=response.text)
-        logger.debug("Response from openid introspect", response=data)
+    @abstractmethod
+    async def authorize(self, request: HTTPConnection, user: OIDCUserModel) -> Optional[bool]:
+        pass
 
-        if response.status_code not in range(200, 300):
-            logger.debug(
-                "Introspect cannot find an active token, user unauthorized",
-                detail=response.text,
-                resource_server_id=self.resource_server_id,
-                openid_url=self.openid_url,
-            )
-            raise HTTPException(status_code=HTTPStatus.UNAUTHORIZED, detail=response.text)
 
-        return OIDCUserModel(data)
+class GraphqlAuthorization(ABC):
+    """Defines the graphql authorization logic interface.
 
+    Implementations must provide an async method to authorize based on request and user info.
+    """
 
-async def _get_decision(async_request: AsyncClient, opa_url: str, opa_input: dict) -> OPAResult:
-    logger.debug("Posting input json to Policy agent", opa_url=opa_url, input=opa_input)
-    try:
-        result = await async_request.post(opa_url, json=opa_input)
-    except (NetworkError, TypeError) as exc:
-        logger.debug("Could not get decision from policy agent", error=str(exc))
-        raise HTTPException(status_code=HTTPStatus.SERVICE_UNAVAILABLE, detail="Policy agent is unavailable")
+    @abstractmethod
+    async def authorize(self, request: RequestPath, user: OIDCUserModel) -> Optional[bool]:
+        pass
 
-    return OPAResult.parse_obj(result.json())
 
+class OPAMixin:
+    """Base for OPA-based authorization logic.
 
-def _evaluate_decision(decision: OPAResult, auto_error: bool, **context: dict[str, Any]) -> bool:
-    did = decision.decision_id
+    Supports getting and evaluating OPA policy decisions.
+    """
 
-    if decision.result:
-        logger.debug("User is authorized to access the resource", decision_id=did, **context)
-        return True
+    def __init__(self, opa_url: str, auto_error: bool = True, opa_kwargs: Union[Mapping[str, Any], None] = None):
+        self.opa_url = opa_url
+        self.auto_error = auto_error
+        self.opa_kwargs = opa_kwargs
 
-    logger.debug("User is not allowed to access the resource", decision_id=did, **context)
-    if not auto_error:
-        return False
+    async def get_decision(self, async_client: AsyncClient, opa_input: dict) -> OPAResult:
+        logger.debug("Posting input json to Policy agent", opa_url=self.opa_url, input=opa_input)
+        try:
+            result = await async_client.post(self.opa_url, json=opa_input)
+        except (NetworkError, TypeError) as exc:
+            logger.debug("Could not get decision from policy agent", error=str(exc))
+            raise HTTPException(status_code=HTTPStatus.SERVICE_UNAVAILABLE, detail="Policy agent is unavailable")
+
+        json_result = result.json()
+        logger.debug("Received decision from policy agent", decision=json_result)
+        return OPAResult.parse_obj(json_result)
+
+    def evaluate_decision(self, decision: OPAResult, **context: dict[str, Any]) -> bool:
+        did = decision.decision_id
+
+        if decision.result:
+            logger.debug("User is authorized to access the resource", decision_id=did, **context)
+            return True
+
+        logger.debug("User is not allowed to access the resource", decision_id=did, **context)
+        if not self.auto_error:
+            return False
+
+        raise HTTPException(
+            status_code=HTTPStatus.FORBIDDEN,
+            detail=f"User is not allowed to access resource: {context.get('resource')} Decision was taken with id: {did}",
+        )
 
-    raise HTTPException(
-        status_code=HTTPStatus.FORBIDDEN,
-        detail=f"User is not allowed to access resource: {context.get('resource')} Decision was taken with id: {did}",
-    )
-
-
-def opa_decision(
-    opa_url: str,
-    oidc_security: OIDCUser,
-    auto_error: bool = True,
-    opa_kwargs: Union[Mapping[str, str], None] = None,
-) -> Callable[[Request, OIDCUserModel, AsyncClient], Awaitable[Union[bool, None]]]:
-    async def _opa_decision(
-        request: Request,
-        user_info: OIDCUserModel = Depends(oidc_security),
-        async_request: AsyncClient = Depends(_make_async_client),
-    ) -> Union[bool, None]:
-        """Check OIDCUserModel against the OPA policy.
 
-        This is used as a security module in Fastapi projects
-        This method will make an async call towards the Policy agent.
+class OPAAuthorization(Authorization, OPAMixin):
+    """Applies OPA decisions to HTTP requests for authorization.
 
-        Args:
-            request: Request object that will be used to retrieve request metadata.
-            user_info: The OIDCUserModel object that will be checked
-            async_request: The httpx client.
-        """
+    Uses OAUTH2 settings and request information to authorize actions.
+    """
 
+    async def authorize(self, request: HTTPConnection, user_info: OIDCUserModel) -> Optional[bool]:
         if not (oauth2lib_settings.OAUTH2_ACTIVE and oauth2lib_settings.OAUTH2_AUTHORIZATION_ACTIVE):
             return None
 
         try:
-            json = await request.json()
+            if isinstance(request, WebSocket):
+                json = {}
+            else:
+                request = cast(Request, request)
+                json = await request.json()
         # Silencing the Decode error or Type error when request.json() does not return anything sane.
         # Some requests do not have a json response therefore as this code gets called on every request
         # we need to suppress the `None` case (TypeError) or the `other than json` case (JSONDecodeError)
         # Suppress AttributeError in case of websocket request, it doesn't have .json
         except (JSONDecodeError, TypeError, ClientDisconnect, AttributeError, RuntimeError) as e:
             if isinstance(e, RuntimeError) and "Stream consumed" not in str(e):
                 # RuntimeError is a very broad error class. We only want to catch and ignore a stream
@@ -356,73 +341,110 @@
                 raise e
             json = {}
 
         # defaulting to GET request method for WebSocket request, it doesn't have .method
         request_method = request.method if hasattr(request, "method") else "GET"
         opa_input = {
             "input": {
-                **(opa_kwargs or {}),
+                **(self.opa_kwargs or {}),
                 **user_info,
                 "resource": request.url.path,
                 "method": request_method,
                 "arguments": {"path": request.path_params, "query": {**request.query_params}, "json": json},
             }
         }
 
-        decision = await _get_decision(async_request, opa_url, opa_input)
+        async with AsyncClient(http1=True, verify=HTTPX_SSL_CONTEXT) as async_request:
+            decision = await self.get_decision(async_request, opa_input)
 
         context = {
             "resource": opa_input["input"]["resource"],
             "method": opa_input["input"]["method"],
             "user_info": user_info,
             "input": opa_input,
             "url": request.url,
         }
-        return _evaluate_decision(decision, auto_error, **context)
+        return self.evaluate_decision(decision, **context)
 
-    return _opa_decision
 
+class GraphQLOPAAuthorization(GraphqlAuthorization, OPAMixin):
+    """Specializes OPA authorization for GraphQL operations.
 
-def opa_graphql_decision(
-    opa_url: str,
-    _oidc_security: OIDCUser,
-    auto_error: bool = False,  # By default don't raise HTTP 403 because partial results are preferred
-    opa_kwargs: Union[Mapping[str, str], None] = None,
-    async_request: Union[AsyncClient, None] = None,
-) -> Callable[[str, OIDCUserModel], Awaitable[Union[bool, None]]]:
-    async def _opa_decision(
-        path: str,
-        oidc_user: OIDCUserModel = Depends(_oidc_security),
-        async_request_1: Union[AsyncClient, None] = None,
-    ) -> Union[bool, None]:
-        """Check OIDCUserModel against the OPA policy.
+    Customizable to handle partial results without raising HTTP 403.
+    """
 
-        This is used as a security module in Graphql projects
-        This method will make an async call towards the Policy agent.
+    def __init__(self, opa_url: str, auto_error: bool = False, opa_kwargs: Union[Mapping[str, Any], None] = None):
+        # By default don't raise HTTP 403 because partial results are preferred
+        super().__init__(opa_url, auto_error, opa_kwargs)
 
-        Args:
-            path: the graphql path that will be checked against the permissions of the oidc_user
-            oidc_user: The OIDCUserModel object that will be checked
-            async_request_1: The Async client
-        """
+    async def authorize(self, request: RequestPath, user_info: OIDCUserModel) -> Optional[bool]:
         if not (oauth2lib_settings.OAUTH2_ACTIVE and oauth2lib_settings.OAUTH2_AUTHORIZATION_ACTIVE):
             return None
 
         opa_input = {
             "input": {
-                **(opa_kwargs or {}),
-                **oidc_user,
-                "resource": path,
+                **(self.opa_kwargs or {}),
+                **user_info,
+                "resource": request,
                 "method": "POST",
             }
         }
 
-        client_request = async_request or async_request_1
-        if not client_request:
-            client_request = AsyncClient(http1=True, verify=HTTPX_SSL_CONTEXT)
-
-        decision = await _get_decision(client_request, opa_url, opa_input)
+        async with AsyncClient(http1=True, verify=HTTPX_SSL_CONTEXT) as async_request:
+            decision = await self.get_decision(async_request, opa_input)
 
         context = {"resource": opa_input["input"]["resource"], "input": opa_input}
-        return _evaluate_decision(decision, auto_error, **context)
+        return self.evaluate_decision(decision, **context)
+
+
+class AuthManager:
+    """Manages the authentication and authorization mechanisms for the application.
+
+    This manager class orchestrates authentication and authorization, utilizing OpenID Connect (OIDC) and
+    Open Policy Agent (OPA) respectively. It serves as a central hub for user authentication states and
+    authorization policies. If defaults are insufficient, users can register alternatives or customize existing ones.
+
+    Attributes:
+        _authentication (OIDCAuth): Handles user authentication.
+        _authorization (Authorization): Manages access controls.
+        _graphql_authorization (GraphqlAuthorization): Manages GraphQL-specific authorization.
+
+    Methods:
+        authentication: Gets or sets the OIDCAuth instance, allowing customization of the authentication process.
+        authorization: Gets or sets the Authorization instance, permitting customization of access controls.
+        graphql_authorization: Gets or sets the GraphqlAuthorization instance, enabling specific security policies for GraphQL.
+    """
+
+    def __init__(self) -> None:
+        self._authentication = OIDCAuth(
+            openid_url=oauth2lib_settings.OIDC_BASE_URL,
+            openid_config_url=oauth2lib_settings.OIDC_CONF_URL,  # Corrected parameter name
+            resource_server_id=oauth2lib_settings.OAUTH2_RESOURCE_SERVER_ID,
+            resource_server_secret=oauth2lib_settings.OAUTH2_RESOURCE_SERVER_SECRET,
+            oidc_user_model_cls=OIDCUserModel,
+        )
+        self._authorization: Authorization = OPAAuthorization(opa_url=oauth2lib_settings.OPA_URL)
+        self._graphql_authorization: GraphqlAuthorization = GraphQLOPAAuthorization(opa_url=oauth2lib_settings.OPA_URL)
+
+    @property
+    def authentication(self) -> OIDCAuth:
+        return self._authentication
+
+    @authentication.setter
+    def authentication(self, auth_instance: OIDCAuth) -> None:
+        self._authentication = auth_instance
+
+    @property
+    def authorization(self) -> Authorization:
+        return self._authorization
+
+    @authorization.setter
+    def authorization(self, auth_instance: Authorization) -> None:
+        self._authorization = auth_instance
+
+    @property
+    def graphql_authorization(self) -> GraphqlAuthorization:
+        return self._graphql_authorization
 
-    return _opa_decision
+    @graphql_authorization.setter
+    def graphql_authorization(self, auth_instance: GraphqlAuthorization) -> None:
+        self._graphql_authorization = auth_instance
```

### Comparing `oauth2_lib-1.5.0/oauth2_lib/settings.py` & `oauth2_lib-2.0.0/oauth2_lib/settings.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,10 +27,16 @@
     SERVICE_NAME: str = ""
     MUTATIONS_ENABLED: bool = False
     ENVIRONMENT_IGNORE_MUTATION_DISABLED: list[str] = Field(
         default_factory=list, description="Environments for which to allow unauthenticated mutations"
     )
     OAUTH2_ACTIVE: bool = True
     OAUTH2_AUTHORIZATION_ACTIVE: bool = True
+    OAUTH2_RESOURCE_SERVER_ID: str = ""
+    OAUTH2_RESOURCE_SERVER_SECRET: str = ""
+    OAUTH2_TOKEN_URL: str = ""
+    OIDC_BASE_URL: str = ""
+    OIDC_CONF_URL: str = ""
+    OPA_URL: str = ""
 
 
 oauth2lib_settings = Oauth2LibSettings()
```

### Comparing `oauth2_lib-1.5.0/oauth2_lib/strawberry.py` & `oauth2_lib-2.0.0/oauth2_lib/strawberry.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,66 +6,63 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from collections.abc import Awaitable
-from typing import Any, Callable, Union
+from typing import Any, Callable, Optional, Union
 
 import asyncstdlib
 import strawberry
 import structlog
 from fastapi import HTTPException
 from graphql.pyutils import Path
 from starlette.requests import Request
 from strawberry import BasePermission
 from strawberry.fastapi import BaseContext
 from strawberry.types import Info
 from strawberry.types.fields.resolver import StrawberryResolver
 from strawberry.types.info import RootValueType
 
-from oauth2_lib.fastapi import OIDCUserModel
+from oauth2_lib.fastapi import AuthManager, OIDCUserModel
 from oauth2_lib.settings import oauth2lib_settings
 
 logger = structlog.get_logger(__name__)
 
 
 class OauthContext(BaseContext):
+    def __init__(
+        self,
+        auth_manager: AuthManager,
+    ):
+        self.auth_manager = auth_manager
+        super().__init__()
+
     @asyncstdlib.cached_property
-    async def get_current_user(self) -> Union[OIDCUserModel, None]:
+    async def get_current_user(self) -> Optional[OIDCUserModel]:
         """Retrieve the OIDCUserModel once per graphql request.
 
         Note:
             This function should not raise exceptions, otherwise it will not be cached.
         """
         if not isinstance(self.request, Request):  # it could be None or a WebSocket
             logger.debug("Can't retrieve OIDCUserModel without a starlette Request", request_type=type(self.request))
             return None
 
         if not oauth2lib_settings.OAUTH2_ACTIVE:
             logger.debug("Not retrieving OIDCUserModel because OAUTH2_ACTIVE=False")
             return None
 
         try:
-            return await self._get_current_user(self.request)
+            return await self.auth_manager.authentication.authenticate(self.request)
         except HTTPException as exc:
             logger.debug("User is not authenticated", status_code=exc.status_code, detail=exc.detail)
             return None
 
-    def __init__(
-        self,
-        get_current_user: Callable[[Request], Awaitable[OIDCUserModel]],
-        get_opa_decision: Callable[[str, OIDCUserModel], Awaitable[Union[bool, None]]],
-    ):
-        self._get_current_user = get_current_user
-        self.get_opa_decision = get_opa_decision
-        super().__init__()
-
 
 OauthInfo = Info[OauthContext, RootValueType]
 
 
 def get_path_as_string(path: Path) -> str:
     if path.prev:
         return f"{get_path_as_string(path.prev)}/{path.key}"
@@ -105,17 +102,22 @@
 async def is_authorized(info: OauthInfo, path: str) -> bool:
     """Check that the user is allowed to query/mutate this path."""
     context = info.context
     current_user = await context.get_current_user
     if not current_user:
         return False
 
-    opa_decision = await context.get_opa_decision(path, current_user)
-    authorized = bool(opa_decision)
-    logger.debug("Received opa decision", path=path, opa_decision=opa_decision, is_authorized=authorized)
+    authorization_decision = await context.auth_manager.graphql_authorization.authorize(path, current_user)
+    authorized = bool(authorization_decision)
+    logger.debug(
+        "Received graphql authorization decision",
+        path=path,
+        authorization_decision=authorization_decision,
+        is_authorized=authorized,
+    )
 
     return authorized
 
 
 class IsAuthenticatedForQuery(BasePermission):
     message = "User is not authenticated"
```

### Comparing `oauth2_lib-1.5.0/pyproject.toml` & `oauth2_lib-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 
 [tool.flit.metadata.requires-extra]
 test = [
     "apache-license-check",
     "black",
     "ruff",
     "mypy",
-    "opentelemetry-instrumentation-urllib3",
     "pygments",
     "pytest",
     "pytest-asyncio",
     "pytest-cov",
     "pytest-xdist",
     "requests_mock",
     "urllib3_mock==0.3.3",
```

### Comparing `oauth2_lib-1.5.0/setup.cfg` & `oauth2_lib-2.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.5.0/tests/strawberry/conftest.py` & `oauth2_lib-2.0.0/tests/strawberry/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,49 @@
+from typing import Optional
+
 import pytest
 import strawberry
 from fastapi import Depends, FastAPI
+from starlette.requests import Request
 from starlette.testclient import TestClient
 from strawberry.fastapi import GraphQLRouter
 
-from oauth2_lib.fastapi import opa_graphql_decision
+from oauth2_lib.fastapi import AuthManager, GraphQLOPAAuthorization, OIDCAuth, OIDCUserModel
 from oauth2_lib.strawberry import (
     OauthContext,
     authenticated_federated_field,
     authenticated_field,
     authenticated_mutation_field,
 )
 from tests.test_fastapi import user_info_matching
 
 
-@pytest.fixture
-def mock_graphql_app(make_mock_async_client):  # noqa: C901
-    def _mock_graphql_app(authorized=True):
-        mock_async_client = make_mock_async_client({"result": authorized, "decision_id": "hoi"})
+async def get_oidc_authentication():
+    class OIDCAuthMock(OIDCAuth):
+        async def userinfo(self, request: Request, token: Optional[str] = None) -> Optional[OIDCUserModel]:
+            return user_info_matching
+
+    return OIDCAuthMock("openid_url", "openid_url/.well-known/openid-configuration", "id", "secret", OIDCUserModel)
+
+
+async def get_opa_security_graphql():
+    return GraphQLOPAAuthorization(opa_url="https://opa_url.test")
 
+
+async def get_auth_manger():
+    auth_manager = AuthManager()
+    auth_manager.authentication = await get_oidc_authentication()
+    auth_manager.graphql_authorization = await get_opa_security_graphql()
+
+    return auth_manager
+
+
+@pytest.fixture
+def mock_graphql_app():  # noqa: C901
+    def _mock_graphql_app():
         @strawberry.type
         class BookType:
             title: str
             author: str
 
         @strawberry.type
         class bookNestedAuthType:
@@ -48,28 +69,16 @@
 
         @strawberry.type
         class Mutation:
             @authenticated_mutation_field("mutation test")
             def add_book(self, title: str, author: str) -> BookType:
                 return BookType(title=title, author=author)
 
-        async def get_oidc_user():
-            async def get_current_user(request=None):
-                return user_info_matching
-
-            return get_current_user
-
-        async def get_opa_security_graphql():
-            return opa_graphql_decision("https://opa_url.test", None, async_request=mock_async_client)
-
-        async def get_context(
-            get_current_user=Depends(get_oidc_user),  # noqa: B008
-            get_opa_decision=Depends(get_opa_security_graphql),  # noqa: B008
-        ) -> OauthContext:  # type: ignore # noqa: B008
-            return OauthContext(get_current_user=get_current_user, get_opa_decision=get_opa_decision)
+        async def get_context(auth_manager=Depends(get_auth_manger)) -> OauthContext:  # type: ignore # noqa: B008
+            return OauthContext(auth_manager=auth_manager)
 
         app = FastAPI()
         schema = strawberry.Schema(query=Query, mutation=Mutation)
         graphql_app = GraphQLRouter(schema, context_getter=get_context)
         app.include_router(graphql_app, prefix="/graphql")
 
         return TestClient(app)
```

### Comparing `oauth2_lib-1.5.0/tests/strawberry/test_authenticated_field.py` & `oauth2_lib-2.0.0/tests/strawberry/test_authenticated_federated_field.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,65 @@
 from unittest import mock
 
 from oauth2_lib.settings import oauth2lib_settings
+from tests.conftest import MockResponse
 
 
 @mock.patch.object(oauth2lib_settings, "OAUTH2_ACTIVE", False)
 def test_query_returns_data_when_oauth_is_disabled(mock_graphql_app):
-    test_client = mock_graphql_app(False)
-
-    response = test_client.post("/graphql", json={"query": "{ book { title, author } }"})
-    response_data = response.json()
-
-    assert response.status_code == 200
-    assert response_data["data"] == {"book": {"title": "test title", "author": "test author"}}
-
-
-@mock.patch.object(oauth2lib_settings, "OAUTH2_ACTIVE", True)
-def test_query_raises_error_when_permission_is_denied(mock_graphql_app):
-    test_client = mock_graphql_app(False)
-
-    response = test_client.post("/graphql", json={"query": "{ book { title, author } }"})
-    response_data = response.json()
-
-    assert response.status_code == 200
-    assert response_data["errors"][0]["message"] == "User is not authorized to query `/book/`"
-
-
-@mock.patch.object(oauth2lib_settings, "OAUTH2_ACTIVE", True)
-def test_query_returns_data_when_permission_is_allowed(mock_graphql_app):
     test_client = mock_graphql_app()
 
-    response = test_client.post("/graphql", json={"query": "{ book { title, author } }"})
+    response = test_client.post("/graphql", json={"query": "{ federatedBook { title, author } }"})
     response_data = response.json()
 
     assert response.status_code == 200
-    assert response_data["data"] == {"book": {"title": "test title", "author": "test author"}}
+    assert response_data["data"] == {
+        "federatedBook": {"title": "test title federated field", "author": "test author federated field"}
+    }
 
 
 @mock.patch.object(oauth2lib_settings, "OAUTH2_ACTIVE", True)
-def test_query_with_nested_auth_raises_error_when_permission_is_denied(mock_graphql_app):
-    test_client = mock_graphql_app(False)
+def test_query_raises_error_when_permission_is_denied(mock_graphql_app, make_mock_async_client, discovery):
+    mock_async_client = make_mock_async_client(
+        [
+            MockResponse(json=discovery),
+            MockResponse(json={"result": False, "decision_id": "8ef9daf0-1a23-4a6b-8433-c64ef028bee8"}),
+        ]
+    )
+
+    with mock.patch("oauth2_lib.fastapi.AsyncClient", return_value=mock_async_client):
+        test_client = mock_graphql_app()
+
+        response = test_client.post(
+            "/graphql",
+            json={"query": "{ federatedBook { title, author } }"},
+            headers={"Authorization": "Bearer example_token"},
+        )
+        response_data = response.json()
 
-    response = test_client.post("/graphql", json={"query": "{ bookNestedAuth { title, author } }"})
-    response_data = response.json()
-
-    assert response.status_code == 200
-    assert response_data["errors"][0]["message"] == "User is not authorized to query `/booknestedauth/author/`"
+        assert response.status_code == 200
+        assert response_data["errors"][0]["message"] == "User is not authorized to query `/federatedbook/`"
 
 
 @mock.patch.object(oauth2lib_settings, "OAUTH2_ACTIVE", True)
-def test_query_with_nested_auth_returns_data_when_permission_is_allowed(mock_graphql_app):
-    test_client = mock_graphql_app()
-
-    response = test_client.post("/graphql", json={"query": "{ bookNestedAuth { title, author } }"})
-    response_data = response.json()
-
-    assert response.status_code == 200
-    assert response_data["data"] == {"bookNestedAuth": {"title": "test title", "author": "test title author"}}
+def test_query_returns_data_when_permission_is_allowed(mock_graphql_app, make_mock_async_client, discovery):
+    mock_async_client = make_mock_async_client(
+        [
+            MockResponse(json=discovery),
+            MockResponse(json={"result": True, "decision_id": "8ef9daf0-1a23-4a6b-8433-c64ef028bee8"}),
+        ]
+    )
+
+    with mock.patch("oauth2_lib.fastapi.AsyncClient", return_value=mock_async_client):
+        test_client = mock_graphql_app()
+
+        response = test_client.post(
+            "/graphql",
+            json={"query": "{ federatedBook { title, author } }"},
+            headers={"Authorization": "Bearer example_token"},
+        )
+        response_data = response.json()
+
+        assert response.status_code == 200
+        assert response_data["data"] == {
+            "federatedBook": {"title": "test title federated field", "author": "test author federated field"}
+        }
```

### Comparing `oauth2_lib-1.5.0/tests/test_async_api_client.py` & `oauth2_lib-2.0.0/tests/test_async_api_client.py`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.5.0/tests/test_opa_decision.py` & `oauth2_lib-2.0.0/tests/test_opa_decision.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,33 +2,20 @@
 from unittest import mock
 
 import pytest
 from fastapi import HTTPException
 from starlette.requests import Request
 from starlette.websockets import WebSocket
 
-from oauth2_lib.fastapi import OIDCUser, opa_decision
+from oauth2_lib.fastapi import OIDCUserModel, OPAAuthorization
 from oauth2_lib.settings import oauth2lib_settings
+from tests.conftest import MockResponse
 from tests.test_fastapi import user_info_matching
 
 
-@pytest.mark.asyncio
-async def test_opa_decision_auto_error():
-    def mock_user_info():
-        return {}
-
-    oauth2lib_settings.OAUTH2_ACTIVE = False
-    opa_decision_security = opa_decision("https://opa_url.test", cast(OIDCUser, mock_user_info))
-
-    mock_request = mock.MagicMock(spec=Request)
-
-    assert await opa_decision_security(mock_request, {}, None) is None  # type:ignore
-    oauth2lib_settings.OAUTH2_ACTIVE = True
-
-
 @pytest.fixture
 def mock_request():
     mock_request = mock.MagicMock(spec=Request)
     mock_request.url.path = "/test/path"
     mock_request.method = "GET"
     mock_request.path_params = {}
     mock_request.json.return_value = {}
@@ -40,154 +27,179 @@
     mock_request = mock.MagicMock(spec=WebSocket)
     mock_request.url.path = "/test/path"
     mock_request.path_params = {}
     return mock_request
 
 
 @pytest.mark.asyncio
+async def test_opa_decision_auto_error(mock_request):
+    oauth2lib_settings.OAUTH2_ACTIVE = False
+    authorization = OPAAuthorization("https://opa_url.test")
+    assert await authorization.authorize(mock_request, cast(OIDCUserModel, {})) is None
+    oauth2lib_settings.OAUTH2_ACTIVE = True
+
+
+@pytest.mark.asyncio
 async def test_opa_decision_user_not_allowed(make_mock_async_client, mock_request):
-    mock_async_client = make_mock_async_client({"result": False, "decision_id": "hoi"})
+    mock_async_client = make_mock_async_client(
+        MockResponse(json={"result": False, "decision_id": "8ef9daf0-1a23-4a6b-8433-c64ef028bee8"})
+    )
 
-    opa_decision_security = opa_decision("https://opa_url.test", None)  # type:ignore
+    with mock.patch("oauth2_lib.fastapi.AsyncClient", return_value=mock_async_client):
+        authorization = OPAAuthorization(opa_url="https://opa_url.test")
 
-    with pytest.raises(HTTPException) as exception:
-        await opa_decision_security(mock_request, user_info_matching, mock_async_client)
+        with pytest.raises(HTTPException) as exception:
+            await authorization.authorize(mock_request, user_info_matching)
 
-    assert exception.value.status_code == 403
-    opa_input = {
-        "input": {
-            **user_info_matching,
-            "resource": "/test/path",
-            "method": "GET",
-            "arguments": {"path": {}, "query": {}, "json": {}},
+        assert exception.value.status_code == 403
+        assert (
+            exception.value.detail
+            == f"User is not allowed to access resource: /test/path Decision was taken with id: {'8ef9daf0-1a23-4a6b-8433-c64ef028bee8'}"
+        )
+
+        opa_input = {
+            "input": {
+                **user_info_matching,
+                "resource": "/test/path",
+                "method": "GET",
+                "arguments": {"path": {}, "query": {}, "json": {}},
+            }
         }
-    }
-    mock_async_client.post.assert_called_with("https://opa_url.test", json=opa_input)
+        mock_async_client.client.post.assert_called_with("https://opa_url.test", json=opa_input)
 
 
 @pytest.mark.asyncio
 async def test_opa_decision_network_or_type_error(make_mock_async_client, mock_request):
-    mock_async_client = make_mock_async_client(error=TypeError())
+    mock_async_client = make_mock_async_client(MockResponse(error=TypeError()))
 
-    opa_decision_security = opa_decision("https://opa_url.test", None)  # type:ignore
+    with mock.patch("oauth2_lib.fastapi.AsyncClient", return_value=mock_async_client):
+        authorization = OPAAuthorization(opa_url="https://opa_url.test")
 
-    with pytest.raises(HTTPException) as exception:
-        await opa_decision_security(mock_request, user_info_matching, mock_async_client)
+        with pytest.raises(HTTPException) as exception:
+            await authorization.authorize(mock_request, user_info_matching)
 
-    assert exception.value.status_code == 503
+        assert exception.value.status_code == 503
+        assert exception.value.detail == "Policy agent is unavailable"
 
 
 @pytest.mark.asyncio
 async def test_opa_decision_user_allowed(make_mock_async_client, mock_request):
-    mock_async_client = make_mock_async_client({"result": True, "decision_id": "hoi"})
-
-    opa_decision_security = opa_decision("https://opa_url.test", None)  # type:ignore
-
-    result = await opa_decision_security(mock_request, user_info_matching, mock_async_client)
+    mock_async_client = make_mock_async_client(
+        MockResponse(json={"result": True, "decision_id": "8ef9daf0-1a23-4a6b-8433-c64ef028bee8"})
+    )
 
-    assert result is True
-    opa_input = {
-        "input": {
-            **user_info_matching,
-            "resource": "/test/path",
-            "method": "GET",
-            "arguments": {"path": {}, "query": {}, "json": {}},
+    with mock.patch("oauth2_lib.fastapi.AsyncClient", return_value=mock_async_client):
+        authorization = OPAAuthorization(opa_url="https://opa_url.test")
+        result = await authorization.authorize(mock_request, user_info_matching)
+
+        assert result is True
+        opa_input = {
+            "input": {
+                **user_info_matching,
+                "resource": "/test/path",
+                "method": "GET",
+                "arguments": {"path": {}, "query": {}, "json": {}},
+            }
         }
-    }
-    mock_async_client.post.assert_called_with("https://opa_url.test", json=opa_input)
+        mock_async_client.client.post.assert_called_with("https://opa_url.test", json=opa_input)
 
 
 @pytest.mark.asyncio
 async def test_opa_decision_user_allowed_websocket_request(make_mock_async_client, mock_websocket_request):
-    mock_async_client = make_mock_async_client({"result": True, "decision_id": "hoi"})
-
-    opa_decision_security = opa_decision("https://opa_url.test", None)  # type:ignore
-
-    result = await opa_decision_security(mock_websocket_request, user_info_matching, mock_async_client)
+    mock_async_client = make_mock_async_client(
+        MockResponse(json={"result": True, "decision_id": "8ef9daf0-1a23-4a6b-8433-c64ef028bee8"})
+    )
 
-    assert result is True
-    opa_input = {
-        "input": {
-            **user_info_matching,
-            "resource": "/test/path",
-            "method": "GET",
-            "arguments": {"path": {}, "query": {}, "json": {}},
+    with mock.patch("oauth2_lib.fastapi.AsyncClient", return_value=mock_async_client):
+        authorization = OPAAuthorization(opa_url="https://opa_url.test")
+        result = await authorization.authorize(mock_websocket_request, user_info_matching)
+
+        assert result is True
+        opa_input = {
+            "input": {
+                **user_info_matching,
+                "resource": "/test/path",
+                "method": "GET",
+                "arguments": {"path": {}, "query": {}, "json": {}},
+            }
         }
-    }
-    mock_async_client.post.assert_called_with("https://opa_url.test", json=opa_input)
+        mock_async_client.client.post.assert_called_with("https://opa_url.test", json=opa_input)
 
 
 @pytest.mark.asyncio
 async def test_opa_decision_kwargs(make_mock_async_client, mock_request):
-    mock_async_client = make_mock_async_client({"result": True, "decision_id": "hoi"})
-
-    opa_decision_security = opa_decision("https://opa_url.test", None, opa_kwargs={"extra": 3})  # type:ignore
-
-    result = await opa_decision_security(mock_request, user_info_matching, mock_async_client)
+    mock_async_client = make_mock_async_client(
+        MockResponse(json={"result": True, "decision_id": "8ef9daf0-1a23-4a6b-8433-c64ef028bee8"})
+    )
 
-    assert result is True
-    opa_input = {
-        "input": {
-            "extra": 3,
-            **user_info_matching,
-            "resource": "/test/path",
-            "method": "GET",
-            "arguments": {"path": {}, "query": {}, "json": {}},
+    with mock.patch("oauth2_lib.fastapi.AsyncClient", return_value=mock_async_client):
+        authorization = OPAAuthorization(opa_url="https://opa_url.test", opa_kwargs={"extra": 3})
+        result = await authorization.authorize(mock_request, user_info_matching)
+
+        assert result is True
+        opa_input = {
+            "input": {
+                "extra": 3,
+                **user_info_matching,
+                "resource": "/test/path",
+                "method": "GET",
+                "arguments": {"path": {}, "query": {}, "json": {}},
+            }
         }
-    }
-    mock_async_client.post.assert_called_with("https://opa_url.test", json=opa_input)
+        mock_async_client.client.post.assert_called_with("https://opa_url.test", json=opa_input)
 
 
 @pytest.mark.asyncio
 async def test_opa_decision_auto_error_not_allowed(make_mock_async_client, mock_request):
-    mock_async_client = make_mock_async_client({"result": False, "decision_id": "hoi"})
-
-    opa_decision_security = opa_decision(
-        "https://opa_url.test", None, opa_kwargs={"extra": 3}, auto_error=False  # type:ignore
+    mock_async_client = make_mock_async_client(
+        MockResponse(json={"result": False, "decision_id": "8ef9daf0-1a23-4a6b-8433-c64ef028bee8"})
     )
 
-    result = await opa_decision_security(mock_request, user_info_matching, mock_async_client)
-
-    assert result is False
-    opa_input = {
-        "input": {
-            "extra": 3,
-            **user_info_matching,
-            "resource": "/test/path",
-            "method": "GET",
-            "arguments": {"path": {}, "query": {}, "json": {}},
+    with mock.patch("oauth2_lib.fastapi.AsyncClient", return_value=mock_async_client):
+        authorization = OPAAuthorization(opa_url="https://opa_url.test", opa_kwargs={"extra": 3}, auto_error=False)
+        result = await authorization.authorize(mock_request, user_info_matching)
+
+        assert result is False
+        opa_input = {
+            "input": {
+                "extra": 3,
+                **user_info_matching,
+                "resource": "/test/path",
+                "method": "GET",
+                "arguments": {"path": {}, "query": {}, "json": {}},
+            }
         }
-    }
-    mock_async_client.post.assert_called_with("https://opa_url.test", json=opa_input)
+        mock_async_client.client.post.assert_called_with("https://opa_url.test", json=opa_input)
 
 
 @pytest.mark.asyncio
 async def test_opa_decision_auto_error_allowed(make_mock_async_client, mock_request):
-    mock_async_client = make_mock_async_client({"result": True, "decision_id": "hoi"})
-
-    opa_decision_security = opa_decision(
-        "https://opa_url.test", None, opa_kwargs={"extra": 3}, auto_error=False  # type:ignore
+    mock_async_client = make_mock_async_client(
+        MockResponse(json={"result": True, "decision_id": "8ef9daf0-1a23-4a6b-8433-c64ef028bee8"})
     )
-    result = await opa_decision_security(mock_request, user_info_matching, mock_async_client)
 
-    assert result is True
-    opa_input = {
-        "input": {
-            "extra": 3,
-            **user_info_matching,
-            "resource": "/test/path",
-            "method": "GET",
-            "arguments": {"path": {}, "query": {}, "json": {}},
+    with mock.patch("oauth2_lib.fastapi.AsyncClient", return_value=mock_async_client):
+        authorization = OPAAuthorization(opa_url="https://opa_url.test", opa_kwargs={"extra": 3}, auto_error=False)
+        result = await authorization.authorize(mock_request, user_info_matching)
+
+        assert result is True
+        opa_input = {
+            "input": {
+                "extra": 3,
+                **user_info_matching,
+                "resource": "/test/path",
+                "method": "GET",
+                "arguments": {"path": {}, "query": {}, "json": {}},
+            }
         }
-    }
-    mock_async_client.post.assert_called_with("https://opa_url.test", json=opa_input)
+        mock_async_client.client.post.assert_called_with("https://opa_url.test", json=opa_input)
 
 
 # @pytest.mark.asyncio
 # async def test_opa_decision_opa_unavailable(make_mock_async_client, mock_request):
-#     mock_async_client = make_mock_async_client({"result": False, "decision_id": "hoi"})
+#     mock_async_client = make_mock_async_client({"result": False, "decision_id": "8ef9daf0-1a23-4a6b-8433-c64ef028bee8"})
 
 #     opa_decision_security = opa_decision("https://opa_url.test", None)
 
 #     with pytest.raises(HTTPException) as exception:
 #         await opa_decision_security(mock_request, user_info_matching, mock_async_client)
 #     assert exception.value.status_code == 503
```

### Comparing `oauth2_lib-1.5.0/PKG-INFO` & `oauth2_lib-2.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oauth2-lib
-Version: 1.5.0
+Version: 2.0.0
 Summary: This is the SURF Oauth2 module that interfaces with the oauth2 setup.
 Home-page: https://github.com/workfloworchestrator/oauth2-lib
 Author: SURF
 Author-email: automation-beheer@surf.nl
 Requires-Python: >=3.9,<3.13
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
@@ -37,15 +37,14 @@
 Requires-Dist: asyncstdlib
 Requires-Dist: bumpversion ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: apache-license-check ; extra == "test"
 Requires-Dist: black ; extra == "test"
 Requires-Dist: ruff ; extra == "test"
 Requires-Dist: mypy ; extra == "test"
-Requires-Dist: opentelemetry-instrumentation-urllib3 ; extra == "test"
 Requires-Dist: pygments ; extra == "test"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-asyncio ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: pytest-xdist ; extra == "test"
 Requires-Dist: requests_mock ; extra == "test"
 Requires-Dist: urllib3_mock==0.3.3 ; extra == "test"
@@ -53,14 +52,15 @@
 Provides-Extra: dev
 Provides-Extra: test
 
 # OAuth2-lib
 
 [![pypi_version](https://img.shields.io/pypi/v/oauth2-lib?color=%2334D058&label=pypi%20package)](https://pypi.org/project/oauth2-lib)
 [![Supported python versions](https://img.shields.io/pypi/pyversions/oauth2-lib.svg?color=%2334D058)](https://pypi.org/project/oauth2-lib)
+[![codecov](https://codecov.io/gh/workfloworchestrator/oauth2-lib/graph/badge.svg?token=JDMMBBOVM4)](https://codecov.io/gh/workfloworchestrator/oauth2-lib)
 
 This Project contains a Mixin class that wraps an openapi-codegen python client, to inject Opentelemetry spans
 and api call retries. It also contains a number of FastAPI dependencies which enables Policy enforcement offloading
 to Open Policy Agent.
 
 The project contains a number of OIDC classes that are tailored to the SURF environment.
```

