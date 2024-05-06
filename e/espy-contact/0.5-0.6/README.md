# Comparing `tmp/espy_contact-0.5.tar.gz` & `tmp/espy_contact-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "espy_contact-0.5.tar", last modified: Sun Apr 28 04:34:07 2024, max compression
+gzip compressed data, was "espy_contact-0.6.tar", last modified: Sun May  5 21:18:08 2024, max compression
```

## Comparing `espy_contact-0.5.tar` & `espy_contact-0.6.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-28 04:34:07.157266 espy_contact-0.5/
--rw-r--r--   0 philipadigun   (501) staff       (20)     1072 2024-04-26 01:29:16.000000 espy_contact-0.5/LICENSE
--rw-r--r--   0 philipadigun   (501) staff       (20)      348 2024-04-28 04:34:07.157119 espy_contact-0.5/PKG-INFO
--rw-r--r--   0 philipadigun   (501) staff       (20)      109 2024-04-27 15:25:29.000000 espy_contact-0.5/README.md
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-28 04:34:07.150799 espy_contact-0.5/espy_contact/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-0.5/espy_contact/__init__.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-28 04:34:07.152432 espy_contact-0.5/espy_contact/model/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:34:03.000000 espy_contact-0.5/espy_contact/model/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     9835 2024-04-28 04:32:29.000000 espy_contact-0.5/espy_contact/model/campus.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      558 2024-04-28 03:38:46.000000 espy_contact-0.5/espy_contact/model/messaging.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     2616 2024-04-28 04:30:37.000000 espy_contact-0.5/espy_contact/model/models.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1821 2024-04-28 03:38:03.000000 espy_contact-0.5/espy_contact/model/tranx.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-28 04:34:07.153930 espy_contact-0.5/espy_contact/schema/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-27 05:18:23.000000 espy_contact-0.5/espy_contact/schema/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     2200 2024-04-28 03:20:57.000000 espy_contact-0.5/espy_contact/schema/campus.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      295 2024-04-28 00:12:40.000000 espy_contact-0.5/espy_contact/schema/messaging.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     5759 2024-04-28 03:39:29.000000 espy_contact-0.5/espy_contact/schema/mgcampus.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     3204 2024-04-28 03:14:05.000000 espy_contact-0.5/espy_contact/schema/schema.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      932 2024-04-28 03:35:00.000000 espy_contact-0.5/espy_contact/schema/tranx.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-28 04:34:07.154256 espy_contact-0.5/espy_contact/service/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-28 00:08:44.000000 espy_contact-0.5/espy_contact/service/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1574 2024-04-27 02:59:30.000000 espy_contact-0.5/espy_contact/service/service.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-28 04:34:07.156091 espy_contact-0.5/espy_contact/util/
--rw-r--r--   0 philipadigun   (501) staff       (20)      959 2024-04-26 03:59:10.000000 espy_contact-0.5/espy_contact/util/CONSTANTS.py
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:33:54.000000 espy_contact-0.5/espy_contact/util/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     3680 2024-04-28 03:56:06.000000 espy_contact-0.5/espy_contact/util/converter.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      184 2024-04-28 03:04:46.000000 espy_contact-0.5/espy_contact/util/db.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     3777 2024-04-26 01:33:55.000000 espy_contact-0.5/espy_contact/util/enums.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     4356 2024-04-28 00:38:37.000000 espy_contact-0.5/espy_contact/util/pg.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-28 04:34:07.151357 espy_contact-0.5/espy_contact.egg-info/
--rw-r--r--   0 philipadigun   (501) staff       (20)      348 2024-04-28 04:34:07.000000 espy_contact-0.5/espy_contact.egg-info/PKG-INFO
--rw-r--r--   0 philipadigun   (501) staff       (20)      861 2024-04-28 04:34:07.000000 espy_contact-0.5/espy_contact.egg-info/SOURCES.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)        1 2024-04-28 04:34:07.000000 espy_contact-0.5/espy_contact.egg-info/dependency_links.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       76 2024-04-28 04:34:07.000000 espy_contact-0.5/espy_contact.egg-info/requires.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       19 2024-04-28 04:34:07.000000 espy_contact-0.5/espy_contact.egg-info/top_level.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       38 2024-04-28 04:34:07.157325 espy_contact-0.5/setup.cfg
--rw-r--r--   0 philipadigun   (501) staff       (20)      655 2024-04-28 04:33:47.000000 espy_contact-0.5/setup.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-04-28 04:34:07.156916 espy_contact-0.5/tests/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-0.5/tests/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1621 2024-04-26 01:31:37.000000 espy_contact-0.5/tests/test_copyright.py
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-0.5/tests/test_service.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-05 21:18:08.129056 espy_contact-0.6/
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1072 2024-04-26 01:29:16.000000 espy_contact-0.6/LICENSE
+-rw-r--r--   0 philipadigun   (501) staff       (20)      348 2024-05-05 21:18:08.128900 espy_contact-0.6/PKG-INFO
+-rw-r--r--   0 philipadigun   (501) staff       (20)      109 2024-04-27 15:25:29.000000 espy_contact-0.6/README.md
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-05 21:18:08.122130 espy_contact-0.6/espy_contact/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-0.6/espy_contact/__init__.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-05 21:18:08.124169 espy_contact-0.6/espy_contact/model/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:34:03.000000 espy_contact-0.6/espy_contact/model/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     9835 2024-04-28 04:32:29.000000 espy_contact-0.6/espy_contact/model/campus.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      558 2024-04-28 03:38:46.000000 espy_contact-0.6/espy_contact/model/messaging.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     2616 2024-05-04 04:42:58.000000 espy_contact-0.6/espy_contact/model/models.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     2419 2024-05-05 21:15:26.000000 espy_contact-0.6/espy_contact/model/reach.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1821 2024-04-28 03:38:03.000000 espy_contact-0.6/espy_contact/model/tranx.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-05 21:18:08.126652 espy_contact-0.6/espy_contact/schema/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-27 05:18:23.000000 espy_contact-0.6/espy_contact/schema/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     2200 2024-04-28 03:20:57.000000 espy_contact-0.6/espy_contact/schema/campus.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      295 2024-04-28 00:12:40.000000 espy_contact-0.6/espy_contact/schema/messaging.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     5759 2024-04-28 03:39:29.000000 espy_contact-0.6/espy_contact/schema/mgcampus.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      781 2024-05-05 21:16:38.000000 espy_contact-0.6/espy_contact/schema/reach.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     3204 2024-04-28 03:14:05.000000 espy_contact-0.6/espy_contact/schema/schema.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      932 2024-04-28 03:35:00.000000 espy_contact-0.6/espy_contact/schema/tranx.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-05 21:18:08.127011 espy_contact-0.6/espy_contact/service/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-28 00:08:44.000000 espy_contact-0.6/espy_contact/service/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1574 2024-04-27 02:59:30.000000 espy_contact-0.6/espy_contact/service/service.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-05 21:18:08.128115 espy_contact-0.6/espy_contact/util/
+-rw-r--r--   0 philipadigun   (501) staff       (20)      959 2024-04-26 03:59:10.000000 espy_contact-0.6/espy_contact/util/CONSTANTS.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:33:54.000000 espy_contact-0.6/espy_contact/util/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      184 2024-04-28 03:04:46.000000 espy_contact-0.6/espy_contact/util/db.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     3797 2024-05-04 04:43:43.000000 espy_contact-0.6/espy_contact/util/enums.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     4356 2024-05-04 17:13:08.000000 espy_contact-0.6/espy_contact/util/pg.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-05 21:18:08.122703 espy_contact-0.6/espy_contact.egg-info/
+-rw-r--r--   0 philipadigun   (501) staff       (20)      348 2024-05-05 21:18:08.000000 espy_contact-0.6/espy_contact.egg-info/PKG-INFO
+-rw-r--r--   0 philipadigun   (501) staff       (20)      887 2024-05-05 21:18:08.000000 espy_contact-0.6/espy_contact.egg-info/SOURCES.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)        1 2024-05-05 21:18:08.000000 espy_contact-0.6/espy_contact.egg-info/dependency_links.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       76 2024-05-05 21:18:08.000000 espy_contact-0.6/espy_contact.egg-info/requires.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       19 2024-05-05 21:18:08.000000 espy_contact-0.6/espy_contact.egg-info/top_level.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       38 2024-05-05 21:18:08.129112 espy_contact-0.6/setup.cfg
+-rw-r--r--   0 philipadigun   (501) staff       (20)      655 2024-05-05 21:17:46.000000 espy_contact-0.6/setup.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-05 21:18:08.128739 espy_contact-0.6/tests/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-0.6/tests/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1621 2024-04-26 01:31:37.000000 espy_contact-0.6/tests/test_copyright.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-0.6/tests/test_service.py
```

### Comparing `espy_contact-0.5/LICENSE` & `espy_contact-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `espy_contact-0.5/espy_contact/model/campus.py` & `espy_contact-0.6/espy_contact/model/campus.py`

 * *Files identical despite different names*

### Comparing `espy_contact-0.5/espy_contact/model/messaging.py` & `espy_contact-0.6/espy_contact/model/messaging.py`

 * *Files identical despite different names*

### Comparing `espy_contact-0.5/espy_contact/model/models.py` & `espy_contact-0.6/espy_contact/model/models.py`

 * *Files identical despite different names*

### Comparing `espy_contact-0.5/espy_contact/model/tranx.py` & `espy_contact-0.6/espy_contact/model/tranx.py`

 * *Files identical despite different names*

### Comparing `espy_contact-0.5/espy_contact/schema/campus.py` & `espy_contact-0.6/espy_contact/schema/campus.py`

 * *Files identical despite different names*

### Comparing `espy_contact-0.5/espy_contact/schema/mgcampus.py` & `espy_contact-0.6/espy_contact/schema/mgcampus.py`

 * *Files identical despite different names*

### Comparing `espy_contact-0.5/espy_contact/schema/schema.py` & `espy_contact-0.6/espy_contact/schema/schema.py`

 * *Files identical despite different names*

### Comparing `espy_contact-0.5/espy_contact/schema/tranx.py` & `espy_contact-0.6/espy_contact/schema/tranx.py`

 * *Files identical despite different names*

### Comparing `espy_contact-0.5/espy_contact/service/service.py` & `espy_contact-0.6/espy_contact/service/service.py`

 * *Files identical despite different names*

### Comparing `espy_contact-0.5/espy_contact/util/CONSTANTS.py` & `espy_contact-0.6/espy_contact/util/CONSTANTS.py`

 * *Files identical despite different names*

### Comparing `espy_contact-0.5/espy_contact/util/enums.py` & `espy_contact-0.6/espy_contact/util/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     USER = "User"
     GUEST = "Guest"
     PARENT = "Parent"
     TEACHER = "Teacher"
     ACCOUNT = "Account"
     REFEREE = "Referee"
     STUDENT = "Student"
+    STAFF = "Staff"
 
 
 class GradeLevel(enum.Enum):
     PRESCHOOL = "PRESCHOOL"
     DAYCARE = "DAYCARE"
     KG1 = "Kindgergaten 1"
     KG2 = "Kindergaten 2"
```

### Comparing `espy_contact-0.5/espy_contact/util/pg.py` & `espy_contact-0.6/espy_contact/util/pg.py`

 * *Files identical despite different names*

### Comparing `espy_contact-0.5/espy_contact.egg-info/SOURCES.txt` & `espy_contact-0.6/espy_contact.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,25 +7,26 @@
 espy_contact.egg-info/dependency_links.txt
 espy_contact.egg-info/requires.txt
 espy_contact.egg-info/top_level.txt
 espy_contact/model/__init__.py
 espy_contact/model/campus.py
 espy_contact/model/messaging.py
 espy_contact/model/models.py
+espy_contact/model/reach.py
 espy_contact/model/tranx.py
 espy_contact/schema/__init__.py
 espy_contact/schema/campus.py
 espy_contact/schema/messaging.py
 espy_contact/schema/mgcampus.py
+espy_contact/schema/reach.py
 espy_contact/schema/schema.py
 espy_contact/schema/tranx.py
 espy_contact/service/__init__.py
 espy_contact/service/service.py
 espy_contact/util/CONSTANTS.py
 espy_contact/util/__init__.py
-espy_contact/util/converter.py
 espy_contact/util/db.py
 espy_contact/util/enums.py
 espy_contact/util/pg.py
 tests/__init__.py
 tests/test_copyright.py
 tests/test_service.py
```

### Comparing `espy_contact-0.5/setup.py` & `espy_contact-0.6/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 VERSION = '0.0.2'
 DESCRIPTION = 'ESSL users management'
 LONG_DESCRIPTION = 'Internal helper package for ESSL users management'
 setup(
     name='espy_contact',
-    version='0.5',
+    version='0.6',
     packages=find_packages(),
     install_requires=[
         'bcrypt==4.1.2',
         'pytest==8.1.1',
         'pydantic==2.7.1',
         'sqlalchemy==2.0.29',
         'bson==0.5.10'
```

### Comparing `espy_contact-0.5/tests/test_copyright.py` & `espy_contact-0.6/tests/test_copyright.py`

 * *Files identical despite different names*

