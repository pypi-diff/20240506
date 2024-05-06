# Comparing `tmp/drakaina-0.7.0b7.tar.gz` & `tmp/drakaina-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drakaina-0.7.0b7.tar", max compression
+gzip compressed data, was "drakaina-0.7.1.tar", max compression
```

## Comparing `drakaina-0.7.0b7.tar` & `drakaina-0.7.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     9020 2023-06-06 11:46:13.593707 drakaina-0.7.0b7/drakaina/__init__.py
--rw-r--r--   0        0        0        0 2023-01-24 15:15:01.981448 drakaina-0.7.0b7/drakaina/contrib/__init__.py
--rw-r--r--   0        0        0     1225 2023-04-04 16:39:30.455695 drakaina-0.7.0b7/drakaina/contrib/django/__init__.py
--rw-r--r--   0        0        0     6410 2023-06-06 11:38:21.333031 drakaina-0.7.0b7/drakaina/contrib/django/middleware.py
--rw-r--r--   0        0        0     3532 2023-04-20 14:07:49.356702 drakaina-0.7.0b7/drakaina/contrib/django/views.py
--rw-r--r--   0        0        0      402 2023-04-07 16:25:48.140700 drakaina-0.7.0b7/drakaina/contrib/jwt/__init__.py
--rw-r--r--   0        0        0      348 2023-03-10 11:02:10.213372 drakaina-0.7.0b7/drakaina/contrib/jwt/errors.py
--rw-r--r--   0        0        0     8847 2023-06-06 11:46:13.593707 drakaina-0.7.0b7/drakaina/contrib/jwt/middleware.py
--rw-r--r--   0        0        0      911 2023-05-29 22:21:28.708378 drakaina-0.7.0b7/drakaina/contrib/jwt/types.py
--rw-r--r--   0        0        0    18201 2023-06-06 11:46:13.594707 drakaina-0.7.0b7/drakaina/contrib/jwt/utils.py
--rw-r--r--   0        0        0     1490 2023-06-02 16:00:38.817771 drakaina-0.7.0b7/drakaina/exceptions.py
--rw-r--r--   0        0        0      357 2023-04-04 11:19:41.564726 drakaina-0.7.0b7/drakaina/middleware/__init__.py
--rw-r--r--   0        0        0     1370 2023-05-29 22:21:28.722375 drakaina-0.7.0b7/drakaina/middleware/base.py
--rw-r--r--   0        0        0     7364 2023-06-06 11:46:13.594707 drakaina-0.7.0b7/drakaina/middleware/cors.py
--rw-r--r--   0        0        0     1967 2023-06-06 11:46:13.594707 drakaina-0.7.0b7/drakaina/middleware/exception.py
--rw-r--r--   0        0        0     1072 2023-05-29 22:42:27.401282 drakaina-0.7.0b7/drakaina/middleware/request_wrapper.py
--rw-r--r--   0        0        0    12337 2023-06-06 11:46:13.595708 drakaina-0.7.0b7/drakaina/registries.py
--rw-r--r--   0        0        0      155 2023-03-02 17:41:49.563857 drakaina-0.7.0b7/drakaina/rpc_protocols/__init__.py
--rw-r--r--   0        0        0     7317 2023-06-06 11:46:13.595708 drakaina-0.7.0b7/drakaina/rpc_protocols/base.py
--rw-r--r--   0        0        0    13954 2023-06-06 11:46:13.595708 drakaina-0.7.0b7/drakaina/rpc_protocols/jsonrpc20.py
--rw-r--r--   0        0        0     4643 2023-05-12 10:10:59.326403 drakaina-0.7.0b7/drakaina/serializers.py
--rw-r--r--   0        0        0    30828 2023-06-06 11:46:13.596708 drakaina-0.7.0b7/drakaina/types.py
--rw-r--r--   0        0        0     3627 2023-06-06 11:46:13.596708 drakaina-0.7.0b7/drakaina/utils.py
--rw-r--r--   0        0        0     8212 2023-06-06 11:46:13.597709 drakaina-0.7.0b7/drakaina/wsgi.py
--rw-r--r--   0        0        0    11372 2023-01-24 23:31:45.206801 drakaina-0.7.0b7/LICENSE
--rw-r--r--   0        0        0     2710 2023-06-06 11:39:11.129309 drakaina-0.7.0b7/pyproject.toml
--rw-r--r--   0        0        0     5366 2023-06-06 11:46:13.593707 drakaina-0.7.0b7/README.md
--rw-r--r--   0        0        0     6888 1970-01-01 00:00:00.000000 drakaina-0.7.0b7/PKG-INFO
+-rw-r--r--   0        0        0     9452 2024-05-06 18:37:59.533917 drakaina-0.7.1/drakaina/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-24 15:15:01.981448 drakaina-0.7.1/drakaina/contrib/__init__.py
+-rw-r--r--   0        0        0     1225 2023-04-04 16:39:30.455695 drakaina-0.7.1/drakaina/contrib/django/__init__.py
+-rw-r--r--   0        0        0     6410 2023-06-06 11:38:21.333031 drakaina-0.7.1/drakaina/contrib/django/middleware.py
+-rw-r--r--   0        0        0     3532 2023-04-20 14:07:49.356702 drakaina-0.7.1/drakaina/contrib/django/views.py
+-rw-r--r--   0        0        0      402 2023-04-07 16:25:48.140700 drakaina-0.7.1/drakaina/contrib/jwt/__init__.py
+-rw-r--r--   0        0        0      351 2024-05-06 19:02:29.664147 drakaina-0.7.1/drakaina/contrib/jwt/errors.py
+-rw-r--r--   0        0        0     8986 2024-05-06 18:57:08.110107 drakaina-0.7.1/drakaina/contrib/jwt/middleware.py
+-rw-r--r--   0        0        0      911 2023-05-29 22:21:28.708378 drakaina-0.7.1/drakaina/contrib/jwt/types.py
+-rw-r--r--   0        0        0    18281 2024-05-06 18:37:59.534916 drakaina-0.7.1/drakaina/contrib/jwt/utils.py
+-rw-r--r--   0        0        0     1490 2023-06-02 16:00:38.817771 drakaina-0.7.1/drakaina/exceptions.py
+-rw-r--r--   0        0        0      357 2023-04-04 11:19:41.564726 drakaina-0.7.1/drakaina/middleware/__init__.py
+-rw-r--r--   0        0        0     1370 2023-05-29 22:21:28.722375 drakaina-0.7.1/drakaina/middleware/base.py
+-rw-r--r--   0        0        0     7749 2024-05-06 18:37:59.534916 drakaina-0.7.1/drakaina/middleware/cors.py
+-rw-r--r--   0        0        0     1991 2024-05-06 18:37:59.534916 drakaina-0.7.1/drakaina/middleware/exception.py
+-rw-r--r--   0        0        0     1072 2023-05-29 22:42:27.401282 drakaina-0.7.1/drakaina/middleware/request_wrapper.py
+-rw-r--r--   0        0        0    12943 2024-05-06 18:37:59.534916 drakaina-0.7.1/drakaina/registries.py
+-rw-r--r--   0        0        0      155 2023-03-02 17:41:49.563857 drakaina-0.7.1/drakaina/rpc_protocols/__init__.py
+-rw-r--r--   0        0        0     8028 2024-05-06 18:37:59.534916 drakaina-0.7.1/drakaina/rpc_protocols/base.py
+-rw-r--r--   0        0        0    14864 2024-05-06 18:37:59.535920 drakaina-0.7.1/drakaina/rpc_protocols/jsonrpc20.py
+-rw-r--r--   0        0        0     4643 2023-05-12 10:10:59.326403 drakaina-0.7.1/drakaina/serializers.py
+-rw-r--r--   0        0        0    34083 2024-05-06 18:37:59.535920 drakaina-0.7.1/drakaina/types.py
+-rw-r--r--   0        0        0     6193 2024-05-06 18:37:59.535920 drakaina-0.7.1/drakaina/utils.py
+-rw-r--r--   0        0        0     8288 2024-05-06 18:37:59.535920 drakaina-0.7.1/drakaina/wsgi.py
+-rw-r--r--   0        0        0    11372 2023-01-24 23:31:45.206801 drakaina-0.7.1/LICENSE
+-rw-r--r--   0        0        0     2703 2024-05-06 19:02:47.259023 drakaina-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     6992 2024-05-06 18:37:59.533917 drakaina-0.7.1/README.md
+-rw-r--r--   0        0        0     8512 1970-01-01 00:00:00.000000 drakaina-0.7.1/PKG-INFO
```

### Comparing `drakaina-0.7.0b7/drakaina/__init__.py` & `drakaina-0.7.1/drakaina/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -141,14 +141,19 @@
             _provide_request=provide_request,
             _metadata={**(metadata or {}), **meta_options},
         )
 
     return decorator
 
 
+# TODO: may be implement `login_required` decorators for
+#  Registries/RPC Handlers/apps for many instances.
+#  But, first need implement nested registers, protocols and applications
+
+
 def login_required(*_args) -> Callable:
     """Requires login decorator.
 
     Gives access to the procedure only to authenticated users.
 
     """
 
@@ -161,26 +166,22 @@
                 "the `drakaina.remote_procedure` decorator first.",
             )
 
         if iscoroutinefunction(procedure):
 
             async def wrapper(*args, **kwargs):
                 request = _get_request(*args, **kwargs)
-                if not _is_authenticated(request):
-                    raise ForbiddenError("Authentication required")
-
+                validate_authentication(request)
                 return await procedure(*args, **kwargs)
 
         else:
 
             def wrapper(*args, **kwargs):
                 request = _get_request(*args, **kwargs)
-                if not _is_authenticated(request):
-                    raise ForbiddenError("Authentication required")
-
+                validate_authentication(request)
                 return procedure(*args, **kwargs)
 
         wrapper = update_wrapper(wrapper, procedure)
         registry.replace(procedure, wrapper)
         return wrapper
 
     if len(_args) > 0:
@@ -239,38 +240,31 @@
         if registry is None:
             raise TypeError(
                 "Incorrect usage of decorator. Please use "
                 "the `drakaina.remote_procedure` decorator first.",
             )
 
         if iscoroutinefunction(procedure):
+            # TODO: reference for async code `starlette.authentication.requires`
 
             async def wrapper(*args, **kwargs):
                 request = _get_request(*args, **kwargs)  # noqa
 
-                if not _is_authenticated(request):
-                    raise ForbiddenError("Authentication required")
-
-                user_scopes = _get_scopes(request)
-                if not comparator(procedure_scopes, user_scopes):
-                    raise ForbiddenError("Forbidden")
+                validate_authentication(request)
+                validate_permissions(request, procedure_scopes, comparator)
 
                 return await procedure(*args, **kwargs)
 
         else:
 
             def wrapper(*args, **kwargs):
                 request = _get_request(*args, **kwargs)  # noqa
 
-                if not _is_authenticated(request):
-                    raise ForbiddenError("Authentication required")
-
-                user_scopes = _get_scopes(request)
-                if not comparator(procedure_scopes, user_scopes):
-                    raise ForbiddenError("Forbidden")
+                validate_authentication(request)
+                validate_permissions(request, procedure_scopes, comparator)
 
                 return procedure(*args, **kwargs)
 
         wrapper = update_wrapper(wrapper, procedure)
         registry.replace(procedure, wrapper)
         return wrapper
 
@@ -287,15 +281,42 @@
 def _is_authenticated(request: AnyRequest) -> bool:
     if isinstance(request, (dict, Mapping)):
         return request.get(ENV_IS_AUTHENTICATED, False)
     else:
         return getattr(request, ENV_IS_AUTHENTICATED, False)
 
 
+def validate_authentication(request: AnyRequest):
+    """Validate authentication.
+
+    :param request:
+    :raise ForbiddenError:
+    """
+    if not _is_authenticated(request):
+        raise ForbiddenError("Authentication required")
+
+
 def _get_scopes(request: AnyRequest) -> Iterable[str]:
     if isinstance(request, (dict, Mapping)) or hasattr(request, "get"):
         scopes = request.get(ENV_AUTH_SCOPES, None)
     else:
         scopes = getattr(request, ENV_AUTH_SCOPES, None)
     if isinstance(scopes, (str, Iterable)):
         return iterable_str_arg(scopes)
     return ()
+
+
+def validate_permissions(
+    request: AnyRequest,
+    procedure_scopes: Iterable[str],
+    comparator: Comparator = match_any,
+):
+    """Validate permissions.
+
+    :param request:
+    :param procedure_scopes:
+    :param comparator:
+    :raise ForbiddenError:
+    """
+    user_scopes = _get_scopes(request)
+    if not comparator(procedure_scopes, user_scopes):
+        raise ForbiddenError("Forbidden")
```

### Comparing `drakaina-0.7.0b7/drakaina/contrib/django/__init__.py` & `drakaina-0.7.1/drakaina/contrib/django/__init__.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b7/drakaina/contrib/django/middleware.py` & `drakaina-0.7.1/drakaina/contrib/django/middleware.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b7/drakaina/contrib/django/views.py` & `drakaina-0.7.1/drakaina/contrib/django/views.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b7/drakaina/contrib/jwt/middleware.py` & `drakaina-0.7.1/drakaina/contrib/jwt/middleware.py`

 * *Files 13% similar despite different names*

```diff
@@ -29,64 +29,48 @@
 from drakaina.utils import iterable_str_arg
 
 
 class JWTAuthenticationMiddleware(BaseMiddleware):
     """The middleware supporting JWT tokens.
 
     :param app: WSGI Application.
-    :type app: WSGIApplication
     :param algorithms: List of supported algorithms.
-    :type algorithms: Iterable[str]
     :param secret_key: A secret key for signature verification.
-    :type secret_key: str
     :param public_key: Public key for signature verification in
         asymmetric algorithms.
-    :type public_key: str
     :param credentials_required: If `True`, the request is expected to
         contain credential data. If they are missing, an exception is raised.
         Default: `True`.
-    :type credentials_required: bool
     :param prefix: The token prefix in the authorization headers.
         Default: `"Bearer"`.
-    :type prefix: str
     :param use_cookies: If true, the token will be searched in the cookie
         headers for the specified key. Default: `False`.
-    :type use_cookies: bool
     :param cookie_key: The key by which the token is stored in the cookie
         headers.
-    :type cookie_key: str
     :param decode_options: The dictionary is passed as is as the `options`
         argument to the `pyjwt.decode` function. Default: `{
             "require": [],  # Require claims
             "verify_iss": False,  # Issuer
             "verify_aud": False,  # Audience
             "verify_exp": True,   # Expiry
             "verify_nbf": False,  # Not Before
             "verify_iat": True,   # Issued at
             "verify_jti": False,  # JWT ID
         }`
-    :type decode_options: dict[str, bool | Iterable[str]] | None
     :param verify_values: A dictionary of key-value pairs, where key is
         the name of the key in the token payload, and the value to check can be
         a specific value, a list of possible values, or a re.Pattern object
         (the result of re.compile).
-    :type verify_values: dict[str, str | Iterable[str] | re.Pattern] | None
     :param leeway_value: The value of leeway in seconds. Default: `0`.
-    :type leeway_value: int | float
     :param user_id_field: The name of the key in the token payload to store
         the user ID. Default: `"user_id"`.
-    :type user_id_field: str
     :param token_getter: Callable for an alternative way to get a token.
-    :type token_getter: TokenGetter | None
     :param user_getter: Callable to retrieve a user object.
-    :type user_getter: UserGetter | None
     :param scopes_getter: Callable to get permission scopes.
-    :type scopes_getter: ScopesGetter | None
     :param revoke_checker: Callable to verify that the token is revoked.
-    :type revoke_checker: RevokeChecker | None
     :param kwargs: Other arguments to pass to the constructor of the base class.
 
     """
 
     __slots__ = (
         "_algorithms",
         "__verify_key",
@@ -169,30 +153,46 @@
 
         token = self.get_token(environ)
 
         if not token and self._credentials_required:
             raise AuthenticationFailedError("Credential required")
 
         if token is not None:
-            token_payload = decode_jwt_token(
-                token=token,
-                algorithms=self._algorithms,
-                verify_key=self.__verify_key,
-                verify=True,
-                decode_options=self._decode_options,
-                verify_values=self._verify_values,
-                leeway=self._leeway,
-            )
+            try:
+                token_payload = decode_jwt_token(
+                    token=token,
+                    algorithms=self._algorithms,
+                    verify_key=self.__verify_key,
+                    verify=True,
+                    decode_options=self._decode_options,
+                    verify_values=self._verify_values,
+                    leeway=self._leeway,
+                )
+                token_is_valid = True
+            except InvalidJWTTokenError as error:
+                if self._credentials_required:
+                    raise error
+                else:
+                    token_payload = decode_jwt_token(
+                        token=token,
+                        algorithms=self._algorithms,
+                        verify_key=self.__verify_key,
+                        verify=False,
+                        decode_options=self._decode_options,
+                        verify_values=self._verify_values,
+                        leeway=self._leeway,
+                    )
+                    token_is_valid = environ.get(ENV_IS_AUTHENTICATED, False)
 
             if callable(self.is_revoked):
                 if self.is_revoked(environ, token_payload):
                     raise ForbiddenError("Token is revoked")
 
             environ[ENV_USER_ID] = token_payload.get(self._user_id_field)
-            environ[ENV_IS_AUTHENTICATED] = True
+            environ[ENV_IS_AUTHENTICATED] = token_is_valid
             environ[ENV_AUTH_PAYLOAD] = token_payload
 
             if callable(self.get_user):
                 environ[ENV_USER] = self.get_user(environ, token_payload)
             if callable(self.get_scopes):
                 environ[ENV_AUTH_SCOPES] = self.get_scopes(
                     environ,
```

### Comparing `drakaina-0.7.0b7/drakaina/contrib/jwt/types.py` & `drakaina-0.7.1/drakaina/contrib/jwt/types.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b7/drakaina/contrib/jwt/utils.py` & `drakaina-0.7.1/drakaina/contrib/jwt/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -336,15 +336,15 @@
             jwt=token,
             key=verify_key,
             algorithms=algorithms,
             options=options,
             **params,
         )
     except InvalidAlgorithmError as error:
-        raise JWTBackendError("Invalid algorithm specified") from error
+        raise InvalidJWTTokenError("Invalid algorithm specified") from error
     except InvalidTokenError:
         raise InvalidJWTTokenError("Token is invalid or expired")
 
     if verify:
         _extra_validation(token_data, verify_values)
 
     return token_data["payload"]
@@ -433,14 +433,15 @@
         set_permission_scopes(payload, permission_scopes)
 
     return encode(
         payload=payload,
         key=signing_key,
         algorithm=algorithm,
         headers=headers,
+        json_encoder=None,  # todo: rewrite for use custom JSON serializer
     )
 
 
 # Helpful functions
 
 
 def copy_payload(
```

### Comparing `drakaina-0.7.0b7/drakaina/exceptions.py` & `drakaina-0.7.1/drakaina/exceptions.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b7/drakaina/middleware/base.py` & `drakaina-0.7.1/drakaina/middleware/base.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b7/drakaina/middleware/cors.py` & `drakaina-0.7.1/drakaina/middleware/cors.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,14 +145,23 @@
         scope: ASGIScope,
         receive: ASGIReceive,
         send: ASGISend,
     ):
         if scope["type"] != "http":
             await self.app(scope, receive, send)
         ...
+        # if scope.get("HTTP_ORIGIN"):
+        #     if scope.get("REQUEST_METHOD") == "OPTIONS":
+        #         return self.options(environ, start_response)
+        #     return await self.app(
+        #         environ,
+        #         self._add_cors_headers(environ, start_response),
+        #     )
+        # else:
+        #     return await self.app(environ, start_response)
 
     def options(
         self,
         environ: WSGIEnvironment,
         start_response: WSGIStartResponse,
     ) -> WSGIResponse:
         """Response for OPTIONS request"""
```

### Comparing `drakaina-0.7.0b7/drakaina/middleware/exception.py` & `drakaina-0.7.1/drakaina/middleware/exception.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,7 +59,8 @@
         send: ASGISend,
     ):
         try:
             await self.app(scope, receive, send)
         except Exception as error:
             if self._logger is not None:
                 self._logger.exception(error)
+            ...  # todo
```

### Comparing `drakaina-0.7.0b7/drakaina/middleware/request_wrapper.py` & `drakaina-0.7.1/drakaina/middleware/request_wrapper.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b7/drakaina/registries.py` & `drakaina-0.7.1/drakaina/registries.py`

 * *Files 3% similar despite different names*

```diff
@@ -114,14 +114,16 @@
             the procedure as a `request` argument.
         :param metadata:
             Metadata that can be processed by middleware or an extension.
         """
         assert callable(extension_procedure)
         assert extension_name and extension_name.startswith("rpc.")
 
+        # TODO: need inspect schema ?
+
         self.__register_callable(
             func=extension_procedure,
             name=extension_name,
             provide_request=provide_request,
             metadata=metadata,
         )
 
@@ -202,14 +204,19 @@
 
             # Get values from docstring
             if docstring and parameter.name in docstring.params_dict:
                 param_doc = docstring.params_dict[parameter.name]
                 param_schema.setdefault("type", param_doc.type_name)
                 param_schema.setdefault("description", param_doc.description)
 
+            # param_schema.setdefault(
+            #     "description",
+            #     short_description_by_name(parameter.name),
+            # )
+
             # Add in method schema
             schema["parameters"].setdefault(parameter.name, param_schema)
 
         # Get return info from signature
         if proc_signature.return_annotation is not Signature.empty:
             # Set return type
             if isinstance(proc_signature.return_annotation, type):
@@ -234,17 +241,25 @@
                 schema["errors"] = []
                 for exc in raises:
                     exc_schema = {"type": exc.type_name}
                     if exc.description:
                         exc_schema["description"] = exc.description
                     schema["errors"].append(exc_schema)
             # Deprecation info
-            if docstring.deprecation:
+            if docstring.deprecation:  # TODO
+                # {
+                #     "version": docstring.deprecation.version,
+                #     "description": docstring.deprecation.description,
+                # }
                 ...
-            if docstring.examples:
+            if docstring.examples:  # TODO
+                # {
+                #     "snippet": docstring.deprecation.snippet,
+                #     "description": docstring.deprecation.description,
+                # }
                 ...
 
         return schema
 
     def __register_callable(
         self,
         func: Callable[..., Any],
@@ -297,14 +312,15 @@
         :param procedure:
         :param new_procedure:
 
         """
         procedure_name = getattr(procedure, RPC_NAME, None)
         if procedure_name is None:
             raise TypeError(f"Callable {procedure} is not an rpc procedure.")
+        # TODO: need duplicate __rpc attributes?
         self._remote_procedures[procedure_name] = new_procedure
 
     def __getitem__(self, key: str) -> Callable[..., Any] | None:
         # Intentionally suppress the rise of the exception,
         # and simply return None if there is no specified procedure.
         return self._remote_procedures.get(key)
```

### Comparing `drakaina-0.7.0b7/drakaina/rpc_protocols/base.py` & `drakaina-0.7.1/drakaina/rpc_protocols/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+from logging import getLogger
 from typing import Any
 from typing import ClassVar
 from typing import Type
 
 from drakaina import rpc_registry
 from drakaina.exceptions import InternalServerError
 from drakaina.exceptions import RPCError
@@ -13,14 +14,16 @@
 from drakaina.serializers import JsonSerializer
 from drakaina.types import OpenAPI
 from drakaina.types import OpenRPC
 from drakaina.utils import unwrap_func
 
 __all__ = ("BaseRPCProtocol",)
 
+log = getLogger()
+
 
 class BaseRPCProtocol:
     """Base class for representing the remote procedure call (RPC) protocol.
 
     To implement your own RPC protocol, you must implement the `handle` method,
     which must accept two parameters - the incoming message of your protocol
     `rpc_request` and an environment object 'request' that contains information
@@ -147,14 +150,15 @@
             The instance or class of the error.
         :type error: RPCError | Type[RPCError] | Exception | Type[Exception]
         :returns: Protocol specific error object.
         :rtype: RPCError
 
         """
 
+        print("handle_error", type(error), f"{error=}")
         if isinstance(error, type) and issubclass(error, Exception):
             error = error()
 
         if isinstance(error, self.base_error_class):
             return error
         else:
             # Try to get mapped error class
@@ -202,19 +206,39 @@
 
         https://spec.open-rpc.org/
 
         """
         raise NotImplementedError()
 
     def get_raw_openrpc_schema(self) -> bytes:
-        return self.schema_serializer.serialize(self.openrpc_schema())
+        # return self.schema_serializer.serialize(self.openrpc_schema())
+        try:
+            return self.schema_serializer.serialize(self.openrpc_schema())
+        except Exception as err:
+            import traceback
+
+            print("get_raw_openrpc_schema", str(err))
+            print(traceback.format_exc())
+
+            log.exception(err)
+            raise err
 
     def openapi_schema(self) -> OpenAPI:
         """Implementation of OpenAPI specification.
 
         https://spec.openapis.org/oas/latest.html
 
         """
         raise NotImplementedError()
 
     def get_raw_openapi_schema(self) -> bytes:
-        return self.schema_serializer.serialize(self.openapi_schema())
+        # return self.schema_serializer.serialize(self.openapi_schema())
+        try:
+            return self.schema_serializer.serialize(self.openapi_schema())
+        except Exception as err:
+            import traceback
+
+            print("get_raw_openrpc_schema", str(err))
+            print(traceback.format_exc())
+
+            log.exception(err)
+            raise err
```

### Comparing `drakaina-0.7.0b7/drakaina/rpc_protocols/jsonrpc20.py` & `drakaina-0.7.1/drakaina/rpc_protocols/jsonrpc20.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from __future__ import annotations
 
 from copy import deepcopy
 from functools import partial
+from inspect import getmembers
+from logging import getLogger
 from typing import Any
 from typing import ClassVar
 
 from drakaina.exceptions import AuthenticationFailedError
 from drakaina.exceptions import BadRequestError
 from drakaina.exceptions import DeserializationError
 from drakaina.exceptions import ForbiddenError
 from drakaina.exceptions import InternalServerError
 from drakaina.exceptions import InvalidParametersError
 from drakaina.exceptions import InvalidPermissionsError
 from drakaina.exceptions import InvalidTokenError
 from drakaina.exceptions import NotFoundError
 from drakaina.exceptions import RPCError
 from drakaina.exceptions import SerializationError
+from drakaina.registries import RPC_META
 from drakaina.registries import RPC_SCHEMA
 from drakaina.registries import RPCRegistry
 from drakaina.rpc_protocols.base import BaseRPCProtocol
 from drakaina.serializers import BaseSerializer
 from drakaina.serializers import JsonSerializer
 from drakaina.types import JSONRPCRequest
 from drakaina.types import JSONRPCRequestObject
@@ -28,14 +31,16 @@
 from drakaina.types import MethodSchema
 from drakaina.types import OAPI
 from drakaina.types import ORPC
 from drakaina.utils import unwrap_func
 
 __all__ = ("JsonRPCv2",)
 
+log = getLogger()
+
 DEFAULT_OPENRPC_SCHEMA = ORPC.OpenRPC(
     openrpc=ORPC.SUPPORTED_VERSION,
     info=ORPC.Info(version="1.0.0", title="JSON-RPC 2.0 service"),
     servers=[ORPC.Server(name="main", url="/")],
     methods=[],
 )
 """This is the default OpenRPC schema.
@@ -404,16 +409,25 @@
             openrpc: ORPC.OpenRPC = deepcopy(self.openrpc_schema_template)
             if not isinstance(openrpc.get("methods"), list):
                 openrpc["methods"] = []
 
             for method_name, procedure_ in self.registry.items():
                 procedure = unwrap_func(procedure_)
                 try:
+                    # TODO
+                    method_metadata: dict = getattr(procedure, RPC_META)
                     method_schema: MethodSchema = getattr(procedure, RPC_SCHEMA)
                 except AttributeError:
+                    # TODO handle error
+                    err = (
+                        f"AttributeError;\n{getmembers(procedure_)=};"
+                        f"\n{getmembers(procedure)=};",
+                    )
+                    print(f"openrpc_schema; {err}")
+                    log.error(err)
                     continue
 
                 openrpc["methods"].append(
                     ORPC.method_by_schema(
                         method_schema,
                         default_name=method_name,
                     ),
@@ -430,16 +444,24 @@
         """
         if not self.__openapi_schema:
             openapi: OAPI.OpenAPI = deepcopy(self.openapi_schema_template)
 
             for method_name, procedure_ in self.registry.items():
                 procedure = unwrap_func(procedure_)
                 try:
+                    # TODO
+                    method_metadata: dict = getattr(procedure, RPC_META)
                     method_schema: MethodSchema = getattr(procedure, RPC_SCHEMA)
                 except AttributeError:
+                    err = (  # TODO handle error
+                        f"AttributeError;\n{getmembers(procedure_)=};"
+                        f"\n{getmembers(procedure)=};",
+                    )
+                    print(f"openrpc_schema; {err}")
+                    log.error(err)
                     continue
 
                 path_name = self.schema_url + "#" + method_name
                 operation = OAPI.operation_by_schema(
                     method_schema,
                     default_name=method_name,
                 )
```

### Comparing `drakaina-0.7.0b7/drakaina/serializers.py` & `drakaina-0.7.1/drakaina/serializers.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b7/drakaina/types.py` & `drakaina-0.7.1/drakaina/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,19 @@
 
     class ReprEnum(Enum):
         """
         Only changes the repr(), leaving str() and format()
         to the mixed-in type.
         """
 
+    class IntEnum(int, ReprEnum):
+        """
+        Enum where members are also (and must be) ints
+        """
+
     class StrEnum(str, ReprEnum):
         """
         Enum where members are also (and must be) strings
         """
 
         def __new__(cls, *values):
             "values must already be of type `str`"
@@ -68,14 +73,15 @@
         def _generate_next_value_(name, start, count, last_values):
             """
             Return the lower-cased version of the member name.
             """
             return name.lower()
 
 else:
+    from enum import IntEnum
     from enum import StrEnum
     from typing import NotRequired
 
 
 """
 JSON-RPC types definitions
 """
@@ -808,14 +814,15 @@
     @staticmethod
     def parameters_by_schema(method_schema: MethodSchema) -> list[OASParameter]:
         result = []
         parameters = method_schema.get("parameters", {})
         for param_name, parameter in parameters.items():
             param = OAPI.Parameter(
                 name=parameter.get("name", param_name),
+                # in=OAPI.ParameterLocation.?,
                 schema=OAPI.Schema(),
                 required=parameter.get("required", False),
                 deprecated=parameter.get("deprecated", False),
             )
             if "type" in parameter:
                 param["schema"]["type"] = OAPI.type_mapping(
                     parameter["type"],
@@ -846,37 +853,52 @@
                         "type": "string",
                         "description": "Procedure (method) name",
                     },
                     "params": {
                         "type": "object",
                         "properties": {
                             param_name: {
+                                # "type": OAPI.type_mapping(
+                                #     parameter.get("type"),
+                                # ),
                                 "default": parameter.get("default", ""),
+                                # "required": parameter.get(
+                                #     "required",
+                                #     False,
+                                # ),
                                 "description": parameter.get(
                                     "description",
                                     "",
                                 ),
                                 "deprecated": parameter.get(
                                     "deprecated",
                                     False,
                                 ),
                             }
                             for param_name, parameter in parameters
                         },
                     },
                     "id": {
+                        # "type": ["string", "integer"],  # TODO
                         "type": "string",
                     },
                 },
                 required=["jsonrpc", "method"],
+                # x={
+                #     "jsonrpc": "2.0",
+                #     "method": method_name,
+                #     "params": {},
+                #     "id": 1,
+                # },  # TODO <-
             ),
         )
         if "example" in method_schema:
             media["example"] = method_schema["example"]
         if "examples" in method_schema:
+            # TODO: {str: OAPI.Example)
             media["examples"] = method_schema["examples"]
         return OASRequestBody(
             content={"application/json": media},
             description="JSON-RPC 2.0 Request Object",
             required=True,
         )
 
@@ -895,30 +917,40 @@
                 )
 
             media = OASMediaType(
                 schema=OASSchema(type="object", properties=jsonrpc_object),
             )
             if "description" in result_schema:
                 media["schema"]["description"] = result_schema["description"]
+            # if "example" in result_schema:
+            #     media["example"] = result_schema["example"]
+            # if "examples" in result_schema:
+            #     # TODO: {str: OAPI.Example)
+            #     media["examples"] = result_schema["examples"]
         else:
+            # If returns type is NoneType
+            # TODO: Move to components
             media = OASMediaType(
                 schema=OAPI.Schema(
                     type="object",
                     properties=dict(
                         jsonrpc=dict(type="string", default="2.0"),
                         result=dict(type="null"),
                         id=dict(type="string"),
                     ),
                 ),
             )
         return OAPI.Responses(
             **{
                 "200": OAPI.Response(
                     description="JSON-RPC 2.0 Response Object",
+                    # TODO: content-type get from serializer
                     content={"application/json": media},
+                    # TODO: required=True,
+                    #  when method is not notification
                 ),
             },
         )
 
 
 """
 WSGI types definitions
@@ -1020,14 +1052,112 @@
 ASGIApplication: TypeAlias = Callable[
     [ASGIScope, ASGIReceive, ASGISend],
     Awaitable[None],
 ]
 
 
 """
+RSGI types definitions
+https://github.com/emmett-framework/granian/blob/master/docs/spec/RSGI.md
+"""
+
+
+class RSGIScope:
+    proto: Literal["http", "ws"] = "http"
+    rsgi_version: Literal["1", "1.1", "2"]
+    http_version: str
+    server: str
+    client: str
+    scheme: Literal["http", "https"]
+    method: str
+    path: str
+    query_string: str
+    headers: Mapping[str, str]
+
+
+class RSGIHTTPProtocol(Protocol):
+    async def __call__(self, body: bytes) -> None:
+        ...
+
+    def response_empty(
+        self,
+        status: int,
+        headers: list[tuple[str, str]],
+        body: None,
+    ) -> None:
+        ...
+
+    def response_str(
+        self,
+        status: int,
+        headers: list[tuple[str, str]],
+        body: str,
+    ) -> None:
+        ...
+
+    def response_bytes(
+        self,
+        status: int,
+        headers: list[tuple[str, str]],
+        body: bytes,
+    ) -> None:
+        ...
+
+    def response_file(
+        self,
+        status: int,
+        headers: list[tuple[str, str]],
+        body: str,
+    ) -> None:
+        ...
+
+
+class RSGITransport(Protocol):
+    async def receive(self) -> bytes:
+        ...
+
+    async def send_bytes(self, message: bytes) -> None:
+        ...
+
+    async def send_str(self, message: str) -> None:
+        ...
+
+
+class MessageKind(IntEnum):
+    CLOSED = 0
+    """Websocket closed by client"""
+    BYTES = 1
+    """Bytes message"""
+    STRING = 2
+    """String message"""
+
+
+class RSGIWebsocketMessage:
+    kind: Literal[0, 1, 2]
+    data: bytes | str | None
+
+
+class RSGIWSProtocol(Protocol):
+    async def accept(self) -> RSGIWebsocketMessage:
+        ...
+
+    def close(self) -> None:
+        ...
+
+
+RSGIProtocol: TypeAlias = Union[RSGIHTTPProtocol, RSGIWSProtocol]
+
+
+RSGIApplication: TypeAlias = Callable[
+    [RSGIScope, RSGIProtocol],
+    Awaitable[None],
+]
+
+
+"""
 Helpful types
 """
 
 
 class Comparator(Protocol):
     def __call__(
         self,
@@ -1038,14 +1168,15 @@
 
 
 class ProxyRequest(MutableMapping):
     """A wrapper class for environment mapping.
 
     :param environment:
 
+    TODO: check requestProxy on get_set_ENV_attrs
     """
 
     __slots__ = ("__environment",)
 
     def __init__(self, environment: ASGIScope | WSGIEnvironment):
         self.__environment = environment
 
@@ -1110,10 +1241,11 @@
 
     def __delattr__(self, item):
         del self.__environment[item]
 
 
 AnyRequest: TypeAlias = Union[
     ASGIScope,
+    RSGIScope,
     WSGIEnvironment,
     ProxyRequest,
 ]
```

### Comparing `drakaina-0.7.0b7/drakaina/wsgi.py` & `drakaina-0.7.1/drakaina/wsgi.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,16 @@
 
 ALLOWED_METHODS = ("OPTIONS", "GET", "POST")
 
 
 class WSGIHandler:
     """Implementation of WSGI protocol.
 
+    # todo: write about urls (route, provide_ args)
+
     :param route:
     :type route: str | re.Pattern
     :param handler: RPC protocol implementation.
     :type handler: BaseRPCProtocol
     :param middlewares: List of WSGI middlewares.
     :type middlewares: Iterable[type[BaseMiddleware] | partial[BaseMiddleware]]
     :param logger: A `logging.Logger` object.
@@ -98,14 +100,15 @@
         openapi_url: str | re.Pattern | None = None,
     ):
         self.handler = handler if handler is not None else JsonRPCv2()
         self._rpc_content_type = self.handler.content_type
 
         self.route = route
         if isinstance(self.route, str) and not self.route.startswith("/"):
+            # need it?
             self.route = "/" + self.route
         schema_url = getattr(self.handler, "schema_url", None)
         if (
             self.route is not None
             and hasattr(self.handler, "schema_url")
             and schema_url is None
         ):
```

### Comparing `drakaina-0.7.0b7/LICENSE` & `drakaina-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b7/pyproject.toml` & `drakaina-0.7.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drakaina"
-version = "0.7.0-beta.7"
+version = "0.7.1"
 description = "Module for simple RPC service implementation"
 authors = ["Aleksey Terentyev <terentyev.a@pm.me>"]
 license = "Apache License 2.0"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Web Environment",
```

### Comparing `drakaina-0.7.0b7/README.md` & `drakaina-0.7.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,85 +1,142 @@
-# drakaina
-
-![Drakaina](content/drakaina.png "Drakaina"){width=200px height=205px}
+<p style="text-align: center;"><img src="https://gitlab.com/tau_lex/drakaina/-/raw/main/content/drakaina300.png" style="" /></p>
+<h2 style="text-align: center;">drakaina</h2>
 
 [![image](https://img.shields.io/pypi/v/drakaina.svg)](https://pypi.python.org/pypi/drakaina)
 [![image](https://img.shields.io/pypi/l/drakaina.svg)](https://pypi.python.org/pypi/drakaina)
 [![image](https://img.shields.io/pypi/pyversions/drakaina.svg)](https://pypi.python.org/pypi/drakaina)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/psf/black)
 [![OpenRPC](https://img.shields.io/endpoint?url=https%3A%2F%2Fgitlab.com%2Ftau_lex%2Fdrakaina%2F-%2Fraw%2Fmain%2Fcontent%2Fopenrpc-badge.json)](https://open-rpc.org)
 [![libera manifesto](https://img.shields.io/badge/libera-manifesto-lightgrey.svg)](https://liberamanifesto.com)
 
-❗ WIP ❗
-
 Framework for simple RPC service implementation.
 
 
-## Quickstart
+## Features
+
+- Serializers layer.
+  - `json`, `orjson`, `ujson` and `msgpack` serializers.
+- Generates schemas for documentation in OpenRPC format.
+- WSGI protocol implementation
+  - CORS middleware
+  - JWT Authorization middleware.
+  - Compatible with middlewares for others wsgi-frameworks,
+    like as [Werkzeug](https://palletsprojects.com/p/werkzeug/),
+    [Flask](https://palletsprojects.com/p/flask/)
+- `login_required` and `check_permissions` decorators.
+
+
+## Installation and Dependencies
 
 Drakaina may be installed via `pip` and requires Python 3.8 or higher :
 
 ```shell
 pip install drakaina
 ```
 
+## Usage Examples
+
 A minimal Drakaina example is:
 
 ```python
+import asyncio
 from drakaina import remote_procedure
+from drakaina.asgi import ASGIHandler
 from drakaina.wsgi import WSGIHandler
 
+
 @remote_procedure("hello")
 def hello_method(name):
     return f"Hello, {name}!"
 
+
 """
 >>> from drakaina.rpc_protocols import JsonRPCv2
 >>> JsonRPCv2().handle({"jsonrpc": "2.0", "method": "hello", "params": ["🐍 Python"] "id": 1})
 {"jsonrpc": "2.0", "result": "Hello, 🐍 Python!", "id": 1}
 """
 
 # Or define WSGI application
 app = WSGIHandler(route="/jrpc")
 
+# Or define ASGI application
+app2 = ASGIHandler(route="/ajrpc")
 ```
 
 
-## Features
+## Roadmap
 
-- Serializers layer.
-  - `json`, `orjson`, `ujson` and `msgpack` serializers.
-- Generates schemas for documentation in OpenRPC format.
-- WSGI protocol implementation
-  - CORS middleware
-  - JWT Authorization middleware.
-  - Compatible with middlewares for others wsgi-frameworks,
+- API Auto Documentation
+  - [x] OpenRPC format.
+  - [ ] OpenAPI format.
+  - [ ] JsonSchema format.
+- Transport protocols
+  - [x] WSGI protocol
+  - [ ] ASGI protocol
+    - [ ] Middlewares support
+  - [ ] RSGI protocol
+- Middlewares
+  - [x] CORS middleware
+  - [x] JWT Authorization middleware.
+
+    **_todo_**: https://pyjwt.readthedocs.io/en/latest/usage.html#oidc-login-flow
+    **_todo_**:**_187_**: what if it coroutine?
+
+  - [x] Compatible with middlewares for others wsgi-frameworks,
     like as [Werkzeug](https://palletsprojects.com/p/werkzeug/),
     [Flask](https://palletsprojects.com/p/flask/)
-- `login_required` and `check_permissions` decorators.
+  - [ ] GZip middleware
+- Permission decorators
+  - [x] `login_required` decorator
+  - [x] `check_permissions` decorator
+- preload or server example
+- Serializers
+  - [x] Json serializer
+  - [x] UJson serializer
+  - [x] ORJson serializer
+  - [x] Msgpack serializer
+  - [ ] Dataclass serializer
+
+    > Наследуется от базового или Json, и содержит внутри Json для сериализации в dict -> bytes
+
+  - [ ] cysimdjson serializer
+  - [ ] msgspec serializer
+  - [ ] pickle serializer
+  - [ ] cbor serializer
 
 
+# NOTES (> Don't commit this section! <)
+
+- https://githab.com/abersheeran/rpc.py
+- https://gitlab.com/jsonrpc/jsonrpc-py
+
 # Documentation
 
 
-## Installation
+### Optional requirements
 
 ```shell
-pip install drakaina
+pip install drakaina[jwt, orjson, ujson]
 ```
 
 
-## Middlewares
+## Define remote procedures
+
+
+### Middlewares
 
 
-### CORS
+#### Logging
 
 
-### JWT
+#### CORS
+
+
+#### JWT
 
 Drakaina may be installed via `pip` and requires Python 3.7 or higher :
 
 ```shell
 pip install drakaina[jwt]
 ```
 
@@ -176,15 +233,15 @@
 urlpatterns = [
     ...,
     path("api/", RPCView.as_view(autodiscover="rpc_views")),
 ]
 ```
 
 
-### JWT Authentication in your Django project
+#### JWT Authentication in your Django project
 
 Wrap an instance of `RPCView` with the `JWTAuthenticationMiddleware`.
 
 ```python
 from django.urls import path
 from drakaina.contrib.django import RPCView, JWTAuthenticationMiddleware
 
@@ -203,15 +260,18 @@
 
 DRAKAINA_JWT_SECRET_KEY = "__SECRET_KEY__"
 
 ...
 ```
 
 
-## License
+# Contributing
+
+
+# License
 
 Apache License 2.0
 
-## Artwork
+# Artwork
 
 "[drakaina.png](content/drakaina.png)" by Korolko Anastasia is licensed under
 <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="License Creative Commons" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/80x15.png" /></a> ([CC BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/)).
```

### Comparing `drakaina-0.7.0b7/PKG-INFO` & `drakaina-0.7.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drakaina
-Version: 0.7.0b7
+Version: 0.7.1
 Summary: Module for simple RPC service implementation
 Home-page: https://gitlab.com/tau_lex/drakaina
 License: Apache-2.0
 Keywords: rpc,jsonrpc,openrpc
 Author: Aleksey Terentyev
 Author-email: terentyev.a@pm.me
 Requires-Python: >=3.8,<4.0
@@ -31,92 +31,149 @@
 Requires-Dist: orjson (>=3.8.14,<4.0.0) ; extra == "orjson"
 Requires-Dist: pyjwt (>=2.7.0,<3.0.0) ; extra == "jwt"
 Requires-Dist: typing-extensions (>=4.6.2,<5.0.0)
 Requires-Dist: ujson (>=5.7.0,<6.0.0) ; extra == "ujson"
 Project-URL: Repository, https://gitlab.com/tau_lex/drakaina
 Description-Content-Type: text/markdown
 
-# drakaina
-
-![Drakaina](content/drakaina.png "Drakaina"){width=200px height=205px}
+<p style="text-align: center;"><img src="https://gitlab.com/tau_lex/drakaina/-/raw/main/content/drakaina300.png" style="" /></p>
+<h2 style="text-align: center;">drakaina</h2>
 
 [![image](https://img.shields.io/pypi/v/drakaina.svg)](https://pypi.python.org/pypi/drakaina)
 [![image](https://img.shields.io/pypi/l/drakaina.svg)](https://pypi.python.org/pypi/drakaina)
 [![image](https://img.shields.io/pypi/pyversions/drakaina.svg)](https://pypi.python.org/pypi/drakaina)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/psf/black)
 [![OpenRPC](https://img.shields.io/endpoint?url=https%3A%2F%2Fgitlab.com%2Ftau_lex%2Fdrakaina%2F-%2Fraw%2Fmain%2Fcontent%2Fopenrpc-badge.json)](https://open-rpc.org)
 [![libera manifesto](https://img.shields.io/badge/libera-manifesto-lightgrey.svg)](https://liberamanifesto.com)
 
-❗ WIP ❗
-
 Framework for simple RPC service implementation.
 
 
-## Quickstart
+## Features
+
+- Serializers layer.
+  - `json`, `orjson`, `ujson` and `msgpack` serializers.
+- Generates schemas for documentation in OpenRPC format.
+- WSGI protocol implementation
+  - CORS middleware
+  - JWT Authorization middleware.
+  - Compatible with middlewares for others wsgi-frameworks,
+    like as [Werkzeug](https://palletsprojects.com/p/werkzeug/),
+    [Flask](https://palletsprojects.com/p/flask/)
+- `login_required` and `check_permissions` decorators.
+
+
+## Installation and Dependencies
 
 Drakaina may be installed via `pip` and requires Python 3.8 or higher :
 
 ```shell
 pip install drakaina
 ```
 
+## Usage Examples
+
 A minimal Drakaina example is:
 
 ```python
+import asyncio
 from drakaina import remote_procedure
+from drakaina.asgi import ASGIHandler
 from drakaina.wsgi import WSGIHandler
 
+
 @remote_procedure("hello")
 def hello_method(name):
     return f"Hello, {name}!"
 
+
 """
 >>> from drakaina.rpc_protocols import JsonRPCv2
 >>> JsonRPCv2().handle({"jsonrpc": "2.0", "method": "hello", "params": ["🐍 Python"] "id": 1})
 {"jsonrpc": "2.0", "result": "Hello, 🐍 Python!", "id": 1}
 """
 
 # Or define WSGI application
 app = WSGIHandler(route="/jrpc")
 
+# Or define ASGI application
+app2 = ASGIHandler(route="/ajrpc")
 ```
 
 
-## Features
+## Roadmap
 
-- Serializers layer.
-  - `json`, `orjson`, `ujson` and `msgpack` serializers.
-- Generates schemas for documentation in OpenRPC format.
-- WSGI protocol implementation
-  - CORS middleware
-  - JWT Authorization middleware.
-  - Compatible with middlewares for others wsgi-frameworks,
+- API Auto Documentation
+  - [x] OpenRPC format.
+  - [ ] OpenAPI format.
+  - [ ] JsonSchema format.
+- Transport protocols
+  - [x] WSGI protocol
+  - [ ] ASGI protocol
+    - [ ] Middlewares support
+  - [ ] RSGI protocol
+- Middlewares
+  - [x] CORS middleware
+  - [x] JWT Authorization middleware.
+
+    **_todo_**: https://pyjwt.readthedocs.io/en/latest/usage.html#oidc-login-flow
+    **_todo_**:**_187_**: what if it coroutine?
+
+  - [x] Compatible with middlewares for others wsgi-frameworks,
     like as [Werkzeug](https://palletsprojects.com/p/werkzeug/),
     [Flask](https://palletsprojects.com/p/flask/)
-- `login_required` and `check_permissions` decorators.
+  - [ ] GZip middleware
+- Permission decorators
+  - [x] `login_required` decorator
+  - [x] `check_permissions` decorator
+- preload or server example
+- Serializers
+  - [x] Json serializer
+  - [x] UJson serializer
+  - [x] ORJson serializer
+  - [x] Msgpack serializer
+  - [ ] Dataclass serializer
+
+    > Наследуется от базового или Json, и содержит внутри Json для сериализации в dict -> bytes
+
+  - [ ] cysimdjson serializer
+  - [ ] msgspec serializer
+  - [ ] pickle serializer
+  - [ ] cbor serializer
 
 
+# NOTES (> Don't commit this section! <)
+
+- https://githab.com/abersheeran/rpc.py
+- https://gitlab.com/jsonrpc/jsonrpc-py
+
 # Documentation
 
 
-## Installation
+### Optional requirements
 
 ```shell
-pip install drakaina
+pip install drakaina[jwt, orjson, ujson]
 ```
 
 
-## Middlewares
+## Define remote procedures
+
+
+### Middlewares
 
 
-### CORS
+#### Logging
 
 
-### JWT
+#### CORS
+
+
+#### JWT
 
 Drakaina may be installed via `pip` and requires Python 3.7 or higher :
 
 ```shell
 pip install drakaina[jwt]
 ```
 
@@ -213,15 +270,15 @@
 urlpatterns = [
     ...,
     path("api/", RPCView.as_view(autodiscover="rpc_views")),
 ]
 ```
 
 
-### JWT Authentication in your Django project
+#### JWT Authentication in your Django project
 
 Wrap an instance of `RPCView` with the `JWTAuthenticationMiddleware`.
 
 ```python
 from django.urls import path
 from drakaina.contrib.django import RPCView, JWTAuthenticationMiddleware
 
@@ -240,16 +297,19 @@
 
 DRAKAINA_JWT_SECRET_KEY = "__SECRET_KEY__"
 
 ...
 ```
 
 
-## License
+# Contributing
+
+
+# License
 
 Apache License 2.0
 
-## Artwork
+# Artwork
 
 "[drakaina.png](content/drakaina.png)" by Korolko Anastasia is licensed under
 <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="License Creative Commons" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/80x15.png" /></a> ([CC BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/)).
```

