# Comparing `tmp/django-pikpdf-0.3.4.tar.gz` & `tmp/django-pikpdf-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pikpdf-0.3.4.tar", last modified: Sat Feb  3 16:32:54 2024, max compression
+gzip compressed data, was "django-pikpdf-0.3.5.tar", last modified: Mon May  6 11:01:05 2024, max compression
```

## Comparing `django-pikpdf-0.3.4.tar` & `django-pikpdf-0.3.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-03 16:32:54.216406 django-pikpdf-0.3.4/
--rw-r--r--   0 root         (0) root         (0)      996 2024-02-03 15:32:43.000000 django-pikpdf-0.3.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      205 2024-02-03 15:32:43.000000 django-pikpdf-0.3.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2648 2024-02-03 16:32:54.216406 django-pikpdf-0.3.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1679 2024-02-03 16:32:48.000000 django-pikpdf-0.3.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-03 16:32:54.216406 django-pikpdf-0.3.4/django_pikpdf/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-03 15:32:43.000000 django-pikpdf-0.3.4/django_pikpdf/__init__.py
--rw-r--r--   0 root         (0) root         (0)       63 2024-02-03 15:32:43.000000 django-pikpdf-0.3.4/django_pikpdf/admin.py
--rw-r--r--   0 root         (0) root         (0)      172 2024-02-03 15:32:43.000000 django-pikpdf-0.3.4/django_pikpdf/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-03 16:32:54.216406 django-pikpdf-0.3.4/django_pikpdf/controllers/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-03 15:32:43.000000 django-pikpdf-0.3.4/django_pikpdf/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)      792 2024-02-03 15:32:43.000000 django-pikpdf-0.3.4/django_pikpdf/controllers/api.py
--rw-r--r--   0 root         (0) root         (0)      396 2024-02-03 16:29:33.000000 django-pikpdf-0.3.4/django_pikpdf/controllers/html_transformation.py
--rw-r--r--   0 root         (0) root         (0)     2151 2024-02-03 15:32:43.000000 django-pikpdf-0.3.4/django_pikpdf/controllers/validators.py
--rw-r--r--   0 root         (0) root         (0)     1355 2024-02-03 15:32:43.000000 django-pikpdf-0.3.4/django_pikpdf/converter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-03 16:32:54.216406 django-pikpdf-0.3.4/django_pikpdf/migrations/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-03 15:32:43.000000 django-pikpdf-0.3.4/django_pikpdf/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)       57 2024-02-03 15:32:43.000000 django-pikpdf-0.3.4/django_pikpdf/models.py
--rw-r--r--   0 root         (0) root         (0)       63 2024-02-03 15:32:43.000000 django-pikpdf-0.3.4/django_pikpdf/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-03 16:32:54.216406 django-pikpdf-0.3.4/django_pikpdf.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2648 2024-02-03 16:32:54.000000 django-pikpdf-0.3.4/django_pikpdf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      589 2024-02-03 16:32:54.000000 django-pikpdf-0.3.4/django_pikpdf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-03 16:32:54.000000 django-pikpdf-0.3.4/django_pikpdf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2024-02-03 16:32:54.000000 django-pikpdf-0.3.4/django_pikpdf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-02-03 16:32:54.000000 django-pikpdf-0.3.4/django_pikpdf.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2024-02-03 15:32:43.000000 django-pikpdf-0.3.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      930 2024-02-03 16:32:54.216406 django-pikpdf-0.3.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      324 2024-02-03 16:25:25.000000 django-pikpdf-0.3.4/setup.py
+drwxrwxr-x   0 pikutis   (1003) pikutis   (1003)        0 2024-05-06 11:01:05.283593 django-pikpdf-0.3.5/
+-rw-rw-r--   0 pikutis   (1003) pikutis   (1003)      996 2024-03-18 20:24:53.000000 django-pikpdf-0.3.5/LICENSE
+-rw-rw-r--   0 pikutis   (1003) pikutis   (1003)      205 2024-03-18 20:24:53.000000 django-pikpdf-0.3.5/MANIFEST.in
+-rw-rw-r--   0 pikutis   (1003) pikutis   (1003)     2648 2024-05-06 11:01:05.283593 django-pikpdf-0.3.5/PKG-INFO
+-rw-rw-r--   0 pikutis   (1003) pikutis   (1003)     1679 2024-03-18 20:24:53.000000 django-pikpdf-0.3.5/README.md
+drwxrwxr-x   0 pikutis   (1003) pikutis   (1003)        0 2024-05-06 11:01:05.283593 django-pikpdf-0.3.5/django_pikpdf/
+-rw-rw-r--   0 pikutis   (1003) pikutis   (1003)        0 2024-03-18 20:24:53.000000 django-pikpdf-0.3.5/django_pikpdf/__init__.py
+-rw-rw-r--   0 pikutis   (1003) pikutis   (1003)       63 2024-03-18 20:24:53.000000 django-pikpdf-0.3.5/django_pikpdf/admin.py
+-rw-rw-r--   0 pikutis   (1003) pikutis   (1003)      172 2024-03-18 20:24:53.000000 django-pikpdf-0.3.5/django_pikpdf/apps.py
+drwxrwxr-x   0 pikutis   (1003) pikutis   (1003)        0 2024-05-06 11:01:05.283593 django-pikpdf-0.3.5/django_pikpdf/controllers/
+-rw-rw-r--   0 pikutis   (1003) pikutis   (1003)        0 2024-03-18 20:24:53.000000 django-pikpdf-0.3.5/django_pikpdf/controllers/__init__.py
+-rw-rw-r--   0 pikutis   (1003) pikutis   (1003)      796 2024-05-06 11:00:31.000000 django-pikpdf-0.3.5/django_pikpdf/controllers/api.py
+-rw-rw-r--   0 pikutis   (1003) pikutis   (1003)      396 2024-03-18 20:24:53.000000 django-pikpdf-0.3.5/django_pikpdf/controllers/html_transformation.py
+-rw-rw-r--   0 pikutis   (1003) pikutis   (1003)     2151 2024-03-18 20:24:53.000000 django-pikpdf-0.3.5/django_pikpdf/controllers/validators.py
+-rw-rw-r--   0 pikutis   (1003) pikutis   (1003)     1355 2024-03-18 20:24:53.000000 django-pikpdf-0.3.5/django_pikpdf/converter.py
+drwxrwxr-x   0 pikutis   (1003) pikutis   (1003)        0 2024-05-06 11:01:05.283593 django-pikpdf-0.3.5/django_pikpdf/migrations/
+-rw-rw-r--   0 pikutis   (1003) pikutis   (1003)        0 2024-03-18 20:24:53.000000 django-pikpdf-0.3.5/django_pikpdf/migrations/__init__.py
+-rw-rw-r--   0 pikutis   (1003) pikutis   (1003)       57 2024-03-18 20:24:53.000000 django-pikpdf-0.3.5/django_pikpdf/models.py
+-rw-rw-r--   0 pikutis   (1003) pikutis   (1003)       63 2024-03-18 20:24:53.000000 django-pikpdf-0.3.5/django_pikpdf/views.py
+drwxrwxr-x   0 pikutis   (1003) pikutis   (1003)        0 2024-05-06 11:01:05.283593 django-pikpdf-0.3.5/django_pikpdf.egg-info/
+-rw-rw-r--   0 pikutis   (1003) pikutis   (1003)     2648 2024-05-06 11:01:05.000000 django-pikpdf-0.3.5/django_pikpdf.egg-info/PKG-INFO
+-rw-rw-r--   0 pikutis   (1003) pikutis   (1003)      589 2024-05-06 11:01:05.000000 django-pikpdf-0.3.5/django_pikpdf.egg-info/SOURCES.txt
+-rw-rw-r--   0 pikutis   (1003) pikutis   (1003)        1 2024-05-06 11:01:05.000000 django-pikpdf-0.3.5/django_pikpdf.egg-info/dependency_links.txt
+-rw-rw-r--   0 pikutis   (1003) pikutis   (1003)       32 2024-05-06 11:01:05.000000 django-pikpdf-0.3.5/django_pikpdf.egg-info/requires.txt
+-rw-rw-r--   0 pikutis   (1003) pikutis   (1003)       14 2024-05-06 11:01:05.000000 django-pikpdf-0.3.5/django_pikpdf.egg-info/top_level.txt
+-rw-rw-r--   0 pikutis   (1003) pikutis   (1003)       88 2024-03-18 20:24:53.000000 django-pikpdf-0.3.5/pyproject.toml
+-rw-rw-r--   0 pikutis   (1003) pikutis   (1003)      930 2024-05-06 11:01:05.283593 django-pikpdf-0.3.5/setup.cfg
+-rw-rw-r--   0 pikutis   (1003) pikutis   (1003)      324 2024-03-18 20:24:53.000000 django-pikpdf-0.3.5/setup.py
```

### Comparing `django-pikpdf-0.3.4/LICENSE` & `django-pikpdf-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-pikpdf-0.3.4/PKG-INFO` & `django-pikpdf-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pikpdf
-Version: 0.3.4
+Version: 0.3.5
 Summary: A Django app to convert html to pdf
 Home-page: https://www.pikutis.lt/
 Author: Tadas Pikutis
 Author-email: tadas@pikutis.lt
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `django-pikpdf-0.3.4/README.md` & `django-pikpdf-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `django-pikpdf-0.3.4/django_pikpdf/controllers/api.py` & `django-pikpdf-0.3.5/django_pikpdf/controllers/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     '''
     return settings.PIKUTIS_API_KEY
 
 def call_pdf_api(file_string:str) -> dict:
     '''
         Calls pikutis api and returns response
     '''
-    pdf_request:requests.Request = requests.Request('POST', url="https://pikutis.lt/api/generate-pdf/")
+    pdf_request:requests.Request = requests.Request('POST', url="https://www.pikutis.lt/api/generate-pdf/")
     pdf_request.headers = {"Token": get_api_token()}
     pdf_request.data = file_string.encode('utf-8')
 
     pdf_response:requests.Response = requests.Session().send(pdf_request.prepare())
     return json.loads(pdf_response.content)
 
 def get_pdf_file(pdf_response:dict) -> bytes:
```

### Comparing `django-pikpdf-0.3.4/django_pikpdf/controllers/validators.py` & `django-pikpdf-0.3.5/django_pikpdf/controllers/validators.py`

 * *Files identical despite different names*

### Comparing `django-pikpdf-0.3.4/django_pikpdf/converter.py` & `django-pikpdf-0.3.5/django_pikpdf/converter.py`

 * *Files identical despite different names*

### Comparing `django-pikpdf-0.3.4/django_pikpdf.egg-info/PKG-INFO` & `django-pikpdf-0.3.5/django_pikpdf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pikpdf
-Version: 0.3.4
+Version: 0.3.5
 Summary: A Django app to convert html to pdf
 Home-page: https://www.pikutis.lt/
 Author: Tadas Pikutis
 Author-email: tadas@pikutis.lt
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `django-pikpdf-0.3.4/django_pikpdf.egg-info/SOURCES.txt` & `django-pikpdf-0.3.5/django_pikpdf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-pikpdf-0.3.4/setup.cfg` & `django-pikpdf-0.3.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-pikpdf
-version = 0.3.4
+version = 0.3.5
 description = A Django app to convert html to pdf
 long_description = file: README.rst
 url = https://www.pikutis.lt/
 author = Tadas Pikutis
 author_email = tadas@pikutis.lt
 license = MIT
 classifiers =
```

