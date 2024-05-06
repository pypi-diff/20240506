# Comparing `tmp/django-versionlog-1.7.0.tar.gz` & `tmp/django-versionlog-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-versionlog-1.7.0.tar", last modified: Fri Nov 10 07:35:25 2023, max compression
+gzip compressed data, was "dist/django-versionlog-1.8.0.tar", last modified: Mon May  6 08:20:38 2024, max compression
```

## Comparing `django-versionlog-1.7.0.tar` & `django-versionlog-1.8.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-10 07:35:25.000000 django-versionlog-1.7.0/
--rw-r--r--   0 root         (0) root         (0)      210 2023-11-10 07:35:23.000000 django-versionlog-1.7.0/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-10 07:35:25.000000 django-versionlog-1.7.0/django_versionlog.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1452 2023-11-10 07:35:25.000000 django-versionlog-1.7.0/django_versionlog.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-11-10 07:35:25.000000 django-versionlog-1.7.0/django_versionlog.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-10 07:35:25.000000 django-versionlog-1.7.0/django_versionlog.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-10 07:35:25.000000 django-versionlog-1.7.0/django_versionlog.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-11-10 07:35:25.000000 django-versionlog-1.7.0/django_versionlog.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     6014 2023-11-10 07:35:25.000000 django-versionlog-1.7.0/django_versionlog.egg-info/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-10 07:35:25.000000 django-versionlog-1.7.0/docs/
--rw-r--r--   0 root         (0) root         (0)      690 2023-11-10 07:35:23.000000 django-versionlog-1.7.0/docs/structure.md
--rw-r--r--   0 root         (0) root         (0)     3836 2023-11-10 07:35:23.000000 django-versionlog-1.7.0/docs/usage.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-10 07:35:25.000000 django-versionlog-1.7.0/docs/img/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-10 07:35:25.000000 django-versionlog-1.7.0/docs/img/demos/
--rw-r--r--   0 root         (0) root         (0)   134216 2023-11-10 07:35:23.000000 django-versionlog-1.7.0/docs/img/demos/dialog-page.png
--rw-r--r--   0 root         (0) root         (0)   169230 2023-11-10 07:35:23.000000 django-versionlog-1.7.0/docs/img/demos/dialog.png
--rw-r--r--   0 root         (0) root         (0)    52475 2023-11-10 07:35:23.000000 django-versionlog-1.7.0/docs/img/demos/gitbook-page.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-10 07:35:25.000000 django-versionlog-1.7.0/docs/img/icons/
--rw-r--r--   0 root         (0) root         (0)   146107 2023-11-10 07:35:23.000000 django-versionlog-1.7.0/docs/img/icons/django-versionlog.png
--rw-r--r--   0 root         (0) root         (0)  2421404 2023-11-10 07:35:23.000000 django-versionlog-1.7.0/docs/img/icons/qr_code.png
--rw-r--r--   0 root         (0) root         (0)      876 2023-11-10 07:35:23.000000 django-versionlog-1.7.0/docs/feature.md
--rw-r--r--   0 root         (0) root         (0)     1097 2023-11-10 07:35:23.000000 django-versionlog-1.7.0/docs/contributing.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-10 07:35:25.000000 django-versionlog-1.7.0/version_log/
--rw-r--r--   0 root         (0) root         (0)     2234 2023-11-10 07:35:23.000000 django-versionlog-1.7.0/version_log/models.py
--rw-r--r--   0 root         (0) root         (0)     2698 2023-11-10 07:35:23.000000 django-versionlog-1.7.0/version_log/decorators.py
--rw-r--r--   0 root         (0) root         (0)     3127 2023-11-10 07:35:23.000000 django-versionlog-1.7.0/version_log/middleware.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-11-10 07:35:23.000000 django-versionlog-1.7.0/version_log/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-10 07:35:25.000000 django-versionlog-1.7.0/version_log/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-10 07:35:25.000000 django-versionlog-1.7.0/version_log/templates/version_log/
--rw-r--r--   0 root         (0) root         (0)     3226 2023-11-10 07:35:23.000000 django-versionlog-1.7.0/version_log/templates/version_log/version_logs_page.html
--rw-r--r--   0 root         (0) root         (0)     5197 2023-11-10 07:35:23.000000 django-versionlog-1.7.0/version_log/templates/version_log/version_logs_block.html
--rw-r--r--   0 root         (0) root         (0)     2437 2023-11-10 07:35:23.000000 django-versionlog-1.7.0/version_log/templates/version_log/version_logs_dialog_page.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-10 07:35:25.000000 django-versionlog-1.7.0/version_log/migrations/
--rw-r--r--   0 root         (0) root         (0)      750 2023-11-10 07:35:23.000000 django-versionlog-1.7.0/version_log/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1452 2023-11-10 07:35:23.000000 django-versionlog-1.7.0/version_log/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)     1043 2023-11-10 07:35:23.000000 django-versionlog-1.7.0/version_log/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-10 07:35:25.000000 django-versionlog-1.7.0/version_log/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-10 07:35:25.000000 django-versionlog-1.7.0/version_log/static/version_log/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-10 07:35:25.000000 django-versionlog-1.7.0/version_log/static/version_log/js/
--rw-r--r--   0 root         (0) root         (0)    40547 2023-11-10 07:35:23.000000 django-versionlog-1.7.0/version_log/static/version_log/js/jquery.mCustomScrollbar.concat.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-10 07:35:25.000000 django-versionlog-1.7.0/version_log/static/version_log/images/
--rw-r--r--   0 root         (0) root         (0)      144 2023-11-10 07:35:23.000000 django-versionlog-1.7.0/version_log/static/version_log/images/back.svg
--rw-r--r--   0 root         (0) root         (0)      474 2023-11-10 07:35:23.000000 django-versionlog-1.7.0/version_log/static/version_log/images/homepage.svg
--rw-r--r--   0 root         (0) root         (0)    11143 2023-11-10 07:35:23.000000 django-versionlog-1.7.0/version_log/static/version_log/images/error.png
--rw-r--r--   0 root         (0) root         (0)      297 2023-11-10 07:35:23.000000 django-versionlog-1.7.0/version_log/static/version_log/images/down.svg
--rw-r--r--   0 root         (0) root         (0)     1048 2023-11-10 07:35:23.000000 django-versionlog-1.7.0/version_log/static/version_log/images/up.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-10 07:35:25.000000 django-versionlog-1.7.0/version_log/static/version_log/css/
--rw-r--r--   0 root         (0) root         (0)     2761 2023-11-10 07:35:23.000000 django-versionlog-1.7.0/version_log/static/version_log/css/version-log-page.css
--rw-r--r--   0 root         (0) root         (0)    52607 2023-11-10 07:35:23.000000 django-versionlog-1.7.0/version_log/static/version_log/css/jquery.mCustomScrollbar.css
--rw-r--r--   0 root         (0) root         (0)     1579 2023-11-10 07:35:23.000000 django-versionlog-1.7.0/version_log/static/version_log/css/version-log-gitbook-page.css
--rw-r--r--   0 root         (0) root         (0)     1742 2023-11-10 07:35:23.000000 django-versionlog-1.7.0/version_log/urls.py
--rw-r--r--   0 root         (0) root         (0)     3462 2023-11-10 07:35:23.000000 django-versionlog-1.7.0/version_log/config.py
--rw-r--r--   0 root         (0) root         (0)     5909 2023-11-10 07:35:23.000000 django-versionlog-1.7.0/version_log/utils.py
--rw-r--r--   0 root         (0) root         (0)     6937 2023-11-10 07:35:23.000000 django-versionlog-1.7.0/version_log/views.py
--rw-r--r--   0 root         (0) root         (0)     4888 2023-11-10 07:35:23.000000 django-versionlog-1.7.0/README.md
--rw-r--r--   0 root         (0) root         (0)     1514 2023-11-10 07:35:23.000000 django-versionlog-1.7.0/setup.py
--rw-r--r--   0 root         (0) root         (0)     6014 2023-11-10 07:35:25.000000 django-versionlog-1.7.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1069 2023-11-10 07:35:23.000000 django-versionlog-1.7.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       38 2023-11-10 07:35:25.000000 django-versionlog-1.7.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/
+-rw-r--r--   0 root         (0) root         (0)     6014 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1514 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/version_log/
+-rw-r--r--   0 root         (0) root         (0)     1769 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/urls.py
+-rw-r--r--   0 root         (0) root         (0)     1043 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/apps.py
+-rw-r--r--   0 root         (0) root         (0)     6936 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/version_log/migrations/
+-rw-r--r--   0 root         (0) root         (0)      750 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1452 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/migrations/0001_initial.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/version_log/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/version_log/static/version_log/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/version_log/static/version_log/js/
+-rw-r--r--   0 root         (0) root         (0)    40547 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/static/version_log/js/jquery.mCustomScrollbar.concat.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/version_log/static/version_log/images/
+-rw-r--r--   0 root         (0) root         (0)      297 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/static/version_log/images/down.svg
+-rw-r--r--   0 root         (0) root         (0)     1048 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/static/version_log/images/up.svg
+-rw-r--r--   0 root         (0) root         (0)      144 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/static/version_log/images/back.svg
+-rw-r--r--   0 root         (0) root         (0)      474 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/static/version_log/images/homepage.svg
+-rw-r--r--   0 root         (0) root         (0)    11143 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/static/version_log/images/error.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/version_log/static/version_log/css/
+-rw-r--r--   0 root         (0) root         (0)     1579 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/static/version_log/css/version-log-gitbook-page.css
+-rw-r--r--   0 root         (0) root         (0)     2761 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/static/version_log/css/version-log-page.css
+-rw-r--r--   0 root         (0) root         (0)    52607 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/static/version_log/css/jquery.mCustomScrollbar.css
+-rw-r--r--   0 root         (0) root         (0)     2233 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/models.py
+-rw-r--r--   0 root         (0) root         (0)      750 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5909 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2698 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/decorators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/version_log/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/version_log/templates/version_log/
+-rw-r--r--   0 root         (0) root         (0)     3226 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/templates/version_log/version_logs_page.html
+-rw-r--r--   0 root         (0) root         (0)     5197 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/templates/version_log/version_logs_block.html
+-rw-r--r--   0 root         (0) root         (0)     2343 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/templates/version_log/version_logs_dialog_page.html
+-rw-r--r--   0 root         (0) root         (0)     3461 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/config.py
+-rw-r--r--   0 root         (0) root         (0)     3127 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/version_log/middleware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/docs/img/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/docs/img/icons/
+-rw-r--r--   0 root         (0) root         (0)   146107 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/docs/img/icons/django-versionlog.png
+-rw-r--r--   0 root         (0) root         (0)  2421404 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/docs/img/icons/qr_code.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/docs/img/demos/
+-rw-r--r--   0 root         (0) root         (0)    52475 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/docs/img/demos/gitbook-page.png
+-rw-r--r--   0 root         (0) root         (0)   169230 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/docs/img/demos/dialog.png
+-rw-r--r--   0 root         (0) root         (0)   134216 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/docs/img/demos/dialog-page.png
+-rw-r--r--   0 root         (0) root         (0)     1097 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/docs/contributing.md
+-rw-r--r--   0 root         (0) root         (0)      690 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/docs/structure.md
+-rw-r--r--   0 root         (0) root         (0)      876 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/docs/feature.md
+-rw-r--r--   0 root         (0) root         (0)     3836 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/docs/usage.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/django_versionlog.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6014 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/django_versionlog.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/django_versionlog.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/django_versionlog.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/django_versionlog.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/django_versionlog.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1452 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/django_versionlog.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-06 08:20:38.000000 django-versionlog-1.8.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1069 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      210 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4888 2024-05-06 08:20:36.000000 django-versionlog-1.8.0/README.md
```

### Comparing `django-versionlog-1.7.0/django_versionlog.egg-info/SOURCES.txt` & `django-versionlog-1.8.0/django_versionlog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.7.0/django_versionlog.egg-info/PKG-INFO` & `django-versionlog-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: django-versionlog
-Version: 1.7.0
+Version: 1.8.0
 Summary: version log module
 Home-page: https://github.com/TencentBlueKing/django-versionlog
 Author: blueking
 Author-email: blueking@tencent.com
 License: UNKNOWN
 Description: # django-versionlog
         
         ![](docs/img/icons/django-versionlog.png)
         
-        [![license](https://img.shields.io/badge/license-mit-brightgreen.svg?style=flat)](https://github.com/TencentBlueKing/django-versionlog/blob/master/LICENSE) [![Release Version](https://img.shields.io/badge/release-1.7.0-brightgreen.svg)](https://github.com/TencentBlueKing/django-versionlog/releases) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/TencentBlueKing/django-versionlog/pulls) 
+        [![license](https://img.shields.io/badge/license-mit-brightgreen.svg?style=flat)](https://github.com/TencentBlueKing/django-versionlog/blob/master/LICENSE) [![Release Version](https://img.shields.io/badge/release-1.8.0-brightgreen.svg)](https://github.com/TencentBlueKing/django-versionlog/releases) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/TencentBlueKing/django-versionlog/pulls) 
         
         > **重要提示**: `master` 分支是开发分支，可能处于 *不稳定或者不可用状态* 。请通过[releases](https://github.com/TencentBlueKing/django-versionlog/releases) 而非 `master` 去获取稳定的软件包
         
         django-versionlog是为网站开发者提供版本日志快速接入的功能模块，支持django框架，兼容python2和python3。开发者只需在项目中进行简单的配置和维护版本日志目录中的md文件，即可在项目中向用户展示网站版本的更新迭代内容。
         
         ## Overview
```

### Comparing `django-versionlog-1.7.0/docs/structure.md` & `django-versionlog-1.8.0/docs/structure.md`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.7.0/docs/usage.md` & `django-versionlog-1.8.0/docs/usage.md`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.7.0/docs/img/demos/dialog-page.png` & `django-versionlog-1.8.0/docs/img/demos/dialog-page.png`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.7.0/docs/img/demos/dialog.png` & `django-versionlog-1.8.0/docs/img/demos/dialog.png`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.7.0/docs/img/demos/gitbook-page.png` & `django-versionlog-1.8.0/docs/img/demos/gitbook-page.png`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.7.0/docs/img/icons/django-versionlog.png` & `django-versionlog-1.8.0/docs/img/icons/django-versionlog.png`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.7.0/docs/img/icons/qr_code.png` & `django-versionlog-1.8.0/docs/img/icons/qr_code.png`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.7.0/docs/feature.md` & `django-versionlog-1.8.0/docs/feature.md`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.7.0/docs/contributing.md` & `django-versionlog-1.8.0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.7.0/version_log/models.py` & `django-versionlog-1.8.0/version_log/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 http://opensource.org/licenses/MIT
 Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 specific language governing permissions and limitations under the License.
 """
 
 from django.db import models
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from version_log.utils import is_later_version
 from version_log.config import NO_VERSION_CONSTANT
 
 
 class VersionLogVisitedManager(models.Manager):
     def has_visit_latest(self, username, latest_version):
```

### Comparing `django-versionlog-1.7.0/version_log/decorators.py` & `django-versionlog-1.8.0/version_log/decorators.py`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.7.0/version_log/middleware.py` & `django-versionlog-1.8.0/version_log/middleware.py`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.7.0/version_log/__init__.py` & `django-versionlog-1.8.0/version_log/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.7.0/version_log/templates/version_log/version_logs_page.html` & `django-versionlog-1.8.0/version_log/templates/version_log/version_logs_page.html`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.7.0/version_log/templates/version_log/version_logs_block.html` & `django-versionlog-1.8.0/version_log/templates/version_log/version_logs_block.html`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.7.0/version_log/templates/version_log/version_logs_dialog_page.html` & `django-versionlog-1.8.0/version_log/templates/version_log/version_logs_dialog_page.html`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta charset="UTF-8">
     <title>{{ page_title }}</title>
     <link rel="stylesheet" href="https://magicbox.bk.tencent.com/static_api/v3/assets/bootstrap-3.3.4/css/bootstrap.min.css">
     <link rel="stylesheet" href="https://magicbox.bk.tencent.com/static_api/v3/assets/artDialog-6.0.4/css/ui-dialog.css">
-    <script type="text/javascript" src="{% url 'version_log:javascript-catalog' %}"></script>
     <script src="https://magicbox.bk.tencent.com/static_api/v3/assets/js/jquery-1.10.2.min.js"></script>
     <script src="https://magicbox.bk.tencent.com/static_api/v3/assets/bootstrap-3.3.4/js/bootstrap.min.js"></script>
     <script src="https://magicbox.bk.tencent.com/static_api/v3/assets/artDialog-6.0.4/dist/dialog-min.js"></script>
     <script>
         function show_modal() {
             load_modal_frame("{% url 'version_log:block' %}");
         }
```

### Comparing `django-versionlog-1.7.0/version_log/migrations/__init__.py` & `django-versionlog-1.8.0/version_log/__init__.py`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.7.0/version_log/migrations/0001_initial.py` & `django-versionlog-1.8.0/version_log/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.7.0/version_log/apps.py` & `django-versionlog-1.8.0/version_log/apps.py`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.7.0/version_log/static/version_log/js/jquery.mCustomScrollbar.concat.min.js` & `django-versionlog-1.8.0/version_log/static/version_log/js/jquery.mCustomScrollbar.concat.min.js`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.7.0/version_log/static/version_log/images/error.png` & `django-versionlog-1.8.0/version_log/static/version_log/images/error.png`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.7.0/version_log/static/version_log/images/up.svg` & `django-versionlog-1.8.0/version_log/static/version_log/images/up.svg`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.7.0/version_log/static/version_log/css/version-log-page.css` & `django-versionlog-1.8.0/version_log/static/version_log/css/version-log-page.css`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.7.0/version_log/static/version_log/css/jquery.mCustomScrollbar.css` & `django-versionlog-1.8.0/version_log/static/version_log/css/jquery.mCustomScrollbar.css`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.7.0/version_log/static/version_log/css/version-log-gitbook-page.css` & `django-versionlog-1.8.0/version_log/static/version_log/css/version-log-gitbook-page.css`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.7.0/version_log/urls.py` & `django-versionlog-1.8.0/version_log/urls.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 You may obtain a copy of the License at
 http://opensource.org/licenses/MIT
 Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 specific language governing permissions and limitations under the License.
 """
 
-from django.conf.urls import url
+from django.urls import re_path
 
 from version_log import views
 
 app_name = "version_log"
 
 urlpatterns = (
     # 版本日志单页面
-    url(r'^$', views.version_logs_page, name='version_log_page'),
+    re_path(r'^$', views.version_logs_page, name='version_log_page'),
     # 获取版本日志块页面（用于对话框场景）
-    url(r'^block/$', views.version_logs_block, name='block'),
+    re_path(r'^block/$', views.version_logs_block, name='block'),
     # 获取版本日志列表
-    url(r'^version_logs_list/$', views.version_logs_list, name='version_logs_list'),
+    re_path(r'^version_logs_list/$', views.version_logs_list, name='version_logs_list'),
     # 获取版本日志详情
-    url(r'^version_log_detail/', views.get_version_log_detail, name='version_log_detail'),
-    url(r'^markdown_version_log_detail/', views.get_markdown_version_log_detail, name='markdown_version_log_detail'),
+    re_path(r'^version_log_detail/', views.get_version_log_detail, name='version_log_detail'),
+    re_path(r'^markdown_version_log_detail/', views.get_markdown_version_log_detail, name='markdown_version_log_detail'),
     # 查询当前用户是否看过最新版本日志
-    url(r'^has_user_read_latest/', views.has_user_read_latest, name='has_user_read_latest'),
+    re_path(r'^has_user_read_latest/', views.has_user_read_latest, name='has_user_read_latest'),
 
     # 获取版本日志和详情列表
-    url(r"^version_logs_list_with_detail/$", views.version_logs_list_with_detail, name="version_logs_list_with_detail")
+    re_path(r"^version_logs_list_with_detail/$", views.version_logs_list_with_detail, name="version_logs_list_with_detail")
 )
```

### Comparing `django-versionlog-1.7.0/version_log/config.py` & `django-versionlog-1.8.0/version_log/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 specific language governing permissions and limitations under the License.
 """
 
 import re
 import os
 
 from django.conf import settings
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 
 __all__ = ('MD_FILES_DIR', 'PARSED_HTML_FILES_DIR', 'NAME_PATTERN',
            'LATEST_VERSION_INFORM', 'ENTRANCE_URL', 'LANGUAGE_MAPPINGS', 'LANGUAGE_POSTFIX_SEPARATION')
 
 # 默认设置
 VERSION_LOG = {
```

### Comparing `django-versionlog-1.7.0/version_log/utils.py` & `django-versionlog-1.8.0/version_log/utils.py`

 * *Files identical despite different names*

### Comparing `django-versionlog-1.7.0/version_log/views.py` & `django-versionlog-1.8.0/version_log/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 """
 
 import logging
 import functools
 
 from django.shortcuts import render
 from django.http import JsonResponse
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from version_log import config
 from version_log.models import VersionLogVisited
 from version_log.utils import get_version_list, get_parsed_html, get_parsed_markdown_file_path, \
     get_md_files_dir_with_language_code
 
 logger = logging.getLogger(__name__)
```

### Comparing `django-versionlog-1.7.0/README.md` & `django-versionlog-1.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # django-versionlog
 
 ![](docs/img/icons/django-versionlog.png)
 
-[![license](https://img.shields.io/badge/license-mit-brightgreen.svg?style=flat)](https://github.com/TencentBlueKing/django-versionlog/blob/master/LICENSE) [![Release Version](https://img.shields.io/badge/release-1.7.0-brightgreen.svg)](https://github.com/TencentBlueKing/django-versionlog/releases) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/TencentBlueKing/django-versionlog/pulls) 
+[![license](https://img.shields.io/badge/license-mit-brightgreen.svg?style=flat)](https://github.com/TencentBlueKing/django-versionlog/blob/master/LICENSE) [![Release Version](https://img.shields.io/badge/release-1.8.0-brightgreen.svg)](https://github.com/TencentBlueKing/django-versionlog/releases) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/TencentBlueKing/django-versionlog/pulls) 
 
 > **重要提示**: `master` 分支是开发分支，可能处于 *不稳定或者不可用状态* 。请通过[releases](https://github.com/TencentBlueKing/django-versionlog/releases) 而非 `master` 去获取稳定的软件包
 
 django-versionlog是为网站开发者提供版本日志快速接入的功能模块，支持django框架，兼容python2和python3。开发者只需在项目中进行简单的配置和维护版本日志目录中的md文件，即可在项目中向用户展示网站版本的更新迭代内容。
 
 ## Overview
```

### Comparing `django-versionlog-1.7.0/setup.py` & `django-versionlog-1.8.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-versionlog',
-    version='1.7.0',
+    version='1.8.0',
     packages=find_packages(),
     include_package_data=True,
     url="https://github.com/TencentBlueKing/django-versionlog",
     description='version log module',
     long_description=README,
     long_description_content_type='text/markdown',
     author='blueking',
```

### Comparing `django-versionlog-1.7.0/PKG-INFO` & `django-versionlog-1.8.0/django_versionlog.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: django-versionlog
-Version: 1.7.0
+Version: 1.8.0
 Summary: version log module
 Home-page: https://github.com/TencentBlueKing/django-versionlog
 Author: blueking
 Author-email: blueking@tencent.com
 License: UNKNOWN
 Description: # django-versionlog
         
         ![](docs/img/icons/django-versionlog.png)
         
-        [![license](https://img.shields.io/badge/license-mit-brightgreen.svg?style=flat)](https://github.com/TencentBlueKing/django-versionlog/blob/master/LICENSE) [![Release Version](https://img.shields.io/badge/release-1.7.0-brightgreen.svg)](https://github.com/TencentBlueKing/django-versionlog/releases) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/TencentBlueKing/django-versionlog/pulls) 
+        [![license](https://img.shields.io/badge/license-mit-brightgreen.svg?style=flat)](https://github.com/TencentBlueKing/django-versionlog/blob/master/LICENSE) [![Release Version](https://img.shields.io/badge/release-1.8.0-brightgreen.svg)](https://github.com/TencentBlueKing/django-versionlog/releases) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/TencentBlueKing/django-versionlog/pulls) 
         
         > **重要提示**: `master` 分支是开发分支，可能处于 *不稳定或者不可用状态* 。请通过[releases](https://github.com/TencentBlueKing/django-versionlog/releases) 而非 `master` 去获取稳定的软件包
         
         django-versionlog是为网站开发者提供版本日志快速接入的功能模块，支持django框架，兼容python2和python3。开发者只需在项目中进行简单的配置和维护版本日志目录中的md文件，即可在项目中向用户展示网站版本的更新迭代内容。
         
         ## Overview
```

### Comparing `django-versionlog-1.7.0/LICENSE` & `django-versionlog-1.8.0/LICENSE`

 * *Files identical despite different names*

