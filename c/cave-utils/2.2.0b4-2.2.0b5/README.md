# Comparing `tmp/cave_utils-2.2.0b4.tar.gz` & `tmp/cave_utils-2.2.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cave_utils-2.2.0b4.tar", last modified: Wed May  1 20:32:33 2024, max compression
+gzip compressed data, was "cave_utils-2.2.0b5.tar", last modified: Thu May  2 19:58:48 2024, max compression
```

## Comparing `cave_utils-2.2.0b4.tar` & `cave_utils-2.2.0b5.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-01 20:32:33.781966 cave_utils-2.2.0b4/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    11357 2023-06-13 15:21:54.000000 cave_utils-2.2.0b4/LICENSE
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      631 2023-06-13 15:22:15.000000 cave_utils-2.2.0b4/NOTICE.md
--rw-r--r--   0 conmak    (1000) conmak    (1000)     3504 2024-05-01 20:32:33.781966 cave_utils-2.2.0b4/PKG-INFO
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)     2946 2024-03-06 18:01:37.000000 cave_utils-2.2.0b4/README.md
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-01 20:32:33.777966 cave_utils-2.2.0b4/cave_utils/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      414 2024-03-04 18:45:40.000000 cave_utils-2.2.0b4/cave_utils/__init__.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-01 20:32:33.781966 cave_utils-2.2.0b4/cave_utils/api/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     8444 2024-05-01 18:13:43.000000 cave_utils-2.2.0b4/cave_utils/api/__init__.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     4976 2024-05-01 14:13:40.000000 cave_utils-2.2.0b4/cave_utils/api/appBar.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     1063 2023-11-30 18:55:27.000000 cave_utils-2.2.0b4/cave_utils/api/extraKwargs.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     2210 2024-05-01 20:11:17.000000 cave_utils-2.2.0b4/cave_utils/api/globalOutputs.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    16980 2024-04-18 16:17:39.000000 cave_utils-2.2.0b4/cave_utils/api/groupedOutputs.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    11802 2024-05-01 20:06:29.000000 cave_utils-2.2.0b4/cave_utils/api/mapFeatures.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    30324 2024-02-26 14:04:23.000000 cave_utils-2.2.0b4/cave_utils/api/maps.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    12779 2024-04-18 18:22:52.000000 cave_utils-2.2.0b4/cave_utils/api/pages.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     7085 2024-01-31 16:20:08.000000 cave_utils-2.2.0b4/cave_utils/api/panes.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    14930 2024-05-01 16:20:53.000000 cave_utils-2.2.0b4/cave_utils/api/settings.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-01 20:32:33.781966 cave_utils-2.2.0b4/cave_utils/api_utils/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      311 2024-03-04 20:53:07.000000 cave_utils-2.2.0b4/cave_utils/api_utils/__init__.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    35234 2024-05-01 14:01:50.000000 cave_utils-2.2.0b4/cave_utils/api_utils/general.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      990 2024-05-01 16:03:09.000000 cave_utils-2.2.0b4/cave_utils/api_utils/validator.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    16302 2024-05-01 20:22:37.000000 cave_utils-2.2.0b4/cave_utils/api_utils/validator_utils.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     1798 2023-10-16 13:43:50.000000 cave_utils-2.2.0b4/cave_utils/arguments.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-01 20:32:33.781966 cave_utils-2.2.0b4/cave_utils/builders/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      273 2024-03-06 18:02:20.000000 cave_utils-2.2.0b4/cave_utils/builders/__init__.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    15444 2024-03-14 15:24:47.000000 cave_utils-2.2.0b4/cave_utils/builders/groups.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     1529 2023-11-30 18:55:27.000000 cave_utils-2.2.0b4/cave_utils/log.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      364 2024-05-01 20:14:50.000000 cave_utils-2.2.0b4/cave_utils/socket.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-01 20:32:33.781966 cave_utils-2.2.0b4/cave_utils.egg-info/
--rw-r--r--   0 conmak    (1000) conmak    (1000)     3504 2024-05-01 20:32:33.000000 cave_utils-2.2.0b4/cave_utils.egg-info/PKG-INFO
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      895 2024-05-01 20:32:33.000000 cave_utils-2.2.0b4/cave_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2024-05-01 20:32:33.000000 cave_utils-2.2.0b4/cave_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       34 2024-05-01 20:32:33.000000 cave_utils-2.2.0b4/cave_utils.egg-info/requires.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       11 2024-05-01 20:32:33.000000 cave_utils-2.2.0b4/cave_utils.egg-info/top_level.txt
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)      743 2024-05-01 20:29:46.000000 cave_utils-2.2.0b4/pyproject.toml
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      143 2024-05-01 20:32:33.781966 cave_utils-2.2.0b4/setup.cfg
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-01 20:32:33.781966 cave_utils-2.2.0b4/test/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      306 2023-11-30 18:55:27.000000 cave_utils-2.2.0b4/test/test_arguments.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     5107 2024-03-06 18:02:20.000000 cave_utils-2.2.0b4/test/test_builders_groups.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       40 2024-03-06 17:54:00.000000 cave_utils-2.2.0b4/test/test_import.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      233 2023-11-30 18:55:27.000000 cave_utils-2.2.0b4/test/test_log.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    75749 2024-01-31 16:20:08.000000 cave_utils-2.2.0b4/test/test_validator.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-02 19:58:48.640477 cave_utils-2.2.0b5/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    11357 2023-06-13 15:21:54.000000 cave_utils-2.2.0b5/LICENSE
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      631 2023-06-13 15:22:15.000000 cave_utils-2.2.0b5/NOTICE.md
+-rw-r--r--   0 conmak    (1000) conmak    (1000)     3504 2024-05-02 19:58:48.640477 cave_utils-2.2.0b5/PKG-INFO
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)     2946 2024-03-06 18:01:37.000000 cave_utils-2.2.0b5/README.md
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-02 19:58:48.636477 cave_utils-2.2.0b5/cave_utils/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      447 2024-05-02 19:54:41.000000 cave_utils-2.2.0b5/cave_utils/__init__.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-02 19:58:48.640477 cave_utils-2.2.0b5/cave_utils/api/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     8447 2024-05-02 19:54:41.000000 cave_utils-2.2.0b5/cave_utils/api/__init__.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     4977 2024-05-02 19:54:41.000000 cave_utils-2.2.0b5/cave_utils/api/appBar.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1064 2024-05-02 19:54:41.000000 cave_utils-2.2.0b5/cave_utils/api/extraKwargs.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     2211 2024-05-02 19:54:41.000000 cave_utils-2.2.0b5/cave_utils/api/globalOutputs.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    17148 2024-05-02 19:54:41.000000 cave_utils-2.2.0b5/cave_utils/api/groupedOutputs.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    12103 2024-05-02 19:54:41.000000 cave_utils-2.2.0b5/cave_utils/api/mapFeatures.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    30325 2024-05-02 19:54:41.000000 cave_utils-2.2.0b5/cave_utils/api/maps.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    12768 2024-05-02 19:54:41.000000 cave_utils-2.2.0b5/cave_utils/api/pages.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     7086 2024-05-02 19:54:41.000000 cave_utils-2.2.0b5/cave_utils/api/panes.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    14927 2024-05-02 19:54:41.000000 cave_utils-2.2.0b5/cave_utils/api/settings.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-02 19:58:48.640477 cave_utils-2.2.0b5/cave_utils/api_utils/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      311 2024-03-04 20:53:07.000000 cave_utils-2.2.0b5/cave_utils/api_utils/__init__.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    35210 2024-05-02 19:54:41.000000 cave_utils-2.2.0b5/cave_utils/api_utils/general.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      991 2024-05-02 19:54:41.000000 cave_utils-2.2.0b5/cave_utils/api_utils/validator.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    16322 2024-05-02 19:54:41.000000 cave_utils-2.2.0b5/cave_utils/api_utils/validator_utils.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1798 2023-10-16 13:43:50.000000 cave_utils-2.2.0b5/cave_utils/arguments.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-02 19:58:48.640477 cave_utils-2.2.0b5/cave_utils/builders/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      273 2024-03-06 18:02:20.000000 cave_utils-2.2.0b5/cave_utils/builders/__init__.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    15444 2024-03-14 15:24:47.000000 cave_utils-2.2.0b5/cave_utils/builders/groups.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     4924 2024-05-02 19:54:41.000000 cave_utils-2.2.0b5/cave_utils/geo_utils.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1529 2023-11-30 18:55:27.000000 cave_utils-2.2.0b5/cave_utils/log.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      351 2024-05-02 19:54:40.000000 cave_utils-2.2.0b5/cave_utils/socket.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-02 19:58:48.640477 cave_utils-2.2.0b5/cave_utils.egg-info/
+-rw-r--r--   0 conmak    (1000) conmak    (1000)     3504 2024-05-02 19:58:48.000000 cave_utils-2.2.0b5/cave_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      942 2024-05-02 19:58:48.000000 cave_utils-2.2.0b5/cave_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2024-05-02 19:58:48.000000 cave_utils-2.2.0b5/cave_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       34 2024-05-02 19:58:48.000000 cave_utils-2.2.0b5/cave_utils.egg-info/requires.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       11 2024-05-02 19:58:48.000000 cave_utils-2.2.0b5/cave_utils.egg-info/top_level.txt
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)      743 2024-05-02 19:53:36.000000 cave_utils-2.2.0b5/pyproject.toml
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      143 2024-05-02 19:58:48.640477 cave_utils-2.2.0b5/setup.cfg
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-02 19:58:48.640477 cave_utils-2.2.0b5/test/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      306 2023-11-30 18:55:27.000000 cave_utils-2.2.0b5/test/test_arguments.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     5107 2024-03-06 18:02:20.000000 cave_utils-2.2.0b5/test/test_builders_groups.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      570 2024-05-02 19:54:41.000000 cave_utils-2.2.0b5/test/test_geo_utils.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       40 2024-03-06 17:54:00.000000 cave_utils-2.2.0b5/test/test_import.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      233 2023-11-30 18:55:27.000000 cave_utils-2.2.0b5/test/test_log.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    75749 2024-01-31 16:20:08.000000 cave_utils-2.2.0b5/test/test_validator.py
```

### Comparing `cave_utils-2.2.0b4/LICENSE` & `cave_utils-2.2.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b4/NOTICE.md` & `cave_utils-2.2.0b5/NOTICE.md`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b4/PKG-INFO` & `cave_utils-2.2.0b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cave_utils
-Version: 2.2.0b4
+Version: 2.2.0b5
 Summary: Python wrapper for api use in the cave_app
 Author-email: Connor Makowski <conmak@mit.edu>
 Project-URL: Homepage, https://github.com/mit-cave/cave_utils
 Project-URL: Bug Tracker, https://github.com/mit-cave/cave_utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `cave_utils-2.2.0b4/README.md` & `cave_utils-2.2.0b5/README.md`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b4/cave_utils/api/__init__.py` & `cave_utils-2.2.0b5/cave_utils/api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 Classes represent the actual API items and should have relevant API documentation for each item at the class level. In this current module, the `root` class represents the root of the API. The method `spec` details exactly what must be passed to root as well as other relevant documentation.
 
 Submodules (and their classes) are used to define the api at each level. You can use the links on the left to navigate into the API and get detailed documentation for each API item at each level.
 
 See the left hand side for all available submodules.
 """
+
 from cave_utils.api_utils.validator_utils import *
 from cave_utils.api.extraKwargs import extraKwargs
 from cave_utils.api.settings import settings
 from cave_utils.api.appBar import appBar
 from cave_utils.api.panes import panes
 from cave_utils.api.pages import pages
 from cave_utils.api.maps import maps
@@ -93,15 +94,15 @@
             log=self.log,
             prepend_path=["settings"],
             root_data=self.data,
             **kwargs,
         )
         # Special logic to add timeLength to kwargs
         # This is used to validate timeValues across the app
-        kwargs["timeLength"] = pamda.path(["settings","time","timeLength"], self.data)
+        kwargs["timeLength"] = pamda.path(["settings", "time", "timeLength"], self.data)
         # Validate panes
         panes_data = self.data.get("panes")
         pane_validPaneIds = []
         if panes_data is not None:
             panes(data=panes_data, log=self.log, prepend_path=["panes"], **kwargs)
             pane_validPaneIds = list(panes_data.get("data", {}).keys())
         # Validate mapFeatures
```

### Comparing `cave_utils-2.2.0b4/cave_utils/api/appBar.py` & `cave_utils-2.2.0b5/cave_utils/api/appBar.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 simultaneously.
 
 [pages]: pages.html
 [panes]: panes.html
 [predefined]: #appBar_data_star.spec
 [custom]: #appBar_data_star.spec
 """
+
 from cave_utils.api_utils.validator_utils import ApiValidator, CustomKeyValidator
 import type_enforced
 
 
 @type_enforced.Enforcer
 class appBar(ApiValidator):
     """
```

### Comparing `cave_utils-2.2.0b4/cave_utils/api/extraKwargs.py` & `cave_utils-2.2.0b5/cave_utils/api/extraKwargs.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Optionally, pass special arguments to adjust some options related to
 how the CAVE API server handles data.
 """
+
 from cave_utils.api_utils.validator_utils import ApiValidator
 import type_enforced
 
 
 @type_enforced.Enforcer
 class extraKwargs(ApiValidator):
     """
```

### Comparing `cave_utils-2.2.0b4/cave_utils/api/globalOutputs.py` & `cave_utils-2.2.0b5/cave_utils/api/globalOutputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Create outputs that allow for simple charts and tables to present some totalization or global outcome of the data.
 
 These outputs should be general to the entire application and they can be compared across sessions.
 """
+
 from cave_utils.api_utils.validator_utils import ApiValidator, CustomKeyValidator
 from cave_utils.api_utils.general import props, values, layout
 import type_enforced
 
 
 @type_enforced.Enforcer
 class globalOutputs(ApiValidator):
```

### Comparing `cave_utils-2.2.0b4/cave_utils/api/groupedOutputs.py` & `cave_utils-2.2.0b5/cave_utils/api/groupedOutputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Create grouped outputs for building generalized charts and tables.
 """
+
 from cave_utils.api_utils.validator_utils import ApiValidator, CustomKeyValidator
 import type_enforced
 from pamda import pamda
 
 
 @type_enforced.Enforcer
 class groupedOutputs(ApiValidator):
@@ -344,15 +345,22 @@
 @type_enforced.Enforcer
 class groupedOutputs_groupings_star_levels_star(ApiValidator):
     """
     The level data is located under the path **`groupedOutputs.groupings.*.levels.*`**.
     """
 
     @staticmethod
-    def spec(name: str, parent: [str, None] = None, ordering: [list, None] = None, orderWithParent: bool = True, coloring: [dict, None] = None, **kwargs):
+    def spec(
+        name: str,
+        parent: [str, None] = None,
+        ordering: [list, None] = None,
+        orderWithParent: bool = True,
+        coloring: [dict, None] = None,
+        **kwargs,
+    ):
         """
         Arguments:
 
         * **`name`**: `[str]` &rarr; The name of the level.
         * **`parent`**: `[str]` &rarr;
             * The key of the parent level. This is used to create a hierarchy of levels.
             * **Notes**:
@@ -383,19 +391,25 @@
                 subset=[parent],
                 valid_values=kwargs.get("acceptable_parents", []),
                 prepend_path=["parent"],
             )
         ordering = self.data.get("ordering")
         if ordering is not None:
             self.__check_subset_valid__(
-                subset=ordering, valid_values=kwargs.get("acceptable_data_levels", {}).get(kwargs.get('CustomKeyValidatorFieldId'),[]), prepend_path=["ordering"]
+                subset=ordering,
+                valid_values=kwargs.get("acceptable_data_levels", {}).get(
+                    kwargs.get("CustomKeyValidatorFieldId"), []
+                ),
+                prepend_path=["ordering"],
             )
 
         coloring = self.data.get("coloring")
         if coloring is not None:
             self.__check_subset_valid__(
                 subset=list(coloring.keys()),
-                valid_values=kwargs.get("acceptable_data_levels", {}).get(kwargs.get('CustomKeyValidatorFieldId'),[]),
+                valid_values=kwargs.get("acceptable_data_levels", {}).get(
+                    kwargs.get("CustomKeyValidatorFieldId"), []
+                ),
                 prepend_path=["coloring"],
             )
             for key, value in coloring.items():
-                self.__check_rgba_string_valid__(rgba_string=value, prepend_path=['coloring', key])
+                self.__check_rgba_string_valid__(rgba_string=value, prepend_path=["coloring", key])
```

### Comparing `cave_utils-2.2.0b4/cave_utils/api/mapFeatures.py` & `cave_utils-2.2.0b5/cave_utils/api/mapFeatures.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Create visualizations for your map, including `arc`s, `node`s, and `geo`s, and customize their appearance.
 """
+
 from cave_utils.api_utils.validator_utils import ApiValidator, CustomKeyValidator
 from cave_utils.api_utils.general import props, valueLists, layout
 import type_enforced
 from pamda import pamda
 
 
 @type_enforced.Enforcer
@@ -151,18 +152,16 @@
         mapFeatures_data_star_data_location(
             data=location_data,
             log=self.log,
             prepend_path=["location"],
             **kwargs,
         )
         # Validate that all lengths are the same
-        lengths = [
-            len(v) for k, v in location_data.items() if k not in ['timeValues', 'order']
-        ] + [
-            len(v) for k, v in valueLists_data.items() if k not in ['timeValues', 'order']
+        lengths = [len(v) for k, v in location_data.items() if k not in ["timeValues", "order"]] + [
+            len(v) for k, v in valueLists_data.items() if k not in ["timeValues", "order"]
         ]
         if len(set(lengths)) > 1:
             self.__error__(msg=f"location and valueLists keys must have the same length.", path=[])
 
 
 @type_enforced.Enforcer
 class mapFeatures_data_star_data_location(ApiValidator):
@@ -189,18 +188,34 @@
         passed_keys = list(self.data.keys())
         optional_keys = []
         if layer_type == "geo":
             required_keys = ["geoJsonValue"]
         elif layer_type == "arc":
             if layer_geoJson is not None:
                 required_keys = ["geoJsonValue"]
-                optional_keys += ["path", "startLatitude", "startLongitude", "endLatitude", "endLongitude","startAltitude", "endAltitude"]
+                optional_keys += [
+                    "path",
+                    "startLatitude",
+                    "startLongitude",
+                    "endLatitude",
+                    "endLongitude",
+                    "startAltitude",
+                    "endAltitude",
+                ]
             elif "path" in passed_keys:
                 required_keys = ["path"]
-                optional_keys += ["startLatitude", "startLongitude", "endLatitude", "endLongitude", "geoJsonValue","startAltitude", "endAltitude"]
+                optional_keys += [
+                    "startLatitude",
+                    "startLongitude",
+                    "endLatitude",
+                    "endLongitude",
+                    "geoJsonValue",
+                    "startAltitude",
+                    "endAltitude",
+                ]
             else:
                 required_keys = ["startLatitude", "startLongitude", "endLatitude", "endLongitude"]
                 optional_keys += ["startAltitude", "endAltitude", "geoJsonValue", "path"]
         else:
             required_keys = ["latitude", "longitude"]
             optional_keys += ["altitude"]
         missing_keys = pamda.difference(required_keys, list(self.data.keys()))
@@ -211,15 +226,15 @@
             if key not in required_keys + optional_keys:
                 self.__error__(
                     msg=f"`{key}` is not a valid key for location for layer type `{layer_type}`",
                     path=[],
                 )
                 continue
             if key == "geoJsonValue":
-                if len(value_list)!=len(set(value_list)):
+                if len(value_list) != len(set(value_list)):
                     self.__warn__(
                         msg=f"`geoJsonValue` should be a list of unique values. Otherwise, the corresponding map feature may not render correctly.",
                         path=[key],
                     )
             if not isinstance(value_list, list):
                 self.__error__(
                     msg=f"`{key}` must be a list but got {type(value_list)} instead.", path=[key]
```

### Comparing `cave_utils-2.2.0b4/cave_utils/api/maps.py` & `cave_utils-2.2.0b5/cave_utils/api/maps.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Configure the style and UI elements of your application's maps.
 """
+
 from cave_utils.api_utils.validator_utils import ApiValidator, CustomKeyValidator
 import type_enforced
 
 
 @type_enforced.Enforcer
 class maps(ApiValidator):
     """
```

### Comparing `cave_utils-2.2.0b4/cave_utils/api/pages.py` & `cave_utils-2.2.0b5/cave_utils/api/pages.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Configure your application's pages.
 """
+
 from cave_utils.api_utils.validator_utils import ApiValidator, CustomKeyValidator
 import type_enforced
 
 
 @type_enforced.Enforcer
 class pages(ApiValidator):
     """
@@ -133,15 +134,15 @@
         * **`groupedOutputDataId`**: `[str | list]` = `None` &rarr; The id or list of ids representing the grouped output data to use.
         * **`statId`**: `[str | list]` = `None` &rarr; The id or list of ids corresponding to the stat(s) to be used.
         * **`showToolbar`**: `[bool]` = `None` &rarr; Whether or not the chart toolbar should be shown.
             * **Note**: If left unspecified (i.e., `None`), it will default to `settings.showToolbar`.
         * **`maximized`**: `[bool]` = `False` &rarr; Whether or not the layout should be maximized.
             * **Note**: If more than one chart belonging to the same page layout is set to `True`, the first one found in the list will take precedence.
         * **`defaultToZero`**: `[bool]` = `False` &rarr; Whether or not the chart should default missing values to zero.
-            
+
         [area chart]: https://en.wikipedia.org/wiki/Area_chart
         [bar chart]: https://en.wikipedia.org/wiki/Bar_chart
         [stacked bar chart]: https://en.wikipedia.org/wiki/Bar_chart
         [box plot chart]: https://en.wikipedia.org/wiki/Box_plot
         [cumulative line chart]: #
         [gauge chart]: https://echarts.apache.org/examples/en/index.html#chart-type-gauge
         [heatmap chart]: https://en.wikipedia.org/wiki/Heat_map
```

### Comparing `cave_utils-2.2.0b4/cave_utils/api/panes.py` & `cave_utils-2.2.0b5/cave_utils/api/panes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Panes serve as main containers for UI controls such as toggles, text
 and number fields, sliders, etc. They can also contain buttons that
 facilitate interaction with actionable data.
 """
+
 from cave_utils.api_utils.validator_utils import ApiValidator, CustomKeyValidator
 from cave_utils.api_utils.general import props, values, layout
 import type_enforced
 
 
 @type_enforced.Enforcer
 class panes(ApiValidator):
```

### Comparing `cave_utils-2.2.0b4/cave_utils/api/settings.py` & `cave_utils-2.2.0b5/cave_utils/api/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Configure general settings for your application like the icons to use, how to sync data with the server, and more.
 """
+
 from cave_utils.api_utils.validator_utils import *
 import type_enforced
 
 
 @type_enforced.Enforcer
 class settings(ApiValidator):
     """
@@ -287,12 +288,12 @@
         Arguments:
 
         * **`timeLength`**: `[int]` &rarr; The amount of time values to display.
         * **`timeUnits`**: `[str]` &rarr; The units of time to display.
             * **Example**: `"Decade"`.
         """
         return {"kwargs": kwargs, "accepted_values": {}}
-    
+
     def __extend_spec__(self, **kwargs):
         timeLength = self.data.get("timeLength")
         if timeLength < 1:
             self.__error__(f"Time length must be greater than 0.", path=["timeLength"])
```

### Comparing `cave_utils-2.2.0b4/cave_utils/api_utils/general.py` & `cave_utils-2.2.0b5/cave_utils/api_utils/general.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 General API Spec items that are found in multiple places. This is not a key that should be passed as part of your `session_data`.
 """
+
 from pamda import pamda
 import type_enforced
 from cave_utils.api_utils.validator_utils import ApiValidator, CustomKeyValidator
-from typing import Literal
 
 
 @type_enforced.Enforcer
 class props(ApiValidator):
     @staticmethod
     def spec(
         name: str,
@@ -319,21 +319,21 @@
         missing_required = pamda.difference(required_fields, list(passed_values.keys()))
         if len(missing_required) > 0:
             raise Exception(f"Missing required fields: {str(missing_required)}")
         for k, v in passed_values.items():
             if k not in required_fields + optional_fields:
                 kwargs[k] = v
         notationDisplay_options_dict = {
-            'compact': ['short', 'long'],
-            'scientific': ['e', 'e+', 'E', 'E+', 'x10^', 'x10^+'],
-            'engineering': ['e', 'e+', 'E', 'E+', 'x10^', 'x10^+'],
-            'standard': []
+            "compact": ["short", "long"],
+            "scientific": ["e", "e+", "E", "E+", "x10^", "x10^+"],
+            "engineering": ["e", "e+", "E", "E+", "x10^", "x10^+"],
+            "standard": [],
         }
-        notation = passed_values.get('notation', 'standard')
-        legendNotation = passed_values.get('legendNotation', 'standard')
+        notation = passed_values.get("notation", "standard")
+        legendNotation = passed_values.get("legendNotation", "standard")
         view_options_dict = {
             "date": ["year", "month", "day"],
             "time": ["hours", "minutes", "seconds"],
             "datetime": ["year", "month", "day", "hours", "minutes", "seconds"],
         }
         variant = passed_values.get("variant", None)
         return {
@@ -373,14 +373,15 @@
                 log=self.log,
                 prepend_path=["options"],
                 validator=props_options,
                 variant=self.data.get("variant"),
                 **kwargs,
             )
 
+
 @type_enforced.Enforcer
 class props_options(ApiValidator):
     @staticmethod
     def spec(name: str, path: [list[str], None] = None, **kwargs):
         """
         Arguments:
```

### Comparing `cave_utils-2.2.0b4/cave_utils/api_utils/validator.py` & `cave_utils-2.2.0b5/cave_utils/api_utils/validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 This module contains the primary Validator class that is used to validate your session_data against the API spec.
 """
+
 from cave_utils.api_utils.validator_utils import LogObject
 from cave_utils.api import Root
 import type_enforced
 
 
 @type_enforced.Enforcer
 class Validator:
```

### Comparing `cave_utils-2.2.0b4/cave_utils/api_utils/validator_utils.py` & `cave_utils-2.2.0b5/cave_utils/api_utils/validator_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Special utility functions to help in validating your data against the CAVE API. This is not a key that should be passed as part of your `session_data`.
 """
+
 from pamda import pamda
 import type_enforced
 import re, datetime
 from cave_utils.log import LogHelper, LogObject
 
 
 class ApiValidator:
@@ -20,30 +21,30 @@
         This should be overridden by any non utility child class.
         """
         return {
             "kwargs": {},
             "accepted_values": {},
         }
 
-    def __validate__(self, data:dict, log: LogObject, prepend_path: list[str] = list(), **kwargs):
+    def __validate__(self, data: dict, log: LogObject, prepend_path: list[str] = list(), **kwargs):
         """
         Run the API validation process for the passed data.
         """
         # Make a copy of the data to avoid modifying the original
         self.data = {**data}
         self.ignore_keys = kwargs.get("ignore_keys", set())
         self.log = LogHelper(log=log, prepend_path=prepend_path)
         try:
             self.__genericKeyValidation__(**kwargs)
             spec_output = self.spec(**self.data)
             extra_kwargs = spec_output.get("kwargs", {})
             if extra_kwargs != {}:
                 self.__warn__(
                     msg=f"Unknown Fields: {str(list(extra_kwargs.keys()))}",
-                )            
+                )
 
         except Exception as e:
             self.__error__(
                 msg=f"Error validating spec: {e}",
             )
             # Must return since an invalid spec will bug out other validation checks
             return
@@ -73,79 +74,81 @@
 
     # Placeholder method for additional validations
     def __extend_spec__(self, **kwargs):
         pass
 
     # Additional core validations for generic terms like `order` and `timeValues`
     def __genericKeyValidation__(self, **kwargs):
-        # Remove `timeValues` out prior to each level validation 
+        # Remove `timeValues` out prior to each level validation
         data_timeValues = self.data.pop("timeValues", None)
         # Remove `order` out prior to each level validation
         data_order = self.data.pop("order", None)
         if data_timeValues is not None:
             timeLength = kwargs.get("timeLength")
             if timeLength is None:
                 self.__error__(
-                    path=['timeValues'],
+                    path=["timeValues"],
                     msg="`settings.time.timeLength` must be specified to validate `timeValues`",
                 )
             else:
                 self.__timeValues_validation__(timeValues=data_timeValues, timeLength=timeLength)
         if data_order is not None:
             self.__order_validation__(order=data_order)
-            
+
     @type_enforced.Enforcer
-    def __order_validation__(self, order:dict[list[str,int]]):
+    def __order_validation__(self, order: dict[list[str, int]]):
         """
         Check that the ordering options are valid
         """
-        orderable_data_keys = {key: list(value.keys()) for key, value in self.data.items() if isinstance(value, dict)}
+        orderable_data_keys = {
+            key: list(value.keys()) for key, value in self.data.items() if isinstance(value, dict)
+        }
         if self.__check_subset_valid__(
             subset=list(order.keys()),
             valid_values=list(orderable_data_keys.keys()),
             prepend_path=["order"],
         ):
             for order_key, order_list in order.items():
                 self.__check_subset_valid__(
                     subset=order_list,
                     valid_values=orderable_data_keys[order_key],
                     prepend_path=["order", order_key],
                 )
-    
+
     @type_enforced.Enforcer
-    def __timeValues_validation__(self, timeValues: [dict[dict],list[dict]], timeLength:int):
+    def __timeValues_validation__(self, timeValues: [dict[dict], list[dict]], timeLength: int):
         if len(timeValues) == 0:
             return
         if isinstance(timeValues, list):
             if len(timeValues) != timeLength:
                 self.__error__(
-                    path=['timeValues'],
+                    path=["timeValues"],
                     msg=f"The length of `timeValues` (as a list) must be equal to `settings.time.timeLength` ({timeLength})",
                 )
                 return
         if isinstance(timeValues, dict):
             keys = list(timeValues.keys())
             if not all(isinstance(key, int) for key in keys):
                 self.__error__(
-                    path=['timeValues'],
+                    path=["timeValues"],
                     msg="`timeValues` (as a dict) keys must be integers",
                 )
                 return
-            if not all(key >= 0 and key<timeLength for key in keys):
+            if not all(key >= 0 and key < timeLength for key in keys):
                 self.__error__(
-                    path=['timeValues'],
+                    path=["timeValues"],
                     msg=f"`timeValues` (as a dict) keys must be integers between 0 and {timeLength-1} inclusive (1 minus the value at `settings.time.timeLength`)",
                 )
                 return
             timeValues = list(timeValues.values())
-        timeValueTypes = {k:type(v) for k,v in timeValues[0].items()}
+        timeValueTypes = {k: type(v) for k, v in timeValues[0].items()}
         for timeValue in timeValues:
-            if timeValueTypes != {k:type(v) for k,v in timeValue.items()}:
+            if timeValueTypes != {k: type(v) for k, v in timeValue.items()}:
                 self.__error__(
-                    path=['timeValues'],
+                    path=["timeValues"],
                     msg="All timeValues must have the same keys and each key must have the same type",
                 )
                 return
         # Update the data with the first timeValue prioritizing original data
         # over the first timeValue
         self.data = {**timeValues[0], **self.data}
 
@@ -281,15 +284,17 @@
             self.__error__(
                 path=prepend_path,
                 msg=f"Invalid value(s) selected: {str(invalid_values)}. Accepted Values are {valid_values}",
             )
             return False
         return True
 
-    def __check_coord_path_valid__(self, coord_path: list[list[int,float]], prepend_path: list[str] = list()):
+    def __check_coord_path_valid__(
+        self, coord_path: list[list[int, float]], prepend_path: list[str] = list()
+    ):
         """
         Validate a coordinate path and if an issue is present, log an error
         """
         try:
             if len(coord_path) < 2:
                 self.__error__(path=prepend_path, msg="Invalid coordinate path")
                 return
```

### Comparing `cave_utils-2.2.0b4/cave_utils/arguments.py` & `cave_utils-2.2.0b5/cave_utils/arguments.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b4/cave_utils/builders/groups.py` & `cave_utils-2.2.0b5/cave_utils/builders/groups.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b4/cave_utils/log.py` & `cave_utils-2.2.0b5/cave_utils/log.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b4/cave_utils.egg-info/PKG-INFO` & `cave_utils-2.2.0b5/cave_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cave_utils
-Version: 2.2.0b4
+Version: 2.2.0b5
 Summary: Python wrapper for api use in the cave_app
 Author-email: Connor Makowski <conmak@mit.edu>
 Project-URL: Homepage, https://github.com/mit-cave/cave_utils
 Project-URL: Bug Tracker, https://github.com/mit-cave/cave_utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `cave_utils-2.2.0b4/cave_utils.egg-info/SOURCES.txt` & `cave_utils-2.2.0b5/cave_utils.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 NOTICE.md
 README.md
 pyproject.toml
 setup.cfg
 cave_utils/__init__.py
 cave_utils/arguments.py
+cave_utils/geo_utils.py
 cave_utils/log.py
 cave_utils/socket.py
 cave_utils.egg-info/PKG-INFO
 cave_utils.egg-info/SOURCES.txt
 cave_utils.egg-info/dependency_links.txt
 cave_utils.egg-info/requires.txt
 cave_utils.egg-info/top_level.txt
@@ -26,10 +27,11 @@
 cave_utils/api_utils/general.py
 cave_utils/api_utils/validator.py
 cave_utils/api_utils/validator_utils.py
 cave_utils/builders/__init__.py
 cave_utils/builders/groups.py
 test/test_arguments.py
 test/test_builders_groups.py
+test/test_geo_utils.py
 test/test_import.py
 test/test_log.py
 test/test_validator.py
```

### Comparing `cave_utils-2.2.0b4/pyproject.toml` & `cave_utils-2.2.0b5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cave_utils"
-version = "2.2.0b4"
+version = "2.2.0b5"
 description = "Python wrapper for api use in the cave_app"
 authors = [
     {name="Connor Makowski", email="conmak@mit.edu"}
 ]
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `cave_utils-2.2.0b4/test/test_builders_groups.py` & `cave_utils-2.2.0b5/test/test_builders_groups.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b4/test/test_validator.py` & `cave_utils-2.2.0b5/test/test_validator.py`

 * *Files identical despite different names*

