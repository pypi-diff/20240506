# Comparing `tmp/fastapi_jwt-0.2.0-py3-none-any.whl.zip` & `tmp/fastapi_jwt-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,14 @@
-Zip file size: 6271 bytes, number of entries: 7
--rw-r--r--  2.0 unx       39 b- defN 23-Nov-02 09:37 fastapi_jwt/__init__.py
--rw-r--r--  2.0 unx    16251 b- defN 23-Nov-02 09:37 fastapi_jwt/jwt.py
--rw-r--r--  2.0 unx     1078 b- defN 23-Nov-02 09:37 fastapi_jwt-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     4722 b- defN 23-Nov-02 09:37 fastapi_jwt-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Nov-02 09:37 fastapi_jwt-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Nov-02 09:37 fastapi_jwt-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      560 b- defN 23-Nov-02 09:37 fastapi_jwt-0.2.0.dist-info/RECORD
-7 files, 22754 bytes uncompressed, 5277 bytes compressed:  76.8%
+Zip file size: 9059 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       87 b- defN 24-May-06 19:00 fastapi_jwt/__init__.py
+-rw-r--r--  2.0 unx    15301 b- defN 24-May-06 19:00 fastapi_jwt/jwt.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-06 19:00 fastapi_jwt/py.typed
+-rw-r--r--  2.0 unx      275 b- defN 24-May-06 19:00 fastapi_jwt/jwt_backends/__init__.py
+-rw-r--r--  2.0 unx      676 b- defN 24-May-06 19:00 fastapi_jwt/jwt_backends/abstract_backend.py
+-rw-r--r--  2.0 unx     1847 b- defN 24-May-06 19:00 fastapi_jwt/jwt_backends/authlib_backend.py
+-rw-r--r--  2.0 unx     1767 b- defN 24-May-06 19:00 fastapi_jwt/jwt_backends/python_jose_backend.py
+-rw-r--r--  2.0 unx     1078 b- defN 24-May-06 19:00 fastapi_jwt-0.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5189 b- defN 24-May-06 19:00 fastapi_jwt-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-06 19:00 fastapi_jwt-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-May-06 19:00 fastapi_jwt-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1030 b- defN 24-May-06 19:00 fastapi_jwt-0.3.0.dist-info/RECORD
+12 files, 27354 bytes uncompressed, 7305 bytes compressed:  73.3%
```

## zipnote {}

```diff
@@ -1,22 +1,37 @@
 Filename: fastapi_jwt/__init__.py
 Comment: 
 
 Filename: fastapi_jwt/jwt.py
 Comment: 
 
-Filename: fastapi_jwt-0.2.0.dist-info/LICENSE
+Filename: fastapi_jwt/py.typed
 Comment: 
 
-Filename: fastapi_jwt-0.2.0.dist-info/METADATA
+Filename: fastapi_jwt/jwt_backends/__init__.py
 Comment: 
 
-Filename: fastapi_jwt-0.2.0.dist-info/WHEEL
+Filename: fastapi_jwt/jwt_backends/abstract_backend.py
 Comment: 
 
-Filename: fastapi_jwt-0.2.0.dist-info/top_level.txt
+Filename: fastapi_jwt/jwt_backends/authlib_backend.py
 Comment: 
 
-Filename: fastapi_jwt-0.2.0.dist-info/RECORD
+Filename: fastapi_jwt/jwt_backends/python_jose_backend.py
+Comment: 
+
+Filename: fastapi_jwt-0.3.0.dist-info/LICENSE
+Comment: 
+
+Filename: fastapi_jwt-0.3.0.dist-info/METADATA
+Comment: 
+
+Filename: fastapi_jwt-0.3.0.dist-info/WHEEL
+Comment: 
+
+Filename: fastapi_jwt-0.3.0.dist-info/top_level.txt
+Comment: 
+
+Filename: fastapi_jwt-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fastapi_jwt/__init__.py

```diff
@@ -1 +1,2 @@
 from .jwt import *  # noqa: F401, F403
+from .jwt_backends import *  # noqa: F401, F403
```

## fastapi_jwt/jwt.py

```diff
@@ -1,36 +1,48 @@
 from abc import ABC
 from datetime import datetime, timedelta
-from typing import Any, Dict, Optional, Set
+from typing import Any, Dict, Optional, Set, Type
 from uuid import uuid4
 
 from fastapi.exceptions import HTTPException
 from fastapi.param_functions import Security
 from fastapi.responses import Response
 from fastapi.security import APIKeyCookie, HTTPBearer
 from starlette.status import HTTP_401_UNAUTHORIZED
 
-try:
-    from jose import jwt
-except ImportError:  # pragma: nocover
-    jwt = None  # type: ignore[assignment]
+from .jwt_backends import AbstractJWTBackend, authlib_backend, python_jose_backend
+from .jwt_backends.abstract_backend import BackendException
 
+DEFAULT_JWT_BACKEND: Optional[Type[AbstractJWTBackend]] = None
+if authlib_backend.authlib_jose is not None:
+    DEFAULT_JWT_BACKEND = authlib_backend.AuthlibJWTBackend
+elif python_jose_backend.jose is not None:
+    DEFAULT_JWT_BACKEND = python_jose_backend.PythonJoseJWTBackend
+else:  # pragma: nocover
+    raise ImportError("No JWT backend found, please install 'python-jose' or 'authlib'")
 
-def utcnow():
+
+def force_jwt_backend(cls: Type[AbstractJWTBackend]) -> None:
+    global DEFAULT_JWT_BACKEND
+    DEFAULT_JWT_BACKEND = cls
+
+
+def utcnow() -> datetime:
     try:
         from datetime import UTC
     except ImportError:  # pragma: nocover
         # UTC was added in python 3.12, as datetime.utcnow was
         # marked for deprecation.
         return datetime.utcnow()
     else:
         return datetime.now(UTC)
 
 
 __all__ = [
+    "force_jwt_backend",
     "JwtAuthorizationCredentials",
     "JwtAccessBearer",
     "JwtAccessCookie",
     "JwtAccessBearerCookie",
     "JwtRefreshBearer",
     "JwtRefreshCookie",
     "JwtRefreshBearerCookie",
@@ -45,110 +57,78 @@
     def __getitem__(self, item: str) -> Any:
         return self.subject[item]
 
 
 class JwtAuthBase(ABC):
     class JwtAccessCookie(APIKeyCookie):
         def __init__(self, *args: Any, **kwargs: Any):
-            APIKeyCookie.__init__(
-                self, *args, name="access_token_cookie", auto_error=False, **kwargs
-            )
+            APIKeyCookie.__init__(self, *args, name="access_token_cookie", auto_error=False, **kwargs)
 
     class JwtRefreshCookie(APIKeyCookie):
         def __init__(self, *args: Any, **kwargs: Any):
-            APIKeyCookie.__init__(
-                self, *args, name="refresh_token_cookie", auto_error=False, **kwargs
-            )
+            APIKeyCookie.__init__(self, *args, name="refresh_token_cookie", auto_error=False, **kwargs)
 
     class JwtAccessBearer(HTTPBearer):
         def __init__(self, *args: Any, **kwargs: Any):
             HTTPBearer.__init__(self, *args, auto_error=False, **kwargs)
 
     class JwtRefreshBearer(HTTPBearer):
         def __init__(self, *args: Any, **kwargs: Any):
             HTTPBearer.__init__(self, *args, auto_error=False, **kwargs)
 
     def __init__(
         self,
         secret_key: str,
         places: Optional[Set[str]] = None,
         auto_error: bool = True,
-        algorithm: str = jwt.ALGORITHMS.HS256,  # type: ignore[attr-defined]
+        algorithm: Optional[str] = None,
         access_expires_delta: Optional[timedelta] = None,
         refresh_expires_delta: Optional[timedelta] = None,
     ):
-        assert jwt is not None, "python-jose must be installed to use JwtAuth"
-        if places:
-            assert places.issubset(
-                {"header", "cookie"}
-            ), "only 'header'/'cookie' are supported"
-        algorithm = algorithm.upper()
-        assert (
-            hasattr(jwt.ALGORITHMS, algorithm) is True  # type: ignore[attr-defined]
-        ), f"{algorithm} algorithm is not supported by python-jose library"
+        assert DEFAULT_JWT_BACKEND is not None, "No JWT backend found, please install 'python-jose' or 'authlib'"
 
+        self.jwt_backend = DEFAULT_JWT_BACKEND(algorithm)
         self.secret_key = secret_key
 
         self.places = places or {"header"}
+        assert self.places.issubset({"header", "cookie"}), "only 'header' and/or 'cookie' places are supported"
         self.auto_error = auto_error
-        self.algorithm = algorithm
         self.access_expires_delta = access_expires_delta or timedelta(minutes=15)
         self.refresh_expires_delta = refresh_expires_delta or timedelta(days=31)
 
+    @property
+    def algorithm(self) -> str:
+        return self.jwt_backend.algorithm
+
     @classmethod
     def from_other(
         cls,
-        other: 'JwtAuthBase',
+        other: "JwtAuthBase",
         secret_key: Optional[str] = None,
         auto_error: Optional[bool] = None,
         algorithm: Optional[str] = None,
         access_expires_delta: Optional[timedelta] = None,
         refresh_expires_delta: Optional[timedelta] = None,
-    ) -> 'JwtAuthBase':
+    ) -> "JwtAuthBase":
         return cls(
             secret_key=secret_key or other.secret_key,
             auto_error=auto_error or other.auto_error,
             algorithm=algorithm or other.algorithm,
             access_expires_delta=access_expires_delta or other.access_expires_delta,
             refresh_expires_delta=refresh_expires_delta or other.refresh_expires_delta,
         )
 
-    def _decode(self, token: str) -> Optional[Dict[str, Any]]:
-        try:
-            payload: Dict[str, Any] = jwt.decode(
-                token,
-                self.secret_key,
-                algorithms=[self.algorithm],
-                options={"leeway": 10},
-            )
-            return payload
-        except jwt.ExpiredSignatureError as e:  # type: ignore[attr-defined]
-            if self.auto_error:
-                raise HTTPException(
-                    status_code=HTTP_401_UNAUTHORIZED, detail=f"Token time expired: {e}"
-                )
-            else:
-                return None
-        except jwt.JWTError as e:  # type: ignore[attr-defined]
-            if self.auto_error:
-                raise HTTPException(
-                    status_code=HTTP_401_UNAUTHORIZED, detail=f"Wrong token: {e}"
-                )
-            else:
-                return None
-
     def _generate_payload(
         self,
         subject: Dict[str, Any],
         expires_delta: timedelta,
         unique_identifier: str,
         token_type: str,
     ) -> Dict[str, Any]:
         now = utcnow()
-
         return {
             "subject": subject.copy(),  # main subject
             "type": token_type,  # 'access' or 'refresh' token
             "exp": now + expires_delta,  # expire time
             "iat": now,  # creation time
             "jti": unique_identifier,  # uuid
         }
@@ -161,111 +141,92 @@
             token = str(bearer.credentials)  # type: ignore
         elif cookie:
             token = str(cookie)
 
         # Check token exist
         if not token:
             if self.auto_error:
-                raise HTTPException(
-                    status_code=HTTP_401_UNAUTHORIZED, detail="Credentials are not provided"
-                )
+                raise HTTPException(status_code=HTTP_401_UNAUTHORIZED, detail="Credentials are not provided")
             else:
                 return None
 
         # Try to decode jwt token. auto_error on error
-        payload = self._decode(token)
-        return payload
+        try:
+            return self.jwt_backend.decode(token, self.secret_key)
+        except BackendException as e:
+            if self.auto_error:
+                raise HTTPException(status_code=HTTP_401_UNAUTHORIZED, detail=str(e))
+            else:
+                return None
 
     def create_access_token(
         self,
         subject: Dict[str, Any],
         expires_delta: Optional[timedelta] = None,
         unique_identifier: Optional[str] = None,
     ) -> str:
         expires_delta = expires_delta or self.access_expires_delta
         unique_identifier = unique_identifier or str(uuid4())
-        to_encode = self._generate_payload(
-            subject, expires_delta, unique_identifier, "access"
-        )
-
-        jwt_encoded: str = jwt.encode(
-            to_encode, self.secret_key, algorithm=self.algorithm
-        )
-        return jwt_encoded
+        to_encode = self._generate_payload(subject, expires_delta, unique_identifier, "access")
+        return self.jwt_backend.encode(to_encode, self.secret_key)
 
     def create_refresh_token(
         self,
         subject: Dict[str, Any],
         expires_delta: Optional[timedelta] = None,
         unique_identifier: Optional[str] = None,
     ) -> str:
         expires_delta = expires_delta or self.refresh_expires_delta
         unique_identifier = unique_identifier or str(uuid4())
-        to_encode = self._generate_payload(
-            subject, expires_delta, unique_identifier, "refresh"
-        )
-
-        jwt_encoded: str = jwt.encode(
-            to_encode, self.secret_key, algorithm=self.algorithm
-        )
-        return jwt_encoded
+        to_encode = self._generate_payload(subject, expires_delta, unique_identifier, "refresh")
+        return self.jwt_backend.encode(to_encode, self.secret_key)
 
     @staticmethod
-    def set_access_cookie(
-        response: Response, access_token: str, expires_delta: Optional[timedelta] = None
-    ) -> None:
-        seconds_expires: Optional[int] = (
-            int(expires_delta.total_seconds()) if expires_delta else None
-        )
+    def set_access_cookie(response: Response, access_token: str, expires_delta: Optional[timedelta] = None) -> None:
+        seconds_expires: Optional[int] = int(expires_delta.total_seconds()) if expires_delta else None
         response.set_cookie(
             key="access_token_cookie",
             value=access_token,
             httponly=False,
             max_age=seconds_expires,
         )
 
     @staticmethod
     def set_refresh_cookie(
         response: Response,
         refresh_token: str,
         expires_delta: Optional[timedelta] = None,
     ) -> None:
-        seconds_expires: Optional[int] = (
-            int(expires_delta.total_seconds()) if expires_delta else None
-        )
+        seconds_expires: Optional[int] = int(expires_delta.total_seconds()) if expires_delta else None
         response.set_cookie(
             key="refresh_token_cookie",
             value=refresh_token,
             httponly=True,
             max_age=seconds_expires,
         )
 
     @staticmethod
     def unset_access_cookie(response: Response) -> None:
-        response.set_cookie(
-            key="access_token_cookie", value="", httponly=False, max_age=-1
-        )
+        response.set_cookie(key="access_token_cookie", value="", httponly=False, max_age=-1)
 
     @staticmethod
     def unset_refresh_cookie(response: Response) -> None:
-        response.set_cookie(
-            key="refresh_token_cookie", value="", httponly=True, max_age=-1
-        )
+        response.set_cookie(key="refresh_token_cookie", value="", httponly=True, max_age=-1)
 
 
 class JwtAccess(JwtAuthBase):
     _bearer = JwtAuthBase.JwtAccessBearer()
     _cookie = JwtAuthBase.JwtAccessCookie()
 
     def __init__(
         self,
         secret_key: str,
         places: Optional[Set[str]] = None,
         auto_error: bool = True,
-        algorithm: str = jwt.ALGORITHMS.HS256,  # type: ignore[attr-defined]
+        algorithm: Optional[str] = None,
         access_expires_delta: Optional[timedelta] = None,
         refresh_expires_delta: Optional[timedelta] = None,
     ):
         super().__init__(
             secret_key,
             places=places,
             auto_error=auto_error,
@@ -278,26 +239,24 @@
         self,
         bearer: Optional[JwtAuthBase.JwtAccessBearer],
         cookie: Optional[JwtAuthBase.JwtAccessCookie],
     ) -> Optional[JwtAuthorizationCredentials]:
         payload = await self._get_payload(bearer, cookie)
 
         if payload:
-            return JwtAuthorizationCredentials(
-                payload["subject"], payload.get("jti", None)
-            )
+            return JwtAuthorizationCredentials(payload["subject"], payload.get("jti", None))
         return None
 
 
 class JwtAccessBearer(JwtAccess):
     def __init__(
         self,
         secret_key: str,
         auto_error: bool = True,
-        algorithm: str = jwt.ALGORITHMS.HS256,  # type: ignore[attr-defined]
+        algorithm: Optional[str] = None,
         access_expires_delta: Optional[timedelta] = None,
         refresh_expires_delta: Optional[timedelta] = None,
     ):
         super().__init__(
             secret_key=secret_key,
             places={"header"},
             auto_error=auto_error,
@@ -313,15 +272,15 @@
 
 
 class JwtAccessCookie(JwtAccess):
     def __init__(
         self,
         secret_key: str,
         auto_error: bool = True,
-        algorithm: str = jwt.ALGORITHMS.HS256,  # type: ignore[attr-defined]
+        algorithm: Optional[str] = None,
         access_expires_delta: Optional[timedelta] = None,
         refresh_expires_delta: Optional[timedelta] = None,
     ):
         super().__init__(
             secret_key=secret_key,
             places={"cookie"},
             auto_error=auto_error,
@@ -338,15 +297,15 @@
 
 
 class JwtAccessBearerCookie(JwtAccess):
     def __init__(
         self,
         secret_key: str,
         auto_error: bool = True,
-        algorithm: str = jwt.ALGORITHMS.HS256,  # type: ignore[attr-defined]
+        algorithm: Optional[str] = None,
         access_expires_delta: Optional[timedelta] = None,
         refresh_expires_delta: Optional[timedelta] = None,
     ):
         super().__init__(
             secret_key=secret_key,
             places={"header", "cookie"},
             auto_error=auto_error,
@@ -368,15 +327,15 @@
     _cookie = JwtAuthBase.JwtRefreshCookie()
 
     def __init__(
         self,
         secret_key: str,
         places: Optional[Set[str]] = None,
         auto_error: bool = True,
-        algorithm: str = jwt.ALGORITHMS.HS256,  # type: ignore[attr-defined]
+        algorithm: Optional[str] = None,
         access_expires_delta: Optional[timedelta] = None,
         refresh_expires_delta: Optional[timedelta] = None,
     ):
         super().__init__(
             secret_key,
             places=places,
             auto_error=auto_error,
@@ -395,30 +354,28 @@
         if payload is None:
             return None
 
         if "type" not in payload or payload["type"] != "refresh":
             if self.auto_error:
                 raise HTTPException(
                     status_code=HTTP_401_UNAUTHORIZED,
-                    detail="Wrong token: 'type' is not 'refresh'",
+                    detail="Invalid token: 'type' is not 'refresh'",
                 )
             else:
                 return None
 
-        return JwtAuthorizationCredentials(
-            payload["subject"], payload.get("jti", None)
-        )
+        return JwtAuthorizationCredentials(payload["subject"], payload.get("jti", None))
 
 
 class JwtRefreshBearer(JwtRefresh):
     def __init__(
         self,
         secret_key: str,
         auto_error: bool = True,
-        algorithm: str = jwt.ALGORITHMS.HS256,  # type: ignore[attr-defined]
+        algorithm: Optional[str] = None,
         access_expires_delta: Optional[timedelta] = None,
         refresh_expires_delta: Optional[timedelta] = None,
     ):
         super().__init__(
             secret_key=secret_key,
             places={"header"},
             auto_error=auto_error,
@@ -434,15 +391,15 @@
 
 
 class JwtRefreshCookie(JwtRefresh):
     def __init__(
         self,
         secret_key: str,
         auto_error: bool = True,
-        algorithm: str = jwt.ALGORITHMS.HS256,  # type: ignore[attr-defined]
+        algorithm: Optional[str] = None,
         access_expires_delta: Optional[timedelta] = None,
         refresh_expires_delta: Optional[timedelta] = None,
     ):
         super().__init__(
             secret_key=secret_key,
             places={"cookie"},
             auto_error=auto_error,
@@ -459,15 +416,15 @@
 
 
 class JwtRefreshBearerCookie(JwtRefresh):
     def __init__(
         self,
         secret_key: str,
         auto_error: bool = True,
-        algorithm: str = jwt.ALGORITHMS.HS256,  # type: ignore[attr-defined]
+        algorithm: Optional[str] = None,
         access_expires_delta: Optional[timedelta] = None,
         refresh_expires_delta: Optional[timedelta] = None,
     ):
         super().__init__(
             secret_key=secret_key,
             places={"header", "cookie"},
             auto_error=auto_error,
```

## Comparing `fastapi_jwt-0.2.0.dist-info/LICENSE` & `fastapi_jwt-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fastapi_jwt-0.2.0.dist-info/METADATA` & `fastapi_jwt-0.3.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-jwt
-Version: 0.2.0
+Version: 0.3.0
 Summary: `FastAPI` extension for JTW Auth
 Author-email: Konstantin Chernyshev <kdchernyshev@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/k4black/fastapi-jwt
 Project-URL: documentation, https://k4black.github.io/fastapi-jwt/
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -14,32 +14,37 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fastapi >=0.50.0
-Requires-Dist: python-jose[cryptography] >=3.3.0
+Provides-Extra: authlib
+Requires-Dist: Authlib >=1.3.0 ; extra == 'authlib'
 Provides-Extra: docs
 Requires-Dist: mkdocs <2.0.0,>=1.4.0 ; extra == 'docs'
 Requires-Dist: mkdocs-material <10.0.0,>=9.0.0 ; extra == 'docs'
 Requires-Dist: MkAutoDoc <1.0.0,>=0.2.0 ; extra == 'docs'
 Requires-Dist: lazydocs <1.0.0,>=0.4.5 ; extra == 'docs'
 Requires-Dist: mkdocs-include-markdown-plugin <7.0.0,>=4.0.0 ; extra == 'docs'
 Requires-Dist: mkdocs-awesome-pages-plugin <3.0.0,>=2.8.0 ; extra == 'docs'
-Requires-Dist: mike <2.0.0,>=1.1.0 ; extra == 'docs'
+Requires-Dist: mike <3.0.0,>=1.1.0 ; extra == 'docs'
+Provides-Extra: python_jose
+Requires-Dist: python-jose[cryptography] >=3.3.0 ; extra == 'python_jose'
 Provides-Extra: test
+Requires-Dist: Authlib >=1.3.0 ; extra == 'test'
+Requires-Dist: python-jose[cryptography] >=3.3.0 ; extra == 'test'
 Requires-Dist: httpx <1.0.0,>=0.23.0 ; extra == 'test'
-Requires-Dist: pytest <8.0.0,>=7.0.0 ; extra == 'test'
-Requires-Dist: pytest-cov <5.0.0,>=4.0.0 ; extra == 'test'
+Requires-Dist: pytest <9.0.0,>=7.0.0 ; extra == 'test'
+Requires-Dist: pytest-cov <6.0.0,>=4.0.0 ; extra == 'test'
 Requires-Dist: pytest-mock <4.0.0,>=3.0.0 ; extra == 'test'
 Requires-Dist: requests <3.0.0,>=2.28.0 ; extra == 'test'
-Requires-Dist: black ==23.10.1 ; extra == 'test'
+Requires-Dist: black ==24.4.2 ; extra == 'test'
 Requires-Dist: mypy <2.0.0,>=1.0.0 ; extra == 'test'
-Requires-Dist: flake8 <7.0.0,>=6.0.0 ; extra == 'test'
+Requires-Dist: flake8 <8.0.0,>=6.0.0 ; extra == 'test'
 Requires-Dist: ruff <1.0.0,>=0.1.0 ; extra == 'test'
 Requires-Dist: isort <6.0.0,>=5.11.0 ; extra == 'test'
 Requires-Dist: types-python-jose ==3.3.4.8 ; extra == 'test'
 
 # fastapi-jwt
 
 [![Test](https://github.com/k4black/fastapi-jwt/actions/workflows/test.yml/badge.svg)](https://github.com/k4black/fastapi-jwt/actions/workflows/test.yml)
@@ -63,17 +68,22 @@
 * JTI
 * Cookie setting
 
 
 ## Installation
 You can access package [fastapi-jwt in pypi](https://pypi.org/project/fastapi-jwt/)
 ```shell
-pip install fastapi-jwt
+pip install fastapi-jwt[authlib]
+# or
+pip install fastapi-jwt[python_jose]
 ```
 
+The fastapi-jwt will choose the backend automatically if library is installed with the following priority:
+1. authlib
+2. python_jose (deprecated)
 
 ## Usage
 This library made in fastapi style, so it can be used as standard security features 
 
 ```python
 from fastapi import FastAPI, Security, Response
 from fastapi_jwt import JwtAuthorizationCredentials, JwtAccessBearer
@@ -119,11 +129,11 @@
 ## FastAPI Integration 
 
 There it is open and maintained [Pull Request #3305](https://github.com/tiangolo/fastapi/pull/3305) to the `fastapi` repo. Currently, not considered.
 
 ## Requirements 
 
 * `fastapi`
-* `python-jose[cryptography]`
+* `authlib` or `python-jose[cryptography]` (deprecated)
 
 ## License
 This project is licensed under the terms of the MIT license.
```

