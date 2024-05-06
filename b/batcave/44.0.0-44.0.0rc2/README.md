# Comparing `tmp/batcave-44.0.0.tar.gz` & `tmp/batcave-44.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batcave-44.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "batcave-44.0.0rc2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `batcave-44.0.0.tar` & `batcave-44.0.0rc2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0     2198 2024-05-06 00:59:48.263631 batcave-44.0.0/.github/workflows/build.yml
--rw-r--r--   0        0        0     2329 2024-05-06 00:59:48.263631 batcave-44.0.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     4803 2024-05-06 00:59:48.263631 batcave-44.0.0/.gitignore
--rw-r--r--   0        0        0       23 2024-05-06 00:59:48.263631 batcave-44.0.0/.p4cfg
--rw-r--r--   0        0        0     5056 2024-05-06 00:59:48.263631 batcave-44.0.0/.p4ignore
--rw-r--r--   0        0        0      158 2024-05-06 00:59:48.267631 batcave-44.0.0/.pypirc
--rw-r--r--   0        0        0       39 2024-05-06 00:59:48.267631 batcave-44.0.0/.readthedocs.yml
--rw-r--r--   0        0        0     4034 2024-05-06 00:59:48.267631 batcave-44.0.0/.vscode/.ropeproject/config.py
--rw-r--r--   0        0        0      592 2024-05-06 00:59:48.267631 batcave-44.0.0/.vscode/.ropeproject/objectdb
--rw-r--r--   0        0        0     5757 2024-05-06 00:59:48.267631 batcave-44.0.0/.vscode/launch.json
--rw-r--r--   0        0        0      468 2024-05-06 00:59:48.267631 batcave-44.0.0/.vscode/tasks.json
--rw-r--r--   0        0        0    40434 2024-05-06 00:59:48.267631 batcave-44.0.0/CHANGELOG.md
--rw-r--r--   0        0        0       86 2024-05-06 00:59:48.267631 batcave-44.0.0/DOCUMENTATION.md
--rw-r--r--   0        0        0     1072 2024-05-06 00:59:48.267631 batcave-44.0.0/LICENSE
--rw-r--r--   0        0        0       93 2024-05-06 00:59:48.267631 batcave-44.0.0/MANIFEST.in
--rw-r--r--   0        0        0     1150 2024-05-06 00:59:48.267631 batcave-44.0.0/README.md
--rw-r--r--   0        0        0     1834 2024-05-06 01:00:21.495251 batcave-44.0.0/batcave/__init__.py
--rw-r--r--   0        0        0     5485 2024-05-06 00:59:48.267631 batcave-44.0.0/batcave/automation.py
--rw-r--r--   0        0        0    14410 2024-05-06 00:59:48.267631 batcave-44.0.0/batcave/cloudmgr.py
--rw-r--r--   0        0        0    74565 2024-05-06 00:59:48.267631 batcave-44.0.0/batcave/cms.py
--rw-r--r--   0        0        0     8590 2024-05-06 00:59:48.267631 batcave-44.0.0/batcave/commander.py
--rw-r--r--   0        0        0     9592 2024-05-06 00:59:48.267631 batcave-44.0.0/batcave/configmgr.py
--rw-r--r--   0        0        0    27694 2024-05-06 00:59:48.267631 batcave-44.0.0/batcave/data.py
--rw-r--r--   0        0        0    31760 2024-05-06 00:59:48.267631 batcave-44.0.0/batcave/expander.py
--rw-r--r--   0        0        0    10792 2024-05-06 00:59:48.267631 batcave-44.0.0/batcave/fileutil.py
--rw-r--r--   0        0        0    10747 2024-05-06 00:59:48.267631 batcave-44.0.0/batcave/gui.py
--rw-r--r--   0        0        0    28944 2024-05-06 00:59:48.267631 batcave-44.0.0/batcave/iispy.py
--rw-r--r--   0        0        0    22561 2024-05-06 00:59:48.267631 batcave-44.0.0/batcave/k8s.py
--rw-r--r--   0        0        0    10608 2024-05-06 00:59:48.267631 batcave-44.0.0/batcave/lang.py
--rw-r--r--   0        0        0     3035 2024-05-06 00:59:48.267631 batcave-44.0.0/batcave/menu.py
--rw-r--r--   0        0        0     2378 2024-05-06 00:59:48.267631 batcave-44.0.0/batcave/netutil.py
--rw-r--r--   0        0        0     3842 2024-05-06 00:59:48.267631 batcave-44.0.0/batcave/platarch.py
--rw-r--r--   0        0        0        0 2024-05-06 00:59:48.267631 batcave-44.0.0/batcave/py.typed
--rw-r--r--   0        0        0    13106 2024-05-06 00:59:48.267631 batcave-44.0.0/batcave/qbpy.py
--rw-r--r--   0        0        0    28343 2024-05-06 00:59:48.267631 batcave-44.0.0/batcave/reporter.py
--rw-r--r--   0        0        0    52861 2024-05-06 00:59:48.267631 batcave-44.0.0/batcave/servermgr.py
--rw-r--r--   0        0        0    11200 2024-05-06 00:59:48.271631 batcave-44.0.0/batcave/serverpath.py
--rw-r--r--   0        0        0     7801 2024-05-06 00:59:48.271631 batcave-44.0.0/batcave/statemachine.py
--rw-r--r--   0        0        0    23562 2024-05-06 00:59:48.271631 batcave-44.0.0/batcave/sysutil.py
--rw-r--r--   0        0        0     5429 2024-05-06 00:59:48.271631 batcave-44.0.0/batcave/tcpy.py
--rw-r--r--   0        0        0     3342 2024-05-06 00:59:48.271631 batcave-44.0.0/batcave/time.py
--rw-r--r--   0        0        0     3340 2024-05-06 00:59:48.271631 batcave-44.0.0/batcave/version.py
--rw-r--r--   0        0        0      634 2024-05-06 00:59:48.271631 batcave-44.0.0/docs/Makefile
--rw-r--r--   0        0        0     3747 2024-05-06 00:59:48.271631 batcave-44.0.0/docs/batcave.rst
--rw-r--r--   0        0        0     9167 2024-05-06 00:59:48.271631 batcave-44.0.0/docs/coding_standards.py
--rw-r--r--   0        0        0     2109 2024-05-06 00:59:48.271631 batcave-44.0.0/docs/conf.py
--rw-r--r--   0        0        0      469 2024-05-06 00:59:48.271631 batcave-44.0.0/docs/index.rst
--rw-r--r--   0        0        0      795 2024-05-06 00:59:48.271631 batcave-44.0.0/docs/make.bat
--rw-r--r--   0        0        0       65 2024-05-06 00:59:48.271631 batcave-44.0.0/docs/modules.rst
--rw-r--r--   0        0        0      229 2024-05-06 00:59:48.271631 batcave-44.0.0/docs/requirements.txt
--rw-r--r--   0        0        0     2825 2024-05-06 01:00:21.495251 batcave-44.0.0/pyproject.toml
--rw-r--r--   0        0        0       44 2024-05-06 00:59:48.271631 batcave-44.0.0/tests/__init__.py
--rw-r--r--   0        0        0     2808 2024-05-06 00:59:48.271631 batcave-44.0.0/tests/test_fileutil.py
--rw-r--r--   0        0        0     1288 2024-05-06 00:59:48.271631 batcave-44.0.0/tests/test_lang.py
--rw-r--r--   0        0        0     2806 2024-05-06 00:59:48.271631 batcave-44.0.0/tests/test_statemachine.py
--rw-r--r--   0        0        0     3132 2024-05-06 00:59:48.271631 batcave-44.0.0/tests/test_sysutil.py
--rw-r--r--   0        0        0      305 2024-05-06 00:59:48.271631 batcave-44.0.0/util/New-Env.ps1
--rw-r--r--   0        0        0      259 2024-05-06 00:59:48.271631 batcave-44.0.0/util/Update-Env.ps1
--rw-r--r--   0        0        0      261 2024-05-06 00:59:48.271631 batcave-44.0.0/util/new-env.sh
--rw-r--r--   0        0        0      234 2024-05-06 00:59:48.271631 batcave-44.0.0/util/update-env.sh
--rw-r--r--   0        0        0      511 2024-05-06 00:59:48.271631 batcave-44.0.0/vjer.yml
--rw-r--r--   0        0        0     1516 1970-01-01 00:00:00.000000 batcave-44.0.0/setup.py
--rw-r--r--   0        0        0     2222 1970-01-01 00:00:00.000000 batcave-44.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2198 2024-05-05 23:16:15.380723 batcave-44.0.0rc2/.github/workflows/build.yml
+-rw-r--r--   0        0        0     2329 2024-05-05 23:16:15.380723 batcave-44.0.0rc2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     4803 2024-05-05 23:16:15.380723 batcave-44.0.0rc2/.gitignore
+-rw-r--r--   0        0        0       23 2024-05-05 23:16:15.380723 batcave-44.0.0rc2/.p4cfg
+-rw-r--r--   0        0        0     5056 2024-05-05 23:16:15.380723 batcave-44.0.0rc2/.p4ignore
+-rw-r--r--   0        0        0      158 2024-05-05 23:16:15.380723 batcave-44.0.0rc2/.pypirc
+-rw-r--r--   0        0        0       39 2024-05-05 23:16:15.380723 batcave-44.0.0rc2/.readthedocs.yml
+-rw-r--r--   0        0        0     4034 2024-05-05 23:16:15.380723 batcave-44.0.0rc2/.vscode/.ropeproject/config.py
+-rw-r--r--   0        0        0      592 2024-05-05 23:16:15.380723 batcave-44.0.0rc2/.vscode/.ropeproject/objectdb
+-rw-r--r--   0        0        0     5757 2024-05-05 23:16:15.380723 batcave-44.0.0rc2/.vscode/launch.json
+-rw-r--r--   0        0        0      468 2024-05-05 23:16:15.380723 batcave-44.0.0rc2/.vscode/tasks.json
+-rw-r--r--   0        0        0    40434 2024-05-05 23:16:15.384723 batcave-44.0.0rc2/CHANGELOG.md
+-rw-r--r--   0        0        0       86 2024-05-05 23:16:15.384723 batcave-44.0.0rc2/DOCUMENTATION.md
+-rw-r--r--   0        0        0     1072 2024-05-05 23:16:15.384723 batcave-44.0.0rc2/LICENSE
+-rw-r--r--   0        0        0       93 2024-05-05 23:16:15.384723 batcave-44.0.0rc2/MANIFEST.in
+-rw-r--r--   0        0        0     1150 2024-05-05 23:16:15.384723 batcave-44.0.0rc2/README.md
+-rw-r--r--   0        0        0     1894 2024-05-05 23:16:15.384723 batcave-44.0.0rc2/batcave/__init__.py
+-rw-r--r--   0        0        0     5485 2024-05-05 23:16:15.384723 batcave-44.0.0rc2/batcave/automation.py
+-rw-r--r--   0        0        0    14410 2024-05-05 23:16:15.384723 batcave-44.0.0rc2/batcave/cloudmgr.py
+-rw-r--r--   0        0        0    74565 2024-05-05 23:16:15.384723 batcave-44.0.0rc2/batcave/cms.py
+-rw-r--r--   0        0        0     8590 2024-05-05 23:16:15.384723 batcave-44.0.0rc2/batcave/commander.py
+-rw-r--r--   0        0        0     9592 2024-05-05 23:16:15.384723 batcave-44.0.0rc2/batcave/configmgr.py
+-rw-r--r--   0        0        0    27694 2024-05-05 23:16:15.384723 batcave-44.0.0rc2/batcave/data.py
+-rw-r--r--   0        0        0    31760 2024-05-05 23:16:15.384723 batcave-44.0.0rc2/batcave/expander.py
+-rw-r--r--   0        0        0    10792 2024-05-05 23:16:15.384723 batcave-44.0.0rc2/batcave/fileutil.py
+-rw-r--r--   0        0        0    10747 2024-05-05 23:16:15.384723 batcave-44.0.0rc2/batcave/gui.py
+-rw-r--r--   0        0        0    28944 2024-05-05 23:16:15.384723 batcave-44.0.0rc2/batcave/iispy.py
+-rw-r--r--   0        0        0    22561 2024-05-05 23:16:15.384723 batcave-44.0.0rc2/batcave/k8s.py
+-rw-r--r--   0        0        0    10608 2024-05-05 23:16:15.384723 batcave-44.0.0rc2/batcave/lang.py
+-rw-r--r--   0        0        0     3035 2024-05-05 23:16:15.384723 batcave-44.0.0rc2/batcave/menu.py
+-rw-r--r--   0        0        0     2378 2024-05-05 23:16:15.384723 batcave-44.0.0rc2/batcave/netutil.py
+-rw-r--r--   0        0        0     3842 2024-05-05 23:16:15.384723 batcave-44.0.0rc2/batcave/platarch.py
+-rw-r--r--   0        0        0        0 2024-05-05 23:16:15.384723 batcave-44.0.0rc2/batcave/py.typed
+-rw-r--r--   0        0        0    13106 2024-05-05 23:16:15.384723 batcave-44.0.0rc2/batcave/qbpy.py
+-rw-r--r--   0        0        0    28343 2024-05-05 23:16:15.384723 batcave-44.0.0rc2/batcave/reporter.py
+-rw-r--r--   0        0        0    52861 2024-05-05 23:16:15.384723 batcave-44.0.0rc2/batcave/servermgr.py
+-rw-r--r--   0        0        0    11200 2024-05-05 23:16:15.384723 batcave-44.0.0rc2/batcave/serverpath.py
+-rw-r--r--   0        0        0     7801 2024-05-05 23:16:15.384723 batcave-44.0.0rc2/batcave/statemachine.py
+-rw-r--r--   0        0        0    23562 2024-05-05 23:16:15.384723 batcave-44.0.0rc2/batcave/sysutil.py
+-rw-r--r--   0        0        0     5429 2024-05-05 23:16:15.384723 batcave-44.0.0rc2/batcave/tcpy.py
+-rw-r--r--   0        0        0     3342 2024-05-05 23:16:15.384723 batcave-44.0.0rc2/batcave/time.py
+-rw-r--r--   0        0        0     3340 2024-05-05 23:16:15.384723 batcave-44.0.0rc2/batcave/version.py
+-rw-r--r--   0        0        0      634 2024-05-05 23:16:15.384723 batcave-44.0.0rc2/docs/Makefile
+-rw-r--r--   0        0        0     3747 2024-05-05 23:16:15.384723 batcave-44.0.0rc2/docs/batcave.rst
+-rw-r--r--   0        0        0     9167 2024-05-05 23:16:15.388723 batcave-44.0.0rc2/docs/coding_standards.py
+-rw-r--r--   0        0        0     2109 2024-05-05 23:16:15.388723 batcave-44.0.0rc2/docs/conf.py
+-rw-r--r--   0        0        0      469 2024-05-05 23:16:15.388723 batcave-44.0.0rc2/docs/index.rst
+-rw-r--r--   0        0        0      795 2024-05-05 23:16:15.388723 batcave-44.0.0rc2/docs/make.bat
+-rw-r--r--   0        0        0       65 2024-05-05 23:16:15.388723 batcave-44.0.0rc2/docs/modules.rst
+-rw-r--r--   0        0        0      229 2024-05-05 23:16:15.388723 batcave-44.0.0rc2/docs/requirements.txt
+-rw-r--r--   0        0        0     2943 2024-05-05 23:16:15.388723 batcave-44.0.0rc2/pyproject.toml
+-rw-r--r--   0        0        0       44 2024-05-05 23:16:15.388723 batcave-44.0.0rc2/tests/__init__.py
+-rw-r--r--   0        0        0     2808 2024-05-05 23:16:15.388723 batcave-44.0.0rc2/tests/test_fileutil.py
+-rw-r--r--   0        0        0     1288 2024-05-05 23:16:15.388723 batcave-44.0.0rc2/tests/test_lang.py
+-rw-r--r--   0        0        0     2806 2024-05-05 23:16:15.388723 batcave-44.0.0rc2/tests/test_statemachine.py
+-rw-r--r--   0        0        0     3132 2024-05-05 23:16:15.388723 batcave-44.0.0rc2/tests/test_sysutil.py
+-rw-r--r--   0        0        0      305 2024-05-05 23:16:15.388723 batcave-44.0.0rc2/util/New-Env.ps1
+-rw-r--r--   0        0        0      259 2024-05-05 23:16:15.388723 batcave-44.0.0rc2/util/Update-Env.ps1
+-rw-r--r--   0        0        0      261 2024-05-05 23:16:15.388723 batcave-44.0.0rc2/util/new-env.sh
+-rw-r--r--   0        0        0      234 2024-05-05 23:16:15.388723 batcave-44.0.0rc2/util/update-env.sh
+-rw-r--r--   0        0        0      511 2024-05-05 23:16:15.388723 batcave-44.0.0rc2/vjer.yml
+-rw-r--r--   0        0        0     1519 1970-01-01 00:00:00.000000 batcave-44.0.0rc2/setup.py
+-rw-r--r--   0        0        0     2225 1970-01-01 00:00:00.000000 batcave-44.0.0rc2/PKG-INFO
```

### Comparing `batcave-44.0.0/.github/workflows/build.yml` & `batcave-44.0.0rc2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/.github/workflows/publish.yml` & `batcave-44.0.0rc2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/.gitignore` & `batcave-44.0.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/.p4ignore` & `batcave-44.0.0rc2/.p4ignore`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/.vscode/.ropeproject/config.py` & `batcave-44.0.0rc2/.vscode/.ropeproject/config.py`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/.vscode/.ropeproject/objectdb` & `batcave-44.0.0rc2/.vscode/.ropeproject/objectdb`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/.vscode/launch.json` & `batcave-44.0.0rc2/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/CHANGELOG.md` & `batcave-44.0.0rc2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/LICENSE` & `batcave-44.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/README.md` & `batcave-44.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/batcave/__init__.py` & `batcave-44.0.0rc2/batcave/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-"""BatCave Utilities module.
-
-This module provides utilities for making it easier to write Python programs.
-
-The exported modules fall into several categories:
-
-Modules that provide simplified interfaces to standard modules:
-    * commander - argparse
-    * platarch - platform
-
-Modules that provide simplified interfaces to third-party modules:
-    * gui - PyQt5
-    * k8s - kubernetes
-
-Modules that provide Pythonic interfaces to external systems:
-    * cloudmgr - cloud resources
-    * cms - code management systems
-    * data - data sources
-    * iispy - Internet Information Server
-    * netutil - network services
-    * qbpy - QuickBuild
-    * servermgr - OS-independent servers
-    * sysutil - system utilities
-    * tcpy - TeamCity
-
-Modules that provide utilities for accomplishing specific programming tasks:
-    * automation - building automation
-    * configmgr - managing configurations
-    * expander - working with string expansion
-    * fileutil - working with files
-    * lang - Python language utilities
-    * menu - creating command line menus
-    * statemachine - a simple state machine
-    * reporter - creating reports
-    * version - reporting version information
-"""
-
-__all__ = ('__title__', '__summary__', '__uri__',
-           '__version__', '__build_name__', '__build_date__',
-           '__author__', '__email__',
-           '__license__', '__copyright__')
-
-__title__ = 'BatCave'
-__summary__ = 'Python Programming Toolkit'
-__uri__ = 'https://github.com/tardis4500/batcave/'
-
-__version__ = '44.0.0'
-__build_name__ = '{var:build_name}'
-__build_date__ = '{var:build_date}'
-
-__author__ = 'Jeffery G. Smith'
-__email__ = 'web@pobox.com'
-
-__license__ = 'MIT'
-__copyright__ = 'Copyright (c) 2023 Jeffery G. Smith'
-
-# cSpell:ignore iispy netutil qbpy tcpy platarch cloudmgr servermgr configmgr fileutil statemachine
+"""BatCave Utilities module.
+
+This module provides utilities for making it easier to write Python programs.
+
+The exported modules fall into several categories:
+
+Modules that provide simplified interfaces to standard modules:
+    * commander - argparse
+    * platarch - platform
+
+Modules that provide simplified interfaces to third-party modules:
+    * gui - PyQt5
+    * k8s - kubernetes
+
+Modules that provide Pythonic interfaces to external systems:
+    * cloudmgr - cloud resources
+    * cms - code management systems
+    * data - data sources
+    * iispy - Internet Information Server
+    * netutil - network services
+    * qbpy - QuickBuild
+    * servermgr - OS-independent servers
+    * sysutil - system utilities
+    * tcpy - TeamCity
+
+Modules that provide utilities for accomplishing specific programming tasks:
+    * automation - building automation
+    * configmgr - managing configurations
+    * expander - working with string expansion
+    * fileutil - working with files
+    * lang - Python language utilities
+    * menu - creating command line menus
+    * statemachine - a simple state machine
+    * reporter - creating reports
+    * version - reporting version information
+"""
+
+__all__ = ('__title__', '__summary__', '__uri__',
+           '__version__', '__build_name__', '__build_date__',
+           '__author__', '__email__',
+           '__license__', '__copyright__')
+
+__title__ = 'BatCave'
+__summary__ = 'Python Programming Toolkit'
+__uri__ = 'https://github.com/tardis4500/batcave/'
+
+__version__ = '44.0.0rc2'
+__build_name__ = '{var:build_name}'
+__build_date__ = '{var:build_date}'
+
+__author__ = 'Jeffery G. Smith'
+__email__ = 'web@pobox.com'
+
+__license__ = 'MIT'
+__copyright__ = 'Copyright (c) 2023 Jeffery G. Smith'
+
+# cSpell:ignore iispy netutil qbpy tcpy platarch cloudmgr servermgr configmgr fileutil statemachine
```

### Comparing `batcave-44.0.0/batcave/automation.py` & `batcave-44.0.0rc2/batcave/automation.py`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/batcave/cloudmgr.py` & `batcave-44.0.0rc2/batcave/cloudmgr.py`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/batcave/cms.py` & `batcave-44.0.0rc2/batcave/cms.py`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/batcave/commander.py` & `batcave-44.0.0rc2/batcave/commander.py`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/batcave/configmgr.py` & `batcave-44.0.0rc2/batcave/configmgr.py`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/batcave/data.py` & `batcave-44.0.0rc2/batcave/data.py`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/batcave/expander.py` & `batcave-44.0.0rc2/batcave/expander.py`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/batcave/fileutil.py` & `batcave-44.0.0rc2/batcave/fileutil.py`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/batcave/gui.py` & `batcave-44.0.0rc2/batcave/gui.py`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/batcave/iispy.py` & `batcave-44.0.0rc2/batcave/iispy.py`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/batcave/k8s.py` & `batcave-44.0.0rc2/batcave/k8s.py`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/batcave/lang.py` & `batcave-44.0.0rc2/batcave/lang.py`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/batcave/menu.py` & `batcave-44.0.0rc2/batcave/menu.py`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/batcave/netutil.py` & `batcave-44.0.0rc2/batcave/netutil.py`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/batcave/platarch.py` & `batcave-44.0.0rc2/batcave/platarch.py`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/batcave/qbpy.py` & `batcave-44.0.0rc2/batcave/qbpy.py`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/batcave/reporter.py` & `batcave-44.0.0rc2/batcave/reporter.py`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/batcave/servermgr.py` & `batcave-44.0.0rc2/batcave/servermgr.py`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/batcave/serverpath.py` & `batcave-44.0.0rc2/batcave/serverpath.py`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/batcave/statemachine.py` & `batcave-44.0.0rc2/batcave/statemachine.py`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/batcave/sysutil.py` & `batcave-44.0.0rc2/batcave/sysutil.py`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/batcave/tcpy.py` & `batcave-44.0.0rc2/batcave/tcpy.py`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/batcave/time.py` & `batcave-44.0.0rc2/batcave/time.py`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/batcave/version.py` & `batcave-44.0.0rc2/batcave/version.py`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/docs/Makefile` & `batcave-44.0.0rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/docs/batcave.rst` & `batcave-44.0.0rc2/docs/batcave.rst`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/docs/coding_standards.py` & `batcave-44.0.0rc2/docs/coding_standards.py`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/docs/conf.py` & `batcave-44.0.0rc2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/docs/make.bat` & `batcave-44.0.0rc2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/tests/test_fileutil.py` & `batcave-44.0.0rc2/tests/test_fileutil.py`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/tests/test_lang.py` & `batcave-44.0.0rc2/tests/test_lang.py`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/tests/test_statemachine.py` & `batcave-44.0.0rc2/tests/test_statemachine.py`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/tests/test_sysutil.py` & `batcave-44.0.0rc2/tests/test_sysutil.py`

 * *Files identical despite different names*

### Comparing `batcave-44.0.0/setup.py` & `batcave-44.0.0rc2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,15 +35,15 @@
           'types-PyYAML',
           'types-psutil',
           'types-requests',
           'unittest-xml-reporting'],
  "test:sys_platform == 'win32'": ['types-pywin32']}
 
 setup(name='batcave',
-      version='44.0.0',
+      version='44.0.0rc2',
       description='BatCave Utilities module.',
       author=None,
       author_email='"Jeffery G. Smith" <web@pobox.com>',
       url=None,
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

### Comparing `batcave-44.0.0/PKG-INFO` & `batcave-44.0.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batcave
-Version: 44.0.0
+Version: 44.0.0rc2
 Summary: BatCave Utilities module.
 Keywords: python,programming,utilities
 Author-email: "Jeffery G. Smith" <web@pobox.com>
 Requires-Python: ~=3.11
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

