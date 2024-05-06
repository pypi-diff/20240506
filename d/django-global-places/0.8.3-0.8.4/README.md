# Comparing `tmp/django_global_places-0.8.3.tar.gz` & `tmp/django_global_places-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_global_places-0.8.3.tar", last modified: Sun Jan 21 18:53:56 2024, max compression
+gzip compressed data, was "django_global_places-0.8.4.tar", last modified: Mon May  6 09:18:17 2024, max compression
```

## Comparing `django_global_places-0.8.3.tar` & `django_global_places-0.8.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-01-21 18:53:56.238003 django_global_places-0.8.3/
--rw-rw-rw-   0        0        0       63 2024-01-20 16:42:41.000000 django_global_places-0.8.3/AUTHORS
--rw-rw-rw-   0        0        0     1128 2024-01-20 16:31:55.000000 django_global_places-0.8.3/LICENSE
--rw-rw-rw-   0        0        0     4100 2024-01-21 18:53:56.233979 django_global_places-0.8.3/PKG-INFO
--rw-rw-rw-   0        0        0     3347 2024-01-21 18:51:40.000000 django_global_places-0.8.3/README.md
-drwxrwxrwx   0        0        0        0 2024-01-21 18:53:56.183986 django_global_places-0.8.3/django_global_places/
--rw-rw-rw-   0        0        0        0 2023-12-05 17:16:34.000000 django_global_places-0.8.3/django_global_places/__init__.py
--rw-rw-rw-   0        0        0      429 2024-01-21 18:52:51.000000 django_global_places-0.8.3/django_global_places/__version__.py
--rw-rw-rw-   0        0        0     2157 2024-01-20 18:40:29.000000 django_global_places-0.8.3/django_global_places/abstract_models.py
--rw-rw-rw-   0        0        0     1217 2024-01-20 18:05:28.000000 django_global_places-0.8.3/django_global_places/admin.py
--rw-rw-rw-   0        0        0     1175 2024-01-20 18:04:01.000000 django_global_places-0.8.3/django_global_places/app_settings.py
--rw-rw-rw-   0        0        0      212 2024-01-20 18:58:22.000000 django_global_places-0.8.3/django_global_places/apps.py
-drwxrwxrwx   0        0        0        0 2024-01-21 18:53:56.206149 django_global_places-0.8.3/django_global_places/management/
--rw-rw-rw-   0        0        0        0 2023-12-05 17:16:34.000000 django_global_places-0.8.3/django_global_places/management/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-21 18:53:56.210167 django_global_places-0.8.3/django_global_places/management/commands/
--rw-rw-rw-   0        0        0        0 2023-12-05 17:16:34.000000 django_global_places-0.8.3/django_global_places/management/commands/__init__.py
--rw-rw-rw-   0        0        0    12320 2024-01-20 18:35:31.000000 django_global_places-0.8.3/django_global_places/management/commands/populate_global_places.py
-drwxrwxrwx   0        0        0        0 2024-01-21 18:53:56.210167 django_global_places-0.8.3/django_global_places/migrations/
--rw-rw-rw-   0        0        0        0 2024-01-20 18:49:36.000000 django_global_places-0.8.3/django_global_places/migrations/__init__.py
--rw-rw-rw-   0        0        0      739 2024-01-20 18:49:59.000000 django_global_places-0.8.3/django_global_places/models.py
-drwxrwxrwx   0        0        0        0 2024-01-21 18:53:56.222347 django_global_places-0.8.3/django_global_places/serializers/
--rw-rw-rw-   0        0        0        0 2023-12-05 17:16:34.000000 django_global_places-0.8.3/django_global_places/serializers/__init__.py
--rw-rw-rw-   0        0        0      676 2024-01-20 18:27:57.000000 django_global_places-0.8.3/django_global_places/serializers/cities.py
--rw-rw-rw-   0        0        0      617 2024-01-20 18:27:26.000000 django_global_places-0.8.3/django_global_places/serializers/countries.py
--rw-rw-rw-   0        0        0      702 2024-01-20 18:26:03.000000 django_global_places-0.8.3/django_global_places/serializers/states.py
--rw-rw-rw-   0        0        0      711 2024-01-20 19:06:21.000000 django_global_places-0.8.3/django_global_places/urls.py
--rw-rw-rw-   0        0        0      662 2024-01-20 18:09:57.000000 django_global_places-0.8.3/django_global_places/utils.py
-drwxrwxrwx   0        0        0        0 2024-01-21 18:53:56.230457 django_global_places-0.8.3/django_global_places/views/
--rw-rw-rw-   0        0        0        0 2023-12-05 17:16:34.000000 django_global_places-0.8.3/django_global_places/views/__init__.py
--rw-rw-rw-   0        0        0     1438 2024-01-20 18:22:34.000000 django_global_places-0.8.3/django_global_places/views/cities.py
--rw-rw-rw-   0        0        0      999 2024-01-20 18:23:47.000000 django_global_places-0.8.3/django_global_places/views/countries.py
--rw-rw-rw-   0        0        0     1412 2024-01-20 18:22:58.000000 django_global_places-0.8.3/django_global_places/views/states.py
--rw-rw-rw-   0        0        0      857 2024-01-20 18:17:44.000000 django_global_places-0.8.3/django_global_places/viewsets_utils.py
-drwxrwxrwx   0        0        0        0 2024-01-21 18:53:56.233979 django_global_places-0.8.3/django_global_places.egg-info/
--rw-rw-rw-   0        0        0     4100 2024-01-21 18:53:55.000000 django_global_places-0.8.3/django_global_places.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1168 2024-01-21 18:53:56.000000 django_global_places-0.8.3/django_global_places.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-21 18:53:55.000000 django_global_places-0.8.3/django_global_places.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-01-21 18:12:36.000000 django_global_places-0.8.3/django_global_places.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       43 2024-01-21 18:53:56.000000 django_global_places-0.8.3/django_global_places.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-01-21 18:53:56.000000 django_global_places-0.8.3/django_global_places.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-21 18:53:56.238003 django_global_places-0.8.3/setup.cfg
--rw-rw-rw-   0        0        0     1202 2024-01-21 18:41:27.000000 django_global_places-0.8.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:18:17.801533 django_global_places-0.8.4/
+-rw-rw-rw-   0        0        0       63 2024-03-30 19:07:36.000000 django_global_places-0.8.4/AUTHORS
+-rw-rw-rw-   0        0        0     1137 2024-03-30 19:22:19.000000 django_global_places-0.8.4/LICENSE
+-rw-rw-rw-   0        0        0     4009 2024-05-06 09:18:17.800023 django_global_places-0.8.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3347 2024-03-30 19:07:36.000000 django_global_places-0.8.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 09:18:17.747264 django_global_places-0.8.4/django_global_places/
+-rw-rw-rw-   0        0        0        0 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/__init__.py
+-rw-rw-rw-   0        0        0      429 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/__version__.py
+-rw-rw-rw-   0        0        0     2157 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/abstract_models.py
+-rw-rw-rw-   0        0        0     1217 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/admin.py
+-rw-rw-rw-   0        0        0     1175 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/app_settings.py
+-rw-rw-rw-   0        0        0      219 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/apps.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:18:17.783491 django_global_places-0.8.4/django_global_places/management/
+-rw-rw-rw-   0        0        0        0 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/management/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:18:17.786506 django_global_places-0.8.4/django_global_places/management/commands/
+-rw-rw-rw-   0        0        0        0 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/management/commands/__init__.py
+-rw-rw-rw-   0        0        0    12320 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/management/commands/populate_global_places.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:18:17.787510 django_global_places-0.8.4/django_global_places/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/migrations/__init__.py
+-rw-rw-rw-   0        0        0      739 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/models.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:18:17.793035 django_global_places-0.8.4/django_global_places/serializers/
+-rw-rw-rw-   0        0        0        0 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/serializers/__init__.py
+-rw-rw-rw-   0        0        0      676 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/serializers/cities.py
+-rw-rw-rw-   0        0        0      617 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/serializers/countries.py
+-rw-rw-rw-   0        0        0      702 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/serializers/states.py
+-rw-rw-rw-   0        0        0      711 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/urls.py
+-rw-rw-rw-   0        0        0      662 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:18:17.799018 django_global_places-0.8.4/django_global_places/views/
+-rw-rw-rw-   0        0        0        0 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/views/__init__.py
+-rw-rw-rw-   0        0        0     1438 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/views/cities.py
+-rw-rw-rw-   0        0        0      999 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/views/countries.py
+-rw-rw-rw-   0        0        0     1412 2024-03-30 19:07:36.000000 django_global_places-0.8.4/django_global_places/views/states.py
+-rw-rw-rw-   0        0        0      859 2024-03-30 19:10:41.000000 django_global_places-0.8.4/django_global_places/viewsets_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:18:17.780207 django_global_places-0.8.4/django_global_places.egg-info/
+-rw-rw-rw-   0        0        0     4009 2024-05-06 09:18:17.000000 django_global_places-0.8.4/django_global_places.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1168 2024-05-06 09:18:17.000000 django_global_places-0.8.4/django_global_places.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 09:18:17.000000 django_global_places-0.8.4/django_global_places.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-06 09:18:17.000000 django_global_places-0.8.4/django_global_places.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       43 2024-05-06 09:18:17.000000 django_global_places-0.8.4/django_global_places.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-05-06 09:18:17.000000 django_global_places-0.8.4/django_global_places.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 09:18:17.802550 django_global_places-0.8.4/setup.cfg
+-rw-rw-rw-   0        0        0     1202 2024-03-30 19:07:36.000000 django_global_places-0.8.4/setup.py
```

### Comparing `django_global_places-0.8.3/LICENSE` & `django_global_places-0.8.4/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2024 Luca Citta https://github.com/lucacitta/
+Copyright (c) 2024 Luca Citta Giordano https://github.com/lucacitta/
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `django_global_places-0.8.3/PKG-INFO` & `django_global_places-0.8.4/django_global_places.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: django_global_places
-Version: 0.8.3
+Name: django-global-places
+Version: 0.8.4
 Summary: Django Global Places is a simple Django app to provide a model for global places.
 Home-page: https://github.com/lucacitta/Django-GlobalPlaces
 Author: lucacitta
 Author-email: lucacitta.dev@gmail.com
 License: MIT
 Keywords: django global places
 Classifier: Framework :: Django
@@ -12,17 +12,14 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
-Requires-Dist: Django>=3.8.0
-Requires-Dist: pandas>=2.2.0
-Requires-Dist: requests>=2.30
 
 
 # Django-GlobalPlaces
 Plug and play configurations and data for countries, states and cities from all over the globe.
 
 ## Requirements
 - Django >= 3.8 *
```

### Comparing `django_global_places-0.8.3/README.md` & `django_global_places-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.3/django_global_places/abstract_models.py` & `django_global_places-0.8.4/django_global_places/abstract_models.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.3/django_global_places/admin.py` & `django_global_places-0.8.4/django_global_places/admin.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.3/django_global_places/app_settings.py` & `django_global_places-0.8.4/django_global_places/app_settings.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.3/django_global_places/management/commands/populate_global_places.py` & `django_global_places-0.8.4/django_global_places/management/commands/populate_global_places.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.3/django_global_places/models.py` & `django_global_places-0.8.4/django_global_places/models.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.3/django_global_places/serializers/cities.py` & `django_global_places-0.8.4/django_global_places/serializers/cities.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.3/django_global_places/serializers/countries.py` & `django_global_places-0.8.4/django_global_places/serializers/countries.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.3/django_global_places/serializers/states.py` & `django_global_places-0.8.4/django_global_places/serializers/states.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.3/django_global_places/urls.py` & `django_global_places-0.8.4/django_global_places/urls.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.3/django_global_places/utils.py` & `django_global_places-0.8.4/django_global_places/utils.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.3/django_global_places/views/cities.py` & `django_global_places-0.8.4/django_global_places/views/cities.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.3/django_global_places/views/countries.py` & `django_global_places-0.8.4/django_global_places/views/countries.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.3/django_global_places/views/states.py` & `django_global_places-0.8.4/django_global_places/views/states.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.3/django_global_places/viewsets_utils.py` & `django_global_places-0.8.4/django_global_places/viewsets_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         "partial_update": None,
         "destroy": None,
     }
 
     def get_serializer_class(self, *args, **kwargs):
         return self.serializers.get(self.action, None)
 
+
 class BaseReadOnlyModelViewSet(
     ViewSetPermissionMixin,
     ViewSetSerializerMixin,
     ReadOnlyModelViewSet,
 ):
     pass
```

### Comparing `django_global_places-0.8.3/django_global_places.egg-info/PKG-INFO` & `django_global_places-0.8.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_global_places
-Version: 0.8.3
+Version: 0.8.4
 Summary: Django Global Places is a simple Django app to provide a model for global places.
 Home-page: https://github.com/lucacitta/Django-GlobalPlaces
 Author: lucacitta
 Author-email: lucacitta.dev@gmail.com
 License: MIT
 Keywords: django global places
 Classifier: Framework :: Django
@@ -12,17 +12,14 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
-Requires-Dist: Django>=3.8.0
-Requires-Dist: pandas>=2.2.0
-Requires-Dist: requests>=2.30
 
 
 # Django-GlobalPlaces
 Plug and play configurations and data for countries, states and cities from all over the globe.
 
 ## Requirements
 - Django >= 3.8 *
```

### Comparing `django_global_places-0.8.3/django_global_places.egg-info/SOURCES.txt` & `django_global_places-0.8.4/django_global_places.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.3/setup.py` & `django_global_places-0.8.4/setup.py`

 * *Files identical despite different names*

