# Comparing `tmp/kiwitcms-github-marketplace-2.5.0.tar.gz` & `tmp/kiwitcms-github-marketplace-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiwitcms-github-marketplace-2.5.0.tar", last modified: Fri May  3 19:17:32 2024, max compression
+gzip compressed data, was "kiwitcms-github-marketplace-2.5.1.tar", last modified: Mon May  6 17:01:04 2024, max compression
```

## Comparing `kiwitcms-github-marketplace-2.5.0.tar` & `kiwitcms-github-marketplace-2.5.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-03 19:17:32.622196 kiwitcms-github-marketplace-2.5.0/
--rw-rw-r--   0 senko     (1001) senko     (1001)    35149 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.5.0/LICENSE
--rw-rw-r--   0 senko     (1001) senko     (1001)      208 2022-02-23 19:15:12.000000 kiwitcms-github-marketplace-2.5.0/MANIFEST.in
--rw-r--r--   0 senko     (1001) senko     (1001)    12795 2024-05-03 19:17:32.622196 kiwitcms-github-marketplace-2.5.0/PKG-INFO
--rw-r--r--   0 senko     (1001) senko     (1001)    11945 2024-05-03 19:17:08.000000 kiwitcms-github-marketplace-2.5.0/README.rst
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-03 19:17:32.620196 kiwitcms-github-marketplace-2.5.0/kiwitcms_github_marketplace.egg-info/
--rw-r--r--   0 senko     (1001) senko     (1001)    12795 2024-05-03 19:17:32.000000 kiwitcms-github-marketplace-2.5.0/kiwitcms_github_marketplace.egg-info/PKG-INFO
--rw-r--r--   0 senko     (1001) senko     (1001)     2055 2024-05-03 19:17:32.000000 kiwitcms-github-marketplace-2.5.0/kiwitcms_github_marketplace.egg-info/SOURCES.txt
--rw-r--r--   0 senko     (1001) senko     (1001)        1 2024-05-03 19:17:32.000000 kiwitcms-github-marketplace-2.5.0/kiwitcms_github_marketplace.egg-info/dependency_links.txt
--rw-r--r--   0 senko     (1001) senko     (1001)       64 2024-05-03 19:17:32.000000 kiwitcms-github-marketplace-2.5.0/kiwitcms_github_marketplace.egg-info/entry_points.txt
--rw-r--r--   0 senko     (1001) senko     (1001)        1 2024-05-03 19:17:32.000000 kiwitcms-github-marketplace-2.5.0/kiwitcms_github_marketplace.egg-info/not-zip-safe
--rw-r--r--   0 senko     (1001) senko     (1001)       68 2024-05-03 19:17:32.000000 kiwitcms-github-marketplace-2.5.0/kiwitcms_github_marketplace.egg-info/requires.txt
--rw-r--r--   0 senko     (1001) senko     (1001)       42 2024-05-03 19:17:32.000000 kiwitcms-github-marketplace-2.5.0/kiwitcms_github_marketplace.egg-info/top_level.txt
--rw-r--r--   0 senko     (1001) senko     (1001)      133 2024-05-02 21:53:41.000000 kiwitcms-github-marketplace-2.5.0/requirements.txt
--rw-rw-r--   0 senko     (1001) senko     (1001)      129 2024-05-03 19:17:32.622196 kiwitcms-github-marketplace-2.5.0/setup.cfg
--rw-r--r--   0 senko     (1001) senko     (1001)     1783 2024-05-03 19:17:08.000000 kiwitcms-github-marketplace-2.5.0/setup.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-03 19:17:32.621196 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/
--rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/__init__.py
--rw-r--r--   0 senko     (1001) senko     (1001)     6031 2023-04-14 16:28:27.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/admin.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      321 2022-02-20 13:20:22.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/apps.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      553 2022-02-20 13:20:22.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/checks.py
--rw-rw-r--   0 senko     (1001) senko     (1001)     2613 2022-02-16 15:05:52.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/docker.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      879 2022-02-21 15:47:58.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/mailchimp.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      374 2022-02-09 11:11:58.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/menu.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-03 19:17:32.621196 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/migrations/
--rw-r--r--   0 senko     (1001) senko     (1001)     1532 2024-01-05 12:16:28.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/migrations/0001_initial.py
--rw-r--r--   0 senko     (1001) senko     (1001)      965 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/migrations/0002_update_fields.py
--rw-r--r--   0 senko     (1001) senko     (1001)      415 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/migrations/0003_sender_email_field.py
--rw-r--r--   0 senko     (1001) senko     (1001)      391 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/migrations/0004_models_jsonfield.py
--rw-r--r--   0 senko     (1001) senko     (1001)      613 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/migrations/0005_add_support_and_tenant_flags.py
--rw-r--r--   0 senko     (1001) senko     (1001)     1039 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/migrations/0006_add_subscription_field.py
--rw-r--r--   0 senko     (1001) senko     (1001)      694 2023-04-14 16:28:27.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/migrations/0007_manualpurchase.py
--rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/migrations/__init__.py
--rw-r--r--   0 senko     (1001) senko     (1001)     1712 2023-04-14 16:28:27.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/models.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-03 19:17:32.621196 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/quay/
--rw-rw-r--   0 senko     (1001) senko     (1001)       57 2022-02-09 14:16:51.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/quay/__init__.py
--rw-rw-r--   0 senko     (1001) senko     (1001)     2353 2022-02-09 21:44:26.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/quay/quay_api_client.py
--rw-r--r--   0 senko     (1001) senko     (1001)     4708 2024-04-17 13:31:58.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/quay/quay_session.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-03 19:17:32.618196 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/static/
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-03 19:17:32.618196 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/static/tcms_github_marketplace/
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-03 19:17:32.621196 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/static/tcms_github_marketplace/js/
--rw-rw-r--   0 senko     (1001) senko     (1001)      924 2022-02-16 15:05:52.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/static/tcms_github_marketplace/js/subscription.js
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-03 19:17:32.618196 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/templates/
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-03 19:17:32.622196 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/templates/email/
--rw-r--r--   0 senko     (1001) senko     (1001)     1450 2023-04-14 16:28:27.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/templates/email/manual_subscription_notification.txt
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-03 19:17:32.622196 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/templates/tcms_github_marketplace/
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-03 19:17:32.622196 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/templates/tcms_github_marketplace/email/
--rw-rw-r--   0 senko     (1001) senko     (1001)      270 2022-08-14 14:51:18.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/templates/tcms_github_marketplace/email/exit_poll.txt
--rw-rw-r--   0 senko     (1001) senko     (1001)    11048 2022-08-04 08:25:18.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/templates/tcms_github_marketplace/subscription.html
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-03 19:17:32.622196 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/templates/tcms_tenants/
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-03 19:17:32.622196 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/templates/tcms_tenants/include/
--rw-r--r--   0 senko     (1001) senko     (1001)     1030 2024-05-02 21:53:41.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/templates/tcms_tenants/include/tenant_extra_emails.html
--rw-r--r--   0 senko     (1001) senko     (1001)      163 2024-05-02 21:53:41.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/templates/tcms_tenants/override_edit.html
--rw-r--r--   0 senko     (1001) senko     (1001)     2629 2024-05-02 21:53:41.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/templates/tcms_tenants/override_new.html
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-03 19:17:32.622196 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/templatetags/
--rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/templatetags/__init__.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      373 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/templatetags/github_marketplace.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      804 2022-02-09 11:11:58.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/urls.py
--rw-r--r--   0 senko     (1001) senko     (1001)     5632 2023-04-28 11:18:45.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/utils.py
--rw-r--r--   0 senko     (1001) senko     (1001)    28284 2024-05-03 19:17:08.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/views.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-03 19:17:32.622196 kiwitcms-github-marketplace-2.5.0/tcms_settings_dir/
--rw-rw-r--   0 senko     (1001) senko     (1001)       65 2022-02-09 11:11:58.000000 kiwitcms-github-marketplace-2.5.0/tcms_settings_dir/__init__.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-06 17:01:04.302157 kiwitcms-github-marketplace-2.5.1/
+-rw-rw-r--   0 senko     (1001) senko     (1001)    35149 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.5.1/LICENSE
+-rw-rw-r--   0 senko     (1001) senko     (1001)      208 2022-02-23 19:15:12.000000 kiwitcms-github-marketplace-2.5.1/MANIFEST.in
+-rw-r--r--   0 senko     (1001) senko     (1001)    12979 2024-05-06 17:01:04.302157 kiwitcms-github-marketplace-2.5.1/PKG-INFO
+-rw-r--r--   0 senko     (1001) senko     (1001)    12129 2024-05-06 17:00:42.000000 kiwitcms-github-marketplace-2.5.1/README.rst
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-06 17:01:04.301158 kiwitcms-github-marketplace-2.5.1/kiwitcms_github_marketplace.egg-info/
+-rw-r--r--   0 senko     (1001) senko     (1001)    12979 2024-05-06 17:01:04.000000 kiwitcms-github-marketplace-2.5.1/kiwitcms_github_marketplace.egg-info/PKG-INFO
+-rw-r--r--   0 senko     (1001) senko     (1001)     2055 2024-05-06 17:01:04.000000 kiwitcms-github-marketplace-2.5.1/kiwitcms_github_marketplace.egg-info/SOURCES.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)        1 2024-05-06 17:01:04.000000 kiwitcms-github-marketplace-2.5.1/kiwitcms_github_marketplace.egg-info/dependency_links.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)       64 2024-05-06 17:01:04.000000 kiwitcms-github-marketplace-2.5.1/kiwitcms_github_marketplace.egg-info/entry_points.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)        1 2024-05-06 17:01:04.000000 kiwitcms-github-marketplace-2.5.1/kiwitcms_github_marketplace.egg-info/not-zip-safe
+-rw-r--r--   0 senko     (1001) senko     (1001)       68 2024-05-06 17:01:04.000000 kiwitcms-github-marketplace-2.5.1/kiwitcms_github_marketplace.egg-info/requires.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)       42 2024-05-06 17:01:04.000000 kiwitcms-github-marketplace-2.5.1/kiwitcms_github_marketplace.egg-info/top_level.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)      133 2024-05-06 12:49:10.000000 kiwitcms-github-marketplace-2.5.1/requirements.txt
+-rw-rw-r--   0 senko     (1001) senko     (1001)      129 2024-05-06 17:01:04.302157 kiwitcms-github-marketplace-2.5.1/setup.cfg
+-rw-r--r--   0 senko     (1001) senko     (1001)     1783 2024-05-06 17:00:42.000000 kiwitcms-github-marketplace-2.5.1/setup.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-06 17:01:04.301158 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/
+-rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/__init__.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     6031 2023-04-14 16:28:27.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/admin.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      321 2022-02-20 13:20:22.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/apps.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      553 2022-02-20 13:20:22.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/checks.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)     2613 2022-02-16 15:05:52.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/docker.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      879 2022-02-21 15:47:58.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/mailchimp.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      374 2022-02-09 11:11:58.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/menu.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-06 17:01:04.302157 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/migrations/
+-rw-r--r--   0 senko     (1001) senko     (1001)     1532 2024-01-05 12:16:28.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/migrations/0001_initial.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      965 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/migrations/0002_update_fields.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      415 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/migrations/0003_sender_email_field.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      391 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/migrations/0004_models_jsonfield.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      613 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/migrations/0005_add_support_and_tenant_flags.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     1039 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/migrations/0006_add_subscription_field.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      694 2023-04-14 16:28:27.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/migrations/0007_manualpurchase.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/migrations/__init__.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     1712 2023-04-14 16:28:27.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/models.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-06 17:01:04.302157 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/quay/
+-rw-rw-r--   0 senko     (1001) senko     (1001)       57 2022-02-09 14:16:51.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/quay/__init__.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)     2353 2022-02-09 21:44:26.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/quay/quay_api_client.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     4708 2024-04-17 13:31:58.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/quay/quay_session.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-06 17:01:04.300158 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/static/
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-06 17:01:04.300158 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/static/tcms_github_marketplace/
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-06 17:01:04.302157 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/static/tcms_github_marketplace/js/
+-rw-rw-r--   0 senko     (1001) senko     (1001)      924 2022-02-16 15:05:52.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/static/tcms_github_marketplace/js/subscription.js
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-06 17:01:04.300158 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/templates/
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-06 17:01:04.302157 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/templates/email/
+-rw-r--r--   0 senko     (1001) senko     (1001)     1450 2023-04-14 16:28:27.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/templates/email/manual_subscription_notification.txt
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-06 17:01:04.302157 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/templates/tcms_github_marketplace/
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-06 17:01:04.302157 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/templates/tcms_github_marketplace/email/
+-rw-rw-r--   0 senko     (1001) senko     (1001)      270 2022-08-14 14:51:18.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/templates/tcms_github_marketplace/email/exit_poll.txt
+-rw-rw-r--   0 senko     (1001) senko     (1001)    11048 2022-08-04 08:25:18.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/templates/tcms_github_marketplace/subscription.html
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-06 17:01:04.302157 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/templates/tcms_tenants/
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-06 17:01:04.302157 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/templates/tcms_tenants/include/
+-rw-r--r--   0 senko     (1001) senko     (1001)     1030 2024-05-02 21:53:41.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/templates/tcms_tenants/include/tenant_extra_emails.html
+-rw-r--r--   0 senko     (1001) senko     (1001)      163 2024-05-02 21:53:41.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/templates/tcms_tenants/override_edit.html
+-rw-r--r--   0 senko     (1001) senko     (1001)     2629 2024-05-02 21:53:41.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/templates/tcms_tenants/override_new.html
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-06 17:01:04.302157 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/templatetags/
+-rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/templatetags/__init__.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      373 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/templatetags/github_marketplace.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      804 2022-02-09 11:11:58.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/urls.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     5893 2024-05-06 17:00:42.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/utils.py
+-rw-r--r--   0 senko     (1001) senko     (1001)    28284 2024-05-03 19:17:08.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/views.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-06 17:01:04.302157 kiwitcms-github-marketplace-2.5.1/tcms_settings_dir/
+-rw-rw-r--   0 senko     (1001) senko     (1001)       65 2022-02-09 11:11:58.000000 kiwitcms-github-marketplace-2.5.1/tcms_settings_dir/__init__.py
```

### Comparing `kiwitcms-github-marketplace-2.5.0/LICENSE` & `kiwitcms-github-marketplace-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.5.0/PKG-INFO` & `kiwitcms-github-marketplace-2.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwitcms-github-marketplace
-Version: 2.5.0
+Version: 2.5.1
 Summary: GitHub Marketplace integration for Kiwi TCMS
 Home-page: https://github.com/kiwitcms/github-marketplace/
 Author: Kiwi TCMS
 Author-email: info@kiwitcms.org
 License: GPLv3+
 Classifier: Framework :: Django
 Classifier: Development Status :: 5 - Production/Stable
@@ -80,14 +80,22 @@
   to private docker repositories. Format is
   ``Docker repositories: quay.io/kiwitcms/<repo1>, quay.io/kiwitcms/<repo2>``
 
 
 Changelog
 ---------
 
+v2.5.1 (06 May 2024)
+~~~~~~~~~~~~~~~~~~~~
+
+- Adjust name of settings for ``revoke_oauth_token()`` to match production
+  environment
+- Adjust arguments for newer versions of PyGithub
+
+
 v2.5.0 (03 May 2024)
 ~~~~~~~~~~~~~~~~~~~~
 
 - Allow edits to ``Tenant.extra_emails`` field by overriding the HTML templates
   so we can expose this inside the UI. This new field is shown when creating
   a new tenant or editing an existing one
 - FastSpring webhooks handler will also try matching the
```

### Comparing `kiwitcms-github-marketplace-2.5.0/README.rst` & `kiwitcms-github-marketplace-2.5.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -59,14 +59,22 @@
   to private docker repositories. Format is
   ``Docker repositories: quay.io/kiwitcms/<repo1>, quay.io/kiwitcms/<repo2>``
 
 
 Changelog
 ---------
 
+v2.5.1 (06 May 2024)
+~~~~~~~~~~~~~~~~~~~~
+
+- Adjust name of settings for ``revoke_oauth_token()`` to match production
+  environment
+- Adjust arguments for newer versions of PyGithub
+
+
 v2.5.0 (03 May 2024)
 ~~~~~~~~~~~~~~~~~~~~
 
 - Allow edits to ``Tenant.extra_emails`` field by overriding the HTML templates
   so we can expose this inside the UI. This new field is shown when creating
   a new tenant or editing an existing one
 - FastSpring webhooks handler will also try matching the
```

### Comparing `kiwitcms-github-marketplace-2.5.0/kiwitcms_github_marketplace.egg-info/PKG-INFO` & `kiwitcms-github-marketplace-2.5.1/kiwitcms_github_marketplace.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwitcms-github-marketplace
-Version: 2.5.0
+Version: 2.5.1
 Summary: GitHub Marketplace integration for Kiwi TCMS
 Home-page: https://github.com/kiwitcms/github-marketplace/
 Author: Kiwi TCMS
 Author-email: info@kiwitcms.org
 License: GPLv3+
 Classifier: Framework :: Django
 Classifier: Development Status :: 5 - Production/Stable
@@ -80,14 +80,22 @@
   to private docker repositories. Format is
   ``Docker repositories: quay.io/kiwitcms/<repo1>, quay.io/kiwitcms/<repo2>``
 
 
 Changelog
 ---------
 
+v2.5.1 (06 May 2024)
+~~~~~~~~~~~~~~~~~~~~
+
+- Adjust name of settings for ``revoke_oauth_token()`` to match production
+  environment
+- Adjust arguments for newer versions of PyGithub
+
+
 v2.5.0 (03 May 2024)
 ~~~~~~~~~~~~~~~~~~~~
 
 - Allow edits to ``Tenant.extra_emails`` field by overriding the HTML templates
   so we can expose this inside the UI. This new field is shown when creating
   a new tenant or editing an existing one
 - FastSpring webhooks handler will also try matching the
```

### Comparing `kiwitcms-github-marketplace-2.5.0/kiwitcms_github_marketplace.egg-info/SOURCES.txt` & `kiwitcms-github-marketplace-2.5.1/kiwitcms_github_marketplace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.5.0/setup.py` & `kiwitcms-github-marketplace-2.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
                 continue
             requires.append(line.strip())
         return requires
 
 
 setup(
     name="kiwitcms-github-marketplace",
-    version="2.5.0",
+    version="2.5.1",
     description="GitHub Marketplace integration for Kiwi TCMS",
     long_description=get_long_description(),
     author="Kiwi TCMS",
     author_email="info@kiwitcms.org",
     url="https://github.com/kiwitcms/github-marketplace/",
     license="GPLv3+",
     install_requires=get_install_requires("requirements.txt"),
```

### Comparing `kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/admin.py` & `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/admin.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/checks.py` & `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/checks.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/docker.py` & `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/docker.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/mailchimp.py` & `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/mailchimp.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/migrations/0001_initial.py` & `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/migrations/0002_update_fields.py` & `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/migrations/0002_update_fields.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/migrations/0005_add_support_and_tenant_flags.py` & `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/migrations/0005_add_support_and_tenant_flags.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/migrations/0006_add_subscription_field.py` & `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/migrations/0006_add_subscription_field.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/migrations/0007_manualpurchase.py` & `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/migrations/0007_manualpurchase.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/models.py` & `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/models.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/quay/quay_api_client.py` & `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/quay/quay_api_client.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/quay/quay_session.py` & `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/quay/quay_session.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/static/tcms_github_marketplace/js/subscription.js` & `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/static/tcms_github_marketplace/js/subscription.js`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/templates/email/manual_subscription_notification.txt` & `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/templates/email/manual_subscription_notification.txt`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/templates/tcms_github_marketplace/subscription.html` & `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/templates/tcms_github_marketplace/subscription.html`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/templates/tcms_tenants/include/tenant_extra_emails.html` & `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/templates/tcms_tenants/include/tenant_extra_emails.html`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/templates/tcms_tenants/override_new.html` & `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/templates/tcms_tenants/override_new.html`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/urls.py` & `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/urls.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/utils.py` & `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-# Copyright (c) 2019-2023 Alexander Todorov <atodorov@MrSenko.com>
+# Copyright (c) 2019-2024 Alexander Todorov <atodorov@MrSenko.com>
 
 # Licensed under the GPL 3.0: https://www.gnu.org/licenses/gpl-3.0.txt
 
 import hmac
 import hashlib
 from base64 import b64encode
 from datetime import timedelta
 
 import github
+from github.GithubRetry import GithubRetry
 from github.Requester import Requester
 from social_django.models import UserSocialAuth
 
 from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.http import HttpResponse, HttpResponseForbidden
 from django.utils.translation import gettext_lazy as _
@@ -53,28 +54,32 @@
     # note: Requester is the internal transport used by PyGithub
     # b/c it is missing this functionality built-in
     #
     # note2: GitHub documentation says that for this method we must
     # use Basic Authentication, where the username is the OAuth application
     # client_id and the password is its client_secret.
     gh_api = Requester(
-        settings.SOCIAL_AUTH_GITHUB_KEY,
-        settings.SOCIAL_AUTH_GITHUB_SECRET,
-        None,
-        None,
+        github.Auth.Login(
+            settings.SOCIAL_AUTH_GITHUB_APP_KEY,
+            settings.SOCIAL_AUTH_GITHUB_APP_SECRET,
+        ),
         github.Consts.DEFAULT_BASE_URL,
         github.Consts.DEFAULT_TIMEOUT,
         "KiwiTCMS/Python",
         github.Consts.DEFAULT_PER_PAGE,
         True,
+        GithubRetry(),
         None,
-        None,
+        github.Consts.DEFAULT_SECONDS_BETWEEN_REQUESTS,
+        github.Consts.DEFAULT_SECONDS_BETWEEN_WRITES,
     )
 
-    revoke_url = f"/applications/{settings.SOCIAL_AUTH_GITHUB_KEY}/tokens/{token}"
+    # note3: vvv this API method seems to have been removed already
+
+    revoke_url = f"/applications/{settings.SOCIAL_AUTH_GITHUB_APP_KEY}/tokens/{token}"
     _headers, _data = gh_api.requestJsonAndCheck("DELETE", revoke_url)
 
 
 def cancel_plan(purchase):
     """
     Cancells the current plan from Marketplace:
     https://developer.github.com/marketplace/integrating-with-the-github-marketplace-api/cancelling-plans/
```

### Comparing `kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/views.py` & `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/views.py`

 * *Files identical despite different names*

