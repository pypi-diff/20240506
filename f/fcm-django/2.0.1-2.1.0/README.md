# Comparing `tmp/fcm-django-2.0.1.tar.gz` & `tmp/fcm_django-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fcm-django-2.0.1.tar", last modified: Sat Dec 30 18:17:08 2023, max compression
+gzip compressed data, was "fcm_django-2.1.0.tar", last modified: Mon May  6 10:32:15 2024, max compression
```

## Comparing `fcm-django-2.0.1.tar` & `fcm_django-2.1.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 mojcarojko   (501) staff       (20)        0 2023-12-30 18:17:08.992852 fcm-django-2.0.1/
--rw-r--r--   0 mojcarojko   (501) staff       (20)     1130 2023-04-05 08:36:57.000000 fcm-django-2.0.1/LICENSE.txt
--rw-r--r--   0 mojcarojko   (501) staff       (20)       55 2023-04-05 08:36:57.000000 fcm-django-2.0.1/MANIFEST.in
--rw-r--r--   0 mojcarojko   (501) staff       (20)     1098 2023-12-30 18:17:08.992534 fcm-django-2.0.1/PKG-INFO
--rw-r--r--   0 mojcarojko   (501) staff       (20)    14995 2023-12-30 18:15:06.000000 fcm-django-2.0.1/README.rst
-drwxr-xr-x   0 mojcarojko   (501) staff       (20)        0 2023-12-30 18:17:08.969978 fcm-django-2.0.1/fcm_django/
--rw-r--r--   0 mojcarojko   (501) staff       (20)      309 2023-12-30 18:15:40.000000 fcm-django-2.0.1/fcm_django/__init__.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)     8787 2023-04-05 08:36:57.000000 fcm-django-2.0.1/fcm_django/admin.py
-drwxr-xr-x   0 mojcarojko   (501) staff       (20)        0 2023-12-30 18:17:08.976828 fcm-django-2.0.1/fcm_django/api/
--rw-r--r--   0 mojcarojko   (501) staff       (20)      341 2023-04-05 08:36:57.000000 fcm-django-2.0.1/fcm_django/api/__init__.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)     5909 2023-04-05 08:36:57.000000 fcm-django-2.0.1/fcm_django/api/rest_framework.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)      806 2023-04-05 08:36:57.000000 fcm-django-2.0.1/fcm_django/api/tastypie.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)      207 2023-04-05 08:36:57.000000 fcm-django-2.0.1/fcm_django/apps.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)     4147 2023-04-05 08:36:57.000000 fcm-django-2.0.1/fcm_django/fields.py
-drwxr-xr-x   0 mojcarojko   (501) staff       (20)        0 2023-12-30 18:17:08.987417 fcm-django-2.0.1/fcm_django/migrations/
--rw-r--r--   0 mojcarojko   (501) staff       (20)     2555 2023-04-05 08:36:57.000000 fcm-django-2.0.1/fcm_django/migrations/0001_initial.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)      598 2023-04-05 08:36:57.000000 fcm-django-2.0.1/fcm_django/migrations/0002_auto_20160808_1645.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)      504 2023-04-05 08:36:57.000000 fcm-django-2.0.1/fcm_django/migrations/0003_auto_20170313_1314.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)      444 2023-04-05 08:36:57.000000 fcm-django-2.0.1/fcm_django/migrations/0004_auto_20181128_1642.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)      750 2023-04-05 08:36:57.000000 fcm-django-2.0.1/fcm_django/migrations/0005_auto_20170808_1145.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)      610 2023-04-05 08:36:57.000000 fcm-django-2.0.1/fcm_django/migrations/0006_auto_20210802_1140.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)      362 2023-04-05 08:36:57.000000 fcm-django-2.0.1/fcm_django/migrations/0007_auto_20211001_1440.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)      477 2023-04-05 08:36:57.000000 fcm-django-2.0.1/fcm_django/migrations/0008_auto_20211224_1205.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)      734 2023-04-05 08:36:57.000000 fcm-django-2.0.1/fcm_django/migrations/0009_alter_fcmdevice_user.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)     1233 2023-12-30 18:15:06.000000 fcm-django-2.0.1/fcm_django/migrations/0010_unique_registration_id.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)     1216 2023-12-30 18:15:06.000000 fcm-django-2.0.1/fcm_django/migrations/0011_fcmdevice_fcm_django_registration_id_user_id_idx.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)        0 2023-04-05 08:36:57.000000 fcm-django-2.0.1/fcm_django/migrations/__init__.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)    14143 2023-12-30 18:15:06.000000 fcm-django-2.0.1/fcm_django/models.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)      902 2023-05-05 08:22:10.000000 fcm-django-2.0.1/fcm_django/settings.py
-drwxr-xr-x   0 mojcarojko   (501) staff       (20)        0 2023-12-30 18:17:08.974158 fcm-django-2.0.1/fcm_django.egg-info/
--rw-r--r--   0 mojcarojko   (501) staff       (20)     1098 2023-12-30 18:17:08.000000 fcm-django-2.0.1/fcm_django.egg-info/PKG-INFO
--rw-r--r--   0 mojcarojko   (501) staff       (20)     1176 2023-12-30 18:17:08.000000 fcm-django-2.0.1/fcm_django.egg-info/SOURCES.txt
--rw-r--r--   0 mojcarojko   (501) staff       (20)        1 2023-12-30 18:17:08.000000 fcm-django-2.0.1/fcm_django.egg-info/dependency_links.txt
--rw-r--r--   0 mojcarojko   (501) staff       (20)       28 2023-12-30 18:17:08.000000 fcm-django-2.0.1/fcm_django.egg-info/requires.txt
--rw-r--r--   0 mojcarojko   (501) staff       (20)       48 2023-12-30 18:17:08.000000 fcm-django-2.0.1/fcm_django.egg-info/top_level.txt
--rw-r--r--   0 mojcarojko   (501) staff       (20)       94 2023-12-30 18:15:06.000000 fcm-django-2.0.1/pyproject.toml
--rw-r--r--   0 mojcarojko   (501) staff       (20)       67 2023-12-30 18:17:08.993782 fcm-django-2.0.1/setup.cfg
--rw-r--r--   0 mojcarojko   (501) staff       (20)     1378 2023-12-30 18:15:06.000000 fcm-django-2.0.1/setup.py
-drwxr-xr-x   0 mojcarojko   (501) staff       (20)        0 2023-12-30 18:17:08.991231 fcm-django-2.0.1/tests/
--rw-r--r--   0 mojcarojko   (501) staff       (20)      611 2023-12-30 18:15:06.000000 fcm-django-2.0.1/tests/test_admin.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)     1601 2023-12-30 18:15:06.000000 fcm-django-2.0.1/tests/test_api_rest_framework.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)      829 2023-12-30 18:15:06.000000 fcm-django-2.0.1/tests/test_api_tastypie.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)     5867 2023-12-30 18:15:06.000000 fcm-django-2.0.1/tests/test_models.py
--rw-r--r--   0 mojcarojko   (501) staff       (20)     1114 2023-12-30 18:15:06.000000 fcm-django-2.0.1/tests/testing_settings.py
+drwxr-xr-x   0 mojcarojko   (501) staff       (20)        0 2024-05-06 10:32:15.872022 fcm_django-2.1.0/
+-rw-r--r--   0 mojcarojko   (501) staff       (20)     1130 2023-04-05 08:36:57.000000 fcm_django-2.1.0/LICENSE.txt
+-rw-r--r--   0 mojcarojko   (501) staff       (20)       55 2023-04-05 08:36:57.000000 fcm_django-2.1.0/MANIFEST.in
+-rw-r--r--   0 mojcarojko   (501) staff       (20)     1100 2024-05-06 10:32:15.871769 fcm_django-2.1.0/PKG-INFO
+-rw-r--r--   0 mojcarojko   (501) staff       (20)    14995 2023-12-30 18:15:06.000000 fcm_django-2.1.0/README.rst
+drwxr-xr-x   0 mojcarojko   (501) staff       (20)        0 2024-05-06 10:32:15.851190 fcm_django-2.1.0/fcm_django/
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      309 2024-05-06 10:27:57.000000 fcm_django-2.1.0/fcm_django/__init__.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)     8771 2024-05-06 10:27:29.000000 fcm_django-2.1.0/fcm_django/admin.py
+drwxr-xr-x   0 mojcarojko   (501) staff       (20)        0 2024-05-06 10:32:15.856190 fcm_django-2.1.0/fcm_django/api/
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      341 2023-04-05 08:36:57.000000 fcm_django-2.1.0/fcm_django/api/__init__.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)     5909 2023-04-05 08:36:57.000000 fcm_django-2.1.0/fcm_django/api/rest_framework.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      806 2023-04-05 08:36:57.000000 fcm_django-2.1.0/fcm_django/api/tastypie.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      207 2023-04-05 08:36:57.000000 fcm_django-2.1.0/fcm_django/apps.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)     4147 2023-04-05 08:36:57.000000 fcm_django-2.1.0/fcm_django/fields.py
+drwxr-xr-x   0 mojcarojko   (501) staff       (20)        0 2024-05-06 10:32:15.864675 fcm_django-2.1.0/fcm_django/migrations/
+-rw-r--r--   0 mojcarojko   (501) staff       (20)     2555 2023-04-05 08:36:57.000000 fcm_django-2.1.0/fcm_django/migrations/0001_initial.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      598 2023-04-05 08:36:57.000000 fcm_django-2.1.0/fcm_django/migrations/0002_auto_20160808_1645.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      504 2023-04-05 08:36:57.000000 fcm_django-2.1.0/fcm_django/migrations/0003_auto_20170313_1314.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      444 2023-04-05 08:36:57.000000 fcm_django-2.1.0/fcm_django/migrations/0004_auto_20181128_1642.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      750 2023-04-05 08:36:57.000000 fcm_django-2.1.0/fcm_django/migrations/0005_auto_20170808_1145.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      610 2023-04-05 08:36:57.000000 fcm_django-2.1.0/fcm_django/migrations/0006_auto_20210802_1140.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      362 2023-04-05 08:36:57.000000 fcm_django-2.1.0/fcm_django/migrations/0007_auto_20211001_1440.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      477 2023-04-05 08:36:57.000000 fcm_django-2.1.0/fcm_django/migrations/0008_auto_20211224_1205.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      734 2023-04-05 08:36:57.000000 fcm_django-2.1.0/fcm_django/migrations/0009_alter_fcmdevice_user.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)     1233 2023-12-30 18:15:06.000000 fcm_django-2.1.0/fcm_django/migrations/0010_unique_registration_id.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)     1216 2023-12-30 18:15:06.000000 fcm_django-2.1.0/fcm_django/migrations/0011_fcmdevice_fcm_django_registration_id_user_id_idx.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)        0 2023-04-05 08:36:57.000000 fcm_django-2.1.0/fcm_django/migrations/__init__.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)    14147 2024-05-06 10:27:29.000000 fcm_django-2.1.0/fcm_django/models.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      902 2023-05-05 08:22:10.000000 fcm_django-2.1.0/fcm_django/settings.py
+drwxr-xr-x   0 mojcarojko   (501) staff       (20)        0 2024-05-06 10:32:15.870883 fcm_django-2.1.0/fcm_django.egg-info/
+-rw-r--r--   0 mojcarojko   (501) staff       (20)     1100 2024-05-06 10:32:15.000000 fcm_django-2.1.0/fcm_django.egg-info/PKG-INFO
+-rw-r--r--   0 mojcarojko   (501) staff       (20)     1176 2024-05-06 10:32:15.000000 fcm_django-2.1.0/fcm_django.egg-info/SOURCES.txt
+-rw-r--r--   0 mojcarojko   (501) staff       (20)        1 2024-05-06 10:32:15.000000 fcm_django-2.1.0/fcm_django.egg-info/dependency_links.txt
+-rw-r--r--   0 mojcarojko   (501) staff       (20)       30 2024-05-06 10:32:15.000000 fcm_django-2.1.0/fcm_django.egg-info/requires.txt
+-rw-r--r--   0 mojcarojko   (501) staff       (20)       48 2024-05-06 10:32:15.000000 fcm_django-2.1.0/fcm_django.egg-info/top_level.txt
+-rw-r--r--   0 mojcarojko   (501) staff       (20)       94 2023-12-30 18:15:06.000000 fcm_django-2.1.0/pyproject.toml
+-rw-r--r--   0 mojcarojko   (501) staff       (20)       67 2024-05-06 10:32:15.872896 fcm_django-2.1.0/setup.cfg
+-rw-r--r--   0 mojcarojko   (501) staff       (20)     1380 2024-05-06 10:27:29.000000 fcm_django-2.1.0/setup.py
+drwxr-xr-x   0 mojcarojko   (501) staff       (20)        0 2024-05-06 10:32:15.869849 fcm_django-2.1.0/tests/
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      611 2023-12-30 18:15:06.000000 fcm_django-2.1.0/tests/test_admin.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)     1601 2023-12-30 18:15:06.000000 fcm_django-2.1.0/tests/test_api_rest_framework.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      829 2023-12-30 18:15:06.000000 fcm_django-2.1.0/tests/test_api_tastypie.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)     5867 2023-12-30 18:15:06.000000 fcm_django-2.1.0/tests/test_models.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)     1114 2023-12-30 18:15:06.000000 fcm_django-2.1.0/tests/testing_settings.py
```

### Comparing `fcm-django-2.0.1/LICENSE.txt` & `fcm_django-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fcm-django-2.0.1/PKG-INFO` & `fcm_django-2.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fcm-django
-Version: 2.0.1
+Version: 2.1.0
 Summary: Send push notifications to mobile devices & browsers through FCM in Django.
 Home-page: https://github.com/xtrinch/fcm-django
 Download-URL: https://github.com/xtrinch/fcm-django/tarball/master
 Author: xTrinch
 Author-email: mojca.rojko@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -18,9 +18,9 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Networking
 Requires-Python: >=3.7
 License-File: LICENSE.txt
-Requires-Dist: firebase-admin<7,>=5
+Requires-Dist: firebase-admin<7,>=6.2
 Requires-Dist: Django
```

### Comparing `fcm-django-2.0.1/README.rst` & `fcm_django-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `fcm-django-2.0.1/fcm_django/admin.py` & `fcm_django-2.1.0/fcm_django/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
         "type",
         "user",
         "active",
         "date_created",
     )
     list_filter = (
         "active",
-        "user",
         "type",
     )
     actions = (
         "send_message",
         "send_bulk_message",
         "subscribe_to_topic",
         "bulk_subscribe_to_topic",
```

### Comparing `fcm-django-2.0.1/fcm_django/api/rest_framework.py` & `fcm_django-2.1.0/fcm_django/api/rest_framework.py`

 * *Files identical despite different names*

### Comparing `fcm-django-2.0.1/fcm_django/api/tastypie.py` & `fcm_django-2.1.0/fcm_django/api/tastypie.py`

 * *Files identical despite different names*

### Comparing `fcm-django-2.0.1/fcm_django/fields.py` & `fcm_django-2.1.0/fcm_django/fields.py`

 * *Files identical despite different names*

### Comparing `fcm-django-2.0.1/fcm_django/migrations/0001_initial.py` & `fcm_django-2.1.0/fcm_django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `fcm-django-2.0.1/fcm_django/migrations/0002_auto_20160808_1645.py` & `fcm_django-2.1.0/fcm_django/migrations/0002_auto_20160808_1645.py`

 * *Files identical despite different names*

### Comparing `fcm-django-2.0.1/fcm_django/migrations/0005_auto_20170808_1145.py` & `fcm_django-2.1.0/fcm_django/migrations/0005_auto_20170808_1145.py`

 * *Files identical despite different names*

### Comparing `fcm-django-2.0.1/fcm_django/migrations/0006_auto_20210802_1140.py` & `fcm_django-2.1.0/fcm_django/migrations/0006_auto_20210802_1140.py`

 * *Files identical despite different names*

### Comparing `fcm-django-2.0.1/fcm_django/migrations/0009_alter_fcmdevice_user.py` & `fcm_django-2.1.0/fcm_django/migrations/0009_alter_fcmdevice_user.py`

 * *Files identical despite different names*

### Comparing `fcm-django-2.0.1/fcm_django/migrations/0010_unique_registration_id.py` & `fcm_django-2.1.0/fcm_django/migrations/0010_unique_registration_id.py`

 * *Files identical despite different names*

### Comparing `fcm-django-2.0.1/fcm_django/migrations/0011_fcmdevice_fcm_django_registration_id_user_id_idx.py` & `fcm_django-2.1.0/fcm_django/migrations/0011_fcmdevice_fcm_django_registration_id_user_id_idx.py`

 * *Files identical despite different names*

### Comparing `fcm-django-2.0.1/fcm_django/models.py` & `fcm_django-2.1.0/fcm_django/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,25 +127,25 @@
         additional_registration_ids: Sequence[str] = None,
         app: "firebase_admin.App" = SETTINGS["DEFAULT_FIREBASE_APP"],
         **more_send_message_kwargs,
     ) -> FirebaseResponseDict:
         """
         Send notification of single message for all active devices in
         queryset and deactivate if DELETE_INACTIVE_DEVICES setting is set to True.
-        Bulk sends using firebase.messaging.send_all. For every 500 messages, we send a
+        Bulk sends using firebase.messaging.send_each. For every 500 messages, we send a
         single HTTP request to Firebase (the 500 is set by the firebase-sdk).
 
         :param message: firebase.messaging.Message. If `message` includes a token/id, it
         will be overridden.
         :param skip_registration_id_lookup: skips the QuerySet lookup and solely uses
         the list of IDs from additional_registration_ids
         :param additional_registration_ids: specific registration_ids to add to the
         :param app: firebase_admin.App. Specify a specific app to use
         QuerySet lookup
-        :param more_send_message_kwargs: Parameters for firebase.messaging.send_all()
+        :param more_send_message_kwargs: Parameters for firebase.messaging.send_each()
         - dry_run: bool. Whether to actually send the notification to the device
         If there are any new parameters, you can still specify them here.
 
         :raises FirebaseError
         :returns FirebaseResponseDict
         """
         registration_ids = self.get_registration_ids(
@@ -157,15 +157,15 @@
         responses: List[messaging.SendResponse] = []
         for i in range(0, len(registration_ids), MAX_MESSAGES_PER_BATCH):
             messages = [
                 self._prepare_message(message, token)
                 for token in registration_ids[i : i + MAX_MESSAGES_PER_BATCH]
             ]
             responses.extend(
-                messaging.send_all(
+                messaging.send_each(
                     messages, app=app, **more_send_message_kwargs
                 ).responses
             )
         return FirebaseResponseDict(
             response=messaging.BatchResponse(responses),
             registration_ids_sent=registration_ids,
             deactivated_registration_ids=self.deactivate_devices_with_error_results(
@@ -298,15 +298,15 @@
         """
         Send single message. The message's token should be blank (and will be
         overridden if not). Responds with message ID string.
 
         :param message: firebase.messaging.Message. If `message` includes a token/id, it
         will be overridden.
         :param app: firebase_admin.App. Specify a specific app to use
-        :param more_send_message_kwargs: Parameters for firebase.messaging.send_all()
+        :param more_send_message_kwargs: Parameters for firebase.messaging.send_each()
         - dry_run: bool. Whether to actually send the notification to the device
         If there are any new parameters, you can still specify them here.
 
         :raises FirebaseError
         :returns messaging.SendResponse or FirebaseError if the device was
         deactivated due to an error.
         """
```

### Comparing `fcm-django-2.0.1/fcm_django/settings.py` & `fcm_django-2.1.0/fcm_django/settings.py`

 * *Files identical despite different names*

### Comparing `fcm-django-2.0.1/fcm_django.egg-info/PKG-INFO` & `fcm_django-2.1.0/fcm_django.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fcm-django
-Version: 2.0.1
+Version: 2.1.0
 Summary: Send push notifications to mobile devices & browsers through FCM in Django.
 Home-page: https://github.com/xtrinch/fcm-django
 Download-URL: https://github.com/xtrinch/fcm-django/tarball/master
 Author: xTrinch
 Author-email: mojca.rojko@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -18,9 +18,9 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Networking
 Requires-Python: >=3.7
 License-File: LICENSE.txt
-Requires-Dist: firebase-admin<7,>=5
+Requires-Dist: firebase-admin<7,>=6.2
 Requires-Dist: Django
```

### Comparing `fcm-django-2.0.1/fcm_django.egg-info/SOURCES.txt` & `fcm_django-2.1.0/fcm_django.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fcm-django-2.0.1/setup.py` & `fcm_django-2.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     name="fcm-django",
     packages=[
         "fcm_django",
         "fcm_django/api",
         "fcm_django/migrations",
     ],
     python_requires=">=3.7",
-    install_requires=["firebase-admin>=5,<7", "Django"],
+    install_requires=["firebase-admin>=6.2,<7", "Django"],
     author=fcm_django.__author__,
     author_email=fcm_django.__email__,
     classifiers=CLASSIFIERS,
     description="Send push notifications to mobile devices & browsers through "
     "FCM in Django.",
     download_url="https://github.com/xtrinch/fcm-django/tarball/master",
     long_description="",
```

### Comparing `fcm-django-2.0.1/tests/test_admin.py` & `fcm_django-2.1.0/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `fcm-django-2.0.1/tests/test_api_rest_framework.py` & `fcm_django-2.1.0/tests/test_api_rest_framework.py`

 * *Files identical despite different names*

### Comparing `fcm-django-2.0.1/tests/test_api_tastypie.py` & `fcm_django-2.1.0/tests/test_api_tastypie.py`

 * *Files identical despite different names*

### Comparing `fcm-django-2.0.1/tests/test_models.py` & `fcm_django-2.1.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `fcm-django-2.0.1/tests/testing_settings.py` & `fcm_django-2.1.0/tests/testing_settings.py`

 * *Files identical despite different names*

