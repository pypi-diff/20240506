# Comparing `tmp/django_ninja_extra-0.20.6.tar.gz` & `tmp/django_ninja_extra-0.20.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_ninja_extra-0.20.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_ninja_extra-0.20.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_ninja_extra-0.20.6.tar` & `django_ninja_extra-0.20.7.tar`

### file list

```diff
@@ -1,57 +1,61 @@
--rw-r--r--   0        0        0     4290 2024-04-24 17:36:28.085167 django_ninja_extra-0.20.6/README.md
--rw-r--r--   0        0        0     1554 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/__init__.py
--rw-r--r--   0        0        0     1291 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/apps.py
--rw-r--r--   0        0        0      440 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/compatible.py
--rw-r--r--   0        0        0       55 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/conf/__init__.py
--rw-r--r--   0        0        0     3560 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/conf/settings.py
--rw-r--r--   0        0        0      577 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/constants.py
--rw-r--r--   0        0        0     1159 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/controllers/__init__.py
--rw-r--r--   0        0        0    19313 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/controllers/base.py
--rw-r--r--   0        0        0      476 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/controllers/model/__init__.py
--rw-r--r--   0        0        0     6976 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/controllers/model/builder.py
--rw-r--r--   0        0        0    26945 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/controllers/model/endpoints.py
--rw-r--r--   0        0        0     1813 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/controllers/model/interfaces.py
--rw-r--r--   0        0        0     5466 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/controllers/model/path_resolver.py
--rw-r--r--   0        0        0     8116 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/controllers/model/schemas.py
--rw-r--r--   0        0        0     3774 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/controllers/model/service.py
--rw-r--r--   0        0        0     1286 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/controllers/registry.py
--rw-r--r--   0        0        0      854 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/controllers/response.py
--rw-r--r--   0        0        0    25873 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/controllers/route/__init__.py
--rw-r--r--   0        0        0     1271 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/controllers/route/context.py
--rw-r--r--   0        0        0     7875 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/controllers/route/route_functions.py
--rw-r--r--   0        0        0     1434 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/dependency_resolver.py
--rw-r--r--   0        0        0     1879 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/details.py
--rw-r--r--   0        0        0     8928 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/exceptions.py
--rw-r--r--   0        0        0     1775 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/generic.py
--rw-r--r--   0        0        0      597 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/helper.py
--rw-r--r--   0        0        0      670 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/lazy.py
--rw-r--r--   0        0        0       61 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/logger.py
--rw-r--r--   0        0        0     4782 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/main.py
--rw-r--r--   0        0        0     1099 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/modules.py
--rw-r--r--   0        0        0    12921 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/operation.py
--rw-r--r--   0        0        0     8121 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/ordering.py
--rw-r--r--   0        0        0     8354 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/pagination.py
--rw-r--r--   0        0        0      281 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/permissions/__init__.py
--rw-r--r--   0        0        0     5633 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/permissions/base.py
--rw-r--r--   0        0        0     1622 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/permissions/common.py
--rw-r--r--   0        0        0        0 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/py.typed
--rw-r--r--   0        0        0     2195 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/router.py
--rw-r--r--   0        0        0      430 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/schemas/__init__.py
--rw-r--r--   0        0        0     2230 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/schemas/response.py
--rw-r--r--   0        0        0     9207 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/searching.py
--rw-r--r--   0        0        0      748 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/security/__init__.py
--rw-r--r--   0        0        0      880 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/security/api_key.py
--rw-r--r--   0        0        0     1696 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/security/http.py
--rw-r--r--   0        0        0      542 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/security/session.py
--rw-r--r--   0        0        0     2503 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/shortcuts.py
--rw-r--r--   0        0        0      163 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/signals.py
--rw-r--r--   0        0        0     2515 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/status.py
--rw-r--r--   0        0        0      112 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/testing/__init__.py
--rw-r--r--   0        0        0     2089 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/testing/client.py
--rw-r--r--   0        0        0      318 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/throttling/__init__.py
--rw-r--r--   0        0        0     3931 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/throttling/decorator.py
--rw-r--r--   0        0        0     8243 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/throttling/model.py
--rw-r--r--   0        0        0      267 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/types.py
--rw-r--r--   0        0        0     1104 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/ninja_extra/urls.py
--rw-r--r--   0        0        0     2695 2024-04-24 17:36:28.125166 django_ninja_extra-0.20.6/pyproject.toml
--rw-r--r--   0        0        0     6195 1970-01-01 00:00:00.000000 django_ninja_extra-0.20.6/PKG-INFO
+-rw-r--r--   0        0        0     4290 2024-05-06 14:32:32.334449 django_ninja_extra-0.20.7/README.md
+-rw-r--r--   0        0        0     1554 2024-05-06 14:32:32.370449 django_ninja_extra-0.20.7/ninja_extra/__init__.py
+-rw-r--r--   0        0        0     1291 2024-05-06 14:32:32.370449 django_ninja_extra-0.20.7/ninja_extra/apps.py
+-rw-r--r--   0        0        0      440 2024-05-06 14:32:32.370449 django_ninja_extra-0.20.7/ninja_extra/compatible.py
+-rw-r--r--   0        0        0       55 2024-05-06 14:32:32.370449 django_ninja_extra-0.20.7/ninja_extra/conf/__init__.py
+-rw-r--r--   0        0        0     3560 2024-05-06 14:32:32.370449 django_ninja_extra-0.20.7/ninja_extra/conf/settings.py
+-rw-r--r--   0        0        0      577 2024-05-06 14:32:32.370449 django_ninja_extra-0.20.7/ninja_extra/constants.py
+-rw-r--r--   0        0        0     1159 2024-05-06 14:32:32.370449 django_ninja_extra-0.20.7/ninja_extra/controllers/__init__.py
+-rw-r--r--   0        0        0    19313 2024-05-06 14:32:32.370449 django_ninja_extra-0.20.7/ninja_extra/controllers/base.py
+-rw-r--r--   0        0        0      476 2024-05-06 14:32:32.370449 django_ninja_extra-0.20.7/ninja_extra/controllers/model/__init__.py
+-rw-r--r--   0        0        0     6976 2024-05-06 14:32:32.370449 django_ninja_extra-0.20.7/ninja_extra/controllers/model/builder.py
+-rw-r--r--   0        0        0    26945 2024-05-06 14:32:32.370449 django_ninja_extra-0.20.7/ninja_extra/controllers/model/endpoints.py
+-rw-r--r--   0        0        0     1813 2024-05-06 14:32:32.370449 django_ninja_extra-0.20.7/ninja_extra/controllers/model/interfaces.py
+-rw-r--r--   0        0        0     5493 2024-05-06 14:32:32.370449 django_ninja_extra-0.20.7/ninja_extra/controllers/model/path_resolver.py
+-rw-r--r--   0        0        0     8116 2024-05-06 14:32:32.370449 django_ninja_extra-0.20.7/ninja_extra/controllers/model/schemas.py
+-rw-r--r--   0        0        0     3774 2024-05-06 14:32:32.370449 django_ninja_extra-0.20.7/ninja_extra/controllers/model/service.py
+-rw-r--r--   0        0        0     1286 2024-05-06 14:32:32.370449 django_ninja_extra-0.20.7/ninja_extra/controllers/registry.py
+-rw-r--r--   0        0        0      854 2024-05-06 14:32:32.370449 django_ninja_extra-0.20.7/ninja_extra/controllers/response.py
+-rw-r--r--   0        0        0    25873 2024-05-06 14:32:32.370449 django_ninja_extra-0.20.7/ninja_extra/controllers/route/__init__.py
+-rw-r--r--   0        0        0     1271 2024-05-06 14:32:32.370449 django_ninja_extra-0.20.7/ninja_extra/controllers/route/context.py
+-rw-r--r--   0        0        0     7875 2024-05-06 14:32:32.370449 django_ninja_extra-0.20.7/ninja_extra/controllers/route/route_functions.py
+-rw-r--r--   0        0        0     1434 2024-05-06 14:32:32.370449 django_ninja_extra-0.20.7/ninja_extra/dependency_resolver.py
+-rw-r--r--   0        0        0     1879 2024-05-06 14:32:32.370449 django_ninja_extra-0.20.7/ninja_extra/details.py
+-rw-r--r--   0        0        0     8928 2024-05-06 14:32:32.370449 django_ninja_extra-0.20.7/ninja_extra/exceptions.py
+-rw-r--r--   0        0        0     1775 2024-05-06 14:32:32.370449 django_ninja_extra-0.20.7/ninja_extra/generic.py
+-rw-r--r--   0        0        0      597 2024-05-06 14:32:32.370449 django_ninja_extra-0.20.7/ninja_extra/helper.py
+-rw-r--r--   0        0        0      670 2024-05-06 14:32:32.370449 django_ninja_extra-0.20.7/ninja_extra/lazy.py
+-rw-r--r--   0        0        0       61 2024-05-06 14:32:32.370449 django_ninja_extra-0.20.7/ninja_extra/logger.py
+-rw-r--r--   0        0        0     5032 2024-05-06 14:32:32.370449 django_ninja_extra-0.20.7/ninja_extra/main.py
+-rw-r--r--   0        0        0     1099 2024-05-06 14:32:32.370449 django_ninja_extra-0.20.7/ninja_extra/modules.py
+-rw-r--r--   0        0        0    12947 2024-05-06 14:32:32.370449 django_ninja_extra-0.20.7/ninja_extra/operation.py
+-rw-r--r--   0        0        0     8518 2024-05-06 14:32:32.374449 django_ninja_extra-0.20.7/ninja_extra/ordering.py
+-rw-r--r--   0        0        0      524 2024-05-06 14:32:32.374449 django_ninja_extra-0.20.7/ninja_extra/pagination/__init__.py
+-rw-r--r--   0        0        0     1779 2024-05-06 14:32:32.374449 django_ninja_extra-0.20.7/ninja_extra/pagination/decorator.py
+-rw-r--r--   0        0        0      102 2024-05-06 14:32:32.374449 django_ninja_extra-0.20.7/ninja_extra/pagination/models/__init__.py
+-rw-r--r--   0        0        0     3522 2024-05-06 14:32:32.374449 django_ninja_extra-0.20.7/ninja_extra/pagination/models/page_by_number.py
+-rw-r--r--   0        0        0     3555 2024-05-06 14:32:32.374449 django_ninja_extra-0.20.7/ninja_extra/pagination/operations.py
+-rw-r--r--   0        0        0      281 2024-05-06 14:32:32.374449 django_ninja_extra-0.20.7/ninja_extra/permissions/__init__.py
+-rw-r--r--   0        0        0     5633 2024-05-06 14:32:32.374449 django_ninja_extra-0.20.7/ninja_extra/permissions/base.py
+-rw-r--r--   0        0        0     1622 2024-05-06 14:32:32.374449 django_ninja_extra-0.20.7/ninja_extra/permissions/common.py
+-rw-r--r--   0        0        0        0 2024-05-06 14:32:32.374449 django_ninja_extra-0.20.7/ninja_extra/py.typed
+-rw-r--r--   0        0        0     2195 2024-05-06 14:32:32.374449 django_ninja_extra-0.20.7/ninja_extra/router.py
+-rw-r--r--   0        0        0      430 2024-05-06 14:32:32.374449 django_ninja_extra-0.20.7/ninja_extra/schemas/__init__.py
+-rw-r--r--   0        0        0     2230 2024-05-06 14:32:32.374449 django_ninja_extra-0.20.7/ninja_extra/schemas/response.py
+-rw-r--r--   0        0        0     8964 2024-05-06 14:32:32.374449 django_ninja_extra-0.20.7/ninja_extra/searching.py
+-rw-r--r--   0        0        0      748 2024-05-06 14:32:32.374449 django_ninja_extra-0.20.7/ninja_extra/security/__init__.py
+-rw-r--r--   0        0        0      880 2024-05-06 14:32:32.374449 django_ninja_extra-0.20.7/ninja_extra/security/api_key.py
+-rw-r--r--   0        0        0     1696 2024-05-06 14:32:32.374449 django_ninja_extra-0.20.7/ninja_extra/security/http.py
+-rw-r--r--   0        0        0      542 2024-05-06 14:32:32.374449 django_ninja_extra-0.20.7/ninja_extra/security/session.py
+-rw-r--r--   0        0        0     2503 2024-05-06 14:32:32.374449 django_ninja_extra-0.20.7/ninja_extra/shortcuts.py
+-rw-r--r--   0        0        0      163 2024-05-06 14:32:32.374449 django_ninja_extra-0.20.7/ninja_extra/signals.py
+-rw-r--r--   0        0        0     2515 2024-05-06 14:32:32.374449 django_ninja_extra-0.20.7/ninja_extra/status.py
+-rw-r--r--   0        0        0      112 2024-05-06 14:32:32.374449 django_ninja_extra-0.20.7/ninja_extra/testing/__init__.py
+-rw-r--r--   0        0        0     2089 2024-05-06 14:32:32.374449 django_ninja_extra-0.20.7/ninja_extra/testing/client.py
+-rw-r--r--   0        0        0      318 2024-05-06 14:32:32.374449 django_ninja_extra-0.20.7/ninja_extra/throttling/__init__.py
+-rw-r--r--   0        0        0     3931 2024-05-06 14:32:32.374449 django_ninja_extra-0.20.7/ninja_extra/throttling/decorator.py
+-rw-r--r--   0        0        0     8243 2024-05-06 14:32:32.374449 django_ninja_extra-0.20.7/ninja_extra/throttling/model.py
+-rw-r--r--   0        0        0      267 2024-05-06 14:32:32.374449 django_ninja_extra-0.20.7/ninja_extra/types.py
+-rw-r--r--   0        0        0     1104 2024-05-06 14:32:32.374449 django_ninja_extra-0.20.7/ninja_extra/urls.py
+-rw-r--r--   0        0        0     2746 2024-05-06 14:32:32.374449 django_ninja_extra-0.20.7/pyproject.toml
+-rw-r--r--   0        0        0     6251 1970-01-01 00:00:00.000000 django_ninja_extra-0.20.7/PKG-INFO
```

### Comparing `django_ninja_extra-0.20.6/README.md` & `django_ninja_extra-0.20.7/README.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.6/ninja_extra/__init__.py` & `django_ninja_extra-0.20.7/ninja_extra/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Django Ninja Extra - Class Based Utility and more for Django Ninja(Fast Django REST framework)"""
 
-__version__ = "0.20.6"
+__version__ = "0.20.7"
 
 import django
 
 from ninja_extra.controllers import (
     ControllerBase,
     ModelAsyncEndpointFactory,
     ModelConfig,
```

### Comparing `django_ninja_extra-0.20.6/ninja_extra/apps.py` & `django_ninja_extra-0.20.7/ninja_extra/apps.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.6/ninja_extra/conf/settings.py` & `django_ninja_extra-0.20.7/ninja_extra/conf/settings.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.6/ninja_extra/constants.py` & `django_ninja_extra-0.20.7/ninja_extra/constants.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.6/ninja_extra/controllers/__init__.py` & `django_ninja_extra-0.20.7/ninja_extra/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.6/ninja_extra/controllers/base.py` & `django_ninja_extra-0.20.7/ninja_extra/controllers/base.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.6/ninja_extra/controllers/model/builder.py` & `django_ninja_extra-0.20.7/ninja_extra/controllers/model/builder.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.6/ninja_extra/controllers/model/endpoints.py` & `django_ninja_extra-0.20.7/ninja_extra/controllers/model/endpoints.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.6/ninja_extra/controllers/model/interfaces.py` & `django_ninja_extra-0.20.7/ninja_extra/controllers/model/interfaces.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.6/ninja_extra/controllers/model/path_resolver.py` & `django_ninja_extra-0.20.7/ninja_extra/controllers/model/path_resolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 
                 add_ninja_contribute_args(
                     func,
                     (self.query_construct_name, dynamic_query_model, Query(...)),
                 )
             self.as_view = functools.wraps(func)(self.get_view_function())
         else:
-            self.as_view = func
+            self.as_view = func  # type:ignore[assignment]
 
     def get_path_fields(self) -> t.Generator:
         for path_name, path_type in self.compiled_path.param_convertors.items():
             yield path_name, (path_type, ...)
 
     def get_query_fields(self) -> t.Generator:
         for path_name, path_type in self.compiled_path.query_parameters.items():
```

### Comparing `django_ninja_extra-0.20.6/ninja_extra/controllers/model/schemas.py` & `django_ninja_extra-0.20.7/ninja_extra/controllers/model/schemas.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.6/ninja_extra/controllers/model/service.py` & `django_ninja_extra-0.20.7/ninja_extra/controllers/model/service.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.6/ninja_extra/controllers/registry.py` & `django_ninja_extra-0.20.7/ninja_extra/controllers/registry.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.6/ninja_extra/controllers/response.py` & `django_ninja_extra-0.20.7/ninja_extra/controllers/response.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.6/ninja_extra/controllers/route/__init__.py` & `django_ninja_extra-0.20.7/ninja_extra/controllers/route/__init__.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.6/ninja_extra/controllers/route/context.py` & `django_ninja_extra-0.20.7/ninja_extra/controllers/route/context.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.6/ninja_extra/controllers/route/route_functions.py` & `django_ninja_extra-0.20.7/ninja_extra/controllers/route/route_functions.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.6/ninja_extra/dependency_resolver.py` & `django_ninja_extra-0.20.7/ninja_extra/dependency_resolver.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.6/ninja_extra/details.py` & `django_ninja_extra-0.20.7/ninja_extra/details.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.6/ninja_extra/exceptions.py` & `django_ninja_extra-0.20.7/ninja_extra/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.6/ninja_extra/generic.py` & `django_ninja_extra-0.20.7/ninja_extra/generic.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.6/ninja_extra/helper.py` & `django_ninja_extra-0.20.7/ninja_extra/helper.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.6/ninja_extra/lazy.py` & `django_ninja_extra-0.20.7/ninja_extra/lazy.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.6/ninja_extra/main.py` & `django_ninja_extra-0.20.7/ninja_extra/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 from importlib import import_module
-from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Type, Union
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+    cast,
+)
 
 from django.core.exceptions import ImproperlyConfigured
 from django.http import HttpRequest, HttpResponse
 from django.urls import URLPattern, URLResolver
-from django.utils.module_loading import module_has_submodule
+from django.utils.module_loading import import_string, module_has_submodule
 from ninja import NinjaAPI
 from ninja.constants import NOT_SET
 from ninja.openapi.docs import DocsBase, Swagger
 from ninja.parser import Parser
 from ninja.renderers import BaseRenderer
 from ninja.types import DictStrAny, TCallable
 
@@ -90,17 +101,22 @@
         return (
             _url_tuple[0],
             self.app_name,
             str(_url_tuple[len(_url_tuple) - 1]),
         )
 
     def register_controllers(
-        self, *controllers: Union[Type[ControllerBase], Type]
+        self, *controllers: Union[Type[ControllerBase], Type, str]
     ) -> None:
         for controller in controllers:
+            if isinstance(controller, str):
+                controller = cast(
+                    Union[Type[ControllerBase], Type], import_string(controller)
+                )
+
             if not issubclass(controller, ControllerBase):
                 raise ImproperlyConfigured(
                     f"{controller.__class__.__name__} class is not a controller"
                 )
             api_controller: APIController = controller.get_api_controller()
             if not api_controller.registered:
                 self._routers.extend(api_controller.build_routers())  # type: ignore
```

### Comparing `django_ninja_extra-0.20.6/ninja_extra/modules.py` & `django_ninja_extra-0.20.7/ninja_extra/modules.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.6/ninja_extra/operation.py` & `django_ninja_extra-0.20.7/ninja_extra/operation.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     cast,
 )
 
 from django.http import HttpRequest
 from django.http.response import HttpResponse, HttpResponseBase
 from django.utils.encoding import force_str
 from ninja.constants import NOT_SET
+from ninja.errors import AuthenticationError
 from ninja.operation import (
     AsyncOperation as NinjaAsyncOperation,
 )
 from ninja.operation import (
     Operation as NinjaOperation,
 )
 from ninja.operation import (
@@ -241,15 +242,16 @@
                     result = callback(request)
             except Exception as exc:
                 return self.api.on_exception(request, exc)
 
             if result:
                 request.auth = result  # type: ignore
                 return None
-        return self.api.create_response(request, {"detail": "Unauthorized"}, status=401)
+
+        return self.api.on_exception(request, AuthenticationError())
 
     @asynccontextmanager
     async def _prep_run(  # type:ignore
         self, request: HttpRequest, **kw: Any
     ) -> AsyncIterator[RouteContext]:
         try:
             start_time = time.time()
```

### Comparing `django_ninja_extra-0.20.6/ninja_extra/ordering.py` & `django_ninja_extra-0.20.7/ninja_extra/ordering.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,16 @@
     Union,
     cast,
     overload,
 )
 
 from asgiref.sync import sync_to_async
 from django.db.models import QuerySet
-from ninja import Field, Query, Schema
+from django.http import HttpRequest
+from ninja import Field, P, Query, Schema
 from ninja.constants import NOT_SET
 from ninja.signature import is_async
 from pydantic import BaseModel
 
 from ninja_extra.conf import settings
 from ninja_extra.shortcuts import add_ninja_contribute_args
 
@@ -61,35 +62,45 @@
     def __init__(
         self,
         ordering_fields: Optional[List[str]] = None,
         pass_parameter: Optional[str] = None,
     ) -> None:
         super().__init__(pass_parameter=pass_parameter)
         self.ordering_fields = ordering_fields or "__all__"
+        self.Input = self.create_input(ordering_fields)  # type:ignore
+
+    def create_input(self, ordering_fields: Optional[List[str]]) -> Type[Input]:
+        if ordering_fields:
+
+            class DynamicInput(Ordering.Input):
+                ordering: Query[Optional[str], P(default=",".join(ordering_fields))]  # type:ignore[type-arg,valid-type]
+
+            return DynamicInput
+        return Ordering.Input
 
     def ordering_queryset(
         self, items: Union[QuerySet, List], ordering_input: Input
     ) -> Union[QuerySet, List]:
-        ordering = self.get_ordering(items, ordering_input.ordering)
-        if ordering:
+        ordering_ = self.get_ordering(items, ordering_input.ordering)
+        if ordering_:
             if isinstance(items, QuerySet):  # type:ignore
-                return items.order_by(*ordering)
+                return items.order_by(*ordering_)
             elif isinstance(items, list) and items:
 
                 def multisort(xs: List, specs: List[Tuple[str, bool]]) -> List:
                     orerator = itemgetter if isinstance(xs[0], dict) else attrgetter
-                    for key, reverse in specs:
+                    for key, reverse in reversed(specs):
                         xs.sort(key=orerator(key), reverse=reverse)
                     return xs
 
                 return multisort(
                     items,
                     [
                         (o[int(o.startswith("-")) :], o.startswith("-"))
-                        for o in ordering
+                        for o in ordering_
                     ],
                 )
         return items
 
     def get_ordering(
         self, items: Union[QuerySet, List], value: Optional[str]
     ) -> List[str]:
@@ -197,56 +208,58 @@
         orderator_kwargs_name: str = "ordering",
     ) -> None:
         self.orderator = orderator
         self.orderator_kwargs_name = orderator_kwargs_name
         self.view_func = view_func
 
         orderator_view = self.get_view_function()
-        _ninja_contribute_args: List[Tuple] = getattr(
-            self.view_func, "_ninja_contribute_args", []
-        )
-        orderator_view._ninja_contribute_args = (  # type:ignore[attr-defined]
-            _ninja_contribute_args
-        )
+        self.as_view = wraps(view_func)(orderator_view)
         add_ninja_contribute_args(
-            orderator_view,
+            self.as_view,
             (
                 self.orderator_kwargs_name,
                 self.orderator.Input,
                 self.orderator.InputSource,
             ),
         )
         orderator_view.orderator_operation = self  # type:ignore[attr-defined]
-        self.as_view = wraps(view_func)(orderator_view)
 
     @property
     def view_func_has_kwargs(self) -> bool:  # pragma: no cover
         return self.orderator.pass_parameter is not None
 
     def get_view_function(self) -> Callable:
-        def as_view(controller: "ControllerBase", *args: Any, **kw: Any) -> Any:
+        def as_view(
+            request_or_controller: Union["ControllerBase", HttpRequest],
+            *args: Any,
+            **kw: Any,
+        ) -> Any:
             func_kwargs = dict(**kw)
             ordering_params = func_kwargs.pop(self.orderator_kwargs_name)
             if self.orderator.pass_parameter:
                 func_kwargs[self.orderator.pass_parameter] = ordering_params
 
-            items = self.view_func(controller, *args, **func_kwargs)
+            items = self.view_func(request_or_controller, *args, **func_kwargs)
             return self.orderator.ordering_queryset(items, ordering_params)
 
         return as_view
 
 
 class AsyncOrderatorOperation(OrderatorOperation):
     def get_view_function(self) -> Callable:
-        async def as_view(controller: "ControllerBase", *args: Any, **kw: Any) -> Any:
+        async def as_view(
+            request_or_controller: Union["ControllerBase", HttpRequest],
+            *args: Any,
+            **kw: Any,
+        ) -> Any:
             func_kwargs = dict(**kw)
             ordering_params = func_kwargs.pop(self.orderator_kwargs_name)
             if self.orderator.pass_parameter:
                 func_kwargs[self.orderator.pass_parameter] = ordering_params
 
-            items = await self.view_func(controller, *args, **func_kwargs)
+            items = await self.view_func(request_or_controller, *args, **func_kwargs)
             ordering_queryset = cast(
                 Callable, sync_to_async(self.orderator.ordering_queryset)
             )
             return await ordering_queryset(items, ordering_params)
 
         return as_view
```

### Comparing `django_ninja_extra-0.20.6/ninja_extra/permissions/base.py` & `django_ninja_extra-0.20.7/ninja_extra/permissions/base.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.6/ninja_extra/permissions/common.py` & `django_ninja_extra-0.20.7/ninja_extra/permissions/common.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.6/ninja_extra/router.py` & `django_ninja_extra-0.20.7/ninja_extra/router.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.6/ninja_extra/schemas/response.py` & `django_ninja_extra-0.20.7/ninja_extra/schemas/response.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.6/ninja_extra/searching.py` & `django_ninja_extra-0.20.7/ninja_extra/searching.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,16 +87,16 @@
     }
 
     def __init__(
         self,
         search_fields: Optional[List[str]] = None,
         pass_parameter: Optional[str] = None,
     ) -> None:
+        super().__init__(pass_parameter=pass_parameter)
         self.search_fields = search_fields or []
-        self.pass_parameter = pass_parameter
 
     def searching_queryset(
         self, items: Union[QuerySet, List], searching_input: Input
     ) -> Union[QuerySet, List]:
         search_terms = self.get_search_terms(searching_input.search)
 
         if self.search_fields and search_terms:
@@ -236,30 +236,24 @@
         searcherator_kwargs_name: str = "searching",
     ) -> None:
         self.searcherator = searcherator
         self.searcherator_kwargs_name = searcherator_kwargs_name
         self.view_func = view_func
 
         searcherator_view = self.get_view_function()
-        _ninja_contribute_args: List[Tuple] = getattr(
-            self.view_func, "_ninja_contribute_args", []
-        )
-        searcherator_view._ninja_contribute_args = (  # type:ignore[attr-defined]
-            _ninja_contribute_args
-        )
+        self.as_view = wraps(view_func)(searcherator_view)
         add_ninja_contribute_args(
-            searcherator_view,
+            self.as_view,
             (
                 self.searcherator_kwargs_name,
                 self.searcherator.Input,
                 self.searcherator.InputSource,
             ),
         )
         searcherator_view.searcherator_operation = self  # type:ignore[attr-defined]
-        self.as_view = wraps(view_func)(searcherator_view)
 
     @property
     def view_func_has_kwargs(self) -> bool:  # pragma: no cover
         return self.searcherator.pass_parameter is not None
 
     def get_view_function(self) -> Callable:
         def as_view(controller: "ControllerBase", *args: Any, **kw: Any) -> Any:
```

### Comparing `django_ninja_extra-0.20.6/ninja_extra/security/__init__.py` & `django_ninja_extra-0.20.7/ninja_extra/security/__init__.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.6/ninja_extra/security/api_key.py` & `django_ninja_extra-0.20.7/ninja_extra/security/api_key.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.6/ninja_extra/security/http.py` & `django_ninja_extra-0.20.7/ninja_extra/security/http.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.6/ninja_extra/security/session.py` & `django_ninja_extra-0.20.7/ninja_extra/security/session.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.6/ninja_extra/shortcuts.py` & `django_ninja_extra-0.20.7/ninja_extra/shortcuts.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.6/ninja_extra/status.py` & `django_ninja_extra-0.20.7/ninja_extra/status.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.6/ninja_extra/testing/client.py` & `django_ninja_extra-0.20.7/ninja_extra/testing/client.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.6/ninja_extra/throttling/decorator.py` & `django_ninja_extra-0.20.7/ninja_extra/throttling/decorator.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.6/ninja_extra/throttling/model.py` & `django_ninja_extra-0.20.7/ninja_extra/throttling/model.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.6/ninja_extra/urls.py` & `django_ninja_extra-0.20.7/ninja_extra/urls.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.20.6/pyproject.toml` & `django_ninja_extra-0.20.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 [tool.flit.metadata]
 module = "ninja_extra"
 dist-name = "django-ninja-extra"
 author = "Ezeudoh Tochukwu"
 author-email = "tochukwu.ezeudoh@gmail.com"
 home-page = "https://github.com/eadwinCode/django-ninja-extra"
 classifiers = [
+    "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Information Technology",
     "Intended Audience :: System Administrators",
     "Operating System :: OS Independent",
     "Topic :: Internet",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Libraries",
```

### Comparing `django_ninja_extra-0.20.6/PKG-INFO` & `django_ninja_extra-0.20.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: django-ninja-extra
-Version: 0.20.6
+Version: 0.20.7
 Summary: Django Ninja Extra - Class Based Utility and more for Django Ninja(Fast Django REST framework)
 Home-page: https://github.com/eadwinCode/django-ninja-extra
 Author: Ezeudoh Tochukwu
 Author-email: tochukwu.ezeudoh@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
```

