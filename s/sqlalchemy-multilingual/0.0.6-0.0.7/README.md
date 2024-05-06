# Comparing `tmp/sqlalchemy_multilingual-0.0.6.tar.gz` & `tmp/sqlalchemy_multilingual-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_multilingual-0.0.6.tar", last modified: Sun May  5 20:34:19 2024, max compression
+gzip compressed data, was "sqlalchemy_multilingual-0.0.7.tar", last modified: Sun May  5 20:38:50 2024, max compression
```

## Comparing `sqlalchemy_multilingual-0.0.6.tar` & `sqlalchemy_multilingual-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2024-05-05 20:34:19.472534 sqlalchemy_multilingual-0.0.6/
--rw-r--r--   0 vitya      (501) staff       (20)     1063 2024-05-05 20:11:04.000000 sqlalchemy_multilingual-0.0.6/LICENSE.txt
--rw-r--r--   0 vitya      (501) staff       (20)       34 2023-06-27 13:11:56.000000 sqlalchemy_multilingual-0.0.6/MANIFEST.in
--rw-r--r--   0 vitya      (501) staff       (20)      607 2024-05-05 20:34:19.472448 sqlalchemy_multilingual-0.0.6/PKG-INFO
--rw-r--r--   0 vitya      (501) staff       (20)        0 2024-05-05 19:57:01.000000 sqlalchemy_multilingual-0.0.6/README.md
--rw-r--r--   0 vitya      (501) staff       (20)      835 2024-05-05 20:34:17.000000 sqlalchemy_multilingual-0.0.6/pyproject.toml
--rw-r--r--   0 vitya      (501) staff       (20)      579 2024-05-05 20:34:19.472831 sqlalchemy_multilingual-0.0.6/setup.cfg
--rw-r--r--   0 vitya      (501) staff       (20)      235 2024-05-05 20:29:38.000000 sqlalchemy_multilingual-0.0.6/setup.py
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2024-05-05 20:34:19.472228 sqlalchemy_multilingual-0.0.6/sqlalchemy_multilingual.egg-info/
--rw-r--r--   0 vitya      (501) staff       (20)      607 2024-05-05 20:34:19.000000 sqlalchemy_multilingual-0.0.6/sqlalchemy_multilingual.egg-info/PKG-INFO
--rw-r--r--   0 vitya      (501) staff       (20)      301 2024-05-05 20:34:19.000000 sqlalchemy_multilingual-0.0.6/sqlalchemy_multilingual.egg-info/SOURCES.txt
--rw-r--r--   0 vitya      (501) staff       (20)        1 2024-05-05 20:34:19.000000 sqlalchemy_multilingual-0.0.6/sqlalchemy_multilingual.egg-info/dependency_links.txt
--rw-r--r--   0 vitya      (501) staff       (20)       43 2024-05-05 20:34:19.000000 sqlalchemy_multilingual-0.0.6/sqlalchemy_multilingual.egg-info/requires.txt
--rw-r--r--   0 vitya      (501) staff       (20)        1 2024-05-05 20:34:19.000000 sqlalchemy_multilingual-0.0.6/sqlalchemy_multilingual.egg-info/top_level.txt
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2024-05-05 20:38:50.319043 sqlalchemy_multilingual-0.0.7/
+-rw-r--r--   0 vitya      (501) staff       (20)     1063 2024-05-05 20:11:04.000000 sqlalchemy_multilingual-0.0.7/LICENSE.txt
+-rw-r--r--   0 vitya      (501) staff       (20)       34 2023-06-27 13:11:56.000000 sqlalchemy_multilingual-0.0.7/MANIFEST.in
+-rw-r--r--   0 vitya      (501) staff       (20)      534 2024-05-05 20:38:50.319107 sqlalchemy_multilingual-0.0.7/PKG-INFO
+-rw-r--r--   0 vitya      (501) staff       (20)        0 2024-05-05 19:57:01.000000 sqlalchemy_multilingual-0.0.7/README.md
+-rw-r--r--   0 vitya      (501) staff       (20)      835 2024-05-05 20:38:49.000000 sqlalchemy_multilingual-0.0.7/pyproject.toml
+-rw-r--r--   0 vitya      (501) staff       (20)      579 2024-05-05 20:38:50.319358 sqlalchemy_multilingual-0.0.7/setup.cfg
+-rw-r--r--   0 vitya      (501) staff       (20)      235 2024-05-05 20:29:38.000000 sqlalchemy_multilingual-0.0.7/setup.py
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2024-05-05 20:38:50.318950 sqlalchemy_multilingual-0.0.7/sqlalchemy_multilingual.egg-info/
+-rw-r--r--   0 vitya      (501) staff       (20)      534 2024-05-05 20:38:50.000000 sqlalchemy_multilingual-0.0.7/sqlalchemy_multilingual.egg-info/PKG-INFO
+-rw-r--r--   0 vitya      (501) staff       (20)      301 2024-05-05 20:38:50.000000 sqlalchemy_multilingual-0.0.7/sqlalchemy_multilingual.egg-info/SOURCES.txt
+-rw-r--r--   0 vitya      (501) staff       (20)        1 2024-05-05 20:38:50.000000 sqlalchemy_multilingual-0.0.7/sqlalchemy_multilingual.egg-info/dependency_links.txt
+-rw-r--r--   0 vitya      (501) staff       (20)       43 2024-05-05 20:38:50.000000 sqlalchemy_multilingual-0.0.7/sqlalchemy_multilingual.egg-info/requires.txt
+-rw-r--r--   0 vitya      (501) staff       (20)        1 2024-05-05 20:38:50.000000 sqlalchemy_multilingual-0.0.7/sqlalchemy_multilingual.egg-info/top_level.txt
```

### Comparing `sqlalchemy_multilingual-0.0.6/LICENSE.txt` & `sqlalchemy_multilingual-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sqlalchemy_multilingual-0.0.6/PKG-INFO` & `sqlalchemy_multilingual-0.0.7/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: sqlalchemy_multilingual
-Version: 0.0.6
+Version: 0.0.7
 Author: Kosenko Viktor
 Author-email: oxpaoff <kosenkoviktor11@gmail.com>
 Project-URL: Homepage, https://github.com/oxpaoff/sqlalchemy-multilingual
 Project-URL: Bug Tracker, https://github.com/oxpaoff/sqlalchemy-multilingual/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: SQLAlchemy>=2.0.0
-Requires-Dist: typing_extensions==4.6.3
```

### Comparing `sqlalchemy_multilingual-0.0.6/pyproject.toml` & `sqlalchemy_multilingual-0.0.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sqlalchemy_multilingual"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
     { name = "oxpaoff", email = "kosenkoviktor11@gmail.com" },
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `sqlalchemy_multilingual-0.0.6/setup.cfg` & `sqlalchemy_multilingual-0.0.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sqlalchemy_multilingual
-version = 0.0.6
+version = 0.0.7
 description = ""
 long_description = file: README.md
 author = Kosenko Viktor
 author_email = kosenkoviktor11@gmail.com
 classifiers = 
 	Environment :: Web Environment
 	Intended Audience :: Developers
```

### Comparing `sqlalchemy_multilingual-0.0.6/sqlalchemy_multilingual.egg-info/PKG-INFO` & `sqlalchemy_multilingual-0.0.7/sqlalchemy_multilingual.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
-Name: sqlalchemy_multilingual
-Version: 0.0.6
+Name: sqlalchemy-multilingual
+Version: 0.0.7
 Author: Kosenko Viktor
 Author-email: oxpaoff <kosenkoviktor11@gmail.com>
 Project-URL: Homepage, https://github.com/oxpaoff/sqlalchemy-multilingual
 Project-URL: Bug Tracker, https://github.com/oxpaoff/sqlalchemy-multilingual/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: SQLAlchemy>=2.0.0
-Requires-Dist: typing_extensions==4.6.3
```

