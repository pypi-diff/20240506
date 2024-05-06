# Comparing `tmp/hashboard_cli-1.1.1.tar.gz` & `tmp/hashboard_cli-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hashboard_cli-1.1.1.tar", last modified: Tue Apr 30 15:42:37 2024, max compression
+gzip compressed data, was "hashboard_cli-1.1.2.tar", last modified: Mon May  6 18:51:16 2024, max compression
```

## Comparing `hashboard_cli-1.1.1.tar` & `hashboard_cli-1.1.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-30 15:42:37.996304 hashboard_cli-1.1.1/
--rw-r--r--   0 anixon     (501) staff       (20)    11357 2022-12-17 00:47:55.000000 hashboard_cli-1.1.1/LICENSE
--rw-r--r--   0 anixon     (501) staff       (20)      924 2024-04-30 15:42:37.996247 hashboard_cli-1.1.1/PKG-INFO
--rw-r--r--   0 anixon     (501) staff       (20)      141 2023-09-29 18:00:46.000000 hashboard_cli-1.1.1/README.md
--rw-r--r--   0 anixon     (501) staff       (20)      104 2023-08-30 15:47:31.000000 hashboard_cli-1.1.1/pyproject.toml
--rw-r--r--   0 anixon     (501) staff       (20)      878 2024-04-30 15:42:37.996575 hashboard_cli-1.1.1/setup.cfg
--rw-r--r--   0 anixon     (501) staff       (20)       38 2022-12-17 00:47:55.000000 hashboard_cli-1.1.1/setup.py
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-30 15:42:37.988758 hashboard_cli-1.1.1/src/
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-30 15:42:37.991011 hashboard_cli-1.1.1/src/hashboard/
--rw-r--r--   0 anixon     (501) staff       (20)       18 2024-04-30 15:41:53.000000 hashboard_cli-1.1.1/src/hashboard/__init__.py
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-30 15:42:37.991280 hashboard_cli-1.1.1/src/hashboard/api/
--rw-r--r--   0 anixon     (501) staff       (20)    15394 2024-04-30 14:54:57.000000 hashboard_cli-1.1.1/src/hashboard/api/__init__.py
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-30 15:42:37.992023 hashboard_cli-1.1.1/src/hashboard/api/access_keys/
--rw-r--r--   0 anixon     (501) staff       (20)        0 2023-09-19 18:12:31.000000 hashboard_cli-1.1.1/src/hashboard/api/access_keys/__init__.py
--rw-r--r--   0 anixon     (501) staff       (20)     4227 2023-09-19 18:12:31.000000 hashboard_cli-1.1.1/src/hashboard/api/access_keys/browser_auth.py
--rw-r--r--   0 anixon     (501) staff       (20)     4409 2024-03-18 20:02:56.000000 hashboard_cli-1.1.1/src/hashboard/api/access_keys/existing_user.py
--rw-r--r--   0 anixon     (501) staff       (20)     2143 2024-03-18 20:02:56.000000 hashboard_cli-1.1.1/src/hashboard/api/access_keys/utils.py
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-30 15:42:37.992712 hashboard_cli-1.1.1/src/hashboard/api/analytics/
--rw-r--r--   0 anixon     (501) staff       (20)      900 2023-09-29 18:00:46.000000 hashboard_cli-1.1.1/src/hashboard/api/analytics/__init__.py
--rw-r--r--   0 anixon     (501) staff       (20)     4003 2023-09-29 18:00:46.000000 hashboard_cli-1.1.1/src/hashboard/api/analytics/cli_with_tracking.py
--rw-r--r--   0 anixon     (501) staff       (20)       20 2024-04-16 20:21:42.000000 hashboard_cli-1.1.1/src/hashboard/api/analytics/events.py
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-30 15:42:37.993247 hashboard_cli-1.1.1/src/hashboard/api/datasource/
--rw-r--r--   0 anixon     (501) staff       (20)        0 2024-04-22 20:51:24.000000 hashboard_cli-1.1.1/src/hashboard/api/datasource/__init__.py
--rw-r--r--   0 anixon     (501) staff       (20)     9994 2024-04-26 20:17:46.000000 hashboard_cli-1.1.1/src/hashboard/api/datasource/datasource_cli.py
--rw-r--r--   0 anixon     (501) staff       (20)    10025 2024-04-26 20:17:46.000000 hashboard_cli-1.1.1/src/hashboard/api/datasource/utils.py
--rw-r--r--   0 anixon     (501) staff       (20)    39341 2024-04-30 14:54:57.000000 hashboard_cli-1.1.1/src/hashboard/cli.py
--rw-r--r--   0 anixon     (501) staff       (20)      346 2023-09-19 18:12:31.000000 hashboard_cli-1.1.1/src/hashboard/constants.py
--rw-r--r--   0 anixon     (501) staff       (20)     1744 2023-09-19 18:12:31.000000 hashboard_cli-1.1.1/src/hashboard/credentials.py
--rw-r--r--   0 anixon     (501) staff       (20)     3843 2024-04-16 20:21:42.000000 hashboard_cli-1.1.1/src/hashboard/filesystem.py
--rw-r--r--   0 anixon     (501) staff       (20)      597 2023-09-29 18:00:46.000000 hashboard_cli-1.1.1/src/hashboard/session.py
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-30 15:42:37.994389 hashboard_cli-1.1.1/src/hashboard/utils/
--rw-r--r--   0 anixon     (501) staff       (20)        0 2023-09-19 18:12:31.000000 hashboard_cli-1.1.1/src/hashboard/utils/__init__.py
--rw-r--r--   0 anixon     (501) staff       (20)      665 2023-09-19 18:12:31.000000 hashboard_cli-1.1.1/src/hashboard/utils/cli.py
--rw-r--r--   0 anixon     (501) staff       (20)     1977 2024-04-16 20:21:42.000000 hashboard_cli-1.1.1/src/hashboard/utils/config.py
--rw-r--r--   0 anixon     (501) staff       (20)      230 2023-09-19 18:12:31.000000 hashboard_cli-1.1.1/src/hashboard/utils/env.py
--rw-r--r--   0 anixon     (501) staff       (20)     2922 2023-11-06 18:51:09.000000 hashboard_cli-1.1.1/src/hashboard/utils/grn.py
--rw-r--r--   0 anixon     (501) staff       (20)      941 2023-09-19 18:12:31.000000 hashboard_cli-1.1.1/src/hashboard/utils/input_validation.py
--rw-r--r--   0 anixon     (501) staff       (20)     1468 2023-09-19 18:12:31.000000 hashboard_cli-1.1.1/src/hashboard/utils/resource.py
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-30 15:42:37.995855 hashboard_cli-1.1.1/src/hashboard_cli.egg-info/
--rw-r--r--   0 anixon     (501) staff       (20)      924 2024-04-30 15:42:37.000000 hashboard_cli-1.1.1/src/hashboard_cli.egg-info/PKG-INFO
--rw-r--r--   0 anixon     (501) staff       (20)     1224 2024-04-30 15:42:37.000000 hashboard_cli-1.1.1/src/hashboard_cli.egg-info/SOURCES.txt
--rw-r--r--   0 anixon     (501) staff       (20)        1 2024-04-30 15:42:37.000000 hashboard_cli-1.1.1/src/hashboard_cli.egg-info/dependency_links.txt
--rw-r--r--   0 anixon     (501) staff       (20)       42 2024-04-30 15:42:37.000000 hashboard_cli-1.1.1/src/hashboard_cli.egg-info/entry_points.txt
--rw-r--r--   0 anixon     (501) staff       (20)      138 2024-04-30 15:42:37.000000 hashboard_cli-1.1.1/src/hashboard_cli.egg-info/requires.txt
--rw-r--r--   0 anixon     (501) staff       (20)       10 2024-04-30 15:42:37.000000 hashboard_cli-1.1.1/src/hashboard_cli.egg-info/top_level.txt
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-30 15:42:37.995684 hashboard_cli-1.1.1/tests/
--rw-r--r--   0 anixon     (501) staff       (20)      310 2023-09-19 18:12:31.000000 hashboard_cli-1.1.1/tests/test_cli.py
--rw-r--r--   0 anixon     (501) staff       (20)     1534 2023-09-19 18:12:31.000000 hashboard_cli-1.1.1/tests/test_credentials.py
--rw-r--r--   0 anixon     (501) staff       (20)     3890 2024-04-16 20:21:42.000000 hashboard_cli-1.1.1/tests/test_filesystem.py
--rw-r--r--   0 anixon     (501) staff       (20)      668 2023-09-19 18:12:31.000000 hashboard_cli-1.1.1/tests/test_hashboard_api.py
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-05-06 18:51:16.762000 hashboard_cli-1.1.2/
+-rw-r--r--   0 anixon     (501) staff       (20)    11357 2022-12-17 00:47:55.000000 hashboard_cli-1.1.2/LICENSE
+-rw-r--r--   0 anixon     (501) staff       (20)      924 2024-05-06 18:51:16.761922 hashboard_cli-1.1.2/PKG-INFO
+-rw-r--r--   0 anixon     (501) staff       (20)      141 2023-09-29 18:00:46.000000 hashboard_cli-1.1.2/README.md
+-rw-r--r--   0 anixon     (501) staff       (20)      104 2023-08-30 15:47:31.000000 hashboard_cli-1.1.2/pyproject.toml
+-rw-r--r--   0 anixon     (501) staff       (20)      878 2024-05-06 18:51:16.762310 hashboard_cli-1.1.2/setup.cfg
+-rw-r--r--   0 anixon     (501) staff       (20)       38 2022-12-17 00:47:55.000000 hashboard_cli-1.1.2/setup.py
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-05-06 18:51:16.754000 hashboard_cli-1.1.2/src/
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-05-06 18:51:16.756283 hashboard_cli-1.1.2/src/hashboard/
+-rw-r--r--   0 anixon     (501) staff       (20)       18 2024-05-06 18:49:33.000000 hashboard_cli-1.1.2/src/hashboard/__init__.py
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-05-06 18:51:16.756493 hashboard_cli-1.1.2/src/hashboard/api/
+-rw-r--r--   0 anixon     (501) staff       (20)    15394 2024-04-30 14:54:57.000000 hashboard_cli-1.1.2/src/hashboard/api/__init__.py
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-05-06 18:51:16.757477 hashboard_cli-1.1.2/src/hashboard/api/access_keys/
+-rw-r--r--   0 anixon     (501) staff       (20)        0 2023-09-19 18:12:31.000000 hashboard_cli-1.1.2/src/hashboard/api/access_keys/__init__.py
+-rw-r--r--   0 anixon     (501) staff       (20)     4227 2023-09-19 18:12:31.000000 hashboard_cli-1.1.2/src/hashboard/api/access_keys/browser_auth.py
+-rw-r--r--   0 anixon     (501) staff       (20)     4409 2024-03-18 20:02:56.000000 hashboard_cli-1.1.2/src/hashboard/api/access_keys/existing_user.py
+-rw-r--r--   0 anixon     (501) staff       (20)     2143 2024-03-18 20:02:56.000000 hashboard_cli-1.1.2/src/hashboard/api/access_keys/utils.py
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-05-06 18:51:16.758173 hashboard_cli-1.1.2/src/hashboard/api/analytics/
+-rw-r--r--   0 anixon     (501) staff       (20)      900 2023-09-29 18:00:46.000000 hashboard_cli-1.1.2/src/hashboard/api/analytics/__init__.py
+-rw-r--r--   0 anixon     (501) staff       (20)     4003 2023-09-29 18:00:46.000000 hashboard_cli-1.1.2/src/hashboard/api/analytics/cli_with_tracking.py
+-rw-r--r--   0 anixon     (501) staff       (20)       20 2024-04-16 20:21:42.000000 hashboard_cli-1.1.2/src/hashboard/api/analytics/events.py
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-05-06 18:51:16.758751 hashboard_cli-1.1.2/src/hashboard/api/datasource/
+-rw-r--r--   0 anixon     (501) staff       (20)        0 2024-04-22 20:51:24.000000 hashboard_cli-1.1.2/src/hashboard/api/datasource/__init__.py
+-rw-r--r--   0 anixon     (501) staff       (20)     9994 2024-04-26 20:17:46.000000 hashboard_cli-1.1.2/src/hashboard/api/datasource/datasource_cli.py
+-rw-r--r--   0 anixon     (501) staff       (20)    10025 2024-04-26 20:17:46.000000 hashboard_cli-1.1.2/src/hashboard/api/datasource/utils.py
+-rw-r--r--   0 anixon     (501) staff       (20)    40009 2024-05-06 18:45:35.000000 hashboard_cli-1.1.2/src/hashboard/cli.py
+-rw-r--r--   0 anixon     (501) staff       (20)      346 2023-09-19 18:12:31.000000 hashboard_cli-1.1.2/src/hashboard/constants.py
+-rw-r--r--   0 anixon     (501) staff       (20)     1744 2023-09-19 18:12:31.000000 hashboard_cli-1.1.2/src/hashboard/credentials.py
+-rw-r--r--   0 anixon     (501) staff       (20)     3973 2024-05-06 18:45:35.000000 hashboard_cli-1.1.2/src/hashboard/filesystem.py
+-rw-r--r--   0 anixon     (501) staff       (20)      597 2023-09-29 18:00:46.000000 hashboard_cli-1.1.2/src/hashboard/session.py
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-05-06 18:51:16.759865 hashboard_cli-1.1.2/src/hashboard/utils/
+-rw-r--r--   0 anixon     (501) staff       (20)        0 2023-09-19 18:12:31.000000 hashboard_cli-1.1.2/src/hashboard/utils/__init__.py
+-rw-r--r--   0 anixon     (501) staff       (20)      665 2023-09-19 18:12:31.000000 hashboard_cli-1.1.2/src/hashboard/utils/cli.py
+-rw-r--r--   0 anixon     (501) staff       (20)     1977 2024-04-16 20:21:42.000000 hashboard_cli-1.1.2/src/hashboard/utils/config.py
+-rw-r--r--   0 anixon     (501) staff       (20)      230 2023-09-19 18:12:31.000000 hashboard_cli-1.1.2/src/hashboard/utils/env.py
+-rw-r--r--   0 anixon     (501) staff       (20)     2922 2023-11-06 18:51:09.000000 hashboard_cli-1.1.2/src/hashboard/utils/grn.py
+-rw-r--r--   0 anixon     (501) staff       (20)      941 2023-09-19 18:12:31.000000 hashboard_cli-1.1.2/src/hashboard/utils/input_validation.py
+-rw-r--r--   0 anixon     (501) staff       (20)     1468 2023-09-19 18:12:31.000000 hashboard_cli-1.1.2/src/hashboard/utils/resource.py
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-05-06 18:51:16.761493 hashboard_cli-1.1.2/src/hashboard_cli.egg-info/
+-rw-r--r--   0 anixon     (501) staff       (20)      924 2024-05-06 18:51:16.000000 hashboard_cli-1.1.2/src/hashboard_cli.egg-info/PKG-INFO
+-rw-r--r--   0 anixon     (501) staff       (20)     1224 2024-05-06 18:51:16.000000 hashboard_cli-1.1.2/src/hashboard_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 anixon     (501) staff       (20)        1 2024-05-06 18:51:16.000000 hashboard_cli-1.1.2/src/hashboard_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 anixon     (501) staff       (20)       42 2024-05-06 18:51:16.000000 hashboard_cli-1.1.2/src/hashboard_cli.egg-info/entry_points.txt
+-rw-r--r--   0 anixon     (501) staff       (20)      138 2024-05-06 18:51:16.000000 hashboard_cli-1.1.2/src/hashboard_cli.egg-info/requires.txt
+-rw-r--r--   0 anixon     (501) staff       (20)       10 2024-05-06 18:51:16.000000 hashboard_cli-1.1.2/src/hashboard_cli.egg-info/top_level.txt
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-05-06 18:51:16.761253 hashboard_cli-1.1.2/tests/
+-rw-r--r--   0 anixon     (501) staff       (20)      310 2023-09-19 18:12:31.000000 hashboard_cli-1.1.2/tests/test_cli.py
+-rw-r--r--   0 anixon     (501) staff       (20)     1534 2023-09-19 18:12:31.000000 hashboard_cli-1.1.2/tests/test_credentials.py
+-rw-r--r--   0 anixon     (501) staff       (20)     4245 2024-05-06 18:45:35.000000 hashboard_cli-1.1.2/tests/test_filesystem.py
+-rw-r--r--   0 anixon     (501) staff       (20)      668 2023-09-19 18:12:31.000000 hashboard_cli-1.1.2/tests/test_hashboard_api.py
```

### Comparing `hashboard_cli-1.1.1/LICENSE` & `hashboard_cli-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.1.1/PKG-INFO` & `hashboard_cli-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashboard-cli
-Version: 1.1.1
+Version: 1.1.2
 Summary: Command-line tools for interacting with Hashboard
 Home-page: https://hashboard.com/
 Author: Dan Eisenberg
 Author-email: dan@hashboard.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `hashboard_cli-1.1.1/setup.cfg` & `hashboard_cli-1.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.1.1/src/hashboard/api/__init__.py` & `hashboard_cli-1.1.2/src/hashboard/api/__init__.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.1.1/src/hashboard/api/access_keys/browser_auth.py` & `hashboard_cli-1.1.2/src/hashboard/api/access_keys/browser_auth.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.1.1/src/hashboard/api/access_keys/existing_user.py` & `hashboard_cli-1.1.2/src/hashboard/api/access_keys/existing_user.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.1.1/src/hashboard/api/access_keys/utils.py` & `hashboard_cli-1.1.2/src/hashboard/api/access_keys/utils.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.1.1/src/hashboard/api/analytics/__init__.py` & `hashboard_cli-1.1.2/src/hashboard/api/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.1.1/src/hashboard/api/analytics/cli_with_tracking.py` & `hashboard_cli-1.1.2/src/hashboard/api/analytics/cli_with_tracking.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.1.1/src/hashboard/api/datasource/datasource_cli.py` & `hashboard_cli-1.1.2/src/hashboard/api/datasource/datasource_cli.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.1.1/src/hashboard/api/datasource/utils.py` & `hashboard_cli-1.1.2/src/hashboard/api/datasource/utils.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.1.1/src/hashboard/cli.py` & `hashboard_cli-1.1.2/src/hashboard/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -427,19 +427,19 @@
         click.echo("\r" + next(spinner), nl=False)
         if not i % 10:
             click.echo("\b ", nl=False)
             sys.stdout.flush()
             partial_build = fetch_build_status(s, build_id)
             if ("errors" in partial_build and partial_build["errors"]) or partial_build[
                 "data"
-            ]["fetchBuild"]["status"] == "completed":
+            ]["fetchBuild"]["status"] in ["completed", "applied"]:
                 build = fetch_build(s, build_id)
                 return build
             elif (
-                partial_build["data"]["fetchBuild"]["status"] == "running"
+                partial_build["data"]["fetchBuild"]["status"] == "building"
                 and not is_running
             ):
                 click.echo("\bBuilding resources... ")
                 is_running = True
         time.sleep(0.5)
     click.echo("Error fetching build, max attempt.", fg="red")
     click.get_current_context().exit(1)
@@ -865,14 +865,15 @@
     return {
         "modelBundles": [],
         "metrics": [],
         "savedViews": [],
         "dashboards": [],
         "colorPalettes": [],
         "homepageLaunchpads": [],
+        "reportSchedules": [],
     }
 
 
 def _convert_to_resource_update_list(resource_changes: dict):
     result = {
         "added": _get_empty_status_groups(),
         "changed": _get_empty_status_groups(),
@@ -888,16 +889,22 @@
     type_to_status_group = {
         "modelBundle": "modelBundles",
         "savedView": "savedViews",
         "dashboard-v2": "dashboards",
         "projectMetric": "metrics",
         "colorPalette": "colorPalettes",
         "homepageLaunchpad": "homepageLaunchpads",
+        "reportSchedule": "reportSchedules",
     }
     for rc in resource_changes.values():
+        rcType = rc["newContent"]["value"]["type"]
+        content = rc["newContent"]["value"]
+        if rcType == "reportSchedule":
+            report_id = content.get("id")
+            content["name"] = content.get("subject", f"Report schedule {report_id}")
         result[action_to_status[rc["action"]]][
             type_to_status_group[rc["newContent"]["value"]["type"]]
         ].append(rc["newContent"]["value"])
 
     return result
 
 
@@ -1037,22 +1044,24 @@
 def _echo_resources_with_status(resources: dict, status: str, title: str):
     model_bundles = resources[status]["modelBundles"]
     metrics = resources[status]["metrics"]
     saved_views = resources[status]["savedViews"]
     dashboards = resources[status]["dashboards"]
     color_palettes = resources[status]["colorPalettes"]
     homepage_launchpads = resources[status]["homepageLaunchpads"]
+    report_schedules = resources[status].get("reportSchedules", [])
 
     combinedResources = (
         model_bundles
         + metrics
         + saved_views
         + dashboards
         + color_palettes
         + homepage_launchpads
+        + report_schedules
     )
 
     if combinedResources:
         click.echo(title)
         _echo_list(
             [
                 click.style("Model - ", fg="bright_black")
@@ -1079,14 +1088,21 @@
                 click.style("Dashboard - ", fg="bright_black")
                 + click.style(r["name"], fg="white")
                 for r in dashboards
             ]
         )
         _echo_list(
             [
+                click.style("Report schedule - ", fg="bright_black")
+                + click.style(r["name"], fg="white")
+                for r in report_schedules
+            ]
+        )
+        _echo_list(
+            [
                 click.style("Color Palette - ", fg="bright_black")
                 + click.style(r["name"], fg="white")
                 for r in color_palettes
             ]
         )
         _echo_list(
             [
```

### Comparing `hashboard_cli-1.1.1/src/hashboard/credentials.py` & `hashboard_cli-1.1.2/src/hashboard/credentials.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.1.1/src/hashboard/filesystem.py` & `hashboard_cli-1.1.2/src/hashboard/filesystem.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,18 @@
         try:
             with open(Path(dbt_manifest_path), "r") as f:
                 dbt_manifest = f.read()
         except Exception as e:
             raise ClickException(f"Could not read dbt manifest file: {e}")
 
     for root, subdirs, filenames in os.walk(path):
+        current_dir = os.path.basename(root)
+        if current_dir.startswith('.') and current_dir != ".":
+            continue
+
         for filename in filenames:
             if pathlib.Path(filename).suffix not in VALID_FILE_EXTENSIONS:
                 continue
             if targets:
                 if filename not in targets:
                     continue
             with open(os.path.join(root, filename), "r") as f:
```

### Comparing `hashboard_cli-1.1.1/src/hashboard/session.py` & `hashboard_cli-1.1.2/src/hashboard/session.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.1.1/src/hashboard/utils/cli.py` & `hashboard_cli-1.1.2/src/hashboard/utils/cli.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.1.1/src/hashboard/utils/config.py` & `hashboard_cli-1.1.2/src/hashboard/utils/config.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.1.1/src/hashboard/utils/grn.py` & `hashboard_cli-1.1.2/src/hashboard/utils/grn.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.1.1/src/hashboard/utils/input_validation.py` & `hashboard_cli-1.1.2/src/hashboard/utils/input_validation.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.1.1/src/hashboard/utils/resource.py` & `hashboard_cli-1.1.2/src/hashboard/utils/resource.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.1.1/src/hashboard_cli.egg-info/PKG-INFO` & `hashboard_cli-1.1.2/src/hashboard_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashboard-cli
-Version: 1.1.1
+Version: 1.1.2
 Summary: Command-line tools for interacting with Hashboard
 Home-page: https://hashboard.com/
 Author: Dan Eisenberg
 Author-email: dan@hashboard.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `hashboard_cli-1.1.1/src/hashboard_cli.egg-info/SOURCES.txt` & `hashboard_cli-1.1.2/src/hashboard_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.1.1/tests/test_credentials.py` & `hashboard_cli-1.1.2/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.1.1/tests/test_filesystem.py` & `hashboard_cli-1.1.2/tests/test_filesystem.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,7 +118,19 @@
                 "type": "saved_view",
                 "model": "../models/model.yaml",
             },
             type="saved_view",
             grn=None,
         ),
     }
+
+    # Test to ensure files in hidden folders aren't being read
+    assert display(
+        local_resources(get_fixture_path("model_config_files/with_hidden_folders"))
+    ) == {
+        "model.yml": Resource(
+            hb_version="1.0",
+            raw={"glean": "1.0", "type": "model"},
+            type="model",
+            grn=None,
+        ),
+    }
```

### Comparing `hashboard_cli-1.1.1/tests/test_hashboard_api.py` & `hashboard_cli-1.1.2/tests/test_hashboard_api.py`

 * *Files identical despite different names*

