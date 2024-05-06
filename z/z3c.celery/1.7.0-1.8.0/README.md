# Comparing `tmp/z3c.celery-1.7.0.tar.gz` & `tmp/z3c_celery-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "z3c.celery-1.7.0.tar", last modified: Fri Mar 22 08:41:27 2024, max compression
+gzip compressed data, was "z3c_celery-1.8.0.tar", last modified: Mon May  6 11:40:46 2024, max compression
```

## Comparing `z3c.celery-1.7.0.tar` & `z3c_celery-1.8.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 wolfgang.schnerring   (502) staff       (20)        0 2024-03-22 08:41:27.014034 z3c.celery-1.7.0/
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)      100 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/.coveragerc
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     2109 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/CHANGES.rst
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     1505 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/LICENSE.txt
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)      196 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/MANIFEST.in
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     4269 2024-03-22 08:41:27.013573 z3c.celery-1.7.0/PKG-INFO
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)      468 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/README.rst
-drwxr-xr-x   0 wolfgang.schnerring   (502) staff       (20)        0 2024-03-22 08:41:26.966376 z3c.celery-1.7.0/doc/
-drwxr-xr-x   0 wolfgang.schnerring   (502) staff       (20)        0 2024-03-22 08:41:26.970236 z3c.celery-1.7.0/doc/_api/
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)      390 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/doc/_api/z3c.celery.celery.rst
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)      199 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/doc/_api/z3c.celery.layer.rst
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)       52 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/doc/about.rst
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)      126 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/doc/api.rst
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)       28 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/doc/changes.rst
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     1356 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/doc/conf.py
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)      618 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/doc/index.rst
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)      191 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/doc/project-links.html
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)      513 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/doc/testing.rst
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     6529 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/doc/usage.rst
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)      181 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/pytest.ini
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)       38 2024-03-22 08:41:27.014095 z3c.celery-1.7.0/setup.cfg
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     2105 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/setup.py
-drwxr-xr-x   0 wolfgang.schnerring   (502) staff       (20)        0 2024-03-22 08:41:26.930417 z3c.celery-1.7.0/src/
-drwxr-xr-x   0 wolfgang.schnerring   (502) staff       (20)        0 2024-03-22 08:41:26.970694 z3c.celery-1.7.0/src/z3c/
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)       75 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/src/z3c/__init__.py
-drwxr-xr-x   0 wolfgang.schnerring   (502) staff       (20)        0 2024-03-22 08:41:27.001061 z3c.celery-1.7.0/src/z3c/celery/
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)      122 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/src/z3c/celery/__init__.py
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)    12378 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/src/z3c/celery/celery.py
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     3805 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/src/z3c/celery/conftest.py
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)      673 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/src/z3c/celery/ftesting.zcml
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     1793 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/src/z3c/celery/layer.py
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     3357 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/src/z3c/celery/loader.py
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)      958 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/src/z3c/celery/logging.py
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     1852 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/src/z3c/celery/session.py
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)      882 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/src/z3c/celery/testing.py
-drwxr-xr-x   0 wolfgang.schnerring   (502) staff       (20)        0 2024-03-22 08:41:27.012254 z3c.celery-1.7.0/src/z3c/celery/tests/
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)        0 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/src/z3c/celery/tests/__init__.py
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     1021 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/src/z3c/celery/tests/shared_tasks.py
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)    15596 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/src/z3c/celery/tests/test_celery.py
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     2335 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/src/z3c/celery/tests/test_layer.py
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     3838 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/src/z3c/celery/tests/test_loader.py
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     1728 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/src/z3c/celery/tests/test_logging.py
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)      283 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/src/z3c/celery/tests/test_session.py
-drwxr-xr-x   0 wolfgang.schnerring   (502) staff       (20)        0 2024-03-22 08:41:27.012675 z3c.celery-1.7.0/src/z3c.celery.egg-info/
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     4269 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/src/z3c.celery.egg-info/PKG-INFO
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     1047 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/src/z3c.celery.egg-info/SOURCES.txt
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)        1 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/src/z3c.celery.egg-info/dependency_links.txt
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)        4 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/src/z3c.celery.egg-info/namespace_packages.txt
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)        1 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/src/z3c.celery.egg-info/not-zip-safe
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)      326 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/src/z3c.celery.egg-info/requires.txt
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)        4 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/src/z3c.celery.egg-info/top_level.txt
--rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     1722 2024-03-22 08:41:26.000000 z3c.celery-1.7.0/tox.ini
+drwxr-xr-x   0 wolfgang.schnerring   (502) staff       (20)        0 2024-05-06 11:40:46.970790 z3c_celery-1.8.0/
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)      100 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/.coveragerc
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     2262 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/CHANGES.rst
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     1505 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/LICENSE.txt
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)      196 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/MANIFEST.in
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     4423 2024-05-06 11:40:46.970299 z3c_celery-1.8.0/PKG-INFO
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)      468 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/README.rst
+drwxr-xr-x   0 wolfgang.schnerring   (502) staff       (20)        0 2024-05-06 11:40:46.912888 z3c_celery-1.8.0/doc/
+drwxr-xr-x   0 wolfgang.schnerring   (502) staff       (20)        0 2024-05-06 11:40:46.917334 z3c_celery-1.8.0/doc/_api/
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)      390 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/doc/_api/z3c.celery.celery.rst
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)      199 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/doc/_api/z3c.celery.layer.rst
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)       52 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/doc/about.rst
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)      126 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/doc/api.rst
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)       28 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/doc/changes.rst
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     1356 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/doc/conf.py
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)      618 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/doc/index.rst
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)      191 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/doc/project-links.html
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)      513 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/doc/testing.rst
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     6529 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/doc/usage.rst
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)      181 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/pytest.ini
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)       38 2024-05-06 11:40:46.970852 z3c_celery-1.8.0/setup.cfg
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     2084 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/setup.py
+drwxr-xr-x   0 wolfgang.schnerring   (502) staff       (20)        0 2024-05-06 11:40:46.876712 z3c_celery-1.8.0/src/
+drwxr-xr-x   0 wolfgang.schnerring   (502) staff       (20)        0 2024-05-06 11:40:46.917741 z3c_celery-1.8.0/src/z3c/
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)       75 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/src/z3c/__init__.py
+drwxr-xr-x   0 wolfgang.schnerring   (502) staff       (20)        0 2024-05-06 11:40:46.953420 z3c_celery-1.8.0/src/z3c/celery/
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)      122 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/src/z3c/celery/__init__.py
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)    12605 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/src/z3c/celery/celery.py
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     3805 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/src/z3c/celery/conftest.py
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)      673 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/src/z3c/celery/ftesting.zcml
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     1793 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/src/z3c/celery/layer.py
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     3357 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/src/z3c/celery/loader.py
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)      958 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/src/z3c/celery/logging.py
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     1852 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/src/z3c/celery/session.py
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)      882 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/src/z3c/celery/testing.py
+drwxr-xr-x   0 wolfgang.schnerring   (502) staff       (20)        0 2024-05-06 11:40:46.968851 z3c_celery-1.8.0/src/z3c/celery/tests/
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)        0 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/src/z3c/celery/tests/__init__.py
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     1021 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/src/z3c/celery/tests/shared_tasks.py
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)    16117 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/src/z3c/celery/tests/test_celery.py
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     2335 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/src/z3c/celery/tests/test_layer.py
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     3838 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/src/z3c/celery/tests/test_loader.py
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     1728 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/src/z3c/celery/tests/test_logging.py
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)      283 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/src/z3c/celery/tests/test_session.py
+drwxr-xr-x   0 wolfgang.schnerring   (502) staff       (20)        0 2024-05-06 11:40:46.969292 z3c_celery-1.8.0/src/z3c.celery.egg-info/
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     4423 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/src/z3c.celery.egg-info/PKG-INFO
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     1047 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/src/z3c.celery.egg-info/SOURCES.txt
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)        1 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/src/z3c.celery.egg-info/dependency_links.txt
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)        4 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/src/z3c.celery.egg-info/namespace_packages.txt
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)        1 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/src/z3c.celery.egg-info/not-zip-safe
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)      308 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/src/z3c.celery.egg-info/requires.txt
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)        4 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/src/z3c.celery.egg-info/top_level.txt
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     1722 2024-05-06 11:40:46.000000 z3c_celery-1.8.0/tox.ini
```

### Comparing `z3c.celery-1.7.0/CHANGES.rst` & `z3c_celery-1.8.0/CHANGES.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 =========================
 Change log for z3c.celery
 =========================
 
+1.8.0 (2024-05-06)
+==================
+
+- Also apply "retry on ConflictError" when raised by the task execution itself,
+  not only if raised on commit.
+
+
 1.7.0 (2024-03-22)
 ==================
 
 - Added support for Python 3.12
 
 
 1.6.0 (2022-06-23)
```

### Comparing `z3c.celery-1.7.0/LICENSE.txt` & `z3c_celery-1.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `z3c.celery-1.7.0/PKG-INFO` & `z3c_celery-1.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: z3c.celery
-Version: 1.7.0
+Version: 1.8.0
 Summary: Integration of Celery 4 with Zope 3.
 Home-page: https://github.com/ZeitOnline/z3c.celery
 Author: gocept, Zeit Online
 Author-email: zon-backend@zeit.de
 License: BSD
 Keywords: celery Zope transaction
 Classifier: Development Status :: 3 - Alpha
@@ -20,32 +20,31 @@
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Testing
 License-File: LICENSE.txt
 Requires-Dist: celery>=4.0.2
 Requires-Dist: setuptools
 Requires-Dist: transaction
-Requires-Dist: ZODB
-Requires-Dist: zope.app.appsetup
 Requires-Dist: zope.app.publication
 Requires-Dist: zope.app.wsgi
 Requires-Dist: zope.authentication
 Requires-Dist: zope.component
 Requires-Dist: zope.exceptions
 Requires-Dist: zope.interface
 Requires-Dist: zope.publisher
 Requires-Dist: zope.security
-Requires-Dist: zope.principalregistry
 Provides-Extra: test
+Requires-Dist: ZODB; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-celery; extra == "test"
 Requires-Dist: gocept.pytestlayer; extra == "test"
 Requires-Dist: plone.testing; extra == "test"
 Requires-Dist: redis; extra == "test"
 Requires-Dist: tblib; extra == "test"
+Requires-Dist: zope.principalregistry; extra == "test"
 Requires-Dist: zope.traversing; extra == "test"
 Provides-Extra: layer
 Requires-Dist: plone.testing; extra == "layer"
 
 ==========
 z3c.celery
 ==========
@@ -70,14 +69,21 @@
     https://raw.githubusercontent.com/ZeitOnline/z3c.celery/master/CHANGES.rst
 
 
 =========================
 Change log for z3c.celery
 =========================
 
+1.8.0 (2024-05-06)
+==================
+
+- Also apply "retry on ConflictError" when raised by the task execution itself,
+  not only if raised on commit.
+
+
 1.7.0 (2024-03-22)
 ==================
 
 - Added support for Python 3.12
 
 
 1.6.0 (2022-06-23)
```

### Comparing `z3c.celery-1.7.0/doc/conf.py` & `z3c_celery-1.8.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `z3c.celery-1.7.0/doc/index.rst` & `z3c_celery-1.8.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `z3c.celery-1.7.0/doc/testing.rst` & `z3c_celery-1.8.0/doc/testing.rst`

 * *Files identical despite different names*

### Comparing `z3c.celery-1.7.0/doc/usage.rst` & `z3c_celery-1.8.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `z3c.celery-1.7.0/setup.py` & `z3c_celery-1.8.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,41 +3,40 @@
 """Integration of Celery 4 with Zope 3.
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name='z3c.celery',
-    version='1.7.0',
+    version='1.8.0',
 
     install_requires=[
         'celery >= 4.0.2',
         'setuptools',
         'transaction',
-        'ZODB',
-        'zope.app.appsetup',
         'zope.app.publication',
         'zope.app.wsgi',
         'zope.authentication',
         'zope.component',
         'zope.exceptions',
         'zope.interface',
         'zope.publisher',
         'zope.security',
-        'zope.principalregistry',
     ],
 
     extras_require={
         'test': [
+            'ZODB',
             'pytest',
             'pytest-celery',
             'gocept.pytestlayer',
             'plone.testing',
             'redis',
             'tblib',
+            'zope.principalregistry',
             'zope.traversing',
         ],
         'layer': [  # use this extra when using the EndToEndLayer
             'plone.testing',
         ],
 
     },
```

### Comparing `z3c.celery-1.7.0/src/z3c/celery/celery.py` & `z3c_celery-1.8.0/src/z3c/celery/celery.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from .loader import ZopeLoader
 from .session import celery_session
 from celery._state import _task_stack
 from celery.utils.serialization import raise_with_context
-import ZODB.POSException
 import celery
 import celery.exceptions
 import celery.utils
 import contextlib
 import json
 import logging
 import random
@@ -187,22 +186,27 @@
             transaction.begin()
             login_principal(get_principal(principal_id), self.name)
             txn = transaction.get()
             txn.setUser(str(principal_id))
             txn.setExtendedInfo('task_name', self.name)
         try:
             yield
+        except transaction.interfaces.TransientError:
+            log.warning('ConflictError, retrying', exc_info=True)
+            transaction.abort()
+            self.retry(
+                countdown=random.uniform(0, 2 ** self.request.retries))
         except Exception:
             transaction.abort()
             raise
         else:
             try:
                 transaction.commit()
-            except ZODB.POSException.ConflictError:
-                log.warning('Conflict while publishing', exc_info=True)
+            except transaction.interfaces.TransientError:
+                log.warning('ConflictError, retrying', exc_info=True)
                 transaction.abort()
                 self.retry(
                     countdown=random.uniform(0, 2 ** self.request.retries))
         finally:
             transaction.abort()
             zope.security.management.endInteraction()
```

### Comparing `z3c.celery-1.7.0/src/z3c/celery/conftest.py` & `z3c_celery-1.8.0/src/z3c/celery/conftest.py`

 * *Files identical despite different names*

### Comparing `z3c.celery-1.7.0/src/z3c/celery/ftesting.zcml` & `z3c_celery-1.8.0/src/z3c/celery/ftesting.zcml`

 * *Files identical despite different names*

### Comparing `z3c.celery-1.7.0/src/z3c/celery/layer.py` & `z3c_celery-1.8.0/src/z3c/celery/layer.py`

 * *Files identical despite different names*

### Comparing `z3c.celery-1.7.0/src/z3c/celery/loader.py` & `z3c_celery-1.8.0/src/z3c/celery/loader.py`

 * *Files identical despite different names*

### Comparing `z3c.celery-1.7.0/src/z3c/celery/logging.py` & `z3c_celery-1.8.0/src/z3c/celery/logging.py`

 * *Files identical despite different names*

### Comparing `z3c.celery-1.7.0/src/z3c/celery/session.py` & `z3c_celery-1.8.0/src/z3c/celery/session.py`

 * *Files identical despite different names*

### Comparing `z3c.celery-1.7.0/src/z3c/celery/testing.py` & `z3c_celery-1.8.0/src/z3c/celery/testing.py`

 * *Files identical despite different names*

### Comparing `z3c.celery-1.7.0/src/z3c/celery/tests/shared_tasks.py` & `z3c_celery-1.8.0/src/z3c/celery/tests/shared_tasks.py`

 * *Files identical despite different names*

### Comparing `z3c.celery-1.7.0/src/z3c/celery/tests/test_celery.py` & `z3c_celery-1.8.0/src/z3c/celery/tests/test_celery.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,15 +183,15 @@
             eager_task(_run_asynchronously_=True)
 
     assert run.called
     assert abort.called
 
 
 @shared_task(max_retries=1)
-def conflict_task(bind=True, context=None, datetime=None):
+def conflict_on_commit_task(bind=True, context=None, datetime=None):
     """Dummy task which injects a DataManager that votes a ConflictError."""
     transaction.get().join(VoteExceptionDataManager())
 
 
 class NoopDatamanager:
     """Datamanager which does nothing."""
 
@@ -219,15 +219,15 @@
         # that we can throw an Error as last part of vote:
         return '~~sort-me-last'
 
 
 def test_celery__TransactionAwareTask____call____2(
         celery_session_worker, interaction):
     """It aborts the transaction and retries in case of an ConflictError."""
-    result = conflict_task.delay()
+    result = conflict_on_commit_task.delay()
     transaction.commit()
     with pytest.raises(Exception) as err:
         result.get()
     assert 'MaxRetriesExceededError' == err.value.__class__.__name__
 
 
 @shared_task(max_retries=2)
@@ -254,14 +254,30 @@
             mock.patch('time.sleep') as sleep:
         with pytest.raises(HandleAfterAbort):
             conflict_after_abort_task(_run_asynchronously_=True)
         assert sleep.call_count == 1
         assert conflicts_after_abort == 2
 
 
+@shared_task(max_retries=1)
+def conflict_during_task():
+    raise ZODB.POSException.ConflictError()
+
+
+def test_celery__TransactionAwareTask____call____2b(
+        celery_session_worker, interaction):
+    """It retries on ConflictError caused during task execution
+    (not only caused by commit)."""
+    result = conflict_during_task.delay()
+    transaction.commit()
+    with pytest.raises(Exception) as err:
+        result.get()
+    assert 'MaxRetriesExceededError' == err.value.__class__.__name__
+
+
 def test_celery__TransactionAwareTask____call____3(
         celery_session_worker, zcml):
     """It runs as given principal in asynchronous mode."""
     auth = zope.component.getUtility(
         zope.authentication.interfaces.IAuthentication)
     principal = auth.getPrincipal('example.user')
     z3c.celery.celery.login_principal(principal)
```

### Comparing `z3c.celery-1.7.0/src/z3c/celery/tests/test_layer.py` & `z3c_celery-1.8.0/src/z3c/celery/tests/test_layer.py`

 * *Files identical despite different names*

### Comparing `z3c.celery-1.7.0/src/z3c/celery/tests/test_loader.py` & `z3c_celery-1.8.0/src/z3c/celery/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `z3c.celery-1.7.0/src/z3c/celery/tests/test_logging.py` & `z3c_celery-1.8.0/src/z3c/celery/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `z3c.celery-1.7.0/src/z3c.celery.egg-info/PKG-INFO` & `z3c_celery-1.8.0/src/z3c.celery.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: z3c.celery
-Version: 1.7.0
+Version: 1.8.0
 Summary: Integration of Celery 4 with Zope 3.
 Home-page: https://github.com/ZeitOnline/z3c.celery
 Author: gocept, Zeit Online
 Author-email: zon-backend@zeit.de
 License: BSD
 Keywords: celery Zope transaction
 Classifier: Development Status :: 3 - Alpha
@@ -20,32 +20,31 @@
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Testing
 License-File: LICENSE.txt
 Requires-Dist: celery>=4.0.2
 Requires-Dist: setuptools
 Requires-Dist: transaction
-Requires-Dist: ZODB
-Requires-Dist: zope.app.appsetup
 Requires-Dist: zope.app.publication
 Requires-Dist: zope.app.wsgi
 Requires-Dist: zope.authentication
 Requires-Dist: zope.component
 Requires-Dist: zope.exceptions
 Requires-Dist: zope.interface
 Requires-Dist: zope.publisher
 Requires-Dist: zope.security
-Requires-Dist: zope.principalregistry
 Provides-Extra: test
+Requires-Dist: ZODB; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-celery; extra == "test"
 Requires-Dist: gocept.pytestlayer; extra == "test"
 Requires-Dist: plone.testing; extra == "test"
 Requires-Dist: redis; extra == "test"
 Requires-Dist: tblib; extra == "test"
+Requires-Dist: zope.principalregistry; extra == "test"
 Requires-Dist: zope.traversing; extra == "test"
 Provides-Extra: layer
 Requires-Dist: plone.testing; extra == "layer"
 
 ==========
 z3c.celery
 ==========
@@ -70,14 +69,21 @@
     https://raw.githubusercontent.com/ZeitOnline/z3c.celery/master/CHANGES.rst
 
 
 =========================
 Change log for z3c.celery
 =========================
 
+1.8.0 (2024-05-06)
+==================
+
+- Also apply "retry on ConflictError" when raised by the task execution itself,
+  not only if raised on commit.
+
+
 1.7.0 (2024-03-22)
 ==================
 
 - Added support for Python 3.12
 
 
 1.6.0 (2022-06-23)
```

### Comparing `z3c.celery-1.7.0/src/z3c.celery.egg-info/SOURCES.txt` & `z3c_celery-1.8.0/src/z3c.celery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `z3c.celery-1.7.0/tox.ini` & `z3c_celery-1.8.0/tox.ini`

 * *Files identical despite different names*

