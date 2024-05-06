# Comparing `tmp/skysurvey_sniapop-0.3.0.tar.gz` & `tmp/skysurvey_sniapop-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skysurvey_sniapop-0.3.0.tar", last modified: Wed Dec 13 10:37:36 2023, max compression
+gzip compressed data, was "skysurvey_sniapop-0.3.1.tar", last modified: Mon May  6 18:42:57 2024, max compression
```

## Comparing `skysurvey_sniapop-0.3.0.tar` & `skysurvey_sniapop-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-12-13 10:37:36.394071 skysurvey_sniapop-0.3.0/
--rw-r--r--   0 rigault   (2358) staff       (20)    11357 2023-11-18 15:23:02.000000 skysurvey_sniapop-0.3.0/LICENSE
--rw-r--r--   0 rigault   (2358) staff       (20)     1043 2023-12-13 10:37:36.394021 skysurvey_sniapop-0.3.0/PKG-INFO
--rw-r--r--   0 rigault   (2358) staff       (20)      385 2023-11-20 08:50:08.000000 skysurvey_sniapop-0.3.0/README.md
--rw-r--r--   0 rigault   (2358) staff       (20)     1151 2023-12-13 10:37:36.394365 skysurvey_sniapop-0.3.0/setup.cfg
--rw-r--r--   0 rigault   (2358) staff       (20)       37 2023-11-18 15:23:42.000000 skysurvey_sniapop-0.3.0/setup.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-12-13 10:37:36.392437 skysurvey_sniapop-0.3.0/skysurvey_sniapop/
--rw-r--r--   0 rigault   (2358) staff       (20)       67 2023-12-08 09:12:24.000000 skysurvey_sniapop-0.3.0/skysurvey_sniapop/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)     6034 2023-12-11 10:33:45.000000 skysurvey_sniapop-0.3.0/skysurvey_sniapop/agepop.py
--rw-r--r--   0 rigault   (2358) staff       (20)     4537 2023-12-08 08:24:54.000000 skysurvey_sniapop-0.3.0/skysurvey_sniapop/hostmass.py
--rw-r--r--   0 rigault   (2358) staff       (20)      592 2023-12-08 15:51:14.000000 skysurvey_sniapop-0.3.0/skysurvey_sniapop/lss.py
--rw-r--r--   0 rigault   (2358) staff       (20)     1787 2023-11-22 10:53:28.000000 skysurvey_sniapop-0.3.0/skysurvey_sniapop/magnitude.py
--rw-r--r--   0 rigault   (2358) staff       (20)     2209 2023-12-13 09:52:02.000000 skysurvey_sniapop-0.3.0/skysurvey_sniapop/models.py
--rw-r--r--   0 rigault   (2358) staff       (20)      387 2023-12-06 09:53:31.000000 skysurvey_sniapop-0.3.0/skysurvey_sniapop/utils.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-12-13 10:37:36.393643 skysurvey_sniapop-0.3.0/skysurvey_sniapop.egg-info/
--rw-r--r--   0 rigault   (2358) staff       (20)     1043 2023-12-13 10:37:36.000000 skysurvey_sniapop-0.3.0/skysurvey_sniapop.egg-info/PKG-INFO
--rw-r--r--   0 rigault   (2358) staff       (20)      479 2023-12-13 10:37:36.000000 skysurvey_sniapop-0.3.0/skysurvey_sniapop.egg-info/SOURCES.txt
--rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-12-13 10:37:36.000000 skysurvey_sniapop-0.3.0/skysurvey_sniapop.egg-info/dependency_links.txt
--rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-11-18 15:35:54.000000 skysurvey_sniapop-0.3.0/skysurvey_sniapop.egg-info/not-zip-safe
--rw-r--r--   0 rigault   (2358) staff       (20)      127 2023-12-13 10:37:36.000000 skysurvey_sniapop-0.3.0/skysurvey_sniapop.egg-info/requires.txt
--rw-r--r--   0 rigault   (2358) staff       (20)       18 2023-12-13 10:37:36.000000 skysurvey_sniapop-0.3.0/skysurvey_sniapop.egg-info/top_level.txt
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2024-05-06 18:42:57.464811 skysurvey_sniapop-0.3.1/
+-rw-r--r--   0 rigault   (2358) staff       (20)    11357 2023-11-18 15:23:02.000000 skysurvey_sniapop-0.3.1/LICENSE
+-rw-r--r--   0 rigault   (2358) staff       (20)     1043 2024-05-06 18:42:57.464756 skysurvey_sniapop-0.3.1/PKG-INFO
+-rw-r--r--   0 rigault   (2358) staff       (20)      385 2023-11-20 08:50:08.000000 skysurvey_sniapop-0.3.1/README.md
+-rw-r--r--   0 rigault   (2358) staff       (20)     1151 2024-05-06 18:42:57.465087 skysurvey_sniapop-0.3.1/setup.cfg
+-rw-r--r--   0 rigault   (2358) staff       (20)       37 2023-11-18 15:23:42.000000 skysurvey_sniapop-0.3.1/setup.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2024-05-06 18:42:57.463296 skysurvey_sniapop-0.3.1/skysurvey_sniapop/
+-rw-r--r--   0 rigault   (2358) staff       (20)       70 2024-05-06 18:41:56.000000 skysurvey_sniapop-0.3.1/skysurvey_sniapop/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     6034 2023-12-11 10:33:45.000000 skysurvey_sniapop-0.3.1/skysurvey_sniapop/agepop.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     4537 2023-12-08 08:24:54.000000 skysurvey_sniapop-0.3.1/skysurvey_sniapop/hostmass.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      592 2023-12-08 15:51:14.000000 skysurvey_sniapop-0.3.1/skysurvey_sniapop/lss.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     1787 2023-11-22 10:53:28.000000 skysurvey_sniapop-0.3.1/skysurvey_sniapop/magnitude.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     2209 2023-12-13 09:52:02.000000 skysurvey_sniapop-0.3.1/skysurvey_sniapop/models.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      387 2023-12-06 09:53:31.000000 skysurvey_sniapop-0.3.1/skysurvey_sniapop/utils.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2024-05-06 18:42:57.464369 skysurvey_sniapop-0.3.1/skysurvey_sniapop.egg-info/
+-rw-r--r--   0 rigault   (2358) staff       (20)     1043 2024-05-06 18:42:57.000000 skysurvey_sniapop-0.3.1/skysurvey_sniapop.egg-info/PKG-INFO
+-rw-r--r--   0 rigault   (2358) staff       (20)      479 2024-05-06 18:42:57.000000 skysurvey_sniapop-0.3.1/skysurvey_sniapop.egg-info/SOURCES.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)        1 2024-05-06 18:42:57.000000 skysurvey_sniapop-0.3.1/skysurvey_sniapop.egg-info/dependency_links.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-11-18 15:35:54.000000 skysurvey_sniapop-0.3.1/skysurvey_sniapop.egg-info/not-zip-safe
+-rw-r--r--   0 rigault   (2358) staff       (20)      127 2024-05-06 18:42:57.000000 skysurvey_sniapop-0.3.1/skysurvey_sniapop.egg-info/requires.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)       18 2024-05-06 18:42:57.000000 skysurvey_sniapop-0.3.1/skysurvey_sniapop.egg-info/top_level.txt
```

### Comparing `skysurvey_sniapop-0.3.0/LICENSE` & `skysurvey_sniapop-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `skysurvey_sniapop-0.3.0/PKG-INFO` & `skysurvey_sniapop-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skysurvey_sniapop
-Version: 0.3.0
+Version: 0.3.1
 Summary: Extension of skysurvey for Type Ia supernovae modelling
 Home-page: https://github.com/MickaelRigault/skysurvey-sniapop
 Author: Mickael Rigault
 Author-email: m.rigault@ipnl.in2p3.fr
 License: Apache Software License
 Keywords: astronomy,astrophysics
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `skysurvey_sniapop-0.3.0/setup.cfg` & `skysurvey_sniapop-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `skysurvey_sniapop-0.3.0/skysurvey_sniapop/agepop.py` & `skysurvey_sniapop-0.3.1/skysurvey_sniapop/agepop.py`

 * *Files identical despite different names*

### Comparing `skysurvey_sniapop-0.3.0/skysurvey_sniapop/hostmass.py` & `skysurvey_sniapop-0.3.1/skysurvey_sniapop/hostmass.py`

 * *Files identical despite different names*

### Comparing `skysurvey_sniapop-0.3.0/skysurvey_sniapop/lss.py` & `skysurvey_sniapop-0.3.1/skysurvey_sniapop/lss.py`

 * *Files identical despite different names*

### Comparing `skysurvey_sniapop-0.3.0/skysurvey_sniapop/magnitude.py` & `skysurvey_sniapop-0.3.1/skysurvey_sniapop/magnitude.py`

 * *Files identical despite different names*

### Comparing `skysurvey_sniapop-0.3.0/skysurvey_sniapop/models.py` & `skysurvey_sniapop-0.3.1/skysurvey_sniapop/models.py`

 * *Files identical despite different names*

### Comparing `skysurvey_sniapop-0.3.0/skysurvey_sniapop.egg-info/PKG-INFO` & `skysurvey_sniapop-0.3.1/skysurvey_sniapop.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: skysurvey-sniapop
-Version: 0.3.0
+Name: skysurvey_sniapop
+Version: 0.3.1
 Summary: Extension of skysurvey for Type Ia supernovae modelling
 Home-page: https://github.com/MickaelRigault/skysurvey-sniapop
 Author: Mickael Rigault
 Author-email: m.rigault@ipnl.in2p3.fr
 License: Apache Software License
 Keywords: astronomy,astrophysics
 Classifier: Development Status :: 2 - Pre-Alpha
```

