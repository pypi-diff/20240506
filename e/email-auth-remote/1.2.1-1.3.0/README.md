# Comparing `tmp/email-auth-remote-1.2.1.tar.gz` & `tmp/email_auth_remote-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "email-auth-remote-1.2.1.tar", last modified: Wed Apr 10 05:19:14 2024, max compression
+gzip compressed data, was "email_auth_remote-1.3.0.tar", last modified: Mon May  6 05:06:32 2024, max compression
```

## Comparing `email-auth-remote-1.2.1.tar` & `email_auth_remote-1.3.0.tar`

### file list

```diff
@@ -1,27 +1,25 @@
-drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2024-04-10 05:19:14.796538 email-auth-remote-1.2.1/
--rw-r--r--   0 nikita    (1000) nikita    (1000)     3456 2024-04-10 05:19:14.796538 email-auth-remote-1.2.1/PKG-INFO
--rw-rw-r--   0 nikita    (1000) nikita    (1000)     2835 2024-04-09 06:14:20.000000 email-auth-remote-1.2.1/README.md
-drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2024-04-10 05:19:14.796538 email-auth-remote-1.2.1/email_auth_remote/
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      351 2024-04-08 14:54:42.000000 email-auth-remote-1.2.1/email_auth_remote/__init__.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      224 2024-04-10 05:18:08.000000 email-auth-remote-1.2.1/email_auth_remote/admin.py
-drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2024-04-10 05:19:14.796538 email-auth-remote-1.2.1/email_auth_remote/admin_override/
--rw-rw-r--   0 nikita    (1000) nikita    (1000)        0 2024-04-09 17:58:40.000000 email-auth-remote-1.2.1/email_auth_remote/admin_override/__init__.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      177 2024-04-09 18:01:10.000000 email-auth-remote-1.2.1/email_auth_remote/admin_override/apps.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      311 2024-04-09 17:22:04.000000 email-auth-remote-1.2.1/email_auth_remote/apps.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)     1225 2024-04-10 03:56:04.000000 email-auth-remote-1.2.1/email_auth_remote/authentication.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      251 2024-04-10 03:45:16.000000 email-auth-remote-1.2.1/email_auth_remote/context_processors.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      635 2024-04-10 04:18:27.000000 email-auth-remote-1.2.1/email_auth_remote/middleware.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)     1494 2024-04-08 14:45:35.000000 email-auth-remote-1.2.1/email_auth_remote/models.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      212 2024-04-08 07:54:28.000000 email-auth-remote-1.2.1/email_auth_remote/schema.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      459 2024-04-10 05:18:26.000000 email-auth-remote-1.2.1/email_auth_remote/settings.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      251 2024-04-08 16:40:59.000000 email-auth-remote-1.2.1/email_auth_remote/urls.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      660 2024-04-10 03:55:41.000000 email-auth-remote-1.2.1/email_auth_remote/utils.py
--rw-rw-r--   0 nikita    (1000) nikita    (1000)     1159 2024-04-10 03:53:38.000000 email-auth-remote-1.2.1/email_auth_remote/views.py
-drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2024-04-10 05:19:14.796538 email-auth-remote-1.2.1/email_auth_remote.egg-info/
--rw-r--r--   0 nikita    (1000) nikita    (1000)     3456 2024-04-10 05:19:14.000000 email-auth-remote-1.2.1/email_auth_remote.egg-info/PKG-INFO
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      671 2024-04-10 05:19:14.000000 email-auth-remote-1.2.1/email_auth_remote.egg-info/SOURCES.txt
--rw-rw-r--   0 nikita    (1000) nikita    (1000)        1 2024-04-10 05:19:14.000000 email-auth-remote-1.2.1/email_auth_remote.egg-info/dependency_links.txt
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      110 2024-04-10 05:19:14.000000 email-auth-remote-1.2.1/email_auth_remote.egg-info/requires.txt
--rw-rw-r--   0 nikita    (1000) nikita    (1000)       18 2024-04-10 05:19:14.000000 email-auth-remote-1.2.1/email_auth_remote.egg-info/top_level.txt
--rw-rw-r--   0 nikita    (1000) nikita    (1000)      674 2024-04-10 05:18:53.000000 email-auth-remote-1.2.1/pyproject.toml
--rw-rw-r--   0 nikita    (1000) nikita    (1000)       38 2024-04-10 05:19:14.796538 email-auth-remote-1.2.1/setup.cfg
+drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2024-05-06 05:06:32.842818 email_auth_remote-1.3.0/
+-rw-r--r--   0 nikita    (1000) nikita    (1000)     3884 2024-05-06 05:06:32.842818 email_auth_remote-1.3.0/PKG-INFO
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     3263 2024-05-06 05:04:52.000000 email_auth_remote-1.3.0/README.md
+drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2024-05-06 05:06:32.842818 email_auth_remote-1.3.0/email_auth_remote/
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      351 2024-04-19 16:14:00.000000 email_auth_remote-1.3.0/email_auth_remote/__init__.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      224 2024-04-19 16:14:00.000000 email_auth_remote-1.3.0/email_auth_remote/admin.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      311 2024-04-19 16:14:00.000000 email_auth_remote-1.3.0/email_auth_remote/apps.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     1225 2024-04-19 16:14:00.000000 email_auth_remote-1.3.0/email_auth_remote/authentication.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      251 2024-04-19 16:14:00.000000 email_auth_remote-1.3.0/email_auth_remote/context_processors.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      635 2024-04-19 16:14:00.000000 email_auth_remote-1.3.0/email_auth_remote/middleware.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     1535 2024-05-06 04:51:25.000000 email_auth_remote-1.3.0/email_auth_remote/models.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     1461 2024-05-06 04:58:55.000000 email_auth_remote-1.3.0/email_auth_remote/permissions.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      212 2024-04-19 16:14:00.000000 email_auth_remote-1.3.0/email_auth_remote/schema.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      459 2024-04-19 16:14:00.000000 email_auth_remote-1.3.0/email_auth_remote/settings.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      251 2024-04-19 16:14:00.000000 email_auth_remote-1.3.0/email_auth_remote/urls.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      624 2024-05-06 05:05:37.000000 email_auth_remote-1.3.0/email_auth_remote/utils.py
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)     1159 2024-04-19 16:14:00.000000 email_auth_remote-1.3.0/email_auth_remote/views.py
+drwxrwxr-x   0 nikita    (1000) nikita    (1000)        0 2024-05-06 05:06:32.842818 email_auth_remote-1.3.0/email_auth_remote.egg-info/
+-rw-r--r--   0 nikita    (1000) nikita    (1000)     3884 2024-05-06 05:06:32.000000 email_auth_remote-1.3.0/email_auth_remote.egg-info/PKG-INFO
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      618 2024-05-06 05:06:32.000000 email_auth_remote-1.3.0/email_auth_remote.egg-info/SOURCES.txt
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)        1 2024-05-06 05:06:32.000000 email_auth_remote-1.3.0/email_auth_remote.egg-info/dependency_links.txt
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      110 2024-05-06 05:06:32.000000 email_auth_remote-1.3.0/email_auth_remote.egg-info/requires.txt
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)       18 2024-05-06 05:06:32.000000 email_auth_remote-1.3.0/email_auth_remote.egg-info/top_level.txt
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)      674 2024-05-06 05:00:33.000000 email_auth_remote-1.3.0/pyproject.toml
+-rw-rw-r--   0 nikita    (1000) nikita    (1000)       38 2024-05-06 05:06:32.842818 email_auth_remote-1.3.0/setup.cfg
```

### Comparing `email-auth-remote-1.2.1/PKG-INFO` & `email_auth_remote-1.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: email-auth-remote
-Version: 1.2.1
+Version: 1.3.0
 Summary: Django app for an endpoint authentication.
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.11
@@ -98,14 +98,34 @@
 ```
 
 **Важная информация:**
 При использовании библиотеки модель CustomTokenUser, полученная через request.user не будет
 сохранена в
 БД. На эту модель невозможно ссылаться через ForeignKey и тд. Сохранение в БД также невозможно.
 
+## Разрешения IsDesigner IsSeller 
+
+Всего есть 4 возможных permissions. 
+
+```python
+from email_auth_remote.permissions import (
+    IsDesigner,
+    IsSeller,
+    IsSellerOrReadOnly,
+    IsDesignerOrReadOnly,
+)
+
+class ExampleView(generics.GenericAPIView):
+    """
+    Пример View только для продавца.
+    """
+    permission_classes = (IsSeller,)
+    # other logic here ...
+```
+
 ## Сборка
 
 ***Необходимо только для сборки, для интеграции не надо.***
 
 Как собрать проект локально
 
 ```bash
```

### Comparing `email-auth-remote-1.2.1/README.md` & `email_auth_remote-1.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -81,14 +81,34 @@
 ```
 
 **Важная информация:**
 При использовании библиотеки модель CustomTokenUser, полученная через request.user не будет
 сохранена в
 БД. На эту модель невозможно ссылаться через ForeignKey и тд. Сохранение в БД также невозможно.
 
+## Разрешения IsDesigner IsSeller 
+
+Всего есть 4 возможных permissions. 
+
+```python
+from email_auth_remote.permissions import (
+    IsDesigner,
+    IsSeller,
+    IsSellerOrReadOnly,
+    IsDesignerOrReadOnly,
+)
+
+class ExampleView(generics.GenericAPIView):
+    """
+    Пример View только для продавца.
+    """
+    permission_classes = (IsSeller,)
+    # other logic here ...
+```
+
 ## Сборка
 
 ***Необходимо только для сборки, для интеграции не надо.***
 
 Как собрать проект локально
 
 ```bash
```

### Comparing `email-auth-remote-1.2.1/email_auth_remote/authentication.py` & `email_auth_remote-1.3.0/email_auth_remote/authentication.py`

 * *Files identical despite different names*

### Comparing `email-auth-remote-1.2.1/email_auth_remote/middleware.py` & `email_auth_remote-1.3.0/email_auth_remote/middleware.py`

 * *Files identical despite different names*

### Comparing `email-auth-remote-1.2.1/email_auth_remote/models.py` & `email_auth_remote-1.3.0/email_auth_remote/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import Optional
 
 from django.utils.functional import cached_property
 from rest_framework_simplejwt.models import TokenUser
 
 
 class CustomTokenUser(TokenUser):
-
     def save(self) -> None:
         raise NotImplementedError("Token users have no DB representation")
 
     def delete(self) -> None:
         raise NotImplementedError("Token users have no DB representation")
 
     def set_password(self, raw_password: str) -> None:
@@ -34,12 +33,13 @@
         """
         # Active superusers have all permissions.
         if self.is_active and self.is_superuser:
             return True
         return False
 
     @cached_property
-    def short_name(self) -> str:
-        return self.token.get("first_name", "")
+    def is_seller(self) -> bool:
+        return self.token.get("is_seller", False)
 
-    def get_short_name(self) -> str:
-        return self.short_name
+    @cached_property
+    def is_designer(self) -> bool:
+        return self.token.get("is_designer", False)
```

### Comparing `email-auth-remote-1.2.1/email_auth_remote/utils.py` & `email_auth_remote-1.3.0/email_auth_remote/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from rest_framework import exceptions
 from rest_framework.authentication import CSRFCheck
 
-from .settings import api_settings
-
 
 def enforce_csrf(request):
     """
     Enforce CSRF validation for session based authentication.
     """
 
     def dummy_get_response(request):  # pragma: no cover
```

### Comparing `email-auth-remote-1.2.1/email_auth_remote/views.py` & `email_auth_remote-1.3.0/email_auth_remote/views.py`

 * *Files identical despite different names*

### Comparing `email-auth-remote-1.2.1/email_auth_remote.egg-info/PKG-INFO` & `email_auth_remote-1.3.0/email_auth_remote.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: email-auth-remote
-Version: 1.2.1
+Version: 1.3.0
 Summary: Django app for an endpoint authentication.
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.11
@@ -98,14 +98,34 @@
 ```
 
 **Важная информация:**
 При использовании библиотеки модель CustomTokenUser, полученная через request.user не будет
 сохранена в
 БД. На эту модель невозможно ссылаться через ForeignKey и тд. Сохранение в БД также невозможно.
 
+## Разрешения IsDesigner IsSeller 
+
+Всего есть 4 возможных permissions. 
+
+```python
+from email_auth_remote.permissions import (
+    IsDesigner,
+    IsSeller,
+    IsSellerOrReadOnly,
+    IsDesignerOrReadOnly,
+)
+
+class ExampleView(generics.GenericAPIView):
+    """
+    Пример View только для продавца.
+    """
+    permission_classes = (IsSeller,)
+    # other logic here ...
+```
+
 ## Сборка
 
 ***Необходимо только для сборки, для интеграции не надо.***
 
 Как собрать проект локально
 
 ```bash
```

### Comparing `email-auth-remote-1.2.1/email_auth_remote.egg-info/SOURCES.txt` & `email_auth_remote-1.3.0/email_auth_remote.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 email_auth_remote/__init__.py
 email_auth_remote/admin.py
 email_auth_remote/apps.py
 email_auth_remote/authentication.py
 email_auth_remote/context_processors.py
 email_auth_remote/middleware.py
 email_auth_remote/models.py
+email_auth_remote/permissions.py
 email_auth_remote/schema.py
 email_auth_remote/settings.py
 email_auth_remote/urls.py
 email_auth_remote/utils.py
 email_auth_remote/views.py
 email_auth_remote.egg-info/PKG-INFO
 email_auth_remote.egg-info/SOURCES.txt
 email_auth_remote.egg-info/dependency_links.txt
 email_auth_remote.egg-info/requires.txt
-email_auth_remote.egg-info/top_level.txt
-email_auth_remote/admin_override/__init__.py
-email_auth_remote/admin_override/apps.py
+email_auth_remote.egg-info/top_level.txt
```

### Comparing `email-auth-remote-1.2.1/pyproject.toml` & `email_auth_remote-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "email-auth-remote"
-version = "1.2.1"
+version = "1.3.0"
 description = "Django app for an endpoint authentication."
 readme = "README.md"
 requires-python = ">=3.11"
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
```

