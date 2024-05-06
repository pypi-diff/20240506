# Comparing `tmp/toga-0.4.2.tar.gz` & `tmp/toga-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toga-0.4.2.tar", last modified: Tue Feb  6 05:54:57 2024, max compression
+gzip compressed data, was "toga-0.4.3.tar", last modified: Mon May  6 06:43:33 2024, max compression
```

## Comparing `toga-0.4.2.tar` & `toga-0.4.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:54:57.843910 toga-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-02-06 05:54:24.000000 toga-0.4.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-02-06 05:54:24.000000 toga-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-02-06 05:54:57.843910 toga-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-02-06 05:54:24.000000 toga-0.4.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-02-06 05:54:24.000000 toga-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 05:54:57.843910 toga-0.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:54:57.843910 toga-0.4.2/toga.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-02-06 05:54:57.000000 toga-0.4.2/toga.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-02-06 05:54:57.000000 toga-0.4.2/toga.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 05:54:57.000000 toga-0.4.2/toga.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-02-06 05:54:57.000000 toga-0.4.2/toga.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 05:54:57.000000 toga-0.4.2/toga.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:33.304445 toga-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-06 06:43:03.000000 toga-0.4.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-06 06:43:03.000000 toga-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-05-06 06:43:33.304445 toga-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-06 06:43:03.000000 toga-0.4.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-06 06:43:03.000000 toga-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 06:43:33.304445 toga-0.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:33.304445 toga-0.4.3/toga.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-05-06 06:43:33.000000 toga-0.4.3/toga.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-06 06:43:33.000000 toga-0.4.3/toga.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 06:43:33.000000 toga-0.4.3/toga.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-06 06:43:33.000000 toga-0.4.3/toga.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 06:43:33.000000 toga-0.4.3/toga.egg-info/top_level.txt
```

### Comparing `toga-0.4.2/LICENSE` & `toga-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `toga-0.4.2/PKG-INFO` & `toga-0.4.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 Metadata-Version: 2.1
 Name: toga
-Version: 0.4.2
+Version: 0.4.3
 Summary: A Python native, OS native GUI toolkit.
 Author-email: Russell Keith-Magee <russell@keith-magee.com>
 Maintainer-email: BeeWare Team <team@beeware.org>
 License: New BSD
 Project-URL: Homepage, https://beeware.org/project/projects/libraries/toga/
 Project-URL: Funding, https://beeware.org/contributing/membership/
-Project-URL: Documentation, https://toga.readthedocs.io/en/latest/
+Project-URL: Documentation, https://toga.readthedocs.io/
 Project-URL: Tracker, https://github.com/beeware/toga/issues
 Project-URL: Source, https://github.com/beeware/toga
+Project-URL: Changelog, https://toga.readthedocs.io/en/stable/background/project/releases.html
 Keywords: gui,widget,cross-platform,toga,desktop,mobile,web,macOS,cocoa,iOS,android,windows,winforms,linux,freeBSD,gtk,console,web
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Software Development :: Widget Sets
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: toga-winforms==0.4.2; sys_platform == "win32"
-Requires-Dist: toga-gtk==0.4.2; sys_platform == "linux"
-Requires-Dist: toga-gtk==0.4.2; "freebsd" in sys_platform
-Requires-Dist: toga-cocoa==0.4.2; sys_platform == "darwin"
-Requires-Dist: toga-iOS==0.4.2; sys_platform == "ios"
-Requires-Dist: toga-android==0.4.2; sys_platform == "android"
-Requires-Dist: toga-web==0.4.2; sys_platform == "emscripten"
+Requires-Dist: toga-winforms==0.4.3; sys_platform == "win32"
+Requires-Dist: toga-gtk==0.4.3; sys_platform == "linux"
+Requires-Dist: toga-gtk==0.4.3; "freebsd" in sys_platform
+Requires-Dist: toga-cocoa==0.4.3; sys_platform == "darwin"
+Requires-Dist: toga-iOS==0.4.3; sys_platform == "ios"
+Requires-Dist: toga-android==0.4.3; sys_platform == "android"
+Requires-Dist: toga-web==0.4.3; sys_platform == "emscripten"
 
 toga
 ====
 
 A meta-package for installing the `Toga widget toolkit`_.
 
 This package installs the `toga-core <https://pypi.org/project/toga-core>`__ library,
@@ -51,15 +53,15 @@
 Backends are also available for `Android <https://pypi.org/project/toga-android>`__,
 `iOS <https://pypi.org/project/toga-iOS>`__, `single-page web apps
 <https://pypi.org/project/toga-web>`__, and `testing
 <https://pypi.org/project/toga-dummy>`__; however, these must be installed manually.
 
 Toga requires **Python 3.8** or newer. It does not support Python 2. Some platforms have
 additional prerequisites; see the `Toga platform guide
-<https://toga.readthedocs.io/en/stable/reference/platforms/index.html>`__ for details.
+<https://toga.readthedocs.io/en/latest/reference/platforms/index.html>`__ for details.
 
 For more details, see the `Toga project on Github`_.
 
 .. _Toga widget toolkit: https://beeware.org/toga
 .. _Toga project on Github: https://github.com/beeware/toga
 
 Community
```

### Comparing `toga-0.4.2/README.rst` & `toga-0.4.3/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Backends are also available for `Android <https://pypi.org/project/toga-android>`__,
 `iOS <https://pypi.org/project/toga-iOS>`__, `single-page web apps
 <https://pypi.org/project/toga-web>`__, and `testing
 <https://pypi.org/project/toga-dummy>`__; however, these must be installed manually.
 
 Toga requires **Python 3.8** or newer. It does not support Python 2. Some platforms have
 additional prerequisites; see the `Toga platform guide
-<https://toga.readthedocs.io/en/stable/reference/platforms/index.html>`__ for details.
+<https://toga.readthedocs.io/en/latest/reference/platforms/index.html>`__ for details.
 
 For more details, see the `Toga project on Github`_.
 
 .. _Toga widget toolkit: https://beeware.org/toga
 .. _Toga project on Github: https://github.com/beeware/toga
 
 Community
```

### Comparing `toga-0.4.2/pyproject.toml` & `toga-0.4.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [build-system]
 requires = [
-    "setuptools==69.0.0",
+    "setuptools==69.5.1",
     "setuptools_scm==8.0.4",
     "setuptools_dynamic_dependencies @ git+https://github.com/beeware/setuptools_dynamic_dependencies",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 dynamic = ["version", "dependencies"]
@@ -46,26 +46,28 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: 3.13",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Software Development",
     "Topic :: Software Development :: User Interfaces",
     "Topic :: Software Development :: Widget Sets",
 ]
 
 [project.urls]
 Homepage = "https://beeware.org/project/projects/libraries/toga/"
 Funding = "https://beeware.org/contributing/membership/"
-Documentation = "https://toga.readthedocs.io/en/latest/"
+Documentation = "https://toga.readthedocs.io/"
 Tracker = "https://github.com/beeware/toga/issues"
 Source = "https://github.com/beeware/toga"
+Changelog = "https://toga.readthedocs.io/en/stable/background/project/releases.html"
 
 [tool.setuptools_scm]
 root = ".."
 
 [tool.setuptools_dynamic_dependencies]
 dependencies = [
     # Desktop platforms
```

### Comparing `toga-0.4.2/toga.egg-info/PKG-INFO` & `toga-0.4.3/toga.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 Metadata-Version: 2.1
 Name: toga
-Version: 0.4.2
+Version: 0.4.3
 Summary: A Python native, OS native GUI toolkit.
 Author-email: Russell Keith-Magee <russell@keith-magee.com>
 Maintainer-email: BeeWare Team <team@beeware.org>
 License: New BSD
 Project-URL: Homepage, https://beeware.org/project/projects/libraries/toga/
 Project-URL: Funding, https://beeware.org/contributing/membership/
-Project-URL: Documentation, https://toga.readthedocs.io/en/latest/
+Project-URL: Documentation, https://toga.readthedocs.io/
 Project-URL: Tracker, https://github.com/beeware/toga/issues
 Project-URL: Source, https://github.com/beeware/toga
+Project-URL: Changelog, https://toga.readthedocs.io/en/stable/background/project/releases.html
 Keywords: gui,widget,cross-platform,toga,desktop,mobile,web,macOS,cocoa,iOS,android,windows,winforms,linux,freeBSD,gtk,console,web
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Software Development :: Widget Sets
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: toga-winforms==0.4.2; sys_platform == "win32"
-Requires-Dist: toga-gtk==0.4.2; sys_platform == "linux"
-Requires-Dist: toga-gtk==0.4.2; "freebsd" in sys_platform
-Requires-Dist: toga-cocoa==0.4.2; sys_platform == "darwin"
-Requires-Dist: toga-iOS==0.4.2; sys_platform == "ios"
-Requires-Dist: toga-android==0.4.2; sys_platform == "android"
-Requires-Dist: toga-web==0.4.2; sys_platform == "emscripten"
+Requires-Dist: toga-winforms==0.4.3; sys_platform == "win32"
+Requires-Dist: toga-gtk==0.4.3; sys_platform == "linux"
+Requires-Dist: toga-gtk==0.4.3; "freebsd" in sys_platform
+Requires-Dist: toga-cocoa==0.4.3; sys_platform == "darwin"
+Requires-Dist: toga-iOS==0.4.3; sys_platform == "ios"
+Requires-Dist: toga-android==0.4.3; sys_platform == "android"
+Requires-Dist: toga-web==0.4.3; sys_platform == "emscripten"
 
 toga
 ====
 
 A meta-package for installing the `Toga widget toolkit`_.
 
 This package installs the `toga-core <https://pypi.org/project/toga-core>`__ library,
@@ -51,15 +53,15 @@
 Backends are also available for `Android <https://pypi.org/project/toga-android>`__,
 `iOS <https://pypi.org/project/toga-iOS>`__, `single-page web apps
 <https://pypi.org/project/toga-web>`__, and `testing
 <https://pypi.org/project/toga-dummy>`__; however, these must be installed manually.
 
 Toga requires **Python 3.8** or newer. It does not support Python 2. Some platforms have
 additional prerequisites; see the `Toga platform guide
-<https://toga.readthedocs.io/en/stable/reference/platforms/index.html>`__ for details.
+<https://toga.readthedocs.io/en/latest/reference/platforms/index.html>`__ for details.
 
 For more details, see the `Toga project on Github`_.
 
 .. _Toga widget toolkit: https://beeware.org/toga
 .. _Toga project on Github: https://github.com/beeware/toga
 
 Community
```

