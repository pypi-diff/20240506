# Comparing `tmp/django-societies-0.1.6.tar.gz` & `tmp/django-societies-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-societies-0.1.6.tar", last modified: Tue Mar  5 17:19:35 2024, max compression
+gzip compressed data, was "django-societies-0.1.7.tar", last modified: Sun Apr 21 14:54:12 2024, max compression
```

## Comparing `django-societies-0.1.6.tar` & `django-societies-0.1.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)        0 2024-03-05 17:19:35.075988 django-societies-0.1.6/
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)    35149 2023-12-14 11:32:43.000000 django-societies-0.1.6/LICENSE
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       60 2023-12-14 11:32:43.000000 django-societies-0.1.6/MANIFEST.in
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     1604 2024-03-05 17:19:35.074988 django-societies-0.1.6/PKG-INFO
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      517 2023-12-14 11:32:43.000000 django-societies-0.1.6/README.rst
-drwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)        0 2024-03-05 17:19:35.074988 django-societies-0.1.6/django_societies.egg-info/
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     1604 2024-03-05 17:19:34.000000 django-societies-0.1.6/django_societies.egg-info/PKG-INFO
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      434 2024-03-05 17:19:34.000000 django-societies-0.1.6/django_societies.egg-info/SOURCES.txt
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)        1 2024-03-05 17:19:34.000000 django-societies-0.1.6/django_societies.egg-info/dependency_links.txt
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       12 2024-03-05 17:19:34.000000 django-societies-0.1.6/django_societies.egg-info/requires.txt
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       10 2024-03-05 17:19:34.000000 django-societies-0.1.6/django_societies.egg-info/top_level.txt
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       90 2023-12-14 11:32:43.000000 django-societies-0.1.6/pyproject.toml
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     1059 2024-03-05 17:19:35.076989 django-societies-0.1.6/setup.cfg
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       38 2023-12-14 11:32:43.000000 django-societies-0.1.6/setup.py
-drwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)        0 2024-03-05 17:19:35.073989 django-societies-0.1.6/societies/
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)        0 2023-12-14 11:32:43.000000 django-societies-0.1.6/societies/__init__.py
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       63 2023-12-14 11:32:43.000000 django-societies-0.1.6/societies/admin.py
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      150 2023-12-14 11:32:43.000000 django-societies-0.1.6/societies/apps.py
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)    10049 2024-03-05 17:13:35.000000 django-societies-0.1.6/societies/choices.py
-drwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)        0 2024-03-05 17:19:35.073989 django-societies-0.1.6/societies/migrations/
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)        0 2023-12-14 11:32:43.000000 django-societies-0.1.6/societies/migrations/__init__.py
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     4650 2024-03-04 05:29:13.000000 django-societies-0.1.6/societies/models.py
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       60 2023-12-14 11:32:43.000000 django-societies-0.1.6/societies/tests.py
--rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       63 2023-12-14 11:32:43.000000 django-societies-0.1.6/societies/views.py
+drwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)        0 2024-04-21 14:54:12.286090 django-societies-0.1.7/
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)    35149 2023-12-14 11:32:43.000000 django-societies-0.1.7/LICENSE
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       60 2023-12-14 11:32:43.000000 django-societies-0.1.7/MANIFEST.in
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     1604 2024-04-21 14:54:12.286090 django-societies-0.1.7/PKG-INFO
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      517 2023-12-14 11:32:43.000000 django-societies-0.1.7/README.rst
+drwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)        0 2024-04-21 14:54:12.286090 django-societies-0.1.7/django_societies.egg-info/
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     1604 2024-04-21 14:54:12.000000 django-societies-0.1.7/django_societies.egg-info/PKG-INFO
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      434 2024-04-21 14:54:12.000000 django-societies-0.1.7/django_societies.egg-info/SOURCES.txt
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)        1 2024-04-21 14:54:12.000000 django-societies-0.1.7/django_societies.egg-info/dependency_links.txt
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       12 2024-04-21 14:54:12.000000 django-societies-0.1.7/django_societies.egg-info/requires.txt
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       10 2024-04-21 14:54:12.000000 django-societies-0.1.7/django_societies.egg-info/top_level.txt
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       90 2023-12-14 11:32:43.000000 django-societies-0.1.7/pyproject.toml
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     1059 2024-04-21 14:54:12.287090 django-societies-0.1.7/setup.cfg
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       38 2023-12-14 11:32:43.000000 django-societies-0.1.7/setup.py
+drwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)        0 2024-04-21 14:54:12.285090 django-societies-0.1.7/societies/
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)        0 2023-12-14 11:32:43.000000 django-societies-0.1.7/societies/__init__.py
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       63 2023-12-14 11:32:43.000000 django-societies-0.1.7/societies/admin.py
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)      150 2023-12-14 11:32:43.000000 django-societies-0.1.7/societies/apps.py
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)    10049 2024-03-05 17:13:35.000000 django-societies-0.1.7/societies/choices.py
+drwxr-xr-x   0 schemefusion  (7515) schemefusion  (7515)        0 2024-04-21 14:54:12.286090 django-societies-0.1.7/societies/migrations/
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)        0 2023-12-14 11:32:43.000000 django-societies-0.1.7/societies/migrations/__init__.py
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)     4659 2024-04-21 14:52:24.000000 django-societies-0.1.7/societies/models.py
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       60 2023-12-14 11:32:43.000000 django-societies-0.1.7/societies/tests.py
+-rw-r--r--   0 schemefusion  (7515) schemefusion  (7515)       63 2023-12-14 11:32:43.000000 django-societies-0.1.7/societies/views.py
```

### Comparing `django-societies-0.1.6/LICENSE` & `django-societies-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django-societies-0.1.6/PKG-INFO` & `django-societies-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-societies
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Django module that provides a collection of abstract models for handling data associated with people, groups, organizations, places, events and means of communication.
 Home-page: https://www.schemefusion.com/
 Author: Onyeibo Oku
 Author-email: onyeibo@schemefusion.com
 License: GPLv3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-societies-0.1.6/README.rst` & `django-societies-0.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `django-societies-0.1.6/django_societies.egg-info/PKG-INFO` & `django-societies-0.1.7/django_societies.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-societies
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Django module that provides a collection of abstract models for handling data associated with people, groups, organizations, places, events and means of communication.
 Home-page: https://www.schemefusion.com/
 Author: Onyeibo Oku
 Author-email: onyeibo@schemefusion.com
 License: GPLv3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-societies-0.1.6/setup.cfg` & `django-societies-0.1.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-societies
-version = 0.1.6
+version = 0.1.7
 description = A Django module that provides a collection of abstract models for handling data associated with people, groups, organizations, places, events and means of communication.
 long_description = file: README.rst
 url = https://www.schemefusion.com/
 author = Onyeibo Oku
 author_email = onyeibo@schemefusion.com
 license = GPLv3
 classifiers =
```

### Comparing `django-societies-0.1.6/societies/choices.py` & `django-societies-0.1.7/societies/choices.py`

 * *Files identical despite different names*

### Comparing `django-societies-0.1.6/societies/models.py` & `django-societies-0.1.7/societies/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,16 @@
     suffix = models.CharField(blank=True, choices=choices.HONORIFICS, null=True)
 
     def __str__(self):
         """Print String for this Model"""
 
         return self.last_name
 
-    def full_name(self): 
+    @property
+    def name(self): 
         """Return the fullname of this Person""" 
         
         prefix = self.prefix if self.prefix else ""
         middle_name = self.middle_name if self.middle_name else ""
         return f"{prefix} {self.last_name}, {self.first_name} {middle_name}" 
 
     class Meta:
```

