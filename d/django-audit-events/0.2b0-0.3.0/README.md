# Comparing `tmp/django-audit-events-0.2b0.tar.gz` & `tmp/django-audit-events-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-audit-events-0.2b0.tar", last modified: Fri Jun  5 08:21:55 2020, max compression
+gzip compressed data, was "dist/django-audit-events-0.3.0.tar", last modified: Mon May  6 06:52:16 2024, max compression
```

## Comparing `django-audit-events-0.2b0.tar` & `django-audit-events-0.3.0.tar`

### file list

```diff
@@ -1,64 +1,70 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-05 08:21:55.000000 django-audit-events-0.2b0/
--rw-rw-rw-   0 root         (0) root         (0)      220 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/.editorconfig
--rw-rw-rw-   0 root         (0) root         (0)       94 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      113 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/.isort.cfg
--rw-rw-rw-   0 root         (0) root         (0)       27 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)     1050 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)     3417 2020-06-05 08:21:55.000000 django-audit-events-0.2b0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1714 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2377 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-05 08:21:55.000000 django-audit-events-0.2b0/django_audit_events/
--rw-rw-rw-   0 root         (0) root         (0)      380 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      396 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      251 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      557 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     3628 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/context.py
--rw-rw-rw-   0 root         (0) root         (0)      399 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/filters.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-05 08:21:55.000000 django-audit-events-0.2b0/django_audit_events/locale/
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-05 08:21:55.000000 django-audit-events-0.2b0/django_audit_events/locale/tr/
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-05 08:21:55.000000 django-audit-events-0.2b0/django_audit_events/locale/tr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     1481 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/locale/tr/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)      843 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/middleware.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-05 08:21:55.000000 django-audit-events-0.2b0/django_audit_events/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     2007 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      662 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     4032 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/models.py
--rw-rw-rw-   0 root         (0) root         (0)      380 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)     1226 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/tasks.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-05 08:21:55.000000 django-audit-events-0.2b0/django_audit_events/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      290 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/tests/test_conf.py
--rw-rw-rw-   0 root         (0) root         (0)     3958 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/tests/test_context.py
--rw-rw-rw-   0 root         (0) root         (0)     1215 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/tests/test_middleware.py
--rw-rw-rw-   0 root         (0) root         (0)     1539 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/tests/test_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     2062 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     1847 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/tests/test_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)       58 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/tests/urls.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-05 08:21:55.000000 django-audit-events-0.2b0/django_audit_events/tests/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/tests/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      160 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/tests/utils/models.py
--rw-rw-rw-   0 root         (0) root         (0)      175 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/urls.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2020-06-05 08:21:55.000000 django-audit-events-0.2b0/django_audit_events/version.py
--rw-rw-rw-   0 root         (0) root         (0)     1396 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/django_audit_events/views.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-05 08:21:55.000000 django-audit-events-0.2b0/django_audit_events.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     3417 2020-06-05 08:21:55.000000 django-audit-events-0.2b0/django_audit_events.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1479 2020-06-05 08:21:55.000000 django-audit-events-0.2b0/django_audit_events.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2020-06-05 08:21:55.000000 django-audit-events-0.2b0/django_audit_events.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2020-06-05 08:21:55.000000 django-audit-events-0.2b0/django_audit_events.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       20 2020-06-05 08:21:55.000000 django-audit-events-0.2b0/django_audit_events.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-05 08:21:55.000000 django-audit-events-0.2b0/docs/
--rw-rw-rw-   0 root         (0) root         (0)      634 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     1609 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/docs/advanced.rst
--rw-rw-rw-   0 root         (0) root         (0)     2080 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     1054 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/docs/configuration.rst
--rw-rw-rw-   0 root         (0) root         (0)      944 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1252 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/docs/introduction.rst
--rw-rw-rw-   0 root         (0) root         (0)      795 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)     2265 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/docs/quickstart.rst
--rw-rw-rw-   0 root         (0) root         (0)      310 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      204 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     2218 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/runtests.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2020-06-05 08:21:55.000000 django-audit-events-0.2b0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2289 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1177 2020-06-05 08:20:55.000000 django-audit-events-0.2b0/tox.ini
+drwxrwxr-x   0 ozkok     (1000) ozkok     (1000)        0 2024-05-06 06:52:16.000000 django-audit-events-0.3.0/
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      220 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/.editorconfig
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      101 2024-05-06 06:51:16.000000 django-audit-events-0.3.0/.gitignore
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      113 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/.isort.cfg
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)       27 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/CHANGELOG.md
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1050 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/LICENSE.txt
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     3505 2024-05-06 06:52:16.000000 django-audit-events-0.3.0/PKG-INFO
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1714 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/README.md
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     2612 2024-05-06 06:51:16.000000 django-audit-events-0.3.0/bitbucket-pipelines.yml
+drwxrwxr-x   0 ozkok     (1000) ozkok     (1000)        0 2024-05-06 06:52:16.000000 django-audit-events-0.3.0/django_audit_events/
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      380 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/__init__.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      396 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/admin.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      447 2023-11-29 08:37:50.000000 django-audit-events-0.3.0/django_audit_events/apps.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      733 2024-05-06 06:51:16.000000 django-audit-events-0.3.0/django_audit_events/conf.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     4523 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/context.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1842 2024-05-06 06:51:16.000000 django-audit-events-0.3.0/django_audit_events/filters.py
+drwxrwxr-x   0 ozkok     (1000) ozkok     (1000)        0 2024-05-06 06:52:16.000000 django-audit-events-0.3.0/django_audit_events/locale/
+drwxrwxr-x   0 ozkok     (1000) ozkok     (1000)        0 2024-05-06 06:52:16.000000 django-audit-events-0.3.0/django_audit_events/locale/tr/
+drwxrwxr-x   0 ozkok     (1000) ozkok     (1000)        0 2024-05-06 06:52:16.000000 django-audit-events-0.3.0/django_audit_events/locale/tr/LC_MESSAGES/
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1544 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/locale/tr/LC_MESSAGES/django.po
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      843 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/middleware.py
+drwxrwxr-x   0 ozkok     (1000) ozkok     (1000)        0 2024-05-06 06:52:16.000000 django-audit-events-0.3.0/django_audit_events/migrations/
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1984 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/migrations/0001_initial.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     2207 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/migrations/0002_archivedauditevent.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      712 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/migrations/0003_auto_20201218_1113.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      650 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/migrations/0004_auto_20210127_2021.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      768 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/migrations/0005_auto_20220215_0756.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      669 2023-11-29 08:37:50.000000 django-audit-events-0.3.0/django_audit_events/migrations/0006_auto_20220920_1327.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)        0 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/migrations/__init__.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      857 2023-11-29 08:37:50.000000 django-audit-events-0.3.0/django_audit_events/mixin.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     4659 2023-11-29 08:37:50.000000 django-audit-events-0.3.0/django_audit_events/models.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      476 2023-11-29 08:37:50.000000 django-audit-events-0.3.0/django_audit_events/serializers.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1675 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/tasks.py
+drwxrwxr-x   0 ozkok     (1000) ozkok     (1000)        0 2024-05-06 06:52:16.000000 django-audit-events-0.3.0/django_audit_events/tests/
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)        0 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/tests/__init__.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      290 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/tests/test_conf.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     6001 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/tests/test_context.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1362 2023-11-29 08:37:50.000000 django-audit-events-0.3.0/django_audit_events/tests/test_middleware.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1539 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/tests/test_mixin.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     2062 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/tests/test_models.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     2548 2023-11-29 08:37:50.000000 django-audit-events-0.3.0/django_audit_events/tests/test_tasks.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)       58 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/tests/urls.py
+drwxrwxr-x   0 ozkok     (1000) ozkok     (1000)        0 2024-05-06 06:52:16.000000 django-audit-events-0.3.0/django_audit_events/tests/utils/
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)       65 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/tests/utils/__init__.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      160 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/tests/utils/models.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      205 2024-05-06 06:51:16.000000 django-audit-events-0.3.0/django_audit_events/urls.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      917 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/utils.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)       22 2024-05-06 06:52:16.000000 django-audit-events-0.3.0/django_audit_events/version.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1060 2023-11-29 08:37:50.000000 django-audit-events-0.3.0/django_audit_events/views.py
+drwxrwxr-x   0 ozkok     (1000) ozkok     (1000)        0 2024-05-06 06:52:16.000000 django-audit-events-0.3.0/django_audit_events.egg-info/
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     3505 2024-05-06 06:52:16.000000 django-audit-events-0.3.0/django_audit_events.egg-info/PKG-INFO
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1798 2024-05-06 06:52:16.000000 django-audit-events-0.3.0/django_audit_events.egg-info/SOURCES.txt
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)        1 2024-05-06 06:52:16.000000 django-audit-events-0.3.0/django_audit_events.egg-info/dependency_links.txt
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)        1 2024-05-06 06:50:27.000000 django-audit-events-0.3.0/django_audit_events.egg-info/not-zip-safe
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)       20 2024-05-06 06:52:16.000000 django-audit-events-0.3.0/django_audit_events.egg-info/top_level.txt
+drwxrwxr-x   0 ozkok     (1000) ozkok     (1000)        0 2024-05-06 06:52:16.000000 django-audit-events-0.3.0/docs/
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      634 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/docs/Makefile
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1609 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/docs/advanced.rst
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     2080 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/docs/conf.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1533 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/docs/configuration.rst
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      944 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/docs/index.rst
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1252 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/docs/introduction.rst
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      795 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/docs/make.bat
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     2265 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/docs/quickstart.rst
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      310 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/pyproject.toml
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      396 2024-05-06 06:51:16.000000 django-audit-events-0.3.0/requirements.txt
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     2337 2024-05-06 06:51:16.000000 django-audit-events-0.3.0/runtests.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)       38 2024-05-06 06:52:16.000000 django-audit-events-0.3.0/setup.cfg
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     2628 2024-05-06 06:51:16.000000 django-audit-events-0.3.0/setup.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1819 2024-05-06 06:51:16.000000 django-audit-events-0.3.0/tox.ini
```

### Comparing `django-audit-events-0.2b0/LICENSE.txt` & `django-audit-events-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.2b0/PKG-INFO` & `django-audit-events-0.3.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,70 +1,79 @@
 Metadata-Version: 2.1
 Name: django-audit-events
-Version: 0.2b0
+Version: 0.3.0
 Summary: Log audit events in Django
 Home-page: https://bitbucket.org/akinonteam/django-audit-events
 Author: Onur Güzel
 Author-email: dev@akinon.com
 Maintainer: Akinon
 Maintainer-email: dev@akinon.com
 License: MIT
 Project-URL: Documentation, https://django-audit-events.readthedocs.io/
 Project-URL: Source Code, https://bitbucket.org/akinonteam/django-audit-events
-Description: # Django Audit Events
-        
-        [![Build status](https://img.shields.io/bitbucket/pipelines/akinonteam/django-audit-events)](https://bitbucket.org/akinonteam/django-audit-events/addon/pipelines/home)
-        [![Documentation status](https://readthedocs.org/projects/django-audit-events/badge/?version=latest)](https://django-audit-events.readthedocs.io/en/latest/?badge=latest)
-        ![PyPI](https://img.shields.io/pypi/v/django-audit-events)
-        ![PyPI - Django version](https://img.shields.io/pypi/djversions/django-audit-events)
-        ![PyPI - Python version](https://img.shields.io/pypi/pyversions/django-audit-events)
-        ![PyPI - License](https://img.shields.io/pypi/l/django-audit-events)
-        [![Total alerts](https://img.shields.io/lgtm/alerts/bitbucket/akinonteam/django-audit-events)](https://lgtm.com/projects/b/akinonteam/django-audit-events/alerts/)
-        [![Code quality](https://img.shields.io/lgtm/grade/python/bitbucket/akinonteam/django-audit-events)](https://lgtm.com/projects/b/akinonteam/django-audit-events/context:python)
-        
-        Extensible custom audit events for humans! This Django app allows you to easily create your own events in your project. Currently only works on PostgreSQL.
-        
-        Let's have a look:
-        
-        ```python
-        def awesome_view(request):
-            foo_obj = Foo.objects.get(pk=1)
-            # Do something with foo_obj...
-            request.audit_context.create_event(
-                foo_obj,
-                something="done",
-                bar="baz"
-            )
-        ```
-        
-        This will create an audit event, including the request URL, logged-in user, remote IP address, and the following event content:
-        
-        ```
-        >>> event.content
-        {"something": "done", "bar: "baz"}
-        ```
-        
-        For more information about installation and usage, check out the [documentation](https://django-audit-events.readthedocs.io/)!
-        
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.10
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 3.1
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# Django Audit Events
+
+[![Build status](https://img.shields.io/bitbucket/pipelines/akinonteam/django-audit-events)](https://bitbucket.org/akinonteam/django-audit-events/addon/pipelines/home)
+[![Documentation status](https://readthedocs.org/projects/django-audit-events/badge/?version=latest)](https://django-audit-events.readthedocs.io/en/latest/?badge=latest)
+![PyPI](https://img.shields.io/pypi/v/django-audit-events)
+![PyPI - Django version](https://img.shields.io/pypi/djversions/django-audit-events)
+![PyPI - Python version](https://img.shields.io/pypi/pyversions/django-audit-events)
+![PyPI - License](https://img.shields.io/pypi/l/django-audit-events)
+[![Total alerts](https://img.shields.io/lgtm/alerts/bitbucket/akinonteam/django-audit-events)](https://lgtm.com/projects/b/akinonteam/django-audit-events/alerts/)
+[![Code quality](https://img.shields.io/lgtm/grade/python/bitbucket/akinonteam/django-audit-events)](https://lgtm.com/projects/b/akinonteam/django-audit-events/context:python)
+
+Extensible custom audit events for humans! This Django app allows you to easily create your own events in your project. Currently only works on PostgreSQL.
+
+Let's have a look:
+
+```python
+def awesome_view(request):
+    foo_obj = Foo.objects.get(pk=1)
+    # Do something with foo_obj...
+    request.audit_context.create_event(
+        foo_obj,
+        something="done",
+        bar="baz"
+    )
+```
+
+This will create an audit event, including the request URL, logged-in user, remote IP address, and the following event content:
+
+```
+>>> event.content
+{"something": "done", "bar: "baz"}
+```
+
+For more information about installation and usage, check out the [documentation](https://django-audit-events.readthedocs.io/)!
```

### Comparing `django-audit-events-0.2b0/README.md` & `django-audit-events-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.2b0/bitbucket-pipelines.yml` & `django-audit-events-0.3.0/bitbucket-pipelines.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,78 +1,79 @@
 pipelines:
   default:
-    - step:
-        name: linting
-        image: python:3.7-alpine
-        script:
-          - apk add gcc git musl-dev
-          - pip install tox
-          - tox -e linting
-    - step:
-        name: py27    
-        image: python:2.7-alpine
-        script:
-          - apk add postgresql-dev gcc git python2-dev musl-dev
-          - pip install tox
-          - tox -e py27-django110,py27-django111
-        services:
-          - postgres
-    - step:
-        name: py34
-        image: python:3.4-alpine
-        script:
-          - apk add postgresql-dev gcc git python3-dev musl-dev
-          - pip install tox
-          - tox -e py34-django110,py34-django111,py34-django20
-        services:
-          - postgres
-    - step:
-        name: py35
-        image: python:3.5-alpine
-        script:
-          - apk add postgresql-dev gcc git python3-dev musl-dev
-          - pip install tox
-          - tox -e py35-django110,py35-django111,py35-django20,py35-django21,py35-django22
-        services:
-          - postgres
-    - step:
-        name: py36
-        image: python:3.6-alpine
-        script:
-          - apk add postgresql-dev gcc git python3-dev musl-dev
-          - pip install tox
-          - tox -e py36-django111,py36-django20,py36-django21,py36-django22,py36-django30
-        services:
-          - postgres
-    - step:
-        name: py37
-        image: python:3.7-alpine
-        script:
-          - apk add postgresql-dev gcc git python3-dev musl-dev
-          - pip install tox
-          - tox -e py37-django111,py37-django20,py37-django21,py37-django22,py37-django30
-        services:
-          - postgres
-    - step:
-        name: py38
-        image: python:3.8-alpine
-        script:
-          - apk add postgresql-dev gcc git python3-dev musl-dev
-          - pip install tox
-          - tox -e py38-django22,py38-django30
-        services:
-          - postgres
+    - parallel:
+      - step:
+          name: linting
+          image: python:3.7-alpine
+          script:
+            - apk add gcc git musl-dev
+            - pip install tox
+            - tox -e linting
+      - step:
+          name: py27
+          image: python:2.7-alpine
+          script:
+            - apk add postgresql-dev gcc git python2-dev musl-dev
+            - pip install tox
+            - tox -e py27-django110,py27-django111
+          services:
+            - postgres
+      - step:
+          name: py34
+          image: python:3.4-alpine
+          script:
+            - apk add postgresql-dev gcc git python3-dev musl-dev
+            - pip install tox
+            - tox -e py34-django110,py34-django111,py34-django20
+          services:
+            - postgres
+      - step:
+          name: py35
+          image: python:3.5-alpine
+          script:
+            - apk add postgresql-dev gcc git python3-dev musl-dev
+            - pip install tox
+            - tox -e py35-django110,py35-django111,py35-django20,py35-django21,py35-django22
+          services:
+            - postgres
+      - step:
+          name: py36
+          image: python:3.6-alpine
+          script:
+            - apk add postgresql-dev gcc git python3-dev musl-dev
+            - pip install tox
+            - tox -e py36-django111,py36-django20,py36-django21,py36-django22,py36-django30
+          services:
+            - postgres
+      - step:
+          name: py37
+          image: python:3.7-alpine
+          script:
+            - apk add postgresql-dev gcc git python3-dev musl-dev
+            - pip install tox
+            - tox -e py37-django111,py37-django20,py37-django21,py37-django22,py37-django30
+          services:
+            - postgres
+      - step:
+          name: py38
+          image: python:3.8-alpine
+          script:
+            - apk add postgresql-dev gcc git python3-dev musl-dev
+            - pip install tox
+            - tox -e py38-django22,py38-django30,py38-django31,py38-django32,py38-django40,py38-django41,py38-django42
+          services:
+            - postgres
   tags:
     '*':
       - step:
           name: Publish to PyPI
           image: python:3.7-alpine
           script:
             - apk add gcc git libffi-dev musl-dev openssl-dev python3-dev
-            - pip install setuptools setuptools_scm twine
+            - CRYPTOGRAPHY_DONT_BUILD_RUST=1 pip install setuptools setuptools_scm twine
             - python setup.py sdist bdist_wheel
             - twine upload -u $PYPI_USERNAME -p $PYPI_PASSWORD dist/*
 definitions:
   services:
     postgres:
       image: postgres
       variables:
```

### Comparing `django-audit-events-0.2b0/django_audit_events/conf.py` & `django-audit-events-0.3.0/django_audit_events/conf.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from django.conf import settings as django_settings
 
 DEFAULT_SETTINGS = {
     "AUDIT_EVENT_MODEL": "django_audit_events.AuditEvent",
     "AUDIT_EVENT_ARCHIVE_MODEL": "django_audit_events.ArchivedAuditEvent",
     "AUDIT_INCLUDE_QUERY_PARAMS": False,
     "AUDIT_INCLUDE_POST_DATA": False,
+    "AUDIT_INCLUDE_HEADERS": False,
     "AUDIT_MASK_POST_FIELDS": ("password",),
+    "AUDIT_CLIENT_IP_RESOLVER_FUNCTION": "django_audit_events.utils.get_client_ip",
+    "DEFAULT_AUTO_FIELD": "django.models.db.AutoField",
 }
 
 
 class Settings(object):
     def __getattr__(self, item):
         if item in DEFAULT_SETTINGS:
             return getattr(django_settings, item, DEFAULT_SETTINGS[item])
```

### Comparing `django-audit-events-0.2b0/django_audit_events/context.py` & `django-audit-events-0.3.0/django_audit_events/context.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 from copy import deepcopy
 
 from django.apps import apps
 from django.contrib.auth.models import AnonymousUser
+from django.utils.module_loading import import_string
 
 from django_audit_events.conf import settings
 
 MASK_VALUE = "*" * 16
 
 
 class AuditContext(object):
     extra_data = {}
-    __slots__ = ["url", "remote_addr", "user", "query_params", "post_data"]
+    __slots__ = ["url", "remote_addr", "user", "query_params", "post_data", "headers"]
 
     def __init__(
-        self, url=None, remote_addr=None, user=None, query_params=None, post_data=None
+        self,
+        url=None,
+        remote_addr=None,
+        user=None,
+        query_params=None,
+        post_data=None,
+        headers=None,
     ):
         super(AuditContext, self).__setattr__("url", url)
         super(AuditContext, self).__setattr__("remote_addr", remote_addr)
         super(AuditContext, self).__setattr__("user", user)
         super(AuditContext, self).__setattr__("query_params", query_params or {})
         super(AuditContext, self).__setattr__("post_data", post_data or {})
+        super(AuditContext, self).__setattr__("headers", headers or {})
 
     def __setattr__(self, key, value):
         raise NotImplementedError
 
     def __delattr__(self, item):
         raise NotImplementedError
 
@@ -33,33 +41,46 @@
         Create a context from HTTP request
 
         :type request: django.http.HttpRequest
         :return: An audit context
         :rtype: AuditContext
         """
         # noinspection PyUnresolvedReferences
+        client_ip_function = cls.get_client_ip_function()
         context = {
             "url": request.build_absolute_uri(),
-            "remote_addr": request.META.get("REMOTE_ADDR"),
+            "remote_addr": client_ip_function(request),
             "user": request.user,
         }
 
         if isinstance(context["user"], AnonymousUser):
             context["user"] = None
 
         if settings.AUDIT_INCLUDE_QUERY_PARAMS:
             context["query_params"] = request.GET
 
         if settings.AUDIT_INCLUDE_POST_DATA:
             # Copy POST data before masking sensitive fields
             # noinspection PyArgumentList
             context["post_data"] = cls.mask_fields(
-                request.POST.copy(), settings.AUDIT_MASK_POST_FIELDS,
+                request.POST.copy(),
+                settings.AUDIT_MASK_POST_FIELDS,
             )
 
+        if settings.AUDIT_INCLUDE_HEADERS and isinstance(
+            settings.AUDIT_INCLUDE_HEADERS, list
+        ):
+            context["headers"] = {
+                header.replace("HTTP_", "", 1)
+                .replace("_", "-")
+                .title(): request.META.get(header)
+                for header in settings.AUDIT_INCLUDE_HEADERS
+                if request.META.get(header)
+            }
+
         return cls(**context)
 
     @staticmethod
     def mask_fields(data, fields_to_mask):
         """
         Replace sensitive information in POST data
         :param data: POST data
@@ -103,7 +124,14 @@
         :param content: Event content
         :return: Saved audit event
         :rtype: django_audit_events.models.AbstractAuditEvent
         """
         for field in fields:
             content[field] = getattr(content_object, field)
         return self.create_event(content_object, **content)
+
+    @classmethod
+    def get_client_ip_function(cls):
+        _function = settings.AUDIT_CLIENT_IP_RESOLVER_FUNCTION
+        if callable(_function):
+            return _function
+        return import_string(_function)
```

### Comparing `django-audit-events-0.2b0/django_audit_events/locale/tr/LC_MESSAGES/django.po` & `django-audit-events-0.3.0/django_audit_events/locale/tr/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,18 @@
 msgid "Query params"
 msgstr "Sorgu parametreleri"
 
 #: models.py:28
 msgid "Post data"
 msgstr "Form verisi"
 
+#: models.py:54
+msgid "Headers"
+msgstr "İstek başlıkları"
+
 #: models.py:32
 msgid "Content"
 msgstr "İçerik"
 
 #: models.py:35
 msgid "Audit event"
 msgstr "Denetim olayı"
```

### Comparing `django-audit-events-0.2b0/django_audit_events/middleware.py` & `django-audit-events-0.3.0/django_audit_events/middleware.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.2b0/django_audit_events/migrations/0001_initial.py` & `django-audit-events-0.3.0/django_audit_events/migrations/0002_archivedauditevent.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,49 @@
-# Generated by Django 3.0.1 on 2019-12-26 14:35
+# -*- coding: utf-8 -*-
+# Generated by Django 1.10.3 on 2020-09-14 13:08
+from __future__ import unicode_literals
 
 import uuid
 
-import django.contrib.postgres.fields.jsonb
 import django.db.models.deletion
 from django.conf import settings
 from django.db import migrations, models
 
+try:
+    from django.db.models import JSONField
+except ImportError:
+    from django.contrib.postgres.fields.jsonb import JSONField
 
-class Migration(migrations.Migration):
 
-    initial = True
+class Migration(migrations.Migration):
 
     dependencies = [
         ('contenttypes', '0002_remove_content_type_name'),
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
+        ('django_audit_events', '0001_initial'),
     ]
 
     operations = [
         migrations.CreateModel(
-            name='AuditEvent',
+            name='ArchivedAuditEvent',
             fields=[
                 ('uuid', models.UUIDField(default=uuid.uuid4, primary_key=True, serialize=False, verbose_name='ID')),
-                ('timestamp', models.DateTimeField(auto_now_add=True, verbose_name='Timestamp')),
                 ('remote_addr', models.GenericIPAddressField(blank=True, null=True, verbose_name='IP address')),
                 ('url', models.URLField(blank=True, null=True, verbose_name='URL')),
-                ('query_params', django.contrib.postgres.fields.jsonb.JSONField(blank=True, default=dict, null=True, verbose_name='Query params')),
-                ('post_data', django.contrib.postgres.fields.jsonb.JSONField(blank=True, default=dict, null=True, verbose_name='Post data')),
+                ('query_params', JSONField(blank=True, default=dict, null=True, verbose_name='Query params')),
+                ('post_data', JSONField(blank=True, default=dict, null=True, verbose_name='Post data')),
                 ('object_id', models.PositiveIntegerField()),
-                ('content', django.contrib.postgres.fields.jsonb.JSONField(default=dict, verbose_name='Content')),
+                ('content', JSONField(default=dict, verbose_name='Content')),
+                ('timestamp', models.DateTimeField(verbose_name='Timestamp')),
+                ('archive_timestamp', models.DateTimeField(auto_now_add=True, verbose_name='Archive timestamp')),
                 ('content_type', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='contenttypes.ContentType')),
                 ('user', models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, to=settings.AUTH_USER_MODEL, verbose_name='User')),
             ],
             options={
                 'ordering': ('-timestamp',),
-                'verbose_name': 'Audit event',
-                'verbose_name_plural': 'Audit events',
                 'abstract': False,
-                'swappable': 'AUDIT_EVENT_MODEL',
+                'verbose_name': 'Archived audit event',
+                'swappable': 'AUDIT_EVENT_ARCHIVE_MODEL',
+                'verbose_name_plural': 'Archived audit events',
             },
         ),
     ]
```

### Comparing `django-audit-events-0.2b0/django_audit_events/mixin.py` & `django-audit-events-0.3.0/django_audit_events/mixin.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 from __future__ import unicode_literals
 
-from django.utils.translation import ugettext_lazy as _
+from distutils.version import StrictVersion
+
+import django
+
+if StrictVersion(django.get_version()) >= StrictVersion("2.0.0"):
+    from django.utils.translation import gettext_lazy as _
+else:
+    from django.utils.translation import ugettext_lazy as _
 
 from django_audit_events.context import AuditContext
 
 
 class AuditContextMixin(object):
     audit_context = AuditContext()
```

### Comparing `django-audit-events-0.2b0/django_audit_events/models.py` & `django-audit-events-0.3.0/django_audit_events/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,88 @@
 from __future__ import unicode_literals
 
+from distutils.version import StrictVersion
+
+import django
+
+if StrictVersion(django.get_version()) >= StrictVersion("2.0.0"):
+    from django.utils.translation import gettext_lazy as _
+else:
+    from django.utils.translation import ugettext_lazy as _
+
 import uuid
 
 from django.apps import apps
 from django.conf import settings as django_settings
 from django.contrib.contenttypes.fields import GenericForeignKey
 from django.contrib.contenttypes.models import ContentType
-from django.contrib.postgres.fields import JSONField
 from django.core.exceptions import ImproperlyConfigured
 from django.db import models
-from django.utils.translation import ugettext_lazy as _
 
 from django_audit_events.conf import settings
 
+try:
+    from django.db.models import JSONField
+except ImportError:
+    from django.contrib.postgres.fields import JSONField
+
 
 class AbstractAuditEvent(models.Model):
-    uuid = models.UUIDField(verbose_name=_("ID"), default=uuid.uuid4, primary_key=True,)
+    uuid = models.UUIDField(
+        verbose_name=_("ID"),
+        default=uuid.uuid4,
+        primary_key=True,
+    )
     timestamp = models.DateTimeField(verbose_name=_("Timestamp"), auto_now_add=True)
     user = models.ForeignKey(
         django_settings.AUTH_USER_MODEL,
         on_delete=models.SET_NULL,
         verbose_name=_("User"),
         blank=True,
         null=True,
     )
     remote_addr = models.GenericIPAddressField(
-        verbose_name=_("IP address"), blank=True, null=True,
+        verbose_name=_("IP address"),
+        blank=True,
+        null=True,
+    )
+    url = models.URLField(
+        verbose_name=_("URL"),
+        blank=True,
+        null=True,
+        max_length=1000,
     )
-    url = models.URLField(verbose_name=_("URL"), blank=True, null=True,)
     query_params = JSONField(
-        verbose_name=_("Query params"), default=dict, blank=True, null=True,
+        verbose_name=_("Query params"),
+        default=dict,
+        blank=True,
+        null=True,
     )
     post_data = JSONField(
-        verbose_name=_("Post data"), default=dict, blank=True, null=True,
+        verbose_name=_("Post data"),
+        default=dict,
+        blank=True,
+        null=True,
+    )
+    headers = JSONField(
+        verbose_name=_("Headers"),
+        default=dict,
+        blank=True,
+        null=True,
+    )
+    content_type = models.ForeignKey(
+        ContentType,
+        on_delete=models.CASCADE,
     )
-    content_type = models.ForeignKey(ContentType, on_delete=models.CASCADE,)
     object_id = models.PositiveIntegerField()
     content_object = GenericForeignKey("content_type", "object_id")
-    content = JSONField(verbose_name=_("Content"), default=dict,)
+    content = JSONField(
+        verbose_name=_("Content"),
+        default=dict,
+    )
 
     class Meta:
         verbose_name = _("Audit event")
         verbose_name_plural = _("Audit events")
         ordering = ("-timestamp",)
         abstract = True
 
@@ -57,14 +98,15 @@
 
         obj = cls()
         obj.user = context.user
         obj.remote_addr = context.remote_addr
         obj.url = context.url
         obj.query_params = context.query_params
         obj.post_data = context.post_data
+        obj.headers = context.headers
         return obj
 
     def as_archive_event(self):
         archive_model = get_audit_event_archive_model()
         fields = archive_model._meta.get_fields()
         return archive_model(
             **{field.name: getattr(self, field.name, None) for field in fields}
```

### Comparing `django-audit-events-0.2b0/django_audit_events/tasks.py` & `django-audit-events-0.3.0/django_audit_events/tasks.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,17 +24,29 @@
 
 @app.task
 def archive_old_audit_events(older_than=90):
     audit_event_model = get_audit_event_model()
     archived_audit_event_model = get_audit_event_archive_model()
 
     reference_date = timezone.now() - timedelta(days=older_than)
-    events_to_archive = audit_event_model.objects.filter(timestamp__lte=reference_date)
+    events_to_delete = set()
+
+    for event in audit_event_model.objects.iterator():
+        if event.content_object is None:
+            events_to_delete.add(event.uuid)
+
+    events_to_delete = list(events_to_delete)
 
+    for chunk in _chunks(events_to_delete):
+        with transaction.atomic():
+            audit_event_model.objects.filter(uuid__in=[e for e in chunk]).delete()
+
+    events_to_archive = audit_event_model.objects.filter(timestamp__lte=reference_date)
     archive_items = [event.as_archive_event() for event in events_to_archive]
 
     for chunk in _chunks(archive_items):
         with transaction.atomic():
             archived_audit_event_model.objects.bulk_create(chunk)
             audit_event_model.objects.filter(uuid__in=[e.uuid for e in chunk]).delete()
 
     logger.info("Archived %d audit events." % events_to_archive.count())
+    logger.info("Deleted %d audit events." % len(events_to_delete))
```

### Comparing `django-audit-events-0.2b0/django_audit_events/tests/test_middleware.py` & `django-audit-events-0.3.0/django_audit_events/tests/test_middleware.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,30 +5,33 @@
 
 from django_audit_events.middleware import AuditEventsMiddleware
 
 
 class MiddlewareTestMixin:
     request = HttpRequest()
 
+    def dummy_get_response(self):
+        return None
+
     def reset_request(self):
         self.request = HttpRequest()
         self.request.META = {"SERVER_NAME": "localhost", "SERVER_PORT": 80}
 
     def apply_middleware(self):
-        SessionMiddleware().process_request(self.request)
-        AuthenticationMiddleware().process_request(self.request)
-        AuditEventsMiddleware().process_request(self.request)
+        SessionMiddleware(self.dummy_get_response).process_request(self.request)
+        AuthenticationMiddleware(self.dummy_get_response).process_request(self.request)
+        AuditEventsMiddleware(self.dummy_get_response).process_request(self.request)
 
 
 class MiddlewareTestCase(TestCase, MiddlewareTestMixin):
     def setUp(self):
         self.reset_request()
 
     def test_without_authentication_middleware(self):
         with self.assertRaises(AssertionError):
-            AuditEventsMiddleware().process_request(self.request)
+            AuditEventsMiddleware(self.dummy_get_response).process_request(self.request)
 
     def test_with_authentication_middleware(self):
         self.apply_middleware()
         self.assertTrue(hasattr(self.request, "audit_context"))
         # noinspection PyUnresolvedReferences
         self.assertIsNotNone(self.request.audit_context)
```

### Comparing `django-audit-events-0.2b0/django_audit_events/tests/test_mixin.py` & `django-audit-events-0.3.0/django_audit_events/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.2b0/django_audit_events/tests/test_models.py` & `django-audit-events-0.3.0/django_audit_events/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.2b0/django_audit_events/tests/test_tasks.py` & `django-audit-events-0.3.0/django_audit_events/tests/test_tasks.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,34 +16,54 @@
         events = [
             baker.prepare(AuditEvent, content_object=baker.make(Poll))
             for _ in range(100)
         ]
         AuditEvent.objects.bulk_create(events)
         for event in events:
             event.timestamp = self.get_random_past_date()
-            event.save()
+            event.save(update_fields=["timestamp"])
+
+        for _ in range(25):
+            random_event = random.choice(events)
+
+            if random_event.content_object:
+                random_event.content_object.delete()
+            else:
+                random_event.save()
 
     def tearDown(self):
         AuditEvent.objects.all().delete()
         ArchivedAuditEvent.objects.all().delete()
 
     @override_settings(CELERY_ALWAYS_EAGER=True)
     def test_archiver_task(self):
         older_than = 90
         query = Q(timestamp__lte=timezone.now() - timedelta(days=older_than))
-        events_to_archive = AuditEvent.objects.filter(query)
+        events_to_delete = set()
+
+        for event in AuditEvent.objects.iterator():
+            if event.content_object is None:
+                events_to_delete.add(event.uuid)
+
+        events_to_archive = AuditEvent.objects.filter(query).exclude(
+            uuid__in=events_to_delete
+        )
         uuids = set([e.uuid for e in events_to_archive])
 
         archive_old_audit_events(older_than=older_than)
 
         archived_events = ArchivedAuditEvent.objects.all()
         archived_uuids = set([e.uuid for e in archived_events])
         self.assertEqual(len(events_to_archive), len(archived_events))
         self.assertSetEqual(uuids, archived_uuids)
         self.assertFalse(AuditEvent.objects.filter(uuid__in=archived_uuids).exists())
+        self.assertFalse(
+            ArchivedAuditEvent.objects.filter(uuid__in=events_to_delete).exists()
+        )
+        self.assertFalse(AuditEvent.objects.filter(uuid__in=events_to_delete).exists())
 
     def get_random_past_date(self, base=timezone.now, date_range=timedelta(days=365)):
         if callable(base):
             base = base()
         seconds = date_range.total_seconds()
         minus_seconds = random.randint(0, seconds)
         return base - timedelta(seconds=minus_seconds)
```

### Comparing `django-audit-events-0.2b0/django_audit_events/views.py` & `django-audit-events-0.3.0/django_audit_events/views.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,29 @@
 from django.db.models import ForeignObject, ManyToManyField
 from rest_framework import viewsets
 
 from django_audit_events.filters import AuditEventFilterSet
 from django_audit_events.models import get_audit_event_model
 from django_audit_events.serializers import EventSerializer
 
-AuditEvent = get_audit_event_model()
-
 
 class AuditEventViewSet(viewsets.ReadOnlyModelViewSet):
-    queryset = AuditEvent.objects.all()
+    queryset = get_audit_event_model().objects.all()
     filter_class = AuditEventFilterSet
-
-    def __new__(cls, *args, **kwargs):
-        obj = super(AuditEventViewSet, cls).__new__(cls, *args, **kwargs)
-        obj.filter_class.Meta.model = AuditEvent
-        return obj
-
-    # noinspection PyMethodMayBeStatic
-    def get_serializer_class(self, *args, **kwargs):
-        EventSerializer.Meta.model = AuditEvent
-        return EventSerializer
+    serializer_class = EventSerializer
 
     def get_queryset(self):
+        queryset = super(AuditEventViewSet, self).get_queryset()
         # noinspection PyProtectedMember
-        fields = AuditEvent._meta.local_fields
+        fields = queryset.model._meta.local_fields
         select_related = []
         prefetch_related = []
 
         for field in fields:
             if isinstance(field, ForeignObject):
                 select_related.append(field.name)
             elif isinstance(field, ManyToManyField):
                 prefetch_related.append(field.name)
 
-        queryset = super(AuditEventViewSet, self).get_queryset()
         return queryset.select_related(*select_related).prefetch_related(
             *prefetch_related
         )
```

### Comparing `django-audit-events-0.2b0/django_audit_events.egg-info/PKG-INFO` & `django-audit-events-0.3.0/django_audit_events.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,70 +1,79 @@
 Metadata-Version: 2.1
 Name: django-audit-events
-Version: 0.2b0
+Version: 0.3.0
 Summary: Log audit events in Django
 Home-page: https://bitbucket.org/akinonteam/django-audit-events
 Author: Onur Güzel
 Author-email: dev@akinon.com
 Maintainer: Akinon
 Maintainer-email: dev@akinon.com
 License: MIT
 Project-URL: Documentation, https://django-audit-events.readthedocs.io/
 Project-URL: Source Code, https://bitbucket.org/akinonteam/django-audit-events
-Description: # Django Audit Events
-        
-        [![Build status](https://img.shields.io/bitbucket/pipelines/akinonteam/django-audit-events)](https://bitbucket.org/akinonteam/django-audit-events/addon/pipelines/home)
-        [![Documentation status](https://readthedocs.org/projects/django-audit-events/badge/?version=latest)](https://django-audit-events.readthedocs.io/en/latest/?badge=latest)
-        ![PyPI](https://img.shields.io/pypi/v/django-audit-events)
-        ![PyPI - Django version](https://img.shields.io/pypi/djversions/django-audit-events)
-        ![PyPI - Python version](https://img.shields.io/pypi/pyversions/django-audit-events)
-        ![PyPI - License](https://img.shields.io/pypi/l/django-audit-events)
-        [![Total alerts](https://img.shields.io/lgtm/alerts/bitbucket/akinonteam/django-audit-events)](https://lgtm.com/projects/b/akinonteam/django-audit-events/alerts/)
-        [![Code quality](https://img.shields.io/lgtm/grade/python/bitbucket/akinonteam/django-audit-events)](https://lgtm.com/projects/b/akinonteam/django-audit-events/context:python)
-        
-        Extensible custom audit events for humans! This Django app allows you to easily create your own events in your project. Currently only works on PostgreSQL.
-        
-        Let's have a look:
-        
-        ```python
-        def awesome_view(request):
-            foo_obj = Foo.objects.get(pk=1)
-            # Do something with foo_obj...
-            request.audit_context.create_event(
-                foo_obj,
-                something="done",
-                bar="baz"
-            )
-        ```
-        
-        This will create an audit event, including the request URL, logged-in user, remote IP address, and the following event content:
-        
-        ```
-        >>> event.content
-        {"something": "done", "bar: "baz"}
-        ```
-        
-        For more information about installation and usage, check out the [documentation](https://django-audit-events.readthedocs.io/)!
-        
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.10
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 3.1
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# Django Audit Events
+
+[![Build status](https://img.shields.io/bitbucket/pipelines/akinonteam/django-audit-events)](https://bitbucket.org/akinonteam/django-audit-events/addon/pipelines/home)
+[![Documentation status](https://readthedocs.org/projects/django-audit-events/badge/?version=latest)](https://django-audit-events.readthedocs.io/en/latest/?badge=latest)
+![PyPI](https://img.shields.io/pypi/v/django-audit-events)
+![PyPI - Django version](https://img.shields.io/pypi/djversions/django-audit-events)
+![PyPI - Python version](https://img.shields.io/pypi/pyversions/django-audit-events)
+![PyPI - License](https://img.shields.io/pypi/l/django-audit-events)
+[![Total alerts](https://img.shields.io/lgtm/alerts/bitbucket/akinonteam/django-audit-events)](https://lgtm.com/projects/b/akinonteam/django-audit-events/alerts/)
+[![Code quality](https://img.shields.io/lgtm/grade/python/bitbucket/akinonteam/django-audit-events)](https://lgtm.com/projects/b/akinonteam/django-audit-events/context:python)
+
+Extensible custom audit events for humans! This Django app allows you to easily create your own events in your project. Currently only works on PostgreSQL.
+
+Let's have a look:
+
+```python
+def awesome_view(request):
+    foo_obj = Foo.objects.get(pk=1)
+    # Do something with foo_obj...
+    request.audit_context.create_event(
+        foo_obj,
+        something="done",
+        bar="baz"
+    )
+```
+
+This will create an audit event, including the request URL, logged-in user, remote IP address, and the following event content:
+
+```
+>>> event.content
+{"something": "done", "bar: "baz"}
+```
+
+For more information about installation and usage, check out the [documentation](https://django-audit-events.readthedocs.io/)!
```

### Comparing `django-audit-events-0.2b0/django_audit_events.egg-info/SOURCES.txt` & `django-audit-events-0.3.0/django_audit_events.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -18,23 +18,29 @@
 django_audit_events/filters.py
 django_audit_events/middleware.py
 django_audit_events/mixin.py
 django_audit_events/models.py
 django_audit_events/serializers.py
 django_audit_events/tasks.py
 django_audit_events/urls.py
+django_audit_events/utils.py
 django_audit_events/version.py
 django_audit_events/views.py
 django_audit_events.egg-info/PKG-INFO
 django_audit_events.egg-info/SOURCES.txt
 django_audit_events.egg-info/dependency_links.txt
 django_audit_events.egg-info/not-zip-safe
 django_audit_events.egg-info/top_level.txt
 django_audit_events/locale/tr/LC_MESSAGES/django.po
 django_audit_events/migrations/0001_initial.py
+django_audit_events/migrations/0002_archivedauditevent.py
+django_audit_events/migrations/0003_auto_20201218_1113.py
+django_audit_events/migrations/0004_auto_20210127_2021.py
+django_audit_events/migrations/0005_auto_20220215_0756.py
+django_audit_events/migrations/0006_auto_20220920_1327.py
 django_audit_events/migrations/__init__.py
 django_audit_events/tests/__init__.py
 django_audit_events/tests/test_conf.py
 django_audit_events/tests/test_context.py
 django_audit_events/tests/test_middleware.py
 django_audit_events/tests/test_mixin.py
 django_audit_events/tests/test_models.py
```

### Comparing `django-audit-events-0.2b0/docs/Makefile` & `django-audit-events-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.2b0/docs/advanced.rst` & `django-audit-events-0.3.0/docs/advanced.rst`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.2b0/docs/conf.py` & `django-audit-events-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.2b0/docs/index.rst` & `django-audit-events-0.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.2b0/docs/introduction.rst` & `django-audit-events-0.3.0/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.2b0/docs/make.bat` & `django-audit-events-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.2b0/docs/quickstart.rst` & `django-audit-events-0.3.0/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.2b0/runtests.py` & `django-audit-events-0.3.0/runtests.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import logging
 import sys
 from os.path import dirname
 
 import django
 from django.conf import settings
+from django.test.utils import get_runner
 from django.test.runner import DiscoverRunner
 
 sys.path.insert(0, dirname(__file__))
 
 installed_apps = [
     "django.contrib.contenttypes",
     "django.contrib.auth",
@@ -27,17 +28,19 @@
         return True
 
     def __getitem__(self, item):
         return None
 
 
 DEFAULT_SETTINGS = dict(
+    SECRET_KEY='SECRET',
     ALLOWED_HOSTS=["localhost"],
     ROOT_URLCONF="django_audit_events.tests.urls",
     INSTALLED_APPS=installed_apps,
+    DEFAULT_AUTO_FIELD="django.db.models.AutoField",
     DATABASES={
         "default": {
             "ENGINE": "django.db.backends.postgresql",
             "NAME": "postgres",
             "USER": "postgres",
             "PASSWORD": "postgres",
             "HOST": "localhost",
```

### Comparing `django-audit-events-0.2b0/setup.py` & `django-audit-events-0.3.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -53,21 +53,29 @@
         "Framework :: Django",
         "Framework :: Django :: 1.10",
         "Framework :: Django :: 1.11",
         "Framework :: Django :: 2.0",
         "Framework :: Django :: 2.1",
         "Framework :: Django :: 2.2",
         "Framework :: Django :: 3.0",
+        "Framework :: Django :: 3.1",
+        "Framework :: Django :: 3.2",
+        "Framework :: Django :: 4.0",
+        "Framework :: Django :: 4.1",
+        "Framework :: Django :: 4.2",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

