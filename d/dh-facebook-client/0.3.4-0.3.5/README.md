# Comparing `tmp/dh-facebook-client-0.3.4.tar.gz` & `tmp/dh-facebook-client-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dh-facebook-client-0.3.4.tar", max compression
+gzip compressed data, was "dh-facebook-client-0.3.5.tar", max compression
```

## Comparing `dh-facebook-client-0.3.4.tar` & `dh-facebook-client-0.3.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       21 2024-05-03 14:50:35.479809 dh-facebook-client-0.3.4/PYPI_README.md
--rw-r--r--   0        0        0      927 2024-05-03 14:50:35.479809 dh-facebook-client-0.3.4/dh_facebook_client/__init__.py
--rw-r--r--   0        0        0    12270 2024-05-03 14:50:35.479809 dh-facebook-client-0.3.4/dh_facebook_client/client.py
--rw-r--r--   0        0        0      296 2024-05-03 14:50:35.479809 dh-facebook-client-0.3.4/dh_facebook_client/constants.py
--rw-r--r--   0        0        0     2707 2024-05-03 14:50:35.479809 dh-facebook-client-0.3.4/dh_facebook_client/dataclasses.py
--rw-r--r--   0        0        0      521 2024-05-03 14:50:35.479809 dh-facebook-client-0.3.4/dh_facebook_client/error_code.py
--rw-r--r--   0        0        0     4643 2024-05-03 14:50:35.479809 dh-facebook-client-0.3.4/dh_facebook_client/exceptions.py
--rw-r--r--   0        0        0     2946 2024-05-03 14:50:35.479809 dh-facebook-client-0.3.4/dh_facebook_client/helpers.py
--rw-r--r--   0        0        0      435 2024-05-03 14:50:35.479809 dh-facebook-client-0.3.4/dh_facebook_client/typings.py
--rw-r--r--   0        0        0      731 2024-05-03 14:50:35.479809 dh-facebook-client-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      709 2024-05-03 14:51:14.122117 dh-facebook-client-0.3.4/setup.py
--rw-r--r--   0        0        0      454 2024-05-03 14:51:14.122347 dh-facebook-client-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0       21 2024-05-06 16:30:42.057899 dh-facebook-client-0.3.5/PYPI_README.md
+-rw-r--r--   0        0        0      927 2024-05-06 16:30:42.057899 dh-facebook-client-0.3.5/dh_facebook_client/__init__.py
+-rw-r--r--   0        0        0    12419 2024-05-06 16:30:42.057899 dh-facebook-client-0.3.5/dh_facebook_client/client.py
+-rw-r--r--   0        0        0      296 2024-05-06 16:30:42.057899 dh-facebook-client-0.3.5/dh_facebook_client/constants.py
+-rw-r--r--   0        0        0     3996 2024-05-06 16:30:42.057899 dh-facebook-client-0.3.5/dh_facebook_client/dataclasses.py
+-rw-r--r--   0        0        0      521 2024-05-06 16:30:42.057899 dh-facebook-client-0.3.5/dh_facebook_client/error_code.py
+-rw-r--r--   0        0        0     4643 2024-05-06 16:30:42.057899 dh-facebook-client-0.3.5/dh_facebook_client/exceptions.py
+-rw-r--r--   0        0        0     2946 2024-05-06 16:30:42.057899 dh-facebook-client-0.3.5/dh_facebook_client/helpers.py
+-rw-r--r--   0        0        0      435 2024-05-06 16:30:42.057899 dh-facebook-client-0.3.5/dh_facebook_client/typings.py
+-rw-r--r--   0        0        0      731 2024-05-06 16:30:42.057899 dh-facebook-client-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      709 2024-05-06 16:31:19.212638 dh-facebook-client-0.3.5/setup.py
+-rw-r--r--   0        0        0      454 2024-05-06 16:31:19.212879 dh-facebook-client-0.3.5/PKG-INFO
```

### Comparing `dh-facebook-client-0.3.4/dh_facebook_client/__init__.py` & `dh-facebook-client-0.3.5/dh_facebook_client/__init__.py`

 * *Files identical despite different names*

### Comparing `dh-facebook-client-0.3.4/dh_facebook_client/client.py` & `dh-facebook-client-0.3.5/dh_facebook_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,20 @@
 from typing import Any, Final, Generator, Optional, Type
 
 import backoff
 from requests import Response, Session
 from requests.exceptions import JSONDecodeError
 
 from .constants import GRAPH_API_URL, GRAPH_API_VERSIONS
-from .dataclasses import AppUsageDetails, GraphAPIResponse, MarketingAPIThrottleInsights
+from .dataclasses import (
+    AppUsageDetails,
+    BusinessUseCaseUsageDetails,
+    GraphAPIResponse,
+    MarketingAPIThrottleInsights,
+)
 from .error_code import GraphAPICommonErrorCode
 from .exceptions import (
     GraphAPIApplicationError,
     GraphAPIError,
     GraphAPIServiceError,
     GraphAPITokenError,
     GraphAPIUsageError,
@@ -262,14 +267,15 @@
                 data=data,
                 timeout=timeout or self.global_timeout,
             )
             result, paging = self._parse_response_body_or_raise(response)
 
             return GraphAPIResponse(
                 app_usage_details=AppUsageDetails.from_header(response),
+                business_use_case_usage_details=BusinessUseCaseUsageDetails.from_header(response),
                 marketing_api_throttle_insights=MarketingAPIThrottleInsights.from_header(response),
                 data=result,
                 paging=paging,
             )
 
         return _retry_parameterizer()
```

### Comparing `dh-facebook-client-0.3.4/dh_facebook_client/error_code.py` & `dh-facebook-client-0.3.5/dh_facebook_client/error_code.py`

 * *Files identical despite different names*

### Comparing `dh-facebook-client-0.3.4/dh_facebook_client/exceptions.py` & `dh-facebook-client-0.3.5/dh_facebook_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `dh-facebook-client-0.3.4/dh_facebook_client/helpers.py` & `dh-facebook-client-0.3.5/dh_facebook_client/helpers.py`

 * *Files identical despite different names*

### Comparing `dh-facebook-client-0.3.4/pyproject.toml` & `dh-facebook-client-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dh-facebook-client"
-version = "0.3.4"
+version = "0.3.5"
 description = "Simple client for interacting with the Facebook Graph API"
 authors = ["pchisholm <chisholm.p@gmail.com>"]
 readme = "PYPI_README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.26.0"
```

### Comparing `dh-facebook-client-0.3.4/setup.py` & `dh-facebook-client-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['backoff>=1.11.1,<2.0.0', 'requests>=2.26.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'dh-facebook-client',
-    'version': '0.3.4',
+    'version': '0.3.5',
     'description': 'Simple client for interacting with the Facebook Graph API',
     'long_description': '# dh-facebook-client\n',
     'author': 'pchisholm',
     'author_email': 'chisholm.p@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

