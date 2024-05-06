# Comparing `tmp/itrm-0.1.7.tar.gz` & `tmp/itrm-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itrm-0.1.7.tar", last modified: Mon May  6 20:33:34 2024, max compression
+gzip compressed data, was "itrm-0.1.8.tar", last modified: Mon May  6 20:35:13 2024, max compression
```

## Comparing `itrm-0.1.7.tar` & `itrm-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 20:33:34.557486 itrm-0.1.7/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 itrm-0.1.7/LICENSE.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     8988 2024-05-06 20:33:34.557366 itrm-0.1.7/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     8531 2024-05-06 19:59:43.000000 itrm-0.1.7/README.md
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 itrm-0.1.7/pyproject.toml
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      579 2024-05-06 20:33:34.557735 itrm-0.1.7/setup.cfg
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 20:33:34.555518 itrm-0.1.7/src/
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 20:33:34.556353 itrm-0.1.7/src/itrm/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       54 2024-05-06 19:09:39.000000 itrm-0.1.7/src/itrm/__init__.py
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      308 2024-05-06 20:32:31.000000 itrm-0.1.7/src/itrm/eg_iplot.py
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    49282 2024-05-06 20:32:52.000000 itrm-0.1.7/src/itrm/itrm.py
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 20:33:34.557172 itrm-0.1.7/src/itrm.egg-info/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     8988 2024-05-06 20:33:34.000000 itrm-0.1.7/src/itrm.egg-info/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      264 2024-05-06 20:33:34.000000 itrm-0.1.7/src/itrm.egg-info/SOURCES.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-05-06 20:33:34.000000 itrm-0.1.7/src/itrm.egg-info/dependency_links.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-05-06 20:33:34.000000 itrm-0.1.7/src/itrm.egg-info/requires.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        5 2024-05-06 20:33:34.000000 itrm-0.1.7/src/itrm.egg-info/top_level.txt
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 20:35:13.140181 itrm-0.1.8/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 itrm-0.1.8/LICENSE.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     8988 2024-05-06 20:35:13.140050 itrm-0.1.8/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     8531 2024-05-06 19:59:43.000000 itrm-0.1.8/README.md
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 itrm-0.1.8/pyproject.toml
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      579 2024-05-06 20:35:13.140445 itrm-0.1.8/setup.cfg
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 20:35:13.138035 itrm-0.1.8/src/
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 20:35:13.138831 itrm-0.1.8/src/itrm/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       54 2024-05-06 19:09:39.000000 itrm-0.1.8/src/itrm/__init__.py
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      308 2024-05-06 20:32:31.000000 itrm-0.1.8/src/itrm/eg_iplot.py
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    49282 2024-05-06 20:32:52.000000 itrm-0.1.8/src/itrm/itrm.py
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 20:35:13.139755 itrm-0.1.8/src/itrm.egg-info/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     8988 2024-05-06 20:35:13.000000 itrm-0.1.8/src/itrm.egg-info/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      264 2024-05-06 20:35:13.000000 itrm-0.1.8/src/itrm.egg-info/SOURCES.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-05-06 20:35:13.000000 itrm-0.1.8/src/itrm.egg-info/dependency_links.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-05-06 20:35:13.000000 itrm-0.1.8/src/itrm.egg-info/requires.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        5 2024-05-06 20:35:13.000000 itrm-0.1.8/src/itrm.egg-info/top_level.txt
```

### Comparing `itrm-0.1.7/LICENSE.txt` & `itrm-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `itrm-0.1.7/PKG-INFO` & `itrm-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itrm
-Version: 0.1.7
+Version: 0.1.8
 Summary: Interactive Terminal Utilities
 Home-page: https://gitlab.com/davidwoodburn/itrm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `itrm-0.1.7/README.md` & `itrm-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `itrm-0.1.7/setup.cfg` & `itrm-0.1.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = itrm
-version = 0.1.7
+version = 0.1.8
 author = David Woodburn
 author_email = david.woodburn@icloud.com
 description = Interactive Terminal Utilities
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/davidwoodburn/itrm
 classifiers =
```

### Comparing `itrm-0.1.7/src/itrm/itrm.py` & `itrm-0.1.8/src/itrm/itrm.py`

 * *Files identical despite different names*

### Comparing `itrm-0.1.7/src/itrm.egg-info/PKG-INFO` & `itrm-0.1.8/src/itrm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itrm
-Version: 0.1.7
+Version: 0.1.8
 Summary: Interactive Terminal Utilities
 Home-page: https://gitlab.com/davidwoodburn/itrm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

