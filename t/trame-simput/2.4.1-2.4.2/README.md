# Comparing `tmp/trame-simput-2.4.1.tar.gz` & `tmp/trame-simput-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-simput-2.4.1.tar", last modified: Fri Jan  5 08:58:39 2024, max compression
+gzip compressed data, was "trame-simput-2.4.2.tar", last modified: Mon May  6 14:27:00 2024, max compression
```

## Comparing `trame-simput-2.4.1.tar` & `trame-simput-2.4.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:58:39.242319 trame-simput-2.4.1/
--rw-r--r--   0 root         (0) root         (0)      583 2024-01-05 08:58:02.000000 trame-simput-2.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       32 2024-01-05 08:58:02.000000 trame-simput-2.4.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4666 2024-01-05 08:58:39.242319 trame-simput-2.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3894 2024-01-05 08:58:02.000000 trame-simput-2.4.1/README.rst
--rw-r--r--   0 root         (0) root         (0)      923 2024-01-05 08:58:39.242319 trame-simput-2.4.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-05 08:58:02.000000 trame-simput-2.4.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:58:39.234319 trame-simput-2.4.1/trame/
--rw-r--r--   0 root         (0) root         (0)       65 2024-01-05 08:58:02.000000 trame-simput-2.4.1/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:58:39.234319 trame-simput-2.4.1/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       65 2024-01-05 08:58:02.000000 trame-simput-2.4.1/trame/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)       34 2024-01-05 08:58:02.000000 trame-simput-2.4.1/trame/modules/simput.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:58:39.234319 trame-simput-2.4.1/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2024-01-05 08:58:02.000000 trame-simput-2.4.1/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      138 2024-01-05 08:58:02.000000 trame-simput-2.4.1/trame/widgets/simput.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:58:39.234319 trame-simput-2.4.1/trame_simput/
--rw-r--r--   0 root         (0) root         (0)      192 2024-01-05 08:58:02.000000 trame-simput-2.4.1/trame_simput/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:58:39.238319 trame-simput-2.4.1/trame_simput/core/
--rw-r--r--   0 root         (0) root         (0)       81 2024-01-05 08:58:02.000000 trame-simput-2.4.1/trame_simput/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9142 2024-01-05 08:58:02.000000 trame-simput-2.4.1/trame_simput/core/domains.py
--rw-r--r--   0 root         (0) root         (0)      648 2024-01-05 08:58:02.000000 trame-simput-2.4.1/trame_simput/core/factory.py
--rw-r--r--   0 root         (0) root         (0)     1985 2024-01-05 08:58:02.000000 trame-simput-2.4.1/trame_simput/core/mapping.py
--rw-r--r--   0 root         (0) root         (0)    29212 2024-01-05 08:58:02.000000 trame-simput-2.4.1/trame_simput/core/proxy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:58:39.238319 trame-simput-2.4.1/trame_simput/core/ui/
--rw-r--r--   0 root         (0) root         (0)      133 2024-01-05 08:58:02.000000 trame-simput-2.4.1/trame_simput/core/ui/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4685 2024-01-05 08:58:02.000000 trame-simput-2.4.1/trame_simput/core/ui/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:58:39.238319 trame-simput-2.4.1/trame_simput/core/ui/resolvers/
--rw-r--r--   0 root         (0) root         (0)       75 2024-01-05 08:58:02.000000 trame-simput-2.4.1/trame_simput/core/ui/resolvers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4997 2024-01-05 08:58:02.000000 trame-simput-2.4.1/trame_simput/core/ui/resolvers/vuetify.py
--rw-r--r--   0 root         (0) root         (0)     1810 2024-01-05 08:58:02.000000 trame-simput-2.4.1/trame_simput/core/ui/utils.py
--rw-r--r--   0 root         (0) root         (0)      672 2024-01-05 08:58:02.000000 trame-simput-2.4.1/trame_simput/core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:58:39.238319 trame-simput-2.4.1/trame_simput/module/
--rw-r--r--   0 root         (0) root         (0)      979 2024-01-05 08:58:02.000000 trame-simput-2.4.1/trame_simput/module/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8342 2024-01-05 08:58:02.000000 trame-simput-2.4.1/trame_simput/module/core.py
--rw-r--r--   0 root         (0) root         (0)     3257 2024-01-05 08:58:02.000000 trame-simput-2.4.1/trame_simput/module/protocol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:58:39.242319 trame-simput-2.4.1/trame_simput/module/serve/
--rw-r--r--   0 root         (0) root         (0)      208 2024-01-05 08:58:29.000000 trame-simput-2.4.1/trame_simput/module/serve/demo.html
--rw-r--r--   0 root         (0) root         (0)   326277 2024-01-05 08:58:29.000000 trame-simput-2.4.1/trame_simput/module/serve/vue-trame_simput.common.js
--rw-r--r--   0 root         (0) root         (0)   450349 2024-01-05 08:58:29.000000 trame-simput-2.4.1/trame_simput/module/serve/vue-trame_simput.common.js.map
--rw-r--r--   0 root         (0) root         (0)   326677 2024-01-05 08:58:29.000000 trame-simput-2.4.1/trame_simput/module/serve/vue-trame_simput.umd.js
--rw-r--r--   0 root         (0) root         (0)   450910 2024-01-05 08:58:29.000000 trame-simput-2.4.1/trame_simput/module/serve/vue-trame_simput.umd.js.map
--rw-r--r--   0 root         (0) root         (0)   113788 2024-01-05 08:58:30.000000 trame-simput-2.4.1/trame_simput/module/serve/vue-trame_simput.umd.min.js
--rw-r--r--   0 root         (0) root         (0)   482718 2024-01-05 08:58:30.000000 trame-simput-2.4.1/trame_simput/module/serve/vue-trame_simput.umd.min.js.map
--rw-r--r--   0 root         (0) root         (0)    80369 2024-01-05 08:58:36.000000 trame-simput-2.4.1/trame_simput/module/serve/vue3-trame_simput.umd.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:58:39.242319 trame-simput-2.4.1/trame_simput/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-05 08:58:02.000000 trame-simput-2.4.1/trame_simput/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4997 2024-01-05 08:58:02.000000 trame-simput-2.4.1/trame_simput/widgets/simput.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:58:39.234319 trame-simput-2.4.1/trame_simput.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4666 2024-01-05 08:58:39.000000 trame-simput-2.4.1/trame_simput.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1291 2024-01-05 08:58:39.000000 trame-simput-2.4.1/trame_simput.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-05 08:58:39.000000 trame-simput-2.4.1/trame_simput.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-01-05 08:58:39.000000 trame-simput-2.4.1/trame_simput.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-01-05 08:58:39.000000 trame-simput-2.4.1/trame_simput.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 14:27:00.057639 trame-simput-2.4.2/
+-rw-r--r--   0 root         (0) root         (0)      583 2024-05-06 14:26:23.000000 trame-simput-2.4.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       32 2024-05-06 14:26:23.000000 trame-simput-2.4.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4666 2024-05-06 14:27:00.057639 trame-simput-2.4.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3894 2024-05-06 14:26:23.000000 trame-simput-2.4.2/README.rst
+-rw-r--r--   0 root         (0) root         (0)      923 2024-05-06 14:27:00.057639 trame-simput-2.4.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-06 14:26:23.000000 trame-simput-2.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 14:27:00.045639 trame-simput-2.4.2/trame/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 14:27:00.049639 trame-simput-2.4.2/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       34 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame/modules/simput.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 14:27:00.049639 trame-simput-2.4.2/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      138 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame/widgets/simput.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 14:27:00.049639 trame-simput-2.4.2/trame_simput/
+-rw-r--r--   0 root         (0) root         (0)      192 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame_simput/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 14:27:00.049639 trame-simput-2.4.2/trame_simput/core/
+-rw-r--r--   0 root         (0) root         (0)       81 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame_simput/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9142 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame_simput/core/domains.py
+-rw-r--r--   0 root         (0) root         (0)      648 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame_simput/core/factory.py
+-rw-r--r--   0 root         (0) root         (0)     1985 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame_simput/core/mapping.py
+-rw-r--r--   0 root         (0) root         (0)    29212 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame_simput/core/proxy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 14:27:00.049639 trame-simput-2.4.2/trame_simput/core/ui/
+-rw-r--r--   0 root         (0) root         (0)      133 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame_simput/core/ui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4685 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame_simput/core/ui/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 14:27:00.049639 trame-simput-2.4.2/trame_simput/core/ui/resolvers/
+-rw-r--r--   0 root         (0) root         (0)       75 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame_simput/core/ui/resolvers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4997 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame_simput/core/ui/resolvers/vuetify.py
+-rw-r--r--   0 root         (0) root         (0)     1810 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame_simput/core/ui/utils.py
+-rw-r--r--   0 root         (0) root         (0)      672 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame_simput/core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 14:27:00.053639 trame-simput-2.4.2/trame_simput/module/
+-rw-r--r--   0 root         (0) root         (0)      979 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame_simput/module/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8342 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame_simput/module/core.py
+-rw-r--r--   0 root         (0) root         (0)     3257 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame_simput/module/protocol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 14:27:00.057639 trame-simput-2.4.2/trame_simput/module/serve/
+-rw-r--r--   0 root         (0) root         (0)      208 2024-05-06 14:26:49.000000 trame-simput-2.4.2/trame_simput/module/serve/demo.html
+-rw-r--r--   0 root         (0) root         (0)   326277 2024-05-06 14:26:49.000000 trame-simput-2.4.2/trame_simput/module/serve/vue-trame_simput.common.js
+-rw-r--r--   0 root         (0) root         (0)   450349 2024-05-06 14:26:49.000000 trame-simput-2.4.2/trame_simput/module/serve/vue-trame_simput.common.js.map
+-rw-r--r--   0 root         (0) root         (0)   326677 2024-05-06 14:26:49.000000 trame-simput-2.4.2/trame_simput/module/serve/vue-trame_simput.umd.js
+-rw-r--r--   0 root         (0) root         (0)   450910 2024-05-06 14:26:49.000000 trame-simput-2.4.2/trame_simput/module/serve/vue-trame_simput.umd.js.map
+-rw-r--r--   0 root         (0) root         (0)   113788 2024-05-06 14:26:50.000000 trame-simput-2.4.2/trame_simput/module/serve/vue-trame_simput.umd.min.js
+-rw-r--r--   0 root         (0) root         (0)   482718 2024-05-06 14:26:50.000000 trame-simput-2.4.2/trame_simput/module/serve/vue-trame_simput.umd.min.js.map
+-rw-r--r--   0 root         (0) root         (0)    79047 2024-05-06 14:26:56.000000 trame-simput-2.4.2/trame_simput/module/serve/vue3-trame_simput.umd.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 14:27:00.057639 trame-simput-2.4.2/trame_simput/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame_simput/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4997 2024-05-06 14:26:23.000000 trame-simput-2.4.2/trame_simput/widgets/simput.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 14:27:00.049639 trame-simput-2.4.2/trame_simput.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4666 2024-05-06 14:27:00.000000 trame-simput-2.4.2/trame_simput.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1291 2024-05-06 14:27:00.000000 trame-simput-2.4.2/trame_simput.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 14:27:00.000000 trame-simput-2.4.2/trame_simput.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-06 14:27:00.000000 trame-simput-2.4.2/trame_simput.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-05-06 14:27:00.000000 trame-simput-2.4.2/trame_simput.egg-info/top_level.txt
```

### Comparing `trame-simput-2.4.1/LICENSE` & `trame-simput-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.1/PKG-INFO` & `trame-simput-2.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-simput
-Version: 2.4.1
+Version: 2.4.2
 Summary: Simput implementation for trame
 Author: Kitware Inc.
 License: Apache Software License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trame-simput-2.4.1/README.rst` & `trame-simput-2.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.1/setup.cfg` & `trame-simput-2.4.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-simput
-version = 2.4.1
+version = 2.4.2
 description = Simput implementation for trame
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = Apache Software License
 classifiers = 
 	Development Status :: 5 - Production/Stable
```

### Comparing `trame-simput-2.4.1/trame_simput/core/domains.py` & `trame-simput-2.4.2/trame_simput/core/domains.py`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.1/trame_simput/core/factory.py` & `trame-simput-2.4.2/trame_simput/core/factory.py`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.1/trame_simput/core/mapping.py` & `trame-simput-2.4.2/trame_simput/core/mapping.py`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.1/trame_simput/core/proxy.py` & `trame-simput-2.4.2/trame_simput/core/proxy.py`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.1/trame_simput/core/ui/manager.py` & `trame-simput-2.4.2/trame_simput/core/ui/manager.py`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.1/trame_simput/core/ui/resolvers/vuetify.py` & `trame-simput-2.4.2/trame_simput/core/ui/resolvers/vuetify.py`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.1/trame_simput/core/ui/utils.py` & `trame-simput-2.4.2/trame_simput/core/ui/utils.py`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.1/trame_simput/core/utils.py` & `trame-simput-2.4.2/trame_simput/core/utils.py`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.1/trame_simput/module/__init__.py` & `trame-simput-2.4.2/trame_simput/module/__init__.py`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.1/trame_simput/module/core.py` & `trame-simput-2.4.2/trame_simput/module/core.py`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.1/trame_simput/module/protocol.py` & `trame-simput-2.4.2/trame_simput/module/protocol.py`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.1/trame_simput/module/serve/vue-trame_simput.common.js` & `trame-simput-2.4.2/trame_simput/module/serve/vue-trame_simput.common.js`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.1/trame_simput/module/serve/vue-trame_simput.common.js.map` & `trame-simput-2.4.2/trame_simput/module/serve/vue-trame_simput.common.js.map`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.1/trame_simput/module/serve/vue-trame_simput.umd.js` & `trame-simput-2.4.2/trame_simput/module/serve/vue-trame_simput.umd.js`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.1/trame_simput/module/serve/vue-trame_simput.umd.js.map` & `trame-simput-2.4.2/trame_simput/module/serve/vue-trame_simput.umd.js.map`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.1/trame_simput/module/serve/vue-trame_simput.umd.min.js` & `trame-simput-2.4.2/trame_simput/module/serve/vue-trame_simput.umd.min.js`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.1/trame_simput/module/serve/vue-trame_simput.umd.min.js.map` & `trame-simput-2.4.2/trame_simput/module/serve/vue-trame_simput.umd.min.js.map`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.1/trame_simput/module/serve/vue3-trame_simput.umd.js` & `trame-simput-2.4.2/trame_simput/module/serve/vue3-trame_simput.umd.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1190,22 +1190,25 @@
         }, {
             default: vue.withCtx(() => [
                 (vue.openBlock(), vue.createBlock(_component_v_select, {
                     key: _ctx.tsKey,
                     label: _ctx.label,
                     hint: _ctx.computedHelp,
                     modelValue: _ctx.model,
-                    "onUpdate:modelValue": _cache[0] || (_cache[0] = ($event) => _ctx.model = $event),
+                    "onUpdate:modelValue": [
+                        _cache[0] || (_cache[0] = ($event) => _ctx.model = $event),
+                        _ctx.validate
+                    ],
+                    density: "compact",
                     items: _ctx.computedItems,
                     multiple: _ctx.multiple,
-                    onChange: _ctx.validate,
                     "persistent-hint": !!(_ctx.useRangeHelp || _ctx.help),
                     disabled: _ctx.disabled || !_ctx.decorator.enable,
                     readonly: _ctx.readonly
-                }, null, 8, ["label", "hint", "modelValue", "items", "multiple", "onChange", "persistent-hint", "disabled", "readonly"]))
+                }, null, 8, ["label", "hint", "modelValue", "items", "multiple", "onUpdate:modelValue", "persistent-hint", "disabled", "readonly"]))
             ]),
             _: 1
         }, 512)), [
             [vue.vShow, _ctx.shouldShow]
         ]);
     }
     const SwSelect = /* @__PURE__ */ _export_sfc(_sfc_main$9, [
@@ -1507,66 +1510,42 @@
         style: {
             "max-width": "60px",
             "min-width": "60px"
         }
     };
 
     function render$8(_ctx, _cache, $props, $setup, $data, $options) {
-        const _component_v_icon = vue.resolveComponent("v-icon");
         const _component_v_btn = vue.resolveComponent("v-btn");
         const _component_v_divider = vue.resolveComponent("v-divider");
         const _component_v_col = vue.resolveComponent("v-col");
         const _component_v_row = vue.resolveComponent("v-row");
         const _component_v_slider = vue.resolveComponent("v-slider");
         const _component_v_alert = vue.resolveComponent("v-alert");
+        const _component_v_icon = vue.resolveComponent("v-icon");
         const _component_v_container = vue.resolveComponent("v-container");
         return vue.withDirectives((vue.openBlock(), vue.createBlock(_component_v_container, {
             fluid: "",
             style: {
                 "position": "relative"
             }
         }, {
             default: vue.withCtx(() => [
                 vue.createElementVNode("div", _hoisted_1$2, [
                     _ctx.help && _ctx.size > 1 ? (vue.openBlock(), vue.createBlock(_component_v_btn, {
                         key: 0,
-                        icon: "",
-                        "x-small": "",
+                        icon: "mdi-lifebuoy",
+                        size: "x-small",
                         onClick: _cache[0] || (_cache[0] = ($event) => _ctx.showHelp = !_ctx.showHelp)
-                    }, {
-                        default: vue.withCtx(() => [
-                            vue.createVNode(_component_v_icon, {
-                                small: ""
-                            }, {
-                                default: vue.withCtx(() => [
-                                    vue.createTextVNode("mdi-lifebuoy")
-                                ]),
-                                _: 1
-                            })
-                        ]),
-                        _: 1
                     })) : vue.createCommentVNode("", true),
                     _ctx.computedSizeControl ? (vue.openBlock(), vue.createBlock(_component_v_btn, {
                         key: 1,
-                        icon: "",
-                        "x-small": "",
+                        icon: "mdi-plus-circle-outline",
+                        size: "x-small",
                         onClick: _ctx.addEntry
-                    }, {
-                        default: vue.withCtx(() => [
-                            vue.createVNode(_component_v_icon, {
-                                small: ""
-                            }, {
-                                default: vue.withCtx(() => [
-                                    vue.createTextVNode("mdi-plus-circle-outline")
-                                ]),
-                                _: 1
-                            })
-                        ]),
-                        _: 1
-                    }, 8, ["onClick"])) : vue.createCommentVNode("", true)
+                    }, null, 8, ["onClick"])) : vue.createCommentVNode("", true)
                 ]),
                 vue.createVNode(_component_v_row, null, {
                     default: vue.withCtx(() => [
                         _ctx.label && _ctx.size != 1 ? (vue.openBlock(), vue.createBlock(_component_v_col, {
                             key: 0,
                             class: "py-0"
                         }, {
@@ -1609,82 +1588,71 @@
                                             default: vue.withCtx(() => [
                                                 vue.createTextVNode(vue.toDisplayString(_ctx.model), 1)
                                             ]),
                                             _: 1
                                         }),
                                         _ctx.help ? (vue.openBlock(), vue.createBlock(_component_v_btn, {
                                             key: 0,
-                                            icon: "",
-                                            "x-small": "",
+                                            icon: "mdi-lifebuoy",
+                                            size: "x-small",
                                             onClick: _cache[1] || (_cache[1] = ($event) => _ctx.showHelp = !_ctx.showHelp)
-                                        }, {
-                                            default: vue.withCtx(() => [
-                                                vue.createVNode(_component_v_icon, {
-                                                    small: ""
-                                                }, {
-                                                    default: vue.withCtx(() => [
-                                                        vue.createTextVNode("mdi-lifebuoy")
-                                                    ]),
-                                                    _: 1
-                                                })
-                                            ]),
-                                            _: 1
                                         })) : vue.createCommentVNode("", true)
                                     ]),
                                     _: 1
                                 }),
                                 vue.createVNode(_component_v_slider, {
                                     name: `${_ctx.data().type}:${_ctx.name}:${_ctx.i}`,
                                     modelValue: _ctx.model,
                                     "onUpdate:modelValue": [
                                         _cache[2] || (_cache[2] = ($event) => _ctx.model = $event),
                                         _cache[3] || (_cache[3] = ($event) => _ctx.validate())
                                     ],
                                     "hide-details": "",
-                                    dense: "",
+                                    density: "compact",
                                     rules: [_ctx.rule],
                                     min: _ctx.computedMin,
                                     max: _ctx.computedMax,
                                     step: _ctx.computedStep,
                                     disabled: _ctx.disabled || !_ctx.decorator.enable,
                                     readonly: _ctx.readonly
                                 }, null, 8, ["name", "modelValue", "rules", "min", "max", "step", "disabled", "readonly"]),
                                 _ctx.help && _ctx.showHelp ? (vue.openBlock(), vue.createElementBlock("div", _hoisted_4, vue.toDisplayString(_ctx.help), 1)) : vue.createCommentVNode("", true),
                                 (vue.openBlock(true), vue.createElementBlock(vue.Fragment, null, vue.renderList(_ctx.hints, (hint, idx) => {
                                     return vue.openBlock(), vue.createBlock(_component_v_alert, {
                                         key: idx,
                                         class: "mb-1",
                                         type: _ctx.levelToType(hint.level),
-                                        dense: "",
+                                        density: "compact",
                                         text: hint.message
                                     }, null, 8, ["type", "text"]);
                                 }), 128))
                             ]),
                             _: 1
                         })) : vue.createCommentVNode("", true),
                         _ctx.size != 1 ? (vue.openBlock(true), vue.createElementBlock(vue.Fragment, {
                             key: 1
                         }, vue.renderList(_ctx.computedSize, (i) => {
                             return vue.openBlock(), vue.createBlock(_component_v_col, vue.mergeProps({
                                 class: "py-1",
-                                key: i
+                                key: i,
+                                ref_for: true
                             }, _ctx.getComponentProps(i - 1)), {
                                 default: vue.withCtx(() => [
                                     vue.createVNode(_component_v_row, {
                                         "no-gutters": "",
                                         class: "align-center"
                                     }, {
                                         default: vue.withCtx(() => [
                                             vue.createVNode(_component_v_slider, {
                                                 class: "mt-0",
                                                 name: `${_ctx.data().type}:${_ctx.name}:${i}`,
                                                 modelValue: _ctx.model[i - 1],
                                                 "onUpdate:modelValue": [($event) => _ctx.model[i - 1] = $event, ($event) => _ctx.validate(i)],
                                                 "hide-details": "",
-                                                dense: "",
+                                                density: "compact",
                                                 rules: [_ctx.rule],
                                                 min: _ctx.computedMin,
                                                 max: _ctx.computedMax,
                                                 step: _ctx.computedStep,
                                                 disabled: _ctx.disabled || !_ctx.decorator.enable,
                                                 readonly: _ctx.readonly
                                             }, null, 8, ["name", "modelValue", "onUpdate:modelValue", "rules", "min", "max", "step", "disabled", "readonly"]),
@@ -1711,15 +1679,15 @@
                                         _: 2
                                     }, 1024),
                                     (vue.openBlock(true), vue.createElementBlock(vue.Fragment, null, vue.renderList(_ctx.hints, (hint, idx) => {
                                         return vue.openBlock(), vue.createBlock(_component_v_alert, {
                                             key: idx,
                                             class: "mb-1",
                                             type: _ctx.levelToType(hint.level),
-                                            dense: "",
+                                            density: "compact",
                                             text: hint.message
                                         }, null, 8, ["type", "text"]);
                                     }), 128))
                                 ]),
                                 _: 2
                             }, 1040);
                         }), 128)) : vue.createCommentVNode("", true)
@@ -1834,15 +1802,14 @@
             };
         }
     };
 
     function render$7(_ctx, _cache, $props, $setup, $data, $options) {
         const _component_v_switch = vue.resolveComponent("v-switch");
         const _component_v_spacer = vue.resolveComponent("v-spacer");
-        const _component_v_icon = vue.resolveComponent("v-icon");
         const _component_v_btn = vue.resolveComponent("v-btn");
         const _component_v_row = vue.resolveComponent("v-row");
         const _component_v_col = vue.resolveComponent("v-col");
         return vue.withDirectives((vue.openBlock(), vue.createBlock(_component_v_col, null, {
             default: vue.withCtx(() => [
                 vue.createVNode(_component_v_row, {
                     class: "ma-0 align-center",
@@ -1852,43 +1819,33 @@
                 }, {
                     default: vue.withCtx(() => [
                         vue.createVNode(_component_v_switch, {
                             class: "py-0 mt-0",
                             label: _ctx.label,
                             hint: _ctx.help,
                             modelValue: _ctx.model,
-                            "onUpdate:modelValue": _cache[0] || (_cache[0] = ($event) => _ctx.model = $event),
-                            onChange: _ctx.validate,
-                            dense: "",
+                            "onUpdate:modelValue": [
+                                _cache[0] || (_cache[0] = ($event) => _ctx.model = $event),
+                                _ctx.validate
+                            ],
+                            density: "compact",
                             "hide-details": "",
                             disabled: _ctx.disabled || !_ctx.decorator.enable,
                             readonly: _ctx.readonly
-                        }, null, 8, ["label", "hint", "modelValue", "onChange", "disabled", "readonly"]),
+                        }, null, 8, ["label", "hint", "modelValue", "onUpdate:modelValue", "disabled", "readonly"]),
                         vue.createVNode(_component_v_spacer),
                         _ctx.help ? (vue.openBlock(), vue.createBlock(_component_v_btn, {
                             key: 0,
-                            icon: "",
-                            "x-small": "",
+                            icon: "mdi-lifebuoy",
+                            size: "x-small",
                             style: {
                                 "position": "absolute",
                                 "right": "0"
                             },
                             onClick: _cache[1] || (_cache[1] = ($event) => _ctx.showHelp = !_ctx.showHelp)
-                        }, {
-                            default: vue.withCtx(() => [
-                                vue.createVNode(_component_v_icon, {
-                                    small: ""
-                                }, {
-                                    default: vue.withCtx(() => [
-                                        vue.createTextVNode("mdi-lifebuoy")
-                                    ]),
-                                    _: 1
-                                })
-                            ]),
-                            _: 1
                         })) : vue.createCommentVNode("", true)
                     ]),
                     _: 1
                 }),
                 _ctx.help && _ctx.showHelp ? (vue.openBlock(), vue.createBlock(_component_v_row, {
                     key: 0,
                     class: "ma-0 text-caption text--secondary"
@@ -1952,18 +1909,14 @@
                 type: Boolean,
                 default: false
             },
             "no-resize": {
                 type: Boolean,
                 default: false
             },
-            "row-height": {
-                type: Boolean,
-                default: false
-            },
             rows: {
                 type: [String, Number],
                 default: 5
             }
         },
         setup(props) {
             ref$2(false);
@@ -1997,28 +1950,28 @@
             };
         }
     };
 
     function render$6(_ctx, _cache, $props, $setup, $data, $options) {
         const _component_v_textarea = vue.resolveComponent("v-textarea");
         return vue.withDirectives((vue.openBlock(), vue.createBlock(_component_v_textarea, {
+            density: "compact",
             label: _ctx.label,
             hint: _ctx.help,
             modelValue: _ctx.model,
             "onUpdate:modelValue": _cache[0] || (_cache[0] = ($event) => _ctx.model = $event),
             onChange: _ctx.validate,
             "auto-grow": _ctx.auto - _ctx.grow,
             autofocus: _ctx.autofocus,
             clearable: _ctx.clearable,
             readonly: _ctx.readonly,
             "no-resize": _ctx.no - _ctx.resize,
-            "row-height": _ctx.row - _ctx.height,
             rows: _ctx.rows,
             disabled: _ctx.disabled || !_ctx.decorator.enable
-        }, null, 8, ["label", "hint", "modelValue", "onChange", "auto-grow", "autofocus", "clearable", "readonly", "no-resize", "row-height", "rows", "disabled"])), [
+        }, null, 8, ["label", "hint", "modelValue", "onChange", "auto-grow", "autofocus", "clearable", "readonly", "no-resize", "rows", "disabled"])), [
             [vue.vShow, _ctx.decorator.show]
         ]);
     }
     const SwTextArea = /* @__PURE__ */ _export_sfc(_sfc_main$6, [
         ["render", render$6]
     ]);
     const {
@@ -2418,60 +2371,62 @@
                         _ctx.size == 1 ? (vue.openBlock(), vue.createBlock(_component_v_col, {
                             key: 0,
                             class: "pt-0 pb-1"
                         }, {
                             default: vue.withCtx(() => [
                                 vue.createVNode(_component_v_text_field, {
                                     name: `${_ctx.data().type}:${_ctx.name}:${_ctx.i}`,
-                                    "background-color": _ctx.color(),
+                                    "bg-color": _ctx.color(),
                                     modelValue: _ctx.model,
-                                    "onUpdate:modelValue": _cache[1] || (_cache[1] = ($event) => _ctx.model = $event),
-                                    onInput: _cache[2] || (_cache[2] = ($event) => _ctx.update()),
+                                    "onUpdate:modelValue": [
+                                        _cache[1] || (_cache[1] = ($event) => _ctx.model = $event),
+                                        _cache[2] || (_cache[2] = ($event) => _ctx.update())
+                                    ],
                                     label: _ctx.label,
                                     hint: _ctx.help,
-                                    dens: "",
+                                    density: "compact",
                                     rules: [_ctx.rule],
                                     onBlur: _cache[3] || (_cache[3] = ($event) => _ctx.validate()),
                                     onKeydown: _cache[4] || (_cache[4] = vue.withKeys(($event) => _ctx.validate(), ["enter"])),
                                     "persistent-hint": _ctx.showHelp,
                                     "hide-details": !_ctx.showHelp || !_ctx.help,
                                     disabled: _ctx.disabled || !_ctx.decorator.enable,
                                     readonly: _ctx.readonly
-                                }, null, 8, ["name", "background-color", "modelValue", "label", "hint", "rules", "persistent-hint", "hide-details", "disabled", "readonly"])
+                                }, null, 8, ["name", "bg-color", "modelValue", "label", "hint", "rules", "persistent-hint", "hide-details", "disabled", "readonly"])
                             ]),
                             _: 1
                         })) : vue.createCommentVNode("", true),
                         _ctx.size != 1 ? (vue.openBlock(true), vue.createElementBlock(vue.Fragment, {
                             key: 1
                         }, vue.renderList(_ctx.computedSize, (i) => {
                             return vue.openBlock(), vue.createBlock(_component_v_col, vue.mergeProps({
                                 class: "py-1",
-                                key: i
+                                key: i,
+                                ref_for: true
                             }, _ctx.getComponentProps(i - 1)), {
                                 default: vue.withCtx(() => [
                                     vue.createVNode(_component_v_row, {
                                         "no-gutters": "",
                                         class: "align-center"
                                     }, {
                                         default: vue.withCtx(() => [
                                             vue.createVNode(_component_v_text_field, {
                                                 class: "mt-0",
                                                 name: `${_ctx.data().type}:${_ctx.name}:${i}`,
-                                                "background-color": _ctx.color(i),
+                                                "bg-color": _ctx.color(i),
                                                 modelValue: _ctx.model[i - 1],
-                                                "onUpdate:modelValue": ($event) => _ctx.model[i - 1] = $event,
-                                                onInput: ($event) => _ctx.update(i),
-                                                dense: "",
+                                                "onUpdate:modelValue": [($event) => _ctx.model[i - 1] = $event, ($event) => _ctx.update(i)],
+                                                density: "compact",
                                                 rules: [_ctx.rule],
-                                                onBlur: ($event) => _ctx.validate(i),
+                                                "onUpdate:focused": ($event) => _ctx.validate(i),
                                                 onKeydown: vue.withKeys(($event) => _ctx.validate(i), ["enter"]),
                                                 "hide-details": "",
                                                 disabled: _ctx.disabled || !_ctx.decorator.enable,
                                                 readonly: _ctx.readonly
-                                            }, null, 8, ["name", "background-color", "modelValue", "onUpdate:modelValue", "onInput", "rules", "onBlur", "onKeydown", "disabled", "readonly"]),
+                                            }, null, 8, ["name", "bg-color", "modelValue", "onUpdate:modelValue", "rules", "onUpdate:focused", "onKeydown", "disabled", "readonly"]),
                                             _ctx.computedSizeControl ? (vue.openBlock(), vue.createBlock(_component_v_btn, {
                                                 key: 0,
                                                 class: "ml-2",
                                                 icon: "",
                                                 "x-small": "",
                                                 onClick: ($event) => _ctx.deleteEntry(i - 1),
                                                 disabled: _ctx.disabled || !_ctx.decorator.enable,
@@ -2503,23 +2458,22 @@
                 }, {
                     default: vue.withCtx(() => [
                         (vue.openBlock(true), vue.createElementBlock(vue.Fragment, null, vue.renderList(_ctx.hints, (hint, idx) => {
                             return vue.openBlock(), vue.createBlock(_component_v_alert, {
                                 key: idx,
                                 class: "mb-1",
                                 type: _ctx.levelToType(hint.level),
-                                border: "left",
-                                dense: "",
-                                icon: _ctx.levelToIcon(hint.level)
+                                border: "start",
+                                density: "compact"
                             }, {
                                 default: vue.withCtx(() => [
                                     vue.createTextVNode(vue.toDisplayString(hint.message), 1)
                                 ]),
                                 _: 2
-                            }, 1032, ["type", "icon"]);
+                            }, 1032, ["type"]);
                         }), 128))
                     ]),
                     _: 1
                 })) : vue.createCommentVNode("", true)
             ]),
             _: 1
         }, 512)), [
```

### Comparing `trame-simput-2.4.1/trame_simput/widgets/simput.py` & `trame-simput-2.4.2/trame_simput/widgets/simput.py`

 * *Files identical despite different names*

### Comparing `trame-simput-2.4.1/trame_simput.egg-info/PKG-INFO` & `trame-simput-2.4.2/trame_simput.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-simput
-Version: 2.4.1
+Version: 2.4.2
 Summary: Simput implementation for trame
 Author: Kitware Inc.
 License: Apache Software License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trame-simput-2.4.1/trame_simput.egg-info/SOURCES.txt` & `trame-simput-2.4.2/trame_simput.egg-info/SOURCES.txt`

 * *Files identical despite different names*

