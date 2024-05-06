# Comparing `tmp/iommi-7.0.0.tar.gz` & `tmp/iommi-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iommi-7.0.0.tar", last modified: Mon Apr 15 10:45:20 2024, max compression
+gzip compressed data, was "iommi-7.1.0.tar", last modified: Mon May  6 14:09:23 2024, max compression
```

## Comparing `iommi-7.0.0.tar` & `iommi-7.1.0.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.745983 iommi-7.0.0/
--rw-r--r--   0 boxed      (501) staff       (20)     1102 2024-02-18 13:30:36.000000 iommi-7.0.0/AUTHORS.rst
--rw-r--r--   0 boxed      (501) staff       (20)      212 2021-01-28 10:44:48.000000 iommi-7.0.0/CONTRIBUTING.rst
--rw-r--r--   0 boxed      (501) staff       (20)    42689 2024-04-15 10:35:27.000000 iommi-7.0.0/HISTORY.rst
--rw-r--r--   0 boxed      (501) staff       (20)     1485 2021-01-28 10:44:48.000000 iommi-7.0.0/LICENSE
--rw-r--r--   0 boxed      (501) staff       (20)      332 2022-01-21 14:21:52.000000 iommi-7.0.0/MANIFEST.in
--rw-r--r--   0 boxed      (501) staff       (20)     3079 2024-04-15 10:45:20.745852 iommi-7.0.0/PKG-INFO
--rw-r--r--   0 boxed      (501) staff       (20)     2781 2023-04-05 18:05:05.000000 iommi-7.0.0/README.rst
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.724551 iommi-7.0.0/iommi/
--rw-r--r--   0 boxed      (501) staff       (20)     8196 2024-04-06 11:17:02.000000 iommi-7.0.0/iommi/.DS_Store
--rw-r--r--   0 boxed      (501) staff       (20)     3606 2024-04-15 10:38:38.000000 iommi-7.0.0/iommi/__init__.py
--rw-r--r--   0 boxed      (501) staff       (20)     6391 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/_db_compat.py
--rw-r--r--   0 boxed      (501) staff       (20)     6578 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/_web_compat.py
--rw-r--r--   0 boxed      (501) staff       (20)      532 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/_web_compat_flask.py
--rw-r--r--   0 boxed      (501) staff       (20)     5757 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/action.py
--rw-r--r--   0 boxed      (501) staff       (20)    21492 2024-04-15 07:14:49.000000 iommi-7.0.0/iommi/admin.py
--rw-r--r--   0 boxed      (501) staff       (20)     1892 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/apps.py
--rw-r--r--   0 boxed      (501) staff       (20)     1950 2023-02-13 19:03:15.000000 iommi-7.0.0/iommi/asset.py
--rw-r--r--   0 boxed      (501) staff       (20)     5010 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/attrs.py
--rw-r--r--   0 boxed      (501) staff       (20)     2591 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/base.py
--rw-r--r--   0 boxed      (501) staff       (20)     4902 2022-01-19 10:19:49.000000 iommi-7.0.0/iommi/datetime_parsing.py
--rw-r--r--   0 boxed      (501) staff       (20)    11898 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/debug.py
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.727993 iommi-7.0.0/iommi/declarative/
--rw-r--r--   0 boxed      (501) staff       (20)     6148 2023-12-11 09:30:40.000000 iommi-7.0.0/iommi/declarative/.DS_Store
--rw-r--r--   0 boxed      (501) staff       (20)     5461 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/declarative/__init__.py
--rw-r--r--   0 boxed      (501) staff       (20)      571 2023-02-13 19:03:15.000000 iommi-7.0.0/iommi/declarative/dispatch.py
--rw-r--r--   0 boxed      (501) staff       (20)     7994 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/declarative/namespace.py
--rw-r--r--   0 boxed      (501) staff       (20)     1938 2023-02-13 19:03:15.000000 iommi-7.0.0/iommi/declarative/util.py
--rw-r--r--   0 boxed      (501) staff       (20)     1501 2023-09-06 07:14:35.000000 iommi-7.0.0/iommi/declarative/with_meta.py
--rw-r--r--   0 boxed      (501) staff       (20)    12419 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/docs.py
--rw-r--r--   0 boxed      (501) staff       (20)    17950 2024-04-15 07:14:49.000000 iommi-7.0.0/iommi/edit_table.py
--rw-r--r--   0 boxed      (501) staff       (20)     3769 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/endpoint.py
--rw-r--r--   0 boxed      (501) staff       (20)     1477 2023-02-13 19:03:15.000000 iommi-7.0.0/iommi/error.py
--rw-r--r--   0 boxed      (501) staff       (20)     5018 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/evaluate.py
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.728917 iommi-7.0.0/iommi/experimental/
--rw-r--r--   0 boxed      (501) staff       (20)     6148 2023-12-11 09:30:40.000000 iommi-7.0.0/iommi/experimental/.DS_Store
--rw-r--r--   0 boxed      (501) staff       (20)        0 2022-01-19 10:19:49.000000 iommi-7.0.0/iommi/experimental/__init__.py
--rw-r--r--   0 boxed      (501) staff       (20)      133 2023-02-13 19:03:15.000000 iommi-7.0.0/iommi/experimental/edit_table.py
--rw-r--r--   0 boxed      (501) staff       (20)    71882 2024-04-15 10:35:20.000000 iommi-7.0.0/iommi/form.py
--rw-r--r--   0 boxed      (501) staff       (20)     8184 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/fragment.py
--rw-r--r--   0 boxed      (501) staff       (20)    10165 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/from_model.py
--rw-r--r--   0 boxed      (501) staff       (20)    19710 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/live_edit.py
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.729234 iommi-7.0.0/iommi/locale/
--rw-r--r--   0 boxed      (501) staff       (20)     6148 2024-01-05 19:32:48.000000 iommi-7.0.0/iommi/locale/.DS_Store
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.699282 iommi-7.0.0/iommi/locale/cs/
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.729828 iommi-7.0.0/iommi/locale/cs/LC_MESSAGES/
--rw-r--r--   0 boxed      (501) staff       (20)     4410 2023-12-13 09:01:15.000000 iommi-7.0.0/iommi/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 boxed      (501) staff       (20)     7115 2023-11-22 17:28:48.000000 iommi-7.0.0/iommi/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.730226 iommi-7.0.0/iommi/locale/de/
--rw-r--r--   0 boxed      (501) staff       (20)     6148 2022-01-02 19:23:31.000000 iommi-7.0.0/iommi/locale/de/.DS_Store
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.730827 iommi-7.0.0/iommi/locale/de/LC_MESSAGES/
--rw-r--r--   0 boxed      (501) staff       (20)     4442 2023-12-13 09:01:15.000000 iommi-7.0.0/iommi/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 boxed      (501) staff       (20)     7751 2023-11-22 17:28:48.000000 iommi-7.0.0/iommi/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.731134 iommi-7.0.0/iommi/locale/sv/
--rw-r--r--   0 boxed      (501) staff       (20)     6148 2022-01-02 19:23:31.000000 iommi-7.0.0/iommi/locale/sv/.DS_Store
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.731590 iommi-7.0.0/iommi/locale/sv/LC_MESSAGES/
--rw-r--r--   0 boxed      (501) staff       (20)     5588 2023-12-13 09:01:15.000000 iommi-7.0.0/iommi/locale/sv/LC_MESSAGES/django.mo
--rw-r--r--   0 boxed      (501) staff       (20)     7390 2023-11-22 17:28:48.000000 iommi-7.0.0/iommi/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.699837 iommi-7.0.0/iommi/locale/uk/
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.732145 iommi-7.0.0/iommi/locale/uk/LC_MESSAGES/
--rw-r--r--   0 boxed      (501) staff       (20)     5610 2023-12-13 09:01:15.000000 iommi-7.0.0/iommi/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0 boxed      (501) staff       (20)     8431 2023-11-22 17:28:48.000000 iommi-7.0.0/iommi/locale/uk/LC_MESSAGES/django.po
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.699998 iommi-7.0.0/iommi/locale/zh_Hans/
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.732768 iommi-7.0.0/iommi/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 boxed      (501) staff       (20)     3975 2023-12-13 09:01:15.000000 iommi-7.0.0/iommi/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 boxed      (501) staff       (20)     7182 2023-11-22 17:28:48.000000 iommi-7.0.0/iommi/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0 boxed      (501) staff       (20)    10204 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/member.py
--rw-r--r--   0 boxed      (501) staff       (20)    11141 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/menu.py
--rw-r--r--   0 boxed      (501) staff       (20)     3761 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/page.py
--rw-r--r--   0 boxed      (501) staff       (20)     8450 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/part.py
--rw-r--r--   0 boxed      (501) staff       (20)     4729 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/path.py
--rw-r--r--   0 boxed      (501) staff       (20)    10196 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/profiling.py
--rw-r--r--   0 boxed      (501) staff       (20)    36786 2024-04-15 07:51:09.000000 iommi-7.0.0/iommi/query.py
--rw-r--r--   0 boxed      (501) staff       (20)     8657 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/refinable.py
--rw-r--r--   0 boxed      (501) staff       (20)     2717 2023-02-13 19:03:15.000000 iommi-7.0.0/iommi/shortcut.py
--rw-r--r--   0 boxed      (501) staff       (20)     2540 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/sort_after.py
--rw-r--r--   0 boxed      (501) staff       (20)    17400 2024-04-15 10:17:16.000000 iommi-7.0.0/iommi/sql_trace.py
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.733190 iommi-7.0.0/iommi/static/
--rw-r--r--   0 boxed      (501) staff       (20)     6148 2024-01-05 19:32:48.000000 iommi-7.0.0/iommi/static/.DS_Store
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.733529 iommi-7.0.0/iommi/static/js/
--rw-r--r--   0 boxed      (501) staff       (20)    19226 2024-04-15 07:51:09.000000 iommi-7.0.0/iommi/static/js/iommi.js
--rw-r--r--   0 boxed      (501) staff       (20)     3716 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/struct.py
--rw-r--r--   0 boxed      (501) staff       (20)    10314 2024-04-15 08:37:40.000000 iommi-7.0.0/iommi/style.py
--rw-r--r--   0 boxed      (501) staff       (20)     5437 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/style_base.py
--rw-r--r--   0 boxed      (501) staff       (20)     6372 2023-10-23 18:24:08.000000 iommi-7.0.0/iommi/style_bootstrap.py
--rw-r--r--   0 boxed      (501) staff       (20)     6001 2023-02-13 19:03:15.000000 iommi-7.0.0/iommi/style_bootstrap5.py
--rw-r--r--   0 boxed      (501) staff       (20)      630 2024-04-15 08:39:12.000000 iommi-7.0.0/iommi/style_bootstrap_docs.py
--rw-r--r--   0 boxed      (501) staff       (20)      783 2024-01-31 10:54:17.000000 iommi-7.0.0/iommi/style_bootstrap_icons.py
--rw-r--r--   0 boxed      (501) staff       (20)     4529 2024-01-22 08:06:57.000000 iommi-7.0.0/iommi/style_bulma.py
--rw-r--r--   0 boxed      (501) staff       (20)     1856 2023-02-13 19:03:15.000000 iommi-7.0.0/iommi/style_django_admin.py
--rw-r--r--   0 boxed      (501) staff       (20)      793 2024-01-31 10:54:17.000000 iommi-7.0.0/iommi/style_font_awesome_4.py
--rw-r--r--   0 boxed      (501) staff       (20)      785 2024-04-15 08:36:19.000000 iommi-7.0.0/iommi/style_font_awesome_6.py
--rw-r--r--   0 boxed      (501) staff       (20)     2551 2022-01-19 10:19:49.000000 iommi-7.0.0/iommi/style_foundation.py
--rw-r--r--   0 boxed      (501) staff       (20)     3817 2023-09-06 07:14:35.000000 iommi-7.0.0/iommi/style_semantic_ui.py
--rw-r--r--   0 boxed      (501) staff       (20)      934 2024-02-26 08:28:08.000000 iommi-7.0.0/iommi/style_test_base.py
--rw-r--r--   0 boxed      (501) staff       (20)     1775 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/style_uikit.py
--rw-r--r--   0 boxed      (501) staff       (20)      309 2023-02-14 18:44:36.000000 iommi-7.0.0/iommi/style_water.py
--rw-r--r--   0 boxed      (501) staff       (20)     1887 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/synthetic_traceback.py
--rw-r--r--   0 boxed      (501) staff       (20)    83012 2024-04-15 07:51:09.000000 iommi-7.0.0/iommi/table.py
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.734191 iommi-7.0.0/iommi/templates/
--rw-r--r--   0 boxed      (501) staff       (20)     6148 2023-09-30 13:08:45.000000 iommi-7.0.0/iommi/templates/.DS_Store
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.735117 iommi-7.0.0/iommi/templates/iommi/
--rw-r--r--   0 boxed      (501) staff       (20)     6148 2022-12-11 08:59:39.000000 iommi-7.0.0/iommi/templates/iommi/.DS_Store
--rw-r--r--   0 boxed      (501) staff       (20)      623 2023-09-26 07:33:27.000000 iommi-7.0.0/iommi/templates/iommi/base.html
--rw-r--r--   0 boxed      (501) staff       (20)        0 2022-01-19 10:19:49.000000 iommi-7.0.0/iommi/templates/iommi/blank.html
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.737651 iommi-7.0.0/iommi/templates/iommi/form/
--rw-r--r--   0 boxed      (501) staff       (20)     6148 2022-12-11 19:05:37.000000 iommi-7.0.0/iommi/templates/iommi/form/.DS_Store
--rw-r--r--   0 boxed      (501) staff       (20)      873 2021-01-28 10:44:48.000000 iommi-7.0.0/iommi/templates/iommi/form/actions.html
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.737957 iommi-7.0.0/iommi/templates/iommi/form/bulma/
--rw-r--r--   0 boxed      (501) staff       (20)      255 2023-02-14 18:44:36.000000 iommi-7.0.0/iommi/templates/iommi/form/bulma/field.html
--rw-r--r--   0 boxed      (501) staff       (20)      418 2023-09-06 07:14:35.000000 iommi-7.0.0/iommi/templates/iommi/form/checkboxes.html
--rw-r--r--   0 boxed      (501) staff       (20)      495 2023-02-13 19:03:15.000000 iommi-7.0.0/iommi/templates/iommi/form/choice.html
--rw-r--r--   0 boxed      (501) staff       (20)      709 2023-02-13 19:03:15.000000 iommi-7.0.0/iommi/templates/iommi/form/choice_select2.html
--rw-r--r--   0 boxed      (501) staff       (20)      440 2024-04-15 07:32:29.000000 iommi-7.0.0/iommi/templates/iommi/form/form.html
--rw-r--r--   0 boxed      (501) staff       (20)       78 2022-01-19 10:19:49.000000 iommi-7.0.0/iommi/templates/iommi/form/heading.html
--rw-r--r--   0 boxed      (501) staff       (20)      187 2022-02-09 12:13:49.000000 iommi-7.0.0/iommi/templates/iommi/form/image_row.html
--rw-r--r--   0 boxed      (501) staff       (20)      415 2023-02-13 19:03:15.000000 iommi-7.0.0/iommi/templates/iommi/form/radio.html
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.738919 iommi-7.0.0/iommi/templates/iommi/form/semantic_ui/
--rw-r--r--   0 boxed      (501) staff       (20)      499 2023-09-06 07:14:35.000000 iommi-7.0.0/iommi/templates/iommi/form/semantic_ui/checkboxes.html
--rw-r--r--   0 boxed      (501) staff       (20)      496 2021-01-28 10:44:48.000000 iommi-7.0.0/iommi/templates/iommi/form/semantic_ui/radio.html
--rw-r--r--   0 boxed      (501) staff       (20)      166 2022-03-31 08:29:44.000000 iommi-7.0.0/iommi/templates/iommi/form/semantic_ui/row_checkbox.html
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.739204 iommi-7.0.0/iommi/templates/iommi/form/uikit/
--rw-r--r--   0 boxed      (501) staff       (20)      379 2023-02-14 18:44:36.000000 iommi-7.0.0/iommi/templates/iommi/form/uikit/row_checkbox.html
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.740170 iommi-7.0.0/iommi/templates/iommi/query/
--rw-r--r--   0 boxed      (501) staff       (20)     2622 2022-01-19 10:19:49.000000 iommi-7.0.0/iommi/templates/iommi/query/advanced.html
--rw-r--r--   0 boxed      (501) staff       (20)     1498 2021-04-15 06:01:07.000000 iommi-7.0.0/iommi/templates/iommi/query/form.html
--rw-r--r--   0 boxed      (501) staff       (20)     2808 2021-01-28 10:44:48.000000 iommi-7.0.0/iommi/templates/iommi/query/form_toggle_script.html
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.743188 iommi-7.0.0/iommi/templates/iommi/table/
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.743515 iommi-7.0.0/iommi/templates/iommi/table/bootstrap/
--rw-r--r--   0 boxed      (501) staff       (20)     1526 2024-04-15 07:16:46.000000 iommi-7.0.0/iommi/templates/iommi/table/bootstrap/paginator.html
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.743829 iommi-7.0.0/iommi/templates/iommi/table/bulma/
--rw-r--r--   0 boxed      (501) staff       (20)     1555 2024-01-22 08:06:57.000000 iommi-7.0.0/iommi/templates/iommi/table/bulma/paginator.html
--rw-r--r--   0 boxed      (501) staff       (20)      125 2024-04-15 07:14:49.000000 iommi-7.0.0/iommi/templates/iommi/table/edit_table_container.html
--rw-r--r--   0 boxed      (501) staff       (20)      188 2023-09-21 07:03:11.000000 iommi-7.0.0/iommi/templates/iommi/table/header.html
--rw-r--r--   0 boxed      (501) staff       (20)     2303 2021-01-28 10:44:48.000000 iommi-7.0.0/iommi/templates/iommi/table/js_select_all.html
--rw-r--r--   0 boxed      (501) staff       (20)     1814 2024-04-15 07:16:49.000000 iommi-7.0.0/iommi/templates/iommi/table/paginator.html
--rw-r--r--   0 boxed      (501) staff       (20)      102 2023-02-13 19:03:15.000000 iommi-7.0.0/iommi/templates/iommi/table/row_group.html
--rw-r--r--   0 boxed      (501) staff       (20)      196 2022-10-31 14:55:23.000000 iommi-7.0.0/iommi/templates/iommi/table/select_column_header.html
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.744138 iommi-7.0.0/iommi/templates/iommi/table/semantic_ui/
--rw-r--r--   0 boxed      (501) staff       (20)     1091 2023-02-13 19:03:15.000000 iommi-7.0.0/iommi/templates/iommi/table/semantic_ui/paginator.html
--rw-r--r--   0 boxed      (501) staff       (20)       18 2023-02-13 19:03:15.000000 iommi-7.0.0/iommi/templates/iommi/table/table.html
--rw-r--r--   0 boxed      (501) staff       (20)      669 2024-04-15 07:14:49.000000 iommi-7.0.0/iommi/templates/iommi/table/table_container.html
--rw-r--r--   0 boxed      (501) staff       (20)      209 2021-01-28 10:44:48.000000 iommi-7.0.0/iommi/templates/iommi/table/table_header_rows.html
--rw-r--r--   0 boxed      (501) staff       (20)      560 2023-04-26 11:31:39.000000 iommi-7.0.0/iommi/templates/iommi/table/table_tag.html
--rw-r--r--   0 boxed      (501) staff       (20)      207 2022-01-13 18:46:04.000000 iommi-7.0.0/iommi/thread_locals.py
--rw-r--r--   0 boxed      (501) staff       (20)    11874 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/traversable.py
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.725965 iommi-7.0.0/iommi.egg-info/
--rw-r--r--   0 boxed      (501) staff       (20)     3079 2024-04-15 10:45:20.000000 iommi-7.0.0/iommi.egg-info/PKG-INFO
--rw-r--r--   0 boxed      (501) staff       (20)     3621 2024-04-15 10:45:20.000000 iommi-7.0.0/iommi.egg-info/SOURCES.txt
--rw-r--r--   0 boxed      (501) staff       (20)        1 2024-04-15 10:45:20.000000 iommi-7.0.0/iommi.egg-info/dependency_links.txt
--rw-r--r--   0 boxed      (501) staff       (20)        1 2021-01-28 11:41:36.000000 iommi-7.0.0/iommi.egg-info/not-zip-safe
--rw-r--r--   0 boxed      (501) staff       (20)       22 2024-04-15 10:45:20.000000 iommi-7.0.0/iommi.egg-info/requires.txt
--rw-r--r--   0 boxed      (501) staff       (20)        6 2024-04-15 10:45:20.000000 iommi-7.0.0/iommi.egg-info/top_level.txt
--rw-r--r--   0 boxed      (501) staff       (20)      534 2024-03-07 08:19:20.000000 iommi-7.0.0/pyproject.toml
--rw-r--r--   0 boxed      (501) staff       (20)       10 2023-02-13 19:03:15.000000 iommi-7.0.0/requirements.txt
--rw-r--r--   0 boxed      (501) staff       (20)     1158 2024-04-15 10:45:20.746782 iommi-7.0.0/setup.cfg
--rwxr-xr-x   0 boxed      (501) staff       (20)     2893 2024-03-07 08:19:20.000000 iommi-7.0.0/setup.py
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-05-06 14:09:23.785540 iommi-7.1.0/
+-rw-r--r--   0 boxed      (501) staff       (20)     1102 2024-02-18 13:30:36.000000 iommi-7.1.0/AUTHORS.rst
+-rw-r--r--   0 boxed      (501) staff       (20)      212 2021-01-28 10:44:48.000000 iommi-7.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 boxed      (501) staff       (20)    43006 2024-05-06 14:07:01.000000 iommi-7.1.0/HISTORY.rst
+-rw-r--r--   0 boxed      (501) staff       (20)     1485 2021-01-28 10:44:48.000000 iommi-7.1.0/LICENSE
+-rw-r--r--   0 boxed      (501) staff       (20)      332 2022-01-21 14:21:52.000000 iommi-7.1.0/MANIFEST.in
+-rw-r--r--   0 boxed      (501) staff       (20)     3079 2024-05-06 14:09:23.785474 iommi-7.1.0/PKG-INFO
+-rw-r--r--   0 boxed      (501) staff       (20)     2781 2023-04-05 18:05:05.000000 iommi-7.1.0/README.rst
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-05-06 14:09:23.770960 iommi-7.1.0/iommi/
+-rw-r--r--   0 boxed      (501) staff       (20)     8196 2024-05-04 18:55:45.000000 iommi-7.1.0/iommi/.DS_Store
+-rw-r--r--   0 boxed      (501) staff       (20)     3606 2024-05-06 14:08:12.000000 iommi-7.1.0/iommi/__init__.py
+-rw-r--r--   0 boxed      (501) staff       (20)     6392 2024-04-17 06:35:25.000000 iommi-7.1.0/iommi/_db_compat.py
+-rw-r--r--   0 boxed      (501) staff       (20)     6583 2024-04-17 06:35:25.000000 iommi-7.1.0/iommi/_web_compat.py
+-rw-r--r--   0 boxed      (501) staff       (20)      532 2024-03-07 08:19:20.000000 iommi-7.1.0/iommi/_web_compat_flask.py
+-rw-r--r--   0 boxed      (501) staff       (20)     5757 2024-03-07 08:19:20.000000 iommi-7.1.0/iommi/action.py
+-rw-r--r--   0 boxed      (501) staff       (20)    21292 2024-04-17 06:35:25.000000 iommi-7.1.0/iommi/admin.py
+-rw-r--r--   0 boxed      (501) staff       (20)     1893 2024-04-17 06:35:25.000000 iommi-7.1.0/iommi/apps.py
+-rw-r--r--   0 boxed      (501) staff       (20)     1950 2023-02-13 19:03:15.000000 iommi-7.1.0/iommi/asset.py
+-rw-r--r--   0 boxed      (501) staff       (20)     5010 2024-03-07 08:19:20.000000 iommi-7.1.0/iommi/attrs.py
+-rw-r--r--   0 boxed      (501) staff       (20)     2591 2024-03-07 08:19:20.000000 iommi-7.1.0/iommi/base.py
+-rw-r--r--   0 boxed      (501) staff       (20)     4902 2022-01-19 10:19:49.000000 iommi-7.1.0/iommi/datetime_parsing.py
+-rw-r--r--   0 boxed      (501) staff       (20)    12111 2024-04-17 06:35:25.000000 iommi-7.1.0/iommi/debug.py
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-05-06 14:09:23.773204 iommi-7.1.0/iommi/declarative/
+-rw-r--r--   0 boxed      (501) staff       (20)     6148 2023-12-11 09:30:40.000000 iommi-7.1.0/iommi/declarative/.DS_Store
+-rw-r--r--   0 boxed      (501) staff       (20)     5461 2024-03-07 08:19:20.000000 iommi-7.1.0/iommi/declarative/__init__.py
+-rw-r--r--   0 boxed      (501) staff       (20)      571 2023-02-13 19:03:15.000000 iommi-7.1.0/iommi/declarative/dispatch.py
+-rw-r--r--   0 boxed      (501) staff       (20)     7950 2024-04-17 06:35:25.000000 iommi-7.1.0/iommi/declarative/namespace.py
+-rw-r--r--   0 boxed      (501) staff       (20)     1938 2023-02-13 19:03:15.000000 iommi-7.1.0/iommi/declarative/util.py
+-rw-r--r--   0 boxed      (501) staff       (20)     1501 2023-09-06 07:14:35.000000 iommi-7.1.0/iommi/declarative/with_meta.py
+-rw-r--r--   0 boxed      (501) staff       (20)    12419 2024-03-07 08:19:20.000000 iommi-7.1.0/iommi/docs.py
+-rw-r--r--   0 boxed      (501) staff       (20)    17950 2024-04-15 07:14:49.000000 iommi-7.1.0/iommi/edit_table.py
+-rw-r--r--   0 boxed      (501) staff       (20)     3769 2024-03-07 08:19:20.000000 iommi-7.1.0/iommi/endpoint.py
+-rw-r--r--   0 boxed      (501) staff       (20)     1477 2023-02-13 19:03:15.000000 iommi-7.1.0/iommi/error.py
+-rw-r--r--   0 boxed      (501) staff       (20)     5020 2024-04-17 06:35:25.000000 iommi-7.1.0/iommi/evaluate.py
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-05-06 14:09:23.773801 iommi-7.1.0/iommi/experimental/
+-rw-r--r--   0 boxed      (501) staff       (20)     6148 2023-12-11 09:30:40.000000 iommi-7.1.0/iommi/experimental/.DS_Store
+-rw-r--r--   0 boxed      (501) staff       (20)        0 2022-01-19 10:19:49.000000 iommi-7.1.0/iommi/experimental/__init__.py
+-rw-r--r--   0 boxed      (501) staff       (20)      133 2023-02-13 19:03:15.000000 iommi-7.1.0/iommi/experimental/edit_table.py
+-rw-r--r--   0 boxed      (501) staff       (20)    71770 2024-04-17 06:35:25.000000 iommi-7.1.0/iommi/form.py
+-rw-r--r--   0 boxed      (501) staff       (20)     8184 2024-03-07 08:19:20.000000 iommi-7.1.0/iommi/fragment.py
+-rw-r--r--   0 boxed      (501) staff       (20)    10065 2024-04-17 06:35:25.000000 iommi-7.1.0/iommi/from_model.py
+-rw-r--r--   0 boxed      (501) staff       (20)    19707 2024-04-17 06:35:25.000000 iommi-7.1.0/iommi/live_edit.py
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-05-06 14:09:23.774004 iommi-7.1.0/iommi/locale/
+-rw-r--r--   0 boxed      (501) staff       (20)     6148 2024-01-05 19:32:48.000000 iommi-7.1.0/iommi/locale/.DS_Store
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-05-06 14:09:23.753395 iommi-7.1.0/iommi/locale/cs/
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-05-06 14:09:23.774517 iommi-7.1.0/iommi/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 boxed      (501) staff       (20)     4410 2023-12-13 09:01:15.000000 iommi-7.1.0/iommi/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 boxed      (501) staff       (20)     7115 2023-11-22 17:28:48.000000 iommi-7.1.0/iommi/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-05-06 14:09:23.774873 iommi-7.1.0/iommi/locale/de/
+-rw-r--r--   0 boxed      (501) staff       (20)     6148 2022-01-02 19:23:31.000000 iommi-7.1.0/iommi/locale/de/.DS_Store
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-05-06 14:09:23.775397 iommi-7.1.0/iommi/locale/de/LC_MESSAGES/
+-rw-r--r--   0 boxed      (501) staff       (20)     4442 2023-12-13 09:01:15.000000 iommi-7.1.0/iommi/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 boxed      (501) staff       (20)     7751 2023-11-22 17:28:48.000000 iommi-7.1.0/iommi/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-05-06 14:09:23.775635 iommi-7.1.0/iommi/locale/sv/
+-rw-r--r--   0 boxed      (501) staff       (20)     6148 2022-01-02 19:23:31.000000 iommi-7.1.0/iommi/locale/sv/.DS_Store
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-05-06 14:09:23.776037 iommi-7.1.0/iommi/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 boxed      (501) staff       (20)     5588 2023-12-13 09:01:15.000000 iommi-7.1.0/iommi/locale/sv/LC_MESSAGES/django.mo
+-rw-r--r--   0 boxed      (501) staff       (20)     7390 2023-11-22 17:28:48.000000 iommi-7.1.0/iommi/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-05-06 14:09:23.753740 iommi-7.1.0/iommi/locale/uk/
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-05-06 14:09:23.776526 iommi-7.1.0/iommi/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 boxed      (501) staff       (20)     5610 2023-12-13 09:01:15.000000 iommi-7.1.0/iommi/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0 boxed      (501) staff       (20)     8431 2023-11-22 17:28:48.000000 iommi-7.1.0/iommi/locale/uk/LC_MESSAGES/django.po
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-05-06 14:09:23.753847 iommi-7.1.0/iommi/locale/zh_Hans/
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-05-06 14:09:23.777070 iommi-7.1.0/iommi/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 boxed      (501) staff       (20)     3975 2023-12-13 09:01:15.000000 iommi-7.1.0/iommi/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 boxed      (501) staff       (20)     7182 2023-11-22 17:28:48.000000 iommi-7.1.0/iommi/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0 boxed      (501) staff       (20)    10204 2024-03-07 08:19:20.000000 iommi-7.1.0/iommi/member.py
+-rw-r--r--   0 boxed      (501) staff       (20)    11434 2024-04-17 06:35:25.000000 iommi-7.1.0/iommi/menu.py
+-rw-r--r--   0 boxed      (501) staff       (20)     3761 2024-03-07 08:19:20.000000 iommi-7.1.0/iommi/page.py
+-rw-r--r--   0 boxed      (501) staff       (20)     8408 2024-04-17 06:35:25.000000 iommi-7.1.0/iommi/part.py
+-rw-r--r--   0 boxed      (501) staff       (20)     4769 2024-04-17 06:35:25.000000 iommi-7.1.0/iommi/path.py
+-rw-r--r--   0 boxed      (501) staff       (20)    10370 2024-04-17 06:35:25.000000 iommi-7.1.0/iommi/profiling.py
+-rw-r--r--   0 boxed      (501) staff       (20)    36786 2024-04-15 07:51:09.000000 iommi-7.1.0/iommi/query.py
+-rw-r--r--   0 boxed      (501) staff       (20)     8660 2024-04-17 06:35:25.000000 iommi-7.1.0/iommi/refinable.py
+-rw-r--r--   0 boxed      (501) staff       (20)     2717 2023-02-13 19:03:15.000000 iommi-7.1.0/iommi/shortcut.py
+-rw-r--r--   0 boxed      (501) staff       (20)     2540 2024-03-07 08:19:20.000000 iommi-7.1.0/iommi/sort_after.py
+-rw-r--r--   0 boxed      (501) staff       (20)    17493 2024-04-17 06:35:25.000000 iommi-7.1.0/iommi/sql_trace.py
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-05-06 14:09:23.777376 iommi-7.1.0/iommi/static/
+-rw-r--r--   0 boxed      (501) staff       (20)     6148 2024-01-05 19:32:48.000000 iommi-7.1.0/iommi/static/.DS_Store
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-05-06 14:09:23.777619 iommi-7.1.0/iommi/static/js/
+-rw-r--r--   0 boxed      (501) staff       (20)    19226 2024-04-15 07:51:09.000000 iommi-7.1.0/iommi/static/js/iommi.js
+-rw-r--r--   0 boxed      (501) staff       (20)     3646 2024-04-17 06:35:25.000000 iommi-7.1.0/iommi/struct.py
+-rw-r--r--   0 boxed      (501) staff       (20)    10316 2024-04-17 06:35:25.000000 iommi-7.1.0/iommi/style.py
+-rw-r--r--   0 boxed      (501) staff       (20)     5506 2024-04-17 06:35:25.000000 iommi-7.1.0/iommi/style_base.py
+-rw-r--r--   0 boxed      (501) staff       (20)     6459 2024-04-17 06:35:25.000000 iommi-7.1.0/iommi/style_bootstrap.py
+-rw-r--r--   0 boxed      (501) staff       (20)     6001 2024-04-15 11:14:35.000000 iommi-7.1.0/iommi/style_bootstrap5.py
+-rw-r--r--   0 boxed      (501) staff       (20)      630 2024-04-15 08:39:12.000000 iommi-7.1.0/iommi/style_bootstrap_docs.py
+-rw-r--r--   0 boxed      (501) staff       (20)      878 2024-04-17 06:35:25.000000 iommi-7.1.0/iommi/style_bootstrap_icons.py
+-rw-r--r--   0 boxed      (501) staff       (20)     4529 2024-01-22 08:06:57.000000 iommi-7.1.0/iommi/style_bulma.py
+-rw-r--r--   0 boxed      (501) staff       (20)     1856 2023-02-13 19:03:15.000000 iommi-7.1.0/iommi/style_django_admin.py
+-rw-r--r--   0 boxed      (501) staff       (20)      787 2024-04-17 06:35:25.000000 iommi-7.1.0/iommi/style_font_awesome_4.py
+-rw-r--r--   0 boxed      (501) staff       (20)      873 2024-04-17 06:35:25.000000 iommi-7.1.0/iommi/style_font_awesome_6.py
+-rw-r--r--   0 boxed      (501) staff       (20)     2551 2022-01-19 10:19:49.000000 iommi-7.1.0/iommi/style_foundation.py
+-rw-r--r--   0 boxed      (501) staff       (20)     3817 2023-09-06 07:14:35.000000 iommi-7.1.0/iommi/style_semantic_ui.py
+-rw-r--r--   0 boxed      (501) staff       (20)      934 2024-02-26 08:28:08.000000 iommi-7.1.0/iommi/style_test_base.py
+-rw-r--r--   0 boxed      (501) staff       (20)     1775 2024-04-17 06:35:25.000000 iommi-7.1.0/iommi/style_uikit.py
+-rw-r--r--   0 boxed      (501) staff       (20)      309 2023-02-14 18:44:36.000000 iommi-7.1.0/iommi/style_water.py
+-rw-r--r--   0 boxed      (501) staff       (20)     1887 2024-03-07 08:19:20.000000 iommi-7.1.0/iommi/synthetic_traceback.py
+-rw-r--r--   0 boxed      (501) staff       (20)    83053 2024-04-17 06:35:25.000000 iommi-7.1.0/iommi/table.py
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-05-06 14:09:23.777960 iommi-7.1.0/iommi/templates/
+-rw-r--r--   0 boxed      (501) staff       (20)     6148 2023-09-30 13:08:45.000000 iommi-7.1.0/iommi/templates/.DS_Store
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-05-06 14:09:23.778684 iommi-7.1.0/iommi/templates/iommi/
+-rw-r--r--   0 boxed      (501) staff       (20)     6148 2022-12-11 08:59:39.000000 iommi-7.1.0/iommi/templates/iommi/.DS_Store
+-rw-r--r--   0 boxed      (501) staff       (20)      623 2023-09-26 07:33:27.000000 iommi-7.1.0/iommi/templates/iommi/base.html
+-rw-r--r--   0 boxed      (501) staff       (20)        0 2022-01-19 10:19:49.000000 iommi-7.1.0/iommi/templates/iommi/blank.html
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-05-06 14:09:23.780517 iommi-7.1.0/iommi/templates/iommi/form/
+-rw-r--r--   0 boxed      (501) staff       (20)     6148 2022-12-11 19:05:37.000000 iommi-7.1.0/iommi/templates/iommi/form/.DS_Store
+-rw-r--r--   0 boxed      (501) staff       (20)      873 2021-01-28 10:44:48.000000 iommi-7.1.0/iommi/templates/iommi/form/actions.html
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-05-06 14:09:23.780651 iommi-7.1.0/iommi/templates/iommi/form/bulma/
+-rw-r--r--   0 boxed      (501) staff       (20)      255 2023-02-14 18:44:36.000000 iommi-7.1.0/iommi/templates/iommi/form/bulma/field.html
+-rw-r--r--   0 boxed      (501) staff       (20)      418 2023-09-06 07:14:35.000000 iommi-7.1.0/iommi/templates/iommi/form/checkboxes.html
+-rw-r--r--   0 boxed      (501) staff       (20)      495 2023-02-13 19:03:15.000000 iommi-7.1.0/iommi/templates/iommi/form/choice.html
+-rw-r--r--   0 boxed      (501) staff       (20)      709 2023-02-13 19:03:15.000000 iommi-7.1.0/iommi/templates/iommi/form/choice_select2.html
+-rw-r--r--   0 boxed      (501) staff       (20)      440 2024-04-15 07:32:29.000000 iommi-7.1.0/iommi/templates/iommi/form/form.html
+-rw-r--r--   0 boxed      (501) staff       (20)       78 2022-01-19 10:19:49.000000 iommi-7.1.0/iommi/templates/iommi/form/heading.html
+-rw-r--r--   0 boxed      (501) staff       (20)      187 2022-02-09 12:13:49.000000 iommi-7.1.0/iommi/templates/iommi/form/image_row.html
+-rw-r--r--   0 boxed      (501) staff       (20)      415 2023-02-13 19:03:15.000000 iommi-7.1.0/iommi/templates/iommi/form/radio.html
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-05-06 14:09:23.781308 iommi-7.1.0/iommi/templates/iommi/form/semantic_ui/
+-rw-r--r--   0 boxed      (501) staff       (20)      499 2023-09-06 07:14:35.000000 iommi-7.1.0/iommi/templates/iommi/form/semantic_ui/checkboxes.html
+-rw-r--r--   0 boxed      (501) staff       (20)      496 2021-01-28 10:44:48.000000 iommi-7.1.0/iommi/templates/iommi/form/semantic_ui/radio.html
+-rw-r--r--   0 boxed      (501) staff       (20)      166 2022-03-31 08:29:44.000000 iommi-7.1.0/iommi/templates/iommi/form/semantic_ui/row_checkbox.html
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-05-06 14:09:23.781527 iommi-7.1.0/iommi/templates/iommi/form/uikit/
+-rw-r--r--   0 boxed      (501) staff       (20)      379 2023-02-14 18:44:36.000000 iommi-7.1.0/iommi/templates/iommi/form/uikit/row_checkbox.html
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-05-06 14:09:23.782310 iommi-7.1.0/iommi/templates/iommi/query/
+-rw-r--r--   0 boxed      (501) staff       (20)     2622 2022-01-19 10:19:49.000000 iommi-7.1.0/iommi/templates/iommi/query/advanced.html
+-rw-r--r--   0 boxed      (501) staff       (20)     1498 2021-04-15 06:01:07.000000 iommi-7.1.0/iommi/templates/iommi/query/form.html
+-rw-r--r--   0 boxed      (501) staff       (20)     2808 2021-01-28 10:44:48.000000 iommi-7.1.0/iommi/templates/iommi/query/form_toggle_script.html
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-05-06 14:09:23.784600 iommi-7.1.0/iommi/templates/iommi/table/
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-05-06 14:09:23.784819 iommi-7.1.0/iommi/templates/iommi/table/bootstrap/
+-rw-r--r--   0 boxed      (501) staff       (20)     1526 2024-04-15 07:16:46.000000 iommi-7.1.0/iommi/templates/iommi/table/bootstrap/paginator.html
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-05-06 14:09:23.784990 iommi-7.1.0/iommi/templates/iommi/table/bulma/
+-rw-r--r--   0 boxed      (501) staff       (20)     1555 2024-01-22 08:06:57.000000 iommi-7.1.0/iommi/templates/iommi/table/bulma/paginator.html
+-rw-r--r--   0 boxed      (501) staff       (20)      125 2024-04-15 07:14:49.000000 iommi-7.1.0/iommi/templates/iommi/table/edit_table_container.html
+-rw-r--r--   0 boxed      (501) staff       (20)      188 2023-09-21 07:03:11.000000 iommi-7.1.0/iommi/templates/iommi/table/header.html
+-rw-r--r--   0 boxed      (501) staff       (20)     2303 2021-01-28 10:44:48.000000 iommi-7.1.0/iommi/templates/iommi/table/js_select_all.html
+-rw-r--r--   0 boxed      (501) staff       (20)     1814 2024-04-15 07:16:49.000000 iommi-7.1.0/iommi/templates/iommi/table/paginator.html
+-rw-r--r--   0 boxed      (501) staff       (20)      102 2023-02-13 19:03:15.000000 iommi-7.1.0/iommi/templates/iommi/table/row_group.html
+-rw-r--r--   0 boxed      (501) staff       (20)      206 2024-04-15 11:07:29.000000 iommi-7.1.0/iommi/templates/iommi/table/select_column_header.html
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-05-06 14:09:23.785211 iommi-7.1.0/iommi/templates/iommi/table/semantic_ui/
+-rw-r--r--   0 boxed      (501) staff       (20)     1091 2023-02-13 19:03:15.000000 iommi-7.1.0/iommi/templates/iommi/table/semantic_ui/paginator.html
+-rw-r--r--   0 boxed      (501) staff       (20)       18 2023-02-13 19:03:15.000000 iommi-7.1.0/iommi/templates/iommi/table/table.html
+-rw-r--r--   0 boxed      (501) staff       (20)      669 2024-04-15 07:14:49.000000 iommi-7.1.0/iommi/templates/iommi/table/table_container.html
+-rw-r--r--   0 boxed      (501) staff       (20)      209 2021-01-28 10:44:48.000000 iommi-7.1.0/iommi/templates/iommi/table/table_header_rows.html
+-rw-r--r--   0 boxed      (501) staff       (20)      560 2023-04-26 11:31:39.000000 iommi-7.1.0/iommi/templates/iommi/table/table_tag.html
+-rw-r--r--   0 boxed      (501) staff       (20)      207 2022-01-13 18:46:04.000000 iommi-7.1.0/iommi/thread_locals.py
+-rw-r--r--   0 boxed      (501) staff       (20)    12076 2024-05-06 14:04:48.000000 iommi-7.1.0/iommi/traversable.py
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-05-06 14:09:23.771923 iommi-7.1.0/iommi.egg-info/
+-rw-r--r--   0 boxed      (501) staff       (20)     3079 2024-05-06 14:09:23.000000 iommi-7.1.0/iommi.egg-info/PKG-INFO
+-rw-r--r--   0 boxed      (501) staff       (20)     3621 2024-05-06 14:09:23.000000 iommi-7.1.0/iommi.egg-info/SOURCES.txt
+-rw-r--r--   0 boxed      (501) staff       (20)        1 2024-05-06 14:09:23.000000 iommi-7.1.0/iommi.egg-info/dependency_links.txt
+-rw-r--r--   0 boxed      (501) staff       (20)        1 2021-01-28 11:41:36.000000 iommi-7.1.0/iommi.egg-info/not-zip-safe
+-rw-r--r--   0 boxed      (501) staff       (20)       22 2024-05-06 14:09:23.000000 iommi-7.1.0/iommi.egg-info/requires.txt
+-rw-r--r--   0 boxed      (501) staff       (20)        6 2024-05-06 14:09:23.000000 iommi-7.1.0/iommi.egg-info/top_level.txt
+-rw-r--r--   0 boxed      (501) staff       (20)      534 2024-03-07 08:19:20.000000 iommi-7.1.0/pyproject.toml
+-rw-r--r--   0 boxed      (501) staff       (20)       10 2023-02-13 19:03:15.000000 iommi-7.1.0/requirements.txt
+-rw-r--r--   0 boxed      (501) staff       (20)     1158 2024-05-06 14:09:23.785908 iommi-7.1.0/setup.cfg
+-rwxr-xr-x   0 boxed      (501) staff       (20)     2893 2024-03-07 08:19:20.000000 iommi-7.1.0/setup.py
```

### Comparing `iommi-7.0.0/AUTHORS.rst` & `iommi-7.1.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/HISTORY.rst` & `iommi-7.1.0/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,25 @@
 Changelog
 ---------
 
+7.1.0 (2024-05-06)
+~~~~~~~~~~~~~~~~~~
+
+* `user` is now included in the evaluate parameters
+
+* All params from `params` are now included in evaluate parameters
+
+* Fix bulk form render when not needed
+
+* Admin: remove default bulk delete
+
+* Select all fixed
+
+* Admin all models list should be `Table`, not `EditTable`
+
 7.0.0 (2024-04-15)
 ~~~~~~~~~~~~~~~~~~
 
 * `EditTable`s `EditColumn.edit` namespace is now called `field`. This is a breaking change. There was a namespace conflict between `Column.edit` and `EditColumn.edit`.
 
 * `EditTable` and bulk editing and filtering now compose cleanly
```

### Comparing `iommi-7.0.0/LICENSE` & `iommi-7.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/PKG-INFO` & `iommi-7.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iommi
-Version: 7.0.0
+Version: 7.1.0
 Summary: iommi is a high level framework built on django
 Home-page: https://github.com/iommirocks/iommi
 Author: Anders Hovmöller
 Author-email: boxed@killingar.net
 License: BSD
 Keywords: iommi
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `iommi-7.0.0/README.rst` & `iommi-7.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/.DS_Store` & `iommi-7.1.0/iommi/.DS_Store`

 * *Files 16% similar despite different names*

```diff
@@ -253,34 +253,34 @@
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0000 0000 001e 0000 000b  ................
 00001010: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00001020: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00001030: 0000 007a 4c87 0000 000b 005f 005f 0070  ...zL......_._.p
+00001030: 0000 00a6 f159 0000 000b 005f 005f 0070  .....Y....._._.p
 00001040: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00001050: 6d6f 4444 626c 6f62 0000 0008 0cb6 dc6a  moDDblob.......j
-00001060: b4de c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
+00001050: 6d6f 4444 626c 6f62 0000 0008 8e45 6a97  moDDblob.....Ej.
+00001060: d2e7 c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
 00001070: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00001080: 6444 626c 6f62 0000 0008 0cb6 dc6a b4de  dDblob.......j..
+00001080: 6444 626c 6f62 0000 0008 8e45 6a97 d2e7  dDblob.....Ej...
 00001090: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000010a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000010b0: 636f 6d70 0000 0000 0083 f000 0000 000b  comp............
+000010b0: 636f 6d70 0000 0000 00b1 d000 0000 000b  comp............
 000010c0: 0064 0065 0063 006c 0061 0072 0061 0074  .d.e.c.l.a.r.a.t
 000010d0: 0069 0076 0065 6c67 3153 636f 6d70 0000  .i.v.elg1Scomp..
-000010e0: 0000 000c 11d5 0000 000b 0064 0065 0063  ...........d.e.c
+000010e0: 0000 0010 2de7 0000 000b 0064 0065 0063  ....-......d.e.c
 000010f0: 006c 0061 0072 0061 0074 0069 0076 0065  .l.a.r.a.t.i.v.e
-00001100: 6d6f 4444 626c 6f62 0000 0008 c304 0304  moDDblob........
-00001110: d8cc c541 0000 000b 0064 0065 0063 006c  ...A.....d.e.c.l
+00001100: 6d6f 4444 626c 6f62 0000 0008 ae1a d996  moDDblob........
+00001110: d2e7 c541 0000 000b 0064 0065 0063 006c  ...A.....d.e.c.l
 00001120: 0061 0072 0061 0074 0069 0076 0065 6d6f  .a.r.a.t.i.v.emo
-00001130: 6444 626c 6f62 0000 0008 c304 0304 d8cc  dDblob..........
+00001130: 6444 626c 6f62 0000 0008 ae1a d996 d2e7  dDblob..........
 00001140: c541 0000 000b 0064 0065 0063 006c 0061  .A.....d.e.c.l.a
 00001150: 0072 0061 0074 0069 0076 0065 7068 3153  .r.a.t.i.v.eph1S
-00001160: 636f 6d70 0000 0000 000d 7000 0000 000c  comp......p.....
+00001160: 636f 6d70 0000 0000 0011 b000 0000 000c  comp............
 00001170: 0065 0078 0070 0065 0072 0069 006d 0065  .e.x.p.e.r.i.m.e
 00001180: 006e 0074 0061 006c 6c67 3153 636f 6d70  .n.t.a.llg1Scomp
 00001190: 0000 0000 0000 1f80 0000 000c 0065 0078  .............e.x
 000011a0: 0070 0065 0072 0069 006d 0065 006e 0074  .p.e.r.i.m.e.n.t
 000011b0: 0061 006c 6d6f 4444 626c 6f62 0000 0008  .a.lmoDDblob....
 000011c0: 19bd aa79 60cd c441 0000 000c 0065 0078  ...y`..A.....e.x
 000011d0: 0070 0065 0072 0069 006d 0065 006e 0074  .p.e.r.i.m.e.n.t
@@ -319,32 +319,32 @@
 000013e0: 6f62 0000 0008 cbc8 6f15 d4c1 c341 0000  ob......o....A..
 000013f0: 0009 0073 006e 0061 0070 0073 0068 006f  ...s.n.a.p.s.h.o
 00001400: 0074 0073 6d6f 6444 626c 6f62 0000 0008  .t.smodDblob....
 00001410: cbc8 6f15 d4c1 c341 0000 0009 0073 006e  ..o....A.....s.n
 00001420: 0061 0070 0073 0068 006f 0074 0073 7068  .a.p.s.h.o.t.sph
 00001430: 3153 636f 6d70 0000 0000 0000 a000 0000  1Scomp..........
 00001440: 0006 0073 0074 0061 0074 0069 0063 6c67  ...s.t.a.t.i.clg
-00001450: 3153 636f 6d70 0000 0000 0000 6e00 0000  1Scomp......n...
+00001450: 3153 636f 6d70 0000 0000 0000 631e 0000  1Scomp......c...
 00001460: 0006 0073 0074 0061 0074 0069 0063 6d6f  ...s.t.a.t.i.cmo
 00001470: 4444 626c 6f62 0000 0008 c31c 49cb 3149  DDblob......I.1I
 00001480: c541 0000 0006 0073 0074 0061 0074 0069  .A.....s.t.a.t.i
 00001490: 0063 6d6f 6444 626c 6f62 0000 0008 c31c  .cmodDblob......
 000014a0: 49cb 3149 c541 0000 0006 0073 0074 0061  I.1I.A.....s.t.a
 000014b0: 0074 0069 0063 7068 3153 636f 6d70 0000  .t.i.cph1Scomp..
-000014c0: 0000 0000 8000 0000 0009 0074 0065 006d  ...........t.e.m
+000014c0: 0000 0000 7000 0000 0009 0074 0065 006d  ....p......t.e.m
 000014d0: 0070 006c 0061 0074 0065 0073 6c67 3153  .p.l.a.t.e.slg1S
-000014e0: 636f 6d70 0000 0000 0000 a1aa 0000 0009  comp............
+000014e0: 636f 6d70 0000 0000 0000 a32b 0000 0009  comp.......+....
 000014f0: 0074 0065 006d 0070 006c 0061 0074 0065  .t.e.m.p.l.a.t.e
 00001500: 0073 6d6f 4444 626c 6f62 0000 0008 fda2  .smoDDblob......
 00001510: b6ff 0614 c341 0000 0009 0074 0065 006d  .....A.....t.e.m
 00001520: 0070 006c 0061 0074 0065 0073 6d6f 6444  .p.l.a.t.e.smodD
 00001530: 626c 6f62 0000 0008 fda2 b6ff 0614 c341  blob...........A
 00001540: 0000 0009 0074 0065 006d 0070 006c 0061  .....t.e.m.p.l.a
 00001550: 0074 0065 0073 7068 3153 636f 6d70 0000  .t.e.sph1Scomp..
-00001560: 0000 0002 3000 0000 0000 0000 0000 0000  ....0...........
+00001560: 0000 0002 4000 0000 0000 0000 0000 0000  ....@...........
 00001570: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001580: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001590: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000015a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000015b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000015c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000015d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -464,15 +464,15 @@
 00001cf0: 0000 0000 0140 0000 0000 0000 0074 0065  .....@.......t.e
 00001d00: 0073 6d6f 4444 626c 6f62 0000 0008 fda2  .smoDDblob......
 00001d10: b6ff 0614 c341 0000 0009 0074 0065 006d  .....A.....t.e.m
 00001d20: 0070 006c 0061 0074 0065 0073 6d6f 6444  .p.l.a.t.e.smodD
 00001d30: 626c 6f62 0000 0008 fda2 b6ff 0614 c341  blob...........A
 00001d40: 0000 0009 0074 0065 006d 0070 006c 0061  .....t.e.m.p.l.a
 00001d50: 0074 0065 0073 7068 3153 636f 6d70 0000  .t.e.sph1Scomp..
-00001d60: 0000 0002 3000 0000 0000 0000 0000 0000  ....0...........
+00001d60: 0000 0002 4000 0000 0000 0000 0000 0000  ....@...........
 00001d70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001da0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001dd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `iommi-7.0.0/iommi/__init__.py` & `iommi-7.1.0/iommi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '7.0.0'
+__version__ = '7.1.0'
 
 from functools import wraps
 
 import django
 from django.core.exceptions import ImproperlyConfigured
 
 from iommi._db_compat import (
```

### Comparing `iommi-7.0.0/iommi/_db_compat.py` & `iommi-7.1.0/iommi/_db_compat.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,14 +92,15 @@
 
     register_field_factory(CharField, factory=char_field_field_factory)
     register_filter_factory(CharField, factory=char_field_filter_factory)
     register_column_factory(CharField, factory=char_field_column_factory)
 
     try:
         from django.contrib.postgres.search import SearchVectorField
+
         register_factory(SearchVectorField, factory=None)
     except ImportError:
         pass
     register_factory(UUIDField, shortcut_name='text')
     register_factory(TimeField, shortcut_name='time')
     register_factory(EmailField, shortcut_name='email')
     register_factory(DecimalField, shortcut_name='decimal')
```

### Comparing `iommi-7.0.0/iommi/_web_compat.py` & `iommi-7.1.0/iommi/_web_compat.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,30 +49,34 @@
         import jinja2  # noqa: F401
         from jinja2 import Template as JinjaTemplate
 
         template_types += (JinjaTemplate,)
 except ImproperlyConfigured:
     pass
 
+
 class Template:
     def __init__(self, template_string):
         self.s = template_string
 
     def render(self, context):  # noqa: F811
         if DjangoTemplate is not None:
             return DjangoTemplate(self.s).render(context=context)
         else:
             assert JinjaTemplate is not None
             return JinjaTemplate(self.s).render(**context.flatten())
 
+
 template_types = template_types + (Template,)
 
+
 def csrf(request):
     return {} if request is None else csrf_(request)
 
+
 try:
     from django.template.loader import get_template_from_string
 except ImportError:  # pragma: no cover
     # Django 1.8+
     # noinspection PyUnresolvedReferences
     from django.template import engines
 
@@ -114,14 +118,15 @@
     elif isinstance(template, DjangoLoadedTemplate):
         return mark_safe(template.render(context=context, request=request))
     elif isinstance(template, template_types):
         return mark_safe(template.render(context=RequestContext(request, context)))
     else:
         return mark_safe(template.render(context, request))
 
+
 # except ImportError:  # pragma: no cover This flask support is a work in progress/future plan
 #     from jinja2 import Markup
 #     from flask import render_template as render
 #     from ._web_compat_flask import HttpRequest  # noqa: F401
 #
 #     csrf = None
 #
```

### Comparing `iommi-7.0.0/iommi/_web_compat_flask.py` & `iommi-7.1.0/iommi/_web_compat_flask.py`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/action.py` & `iommi-7.1.0/iommi/action.py`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/admin.py` & `iommi-7.1.0/iommi/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
     path,
     reverse,
 )
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext
 
 from iommi import (
-    EditTable,
     LAST,
+    EditTable,
     Field,
     Form,
     Fragment,
     Menu,
     MenuItem,
     Page,
     Table,
@@ -183,18 +183,17 @@
                 is_superuser__filter__include=True,
             ),
         ),
     )
     def __init__(self, parts, apps, **kwargs):
         # Validate apps params
         for k in apps.keys():
-            assert (
-                k in joined_app_name_and_model
-            ), f'{k} is not a valid app/model key.\n\n' f'Valid keys:\n    ' + '\n    '.join(
-                sorted(joined_app_name_and_model)
+            assert k in joined_app_name_and_model, (
+                f'{k} is not a valid app/model key.\n\n'
+                f'Valid keys:\n    ' + '\n    '.join(sorted(joined_app_name_and_model))
             )
         super(Admin, self).__init__(parts=parts, apps=apps, **kwargs)
 
     def refine_with_params(self, app_name: str = None, model_name: str = None, pk: str = None):
         refined_admin = self.refine(app_name=app_name, model_name=model_name)
 
         model = django_apps.all_models[app_name][model_name] if app_name and model_name else None
@@ -346,30 +345,32 @@
                         key=key,
                     )
 
         table = setdefaults_path(
             Namespace(),
             table if table is not None else {},
             title=gettext('All models'),
-            call_target__cls=cls.get_meta().table_class,
+            call_target__cls=Table,
             call_target__attribute='div',
             sortable=False,
             rows=rows,
             page_size=None,
             columns__name=dict(
                 cell__url=lambda row, **_: row.url if getattr(row, 'pk', None) != '#sentinel#' else None,
                 display_name='',
-                cell__format=lambda row, **format_kwargs: row.format(row=row, **format_kwargs) if getattr(row, 'pk', None) != '#sentinel#' else '',
+                cell__format=lambda row, **format_kwargs: (
+                    row.format(row=row, **format_kwargs) if getattr(row, 'pk', None) != '#sentinel#' else ''
+                ),
             ),
         )
 
         add_models = setdefaults_path(
             Namespace(),
             include=settings.DEBUG,
-            call_target__cls=cls.get_meta().table_class,
+            call_target__cls=Table,
             sortable=False,
             rows=functools.partial(rows, included_filter=True),
             page_size=None,
             columns__conf=(
                 cls.get_meta()
                 .table_class.get_meta()
                 .member_class(
@@ -390,15 +391,17 @@
                     ),
                     # cell__url=lambda row, **_: f'{row.url}add_model/' if row.key else None,
                     after=LAST,
                 )
             ),
             columns__name=dict(
                 display_name='',
-                cell__format=lambda row, **format_kwargs: row.format(row=row, **format_kwargs) if getattr(row, 'pk', None) != '#sentinel#' else '',
+                cell__format=lambda row, **format_kwargs: (
+                    row.format(row=row, **format_kwargs) if getattr(row, 'pk', None) != '#sentinel#' else ''
+                ),
             ),
         )
 
         return cls(
             parts=dict(
                 all_models=table,
                 add_models_title=html.h1(gettext('Add models to admin'), include=settings.DEBUG),
@@ -423,15 +426,14 @@
     )
     def list(cls, table=None, **kwargs):
         table = setdefaults_path(
             Namespace(),
             table if table is not None else {},
             call_target__cls=cls.get_meta().table_class,
             columns=dict(
-                select__include=True,
                 edit=dict(
                     call_target__attribute='edit',
                     after=0,
                     cell__url=lambda row, **_: '%s/edit/' % row.pk,
                 ),
                 delete=dict(
                     call_target__attribute='delete',
@@ -447,17 +449,14 @@
                     display_name=lambda page, **_: (
                         gettext('Create %(model_name)s') % dict(model_name=page.model._meta.verbose_name)
                     ),
                     attrs__href='create/',
                 ),
             ),
             query_from_indexes=True,
-            bulk__actions__delete__include=lambda request, table, **_: (
-                cls.has_permission(request, instance=None, model=table.model, operation='delete')
-            ),
         )
 
         return cls(
             parts__header__children__link__attrs__href='../..',
             parts__table=table,
             **kwargs,
         )
```

### Comparing `iommi-7.0.0/iommi/apps.py` & `iommi-7.1.0/iommi/apps.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,9 +45,10 @@
 
         from django.contrib.contenttypes.fields import (
             GenericForeignKey,
             GenericRelation,
         )
 
         from iommi import register_factory
+
         register_factory(GenericRelation, factory=None)
         register_factory(GenericForeignKey, factory=None)
```

### Comparing `iommi-7.0.0/iommi/asset.py` & `iommi-7.1.0/iommi/asset.py`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/attrs.py` & `iommi-7.1.0/iommi/attrs.py`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/base.py` & `iommi-7.1.0/iommi/base.py`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/datetime_parsing.py` & `iommi-7.1.0/iommi/datetime_parsing.py`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/debug.py` & `iommi-7.1.0/iommi/debug.py`

 * *Files 4% similar despite different names*

```diff
@@ -168,42 +168,53 @@
 
     return TreeTable(rows=rows(root)).bind(request=request)
 
 
 def endpoint__debug_templates_used(endpoint, request, **_):
     root = endpoint.iommi_root()
     from iommi.part import render_root
+
     render_root(part=root)
 
     def url_for_template(t):
         if isinstance(t, str):
             t = get_template(t).origin.name
         else:
             t = t.origin.name
 
         return local_debug_url_builder(t, 1)
 
     links = [
-        format_html('<li><a href="{}">{}</a></li>', url_for_template(t), t)
+        format_html(
+            '<li><a href="{}">{}</a></li>',
+            url_for_template(t),
+            t,
+        )
         for t in request.iommi_used_templates
     ]
     links = format_html('{}' * len(links), *links)
-    return HttpResponse(format_html('''
-        <html>
-            <head>
-                <style>
-                </style>
-            </head>
-            <body>
-                <ul>
-                    {}
-                </ul>
-            </body>
-        </html>
-        ''', links))
+    return HttpResponse(
+        # language=HTML
+        format_html(
+            '''
+                <html>
+                    <head>
+                        <style>
+                        </style>
+                    </head>
+                    <body>
+                        <ul>
+                            {}
+                        </ul>
+                    </body>
+                </html>
+            ''',
+            links,
+        )
+    )
 
 
 def local_debug_url_builder(filename, lineno):
     if not isabs(filename):
         filename = join(settings.BASE_DIR, filename)
     if hasattr(settings, 'IOMMI_DEBUG_URL_MAPPING'):
         filename = filename.replace(*settings.IOMMI_DEBUG_URL_MAPPING)
```

### Comparing `iommi-7.0.0/iommi/declarative/.DS_Store` & `iommi-7.1.0/iommi/declarative/.DS_Store`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/declarative/__init__.py` & `iommi-7.1.0/iommi/declarative/__init__.py`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/declarative/dispatch.py` & `iommi-7.1.0/iommi/declarative/dispatch.py`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/declarative/namespace.py` & `iommi-7.1.0/iommi/declarative/namespace.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,24 +81,20 @@
                 else:
                     self[key] = value
             else:
                 self[key] = value
 
     def __repr__(self):
         # Note: `repr` is called on any values in the namespace
-        flattened_key_value_pairs = ", ".join(
-            f'{k}={v!r}' for k, v in sorted(flatten_items(self), key=lambda x: x[0])
-        )
+        flattened_key_value_pairs = ", ".join(f'{k}={v!r}' for k, v in sorted(flatten_items(self), key=lambda x: x[0]))
         return f"{type(self).__name__}({flattened_key_value_pairs})"
 
     def __str__(self):
         # Note: `str` is called on any values in the namespace
-        flattened_key_value_pairs = ", ".join(
-            f'{k}={v}' for k, v in sorted(flatten_items(self), key=lambda x: x[0])
-        )
+        flattened_key_value_pairs = ", ".join(f'{k}={v}' for k, v in sorted(flatten_items(self), key=lambda x: x[0]))
         return "{}({})".format(type(self).__name__, flattened_key_value_pairs)
 
     def __call__(self, *args, **kwargs):
         params = Namespace(self, kwargs)
 
         try:
             call_target = params.pop('call_target')
```

### Comparing `iommi-7.0.0/iommi/declarative/util.py` & `iommi-7.1.0/iommi/declarative/util.py`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/declarative/with_meta.py` & `iommi-7.1.0/iommi/declarative/with_meta.py`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/docs.py` & `iommi-7.1.0/iommi/docs.py`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/edit_table.py` & `iommi-7.1.0/iommi/edit_table.py`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/endpoint.py` & `iommi-7.1.0/iommi/endpoint.py`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/error.py` & `iommi-7.1.0/iommi/error.py`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/evaluate.py` & `iommi-7.1.0/iommi/evaluate.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,17 +30,17 @@
         result = False  # Special case to not match no-specification function "lambda **whatever: ..."
     else:
         if wildcard:
             result = caller >= required
         else:
             result = required <= caller <= required.union(optional)
 
-    _matches_cache[
-        cache_key
-    ] = result  # pragma: no mutate (mutation changes result to None which just makes things slower)
+    _matches_cache[cache_key] = (
+        result  # pragma: no mutate (mutation changes result to None which just makes things slower)
+    )
     return result
 
 
 def get_callable_description(c):
     if getattr(c, '__name__', None) == '<lambda>':
         import inspect
```

### Comparing `iommi-7.0.0/iommi/experimental/.DS_Store` & `iommi-7.1.0/iommi/experimental/.DS_Store`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/form.py` & `iommi-7.1.0/iommi/form.py`

 * *Files 0% similar despite different names*

```diff
@@ -1256,17 +1256,15 @@
     def choice_queryset(cls, choices: QuerySet = None, **kwargs):
         if 'model' not in kwargs:
             if isinstance(choices, QuerySet):
                 kwargs['model'] = choices.model
             elif 'model_field' in kwargs:
                 pass
             else:
-                assert (
-                    False
-                ), 'The convenience feature to automatically get the parameter model set only works for QuerySet instances or if you specify model_field'
+                assert False, 'The convenience feature to automatically get the parameter model set only works for QuerySet instances or if you specify model_field'
 
         instance = cls.choice(**kwargs)
         instance = instance.refine(
             Prio.shortcut,
             choices=(
                 (lambda form, **_: choices.all()) if isinstance(choices, QuerySet) else choices
             ),  # clone the QuerySet if needed
@@ -1472,20 +1470,15 @@
 
 def is_django_promise_with_string_proxy(redirect_to):
     if not isinstance(redirect_to, Promise):
         return False
     # django 5.0+ uses _kw and _args
     kwargs = getattr(redirect_to, '_proxy____kw', getattr(redirect_to, '_kw', None))
     args = getattr(redirect_to, '_proxy____args', getattr(redirect_to, '_args', None))
-    return (
-        isinstance(redirect_to, Promise)
-        and kwargs == {}
-        and len(args) == 1
-        and isinstance(args[0], str)
-    )
+    return isinstance(redirect_to, Promise) and kwargs == {} and len(args) == 1 and isinstance(args[0], str)
 
 
 def create_or_edit_object_redirect(is_create, redirect_to, redirect, form):
     assert (
         redirect_to is None or isinstance(redirect_to, str) or is_django_promise_with_string_proxy(redirect_to)
     ), 'redirect_to must be a str'
     if redirect_to is None:
@@ -1690,17 +1683,15 @@
             **kwargs,
         )
 
     def on_refine_done(self):
         extra_member_defaults = dict()
         if self.auto:
             auto = FormAutoConfig(**self.auto).refine_done(parent=self)
-            assert (
-                not self.model
-            ), "You can't use the auto feature and explicitly pass model. Either pass auto__model, or we will set the model for you from auto__instance"
+            assert not self.model, "You can't use the auto feature and explicitly pass model. Either pass auto__model, or we will set the model for you from auto__instance"
             if auto.model is None:
                 auto.model = auto.instance.__class__
 
             model, fields_from_auto = self._from_model(
                 model=auto.model,
                 include=auto.include,
                 exclude=auto.exclude,
```

### Comparing `iommi-7.0.0/iommi/fragment.py` & `iommi-7.1.0/iommi/fragment.py`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/from_model.py` & `iommi-7.1.0/iommi/from_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,23 @@
 from typing import (
     Dict,
     List,
     Type,
 )
 
 from django.core.exceptions import FieldDoesNotExist
-from django.db.models import (
-    Field as DjangoField,
-)
+from django.db.models import Field as DjangoField
 from django.db.models import (
     ManyToManyRel,
     ManyToOneRel,
     Model,
     OneToOneRel,
 )
 
-from iommi.base import (
-    MISSING,
-)
+from iommi.base import MISSING
 from iommi.declarative.dispatch import dispatch
 from iommi.declarative.namespace import (
     Namespace,
     setdefaults_path,
 )
 from iommi.evaluate import evaluate
 from iommi.refinable import (
@@ -159,18 +155,15 @@
         kwargs.update(**defaults)
 
     return factory(model_field=model_field, model_field_name=model_field_name, model=model, **kwargs)
 
 
 def get_field_by_name(model: Type[Model]) -> Dict[str, DjangoField]:
     if not hasattr(model._meta, '_iommi_fields'):
-        model._meta._iommi_fields = {
-            get_field_name(field): field
-            for field in model._meta.get_fields()
-        }
+        model._meta._iommi_fields = {get_field_name(field): field for field in model._meta.get_fields()}
         if None in model._meta._iommi_fields:
             model._meta._iommi_fields.pop(None)
     return model._meta._iommi_fields
 
 
 def get_field_name(field: DjangoField) -> str:
     if isinstance(field, ManyToManyRel):
@@ -192,15 +185,17 @@
     if field_name == 'pk':
         return model._meta.auto_field
 
     try:
         return get_field_by_name(model)[field_name]
     except KeyError:
         valid_names = '\n    '.join(sorted(get_field_by_name(model).keys()))
-        raise FieldDoesNotExist(f"{model._meta.object_name} has no field with name '{field_name}', valid names are:\n\n    {valid_names}")
+        raise FieldDoesNotExist(
+            f"{model._meta.object_name} has no field with name '{field_name}', valid names are:\n\n    {valid_names}"
+        )
 
 
 def get_field_path(model, path):
     def _get_field_path(current_model, sub_path):
         first, _, rest = sub_path.partition('__')
         field = get_field(current_model, first)
         if not rest:
@@ -219,18 +214,15 @@
         prefix = []
         current_model = model
         for part in missing_path.split('__'):
             try:
                 current_model = get_field(current_model, part).remote_field.model
             except FieldDoesNotExist:
                 return sorted(
-                    [
-                        '__'.join(prefix + [name])
-                        for name in get_field_by_name(current_model).keys()
-                    ]
+                    ['__'.join(prefix + [name]) for name in get_field_by_name(current_model).keys()]
                     + ['__'.join(prefix + ['pk'])]
                 )
             else:
                 prefix.append(part)
 
     if paths:
         for path in paths:
```

### Comparing `iommi-7.0.0/iommi/live_edit.py` & `iommi-7.1.0/iommi/live_edit.py`

 * *Files 0% similar despite different names*

```diff
@@ -298,14 +298,15 @@
                 integrity='sha512-GZ1RIgZaSc8rnco/8CXfRdCpDxRCphenIiZ2ztLy3XQfCbQUSCuk8IudvNHxkRA3oUg6q0qejgN/qqyG1duv5Q==',
                 crossorigin='anonymous',
             ),
             after=-1,
         ),
         assets__live_edit_page_custom=Asset(
             tag='style',
+            # language=css
             text='''
                 .container {
                     padding: 0 !important;
                     margin: 0 !important;
                     max-width: 100%;
                 }
 
@@ -333,17 +334,15 @@
                 #editor {
                     height: 90% !important;
                 }
 
                 #error {
                     height: 10% !important;
                 }
-            '''.replace(
-                '<<flow_direction>>', flow_direction
-            ),
+            '''.replace('<<flow_direction>>', flow_direction),
         ),
         iommi_style='bootstrap',
         parts__result=html.iframe(attrs__id='result'),
         parts__editor_and_error=html.div(
             attrs__id='editor_and_error',
             children=dict(
                 editor=html.div(
```

### Comparing `iommi-7.0.0/iommi/locale/.DS_Store` & `iommi-7.1.0/iommi/locale/.DS_Store`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/locale/cs/LC_MESSAGES/django.mo` & `iommi-7.1.0/iommi/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/locale/cs/LC_MESSAGES/django.po` & `iommi-7.1.0/iommi/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/locale/de/.DS_Store` & `iommi-7.1.0/iommi/locale/de/.DS_Store`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/locale/de/LC_MESSAGES/django.mo` & `iommi-7.1.0/iommi/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/locale/de/LC_MESSAGES/django.po` & `iommi-7.1.0/iommi/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/locale/sv/.DS_Store` & `iommi-7.1.0/iommi/locale/sv/.DS_Store`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/locale/sv/LC_MESSAGES/django.mo` & `iommi-7.1.0/iommi/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/locale/sv/LC_MESSAGES/django.po` & `iommi-7.1.0/iommi/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/locale/uk/LC_MESSAGES/django.mo` & `iommi-7.1.0/iommi/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/locale/uk/LC_MESSAGES/django.po` & `iommi-7.1.0/iommi/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/locale/zh_Hans/LC_MESSAGES/django.mo` & `iommi-7.1.0/iommi/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/locale/zh_Hans/LC_MESSAGES/django.po` & `iommi-7.1.0/iommi/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/member.py` & `iommi-7.1.0/iommi/member.py`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/menu.py` & `iommi-7.1.0/iommi/menu.py`

 * *Files 2% similar despite different names*

```diff
@@ -304,24 +304,42 @@
 
         if current:
             current._active = True
 
 
 def get_debug_menu(**kwargs):
     class DebugMenu(Menu):
-        code = MenuItem(tag='li')
-        templates = MenuItem(url='?/debug_templates_used', tag='li', include=lambda request, **_: getattr(request, 'iommi_used_templates', None))
-        tree = MenuItem(url='?/debug_tree', tag='li')
-        pick = MenuItem(url='#', attrs__onclick='window.iommi_start_pick()', tag='li')
+        code = MenuItem(
+            tag='li',
+        )
+        templates = MenuItem(
+            url='?/debug_templates_used',
+            tag='li',
+            include=lambda request, **_: getattr(request, 'iommi_used_templates', None),
+        )
+        tree = MenuItem(
+            url='?/debug_tree',
+            tag='li',
+        )
+        pick = MenuItem(
+            url='#',
+            attrs__onclick='window.iommi_start_pick()',
+            tag='li',
+        )
         edit = MenuItem(
-            display_name=lambda request, **_: 'Edit vertical'
-            if request.GET.get('_iommi_live_edit') is not None and request.GET.get('_iommi_live_edit_flow') != 'row' else 'Edit',
-            url=lambda request, **_: '?_iommi_live_edit&_iommi_live_edit_flow=row'
-            if request.GET.get('_iommi_live_edit') is not None and request.GET.get('_iommi_live_edit_flow') != 'row'
-            else '?_iommi_live_edit',
+            display_name=lambda request, **_: (
+                'Edit vertical'
+                if request.GET.get('_iommi_live_edit') is not None and request.GET.get('_iommi_live_edit_flow') != 'row'
+                else 'Edit'
+            ),
+            url=lambda request, **_: (
+                '?_iommi_live_edit&_iommi_live_edit_flow=row'
+                if request.GET.get('_iommi_live_edit') is not None and request.GET.get('_iommi_live_edit_flow') != 'row'
+                else '?_iommi_live_edit'
+            ),
             tag='li',
             include=lambda **_: 'iommi.live_edit.Middleware' in settings.MIDDLEWARE,
         )
         stop_editing = MenuItem(
             display_name='Stop editing',
             url='?_iommi_live_edit=stop',
             tag='li',
@@ -329,27 +347,29 @@
         )
         edit_style = MenuItem(
             url='?_iommi_live_edit=style_editor',
             tag='li',
             include=lambda **_: 'iommi.live_edit.Middleware' in settings.MIDDLEWARE,
         )
         profile = MenuItem(
-            url='?_iommi_prof', tag='li', include=lambda **_: 'iommi.profiling.Middleware' in settings.MIDDLEWARE
+            url='?_iommi_prof',
+            tag='li',
+            include=lambda **_: 'iommi.profiling.Middleware' in settings.MIDDLEWARE,
         )
         profile_post = MenuItem(
             display_name='Profile POST',
             url='#',
             # language=js
             attrs__onclick="""
-            for (form of document.querySelectorAll('form')) {
-                var input = document.createElement("input");
-                input.setAttribute("type", "hidden");
-                input.setAttribute("name", "_iommi_prof");
-                form.appendChild(input);
-            }
+                for (form of document.querySelectorAll('form')) {
+                    var input = document.createElement("input");
+                    input.setAttribute("type", "hidden");
+                    input.setAttribute("name", "_iommi_prof");
+                    form.appendChild(input);
+                }
             """,
             tag='li',
             include=lambda **_: 'iommi.profiling.Middleware' in settings.MIDDLEWARE,
         )
         sql_trace = MenuItem(
             display_name='SQL trace',
             url='?_iommi_sql_trace',
```

### Comparing `iommi-7.0.0/iommi/page.py` & `iommi-7.1.0/iommi/page.py`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/part.py` & `iommi-7.1.0/iommi/part.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,20 +38,16 @@
     perform_post_dispatch,
 )
 from iommi.member import (
     bind_members,
     refine_done_members,
 )
 from iommi.shortcut import with_defaults
-from iommi.style import (
-    get_style_object,
-)
-from iommi.traversable import (
-    Traversable,
-)
+from iommi.style import get_style_object
+from iommi.traversable import Traversable
 
 from ._web_compat import (
     QueryDict,
     settings,
     template_types,
 )
 from .refinable import (
@@ -230,17 +226,15 @@
     request = part.get_request()
 
     context = dict(
         container=Container(_name='Container').refine_done(parent=part).bind(parent=part),
         content=content,
         title=title if title not in (None, MISSING) else '',
         iommi_debug_panel=(
-            iommi_debug_panel(part)
-            if iommi_debug_on() and '_iommi_disable_debug_panel' not in request.GET
-            else ''
+            iommi_debug_panel(part) if iommi_debug_on() and '_iommi_disable_debug_panel' not in request.GET else ''
         ),
         iommi_language_code=getattr(request, 'LANGUAGE_CODE', settings.LANGUAGE_CODE),
         assets=assets,
         **(part.context if isinstance(part, Page) else {}),
         **context,
     )
```

### Comparing `iommi-7.0.0/iommi/path.py` & `iommi-7.1.0/iommi/path.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,25 +28,31 @@
         else:
             return self._decode(lookup=lookup, string=string, model=model, **kwargs)
 
 
 class PathDecoder:
     def __init__(self, *, decode=None, model=None, name):
         if decode is None:
+
             def decode(string, _model=model, **_):
                 return _model.objects.get(pk=string)
 
         self.decode = decode
         self.model = model
         self.name = name
 
 
 _path_component_to_decode_data: typing.Dict[
     str,
-    typing.Tuple[typing.Optional[typing.Type[Model]], str, typing.Optional[str], typing.Union[Decoder, PathDecoder]],
+    typing.Tuple[
+        typing.Optional[typing.Type[Model]],
+        str,
+        typing.Optional[str],
+        typing.Union[Decoder, PathDecoder],
+    ],
 ] = {}
 
 
 _default_decoder = Decoder('pk', 'name')
 
 
 def camel_to_snake(s):
```

### Comparing `iommi-7.0.0/iommi/profiling.py` & `iommi-7.1.0/iommi/profiling.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,41 +33,47 @@
     return None
 
 
 def should_profile(request):
     disabled = getattr(request, 'profiler_disabled', True)
     is_staff = hasattr(request, 'user') and request.user.is_staff
 
-    return ('_iommi_prof' in request.GET or '_iommi_prof' in request.POST) and ((not disabled and is_staff) or settings.DEBUG)
+    return ('_iommi_prof' in request.GET or '_iommi_prof' in request.POST) and (
+        (not disabled and is_staff) or settings.DEBUG
+    )
 
 
 def strip_extra_path(s, token):
     if token not in s:
         return s
     pre, _, post = s.rpartition(' ')
     post = post[post.rindex(token) + len(token) :]
     return f'{pre} {post}'
 
 
 class HTMLStats(pstats.Stats):
     def print_title(self):
-        print('''
-            <thead>
-                <tr>
-                    <th class="numeric"><a href="?_iommi_prof=ncalls">ncalls</a></th>
-                    <th class="numeric"><a href="?_iommi_prof=tottime">tottime</a></th>
-                    <th class="numeric">percall</th>
-                    <th class="numeric"><a href="?_iommi_prof=cumtime">cumtime</a></th>
-                    <th class="numeric">percall</th>
-                    <th>function</th>
-                    <th>filename</th>
-                    <th>lineno</th>
-                </tr>
-            </thead>
-        ''', file=self.stream)
+        print(
+            # language=HTML
+            '''
+                <thead>
+                    <tr>
+                        <th class="numeric"><a href="?_iommi_prof=ncalls">ncalls</a></th>
+                        <th class="numeric"><a href="?_iommi_prof=tottime">tottime</a></th>
+                        <th class="numeric">percall</th>
+                        <th class="numeric"><a href="?_iommi_prof=cumtime">cumtime</a></th>
+                        <th class="numeric">percall</th>
+                        <th>function</th>
+                        <th>filename</th>
+                        <th>lineno</th>
+                    </tr>
+                </thead>
+            ''',
+            file=self.stream,
+        )
 
     def print_stats(self, *amount):
         for filename in self.files:
             print(filename, file=self.stream)
         if self.files:
             print(file=self.stream)
         indent = ' ' * 8
@@ -125,15 +131,18 @@
         print(f'<td class="numeric">{f8(ct)}</td>', file=self.stream)
         if cc == 0:
             print('<td></td>', file=self.stream)
         else:
             print(f'<td class="numeric">{f8(ct/cc)}</td>', file=self.stream)
 
         if line_number and path:
-            print(f'<td><a href="{src_debug_url_builder(path, line_number)}">{escape(function_name)}</a></td>', file=self.stream)
+            print(
+                f'<td><a href="{src_debug_url_builder(path, line_number)}">{escape(function_name)}</a></td>',
+                file=self.stream,
+            )
         else:
             print(f'<td>{escape(function_name)}</td>', file=self.stream)
 
         print(f'<td>{nice_path}</td>', file=self.stream)
         print(f'<td class="numeric">{line_number}</td>', file=self.stream)
         print('</tr>', file=self.stream)
 
@@ -166,15 +175,14 @@
                 for line in response.streaming_content:
                     print(line.decode(), file=sys.__stdout__)
 
             response = HttpResponse()
             for prof in request._iommi_prof:
                 prof.disable()
 
-
             s = StringIO()
             ps = HTMLStats(*request._iommi_prof, stream=s)
 
             prof_command = request.GET.get('_iommi_prof')
 
             if prof_command == 'graph':
                 with NamedTemporaryFile() as stats_dump:
@@ -184,15 +192,14 @@
                     gprof2dot_path = Path(sys.executable).parent / 'gprof2dot'
                     if not gprof2dot_path.exists():
                         raise Exception('gprof2dot not found. Please install it to use the graph feature.')
 
                     with subprocess.Popen(
                         (sys.executable, gprof2dot_path, '-f', 'pstats', stats_dump.name), stdout=subprocess.PIPE
                     ) as gprof2dot:
-
                         response['Content-Type'] = 'image/svg+xml'
 
                         dot_path = get_dot_path()
                         if dot_path:
                             response.content = subprocess.check_output((dot_path, '-Tsvg'), stdin=gprof2dot.stdout)
                         else:
                             response['Content-Type'] = 'text/plain'
```

### Comparing `iommi-7.0.0/iommi/query.py` & `iommi-7.1.0/iommi/query.py`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/refinable.py` & `iommi-7.1.0/iommi/refinable.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,25 +159,28 @@
         _get_evaluated_attributes_cache[class_] = r
         return r
 
 
 class SpecialEvaluatedRefinable(Refinable):
     pass
 
+
 def special_evaluated_refinable(f):
     f = refinable(f)
     f.__iommi__special_evaluated = True
     return f
 
+
 def is_special_evaluated_refinable(x):
     return isinstance(x, SpecialEvaluatedRefinable) or getattr(x, '__iommi__special_evaluated', False)
 
 
 _get_special_evaluated_attributes_cache = {}
 
+
 def get_special_evaluated_attributes(result):
     class_ = type(result)
     try:
         return _get_special_evaluated_attributes_cache[class_]
     except KeyError:
         r = [k for k, v in items(result.get_declared('refinable')) if is_special_evaluated_refinable(v)]
         _get_special_evaluated_attributes_cache[class_] = r
```

### Comparing `iommi-7.0.0/iommi/shortcut.py` & `iommi-7.1.0/iommi/shortcut.py`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/sort_after.py` & `iommi-7.1.0/iommi/sort_after.py`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/sql_trace.py` & `iommi-7.1.0/iommi/sql_trace.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     set_current_request,
 )
 
 
 def no_coloring(text, color=None, on_color=None, attrs=None):
     return text
 
+
 try:
     from termcolor import colored
 except ImportError:
     colored = no_coloring
 
 
 log = logging.getLogger('db')
@@ -114,28 +115,29 @@
                 return response
 
             if sql_trace is not None:
                 iommi_sql_debug_log = getattr(request, 'iommi_sql_debug_log', None)
                 if iommi_sql_debug_log is not None:
                     total_duration = float(sum(x['duration'] for x in iommi_sql_debug_log))
                     result = [
+                        # language=HTML
                         '''
-                        <style>
-                            a, span {
-                                box-sizing: border-box;
-                            }
-                            @media (prefers-color-scheme: dark) {
-                                html {
-                                    background-color: black;
-                                    color: #bbb;
+                            <style>
+                                a, span {
+                                    box-sizing: border-box;
                                 }
-                                b {
-                                    color: white;
+                                @media (prefers-color-scheme: dark) {
+                                    html {
+                                        background-color: black;
+                                        color: #bbb;
+                                    }
+                                    b {
+                                        color: white;
+                                    }
                                 }
-                            }
                             </style>
                         ''',
                         f'{len(iommi_sql_debug_log)} queries, {total_duration:.3} seconds total<br><br>',
                     ]
 
                     if total_duration:
                         color = '#4f4fff'
```

### Comparing `iommi-7.0.0/iommi/static/.DS_Store` & `iommi-7.1.0/iommi/static/.DS_Store`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/static/js/iommi.js` & `iommi-7.1.0/iommi/static/js/iommi.js`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/struct.py` & `iommi-7.1.0/iommi/struct.py`

 * *Files 12% similar despite different names*

```diff
@@ -74,33 +74,33 @@
             _hash = dict.__getattribute__(self, hash_key)
         except AttributeError:
             _hash = hash(tuple((k, self[k]) for k in sorted(self.keys())))
             dict.__setattr__(self, hash_key, _hash)
         return _hash
 
     def __setitem__(self, *_, **__):
-        raise TypeError("'{}' object attributes are read-only".format(type(self).__name__, ))
+        raise TypeError(f"'{type(self).__name__}' object attributes are read-only")
 
     def __setattr__(self, key, value):
-        raise TypeError("'{}' object attributes are read-only".format(type(self).__name__, ))
+        raise TypeError(f"'{type(self).__name__}' object attributes are read-only")
 
     def setdefault(self, *_, **__):
-        raise TypeError("'{}' object attributes are read-only".format(type(self).__name__, ))
+        raise TypeError(f"'{type(self).__name__}' object attributes are read-only")
 
     def update(self, *_, **__):
-        raise TypeError("'{}' object attributes are read-only".format(type(self).__name__, ))
+        raise TypeError(f"'{type(self).__name__}' object attributes are read-only")
 
     def clear(self, *_, **__):
-        raise TypeError("'{}' object attributes are read-only".format(type(self).__name__, ))
+        raise TypeError(f"'{type(self).__name__}' object attributes are read-only")
 
     def __delitem__(self, *_, **__):
-        raise TypeError("'{}' object attributes are read-only".format(type(self).__name__, ))
+        raise TypeError(f"'{type(self).__name__}' object attributes are read-only")
 
     def __delattr__(self, *_, **__):
-        raise TypeError("'{}' object attributes are read-only".format(type(self).__name__, ))
+        raise TypeError(f"'{type(self).__name__}' object attributes are read-only")
 
     def __reduce__(self):
         return type(self), (), dict(self)
 
     def __setstate__(self, state):
         dict.update(self, state)
```

### Comparing `iommi-7.0.0/iommi/style.py` & `iommi-7.1.0/iommi/style.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,16 +107,18 @@
                         sub_style_bases.append(sub_style_base)
                 self.sub_styles[k] = Style(*sub_style_bases, **v)
 
         for name, sub_style in items(self.sub_styles):
             sub_style.name = name
 
         from iommi.debug import iommi_debug_on
+
         if iommi_debug_on():
             import inspect
+
             self._instantiated_at_frame = inspect.currentframe().f_back
 
     def resolve(self, obj, is_root=False):
         """
         Calculate the namespaces of additional argument that should be applied
         to the given object. If is_root is set to True, assets might also be
         added to the namespace.
```

### Comparing `iommi-7.0.0/iommi/style_base.py` & `iommi-7.1.0/iommi/style_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,19 @@
             ),
             iommi_js=Asset.js(
                 attrs=dict(
                     src=lambda **_: static('js/iommi.js'),
                 ),
             ),
             iommi_js_init=iommi_js_init,
-            meta=Asset(mark_safe('''<meta content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no" name="viewport">'''))
+            meta=Asset(
+                mark_safe(
+                    '''<meta content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no" name="viewport">'''
+                )
+            ),
         ),
     ),
     Form=dict(
         shortcuts=dict(
             edit__actions__submit__display_name=gettext_lazy('Save'),
             create__actions__submit__display_name=gettext_lazy('Create'),
             delete__actions__submit__display_name=gettext_lazy('Delete'),
```

#### html2text {}

```diff
@@ -22,16 +22,16 @@
 ( endpoints__debug_tree=dict( include=lambda endpoint, **_: iommi_debug_on(),
 func=endpoint__debug_tree, ), endpoints__debug_templates_used=dict
 ( include=lambda endpoint, **_: iommi_debug_on(),
 func=endpoint__debug_templates_used, ), assets=dict( jquery=Asset.js
 ( attrs=dict( src='https://code.jquery.com/jquery-3.4.1.js', integrity='sha256-
 WpOohJOqMqqyKL9FccASB9O0KwACQJpFTUBLTYOVvVU=', crossorigin='anonymous', ),
 after=-1, ), iommi_js=Asset.js( attrs=dict( src=lambda **_: static('js/
-iommi.js'), ), ), iommi_js_init=iommi_js_init, meta=Asset(mark_safe('''
-''')) ), ), Form=dict( shortcuts=dict
+iommi.js'), ), ), iommi_js_init=iommi_js_init, meta=Asset( mark_safe( '''
+''' ) ), ), ), Form=dict( shortcuts=dict
 ( edit__actions__submit__display_name=gettext_lazy('Save'),
 create__actions__submit__display_name=gettext_lazy('Create'),
 delete__actions__submit__display_name=gettext_lazy('Delete'), ), ), Field=dict
 ( shortcuts=dict( boolean=dict( input__after=0, input__attrs__type='checkbox',
 ), choice=dict( input__template='iommi/form/choice.html',
 input__attrs__value=None, input__attrs__type=None, ),
 date__input__attrs__type='date', radio=dict( input__template='iommi/form/
```

### Comparing `iommi-7.0.0/iommi/style_bootstrap.py` & `iommi-7.1.0/iommi/style_bootstrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,19 +98,22 @@
             'form-text': True,
             'text-muted': True,
         },
     ),
     FieldGroup=dict(
         tag='div',
         attrs__class={'form-row': True},
-        assets__field_group_select2_css=Asset('''
+        assets__field_group_select2_css=Asset(
+            '''
         .form-group .select2-container {
             display: block;
         }
-        ''', tag='style'),
+        ''',
+            tag='style',
+        ),
     ),
     Action=dict(
         shortcuts=dict(
             # In bootstrap one must choose a button style (secondary, success, ...)
             # otherwise the styling is roughly identical to text.
             button__attrs__class={
                 'btn': True,
@@ -133,14 +136,15 @@
     Column=dict(
         header__attrs__class={'text-nowrap': True},
         shortcuts=dict(
             select=dict(
                 header__attrs__title='Select all',
                 header__attrs__class={'text-center': True},
                 cell__attrs__class={'text-center': True},
+                extra__icon='fa fa-check-square-o',
             ),
             number=dict(
                 cell__attrs__class={'text-right': True},
                 header__attrs__class={'text-right': True},
             ),
             boolean__cell__attrs__class={'text-center': True},
             delete=dict(
```

### Comparing `iommi-7.0.0/iommi/style_bootstrap5.py` & `iommi-7.1.0/iommi/style_bootstrap5.py`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/style_bootstrap_docs.py` & `iommi-7.1.0/iommi/style_bootstrap_docs.py`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/style_bootstrap_icons.py` & `iommi-7.1.0/iommi/style_bootstrap_icons.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,10 +15,15 @@
             icon_prefix='bi-',
         ),
         edit__extra__icon='pencil-square',
         delete__extra__icon='trash',
         download__extra__icon='download',
         boolean__cell__format=lambda value, **_: mark_safe(
             f'<i class="bi bi-check-lg fs-3" title="{gettext("Yes")}"></i>'
-        ) if value else '',
+        )
+        if value
+        else '',
+        select=dict(
+            extra__icon='bi bi-check2-square',
+        ),
     ),
 )
```

### Comparing `iommi-7.0.0/iommi/style_bulma.py` & `iommi-7.1.0/iommi/style_bulma.py`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/style_django_admin.py` & `iommi-7.1.0/iommi/style_django_admin.py`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/style_font_awesome_4.py` & `iommi-7.1.0/iommi/style_font_awesome_4.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,12 +13,12 @@
         icon__extra=dict(
             icon_attrs__class={'fa': True, 'fa-lg': True},
             icon_prefix='fa-',
         ),
         edit__extra__icon='pencil-square-o',
         delete__extra__icon='trash-o',
         download__extra__icon='download',
-        boolean__cell__format=lambda value, **_: mark_safe(
-            f'<i class="fa fa-check" title="{gettext("Yes")}"></i>'
-        ) if value else '',
+        boolean__cell__format=lambda value, **_: mark_safe(f'<i class="fa fa-check" title="{gettext("Yes")}"></i>')
+        if value
+        else '',
     ),
 )
```

### Comparing `iommi-7.0.0/iommi/style_font_awesome_6.py` & `iommi-7.1.0/iommi/style_font_awesome_6.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext
 
 from iommi import (
-    html,
     Style,
+    html,
 )
 
 font_awesome_6 = Style(
     root__assets__icons=html.link(
         attrs__rel="stylesheet",
         attrs__href="https://cdn.jsdelivr.net/npm/@fortawesome/fontawesome-free@6.5.2/css/all.min.css",
     ),
@@ -15,12 +15,15 @@
         icon__extra=dict(
             icon_attrs__class={'fa': True, 'fa-lg': True},
             icon_prefix='fa-',
         ),
         edit__extra__icon='pencil-square-o',
         delete__extra__icon='trash-o',
         download__extra__icon='download',
-        boolean__cell__format=lambda value, **_: mark_safe(
-            f'<i class="fa fa-check" title="{gettext("Yes")}"></i>'
-        ) if value else '',
+        boolean__cell__format=lambda value, **_: (
+            mark_safe(f'<i class="fa fa-check" title="{gettext("Yes")}"></i>') if value else ''
+        ),
+        select=dict(
+            extra__icon='fa-regular fa-square-check',
+        ),
     ),
 )
```

### Comparing `iommi-7.0.0/iommi/style_foundation.py` & `iommi-7.1.0/iommi/style_foundation.py`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/style_semantic_ui.py` & `iommi-7.1.0/iommi/style_semantic_ui.py`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/style_test_base.py` & `iommi-7.1.0/iommi/style_test_base.py`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/style_uikit.py` & `iommi-7.1.0/iommi/style_uikit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from iommi.asset import Asset
 from iommi.style import Style
 from iommi.style_base import base
 
 uikit = Style(
     base,
     root__assets__css=Asset.css(
@@ -59,9 +58,9 @@
         container__tag='ul',
         item__tag='li',
         active_item=dict(
             tag='li',
             attrs__class={'uk-active': True},
         ),
         container__attrs__class={'uk-pagination': True},
-    )
+    ),
 )
```

### Comparing `iommi-7.0.0/iommi/synthetic_traceback.py` & `iommi-7.1.0/iommi/synthetic_traceback.py`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/table.py` & `iommi-7.1.0/iommi/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -454,17 +454,15 @@
         self.header = HeaderColumnConfig(**self.header).refine_done(parent=self)
         self.is_sorting: bool = None
         self.sort_direction: str = None
         self.table = None
         super(Column, self).on_refine_done()
 
     def __html__(self, *, render=None):
-        assert (
-            False
-        ), "This is implemented just to make linting happy that we've implemented all abstract methods. Don't call this!"  # pragma: no cover
+        assert False, "This is implemented just to make linting happy that we've implemented all abstract methods. Don't call this!"  # pragma: no cover
 
     @staticmethod
     @evaluated_refinable
     def sort_key(table, column, **_):
         return column.attr
 
     @staticmethod
@@ -660,32 +658,32 @@
         sortable=False,
         filter__is_valid_filter=lambda **_: (True, ''),
         filter__field__include=False,
         attr=None,
         cell__value=lambda table, cells, row, **_: (
             row.pk
             if isinstance(table.rows, QuerySet)
-            else
             # row_index is the visible row number
             # See selection() for the code that does the lookup
-            cells.row_index
+            else cells.row_index
         ),
         cell__format=lambda column, row, value, **kwargs: format_html(
             # language=HTML
             '<input type="checkbox" class="checkbox" name="{checkbox_name}_{row_id}" {checked_str} />',
             checkbox_name=column.extra.checkbox_name,
             row_id=value,
             checked_str=(
                 'checked'
                 if evaluate_strict(column.extra.checked, column=column, row=row, value=value, **kwargs)
                 else ''
             ),
         ),
         extra__checkbox_name='pk',
         extra__checked=lambda **_: False,
+        extra__icon='fa fa-check-square-o',
     )
     def select(cls, **kwargs):
         # language=rst
         """
         Shortcut for a column of checkboxes to select rows. This is useful for implementing bulk operations.
 
         By default tables have a column named `select` that is hidden that is used for this purpose, so you only
@@ -2163,16 +2161,18 @@
             self.rows = self.sorted_and_filtered_rows
 
     def _bind_bulk_form(self):
         if self.bulk is None:
             return
 
         bind_member(self, name='bulk')
-        if self.bulk is not None:
+        if self.should_render_form_tag():
             self._bound_members.bulk = self.bulk
+        else:
+            self.bulk = None
 
     # property for jinja2 compatibility
     @property
     def render_actions(self):
         assert self._is_bound, NOT_BOUND_MESSAGE
         non_grouped_actions, grouped_actions = group_actions(self.actions)
         return render_template(
@@ -2191,17 +2191,15 @@
         if auto_rowspan_columns:
             self.visible_rows = list(self.get_visible_rows())
             no_value_set = object()
             for column in auto_rowspan_columns:
                 if column.cell.attrs.get('rowspan', no_value_set) is not no_value_set:
                     continue
 
-                rowspan_by_row = (
-                    {}
-                )  # cells for rows in this dict are displayed, if they're not in here, they get style="display: none"
+                rowspan_by_row = {}  # cells for rows in this dict are displayed, if they're not in here, they get style="display: none"
                 prev_value = no_value_set
                 prev_row = no_value_set
                 for cells in self.cells_for_rows():
                     value = Cell(cells, column).refine_done(parent=self).value
                     if prev_value != value:
                         rowspan_by_row[id(cells.row)] = 1
                         prev_value = value
@@ -2397,15 +2395,15 @@
         For use in post_handlers. Only valid when rows was a queryset.
         """
         assert isinstance(self.initial_rows, QuerySet), "bulk_queryset can only be used on querysets"
 
         return self.selection(prefix=prefix).filter(**self.bulk_filter).exclude(**self.bulk_exclude)
 
     def should_render_form_tag(self):
-        return bool(self.bulk)
+        return bool(self.bulk and self.bulk.actions)
 
     @dispatch(
         render=render_template,
     )
     def __html__(self, *, template=None, render=None):
         assert self._is_bound, NOT_BOUND_MESSAGE
```

### Comparing `iommi-7.0.0/iommi/templates/.DS_Store` & `iommi-7.1.0/iommi/templates/.DS_Store`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/templates/iommi/.DS_Store` & `iommi-7.1.0/iommi/templates/iommi/.DS_Store`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/templates/iommi/base.html` & `iommi-7.1.0/iommi/templates/iommi/base.html`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/templates/iommi/form/.DS_Store` & `iommi-7.1.0/iommi/templates/iommi/form/.DS_Store`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/templates/iommi/form/actions.html` & `iommi-7.1.0/iommi/templates/iommi/form/actions.html`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/templates/iommi/form/choice_select2.html` & `iommi-7.1.0/iommi/templates/iommi/form/choice_select2.html`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/templates/iommi/query/advanced.html` & `iommi-7.1.0/iommi/templates/iommi/query/advanced.html`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/templates/iommi/query/form.html` & `iommi-7.1.0/iommi/templates/iommi/query/form.html`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/templates/iommi/query/form_toggle_script.html` & `iommi-7.1.0/iommi/templates/iommi/query/form_toggle_script.html`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/templates/iommi/table/bootstrap/paginator.html` & `iommi-7.1.0/iommi/templates/iommi/table/bootstrap/paginator.html`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/templates/iommi/table/bulma/paginator.html` & `iommi-7.1.0/iommi/templates/iommi/table/bulma/paginator.html`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/templates/iommi/table/js_select_all.html` & `iommi-7.1.0/iommi/templates/iommi/table/js_select_all.html`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/templates/iommi/table/paginator.html` & `iommi-7.1.0/iommi/templates/iommi/table/paginator.html`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/templates/iommi/table/semantic_ui/paginator.html` & `iommi-7.1.0/iommi/templates/iommi/table/semantic_ui/paginator.html`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/templates/iommi/table/table_container.html` & `iommi-7.1.0/iommi/templates/iommi/table/table_container.html`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/templates/iommi/table/table_tag.html` & `iommi-7.1.0/iommi/templates/iommi/table/table_tag.html`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/iommi/traversable.py` & `iommi-7.1.0/iommi/traversable.py`

 * *Files 8% similar despite different names*

```diff
@@ -188,21 +188,28 @@
 
         evaluate_parameters = {
             **(parent.iommi_evaluate_parameters() if parent is not None else {}),
             **result.own_evaluate_parameters(),
             'traversable': result,
         }
         if parent is None:
-            evaluate_parameters['request'] = request
+            evaluate_parameters = {
+                'request': request,
+                'user': getattr(request, 'user', None),
+                **evaluate_parameters,
+            }
+
             if hasattr(request, 'iommi_view_params'):
                 params = request.iommi_view_params
                 extra_params = result.extra_params(request=request, **params)
                 assert isinstance(extra_params, dict), 'extra_params needs to return a dict with additional parameters'
                 params.update(extra_params)
                 evaluate_parameters['params'] = params
+                evaluate_parameters = {**params, **evaluate_parameters}
+
         result._evaluate_parameters = evaluate_parameters
 
         if hasattr(result, 'include'):
             include = evaluate_strict(result.include, **evaluate_parameters)
             if not bool(include):
                 return None
```

### Comparing `iommi-7.0.0/iommi.egg-info/PKG-INFO` & `iommi-7.1.0/iommi.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iommi
-Version: 7.0.0
+Version: 7.1.0
 Summary: iommi is a high level framework built on django
 Home-page: https://github.com/iommirocks/iommi
 Author: Anders Hovmöller
 Author-email: boxed@killingar.net
 License: BSD
 Keywords: iommi
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `iommi-7.0.0/iommi.egg-info/SOURCES.txt` & `iommi-7.1.0/iommi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/pyproject.toml` & `iommi-7.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/setup.cfg` & `iommi-7.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `iommi-7.0.0/setup.py` & `iommi-7.1.0/setup.py`

 * *Files identical despite different names*

