# Comparing `tmp/SQLConn-0.0.3.tar.gz` & `tmp/SQLConn-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SQLConn-0.0.3.tar", last modified: Mon May  6 09:29:12 2024, max compression
+gzip compressed data, was "SQLConn-0.0.4.tar", last modified: Mon May  6 09:40:59 2024, max compression
```

## Comparing `SQLConn-0.0.3.tar` & `SQLConn-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 09:29:12.955936 SQLConn-0.0.3/
--rw-rw-rw-   0        0        0     9260 2024-05-06 09:29:12.952936 SQLConn-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     8818 2024-05-06 08:56:32.000000 SQLConn-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 09:29:12.939938 SQLConn-0.0.3/SQLConn/
--rw-rw-rw-   0        0        0     5570 2024-05-06 09:26:10.000000 SQLConn-0.0.3/SQLConn/SQLConn.py
--rw-rw-rw-   0        0        0      293 2024-05-06 09:26:20.000000 SQLConn-0.0.3/SQLConn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 09:29:12.950936 SQLConn-0.0.3/SQLConn.egg-info/
--rw-rw-rw-   0        0        0     9260 2024-05-06 09:29:12.000000 SQLConn-0.0.3/SQLConn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2024-05-06 09:29:12.000000 SQLConn-0.0.3/SQLConn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 09:29:12.000000 SQLConn-0.0.3/SQLConn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-05-06 09:29:12.000000 SQLConn-0.0.3/SQLConn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-06 09:29:12.000000 SQLConn-0.0.3/SQLConn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 09:29:12.955936 SQLConn-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      650 2024-05-06 09:29:04.000000 SQLConn-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:40:59.401677 SQLConn-0.0.4/
+-rw-rw-rw-   0        0        0     9260 2024-05-06 09:40:59.400017 SQLConn-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     8818 2024-05-06 08:56:32.000000 SQLConn-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 09:40:59.377308 SQLConn-0.0.4/SQLConn/
+-rw-rw-rw-   0        0        0     5570 2024-05-06 09:26:10.000000 SQLConn-0.0.4/SQLConn/SQLConn.py
+-rw-rw-rw-   0        0        0      293 2024-05-06 09:40:40.000000 SQLConn-0.0.4/SQLConn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:40:59.398018 SQLConn-0.0.4/SQLConn.egg-info/
+-rw-rw-rw-   0        0        0     9260 2024-05-06 09:40:59.000000 SQLConn-0.0.4/SQLConn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2024-05-06 09:40:59.000000 SQLConn-0.0.4/SQLConn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 09:40:59.000000 SQLConn-0.0.4/SQLConn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-05-06 09:40:59.000000 SQLConn-0.0.4/SQLConn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-06 09:40:59.000000 SQLConn-0.0.4/SQLConn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 09:40:59.401677 SQLConn-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      650 2024-05-06 09:40:55.000000 SQLConn-0.0.4/setup.py
```

### Comparing `SQLConn-0.0.3/PKG-INFO` & `SQLConn-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLConn
-Version: 0.0.3
+Version: 0.0.4
 Summary: This package facilitates easy SQL database integration.
 Home-page: https://github.com/janyoungjin/SQLConn
 Author: janyoungjin
 Keywords: mysql,postgresql,sqlite,mssql,oracle,sql
 Description-Content-Type: text/markdown
 Requires-Dist: mysqlclient
 Requires-Dist: pandas
```

### Comparing `SQLConn-0.0.3/README.md` & `SQLConn-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `SQLConn-0.0.3/SQLConn/SQLConn.py` & `SQLConn-0.0.4/SQLConn/SQLConn.py`

 * *Files identical despite different names*

### Comparing `SQLConn-0.0.3/SQLConn.egg-info/PKG-INFO` & `SQLConn-0.0.4/SQLConn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLConn
-Version: 0.0.3
+Version: 0.0.4
 Summary: This package facilitates easy SQL database integration.
 Home-page: https://github.com/janyoungjin/SQLConn
 Author: janyoungjin
 Keywords: mysql,postgresql,sqlite,mssql,oracle,sql
 Description-Content-Type: text/markdown
 Requires-Dist: mysqlclient
 Requires-Dist: pandas
```

### Comparing `SQLConn-0.0.3/setup.py` & `SQLConn-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='SQLConn',
-    version='0.0.3',
+    version='0.0.4',
     description='This package facilitates easy SQL database integration.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='janyoungjin',
     install_requires=['mysqlclient', 'pandas', 'cx_oracle', 'psycopg2', 'pymssql','sqlalchemy'],
     packages=find_packages(exclude=[]),
     url='https://github.com/janyoungjin/SQLConn',
```

