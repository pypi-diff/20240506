# Comparing `tmp/netbox_napalm_plugin-0.1.9.tar.gz` & `tmp/netbox_napalm_plugin-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_napalm_plugin-0.1.9.tar", last modified: Mon Apr 29 22:57:49 2024, max compression
+gzip compressed data, was "netbox_napalm_plugin-0.2.0.tar", last modified: Mon May  6 19:35:26 2024, max compression
```

## Comparing `netbox_napalm_plugin-0.1.9.tar` & `netbox_napalm_plugin-0.2.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:57:49.473242 netbox_napalm_plugin-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    10175 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-04-29 22:57:49.473242 netbox_napalm_plugin-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:57:49.469242 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:57:49.469242 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/filtersets.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:57:49.469242 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/migrations/0002_auto_20230215_1752.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/navigation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:57:49.465242 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:57:49.465242 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/static/netbox_napalm_plugin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:57:49.473242 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/static/netbox_napalm_plugin/js/
--rw-r--r--   0 runner    (1001) docker     (127)   196388 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/static/netbox_napalm_plugin/js/config.js
--rw-r--r--   0 runner    (1001) docker     (127)   198227 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/static/netbox_napalm_plugin/js/lldp.js
--rw-r--r--   0 runner    (1001) docker     (127)   234145 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/static/netbox_napalm_plugin/js/status.js
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:57:49.465242 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:57:49.473242 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/templates/netbox_napalm_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/templates/netbox_napalm_plugin/config.html
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/templates/netbox_napalm_plugin/lldp_neighbors.html
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/templates/netbox_napalm_plugin/napalmplatformconfig.html
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/templates/netbox_napalm_plugin/status.html
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:57:49.473242 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-04-29 22:57:49.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-29 22:57:49.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 22:57:49.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-29 22:57:49.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-29 22:57:49.000000 netbox_napalm_plugin-0.1.9/netbox_napalm_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 22:57:49.473242 netbox_napalm_plugin-0.1.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:57:49.473242 netbox_napalm_plugin-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-29 22:57:45.000000 netbox_napalm_plugin-0.1.9/tests/test_netbox_napalm_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:35:26.557453 netbox_napalm_plugin-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10175 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-06 19:35:26.557453 netbox_napalm_plugin-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:35:26.553453 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:35:26.553453 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/filtersets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:35:26.553453 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/migrations/0002_auto_20230215_1752.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/navigation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:35:26.549453 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:35:26.549453 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/static/netbox_napalm_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:35:26.553453 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/static/netbox_napalm_plugin/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   196388 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/static/netbox_napalm_plugin/js/config.js
+-rw-r--r--   0 runner    (1001) docker     (127)   198227 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/static/netbox_napalm_plugin/js/lldp.js
+-rw-r--r--   0 runner    (1001) docker     (127)   234145 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/static/netbox_napalm_plugin/js/status.js
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:35:26.549453 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:35:26.557453 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/templates/netbox_napalm_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/templates/netbox_napalm_plugin/config.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/templates/netbox_napalm_plugin/lldp_neighbors.html
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/templates/netbox_napalm_plugin/napalmplatformconfig.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/templates/netbox_napalm_plugin/status.html
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:35:26.557453 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-06 19:35:26.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-06 19:35:26.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 19:35:26.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-06 19:35:26.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-06 19:35:26.000000 netbox_napalm_plugin-0.2.0/netbox_napalm_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 19:35:26.557453 netbox_napalm_plugin-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:35:26.557453 netbox_napalm_plugin-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-06 19:35:22.000000 netbox_napalm_plugin-0.2.0/tests/test_netbox_napalm_plugin.py
```

### Comparing `netbox_napalm_plugin-0.1.9/CONTRIBUTING.md` & `netbox_napalm_plugin-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.9/LICENSE` & `netbox_napalm_plugin-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.9/PKG-INFO` & `netbox_napalm_plugin-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: netbox-napalm-plugin
-Version: 0.1.9
+Version: 0.2.0
 Summary: NetBox plugin for Napalm.
 Author-email: Arthur Hanson <ahanson@netboxlabs.com>
 Project-URL: Documentation, https://github.com/netbox-community/netbox-napalm-plugin/blob/main/README.md
 Project-URL: Source, https://github.com/netbox-community/netbox-napalm-plugin
 Project-URL: Tracker, https://github.com/netbox-community/netbox-napalm-plugin/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8.1
+Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: napalm<5.0
 Provides-Extra: test
 Requires-Dist: black==24.3.0; extra == "test"
 Requires-Dist: check-manifest==0.49; extra == "test"
 Requires-Dist: flake8; extra == "test"
```

### Comparing `netbox_napalm_plugin-0.1.9/README.md` & `netbox_napalm_plugin-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/api/serializers.py` & `netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/api/views.py` & `netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/api/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dcim.models import Device
 from django.shortcuts import get_object_or_404, redirect, render
-from extras.plugins.utils import get_plugin_config
+from netbox.plugins.utils import get_plugin_config
 from netbox.api.exceptions import ServiceUnavailable
 from netbox.api.pagination import StripCountAnnotationsPaginator
 from netbox.api.viewsets import NetBoxModelViewSet
 
 from rest_framework.decorators import action
 from rest_framework.response import Response
```

### Comparing `netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/filtersets.py` & `netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/migrations/0001_initial.py` & `netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/migrations/0002_auto_20230215_1752.py` & `netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/migrations/0002_auto_20230215_1752.py`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/models.py` & `netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/models.py`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/static/netbox_napalm_plugin/js/config.js` & `netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/static/netbox_napalm_plugin/js/config.js`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/static/netbox_napalm_plugin/js/lldp.js` & `netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/static/netbox_napalm_plugin/js/lldp.js`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/static/netbox_napalm_plugin/js/status.js` & `netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/static/netbox_napalm_plugin/js/status.js`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/tables.py` & `netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/tables.py`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/templates/netbox_napalm_plugin/config.html` & `netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/templates/netbox_napalm_plugin/config.html`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/templates/netbox_napalm_plugin/lldp_neighbors.html` & `netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/templates/netbox_napalm_plugin/lldp_neighbors.html`

 * *Files 10% similar despite different names*

```diff
@@ -13,54 +13,52 @@
             <div class="spinner-border" role="status">
                 <span class="visually-hidden">Loading...</span>
             </div>
         </div>
         <div class="card-header">
             <h5 class="d-inline">LLDP Neighbors</h5>
         </div>
-        <div class="card-body">
-            <table class="table table-hover">
-                <thead>
-                    <tr>
-                        <th>Interface</th>
-                        <th>Configured Device</th>
-                        <th>Configured Interface</th>
-                        <th>LLDP Device</th>
-                        <th>LLDP Interface</th>
-                    </tr>
-                </thead>
-                <tbody>
-                    {% for iface in interfaces %}
-                        <tr id="{{ iface.name }}">
-                            <td>{{ iface }}</td>
-                            {% with peer=iface.connected_endpoints.0 %}
-                              {% if peer.device %}
-                                  <td class="configured_device" data="{{ peer.device.name }}" data-chassis="{{ peer.device.virtual_chassis.name }}">
-                                      <a href="{% url 'dcim:device' pk=peer.device.pk %}">{{ peer.device }}</a>
-                                  </td>
-                                  <td class="configured_interface" data="{{ peer.name }}">
-                                      <span title="{{ peer.get_type_display }}">{{ peer }}</span>
+        <table class="table table-hover">
+            <thead>
+                <tr>
+                    <th>Interface</th>
+                    <th>Configured Device</th>
+                    <th>Configured Interface</th>
+                    <th>LLDP Device</th>
+                    <th>LLDP Interface</th>
+                </tr>
+            </thead>
+            <tbody>
+                {% for iface in interfaces %}
+                    <tr id="{{ iface.name }}">
+                        <td>{{ iface }}</td>
+                        {% with peer=iface.connected_endpoints.0 %}
+                          {% if peer.device %}
+                              <td class="configured_device" data="{{ peer.device.name }}" data-chassis="{{ peer.device.virtual_chassis.name }}">
+                                  <a href="{% url 'dcim:device' pk=peer.device.pk %}">{{ peer.device }}</a>
+                              </td>
+                              <td class="configured_interface" data="{{ peer.name }}">
+                                  <span title="{{ peer.get_type_display }}">{{ peer }}</span>
+                              </td>
+                          {% elif peer.circuit %}
+                              {% with circuit=peer.circuit %}
+                                  <td colspan="2">
+                                      <i class="mdi mdi-lightning-bolt" title="Circuit"></i>
+                                      <a href="{{ circuit.get_absolute_url }}">{{ circuit.provider }} {{ circuit }}</a>
                                   </td>
-                              {% elif peer.circuit %}
-                                  {% with circuit=peer.circuit %}
-                                      <td colspan="2">
-                                          <i class="mdi mdi-lightning-bolt" title="Circuit"></i>
-                                          <a href="{{ circuit.get_absolute_url }}">{{ circuit.provider }} {{ circuit }}</a>
-                                      </td>
-                                  {% endwith %}
-                              {% else %}
-                                  <td class="text-muted" colspan="2">None</td>
-                              {% endif %}
-                            {% endwith %}
-                            <td class="device"></td>
-                            <td class="interface"></td>
-                        </tr>
-                    {% endfor %}
-                </tbody>
-            </table>
-        </div>
+                              {% endwith %}
+                          {% else %}
+                              <td class="text-muted" colspan="2">None</td>
+                          {% endif %}
+                        {% endwith %}
+                        <td class="device"></td>
+                        <td class="interface"></td>
+                    </tr>
+                {% endfor %}
+            </tbody>
+        </table>
     </div>
 {% endblock %}
 
 {% block data %}
 <span data-object-url="{% url 'plugins-api:netbox_napalm_plugin-api:napalmplatformconfig-napalm' pk=object.pk %}?method=get_lldp_neighbors_detail"></span>
 {% endblock %}
```

### Comparing `netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/templates/netbox_napalm_plugin/napalmplatformconfig.html` & `netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/templates/netbox_napalm_plugin/napalmplatformconfig.html`

 * *Files 6% similar despite different names*

```diff
@@ -5,26 +5,24 @@
 {% block content %}
   <div class="row mb-3">
     <div class="col col-md-6">
       <div class="card">
 
         <h5 class="card-header">NetBox Napalm Plugin</h5>
 
-        <div class="card-body">
-          <table class="table table-hover attr-table">
-            <tr>
-                <th scope="row">Platform</th>
-                <td>{{ object.platform|linkify|placeholder }}</td>
-            </tr>
-            <tr>
-              <th scope="row">NAPALM Driver</th>
-              <td>{{ object.napalm_driver|placeholder }}</td>
-            </tr>
-          </table>
-        </div>
+        <table class="table table-hover attr-table">
+          <tr>
+              <th scope="row">Platform</th>
+              <td>{{ object.platform|linkify|placeholder }}</td>
+          </tr>
+          <tr>
+            <th scope="row">NAPALM Driver</th>
+            <td>{{ object.napalm_driver|placeholder }}</td>
+          </tr>
+        </table>
       </div>
       {% include 'inc/panels/tags.html' %}
       {% include 'inc/panels/custom_fields.html' %}
     </div>
 
     <div class="col col-md-6">
       <div class="card">
```

### Comparing `netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/templates/netbox_napalm_plugin/status.html` & `netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/templates/netbox_napalm_plugin/status.html`

 * *Files 5% similar despite different names*

```diff
@@ -13,80 +13,76 @@
             <div class="card">
                 <div class="card-overlay">
                     <div class="spinner-border" role="status">
                         <span class="visually-hidden">Loading...</span>
                     </div>
                 </div>
                 <h5 class="card-header">Device Facts</h5>
-                <div class="card-body">
-                    <table class="table">
-                        <tr>
-                            <th scope="row">Hostname</th>
-                            <td id="hostname"></td>
-                        </tr>
-                        <tr>
-                            <th scope="row">FQDN</th>
-                            <td id="fqdn"></td>
-                        </tr>
-                        <tr>
-                            <th scope="row">Vendor</th>
-                            <td id="vendor"></td>
-                        </tr>
-                        <tr>
-                            <th scope="row">Model</th>
-                            <td id="model"></td>
-                        </tr>
-                        <tr>
-                            <th scope="row">Serial Number</th>
-                            <td id="serial_number" class="text-monospace"></td>
-                        </tr>
-                        <tr>
-                            <th scope="row">OS Version</th>
-                            <td id="os_version"></td>
-                        </tr>
-                        <tr class="align-middle">
-                            <th scope="row">Uptime</th>
-                            <td>
-                                <div id="uptime-duration"></div>
-                                <div id="uptime" class="small text-muted"></div>
-                            </td>
-                        </tr>
-                    </table>
-                </div>
+                <table class="table">
+                    <tr>
+                        <th scope="row">Hostname</th>
+                        <td id="hostname"></td>
+                    </tr>
+                    <tr>
+                        <th scope="row">FQDN</th>
+                        <td id="fqdn"></td>
+                    </tr>
+                    <tr>
+                        <th scope="row">Vendor</th>
+                        <td id="vendor"></td>
+                    </tr>
+                    <tr>
+                        <th scope="row">Model</th>
+                        <td id="model"></td>
+                    </tr>
+                    <tr>
+                        <th scope="row">Serial Number</th>
+                        <td id="serial_number" class="text-monospace"></td>
+                    </tr>
+                    <tr>
+                        <th scope="row">OS Version</th>
+                        <td id="os_version"></td>
+                    </tr>
+                    <tr class="align-middle">
+                        <th scope="row">Uptime</th>
+                        <td>
+                            <div id="uptime-duration"></div>
+                            <div id="uptime" class="small text-muted"></div>
+                        </td>
+                    </tr>
+                </table>
             </div>
         </div>
         <div class="col col-md-6">
             <div class="card">
                 <div class="card-overlay">
                     <div class="spinner-border" role="status">
                         <span class="visually-hidden">Loading...</span>
                     </div>
                 </div>
                 <h5 class="card-header">Environment</h5>
-                <div class="card-body">
-                    <table class="table">
-                        <tr id="status-cpu">
-                            <th colspan="2"><i class="mdi mdi-gauge"></i> CPU</th>
-                        </tr>
-                        <tr id="status-memory">
-                            <th colspan="2"><i class="mdi mdi-chip"></i> Memory</th>
-                        </tr>
-                        <tr id="status-temperature">
-                            <th colspan="2"><i class="mdi mdi-thermometer"></i> Temperature</th>
-                        </tr>
-                        <tr id="status-fans">
-                            <th colspan="2"><i class="mdi mdi-fan"></i> Fans</th>
-                        </tr>
-                        <tr id="status-power">
-                            <th colspan="2"><i class="mdi mdi-power"></i> Power</th>
-                        </tr>
-                        <tr class="napalm-table-placeholder d-none invisible">
-                        </tr>
-                    </table>
-                </div>
+                <table class="table">
+                    <tr id="status-cpu">
+                        <th colspan="2"><i class="mdi mdi-gauge"></i> CPU</th>
+                    </tr>
+                    <tr id="status-memory">
+                        <th colspan="2"><i class="mdi mdi-chip"></i> Memory</th>
+                    </tr>
+                    <tr id="status-temperature">
+                        <th colspan="2"><i class="mdi mdi-thermometer"></i> Temperature</th>
+                    </tr>
+                    <tr id="status-fans">
+                        <th colspan="2"><i class="mdi mdi-fan"></i> Fans</th>
+                    </tr>
+                    <tr id="status-power">
+                        <th colspan="2"><i class="mdi mdi-power"></i> Power</th>
+                    </tr>
+                    <tr class="napalm-table-placeholder d-none invisible">
+                    </tr>
+                </table>
             </div>
         </div>
     </div>
 {% endblock %}
 
 {% block data %}
     <span data-object-url="{% url 'plugins-api:netbox_napalm_plugin-api:napalmplatformconfig-napalm' pk=object.pk %}?method=get_facts&method=get_environment"></span>
```

### Comparing `netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/urls.py` & `netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.9/netbox_napalm_plugin/views.py` & `netbox_napalm_plugin-0.2.0/netbox_napalm_plugin/views.py`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.9/netbox_napalm_plugin.egg-info/PKG-INFO` & `netbox_napalm_plugin-0.2.0/netbox_napalm_plugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: netbox-napalm-plugin
-Version: 0.1.9
+Version: 0.2.0
 Summary: NetBox plugin for Napalm.
 Author-email: Arthur Hanson <ahanson@netboxlabs.com>
 Project-URL: Documentation, https://github.com/netbox-community/netbox-napalm-plugin/blob/main/README.md
 Project-URL: Source, https://github.com/netbox-community/netbox-napalm-plugin
 Project-URL: Tracker, https://github.com/netbox-community/netbox-napalm-plugin/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8.1
+Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: napalm<5.0
 Provides-Extra: test
 Requires-Dist: black==24.3.0; extra == "test"
 Requires-Dist: check-manifest==0.49; extra == "test"
 Requires-Dist: flake8; extra == "test"
```

### Comparing `netbox_napalm_plugin-0.1.9/netbox_napalm_plugin.egg-info/SOURCES.txt` & `netbox_napalm_plugin-0.2.0/netbox_napalm_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.9/pyproject.toml` & `netbox_napalm_plugin-0.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -3,33 +3,32 @@
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name =  "netbox-napalm-plugin"
-version = "0.1.9"
+version = "0.2.0"
 authors = [
     {name = "Arthur Hanson", email = "ahanson@netboxlabs.com"},
 ]
 description = "NetBox plugin for Napalm."
 readme = "README.md"
 
 classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'Natural Language :: English',
     "Programming Language :: Python :: 3 :: Only",
-    'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Programming Language :: Python :: 3.12',
 ]
 
-requires-python = ">=3.8.1"
+requires-python = ">=3.10.0"
 dependencies = [
     'napalm<5.0'
 ]
 
 [project.optional-dependencies]
 test = [
     "black==24.3.0",
@@ -43,11 +42,11 @@
 [project.urls]
 Documentation = "https://github.com/netbox-community/netbox-napalm-plugin/blob/main/README.md"
 Source = "https://github.com/netbox-community/netbox-napalm-plugin"
 Tracker = "https://github.com/netbox-community/netbox-napalm-plugin/issues"
 
 [tool.black]
 line-length = 120
-target_version = ['py39', 'py310', 'py311', 'py312']
+target_version = ['py310', 'py311', 'py312']
 
 [tool.setuptools.package-data]
 netbox_napalm_plugin = ["templates/**"]
```

