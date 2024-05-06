# Comparing `tmp/platform_plugin_aspects-0.7.4.tar.gz` & `tmp/platform_plugin_aspects-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "platform_plugin_aspects-0.7.4.tar", last modified: Wed May  1 00:59:10 2024, max compression
+gzip compressed data, was "platform_plugin_aspects-0.8.0.tar", last modified: Mon May  6 18:18:35 2024, max compression
```

## Comparing `platform_plugin_aspects-0.7.4.tar` & `platform_plugin_aspects-0.8.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:59:10.320966 platform_plugin_aspects-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11636 2024-05-01 00:59:10.320966 platform_plugin_aspects-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8698 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:59:10.312966 platform_plugin_aspects-0.7.4/platform_plugin_aspects/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:59:10.316966 platform_plugin_aspects-0.7.4/platform_plugin_aspects/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects/extensions/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:59:10.316966 platform_plugin_aspects-0.7.4/platform_plugin_aspects/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:59:10.316966 platform_plugin_aspects-0.7.4/platform_plugin_aspects/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects/management/commands/load_test_tracking_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    14268 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:59:10.316966 platform_plugin_aspects-0.7.4/platform_plugin_aspects/settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects/settings/production.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:59:10.316966 platform_plugin_aspects-0.7.4/platform_plugin_aspects/sinks/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects/sinks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12821 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects/sinks/base_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     7964 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects/sinks/course_overview_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects/sinks/external_id_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects/sinks/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects/sinks/user_profile_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects/sinks/user_retire_sink.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:59:10.308966 platform_plugin_aspects-0.7.4/platform_plugin_aspects/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:59:10.316966 platform_plugin_aspects-0.7.4/platform_plugin_aspects/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects/static/css/superset.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:59:10.316966 platform_plugin_aspects-0.7.4/platform_plugin_aspects/static/html/
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects/static/html/superset.html
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects/static/html/superset_student.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:59:10.316966 platform_plugin_aspects-0.7.4/platform_plugin_aspects/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects/static/js/embed_dashboard.js
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects/static/js/install_required.js
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects/static/js/superset.js
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:59:10.312966 platform_plugin_aspects-0.7.4/platform_plugin_aspects/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:59:10.316966 platform_plugin_aspects-0.7.4/platform_plugin_aspects/templates/instructor_dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects/templates/instructor_dashboard/aspects.html
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     8437 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects/views.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects/waffle.py
--rw-r--r--   0 runner    (1001) docker     (127)     6858 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects/xblock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:59:10.320966 platform_plugin_aspects-0.7.4/platform_plugin_aspects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11636 2024-05-01 00:59:10.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-01 00:59:10.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:59:10.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-01 00:59:10.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:59:10.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-01 00:59:10.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 00:59:10.000000 platform_plugin_aspects-0.7.4/platform_plugin_aspects.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:59:10.316966 platform_plugin_aspects-0.7.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-01 00:59:10.320966 platform_plugin_aspects-0.7.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     6997 2024-05-01 00:59:03.000000 platform_plugin_aspects-0.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:18:35.078527 platform_plugin_aspects-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11726 2024-05-06 18:18:35.078527 platform_plugin_aspects-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8698 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:18:35.074527 platform_plugin_aspects-0.8.0/platform_plugin_aspects/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:18:35.074527 platform_plugin_aspects-0.8.0/platform_plugin_aspects/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects/extensions/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:18:35.074527 platform_plugin_aspects-0.8.0/platform_plugin_aspects/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:18:35.074527 platform_plugin_aspects-0.8.0/platform_plugin_aspects/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects/management/commands/load_test_tracking_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14268 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:18:35.074527 platform_plugin_aspects-0.8.0/platform_plugin_aspects/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:18:35.078527 platform_plugin_aspects-0.8.0/platform_plugin_aspects/sinks/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects/sinks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12821 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects/sinks/base_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects/sinks/course_overview_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects/sinks/external_id_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects/sinks/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects/sinks/user_profile_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects/sinks/user_retire_sink.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:18:35.070527 platform_plugin_aspects-0.8.0/platform_plugin_aspects/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:18:35.078527 platform_plugin_aspects-0.8.0/platform_plugin_aspects/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects/static/css/superset.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:18:35.078527 platform_plugin_aspects-0.8.0/platform_plugin_aspects/static/html/
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects/static/html/superset.html
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects/static/html/superset_student.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:18:35.078527 platform_plugin_aspects-0.8.0/platform_plugin_aspects/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects/static/js/embed_dashboard.js
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects/static/js/install_required.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects/static/js/superset.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:18:35.070527 platform_plugin_aspects-0.8.0/platform_plugin_aspects/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:18:35.078527 platform_plugin_aspects-0.8.0/platform_plugin_aspects/templates/instructor_dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects/templates/instructor_dashboard/aspects.html
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects/waffle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6858 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects/xblock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:18:35.078527 platform_plugin_aspects-0.8.0/platform_plugin_aspects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11726 2024-05-06 18:18:35.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-06 18:18:35.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 18:18:35.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-06 18:18:35.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 18:18:35.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-06 18:18:35.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-06 18:18:35.000000 platform_plugin_aspects-0.8.0/platform_plugin_aspects.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:18:35.078527 platform_plugin_aspects-0.8.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-06 18:18:35.078527 platform_plugin_aspects-0.8.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6997 2024-05-06 18:18:31.000000 platform_plugin_aspects-0.8.0/setup.py
```

### Comparing `platform_plugin_aspects-0.7.4/CHANGELOG.rst` & `platform_plugin_aspects-0.8.0/CHANGELOG.rst`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,22 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
-*
+0.8.0 - 2024-05-06
+******************
+
+Added
+=====
+
+* Added tags to xblocks in course dump
+
 
 0.7.4 - 2024-04-30
 ******************
 
 Fixed
 =====
 * Fixed Superset XBlock and default filters.
```

### Comparing `platform_plugin_aspects-0.7.4/LICENSE` & `platform_plugin_aspects-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.4/PKG-INFO` & `platform_plugin_aspects-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platform-plugin-aspects
-Version: 0.7.4
+Version: 0.8.0
 Summary: Aspects plugins for edx-platform
 Home-page: https://github.com/openedx/platform-plugin-aspects
 Author: Open edX Project
 Author-email: oscm@openedx.org
 License: Apache 2.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -272,15 +272,22 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
-*
+0.8.0 - 2024-05-06
+******************
+
+Added
+=====
+
+* Added tags to xblocks in course dump
+
 
 0.7.4 - 2024-04-30
 ******************
 
 Fixed
 =====
 * Fixed Superset XBlock and default filters.
```

### Comparing `platform_plugin_aspects-0.7.4/README.rst` & `platform_plugin_aspects-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.4/platform_plugin_aspects/apps.py` & `platform_plugin_aspects-0.8.0/platform_plugin_aspects/apps.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.4/platform_plugin_aspects/extensions/filters.py` & `platform_plugin_aspects-0.8.0/platform_plugin_aspects/extensions/filters.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.4/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py` & `platform_plugin_aspects-0.8.0/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.4/platform_plugin_aspects/management/commands/load_test_tracking_events.py` & `platform_plugin_aspects-0.8.0/platform_plugin_aspects/management/commands/load_test_tracking_events.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.4/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py` & `platform_plugin_aspects-0.8.0/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.4/platform_plugin_aspects/settings/common.py` & `platform_plugin_aspects-0.8.0/platform_plugin_aspects/settings/common.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.4/platform_plugin_aspects/settings/production.py` & `platform_plugin_aspects-0.8.0/platform_plugin_aspects/settings/production.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.4/platform_plugin_aspects/signals.py` & `platform_plugin_aspects-0.8.0/platform_plugin_aspects/signals.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.4/platform_plugin_aspects/sinks/base_sink.py` & `platform_plugin_aspects-0.8.0/platform_plugin_aspects/sinks/base_sink.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.4/platform_plugin_aspects/sinks/course_overview_sink.py` & `platform_plugin_aspects-0.8.0/platform_plugin_aspects/sinks/course_overview_sink.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,19 @@
 import datetime
 import json
 
 from opaque_keys.edx.keys import CourseKey
 
 from platform_plugin_aspects.sinks.base_sink import ModelBaseSink
 from platform_plugin_aspects.sinks.serializers import CourseOverviewSerializer
-from platform_plugin_aspects.utils import get_detached_xblock_types, get_modulestore
+from platform_plugin_aspects.utils import (
+    get_detached_xblock_types,
+    get_modulestore,
+    get_tags_for_block,
+)
 
 # Defaults we want to ensure we fail early on bulk inserts
 CLICKHOUSE_BULK_INSERT_PARAMS = {
     "input_format_allow_errors_num": 1,
     "input_format_allow_errors_ratio": 0.1,
 }
 
@@ -82,14 +86,17 @@
                 unit_idx = 0
             elif fields["xblock_data_json"]["block_type"] == "vertical":
                 unit_idx += 1
 
             fields["xblock_data_json"]["section"] = section_idx
             fields["xblock_data_json"]["subsection"] = subsection_idx
             fields["xblock_data_json"]["unit"] = unit_idx
+            fields["xblock_data_json"]["tags"] = get_tags_for_block(
+                fields["location"],
+            )
 
             fields["xblock_data_json"] = json.dumps(fields["xblock_data_json"])
             location_to_node[XBlockSink.strip_branch_and_version(block.location)] = (
                 fields
             )
 
         return list(location_to_node.values())
```

### Comparing `platform_plugin_aspects-0.7.4/platform_plugin_aspects/sinks/external_id_sink.py` & `platform_plugin_aspects-0.8.0/platform_plugin_aspects/sinks/external_id_sink.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.4/platform_plugin_aspects/sinks/serializers.py` & `platform_plugin_aspects-0.8.0/platform_plugin_aspects/sinks/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import json
 import uuid
 
 from django.utils import timezone
 from rest_framework import serializers
 
-from platform_plugin_aspects.utils import get_model
+from platform_plugin_aspects.utils import get_model, get_tags_for_block
 
 
 class BaseSinkSerializer(serializers.Serializer):  # pylint: disable=abstract-method
     """Base sink serializer for ClickHouse."""
 
     dump_id = serializers.SerializerMethodField()
     time_last_dumped = serializers.SerializerMethodField()
@@ -142,13 +142,14 @@
                 overview, "max_student_enrollments_allowed", None
             ),
             "effort": getattr(overview, "effort", ""),
             "enable_proctored_exams": getattr(overview, "enable_proctored_exams", ""),
             "entrance_exam_enabled": getattr(overview, "entrance_exam_enabled", ""),
             "external_id": getattr(overview, "external_id", ""),
             "language": getattr(overview, "language", ""),
+            "tags": get_tags_for_block(overview.id),
         }
         return json.dumps(json_fields)
 
     def get_course_key(self, overview):
         """Return the course key as a string."""
         return str(overview.id)
```

### Comparing `platform_plugin_aspects-0.7.4/platform_plugin_aspects/sinks/user_profile_sink.py` & `platform_plugin_aspects-0.8.0/platform_plugin_aspects/sinks/user_profile_sink.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.4/platform_plugin_aspects/sinks/user_retire_sink.py` & `platform_plugin_aspects-0.8.0/platform_plugin_aspects/sinks/user_retire_sink.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.4/platform_plugin_aspects/static/css/superset.css` & `platform_plugin_aspects-0.8.0/platform_plugin_aspects/static/css/superset.css`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.4/platform_plugin_aspects/static/html/superset.html` & `platform_plugin_aspects-0.8.0/platform_plugin_aspects/static/html/superset.html`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.4/platform_plugin_aspects/static/js/embed_dashboard.js` & `platform_plugin_aspects-0.8.0/platform_plugin_aspects/static/js/embed_dashboard.js`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.4/platform_plugin_aspects/static/js/superset.js` & `platform_plugin_aspects-0.8.0/platform_plugin_aspects/static/js/superset.js`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.4/platform_plugin_aspects/tasks.py` & `platform_plugin_aspects-0.8.0/platform_plugin_aspects/tasks.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.4/platform_plugin_aspects/templates/instructor_dashboard/aspects.html` & `platform_plugin_aspects-0.8.0/platform_plugin_aspects/templates/instructor_dashboard/aspects.html`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.4/platform_plugin_aspects/urls.py` & `platform_plugin_aspects-0.8.0/platform_plugin_aspects/urls.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.4/platform_plugin_aspects/utils.py` & `platform_plugin_aspects-0.8.0/platform_plugin_aspects/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -274,7 +274,51 @@
     """
     Generate an idempotent uuid.
     """
     base_uuid = uuid.UUID(base_uuid)
     base_namespace = uuid.uuid5(base_uuid, "superset")
     normalized_language = language.lower().replace("-", "_")
     return str(uuid.uuid5(base_namespace, normalized_language))
+
+
+def _get_object_tags(usage_key):  # pragma: no cover
+    """
+    Wrap the Open edX tagging API method get_object_tags.
+    """
+    try:
+        # pylint: disable=import-outside-toplevel
+        from openedx.core.djangoapps.content_tagging.api import get_object_tags
+
+        return get_object_tags(object_id=str(usage_key))
+    # Pre-Redwood versions of Open edX don't have this API
+    except ImportError:
+        return {}
+
+
+def get_tags_for_block(usage_key) -> dict:
+    """
+    Return all the tags (and their parent tags) applied to the given block.
+
+    Returns a dict of [taxonomy]: [tag, tag, tag]
+    """
+    tags = _get_object_tags(usage_key)
+    serialized_tags = {}
+
+    for explicit_tag in tags:
+        _add_tag(explicit_tag, serialized_tags)
+        implicit_tag = explicit_tag.tag.parent
+
+        while implicit_tag:
+            _add_tag(implicit_tag, serialized_tags)
+            implicit_tag = implicit_tag.parent
+
+    return serialized_tags
+
+
+def _add_tag(tag, serialized_tags):
+    """
+    Add a tag to our serialized list of tags.
+    """
+    if tag.taxonomy.name not in serialized_tags:
+        serialized_tags[tag.taxonomy.name] = [tag.value]
+    else:
+        serialized_tags[tag.taxonomy.name].append(tag.value)
```

### Comparing `platform_plugin_aspects-0.7.4/platform_plugin_aspects/views.py` & `platform_plugin_aspects-0.8.0/platform_plugin_aspects/views.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.4/platform_plugin_aspects/xblock.py` & `platform_plugin_aspects-0.8.0/platform_plugin_aspects/xblock.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.4/platform_plugin_aspects.egg-info/PKG-INFO` & `platform_plugin_aspects-0.8.0/platform_plugin_aspects.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platform-plugin-aspects
-Version: 0.7.4
+Version: 0.8.0
 Summary: Aspects plugins for edx-platform
 Home-page: https://github.com/openedx/platform-plugin-aspects
 Author: Open edX Project
 Author-email: oscm@openedx.org
 License: Apache 2.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -272,15 +272,22 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
-*
+0.8.0 - 2024-05-06
+******************
+
+Added
+=====
+
+* Added tags to xblocks in course dump
+
 
 0.7.4 - 2024-04-30
 ******************
 
 Fixed
 =====
 * Fixed Superset XBlock and default filters.
```

### Comparing `platform_plugin_aspects-0.7.4/platform_plugin_aspects.egg-info/SOURCES.txt` & `platform_plugin_aspects-0.8.0/platform_plugin_aspects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.4/requirements/constraints.txt` & `platform_plugin_aspects-0.8.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.4/setup.py` & `platform_plugin_aspects-0.8.0/setup.py`

 * *Files identical despite different names*

