# Comparing `tmp/django_translate_gettext-0.3.5.tar.gz` & `tmp/django_translate_gettext-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_translate_gettext-0.3.5.tar", max compression
+gzip compressed data, was "django_translate_gettext-0.3.6.tar", max compression
```

## Comparing `django_translate_gettext-0.3.5.tar` & `django_translate_gettext-0.3.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1070 2024-02-12 09:40:17.104704 django_translate_gettext-0.3.5/LICENSE
--rw-r--r--   0        0        0     6123 2024-03-18 06:45:00.340098 django_translate_gettext-0.3.5/README.md
--rw-r--r--   0        0        0        0 2024-02-12 09:40:17.105244 django_translate_gettext-0.3.5/django_translate_gettext/__init__.py
--rw-r--r--   0        0        0      178 2024-02-12 09:40:17.105402 django_translate_gettext-0.3.5/django_translate_gettext/apps.py
--rw-r--r--   0        0        0       89 2024-03-03 11:40:28.823005 django_translate_gettext-0.3.5/django_translate_gettext/constants.py
--rw-r--r--   0        0        0      137 2024-03-18 06:45:00.340338 django_translate_gettext-0.3.5/django_translate_gettext/exceptions.py
--rw-r--r--   0        0        0        0 2024-02-12 09:40:17.105536 django_translate_gettext-0.3.5/django_translate_gettext/management/__init__.py
--rw-r--r--   0        0        0        0 2024-02-12 09:40:17.105682 django_translate_gettext-0.3.5/django_translate_gettext/management/commands/__init__.py
--rw-r--r--   0        0        0     5060 2024-03-22 09:21:15.070546 django_translate_gettext-0.3.5/django_translate_gettext/management/commands/translate.py
--rw-r--r--   0        0        0      101 2024-02-13 07:49:12.693912 django_translate_gettext-0.3.5/django_translate_gettext/services/__init__.py
--rw-r--r--   0        0        0     1116 2024-03-18 06:45:00.340924 django_translate_gettext-0.3.5/django_translate_gettext/services/files.py
--rw-r--r--   0        0        0      570 2024-02-20 12:24:32.610623 django_translate_gettext-0.3.5/django_translate_gettext/services/models.py
--rw-r--r--   0        0        0    10740 2024-03-22 09:21:15.070764 django_translate_gettext-0.3.5/django_translate_gettext/services/transformers.py
--rw-r--r--   0        0        0     2199 2024-03-18 06:45:00.341470 django_translate_gettext-0.3.5/django_translate_gettext/services/translators.py
--rw-r--r--   0        0        0     1903 2024-03-22 09:27:46.274932 django_translate_gettext-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     7543 1970-01-01 00:00:00.000000 django_translate_gettext-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-02-12 09:40:17.104704 django_translate_gettext-0.3.6/LICENSE
+-rw-r--r--   0        0        0     6123 2024-03-18 06:45:00.340098 django_translate_gettext-0.3.6/README.md
+-rw-r--r--   0        0        0        0 2024-02-12 09:40:17.105244 django_translate_gettext-0.3.6/django_translate_gettext/__init__.py
+-rw-r--r--   0        0        0      178 2024-02-12 09:40:17.105402 django_translate_gettext-0.3.6/django_translate_gettext/apps.py
+-rw-r--r--   0        0        0       89 2024-03-03 11:40:28.823005 django_translate_gettext-0.3.6/django_translate_gettext/constants.py
+-rw-r--r--   0        0        0      137 2024-03-18 06:45:00.340338 django_translate_gettext-0.3.6/django_translate_gettext/exceptions.py
+-rw-r--r--   0        0        0        0 2024-02-12 09:40:17.105536 django_translate_gettext-0.3.6/django_translate_gettext/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-12 09:40:17.105682 django_translate_gettext-0.3.6/django_translate_gettext/management/commands/__init__.py
+-rw-r--r--   0        0        0     5060 2024-03-22 09:21:15.070546 django_translate_gettext-0.3.6/django_translate_gettext/management/commands/translate.py
+-rw-r--r--   0        0        0      101 2024-02-13 07:49:12.693912 django_translate_gettext-0.3.6/django_translate_gettext/services/__init__.py
+-rw-r--r--   0        0        0     1116 2024-03-18 06:45:00.340924 django_translate_gettext-0.3.6/django_translate_gettext/services/files.py
+-rw-r--r--   0        0        0      570 2024-02-20 12:24:32.610623 django_translate_gettext-0.3.6/django_translate_gettext/services/models.py
+-rw-r--r--   0        0        0    10740 2024-03-22 09:21:15.070764 django_translate_gettext-0.3.6/django_translate_gettext/services/transformers.py
+-rw-r--r--   0        0        0     2199 2024-03-18 06:45:00.341470 django_translate_gettext-0.3.6/django_translate_gettext/services/translators.py
+-rw-r--r--   0        0        0     1903 2024-05-06 08:30:30.394442 django_translate_gettext-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     7543 1970-01-01 00:00:00.000000 django_translate_gettext-0.3.6/PKG-INFO
```

### Comparing `django_translate_gettext-0.3.5/LICENSE` & `django_translate_gettext-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django_translate_gettext-0.3.5/README.md` & `django_translate_gettext-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `django_translate_gettext-0.3.5/django_translate_gettext/management/commands/translate.py` & `django_translate_gettext-0.3.6/django_translate_gettext/management/commands/translate.py`

 * *Files identical despite different names*

### Comparing `django_translate_gettext-0.3.5/django_translate_gettext/services/files.py` & `django_translate_gettext-0.3.6/django_translate_gettext/services/files.py`

 * *Files identical despite different names*

### Comparing `django_translate_gettext-0.3.5/django_translate_gettext/services/models.py` & `django_translate_gettext-0.3.6/django_translate_gettext/services/models.py`

 * *Files identical despite different names*

### Comparing `django_translate_gettext-0.3.5/django_translate_gettext/services/transformers.py` & `django_translate_gettext-0.3.6/django_translate_gettext/services/transformers.py`

 * *Files identical despite different names*

### Comparing `django_translate_gettext-0.3.5/django_translate_gettext/services/translators.py` & `django_translate_gettext-0.3.6/django_translate_gettext/services/translators.py`

 * *Files identical despite different names*

### Comparing `django_translate_gettext-0.3.5/pyproject.toml` & `django_translate_gettext-0.3.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-translate-gettext"
-version = "0.3.5"
+version = "0.3.6"
 description = "Django app to wrap app files class fields to gettext calling for the given apps"
 authors = ["Denis Novikov <alpden550@gmail.com>"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.10",
@@ -27,16 +27,16 @@
 repository = 'https://github.com/alpden550/django-translate-gettext'
 keywords = ["django", "django-orm", "django app", "ast", "orm"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 django = "^4.0.1"
 loguru = "^0.7.2"
-ruff = "^0.3.0"
 deep-translator = "^1.11.4"
+ruff = "^0.4.3"
 
 [tool.poetry.group.dev.dependencies]
 complexipy = "^0.3.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `django_translate_gettext-0.3.5/PKG-INFO` & `django_translate_gettext-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-translate-gettext
-Version: 0.3.5
+Version: 0.3.6
 Summary: Django app to wrap app files class fields to gettext calling for the given apps
 Home-page: https://github.com/alpden550/django-translate-gettext
 License: MIT
 Keywords: django,django-orm,django app,ast,orm
 Author: Denis Novikov
 Author-email: alpden550@gmail.com
 Requires-Python: >=3.11,<4.0
@@ -24,15 +24,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Requires-Dist: deep-translator (>=1.11.4,<2.0.0)
 Requires-Dist: django (>=4.0.1,<5.0.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
-Requires-Dist: ruff (>=0.3.0,<0.4.0)
+Requires-Dist: ruff (>=0.4.3,<0.5.0)
 Project-URL: Repository, https://github.com/alpden550/django-translate-gettext
 Description-Content-Type: text/markdown
 
 # Django-translate-getetxt
 
 This is a django app that allows you to wrap django applications files fields with a gettext translation field (not for Pycharm and docker-compose python interpretator).
```

