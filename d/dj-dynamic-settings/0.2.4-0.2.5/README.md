# Comparing `tmp/dj-dynamic-settings-0.2.4.tar.gz` & `tmp/dj-dynamic-settings-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj-dynamic-settings-0.2.4.tar", last modified: Mon Nov 27 11:17:57 2023, max compression
+gzip compressed data, was "dist/dj-dynamic-settings-0.2.5.tar", last modified: Mon May  6 06:45:22 2024, max compression
```

## Comparing `dj-dynamic-settings-0.2.4.tar` & `dj-dynamic-settings-0.2.5.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-27 11:17:57.385698 dj-dynamic-settings-0.2.4/
--rw-rw-rw-   0 root         (0) root         (0)     1304 2023-11-27 11:17:32.000000 dj-dynamic-settings-0.2.4/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-11-27 11:17:32.000000 dj-dynamic-settings-0.2.4/.isort.cfg
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-11-27 11:17:32.000000 dj-dynamic-settings-0.2.4/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)     1050 2023-11-27 11:17:32.000000 dj-dynamic-settings-0.2.4/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)     4609 2023-11-27 11:17:57.385698 dj-dynamic-settings-0.2.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3305 2023-11-27 11:17:32.000000 dj-dynamic-settings-0.2.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2435 2023-11-27 11:17:32.000000 dj-dynamic-settings-0.2.4/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-27 11:17:57.381698 dj-dynamic-settings-0.2.4/dj_dynamic_settings/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-27 11:17:32.000000 dj-dynamic-settings-0.2.4/dj_dynamic_settings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-11-27 11:17:32.000000 dj-dynamic-settings-0.2.4/dj_dynamic_settings/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      771 2023-11-27 11:17:32.000000 dj-dynamic-settings-0.2.4/dj_dynamic_settings/app_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      152 2023-11-27 11:17:32.000000 dj-dynamic-settings-0.2.4/dj_dynamic_settings/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      602 2023-11-27 11:17:32.000000 dj-dynamic-settings-0.2.4/dj_dynamic_settings/compat.py
--rw-rw-rw-   0 root         (0) root         (0)     3093 2023-11-27 11:17:32.000000 dj-dynamic-settings-0.2.4/dj_dynamic_settings/conf.py
--rw-rw-rw-   0 root         (0) root         (0)       52 2023-11-27 11:17:32.000000 dj-dynamic-settings-0.2.4/dj_dynamic_settings/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)      811 2023-11-27 11:17:32.000000 dj-dynamic-settings-0.2.4/dj_dynamic_settings/metadata.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-27 11:17:57.381698 dj-dynamic-settings-0.2.4/dj_dynamic_settings/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      970 2023-11-27 11:17:32.000000 dj-dynamic-settings-0.2.4/dj_dynamic_settings/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-27 11:17:32.000000 dj-dynamic-settings-0.2.4/dj_dynamic_settings/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1215 2023-11-27 11:17:32.000000 dj-dynamic-settings-0.2.4/dj_dynamic_settings/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1352 2023-11-27 11:17:32.000000 dj-dynamic-settings-0.2.4/dj_dynamic_settings/registry.py
--rw-rw-rw-   0 root         (0) root         (0)     2515 2023-11-27 11:17:32.000000 dj-dynamic-settings-0.2.4/dj_dynamic_settings/serializers.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-27 11:17:57.385698 dj-dynamic-settings-0.2.4/dj_dynamic_settings/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-27 11:17:32.000000 dj-dynamic-settings-0.2.4/dj_dynamic_settings/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1790 2023-11-27 11:17:32.000000 dj-dynamic-settings-0.2.4/dj_dynamic_settings/tests/definitions.py
--rw-rw-rw-   0 root         (0) root         (0)     4250 2023-11-27 11:17:32.000000 dj-dynamic-settings-0.2.4/dj_dynamic_settings/tests/test_dynamic_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     2377 2023-11-27 11:17:32.000000 dj-dynamic-settings-0.2.4/dj_dynamic_settings/tests/test_override_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      573 2023-11-27 11:17:32.000000 dj-dynamic-settings-0.2.4/dj_dynamic_settings/tests/test_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     4014 2023-11-27 11:17:32.000000 dj-dynamic-settings-0.2.4/dj_dynamic_settings/tests/test_views.py
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-11-27 11:17:32.000000 dj-dynamic-settings-0.2.4/dj_dynamic_settings/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      630 2023-11-27 11:17:32.000000 dj-dynamic-settings-0.2.4/dj_dynamic_settings/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3550 2023-11-27 11:17:32.000000 dj-dynamic-settings-0.2.4/dj_dynamic_settings/validators.py
--rw-rw-rw-   0 root         (0) root         (0)     1004 2023-11-27 11:17:32.000000 dj-dynamic-settings-0.2.4/dj_dynamic_settings/views.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-27 11:17:57.381698 dj-dynamic-settings-0.2.4/dj_dynamic_settings.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4609 2023-11-27 11:17:57.000000 dj-dynamic-settings-0.2.4/dj_dynamic_settings.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1176 2023-11-27 11:17:57.000000 dj-dynamic-settings-0.2.4/dj_dynamic_settings.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-11-27 11:17:57.000000 dj-dynamic-settings-0.2.4/dj_dynamic_settings.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-11-27 11:17:57.000000 dj-dynamic-settings-0.2.4/dj_dynamic_settings.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       20 2023-11-27 11:17:57.000000 dj-dynamic-settings-0.2.4/dj_dynamic_settings.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      302 2023-11-27 11:17:32.000000 dj-dynamic-settings-0.2.4/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       42 2023-11-27 11:17:32.000000 dj-dynamic-settings-0.2.4/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      430 2023-11-27 11:17:32.000000 dj-dynamic-settings-0.2.4/runtests.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-11-27 11:17:57.385698 dj-dynamic-settings-0.2.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2105 2023-11-27 11:17:32.000000 dj-dynamic-settings-0.2.4/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1253 2023-11-27 11:17:32.000000 dj-dynamic-settings-0.2.4/tox.ini
+drwxrwxr-x   0 ozkok     (1000) ozkok     (1000)        0 2024-05-06 06:45:22.000000 dj-dynamic-settings-0.2.5/
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1304 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/.gitignore
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      113 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/.isort.cfg
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)       28 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/CHANGELOG.md
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1050 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/LICENSE.txt
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     4765 2024-05-06 06:45:22.000000 dj-dynamic-settings-0.2.5/PKG-INFO
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     3305 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/README.md
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     2629 2024-04-30 14:37:07.000000 dj-dynamic-settings-0.2.5/bitbucket-pipelines.yml
+drwxrwxr-x   0 ozkok     (1000) ozkok     (1000)        0 2024-05-06 06:45:22.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)        0 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/__init__.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)       63 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/admin.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      856 2024-04-30 16:15:59.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/app_settings.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      152 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/apps.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      602 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/compat.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     3093 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/conf.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)       52 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/exceptions.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      811 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/metadata.py
+drwxrwxr-x   0 ozkok     (1000) ozkok     (1000)        0 2024-05-06 06:45:22.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/migrations/
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      970 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/migrations/0001_initial.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)        0 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/migrations/__init__.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1215 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/models.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1352 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/registry.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     2515 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/serializers.py
+drwxrwxr-x   0 ozkok     (1000) ozkok     (1000)        0 2024-05-06 06:45:22.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/tests/
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)        0 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/tests/__init__.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1790 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/tests/definitions.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     4250 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/tests/test_dynamic_settings.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     2377 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/tests/test_override_settings.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      624 2024-04-30 16:24:36.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/tests/test_settings.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     4014 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/tests/test_views.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      225 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/urls.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      630 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/utils.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     3550 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/validators.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1004 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/views.py
+drwxrwxr-x   0 ozkok     (1000) ozkok     (1000)        0 2024-05-06 06:45:22.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings.egg-info/
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     4765 2024-05-06 06:45:22.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings.egg-info/PKG-INFO
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1176 2024-05-06 06:45:22.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings.egg-info/SOURCES.txt
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)        1 2024-05-06 06:45:22.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings.egg-info/dependency_links.txt
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)        1 2024-05-06 06:45:22.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings.egg-info/not-zip-safe
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)       20 2024-05-06 06:45:22.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings.egg-info/top_level.txt
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      302 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/pyproject.toml
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)       42 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/requirements.txt
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      430 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/runtests.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)       38 2024-05-06 06:45:22.000000 dj-dynamic-settings-0.2.5/setup.cfg
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     2257 2024-04-30 14:37:07.000000 dj-dynamic-settings-0.2.5/setup.py
+-rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1385 2024-04-30 14:43:01.000000 dj-dynamic-settings-0.2.5/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `dj-dynamic-settings-0.2.4/.gitignore` & `dj-dynamic-settings-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.4/LICENSE.txt` & `dj-dynamic-settings-0.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.4/PKG-INFO` & `dj-dynamic-settings-0.2.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-dynamic-settings
-Version: 0.2.4
+Version: 0.2.5
 Summary: Stay informed of it
 Home-page: https://bitbucket.org/akinonteam/dj-dynamic-settings/
 Author: Akinon
 Author-email: dev@akinon.com
 Maintainer: Akinon
 Maintainer-email: dev@akinon.com
 License: MIT
@@ -25,14 +25,18 @@
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.10
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Django Dynamic Settings
 
 [![Build status](https://img.shields.io/bitbucket/pipelines/akinonteam/dj-dynamic-settings)](https://bitbucket.org/akinonteam/dj-dynamic-settings/addon/pipelines/home)
 ![PyPI](https://img.shields.io/pypi/v/dj-dynamic-settings)
```

### Comparing `dj-dynamic-settings-0.2.4/README.md` & `dj-dynamic-settings-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.4/bitbucket-pipelines.yml` & `dj-dynamic-settings-0.2.5/bitbucket-pipelines.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,70 +1,71 @@
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
+            - tox -e py38-django22,py38-django30,py38-django32,py38-django40,py38-django41,py38-django42
+          services:
+            - postgres
   tags:
     '*':
       - step:
           name: Publish to PyPI
           image: python:3.8-alpine
           script:
             - apk add gcc git libffi-dev musl-dev openssl-dev python3-dev
```

### Comparing `dj-dynamic-settings-0.2.4/dj_dynamic_settings/app_settings.py` & `dj-dynamic-settings-0.2.5/dj_dynamic_settings/app_settings.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from django.conf import settings
 from django.core.cache import DEFAULT_CACHE_ALIAS
 
 __all__ = ["app_settings"]
 
+from django.db import models
 
 defaults = {
     "CACHE_KEY_PREFIX": "dynamic-settings",
     "CACHE_ALIAS": DEFAULT_CACHE_ALIAS,
     "USE_CACHE": True,
     "CACHE_TIMEOUT": 1 * 60 * 60,
+    "DEFAULT_AUTO_FIELD": "django.db.models.AutoField",
 }
 
 
 class AppSettings(object):
     def __init__(self, prefix):
         self._prefix = prefix
```

### Comparing `dj-dynamic-settings-0.2.4/dj_dynamic_settings/compat.py` & `dj-dynamic-settings-0.2.5/dj_dynamic_settings/compat.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.4/dj_dynamic_settings/conf.py` & `dj-dynamic-settings-0.2.5/dj_dynamic_settings/conf.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.4/dj_dynamic_settings/metadata.py` & `dj-dynamic-settings-0.2.5/dj_dynamic_settings/metadata.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.4/dj_dynamic_settings/migrations/0001_initial.py` & `dj-dynamic-settings-0.2.5/dj_dynamic_settings/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.4/dj_dynamic_settings/models.py` & `dj-dynamic-settings-0.2.5/dj_dynamic_settings/models.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.4/dj_dynamic_settings/registry.py` & `dj-dynamic-settings-0.2.5/dj_dynamic_settings/registry.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.4/dj_dynamic_settings/serializers.py` & `dj-dynamic-settings-0.2.5/dj_dynamic_settings/serializers.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.4/dj_dynamic_settings/tests/definitions.py` & `dj-dynamic-settings-0.2.5/dj_dynamic_settings/tests/definitions.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.4/dj_dynamic_settings/tests/test_dynamic_settings.py` & `dj-dynamic-settings-0.2.5/dj_dynamic_settings/tests/test_dynamic_settings.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.4/dj_dynamic_settings/tests/test_override_settings.py` & `dj-dynamic-settings-0.2.5/dj_dynamic_settings/tests/test_override_settings.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.4/dj_dynamic_settings/tests/test_settings.py` & `dj-dynamic-settings-0.2.5/dj_dynamic_settings/tests/test_settings.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,14 +4,16 @@
     "django.contrib.auth",
     "django.contrib.contenttypes",
     "django.contrib.sessions",
     "django.contrib.messages",
     "dj_dynamic_settings",
 ]
 
+DEFAULT_AUTO_FIELD = "django.db.models.AutoField"
+
 DATABASES = {
     "default": {
         "ENGINE": "django.db.backends.postgresql",
         "NAME": "postgres",
         "USER": "postgres",
         "PASSWORD": "postgres",
         "HOST": "localhost",
```

### Comparing `dj-dynamic-settings-0.2.4/dj_dynamic_settings/tests/test_views.py` & `dj-dynamic-settings-0.2.5/dj_dynamic_settings/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.4/dj_dynamic_settings/utils.py` & `dj-dynamic-settings-0.2.5/dj_dynamic_settings/utils.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.4/dj_dynamic_settings/validators.py` & `dj-dynamic-settings-0.2.5/dj_dynamic_settings/validators.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.4/dj_dynamic_settings/views.py` & `dj-dynamic-settings-0.2.5/dj_dynamic_settings/views.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.4/dj_dynamic_settings.egg-info/PKG-INFO` & `dj-dynamic-settings-0.2.5/dj_dynamic_settings.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-dynamic-settings
-Version: 0.2.4
+Version: 0.2.5
 Summary: Stay informed of it
 Home-page: https://bitbucket.org/akinonteam/dj-dynamic-settings/
 Author: Akinon
 Author-email: dev@akinon.com
 Maintainer: Akinon
 Maintainer-email: dev@akinon.com
 License: MIT
@@ -25,14 +25,18 @@
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.10
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Django Dynamic Settings
 
 [![Build status](https://img.shields.io/bitbucket/pipelines/akinonteam/dj-dynamic-settings)](https://bitbucket.org/akinonteam/dj-dynamic-settings/addon/pipelines/home)
 ![PyPI](https://img.shields.io/pypi/v/dj-dynamic-settings)
```

### Comparing `dj-dynamic-settings-0.2.4/dj_dynamic_settings.egg-info/SOURCES.txt` & `dj-dynamic-settings-0.2.5/dj_dynamic_settings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.4/tox.ini` & `dj-dynamic-settings-0.2.5/tox.ini`

 * *Files 27% similar despite different names*

```diff
@@ -6,32 +6,35 @@
 [tox]
 isolated_build = True
 skip_missing_interpreters = True
 envlist = py27-{django110,django111}
           py34-{django110,django111,django20}
           py35-{django110,django111,django20,django21,django22}
           {py36,py37}-{django111,django20,django21,django22,django30,django31,django32}
-          py38-{django22,django30,django31,django32}
+          py38-{django22,django30,django31,django32, django40, django41, django42}
           linting
 
 [testenv]
 deps = django110: Django>=1.10,<1.11
        django111: Django>=1.11.7,<2.0
        django20: Django>=2.0,<2.1
        django21: Django>=2.1,<2.2
        django22: Django>=2.2.8,<3.0
        django30: Django>=3.0,<3.1
        django31: Django>=3.1,<3.2
-       django32: Django>=3.2
-       djangorestframework<3.12
+       django32: Django>=3.2,<4.0
+       django40: Django>=4.0,<4.1
+       django41: Django>=4.1,<4.2
+       django42: Django>=4.2
+       djangorestframework<3.15
        psycopg2-binary
        pytz
        mock
 commands = python runtests.py
 
 [testenv:linting]
 deps = black
        isort==5.0.4
        Django>=2.2.8,<3.0
-       djangorestframework<3.12
+       djangorestframework<3.15
 commands = black --check --quiet --exclude=migrations/ dj_dynamic_settings
            isort -c --skip=migrations dj_dynamic_settings
```

