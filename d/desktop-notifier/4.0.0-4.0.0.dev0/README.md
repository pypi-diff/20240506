# Comparing `tmp/desktop_notifier-4.0.0.tar.gz` & `tmp/desktop_notifier-4.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desktop_notifier-4.0.0.tar", last modified: Mon May  6 20:19:33 2024, max compression
+gzip compressed data, was "desktop_notifier-4.0.0.dev0.tar", last modified: Mon May  6 20:19:35 2024, max compression
```

## Comparing `desktop_notifier-4.0.0.tar` & `desktop_notifier-4.0.0.dev0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:19:33.964947 desktop_notifier-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-06 20:19:27.000000 desktop_notifier-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9427 2024-05-06 20:19:33.964947 desktop_notifier-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-05-06 20:19:27.000000 desktop_notifier-4.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-06 20:19:27.000000 desktop_notifier-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 20:19:33.964947 desktop_notifier-4.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:19:33.960947 desktop_notifier-4.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:19:33.964947 desktop_notifier-4.0.0/src/desktop_notifier/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-06 20:19:27.000000 desktop_notifier-4.0.0/src/desktop_notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10425 2024-05-06 20:19:27.000000 desktop_notifier-4.0.0/src/desktop_notifier/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8730 2024-05-06 20:19:27.000000 desktop_notifier-4.0.0/src/desktop_notifier/dbus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-06 20:19:27.000000 desktop_notifier-4.0.0/src/desktop_notifier/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)    14971 2024-05-06 20:19:27.000000 desktop_notifier-4.0.0/src/desktop_notifier/macos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-06 20:19:27.000000 desktop_notifier-4.0.0/src/desktop_notifier/macos_support.py
--rw-r--r--   0 runner    (1001) docker     (127)    12770 2024-05-06 20:19:27.000000 desktop_notifier-4.0.0/src/desktop_notifier/main.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 20:19:27.000000 desktop_notifier-4.0.0/src/desktop_notifier/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:19:33.964947 desktop_notifier-4.0.0/src/desktop_notifier/resources/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-06 20:19:27.000000 desktop_notifier-4.0.0/src/desktop_notifier/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-06 20:19:27.000000 desktop_notifier-4.0.0/src/desktop_notifier/resources/python.png
--rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-05-06 20:19:27.000000 desktop_notifier-4.0.0/src/desktop_notifier/winrt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:19:33.964947 desktop_notifier-4.0.0/src/desktop_notifier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9427 2024-05-06 20:19:33.000000 desktop_notifier-4.0.0/src/desktop_notifier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-06 20:19:33.000000 desktop_notifier-4.0.0/src/desktop_notifier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 20:19:33.000000 desktop_notifier-4.0.0/src/desktop_notifier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-06 20:19:33.000000 desktop_notifier-4.0.0/src/desktop_notifier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-06 20:19:33.000000 desktop_notifier-4.0.0/src/desktop_notifier.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:19:33.964947 desktop_notifier-4.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-06 20:19:27.000000 desktop_notifier-4.0.0/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:19:35.469434 desktop_notifier-4.0.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-06 20:19:28.000000 desktop_notifier-4.0.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9432 2024-05-06 20:19:35.469434 desktop_notifier-4.0.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-05-06 20:19:28.000000 desktop_notifier-4.0.0.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-06 20:19:28.000000 desktop_notifier-4.0.0.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 20:19:35.469434 desktop_notifier-4.0.0.dev0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:19:35.465434 desktop_notifier-4.0.0.dev0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:19:35.465434 desktop_notifier-4.0.0.dev0/src/desktop_notifier/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-06 20:19:28.000000 desktop_notifier-4.0.0.dev0/src/desktop_notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10425 2024-05-06 20:19:28.000000 desktop_notifier-4.0.0.dev0/src/desktop_notifier/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8730 2024-05-06 20:19:28.000000 desktop_notifier-4.0.0.dev0/src/desktop_notifier/dbus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-06 20:19:28.000000 desktop_notifier-4.0.0.dev0/src/desktop_notifier/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14971 2024-05-06 20:19:28.000000 desktop_notifier-4.0.0.dev0/src/desktop_notifier/macos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-06 20:19:28.000000 desktop_notifier-4.0.0.dev0/src/desktop_notifier/macos_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12770 2024-05-06 20:19:28.000000 desktop_notifier-4.0.0.dev0/src/desktop_notifier/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 20:19:28.000000 desktop_notifier-4.0.0.dev0/src/desktop_notifier/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:19:35.465434 desktop_notifier-4.0.0.dev0/src/desktop_notifier/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-06 20:19:28.000000 desktop_notifier-4.0.0.dev0/src/desktop_notifier/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-06 20:19:28.000000 desktop_notifier-4.0.0.dev0/src/desktop_notifier/resources/python.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-05-06 20:19:28.000000 desktop_notifier-4.0.0.dev0/src/desktop_notifier/winrt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:19:35.465434 desktop_notifier-4.0.0.dev0/src/desktop_notifier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9432 2024-05-06 20:19:35.000000 desktop_notifier-4.0.0.dev0/src/desktop_notifier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-06 20:19:35.000000 desktop_notifier-4.0.0.dev0/src/desktop_notifier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 20:19:35.000000 desktop_notifier-4.0.0.dev0/src/desktop_notifier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-06 20:19:35.000000 desktop_notifier-4.0.0.dev0/src/desktop_notifier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-06 20:19:35.000000 desktop_notifier-4.0.0.dev0/src/desktop_notifier.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:19:35.465434 desktop_notifier-4.0.0.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-06 20:19:28.000000 desktop_notifier-4.0.0.dev0/tests/test_api.py
```

### Comparing `desktop_notifier-4.0.0/LICENSE` & `desktop_notifier-4.0.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `desktop_notifier-4.0.0/PKG-INFO` & `desktop_notifier-4.0.0.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: desktop-notifier
-Version: 4.0.0
+Version: 4.0.0.dev0
 Summary: Python library for cross-platform desktop notifications
 Author-email: Sam Schott <sam.schott@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/samschott/desktop-notifier
 Keywords: desktop-notifier
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `desktop_notifier-4.0.0/README.md` & `desktop_notifier-4.0.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `desktop_notifier-4.0.0/pyproject.toml` & `desktop_notifier-4.0.0.dev0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2", "build"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "desktop-notifier"
-version = "4.0.0"
+version = "4.0.0.dev0"
 authors = [{name = "Sam Schott", email = "sam.schott@outlook.com"}]
 license = {text = "MIT"}
 description = "Python library for cross-platform desktop notifications"
 keywords = ["desktop-notifier"]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
```

### Comparing `desktop_notifier-4.0.0/src/desktop_notifier/base.py` & `desktop_notifier-4.0.0.dev0/src/desktop_notifier/base.py`

 * *Files identical despite different names*

### Comparing `desktop_notifier-4.0.0/src/desktop_notifier/dbus.py` & `desktop_notifier-4.0.0.dev0/src/desktop_notifier/dbus.py`

 * *Files identical despite different names*

### Comparing `desktop_notifier-4.0.0/src/desktop_notifier/dummy.py` & `desktop_notifier-4.0.0.dev0/src/desktop_notifier/dummy.py`

 * *Files identical despite different names*

### Comparing `desktop_notifier-4.0.0/src/desktop_notifier/macos.py` & `desktop_notifier-4.0.0.dev0/src/desktop_notifier/macos.py`

 * *Files identical despite different names*

### Comparing `desktop_notifier-4.0.0/src/desktop_notifier/macos_support.py` & `desktop_notifier-4.0.0.dev0/src/desktop_notifier/macos_support.py`

 * *Files identical despite different names*

### Comparing `desktop_notifier-4.0.0/src/desktop_notifier/main.py` & `desktop_notifier-4.0.0.dev0/src/desktop_notifier/main.py`

 * *Files identical despite different names*

### Comparing `desktop_notifier-4.0.0/src/desktop_notifier/resources/python.png` & `desktop_notifier-4.0.0.dev0/src/desktop_notifier/resources/python.png`

 * *Files identical despite different names*

### Comparing `desktop_notifier-4.0.0/src/desktop_notifier/winrt.py` & `desktop_notifier-4.0.0.dev0/src/desktop_notifier/winrt.py`

 * *Files identical despite different names*

### Comparing `desktop_notifier-4.0.0/src/desktop_notifier.egg-info/PKG-INFO` & `desktop_notifier-4.0.0.dev0/src/desktop_notifier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: desktop-notifier
-Version: 4.0.0
+Version: 4.0.0.dev0
 Summary: Python library for cross-platform desktop notifications
 Author-email: Sam Schott <sam.schott@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/samschott/desktop-notifier
 Keywords: desktop-notifier
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `desktop_notifier-4.0.0/src/desktop_notifier.egg-info/SOURCES.txt` & `desktop_notifier-4.0.0.dev0/src/desktop_notifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `desktop_notifier-4.0.0/tests/test_api.py` & `desktop_notifier-4.0.0.dev0/tests/test_api.py`

 * *Files identical despite different names*

