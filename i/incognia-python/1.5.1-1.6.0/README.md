# Comparing `tmp/incognia-python-1.5.1.tar.gz` & `tmp/incognia_python-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "incognia-python-1.5.1.tar", last modified: Wed Mar 20 20:46:44 2024, max compression
+gzip compressed data, was "incognia_python-1.6.0.tar", last modified: Mon May  6 15:24:42 2024, max compression
```

## Comparing `incognia-python-1.5.1.tar` & `incognia_python-1.6.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:46:44.165672 incognia-python-1.5.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:46:44.161672 incognia-python-1.5.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-20 20:46:39.000000 incognia-python-1.5.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:46:44.161672 incognia-python-1.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-03-20 20:46:39.000000 incognia-python-1.5.1/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-03-20 20:46:39.000000 incognia-python-1.5.1/.github/workflows/continuous.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-03-20 20:46:39.000000 incognia-python-1.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-20 20:46:39.000000 incognia-python-1.5.1/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-20 20:46:39.000000 incognia-python-1.5.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-20 20:46:39.000000 incognia-python-1.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8807 2024-03-20 20:46:44.165672 incognia-python-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8277 2024-03-20 20:46:39.000000 incognia-python-1.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:46:44.165672 incognia-python-1.5.1/incognia/
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-20 20:46:39.000000 incognia-python-1.5.1/incognia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-03-20 20:46:39.000000 incognia-python-1.5.1/incognia/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-03-20 20:46:39.000000 incognia-python-1.5.1/incognia/base_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-20 20:46:39.000000 incognia-python-1.5.1/incognia/datetime_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-20 20:46:39.000000 incognia-python-1.5.1/incognia/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-20 20:46:39.000000 incognia-python-1.5.1/incognia/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-03-20 20:46:39.000000 incognia-python-1.5.1/incognia/feedback_events.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-20 20:46:39.000000 incognia-python-1.5.1/incognia/json_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-03-20 20:46:39.000000 incognia-python-1.5.1/incognia/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-03-20 20:46:39.000000 incognia-python-1.5.1/incognia/token_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:46:44.165672 incognia-python-1.5.1/incognia_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8807 2024-03-20 20:46:44.000000 incognia-python-1.5.1/incognia_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-20 20:46:44.000000 incognia-python-1.5.1/incognia_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 20:46:44.000000 incognia-python-1.5.1/incognia_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 20:46:43.000000 incognia-python-1.5.1/incognia_python.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-20 20:46:44.000000 incognia-python-1.5.1/incognia_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-20 20:46:44.000000 incognia-python-1.5.1/incognia_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-20 20:46:39.000000 incognia-python-1.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-20 20:46:39.000000 incognia-python-1.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-03-20 20:46:44.165672 incognia-python-1.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:46:44.165672 incognia-python-1.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 20:46:39.000000 incognia-python-1.5.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21846 2024-03-20 20:46:39.000000 incognia-python-1.5.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-03-20 20:46:39.000000 incognia-python-1.5.1/tests/test_base_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-03-20 20:46:39.000000 incognia-python-1.5.1/tests/test_token_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:24:42.554084 incognia_python-1.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:24:42.550084 incognia_python-1.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-06 15:24:33.000000 incognia_python-1.6.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:24:42.550084 incognia_python-1.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-06 15:24:33.000000 incognia_python-1.6.0/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-06 15:24:33.000000 incognia_python-1.6.0/.github/workflows/continuous.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-06 15:24:33.000000 incognia_python-1.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-06 15:24:33.000000 incognia_python-1.6.0/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-06 15:24:33.000000 incognia_python-1.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-06 15:24:33.000000 incognia_python-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9068 2024-05-06 15:24:42.554084 incognia_python-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-05-06 15:24:33.000000 incognia_python-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:24:42.554084 incognia_python-1.6.0/incognia/
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-06 15:24:33.000000 incognia_python-1.6.0/incognia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-05-06 15:24:33.000000 incognia_python-1.6.0/incognia/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-06 15:24:33.000000 incognia_python-1.6.0/incognia/base_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-06 15:24:33.000000 incognia_python-1.6.0/incognia/datetime_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-06 15:24:33.000000 incognia_python-1.6.0/incognia/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-06 15:24:33.000000 incognia_python-1.6.0/incognia/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-06 15:24:33.000000 incognia_python-1.6.0/incognia/feedback_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-06 15:24:33.000000 incognia_python-1.6.0/incognia/json_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-06 15:24:33.000000 incognia_python-1.6.0/incognia/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-06 15:24:33.000000 incognia_python-1.6.0/incognia/token_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:24:42.554084 incognia_python-1.6.0/incognia_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9068 2024-05-06 15:24:42.000000 incognia_python-1.6.0/incognia_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-06 15:24:42.000000 incognia_python-1.6.0/incognia_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 15:24:42.000000 incognia_python-1.6.0/incognia_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 15:24:42.000000 incognia_python-1.6.0/incognia_python.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-06 15:24:42.000000 incognia_python-1.6.0/incognia_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-06 15:24:42.000000 incognia_python-1.6.0/incognia_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-06 15:24:33.000000 incognia_python-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-06 15:24:33.000000 incognia_python-1.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-06 15:24:42.554084 incognia_python-1.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:24:42.554084 incognia_python-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:24:33.000000 incognia_python-1.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22323 2024-05-06 15:24:33.000000 incognia_python-1.6.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-05-06 15:24:33.000000 incognia_python-1.6.0/tests/test_base_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-06 15:24:33.000000 incognia_python-1.6.0/tests/test_token_manager.py
```

### Comparing `incognia-python-1.5.1/.github/workflows/codeql.yaml` & `incognia_python-1.6.0/.github/workflows/codeql.yaml`

 * *Files identical despite different names*

### Comparing `incognia-python-1.5.1/.github/workflows/continuous.yaml` & `incognia_python-1.6.0/.github/workflows/continuous.yaml`

 * *Files identical despite different names*

### Comparing `incognia-python-1.5.1/.gitignore` & `incognia_python-1.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `incognia-python-1.5.1/LICENSE.txt` & `incognia_python-1.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `incognia-python-1.5.1/PKG-INFO` & `incognia_python-1.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: incognia-python
-Version: 1.5.1
+Version: 1.6.0
 Summary: Python lightweight client library for Incognia APIs
 Home-page: https://github.com/inloco/incognia-python
 Author: Incognia
 Author-email: opensource@incognia.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
@@ -187,33 +187,41 @@
             'last_four_digits': '1234',
             'expiry_year': '2027',
             'expiry_month': '10'
         }
     }
 ]
 
+policy_id: str = 'policy-id'
+
 assessment: dict = api.register_payment('installation-id',
                                         'account-id',
                                         'external-id',
                                         addresses=addresses,
                                         payment_value=payment_value,
-                                        payment_methods=payment_methods)
+                                        payment_methods=payment_methods,
+                                        policy_id=policy_id)
 ```
 
 #### Registering Login
 
 This method registers a new login for the given installation and account, returning a `dict`,
 containing the risk assessment and supporting evidence.
 
 ```python3
 from incognia.api import IncogniaAPI
 
 api = IncogniaAPI('client-id', 'client-secret')
 
-assessment: dict = api.register_login('installation-id', 'account-id', 'external-id')
+policy_id: str = 'policy-id'
+
+assessment: dict = api.register_login('installation-id', 
+                                      'account-id', 
+                                      'external-id', 
+                                      policy_id='policy_id')
 ```
 
 ## Evidences
 
 Every assessment response includes supporting evidence in a dict. You can find all available
 evidences [here](https://docs.incognia.com/apis/understanding-assessment-evidence).
```

### Comparing `incognia-python-1.5.1/README.md` & `incognia_python-1.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -171,33 +171,41 @@
             'last_four_digits': '1234',
             'expiry_year': '2027',
             'expiry_month': '10'
         }
     }
 ]
 
+policy_id: str = 'policy-id'
+
 assessment: dict = api.register_payment('installation-id',
                                         'account-id',
                                         'external-id',
                                         addresses=addresses,
                                         payment_value=payment_value,
-                                        payment_methods=payment_methods)
+                                        payment_methods=payment_methods,
+                                        policy_id=policy_id)
 ```
 
 #### Registering Login
 
 This method registers a new login for the given installation and account, returning a `dict`,
 containing the risk assessment and supporting evidence.
 
 ```python3
 from incognia.api import IncogniaAPI
 
 api = IncogniaAPI('client-id', 'client-secret')
 
-assessment: dict = api.register_login('installation-id', 'account-id', 'external-id')
+policy_id: str = 'policy-id'
+
+assessment: dict = api.register_login('installation-id', 
+                                      'account-id', 
+                                      'external-id', 
+                                      policy_id='policy_id')
 ```
 
 ## Evidences
 
 Every assessment response includes supporting evidence in a dict. You can find all available
 evidences [here](https://docs.incognia.com/apis/understanding-assessment-evidence).
```

### Comparing `incognia-python-1.5.1/incognia/api.py` & `incognia_python-1.6.0/incognia/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,15 +97,16 @@
     def register_payment(self,
                          installation_id: str,
                          account_id: str,
                          external_id: Optional[str] = None,
                          addresses: Optional[List[TransactionAddress]] = None,
                          payment_value: Optional[PaymentValue] = None,
                          payment_methods: Optional[List[PaymentMethod]] = None,
-                         evaluate: Optional[bool] = None) -> dict:
+                         evaluate: Optional[bool] = None,
+                         policy_id: Optional[str] = None) -> dict:
         if not installation_id:
             raise IncogniaError('installation_id is required.')
         if not account_id:
             raise IncogniaError('account_id is required.')
 
         try:
             headers = self.__get_authorization_header()
@@ -114,69 +115,74 @@
             body = {
                 'type': 'payment',
                 'installation_id': installation_id,
                 'account_id': account_id,
                 'external_id': external_id,
                 'addresses': addresses,
                 'payment_value': payment_value,
-                'payment_methods': payment_methods
+                'payment_methods': payment_methods,
+                'policy_id': policy_id
             }
             data = encode(body)
             return self.__request.post(Endpoints.TRANSACTIONS, headers=headers, params=params,
                                        data=data)
 
         except IncogniaHTTPError as e:
             raise IncogniaHTTPError(e) from None
 
     def register_login(self,
                        installation_id: str,
                        account_id: str,
                        external_id: Optional[str] = None,
-                       evaluate: Optional[bool] = None) -> dict:
+                       evaluate: Optional[bool] = None,
+                       policy_id: Optional[str] = None) -> dict:
         if not installation_id:
             raise IncogniaError('installation_id is required.')
         if not account_id:
             raise IncogniaError('account_id is required.')
 
         try:
             headers = self.__get_authorization_header()
             headers.update(JSON_CONTENT_HEADER)
             params = None if evaluate is None else {'eval': evaluate}
             body = {
                 'type': 'login',
                 'installation_id': installation_id,
                 'account_id': account_id,
-                'external_id': external_id
+                'external_id': external_id,
+                'policy_id': policy_id
             }
             data = encode(body)
             return self.__request.post(Endpoints.TRANSACTIONS, headers=headers, params=params,
                                        data=data)
 
         except IncogniaHTTPError as e:
             raise IncogniaHTTPError(e) from None
 
     def register_web_login(self,
                            session_token: str,
                            account_id: str,
                            external_id: Optional[str] = None,
-                           evaluate: Optional[bool] = None) -> dict:
+                           evaluate: Optional[bool] = None,
+                           policy_id: Optional[str] = None) -> dict:
         if not session_token:
             raise IncogniaError('session_token is required.')
         if not account_id:
             raise IncogniaError('account_id is required.')
 
         try:
             headers = self.__get_authorization_header()
             headers.update(JSON_CONTENT_HEADER)
             params = None if evaluate is None else {'eval': evaluate}
             body = {
                 'type': 'login',
                 'session_token': session_token,
                 'account_id': account_id,
-                'external_id': external_id
+                'external_id': external_id,
+                'policy_id': policy_id
             }
             data = encode(body)
             return self.__request.post(Endpoints.TRANSACTIONS, headers=headers, params=params,
                                        data=data)
 
         except IncogniaHTTPError as e:
             raise IncogniaHTTPError(e) from None
```

### Comparing `incognia-python-1.5.1/incognia/base_request.py` & `incognia_python-1.6.0/incognia/base_request.py`

 * *Files identical despite different names*

### Comparing `incognia-python-1.5.1/incognia/feedback_events.py` & `incognia_python-1.6.0/incognia/feedback_events.py`

 * *Files identical despite different names*

### Comparing `incognia-python-1.5.1/incognia/models.py` & `incognia_python-1.6.0/incognia/models.py`

 * *Files identical despite different names*

### Comparing `incognia-python-1.5.1/incognia/token_manager.py` & `incognia_python-1.6.0/incognia/token_manager.py`

 * *Files identical despite different names*

### Comparing `incognia-python-1.5.1/incognia_python.egg-info/PKG-INFO` & `incognia_python-1.6.0/incognia_python.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: incognia-python
-Version: 1.5.1
+Version: 1.6.0
 Summary: Python lightweight client library for Incognia APIs
 Home-page: https://github.com/inloco/incognia-python
 Author: Incognia
 Author-email: opensource@incognia.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
@@ -187,33 +187,41 @@
             'last_four_digits': '1234',
             'expiry_year': '2027',
             'expiry_month': '10'
         }
     }
 ]
 
+policy_id: str = 'policy-id'
+
 assessment: dict = api.register_payment('installation-id',
                                         'account-id',
                                         'external-id',
                                         addresses=addresses,
                                         payment_value=payment_value,
-                                        payment_methods=payment_methods)
+                                        payment_methods=payment_methods,
+                                        policy_id=policy_id)
 ```
 
 #### Registering Login
 
 This method registers a new login for the given installation and account, returning a `dict`,
 containing the risk assessment and supporting evidence.
 
 ```python3
 from incognia.api import IncogniaAPI
 
 api = IncogniaAPI('client-id', 'client-secret')
 
-assessment: dict = api.register_login('installation-id', 'account-id', 'external-id')
+policy_id: str = 'policy-id'
+
+assessment: dict = api.register_login('installation-id', 
+                                      'account-id', 
+                                      'external-id', 
+                                      policy_id='policy_id')
 ```
 
 ## Evidences
 
 Every assessment response includes supporting evidence in a dict. You can find all available
 evidences [here](https://docs.incognia.com/apis/understanding-assessment-evidence).
```

### Comparing `incognia-python-1.5.1/incognia_python.egg-info/SOURCES.txt` & `incognia_python-1.6.0/incognia_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `incognia-python-1.5.1/setup.cfg` & `incognia_python-1.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `incognia-python-1.5.1/tests/test_api.py` & `incognia_python-1.6.0/tests/test_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,30 +79,33 @@
     REGISTER_INVALID_FEEDBACK_DATA: Final[bytes] = encode({
         'event': f'{INVALID_EVENT_FEEDBACK_TYPE}',
         'timestamp': 0
     })
     REGISTER_VALID_PAYMENT_DATA: Final[bytes] = encode({
         'type': 'payment',
         'installation_id': f'{INSTALLATION_ID}',
-        'account_id': f'{ACCOUNT_ID}'
+        'account_id': f'{ACCOUNT_ID}',
+        'policy_id': f'{POLICY_ID}'
     })
     REGISTER_INVALID_PAYMENT_DATA: Final[bytes] = encode({
         'type': 'payment',
         'installation_id': f'{INVALID_INSTALLATION_ID}',
         'account_id': f'{INVALID_ACCOUNT_ID}'
     })
     REGISTER_VALID_LOGIN_DATA: Final[bytes] = encode({
         'type': 'login',
         'installation_id': f'{INSTALLATION_ID}',
-        'account_id': f'{ACCOUNT_ID}'
+        'account_id': f'{ACCOUNT_ID}',
+        'policy_id': f'{POLICY_ID}'
     })
     REGISTER_VALID_WEB_LOGIN_DATA: Final[bytes] = encode({
         'type': 'login',
         'session_token': f'{SESSION_TOKEN}',
-        'account_id': f'{ACCOUNT_ID}'
+        'account_id': f'{ACCOUNT_ID}',
+        'policy_id': f'{POLICY_ID}'
     })
     REGISTER_INVALID_LOGIN_DATA: Final[bytes] = encode({
         'type': 'login',
         'installation_id': f'{INVALID_INSTALLATION_ID}',
         'account_id': f'{INVALID_ACCOUNT_ID}'
     })
     REGISTER_INVALID_WEB_LOGIN_DATA: Final[bytes] = encode({
@@ -273,15 +276,17 @@
     @patch.object(TokenManager, 'get', return_value=TOKEN_VALUES)
     def test_register_payment_when_required_fields_are_valid_should_work(
             self, mock_token_manager_get: Mock, mock_base_request_post: Mock):
         mock_base_request_post.configure_mock(return_value=self.JSON_RESPONSE)
 
         api = IncogniaAPI(self.CLIENT_ID, self.CLIENT_SECRET)
 
-        request_response = api.register_payment(self.INSTALLATION_ID, self.ACCOUNT_ID)
+        request_response = api.register_payment(self.INSTALLATION_ID,
+                                                self.ACCOUNT_ID,
+                                                policy_id=self.POLICY_ID)
 
         mock_token_manager_get.assert_called()
         mock_base_request_post.assert_called_with(Endpoints.TRANSACTIONS,
                                                   headers=self.AUTH_AND_JSON_CONTENT_HEADERS,
                                                   params=self.DEFAULT_PARAMS,
                                                   data=self.REGISTER_VALID_PAYMENT_DATA)
 
@@ -333,15 +338,17 @@
     @patch.object(TokenManager, 'get', return_value=TOKEN_VALUES)
     def test_register_login_when_required_fields_are_valid_should_work(
             self, mock_token_manager_get: Mock, mock_base_request_post: Mock):
         mock_base_request_post.configure_mock(return_value=self.JSON_RESPONSE)
 
         api = IncogniaAPI(self.CLIENT_ID, self.CLIENT_SECRET)
 
-        request_response = api.register_login(self.INSTALLATION_ID, self.ACCOUNT_ID)
+        request_response = api.register_login(self.INSTALLATION_ID,
+                                              self.ACCOUNT_ID,
+                                              policy_id=self.POLICY_ID)
 
         mock_token_manager_get.assert_called()
         mock_base_request_post.assert_called_with(Endpoints.TRANSACTIONS,
                                                   headers=self.AUTH_AND_JSON_CONTENT_HEADERS,
                                                   params=self.DEFAULT_PARAMS,
                                                   data=self.REGISTER_VALID_LOGIN_DATA)
 
@@ -393,15 +400,17 @@
     @patch.object(TokenManager, 'get', return_value=TOKEN_VALUES)
     def test_register_web_login_when_required_fields_are_valid_should_work(
             self, mock_token_manager_get: Mock, mock_base_request_post: Mock):
         mock_base_request_post.configure_mock(return_value=self.JSON_RESPONSE)
 
         api = IncogniaAPI(self.CLIENT_ID, self.CLIENT_SECRET)
 
-        request_response = api.register_web_login(self.SESSION_TOKEN, self.ACCOUNT_ID)
+        request_response = api.register_web_login(self.SESSION_TOKEN,
+                                                  self.ACCOUNT_ID,
+                                                  policy_id=self.POLICY_ID)
 
         mock_token_manager_get.assert_called()
         mock_base_request_post.assert_called_with(Endpoints.TRANSACTIONS,
                                                   headers=self.AUTH_AND_JSON_CONTENT_HEADERS,
                                                   params=self.DEFAULT_PARAMS,
                                                   data=self.REGISTER_VALID_WEB_LOGIN_DATA)
```

### Comparing `incognia-python-1.5.1/tests/test_base_request.py` & `incognia_python-1.6.0/tests/test_base_request.py`

 * *Files identical despite different names*

### Comparing `incognia-python-1.5.1/tests/test_token_manager.py` & `incognia_python-1.6.0/tests/test_token_manager.py`

 * *Files identical despite different names*

