# Comparing `tmp/trix-4.1.1.tar.gz` & `tmp/trix-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trix-4.1.1.tar", last modified: Thu Feb  8 18:40:10 2024, max compression
+gzip compressed data, was "trix-4.1.2.tar", last modified: Mon May  6 13:30:56 2024, max compression
```

## Comparing `trix-4.1.1.tar` & `trix-4.1.2.tar`

### file list

```diff
@@ -1,320 +1,320 @@
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:10.161743 trix-4.1.1/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1483 2023-02-14 12:27:42.000000 trix-4.1.1/LICENSE
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      626 2023-02-14 12:27:42.000000 trix-4.1.1/MANIFEST.in
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      947 2024-02-08 18:40:10.155695 trix-4.1.1/PKG-INFO
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      286 2023-02-14 12:27:42.000000 trix-4.1.1/README.md
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)       38 2024-02-08 18:40:10.162749 trix-4.1.1/setup.cfg
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1239 2024-02-05 10:48:43.000000 trix-4.1.1/setup.py
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.245719 trix-4.1.1/trix/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)       41 2023-02-14 12:27:42.000000 trix-4.1.1/trix/__init__.py
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.280582 trix-4.1.1/trix/project/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2023-02-14 12:27:42.000000 trix-4.1.1/trix/project/__init__.py
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.289460 trix-4.1.1/trix/project/default/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2023-02-14 12:27:42.000000 trix-4.1.1/trix/project/default/__init__.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      625 2024-02-05 10:48:43.000000 trix-4.1.1/trix/project/default/default_urls.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     4961 2024-02-05 10:48:43.000000 trix-4.1.1/trix/project/default/settings.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      161 2024-02-05 10:48:43.000000 trix-4.1.1/trix/project/default/templatecontext.py
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.295489 trix-4.1.1/trix/project/develop/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2023-02-14 12:27:42.000000 trix-4.1.1/trix/project/develop/__init__.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     3204 2023-02-14 12:27:42.000000 trix-4.1.1/trix/project/develop/developtasks.py
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.359219 trix-4.1.1/trix/project/develop/dumps/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)       93 2023-02-14 12:27:42.000000 trix-4.1.1/trix/project/develop/dumps/__init__.py
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.370438 trix-4.1.1/trix/project/develop/dumps/dev/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)       69 2023-02-14 12:27:42.000000 trix-4.1.1/trix/project/develop/dumps/dev/__init__.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)    11751 2023-02-14 12:27:42.000000 trix-4.1.1/trix/project/develop/dumps/dev/data.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      532 2023-02-14 12:27:42.000000 trix-4.1.1/trix/project/develop/dumps/dev/import_helper.py
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.392622 trix-4.1.1/trix/project/develop/settings/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2023-02-14 12:27:42.000000 trix-4.1.1/trix/project/develop/settings/__init__.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      605 2023-02-14 12:27:42.000000 trix-4.1.1/trix/project/develop/settings/common.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)       57 2023-02-14 12:27:42.000000 trix-4.1.1/trix/project/develop/settings/develop.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      319 2023-02-14 12:27:42.000000 trix-4.1.1/trix/project/develop/settings/test.py
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.399695 trix-4.1.1/trix/project/develop/testhelpers/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2023-02-14 12:27:43.000000 trix-4.1.1/trix/project/develop/testhelpers/__init__.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1893 2023-02-14 12:27:43.000000 trix-4.1.1/trix/project/develop/testhelpers/login.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      602 2023-02-14 12:27:43.000000 trix-4.1.1/trix/project/develop/testhelpers/user.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)       88 2023-02-14 12:27:43.000000 trix-4.1.1/trix/project/develop/urls.py
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.406777 trix-4.1.1/trix/project/production/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2023-02-14 12:27:43.000000 trix-4.1.1/trix/project/production/__init__.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1453 2023-02-14 12:27:43.000000 trix-4.1.1/trix/project/production/settings.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)       88 2023-02-14 12:27:43.000000 trix-4.1.1/trix/project/production/urls.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)       88 2024-02-05 10:48:43.000000 trix-4.1.1/trix/project/production/wsgi.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      896 2023-02-14 12:27:43.000000 trix-4.1.1/trix/project/settingsproxy.py
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.424948 trix-4.1.1/trix/trix_admin/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_admin/__init__.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     2932 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_admin/cradmin.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      652 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_admin/css_icon_map.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     4966 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_admin/editor_widget.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      784 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_admin/formfields.py
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.036688 trix-4.1.1/trix/trix_admin/locale/
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.038707 trix-4.1.1/trix/trix_admin/locale/nb/
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.433018 trix-4.1.1/trix/trix_admin/locale/nb/LC_MESSAGES/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     4106 2024-01-11 06:51:52.000000 trix-4.1.1/trix/trix_admin/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     7746 2024-01-10 13:44:45.000000 trix-4.1.1/trix/trix_admin/locale/nb/LC_MESSAGES/django.po
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.435041 trix-4.1.1/trix/trix_admin/management/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_admin/management/__init__.py
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.451209 trix-4.1.1/trix/trix_admin/management/commands/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_admin/management/commands/__init__.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     3650 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_admin/management/commands/generatetestdata.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_admin/models.py
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.054870 trix-4.1.1/trix/trix_admin/static/
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.055883 trix-4.1.1/trix/trix_admin/static/trix_admin/
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.459283 trix-4.1.1/trix/trix_admin/static/trix_admin/plain_es6/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)    27289 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_admin/static/trix_admin/plain_es6/commentEditor.js
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      569 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_admin/static/trix_admin/plain_es6/cookie.js
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      503 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_admin/static/trix_admin/plain_es6/datepicker.js
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      138 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_admin/static/trix_admin/plain_es6/webcomponent_utils.js
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.072059 trix-4.1.1/trix/trix_admin/templates/
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.473422 trix-4.1.1/trix/trix_admin/templates/cradmin_legacy/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      248 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_admin/templates/cradmin_legacy/base.django.html
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.059926 trix-4.1.1/trix/trix_admin/templates/cradmin_legacy/layouts/
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.475447 trix-4.1.1/trix/trix_admin/templates/cradmin_legacy/layouts/standalone/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      149 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_admin/templates/cradmin_legacy/layouts/standalone/focused.django.html
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.069030 trix-4.1.1/trix/trix_admin/templates/cradmin_legacy/pagepreview/
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.493638 trix-4.1.1/trix/trix_admin/templates/cradmin_legacy/pagepreview/includes/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1886 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_admin/templates/cradmin_legacy/pagepreview/includes/pagepreview-fullsize-iframe-wrapper.django.html
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      694 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_admin/templates/cradmin_legacy/standalone-base.django.html
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.071049 trix-4.1.1/trix/trix_admin/templates/cradmin_legacy/viewhelpers/
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.495662 trix-4.1.1/trix/trix_admin/templates/cradmin_legacy/viewhelpers/objecttable/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)    13943 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_admin/templates/cradmin_legacy/viewhelpers/objecttable/objecttable.django.html
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.506780 trix-4.1.1/trix/trix_admin/templates/trix_admin/
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.510827 trix-4.1.1/trix/trix_admin/templates/trix_admin/assignments/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      796 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_admin/templates/trix_admin/assignments/multiedit.django.html
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      420 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_admin/templates/trix_admin/assignments/preview.django.html
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      744 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_admin/templates/trix_admin/delete.django.html
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.514875 trix-4.1.1/trix/trix_admin/templates/trix_admin/editor/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      279 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_admin/templates/trix_admin/editor/devilry_markdown_editor.django.html
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)    10174 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_admin/templates/trix_admin/editor/markdown_help.django.html
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.517918 trix-4.1.1/trix/trix_admin/templates/trix_admin/include/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      412 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_admin/templates/trix_admin/include/progress_bar.django.html
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      266 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_admin/templates/trix_admin/menu.django.html
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      230 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_admin/templates/trix_admin/menuitems.django.html
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1186 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_admin/templates/trix_admin/roleselect.django.html
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     8069 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_admin/templates/trix_admin/statistics.django.html
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.527025 trix-4.1.1/trix/trix_admin/templatetags/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_admin/templatetags/__init__.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      950 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_admin/templatetags/trix_admin_tags.py
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.530054 trix-4.1.1/trix/trix_admin/tests/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_admin/tests/__init__.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      738 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_admin/tests/test_assignments.py
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.552291 trix-4.1.1/trix/trix_admin/views/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_admin/views/__init__.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)    16027 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_admin/views/assignments.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      151 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_admin/views/markdown_help.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     4492 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_admin/views/permalinks.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      886 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_admin/views/roleselect.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)    10340 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_admin/views/statistics.py
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.568481 trix-4.1.1/trix/trix_auth/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_auth/__init__.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     3356 2024-02-08 18:21:25.000000 trix-4.1.1/trix/trix_auth/allauth_adapter.py
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.082180 trix-4.1.1/trix/trix_auth/locale/
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.093288 trix-4.1.1/trix/trix_auth/locale/nb/
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.586741 trix-4.1.1/trix/trix_auth/locale/nb/LC_MESSAGES/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1309 2024-01-11 06:51:52.000000 trix-4.1.1/trix/trix_auth/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     2538 2024-01-10 13:44:48.000000 trix-4.1.1/trix/trix_auth/locale/nb/LC_MESSAGES/django.po
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.108419 trix-4.1.1/trix/trix_auth/templates/
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.588768 trix-4.1.1/trix/trix_auth/templates/socialaccount/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      388 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_auth/templates/socialaccount/authentication_error.html
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.593825 trix-4.1.1/trix/trix_auth/templates/trix_auth/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      972 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_auth/templates/trix_auth/auth_logout.django.html
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      724 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_auth/templates/trix_auth/login.django.html
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      503 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_auth/templates/trix_auth/logout.django.html
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      729 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_auth/urls.py
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.612035 trix-4.1.1/trix/trix_auth/views/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_auth/views/__init__.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1337 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_auth/views/allauth_views.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     2829 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_auth/views/login.py
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.647412 trix-4.1.1/trix/trix_core/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_core/__init__.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     4851 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_core/admin.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      965 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_core/api.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      151 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_core/apps.py
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.149737 trix-4.1.1/trix/trix_core/locale/
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.158791 trix-4.1.1/trix/trix_core/locale/nb/
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.651451 trix-4.1.1/trix/trix_core/locale/nb/LC_MESSAGES/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     2787 2024-01-11 06:51:52.000000 trix-4.1.1/trix/trix_core/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     4761 2024-01-10 13:44:51.000000 trix-4.1.1/trix/trix_core/locale/nb/LC_MESSAGES/django.po
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.698946 trix-4.1.1/trix/trix_core/migrations/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     5853 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_core/migrations/0001_initial.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      537 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_core/migrations/0002_assignment_hidden.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      661 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_core/migrations/0003_auto_20180809_1220.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      495 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_core/migrations/0004_user_fix.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     2834 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_core/migrations/0005_auto_20190818_2150.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1076 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_core/migrations/0006_auto_20221121_1419.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1102 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_core/migrations/0007_auto_20221130_1209.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      463 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_core/migrations/0008_course_visible.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_core/migrations/__init__.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     9437 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_core/models.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)    10082 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_core/multiassignment_serialize.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     2159 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_core/tagutils.py
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.702975 trix-4.1.1/trix/trix_core/templatetags/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_core/templatetags/__init__.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      905 2024-01-16 13:38:07.000000 trix-4.1.1/trix/trix_core/templatetags/trix_core_tags.py
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.715115 trix-4.1.1/trix/trix_core/tests/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_core/tests/__init__.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     7769 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_core/tests/test_multiassignment_serialize.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      936 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_core/tests/test_tagutils.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      286 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_core/tests/test_trix_core_tags.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      421 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_core/tests/test_trix_markdown.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      873 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_core/trix_markdown.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      308 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_core/urls.py
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.718136 trix-4.1.1/trix/trix_course/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_course/__init__.py
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.166855 trix-4.1.1/trix/trix_course/locale/
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.167862 trix-4.1.1/trix/trix_course/locale/nb/
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.732272 trix-4.1.1/trix/trix_course/locale/nb/LC_MESSAGES/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     2200 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_course/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     5146 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_course/locale/nb/LC_MESSAGES/django.po
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.170889 trix-4.1.1/trix/trix_course/templates/
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.753496 trix-4.1.1/trix/trix_course/templates/trix_course/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     2781 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_course/templates/trix_course/add_course_admin.django.html
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     4131 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_course/templates/trix_course/base.django.html
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1941 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_course/templates/trix_course/course_admin.django.html
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      854 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_course/templates/trix_course/course_dashboard.django.html
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1135 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_course/templates/trix_course/remove_course_admin.django.html
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      826 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_course/urls.py
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.776739 trix-4.1.1/trix/trix_course/views/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_course/views/__init__.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     2932 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_course/views/add.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1113 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_course/views/administer.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      433 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_course/views/base.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1114 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_course/views/course.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1637 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_course/views/remove.py
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.786841 trix-4.1.1/trix/trix_student/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/__init__.py
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.175921 trix-4.1.1/trix/trix_student/locale/
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.189071 trix-4.1.1/trix/trix_student/locale/nb/
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.790881 trix-4.1.1/trix/trix_student/locale/nb/LC_MESSAGES/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     7444 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_student/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)    14993 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_student/locale/nb/LC_MESSAGES/django.po
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.795926 trix-4.1.1/trix/trix_student/middleware/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/middleware/__init__.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      719 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/middleware/consent.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/models.py
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.192158 trix-4.1.1/trix/trix_student/static/
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.805000 trix-4.1.1/trix/trix_student/static/trix_student/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)       43 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/.gitignore
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     4770 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/Gruntfile.coffee
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      416 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/bower.json
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.197246 trix-4.1.1/trix/trix_student/static/trix_student/dist/
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.820111 trix-4.1.1/trix/trix_student/static/trix_student/dist/css/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)   227456 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/dist/css/styles.css
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1079 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/dist/css/wcag.css
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.836222 trix-4.1.1/trix/trix_student/static/trix_student/dist/fonts/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)    20335 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/dist/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)    62927 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/dist/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)    41280 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/dist/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)    23320 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/dist/fonts/glyphicons-halflings-regular.woff
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.852366 trix-4.1.1/trix/trix_student/static/trix_student/dist/js/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     6862 2024-02-02 08:23:36.000000 trix-4.1.1/trix/trix_student/static/trix_student/dist/js/trix_student.js
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     4644 2024-02-02 08:23:36.000000 trix-4.1.1/trix/trix_student/static/trix_student/dist/js/trix_student.min.js
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     4191 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/dist/js/trix_student.min.js.map
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.212396 trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.936031 trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/fonts/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)   124904 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-brands-400.eot
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)   700511 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-brands-400.svg
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)   124668 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-brands-400.ttf
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)    80664 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-brands-400.woff
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)    68912 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-brands-400.woff2
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)    40576 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-regular-400.eot
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)   142447 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-regular-400.svg
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)    40348 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-regular-400.ttf
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)    18168 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-regular-400.woff
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)    14872 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-regular-400.woff2
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)   191512 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-solid-900.eot
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)   726153 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-solid-900.svg
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)   191292 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-solid-900.ttf
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)    92800 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-solid-900.woff
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)    71948 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-solid-900.woff2
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.990448 trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/js/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     2113 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/js/alert.js
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1331 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/js/angular-cookies.min.js
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     3117 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/js/angular-cookies.min.js.map
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     5721 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/js/angular-route.min.js
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)    14578 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/js/angular-route.min.js.map
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)   177366 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/js/angular.min.js
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)   470349 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/js/angular.min.js.map
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)    38510 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/js/bootstrap-datetimepicker.min.js
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)    29110 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/js/bootstrap.min.js
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)    72372 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/js/jquery.slim.min.js
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)   110315 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/js/jquery.slim.min.map
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)   103577 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/js/ui-bootstrap.min.js
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     4012 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/js/url.min.js
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      495 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/package.json
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.217465 trix-4.1.1/trix/trix_student/static/trix_student/src/
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:10.011590 trix-4.1.1/trix/trix_student/static/trix_student/src/app/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      458 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/src/app/app.coffee
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:10.013604 trix-4.1.1/trix/trix_student/static/trix_student/src/app/assignments/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     4479 2024-02-02 08:23:36.000000 trix-4.1.1/trix/trix_student/static/trix_student/src/app/assignments/controllers.coffee
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      530 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/src/app/directives.coffee
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:10.057954 trix-4.1.1/trix/trix_student/static/trix_student/src/less/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      221 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/src/less/alerts.less
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     3018 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/src/less/assignments.less
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      326 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/src/less/bootstrap.less
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)       59 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/src/less/buttons.less
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1614 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/src/less/comment-editor.less
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      405 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/src/less/consent.less
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     5809 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/src/less/course.less
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      205 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/src/less/delete.less
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      887 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/src/less/font-awesome.less
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      486 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/src/less/footer.less
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      179 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/src/less/header.less
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      905 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/src/less/menu.less
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      169 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/src/less/page-header.less
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      549 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/src/less/pager.less
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      783 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/src/less/print.less
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     2841 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/src/less/statistics.less
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      613 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/src/less/styles.less
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      401 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/src/less/tag-filter.less
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     7357 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/src/less/trix.less
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      338 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/src/less/users.less
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      584 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/src/less/variables.less
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1151 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_student/static/trix_student/src/less/wcag.less
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:10.066006 trix-4.1.1/trix/trix_student/templates/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      357 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/templates/400.html
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      377 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/templates/403.html
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      373 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/templates/404.html
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      366 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/templates/500.html
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:10.097235 trix-4.1.1/trix/trix_student/templates/trix_student/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     4340 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_student/templates/trix_student/assignment_list_base.django.html
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      351 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/templates/trix_student/assignments.django.html
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     3127 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_student/templates/trix_student/base.django.html
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      160 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/templates/trix_student/consent_form.django.html
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     2591 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_student/templates/trix_student/consent_form_base.django.html
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      799 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/templates/trix_student/course.django.html
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1604 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_student/templates/trix_student/dashboard.django.html
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:10.117393 trix-4.1.1/trix/trix_student/templates/trix_student/include/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     4116 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_student/templates/trix_student/include/assignment.django.html
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      638 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_student/templates/trix_student/include/footer.django.html
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      146 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/templates/trix_student/include/footer_base.django.html
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     3188 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_student/templates/trix_student/include/header.django.html
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     2052 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/templates/trix_student/include/pager.django.html
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      690 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/templates/trix_student/permalink.django.html
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      797 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/templates/trix_student/permalink_list.django.html
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1004 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/templates/trix_student/user_delete.django.html
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1818 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/templates/trix_student/users.django.html
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:10.121420 trix-4.1.1/trix/trix_student/tests/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/tests/__init__.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     3553 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/tests/test_howsolved.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1390 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_student/urls.py
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:10.142577 trix-4.1.1/trix/trix_student/views/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/views/__init__.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      822 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/views/assignments.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      747 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/views/base.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     5376 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/views/common.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      509 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_student/views/consent.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1477 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/views/course.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1092 2024-02-05 10:48:43.000000 trix-4.1.1/trix/trix_student/views/dashboard.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     2574 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/views/howsolved.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1666 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/views/permalink.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1829 2023-02-14 12:27:43.000000 trix-4.1.1/trix/trix_student/views/users.py
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:10.152664 trix-4.1.1/trix/utils/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2023-02-14 12:27:43.000000 trix-4.1.1/trix/utils/__init__.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      193 2023-02-14 12:27:43.000000 trix-4.1.1/trix/utils/template.py
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)       22 2024-02-08 18:35:19.000000 trix-4.1.1/trix/version.py
-drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-02-08 18:40:09.262814 trix-4.1.1/trix.egg-info/
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      947 2024-02-08 18:40:08.000000 trix-4.1.1/trix.egg-info/PKG-INFO
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)    11873 2024-02-08 18:40:08.000000 trix-4.1.1/trix.egg-info/SOURCES.txt
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)        1 2024-02-08 18:40:08.000000 trix-4.1.1/trix.egg-info/dependency_links.txt
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)        1 2024-01-05 11:39:51.000000 trix-4.1.1/trix.egg-info/not-zip-safe
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)      135 2024-02-08 18:40:08.000000 trix-4.1.1/trix.egg-info/requires.txt
--rw-r--r--   0 torgeirl (120615) torgeirl (140705)        5 2024-02-08 18:40:08.000000 trix-4.1.1/trix.egg-info/top_level.txt
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.860999 trix-4.1.2/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1483 2024-05-06 12:39:49.000000 trix-4.1.2/LICENSE
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      626 2024-05-06 12:39:49.000000 trix-4.1.2/MANIFEST.in
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      947 2024-05-06 13:30:56.856963 trix-4.1.2/PKG-INFO
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      286 2024-05-06 12:39:49.000000 trix-4.1.2/README.md
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)       38 2024-05-06 13:30:56.862005 trix-4.1.2/setup.cfg
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1239 2024-05-06 12:39:49.000000 trix-4.1.2/setup.py
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:55.943631 trix-4.1.2/trix/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)       41 2024-05-06 12:39:49.000000 trix-4.1.2/trix/__init__.py
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:55.957769 trix-4.1.2/trix/project/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 12:39:49.000000 trix-4.1.2/trix/project/__init__.py
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:55.965843 trix-4.1.2/trix/project/default/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 12:39:49.000000 trix-4.1.2/trix/project/default/__init__.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      625 2024-05-06 12:39:49.000000 trix-4.1.2/trix/project/default/default_urls.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     4961 2024-05-06 12:39:49.000000 trix-4.1.2/trix/project/default/settings.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      161 2024-05-06 12:39:49.000000 trix-4.1.2/trix/project/default/templatecontext.py
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:55.982022 trix-4.1.2/trix/project/develop/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 12:39:49.000000 trix-4.1.2/trix/project/develop/__init__.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     3204 2024-05-06 12:39:49.000000 trix-4.1.2/trix/project/develop/developtasks.py
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:55.984044 trix-4.1.2/trix/project/develop/dumps/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)       93 2024-05-06 12:39:49.000000 trix-4.1.2/trix/project/develop/dumps/__init__.py
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.009313 trix-4.1.2/trix/project/develop/dumps/dev/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)       69 2024-05-06 12:39:49.000000 trix-4.1.2/trix/project/develop/dumps/dev/__init__.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)    11751 2024-05-06 12:39:49.000000 trix-4.1.2/trix/project/develop/dumps/dev/data.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      532 2024-05-06 12:39:49.000000 trix-4.1.2/trix/project/develop/dumps/dev/import_helper.py
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.025460 trix-4.1.2/trix/project/develop/settings/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 12:39:49.000000 trix-4.1.2/trix/project/develop/settings/__init__.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      605 2024-05-06 12:39:49.000000 trix-4.1.2/trix/project/develop/settings/common.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)       57 2024-05-06 12:39:49.000000 trix-4.1.2/trix/project/develop/settings/develop.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      319 2024-05-06 12:39:49.000000 trix-4.1.2/trix/project/develop/settings/test.py
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.048623 trix-4.1.2/trix/project/develop/testhelpers/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 12:39:49.000000 trix-4.1.2/trix/project/develop/testhelpers/__init__.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1893 2024-05-06 12:39:49.000000 trix-4.1.2/trix/project/develop/testhelpers/login.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      602 2024-05-06 12:39:49.000000 trix-4.1.2/trix/project/develop/testhelpers/user.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)       88 2024-05-06 12:39:49.000000 trix-4.1.2/trix/project/develop/urls.py
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.066762 trix-4.1.2/trix/project/production/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 12:39:49.000000 trix-4.1.2/trix/project/production/__init__.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1453 2024-05-06 12:39:49.000000 trix-4.1.2/trix/project/production/settings.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)       88 2024-05-06 12:39:49.000000 trix-4.1.2/trix/project/production/urls.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)       88 2024-05-06 12:39:49.000000 trix-4.1.2/trix/project/production/wsgi.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      896 2024-05-06 12:39:49.000000 trix-4.1.2/trix/project/settingsproxy.py
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.122203 trix-4.1.2/trix/trix_admin/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_admin/__init__.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     2932 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_admin/cradmin.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      652 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_admin/css_icon_map.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     4966 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_admin/editor_widget.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      784 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_admin/formfields.py
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:55.756549 trix-4.1.2/trix/trix_admin/locale/
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:55.757559 trix-4.1.2/trix/trix_admin/locale/nb/
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.127232 trix-4.1.2/trix/trix_admin/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     4106 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_admin/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     7746 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_admin/locale/nb/LC_MESSAGES/django.po
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.129253 trix-4.1.2/trix/trix_admin/management/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_admin/management/__init__.py
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.152428 trix-4.1.2/trix/trix_admin/management/commands/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_admin/management/commands/__init__.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     3650 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_admin/management/commands/generatetestdata.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_admin/models.py
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:55.759579 trix-4.1.2/trix/trix_admin/static/
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:55.760589 trix-4.1.2/trix/trix_admin/static/trix_admin/
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.162525 trix-4.1.2/trix/trix_admin/static/trix_admin/plain_es6/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)    27289 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_admin/static/trix_admin/plain_es6/commentEditor.js
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      569 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_admin/static/trix_admin/plain_es6/cookie.js
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      503 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_admin/static/trix_admin/plain_es6/datepicker.js
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      138 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_admin/static/trix_admin/plain_es6/webcomponent_utils.js
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:55.784830 trix-4.1.2/trix/trix_admin/templates/
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.166559 trix-4.1.2/trix/trix_admin/templates/cradmin_legacy/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      248 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_admin/templates/cradmin_legacy/base.django.html
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:55.764630 trix-4.1.2/trix/trix_admin/templates/cradmin_legacy/layouts/
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.168579 trix-4.1.2/trix/trix_admin/templates/cradmin_legacy/layouts/standalone/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      149 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_admin/templates/cradmin_legacy/layouts/standalone/focused.django.html
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:55.766651 trix-4.1.2/trix/trix_admin/templates/cradmin_legacy/pagepreview/
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.170596 trix-4.1.2/trix/trix_admin/templates/cradmin_legacy/pagepreview/includes/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1886 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_admin/templates/cradmin_legacy/pagepreview/includes/pagepreview-fullsize-iframe-wrapper.django.html
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      694 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_admin/templates/cradmin_legacy/standalone-base.django.html
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:55.783816 trix-4.1.2/trix/trix_admin/templates/cradmin_legacy/viewhelpers/
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.172612 trix-4.1.2/trix/trix_admin/templates/cradmin_legacy/viewhelpers/objecttable/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)    13943 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_admin/templates/cradmin_legacy/viewhelpers/objecttable/objecttable.django.html
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.183705 trix-4.1.2/trix/trix_admin/templates/trix_admin/
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.187729 trix-4.1.2/trix/trix_admin/templates/trix_admin/assignments/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      796 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_admin/templates/trix_admin/assignments/multiedit.django.html
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      420 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_admin/templates/trix_admin/assignments/preview.django.html
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      744 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_admin/templates/trix_admin/delete.django.html
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.191765 trix-4.1.2/trix/trix_admin/templates/trix_admin/editor/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      279 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_admin/templates/trix_admin/editor/devilry_markdown_editor.django.html
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)    10174 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_admin/templates/trix_admin/editor/markdown_help.django.html
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.194784 trix-4.1.2/trix/trix_admin/templates/trix_admin/include/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      412 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_admin/templates/trix_admin/include/progress_bar.django.html
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      266 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_admin/templates/trix_admin/menu.django.html
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      230 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_admin/templates/trix_admin/menuitems.django.html
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1186 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_admin/templates/trix_admin/roleselect.django.html
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     8069 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_admin/templates/trix_admin/statistics.django.html
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.198817 trix-4.1.2/trix/trix_admin/templatetags/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_admin/templatetags/__init__.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      950 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_admin/templatetags/trix_admin_tags.py
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.215930 trix-4.1.2/trix/trix_admin/tests/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_admin/tests/__init__.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      738 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_admin/tests/test_assignments.py
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.237063 trix-4.1.2/trix/trix_admin/views/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_admin/views/__init__.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)    16027 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_admin/views/assignments.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      151 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_admin/views/markdown_help.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     4492 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_admin/views/permalinks.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      886 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_admin/views/roleselect.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)    10354 2024-05-06 13:03:23.000000 trix-4.1.2/trix/trix_admin/views/statistics.py
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.243107 trix-4.1.2/trix/trix_auth/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_auth/__init__.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     3356 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_auth/allauth_adapter.py
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:55.790891 trix-4.1.2/trix/trix_auth/locale/
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:55.791904 trix-4.1.2/trix/trix_auth/locale/nb/
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.248146 trix-4.1.2/trix/trix_auth/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1309 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_auth/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     2538 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_auth/locale/nb/LC_MESSAGES/django.po
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:55.793929 trix-4.1.2/trix/trix_auth/templates/
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.250167 trix-4.1.2/trix/trix_auth/templates/socialaccount/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      388 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_auth/templates/socialaccount/authentication_error.html
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.256223 trix-4.1.2/trix/trix_auth/templates/trix_auth/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      972 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_auth/templates/trix_auth/auth_logout.django.html
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      724 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_auth/templates/trix_auth/login.django.html
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      503 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_auth/templates/trix_auth/logout.django.html
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      729 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_auth/urls.py
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.271339 trix-4.1.2/trix/trix_auth/views/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_auth/views/__init__.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1337 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_auth/views/allauth_views.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     2829 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_auth/views/login.py
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.311627 trix-4.1.2/trix/trix_core/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_core/__init__.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     4851 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_core/admin.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      965 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_core/api.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      151 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_core/apps.py
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:55.796960 trix-4.1.2/trix/trix_core/locale/
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:55.796960 trix-4.1.2/trix/trix_core/locale/nb/
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.325738 trix-4.1.2/trix/trix_core/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     2787 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_core/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     4761 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_core/locale/nb/LC_MESSAGES/django.po
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.362062 trix-4.1.2/trix/trix_core/migrations/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     5853 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_core/migrations/0001_initial.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      537 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_core/migrations/0002_assignment_hidden.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      661 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_core/migrations/0003_auto_20180809_1220.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      495 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_core/migrations/0004_user_fix.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     2834 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_core/migrations/0005_auto_20190818_2150.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1076 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_core/migrations/0006_auto_20221121_1419.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1102 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_core/migrations/0007_auto_20221130_1209.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      463 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_core/migrations/0008_course_visible.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_core/migrations/__init__.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     9437 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_core/models.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)    10082 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_core/multiassignment_serialize.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     2159 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_core/tagutils.py
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.365076 trix-4.1.2/trix/trix_core/templatetags/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_core/templatetags/__init__.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      905 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_core/templatetags/trix_core_tags.py
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.406425 trix-4.1.2/trix/trix_core/tests/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_core/tests/__init__.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     7769 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_core/tests/test_multiassignment_serialize.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      936 2024-05-06 12:39:49.000000 trix-4.1.2/trix/trix_core/tests/test_tagutils.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      286 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_core/tests/test_trix_core_tags.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      421 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_core/tests/test_trix_markdown.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      873 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_core/trix_markdown.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      308 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_core/urls.py
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.410470 trix-4.1.2/trix/trix_course/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_course/__init__.py
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:55.829231 trix-4.1.2/trix/trix_course/locale/
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:55.830241 trix-4.1.2/trix/trix_course/locale/nb/
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.414516 trix-4.1.2/trix/trix_course/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     2200 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_course/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     5146 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_course/locale/nb/LC_MESSAGES/django.po
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:55.831254 trix-4.1.2/trix/trix_course/templates/
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.445881 trix-4.1.2/trix/trix_course/templates/trix_course/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     2781 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_course/templates/trix_course/add_course_admin.django.html
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     4131 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_course/templates/trix_course/base.django.html
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1941 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_course/templates/trix_course/course_admin.django.html
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      854 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_course/templates/trix_course/course_dashboard.django.html
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1135 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_course/templates/trix_course/remove_course_admin.django.html
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      826 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_course/urls.py
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.472163 trix-4.1.2/trix/trix_course/views/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_course/views/__init__.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     2932 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_course/views/add.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1113 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_course/views/administer.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      433 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_course/views/base.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1114 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_course/views/course.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1637 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_course/views/remove.py
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.477240 trix-4.1.2/trix/trix_student/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/__init__.py
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:55.851477 trix-4.1.2/trix/trix_student/locale/
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:55.852487 trix-4.1.2/trix/trix_student/locale/nb/
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.481289 trix-4.1.2/trix/trix_student/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     7444 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)    14993 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/locale/nb/LC_MESSAGES/django.po
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.485327 trix-4.1.2/trix/trix_student/middleware/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/middleware/__init__.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      719 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/middleware/consent.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/models.py
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:55.865654 trix-4.1.2/trix/trix_student/static/
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.492390 trix-4.1.2/trix/trix_student/static/trix_student/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)       43 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/.gitignore
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     4770 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/Gruntfile.coffee
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      416 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/bower.json
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:55.870708 trix-4.1.2/trix/trix_student/static/trix_student/dist/
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.499462 trix-4.1.2/trix/trix_student/static/trix_student/dist/css/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)   227456 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/dist/css/styles.css
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1079 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/dist/css/wcag.css
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.539843 trix-4.1.2/trix/trix_student/static/trix_student/dist/fonts/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)    20335 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/dist/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)    62927 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/dist/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)    41280 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/dist/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)    23320 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/dist/fonts/glyphicons-halflings-regular.woff
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.561051 trix-4.1.2/trix/trix_student/static/trix_student/dist/js/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     6862 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/dist/js/trix_student.js
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     4644 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/dist/js/trix_student.min.js
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     4191 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/dist/js/trix_student.min.js.map
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:55.872727 trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.629708 trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/fonts/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)   124904 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-brands-400.eot
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)   700511 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-brands-400.svg
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)   124668 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-brands-400.ttf
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)    80664 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-brands-400.woff
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)    68912 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-brands-400.woff2
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)    40576 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-regular-400.eot
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)   142447 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-regular-400.svg
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)    40348 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-regular-400.ttf
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)    18168 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-regular-400.woff
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)    14872 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-regular-400.woff2
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)   191512 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-solid-900.eot
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)   726153 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-solid-900.svg
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)   191292 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-solid-900.ttf
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)    92800 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-solid-900.woff
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)    71948 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-solid-900.woff2
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.693315 trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/js/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     2113 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/js/alert.js
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1331 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/js/angular-cookies.min.js
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     3117 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/js/angular-cookies.min.js.map
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     5721 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/js/angular-route.min.js
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)    14578 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/js/angular-route.min.js.map
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)   177366 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/js/angular.min.js
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)   470349 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/js/angular.min.js.map
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)    38510 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/js/bootstrap-datetimepicker.min.js
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)    29110 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/js/bootstrap.min.js
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)    72372 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/js/jquery.slim.min.js
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)   110315 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/js/jquery.slim.min.map
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)   103577 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/js/ui-bootstrap.min.js
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     4012 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/js/url.min.js
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      495 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/package.json
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:55.910141 trix-4.1.2/trix/trix_student/static/trix_student/src/
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.696343 trix-4.1.2/trix/trix_student/static/trix_student/src/app/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      458 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/src/app/app.coffee
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.698373 trix-4.1.2/trix/trix_student/static/trix_student/src/app/assignments/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     4479 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/src/app/assignments/controllers.coffee
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      530 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/src/app/directives.coffee
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.750903 trix-4.1.2/trix/trix_student/static/trix_student/src/less/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      221 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/src/less/alerts.less
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     3018 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/src/less/assignments.less
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      326 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/src/less/bootstrap.less
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)       59 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/src/less/buttons.less
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1614 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/src/less/comment-editor.less
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      405 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/src/less/consent.less
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     5809 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/src/less/course.less
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      205 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/src/less/delete.less
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      887 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/src/less/font-awesome.less
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      486 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/src/less/footer.less
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      179 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/src/less/header.less
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      905 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/src/less/menu.less
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      169 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/src/less/page-header.less
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      549 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/src/less/pager.less
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      783 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/src/less/print.less
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     2841 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/src/less/statistics.less
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      613 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/src/less/styles.less
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      401 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/src/less/tag-filter.less
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     7357 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/src/less/trix.less
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      338 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/src/less/users.less
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      584 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/src/less/variables.less
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1151 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/static/trix_student/src/less/wcag.less
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.759986 trix-4.1.2/trix/trix_student/templates/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      357 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/templates/400.html
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      377 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/templates/403.html
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      373 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/templates/404.html
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      366 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/templates/500.html
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.801407 trix-4.1.2/trix/trix_student/templates/trix_student/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     4340 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/templates/trix_student/assignment_list_base.django.html
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      351 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/templates/trix_student/assignments.django.html
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     3127 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/templates/trix_student/base.django.html
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      160 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/templates/trix_student/consent_form.django.html
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     2591 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/templates/trix_student/consent_form_base.django.html
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      799 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/templates/trix_student/course.django.html
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1604 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/templates/trix_student/dashboard.django.html
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.828639 trix-4.1.2/trix/trix_student/templates/trix_student/include/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     4116 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/templates/trix_student/include/assignment.django.html
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      638 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/templates/trix_student/include/footer.django.html
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      146 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/templates/trix_student/include/footer_base.django.html
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     3188 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/templates/trix_student/include/header.django.html
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     2052 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/templates/trix_student/include/pager.django.html
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      690 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/templates/trix_student/permalink.django.html
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      797 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/templates/trix_student/permalink_list.django.html
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1004 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/templates/trix_student/user_delete.django.html
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1818 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/templates/trix_student/users.django.html
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.831663 trix-4.1.2/trix/trix_student/tests/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/tests/__init__.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     3553 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/tests/test_howsolved.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1390 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/urls.py
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.850879 trix-4.1.2/trix/trix_student/views/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/views/__init__.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      822 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/views/assignments.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      747 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/views/base.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     5376 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/views/common.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      509 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/views/consent.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1477 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/views/course.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1092 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/views/dashboard.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     2574 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/views/howsolved.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1666 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/views/permalink.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)     1829 2024-05-06 12:39:50.000000 trix-4.1.2/trix/trix_student/views/users.py
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:56.853926 trix-4.1.2/trix/utils/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 12:39:50.000000 trix-4.1.2/trix/utils/__init__.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      193 2024-05-06 12:39:50.000000 trix-4.1.2/trix/utils/template.py
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)       22 2024-05-06 13:19:28.000000 trix-4.1.2/trix/version.py
+drwxr-xr-x   0 torgeirl (120615) torgeirl (140705)        0 2024-05-06 13:30:55.953722 trix-4.1.2/trix.egg-info/
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      947 2024-05-06 13:30:55.000000 trix-4.1.2/trix.egg-info/PKG-INFO
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)    11873 2024-05-06 13:30:55.000000 trix-4.1.2/trix.egg-info/SOURCES.txt
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)        1 2024-05-06 13:30:55.000000 trix-4.1.2/trix.egg-info/dependency_links.txt
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)        1 2024-05-06 13:06:45.000000 trix-4.1.2/trix.egg-info/not-zip-safe
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)      135 2024-05-06 13:30:55.000000 trix-4.1.2/trix.egg-info/requires.txt
+-rw-r--r--   0 torgeirl (120615) torgeirl (140705)        5 2024-05-06 13:30:55.000000 trix-4.1.2/trix.egg-info/top_level.txt
```

### Comparing `trix-4.1.1/LICENSE` & `trix-4.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/MANIFEST.in` & `trix-4.1.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/PKG-INFO` & `trix-4.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trix
-Version: 4.1.1
+Version: 4.1.2
 Summary: Next generation Trix. Detailed task control and statistics app for better learning outcome.
 Home-page: https://github.com/devilry/trix2
 Author: Tor Johansen, Espen Angell Kristiansen, Jonas Sandbekk
 Author-email: tor@appresso.no, espen@appresso.no, jonassandbekk@gmail.com
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `trix-4.1.1/setup.py` & `trix-4.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/project/default/default_urls.py` & `trix-4.1.2/trix/project/default/default_urls.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/project/default/settings.py` & `trix-4.1.2/trix/project/default/settings.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/project/develop/developtasks.py` & `trix-4.1.2/trix/project/develop/developtasks.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/project/develop/dumps/dev/data.py` & `trix-4.1.2/trix/project/develop/dumps/dev/data.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/project/develop/dumps/dev/import_helper.py` & `trix-4.1.2/trix/project/develop/dumps/dev/import_helper.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/project/develop/settings/common.py` & `trix-4.1.2/trix/project/develop/settings/common.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/project/develop/testhelpers/login.py` & `trix-4.1.2/trix/project/develop/testhelpers/login.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/project/develop/testhelpers/user.py` & `trix-4.1.2/trix/project/develop/testhelpers/user.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/project/production/settings.py` & `trix-4.1.2/trix/project/production/settings.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/project/settingsproxy.py` & `trix-4.1.2/trix/project/settingsproxy.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_admin/cradmin.py` & `trix-4.1.2/trix/trix_admin/cradmin.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_admin/css_icon_map.py` & `trix-4.1.2/trix/trix_admin/css_icon_map.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_admin/editor_widget.py` & `trix-4.1.2/trix/trix_admin/editor_widget.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_admin/formfields.py` & `trix-4.1.2/trix/trix_admin/formfields.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_admin/locale/nb/LC_MESSAGES/django.mo` & `trix-4.1.2/trix/trix_admin/locale/nb/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_admin/locale/nb/LC_MESSAGES/django.po` & `trix-4.1.2/trix/trix_admin/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_admin/management/commands/generatetestdata.py` & `trix-4.1.2/trix/trix_admin/management/commands/generatetestdata.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_admin/static/trix_admin/plain_es6/commentEditor.js` & `trix-4.1.2/trix/trix_admin/static/trix_admin/plain_es6/commentEditor.js`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_admin/static/trix_admin/plain_es6/cookie.js` & `trix-4.1.2/trix/trix_admin/static/trix_admin/plain_es6/cookie.js`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_admin/templates/cradmin_legacy/pagepreview/includes/pagepreview-fullsize-iframe-wrapper.django.html` & `trix-4.1.2/trix/trix_admin/templates/cradmin_legacy/pagepreview/includes/pagepreview-fullsize-iframe-wrapper.django.html`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_admin/templates/cradmin_legacy/standalone-base.django.html` & `trix-4.1.2/trix/trix_admin/templates/cradmin_legacy/standalone-base.django.html`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_admin/templates/cradmin_legacy/viewhelpers/objecttable/objecttable.django.html` & `trix-4.1.2/trix/trix_admin/templates/cradmin_legacy/viewhelpers/objecttable/objecttable.django.html`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_admin/templates/trix_admin/assignments/multiedit.django.html` & `trix-4.1.2/trix/trix_admin/templates/trix_admin/assignments/multiedit.django.html`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_admin/templates/trix_admin/delete.django.html` & `trix-4.1.2/trix/trix_admin/templates/trix_admin/delete.django.html`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_admin/templates/trix_admin/editor/markdown_help.django.html` & `trix-4.1.2/trix/trix_admin/templates/trix_admin/editor/markdown_help.django.html`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_admin/templates/trix_admin/roleselect.django.html` & `trix-4.1.2/trix/trix_admin/templates/trix_admin/roleselect.django.html`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_admin/templates/trix_admin/statistics.django.html` & `trix-4.1.2/trix/trix_admin/templates/trix_admin/statistics.django.html`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_admin/templatetags/trix_admin_tags.py` & `trix-4.1.2/trix/trix_admin/templatetags/trix_admin_tags.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_admin/tests/test_assignments.py` & `trix-4.1.2/trix/trix_admin/tests/test_assignments.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_admin/views/assignments.py` & `trix-4.1.2/trix/trix_admin/views/assignments.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_admin/views/permalinks.py` & `trix-4.1.2/trix/trix_admin/views/permalinks.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_admin/views/roleselect.py` & `trix-4.1.2/trix/trix_admin/views/roleselect.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_admin/views/statistics.py` & `trix-4.1.2/trix/trix_admin/views/statistics.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 
 class AssignmentStatsCsv(AssignmentStatsMixin, View):
 
     def get(self, request, *args, **kwargs):
         self.tags = self.get_tags()
         if not self.tags:
             return HttpResponseBadRequest()
-        if self.request.cradmin_role.course_tag.tag not in self.tags:
+        if not self.tags.filter(tag=self.request.cradmin_role.course_tag).exists():
             raise PermissionDenied()
         assignmentqueryset = self.get_queryset()
 
         user_count = get_usercount_within_assignments(assignmentqueryset)
         response = HttpResponse(content_type='text/csv')
         csv.register_dialect('semicolons', delimiter=';')
```

### Comparing `trix-4.1.1/trix/trix_auth/allauth_adapter.py` & `trix-4.1.2/trix/trix_auth/allauth_adapter.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_auth/locale/nb/LC_MESSAGES/django.mo` & `trix-4.1.2/trix/trix_auth/locale/nb/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_auth/locale/nb/LC_MESSAGES/django.po` & `trix-4.1.2/trix/trix_auth/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_auth/templates/trix_auth/auth_logout.django.html` & `trix-4.1.2/trix/trix_auth/templates/trix_auth/auth_logout.django.html`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_auth/templates/trix_auth/login.django.html` & `trix-4.1.2/trix/trix_auth/templates/trix_auth/login.django.html`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_auth/urls.py` & `trix-4.1.2/trix/trix_auth/urls.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_auth/views/allauth_views.py` & `trix-4.1.2/trix/trix_auth/views/allauth_views.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_auth/views/login.py` & `trix-4.1.2/trix/trix_auth/views/login.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_core/admin.py` & `trix-4.1.2/trix/trix_core/admin.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_core/api.py` & `trix-4.1.2/trix/trix_core/api.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_core/locale/nb/LC_MESSAGES/django.mo` & `trix-4.1.2/trix/trix_core/locale/nb/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_core/locale/nb/LC_MESSAGES/django.po` & `trix-4.1.2/trix/trix_core/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_core/migrations/0001_initial.py` & `trix-4.1.2/trix/trix_core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_core/migrations/0002_assignment_hidden.py` & `trix-4.1.2/trix/trix_core/migrations/0002_assignment_hidden.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_core/migrations/0003_auto_20180809_1220.py` & `trix-4.1.2/trix/trix_core/migrations/0003_auto_20180809_1220.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_core/migrations/0005_auto_20190818_2150.py` & `trix-4.1.2/trix/trix_core/migrations/0005_auto_20190818_2150.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_core/migrations/0006_auto_20221121_1419.py` & `trix-4.1.2/trix/trix_core/migrations/0006_auto_20221121_1419.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_core/migrations/0007_auto_20221130_1209.py` & `trix-4.1.2/trix/trix_core/migrations/0007_auto_20221130_1209.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_core/models.py` & `trix-4.1.2/trix/trix_core/models.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_core/multiassignment_serialize.py` & `trix-4.1.2/trix/trix_core/multiassignment_serialize.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_core/tagutils.py` & `trix-4.1.2/trix/trix_core/tagutils.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_core/templatetags/trix_core_tags.py` & `trix-4.1.2/trix/trix_core/templatetags/trix_core_tags.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_core/tests/test_multiassignment_serialize.py` & `trix-4.1.2/trix/trix_core/tests/test_multiassignment_serialize.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_core/tests/test_tagutils.py` & `trix-4.1.2/trix/trix_core/tests/test_tagutils.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_core/trix_markdown.py` & `trix-4.1.2/trix/trix_core/trix_markdown.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_course/locale/nb/LC_MESSAGES/django.mo` & `trix-4.1.2/trix/trix_course/locale/nb/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_course/locale/nb/LC_MESSAGES/django.po` & `trix-4.1.2/trix/trix_course/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_course/templates/trix_course/add_course_admin.django.html` & `trix-4.1.2/trix/trix_course/templates/trix_course/add_course_admin.django.html`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_course/templates/trix_course/base.django.html` & `trix-4.1.2/trix/trix_course/templates/trix_course/base.django.html`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_course/templates/trix_course/course_admin.django.html` & `trix-4.1.2/trix/trix_course/templates/trix_course/course_admin.django.html`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_course/templates/trix_course/course_dashboard.django.html` & `trix-4.1.2/trix/trix_course/templates/trix_course/course_dashboard.django.html`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_course/templates/trix_course/remove_course_admin.django.html` & `trix-4.1.2/trix/trix_course/templates/trix_course/remove_course_admin.django.html`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_course/urls.py` & `trix-4.1.2/trix/trix_course/urls.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_course/views/add.py` & `trix-4.1.2/trix/trix_course/views/add.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_course/views/administer.py` & `trix-4.1.2/trix/trix_course/views/administer.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_course/views/course.py` & `trix-4.1.2/trix/trix_course/views/course.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_course/views/remove.py` & `trix-4.1.2/trix/trix_course/views/remove.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/locale/nb/LC_MESSAGES/django.mo` & `trix-4.1.2/trix/trix_student/locale/nb/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/locale/nb/LC_MESSAGES/django.po` & `trix-4.1.2/trix/trix_student/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/middleware/consent.py` & `trix-4.1.2/trix/trix_student/middleware/consent.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/Gruntfile.coffee` & `trix-4.1.2/trix/trix_student/static/trix_student/Gruntfile.coffee`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/dist/css/styles.css` & `trix-4.1.2/trix/trix_student/static/trix_student/dist/css/styles.css`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/dist/css/wcag.css` & `trix-4.1.2/trix/trix_student/static/trix_student/dist/css/wcag.css`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/dist/fonts/glyphicons-halflings-regular.eot` & `trix-4.1.2/trix/trix_student/static/trix_student/dist/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/dist/fonts/glyphicons-halflings-regular.svg` & `trix-4.1.2/trix/trix_student/static/trix_student/dist/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/dist/fonts/glyphicons-halflings-regular.ttf` & `trix-4.1.2/trix/trix_student/static/trix_student/dist/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/dist/fonts/glyphicons-halflings-regular.woff` & `trix-4.1.2/trix/trix_student/static/trix_student/dist/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/dist/js/trix_student.js` & `trix-4.1.2/trix/trix_student/static/trix_student/dist/js/trix_student.js`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/dist/js/trix_student.min.js` & `trix-4.1.2/trix/trix_student/static/trix_student/dist/js/trix_student.min.js`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/dist/js/trix_student.min.js.map` & `trix-4.1.2/trix/trix_student/static/trix_student/dist/js/trix_student.min.js.map`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-brands-400.eot` & `trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-brands-400.svg` & `trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-brands-400.ttf` & `trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-brands-400.woff` & `trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-brands-400.woff2` & `trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-regular-400.eot` & `trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-regular-400.svg` & `trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-regular-400.ttf` & `trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-regular-400.woff` & `trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-regular-400.woff2` & `trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-solid-900.eot` & `trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-solid-900.svg` & `trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-solid-900.ttf` & `trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-solid-900.woff` & `trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-solid-900.woff2` & `trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/fonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/js/alert.js` & `trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/js/alert.js`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/js/angular-cookies.min.js` & `trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/js/angular-cookies.min.js`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/js/angular-cookies.min.js.map` & `trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/js/angular-cookies.min.js.map`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/js/angular-route.min.js` & `trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/js/angular-route.min.js`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/js/angular-route.min.js.map` & `trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/js/angular-route.min.js.map`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/js/angular.min.js` & `trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/js/angular.min.js`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/js/angular.min.js.map` & `trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/js/angular.min.js.map`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/js/bootstrap-datetimepicker.min.js` & `trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/js/bootstrap-datetimepicker.min.js`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/js/bootstrap.min.js` & `trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/js/jquery.slim.min.js` & `trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/js/jquery.slim.min.js`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/js/jquery.slim.min.map` & `trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/js/jquery.slim.min.map`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/js/ui-bootstrap.min.js` & `trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/js/ui-bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/dist/vendor/js/url.min.js` & `trix-4.1.2/trix/trix_student/static/trix_student/dist/vendor/js/url.min.js`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/src/app/assignments/controllers.coffee` & `trix-4.1.2/trix/trix_student/static/trix_student/src/app/assignments/controllers.coffee`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/src/app/directives.coffee` & `trix-4.1.2/trix/trix_student/static/trix_student/src/app/directives.coffee`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/src/less/assignments.less` & `trix-4.1.2/trix/trix_student/static/trix_student/src/less/assignments.less`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/src/less/comment-editor.less` & `trix-4.1.2/trix/trix_student/static/trix_student/src/less/comment-editor.less`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/src/less/course.less` & `trix-4.1.2/trix/trix_student/static/trix_student/src/less/course.less`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/src/less/font-awesome.less` & `trix-4.1.2/trix/trix_student/static/trix_student/src/less/font-awesome.less`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/src/less/menu.less` & `trix-4.1.2/trix/trix_student/static/trix_student/src/less/menu.less`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/src/less/pager.less` & `trix-4.1.2/trix/trix_student/static/trix_student/src/less/pager.less`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/src/less/print.less` & `trix-4.1.2/trix/trix_student/static/trix_student/src/less/print.less`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/src/less/statistics.less` & `trix-4.1.2/trix/trix_student/static/trix_student/src/less/statistics.less`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/src/less/styles.less` & `trix-4.1.2/trix/trix_student/static/trix_student/src/less/styles.less`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/src/less/trix.less` & `trix-4.1.2/trix/trix_student/static/trix_student/src/less/trix.less`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/src/less/variables.less` & `trix-4.1.2/trix/trix_student/static/trix_student/src/less/variables.less`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/static/trix_student/src/less/wcag.less` & `trix-4.1.2/trix/trix_student/static/trix_student/src/less/wcag.less`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/templates/trix_student/assignment_list_base.django.html` & `trix-4.1.2/trix/trix_student/templates/trix_student/assignment_list_base.django.html`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/templates/trix_student/base.django.html` & `trix-4.1.2/trix/trix_student/templates/trix_student/base.django.html`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/templates/trix_student/consent_form_base.django.html` & `trix-4.1.2/trix/trix_student/templates/trix_student/consent_form_base.django.html`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/templates/trix_student/course.django.html` & `trix-4.1.2/trix/trix_student/templates/trix_student/course.django.html`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/templates/trix_student/dashboard.django.html` & `trix-4.1.2/trix/trix_student/templates/trix_student/dashboard.django.html`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/templates/trix_student/include/assignment.django.html` & `trix-4.1.2/trix/trix_student/templates/trix_student/include/assignment.django.html`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/templates/trix_student/include/footer.django.html` & `trix-4.1.2/trix/trix_student/templates/trix_student/include/footer.django.html`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/templates/trix_student/include/header.django.html` & `trix-4.1.2/trix/trix_student/templates/trix_student/include/header.django.html`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/templates/trix_student/include/pager.django.html` & `trix-4.1.2/trix/trix_student/templates/trix_student/include/pager.django.html`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/templates/trix_student/permalink.django.html` & `trix-4.1.2/trix/trix_student/templates/trix_student/permalink.django.html`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/templates/trix_student/permalink_list.django.html` & `trix-4.1.2/trix/trix_student/templates/trix_student/permalink_list.django.html`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/templates/trix_student/user_delete.django.html` & `trix-4.1.2/trix/trix_student/templates/trix_student/user_delete.django.html`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/templates/trix_student/users.django.html` & `trix-4.1.2/trix/trix_student/templates/trix_student/users.django.html`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/tests/test_howsolved.py` & `trix-4.1.2/trix/trix_student/tests/test_howsolved.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/urls.py` & `trix-4.1.2/trix/trix_student/urls.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/views/assignments.py` & `trix-4.1.2/trix/trix_student/views/assignments.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/views/base.py` & `trix-4.1.2/trix/trix_student/views/base.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/views/common.py` & `trix-4.1.2/trix/trix_student/views/common.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/views/course.py` & `trix-4.1.2/trix/trix_student/views/course.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/views/dashboard.py` & `trix-4.1.2/trix/trix_student/views/dashboard.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/views/howsolved.py` & `trix-4.1.2/trix/trix_student/views/howsolved.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/views/permalink.py` & `trix-4.1.2/trix/trix_student/views/permalink.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix/trix_student/views/users.py` & `trix-4.1.2/trix/trix_student/views/users.py`

 * *Files identical despite different names*

### Comparing `trix-4.1.1/trix.egg-info/PKG-INFO` & `trix-4.1.2/trix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trix
-Version: 4.1.1
+Version: 4.1.2
 Summary: Next generation Trix. Detailed task control and statistics app for better learning outcome.
 Home-page: https://github.com/devilry/trix2
 Author: Tor Johansen, Espen Angell Kristiansen, Jonas Sandbekk
 Author-email: tor@appresso.no, espen@appresso.no, jonassandbekk@gmail.com
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `trix-4.1.1/trix.egg-info/SOURCES.txt` & `trix-4.1.2/trix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

