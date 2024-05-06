# Comparing `tmp/django_activitylog_jwt-1.0.1.tar.gz` & `tmp/django_activitylog_jwt-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_activitylog_jwt-1.0.1.tar", last modified: Sun May  5 14:54:47 2024, max compression
+gzip compressed data, was "django_activitylog_jwt-1.0.2.tar", last modified: Mon May  6 16:07:55 2024, max compression
```

## Comparing `django_activitylog_jwt-1.0.1.tar` & `django_activitylog_jwt-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:54:47.347955 django_activitylog_jwt-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-05-05 14:54:47.347955 django_activitylog_jwt-1.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:54:47.347955 django_activitylog_jwt-1.0.1/activitylog/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 14:54:34.000000 django_activitylog_jwt-1.0.1/activitylog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-05-05 14:54:34.000000 django_activitylog_jwt-1.0.1/activitylog/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-05 14:54:34.000000 django_activitylog_jwt-1.0.1/activitylog/admin_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-05 14:54:34.000000 django_activitylog_jwt-1.0.1/activitylog/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-05 14:54:34.000000 django_activitylog_jwt-1.0.1/activitylog/backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-05-05 14:54:34.000000 django_activitylog_jwt-1.0.1/activitylog/crudhistory_admin_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-05-05 14:54:34.000000 django_activitylog_jwt-1.0.1/activitylog/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7882 2024-05-05 14:54:34.000000 django_activitylog_jwt-1.0.1/activitylog/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-05 14:54:34.000000 django_activitylog_jwt-1.0.1/activitylog/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-05 14:54:34.000000 django_activitylog_jwt-1.0.1/activitylog/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:54:47.347955 django_activitylog_jwt-1.0.1/django_activitylog_jwt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-05-05 14:54:47.000000 django_activitylog_jwt-1.0.1/django_activitylog_jwt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-05 14:54:47.000000 django_activitylog_jwt-1.0.1/django_activitylog_jwt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 14:54:47.000000 django_activitylog_jwt-1.0.1/django_activitylog_jwt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-05 14:54:47.000000 django_activitylog_jwt-1.0.1/django_activitylog_jwt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-05 14:54:47.000000 django_activitylog_jwt-1.0.1/django_activitylog_jwt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 14:54:47.347955 django_activitylog_jwt-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-05 14:54:34.000000 django_activitylog_jwt-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:55.683251 django_activitylog_jwt-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-05-06 16:07:55.683251 django_activitylog_jwt-1.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:55.679251 django_activitylog_jwt-1.0.2/activitylog/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:41.000000 django_activitylog_jwt-1.0.2/activitylog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-05-06 16:07:41.000000 django_activitylog_jwt-1.0.2/activitylog/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-06 16:07:41.000000 django_activitylog_jwt-1.0.2/activitylog/admin_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-06 16:07:41.000000 django_activitylog_jwt-1.0.2/activitylog/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-06 16:07:41.000000 django_activitylog_jwt-1.0.2/activitylog/backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-05-06 16:07:41.000000 django_activitylog_jwt-1.0.2/activitylog/crudhistory_admin_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-05-06 16:07:42.000000 django_activitylog_jwt-1.0.2/activitylog/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7882 2024-05-06 16:07:42.000000 django_activitylog_jwt-1.0.2/activitylog/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-06 16:07:42.000000 django_activitylog_jwt-1.0.2/activitylog/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-06 16:07:42.000000 django_activitylog_jwt-1.0.2/activitylog/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:55.683251 django_activitylog_jwt-1.0.2/django_activitylog_jwt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-05-06 16:07:55.000000 django_activitylog_jwt-1.0.2/django_activitylog_jwt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-06 16:07:55.000000 django_activitylog_jwt-1.0.2/django_activitylog_jwt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:07:55.000000 django_activitylog_jwt-1.0.2/django_activitylog_jwt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-06 16:07:55.000000 django_activitylog_jwt-1.0.2/django_activitylog_jwt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-06 16:07:55.000000 django_activitylog_jwt-1.0.2/django_activitylog_jwt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 16:07:55.683251 django_activitylog_jwt-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-06 16:07:42.000000 django_activitylog_jwt-1.0.2/setup.py
```

### Comparing `django_activitylog_jwt-1.0.1/PKG-INFO` & `django_activitylog_jwt-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-activitylog-jwt
-Version: 1.0.1
+Version: 1.0.2
 Summary: Get started with django-activitylog-jwt today to bolster the security and audit capabilities of your Django application while leveraging the power of JWT authentication.
 Home-page: https://github.com/knand4930/django-activitylog-jwt.git
 Author: Nand Kishore
 Author-email: knand4930@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django_activitylog_jwt-1.0.1/activitylog/admin.py` & `django_activitylog_jwt-1.0.2/activitylog/admin.py`

 * *Files identical despite different names*

### Comparing `django_activitylog_jwt-1.0.1/activitylog/admin_helpers.py` & `django_activitylog_jwt-1.0.2/activitylog/admin_helpers.py`

 * *Files identical despite different names*

### Comparing `django_activitylog_jwt-1.0.1/activitylog/crudhistory_admin_mixin.py` & `django_activitylog_jwt-1.0.2/activitylog/crudhistory_admin_mixin.py`

 * *Files identical despite different names*

### Comparing `django_activitylog_jwt-1.0.1/activitylog/models.py` & `django_activitylog_jwt-1.0.2/activitylog/models.py`

 * *Files identical despite different names*

### Comparing `django_activitylog_jwt-1.0.1/activitylog/settings.py` & `django_activitylog_jwt-1.0.2/activitylog/settings.py`

 * *Files identical despite different names*

### Comparing `django_activitylog_jwt-1.0.1/activitylog/utils.py` & `django_activitylog_jwt-1.0.2/activitylog/utils.py`

 * *Files identical despite different names*

### Comparing `django_activitylog_jwt-1.0.1/django_activitylog_jwt.egg-info/PKG-INFO` & `django_activitylog_jwt-1.0.2/django_activitylog_jwt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-activitylog-jwt
-Version: 1.0.1
+Version: 1.0.2
 Summary: Get started with django-activitylog-jwt today to bolster the security and audit capabilities of your Django application while leveraging the power of JWT authentication.
 Home-page: https://github.com/knand4930/django-activitylog-jwt.git
 Author: Nand Kishore
 Author-email: knand4930@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django_activitylog_jwt-1.0.1/setup.py` & `django_activitylog_jwt-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("readME.md", "r") as f:
     description = f.read()
 
 setup(
     name='django-activitylog-jwt',
-    version='1.0.1',
+    version='1.0.2',
     description='Get started with django-activitylog-jwt today to bolster the security and audit capabilities of your '
                 'Django application while leveraging the power of JWT authentication.',
     author='Nand Kishore',
     author_email='knand4930@gmail.com',
     license='MIT',
     url='https://github.com/knand4930/django-activitylog-jwt.git',
     packages=['activitylog'],
```

