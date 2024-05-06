# Comparing `tmp/itrm-0.1.1.tar.gz` & `tmp/itrm-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itrm-0.1.1.tar", last modified: Mon May  6 19:17:56 2024, max compression
+gzip compressed data, was "itrm-0.1.2.tar", last modified: Mon May  6 19:25:39 2024, max compression
```

## Comparing `itrm-0.1.1.tar` & `itrm-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 19:17:56.828937 itrm-0.1.1/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 itrm-0.1.1/LICENSE.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     8894 2024-05-06 19:17:56.828822 itrm-0.1.1/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     8437 2024-05-06 19:17:36.000000 itrm-0.1.1/README.md
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 itrm-0.1.1/pyproject.toml
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      579 2024-05-06 19:17:56.829162 itrm-0.1.1/setup.cfg
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 19:17:56.827186 itrm-0.1.1/src/
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 19:17:56.828620 itrm-0.1.1/src/itrm.egg-info/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     8894 2024-05-06 19:17:56.000000 itrm-0.1.1/src/itrm.egg-info/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      241 2024-05-06 19:17:56.000000 itrm-0.1.1/src/itrm.egg-info/SOURCES.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-05-06 19:17:56.000000 itrm-0.1.1/src/itrm.egg-info/dependency_links.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-05-06 19:17:56.000000 itrm-0.1.1/src/itrm.egg-info/requires.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2024-05-06 19:17:56.000000 itrm-0.1.1/src/itrm.egg-info/top_level.txt
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 19:17:56.828403 itrm-0.1.1/src/trm/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       54 2024-05-06 19:09:39.000000 itrm-0.1.1/src/trm/__init__.py
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    48555 2024-05-06 18:57:31.000000 itrm-0.1.1/src/trm/itrm.py
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 19:25:39.106707 itrm-0.1.2/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 itrm-0.1.2/LICENSE.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     8894 2024-05-06 19:25:39.106592 itrm-0.1.2/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     8437 2024-05-06 19:17:36.000000 itrm-0.1.2/README.md
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 itrm-0.1.2/pyproject.toml
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      579 2024-05-06 19:25:39.106936 itrm-0.1.2/setup.cfg
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 19:25:39.104223 itrm-0.1.2/src/
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 19:25:39.105214 itrm-0.1.2/src/itrm/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       54 2024-05-06 19:09:39.000000 itrm-0.1.2/src/itrm/__init__.py
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    48555 2024-05-06 18:57:31.000000 itrm-0.1.2/src/itrm/itrm.py
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 19:25:39.106394 itrm-0.1.2/src/itrm.egg-info/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     8894 2024-05-06 19:25:39.000000 itrm-0.1.2/src/itrm.egg-info/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      243 2024-05-06 19:25:39.000000 itrm-0.1.2/src/itrm.egg-info/SOURCES.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-05-06 19:25:39.000000 itrm-0.1.2/src/itrm.egg-info/dependency_links.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-05-06 19:25:39.000000 itrm-0.1.2/src/itrm.egg-info/requires.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        5 2024-05-06 19:25:39.000000 itrm-0.1.2/src/itrm.egg-info/top_level.txt
```

### Comparing `itrm-0.1.1/LICENSE.txt` & `itrm-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `itrm-0.1.1/PKG-INFO` & `itrm-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itrm
-Version: 0.1.1
+Version: 0.1.2
 Summary: Interactive Terminal Utilities
 Home-page: https://gitlab.com/davidwoodburn/itrm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `itrm-0.1.1/README.md` & `itrm-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `itrm-0.1.1/setup.cfg` & `itrm-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = itrm
-version = 0.1.1
+version = 0.1.2
 author = David Woodburn
 author_email = david.woodburn@icloud.com
 description = Interactive Terminal Utilities
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/davidwoodburn/itrm
 classifiers =
```

### Comparing `itrm-0.1.1/src/itrm.egg-info/PKG-INFO` & `itrm-0.1.2/src/itrm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itrm
-Version: 0.1.1
+Version: 0.1.2
 Summary: Interactive Terminal Utilities
 Home-page: https://gitlab.com/davidwoodburn/itrm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `itrm-0.1.1/src/trm/itrm.py` & `itrm-0.1.2/src/itrm/itrm.py`

 * *Files identical despite different names*

