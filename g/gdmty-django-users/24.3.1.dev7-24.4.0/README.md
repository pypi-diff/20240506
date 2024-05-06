# Comparing `tmp/gdmty-django-users-24.3.1.dev7.tar.gz` & `tmp/gdmty_django_users-24.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdmty-django-users-24.3.1.dev7.tar", last modified: Sat Mar 16 07:06:14 2024, max compression
+gzip compressed data, was "gdmty_django_users-24.4.0.tar", last modified: Mon May  6 03:30:51 2024, max compression
```

## Comparing `gdmty-django-users-24.3.1.dev7.tar` & `gdmty_django_users-24.4.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-03-16 07:06:14.225784 gdmty-django-users-24.3.1.dev7/
--rw-rw-rw-   0        0        0    35182 2024-03-16 06:30:23.000000 gdmty-django-users-24.3.1.dev7/LICENSE
--rw-rw-rw-   0        0        0       51 2024-03-16 06:30:23.000000 gdmty-django-users-24.3.1.dev7/MANIFEST.in
--rw-rw-rw-   0        0        0    47484 2024-03-16 07:06:14.224782 gdmty-django-users-24.3.1.dev7/PKG-INFO
--rw-rw-rw-   0        0        0     5794 2024-03-16 06:30:23.000000 gdmty-django-users-24.3.1.dev7/README.md
--rw-rw-rw-   0        0        0     1611 2024-03-16 07:05:47.000000 gdmty-django-users-24.3.1.dev7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-16 07:06:14.225784 gdmty-django-users-24.3.1.dev7/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-16 07:06:14.198951 gdmty-django-users-24.3.1.dev7/src/
-drwxrwxrwx   0        0        0        0 2024-03-16 07:06:14.215466 gdmty-django-users-24.3.1.dev7/src/gdmty_django_users/
--rw-rw-rw-   0        0        0     1373 2024-03-16 07:05:47.000000 gdmty-django-users-24.3.1.dev7/src/gdmty_django_users/__init__.py
--rw-rw-rw-   0        0        0     2480 2024-03-16 06:30:23.000000 gdmty-django-users-24.3.1.dev7/src/gdmty_django_users/admin.py
--rw-rw-rw-   0        0        0     1051 2024-03-16 06:30:23.000000 gdmty-django-users-24.3.1.dev7/src/gdmty_django_users/apps.py
--rw-rw-rw-   0        0        0      563 2024-03-16 06:30:23.000000 gdmty-django-users-24.3.1.dev7/src/gdmty_django_users/decorators.py
--rw-rw-rw-   0        0        0     1458 2024-03-16 06:30:23.000000 gdmty-django-users-24.3.1.dev7/src/gdmty_django_users/managers.py
-drwxrwxrwx   0        0        0        0 2024-03-16 07:06:14.222221 gdmty-django-users-24.3.1.dev7/src/gdmty_django_users/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-16 06:30:23.000000 gdmty-django-users-24.3.1.dev7/src/gdmty_django_users/migrations/__init__.py
--rw-rw-rw-   0        0        0     2038 2024-03-16 06:56:43.000000 gdmty-django-users-24.3.1.dev7/src/gdmty_django_users/models.py
--rw-rw-rw-   0        0        0      945 2024-03-16 06:30:23.000000 gdmty-django-users-24.3.1.dev7/src/gdmty_django_users/permissions.py
--rw-rw-rw-   0        0        0      889 2024-03-16 06:30:23.000000 gdmty-django-users-24.3.1.dev7/src/gdmty_django_users/serializers.py
--rw-rw-rw-   0        0        0     1070 2024-03-16 06:30:23.000000 gdmty-django-users-24.3.1.dev7/src/gdmty_django_users/settings.py
--rw-rw-rw-   0        0        0      913 2024-03-16 06:30:23.000000 gdmty-django-users-24.3.1.dev7/src/gdmty_django_users/tests.py
--rw-rw-rw-   0        0        0      429 2024-03-16 06:30:23.000000 gdmty-django-users-24.3.1.dev7/src/gdmty_django_users/urls.py
--rw-rw-rw-   0        0        0      877 2024-03-16 06:30:23.000000 gdmty-django-users-24.3.1.dev7/src/gdmty_django_users/views.py
--rw-rw-rw-   0        0        0     4797 2024-03-16 06:30:23.000000 gdmty-django-users-24.3.1.dev7/src/gdmty_django_users/viewsets.py
-drwxrwxrwx   0        0        0        0 2024-03-16 07:06:14.223763 gdmty-django-users-24.3.1.dev7/src/gdmty_django_users.egg-info/
--rw-rw-rw-   0        0        0    47484 2024-03-16 07:06:14.000000 gdmty-django-users-24.3.1.dev7/src/gdmty_django_users.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      763 2024-03-16 07:06:14.000000 gdmty-django-users-24.3.1.dev7/src/gdmty_django_users.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-16 07:06:14.000000 gdmty-django-users-24.3.1.dev7/src/gdmty_django_users.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      129 2024-03-16 07:06:14.000000 gdmty-django-users-24.3.1.dev7/src/gdmty_django_users.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-03-16 07:06:14.000000 gdmty-django-users-24.3.1.dev7/src/gdmty_django_users.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 03:30:51.037202 gdmty_django_users-24.4.0/
+-rw-rw-rw-   0        0        0    35182 2024-03-16 06:30:23.000000 gdmty_django_users-24.4.0/LICENSE
+-rw-rw-rw-   0        0        0       51 2024-03-16 06:30:23.000000 gdmty_django_users-24.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    43751 2024-05-06 03:30:51.037202 gdmty_django_users-24.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2100 2024-05-06 03:29:06.000000 gdmty_django_users-24.4.0/README.md
+-rw-rw-rw-   0        0        0     1577 2024-05-06 03:30:10.000000 gdmty_django_users-24.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-06 03:30:51.038274 gdmty_django_users-24.4.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-06 03:30:51.014047 gdmty_django_users-24.4.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-06 03:30:51.029530 gdmty_django_users-24.4.0/src/gdmty_django_users/
+-rw-rw-rw-   0        0        0     1368 2024-05-06 03:30:10.000000 gdmty_django_users-24.4.0/src/gdmty_django_users/__init__.py
+-rw-rw-rw-   0        0        0     2480 2024-03-16 06:30:23.000000 gdmty_django_users-24.4.0/src/gdmty_django_users/admin.py
+-rw-rw-rw-   0        0        0     1051 2024-03-16 06:30:23.000000 gdmty_django_users-24.4.0/src/gdmty_django_users/apps.py
+-rw-rw-rw-   0        0        0      563 2024-03-16 06:30:23.000000 gdmty_django_users-24.4.0/src/gdmty_django_users/decorators.py
+-rw-rw-rw-   0        0        0     1458 2024-03-16 06:30:23.000000 gdmty_django_users-24.4.0/src/gdmty_django_users/managers.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:30:51.035045 gdmty_django_users-24.4.0/src/gdmty_django_users/migrations/
+-rw-rw-rw-   0        0        0     3284 2024-03-17 01:44:29.000000 gdmty_django_users-24.4.0/src/gdmty_django_users/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2024-03-16 06:30:23.000000 gdmty_django_users-24.4.0/src/gdmty_django_users/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2330 2024-05-06 03:29:06.000000 gdmty_django_users-24.4.0/src/gdmty_django_users/models.py
+-rw-rw-rw-   0        0        0      945 2024-03-16 06:30:23.000000 gdmty_django_users-24.4.0/src/gdmty_django_users/permissions.py
+-rw-rw-rw-   0        0        0      889 2024-03-16 06:30:23.000000 gdmty_django_users-24.4.0/src/gdmty_django_users/serializers.py
+-rw-rw-rw-   0        0        0     1070 2024-03-17 09:01:57.000000 gdmty_django_users-24.4.0/src/gdmty_django_users/settings.py
+-rw-rw-rw-   0        0        0      913 2024-03-16 06:30:23.000000 gdmty_django_users-24.4.0/src/gdmty_django_users/tests.py
+-rw-rw-rw-   0        0        0      882 2024-05-06 03:29:06.000000 gdmty_django_users-24.4.0/src/gdmty_django_users/urls.py
+-rw-rw-rw-   0        0        0      877 2024-03-16 06:30:23.000000 gdmty_django_users-24.4.0/src/gdmty_django_users/views.py
+-rw-rw-rw-   0        0        0     4816 2024-05-06 03:29:06.000000 gdmty_django_users-24.4.0/src/gdmty_django_users/viewsets.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:30:51.036056 gdmty_django_users-24.4.0/src/gdmty_django_users.egg-info/
+-rw-rw-rw-   0        0        0    43751 2024-05-06 03:30:51.000000 gdmty_django_users-24.4.0/src/gdmty_django_users.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      813 2024-05-06 03:30:51.000000 gdmty_django_users-24.4.0/src/gdmty_django_users.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 03:30:51.000000 gdmty_django_users-24.4.0/src/gdmty_django_users.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2024-05-06 03:30:51.000000 gdmty_django_users-24.4.0/src/gdmty_django_users.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-06 03:30:51.000000 gdmty_django_users-24.4.0/src/gdmty_django_users.egg-info/top_level.txt
```

### Comparing `gdmty-django-users-24.3.1.dev7/LICENSE` & `gdmty_django_users-24.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gdmty-django-users-24.3.1.dev7/PKG-INFO` & `gdmty_django_users-24.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdmty-django-users
-Version: 24.3.1.dev7
+Version: 24.4.0
 Summary: Custom Django Rest Framework authentication backend based on email and password for users in Administration panel with reCaptcha token verification.
 Author-email: Gobierno de Monterrey <cesar.benjamin@monterrey.gob.mx>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -673,135 +673,75 @@
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django>=4.1.13
 Requires-Dist: djangorestframework
-Requires-Dist: django-auditlog
 Requires-Dist: tomli; python_version < "3.11"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 
 # gdmty-django-users
 
-Firebase backend to receive a user idToken and authenticate via Django REST Framework 
-'authentication.BaseAuthentication'. Optionally, a new local user can be created in the process. 
-This project is basen on the original work of 
-https://github.com/garyburgmann/drf-firebase-auth but with many own contribs to allow 
-get a few features that don't have the original work, but was not able to make a pull reques or 
-contribs because the use cases can be so specific and  will make breaking changes to original code
-
-## Requirements
-
-* Python 3
-* Django 4
-* Django Rest Framework 3 
-* Firebase Admin SDK
+It's an django app named `gdmty-django-users` of users implemetation that extends AbstractBaseUser for use e-mail as user. And has the option to authenticate with reCaptcha token verification.
+
+The project is maintained by Gobierno de Monterrey. You can find more about the project on
+its [homepage](https://github.com/gobiernodigitalmonterrey/gdmty-django-users) or report issues on
+the [bug tracker](https://github.com/gobiernodigitalmonterrey/gdmty-django-users/issues).
+
+## Features
+
+- Email-based User Identification: Utilizes email addresses as identifier for users.
+- Custom User Model: Extends Django's AbstractBaseUser to provide custom user functionality.
+- Modular Design: Designed as a reusable Django app for easy integration into projects.
+- Compatibility with Python 3.9 and later, and Django 4.1.13 and later.
+
 
 ## Installation
 
 ```bash
-$ pip install gdmty-drf-firebase-auth
+$ pip install gdmty-django-users
 ```
 
 ## Configuration
 
-Add the application to your project's `INSTALLED_APPS` in `settings.py`.
+Add the application to your project's `INSTALLED_APPS` in `settings.py` also add the DRF_ROUTER variable.
 
 ```python
+from rest_framework import routers
+
 INSTALLED_APPS = [
     # ...
     'gdmty_django_users',
     ...
 ]
-```
+DRF_ROUTER = routers.DefaultRouter()  # Necessary for the gdmty_django_users package
 
-### General settings
-
-In your project's `settings.py`, add this to the `REST_FRAMEWORK` configuration. Note that if you want to retain access to the browsable API for locally created users, then you will probably want to keep `rest_framework.authentication.SessionAuthentication` too.
-
-```python
-REST_FRAMEWORK = {
-  # ...
-  'DEFAULT_AUTHENTICATION_CLASSES': [
-    # ...
-    'rest_framework.authentication.SessionAuthentication',  # Optional, better to remove for production
-    'rest_framework.authentication.BasicAuthentication',  # Optional, better to remove for production
-    'gdmty_drf_firebase_auth.authentication.FirebaseAuthentication',
-  ]
-}
-```
-
-The `gdmty_drf_firebase_auth` application comes with the following settings as default, which can be overridden in your project's `settings.py` file. For convenience, most of these can be conveniently set form environment variables also. Make sure to nest them within `DEFAULT_FIREBASE_AUTH_CONFIG` as below:
-
-```python
-DEFAULT_FIREBASE_AUTH_CONFIG = {
-    # allow creation of new local user in db
-    'FIREBASE_CREATE_LOCAL_USER': True,
-    # attempt to split firebase user.display_name and set local user, first_name and last_name
-    'FIREBASE_ATTEMPT_CREATE_WITH_DISPLAY_NAME': False,
-    # Authorization header prefix, commonly JWT or Bearer (e.g. Bearer <token>)
-    'FIREBASE_AUTH_HEADER_PREFIX': 'Bearer',
-    # verify that JWT has not been revoked
-    'FIREBASE_CHECK_JWT_REVOKED': True,
-    # require that firebase user.email_verified is True
-    'FIREBASE_AUTH_EMAIL_VERIFICATION': False,
-    # function should accept firebase_admin.auth.UserRecord as argument and return str
-    'FIREBASE_USERNAME_MAPPING_FUNC': map_firebase_uid_to_username
-}
 ```
 
-You can get away with leaving all the settings as default
-
-### Firebase per-project settings
+An example to use in your 'models.py file:
 
-It is required to have GCP service accounts, the original project only supports one; the original code has been modified to allow more than one service account, To configure the service accounts, the following configuration must be added in the `settings.py` file of your project, where each element corresponds to a project and in turn, its respective service account.
+```python 
+from gdmty_django_users.models import User
 
-`BASE_DIR` is the root of your project, where manage.py lives. We assume that you have a folder called `sa` in the root of your project, and that you have placed your service account keyfiles there. You can change this to wherever you like.
+from django.db import models
 
-```python
-import os
-BASE_DIR = os.path.dirname(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
-
-...
-
-FIREBASE_AUTH_SA_KEYFILES = {
-    'project-1': os.path.join(BASE_DIR, 'sa', 'project-1-keyfile.json'),
-    'project-2': os.path.join(BASE_DIR, 'sa', 'project-2-keyfile.json')
-}
-
-FIREBASE_AUTH_PROJECTS = [
-    {'PROJECT_ID': 'project-1', 'SERVICE_ACCOUNT_KEY': FIREBASE_AUTH_SA_KEYFILES['project-1']},
-    {'PROJECT_ID': 'project-2', 'SERVICE_ACCOUNT_KEY': FIREBASE_AUTH_SA_KEYFILES['project-2']},
-]
-```
-
-Now that you have configured the application, run the migrations so that the Firebase data can be stored.
-
-```bash
-(venv) $ ./manage.py migrate gdmty_drf_firebase_auth
-```
-
-All you need to do now is have your client code handle the Firebase popup/redirect authentication flow, retrieve the idToken from the currentUser (Firebase explains this flow well in their docs: `https://firebase.google.com/docs/auth/admin/verify-id-tokens`), and then use the idToken for the user in an `Authorization` header in requests to your API.
-
-```javascript
-Bearer <token>
+class MyModel(models.Model):
+    user = User.ForeignKey(User, on_delete=User.CASCADE)
 ```
 
-Now, all is ready!
-
 ## Contributing
 
 * Please raise an issue/feature and name your branch 'feature-n' or 'issue-n', where 'n' is the issue number.
-* If you test this code with a Python version not listed above and all is well, please fork and update the README to include the Python version you used :)
+* If you test this code with a Python or package version not listed above and all is well, please fork and update the README to
+  include the Python version you used :)
 
 ## Additional Notes
 
-* This project is a fork of drf-firebase-auth, which seems no longer maintained. The original project only supports one service account, the original code has been modified to allow more than one service account.
-* The initial proposal of this project had the option of use Firebase Auth with email and password, but this option was removed to keep the project clean and simple, and focused on the use of Firebase Auth with idToken for Django REST Framework.
-* If you are looking for a project that supports Firebase Auth with email and password, you can use our side project: `gdmty-django-firebase-auth-email-password` at https://github.com/SIGAMty/gdmty-django-firebase-auth-email-password
-* I almost always setup Django with a custom user class inheriting from AbstractUser, where I switch the USERNAME_FIELD to be 'email'. This backend is set up to assign a username still anyway, but if there are any issues, please raise them and/or make a pull request to help the community!
+* This project is maintained by Gobierno de Monterrey.
+* The project's homepage is [here](https://github.com/gobiernodigitalmonterrey/gdmty-django-users) and issues can be
+  reported [here](https://github.com/gobiernodigitalmonterrey/gdmty-django-users/issues).
```

### Comparing `gdmty-django-users-24.3.1.dev7/pyproject.toml` & `gdmty_django_users-24.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gdmty-django-users"
-version = "24.3.1-dev7"
+version = "24.4.0"
 description = "Custom Django Rest Framework authentication backend based on email and password for users in Administration panel with reCaptcha token verification."
 readme = "README.md"
 authors = [{ name="Gobierno de Monterrey", email="cesar.benjamin@monterrey.gob.mx" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
     "Programming Language :: Python",
@@ -18,29 +18,28 @@
     "Framework :: Django",
     "Framework :: Django :: 4",
 ]
 keywords = ["django", "recaptcha", "users"]
 dependencies = [
     "django>=4.1.13",
     "djangorestframework",
-    "django-auditlog",
     "tomli; python_version < '3.11'",
 ]
 
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 "Homepage" = "https://github.com/gobiernodigital/gdmty-django-users"
 "Bug Tracker" = "https://github.com/gobiernodigital/gdmty-django-users/issues"
 
 [tool.bumpver]
-current_version = "24.3.1-dev7"
+current_version = "24.4.0"
 version_pattern = "MAJOR.MINOR.PATCH[-PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 commit = true
 tag = true
 push = true
```

### Comparing `gdmty-django-users-24.3.1.dev7/src/gdmty_django_users/__init__.py` & `gdmty_django_users-24.4.0/src/gdmty_django_users/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Package: gdmty_django_users
 PyPi: https://pypi.org/project/gdmty-django-users/
 License: GNU Affero General Public License v3 or later (AGPLv3+)
 
 """
 
 __title__ = "gdmty_django_users"
-__version__ = "24.3.1-dev7"
+__version__ = "24.4.0"
 __description__ = "Django module for Users models and permission adding reCAPTCHA token verification."
 __url__ = "https://github.com/SIGAMty/gdmty-django-recaptcha-enterprise"
 __author__ = "César Benjamín"
 __author_email__ = "mathereall@gmail.com"
 __license__ = "GNU Affero General Public License v3 or later (AGPLv3+)"
 __keywords__ = ["django", "users"]
 VERSION = __version__
```

### Comparing `gdmty-django-users-24.3.1.dev7/src/gdmty_django_users/admin.py` & `gdmty_django_users-24.4.0/src/gdmty_django_users/admin.py`

 * *Files identical despite different names*

### Comparing `gdmty-django-users-24.3.1.dev7/src/gdmty_django_users/apps.py` & `gdmty_django_users-24.4.0/src/gdmty_django_users/apps.py`

 * *Files identical despite different names*

### Comparing `gdmty-django-users-24.3.1.dev7/src/gdmty_django_users/decorators.py` & `gdmty_django_users-24.4.0/src/gdmty_django_users/decorators.py`

 * *Files identical despite different names*

### Comparing `gdmty-django-users-24.3.1.dev7/src/gdmty_django_users/managers.py` & `gdmty_django_users-24.4.0/src/gdmty_django_users/managers.py`

 * *Files identical despite different names*

### Comparing `gdmty-django-users-24.3.1.dev7/src/gdmty_django_users/permissions.py` & `gdmty_django_users-24.4.0/src/gdmty_django_users/permissions.py`

 * *Files identical despite different names*

### Comparing `gdmty-django-users-24.3.1.dev7/src/gdmty_django_users/serializers.py` & `gdmty_django_users-24.4.0/src/gdmty_django_users/serializers.py`

 * *Files identical despite different names*

### Comparing `gdmty-django-users-24.3.1.dev7/src/gdmty_django_users/settings.py` & `gdmty_django_users-24.4.0/src/gdmty_django_users/settings.py`

 * *Files identical despite different names*

### Comparing `gdmty-django-users-24.3.1.dev7/src/gdmty_django_users/tests.py` & `gdmty_django_users-24.4.0/src/gdmty_django_users/tests.py`

 * *Files identical despite different names*

### Comparing `gdmty-django-users-24.3.1.dev7/src/gdmty_django_users/views.py` & `gdmty_django_users-24.4.0/src/gdmty_django_users/views.py`

 * *Files identical despite different names*

### Comparing `gdmty-django-users-24.3.1.dev7/src/gdmty_django_users/viewsets.py` & `gdmty_django_users-24.4.0/src/gdmty_django_users/viewsets.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from rest_framework import viewsets
 from .models import User, Group
 from django.contrib.auth.models import Permission
 from .serializers import UserSerializer, GroupSerializer, PermissionSerializer
 from .permissions import IsAuthenticatedAndSelfOrIsStaff
 from rest_framework.response import Response
 from django_filters.rest_framework import DjangoFilterBackend
-from decorators import recaptcha_verify
+from gdmty_django_users.decorators import recaptcha_verify
 
 
 class UserViewSet(viewsets.ModelViewSet):
     filter_backends = [DjangoFilterBackend]
     filterset_fields = ['email', 'username']
 
     def get_serializer_class(self):
```

### Comparing `gdmty-django-users-24.3.1.dev7/src/gdmty_django_users.egg-info/PKG-INFO` & `gdmty_django_users-24.4.0/src/gdmty_django_users.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdmty-django-users
-Version: 24.3.1.dev7
+Version: 24.4.0
 Summary: Custom Django Rest Framework authentication backend based on email and password for users in Administration panel with reCaptcha token verification.
 Author-email: Gobierno de Monterrey <cesar.benjamin@monterrey.gob.mx>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -673,135 +673,75 @@
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django>=4.1.13
 Requires-Dist: djangorestframework
-Requires-Dist: django-auditlog
 Requires-Dist: tomli; python_version < "3.11"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 
 # gdmty-django-users
 
-Firebase backend to receive a user idToken and authenticate via Django REST Framework 
-'authentication.BaseAuthentication'. Optionally, a new local user can be created in the process. 
-This project is basen on the original work of 
-https://github.com/garyburgmann/drf-firebase-auth but with many own contribs to allow 
-get a few features that don't have the original work, but was not able to make a pull reques or 
-contribs because the use cases can be so specific and  will make breaking changes to original code
-
-## Requirements
-
-* Python 3
-* Django 4
-* Django Rest Framework 3 
-* Firebase Admin SDK
+It's an django app named `gdmty-django-users` of users implemetation that extends AbstractBaseUser for use e-mail as user. And has the option to authenticate with reCaptcha token verification.
+
+The project is maintained by Gobierno de Monterrey. You can find more about the project on
+its [homepage](https://github.com/gobiernodigitalmonterrey/gdmty-django-users) or report issues on
+the [bug tracker](https://github.com/gobiernodigitalmonterrey/gdmty-django-users/issues).
+
+## Features
+
+- Email-based User Identification: Utilizes email addresses as identifier for users.
+- Custom User Model: Extends Django's AbstractBaseUser to provide custom user functionality.
+- Modular Design: Designed as a reusable Django app for easy integration into projects.
+- Compatibility with Python 3.9 and later, and Django 4.1.13 and later.
+
 
 ## Installation
 
 ```bash
-$ pip install gdmty-drf-firebase-auth
+$ pip install gdmty-django-users
 ```
 
 ## Configuration
 
-Add the application to your project's `INSTALLED_APPS` in `settings.py`.
+Add the application to your project's `INSTALLED_APPS` in `settings.py` also add the DRF_ROUTER variable.
 
 ```python
+from rest_framework import routers
+
 INSTALLED_APPS = [
     # ...
     'gdmty_django_users',
     ...
 ]
-```
+DRF_ROUTER = routers.DefaultRouter()  # Necessary for the gdmty_django_users package
 
-### General settings
-
-In your project's `settings.py`, add this to the `REST_FRAMEWORK` configuration. Note that if you want to retain access to the browsable API for locally created users, then you will probably want to keep `rest_framework.authentication.SessionAuthentication` too.
-
-```python
-REST_FRAMEWORK = {
-  # ...
-  'DEFAULT_AUTHENTICATION_CLASSES': [
-    # ...
-    'rest_framework.authentication.SessionAuthentication',  # Optional, better to remove for production
-    'rest_framework.authentication.BasicAuthentication',  # Optional, better to remove for production
-    'gdmty_drf_firebase_auth.authentication.FirebaseAuthentication',
-  ]
-}
-```
-
-The `gdmty_drf_firebase_auth` application comes with the following settings as default, which can be overridden in your project's `settings.py` file. For convenience, most of these can be conveniently set form environment variables also. Make sure to nest them within `DEFAULT_FIREBASE_AUTH_CONFIG` as below:
-
-```python
-DEFAULT_FIREBASE_AUTH_CONFIG = {
-    # allow creation of new local user in db
-    'FIREBASE_CREATE_LOCAL_USER': True,
-    # attempt to split firebase user.display_name and set local user, first_name and last_name
-    'FIREBASE_ATTEMPT_CREATE_WITH_DISPLAY_NAME': False,
-    # Authorization header prefix, commonly JWT or Bearer (e.g. Bearer <token>)
-    'FIREBASE_AUTH_HEADER_PREFIX': 'Bearer',
-    # verify that JWT has not been revoked
-    'FIREBASE_CHECK_JWT_REVOKED': True,
-    # require that firebase user.email_verified is True
-    'FIREBASE_AUTH_EMAIL_VERIFICATION': False,
-    # function should accept firebase_admin.auth.UserRecord as argument and return str
-    'FIREBASE_USERNAME_MAPPING_FUNC': map_firebase_uid_to_username
-}
 ```
 
-You can get away with leaving all the settings as default
-
-### Firebase per-project settings
+An example to use in your 'models.py file:
 
-It is required to have GCP service accounts, the original project only supports one; the original code has been modified to allow more than one service account, To configure the service accounts, the following configuration must be added in the `settings.py` file of your project, where each element corresponds to a project and in turn, its respective service account.
+```python 
+from gdmty_django_users.models import User
 
-`BASE_DIR` is the root of your project, where manage.py lives. We assume that you have a folder called `sa` in the root of your project, and that you have placed your service account keyfiles there. You can change this to wherever you like.
+from django.db import models
 
-```python
-import os
-BASE_DIR = os.path.dirname(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
-
-...
-
-FIREBASE_AUTH_SA_KEYFILES = {
-    'project-1': os.path.join(BASE_DIR, 'sa', 'project-1-keyfile.json'),
-    'project-2': os.path.join(BASE_DIR, 'sa', 'project-2-keyfile.json')
-}
-
-FIREBASE_AUTH_PROJECTS = [
-    {'PROJECT_ID': 'project-1', 'SERVICE_ACCOUNT_KEY': FIREBASE_AUTH_SA_KEYFILES['project-1']},
-    {'PROJECT_ID': 'project-2', 'SERVICE_ACCOUNT_KEY': FIREBASE_AUTH_SA_KEYFILES['project-2']},
-]
-```
-
-Now that you have configured the application, run the migrations so that the Firebase data can be stored.
-
-```bash
-(venv) $ ./manage.py migrate gdmty_drf_firebase_auth
-```
-
-All you need to do now is have your client code handle the Firebase popup/redirect authentication flow, retrieve the idToken from the currentUser (Firebase explains this flow well in their docs: `https://firebase.google.com/docs/auth/admin/verify-id-tokens`), and then use the idToken for the user in an `Authorization` header in requests to your API.
-
-```javascript
-Bearer <token>
+class MyModel(models.Model):
+    user = User.ForeignKey(User, on_delete=User.CASCADE)
 ```
 
-Now, all is ready!
-
 ## Contributing
 
 * Please raise an issue/feature and name your branch 'feature-n' or 'issue-n', where 'n' is the issue number.
-* If you test this code with a Python version not listed above and all is well, please fork and update the README to include the Python version you used :)
+* If you test this code with a Python or package version not listed above and all is well, please fork and update the README to
+  include the Python version you used :)
 
 ## Additional Notes
 
-* This project is a fork of drf-firebase-auth, which seems no longer maintained. The original project only supports one service account, the original code has been modified to allow more than one service account.
-* The initial proposal of this project had the option of use Firebase Auth with email and password, but this option was removed to keep the project clean and simple, and focused on the use of Firebase Auth with idToken for Django REST Framework.
-* If you are looking for a project that supports Firebase Auth with email and password, you can use our side project: `gdmty-django-firebase-auth-email-password` at https://github.com/SIGAMty/gdmty-django-firebase-auth-email-password
-* I almost always setup Django with a custom user class inheriting from AbstractUser, where I switch the USERNAME_FIELD to be 'email'. This backend is set up to assign a username still anyway, but if there are any issues, please raise them and/or make a pull request to help the community!
+* This project is maintained by Gobierno de Monterrey.
+* The project's homepage is [here](https://github.com/gobiernodigitalmonterrey/gdmty-django-users) and issues can be
+  reported [here](https://github.com/gobiernodigitalmonterrey/gdmty-django-users/issues).
```

### Comparing `gdmty-django-users-24.3.1.dev7/src/gdmty_django_users.egg-info/SOURCES.txt` & `gdmty_django_users-24.4.0/src/gdmty_django_users.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -16,8 +16,9 @@
 src/gdmty_django_users/views.py
 src/gdmty_django_users/viewsets.py
 src/gdmty_django_users.egg-info/PKG-INFO
 src/gdmty_django_users.egg-info/SOURCES.txt
 src/gdmty_django_users.egg-info/dependency_links.txt
 src/gdmty_django_users.egg-info/requires.txt
 src/gdmty_django_users.egg-info/top_level.txt
+src/gdmty_django_users/migrations/0001_initial.py
 src/gdmty_django_users/migrations/__init__.py
```

