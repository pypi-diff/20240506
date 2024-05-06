# Comparing `tmp/kiwitcms-github-app-1.6.0.tar.gz` & `tmp/kiwitcms-github-app-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiwitcms-github-app-1.6.0.tar", last modified: Mon Jan 15 15:56:19 2024, max compression
+gzip compressed data, was "kiwitcms-github-app-1.7.0.tar", last modified: Mon May  6 10:07:42 2024, max compression
```

## Comparing `kiwitcms-github-app-1.6.0.tar` & `kiwitcms-github-app-1.7.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-01-15 15:56:19.400016 kiwitcms-github-app-1.6.0/
--rw-rw-r--   0 senko     (1001) senko     (1001)    35149 2021-04-27 19:25:12.000000 kiwitcms-github-app-1.6.0/LICENSE
--rw-rw-r--   0 senko     (1001) senko     (1001)      122 2021-04-27 19:25:12.000000 kiwitcms-github-app-1.6.0/MANIFEST.in
--rw-r--r--   0 senko     (1001) senko     (1001)     9379 2024-01-15 15:56:19.400016 kiwitcms-github-app-1.6.0/PKG-INFO
--rw-r--r--   0 senko     (1001) senko     (1001)     8364 2024-01-15 15:56:01.000000 kiwitcms-github-app-1.6.0/README.rst
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-01-15 15:56:19.400016 kiwitcms-github-app-1.6.0/kiwitcms_github_app.egg-info/
--rw-r--r--   0 senko     (1001) senko     (1001)     9379 2024-01-15 15:56:19.000000 kiwitcms-github-app-1.6.0/kiwitcms_github_app.egg-info/PKG-INFO
--rw-r--r--   0 senko     (1001) senko     (1001)      851 2024-01-15 15:56:19.000000 kiwitcms-github-app-1.6.0/kiwitcms_github_app.egg-info/SOURCES.txt
--rw-r--r--   0 senko     (1001) senko     (1001)        1 2024-01-15 15:56:19.000000 kiwitcms-github-app-1.6.0/kiwitcms_github_app.egg-info/dependency_links.txt
--rw-r--r--   0 senko     (1001) senko     (1001)       57 2024-01-15 15:56:19.000000 kiwitcms-github-app-1.6.0/kiwitcms_github_app.egg-info/entry_points.txt
--rw-r--r--   0 senko     (1001) senko     (1001)        1 2024-01-15 15:56:19.000000 kiwitcms-github-app-1.6.0/kiwitcms_github_app.egg-info/not-zip-safe
--rw-r--r--   0 senko     (1001) senko     (1001)      134 2024-01-15 15:56:19.000000 kiwitcms-github-app-1.6.0/kiwitcms_github_app.egg-info/requires.txt
--rw-r--r--   0 senko     (1001) senko     (1001)       34 2024-01-15 15:56:19.000000 kiwitcms-github-app-1.6.0/kiwitcms_github_app.egg-info/top_level.txt
--rw-r--r--   0 senko     (1001) senko     (1001)      394 2024-01-15 11:48:13.000000 kiwitcms-github-app-1.6.0/requirements.txt
--rw-r--r--   0 senko     (1001) senko     (1001)       38 2024-01-15 15:56:19.400016 kiwitcms-github-app-1.6.0/setup.cfg
--rw-r--r--   0 senko     (1001) senko     (1001)     1703 2024-01-15 15:56:01.000000 kiwitcms-github-app-1.6.0/setup.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-01-15 15:56:19.399016 kiwitcms-github-app-1.6.0/tcms_github_app/
--rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-04-27 19:25:12.000000 kiwitcms-github-app-1.6.0/tcms_github_app/__init__.py
--rw-r--r--   0 senko     (1001) senko     (1001)     5736 2024-01-14 21:43:45.000000 kiwitcms-github-app-1.6.0/tcms_github_app/admin.py
--rw-r--r--   0 senko     (1001) senko     (1001)     3509 2024-01-14 21:43:45.000000 kiwitcms-github-app-1.6.0/tcms_github_app/issues.py
--rw-r--r--   0 senko     (1001) senko     (1001)      467 2024-01-14 21:43:45.000000 kiwitcms-github-app-1.6.0/tcms_github_app/menu.py
--rw-r--r--   0 senko     (1001) senko     (1001)     1781 2024-01-14 21:43:45.000000 kiwitcms-github-app-1.6.0/tcms_github_app/middleware.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-01-15 15:56:19.400016 kiwitcms-github-app-1.6.0/tcms_github_app/migrations/
--rw-r--r--   0 senko     (1001) senko     (1001)     2083 2024-01-14 21:43:45.000000 kiwitcms-github-app-1.6.0/tcms_github_app/migrations/0001_initial.py
--rw-r--r--   0 senko     (1001) senko     (1001)     1192 2024-01-14 21:43:45.000000 kiwitcms-github-app-1.6.0/tcms_github_app/migrations/0002_appinstallation_settings_url.py
--rw-r--r--   0 senko     (1001) senko     (1001)      659 2024-01-14 21:43:45.000000 kiwitcms-github-app-1.6.0/tcms_github_app/migrations/0003_models_jsonfield.py
--rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-04-27 19:25:12.000000 kiwitcms-github-app-1.6.0/tcms_github_app/migrations/__init__.py
--rw-r--r--   0 senko     (1001) senko     (1001)     1875 2024-01-14 21:43:45.000000 kiwitcms-github-app-1.6.0/tcms_github_app/models.py
--rw-r--r--   0 senko     (1001) senko     (1001)      468 2024-01-14 21:43:45.000000 kiwitcms-github-app-1.6.0/tcms_github_app/urls.py
--rw-r--r--   0 senko     (1001) senko     (1001)    11443 2024-01-14 21:43:45.000000 kiwitcms-github-app-1.6.0/tcms_github_app/utils.py
--rw-r--r--   0 senko     (1001) senko     (1001)     6473 2024-01-14 21:43:45.000000 kiwitcms-github-app-1.6.0/tcms_github_app/views.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-01-15 15:56:19.400016 kiwitcms-github-app-1.6.0/tcms_settings_dir/
--rw-r--r--   0 senko     (1001) senko     (1001)       65 2024-01-14 21:43:45.000000 kiwitcms-github-app-1.6.0/tcms_settings_dir/__init__.py
--rw-r--r--   0 senko     (1001) senko     (1001)      525 2024-01-14 21:43:45.000000 kiwitcms-github-app-1.6.0/tcms_settings_dir/github_app.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-06 10:07:42.509008 kiwitcms-github-app-1.7.0/
+-rw-rw-r--   0 senko     (1001) senko     (1001)    35149 2021-04-27 19:25:12.000000 kiwitcms-github-app-1.7.0/LICENSE
+-rw-rw-r--   0 senko     (1001) senko     (1001)      122 2021-04-27 19:25:12.000000 kiwitcms-github-app-1.7.0/MANIFEST.in
+-rw-r--r--   0 senko     (1001) senko     (1001)     9469 2024-05-06 10:07:42.509008 kiwitcms-github-app-1.7.0/PKG-INFO
+-rw-r--r--   0 senko     (1001) senko     (1001)     8693 2024-05-06 10:07:29.000000 kiwitcms-github-app-1.7.0/README.rst
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-06 10:07:42.508008 kiwitcms-github-app-1.7.0/kiwitcms_github_app.egg-info/
+-rw-r--r--   0 senko     (1001) senko     (1001)     9469 2024-05-06 10:07:42.000000 kiwitcms-github-app-1.7.0/kiwitcms_github_app.egg-info/PKG-INFO
+-rw-r--r--   0 senko     (1001) senko     (1001)      851 2024-05-06 10:07:42.000000 kiwitcms-github-app-1.7.0/kiwitcms_github_app.egg-info/SOURCES.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)        1 2024-05-06 10:07:42.000000 kiwitcms-github-app-1.7.0/kiwitcms_github_app.egg-info/dependency_links.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)       57 2024-05-06 10:07:42.000000 kiwitcms-github-app-1.7.0/kiwitcms_github_app.egg-info/entry_points.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)        1 2024-05-06 10:07:42.000000 kiwitcms-github-app-1.7.0/kiwitcms_github_app.egg-info/not-zip-safe
+-rw-r--r--   0 senko     (1001) senko     (1001)      150 2024-05-06 10:07:42.000000 kiwitcms-github-app-1.7.0/kiwitcms_github_app.egg-info/requires.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)       34 2024-05-06 10:07:42.000000 kiwitcms-github-app-1.7.0/kiwitcms_github_app.egg-info/top_level.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)      475 2024-05-05 18:05:46.000000 kiwitcms-github-app-1.7.0/requirements.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)       38 2024-05-06 10:07:42.509008 kiwitcms-github-app-1.7.0/setup.cfg
+-rw-r--r--   0 senko     (1001) senko     (1001)     1703 2024-05-06 10:07:29.000000 kiwitcms-github-app-1.7.0/setup.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-06 10:07:42.508008 kiwitcms-github-app-1.7.0/tcms_github_app/
+-rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-04-27 19:25:12.000000 kiwitcms-github-app-1.7.0/tcms_github_app/__init__.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     5736 2024-05-05 19:06:58.000000 kiwitcms-github-app-1.7.0/tcms_github_app/admin.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     1492 2024-05-06 06:50:57.000000 kiwitcms-github-app-1.7.0/tcms_github_app/issues.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      467 2024-05-05 19:06:58.000000 kiwitcms-github-app-1.7.0/tcms_github_app/menu.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     1781 2024-05-05 19:06:58.000000 kiwitcms-github-app-1.7.0/tcms_github_app/middleware.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-06 10:07:42.509008 kiwitcms-github-app-1.7.0/tcms_github_app/migrations/
+-rw-r--r--   0 senko     (1001) senko     (1001)     2083 2024-05-05 19:06:58.000000 kiwitcms-github-app-1.7.0/tcms_github_app/migrations/0001_initial.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     1192 2024-05-05 19:06:58.000000 kiwitcms-github-app-1.7.0/tcms_github_app/migrations/0002_appinstallation_settings_url.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      659 2024-05-05 19:06:58.000000 kiwitcms-github-app-1.7.0/tcms_github_app/migrations/0003_models_jsonfield.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-04-27 19:25:12.000000 kiwitcms-github-app-1.7.0/tcms_github_app/migrations/__init__.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     1875 2024-05-05 19:06:58.000000 kiwitcms-github-app-1.7.0/tcms_github_app/models.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      468 2024-05-05 19:06:58.000000 kiwitcms-github-app-1.7.0/tcms_github_app/urls.py
+-rw-r--r--   0 senko     (1001) senko     (1001)    10672 2024-05-06 06:50:57.000000 kiwitcms-github-app-1.7.0/tcms_github_app/utils.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     6473 2024-05-05 19:06:58.000000 kiwitcms-github-app-1.7.0/tcms_github_app/views.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-06 10:07:42.509008 kiwitcms-github-app-1.7.0/tcms_settings_dir/
+-rw-r--r--   0 senko     (1001) senko     (1001)       65 2024-01-14 21:43:45.000000 kiwitcms-github-app-1.7.0/tcms_settings_dir/__init__.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      525 2024-01-14 21:43:45.000000 kiwitcms-github-app-1.7.0/tcms_settings_dir/github_app.py
```

### Comparing `kiwitcms-github-app-1.6.0/LICENSE` & `kiwitcms-github-app-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-app-1.6.0/PKG-INFO` & `kiwitcms-github-app-1.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwitcms-github-app
-Version: 1.6.0
+Version: 1.7.0
 Summary: GitHub App integration for Kiwi TCMS
 Home-page: https://github.com/kiwitcms/github-app/
 Author: Kiwi TCMS
 Author-email: info@kiwitcms.org
 License: GPLv3+
 Classifier: Framework :: Django
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,21 +13,14 @@
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
-Requires-Dist: social-auth-app-django
-Requires-Dist: social-auth-core>=3.3.0
-Requires-Dist: kiwitcms-tenants
-Requires-Dist: certifi>=2023.7.22
-Requires-Dist: cryptography>=41.0.4
-Requires-Dist: pyjwt>=2.4.0
-Requires-Dist: requests>=2.31.0
 
 GitHub App integration for Kiwi TCMS
 ====================================
 
 .. image:: https://coveralls.io/repos/github/kiwitcms/github-app/badge.svg?branch=master
    :target: https://coveralls.io/github/kiwitcms/github-app?branch=master
 
@@ -130,14 +123,24 @@
   - Create
   - Repository
 
 
 Changelog
 ---------
 
+v1.7.0 (06 May 2024)
+~~~~~~~~~~~~~~~~~~~~
+
+- Pin indirect requirements to reduce the chance of installing vulnerable
+  dependencies
+- Remove the wrapper ``GithubKiwiTCMSBot()`` class
+- Simplify ``self.requester`` override in ``PatchedGithub()`` class
+- Start using the new GitHub Auth parameters introduced in PyGithub==1.59.0
+
+
 v1.6.0 (15 Jan 2024)
 ~~~~~~~~~~~~~~~~~~~~
 
 - 1-click bug report will now use ``execution.build.version.product`` instead
   of ``execution.run.plan.product`` following changes in Kiwi TCMS, see:
   <https://github.com/kiwitcms/Kiwi/commit/48a33a71e664c8c3ed2ceb298b5f1e19d0bddb52>_
   and `PR #3439 <https://github.com/kiwitcms/Kiwi/pull/3439>`_ for more details
```

### Comparing `kiwitcms-github-app-1.6.0/README.rst` & `kiwitcms-github-app-1.7.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -103,14 +103,24 @@
   - Create
   - Repository
 
 
 Changelog
 ---------
 
+v1.7.0 (06 May 2024)
+~~~~~~~~~~~~~~~~~~~~
+
+- Pin indirect requirements to reduce the chance of installing vulnerable
+  dependencies
+- Remove the wrapper ``GithubKiwiTCMSBot()`` class
+- Simplify ``self.requester`` override in ``PatchedGithub()`` class
+- Start using the new GitHub Auth parameters introduced in PyGithub==1.59.0
+
+
 v1.6.0 (15 Jan 2024)
 ~~~~~~~~~~~~~~~~~~~~
 
 - 1-click bug report will now use ``execution.build.version.product`` instead
   of ``execution.run.plan.product`` following changes in Kiwi TCMS, see:
   <https://github.com/kiwitcms/Kiwi/commit/48a33a71e664c8c3ed2ceb298b5f1e19d0bddb52>_
   and `PR #3439 <https://github.com/kiwitcms/Kiwi/pull/3439>`_ for more details
```

### Comparing `kiwitcms-github-app-1.6.0/kiwitcms_github_app.egg-info/PKG-INFO` & `kiwitcms-github-app-1.7.0/kiwitcms_github_app.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwitcms-github-app
-Version: 1.6.0
+Version: 1.7.0
 Summary: GitHub App integration for Kiwi TCMS
 Home-page: https://github.com/kiwitcms/github-app/
 Author: Kiwi TCMS
 Author-email: info@kiwitcms.org
 License: GPLv3+
 Classifier: Framework :: Django
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,21 +13,14 @@
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
-Requires-Dist: social-auth-app-django
-Requires-Dist: social-auth-core>=3.3.0
-Requires-Dist: kiwitcms-tenants
-Requires-Dist: certifi>=2023.7.22
-Requires-Dist: cryptography>=41.0.4
-Requires-Dist: pyjwt>=2.4.0
-Requires-Dist: requests>=2.31.0
 
 GitHub App integration for Kiwi TCMS
 ====================================
 
 .. image:: https://coveralls.io/repos/github/kiwitcms/github-app/badge.svg?branch=master
    :target: https://coveralls.io/github/kiwitcms/github-app?branch=master
 
@@ -130,14 +123,24 @@
   - Create
   - Repository
 
 
 Changelog
 ---------
 
+v1.7.0 (06 May 2024)
+~~~~~~~~~~~~~~~~~~~~
+
+- Pin indirect requirements to reduce the chance of installing vulnerable
+  dependencies
+- Remove the wrapper ``GithubKiwiTCMSBot()`` class
+- Simplify ``self.requester`` override in ``PatchedGithub()`` class
+- Start using the new GitHub Auth parameters introduced in PyGithub==1.59.0
+
+
 v1.6.0 (15 Jan 2024)
 ~~~~~~~~~~~~~~~~~~~~
 
 - 1-click bug report will now use ``execution.build.version.product`` instead
   of ``execution.run.plan.product`` following changes in Kiwi TCMS, see:
   <https://github.com/kiwitcms/Kiwi/commit/48a33a71e664c8c3ed2ceb298b5f1e19d0bddb52>_
   and `PR #3439 <https://github.com/kiwitcms/Kiwi/pull/3439>`_ for more details
```

### Comparing `kiwitcms-github-app-1.6.0/kiwitcms_github_app.egg-info/SOURCES.txt` & `kiwitcms-github-app-1.7.0/kiwitcms_github_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-app-1.6.0/setup.py` & `kiwitcms-github-app-1.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
                 continue
             requires.append(line.strip())
         return requires
 
 
 setup(
     name='kiwitcms-github-app',
-    version='1.6.0',
+    version='1.7.0',
     description='GitHub App integration for Kiwi TCMS',
     long_description=get_long_description(),
     author='Kiwi TCMS',
     author_email='info@kiwitcms.org',
     url='https://github.com/kiwitcms/github-app/',
     license='GPLv3+',
     install_requires=get_install_requires('requirements.txt'),
```

### Comparing `kiwitcms-github-app-1.6.0/tcms_github_app/admin.py` & `kiwitcms-github-app-1.7.0/tcms_github_app/admin.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-app-1.6.0/tcms_github_app/middleware.py` & `kiwitcms-github-app-1.7.0/tcms_github_app/middleware.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-app-1.6.0/tcms_github_app/migrations/0001_initial.py` & `kiwitcms-github-app-1.7.0/tcms_github_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-app-1.6.0/tcms_github_app/migrations/0002_appinstallation_settings_url.py` & `kiwitcms-github-app-1.7.0/tcms_github_app/migrations/0002_appinstallation_settings_url.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-app-1.6.0/tcms_github_app/migrations/0003_models_jsonfield.py` & `kiwitcms-github-app-1.7.0/tcms_github_app/migrations/0003_models_jsonfield.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-app-1.6.0/tcms_github_app/models.py` & `kiwitcms-github-app-1.7.0/tcms_github_app/models.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-app-1.6.0/tcms_github_app/utils.py` & `kiwitcms-github-app-1.7.0/tcms_github_app/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2019-2023 Alexander Todorov <atodorov@MrSenko.com>
+# Copyright (c) 2019-2024 Alexander Todorov <atodorov@MrSenko.com>
 #
 # Licensed under the GPL 3.0: https://www.gnu.org/licenses/gpl-3.0.txt
 #
 
 from django.conf import settings
 from django.contrib import messages
 from django.core.cache import cache
@@ -24,60 +24,26 @@
 
 RECORD_SKIPPED = 0
 RECORD_EXISTS = 10
 RECORD_CREATED = 20
 
 
 class PatchedGithub(github.Github):
-    def __init__(  # pylint: disable=too-many-arguments
-            self,
-            login_or_token=None,
-            password=None,
-            jwt=None,
-            app_auth=None,
-            base_url=github.Consts.DEFAULT_BASE_URL,
-            timeout=github.Consts.DEFAULT_TIMEOUT,
-            user_agent="PyGithub/Python",
-            per_page=github.Consts.DEFAULT_PER_PAGE,
-            verify=True,
-            retry=None,
-            pool_size=None,
-    ):
-        super().__init__(
-            login_or_token,
-            password,
-            jwt,
-            app_auth,
-            base_url,
-            timeout,
-            user_agent,
-            per_page,
-            verify,
-            retry,
-            pool_size,
-        )
+    def get_installation(self, inst_id):
+        """
+        Method removed in https://github.com/PyGithub/PyGithub/pull/1738.
 
-        # create our own b/c we can't access self.__requester from parent class
-        self.requester = github.Requester.Requester(
-            login_or_token,
-            password,
-            jwt,
-            app_auth,
-            base_url,
-            timeout,
-            user_agent,
-            per_page,
-            verify,
-            retry,
-            pool_size,
-        )
+        Doesn't look like it will be introduced again:
+        https://github.com/PyGithub/PyGithub/issues/1776
+        """
+        # b/c this is self.__requester in the parent class
+        requester = self._Github__requester  # pylint: disable=protected-access,no-member
 
-    def get_installation(self, inst_id):
         return github.Installation.Installation(
-            self.requester, headers={}, attributes={"id": inst_id}, completed=True
+            requester, headers={}, attributes={"id": inst_id}, completed=True
         )
 
 
 def find_token_from_app_inst(gh_app, installation):
     """
         Find an installation access token for this app:
         https://docs.github.com/en/rest/reference/apps#create-an-installation-access-token-for-an-app
```

### Comparing `kiwitcms-github-app-1.6.0/tcms_github_app/views.py` & `kiwitcms-github-app-1.7.0/tcms_github_app/views.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-app-1.6.0/tcms_settings_dir/github_app.py` & `kiwitcms-github-app-1.7.0/tcms_settings_dir/github_app.py`

 * *Files identical despite different names*

