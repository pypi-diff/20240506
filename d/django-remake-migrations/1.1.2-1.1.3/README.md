# Comparing `tmp/django_remake_migrations-1.1.2.tar.gz` & `tmp/django_remake_migrations-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_remake_migrations-1.1.2.tar", max compression
+gzip compressed data, was "django_remake_migrations-1.1.3.tar", max compression
```

## Comparing `django_remake_migrations-1.1.2.tar` & `django_remake_migrations-1.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1068 2024-03-11 12:19:55.885976 django_remake_migrations-1.1.2/LICENSE
--rw-r--r--   0        0        0     6160 2024-03-11 12:19:55.885976 django_remake_migrations-1.1.2/README.md
--rw-r--r--   0        0        0     4005 2024-03-11 12:19:56.873967 django_remake_migrations-1.1.2/pyproject.toml
--rw-r--r--   0        0        0       22 2024-03-11 12:19:56.873967 django_remake_migrations-1.1.2/src/django_remake_migrations/__init__.py
--rw-r--r--   0        0        0      266 2024-03-11 12:19:55.885976 django_remake_migrations-1.1.2/src/django_remake_migrations/apps.py
--rw-r--r--   0        0        0     1737 2024-03-11 12:19:55.885976 django_remake_migrations-1.1.2/src/django_remake_migrations/conf.py
--rw-r--r--   0        0        0        0 2024-03-11 12:19:55.885976 django_remake_migrations-1.1.2/src/django_remake_migrations/management/__init__.py
--rw-r--r--   0        0        0        0 2024-03-11 12:19:55.885976 django_remake_migrations-1.1.2/src/django_remake_migrations/management/commands/__init__.py
--rw-r--r--   0        0        0     8387 2024-03-11 12:19:55.885976 django_remake_migrations-1.1.2/src/django_remake_migrations/management/commands/remakemigrations.py
--rw-r--r--   0        0        0        0 2024-03-11 12:19:55.885976 django_remake_migrations-1.1.2/src/django_remake_migrations/py.typed
--rw-r--r--   0        0        0     7701 1970-01-01 00:00:00.000000 django_remake_migrations-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-06 21:17:11.022901 django_remake_migrations-1.1.3/LICENSE
+-rw-r--r--   0        0        0     6160 2024-05-06 21:17:11.022901 django_remake_migrations-1.1.3/README.md
+-rw-r--r--   0        0        0     4007 2024-05-06 21:17:12.258906 django_remake_migrations-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-06 21:17:12.258906 django_remake_migrations-1.1.3/src/django_remake_migrations/__init__.py
+-rw-r--r--   0        0        0      266 2024-05-06 21:17:11.026901 django_remake_migrations-1.1.3/src/django_remake_migrations/apps.py
+-rw-r--r--   0        0        0     1737 2024-05-06 21:17:11.026901 django_remake_migrations-1.1.3/src/django_remake_migrations/conf.py
+-rw-r--r--   0        0        0        0 2024-05-06 21:17:11.026901 django_remake_migrations-1.1.3/src/django_remake_migrations/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 21:17:11.026901 django_remake_migrations-1.1.3/src/django_remake_migrations/management/commands/__init__.py
+-rw-r--r--   0        0        0     8387 2024-05-06 21:17:11.026901 django_remake_migrations-1.1.3/src/django_remake_migrations/management/commands/remakemigrations.py
+-rw-r--r--   0        0        0        0 2024-05-06 21:17:11.026901 django_remake_migrations-1.1.3/src/django_remake_migrations/py.typed
+-rw-r--r--   0        0        0     7701 1970-01-01 00:00:00.000000 django_remake_migrations-1.1.3/PKG-INFO
```

### Comparing `django_remake_migrations-1.1.2/LICENSE` & `django_remake_migrations-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_remake_migrations-1.1.2/README.md` & `django_remake_migrations-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `django_remake_migrations-1.1.2/pyproject.toml` & `django_remake_migrations-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-remake-migrations"
-version = "1.1.2"
+version = "1.1.3"
 description = "A Django admin command to recreate all migrations in a project."
 authors = ["Bruno Alla <oss@browniebroke.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/browniebroke/django-remake-migrations"
 documentation = "https://django-remake-migrations.readthedocs.io"
 classifiers = [
@@ -30,15 +30,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 django = ">=3.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.0"
-pytest-cov = "^4.0"
+pytest-cov = "^5.0.0"
 pytest-django = "^4.5"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 myst-parser = { version = ">=0.16", python = ">=3.11" }
```

### Comparing `django_remake_migrations-1.1.2/src/django_remake_migrations/conf.py` & `django_remake_migrations-1.1.3/src/django_remake_migrations/conf.py`

 * *Files identical despite different names*

### Comparing `django_remake_migrations-1.1.2/src/django_remake_migrations/management/commands/remakemigrations.py` & `django_remake_migrations-1.1.3/src/django_remake_migrations/management/commands/remakemigrations.py`

 * *Files identical despite different names*

### Comparing `django_remake_migrations-1.1.2/PKG-INFO` & `django_remake_migrations-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-remake-migrations
-Version: 1.1.2
+Version: 1.1.3
 Summary: A Django admin command to recreate all migrations in a project.
 Home-page: https://github.com/browniebroke/django-remake-migrations
 License: MIT
 Author: Bruno Alla
 Author-email: oss@browniebroke.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-remake-migrations Version: 1.1.2 Summary: A
+Metadata-Version: 2.1 Name: django-remake-migrations Version: 1.1.3 Summary: A
 Django admin command to recreate all migrations in a project. Home-page: https:
 //github.com/browniebroke/django-remake-migrations License: MIT Author: Bruno
 Alla Author-email: oss@browniebroke.com Requires-Python: >=3.8,<4.0 Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Framework :: Django Classifier:
 Framework :: Django :: 3.2 Classifier: Framework :: Django :: 4.0 Classifier:
 Framework :: Django :: 4.1 Classifier: Framework :: Django :: 4.2 Classifier:
 Framework :: Django :: 5.0 Classifier: Intended Audience :: Developers
```

