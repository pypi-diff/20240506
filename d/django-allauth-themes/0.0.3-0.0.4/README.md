# Comparing `tmp/django_allauth_themes-0.0.3.tar.gz` & `tmp/django_allauth_themes-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_allauth_themes-0.0.3.tar", last modified: Sun May  5 13:31:06 2024, max compression
+gzip compressed data, was "django_allauth_themes-0.0.4.tar", last modified: Sun May  5 19:08:39 2024, max compression
```

## Comparing `django_allauth_themes-0.0.3.tar` & `django_allauth_themes-0.0.4.tar`

### file list

```diff
@@ -1,97 +1,52 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 13:31:06.320333 django_allauth_themes-0.0.3/
--rw-rw-rw-   0        0        0     1064 2024-05-03 03:15:33.000000 django_allauth_themes-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       40 2024-05-05 13:23:31.000000 django_allauth_themes-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2467 2024-05-05 13:31:06.319332 django_allauth_themes-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      852 2024-05-03 03:22:26.000000 django_allauth_themes-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 13:31:06.199952 django_allauth_themes-0.0.3/allauth_themes/
-drwxrwxrwx   0        0        0        0 2024-05-05 13:31:06.210951 django_allauth_themes-0.0.3/allauth_themes/allauth/
--rw-rw-rw-   0        0        0      293 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.3/allauth_themes/allauth/429.html
-drwxrwxrwx   0        0        0        0 2024-05-05 13:31:06.213953 django_allauth_themes-0.0.3/allauth_themes/allauth/account/
--rw-rw-rw-   0        0        0      110 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.3/allauth_themes/allauth/account/base_manage_email.html
--rw-rw-rw-   0        0        0      113 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.3/allauth_themes/allauth/account/base_manage_password.html
-drwxrwxrwx   0        0        0        0 2024-05-05 13:31:06.194951 django_allauth_themes-0.0.3/allauth_themes/allauth/allauth/
-drwxrwxrwx   0        0        0        0 2024-05-05 13:31:06.236333 django_allauth_themes-0.0.3/allauth_themes/allauth/allauth/elements/
--rw-rw-rw-   0        0        0      123 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.3/allauth_themes/allauth/allauth/elements/alert.html
--rw-rw-rw-   0        0        0      348 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.3/allauth_themes/allauth/allauth/elements/badge.html
--rw-rw-rw-   0        0        0     1615 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.3/allauth_themes/allauth/allauth/elements/button.html
--rw-rw-rw-   0        0        0      129 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.3/allauth_themes/allauth/allauth/elements/button__entrance.html
--rw-rw-rw-   0        0        0     3001 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.3/allauth_themes/allauth/allauth/elements/field.html
--rw-rw-rw-   0        0        0      603 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.3/allauth_themes/allauth/allauth/elements/fields.html
--rw-rw-rw-   0        0        0      673 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.3/allauth_themes/allauth/allauth/elements/form.html
--rw-rw-rw-   0        0        0       80 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.3/allauth_themes/allauth/allauth/elements/form__entrance.html
--rw-rw-rw-   0        0        0       84 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.3/allauth_themes/allauth/allauth/elements/h1.html
--rw-rw-rw-   0        0        0       92 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.3/allauth_themes/allauth/allauth/elements/h1__entrance.html
--rw-rw-rw-   0        0        0       92 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.3/allauth_themes/allauth/allauth/elements/h2__entrance.html
--rw-rw-rw-   0        0        0      152 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.3/allauth_themes/allauth/allauth/elements/img.html
--rw-rw-rw-   0        0        0      385 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.3/allauth_themes/allauth/allauth/elements/panel.html
--rw-rw-rw-   0        0        0      122 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.3/allauth_themes/allauth/allauth/elements/provider.html
--rw-rw-rw-   0        0        0       92 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.3/allauth_themes/allauth/allauth/elements/provider_list.html
--rw-rw-rw-   0        0        0       97 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.3/allauth_themes/allauth/allauth/elements/table.html
-drwxrwxrwx   0        0        0        0 2024-05-05 13:31:06.241333 django_allauth_themes-0.0.3/allauth_themes/allauth/allauth/layouts/
--rw-rw-rw-   0        0        0     4814 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.3/allauth_themes/allauth/allauth/layouts/base.html
--rw-rw-rw-   0        0        0      812 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.3/allauth_themes/allauth/allauth/layouts/entrance.html
--rw-rw-rw-   0        0        0     2444 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.3/allauth_themes/allauth/allauth/layouts/manage.html
--rw-rw-rw-   0        0        0      232 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.3/allauth_themes/allauth/index.html
-drwxrwxrwx   0        0        0        0 2024-05-05 13:31:06.242332 django_allauth_themes-0.0.3/allauth_themes/allauth/mfa/
--rw-rw-rw-   0        0        0      108 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.3/allauth_themes/allauth/mfa/base_manage.html
--rw-rw-rw-   0        0        0      188 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.3/allauth_themes/allauth/profile.html
-drwxrwxrwx   0        0        0        0 2024-05-05 13:31:06.244334 django_allauth_themes-0.0.3/allauth_themes/allauth/socialaccount/
--rw-rw-rw-   0        0        0      118 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.3/allauth_themes/allauth/socialaccount/base_manage.html
-drwxrwxrwx   0        0        0        0 2024-05-05 13:31:06.245332 django_allauth_themes-0.0.3/allauth_themes/allauth/usersessions/
--rw-rw-rw-   0        0        0      117 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.3/allauth_themes/allauth/usersessions/base_manage.html
-drwxrwxrwx   0        0        0        0 2024-05-05 13:31:06.250333 django_allauth_themes-0.0.3/allauth_themes/bs5/
--rw-rw-rw-   0        0        0      385 2024-05-04 23:42:47.000000 django_allauth_themes-0.0.3/allauth_themes/bs5/429.html
-drwxrwxrwx   0        0        0        0 2024-05-05 13:31:06.198954 django_allauth_themes-0.0.3/allauth_themes/bs5/allauth/
-drwxrwxrwx   0        0        0        0 2024-05-05 13:31:06.273332 django_allauth_themes-0.0.3/allauth_themes/bs5/allauth/elements/
--rw-rw-rw-   0        0        0       85 2024-05-03 01:14:47.000000 django_allauth_themes-0.0.3/allauth_themes/bs5/allauth/elements/alert.html
--rw-rw-rw-   0        0        0       71 2024-05-03 01:14:47.000000 django_allauth_themes-0.0.3/allauth_themes/bs5/allauth/elements/badge.html
--rw-rw-rw-   0        0        0      479 2024-05-03 01:14:47.000000 django_allauth_themes-0.0.3/allauth_themes/bs5/allauth/elements/button.html
--rw-rw-rw-   0        0        0     1556 2024-05-03 01:14:47.000000 django_allauth_themes-0.0.3/allauth_themes/bs5/allauth/elements/field.html
--rw-rw-rw-   0        0        0       22 2024-05-03 01:14:47.000000 django_allauth_themes-0.0.3/allauth_themes/bs5/allauth/elements/fields.html
--rw-rw-rw-   0        0        0      169 2024-05-03 01:14:47.000000 django_allauth_themes-0.0.3/allauth_themes/bs5/allauth/elements/form.html
--rw-rw-rw-   0        0        0       71 2024-05-03 01:14:47.000000 django_allauth_themes-0.0.3/allauth_themes/bs5/allauth/elements/h1.html
--rw-rw-rw-   0        0        0       71 2024-05-03 01:14:47.000000 django_allauth_themes-0.0.3/allauth_themes/bs5/allauth/elements/h2.html
--rw-rw-rw-   0        0        0        5 2024-05-03 01:14:47.000000 django_allauth_themes-0.0.3/allauth_themes/bs5/allauth/elements/hr.html
--rw-rw-rw-   0        0        0       84 2024-05-03 01:14:47.000000 django_allauth_themes-0.0.3/allauth_themes/bs5/allauth/elements/img.html
--rw-rw-rw-   0        0        0      293 2024-05-03 01:14:47.000000 django_allauth_themes-0.0.3/allauth_themes/bs5/allauth/elements/panel.html
--rw-rw-rw-   0        0        0       88 2024-05-03 01:14:47.000000 django_allauth_themes-0.0.3/allauth_themes/bs5/allauth/elements/provider.html
--rw-rw-rw-   0        0        0       71 2024-05-03 01:14:47.000000 django_allauth_themes-0.0.3/allauth_themes/bs5/allauth/elements/provider_list.html
--rw-rw-rw-   0        0        0       69 2024-05-03 01:14:47.000000 django_allauth_themes-0.0.3/allauth_themes/bs5/allauth/elements/table.html
-drwxrwxrwx   0        0        0        0 2024-05-05 13:31:06.277332 django_allauth_themes-0.0.3/allauth_themes/bs5/allauth/layouts/
--rw-rw-rw-   0        0        0     1740 2024-05-03 01:14:47.000000 django_allauth_themes-0.0.3/allauth_themes/bs5/allauth/layouts/base.html
--rw-rw-rw-   0        0        0       76 2024-05-03 01:14:47.000000 django_allauth_themes-0.0.3/allauth_themes/bs5/allauth/layouts/entrance.html
--rw-rw-rw-   0        0        0       76 2024-05-03 01:14:47.000000 django_allauth_themes-0.0.3/allauth_themes/bs5/allauth/layouts/manage.html
--rw-rw-rw-   0        0        0      232 2024-05-04 23:42:47.000000 django_allauth_themes-0.0.3/allauth_themes/bs5/index.html
--rw-rw-rw-   0        0        0      188 2024-05-04 23:42:47.000000 django_allauth_themes-0.0.3/allauth_themes/bs5/profile.html
-drwxrwxrwx   0        0        0        0 2024-05-05 13:31:06.282333 django_allauth_themes-0.0.3/allauth_themes/new/
--rw-rw-rw-   0        0        0      385 2024-05-04 23:42:47.000000 django_allauth_themes-0.0.3/allauth_themes/new/429.html
-drwxrwxrwx   0        0        0        0 2024-05-05 13:31:06.200957 django_allauth_themes-0.0.3/allauth_themes/new/allauth/
-drwxrwxrwx   0        0        0        0 2024-05-05 13:31:06.303332 django_allauth_themes-0.0.3/allauth_themes/new/allauth/elements/
--rw-rw-rw-   0        0        0       85 2024-05-03 01:14:47.000000 django_allauth_themes-0.0.3/allauth_themes/new/allauth/elements/alert.html
--rw-rw-rw-   0        0        0       71 2024-05-03 01:14:47.000000 django_allauth_themes-0.0.3/allauth_themes/new/allauth/elements/badge.html
--rw-rw-rw-   0        0        0      479 2024-05-03 01:14:47.000000 django_allauth_themes-0.0.3/allauth_themes/new/allauth/elements/button.html
--rw-rw-rw-   0        0        0     1556 2024-05-03 01:14:47.000000 django_allauth_themes-0.0.3/allauth_themes/new/allauth/elements/field.html
--rw-rw-rw-   0        0        0       22 2024-05-03 01:14:47.000000 django_allauth_themes-0.0.3/allauth_themes/new/allauth/elements/fields.html
--rw-rw-rw-   0        0        0      169 2024-05-03 01:14:47.000000 django_allauth_themes-0.0.3/allauth_themes/new/allauth/elements/form.html
--rw-rw-rw-   0        0        0       71 2024-05-03 01:14:47.000000 django_allauth_themes-0.0.3/allauth_themes/new/allauth/elements/h1.html
--rw-rw-rw-   0        0        0       71 2024-05-03 01:14:47.000000 django_allauth_themes-0.0.3/allauth_themes/new/allauth/elements/h2.html
--rw-rw-rw-   0        0        0        5 2024-05-03 01:14:47.000000 django_allauth_themes-0.0.3/allauth_themes/new/allauth/elements/hr.html
--rw-rw-rw-   0        0        0       84 2024-05-03 01:14:47.000000 django_allauth_themes-0.0.3/allauth_themes/new/allauth/elements/img.html
--rw-rw-rw-   0        0        0      293 2024-05-03 01:14:47.000000 django_allauth_themes-0.0.3/allauth_themes/new/allauth/elements/panel.html
--rw-rw-rw-   0        0        0       88 2024-05-03 01:14:47.000000 django_allauth_themes-0.0.3/allauth_themes/new/allauth/elements/provider.html
--rw-rw-rw-   0        0        0       71 2024-05-03 01:14:47.000000 django_allauth_themes-0.0.3/allauth_themes/new/allauth/elements/provider_list.html
--rw-rw-rw-   0        0        0       69 2024-05-03 01:14:47.000000 django_allauth_themes-0.0.3/allauth_themes/new/allauth/elements/table.html
-drwxrwxrwx   0        0        0        0 2024-05-05 13:31:06.308333 django_allauth_themes-0.0.3/allauth_themes/new/allauth/layouts/
--rw-rw-rw-   0        0        0     1740 2024-05-03 01:14:47.000000 django_allauth_themes-0.0.3/allauth_themes/new/allauth/layouts/base.html
--rw-rw-rw-   0        0        0       76 2024-05-03 01:14:47.000000 django_allauth_themes-0.0.3/allauth_themes/new/allauth/layouts/entrance.html
--rw-rw-rw-   0        0        0       76 2024-05-03 01:14:47.000000 django_allauth_themes-0.0.3/allauth_themes/new/allauth/layouts/manage.html
--rw-rw-rw-   0        0        0      232 2024-05-04 23:42:47.000000 django_allauth_themes-0.0.3/allauth_themes/new/index.html
--rw-rw-rw-   0        0        0      188 2024-05-04 23:42:47.000000 django_allauth_themes-0.0.3/allauth_themes/new/profile.html
-drwxrwxrwx   0        0        0        0 2024-05-05 13:31:06.317332 django_allauth_themes-0.0.3/django_allauth_themes.egg-info/
--rw-rw-rw-   0        0        0     2467 2024-05-05 13:31:06.000000 django_allauth_themes-0.0.3/django_allauth_themes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3422 2024-05-05 13:31:06.000000 django_allauth_themes-0.0.3/django_allauth_themes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 13:31:06.000000 django_allauth_themes-0.0.3/django_allauth_themes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-05 13:31:06.000000 django_allauth_themes-0.0.3/django_allauth_themes.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-05 13:31:06.000000 django_allauth_themes-0.0.3/django_allauth_themes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      608 2024-05-05 13:29:36.000000 django_allauth_themes-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-05 13:31:06.320333 django_allauth_themes-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-05 19:08:39.025983 django_allauth_themes-0.0.4/
+-rw-rw-rw-   0        0        0     1064 2024-05-03 03:15:33.000000 django_allauth_themes-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       40 2024-05-05 13:23:31.000000 django_allauth_themes-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2467 2024-05-05 19:08:39.024983 django_allauth_themes-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      852 2024-05-03 03:22:26.000000 django_allauth_themes-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 19:08:38.965984 django_allauth_themes-0.0.4/allauth_themes/
+drwxrwxrwx   0        0        0        0 2024-05-05 19:08:38.978985 django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/
+-rw-rw-rw-   0        0        0        0 2024-05-05 17:31:19.000000 django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/__init__.py
+-rw-rw-rw-   0        0        0      180 2024-05-05 17:47:55.000000 django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/apps.py
+drwxrwxrwx   0        0        0        0 2024-05-05 19:08:38.983986 django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/
+-rw-rw-rw-   0        0        0      293 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/429.html
+drwxrwxrwx   0        0        0        0 2024-05-05 19:08:38.986984 django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/account/
+-rw-rw-rw-   0        0        0      110 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/account/base_manage_email.html
+-rw-rw-rw-   0        0        0      113 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/account/base_manage_password.html
+drwxrwxrwx   0        0        0        0 2024-05-05 19:08:38.967987 django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/allauth/
+drwxrwxrwx   0        0        0        0 2024-05-05 19:08:39.007987 django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/allauth/elements/
+-rw-rw-rw-   0        0        0      123 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/allauth/elements/alert.html
+-rw-rw-rw-   0        0        0      348 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/allauth/elements/badge.html
+-rw-rw-rw-   0        0        0     1615 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/allauth/elements/button.html
+-rw-rw-rw-   0        0        0      129 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/allauth/elements/button__entrance.html
+-rw-rw-rw-   0        0        0     3001 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/allauth/elements/field.html
+-rw-rw-rw-   0        0        0      603 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/allauth/elements/fields.html
+-rw-rw-rw-   0        0        0      673 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/allauth/elements/form.html
+-rw-rw-rw-   0        0        0       80 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/allauth/elements/form__entrance.html
+-rw-rw-rw-   0        0        0       84 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/allauth/elements/h1.html
+-rw-rw-rw-   0        0        0       92 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/allauth/elements/h1__entrance.html
+-rw-rw-rw-   0        0        0       92 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/allauth/elements/h2__entrance.html
+-rw-rw-rw-   0        0        0      152 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/allauth/elements/img.html
+-rw-rw-rw-   0        0        0      385 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/allauth/elements/panel.html
+-rw-rw-rw-   0        0        0      122 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/allauth/elements/provider.html
+-rw-rw-rw-   0        0        0       92 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/allauth/elements/provider_list.html
+-rw-rw-rw-   0        0        0       97 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/allauth/elements/table.html
+drwxrwxrwx   0        0        0        0 2024-05-05 19:08:39.011984 django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/allauth/layouts/
+-rw-rw-rw-   0        0        0     4814 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/allauth/layouts/base.html
+-rw-rw-rw-   0        0        0      812 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/allauth/layouts/entrance.html
+-rw-rw-rw-   0        0        0     2444 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/allauth/layouts/manage.html
+-rw-rw-rw-   0        0        0      232 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/index.html
+drwxrwxrwx   0        0        0        0 2024-05-05 19:08:39.012989 django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/mfa/
+-rw-rw-rw-   0        0        0      108 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/mfa/base_manage.html
+-rw-rw-rw-   0        0        0      188 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/profile.html
+drwxrwxrwx   0        0        0        0 2024-05-05 19:08:39.013986 django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/socialaccount/
+-rw-rw-rw-   0        0        0      118 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/socialaccount/base_manage.html
+drwxrwxrwx   0        0        0        0 2024-05-05 19:08:39.015984 django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/usersessions/
+-rw-rw-rw-   0        0        0      117 2024-05-04 17:45:49.000000 django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/usersessions/base_manage.html
+drwxrwxrwx   0        0        0        0 2024-05-05 19:08:39.023985 django_allauth_themes-0.0.4/django_allauth_themes.egg-info/
+-rw-rw-rw-   0        0        0     2467 2024-05-05 19:08:38.000000 django_allauth_themes-0.0.4/django_allauth_themes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2268 2024-05-05 19:08:38.000000 django_allauth_themes-0.0.4/django_allauth_themes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 19:08:38.000000 django_allauth_themes-0.0.4/django_allauth_themes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-05 19:08:38.000000 django_allauth_themes-0.0.4/django_allauth_themes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-05 19:08:38.000000 django_allauth_themes-0.0.4/django_allauth_themes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      608 2024-05-05 19:08:10.000000 django_allauth_themes-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-05 19:08:39.025983 django_allauth_themes-0.0.4/setup.cfg
```

### Comparing `django_allauth_themes-0.0.3/LICENSE` & `django_allauth_themes-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_allauth_themes-0.0.3/PKG-INFO` & `django_allauth_themes-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-allauth-themes
-Version: 0.0.3
+Version: 0.0.4
 Summary: Themes for Django-Allauth
 Author-email: harrelchris <author@example.com>
 Maintainer-email: harrelchris <maintainer@example.com>
 License: Copyright 2024 StackMuse
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `django_allauth_themes-0.0.3/README.md` & `django_allauth_themes-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `django_allauth_themes-0.0.3/allauth_themes/allauth/allauth/elements/button.html` & `django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/allauth/elements/button.html`

 * *Files identical despite different names*

### Comparing `django_allauth_themes-0.0.3/allauth_themes/allauth/allauth/elements/field.html` & `django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/allauth/elements/field.html`

 * *Files identical despite different names*

### Comparing `django_allauth_themes-0.0.3/allauth_themes/allauth/allauth/elements/fields.html` & `django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/allauth/elements/fields.html`

 * *Files identical despite different names*

### Comparing `django_allauth_themes-0.0.3/allauth_themes/allauth/allauth/elements/form.html` & `django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/allauth/elements/form.html`

 * *Files identical despite different names*

### Comparing `django_allauth_themes-0.0.3/allauth_themes/allauth/allauth/layouts/base.html` & `django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/allauth/layouts/base.html`

 * *Files identical despite different names*

### Comparing `django_allauth_themes-0.0.3/allauth_themes/allauth/allauth/layouts/entrance.html` & `django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/allauth/layouts/entrance.html`

 * *Files identical despite different names*

### Comparing `django_allauth_themes-0.0.3/allauth_themes/allauth/allauth/layouts/manage.html` & `django_allauth_themes-0.0.4/allauth_themes/allauth_bootstrap/templates/allauth/layouts/manage.html`

 * *Files identical despite different names*

### Comparing `django_allauth_themes-0.0.3/django_allauth_themes.egg-info/PKG-INFO` & `django_allauth_themes-0.0.4/django_allauth_themes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-allauth-themes
-Version: 0.0.3
+Version: 0.0.4
 Summary: Themes for Django-Allauth
 Author-email: harrelchris <author@example.com>
 Maintainer-email: harrelchris <maintainer@example.com>
 License: Copyright 2024 StackMuse
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `django_allauth_themes-0.0.3/pyproject.toml` & `django_allauth_themes-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 69.5"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django-allauth-themes"
-version = "0.0.3"
+version = "0.0.4"
 description = "Themes for Django-Allauth"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 authors = [
   {name = "harrelchris", email = "author@example.com" }
 ]
```

