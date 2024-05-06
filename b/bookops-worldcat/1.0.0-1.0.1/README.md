# Comparing `tmp/bookops_worldcat-1.0.0.tar.gz` & `tmp/bookops_worldcat-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bookops_worldcat-1.0.0.tar", max compression
+gzip compressed data, was "bookops_worldcat-1.0.1.tar", max compression
```

## Comparing `bookops_worldcat-1.0.0.tar` & `bookops_worldcat-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      180 2024-03-26 19:30:49.633751 bookops_worldcat-1.0.0/bookops_worldcat/__init__.py
--rw-r--r--   0        0        0      127 2024-03-26 19:30:49.633751 bookops_worldcat-1.0.0/bookops_worldcat/__version__.py
--rw-r--r--   0        0        0     4893 2024-03-26 19:30:49.633751 bookops_worldcat-1.0.0/bookops_worldcat/_session.py
--rw-r--r--   0        0        0     8771 2024-03-26 19:30:49.640084 bookops_worldcat-1.0.0/bookops_worldcat/authorize.py
--rw-r--r--   0        0        0      665 2024-03-26 19:30:49.642078 bookops_worldcat-1.0.0/bookops_worldcat/errors.py
--rw-r--r--   0        0        0    86952 2024-03-26 19:30:49.645461 bookops_worldcat-1.0.0/bookops_worldcat/metadata_api.py
--rw-r--r--   0        0        0        0 2024-03-26 19:30:49.649633 bookops_worldcat-1.0.0/bookops_worldcat/py.typed
--rw-r--r--   0        0        0     2437 2024-03-26 19:30:49.650135 bookops_worldcat-1.0.0/bookops_worldcat/query.py
--rw-r--r--   0        0        0     2778 2024-03-26 19:30:49.650135 bookops_worldcat-1.0.0/bookops_worldcat/utils.py
--rw-r--r--   0        0        0     1084 2024-03-26 18:59:46.634197 bookops_worldcat-1.0.0/LICENSE
--rw-r--r--   0        0        0     2634 2024-03-26 19:30:49.684659 bookops_worldcat-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     7999 2024-03-26 19:30:49.633751 bookops_worldcat-1.0.0/README.md
--rw-r--r--   0        0        0     9215 1970-01-01 00:00:00.000000 bookops_worldcat-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      180 2024-05-06 14:38:37.158240 bookops_worldcat-1.0.1/bookops_worldcat/__init__.py
+-rw-r--r--   0        0        0      127 2024-05-06 15:06:41.450927 bookops_worldcat-1.0.1/bookops_worldcat/__version__.py
+-rw-r--r--   0        0        0     4632 2024-05-06 14:38:37.167311 bookops_worldcat-1.0.1/bookops_worldcat/_session.py
+-rw-r--r--   0        0        0     9932 2024-05-06 14:38:37.169307 bookops_worldcat-1.0.1/bookops_worldcat/authorize.py
+-rw-r--r--   0        0        0      665 2024-05-06 14:38:37.171299 bookops_worldcat-1.0.1/bookops_worldcat/errors.py
+-rw-r--r--   0        0        0    80648 2024-05-06 14:38:37.173503 bookops_worldcat-1.0.1/bookops_worldcat/metadata_api.py
+-rw-r--r--   0        0        0        0 2024-05-06 14:38:37.173503 bookops_worldcat-1.0.1/bookops_worldcat/py.typed
+-rw-r--r--   0        0        0     2722 2024-05-06 14:38:37.173503 bookops_worldcat-1.0.1/bookops_worldcat/query.py
+-rw-r--r--   0        0        0     3448 2024-05-06 14:38:37.173503 bookops_worldcat-1.0.1/bookops_worldcat/utils.py
+-rw-r--r--   0        0        0     1084 2024-05-06 14:38:37.158240 bookops_worldcat-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2634 2024-05-06 15:08:12.860083 bookops_worldcat-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     7999 2024-05-06 14:38:37.158240 bookops_worldcat-1.0.1/README.md
+-rw-r--r--   0        0        0     9215 1970-01-01 00:00:00.000000 bookops_worldcat-1.0.1/PKG-INFO
```

### Comparing `bookops_worldcat-1.0.0/bookops_worldcat/_session.py` & `bookops_worldcat-1.0.1/bookops_worldcat/_session.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # -*- coding: utf-8 -*-
 
 """
-Base session class to allow extention of functionality to Worldcat Search API
-and others.
+Base session class to be subclassed for use with individual OCLC APIs.
 """
 
 from typing import Optional, Tuple, Union, List
 
 import requests
 from urllib3.util import Retry
 
 from . import __title__, __version__
 from .authorize import WorldcatAccessToken
 
 
 class WorldcatSession(requests.Session):
-    """Base class, inherits all requests.Session methods"""
+    """Base class for WorldCat API sessions. Inherits all `requests.Session` methods."""
 
     def __init__(
         self,
         authorization: WorldcatAccessToken,
         agent: Optional[str] = None,
         timeout: Union[int, float, Tuple[int, int], Tuple[float, float], None] = (
             5,
@@ -28,38 +27,43 @@
         totalRetries: int = 0,
         backoffFactor: float = 0,
         statusForcelist: Optional[List[int]] = None,
         allowedMethods: Optional[List[str]] = None,
     ) -> None:
         """
         Args:
-            authorization:          WorldcatAccessToken instance
-            agent:                  "User-agent" parameter to attached to each
-                                    request in the session
-            timeout:                how long to wait for server to send data
-                                    before giving up
-            totalRetries:           optional number of times to retry a request that
-                                    failed or timed out. if totalRetries argument is
-                                    not passed, any arguments passed to
-                                    backoffFactor, statusForcelist, and
-                                    allowedMethods will be ignored. default is 0
-            backoffFactor:          if totalRetries is not 0, the backoff
-                                    factor as a float to use to calculate amount of
-                                    time session will sleep before attempting request
-                                    again. default is 0
-            statusForcelist:        if totalRetries is not 0, a list of HTTP
-                                    status codes to automatically retry requests on.
-                                    if not specified, failed requests with status codes
-                                    413, 429, and 503 will be retried up to number of
-                                    totalRetries.
-                                    example: [500, 502, 503, 504]
-            allowedMethods:         if totalRetries is not 0, set of HTTP methods that
-                                    requests should be retried on. if not specified,
-                                    requests using any HTTP method verbs will be
-                                    retried. example: ["GET", "POST"]
+            authorization:
+                `WorldcatAccessToken` instance.
+            agent:
+                `User-agent` parameter to attached to each request in the session.
+            timeout:
+                How long to wait for server to send data before giving up. Accepts
+                separate values for connect and read timeouts or a single value.
+            totalRetries:
+                Optional number of times to retry a request that has failed or timed
+                out. If `totalRetries` argument is not passed, all arguments passed
+                to `backoffFactor`, `statusForcelist`, and `allowedMethods`
+                will be ignored.
+            backoffFactor:
+                If `totalRetries` is not `0`, the backoff factor as a float to use to
+                calculate amount of time session will sleep before attempting request
+                again.
+            statusForcelist:
+                If `totalRetries` is not `0`, a list of HTTP status codes to
+                automatically retry requests on. If not specified, failed requests with
+                status codes 413, 429, and 503 will be retried up to number of
+                `totalRetries`.
+
+                **EXAMPLE:** `[500, 502, 503, 504]`
+            allowedMethods:
+                If `totalRetries` is not `0`, set of HTTP methods that requests should
+                be retried on. If not specified, requests using any HTTP method verbs
+                will be retried.
+
+                **EXAMPLE:** `["GET", "POST"]`
         """
         super().__init__()
         self.authorization = authorization
 
         if not isinstance(self.authorization, WorldcatAccessToken):
             raise TypeError(
                 "Argument 'authorization' must be 'WorldcatAccessToken' object."
```

### Comparing `bookops_worldcat-1.0.0/bookops_worldcat/authorize.py` & `bookops_worldcat-1.0.1/bookops_worldcat/authorize.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,94 +1,120 @@
 # -*- coding: utf-8 -*-
 
 """
-This module provides means to authenticate and obtain a WorldCat access token.
+Provides means to authenticate and authorize interactions with OCLC web services.
 """
 
 import datetime
 import sys
 from typing import Dict, Optional, Tuple, Union
 
 import requests
 
 from . import __title__, __version__
 from .errors import WorldcatAuthorizationError
 
 
 class WorldcatAccessToken:
     """
-    Requests Worldcat access token.
-    Authenticates and authorizes using Client Credentials Grant. Does not support
-    Explicit Authorization Code and Refresh Token flows. Token with correctly
-    bonded scopes can then be passed into a session of particular web service
-    to authorize requests for resources.
-    More on OCLC's client credentials grant:
-    https://www.oclc.org/developer/api/keys/oauth/client-credentials-grant.en.html
-
-    Args:
-        key:                    your WSKey public client_id
-        secret:                 your WSKey secret
-        scopes:                 request scopes for the access token as a string,
-                                separate different scopes with space
-                                users with WSKeys set up to act as multiple institutions
-                                should provide scope and registryID in the format
-                                "{scope} context:{registryID}"
-                                examples:
-                                    single institution WSKey:
-                                        "WorldCatMetadataAPI"
-                                    multi-institution WSKey:
-                                        "WorldCatMetadataAPI context:00001"
-        agent:                  "User-agent" parameter to be passed in the request
-                                header; usage strongly encouraged
-        timeout:                how long to wait for server to send data before
-                                giving up; default value is 3 seconds
-
-
-    Examples:
-        >>> from bookops_worldcat import WorldcatAccessToken
-        >>> token = WorldcatAccessToken(
-                key="my_WSKey_client_id",
-                secret="my_WSKey_secret",
-                scopes="WorldCatMetadataAPI",
-                agent="my_app/1.0.0")
-        >>> token.token_str
-        "tk_Yebz4BpEp9dAsghA7KpWx6dYD1OZKWBlHjqW"
-        >>> token.is_expired()
-        False
-        >>> token.server_response.json()
-        {"token_token": "tk_Yebz4BpEp9dAsghA7KpWx6dYD1OZKWBlHjqW",
-         "token_type": "bearer",
-         "expires_in": "1199",
-         "principalID": "",
-         "principalIDNS": "",
-         "scopes": "WorldCatMetadataAPI",
-         "contextInstitutionId": "00001",
-         "expires_at": "2020-08-23 18:45:29Z"}
-        >>> token.server_response.request.headers
-        {"User-Agent": "my_app/1.0.0",
-         "Accept-Encoding": "gzip, deflate",
-         "Accept": "application/json",
-         "Connection": "keep-alive",
-         "Content-Length": "67",
-         "Content-Type": "application/x-www-form-urlencoded",
-         "Authorization": "Basic encoded_authorization_here="}
+    Requests a WorldCat access token.
 
-    """
+    Authenticates and authorizes using
+    [Client Credentials Grant](https://www.oclc.org/developer/api/keys/oauth/client-credentials-grant.en.html)
+    flow. A token with correctly bonded scopes can be passed into a session of an
+    OCLC web service to authorize requests for resources.
+
+    Example:
+        ```py
+        from bookops_worldcat import WorldcatAccessToken
+
+        token = WorldcatAccessToken(
+            key="my_WSKey_client_id",
+            secret="my_WSKey_secret",
+            scopes="WorldCatMetadataAPI",
+            agent="my_app/1.0.0")
+        print(token.token_str)
+        #>"tk_Yebz4BpEp9dAsghA7KpWx6dYD1OZKWBlHjqW"
+        print(token.is_expired())
+        #>False
+        print(token.server_response.json())
+        {
+            "token_token": "tk_Yebz4BpEp9dAsghA7KpWx6dYD1OZKWBlHjqW",
+            "token_type": "bearer",
+            "expires_in": "1199",
+            "principalID": "",
+            "principalIDNS": "",
+            "scopes": "WorldCatMetadataAPI",
+            "contextInstitutionId": "00001",
+            "expires_at": "2020-08-23 18:45:29Z"
+        }
+        print(token.server_response.request.headers)
+        {
+            "User-Agent": "my_app/1.0.0",
+            "Accept-Encoding": "gzip, deflate",
+            "Accept": "application/json",
+            "Connection": "keep-alive",
+            "Content-Length": "67",
+            "Content-Type": "application/x-www-form-urlencoded",
+            "Authorization": "Basic encoded_authorization_here="
+        }
+        ```
+    """  # noqa: E501
 
     def __init__(
         self,
         key: str,
         secret: str,
         scopes: str,
         agent: str = "",
-        timeout: Optional[
-            Union[int, float, Tuple[int, int], Tuple[float, float]]
-        ] = None,
+        timeout: Union[int, float, Tuple[int, int], Tuple[float, float], None] = (
+            5,
+            5,
+        ),
     ) -> None:
-        """Constructor"""
+        """Initializes WorldcatAccessToken object.
+
+
+        info: Usage Documentation:
+            - [Basic Usage](../start.md#authentication-and-authorization)
+            - [Advanced Usage](../advanced.md#WorldcatAccessToken)
+
+        Args:
+            key:
+                Your WSKey public client_id
+            secret:
+                Your WSKey secret
+            scopes:
+                Request scopes for the access token as a string. Multiple scopes
+                should be separated with a space. Users with WSKeys set up to act on
+                behalf of multiple institutions should provide scope and registryID
+                in the format:
+                `{scope} context:{registryID}`
+
+                **EXAMPLES:**
+
+                - Single institution WSKey: `"WorldCatMetadataAPI"`
+                - Multi-institution WSKey: `"WorldCatMetadataAPI context:00001"`
+
+            agent:
+                `User-agent` parameter to be passed in the request header. Usage is
+                strongly encouraged.
+            timeout:
+                How long to wait for server to send data before giving up. Accepts
+                separate values for connect and read timeouts or a single value.
+
+        Raises:
+            TypeError:
+                If `agent`, `key`, `secret`, or `scopes` args are passed
+                anything other than a str.
+            ValueError:
+                If an empty str is passed to `key`, `secret` or `scopes` arg.
+            WorldcatAuthorizationError:
+                If request for token encounters any errors.
+        """
 
         self.agent = agent
         self.grant_type = "client_credentials"
         self.key = key
         self.oauth_server = "https://oauth.oclc.org"
         self.scopes = scopes
         self.secret = secret
@@ -122,44 +148,44 @@
         if isinstance(self.scopes, str):
             if not self.scopes.strip():
                 raise ValueError("Argument 'scopes' cannot be an empty string.")
         else:
             raise TypeError("Argument 'scopes' must a string.")
         self.scopes = self.scopes.strip()
 
-        # assign default value for timout
-        if not self.timeout:
-            self.timeout = (3, 3)
-
         # initiate request
         self._request_token()
 
     def _auth(self) -> Tuple[str, str]:
         return (self.key, self.secret)
 
     def _hasten_expiration_time(self, utc_stamp_str: str) -> datetime.datetime:
         """
         Resets expiration time one second earlier to account
         for any delays between expiration check and request for
         new token in session setting.
 
         Args:
-            utcstamp:               utc timestamp string
+            utcstamp: utc timestamp string
 
         Returns:
-            utcstamp
+            UTC timestamp as `datetime.datetime` object
         """
         utcstamp = datetime.datetime.strptime(
             utc_stamp_str, "%Y-%m-%d %H:%M:%SZ"
         ) - datetime.timedelta(seconds=1)
         utcstamp = utcstamp.replace(tzinfo=datetime.timezone.utc)
         return utcstamp
 
     def _parse_server_response(self, response: requests.Response) -> None:
-        """Parses authorization server response"""
+        """Parses authorization server response
+
+        Raises:
+            WorldcatAuthorizationError: If server returns an error code.
+        """
         self.server_response = response
         if response.status_code == requests.codes.ok:
             self.token_str = response.json()["access_token"]
             self.token_expires_at = self._hasten_expiration_time(
                 response.json()["expires_at"]
             )
             self.token_type = response.json()["token_type"]
@@ -174,16 +200,20 @@
         }
 
     def _post_token_request(self) -> requests.Response:
         """
         Fetches Worldcat access token for specified scope (web service)
 
         Returns:
-            requests.models.Response
-        """
+            [`requests.Response`](https://requests.readthedocs.io/en/latest/api/#requests.Response)
+            instance
+
+        Raises:
+            WorldcatAuthorizationError: If access token POST request encounters any errors.
+        """  # noqa: E501
 
         token_url = self._token_url()
         headers = self._token_headers()
         auth = self._auth()
         payload = self._payload()
         try:
             response = requests.post(
@@ -214,20 +244,31 @@
         return f"{self.oauth_server}/token"
 
     def is_expired(self) -> bool:
         """
         Checks if the access token is expired.
 
         Returns:
-            bool
-
-        Examples:
-            >>> token.is_expired()
-            False
+            bool: Whether or not the token is expired.
 
+        Raises:
+            TypeError:
+                If `WorldcatAccessToken.token_expires_at` is not a
+                `datetime.datetime` object.
+
+        Example:
+            ```py
+            token = WorldcatAccessToken(
+                key="my_WSKey_client_id",
+                secret="my_WSKey_secret",
+                scopes="WorldCatMetadataAPI",
+                agent="my_app/1.0.0")
+            print(token.is_expired())
+            #>False
+            ```
         """
         if isinstance(self.token_expires_at, datetime.datetime):
             if self.token_expires_at < datetime.datetime.now(datetime.timezone.utc):
                 return True
             else:
                 return False
         else:
```

### Comparing `bookops_worldcat-1.0.0/bookops_worldcat/errors.py` & `bookops_worldcat-1.0.1/bookops_worldcat/errors.py`

 * *Files identical despite different names*

### Comparing `bookops_worldcat-1.0.0/bookops_worldcat/metadata_api.py` & `bookops_worldcat-1.0.1/bookops_worldcat/metadata_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,65 +1,80 @@
 # -*- coding: utf-8 -*-
 
-"""
-This module provides MetadataSession class for requests to WorldCat Metadata API.
-"""
+"""WorldCat Metadata API wrapper session."""
 
 from typing import Callable, Dict, List, Optional, Tuple, Union, BinaryIO
 
 from requests import Request, Response
 
 from ._session import WorldcatSession
 from .authorize import WorldcatAccessToken
 from .query import Query
 from .utils import verify_oclc_number, verify_oclc_numbers
 
 
 class MetadataSession(WorldcatSession):
-    """OCLC Metadata API wrapper session. Inherits `requests.Session` methods"""
+    """
+    The `MetadataSession` class supports interactions with the WorldCat Metadata API
+    and the child methods of this class allow users to interact with each endpoint
+    of the API.
+
+    `MetadataSession` inherits attributes and methods from `requests.Session`
+    and `WorldcatSession` and contains specific functionality for interacting
+    with the WorldCat Metadata API.
+    """
 
     BASE_URL = "https://metadata.api.oclc.org/worldcat"
 
     def __init__(
         self,
         authorization: WorldcatAccessToken,
         agent: Optional[str] = None,
-        timeout: Union[int, float, Tuple[int, int], Tuple[float, float], None] = None,
+        timeout: Union[int, float, Tuple[int, int], Tuple[float, float], None] = (
+            5,
+            5,
+        ),
         totalRetries: int = 0,
         backoffFactor: float = 0,
         statusForcelist: Optional[List[int]] = None,
         allowedMethods: Optional[List[str]] = None,
     ) -> None:
-        """Initializes MetadataSession
+        """Initializes MetadataSession.
 
         Args:
-            authorization:          WorldcatAccessToken object
-            agent:                  "User-agent" parameter to be passed in the request
-                                    header; usage strongly encouraged
-            timeout:                how long to wait for server to send data before
-                                    giving up; default value is 5 seconds
-            totalRetries:           optional number of times to retry a request that
-                                    failed or timed out. if totalRetries argument is
-                                    not passed, any arguments passed to
-                                    backoffFactor, statusForcelist, and
-                                    allowedMethods will be ignored. default is 0
-            backoffFactor:          if totalRetries is not 0, the backoff
-                                    factor as a float to use to calculate amount of
-                                    time session will sleep before attempting request
-                                    again. default is 0
-            statusForcelist:        if totalRetries is not 0, a list of HTTP
-                                    status codes to automatically retry requests on.
-                                    if not specified, failed requests with status codes
-                                    413, 429, and 503 will be retried up to number of
-                                    totalRetries.
-                                    example: [500, 502, 503, 504]
-            allowedMethods:         if totalRetries is not 0, set of HTTP methods that
-                                    requests should be retried on. if not specified,
-                                    requests using any HTTP method verbs will be
-                                    retried. example: ["GET", "POST"]
+            authorization:
+                `WorldcatAccessToken` object for session.
+            agent:
+                `User-agent` for session to be passed in the request header. Usage is
+                strongly encouraged.
+            timeout:
+                How long to wait for server to send data before giving up. Accepts
+                separate values for connect and read timeouts or a single value.
+            totalRetries:
+                Optional number of times to retry a request that failed or timed out.
+                If `totalRetries` argument is not passed, any arguments passed to
+                `backoffFactor`, `statusForcelist`, and `allowedMethods` will be
+                ignored.
+            backoffFactor:
+                If `totalRetries` is not `0`, the backoff factor as a float to use to
+                calculate amount of time session will sleep before attempting request
+                again.
+            statusForcelist:
+                If `totalRetries` is not `0`, a list of HTTP status codes to
+                automatically retry requests on. If not specified, failed requests
+                with status codes 413, 429, and 503 will be retried up to number of
+                `totalRetries`.
+
+                **EXAMPLE:** `[500, 502, 503, 504]`
+            allowedMethods:
+                If `totalRetries` is not `0`, set of HTTP methods that requests should
+                be retried on. If not specified, requests using any HTTP method verbs
+                will be retried.
+
+                **EXAMPLE:** `["GET", "POST"]`
         """
         super().__init__(
             authorization,
             agent=agent,
             timeout=timeout,
             totalRetries=totalRetries,
             backoffFactor=backoffFactor,
@@ -156,27 +171,32 @@
         record: Union[str, bytes, BinaryIO],
         recordFormat: str,
         responseFormat: str = "application/marcxml+xml",
         hooks: Optional[Dict[str, Callable]] = None,
     ) -> Optional[Response]:
         """
         Create a bib record in OCLC if it does not already exist.
+
         Uses /manage/bibs endpoint.
 
         Args:
-            record:                 MARC record to be created
-            recordFormat:           format of MARC record; options:
-                                    'application/marcxml+xml'; 'application/marc'
-            responseFormat:         format of returned record; options:
-                                    'application/marcxml+xml', 'application/marc'
-                                    default is 'application/marcxml+xml'
-            hooks:                  Requests library hook system that can be used for
-                                    signal event handling. For more information see the
-                                    [Requests docs](https://requests.readthedocs.io/en/
-                                    master/user/advanced/#event-hooks)
+            record:
+                MARC record to be created
+            recordFormat:
+                Format of MARC record.
+
+                **OPTIONS:** `'application/marcxml+xml'` or `'application/marc'`
+            responseFormat:
+                Format of returned record.
+
+                **OPTIONS:** `'application/marcxml+xml'` or `'application/marc'`
+            hooks:
+                Requests library hook system that can be used for signal event
+                handling. For more information see the [Requests docs](https://requests.
+                readthedocs.io/en/master/user/advanced/#event-hooks)
 
         Returns:
             `requests.Response` instance
         """
         url = self._url_manage_bibs_create()
         header = {
             "Accept": responseFormat,
@@ -195,28 +215,30 @@
     def bib_get(
         self,
         oclcNumber: Union[int, str],
         responseFormat: str = "application/marcxml+xml",
         hooks: Optional[Dict[str, Callable]] = None,
     ) -> Optional[Response]:
         """
-        Send a GET request for a full bibliographic resource.
+        Send a GET request for a full bib record.
+
         Uses /manage/bibs/{oclcNumber} endpoint.
 
         Args:
-            oclcNumber:             OCLC bibliographic record number; can be an
-                                    integer or string with or without OCLC Number
-                                    prefix
-            responseFormat:         format of returned record, options:
-                                    'application/marcxml+xml', 'application/marc',
-                                    default is 'application/marcxml+xml'
-            hooks:                  Requests library hook system that can be used for
-                                    signal event handling. For more information see the
-                                    [Requests docs](https://requests.readthedocs.io/en/
-                                    master/user/advanced/#event-hooks)
+            oclcNumber:
+                OCLC bibliographic record number. Can be an integer or string
+                with or without OCLC Number prefix.
+            responseFormat:
+                Format of returned record.
+
+                **OPTIONS:** `'application/marcxml+xml'` or `'application/marc'`
+            hooks:
+                Requests library hook system that can be used for signal event
+                handling. For more information see the [Requests docs](https://requests.
+                readthedocs.io/en/master/user/advanced/#event-hooks)
 
         Returns:
             `requests.Response` instance
         """
         oclcNumber = verify_oclc_number(oclcNumber)
 
         url = self._url_manage_bibs(oclcNumber)
@@ -235,24 +257,25 @@
         self,
         oclcNumber: Union[int, str],
         hooks: Optional[Dict[str, Callable]] = None,
     ) -> Optional[Response]:
         """
         Given an OCLC number, retrieve classification recommendations for the bib
         record.
+
         Uses /search/classification-bibs/{oclcNumber} endpoint.
 
         Args:
-            oclcNumber:             OCLC bibliographic record number; can be an
-                                    integer or string with or without OCLC Number
-                                    prefix
-            hooks:                  Requests library hook system that can be used for
-                                    signal event handling. For more information see the
-                                    [Requests docs](https://requests.readthedocs.io/en/
-                                    master/user/advanced/#event-hooks)
+            oclcNumber:
+                OCLC bibliographic record number. Can be an integer or string
+                with or without OCLC Number prefix.
+            hooks:
+                Requests library hook system that can be used for signal event
+                handling. For more information see the [Requests docs](https://requests.
+                readthedocs.io/en/master/user/advanced/#event-hooks)
 
         Returns:
             `requests.Response` instance
         """
         oclcNumber = verify_oclc_number(oclcNumber)
 
         url = self._url_search_classification_bibs(oclcNumber)
@@ -265,38 +288,42 @@
         # send request
         query = Query(self, prepared_request, timeout=self.timeout)
 
         return query.response
 
     def bib_get_current_oclc_number(
         self,
-        oclcNumbers: Union[str, List[Union[str, int]]],
+        oclcNumbers: Union[int, str, List[Union[str, int]]],
         hooks: Optional[Dict[str, Callable]] = None,
     ) -> Optional[Response]:
         """
         Given one or more OCLC Numbers, retrieve current OCLC numbers.
+
         Uses /manage/bibs/current endpoint.
 
         Args:
-            oclcNumbers:            string or list containing one or more OCLC numbers
-                                    to be checked; numbers can be integers or strings
-                                    with or without OCLC Number prefix;
-                                    if str, the numbers must be separated by a comma
-            hooks:                  Requests library hook system that can be used for
-                                    signal event handling. For more information see the
-                                    [Requests docs](https://requests.readthedocs.io/en/
-                                    master/user/advanced/#event-hooks)
-
+            oclcNumbers:
+                Integer, string or list containing one or more OCLC numbers to be
+                checked. Numbers can be integers or strings with or without OCLC
+                Number prefix. If str, the numbers must be separated by a comma.
+                If int, only one number may be passed as an arg.
+            hooks:
+                Requests library hook system that can be used for signal event
+                handling. For more information see the [Requests docs](https://requests.
+                readthedocs.io/en/master/user/advanced/#event-hooks)
 
-        Returns:
-            `requests.Response` instance
+        Raises:
+            ValueError: If more than 10 items passed to `oclcNumbers` arg.
         """
-
         vetted_numbers = verify_oclc_numbers(oclcNumbers)
 
+        # check that no more than 10 oclc numbers were passed
+        if len(vetted_numbers) > 10:
+            raise ValueError("Too many OCLC Numbers passed to 'oclcNumbers' argument.")
+
         header = {"Accept": "application/json"}
         url = self._url_manage_bibs_current_oclc_number()
         payload = {"oclcNumbers": ",".join(vetted_numbers)}
 
         # prep request
         req = Request("GET", url, params=payload, headers=header, hooks=hooks)
         prepared_request = self.prepare_request(req)
@@ -311,25 +338,29 @@
         record: Union[str, bytes, BinaryIO],
         recordFormat: str,
         hooks: Optional[Dict[str, Callable]] = None,
     ) -> Optional[Response]:
         """
         Given a bib record in MARC21 or MARCXML identify the best match in WorldCat.
         Record must contain at minimum an 008 and 245. Response contains number of
-        potential matches in numberOfRecords and best match in briefRecords.
+        potential matches in `numberOfRecords` and best match in `briefRecords`.
+
         Uses /manage/bibs/match endpoint.
 
         Args:
-            record:                 MARC record to be matched
-            recordFormat:           format of MARC record, options:
-                                    'application/marcxml+xml', 'application/marc'
-            hooks:                  Requests library hook system that can be used for
-                                    signal event handling. For more information see the
-                                    [Requests docs](https://requests.readthedocs.io/en/
-                                    master/user/advanced/#event-hooks)
+            record:
+                MARC record to be matched.
+            recordFormat:
+                Format of MARC record.
+
+                **OPTIONS:** `'application/marcxml+xml'` or `'application/marc'`
+            hooks:
+                Requests library hook system that can be used for signal event
+                handling. For more information see the [Requests docs](https://requests.
+                readthedocs.io/en/master/user/advanced/#event-hooks)
 
         Returns:
             `requests.Response` instance
         """
         url = self._url_manage_bibs_match()
         header = {
             "Accept": "application/json",
@@ -352,30 +383,32 @@
         recordFormat: str,
         responseFormat: str = "application/marcxml+xml",
         hooks: Optional[Dict[str, Callable]] = None,
     ) -> Optional[Response]:
         """
         Given an OCLC number and MARC record, find record in WorldCat and replace it.
         If the record does not exist in WorldCat, a new bib record will be created.
+
         Uses /manage/bibs/{oclcNumber} endpoint.
 
         Args:
-            oclcNumber:             OCLC bibliographic record number; can be an
-                                    integer or string with or without OCLC Number
-                                    prefix
-            record:                 MARC record to replace existing WorldCat record
-            recordFormat:           format of MARC record, options:
-                                    'application/marcxml+xml', 'application/marc'
-            responseFormat:         format of returned record; options:
-                                    'application/marcxml+xml', 'application/marc'
-                                    default is 'application/marcxml+xml'
-            hooks:                  Requests library hook system that can be used for
-                                    signal event handling. For more information see the
-                                    [Requests docs](https://requests.readthedocs.io/en/
-                                    master/user/advanced/#event-hooks)
+            record:
+                MARC record to replace existing WorldCat record
+            recordFormat:
+                Format of MARC record.
+
+                **OPTIONS:** `'application/marcxml+xml'` or `'application/marc'`
+            responseFormat:
+                Format of returned record.
+
+                **OPTIONS:** `'application/marcxml+xml'` or `'application/marc'`
+            hooks:
+                Requests library hook system that can be used for signal event
+                handling. For more information see the [Requests docs](https://requests.
+                readthedocs.io/en/master/user/advanced/#event-hooks)
 
         Returns:
             `requests.Response` instance
         """
         oclcNumber = verify_oclc_number(oclcNumber)
 
         url = self._url_manage_bibs(oclcNumber)
@@ -398,31 +431,40 @@
         record: Union[str, bytes, BinaryIO],
         recordFormat: str,
         validationLevel: str = "validateFull",
         hooks: Optional[Dict[str, Callable]] = None,
     ) -> Optional[Response]:
         """
         Given a bib record, validate that record conforms to MARC standards.
+
         Uses /manage/bibs/validate/{validationLevel} endpoint.
 
         Args:
-            record:                 MARC record to be validated
-            recordFormat:           format of MARC record, options:
-                                    'application/marcxml+xml', 'application/marc'
-            validationLevel:        Level at which to validate records
-                                    available values: 'validateFull', 'validateAdd',
-                                    'validateReplace'
-                                    default is 'validateFull'
-            hooks:                  Requests library hook system that can be used for
-                                    signal event handling. For more information see the
-                                    [Requests docs](https://requests.readthedocs.io/en/
-                                    master/user/advanced/#event-hooks)
+            record:
+                MARC record to validate
+            recordFormat:
+                Format of MARC record.
+
+                **OPTIONS:** `'application/marcxml+xml'` or `'application/marc'`
+            validationLevel:
+                Level at which to validate records.
+
+                **OPTIONS:** `'validateFull'`, `'validateAdd'`, `'validateReplace'`
+            hooks:
+                Requests library hook system that can be used for signal event
+                handling. For more information see the [Requests docs](https://requests.
+                readthedocs.io/en/master/user/advanced/#event-hooks)
 
         Returns:
             `requests.Response` instance
+
+        Raises:
+            ValueError:
+                If value of arg passed to `validationLevel` is not
+                `'validateFull'`, `'validateAdd'`, or `'validateReplace'`.
         """
         if validationLevel not in ["validateFull", "validateAdd", "validateReplace"]:
             raise ValueError(
                 "Invalid argument 'validationLevel'."
                 "Must be either 'validateFull', 'validateAdd', or 'validateReplace'"
             )
 
@@ -448,24 +490,25 @@
         return query.response
 
     def brief_bibs_get(
         self, oclcNumber: Union[int, str], hooks: Optional[Dict[str, Callable]] = None
     ) -> Optional[Response]:
         """
         Retrieve specific brief bibliographic resource.
+
         Uses /search/brief-bibs/{oclcNumber} endpoint.
 
         Args:
-            oclcNumber:             OCLC bibliographic record number; can be an
-                                    integer or string with or without OCLC Number
-                                    prefix
-            hooks:                  Requests library hook system that can be used for
-                                    signal event handling. For more information see the
-                                    [Requests docs](https://requests.readthedocs.io/en/
-                                    master/user/advanced/#event-hooks)
+            oclcNumber:
+                OCLC bibliographic record number. Can be an integer or string
+                with or without OCLC Number prefix.
+            hooks:
+                Requests library hook system that can be used for signal event
+                handling. For more information see the [Requests docs](https://requests.
+                readthedocs.io/en/master/user/advanced/#event-hooks)
 
         Returns:
             `requests.Response` instance
         """
         oclcNumber = verify_oclc_number(oclcNumber)
 
         url = self._url_search_brief_bibs_oclc_number(oclcNumber)
@@ -515,111 +558,157 @@
         orderBy: str = "bestMatch",
         offset: int = 1,
         limit: int = 10,
         hooks: Optional[Dict[str, Callable]] = None,
     ) -> Optional[Response]:
         """
         Search for brief bibliographic resources using WorldCat query syntax.
-        See https://help.oclc.org/Librarian_Toolbox/Searching_WorldCat_Indexes/
-        Bibliographic_records/Bibliographic_record_indexes for more information on
-        available indexes. Request may contain only one of: heldByInstitutionID,
-        heldByGroup, heldBySymbol, or combination of lat and lon.
+        See OCLC
+        [Bibliographic Records Index Documentation](https://help.oclc.org/Librarian_Toolbox/Searching_WorldCat_Indexes/Bibliographic_records/Bibliographic_record_indexes)
+        for more information on available indexes. Request may contain
+        only one of: `heldByInstitutionID`, `heldByGroup`, `heldBySymbol`, or
+        combination of `lat` and `lon`.
+
         Uses /search/brief-bibs endpoint.
 
         Args:
-            q:                      query in the form of a keyword search or
-                                    fielded search;
-                                    examples:
-                                        ti:Zendegi
-                                        ti:"Czarne oceany"
-                                        bn:9781680502404
-                                        kw:python databases
-                                        ti:Zendegi AND au:greg egan
-                                        (au:Okken OR au:Myers) AND su:python
-            deweyNumber:            limits the response to the
-                                    specified dewey classification number(s);
-                                    for multiple values repeat the parameter,
-                                    example:
-                                        '794,180'
-            datePublished:          restricts the response to one or
-                                    more dates, or to a range,
-                                    examples:
-                                        '2000'
-                                        '2000-2005'
-                                        '2000,2005'
-            heldByGroup:            restricts to holdings held by group symbol
-            heldBySymbol:           restricts response to holdings held by specified
-                                    institution symbol
-            heldByInstitutionID:    restricts response to holdings held by specified
-                                    institution registryId
-            inLanguage:             restricts the response to the single
-                                    specified language, example: 'fre'
-            inCatalogLanguage:      restricts the response to specified
-                                    cataloging language, example: 'eng';
-                                    default 'eng'
-            materialType:           restricts responses to specified material type,
-                                    example: 'bks', 'vis'
-            catalogSource:          restrict to responses to single OCLC symbol as
-                                    the cataloging source, example: 'DLC'
-            itemType:               restricts responses to single specified OCLC
-                                    top-level facet type, example: 'book'
-            itemSubType:            restricts responses to single specified OCLC
-                                    sub facet type, example: 'digital'
-            retentionCommitments:   restricts responses to bibliographic records
-                                    with retention commitment; options: True, False,
-                                    (default is False)
-            spProgram:              restricts responses to bibliographic records
-                                    associated with particular shared print
-                                    program
-            genre:                  genre to limit results to (ge index)
-            topic:                  topic to limit results to (s0 index)
-            subtopic:               subtopic to limit results to (s1 index)
-            audience:               audience to limit results to,
-                                    available values: 'juv', 'nonJuv'
-            content:                content to limit results to
-                                    available values: 'fic', 'nonFic', 'bio'
-            openAccess:             restricts response to just open access content
-            peerReviewed:           restricts response to just peer reviewed content
-            facets:                 list of facets to restrict responses
-            groupRelatedEditions:   whether or not use FRBR grouping,
-                                    options: False, True (default is False)
-            groupVariantRecords:    whether or not to group variant records.
-                                    options: False, True (default is False)
-            preferredLanguage:      language of metadata description,
-                                    default value "eng" (English)
-            showHoldingsIndicators: whether or not to show holdings indicators in
-                                    response. options: True, False, (default is False)
-            lat:                    limit to latitude, example: 37.502508
-            lon:                    limit to longitute, example: -122.22702
-            distance:               distance from latitude and longitude
-            unit:                   unit of distance param; options:
-                                    'M' (miles) or 'K' (kilometers), default is 'M'
-            orderBy:                results sort key;
-                                    options:
-                                        'recency'
-                                        'bestMatch'
-                                        'creator'
-                                        'library'
-                                        'publicationDateAsc'
-                                        'publicationDateDesc'
-                                        'mostWidelyHeld'
-                                        'title'
-                                    default is 'bestMatch'
-            offset:                 start position of bibliographic records to
-                                    return; default is 1
-            limit:                  maximum number of records to return;
-                                    maximum is 50, default is 10
-            hooks:                  Requests library hook system that can be used for
-                                    signal event handling. For more information see the
-                                    [Requests docs](https://requests.readthedocs.io/en/
-                                    master/user/advanced/#event-hooks)
+            q:
+                Query in the form of a keyword search or fielded search.
+
+                **EXAMPLES:**
+
+                - `ti:Zendegi`
+                - `ti:"Czarne oceany"`
+                - `bn:9781680502404`
+                - `kw:python databases`
+                - `ti:Zendegi AND au:greg egan`
+                - `(au:Okken OR au:Myers) AND su:python`
+
+            deweyNumber:
+                Limits the response to the specified dewey classification number(s).
+                For multiple values repeat the parameter.
+
+                **EXAMPLE:** `'794'`
+            datePublished:
+                Restricts the response to one or more dates, or to a range.
+
+                **EXAMPLES:** `'2000'`, `'2000-2005'`, `'2000,2005'`
+            heldByGroup:
+                Limits response to holdings held by group symbol.
+            heldBySymbol:
+                Limits response to holdings held by specified institution symbol.
+            heldByInstitutionID:
+                Limits response to holdings held by specified institution registryId.
+            inLanguage:
+                Limits response to the single specified language
+
+                **EXAMPLE:** `'fre'`
+            inCatalogLanguage:
+                Limits response to specified cataloging language.
+
+                **EXAMPLE:** `'eng'`
+            materialType:
+                Limits response to specified material type.
+
+                **EXAMPLES:** `'bks'`, `'vis'`
+            catalogSource:
+                Limits response to single OCLC symbol as the cataloging source.
+
+                **EXAMPLE:** `'DLC'`
+            itemType:
+                Limits response to specified item type.
+
+                **EXAMPLE:** `'book'`, `'vis'`
+            itemSubType:
+                Limits response to specified item subtype.
+
+                **EXAMPLES:** `'book-digital'`, `'audiobook-cd'`
+            retentionCommitments:
+                Limits response to bibliographic records with retention commitment.
+
+                **OPTIONS:** `True` or `False`
+            spProgram:
+                Limits response to bibliographic records associated with particular
+                shared print program.
+            genre:
+                Genre to limit response to (ge index).
+            topic:
+                Topic to limit response to (s0 index).
+            subtopic:
+                Subtopic to limit response to (s1 index).
+            audience:
+                Audience to limit response to.
+
+                **OPTIONS:** `'juv'` or `'nonJuv'`
+            content:
+                Content to limit response to.
+
+                **OPTIONS:** `'fic'`, `'nonFic'`, `'bio'`
+            openAccess:
+                Limits response to just open access content.
+            peerReviewed:
+                Limits response to just peer reviewed content.
+            facets:
+                List of facets to limit responses.
+            groupRelatedEditions:
+                Whether or not use FRBR grouping.
+
+                **OPTIONS:** `True` or `False`
+            groupVariantRecords:
+                Whether or not to group variant records.
+
+                **OPTIONS:** `True` or `False`
+            preferredLanguage:
+                Language user would prefer metadata description in. Does not limit
+                responses. To limit responses use `inCataloglanguage` facet.
+            showHoldingsIndicators:
+                Whether or not to show holdings indicators in response.
+                **OPTIONS:** `True` or `False`
+            lat:
+                Latitude
+
+                **EXAMPLE:** `37.502508`
+            lon:
+                Longitude
+
+                **EXAMPLE:** `-122.22702`
+            distance:
+                Limits response to holdings held by institutions within specified
+                distance from latitude and longitude.
+            unit:
+                Unit of distance from latitude and longitude.
+
+                **OPTIONS:** `'M'` (miles) or `'K'` (kilometers)
+            orderBy:
+                Results sort key.
+
+                **OPTIONS:**
+
+                - `'recency'`
+                - `'bestMatch'`
+                - `'creator'`
+                - `'library'`
+                - `'publicationDateAsc'`
+                - `'publicationDateDesc'`
+                - `'mostWidelyHeld'`
+                - `'title'`
+            offset:
+                Start position of bibliographic records to return.
+            limit:
+                Maximum number of records to return.
+
+                **MAXIMUM:** `50`
+            hooks:
+                Requests library hook system that can be used for signal event
+                handling. For more information see the [Requests docs](https://requests.
+                readthedocs.io/en/master/user/advanced/#event-hooks)
 
         Returns:
             `requests.Response` instance
-        """
+        """  # noqa: E501
         url = self._url_search_brief_bibs()
         header = {"Accept": "application/json"}
         payload = {
             "q": q,
             "deweyNumber": deweyNumber,
             "datePublished": datePublished,
             "heldByGroup": heldByGroup,
@@ -693,94 +782,123 @@
         offset: int = 1,
         limit: int = 10,
         orderBy: str = "publicationDateDesc",
         hooks: Optional[Dict[str, Callable]] = None,
     ) -> Optional[Response]:
         """
         Retrieve other editions related to bibliographic resource with provided
-        OCLC Number. Query may contain only one of: heldByInstitutionID,
-        heldByGroup, heldBySymbol, or spProgram.
+        OCLC Number. Query may contain only one of: `heldByInstitutionID`,
+        `heldByGroup`, `heldBySymbol`, or `spProgram`.
+
         Uses /brief-bibs/{oclcNumber}/other-editions endpoint.
 
         Args:
-            oclcNumber:             OCLC bibliographic record number; can be an
-                                    integer or string with or without OCLC Number
-                                    prefix
-            deweyNumber:            limits the response to the
-                                    specified dewey classification number(s)
-                                    example:
-                                        '794,180'
-            datePublished:          restricts the response to one or
-                                    more dates, or to a range,
-                                    examples:
-                                        '2000'
-                                        '2000-2005'
-                                        '2000,2005'
-            heldByGroup:            restricts to holdings held by group symbol
-            heldBySymbol:           restricts to holdings with specified intitution
-                                    symbol
-            heldByInstitutionID:    restrict to specified institution registryId
-            inLanguage:             restricts the response to the single
-                                    specified language, example: 'fre'
-            inCatalogLanguage:      restricts the response to specified
-                                    cataloging language, example: 'eng';
-                                    default 'eng'
-            materialType:           restricts responses to specified material type,
-                                    example: 'bks', 'vis'
-            catalogSource:          restrict to responses to single OCLC symbol as
-                                    the cataloging source, example: 'DLC'
-            itemType:               restricts responses to single specified OCLC
-                                    top-level facet type, example: 'book'
-            itemSubType:            restricts responses to single specified OCLC
-                                    sub facet type, example: 'digital'
-            retentionCommitments:   restricts responses to bibliographic records
-                                    with retention commitment; options: False, True
-                                    (default is False)
-            spProgram:              restricts responses to bibliographic records
-                                    associated with particular shared print
-                                    program
-            genre:                  genre to limit results to
-            topic:                  topic to limit results to
-            subtopic:               subtopic to limit results to
-            audience:               audience to limit results to,
-                                    example:
-                                        juv,
-                                        nonJuv
-            content:                content to limit results to,
-                                    example:
-                                        fic,
-                                        nonFic,
-                                        fic,bio
-            openAccess:             filter to only open access content, False or True
-            peerReviewed:           filter to only peer reviewed content, False or True
-            facets:                 list of facets to restrict responses
-            groupVariantRecords:    whether or not to group variant records.
-                                    options: False, True (default is False)
-            preferredLanguage:      language of metadata description, default is 'eng'
-            showHoldingsIndicators: whether or not to show holdings indicators in
-                                    response. options: True, False (default is False)
-            offset:                 start position of bibliographic records to
-                                    return; default is 1
-            limit:                  maximum number of records to return;
-                                    maximum is 50, default is 10
-            orderBy:                results sort key;
-                                    options:
-                                        'recency'
-                                        'bestMatch'
-                                        'creator'
-                                        'library'
-                                        'publicationDateAsc'
-                                        'publicationDateDesc'
-                                        'mostWidelyHeld'
-                                        'title'
-                                    default is 'publicationDateDesc'
-            hooks:                  Requests library hook system that can be used for
-                                    signal event handling. For more information see the
-                                    [Requests docs](https://requests.readthedocs.io/en/
-                                    master/user/advanced/#event-hooks)
+            oclcNumber:
+                OCLC bibliographic record number. Can be an integer or string
+                with or without OCLC Number prefix.
+            deweyNumber:
+                Limits response to the specified dewey classification number(s).
+                For multiple values repeat the parameter.
+
+                **EXAMPLE:** `'794'`
+            datePublished:
+                Limits response to one or more dates, or to a range.
+
+                **EXAMPLES:** `'2000'`, `'2000-2005'`, `'2000,2005'`
+            heldByGroup:
+                Limits response to holdings held by group symbol.
+            heldBySymbol:
+                Limits response to holdings held by specified institution symbol.
+            heldByInstitutionID:
+                Limits response to holdings held by specified institution registryId.
+            inLanguage:
+                Limits response to the single specified language
+
+                **EXAMPLE:** `'fre'`
+            inCatalogLanguage:
+                Limits response to specified cataloging language.
+
+                **EXAMPLE:** `'eng'`
+            materialType:
+                Limits response to specified material type.
+
+                **EXAMPLES:** `'bks'`, `'vis'`
+            catalogSource:
+                Limits response to single OCLC symbol as the cataloging source.
+
+                **EXAMPLE:** `'DLC'`
+            itemType:
+                Limits response to specified item type.
+
+                **EXAMPLES:** `'book'`, `'vis'`
+            itemSubType:
+                Limits response to specified item sub type
+
+                **EXAMPLES:** `'book-digital'`, `'audiobook-cd'`
+            retentionCommitments:
+                Limits response to bibliographic records with retention commitment.
+
+                **OPTIONS:** `True` or `False`
+            spProgram:
+                Limits response to bibliographic records associated with particular
+                shared print program.
+            genre:
+                Genre to limit response to (ge index).
+            topic:
+                Topic to limit response to (s0 index).
+            subtopic:
+                Subtopic to limit response to (s1 index).
+            audience:
+                Audience to limit response to.
+
+                **OPTIONS:** `'juv'` or `'nonJuv'`
+            content:
+                Content to limit response to.
+
+                **OPTIONS:** `'fic'`, `'nonFic'`, `'bio'`
+            openAccess:
+                Limits response to just open access content.
+            peerReviewed:
+                Limits response to just peer reviewed content.
+            facets:
+                List of facets to limit responses.
+            groupVariantRecords:
+                Whether or not to group variant records.
+
+                **OPTIONS:** `True` or `False`
+            preferredLanguage:
+                Language user would prefer metadata description in. Does not limit
+                responses. To limit responses use `inCataloglanguage` facet.
+            showHoldingsIndicators:
+                Whether or not to show holdings indicators in response.
+
+                **OPTIONS:** `True` or `False`
+            offset:
+                Start position of bibliographic records to return.
+            limit:
+                Maximum number of records to return.
+
+                **MAXIMUM:** `50`
+            orderBy:
+                Results sort key.
+
+                **OPTIONS:**
+
+                - `'recency'`
+                - `'bestMatch'`
+                - `'creator'`
+                - `'library'`
+                - `'publicationDateAsc'`
+                - `'publicationDateDesc'`
+                - `'mostWidelyHeld'`
+                - `'title'`
+            hooks:
+                Requests library hook system that can be used for signal event
+                handling. For more information see the [Requests docs](https://requests.
+                readthedocs.io/en/master/user/advanced/#event-hooks)
 
         Returns:
             `requests.Response` instance
         """
         oclcNumber = verify_oclc_number(oclcNumber)
 
         url = self._url_search_brief_bibs_other_editions(oclcNumber)
@@ -826,21 +944,23 @@
 
     def holdings_get_codes(
         self,
         hooks: Optional[Dict[str, Callable]] = None,
     ) -> Optional[Response]:
         """
         Retrieve the all holding codes for the authenticated institution.
+
         Uses /manage/institution/holding-codes endpoint.
 
         Args:
-            hooks:                  Requests library hook system that can be used for
-                                    signal event handling. For more information see the
-                                    [Requests docs](https://requests.readthedocs.io/en/
-                                    master/user/advanced/#event-hooks)
+            hooks:
+                Requests library hook system that can be used for signal event
+                handling. For more information see the [Requests docs](https://requests.
+                readthedocs.io/en/master/user/advanced/#event-hooks)
+
         Returns:
             `requests.Response` instance
         """
         url = self._url_manage_ih_codes()
         header = {"Accept": "application/json"}
 
         # prep request
@@ -850,35 +970,40 @@
         # send request
         query = Query(self, prepared_request, timeout=self.timeout)
 
         return query.response
 
     def holdings_get_current(
         self,
-        oclcNumbers: Union[str, List[Union[str, int]]],
+        oclcNumbers: Union[int, str, List[Union[str, int]]],
         hooks: Optional[Dict[str, Callable]] = None,
     ) -> Optional[Response]:
         """
         Retrieves WorldCat holdings status of a record with provided OCLC number.
         The service automatically recognizes the user's institution based on the
         issued access token.
+
         Uses /manage/institution/holdings/current endpoint.
 
         Args:
-            oclcNumbers:            string or list containing one or more OCLC numbers
-                                    to be checked; numbers can be integers or strings
-                                    with or without OCLC Number prefix;
-                                    if str, the numbers must be separated by a comma
-            hooks:                  Requests library hook system that can be used for
-                                    signal event handling. For more information see the
-                                    [Requests docs](https://requests.readthedocs.io/en/
-                                    master/user/advanced/#event-hooks)
+            oclcNumbers:
+                Integer, string or list containing one or more OCLC numbers to be
+                checked. Numbers can be integers or strings with or without OCLC
+                Number prefix. If str, the numbers must be separated by a comma.
+                If int, only one number may be passed as an arg.
+            hooks:
+                Requests library hook system that can be used for signal event
+                handling. For more information see the [Requests docs](https://requests.
+                readthedocs.io/en/master/user/advanced/#event-hooks)
 
         Returns:
             `requests.Response` instance
+
+        Raises:
+            ValueError: If more than 10 items passed to `oclcNumbers` arg.
         """
         vetted_numbers = verify_oclc_numbers(oclcNumbers)
 
         # check that no more than 10 oclc numbers were passed
         if len(vetted_numbers) > 10:
             raise ValueError("Too many OCLC Numbers passed to 'oclcNumbers' argument.")
 
@@ -899,24 +1024,25 @@
     def holdings_set(
         self,
         oclcNumber: Union[int, str],
         hooks: Optional[Dict[str, Callable]] = None,
     ) -> Optional[Response]:
         """
         Sets institution's WorldCat holdings on an individual record.
+
         Uses /manage/institions/holdings/{oclcNumber}/set endpoint.
 
         Args:
-            oclcNumber:             OCLC bibliographic record number; can be an
-                                    integer or string with or without OCLC Number
-                                    prefix
-            hooks:                  Requests library hook system that can be used for
-                                    signal event handling. For more information see the
-                                    [Requests docs](https://requests.readthedocs.io/en/
-                                    master/user/advanced/#event-hooks)
+            oclcNumber:
+                OCLC bibliographic record number. Can be an integer or string
+                with or without OCLC Number prefix.
+            hooks:
+                Requests library hook system that can be used for signal event
+                handling. For more information see the [Requests docs](https://requests.
+                readthedocs.io/en/master/user/advanced/#event-hooks)
 
         Returns:
             `requests.Response` instance
         """
         oclcNumber = verify_oclc_number(oclcNumber)
 
         url = self._url_manage_ih_set(oclcNumber)
@@ -934,24 +1060,25 @@
     def holdings_unset(
         self,
         oclcNumber: Union[int, str],
         hooks: Optional[Dict[str, Callable]] = None,
     ) -> Optional[Response]:
         """
         Unsets institution's WorldCat holdings on an individual record.
+
         Uses /manage/institions/holdings/{oclcNumber}/unset endpoint.
 
         Args:
-            oclcNumber:             OCLC bibliographic record number; can be an
-                                    integer or string with or without OCLC Number
-                                    prefix
-            hooks:                  Requests library hook system that can be used for
-                                    signal event handling. For more information see the
-                                    [Requests docs](https://requests.readthedocs.io/en/
-                                    master/user/advanced/#event-hooks)
+            oclcNumber:
+                OCLC bibliographic record number. Can be an integer or string
+                with or without OCLC Number prefix.
+            hooks:
+                Requests library hook system that can be used for signal event
+                handling. For more information see the [Requests docs](https://requests.
+                readthedocs.io/en/master/user/advanced/#event-hooks)
 
         Returns:
             `requests.Response` instance
         """
         oclcNumber = verify_oclc_number(oclcNumber)
 
         url = self._url_manage_ih_unset(oclcNumber)
@@ -969,27 +1096,31 @@
     def holdings_set_with_bib(
         self,
         record: str,
         recordFormat: str,
         hooks: Optional[Dict[str, Callable]] = None,
     ) -> Optional[Response]:
         """
-        Given a MARC record in MARC XML or MARC21, set institution holdings on the
+        Given a MARC record in MARCXML or MARC21, set institution holdings on the
         record. MARC record must contain OCLC number in 001 or 035 subfield a.
         Only one MARC record is allowed in the request body.
+
         Uses /manage/institution/holdings/set endpoint.
 
         Args:
-            record:                 MARC record on which to set holdings
-            recordFormat:           format of MARC record, options:
-                                    'application/marcxml+xml', 'application/marc'
-            hooks:                  Requests library hook system that can be used for
-                                    signal event handling. For more information see the
-                                    [Requests docs](https://requests.readthedocs.io/en/
-                                    master/user/advanced/#event-hooks)
+            record:
+                MARC record on which to set holdings.
+            recordFormat:
+                Format of MARC record.
+
+                **OPTIONS:** `'application/marcxml+xml'` or `'application/marc'`
+            hooks:
+                Requests library hook system that can be used for signal event
+                handling. For more information see the [Requests docs](https://requests.
+                readthedocs.io/en/master/user/advanced/#event-hooks)
 
         Returns:
             `requests.Response` instance
         """
         url = self._url_manage_ih_set_with_bib()
         header = {
             "Accept": "application/json",
@@ -1008,27 +1139,31 @@
     def holdings_unset_with_bib(
         self,
         record: str,
         recordFormat: str,
         hooks: Optional[Dict[str, Callable]] = None,
     ) -> Optional[Response]:
         """
-        Given a MARC record in MARC XML or MARC21, unset institution holdings on the
+        Given a MARC record in MARCXML or MARC21, unset institution holdings on the
         record. MARC record must contain OCLC number in 001 or 035 subfield a.
         Only one MARC record is allowed in the request body.
+
         Uses /manage/institution/holdings/unset endpoint.
 
         Args:
-            record:                 MARC record on which to unset holdings
-            recordFormat:           format of MARC record, options:
-                                    'application/marcxml+xml', 'application/marc'
-            hooks:                  Requests library hook system that can be used for
-                                    signal event handling. For more information see the
-                                    [Requests docs](https://requests.readthedocs.io/en/
-                                    master/user/advanced/#event-hooks)
+            record:
+                MARC record on which to unset holdings.
+            recordFormat:
+                Format of MARC record.
+
+                **OPTIONS:** `'application/marcxml+xml'` or `'application/marc'`
+            hooks:
+                Requests library hook system that can be used for signal event
+                handling. For more information see the [Requests docs](https://requests.
+                readthedocs.io/en/master/user/advanced/#event-hooks)
 
         Returns:
             `requests.Response` instance
         """
         url = self._url_manage_ih_unset_with_bib()
         header = {
             "Accept": "application/json",
@@ -1048,27 +1183,32 @@
         record: str,
         recordFormat: str,
         responseFormat: str = "application/marcxml+xml",
         hooks: Optional[Dict[str, Callable]] = None,
     ) -> Optional[Response]:
         """
         Given a local bibliographic data record, create it in WorldCat.
+
         Uses /manage/lbds endpoint.
 
         Args:
-            record:                 MARC record to be created
-            recordFormat:           format of MARC record, options:
-                                    'application/marcxml+xml', 'application/marc'
-            responseFormat:         format of returned record; options:
-                                    'application/marcxml+xml', 'application/marc'
-                                    default is 'application/marcxml+xml'
-            hooks:                  Requests library hook system that can be used for
-                                    signal event handling. For more information see the
-                                    [Requests docs](https://requests.readthedocs.io/en/
-                                    master/user/advanced/#event-hooks)
+            record:
+                MARC record to be created.
+            recordFormat:
+                Format of MARC record.
+
+                **OPTIONS:** `'application/marcxml+xml'` or `'application/marc'`
+            responseFormat:
+                Format of returned record.
+
+                **OPTIONS:** `'application/marcxml+xml'` or `'application/marc'`
+            hooks:
+                Requests library hook system that can be used for signal event
+                handling. For more information see the [Requests docs](https://requests.
+                readthedocs.io/en/master/user/advanced/#event-hooks)
 
         Returns:
             `requests.Response` instance
         """
         url = self._url_manage_lbd_create()
         header = {
             "Accept": responseFormat,
@@ -1088,26 +1228,29 @@
         self,
         controlNumber: Union[int, str],
         responseFormat: str = "application/marcxml+xml",
         hooks: Optional[Dict[str, Callable]] = None,
     ) -> Optional[Response]:
         """
         Given a control number, delete the associated Local Bibliographic Data record.
+
         Uses /manage/lbds/{controlNumber} endpoint.
 
         Args:
-            controlNumber:          control number associated with Local Bibliographic
-                                    Data record; can be an integer or string
-            responseFormat:         format of returned record, options:
-                                    'application/marcxml+xml', 'application/marc',
-                                    default is 'application/marcxml+xml'
-            hooks:                  Requests library hook system that can be used for
-                                    signal event handling. For more information see the
-                                    [Requests docs](https://requests.readthedocs.io/en/
-                                    master/user/advanced/#event-hooks)
+            controlNumber:
+                Control number associated with Local Bibliographic Data record.
+                Can be an integer or string.
+            responseFormat:
+                Format of returned record.
+
+                **OPTIONS:** `'application/marcxml+xml'` or `'application/marc'`
+            hooks:
+                Requests library hook system that can be used for signal event
+                handling. For more information see the [Requests docs](https://requests.
+                readthedocs.io/en/master/user/advanced/#event-hooks)
 
         Returns:
             `requests.Response` instance
         """
         url = self._url_manage_lbd(controlNumber)
         header = {"Accept": responseFormat}
 
@@ -1124,26 +1267,29 @@
         self,
         controlNumber: Union[int, str],
         responseFormat: str = "application/marcxml+xml",
         hooks: Optional[Dict[str, Callable]] = None,
     ) -> Optional[Response]:
         """
         Given a Control Number, retrieve a Local Bibliographic Data record.
+
         Uses /manage/lbds/{controlNumber} endpoint.
 
         Args:
-            controlNumber:          control number associated with Local Bibliographic
-                                    Data record; can be an integer or string
-            responseFormat:         format of returned record, options:
-                                    'application/marcxml+xml', 'application/marc',
-                                    default is 'application/marcxml+xml'
-            hooks:                  Requests library hook system that can be used for
-                                    signal event handling. For more information see the
-                                    [Requests docs](https://requests.readthedocs.io/en/
-                                    master/user/advanced/#event-hooks)
+            controlNumber:
+                Control number associated with Local Bibliographic Data record.
+                Can be an integer or string.
+            responseFormat:
+                Format of returned record.
+
+                **OPTIONS:** `'application/marcxml+xml'` or `'application/marc'`
+            hooks:
+                Requests library hook system that can be used for signal event
+                handling. For more information see the [Requests docs](https://requests.
+                readthedocs.io/en/master/user/advanced/#event-hooks)
 
         Returns:
             `requests.Response` instance
         """
         url = self._url_manage_lbd(controlNumber)
         header = {"Accept": responseFormat}
 
@@ -1164,30 +1310,35 @@
         responseFormat: str = "application/marcxml+xml",
         hooks: Optional[Dict[str, Callable]] = None,
     ) -> Optional[Response]:
         """
         Given a Control Number, find the associated Local Bibliographic Data
         Record and replace it. If the Control Number is not found in
         WorldCat, then the provided Local Bibliographic Data Record will be created.
+
         Uses /manage/lbds/{controlNumber} endpoint.
 
         Args:
-            controlNumber:          control number associated with Local Bibliographic
-                                    Data record; can be an integer or string
-            record:                 MARC record to replace existing local
-                                    bibliographic record
-            recordFormat:           format of MARC record, options:
-                                    'application/marcxml+xml', 'application/marc'
-            responseFormat:         format of returned record; options:
-                                    'application/marcxml+xml', 'application/marc'
-                                    default is 'application/marcxml+xml'
-            hooks:                  Requests library hook system that can be used for
-                                    signal event handling. For more information see the
-                                    [Requests docs](https://requests.readthedocs.io/en/
-                                    master/user/advanced/#event-hooks)
+            controlNumber:
+                Control number associated with Local Bibliographic Data record.
+                Can be an integer or string.
+            record:
+                MARC record to replace existing Local Bibliographic Data record.
+            recordFormat:
+                Format of MARC record.
+
+                **OPTIONS:** `'application/marcxml+xml'` or `'application/marc'`
+            responseFormat:
+                Format of returned record.
+
+                **OPTIONS:** `'application/marcxml+xml'` or `'application/marc'`
+            hooks:
+                Requests library hook system that can be used for signal event
+                handling. For more information see the [Requests docs](https://requests.
+                readthedocs.io/en/master/user/advanced/#event-hooks)
 
         Returns:
             `requests.Response` instance
         """
         url = self._url_manage_lbd(controlNumber)
         header = {
             "Accept": responseFormat,
@@ -1208,27 +1359,32 @@
         record: str,
         recordFormat: str,
         responseFormat: str = "application/marcxml+xml",
         hooks: Optional[Dict[str, Callable]] = None,
     ) -> Optional[Response]:
         """
         Given a local holdings record, create it in WorldCat
+
         Uses /manage/lhrs endpoint.
 
         Args:
-            record:                 MARC holdings record to be created
-            recordFormat:           format of MARC holdings record, options:
-                                    'application/marcxml+xml', 'application/marc'
-            responseFormat:         format of returned record; options:
-                                    'application/marcxml+xml', 'application/marc'
-                                    default is 'application/marcxml+xml'
-            hooks:                  Requests library hook system that can be used for
-                                    signal event handling. For more information see the
-                                    [Requests docs](https://requests.readthedocs.io/en/
-                                    master/user/advanced/#event-hooks)
+            record:
+                MARC holdings record to be created.
+            recordFormat:
+                Format of MARC record.
+
+                **OPTIONS:** `'application/marcxml+xml'` or `'application/marc'`
+            responseFormat:
+                Format of returned record.
+
+                **OPTIONS:** `'application/marcxml+xml'` or `'application/marc'`
+            hooks:
+                Requests library hook system that can be used for signal event
+                handling. For more information see the [Requests docs](https://requests.
+                readthedocs.io/en/master/user/advanced/#event-hooks)
 
         Returns:
             `requests.Response` instance
         """
         url = self._url_manage_lhr_create()
         header = {
             "Accept": responseFormat,
@@ -1248,26 +1404,29 @@
         self,
         controlNumber: Union[int, str],
         responseFormat: str = "application/marcxml+xml",
         hooks: Optional[Dict[str, Callable]] = None,
     ) -> Optional[Response]:
         """
         Given a control number, delete a Local Holdings record.
+
         Uses /manage/lhrs/{controlNumber} endpoint.
 
         Args:
-            controlNumber:          control number associated with Local Holdings
-                                    record; can be an integer or string
-            responseFormat:         format of returned record, options:
-                                    'application/marcxml+xml', 'application/marc',
-                                    default is 'application/marcxml+xml'
-            hooks:                  Requests library hook system that can be used for
-                                    signal event handling. For more information see the
-                                    [Requests docs](https://requests.readthedocs.io/en/
-                                    master/user/advanced/#event-hooks)
+            controlNumber:
+                Control number associated with Local Holdings record.
+                Can be an integer or string.
+            responseFormat:
+                Format of returned record.
+
+                **OPTIONS:** `'application/marcxml+xml'` or `'application/marc'`
+            hooks:
+                Requests library hook system that can be used for signal event
+                handling. For more information see the [Requests docs](https://requests.
+                readthedocs.io/en/master/user/advanced/#event-hooks)
 
         Returns:
             `requests.Response` instance
         """
         url = self._url_manage_lhr(controlNumber)
         header = {"Accept": responseFormat}
 
@@ -1284,26 +1443,29 @@
         self,
         controlNumber: Union[int, str],
         responseFormat: str = "application/marcxml+xml",
         hooks: Optional[Dict[str, Callable]] = None,
     ) -> Optional[Response]:
         """
         Send a GET request for a local holdings record
+
         Uses /manage/lhrs/{controlNumber} endpoint.
 
         Args:
-            controlNumber:          control number associated with Local Holdings
-                                    record; can be an integer or string
-            responseFormat:         format of returned record, options:
-                                    'application/marcxml+xml', 'application/marc',
-                                    default is 'application/marcxml+xml'
-            hooks:                  Requests library hook system that can be used for
-                                    signal event handling. For more information see the
-                                    [Requests docs](https://requests.readthedocs.io/en/
-                                    master/user/advanced/#event-hooks)
+            controlNumber:
+                Control number associated with Local Holdings record.
+                Can be an integer or string.
+            responseFormat:
+                Format of returned record.
+
+                **OPTIONS:** `'application/marcxml+xml'` or `'application/marc'`
+            hooks:
+                Requests library hook system that can be used for signal event
+                handling. For more information see the [Requests docs](https://requests.
+                readthedocs.io/en/master/user/advanced/#event-hooks)
 
         Returns:
             `requests.Response` instance
         """
         url = self._url_manage_lhr(controlNumber)
         header = {"Accept": responseFormat}
 
@@ -1324,30 +1486,35 @@
         responseFormat: str = "application/marcxml+xml",
         hooks: Optional[Dict[str, Callable]] = None,
     ) -> Optional[Response]:
         """
         Given a Control Number, find the associated Local Holdings
         Record and replace it. If the Control Number is not found in
         WorldCat, then the provided Local Holdings Record will be created.
+
         Uses /manage/lhrs/{controlNumber} endpoint.
 
         Args:
-            controlNumber:          control number associated with Local Holdings
-                                    record; can be an integer or string
-            record:                 MARC holdings record to replace existing local
-                                    holdings record
-            recordFormat:           format of MARC holdings record, options:
-                                    'application/marcxml+xml', 'application/marc'
-            responseFormat:         format of returned record; options:
-                                    'application/marcxml+xml', 'application/marc'
-                                    default is 'application/marcxml+xml'
-            hooks:                  Requests library hook system that can be used for
-                                    signal event handling. For more information see the
-                                    [Requests docs](https://requests.readthedocs.io/en/
-                                    master/user/advanced/#event-hooks)
+            controlNumber:
+                Control number associated with Local Holdings record.
+                Can be an integer or string.
+            record:
+                MARC holdings record to replace existing local holdings record.
+            recordFormat:
+                Format of MARC record.
+
+                **OPTIONS:** `'application/marcxml+xml'` or `'application/marc'`
+            responseFormat:
+                Format of returned record.
+
+                **OPTIONS:** `'application/marcxml+xml'` or `'application/marc'`
+            hooks:
+                Requests library hook system that can be used for signal event
+                handling. For more information see the [Requests docs](https://requests.
+                readthedocs.io/en/master/user/advanced/#event-hooks)
 
         Returns:
             `requests.Response` instance
         """
         url = self._url_manage_lhr(controlNumber)
         header = {
             "Accept": responseFormat,
@@ -1366,23 +1533,25 @@
     def local_bibs_get(
         self,
         controlNumber: Union[int, str],
         hooks: Optional[Dict[str, Callable]] = None,
     ) -> Optional[Response]:
         """
         Retrieve LBD Resource.
+
         Uses /search/my-local-bib-data/{controlNumber} endpoint.
 
         Args:
-            controlNumber:          control number associated with Local Bibliographic
-                                    Data record; can be an integer or string
-            hooks:                  Requests library hook system that can be used for
-                                    signal event handling. For more information see the
-                                    [Requests docs](https://requests.readthedocs.io/en/
-                                    master/user/advanced/#event-hooks)
+            controlNumber:
+                Control number associated with Local Bibliographic Data record.
+                Can be an integer or string.
+            hooks:
+                Requests library hook system that can be used for signal event
+                handling. For more information see the [Requests docs](https://requests.
+                readthedocs.io/en/master/user/advanced/#event-hooks)
 
         Returns:
             `requests.Response` instance
         """
         url = self._url_search_lbd_control_number(controlNumber)
         header = {"Accept": "application/json"}
 
@@ -1399,42 +1568,46 @@
         self,
         q: str,
         offset: int = 1,
         limit: int = 10,
         hooks: Optional[Dict[str, Callable]] = None,
     ) -> Optional[Response]:
         """
-        Search LBD Resources using WorldCat query syntax.
-        See https://help.oclc.org/Librarian_Toolbox/Searching_WorldCat_Indexes/
-        Local_bibliographic_data_records/Local_bibliographic_data_record_indexes_A-Z
-        for more information on available indexes.
+        Search LBD Resources using WorldCat query syntax. See OCLC
+        [Local Bibliographic Data Record Index](https://help.oclc.org/Librarian_Toolbox/Searching_WorldCat_Indexes/Local_bibliographic_data_records/Local_bibliographic_data_record_indexes_A-Z)
+        Documentation for more information on available indexes.
+
         Uses /search/my-local-bib-data endpoint.
 
         Args:
-            q:                      query in the form of a keyword search or
-                                    fielded search;
-                                    examples:
-                                        ti:Zendegi
-                                        ti:"Czarne oceany"
-                                        bn:9781680502404
-                                        kw:python databases
-                                        ti:Zendegi AND au:greg egan
-                                        (au:Okken OR au:Myers) AND su:python
-            offset:                 start position of bibliographic records to
-                                    return; default is 1
-            limit:                  maximum number of records to return;
-                                    maximum is 50, default is 10
-            hooks:                  Requests library hook system that can be used for
-                                    signal event handling. For more information see the
-                                    [Requests docs](https://requests.readthedocs.io/en/
-                                    master/user/advanced/#event-hooks)
+            q:
+                Query in the form of a keyword search or fielded search.
+
+                **EXAMPLES:**
+
+                - `ti:Zendegi`
+                - `ti:"Czarne oceany"`
+                - `bn:9781680502404`
+                - `kw:python databases`
+                - `ti:Zendegi AND au:greg egan`
+                - `(au:Okken OR au:Myers) AND su:python`
+            offset:
+                Start position of bibliographic records to return.
+            limit:
+                Maximum number of records to return.
+
+                **MAXIMUM:** `50`
+            hooks:
+                Requests library hook system that can be used for signal event
+                handling. For more information see the [Requests docs](https://requests.
+                readthedocs.io/en/master/user/advanced/#event-hooks)
 
         Returns:
             `requests.Response` instance
-        """
+        """  # noqa: E501
         url = self._url_search_lbd()
         header = {"Accept": "application/json"}
         payload = {"q": q, "offset": offset, "limit": limit}
 
         # prep request
         req = Request("GET", url, params=payload, headers=header, hooks=hooks)
         prepared_request = self.prepare_request(req)
@@ -1452,31 +1625,37 @@
         oclcNumber: Optional[Union[int, str]] = None,
         browsePosition: int = 0,
         limit: int = 10,
         hooks: Optional[Dict[str, Callable]] = None,
     ) -> Optional[Response]:
         """
         Browse local holdings.
+
         Uses /browse/my-holdings endpoint.
 
         Args:
-            holdingLocation:        holding location for item
-            shelvingLocation:       shelving location for item
-            callNumber:             call number for item
-            oclcNumber:             OCLC bibliographic record number; can be an
-                                    integer or string with or without OCLC Number
-                                    prefix
-            browsePosition:         position within browse list where the matching
-                                    record should be, default is 0
-            limit:                  maximum number of records to return;
-                                    maximum is 50, default is 10
-            hooks:                  Requests library hook system that can be used for
-                                    signal event handling. For more information see the
-                                    [Requests docs](https://requests.readthedocs.io/en/
-                                    master/user/advanced/#event-hooks)
+            holdingLocation:
+                Holding location for item.
+            shelvingLocation:
+                Shelving location for item.
+            callNumber:
+                Call number for item.
+            oclcNumber:
+                OCLC bibliographic record number. Can be an integer or string
+                with or without OCLC Number prefix.
+            browsePosition:
+                Position within browse list where the matching record should be.
+            limit:
+                Maximum number of records to return.
+
+                **MAXIMUM:** `50`
+            hooks:
+                Requests library hook system that can be used for signal event
+                handling. For more information see the [Requests docs](https://requests.
+                readthedocs.io/en/master/user/advanced/#event-hooks)
 
         Returns:
             `requests.Response` instance
         """
         if oclcNumber is not None:
             oclcNumber = verify_oclc_number(oclcNumber)
 
@@ -1503,23 +1682,25 @@
     def local_holdings_get(
         self,
         controlNumber: Union[int, str],
         hooks: Optional[Dict[str, Callable]] = None,
     ) -> Optional[Response]:
         """
         Retrieve LHR Resource.
+
         Uses /search/my-holdings/{controlNumber} endpoint.
 
         Args:
-            controlNumber:          control number associated with Local Holdings
-                                    record; can be an integer or string
-            hooks:                  Requests library hook system that can be used for
-                                    signal event handling. For more information see the
-                                    [Requests docs](https://requests.readthedocs.io/en/
-                                    master/user/advanced/#event-hooks)
+            controlNumber:
+                Control number associated with Local Holdings record.
+                Can be an integer or string.
+            hooks:
+                Requests library hook system that can be used for signal event
+                handling. For more information see the [Requests docs](https://requests.
+                readthedocs.io/en/master/user/advanced/#event-hooks)
 
         Returns:
             `requests.Response` instance
         """
         url = self._url_search_lhr_control_number(controlNumber)
         header = {"Accept": "application/json"}
 
@@ -1539,36 +1720,38 @@
         orderBy: str = "oclcSymbol",
         offset: int = 1,
         limit: int = 10,
         hooks: Optional[Dict[str, Callable]] = None,
     ) -> Optional[Response]:
         """
         Search LHR Resources. Query must contain, at minimum, either an
-        OCLC Number or barcode.
+        `oclcNumber` or `barcode`.
+
         Uses /search/my-holdings endpoint.
 
         Args:
-            oclcNumber:             OCLC bibliographic record number; can be an
-                                    integer or string with or without OCLC Number
-                                    prefix
-            barcode:                barcode as a string,
-            orderBy:                results sort key;
-                                    options:
-                                        'commitmentExpirationDate'
-                                        'location'
-                                        'oclcSymbol'
-                                    default is 'oclcSymbol'
-            offset:                 start position of bibliographic records to
-                                    return; default is 1
-            limit:                  maximum number of records to return;
-                                    maximum is 50, default is 10
-            hooks:                  Requests library hook system that can be used for
-                                    signal event handling. For more information see the
-                                    [Requests docs](https://requests.readthedocs.io/en/
-                                    master/user/advanced/#event-hooks)
+            oclcNumber:
+                OCLC bibliographic record number. Can be an integer or string
+                with or without OCLC Number prefix.
+            barcode:
+                Barcode as a string.
+            orderBy:
+                Results sort key.
+
+                **OPTIONS:** `'commitmentExpirationDate'`, `'location'`, `'oclcSymbol'`
+            offset:
+                Start position of bibliographic records to return.
+            limit:
+                Maximum number of records to return.
+
+                **MAXIMUM:** `50`
+            hooks:
+                Requests library hook system that can be used for signal event
+                handling. For more information see the [Requests docs](https://requests.
+                readthedocs.io/en/master/user/advanced/#event-hooks)
 
         Returns:
             `requests.Response` instance
         """
         if oclcNumber is not None:
             oclcNumber = verify_oclc_number(oclcNumber)
 
@@ -1601,42 +1784,46 @@
         orderBy: str = "oclcSymbol",
         offset: int = 1,
         limit: int = 10,
         hooks: Optional[Dict[str, Callable]] = None,
     ) -> Optional[Response]:
         """
         Search for shared print LHR Resources. Query must contain, at minimum,
-        either an OCLC Number or barcode and a value for either heldBySymbol,
-        heldByInstitutionID or spProgram.
+        either an `oclcNumber` or `barcode` and a value for either
+        `heldBySymbol`, `heldByInstitutionID` or `spProgram`.
+
         Uses /search/retained-holdings endpoint.
 
         Args:
-            oclcNumber:             OCLC bibliographic record number; can be an
-                                    integer or string with or without OCLC Number
-                                    prefix
-            barcode:                barcode as a string,
-            heldBySymbol:           restricts to holdings with specified institution
-                                    symbol
-            heldByInstitutionID:    restrict to specified institution registryId
-            spProgram:              restricts responses to bibliographic records
-                                    associated with particular shared print program
-            orderBy:                results sort key;
-                                    options:
-                                        'commitmentExpirationDate'
-                                        'location'
-                                        'oclcSymbol'
-                                    default is 'oclcSymbol'
-            offset:                 start position of bibliographic records to
-                                    return; default is 1
-            limit:                  maximum number of records to return;
-                                    maximum is 50, default is 10
-            hooks:                  Requests library hook system that can be used for
-                                    signal event handling. For more information see the
-                                    [Requests docs](https://requests.readthedocs.io/en/
-                                    master/user/advanced/#event-hooks)
+            oclcNumber:
+                OCLC bibliographic record number. Can be an integer or string
+                with or without OCLC Number prefix.
+            barcode:
+                Barcode as a string.
+            heldBySymbol:
+                Restricts to holdings with specified institution symbol.
+            heldByInstitutionID:
+                Restrict to specified institution registryId.
+            spProgram:
+                Limits response to bibliographic records associated with
+                particular shared print program.
+            orderBy:
+                Results sort key.
+
+                **OPTIONS:** `'commitmentExpirationDate'`, `'location'`, `'oclcSymbol'`
+            offset:
+                Start position of bibliographic records to return.
+            limit:
+                Maximum number of records to return.
+
+                **MAXIMUM:** `50`
+            hooks:
+                Requests library hook system that can be used for signal event
+                handling. For more information see the [Requests docs](https://requests.
+                readthedocs.io/en/master/user/advanced/#event-hooks)
 
         Returns:
             `requests.Response` instance
         """
         if oclcNumber is not None:
             oclcNumber = verify_oclc_number(oclcNumber)
 
@@ -1671,34 +1858,48 @@
         heldInState: Optional[str] = None,
         itemType: Optional[List[str]] = None,
         itemSubType: Optional[List[str]] = None,
         hooks: Optional[Dict[str, Callable]] = None,
     ) -> Optional[Response]:
         """
         Finds member shared print holdings for specified item. Query must
-        contain, at minimum, either an OCLC Number, ISBN, or ISSN.
+        contain, at minimum, either an `oclcNumber`, `isbn`, or `issn`.
+
         Uses /search/bibs-retained-holdings endpoint.
 
         Args:
-            oclcNumber:             OCLC bibliographic record number; can be an
-                                    integer or string with or without OCLC Number
-                                    prefix
-            isbn:                   ISBN without any dashes, example: '978149191646x'
-            issn:                   ISSN hyphenated, example: '0099-1234'
-            heldByGroup:            restricts to holdings held by group symbol
-            heldInState:            restricts to holdings held by institutions
-                                    in requested state, example: "NY"
-            itemType:               restricts results to specified item type (example
-                                    'book' or 'vis')
-            itemSubType:            restricts results to specified item sub type
-                                    examples: 'book-digital' or 'audiobook-cd'
-            hooks:                  Requests library hook system that can be used for
-                                    signal event handling. For more information see the
-                                    [Requests docs](https://requests.readthedocs.io/en/
-                                    master/user/advanced/#event-hooks)
+            oclcNumber:
+                OCLC bibliographic record number. Can be an integer or string
+                with or without OCLC Number prefix.
+            isbn:
+                ISBN without any dashes.
+
+                **EXAMPLE:** `'978149191646x'`
+            issn:
+                ISSN, hyphenated.
+
+                **EXAMPLE:** `'0099-1234'`
+            heldByGroup:
+                Restricts to holdings held by group symbol.
+            heldInState:
+                Restricts to holdings held by institutions in requested state.
+
+                **EXAMPLE:** `'US-NY'`
+            itemType:
+                Limits response to specified item type.
+
+                **EXAMPLES:** `'book'`, `'vis'`
+            itemSubType:
+                Limits response to specified item sub type
+
+                **EXAMPLES:** `'book-digital'`, `'audiobook-cd'`
+            hooks:
+                Requests library hook system that can be used for signal event
+                handling. For more information see the [Requests docs](https://requests.
+                readthedocs.io/en/master/user/advanced/#event-hooks)
 
         Returns:
             `requests.Response` instance
         """
         if oclcNumber is not None:
             oclcNumber = verify_oclc_number(oclcNumber)
 
@@ -1743,56 +1944,85 @@
         distance: Optional[int] = None,
         unit: str = "M",
         hooks: Optional[Dict[str, Callable]] = None,
     ) -> Optional[Response]:
         """
         Given a known item, get summary of holdings and brief bib record. Query must
         contain, at minimum, either an OCLC Number, ISBN, or ISSN. Query may contain
-        only one of: heldByInstitutionId, heldByGroup, heldBySymbol, heldInCountry,
-        heldInState or combination of lat, lon and distance. If using lat/lon
-        arguments, query must contain a valid distance argument.
+        only one of: `heldByInstitutionId`, `heldByGroup`, `heldBySymbol`,
+        `heldInCountry`, `heldInState` or combination of `lat`, `lon` and
+        `distance`. If using lat/lon arguments, query must contain a valid
+        distance argument.
+
         Uses /search/bibs-summary-holdings endpoint.
 
         Args:
-            oclcNumber:                 OCLC bibliographic record number; can be an
-                                        integer or string with or without OCLC Number
-                                        prefix
-            isbn:                       ISBN without any dashes,
-                                        example: '978149191646x'
-            issn:                       ISSN (hyphenated, example: '0099-1234')
-            holdingsAllEditions:        get holdings for all editions;
-                                        options: True or False
-            holdingsAllVariantRecords:  get holdings for specific edition across
-                                        variant records; options: False, True
-            preferredLanguage:          language of metadata description;
-                                        default 'eng' (English)
-            holdingsFilterFormat:       get holdings for specific itemSubType,
-                                        example: book-digital
-            heldInCountry:              restricts to holdings held by institutions
-                                        in requested country
-            heldInState:                limits to holdings held by institutions
-                                        in requested state, example: 'US-NY'
-            heldByGroup:                limits to holdings held by indicated by
-                                        symbol group
-            heldBySymbol:               limits to holdings held by institutions
-                                        indicated by institution symbol
-            heldByInstitutionID:        limits to holdings held by institutions
-                                        indicated by institution registryID
-            heldByLibraryType:          limits to holdings held by library type,
-                                        options: 'PUBLIC', 'ALL'
-            lat:                        limit to latitude, example: 37.502508,
-            lon:                        limit to longitute, example: -122.22702
-            distance:                   distance from latitude and longitude
-            unit:                       unit of distance param; options:
-                                        'M' (miles) or 'K' (kilometers), default is 'M'
-            hooks:                      Requests library hook system that can be used
-                                        for signal event handling. For more information
-                                        see the [Requests docs](https://requests.
-                                        readthedocs.io/en/master/user/advanced/
-                                        #event-hooks)
+            oclcNumber:
+                OCLC bibliographic record number. Can be an integer or string
+                with or without OCLC Number prefix.
+            isbn:
+                ISBN without any dashes.
+
+                **EXAMPLE:** `'978149191646x'`
+            issn:
+                ISSN, hyphenated.
+
+                **EXAMPLE:** `'0099-1234'`
+            holdingsAllEditions:
+                Get holdings for all editions.
+
+                **OPTIONS:** `True` or `False`
+            holdingsAllVariantRecords:
+                Get holdings for specific edition across variant records.
+
+                **OPTIONS:** `True` or `False`
+            preferredLanguage:
+                Language user would prefer metadata description in. Does not limit
+                responses. To limit responses use `inCataloglanguage` facet.
+            holdingsFilterFormat:
+                Get holdings for specific itemSubType.
+
+                **EXAMPLE:** `'book-digital'`
+            heldInCountry:
+                Restricts to holdings held by institutions in requested country.
+            heldInState:
+                Restricts to holdings held by institutions in requested state.
+
+                **EXAMPLE:** `'US-NY'`
+            heldByGroup:
+                Restricts to holdings held by group symbol.
+            heldBySymbol:
+                Limits to holdings held by institutions indicated by
+                institution symbol.
+            heldByInstitutionID:
+                Limits to holdings held by institutions indicated by institution
+                registryID.
+            heldByLibraryType:
+                Limits to holdings held by library type.
+
+                **OPTIONS:** `'PUBLIC'`, `'ALL'`
+            lat:
+                Latitude
+
+                **EXAMPLE:** `37.502508`
+            lon:
+                Longitude
+
+                **EXAMPLE:** `-122.22702`
+            distance:
+                Limits results to holdings held by institutions within specified
+                distance from latitude and longitude.
+            unit:
+                Unit of distance from latitude and longitude.
+
+                **OPTIONS:** `'M'` (miles) or `'K'` (kilometers).
+            hooks:
+                Requests library hook system that can be used for signal event
+                handling. For more information see the [Requests docs](https://requests.
+                readthedocs.io/en/master/user/advanced/#event-hooks)
 
         Returns:
             `requests.Response` instance
         """
         if oclcNumber is not None:
             oclcNumber = verify_oclc_number(oclcNumber)
 
@@ -1843,51 +2073,74 @@
         lon: Optional[float] = None,
         distance: Optional[int] = None,
         unit: str = "M",
         hooks: Optional[Dict[str, Callable]] = None,
     ) -> Optional[Response]:
         """
         Given an OCLC number, get summary of holdings. Query may contain
-        only one of: heldByInstitutionId, heldByGroup, heldBySymbol, heldInCountry,
-        heldInState or combination of lat, lon and distance. If using lat/lon
-        arguments, query must contain a valid distance argument.
+        only one of: `heldByInstitutionId`, `heldByGroup`, `heldBySymbol`,
+        `heldInCountry`, `heldInState` or combination of `lat`, `lon` and
+        `distance`. If using lat/lon arguments, query must contain a valid
+        distance argument.
+
         Uses /search/summary-holdings endpoint.
 
         Args:
-            oclcNumber:                 OCLC bibliographic record number; can be an
-                                        integer or string with or without OCLC Number
-                                        prefix
-            holdingsAllEditions:        get holdings for all editions;
-                                        options: True, False
-            holdingsAllVariantRecords:  get holdings for specific edition across
-                                        all variant records; options: True, False
-            holdingsFilterFormat:       get holdings for specific itemSubType,
-                                        example: book-digital
-            heldInCountry:              limits to holdings held by institutions
-                                        in requested country
-            heldInState:                limits to holdings held by institutions
-                                        in requested state, example: 'US-NY'
-            heldByGroup:                limits to holdings held by institutions
-                                        indicated by group symbol
-            heldBySymbol:               limits to holdings held by institutions
-                                        indicated by institution symbol
-            heldByInstitutionID:        limits to holdings held by institutions
-                                        indicated by institution registryID
-            heldByLibraryType:          limits to holdings held by library type,
-                                        options: 'PUBLIC', 'ALL'
-            lat:                        limit to latitude, example: 37.502508
-            lon:                        limit to longitute, example: -122.22702
-            distance:                   distance from latitude and longitude
-            unit:                       unit of distance param; options:
-                                        'M' (miles) or 'K' (kilometers), default is 'M'
-            hooks:                      Requests library hook system that can be used
-                                        for signal event handling. For more information
-                                        see the [Requests docs](https://requests.
-                                        readthedocs.io/en/master/user/advanced/
-                                        #event-hooks)
+            oclcNumber:
+                OCLC bibliographic record number. Can be an integer or string
+                with or without OCLC Number prefix.
+            holdingsAllEditions:
+                Get holdings for all editions.
+
+                **OPTIONS:** `True` or `False`
+            holdingsAllVariantRecords:
+                Get holdings for specific edition across variant records.
+
+                **OPTIONS:** `True` or `False`
+            holdingsFilterFormat:
+                Get holdings for specific itemSubType.
+
+                **EXAMPLE:** `'book-digital'`
+            heldInCountry:
+                Restricts to holdings held by institutions in requested country.
+            heldInState:
+                Restricts to holdings held by institutions in requested state.
+
+                **EXAMPLE:** `'US-NY'`
+            heldByGroup:
+                Restricts to holdings held by group symbol.
+            heldBySymbol:
+                Limits to holdings held by institutions indicated by
+                institution symbol.
+            heldByInstitutionID:
+                Limits to holdings held by institutions indicated by institution
+                registryID.
+            heldByLibraryType:
+                Limits to holdings held by library type.
+
+                **OPTIONS:** `'PUBLIC'`, `'ALL'`
+            lat:
+                Latitude
+
+                **EXAMPLE:** `37.502508`
+            lon:
+                Longitude
+
+                **EXAMPLE:** `-122.22702`
+            distance:
+                Limits results to holdings held by institutions within specified
+                distance from latitude and longitude.
+            unit:
+                Unit of distance from latitude and longitude.
+
+                **OPTIONS:** `'M'` (miles) or `'K'` (kilometers).
+            hooks:
+                Requests library hook system that can be used for signal event
+                handling. For more information see the [Requests docs](https://requests.
+                readthedocs.io/en/master/user/advanced/#event-hooks)
 
         Returns:
             `requests.Response` instance
         """
         oclcNumber = verify_oclc_number(oclcNumber)
 
         url = self._url_search_general_holdings_summary()
```

### Comparing `bookops_worldcat-1.0.0/bookops_worldcat/query.py` & `bookops_worldcat-1.0.1/bookops_worldcat/query.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,55 +1,59 @@
 # -*- coding: utf-8 -*-
 
-"""
-Handles actual requests to OCLC services
-"""
+"""Handles requests to OCLC web services."""
+
 from __future__ import annotations
-from typing import Optional, Union, Tuple, TYPE_CHECKING
+from typing import Union, Tuple, TYPE_CHECKING
 import sys
 
 from requests.models import PreparedRequest
 from requests.exceptions import ConnectionError, HTTPError, Timeout, RetryError
 from .errors import WorldcatRequestError
 
 
 if TYPE_CHECKING:
     from .metadata_api import MetadataSession  # pragma: no cover
 
 
 class Query:
-    """
-    Sends a request to OCLC service and unifies exceptions.
-    Query object handles refreshing expired token before request is
-    made to the web service.
-
-    `Query.response` attribute is `requests.Response` instance that
-    can be parsed to extract information received from the web service.
+    """Sends a request to OCLC web service and unifies exceptions.
 
+    Query object handles automatic refresh of expired token before each
+    request is made to the web service. `Query.response` attribute is
+    [`requests.Response`](https://requests.readthedocs.io/en/latest/api/#requests.PreparedRequest)
+    instance that can be parsed to extract information received from the web service.
     """
 
     def __init__(
         self,
         session: MetadataSession,
         prepared_request: PreparedRequest,
-        timeout: Optional[
-            Union[int, float, Tuple[int, int], Tuple[float, float]]
-        ] = None,
+        timeout: Union[int, float, Tuple[int, int], Tuple[float, float], None] = (
+            5,
+            5,
+        ),
     ) -> None:
         """Initializes Query object.
 
         Args:
-            session:                        `metadata_api.MetadataSession` instance
-            prepared_request:               `requests.models.PreparedRequest` instance
-            timeout:                        how long to wait for server to send data
-                                            before giving up
-
+            session:
+                `metadata_api.MetadataSession` instance.
+            prepared_request:
+                `requests.PreparedRequest` instance.
+            timeout:
+                How long to wait for server to send data before giving up. Accepts
+                separate values for connect and read timeouts or a single value.
 
         Raises:
-            WorldcatRequestError: If the request encounters an error
+            WorldcatRequestError:
+                If the request encounters any errors.
+            TypeError:
+                If `prepared_request` arg is passed anything other than a
+                `requests.PreparedRequest` object.
         """
         if not isinstance(prepared_request, PreparedRequest):
             raise TypeError("Invalid type for argument 'prepared_request'.")
 
         # make sure access token is still valid and if not request a new one
         if session.authorization.is_expired():
             session._get_new_access_token()
```

### Comparing `bookops_worldcat-1.0.0/bookops_worldcat/utils.py` & `bookops_worldcat-1.0.1/bookops_worldcat/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 """
 Shared utilities module.
 """
-
+import re
 from typing import List, Union
 
 from .errors import InvalidOclcNumber
 
 
 def _str2list(s: str) -> List[str]:
     """Converts str into list - use for list of OCLC numbers"""
@@ -15,81 +15,99 @@
 
 
 def prep_oclc_number_str(oclcNumber: str) -> str:
     """
     Checks for OCLC prefixes and removes them.
 
     Args:
-        oclcNumber:                OCLC record as string
+        oclcNumber:
+            OCLC record number as string
 
     Returns:
-        oclcNumber as str
+        `oclcNumber` as str
+
+    Raises:
+        InvalidOclcNumber: If `oclcNumber` argument does not match
+        OCLC number formatting rules.
     """
 
-    if oclcNumber.strip().startswith("ocm") or oclcNumber.strip().startswith("ocn"):
+    if re.match(r"^ocm[0-9]{,8}$", oclcNumber.strip()) or re.match(
+        r"^ocn[0-9]{9}$", oclcNumber.strip()
+    ):
         oclcNumber = oclcNumber.strip()[3:]
-    elif oclcNumber.strip().startswith("on"):
+    elif re.match(r"^on[0-9]{10,}$", oclcNumber.strip()):
         oclcNumber = oclcNumber.strip()[2:]
+    elif re.match(r"^\(OCoLC\)[0-9]{8,}$", oclcNumber.strip()):
+        oclcNumber = oclcNumber.strip()[7:]
 
     try:
         oclcNumber = str(int(oclcNumber))
         return oclcNumber
     except ValueError:
         raise InvalidOclcNumber("Argument 'oclcNumber' does not look like real OCLC #.")
 
 
 def verify_oclc_number(oclcNumber: Union[int, str]) -> str:
     """
     Verifies a valid looking OCLC number is passed and normalize it as integer.
 
     Args:
-        oclcNumber:                OCLC record number
+        oclcNumber:
+            OCLC record number as string or integer
 
     Returns:
-        oclcNumber as str
+        `oclcNumber` as str
 
+    Raises:
+        InvalidOclcNumber: If `oclcNumber` argument is not a str or int or is missing.
     """
     if not oclcNumber:
         raise InvalidOclcNumber("Argument 'oclcNumber' is missing.")
 
     elif isinstance(oclcNumber, int):
         return str(oclcNumber)
 
     elif isinstance(oclcNumber, str):
         return prep_oclc_number_str(oclcNumber)
 
     else:
         raise InvalidOclcNumber("Argument 'oclcNumber' is of invalid type.")
 
 
-def verify_oclc_numbers(oclcNumbers: Union[str, List[Union[str, int]]]) -> List[str]:
+def verify_oclc_numbers(
+    oclcNumbers: Union[int, str, List[Union[str, int]]]
+) -> List[str]:
     """
     Parses and verifies list of oclcNumbers
 
     Args:
-        oclcNumbers:            list of OCLC control numbers for which holdings
-                                should be set;
-                                they can be integers or strings with or without
-                                OCLC # prefix;
-                                if str the numbers must be separated by comma
+        oclcNumbers:
+            List of OCLC control numbers. Control numbers can be integers or strings
+            with or without OCLC # prefix. If str, the numbers must be separated
+            by commas. If int, only one number will be parsed. Lists may contain strings
+            or integers or a combination of both.
 
     Returns:
-        vetted_numbers as list
+        `oclcNumbers` as a list of strings
 
+    Raises:
+        InvalidOclcNumber: If `oclcNumbers` argument is not a list, str, or int.
     """
     if isinstance(oclcNumbers, str):
         oclcNumbers_lst = _str2list(oclcNumbers)
+    elif isinstance(oclcNumbers, int):
+        oclcNumbers_lst = _str2list(str(oclcNumbers))
     elif isinstance(oclcNumbers, list):
-        oclcNumbers_lst = oclcNumbers  # type: ignore
+        oclcNumbers_lst = [str(n) for n in oclcNumbers]
     else:
         raise InvalidOclcNumber(
-            "Argument 'oclcNumbers' must be a list or comma separated string "
-            "of valid OCLC #s."
+            "Argument 'oclcNumbers' must be a single integer, a list or a "
+            "comma separated string of valid OCLC #s."
         )
     if not oclcNumbers_lst:
         raise InvalidOclcNumber(
-            "Argument 'oclcNumbers' must be a list or comma separated string "
-            "of valid OCLC #s."
+            "Argument 'oclcNumbers' must be a single integer, a list or a "
+            "comma separated string of valid OCLC #s."
         )
 
     vetted_numbers = [verify_oclc_number(n) for n in oclcNumbers_lst]
     return vetted_numbers
```

### Comparing `bookops_worldcat-1.0.0/LICENSE` & `bookops_worldcat-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bookops_worldcat-1.0.0/pyproject.toml` & `bookops_worldcat-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bookops-worldcat"
-version = "1.0.0"
+version = "1.0.1"
 description = "OCLC WorldCat Metadata APIs wrapper"
 authors = ["Tomasz Kalata <klingaroo@gmail.com>", "Charlotte Kostelic <charlottekostelic@gmail.com>"]
 license = "MIT"
 exclude = ["bookops_worldcat/temp.py", "bookops_worldcat/temp/*"]
 
 packages = [
     {include = "bookops_worldcat"},
@@ -42,15 +42,15 @@
 "Bug Tracker" = "https://github.com/BookOps-CAT/bookops-worldcat/issues"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.0"
 pytest-cov = "^3.0"
 pytest-mock = "^3.7"
 mkdocs = "^1.4"
-black = "^23.3.0"
+black = "^24.3.0"
 mike = "^2.0.0"
 mypy = "^1.8"
 types-requests = "^2.31.0.20240125"
 mkdocs-material = "^9.5.13"
 mkdocstrings = "^0.24.1"
 mkdocstrings-python = "^1.9.0"
```

### Comparing `bookops_worldcat-1.0.0/README.md` & `bookops_worldcat-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `bookops_worldcat-1.0.0/PKG-INFO` & `bookops_worldcat-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bookops-worldcat
-Version: 1.0.0
+Version: 1.0.1
 Summary: OCLC WorldCat Metadata APIs wrapper
 Home-page: https://bookops-cat.github.io/bookops-worldcat/
 License: MIT
 Keywords: api,api-wrapper,oclc,worldcat,cataloging,bibliographic records,marcxml,holdings,library metadata,marc21
 Author: Tomasz Kalata
 Author-email: klingaroo@gmail.com
 Requires-Python: >=3.8,<4.0
```

