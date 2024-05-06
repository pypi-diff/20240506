# Comparing `tmp/plone.recipe.zeoserver-3.0.1.tar.gz` & `tmp/plone_recipe_zeoserver-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.recipe.zeoserver-3.0.1.tar", last modified: Fri Oct  6 22:32:24 2023, max compression
+gzip compressed data, was "plone_recipe_zeoserver-3.0.2.tar", last modified: Mon May  6 12:54:00 2024, max compression
```

## Comparing `plone.recipe.zeoserver-3.0.1.tar` & `plone_recipe_zeoserver-3.0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:32:24.333317 plone.recipe.zeoserver-3.0.1/
--rw-r--r--   0 maurits    (501) staff       (20)     6492 2023-10-06 22:32:23.000000 plone.recipe.zeoserver-3.0.1/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-10-06 22:32:23.000000 plone.recipe.zeoserver-3.0.1/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      193 2023-10-06 22:32:23.000000 plone.recipe.zeoserver-3.0.1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    15545 2023-10-06 22:32:24.332199 plone.recipe.zeoserver-3.0.1/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     7707 2023-10-06 22:32:23.000000 plone.recipe.zeoserver-3.0.1/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)     4240 2023-10-06 22:32:23.000000 plone.recipe.zeoserver-3.0.1/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)       38 2023-10-06 22:32:24.333544 plone.recipe.zeoserver-3.0.1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1975 2023-10-06 22:32:23.000000 plone.recipe.zeoserver-3.0.1/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:32:24.303447 plone.recipe.zeoserver-3.0.1/src/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:32:24.311008 plone.recipe.zeoserver-3.0.1/src/plone/
--rw-r--r--   0 maurits    (501) staff       (20)      245 2023-10-06 22:32:23.000000 plone.recipe.zeoserver-3.0.1/src/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:32:24.320894 plone.recipe.zeoserver-3.0.1/src/plone/recipe/
--rw-r--r--   0 maurits    (501) staff       (20)      245 2023-10-06 22:32:23.000000 plone.recipe.zeoserver-3.0.1/src/plone/recipe/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:32:24.326979 plone.recipe.zeoserver-3.0.1/src/plone/recipe/zeoserver/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-10-06 22:32:23.000000 plone.recipe.zeoserver-3.0.1/src/plone/recipe/zeoserver/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1057 2023-10-06 22:32:23.000000 plone.recipe.zeoserver-3.0.1/src/plone/recipe/zeoserver/ctl.py
--rw-r--r--   0 maurits    (501) staff       (20)     2259 2023-10-06 22:32:23.000000 plone.recipe.zeoserver-3.0.1/src/plone/recipe/zeoserver/pack.py
--rw-r--r--   0 maurits    (501) staff       (20)    20249 2023-10-06 22:32:23.000000 plone.recipe.zeoserver-3.0.1/src/plone/recipe/zeoserver/recipe.py
--rw-r--r--   0 maurits    (501) staff       (20)      287 2023-10-06 22:32:23.000000 plone.recipe.zeoserver-3.0.1/src/plone/recipe/zeoserver/runzeo.bat
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:32:24.330129 plone.recipe.zeoserver-3.0.1/src/plone/recipe/zeoserver/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        2 2023-10-06 22:32:23.000000 plone.recipe.zeoserver-3.0.1/src/plone/recipe/zeoserver/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1435 2023-10-06 22:32:23.000000 plone.recipe.zeoserver-3.0.1/src/plone/recipe/zeoserver/tests/test_docs.py
--rw-r--r--   0 maurits    (501) staff       (20)    16620 2023-10-06 22:32:23.000000 plone.recipe.zeoserver-3.0.1/src/plone/recipe/zeoserver/tests/zeoserver.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4217 2023-10-06 22:32:23.000000 plone.recipe.zeoserver-3.0.1/src/plone/recipe/zeoserver/zeoservice.py.in
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:32:24.320202 plone.recipe.zeoserver-3.0.1/src/plone.recipe.zeoserver.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    15545 2023-10-06 22:32:24.000000 plone.recipe.zeoserver-3.0.1/src/plone.recipe.zeoserver.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      901 2023-10-06 22:32:24.000000 plone.recipe.zeoserver-3.0.1/src/plone.recipe.zeoserver.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-10-06 22:32:24.000000 plone.recipe.zeoserver-3.0.1/src/plone.recipe.zeoserver.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       61 2023-10-06 22:32:24.000000 plone.recipe.zeoserver-3.0.1/src/plone.recipe.zeoserver.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       19 2023-10-06 22:32:24.000000 plone.recipe.zeoserver-3.0.1/src/plone.recipe.zeoserver.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-10-06 22:32:24.000000 plone.recipe.zeoserver-3.0.1/src/plone.recipe.zeoserver.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      106 2023-10-06 22:32:24.000000 plone.recipe.zeoserver-3.0.1/src/plone.recipe.zeoserver.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-10-06 22:32:24.000000 plone.recipe.zeoserver-3.0.1/src/plone.recipe.zeoserver.egg-info/top_level.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:54:00.335660 plone_recipe_zeoserver-3.0.2/
+-rw-r--r--   0 maurits    (501) staff       (20)     6851 2024-05-06 12:53:59.000000 plone_recipe_zeoserver-3.0.2/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2024-05-06 12:53:59.000000 plone_recipe_zeoserver-3.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      193 2024-05-06 12:53:59.000000 plone_recipe_zeoserver-3.0.2/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    15993 2024-05-06 12:54:00.335255 plone_recipe_zeoserver-3.0.2/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     7707 2024-05-06 12:53:59.000000 plone_recipe_zeoserver-3.0.2/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     4240 2024-05-06 12:53:59.000000 plone_recipe_zeoserver-3.0.2/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2024-05-06 12:54:00.335735 plone_recipe_zeoserver-3.0.2/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2062 2024-05-06 12:53:59.000000 plone_recipe_zeoserver-3.0.2/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:54:00.324363 plone_recipe_zeoserver-3.0.2/src/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:54:00.327515 plone_recipe_zeoserver-3.0.2/src/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)      245 2024-05-06 12:53:59.000000 plone_recipe_zeoserver-3.0.2/src/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:54:00.330685 plone_recipe_zeoserver-3.0.2/src/plone/recipe/
+-rw-r--r--   0 maurits    (501) staff       (20)      245 2024-05-06 12:53:59.000000 plone_recipe_zeoserver-3.0.2/src/plone/recipe/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:54:00.332702 plone_recipe_zeoserver-3.0.2/src/plone/recipe/zeoserver/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-06 12:53:59.000000 plone_recipe_zeoserver-3.0.2/src/plone/recipe/zeoserver/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1057 2024-05-06 12:53:59.000000 plone_recipe_zeoserver-3.0.2/src/plone/recipe/zeoserver/ctl.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2259 2024-05-06 12:53:59.000000 plone_recipe_zeoserver-3.0.2/src/plone/recipe/zeoserver/pack.py
+-rw-r--r--   0 maurits    (501) staff       (20)    20249 2024-05-06 12:53:59.000000 plone_recipe_zeoserver-3.0.2/src/plone/recipe/zeoserver/recipe.py
+-rw-r--r--   0 maurits    (501) staff       (20)      287 2024-05-06 12:53:59.000000 plone_recipe_zeoserver-3.0.2/src/plone/recipe/zeoserver/runzeo.bat
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:54:00.333809 plone_recipe_zeoserver-3.0.2/src/plone/recipe/zeoserver/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        2 2024-05-06 12:53:59.000000 plone_recipe_zeoserver-3.0.2/src/plone/recipe/zeoserver/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1435 2024-05-06 12:53:59.000000 plone_recipe_zeoserver-3.0.2/src/plone/recipe/zeoserver/tests/test_docs.py
+-rw-r--r--   0 maurits    (501) staff       (20)    14964 2024-05-06 12:53:59.000000 plone_recipe_zeoserver-3.0.2/src/plone/recipe/zeoserver/tests/zeoserver.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4217 2024-05-06 12:53:59.000000 plone_recipe_zeoserver-3.0.2/src/plone/recipe/zeoserver/zeoservice.py.in
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:54:00.334493 plone_recipe_zeoserver-3.0.2/src/plone.recipe.zeoserver.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    15993 2024-05-06 12:54:00.000000 plone_recipe_zeoserver-3.0.2/src/plone.recipe.zeoserver.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      901 2024-05-06 12:54:00.000000 plone_recipe_zeoserver-3.0.2/src/plone.recipe.zeoserver.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-05-06 12:54:00.000000 plone_recipe_zeoserver-3.0.2/src/plone.recipe.zeoserver.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       61 2024-05-06 12:54:00.000000 plone_recipe_zeoserver-3.0.2/src/plone.recipe.zeoserver.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       19 2024-05-06 12:54:00.000000 plone_recipe_zeoserver-3.0.2/src/plone.recipe.zeoserver.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-05-06 12:54:00.000000 plone_recipe_zeoserver-3.0.2/src/plone.recipe.zeoserver.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      106 2024-05-06 12:54:00.000000 plone_recipe_zeoserver-3.0.2/src/plone.recipe.zeoserver.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-05-06 12:54:00.000000 plone_recipe_zeoserver-3.0.2/src/plone.recipe.zeoserver.egg-info/top_level.txt
```

### Comparing `plone.recipe.zeoserver-3.0.1/CHANGES.rst` & `plone_recipe_zeoserver-3.0.2/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,27 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.2 (2024-05-06)
+------------------
+
+Tests
+
+
+- Removed tests for Zope Replication Services.
+  The recipe support should still work, but the tests are broken.
+  Note that the `zc.zrs` project is currently unmaintained, so if you rely on this, please step up.
+  See `issue 52 <https://github.com/plone/plone.recipe.zeoserver/issues/52>`_.
+  [maurits] (#52)
+
+
 3.0.1 (2023-10-07)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.recipe.zeoserver-3.0.1/PKG-INFO` & `plone_recipe_zeoserver-3.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: plone.recipe.zeoserver
-Version: 3.0.1
+Version: 3.0.2
 Summary: ZC Buildout recipe for installing a ZEO server
 Home-page: https://github.com/plone/plone.recipe.zeoserver
 Download-URL: https://pypi.org/project/plone.recipe.zeoserver
 Author: Hanno Schlichting
 Author-email: hannosch@plone.org
 License: ZPL 2.1
 Keywords: zope2 zeo zodb buildout
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Framework :: Buildout
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: 6.0
+Classifier: Framework :: Plone :: 6.1
 Classifier: Framework :: Zope
 Classifier: Framework :: Zope :: 5
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Requires-Dist: setuptools
 Requires-Dist: zc.buildout
 Requires-Dist: zc.recipe.egg
@@ -295,14 +297,27 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.2 (2024-05-06)
+------------------
+
+Tests
+
+
+- Removed tests for Zope Replication Services.
+  The recipe support should still work, but the tests are broken.
+  Note that the `zc.zrs` project is currently unmaintained, so if you rely on this, please step up.
+  See `issue 52 <https://github.com/plone/plone.recipe.zeoserver/issues/52>`_.
+  [maurits] (#52)
+
+
 3.0.1 (2023-10-07)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.recipe.zeoserver-3.0.1/README.rst` & `plone_recipe_zeoserver-3.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `plone.recipe.zeoserver-3.0.1/pyproject.toml` & `plone_recipe_zeoserver-3.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.recipe.zeoserver-3.0.1/setup.py` & `plone_recipe_zeoserver-3.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "3.0.1"
+version = "3.0.2"
 
 long_description = (
     f"{Path('README.rst').read_text()}\n{Path('CHANGES.rst').read_text()}"
 )
 
 setup(
     name="plone.recipe.zeoserver",
@@ -25,21 +25,23 @@
     # https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Zope Public License",
         "Framework :: Buildout",
         "Framework :: Plone",
         "Framework :: Plone :: 6.0",
+        "Framework :: Plone :: 6.1",
         "Framework :: Zope",
         "Framework :: Zope :: 5",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: Implementation",
         "Programming Language :: Python :: Implementation :: CPython",
     ],
     python_requires=">=3.8",
     packages=find_packages("src"),
     include_package_data=True,
     package_dir={"": "src"},
```

### Comparing `plone.recipe.zeoserver-3.0.1/src/plone/recipe/zeoserver/ctl.py` & `plone_recipe_zeoserver-3.0.2/src/plone/recipe/zeoserver/ctl.py`

 * *Files identical despite different names*

### Comparing `plone.recipe.zeoserver-3.0.1/src/plone/recipe/zeoserver/pack.py` & `plone_recipe_zeoserver-3.0.2/src/plone/recipe/zeoserver/pack.py`

 * *Files identical despite different names*

### Comparing `plone.recipe.zeoserver-3.0.1/src/plone/recipe/zeoserver/recipe.py` & `plone_recipe_zeoserver-3.0.2/src/plone/recipe/zeoserver/recipe.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
             # logfile value in any case
             z_log_filename = options.get("zeo-log", z_log_name)
             z_log_filename = os.path.join(var_dir, z_log_filename)
             z_log_dir = os.path.dirname(z_log_filename)
             if not os.path.exists(z_log_dir):
                 os.makedirs(z_log_dir)
 
-            # zeo-log-custom superseeds zeo-log
+            # zeo-log-custom supersedes zeo-log
             logformat = options.get("zeo-log-format", "%(asctime)s %(message)s")
             if zeo_log_custom is None:
                 zeo_log_rotate = ""
                 zeo_log_max_size = options.get("zeo-log-max-size", None)
                 if zeo_log_max_size:
                     zeo_log_old_files = options.get("zeo-log-old-files", 1)
                     zeo_log_rotate = "\n".join(
```

### Comparing `plone.recipe.zeoserver-3.0.1/src/plone/recipe/zeoserver/tests/test_docs.py` & `plone_recipe_zeoserver-3.0.2/src/plone/recipe/zeoserver/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `plone.recipe.zeoserver-3.0.1/src/plone/recipe/zeoserver/tests/zeoserver.txt` & `plone_recipe_zeoserver-3.0.2/src/plone/recipe/zeoserver/tests/zeoserver.txt`

 * *Files 3% similar despite different names*

```diff
@@ -78,86 +78,14 @@
       logfile .../sample-buildout/var/log/zeo.log
     </runner>
     <BLANKLINE>
     <BLANKLINE>
     <BLANKLINE>
 
 
-Zope Replication Services
-=========================
-
-Now, let's create a simple buildout to create a primary replication::
-
-    >>> primaryzrs = '''
-    ... [buildout]
-    ... parts = zeo
-    ... find-links = %(sample_buildout)s/eggs
-    ...
-    ... [zeo]
-    ... recipe = plone.recipe.zeoserver[zrs]
-    ... replicate-to = 127.0.0.1:5000
-    ... ''' % globals()
-    >>> write('buildout.cfg', primaryzrs)
-    >>> print(system(join('bin', 'buildout')))
-    ...
-    Uninstalling zeo.
-    Installing zeo.
-    ...
-
-We should have primary zrs config in zeo.conf::
-
-    >>> zeo = os.path.join(sample_buildout, 'parts', 'zeo')
-    >>> with open(os.path.join(zeo, 'etc', 'zeo.conf')) as f:
-    ...     print(f.read())
-    %define INSTANCE ...
-    ...
-    %import zc.zrs
-    <BLANKLINE>
-    <zrs 1>
-     replicate-to 127.0.0.1:5000
-    ...
-    <filestorage 1>
-    ...
-    <BLANKLINE>
-
-And for a secondary::
-
-    >>> primaryzrs = '''
-    ... [buildout]
-    ... parts = zeo
-    ... find-links = %(sample_buildout)s/eggs
-    ...
-    ... [zeo]
-    ... recipe = plone.recipe.zeoserver[zrs]
-    ... replicate-from = 127.0.0.1:5000
-    ... ''' % globals()
-    >>> write('buildout.cfg', primaryzrs)
-    >>> print(system(join('bin', 'buildout')))
-    ...
-    Uninstalling zeo.
-    Installing zeo.
-    ...
-
-We should have primary zrs config in zeo.conf::
-
-    >>> zeo = os.path.join(sample_buildout, 'parts', 'zeo')
-    >>> with open(os.path.join(zeo, 'etc', 'zeo.conf')) as f:
-    ...     print(f.read())
-    %define INSTANCE ...
-    ...
-    %import zc.zrs
-    <BLANKLINE>
-    <zrs 1>
-     replicate-from 127.0.0.1:5000
-    ...
-    <filestorage 1>
-    ...
-    <BLANKLINE>
-
-
 Custom Zeo log
 ==============
 
 `zeo-log-custom` is a new option that allows you to create
 a custom zeo log section. For example, let's say you want
 to use `rotatezlogs`::
```

### Comparing `plone.recipe.zeoserver-3.0.1/src/plone/recipe/zeoserver/zeoservice.py.in` & `plone_recipe_zeoserver-3.0.2/src/plone/recipe/zeoserver/zeoservice.py.in`

 * *Files identical despite different names*

### Comparing `plone.recipe.zeoserver-3.0.1/src/plone.recipe.zeoserver.egg-info/PKG-INFO` & `plone_recipe_zeoserver-3.0.2/src/plone.recipe.zeoserver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: plone.recipe.zeoserver
-Version: 3.0.1
+Version: 3.0.2
 Summary: ZC Buildout recipe for installing a ZEO server
 Home-page: https://github.com/plone/plone.recipe.zeoserver
 Download-URL: https://pypi.org/project/plone.recipe.zeoserver
 Author: Hanno Schlichting
 Author-email: hannosch@plone.org
 License: ZPL 2.1
 Keywords: zope2 zeo zodb buildout
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Framework :: Buildout
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: 6.0
+Classifier: Framework :: Plone :: 6.1
 Classifier: Framework :: Zope
 Classifier: Framework :: Zope :: 5
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Requires-Dist: setuptools
 Requires-Dist: zc.buildout
 Requires-Dist: zc.recipe.egg
@@ -295,14 +297,27 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.2 (2024-05-06)
+------------------
+
+Tests
+
+
+- Removed tests for Zope Replication Services.
+  The recipe support should still work, but the tests are broken.
+  Note that the `zc.zrs` project is currently unmaintained, so if you rely on this, please step up.
+  See `issue 52 <https://github.com/plone/plone.recipe.zeoserver/issues/52>`_.
+  [maurits] (#52)
+
+
 3.0.1 (2023-10-07)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.recipe.zeoserver-3.0.1/src/plone.recipe.zeoserver.egg-info/SOURCES.txt` & `plone_recipe_zeoserver-3.0.2/src/plone.recipe.zeoserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

