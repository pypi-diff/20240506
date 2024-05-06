# Comparing `tmp/django-dynamic-structure-0.0.8.tar.gz` & `tmp/django-dynamic-structure-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-dynamic-structure-0.0.8.tar", last modified: Mon Sep 12 17:59:15 2016, max compression
+gzip compressed data, was "dist/django-dynamic-structure-0.0.9.tar", last modified: Tue Sep 13 07:36:31 2016, max compression
```

## Comparing `django-dynamic-structure-0.0.8.tar` & `django-dynamic-structure-0.0.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 telminov  (1000) scanner    (109)        0 2016-09-12 17:59:15.000000 django-dynamic-structure-0.0.8/
--rw-r--r--   0 telminov  (1000) scanner    (109)      305 2016-08-31 15:02:11.000000 django-dynamic-structure-0.0.8/README.md
-drwxr-xr-x   0 telminov  (1000) scanner    (109)        0 2016-09-12 17:59:15.000000 django-dynamic-structure-0.0.8/dyn_struct/
--rw-r--r--   0 telminov  (1000) scanner    (109)     4052 2016-09-12 17:44:22.000000 django-dynamic-structure-0.0.8/dyn_struct/forms.py
-drwxr-xr-x   0 telminov  (1000) scanner    (109)        0 2016-09-12 17:59:15.000000 django-dynamic-structure-0.0.8/dyn_struct/templatetags/
--rw-r--r--   0 telminov  (1000) scanner    (109)        0 2016-08-31 15:05:30.000000 django-dynamic-structure-0.0.8/dyn_struct/templatetags/__init__.py
--rw-r--r--   0 telminov  (1000) scanner    (109)      483 2016-09-07 08:46:55.000000 django-dynamic-structure-0.0.8/dyn_struct/templatetags/dyn_struct.py
-drwxr-xr-x   0 telminov  (1000) scanner    (109)        0 2016-09-12 17:59:15.000000 django-dynamic-structure-0.0.8/dyn_struct/templates/
-drwxr-xr-x   0 telminov  (1000) scanner    (109)        0 2016-09-12 17:59:15.000000 django-dynamic-structure-0.0.8/dyn_struct/templates/dyn_struct/
--rw-r--r--   0 telminov  (1000) scanner    (109)      146 2016-09-07 07:23:38.000000 django-dynamic-structure-0.0.8/dyn_struct/templates/dyn_struct/render_struct_field_bootstrap3.html
--rw-r--r--   0 telminov  (1000) scanner    (109)      623 2016-09-07 07:40:54.000000 django-dynamic-structure-0.0.8/dyn_struct/templates/dyn_struct/render_struct_field_bootstrap2.html
--rw-r--r--   0 telminov  (1000) scanner    (109)     1001 2016-09-08 01:16:01.000000 django-dynamic-structure-0.0.8/dyn_struct/templates/dyn_struct/render_struct.html
--rw-r--r--   0 telminov  (1000) scanner    (109)        0 2016-09-04 14:27:22.000000 django-dynamic-structure-0.0.8/dyn_struct/__init__.py
--rw-r--r--   0 telminov  (1000) scanner    (109)     1383 2016-09-06 08:48:46.000000 django-dynamic-structure-0.0.8/dyn_struct/datatools.py
--rw-r--r--   0 telminov  (1000) scanner    (109)      111 2016-08-31 16:38:17.000000 django-dynamic-structure-0.0.8/dyn_struct/exceptions.py
-drwxr-xr-x   0 telminov  (1000) scanner    (109)        0 2016-09-12 17:59:15.000000 django-dynamic-structure-0.0.8/dyn_struct/migrations/
--rw-r--r--   0 telminov  (1000) scanner    (109)      615 2016-08-31 19:38:55.000000 django-dynamic-structure-0.0.8/dyn_struct/migrations/0002_auto_20160831_2238.py
--rw-r--r--   0 telminov  (1000) scanner    (109)     4800 2016-08-31 19:02:52.000000 django-dynamic-structure-0.0.8/dyn_struct/migrations/0001_initial.py
--rw-r--r--   0 telminov  (1000) scanner    (109)        0 2016-08-31 19:02:52.000000 django-dynamic-structure-0.0.8/dyn_struct/migrations/__init__.py
--rw-r--r--   0 telminov  (1000) scanner    (109)     1982 2016-09-12 14:52:56.000000 django-dynamic-structure-0.0.8/dyn_struct/migrations/0004_auto_20160912_1752.py
--rw-r--r--   0 telminov  (1000) scanner    (109)     1517 2016-09-06 09:55:26.000000 django-dynamic-structure-0.0.8/dyn_struct/migrations/0003_auto_20160906_1255.py
--rw-r--r--   0 telminov  (1000) scanner    (109)      962 2016-09-12 16:31:46.000000 django-dynamic-structure-0.0.8/dyn_struct/admin.py
-drwxr-xr-x   0 telminov  (1000) scanner    (109)        0 2016-09-12 17:59:15.000000 django-dynamic-structure-0.0.8/dyn_struct/db/
--rw-r--r--   0 telminov  (1000) scanner    (109)      328 2016-09-04 15:39:57.000000 django-dynamic-structure-0.0.8/dyn_struct/db/fields.py
--rw-r--r--   0 telminov  (1000) scanner    (109)     7326 2016-09-12 16:22:16.000000 django-dynamic-structure-0.0.8/dyn_struct/db/models.py
--rw-r--r--   0 telminov  (1000) scanner    (109)        0 2016-09-04 14:27:22.000000 django-dynamic-structure-0.0.8/dyn_struct/db/__init__.py
--rw-r--r--   0 telminov  (1000) scanner    (109)      787 2016-09-04 14:55:37.000000 django-dynamic-structure-0.0.8/dyn_struct/db/validators.py
--rw-r--r--   0 telminov  (1000) scanner    (109)       59 2016-09-12 17:59:15.000000 django-dynamic-structure-0.0.8/setup.cfg
-drwxr-xr-x   0 telminov  (1000) scanner    (109)        0 2016-09-12 17:59:15.000000 django-dynamic-structure-0.0.8/django_dynamic_structure.egg-info/
--rw-r--r--   0 telminov  (1000) scanner    (109)       18 2016-09-12 17:59:13.000000 django-dynamic-structure-0.0.8/django_dynamic_structure.egg-info/requires.txt
--rw-r--r--   0 telminov  (1000) scanner    (109)       11 2016-09-12 17:59:13.000000 django-dynamic-structure-0.0.8/django_dynamic_structure.egg-info/top_level.txt
--rw-r--r--   0 telminov  (1000) scanner    (109)      962 2016-09-12 17:59:15.000000 django-dynamic-structure-0.0.8/django_dynamic_structure.egg-info/SOURCES.txt
--rw-r--r--   0 telminov  (1000) scanner    (109)      362 2016-09-12 17:59:13.000000 django-dynamic-structure-0.0.8/django_dynamic_structure.egg-info/PKG-INFO
--rw-r--r--   0 telminov  (1000) scanner    (109)        1 2016-09-12 17:59:13.000000 django-dynamic-structure-0.0.8/django_dynamic_structure.egg-info/dependency_links.txt
--rw-r--r--   0 telminov  (1000) scanner    (109)       57 2016-09-04 14:48:57.000000 django-dynamic-structure-0.0.8/.gitignore
--rw-r--r--   0 telminov  (1000) scanner    (109)      362 2016-09-12 17:59:15.000000 django-dynamic-structure-0.0.8/PKG-INFO
--rw-r--r--   0 telminov  (1000) scanner    (109)      588 2016-09-12 17:58:16.000000 django-dynamic-structure-0.0.8/setup.py
+drwxr-xr-x   0 telminov  (1000) scanner    (109)        0 2016-09-13 07:36:31.000000 django-dynamic-structure-0.0.9/
+-rw-r--r--   0 telminov  (1000) scanner    (109)      305 2016-08-31 15:02:11.000000 django-dynamic-structure-0.0.9/README.md
+drwxr-xr-x   0 telminov  (1000) scanner    (109)        0 2016-09-13 07:36:31.000000 django-dynamic-structure-0.0.9/dyn_struct/
+-rw-r--r--   0 telminov  (1000) scanner    (109)     4052 2016-09-12 17:44:22.000000 django-dynamic-structure-0.0.9/dyn_struct/forms.py
+drwxr-xr-x   0 telminov  (1000) scanner    (109)        0 2016-09-13 07:36:31.000000 django-dynamic-structure-0.0.9/dyn_struct/templatetags/
+-rw-r--r--   0 telminov  (1000) scanner    (109)        0 2016-08-31 15:05:30.000000 django-dynamic-structure-0.0.9/dyn_struct/templatetags/__init__.py
+-rw-r--r--   0 telminov  (1000) scanner    (109)      483 2016-09-07 08:46:55.000000 django-dynamic-structure-0.0.9/dyn_struct/templatetags/dyn_struct.py
+drwxr-xr-x   0 telminov  (1000) scanner    (109)        0 2016-09-13 07:36:31.000000 django-dynamic-structure-0.0.9/dyn_struct/templates/
+drwxr-xr-x   0 telminov  (1000) scanner    (109)        0 2016-09-13 07:36:31.000000 django-dynamic-structure-0.0.9/dyn_struct/templates/dyn_struct/
+-rw-r--r--   0 telminov  (1000) scanner    (109)      146 2016-09-07 07:23:38.000000 django-dynamic-structure-0.0.9/dyn_struct/templates/dyn_struct/render_struct_field_bootstrap3.html
+-rw-r--r--   0 telminov  (1000) scanner    (109)      623 2016-09-07 07:40:54.000000 django-dynamic-structure-0.0.9/dyn_struct/templates/dyn_struct/render_struct_field_bootstrap2.html
+-rw-r--r--   0 telminov  (1000) scanner    (109)     1001 2016-09-08 01:16:01.000000 django-dynamic-structure-0.0.9/dyn_struct/templates/dyn_struct/render_struct.html
+-rw-r--r--   0 telminov  (1000) scanner    (109)        0 2016-09-04 14:27:22.000000 django-dynamic-structure-0.0.9/dyn_struct/__init__.py
+-rw-r--r--   0 telminov  (1000) scanner    (109)     1383 2016-09-06 08:48:46.000000 django-dynamic-structure-0.0.9/dyn_struct/datatools.py
+-rw-r--r--   0 telminov  (1000) scanner    (109)      111 2016-08-31 16:38:17.000000 django-dynamic-structure-0.0.9/dyn_struct/exceptions.py
+drwxr-xr-x   0 telminov  (1000) scanner    (109)        0 2016-09-13 07:36:31.000000 django-dynamic-structure-0.0.9/dyn_struct/migrations/
+-rw-r--r--   0 telminov  (1000) scanner    (109)      615 2016-08-31 19:38:55.000000 django-dynamic-structure-0.0.9/dyn_struct/migrations/0002_auto_20160831_2238.py
+-rw-r--r--   0 telminov  (1000) scanner    (109)     4800 2016-08-31 19:02:52.000000 django-dynamic-structure-0.0.9/dyn_struct/migrations/0001_initial.py
+-rw-r--r--   0 telminov  (1000) scanner    (109)        0 2016-08-31 19:02:52.000000 django-dynamic-structure-0.0.9/dyn_struct/migrations/__init__.py
+-rw-r--r--   0 telminov  (1000) scanner    (109)     1982 2016-09-12 14:52:56.000000 django-dynamic-structure-0.0.9/dyn_struct/migrations/0004_auto_20160912_1752.py
+-rw-r--r--   0 telminov  (1000) scanner    (109)     1517 2016-09-06 09:55:26.000000 django-dynamic-structure-0.0.9/dyn_struct/migrations/0003_auto_20160906_1255.py
+-rw-r--r--   0 telminov  (1000) scanner    (109)      962 2016-09-12 16:31:46.000000 django-dynamic-structure-0.0.9/dyn_struct/admin.py
+drwxr-xr-x   0 telminov  (1000) scanner    (109)        0 2016-09-13 07:36:31.000000 django-dynamic-structure-0.0.9/dyn_struct/db/
+-rw-r--r--   0 telminov  (1000) scanner    (109)      328 2016-09-04 15:39:57.000000 django-dynamic-structure-0.0.9/dyn_struct/db/fields.py
+-rw-r--r--   0 telminov  (1000) scanner    (109)     7326 2016-09-12 16:22:16.000000 django-dynamic-structure-0.0.9/dyn_struct/db/models.py
+-rw-r--r--   0 telminov  (1000) scanner    (109)        0 2016-09-04 14:27:22.000000 django-dynamic-structure-0.0.9/dyn_struct/db/__init__.py
+-rw-r--r--   0 telminov  (1000) scanner    (109)      787 2016-09-04 14:55:37.000000 django-dynamic-structure-0.0.9/dyn_struct/db/validators.py
+-rw-r--r--   0 telminov  (1000) scanner    (109)       59 2016-09-13 07:36:31.000000 django-dynamic-structure-0.0.9/setup.cfg
+drwxr-xr-x   0 telminov  (1000) scanner    (109)        0 2016-09-13 07:36:31.000000 django-dynamic-structure-0.0.9/django_dynamic_structure.egg-info/
+-rw-r--r--   0 telminov  (1000) scanner    (109)       26 2016-09-13 07:36:28.000000 django-dynamic-structure-0.0.9/django_dynamic_structure.egg-info/requires.txt
+-rw-r--r--   0 telminov  (1000) scanner    (109)       11 2016-09-13 07:36:28.000000 django-dynamic-structure-0.0.9/django_dynamic_structure.egg-info/top_level.txt
+-rw-r--r--   0 telminov  (1000) scanner    (109)      962 2016-09-13 07:36:31.000000 django-dynamic-structure-0.0.9/django_dynamic_structure.egg-info/SOURCES.txt
+-rw-r--r--   0 telminov  (1000) scanner    (109)      362 2016-09-13 07:36:28.000000 django-dynamic-structure-0.0.9/django_dynamic_structure.egg-info/PKG-INFO
+-rw-r--r--   0 telminov  (1000) scanner    (109)        1 2016-09-13 07:36:28.000000 django-dynamic-structure-0.0.9/django_dynamic_structure.egg-info/dependency_links.txt
+-rw-r--r--   0 telminov  (1000) scanner    (109)       57 2016-09-04 14:48:57.000000 django-dynamic-structure-0.0.9/.gitignore
+-rw-r--r--   0 telminov  (1000) scanner    (109)      362 2016-09-13 07:36:31.000000 django-dynamic-structure-0.0.9/PKG-INFO
+-rw-r--r--   0 telminov  (1000) scanner    (109)      596 2016-09-13 07:36:07.000000 django-dynamic-structure-0.0.9/setup.py
```

### Comparing `django-dynamic-structure-0.0.8/dyn_struct/forms.py` & `django-dynamic-structure-0.0.9/dyn_struct/forms.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-structure-0.0.8/dyn_struct/templates/dyn_struct/render_struct_field_bootstrap2.html` & `django-dynamic-structure-0.0.9/dyn_struct/templates/dyn_struct/render_struct_field_bootstrap2.html`

 * *Files identical despite different names*

### Comparing `django-dynamic-structure-0.0.8/dyn_struct/templates/dyn_struct/render_struct.html` & `django-dynamic-structure-0.0.9/dyn_struct/templates/dyn_struct/render_struct.html`

 * *Files identical despite different names*

### Comparing `django-dynamic-structure-0.0.8/dyn_struct/datatools.py` & `django-dynamic-structure-0.0.9/dyn_struct/datatools.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-structure-0.0.8/dyn_struct/migrations/0002_auto_20160831_2238.py` & `django-dynamic-structure-0.0.9/dyn_struct/migrations/0002_auto_20160831_2238.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-structure-0.0.8/dyn_struct/migrations/0001_initial.py` & `django-dynamic-structure-0.0.9/dyn_struct/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-structure-0.0.8/dyn_struct/migrations/0004_auto_20160912_1752.py` & `django-dynamic-structure-0.0.9/dyn_struct/migrations/0004_auto_20160912_1752.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-structure-0.0.8/dyn_struct/migrations/0003_auto_20160906_1255.py` & `django-dynamic-structure-0.0.9/dyn_struct/migrations/0003_auto_20160906_1255.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-structure-0.0.8/dyn_struct/admin.py` & `django-dynamic-structure-0.0.9/dyn_struct/admin.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-structure-0.0.8/dyn_struct/db/models.py` & `django-dynamic-structure-0.0.9/dyn_struct/db/models.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-structure-0.0.8/dyn_struct/db/validators.py` & `django-dynamic-structure-0.0.9/dyn_struct/db/validators.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-structure-0.0.8/django_dynamic_structure.egg-info/SOURCES.txt` & `django-dynamic-structure-0.0.9/django_dynamic_structure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-dynamic-structure-0.0.8/setup.py` & `django-dynamic-structure-0.0.9/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # coding: utf-8
 # python setup.py sdist register bdist_egg upload
 from setuptools import setup, find_packages
 
 setup(
     name='django-dynamic-structure',
-    version='0.0.8',
+    version='0.0.9',
     description='Dynamical django model structure. For example, for user customized medical specialist protocols.',
     author='Nick Sablukov',
     author_email='dessanndes@gmailcom',
     url='https://github.com/NickSablukov/django-dynamic-structure',
     include_package_data=True,
     packages=find_packages(),
     license='The MIT License',
     install_requires=[
-        'django', 'six', 'swutils',
+        'django', 'six', 'sw-python-utils',
     ],
 )
```

