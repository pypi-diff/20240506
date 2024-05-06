# Comparing `tmp/wagtail_feedback-1.3.2.tar.gz` & `tmp/wagtail_feedback-1.3.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_feedback-1.3.2.tar", last modified: Mon Mar 18 15:06:05 2024, max compression
+gzip compressed data, was "wagtail_feedback-1.3.3a1.tar", last modified: Mon May  6 16:45:19 2024, max compression
```

## Comparing `wagtail_feedback-1.3.2.tar` & `wagtail_feedback-1.3.3a1.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxrwxrwx   0        0        0        0 2024-03-18 15:06:05.343697 wagtail_feedback-1.3.2/
--rw-rw-rw-   0        0        0    18429 2024-02-20 11:29:17.000000 wagtail_feedback-1.3.2/LICENSE
--rw-rw-rw-   0        0        0      232 2024-02-23 11:47:10.000000 wagtail_feedback-1.3.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4296 2024-03-18 15:06:05.343697 wagtail_feedback-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     3199 2024-03-18 15:04:24.000000 wagtail_feedback-1.3.2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-18 15:06:05.249079 wagtail_feedback-1.3.2/feedback/
--rw-rw-rw-   0        0        0      891 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/__init__.py
--rw-rw-rw-   0        0        0      154 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/apps.py
-drwxrwxrwx   0        0        0        0 2024-03-18 15:06:05.256160 wagtail_feedback-1.3.2/feedback/backends/
--rw-rw-rw-   0        0        0      171 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/backends/__init__.py
--rw-rw-rw-   0        0        0     1275 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/backends/base.py
--rw-rw-rw-   0        0        0     1593 2024-03-14 14:06:55.000000 wagtail_feedback-1.3.2/feedback/backends/ip.py
--rw-rw-rw-   0        0        0     1788 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/backends/page.py
--rw-rw-rw-   0        0        0     1428 2024-03-14 14:14:20.000000 wagtail_feedback-1.3.2/feedback/backends/session.py
--rw-rw-rw-   0        0        0     5330 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/filters.py
--rw-rw-rw-   0        0        0     2056 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/forms.py
-drwxrwxrwx   0        0        0        0 2024-03-18 15:06:05.209592 wagtail_feedback-1.3.2/feedback/locale/
-drwxrwxrwx   0        0        0        0 2024-03-18 15:06:05.206671 wagtail_feedback-1.3.2/feedback/locale/de/
-drwxrwxrwx   0        0        0        0 2024-03-18 15:06:05.256160 wagtail_feedback-1.3.2/feedback/locale/de/LC_MESSAGES/
--rw-rw-rw-   0        0        0     6577 2024-03-13 16:48:47.000000 wagtail_feedback-1.3.2/feedback/locale/de/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    11741 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/locale/de/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-03-18 15:06:05.209592 wagtail_feedback-1.3.2/feedback/locale/fr/
-drwxrwxrwx   0        0        0        0 2024-03-18 15:06:05.263294 wagtail_feedback-1.3.2/feedback/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0        0        0     6653 2024-03-13 16:48:47.000000 wagtail_feedback-1.3.2/feedback/locale/fr/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    11817 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/locale/fr/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-03-18 15:06:05.210617 wagtail_feedback-1.3.2/feedback/locale/nl/
-drwxrwxrwx   0        0        0        0 2024-03-18 15:06:05.267334 wagtail_feedback-1.3.2/feedback/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     6356 2024-03-13 16:48:47.000000 wagtail_feedback-1.3.2/feedback/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    11536 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/locale/nl/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-03-18 15:06:05.271345 wagtail_feedback-1.3.2/feedback/migrations/
--rw-rw-rw-   0        0        0     1500 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 15:06:05.278195 wagtail_feedback-1.3.2/feedback/migrations/__pycache__/
--rw-rw-rw-   0        0        0     2127 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/migrations/__pycache__/0001_initial.cpython-311.pyc
--rw-rw-rw-   0        0        0      917 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/migrations/__pycache__/0002_alter_feedback_message.cpython-311.pyc
--rw-rw-rw-   0        0        0      227 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3658 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/mixins.py
--rw-rw-rw-   0        0        0     7617 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/models.py
--rw-rw-rw-   0        0        0      588 2024-03-14 14:19:58.000000 wagtail_feedback-1.3.2/feedback/options.py
--rw-rw-rw-   0        0        0     1899 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/panels.py
-drwxrwxrwx   0        0        0        0 2024-03-18 15:06:05.212689 wagtail_feedback-1.3.2/feedback/static/
-drwxrwxrwx   0        0        0        0 2024-03-18 15:06:05.213699 wagtail_feedback-1.3.2/feedback/static/feedback/
-drwxrwxrwx   0        0        0        0 2024-03-18 15:06:05.278195 wagtail_feedback-1.3.2/feedback/static/feedback/css/
--rw-rw-rw-   0        0        0     6832 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/static/feedback/css/feedback.css
-drwxrwxrwx   0        0        0        0 2024-03-18 15:06:05.278195 wagtail_feedback-1.3.2/feedback/static/feedback/js/
--rw-rw-rw-   0        0        0    44799 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/static/feedback/js/feedback.js
-drwxrwxrwx   0        0        0        0 2024-03-18 15:06:05.215712 wagtail_feedback-1.3.2/feedback/templates/
-drwxrwxrwx   0        0        0        0 2024-03-18 15:06:05.289967 wagtail_feedback-1.3.2/feedback/templates/feedback/
--rw-rw-rw-   0        0        0     1904 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/templates/feedback/form.html
--rw-rw-rw-   0        0        0     2887 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/templates/feedback/happy-sad.html
-drwxrwxrwx   0        0        0        0 2024-03-18 15:06:05.291695 wagtail_feedback-1.3.2/feedback/templates/feedback/panels/
--rw-rw-rw-   0        0        0      179 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/templates/feedback/panels/feedback_panel.html
-drwxrwxrwx   0        0        0        0 2024-03-18 15:06:05.306727 wagtail_feedback-1.3.2/feedback/templates/feedback/panels/partials/
--rw-rw-rw-   0        0        0     6207 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/templates/feedback/panels/partials/aggregate.html
--rw-rw-rw-   0        0        0     1177 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/templates/feedback/panels/partials/delete.html
--rw-rw-rw-   0        0        0      182 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/templates/feedback/panels/partials/error.html
--rw-rw-rw-   0        0        0     2237 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/templates/feedback/panels/partials/feedback-list-item.html
--rw-rw-rw-   0        0        0     1631 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/templates/feedback/panels/partials/filters-form.html
--rw-rw-rw-   0        0        0      897 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/templates/feedback/panels/partials/list.html
--rw-rw-rw-   0        0        0     3243 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/templates/feedback/panels/partials/paginator.html
--rw-rw-rw-   0        0        0      639 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/templates/feedback/panels/partials/wrapper.html
--rw-rw-rw-   0        0        0      251 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/templates/feedback/thanks.html
-drwxrwxrwx   0        0        0        0 2024-03-18 15:06:05.306727 wagtail_feedback-1.3.2/feedback/templates/feedback/widgets/
--rw-rw-rw-   0        0        0      417 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/templates/feedback/widgets/range-slider.html
--rw-rw-rw-   0        0        0       99 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/templates/feedback/wrapper.html
-drwxrwxrwx   0        0        0        0 2024-03-18 15:06:05.313022 wagtail_feedback-1.3.2/feedback/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 15:06:05.317046 wagtail_feedback-1.3.2/feedback/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      229 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     6604 2024-03-14 14:18:54.000000 wagtail_feedback-1.3.2/feedback/templatetags/__pycache__/feedback.cpython-311.pyc
--rw-rw-rw-   0        0        0     4192 2024-03-14 14:18:52.000000 wagtail_feedback-1.3.2/feedback/templatetags/feedback.py
--rw-rw-rw-   0        0        0       63 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/tests.py
--rw-rw-rw-   0        0        0      953 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/urls.py
-drwxrwxrwx   0        0        0        0 2024-03-18 15:06:05.326779 wagtail_feedback-1.3.2/feedback/views/
--rw-rw-rw-   0        0        0      213 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/views/__init__.py
--rw-rw-rw-   0        0        0      669 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/views/admin.py
--rw-rw-rw-   0        0        0    10936 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/views/admin_api.py
--rw-rw-rw-   0        0        0     5495 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/views/public.py
--rw-rw-rw-   0        0        0     1496 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/views/utils.py
--rw-rw-rw-   0        0        0      500 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.2/feedback/wagtail_hooks.py
--rw-rw-rw-   0        0        0       90 2024-02-20 11:29:17.000000 wagtail_feedback-1.3.2/pyproject.toml
--rw-rw-rw-   0        0        0     1071 2024-03-18 15:06:05.356615 wagtail_feedback-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-02-20 11:29:17.000000 wagtail_feedback-1.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-18 15:06:05.341699 wagtail_feedback-1.3.2/wagtail_feedback.egg-info/
--rw-rw-rw-   0        0        0     4296 2024-03-18 15:06:04.000000 wagtail_feedback-1.3.2/wagtail_feedback.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2256 2024-03-18 15:06:05.000000 wagtail_feedback-1.3.2/wagtail_feedback.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-18 15:06:04.000000 wagtail_feedback-1.3.2/wagtail_feedback.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-03-18 15:06:04.000000 wagtail_feedback-1.3.2/wagtail_feedback.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-03-18 15:06:04.000000 wagtail_feedback-1.3.2/wagtail_feedback.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 16:45:19.919047 wagtail_feedback-1.3.3a1/
+-rw-rw-rw-   0        0        0    18429 2024-02-20 11:29:17.000000 wagtail_feedback-1.3.3a1/LICENSE
+-rw-rw-rw-   0        0        0      232 2024-02-23 11:47:10.000000 wagtail_feedback-1.3.3a1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4355 2024-05-06 16:45:19.919047 wagtail_feedback-1.3.3a1/PKG-INFO
+-rw-rw-rw-   0        0        0     3256 2024-03-18 15:11:33.000000 wagtail_feedback-1.3.3a1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 16:45:19.842995 wagtail_feedback-1.3.3a1/feedback/
+-rw-rw-rw-   0        0        0      891 2024-05-06 16:42:40.000000 wagtail_feedback-1.3.3a1/feedback/__init__.py
+-rw-rw-rw-   0        0        0      154 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/apps.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:45:19.851001 wagtail_feedback-1.3.3a1/feedback/backends/
+-rw-rw-rw-   0        0        0      171 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/backends/__init__.py
+-rw-rw-rw-   0        0        0     1275 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/backends/base.py
+-rw-rw-rw-   0        0        0     1593 2024-03-14 14:06:55.000000 wagtail_feedback-1.3.3a1/feedback/backends/ip.py
+-rw-rw-rw-   0        0        0     1788 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/backends/page.py
+-rw-rw-rw-   0        0        0     1428 2024-03-14 14:14:20.000000 wagtail_feedback-1.3.3a1/feedback/backends/session.py
+-rw-rw-rw-   0        0        0     5330 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/filters.py
+-rw-rw-rw-   0        0        0     2056 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/forms.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:45:19.816102 wagtail_feedback-1.3.3a1/feedback/locale/
+drwxrwxrwx   0        0        0        0 2024-05-06 16:45:19.815227 wagtail_feedback-1.3.3a1/feedback/locale/de/
+drwxrwxrwx   0        0        0        0 2024-05-06 16:45:19.854095 wagtail_feedback-1.3.3a1/feedback/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     6577 2024-03-13 16:48:47.000000 wagtail_feedback-1.3.3a1/feedback/locale/de/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    11741 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/locale/de/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-05-06 16:45:19.816102 wagtail_feedback-1.3.3a1/feedback/locale/fr/
+drwxrwxrwx   0        0        0        0 2024-05-06 16:45:19.856319 wagtail_feedback-1.3.3a1/feedback/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     6653 2024-03-13 16:48:47.000000 wagtail_feedback-1.3.3a1/feedback/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    11817 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/locale/fr/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-05-06 16:45:19.816102 wagtail_feedback-1.3.3a1/feedback/locale/nl/
+drwxrwxrwx   0        0        0        0 2024-05-06 16:45:19.860021 wagtail_feedback-1.3.3a1/feedback/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     6356 2024-03-13 16:48:47.000000 wagtail_feedback-1.3.3a1/feedback/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    11536 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/locale/nl/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-05-06 16:45:19.864023 wagtail_feedback-1.3.3a1/feedback/migrations/
+-rw-rw-rw-   0        0        0     1500 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:45:19.870021 wagtail_feedback-1.3.3a1/feedback/migrations/__pycache__/
+-rw-rw-rw-   0        0        0     2127 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/migrations/__pycache__/0001_initial.cpython-311.pyc
+-rw-rw-rw-   0        0        0      917 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/migrations/__pycache__/0002_alter_feedback_message.cpython-311.pyc
+-rw-rw-rw-   0        0        0      227 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3658 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/mixins.py
+-rw-rw-rw-   0        0        0     7617 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/models.py
+-rw-rw-rw-   0        0        0      588 2024-03-14 14:19:58.000000 wagtail_feedback-1.3.3a1/feedback/options.py
+-rw-rw-rw-   0        0        0     1899 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/panels.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:45:19.818076 wagtail_feedback-1.3.3a1/feedback/static/
+drwxrwxrwx   0        0        0        0 2024-05-06 16:45:19.819075 wagtail_feedback-1.3.3a1/feedback/static/feedback/
+drwxrwxrwx   0        0        0        0 2024-05-06 16:45:19.872022 wagtail_feedback-1.3.3a1/feedback/static/feedback/css/
+-rw-rw-rw-   0        0        0     6832 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/static/feedback/css/feedback.css
+drwxrwxrwx   0        0        0        0 2024-05-06 16:45:19.873021 wagtail_feedback-1.3.3a1/feedback/static/feedback/js/
+-rw-rw-rw-   0        0        0    44799 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/static/feedback/js/feedback.js
+drwxrwxrwx   0        0        0        0 2024-05-06 16:45:19.820076 wagtail_feedback-1.3.3a1/feedback/templates/
+drwxrwxrwx   0        0        0        0 2024-05-06 16:45:19.881022 wagtail_feedback-1.3.3a1/feedback/templates/feedback/
+-rw-rw-rw-   0        0        0     1904 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/templates/feedback/form.html
+-rw-rw-rw-   0        0        0     2887 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/templates/feedback/happy-sad.html
+drwxrwxrwx   0        0        0        0 2024-05-06 16:45:19.883024 wagtail_feedback-1.3.3a1/feedback/templates/feedback/panels/
+-rw-rw-rw-   0        0        0      179 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/templates/feedback/panels/feedback_panel.html
+drwxrwxrwx   0        0        0        0 2024-05-06 16:45:19.895024 wagtail_feedback-1.3.3a1/feedback/templates/feedback/panels/partials/
+-rw-rw-rw-   0        0        0     6207 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/templates/feedback/panels/partials/aggregate.html
+-rw-rw-rw-   0        0        0     1177 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/templates/feedback/panels/partials/delete.html
+-rw-rw-rw-   0        0        0      182 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/templates/feedback/panels/partials/error.html
+-rw-rw-rw-   0        0        0     2237 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/templates/feedback/panels/partials/feedback-list-item.html
+-rw-rw-rw-   0        0        0     1631 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/templates/feedback/panels/partials/filters-form.html
+-rw-rw-rw-   0        0        0      897 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/templates/feedback/panels/partials/list.html
+-rw-rw-rw-   0        0        0     3243 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/templates/feedback/panels/partials/paginator.html
+-rw-rw-rw-   0        0        0      639 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/templates/feedback/panels/partials/wrapper.html
+-rw-rw-rw-   0        0        0      251 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/templates/feedback/thanks.html
+drwxrwxrwx   0        0        0        0 2024-05-06 16:45:19.898022 wagtail_feedback-1.3.3a1/feedback/templates/feedback/widgets/
+-rw-rw-rw-   0        0        0      417 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/templates/feedback/widgets/range-slider.html
+-rw-rw-rw-   0        0        0       99 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/templates/feedback/wrapper.html
+drwxrwxrwx   0        0        0        0 2024-05-06 16:45:19.900021 wagtail_feedback-1.3.3a1/feedback/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:45:19.903023 wagtail_feedback-1.3.3a1/feedback/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      229 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6604 2024-03-14 14:18:54.000000 wagtail_feedback-1.3.3a1/feedback/templatetags/__pycache__/feedback.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4192 2024-03-14 14:18:52.000000 wagtail_feedback-1.3.3a1/feedback/templatetags/feedback.py
+-rw-rw-rw-   0        0        0       63 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/tests.py
+-rw-rw-rw-   0        0        0      953 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/urls.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:45:19.908573 wagtail_feedback-1.3.3a1/feedback/views/
+-rw-rw-rw-   0        0        0      213 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/views/__init__.py
+-rw-rw-rw-   0        0        0      669 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/views/admin.py
+-rw-rw-rw-   0        0        0    10936 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/views/admin_api.py
+-rw-rw-rw-   0        0        0     5491 2024-05-06 16:41:47.000000 wagtail_feedback-1.3.3a1/feedback/views/public.py
+-rw-rw-rw-   0        0        0     1496 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/views/utils.py
+-rw-rw-rw-   0        0        0      500 2024-03-13 12:42:47.000000 wagtail_feedback-1.3.3a1/feedback/wagtail_hooks.py
+-rw-rw-rw-   0        0        0       90 2024-02-20 11:29:17.000000 wagtail_feedback-1.3.3a1/pyproject.toml
+-rw-rw-rw-   0        0        0     1073 2024-05-06 16:45:19.921046 wagtail_feedback-1.3.3a1/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-02-20 11:29:17.000000 wagtail_feedback-1.3.3a1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:45:19.918048 wagtail_feedback-1.3.3a1/wagtail_feedback.egg-info/
+-rw-rw-rw-   0        0        0     4355 2024-05-06 16:45:19.000000 wagtail_feedback-1.3.3a1/wagtail_feedback.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2256 2024-05-06 16:45:19.000000 wagtail_feedback-1.3.3a1/wagtail_feedback.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 16:45:19.000000 wagtail_feedback-1.3.3a1/wagtail_feedback.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-06 16:45:19.000000 wagtail_feedback-1.3.3a1/wagtail_feedback.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-06 16:45:19.000000 wagtail_feedback-1.3.3a1/wagtail_feedback.egg-info/top_level.txt
```

### Comparing `wagtail_feedback-1.3.2/LICENSE` & `wagtail_feedback-1.3.3a1/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_feedback-1.3.2/PKG-INFO` & `wagtail_feedback-1.3.3a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_feedback
-Version: 1.3.2
+Version: 1.3.3a1
 Summary: A Django/Wagtail app to easily ask users for feedback.
 Home-page: https://github.com/Nigel2392/wagtail_feedback
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -111,35 +111,39 @@
 
 Other backends include:
 
 * `feedback.backends.SessionBasedFeedbackend`
 * `feedback.backends.PageBasedFeedbackend`
 * `feedback.backends.Feedbackend` *(base implementation)*
 
-
 ## **Custom page methods for specifying messages/functionality**
 
 Specifies if the user is allowed to leave a message on positive feedback for this page.
 
-`def allow_feedback_message_on_positive(self):`
+`def allow_feedback_message_on_positive(self) -> bool:`
 
 Specifies the title shown above the feedback form.
-`def get_feedback_title(self):`
 
-How you would like to thank your user after submitting the feedback
-`def get_feedback_thanks(self):`
+`def get_feedback_title(self) -> str:`
+
+How you would like to thank your user after submitting the feedback.
+
+`def get_feedback_thanks(self) -> str:`
+
+A simple short description explaining why you are asking for feedback.
+
+`def get_feedback_explainer(self) -> str:`
+
+Text shown when the user hovers over the positive icon.  
 
-A simple short description explaining why you are asking for feedback
-`def get_feedback_explainer(self):`
+`def get_feedback_positive_text(self) -> str:`
 
-Text shown when the user hovers over the positive icon.
-`def get_feedback_positive_text(self):`
+Text shown when the user hovers over the negative icon.  
 
-Text shown when the user hovers over the negative icon.
-`def get_feedback_negative_text(self):`
+`def get_feedback_negative_text(self) -> str:`
 
 ## **Django proxy settings to get IP-adress**
 
 `USE_X_FORWARDED_HOST` *default: `False`*
 
 Used for setting the appropriate IP-adress on the
```

### Comparing `wagtail_feedback-1.3.2/README.md` & `wagtail_feedback-1.3.3a1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -83,35 +83,39 @@
 
 Other backends include:
 
 * `feedback.backends.SessionBasedFeedbackend`
 * `feedback.backends.PageBasedFeedbackend`
 * `feedback.backends.Feedbackend` *(base implementation)*
 
-
 ## **Custom page methods for specifying messages/functionality**
 
 Specifies if the user is allowed to leave a message on positive feedback for this page.
 
-`def allow_feedback_message_on_positive(self):`
+`def allow_feedback_message_on_positive(self) -> bool:`
 
 Specifies the title shown above the feedback form.
-`def get_feedback_title(self):`
 
-How you would like to thank your user after submitting the feedback
-`def get_feedback_thanks(self):`
+`def get_feedback_title(self) -> str:`
+
+How you would like to thank your user after submitting the feedback.
+
+`def get_feedback_thanks(self) -> str:`
+
+A simple short description explaining why you are asking for feedback.
+
+`def get_feedback_explainer(self) -> str:`
+
+Text shown when the user hovers over the positive icon.  
 
-A simple short description explaining why you are asking for feedback
-`def get_feedback_explainer(self):`
+`def get_feedback_positive_text(self) -> str:`
 
-Text shown when the user hovers over the positive icon.
-`def get_feedback_positive_text(self):`
+Text shown when the user hovers over the negative icon.  
 
-Text shown when the user hovers over the negative icon.
-`def get_feedback_negative_text(self):`
+`def get_feedback_negative_text(self) -> str:`
 
 ## **Django proxy settings to get IP-adress**
 
 `USE_X_FORWARDED_HOST` *default: `False`*
 
 Used for setting the appropriate IP-adress on the
```

### Comparing `wagtail_feedback-1.3.2/feedback/__init__.py` & `wagtail_feedback-1.3.3a1/feedback/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtail_feedback-1.3.2/feedback/backends/base.py` & `wagtail_feedback-1.3.3a1/feedback/backends/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_feedback-1.3.2/feedback/backends/ip.py` & `wagtail_feedback-1.3.3a1/feedback/backends/ip.py`

 * *Files identical despite different names*

### Comparing `wagtail_feedback-1.3.2/feedback/backends/page.py` & `wagtail_feedback-1.3.3a1/feedback/backends/page.py`

 * *Files identical despite different names*

### Comparing `wagtail_feedback-1.3.2/feedback/backends/session.py` & `wagtail_feedback-1.3.3a1/feedback/backends/session.py`

 * *Files identical despite different names*

### Comparing `wagtail_feedback-1.3.2/feedback/filters.py` & `wagtail_feedback-1.3.3a1/feedback/filters.py`

 * *Files identical despite different names*

### Comparing `wagtail_feedback-1.3.2/feedback/forms.py` & `wagtail_feedback-1.3.3a1/feedback/forms.py`

 * *Files identical despite different names*

### Comparing `wagtail_feedback-1.3.2/feedback/locale/de/LC_MESSAGES/django.mo` & `wagtail_feedback-1.3.3a1/feedback/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_feedback-1.3.2/feedback/locale/de/LC_MESSAGES/django.po` & `wagtail_feedback-1.3.3a1/feedback/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_feedback-1.3.2/feedback/locale/fr/LC_MESSAGES/django.mo` & `wagtail_feedback-1.3.3a1/feedback/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_feedback-1.3.2/feedback/locale/fr/LC_MESSAGES/django.po` & `wagtail_feedback-1.3.3a1/feedback/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_feedback-1.3.2/feedback/locale/nl/LC_MESSAGES/django.mo` & `wagtail_feedback-1.3.3a1/feedback/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_feedback-1.3.2/feedback/locale/nl/LC_MESSAGES/django.po` & `wagtail_feedback-1.3.3a1/feedback/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_feedback-1.3.2/feedback/migrations/0001_initial.py` & `wagtail_feedback-1.3.3a1/feedback/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_feedback-1.3.2/feedback/migrations/__pycache__/0001_initial.cpython-311.pyc` & `wagtail_feedback-1.3.3a1/feedback/migrations/__pycache__/0001_initial.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wagtail_feedback-1.3.2/feedback/migrations/__pycache__/0002_alter_feedback_message.cpython-311.pyc` & `wagtail_feedback-1.3.3a1/feedback/migrations/__pycache__/0002_alter_feedback_message.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wagtail_feedback-1.3.2/feedback/mixins.py` & `wagtail_feedback-1.3.3a1/feedback/mixins.py`

 * *Files identical despite different names*

### Comparing `wagtail_feedback-1.3.2/feedback/models.py` & `wagtail_feedback-1.3.3a1/feedback/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_feedback-1.3.2/feedback/options.py` & `wagtail_feedback-1.3.3a1/feedback/options.py`

 * *Files identical despite different names*

### Comparing `wagtail_feedback-1.3.2/feedback/panels.py` & `wagtail_feedback-1.3.3a1/feedback/panels.py`

 * *Files identical despite different names*

### Comparing `wagtail_feedback-1.3.2/feedback/static/feedback/css/feedback.css` & `wagtail_feedback-1.3.3a1/feedback/static/feedback/css/feedback.css`

 * *Files identical despite different names*

### Comparing `wagtail_feedback-1.3.2/feedback/static/feedback/js/feedback.js` & `wagtail_feedback-1.3.3a1/feedback/static/feedback/js/feedback.js`

 * *Files identical despite different names*

### Comparing `wagtail_feedback-1.3.2/feedback/templates/feedback/form.html` & `wagtail_feedback-1.3.3a1/feedback/templates/feedback/form.html`

 * *Files identical despite different names*

### Comparing `wagtail_feedback-1.3.2/feedback/templates/feedback/happy-sad.html` & `wagtail_feedback-1.3.3a1/feedback/templates/feedback/happy-sad.html`

 * *Files identical despite different names*

### Comparing `wagtail_feedback-1.3.2/feedback/templates/feedback/panels/partials/aggregate.html` & `wagtail_feedback-1.3.3a1/feedback/templates/feedback/panels/partials/aggregate.html`

 * *Files identical despite different names*

### Comparing `wagtail_feedback-1.3.2/feedback/templates/feedback/panels/partials/delete.html` & `wagtail_feedback-1.3.3a1/feedback/templates/feedback/panels/partials/delete.html`

 * *Files identical despite different names*

### Comparing `wagtail_feedback-1.3.2/feedback/templates/feedback/panels/partials/feedback-list-item.html` & `wagtail_feedback-1.3.3a1/feedback/templates/feedback/panels/partials/feedback-list-item.html`

 * *Files identical despite different names*

### Comparing `wagtail_feedback-1.3.2/feedback/templates/feedback/panels/partials/filters-form.html` & `wagtail_feedback-1.3.3a1/feedback/templates/feedback/panels/partials/filters-form.html`

 * *Files identical despite different names*

### Comparing `wagtail_feedback-1.3.2/feedback/templates/feedback/panels/partials/list.html` & `wagtail_feedback-1.3.3a1/feedback/templates/feedback/panels/partials/list.html`

 * *Files identical despite different names*

### Comparing `wagtail_feedback-1.3.2/feedback/templates/feedback/panels/partials/paginator.html` & `wagtail_feedback-1.3.3a1/feedback/templates/feedback/panels/partials/paginator.html`

 * *Files identical despite different names*

### Comparing `wagtail_feedback-1.3.2/feedback/templates/feedback/panels/partials/wrapper.html` & `wagtail_feedback-1.3.3a1/feedback/templates/feedback/panels/partials/wrapper.html`

 * *Files identical despite different names*

### Comparing `wagtail_feedback-1.3.2/feedback/templatetags/__pycache__/feedback.cpython-311.pyc` & `wagtail_feedback-1.3.3a1/feedback/templatetags/__pycache__/feedback.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wagtail_feedback-1.3.2/feedback/templatetags/feedback.py` & `wagtail_feedback-1.3.3a1/feedback/templatetags/feedback.py`

 * *Files identical despite different names*

### Comparing `wagtail_feedback-1.3.2/feedback/urls.py` & `wagtail_feedback-1.3.3a1/feedback/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_feedback-1.3.2/feedback/views/admin.py` & `wagtail_feedback-1.3.3a1/feedback/views/admin.py`

 * *Files identical despite different names*

### Comparing `wagtail_feedback-1.3.2/feedback/views/admin_api.py` & `wagtail_feedback-1.3.3a1/feedback/views/admin_api.py`

 * *Files identical despite different names*

### Comparing `wagtail_feedback-1.3.2/feedback/views/public.py` & `wagtail_feedback-1.3.3a1/feedback/views/public.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
             fn(request, form.instance)
 
         backend.end_check(request, page, form, form.instance, exists=False)
 
         # If the feedback is positive and it is allowed, or if it is negative
         # then show the message form.
         if hasattr(page, "allow_feedback_message_on_positive")\
-            and not page.allow_feedback_message_on_positive()\
+            and page.allow_feedback_message_on_positive()\
             and form.instance.positive\
             or not form.instance.positive:
 
             form = FeedbackForm(
                 request=request,
                 page=page,
                 requires_message=True,
```

### Comparing `wagtail_feedback-1.3.2/feedback/views/utils.py` & `wagtail_feedback-1.3.3a1/feedback/views/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_feedback-1.3.2/setup.cfg` & `wagtail_feedback-1.3.3a1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,67 +1,68 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6565 6462   = wagtail_feedb
 00000020: 6163 6b0d 0a76 6572 7369 6f6e 203d 2031  ack..version = 1
-00000030: 2e33 2e32 0d0a 6465 7363 7269 7074 696f  .3.2..descriptio
-00000040: 6e20 3d20 4120 446a 616e 676f 2f57 6167  n = A Django/Wag
-00000050: 7461 696c 2061 7070 2074 6f20 6561 7369  tail app to easi
-00000060: 6c79 2061 736b 2075 7365 7273 2066 6f72  ly ask users for
-00000070: 2066 6565 6462 6163 6b2e 0d0a 6c6f 6e67   feedback...long
-00000080: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
-00000090: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
-000000a0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-000000b0: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
-000000c0: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a61  text/markdown..a
-000000d0: 7574 686f 7220 3d20 4e69 6765 6c0d 0a61  uthor = Nigel..a
-000000e0: 7574 686f 725f 656d 6169 6c20 3d20 6e69  uthor_email = ni
-000000f0: 6765 6c40 676f 6f64 6164 7669 6365 2e69  gel@goodadvice.i
-00000100: 740d 0a6c 6963 656e 7365 203d 2047 504c  t..license = GPL
-00000110: 2d33 2e30 2d6f 6e6c 790d 0a75 726c 203d  -3.0-only..url =
-00000120: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000130: 636f 6d2f 4e69 6765 6c32 3339 322f 7761  com/Nigel2392/wa
-00000140: 6774 6169 6c5f 6665 6564 6261 636b 0d0a  gtail_feedback..
-00000150: 636c 6173 7369 6669 6572 7320 3d20 0d0a  classifiers = ..
-00000160: 0945 6e76 6972 6f6e 6d65 6e74 203a 3a20  .Environment :: 
-00000170: 5765 6220 456e 7669 726f 6e6d 656e 740d  Web Environment.
-00000180: 0a09 4672 616d 6577 6f72 6b20 3a3a 2044  ..Framework :: D
-00000190: 6a61 6e67 6f0d 0a09 4672 616d 6577 6f72  jango...Framewor
-000001a0: 6b20 3a3a 2044 6a61 6e67 6f20 3a3a 2034  k :: Django :: 4
-000001b0: 2e32 0d0a 0949 6e74 656e 6465 6420 4175  .2...Intended Au
-000001c0: 6469 656e 6365 203a 3a20 4465 7665 6c6f  dience :: Develo
-000001d0: 7065 7273 0d0a 094c 6963 656e 7365 203a  pers...License :
-000001e0: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
-000001f0: 3a20 474e 5520 4765 6e65 7261 6c20 5075  : GNU General Pu
-00000200: 626c 6963 204c 6963 656e 7365 2076 3320  blic License v3 
-00000210: 6f72 206c 6174 6572 2028 4750 4c76 332b  or later (GPLv3+
-00000220: 290d 0a09 4f70 6572 6174 696e 6720 5379  )...Operating Sy
-00000230: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
-00000240: 656e 6465 6e74 0d0a 0950 726f 6772 616d  endent...Program
-00000250: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000260: 2050 7974 686f 6e0d 0a09 5072 6f67 7261   Python...Progra
-00000270: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000280: 3a20 5079 7468 6f6e 203a 3a20 330d 0a09  : Python :: 3...
-00000290: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000002a0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000002b0: 3a20 3320 3a3a 204f 6e6c 790d 0a09 5072  : 3 :: Only...Pr
-000002c0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000002d0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-000002e0: 332e 380d 0a09 5072 6f67 7261 6d6d 696e  3.8...Programmin
-000002f0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000300: 7468 6f6e 203a 3a20 332e 390d 0a09 546f  thon :: 3.9...To
-00000310: 7069 6320 3a3a 2049 6e74 6572 6e65 7420  pic :: Internet 
-00000320: 3a3a 2057 5757 2f48 5454 500d 0a09 546f  :: WWW/HTTP...To
-00000330: 7069 6320 3a3a 2049 6e74 6572 6e65 7420  pic :: Internet 
-00000340: 3a3a 2057 5757 2f48 5454 5020 3a3a 2044  :: WWW/HTTP :: D
-00000350: 796e 616d 6963 2043 6f6e 7465 6e74 0d0a  ynamic Content..
-00000360: 0d0a 5b6f 7074 696f 6e73 5d0d 0a69 6e63  ..[options]..inc
-00000370: 6c75 6465 5f70 6163 6b61 6765 5f64 6174  lude_package_dat
-00000380: 6120 3d20 7472 7565 0d0a 7061 636b 6167  a = true..packag
-00000390: 6573 203d 2066 696e 643a 0d0a 7079 7468  es = find:..pyth
-000003a0: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
-000003b0: 332e 380d 0a69 6e73 7461 6c6c 5f72 6571  3.8..install_req
-000003c0: 7569 7265 7320 3d20 0d0a 0944 6a61 6e67  uires = ...Djang
-000003d0: 6f20 3e3d 2034 2e32 0d0a 0957 6167 7461  o >= 4.2...Wagta
-000003e0: 696c 203e 3d20 342e 320d 0a09 646a 616e  il >= 4.2...djan
-000003f0: 676f 2d66 696c 7465 7220 3e3d 2032 332e  go-filter >= 23.
-00000400: 320d 0a0d 0a5b 6567 675f 696e 666f 5d0d  2....[egg_info].
-00000410: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
-00000420: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
+00000030: 2e33 2e33 6131 0d0a 6465 7363 7269 7074  .3.3a1..descript
+00000040: 696f 6e20 3d20 4120 446a 616e 676f 2f57  ion = A Django/W
+00000050: 6167 7461 696c 2061 7070 2074 6f20 6561  agtail app to ea
+00000060: 7369 6c79 2061 736b 2075 7365 7273 2066  sily ask users f
+00000070: 6f72 2066 6565 6462 6163 6b2e 0d0a 6c6f  or feedback...lo
+00000080: 6e67 5f64 6573 6372 6970 7469 6f6e 203d  ng_description =
+00000090: 2066 696c 653a 2052 4541 444d 452e 6d64   file: README.md
+000000a0: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
+000000b0: 6f6e 5f63 6f6e 7465 6e74 5f74 7970 6520  on_content_type 
+000000c0: 3d20 7465 7874 2f6d 6172 6b64 6f77 6e0d  = text/markdown.
+000000d0: 0a61 7574 686f 7220 3d20 4e69 6765 6c0d  .author = Nigel.
+000000e0: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
+000000f0: 6e69 6765 6c40 676f 6f64 6164 7669 6365  nigel@goodadvice
+00000100: 2e69 740d 0a6c 6963 656e 7365 203d 2047  .it..license = G
+00000110: 504c 2d33 2e30 2d6f 6e6c 790d 0a75 726c  PL-3.0-only..url
+00000120: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
+00000130: 622e 636f 6d2f 4e69 6765 6c32 3339 322f  b.com/Nigel2392/
+00000140: 7761 6774 6169 6c5f 6665 6564 6261 636b  wagtail_feedback
+00000150: 0d0a 636c 6173 7369 6669 6572 7320 3d20  ..classifiers = 
+00000160: 0d0a 0945 6e76 6972 6f6e 6d65 6e74 203a  ...Environment :
+00000170: 3a20 5765 6220 456e 7669 726f 6e6d 656e  : Web Environmen
+00000180: 740d 0a09 4672 616d 6577 6f72 6b20 3a3a  t...Framework ::
+00000190: 2044 6a61 6e67 6f0d 0a09 4672 616d 6577   Django...Framew
+000001a0: 6f72 6b20 3a3a 2044 6a61 6e67 6f20 3a3a  ork :: Django ::
+000001b0: 2034 2e32 0d0a 0949 6e74 656e 6465 6420   4.2...Intended 
+000001c0: 4175 6469 656e 6365 203a 3a20 4465 7665  Audience :: Deve
+000001d0: 6c6f 7065 7273 0d0a 094c 6963 656e 7365  lopers...License
+000001e0: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
+000001f0: 203a 3a20 474e 5520 4765 6e65 7261 6c20   :: GNU General 
+00000200: 5075 626c 6963 204c 6963 656e 7365 2076  Public License v
+00000210: 3320 6f72 206c 6174 6572 2028 4750 4c76  3 or later (GPLv
+00000220: 332b 290d 0a09 4f70 6572 6174 696e 6720  3+)...Operating 
+00000230: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
+00000240: 6570 656e 6465 6e74 0d0a 0950 726f 6772  ependent...Progr
+00000250: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000260: 3a3a 2050 7974 686f 6e0d 0a09 5072 6f67  :: Python...Prog
+00000270: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000280: 203a 3a20 5079 7468 6f6e 203a 3a20 330d   :: Python :: 3.
+00000290: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+000002a0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+000002b0: 203a 3a20 3320 3a3a 204f 6e6c 790d 0a09   :: 3 :: Only...
+000002c0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000002d0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+000002e0: 3a20 332e 380d 0a09 5072 6f67 7261 6d6d  : 3.8...Programm
+000002f0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000300: 5079 7468 6f6e 203a 3a20 332e 390d 0a09  Python :: 3.9...
+00000310: 546f 7069 6320 3a3a 2049 6e74 6572 6e65  Topic :: Interne
+00000320: 7420 3a3a 2057 5757 2f48 5454 500d 0a09  t :: WWW/HTTP...
+00000330: 546f 7069 6320 3a3a 2049 6e74 6572 6e65  Topic :: Interne
+00000340: 7420 3a3a 2057 5757 2f48 5454 5020 3a3a  t :: WWW/HTTP ::
+00000350: 2044 796e 616d 6963 2043 6f6e 7465 6e74   Dynamic Content
+00000360: 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d 0a69  ....[options]..i
+00000370: 6e63 6c75 6465 5f70 6163 6b61 6765 5f64  nclude_package_d
+00000380: 6174 6120 3d20 7472 7565 0d0a 7061 636b  ata = true..pack
+00000390: 6167 6573 203d 2066 696e 643a 0d0a 7079  ages = find:..py
+000003a0: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
+000003b0: 3e3d 332e 380d 0a69 6e73 7461 6c6c 5f72  >=3.8..install_r
+000003c0: 6571 7569 7265 7320 3d20 0d0a 0944 6a61  equires = ...Dja
+000003d0: 6e67 6f20 3e3d 2034 2e32 0d0a 0957 6167  ngo >= 4.2...Wag
+000003e0: 7461 696c 203e 3d20 342e 320d 0a09 646a  tail >= 4.2...dj
+000003f0: 616e 676f 2d66 696c 7465 7220 3e3d 2032  ango-filter >= 2
+00000400: 332e 320d 0a0d 0a5b 6567 675f 696e 666f  3.2....[egg_info
+00000410: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
+00000420: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
+00000430: 0a                                       .
```

### Comparing `wagtail_feedback-1.3.2/wagtail_feedback.egg-info/PKG-INFO` & `wagtail_feedback-1.3.3a1/wagtail_feedback.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_feedback
-Version: 1.3.2
+Version: 1.3.3a1
 Summary: A Django/Wagtail app to easily ask users for feedback.
 Home-page: https://github.com/Nigel2392/wagtail_feedback
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -111,35 +111,39 @@
 
 Other backends include:
 
 * `feedback.backends.SessionBasedFeedbackend`
 * `feedback.backends.PageBasedFeedbackend`
 * `feedback.backends.Feedbackend` *(base implementation)*
 
-
 ## **Custom page methods for specifying messages/functionality**
 
 Specifies if the user is allowed to leave a message on positive feedback for this page.
 
-`def allow_feedback_message_on_positive(self):`
+`def allow_feedback_message_on_positive(self) -> bool:`
 
 Specifies the title shown above the feedback form.
-`def get_feedback_title(self):`
 
-How you would like to thank your user after submitting the feedback
-`def get_feedback_thanks(self):`
+`def get_feedback_title(self) -> str:`
+
+How you would like to thank your user after submitting the feedback.
+
+`def get_feedback_thanks(self) -> str:`
+
+A simple short description explaining why you are asking for feedback.
+
+`def get_feedback_explainer(self) -> str:`
+
+Text shown when the user hovers over the positive icon.  
 
-A simple short description explaining why you are asking for feedback
-`def get_feedback_explainer(self):`
+`def get_feedback_positive_text(self) -> str:`
 
-Text shown when the user hovers over the positive icon.
-`def get_feedback_positive_text(self):`
+Text shown when the user hovers over the negative icon.  
 
-Text shown when the user hovers over the negative icon.
-`def get_feedback_negative_text(self):`
+`def get_feedback_negative_text(self) -> str:`
 
 ## **Django proxy settings to get IP-adress**
 
 `USE_X_FORWARDED_HOST` *default: `False`*
 
 Used for setting the appropriate IP-adress on the
```

### Comparing `wagtail_feedback-1.3.2/wagtail_feedback.egg-info/SOURCES.txt` & `wagtail_feedback-1.3.3a1/wagtail_feedback.egg-info/SOURCES.txt`

 * *Files identical despite different names*

