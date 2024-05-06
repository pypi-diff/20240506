# Comparing `tmp/django-db-views-0.1.6.tar.gz` & `tmp/django-db-views-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-db-views-0.1.6.tar", last modified: Sun Dec  3 00:20:39 2023, max compression
+gzip compressed data, was "django-db-views-0.1.7.tar", last modified: Mon May  6 20:58:58 2024, max compression
```

## Comparing `django-db-views-0.1.6.tar` & `django-db-views-0.1.7.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxrwxr-x   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-12-03 00:20:39.941941 django-db-views-0.1.6/
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     1074 2023-07-13 18:00:46.000000 django-db-views-0.1.6/LICENSE
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     5935 2023-12-03 00:20:39.941941 django-db-views-0.1.6/PKG-INFO
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     4926 2023-12-02 21:56:45.000000 django-db-views-0.1.6/README.md
-drwxrwxr-x   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-12-03 00:20:39.941941 django-db-views-0.1.6/django_db_views/
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)       32 2023-07-13 18:00:46.000000 django-db-views-0.1.6/django_db_views/__init__.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)    13376 2023-07-13 18:00:46.000000 django-db-views-0.1.6/django_db_views/autodetector.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      416 2023-07-13 18:00:46.000000 django-db-views-0.1.6/django_db_views/context_manager.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     1408 2023-07-13 18:00:46.000000 django-db-views-0.1.6/django_db_views/db_view.py
-drwxrwxr-x   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-12-03 00:20:39.941941 django-db-views-0.1.6/django_db_views/management/
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-07-13 18:00:46.000000 django-db-views-0.1.6/django_db_views/management/__init__.py
-drwxrwxr-x   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-12-03 00:20:39.941941 django-db-views-0.1.6/django_db_views/management/commands/
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-07-13 18:00:46.000000 django-db-views-0.1.6/django_db_views/management/commands/__init__.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     4797 2023-07-13 18:00:46.000000 django-db-views-0.1.6/django_db_views/management/commands/makeviewmigrations.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     2935 2023-07-13 18:00:46.000000 django-db-views-0.1.6/django_db_views/migration_functions.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     2596 2023-07-13 18:00:46.000000 django-db-views-0.1.6/django_db_views/operations.py
-drwxrwxr-x   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-12-03 00:20:39.941941 django-db-views-0.1.6/django_db_views.egg-info/
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     5935 2023-12-03 00:20:39.000000 django-db-views-0.1.6/django_db_views.egg-info/PKG-INFO
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      886 2023-12-03 00:20:39.000000 django-db-views-0.1.6/django_db_views.egg-info/SOURCES.txt
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)        1 2023-12-03 00:20:39.000000 django-db-views-0.1.6/django_db_views.egg-info/dependency_links.txt
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)       11 2023-12-03 00:20:39.000000 django-db-views-0.1.6/django_db_views.egg-info/requires.txt
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)       22 2023-12-03 00:20:39.000000 django-db-views-0.1.6/django_db_views.egg-info/top_level.txt
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)       38 2023-12-03 00:20:39.941941 django-db-views-0.1.6/setup.cfg
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     1609 2023-12-02 21:56:45.000000 django-db-views-0.1.6/setup.py
-drwxrwxr-x   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-12-03 00:20:39.941941 django-db-views-0.1.6/tests/
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-07-13 18:00:46.000000 django-db-views-0.1.6/tests/__init__.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      529 2023-07-13 18:00:46.000000 django-db-views-0.1.6/tests/asserts_utils.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     1726 2023-07-13 18:00:46.000000 django-db-views-0.1.6/tests/conftest.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      380 2023-07-13 18:00:46.000000 django-db-views-0.1.6/tests/decorators.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     2444 2023-07-13 18:00:46.000000 django-db-views-0.1.6/tests/dynamic_models_fixtures.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     1493 2023-07-13 18:00:46.000000 django-db-views-0.1.6/tests/fixturies.py
-drwxrwxr-x   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-12-03 00:20:39.941941 django-db-views-0.1.6/tests/test_app/
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-07-13 18:00:46.000000 django-db-views-0.1.6/tests/test_app/__init__.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     4370 2023-07-13 18:00:46.000000 django-db-views-0.1.6/tests/test_app/models.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-07-13 18:00:46.000000 django-db-views-0.1.6/tests/test_autodetector.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     1018 2023-07-13 18:00:46.000000 django-db-views-0.1.6/tests/test_backward_compatibility.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-07-13 18:00:46.000000 django-db-views-0.1.6/tests/test_db_functions.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)    12698 2023-12-02 20:12:50.000000 django-db-views-0.1.6/tests/test_db_views.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     3025 2023-07-13 18:00:46.000000 django-db-views-0.1.6/tests/test_materialized_views.py
+drwxrwxr-x   0 bartlomiej  (1000) bartlomiej  (1000)        0 2024-05-06 20:58:58.520457 django-db-views-0.1.7/
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     1074 2023-07-13 18:00:46.000000 django-db-views-0.1.7/LICENSE
+-rw-r--r--   0 bartlomiej  (1000) bartlomiej  (1000)     5976 2024-05-06 20:58:58.520457 django-db-views-0.1.7/PKG-INFO
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     4926 2023-12-02 21:56:45.000000 django-db-views-0.1.7/README.md
+drwxrwxr-x   0 bartlomiej  (1000) bartlomiej  (1000)        0 2024-05-06 20:58:58.516457 django-db-views-0.1.7/django_db_views/
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)       32 2023-07-13 18:00:46.000000 django-db-views-0.1.7/django_db_views/__init__.py
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)    15199 2024-05-06 20:58:07.000000 django-db-views-0.1.7/django_db_views/autodetector.py
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      416 2023-07-13 18:00:46.000000 django-db-views-0.1.7/django_db_views/context_manager.py
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     1408 2023-07-13 18:00:46.000000 django-db-views-0.1.7/django_db_views/db_view.py
+drwxrwxr-x   0 bartlomiej  (1000) bartlomiej  (1000)        0 2024-05-06 20:58:58.520457 django-db-views-0.1.7/django_db_views/management/
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-07-13 18:00:46.000000 django-db-views-0.1.7/django_db_views/management/__init__.py
+drwxrwxr-x   0 bartlomiej  (1000) bartlomiej  (1000)        0 2024-05-06 20:58:58.520457 django-db-views-0.1.7/django_db_views/management/commands/
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-07-13 18:00:46.000000 django-db-views-0.1.7/django_db_views/management/commands/__init__.py
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     4797 2023-07-13 18:00:46.000000 django-db-views-0.1.7/django_db_views/management/commands/makeviewmigrations.py
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     2935 2023-07-13 18:00:46.000000 django-db-views-0.1.7/django_db_views/migration_functions.py
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     2596 2023-07-13 18:00:46.000000 django-db-views-0.1.7/django_db_views/operations.py
+drwxrwxr-x   0 bartlomiej  (1000) bartlomiej  (1000)        0 2024-05-06 20:58:58.520457 django-db-views-0.1.7/django_db_views.egg-info/
+-rw-r--r--   0 bartlomiej  (1000) bartlomiej  (1000)     5976 2024-05-06 20:58:58.000000 django-db-views-0.1.7/django_db_views.egg-info/PKG-INFO
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      901 2024-05-06 20:58:58.000000 django-db-views-0.1.7/django_db_views.egg-info/SOURCES.txt
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)        1 2024-05-06 20:58:58.000000 django-db-views-0.1.7/django_db_views.egg-info/dependency_links.txt
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)       11 2024-05-06 20:58:58.000000 django-db-views-0.1.7/django_db_views.egg-info/requires.txt
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)       22 2024-05-06 20:58:58.000000 django-db-views-0.1.7/django_db_views.egg-info/top_level.txt
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)       38 2024-05-06 20:58:58.520457 django-db-views-0.1.7/setup.cfg
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     1582 2024-05-06 20:58:07.000000 django-db-views-0.1.7/setup.py
+drwxrwxr-x   0 bartlomiej  (1000) bartlomiej  (1000)        0 2024-05-06 20:58:58.520457 django-db-views-0.1.7/tests/
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-07-13 18:00:46.000000 django-db-views-0.1.7/tests/__init__.py
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      529 2023-07-13 18:00:46.000000 django-db-views-0.1.7/tests/asserts_utils.py
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     1541 2024-05-06 20:58:07.000000 django-db-views-0.1.7/tests/conftest.py
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      380 2023-12-27 10:36:42.000000 django-db-views-0.1.7/tests/decorators.py
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     2444 2023-07-13 18:00:46.000000 django-db-views-0.1.7/tests/dynamic_models_fixtures.py
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     1493 2023-07-13 18:00:46.000000 django-db-views-0.1.7/tests/fixturies.py
+drwxrwxr-x   0 bartlomiej  (1000) bartlomiej  (1000)        0 2024-05-06 20:58:58.520457 django-db-views-0.1.7/tests/test_app/
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-07-13 18:00:46.000000 django-db-views-0.1.7/tests/test_app/__init__.py
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     4370 2023-07-13 18:00:46.000000 django-db-views-0.1.7/tests/test_app/models.py
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-07-13 18:00:46.000000 django-db-views-0.1.7/tests/test_autodetector.py
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     1018 2024-05-05 22:09:17.000000 django-db-views-0.1.7/tests/test_backward_compatibility.py
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-07-13 18:00:46.000000 django-db-views-0.1.7/tests/test_db_functions.py
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)    14171 2024-05-06 20:58:07.000000 django-db-views-0.1.7/tests/test_db_views.py
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     3025 2023-07-13 18:00:46.000000 django-db-views-0.1.7/tests/test_materialized_views.py
+-rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      143 2024-05-06 20:58:07.000000 django-db-views-0.1.7/tests/utils.py
```

### Comparing `django-db-views-0.1.6/LICENSE` & `django-db-views-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django-db-views-0.1.6/PKG-INFO` & `django-db-views-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-db-views
-Version: 0.1.6
+Version: 0.1.7
 Summary: Handle database views. Allow to create migrations for database views. View migrations using django code. They can be reversed. Changes in model view definition are detected automatically. Support almost all options as regular makemigrations command
 Home-page: https://github.com/BezBartek/django-db-views
 Author: Bartłomiej Nowak and Mariusz Okulanis
 Author-email: n.bartek3762@gmail.com
 License: MIT
 Keywords: views,database views,django,database perspective,view migrations,database table function,django materialized views
 Classifier: License :: OSI Approved :: MIT License
@@ -12,14 +12,16 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Django
+Requires-Dist: six
 
 # django-db-views
 
 
 [![License](https://img.shields.io/:license-mit-blue.svg)](http://doge.mit-license.org)  
 [![PyPi](https://badge.fury.io/py/django-db-views.svg)](https://pypi.org/project/django-db-views/)  
 **Django Versions** 2.2 to 4.2+
```

### Comparing `django-db-views-0.1.6/README.md` & `django-db-views-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `django-db-views-0.1.6/django_db_views/autodetector.py` & `django-db-views-0.1.7/django_db_views/autodetector.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,34 +3,47 @@
 from typing import Type
 
 import django
 import six
 from django.apps import apps
 from django.conf import settings
 from django.db import connection, ProgrammingError
+from django.db.migrations import SeparateDatabaseAndState
 from django.db.migrations.autodetector import MigrationAutodetector
 from django.db.migrations.graph import MigrationGraph
 
 from django_db_views.db_view import DBView, DBMaterializedView, DBViewsRegistry
-from django_db_views.operations import ViewRunPython, DBViewModelState, ViewDropRunPython
-from django_db_views.migration_functions import ForwardViewMigration, BackwardViewMigration, \
-    ForwardMaterializedViewMigration, BackwardMaterializedViewMigration, ForwardViewMigrationBase, \
-    BackwardViewMigrationBase, DropView, DropMaterializedView, DropViewMigration
+from django_db_views.operations import (
+    ViewRunPython,
+    DBViewModelState,
+    ViewDropRunPython,
+)
+from django_db_views.migration_functions import (
+    ForwardViewMigration,
+    BackwardViewMigration,
+    ForwardMaterializedViewMigration,
+    BackwardMaterializedViewMigration,
+    ForwardViewMigrationBase,
+    BackwardViewMigrationBase,
+    DropView,
+    DropMaterializedView,
+    DropViewMigration,
+)
 
 
 class ViewMigrationAutoDetector(MigrationAutodetector):
     """
-        We overwritten only _detect_changes function.
-        It's almost same code as in regular function,
-        we just removed generating other operations, and instead of them added our detection.
-        rest methods are fully our code which we use for detection.
-        It's detect only view model changes.
+    We overwritten only _detect_changes function.
+    It's almost same code as in regular function,
+    we just removed generating other operations, and instead of them added our detection.
+    rest methods are fully our code which we use for detection.
+    It's detect only view model changes.
     """
-    def _detect_changes(self, convert_apps=None, graph=None) -> dict:
 
+    def _detect_changes(self, convert_apps=None, graph=None) -> dict:
         # <START copy paste from MigrationAutodetector, depends on django version>
         if django.VERSION >= (4,):
             self._detect_changes_preparation_django_version_4_and_above(convert_apps)
         else:
             self._detect_changes_preparation_django_below_version_4(convert_apps)
         # <END of copy paste from MigrationAutodetector>
 
@@ -78,17 +91,16 @@
                 else:
                     self.old_model_keys.append((al, mn))
 
         for al, mn in sorted(self.to_state.models.keys()):
             model = self.new_apps.get_model(al, mn)
             if not model._meta.managed:
                 self.new_unmanaged_keys.append((al, mn))
-            elif (
-                    al not in self.from_state.real_apps or
-                    (convert_apps and al in convert_apps)
+            elif al not in self.from_state.real_apps or (
+                convert_apps and al in convert_apps
             ):
                 if model._meta.proxy:
                     self.new_proxy_keys.append((al, mn))
                 else:
                     self.new_model_keys.append((al, mn))
 
     def _detect_changes_preparation_django_version_4_and_above(self, convert_apps):
@@ -101,54 +113,55 @@
         self.old_model_keys = set()
         self.old_proxy_keys = set()
         self.old_unmanaged_keys = set()
         self.new_model_keys = set()
         self.new_proxy_keys = set()
         self.new_unmanaged_keys = set()
         for (app_label, model_name), model_state in self.from_state.models.items():
-            if not model_state.options.get('managed', True):
+            if not model_state.options.get("managed", True):
                 self.old_unmanaged_keys.add((app_label, model_name))
             elif app_label not in self.from_state.real_apps:
-                if model_state.options.get('proxy'):
+                if model_state.options.get("proxy"):
                     self.old_proxy_keys.add((app_label, model_name))
                 else:
                     self.old_model_keys.add((app_label, model_name))
 
         for (app_label, model_name), model_state in self.to_state.models.items():
-            if not model_state.options.get('managed', True):
+            if not model_state.options.get("managed", True):
                 self.new_unmanaged_keys.add((app_label, model_name))
-            elif (
-                app_label not in self.from_state.real_apps or
-                (convert_apps and app_label in convert_apps)
+            elif app_label not in self.from_state.real_apps or (
+                convert_apps and app_label in convert_apps
             ):
-                if model_state.options.get('proxy'):
+                if model_state.options.get("proxy"):
                     self.new_proxy_keys.add((app_label, model_name))
                 else:
                     self.new_model_keys.add((app_label, model_name))
 
         self.from_state.resolve_fields_and_relations()
         self.to_state.resolve_fields_and_relations()
 
     def delete_old_views(self):
-        for (app_label, table_name), model_state in self.get_previous_view_models_state().items():
+        for (
+            app_label,
+            table_name,
+        ), model_state in self.get_previous_view_models_state().items():
             if model_state.table_name not in DBViewsRegistry:
                 self.add_operation(
                     app_label,
                     ViewDropRunPython(
                         self.get_drop_migration_class(model_state.base_class)(
-                            model_state.table_name,
-                            engine=model_state.view_engine
+                            model_state.table_name, engine=model_state.view_engine
                         ),
                         self.get_backward_migration_class(model_state.base_class)(
                             model_state.view_definition,
                             model_state.table_name,
-                            engine=model_state.view_engine
+                            engine=model_state.view_engine,
                         ),
-                        atomic=False
-                    )
+                        atomic=False,
+                    ),
                 )
 
     def get_previous_view_models_state(self) -> dict:
         view_models = {}
         for (app_label, table_name), model_state in self.from_state.models.items():
             if isinstance(model_state, DBViewModelState):
                 key = (app_label, table_name)
@@ -163,16 +176,20 @@
                     key = (app_label, model_name)
                     view_models[key] = model_class
         return view_models
 
     def is_same_views(self, current: str, new: str) -> bool:
         if not current:
             return False
-        s1_words = filter(lambda x: len(x) != 0, re.split(pattern="[^a-zA-Z]*", string=current))
-        s2_words = filter(lambda x: len(x) != 0, re.split(pattern="[^a-zA-Z]*", string=new))
+        s1_words = filter(
+            lambda x: len(x) != 0, re.split(pattern="[^a-zA-Z]*", string=current)
+        )
+        s2_words = filter(
+            lambda x: len(x) != 0, re.split(pattern="[^a-zA-Z]*", string=new)
+        )
         for w1, w2 in zip_longest(s1_words, s2_words):
             if not w1 or not w2:
                 return False
             if w1.lower() != w2.lower():
                 return False
         return True
 
@@ -180,36 +197,38 @@
         view_models = self.get_current_view_models()
         for (app_label, model_name), view_model in view_models.items():
             new_view_definition = self.get_view_definition_from_model(view_model)
             for engine, latest_view_definition in new_view_definition.items():
                 current_view_definition = self.get_previous_view_definition_state(
                     graph, app_label, view_model._meta.db_table, engine
                 )
-                if not self.is_same_views(current_view_definition, latest_view_definition):
+                if not self.is_same_views(
+                    current_view_definition, latest_view_definition
+                ):
                     # Depend on all bases
                     model_state = self.to_state.models[app_label, model_name]
                     dependencies = []
                     for base in model_state.bases:
                         if isinstance(base, six.string_types) and "." in base:
                             base_app_label, base_name = base.split(".", 1)
                             dependencies.append((base_app_label, base_name, None, True))
                     self.add_operation(
                         app_label,
                         ViewRunPython(
                             self.get_forward_migration_class(view_model)(
                                 latest_view_definition.strip(";"),
                                 view_model._meta.db_table,
-                                engine=engine
+                                engine=engine,
                             ),
                             self.get_backward_migration_class(view_model)(
                                 current_view_definition.strip(";"),
                                 view_model._meta.db_table,
-                                engine=engine
+                                engine=engine,
                             ),
-                            atomic=False
+                            atomic=False,
                         ),
                         dependencies=dependencies,
                     )
 
     def get_forward_migration_class(self, model) -> Type[ForwardViewMigrationBase]:
         if issubclass(model, DBMaterializedView):
             return ForwardMaterializedViewMigration
@@ -239,47 +258,93 @@
         if callable(view_model.view_definition):
             raw_view_definition = view_model.view_definition()
         else:
             raw_view_definition = view_model.view_definition
 
         if isinstance(raw_view_definition, dict):
             for engine, definition in raw_view_definition.items():
-                view_definitions[engine] = self.get_cleaned_view_definition_value(definition)
+                view_definitions[engine] = self.get_cleaned_view_definition_value(
+                    definition
+                )
         else:
-            engine = settings.DATABASES['default']['ENGINE']
-            view_definitions[engine] = self.get_cleaned_view_definition_value(raw_view_definition)
+            engine = settings.DATABASES["default"]["ENGINE"]
+            view_definitions[engine] = self.get_cleaned_view_definition_value(
+                raw_view_definition
+            )
         return view_definitions
 
-    def get_previous_view_definition_state(self, graph: MigrationGraph, app_label: str, for_table_name: str, engine: str):
+    def get_previous_view_definition_state(
+        self, graph: MigrationGraph, app_label: str, for_table_name: str, engine: str
+    ) -> str:
         nodes = graph.leaf_nodes(app_label)
         last_node = nodes[0] if nodes else None
 
         while last_node:
             migration = graph.nodes[last_node]
             if migration.operations:
                 for operation in migration.operations:
                     if isinstance(operation, ViewRunPython):
-                        table_name = operation.code.table_name
-                        previous_view_definition = operation.code.view_definition
-                        previous_view_engine = operation.code.view_engine \
-                            if hasattr(operation.code, 'view_engine') and operation.code.view_engine \
-                            else settings.DATABASES['default']['ENGINE']
-                        if table_name == for_table_name and previous_view_engine == engine:
-                            return previous_view_definition.strip()
+                        (
+                            table_name,
+                            previous_view_engine,
+                        ) = self._get_view_identifiers_from_operation(operation)
+                        if (
+                            table_name == for_table_name
+                            and previous_view_engine == engine
+                        ):
+                            return operation.code.view_definition.strip()
+                    elif isinstance(operation, SeparateDatabaseAndState):
+                        view_operations = list(
+                            filter(
+                                lambda op: isinstance(op, ViewRunPython),
+                                operation.database_operations,
+                            )
+                        )
+                        if view_operations:
+                            assert (
+                                len(view_operations) <= 1
+                            ), "SeparateDatabaseAndState can't contain more than one ViewRunPython operation"
+                            view_operation = view_operations[0]
+                            (
+                                table_name,
+                                previous_view_engine,
+                            ) = self._get_view_identifiers_from_operation(
+                                view_operation
+                            )
+                            if (
+                                table_name == for_table_name
+                                and previous_view_engine == engine
+                            ):
+                                return view_operation.code.view_definition.strip()
             # right now i get only migrations from the same app.
-            app_parents = list(sorted(filter(lambda x: x[0] == app_label, graph.node_map[last_node].parents)))
+            app_parents = list(
+                sorted(
+                    filter(
+                        lambda x: x[0] == app_label, graph.node_map[last_node].parents
+                    )
+                )
+            )
             if app_parents:
                 last_node = app_parents[-1]
-            else:   # if no parents mean we found initial migration
+            else:  # if no parents mean we found initial migration
                 last_node = None
         return ""
 
+    def _get_view_identifiers_from_operation(self, operation) -> tuple[str, str]:
+        table_name = operation.code.table_name
+        if hasattr(operation.code, "view_engine") and operation.code.view_engine:
+            engine = operation.code.view_engine
+        else:
+            engine = settings.DATABASES["default"]["ENGINE"]
+        return table_name, engine
+
     def get_cleaned_view_definition_value(self, view_definition: str) -> str:
-        assert isinstance(view_definition, str), \
-            "View definition must be callable and return string or be itself a string."
+        assert isinstance(
+            view_definition, str
+        ), "View definition must be callable and return string or be itself a string."
         return view_definition.strip()
 
     def get_current_view_definition_from_database(self, table_name: str) -> str:
         """working only with postgres"""
         with connection.cursor() as cursor:
             try:
                 cursor.execute("SELECT pg_get_viewdef('%s')" % table_name)
```

### Comparing `django-db-views-0.1.6/django_db_views/db_view.py` & `django-db-views-0.1.7/django_db_views/db_view.py`

 * *Files identical despite different names*

### Comparing `django-db-views-0.1.6/django_db_views/management/commands/makeviewmigrations.py` & `django-db-views-0.1.7/django_db_views/management/commands/makeviewmigrations.py`

 * *Files identical despite different names*

### Comparing `django-db-views-0.1.6/django_db_views/migration_functions.py` & `django-db-views-0.1.7/django_db_views/migration_functions.py`

 * *Files identical despite different names*

### Comparing `django-db-views-0.1.6/django_db_views/operations.py` & `django-db-views-0.1.7/django_db_views/operations.py`

 * *Files identical despite different names*

### Comparing `django-db-views-0.1.6/django_db_views.egg-info/PKG-INFO` & `django-db-views-0.1.7/django_db_views.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-db-views
-Version: 0.1.6
+Version: 0.1.7
 Summary: Handle database views. Allow to create migrations for database views. View migrations using django code. They can be reversed. Changes in model view definition are detected automatically. Support almost all options as regular makemigrations command
 Home-page: https://github.com/BezBartek/django-db-views
 Author: Bartłomiej Nowak and Mariusz Okulanis
 Author-email: n.bartek3762@gmail.com
 License: MIT
 Keywords: views,database views,django,database perspective,view migrations,database table function,django materialized views
 Classifier: License :: OSI Approved :: MIT License
@@ -12,14 +12,16 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Django
+Requires-Dist: six
 
 # django-db-views
 
 
 [![License](https://img.shields.io/:license-mit-blue.svg)](http://doge.mit-license.org)  
 [![PyPi](https://badge.fury.io/py/django-db-views.svg)](https://pypi.org/project/django-db-views/)  
 **Django Versions** 2.2 to 4.2+
```

### Comparing `django-db-views-0.1.6/django_db_views.egg-info/SOURCES.txt` & `django-db-views-0.1.7/django_db_views.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -22,9 +22,10 @@
 tests/dynamic_models_fixtures.py
 tests/fixturies.py
 tests/test_autodetector.py
 tests/test_backward_compatibility.py
 tests/test_db_functions.py
 tests/test_db_views.py
 tests/test_materialized_views.py
+tests/utils.py
 tests/test_app/__init__.py
 tests/test_app/models.py
```

### Comparing `django-db-views-0.1.6/setup.py` & `django-db-views-0.1.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,25 +6,29 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="django-db-views",
-    version="0.1.6",
+    version="0.1.7",
     description="Handle database views. "
-                "Allow to create migrations for database views. "
-                "View migrations using django code. "
-                "They can be reversed. "
-                "Changes in model view definition are detected automatically. "
-                "Support almost all options as regular makemigrations command",
+    "Allow to create migrations for database views. "
+    "View migrations using django code. "
+    "They can be reversed. "
+    "Changes in model view definition are detected automatically. "
+    "Support almost all options as regular makemigrations command",
     keywords=[
-        'views', 'database views', 'django',
-        'database perspective', 'view migrations',
-        'database table function', 'django materialized views'
+        "views",
+        "database views",
+        "django",
+        "database perspective",
+        "view migrations",
+        "database table function",
+        "django materialized views",
     ],
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/BezBartek/django-db-views",
     author="Bartłomiej Nowak and Mariusz Okulanis",
     author_email="n.bartek3762@gmail.com",
     license="MIT",
```

### Comparing `django-db-views-0.1.6/tests/asserts_utils.py` & `django-db-views-0.1.7/tests/asserts_utils.py`

 * *Files identical despite different names*

### Comparing `django-db-views-0.1.6/tests/dynamic_models_fixtures.py` & `django-db-views-0.1.7/tests/dynamic_models_fixtures.py`

 * *Files identical despite different names*

### Comparing `django-db-views-0.1.6/tests/fixturies.py` & `django-db-views-0.1.7/tests/fixturies.py`

 * *Files identical despite different names*

### Comparing `django-db-views-0.1.6/tests/test_app/models.py` & `django-db-views-0.1.7/tests/test_app/models.py`

 * *Files identical despite different names*

### Comparing `django-db-views-0.1.6/tests/test_backward_compatibility.py` & `django-db-views-0.1.7/tests/test_backward_compatibility.py`

 * *Files identical despite different names*

### Comparing `django-db-views-0.1.6/tests/test_db_views.py` & `django-db-views-0.1.7/tests/test_db_views.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import pytest
 from django.apps import apps
 from django.core.management import call_command
 
 from django_db_views.db_view import DBViewsRegistry
 from tests.asserts_utils import is_view_exists
 from tests.decorators import roll_back_schema
-from tests.fixturies import temp_migrations_dir, dynamic_models_cleanup  # noqa
+from tests.utils import get_base_path
 
 
 @pytest.mark.django_db(transaction=True)
 @roll_back_schema
 def test_make_view_migration_for_db_view_based_on_raw_sql_without_dependencies(
-        temp_migrations_dir, SimpleViewWithoutDependencies
+    temp_migrations_dir, SimpleViewWithoutDependencies
 ):
     assert not (temp_migrations_dir / "0001_initial.py").exists()
     assert not is_view_exists(SimpleViewWithoutDependencies._meta.db_table)
     call_command("makeviewmigrations", "test_app")
     assert (temp_migrations_dir / "0001_initial.py").exists()
     call_command("migrate", "test_app")
     assert is_view_exists(SimpleViewWithoutDependencies._meta.db_table)
@@ -23,109 +23,131 @@
     call_command("migrate", "test_app", "zero")
     assert not is_view_exists(SimpleViewWithoutDependencies._meta.db_table)
 
 
 @pytest.mark.django_db(transaction=True)
 @roll_back_schema
 def test_make_view_migration_for_db_view_based_on_raw_sql_with_dependencies_on_other_models(
-        temp_migrations_dir, Question, Choice, RawViewQuestionStat
+    temp_migrations_dir, Question, Choice, RawViewQuestionStat
 ):
     assert not (temp_migrations_dir / "0001_initial.py").exists()
     assert not is_view_exists(RawViewQuestionStat._meta.db_table)
     call_command("makemigrations", "test_app")  # make migrations for regular tables
-    call_command("makeviewmigrations", "test_app", name="view_migration")  # make migrations for db view
+    call_command(
+        "makeviewmigrations", "test_app", name="view_migration"
+    )  # make migrations for db view
     assert len(temp_migrations_dir.listdir()) == 3, temp_migrations_dir.listdir()
     assert (temp_migrations_dir / "0001_initial.py").exists()
     assert (temp_migrations_dir / "0002_view_migration.py").exists()
-    assert "('test_app', '0001_initial')" in (temp_migrations_dir / "0002_view_migration.py").read()
+    assert (
+        "('test_app', '0001_initial')"
+        in (temp_migrations_dir / "0002_view_migration.py").read()
+    )
     call_command("migrate", "test_app")
     assert is_view_exists(RawViewQuestionStat._meta.db_table)
     assert RawViewQuestionStat.objects.all().count() == 0
     # define some instances
     question_1 = Question.objects.create(text="question_1")
     question_2 = Question.objects.create(text="question_2")
     Choice.objects.create(question=question_1, text="choice_1", votes=10)
     Choice.objects.create(question=question_1, text="choice_2", votes=10)
     Choice.objects.create(question=question_2, text="choice_1", votes=10)
     # check whether the model works correctly
     assert RawViewQuestionStat.objects.all().count() == 2
-    assert RawViewQuestionStat.objects.all().order_by("question").first().question.text == question_1.text
+    assert (
+        RawViewQuestionStat.objects.all().order_by("question").first().question.text
+        == question_1.text
+    )
 
 
 @pytest.mark.django_db(transaction=True)
 @roll_back_schema
 def test_make_view_migration_for_db_view_based_on_queryset_with_dependencies_on_other_models(
-        temp_migrations_dir, Question, Choice, QueryViewQuestionStat
+    temp_migrations_dir, Question, Choice, QueryViewQuestionStat
 ):
     assert not (temp_migrations_dir / "0001_initial.py").exists()
     assert not is_view_exists(QueryViewQuestionStat._meta.db_table)
     call_command("makemigrations", "test_app")  # make migrations for regular tables
-    call_command("makeviewmigrations", "test_app", name="view_migration")  # make migrations for db view
+    call_command(
+        "makeviewmigrations", "test_app", name="view_migration"
+    )  # make migrations for db view
     assert len(temp_migrations_dir.listdir()) == 3
     assert (temp_migrations_dir / "0001_initial.py").exists()
     assert (temp_migrations_dir / "0002_view_migration.py").exists()
-    assert "('test_app', '0001_initial')" in (temp_migrations_dir / "0002_view_migration.py").read()
+    assert (
+        "('test_app', '0001_initial')"
+        in (temp_migrations_dir / "0002_view_migration.py").read()
+    )
     call_command("migrate", "test_app")
     assert is_view_exists(QueryViewQuestionStat._meta.db_table)
     assert QueryViewQuestionStat.objects.all().count() == 0
     # define some instances
     question_1 = Question.objects.create(text="question_1")
     question_2 = Question.objects.create(text="question_2")
     Choice.objects.create(question=question_1, text="choice_1", votes=10)
     Choice.objects.create(question=question_1, text="choice_2", votes=10)
     Choice.objects.create(question=question_2, text="choice_1", votes=10)
     # check whether the model works correctly
     assert QueryViewQuestionStat.objects.all().count() == 2
-    assert QueryViewQuestionStat.objects.all().order_by("question").first().question.text == question_1.text
+    assert (
+        QueryViewQuestionStat.objects.all().order_by("question").first().question.text
+        == question_1.text
+    )
 
 
-@pytest.mark.django_db(databases=['postgres', 'sqlite'], transaction=True)
-@pytest.mark.parametrize("database", ['postgres', 'sqlite'])
+@pytest.mark.django_db(databases=["postgres", "sqlite"], transaction=True)
+@pytest.mark.parametrize("database", ["postgres", "sqlite"])
 @roll_back_schema
 def test_make_view_migration_for_db_raw_view_with_multiple_databases_support(
-        temp_migrations_dir, database, MultipleDBRawView
+    temp_migrations_dir, database, MultipleDBRawView
 ):
     assert not (temp_migrations_dir / "0001_initial.py").exists()
     assert not is_view_exists(MultipleDBRawView._meta.db_table, using=database)
     call_command("makeviewmigrations", "test_app")
     assert (temp_migrations_dir / "0001_initial.py").exists()
     call_command("migrate", "test_app", database=database)
     assert is_view_exists(MultipleDBRawView._meta.db_table, using=database)
     assert MultipleDBRawView.objects.using(database).all().count() == 2
 
 
-@pytest.mark.django_db(databases=['default', 'postgres', 'mysql'], transaction=True)
-@pytest.mark.parametrize("database", ['postgres', 'mysql'])
+@pytest.mark.django_db(databases=["default", "postgres", "mysql"], transaction=True)
+@pytest.mark.parametrize("database", ["postgres", "mysql"])
 @roll_back_schema
 def test_make_view_migration_for_db_queryset_view_with_multiple_databases_support(
-        temp_migrations_dir, database, Question, Choice, MultipleDBQueryViewQuestionStat
+    temp_migrations_dir, database, Question, Choice, MultipleDBQueryViewQuestionStat
 ):
     assert not (temp_migrations_dir / "0001_initial.py").exists()
-    assert not is_view_exists(MultipleDBQueryViewQuestionStat._meta.db_table, using=database)
+    assert not is_view_exists(
+        MultipleDBQueryViewQuestionStat._meta.db_table, using=database
+    )
     call_command("makemigrations", "test_app")
     call_command("makeviewmigrations", "test_app")
     call_command("makemigrations", "test_app")
     assert len(temp_migrations_dir.listdir()) == 3, temp_migrations_dir.listdir()
     assert (temp_migrations_dir / "0001_initial.py").exists()
     call_command("migrate", "test_app", database=database)
-    assert is_view_exists(MultipleDBQueryViewQuestionStat._meta.db_table, using=database)
+    assert is_view_exists(
+        MultipleDBQueryViewQuestionStat._meta.db_table, using=database
+    )
     assert MultipleDBQueryViewQuestionStat.objects.using(database).all().count() == 0
     call_command("migrate", "test_app", "zero", database=database)
-    assert not is_view_exists(MultipleDBQueryViewQuestionStat._meta.db_table, using=database)
+    assert not is_view_exists(
+        MultipleDBQueryViewQuestionStat._meta.db_table, using=database
+    )
 
 
 @pytest.mark.django_db(transaction=True)
 @roll_back_schema
 def test_move_up_and_down_through_simple_view_stages(
-        temp_migrations_dir, SimpleViewWithoutDependencies
+    temp_migrations_dir, SimpleViewWithoutDependencies
 ):
     call_command("makeviewmigrations", "test_app")
     assert (temp_migrations_dir / "0001_initial.py").exists()
     # made changes
-    apps.all_models['test_app']["simpleviewwithoutdependencies"].view_definition = """
+    apps.all_models["test_app"]["simpleviewwithoutdependencies"].view_definition = """
               Select *
                  From  (values (3, 'dummy_3')) A(id, name)
             """
     call_command("makeviewmigrations", "test_app", name="second_view_migration")
     assert (temp_migrations_dir / "0002_second_view_migration.py").exists()
     # no changes
     call_command("makeviewmigrations", "test_app", name="third_view_migration")
@@ -142,20 +164,18 @@
     # move to stag 1
     call_command("migrate", "test_app", "zero")
     assert not is_view_exists(SimpleViewWithoutDependencies._meta.db_table)
 
 
 @pytest.mark.django_db(transaction=True)
 @roll_back_schema
-def test_drop_view(
-        temp_migrations_dir, SimpleViewWithoutDependencies
-):
+def test_drop_view(temp_migrations_dir, SimpleViewWithoutDependencies):
     call_command("makeviewmigrations", "test_app")
     assert (temp_migrations_dir / "0001_initial.py").exists()
-    del apps.all_models['test_app'][SimpleViewWithoutDependencies.__name__.lower()]
+    del apps.all_models["test_app"][SimpleViewWithoutDependencies.__name__.lower()]
     apps.clear_cache()
     DBViewsRegistry.pop(SimpleViewWithoutDependencies._meta.db_table)
     call_command("makeviewmigrations", "test_app", name="delete_view")
     assert (temp_migrations_dir / "0002_delete_view.py").exists()
     migrations = (temp_migrations_dir / "0002_delete_view.py").read()
     assert "DropView" in migrations
     assert "ViewDropRunPython" in migrations
@@ -167,24 +187,28 @@
     call_command("migrate", "test_app", "0001")
     assert is_view_exists(SimpleViewWithoutDependencies._meta.db_table)
 
 
 @pytest.mark.django_db(transaction=True)
 @roll_back_schema
 def test_drop_view_and_update_existing_view_in_same_migration(
-        temp_migrations_dir, SimpleViewWithoutDependencies, SecondSimpleViewWithoutDependencies
+    temp_migrations_dir,
+    SimpleViewWithoutDependencies,
+    SecondSimpleViewWithoutDependencies,
 ):
     call_command("makeviewmigrations", "test_app")
     assert (temp_migrations_dir / "0001_initial.py").exists()
     # Delete existing model
-    del apps.all_models['test_app'][SecondSimpleViewWithoutDependencies.__name__.lower()]
+    del apps.all_models["test_app"][
+        SecondSimpleViewWithoutDependencies.__name__.lower()
+    ]
     apps.clear_cache()
     DBViewsRegistry.pop(SecondSimpleViewWithoutDependencies._meta.db_table)
     # Modify existing model
-    apps.all_models['test_app']["simpleviewwithoutdependencies"].view_definition = """
+    apps.all_models["test_app"]["simpleviewwithoutdependencies"].view_definition = """
         Select *
          From  (values (3, 'dummy_3')) A(id, name)
     """
     # Run migration
     call_command("makeviewmigrations", "test_app", name="delete_view_and_update_view")
     assert (temp_migrations_dir / "0002_delete_view_and_update_view.py").exists()
     migrations = (temp_migrations_dir / "0002_delete_view_and_update_view.py").read()
@@ -192,59 +216,94 @@
     assert "ViewDropRunPython" in migrations
     assert "ViewRunPython" in migrations
 
 
 @pytest.mark.django_db(transaction=True)
 @roll_back_schema
 def test_drop_view_and_update_existing_view_in_next_migration(
-        temp_migrations_dir, SimpleViewWithoutDependencies, SecondSimpleViewWithoutDependencies
+    temp_migrations_dir,
+    SimpleViewWithoutDependencies,
+    SecondSimpleViewWithoutDependencies,
 ):
     call_command("makeviewmigrations", "test_app")
     assert (temp_migrations_dir / "0001_initial.py").exists()
     # Delete existing model
-    del apps.all_models['test_app'][SecondSimpleViewWithoutDependencies.__name__.lower()]
+    del apps.all_models["test_app"][
+        SecondSimpleViewWithoutDependencies.__name__.lower()
+    ]
     apps.clear_cache()
     DBViewsRegistry.pop(SecondSimpleViewWithoutDependencies._meta.db_table)
     # Run migration
     call_command("makeviewmigrations", "test_app", name="delete_view")
     assert (temp_migrations_dir / "0002_delete_view.py").exists()
     migrations = (temp_migrations_dir / "0002_delete_view.py").read()
     assert "DropView" in migrations
     assert "ViewDropRunPython" in migrations
     assert "ViewRunPython" not in migrations
     # Generate model representaions
     call_command("makemigrations", "test_app", name="create_models")
     # Modify existing model
-    apps.all_models['test_app']["simpleviewwithoutdependencies"].view_definition = """
+    apps.all_models["test_app"]["simpleviewwithoutdependencies"].view_definition = """
       Select *
          From  (values (3, 'dummy_3')) A(id, name)
     """
     call_command("makeviewmigrations", "test_app", name="update_view")
     assert (temp_migrations_dir / "0004_update_view.py").exists()
     migrations = (temp_migrations_dir / "0004_update_view.py").read()
     assert "ViewRunPython" in migrations
     assert "DropView" not in migrations
 
 
-@pytest.mark.django_db(databases=['sqlite', 'postgres'], transaction=True)
-@pytest.mark.parametrize("database", ['postgres', 'sqlite'])
+@pytest.mark.django_db(databases=["sqlite", "postgres"], transaction=True)
+@pytest.mark.parametrize("database", ["postgres", "sqlite"])
 @roll_back_schema
-def test_drop_view_multiple_engines(
-        temp_migrations_dir, database, MultipleDBRawView
-):
+def test_drop_view_multiple_engines(temp_migrations_dir, database, MultipleDBRawView):
     call_command("makeviewmigrations", "test_app")
     assert (temp_migrations_dir / "0001_initial.py").exists()
-    del apps.all_models['test_app'][MultipleDBRawView.__name__.lower()]
+    del apps.all_models["test_app"][MultipleDBRawView.__name__.lower()]
     apps.clear_cache()
     DBViewsRegistry.pop(MultipleDBRawView._meta.db_table)
     call_command("makeviewmigrations", "test_app", name="delete_view")
     assert (temp_migrations_dir / "0002_delete_view.py").exists()
     migrations = (temp_migrations_dir / "0002_delete_view.py").read()
     # both migrations are inside.
     assert "engine='django.db.backends.sqlite3" in migrations
     assert "engine='django.db.backends.postgresql" in migrations
     call_command("migrate", "test_app", "0001", database=database)
     assert is_view_exists(MultipleDBRawView._meta.db_table, using=database)
     call_command("migrate", "test_app", database=database)
     assert not is_view_exists(MultipleDBRawView._meta.db_table, using=database)
     call_command("migrate", "test_app", "0001", database=database)
     assert is_view_exists(MultipleDBRawView._meta.db_table, using=database)
+
+
+@pytest.mark.django_db(transaction=True)
+@roll_back_schema
+def test_support_view_migrations_wrapped_in_sparate_database_and_state(
+    temp_migrations_dir, SimpleViewWithoutDependencies
+):
+    initial_migration = temp_migrations_dir / "0001_initial.py"
+    with open(
+        get_base_path()
+        / "tests"
+        / "migrations_samples"
+        / "separate_database_and_state_migration.py"
+    ) as file:
+        initial_migration.write_text(file.read(), encoding="utf-8")
+    assert (temp_migrations_dir / "0001_initial.py").exists()
+    # No changes, no view migration created
+    call_command("makeviewmigrations", "test_app")
+    assert len(temp_migrations_dir.listdir()) == 2
+    # Modify simple view, view migration created
+    apps.all_models["test_app"]["simpleviewwithoutdependencies"].view_definition = """
+      Select *
+         From  (values (3, 'dummy_3')) A(id, name)
+    """
+    call_command("makeviewmigrations", "test_app")
+    assert len(temp_migrations_dir.listdir()) == 3
+    # migrate it
+    call_command("migrate", "test_app")
+    assert is_view_exists(SimpleViewWithoutDependencies._meta.db_table)
+    assert SimpleViewWithoutDependencies.objects.all().count() == 1
+    # check that backward capability works
+    call_command("migrate", "test_app", "0001")
+    assert SimpleViewWithoutDependencies.objects.all().count() == 2
```

### Comparing `django-db-views-0.1.6/tests/test_materialized_views.py` & `django-db-views-0.1.7/tests/test_materialized_views.py`

 * *Files identical despite different names*

