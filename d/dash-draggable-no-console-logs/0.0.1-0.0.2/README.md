# Comparing `tmp/dash_draggable_no_console_logs-0.0.1.tar.gz` & `tmp/dash_draggable_no_console_logs-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_draggable_no_console_logs-0.0.1.tar", last modified: Mon May  6 14:42:01 2024, max compression
+gzip compressed data, was "dash_draggable_no_console_logs-0.0.2.tar", last modified: Mon May  6 15:05:26 2024, max compression
```

## Comparing `dash_draggable_no_console_logs-0.0.1.tar` & `dash_draggable_no_console_logs-0.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 14:42:01.162360 dash_draggable_no_console_logs-0.0.1/
--rw-rw-rw-   0        0        0     1088 2024-05-06 14:13:39.000000 dash_draggable_no_console_logs-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      234 2024-05-06 14:13:39.000000 dash_draggable_no_console_logs-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      313 2024-05-06 14:42:01.158369 dash_draggable_no_console_logs-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4956 2024-05-06 14:13:39.000000 dash_draggable_no_console_logs-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 14:42:01.114093 dash_draggable_no_console_logs-0.0.1/dash_draggable_no_console_logs/
--rw-rw-rw-   0        0        0     2041 2024-05-06 14:13:39.000000 dash_draggable_no_console_logs-0.0.1/dash_draggable_no_console_logs/DashDraggable.py
--rw-rw-rw-   0        0        0     1574 2024-05-06 14:13:39.000000 dash_draggable_no_console_logs-0.0.1/dash_draggable_no_console_logs/DashDraggable2.py
--rw-rw-rw-   0        0        0     1840 2024-05-06 14:13:39.000000 dash_draggable_no_console_logs-0.0.1/dash_draggable_no_console_logs/DashDraggableResponsive.py
--rw-rw-rw-   0        0        0     2940 2024-05-06 14:13:39.000000 dash_draggable_no_console_logs-0.0.1/dash_draggable_no_console_logs/DashboardItem.py
--rw-rw-rw-   0        0        0     3355 2024-05-06 14:13:39.000000 dash_draggable_no_console_logs-0.0.1/dash_draggable_no_console_logs/DashboardItemResponsive.py
--rw-rw-rw-   0        0        0     3202 2024-05-06 14:13:39.000000 dash_draggable_no_console_logs-0.0.1/dash_draggable_no_console_logs/DragItem.py
--rw-rw-rw-   0        0        0     3842 2024-05-06 14:13:39.000000 dash_draggable_no_console_logs-0.0.1/dash_draggable_no_console_logs/DraggableDashboard.py
--rw-rw-rw-   0        0        0     4421 2024-05-06 14:13:39.000000 dash_draggable_no_console_logs-0.0.1/dash_draggable_no_console_logs/DraggableDashboardResponsive.py
--rw-rw-rw-   0        0        0     5682 2024-05-06 14:13:39.000000 dash_draggable_no_console_logs-0.0.1/dash_draggable_no_console_logs/GridLayout.py
--rw-rw-rw-   0        0        0     6144 2024-05-06 14:13:39.000000 dash_draggable_no_console_logs-0.0.1/dash_draggable_no_console_logs/ResponsiveGridLayout.py
--rw-rw-rw-   0        0        0     1315 2024-05-06 14:13:39.000000 dash_draggable_no_console_logs-0.0.1/dash_draggable_no_console_logs/__init__.py
--rw-rw-rw-   0        0        0      501 2024-05-06 14:13:39.000000 dash_draggable_no_console_logs-0.0.1/dash_draggable_no_console_logs/_imports_.py
--rw-rw-rw-   0        0        0     5682 2024-05-06 14:13:39.000000 dash_draggable_no_console_logs-0.0.1/dash_draggable_no_console_logs/demo.py
--rw-rw-rw-   0        0        0     1982 2024-05-06 14:13:39.000000 dash_draggable_no_console_logs-0.0.1/dash_draggable_no_console_logs/test.py
-drwxrwxrwx   0        0        0        0 2024-05-06 14:42:01.144360 dash_draggable_no_console_logs-0.0.1/dash_draggable_no_console_logs.egg-info/
--rw-rw-rw-   0        0        0      313 2024-05-06 14:42:00.000000 dash_draggable_no_console_logs-0.0.1/dash_draggable_no_console_logs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      972 2024-05-06 14:42:00.000000 dash_draggable_no_console_logs-0.0.1/dash_draggable_no_console_logs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 14:42:00.000000 dash_draggable_no_console_logs-0.0.1/dash_draggable_no_console_logs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-05-06 14:42:00.000000 dash_draggable_no_console_logs-0.0.1/dash_draggable_no_console_logs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2087 2024-05-06 14:41:52.000000 dash_draggable_no_console_logs-0.0.1/package.json
--rw-rw-rw-   0        0        0       42 2024-05-06 14:42:01.163369 dash_draggable_no_console_logs-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      533 2024-05-06 14:13:39.000000 dash_draggable_no_console_logs-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 14:42:01.150367 dash_draggable_no_console_logs-0.0.1/tests/
--rw-rw-rw-   0        0        0      945 2024-05-06 14:13:40.000000 dash_draggable_no_console_logs-0.0.1/tests/test_usage.py
+drwxrwxrwx   0        0        0        0 2024-05-06 15:05:26.275503 dash_draggable_no_console_logs-0.0.2/
+-rw-rw-rw-   0        0        0     1088 2024-05-06 14:13:39.000000 dash_draggable_no_console_logs-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      234 2024-05-06 14:13:39.000000 dash_draggable_no_console_logs-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      313 2024-05-06 15:05:26.269501 dash_draggable_no_console_logs-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4956 2024-05-06 14:13:39.000000 dash_draggable_no_console_logs-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 15:05:26.246507 dash_draggable_no_console_logs-0.0.2/dash_draggable_no_console_logs/
+-rw-rw-rw-   0        0        0     2041 2024-05-06 14:13:39.000000 dash_draggable_no_console_logs-0.0.2/dash_draggable_no_console_logs/DashDraggable.py
+-rw-rw-rw-   0        0        0     1574 2024-05-06 14:13:39.000000 dash_draggable_no_console_logs-0.0.2/dash_draggable_no_console_logs/DashDraggable2.py
+-rw-rw-rw-   0        0        0     1840 2024-05-06 14:13:39.000000 dash_draggable_no_console_logs-0.0.2/dash_draggable_no_console_logs/DashDraggableResponsive.py
+-rw-rw-rw-   0        0        0     2940 2024-05-06 14:13:39.000000 dash_draggable_no_console_logs-0.0.2/dash_draggable_no_console_logs/DashboardItem.py
+-rw-rw-rw-   0        0        0     3355 2024-05-06 14:13:39.000000 dash_draggable_no_console_logs-0.0.2/dash_draggable_no_console_logs/DashboardItemResponsive.py
+-rw-rw-rw-   0        0        0     3202 2024-05-06 14:13:39.000000 dash_draggable_no_console_logs-0.0.2/dash_draggable_no_console_logs/DragItem.py
+-rw-rw-rw-   0        0        0     3842 2024-05-06 14:13:39.000000 dash_draggable_no_console_logs-0.0.2/dash_draggable_no_console_logs/DraggableDashboard.py
+-rw-rw-rw-   0        0        0     4421 2024-05-06 14:13:39.000000 dash_draggable_no_console_logs-0.0.2/dash_draggable_no_console_logs/DraggableDashboardResponsive.py
+-rw-rw-rw-   0        0        0     5682 2024-05-06 14:13:39.000000 dash_draggable_no_console_logs-0.0.2/dash_draggable_no_console_logs/GridLayout.py
+-rw-rw-rw-   0        0        0     6144 2024-05-06 14:13:39.000000 dash_draggable_no_console_logs-0.0.2/dash_draggable_no_console_logs/ResponsiveGridLayout.py
+-rw-rw-rw-   0        0        0     1315 2024-05-06 14:13:39.000000 dash_draggable_no_console_logs-0.0.2/dash_draggable_no_console_logs/__init__.py
+-rw-rw-rw-   0        0        0      501 2024-05-06 14:13:39.000000 dash_draggable_no_console_logs-0.0.2/dash_draggable_no_console_logs/_imports_.py
+-rw-rw-rw-   0        0        0     5730 2024-05-06 14:55:36.000000 dash_draggable_no_console_logs-0.0.2/dash_draggable_no_console_logs/demo.py
+-rw-rw-rw-   0        0        0     1982 2024-05-06 14:13:39.000000 dash_draggable_no_console_logs-0.0.2/dash_draggable_no_console_logs/test.py
+drwxrwxrwx   0        0        0        0 2024-05-06 15:05:26.262507 dash_draggable_no_console_logs-0.0.2/dash_draggable_no_console_logs.egg-info/
+-rw-rw-rw-   0        0        0      313 2024-05-06 15:05:25.000000 dash_draggable_no_console_logs-0.0.2/dash_draggable_no_console_logs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      972 2024-05-06 15:05:25.000000 dash_draggable_no_console_logs-0.0.2/dash_draggable_no_console_logs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 15:05:25.000000 dash_draggable_no_console_logs-0.0.2/dash_draggable_no_console_logs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-06 15:05:25.000000 dash_draggable_no_console_logs-0.0.2/dash_draggable_no_console_logs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2087 2024-05-06 15:05:13.000000 dash_draggable_no_console_logs-0.0.2/package.json
+-rw-rw-rw-   0        0        0       42 2024-05-06 15:05:26.276505 dash_draggable_no_console_logs-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      533 2024-05-06 15:05:18.000000 dash_draggable_no_console_logs-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 15:05:26.266504 dash_draggable_no_console_logs-0.0.2/tests/
+-rw-rw-rw-   0        0        0      945 2024-05-06 14:13:40.000000 dash_draggable_no_console_logs-0.0.2/tests/test_usage.py
```

### Comparing `dash_draggable_no_console_logs-0.0.1/LICENSE` & `dash_draggable_no_console_logs-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dash_draggable_no_console_logs-0.0.1/README.md` & `dash_draggable_no_console_logs-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dash_draggable_no_console_logs-0.0.1/dash_draggable_no_console_logs/DashDraggable.py` & `dash_draggable_no_console_logs-0.0.2/dash_draggable_no_console_logs/DashDraggable.py`

 * *Files identical despite different names*

### Comparing `dash_draggable_no_console_logs-0.0.1/dash_draggable_no_console_logs/DashDraggable2.py` & `dash_draggable_no_console_logs-0.0.2/dash_draggable_no_console_logs/DashDraggable2.py`

 * *Files identical despite different names*

### Comparing `dash_draggable_no_console_logs-0.0.1/dash_draggable_no_console_logs/DashDraggableResponsive.py` & `dash_draggable_no_console_logs-0.0.2/dash_draggable_no_console_logs/DashDraggableResponsive.py`

 * *Files identical despite different names*

### Comparing `dash_draggable_no_console_logs-0.0.1/dash_draggable_no_console_logs/DashboardItem.py` & `dash_draggable_no_console_logs-0.0.2/dash_draggable_no_console_logs/DashboardItem.py`

 * *Files identical despite different names*

### Comparing `dash_draggable_no_console_logs-0.0.1/dash_draggable_no_console_logs/DashboardItemResponsive.py` & `dash_draggable_no_console_logs-0.0.2/dash_draggable_no_console_logs/DashboardItemResponsive.py`

 * *Files identical despite different names*

### Comparing `dash_draggable_no_console_logs-0.0.1/dash_draggable_no_console_logs/DragItem.py` & `dash_draggable_no_console_logs-0.0.2/dash_draggable_no_console_logs/DragItem.py`

 * *Files identical despite different names*

### Comparing `dash_draggable_no_console_logs-0.0.1/dash_draggable_no_console_logs/DraggableDashboard.py` & `dash_draggable_no_console_logs-0.0.2/dash_draggable_no_console_logs/DraggableDashboard.py`

 * *Files identical despite different names*

### Comparing `dash_draggable_no_console_logs-0.0.1/dash_draggable_no_console_logs/DraggableDashboardResponsive.py` & `dash_draggable_no_console_logs-0.0.2/dash_draggable_no_console_logs/DraggableDashboardResponsive.py`

 * *Files identical despite different names*

### Comparing `dash_draggable_no_console_logs-0.0.1/dash_draggable_no_console_logs/GridLayout.py` & `dash_draggable_no_console_logs-0.0.2/dash_draggable_no_console_logs/GridLayout.py`

 * *Files identical despite different names*

### Comparing `dash_draggable_no_console_logs-0.0.1/dash_draggable_no_console_logs/ResponsiveGridLayout.py` & `dash_draggable_no_console_logs-0.0.2/dash_draggable_no_console_logs/ResponsiveGridLayout.py`

 * *Files identical despite different names*

### Comparing `dash_draggable_no_console_logs-0.0.1/dash_draggable_no_console_logs/__init__.py` & `dash_draggable_no_console_logs-0.0.2/dash_draggable_no_console_logs/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_draggable_no_console_logs-0.0.1/dash_draggable_no_console_logs/demo.py` & `dash_draggable_no_console_logs-0.0.2/dash_draggable_no_console_logs/demo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import dash_draggable
+import dash_draggable_no_console_logs
 import dash
 from dash.dependencies import Input, Output, State
 from dash.exceptions import PreventUpdate
 import dash_core_components as dcc
 import dash_html_components as html
 import plotly.express as px
 import pandas as pd
@@ -16,15 +16,15 @@
     dcc.Store(id='memory-output', storage_type='local'),
     dcc.Store(id='local', storage_type='local'),
     # Same as the local store but will lose the data
     # when the browser/tab closes.
     dcc.Store(id='session', storage_type='session'),
     html.Div(id='placeholder'),
     html.Button(id="test-btn"),
-    dash_draggable.DashDraggable(
+    dash_draggable_no_console_logs.DashDraggable(
         id='draggable',
         children=[
             "jijijj",
             dcc.Graph(
                 id='graph-with-slider',
                 responsive=True,
                 style=dict(height='100%', width='100%')),
@@ -32,15 +32,15 @@
                 id='year-slider',
                 min=df['year'].min(),
                 max=df['year'].max(),
                 value=df['year'].min(),
                 marks={str(year): str(year) for year in df['year'].unique()},
                 step=None
             ),
-            dash_draggable.DashDraggable(
+            dash_draggable_no_console_logs.DashDraggable(
                 id='draggableee',
                 children=[
                     "jijijj",
                     dcc.Graph(
                         id='graph-with-sliderrr',
                         responsive=True,
                         style=dict(height='100%', width='100%')),
```

### Comparing `dash_draggable_no_console_logs-0.0.1/dash_draggable_no_console_logs/test.py` & `dash_draggable_no_console_logs-0.0.2/dash_draggable_no_console_logs/test.py`

 * *Files identical despite different names*

### Comparing `dash_draggable_no_console_logs-0.0.1/dash_draggable_no_console_logs.egg-info/SOURCES.txt` & `dash_draggable_no_console_logs-0.0.2/dash_draggable_no_console_logs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dash_draggable_no_console_logs-0.0.1/package.json` & `dash_draggable_no_console_logs-0.0.2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.0.2'"}*

```diff
@@ -50,9 +50,9 @@
         "build:js": "webpack --mode production",
         "build:py_and_r": "dash-generate-components ./src/lib/components dash_draggable -p package-info.json --r-prefix '' --jl-prefix ''",
         "build:py_and_r-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack-serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.0.1"
+    "version": "0.0.2"
 }
```

### Comparing `dash_draggable_no_console_logs-0.0.1/setup.py` & `dash_draggable_no_console_logs-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `dash_draggable_no_console_logs-0.0.1/tests/test_usage.py` & `dash_draggable_no_console_logs-0.0.2/tests/test_usage.py`

 * *Files identical despite different names*

