# Comparing `tmp/skytek-utils-0.9.1.tar.gz` & `tmp/skytek_utils-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skytek-utils-0.9.1.tar", last modified: Mon Oct 16 21:41:41 2023, max compression
+gzip compressed data, was "skytek_utils-0.9.2.tar", last modified: Mon May  6 18:46:47 2024, max compression
```

## Comparing `skytek-utils-0.9.1.tar` & `skytek_utils-0.9.2.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 21:41:41.424003 skytek-utils-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2023-10-16 21:41:32.000000 skytek-utils-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      128 2023-10-16 21:41:32.000000 skytek-utils-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      773 2023-10-16 21:41:41.424003 skytek-utils-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-10-16 21:41:32.000000 skytek-utils-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-10-16 21:41:32.000000 skytek-utils-0.9.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 21:41:41.416003 skytek-utils-0.9.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2023-10-16 21:41:32.000000 skytek-utils-0.9.1/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-10-16 21:41:32.000000 skytek-utils-0.9.1/requirements/lint.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2023-10-16 21:41:32.000000 skytek-utils-0.9.1/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-16 21:41:41.428003 skytek-utils-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2023-10-16 21:41:32.000000 skytek-utils-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 21:41:41.420003 skytek-utils-0.9.1/skytek_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-10-16 21:41:34.000000 skytek-utils-0.9.1/skytek_utils/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      206 2023-10-16 21:41:32.000000 skytek-utils-0.9.1/skytek_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2023-10-16 21:41:32.000000 skytek-utils-0.9.1/skytek_utils/celery.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2023-10-16 21:41:32.000000 skytek-utils-0.9.1/skytek_utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 21:41:41.420003 skytek-utils-0.9.1/skytek_utils/django/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 21:41:32.000000 skytek-utils-0.9.1/skytek_utils/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2023-10-16 21:41:32.000000 skytek-utils-0.9.1/skytek_utils/django/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2023-10-16 21:41:32.000000 skytek-utils-0.9.1/skytek_utils/django/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2023-10-16 21:41:32.000000 skytek-utils-0.9.1/skytek_utils/django/shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2023-10-16 21:41:32.000000 skytek-utils-0.9.1/skytek_utils/files.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 21:41:41.420003 skytek-utils-0.9.1/skytek_utils/interconnect/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 21:41:32.000000 skytek-utils-0.9.1/skytek_utils/interconnect/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 21:41:41.424003 skytek-utils-0.9.1/skytek_utils/interconnect/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 21:41:32.000000 skytek-utils-0.9.1/skytek_utils/interconnect/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2023-10-16 21:41:32.000000 skytek-utils-0.9.1/skytek_utils/interconnect/api/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2023-10-16 21:41:32.000000 skytek-utils-0.9.1/skytek_utils/interconnect/api/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2023-10-16 21:41:32.000000 skytek-utils-0.9.1/skytek_utils/interconnect/api/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2023-10-16 21:41:32.000000 skytek-utils-0.9.1/skytek_utils/interconnect/api/jwt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2023-10-16 21:41:32.000000 skytek-utils-0.9.1/skytek_utils/interconnect/api/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2023-10-16 21:41:32.000000 skytek-utils-0.9.1/skytek_utils/interconnect/api/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2023-10-16 21:41:32.000000 skytek-utils-0.9.1/skytek_utils/interconnect/api/user.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2023-10-16 21:41:32.000000 skytek-utils-0.9.1/skytek_utils/iter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2023-10-16 21:41:32.000000 skytek-utils-0.9.1/skytek_utils/monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 21:41:41.424003 skytek-utils-0.9.1/skytek_utils/spatial/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 21:41:32.000000 skytek-utils-0.9.1/skytek_utils/spatial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2023-10-16 21:41:32.000000 skytek-utils-0.9.1/skytek_utils/spatial/tiles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 21:41:41.420003 skytek-utils-0.9.1/skytek_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2023-10-16 21:41:41.000000 skytek-utils-0.9.1/skytek_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-10-16 21:41:41.000000 skytek-utils-0.9.1/skytek_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-16 21:41:41.000000 skytek-utils-0.9.1/skytek_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-16 21:41:41.000000 skytek-utils-0.9.1/skytek_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      119 2023-10-16 21:41:41.000000 skytek-utils-0.9.1/skytek_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-10-16 21:41:41.000000 skytek-utils-0.9.1/skytek_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 21:41:41.424003 skytek-utils-0.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2023-10-16 21:41:32.000000 skytek-utils-0.9.1/tests/test_iter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:46:47.974705 skytek_utils-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-05-06 18:46:42.000000 skytek_utils-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-06 18:46:42.000000 skytek_utils-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-06 18:46:47.974705 skytek_utils-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-06 18:46:42.000000 skytek_utils-0.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-06 18:46:42.000000 skytek_utils-0.9.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:46:47.970705 skytek_utils-0.9.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-06 18:46:42.000000 skytek_utils-0.9.2/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-06 18:46:42.000000 skytek_utils-0.9.2/requirements/lint.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-06 18:46:42.000000 skytek_utils-0.9.2/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 18:46:47.974705 skytek_utils-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-06 18:46:42.000000 skytek_utils-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:46:47.970705 skytek_utils-0.9.2/skytek_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-06 18:46:46.000000 skytek_utils-0.9.2/skytek_utils/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-06 18:46:42.000000 skytek_utils-0.9.2/skytek_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-06 18:46:42.000000 skytek_utils-0.9.2/skytek_utils/celery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-06 18:46:42.000000 skytek_utils-0.9.2/skytek_utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:46:47.974705 skytek_utils-0.9.2/skytek_utils/django/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 18:46:42.000000 skytek_utils-0.9.2/skytek_utils/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-06 18:46:42.000000 skytek_utils-0.9.2/skytek_utils/django/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-06 18:46:42.000000 skytek_utils-0.9.2/skytek_utils/django/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-06 18:46:42.000000 skytek_utils-0.9.2/skytek_utils/django/shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-06 18:46:42.000000 skytek_utils-0.9.2/skytek_utils/files.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:46:47.974705 skytek_utils-0.9.2/skytek_utils/interconnect/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 18:46:42.000000 skytek_utils-0.9.2/skytek_utils/interconnect/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:46:47.974705 skytek_utils-0.9.2/skytek_utils/interconnect/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 18:46:42.000000 skytek_utils-0.9.2/skytek_utils/interconnect/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-06 18:46:42.000000 skytek_utils-0.9.2/skytek_utils/interconnect/api/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-05-06 18:46:42.000000 skytek_utils-0.9.2/skytek_utils/interconnect/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-06 18:46:42.000000 skytek_utils-0.9.2/skytek_utils/interconnect/api/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-06 18:46:42.000000 skytek_utils-0.9.2/skytek_utils/interconnect/api/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-06 18:46:42.000000 skytek_utils-0.9.2/skytek_utils/interconnect/api/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-06 18:46:42.000000 skytek_utils-0.9.2/skytek_utils/interconnect/api/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-06 18:46:42.000000 skytek_utils-0.9.2/skytek_utils/interconnect/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-06 18:46:42.000000 skytek_utils-0.9.2/skytek_utils/iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-06 18:46:42.000000 skytek_utils-0.9.2/skytek_utils/monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:46:47.974705 skytek_utils-0.9.2/skytek_utils/spatial/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 18:46:42.000000 skytek_utils-0.9.2/skytek_utils/spatial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-06 18:46:42.000000 skytek_utils-0.9.2/skytek_utils/spatial/tiles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:46:47.974705 skytek_utils-0.9.2/skytek_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-06 18:46:47.000000 skytek_utils-0.9.2/skytek_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-06 18:46:47.000000 skytek_utils-0.9.2/skytek_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 18:46:47.000000 skytek_utils-0.9.2/skytek_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 18:46:47.000000 skytek_utils-0.9.2/skytek_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-06 18:46:47.000000 skytek_utils-0.9.2/skytek_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-06 18:46:47.000000 skytek_utils-0.9.2/skytek_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:46:47.974705 skytek_utils-0.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-06 18:46:42.000000 skytek_utils-0.9.2/tests/test_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-06 18:46:42.000000 skytek_utils-0.9.2/tests/test_iter.py
```

### Comparing `skytek-utils-0.9.1/LICENSE` & `skytek_utils-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.9.1/PKG-INFO` & `skytek_utils-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skytek-utils
-Version: 0.9.1
+Version: 0.9.2
 Summary: skytek-utils - a set of small util functions
 Home-page: http://github.com/Skytek/skytek-utils
 Author: Skytek Ltd.
 Author-email: wiktor.latanowicz@skytek.com
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `skytek-utils-0.9.1/setup.py` & `skytek_utils-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.9.1/skytek_utils/celery.py` & `skytek_utils-0.9.2/skytek_utils/celery.py`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.9.1/skytek_utils/datetime.py` & `skytek_utils-0.9.2/skytek_utils/datetime.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-from datetime import datetime, timedelta
+from datetime import date, datetime, timedelta
 from typing import Generator, Optional, Tuple, Union
 
 from dateutil.parser import parse
 
 
 def ensure_datetime(value: Optional[Union[str, datetime]]):
     if value is None:
         return value
 
     if isinstance(value, datetime):
         return value
 
+    if isinstance(value, date):
+        return datetime.combine(value, datetime.min.time())
+
     return parse(value)
 
 
 def datetime_range(
     start: Optional[datetime], end: Optional[datetime], step: timedelta
 ) -> Generator[Tuple[Optional[datetime], Optional[datetime]], None, None]:
     if start is None or end is None:
```

### Comparing `skytek-utils-0.9.1/skytek_utils/django/shortcuts.py` & `skytek_utils-0.9.2/skytek_utils/django/shortcuts.py`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.9.1/skytek_utils/interconnect/api/authentication.py` & `skytek_utils-0.9.2/skytek_utils/interconnect/api/authentication.py`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.9.1/skytek_utils/interconnect/api/client.py` & `skytek_utils-0.9.2/skytek_utils/interconnect/api/client.py`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.9.1/skytek_utils/interconnect/api/conf.py` & `skytek_utils-0.9.2/skytek_utils/interconnect/api/conf.py`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.9.1/skytek_utils/interconnect/api/jwt.py` & `skytek_utils-0.9.2/skytek_utils/interconnect/api/jwt.py`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.9.1/skytek_utils/interconnect/api/mixins.py` & `skytek_utils-0.9.2/skytek_utils/interconnect/api/mixins.py`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.9.1/skytek_utils/interconnect/api/permissions.py` & `skytek_utils-0.9.2/skytek_utils/interconnect/api/permissions.py`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.9.1/skytek_utils/monitoring.py` & `skytek_utils-0.9.2/skytek_utils/monitoring.py`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.9.1/skytek_utils/spatial/tiles.py` & `skytek_utils-0.9.2/skytek_utils/spatial/tiles.py`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.9.1/skytek_utils.egg-info/PKG-INFO` & `skytek_utils-0.9.2/skytek_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skytek-utils
-Version: 0.9.1
+Version: 0.9.2
 Summary: skytek-utils - a set of small util functions
 Home-page: http://github.com/Skytek/skytek-utils
 Author: Skytek Ltd.
 Author-email: wiktor.latanowicz@skytek.com
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `skytek-utils-0.9.1/skytek_utils.egg-info/SOURCES.txt` & `skytek_utils-0.9.2/skytek_utils.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -30,8 +30,9 @@
 skytek_utils/interconnect/api/conf.py
 skytek_utils/interconnect/api/jwt.py
 skytek_utils/interconnect/api/mixins.py
 skytek_utils/interconnect/api/permissions.py
 skytek_utils/interconnect/api/user.py
 skytek_utils/spatial/__init__.py
 skytek_utils/spatial/tiles.py
+tests/test_datetime.py
 tests/test_iter.py
```

### Comparing `skytek-utils-0.9.1/tests/test_iter.py` & `skytek_utils-0.9.2/tests/test_iter.py`

 * *Files identical despite different names*

