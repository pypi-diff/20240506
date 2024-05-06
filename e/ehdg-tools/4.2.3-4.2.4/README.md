# Comparing `tmp/ehdg_tools-4.2.3.tar.gz` & `tmp/ehdg_tools-4.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ehdg_tools-4.2.3.tar", last modified: Tue Apr 23 22:51:29 2024, max compression
+gzip compressed data, was "ehdg_tools-4.2.4.tar", last modified: Sun May  5 09:36:40 2024, max compression
```

## Comparing `ehdg_tools-4.2.3.tar` & `ehdg_tools-4.2.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 22:51:29.959441 ehdg_tools-4.2.3/
--rw-rw-rw-   0        0        0    11558 2023-11-17 13:32:14.000000 ehdg_tools-4.2.3/LICENSE
--rw-rw-rw-   0        0        0     3001 2024-04-23 22:51:29.958444 ehdg_tools-4.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     2436 2023-11-22 03:02:06.000000 ehdg_tools-4.2.3/README.md
--rw-rw-rw-   0        0        0      699 2024-04-23 22:49:55.000000 ehdg_tools-4.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-23 22:51:29.959441 ehdg_tools-4.2.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-23 22:51:29.934505 ehdg_tools-4.2.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-23 22:51:29.942484 ehdg_tools-4.2.3/src/ehdg_tools/
--rw-rw-rw-   0        0        0        0 2023-11-05 22:27:51.000000 ehdg_tools-4.2.3/src/ehdg_tools/__init__.py
--rw-rw-rw-   0        0        0     4730 2023-11-21 22:16:22.000000 ehdg_tools-4.2.3/src/ehdg_tools/ehdg_buffers.py
--rw-rw-rw-   0        0        0     6970 2024-04-23 22:48:47.000000 ehdg_tools-4.2.3/src/ehdg_tools/ehdg_functions.py
--rw-rw-rw-   0        0        0     5831 2024-01-30 22:28:51.000000 ehdg_tools-4.2.3/src/ehdg_tools/ehdg_okn_checker.py
--rw-rw-rw-   0        0        0   117333 2024-04-17 02:32:38.000000 ehdg_tools-4.2.3/src/ehdg_tools/ehdg_plotter.py
--rw-rw-rw-   0        0        0    13490 2023-11-29 22:43:57.000000 ehdg_tools-4.2.3/src/ehdg_tools/ehdg_updater.py
-drwxrwxrwx   0        0        0        0 2024-04-23 22:51:29.957446 ehdg_tools-4.2.3/src/ehdg_tools.egg-info/
--rw-rw-rw-   0        0        0     3001 2024-04-23 22:51:29.000000 ehdg_tools-4.2.3/src/ehdg_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2024-04-23 22:51:29.000000 ehdg_tools-4.2.3/src/ehdg_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 22:51:29.000000 ehdg_tools-4.2.3/src/ehdg_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-23 22:51:29.000000 ehdg_tools-4.2.3/src/ehdg_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-05 09:36:40.026301 ehdg_tools-4.2.4/
+-rw-rw-rw-   0        0        0    11558 2023-11-17 13:32:14.000000 ehdg_tools-4.2.4/LICENSE
+-rw-rw-rw-   0        0        0     3001 2024-05-05 09:36:40.025304 ehdg_tools-4.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2436 2023-11-22 03:02:06.000000 ehdg_tools-4.2.4/README.md
+-rw-rw-rw-   0        0        0      699 2024-05-05 08:49:10.000000 ehdg_tools-4.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-05 09:36:40.026301 ehdg_tools-4.2.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-05 09:36:39.998376 ehdg_tools-4.2.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-05 09:36:40.009347 ehdg_tools-4.2.4/src/ehdg_tools/
+-rw-rw-rw-   0        0        0        0 2023-11-05 22:27:51.000000 ehdg_tools-4.2.4/src/ehdg_tools/__init__.py
+-rw-rw-rw-   0        0        0     4730 2023-11-21 22:16:22.000000 ehdg_tools-4.2.4/src/ehdg_tools/ehdg_buffers.py
+-rw-rw-rw-   0        0        0     6970 2024-04-23 22:48:47.000000 ehdg_tools-4.2.4/src/ehdg_tools/ehdg_functions.py
+-rw-rw-rw-   0        0        0     5831 2024-01-30 22:28:51.000000 ehdg_tools-4.2.4/src/ehdg_tools/ehdg_okn_checker.py
+-rw-rw-rw-   0        0        0   117322 2024-05-05 09:31:23.000000 ehdg_tools-4.2.4/src/ehdg_tools/ehdg_plotter.py
+-rw-rw-rw-   0        0        0    13490 2023-11-29 22:43:57.000000 ehdg_tools-4.2.4/src/ehdg_tools/ehdg_updater.py
+drwxrwxrwx   0        0        0        0 2024-05-05 09:36:40.023309 ehdg_tools-4.2.4/src/ehdg_tools.egg-info/
+-rw-rw-rw-   0        0        0     3001 2024-05-05 09:36:39.000000 ehdg_tools-4.2.4/src/ehdg_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2024-05-05 09:36:39.000000 ehdg_tools-4.2.4/src/ehdg_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 09:36:39.000000 ehdg_tools-4.2.4/src/ehdg_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-05 09:36:39.000000 ehdg_tools-4.2.4/src/ehdg_tools.egg-info/top_level.txt
```

### Comparing `ehdg_tools-4.2.3/LICENSE` & `ehdg_tools-4.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ehdg_tools-4.2.3/PKG-INFO` & `ehdg_tools-4.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehdg_tools
-Version: 4.2.3
+Version: 4.2.4
 Summary: Python library useful tools for ABI Eye Health Diagnostic Group
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/ZawLinTun16925410/ehdg_tools
 Project-URL: Bug Tracker, https://github.com/ZawLinTun16925410/ehdg_tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `ehdg_tools-4.2.3/README.md` & `ehdg_tools-4.2.4/README.md`

 * *Files identical despite different names*

### Comparing `ehdg_tools-4.2.3/pyproject.toml` & `ehdg_tools-4.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ehdg_tools"
-version = "4.2.3"
+version = "4.2.4"
 authors = [
   { name="Zaw Lin Tun", email="zawlintun1511@gmail.com" },
 ]
 description = "Python library useful tools for ABI Eye Health Diagnostic Group"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `ehdg_tools-4.2.3/src/ehdg_tools/ehdg_buffers.py` & `ehdg_tools-4.2.4/src/ehdg_tools/ehdg_buffers.py`

 * *Files identical despite different names*

### Comparing `ehdg_tools-4.2.3/src/ehdg_tools/ehdg_functions.py` & `ehdg_tools-4.2.4/src/ehdg_tools/ehdg_functions.py`

 * *Files identical despite different names*

### Comparing `ehdg_tools-4.2.3/src/ehdg_tools/ehdg_okn_checker.py` & `ehdg_tools-4.2.4/src/ehdg_tools/ehdg_okn_checker.py`

 * *Files identical despite different names*

### Comparing `ehdg_tools-4.2.3/src/ehdg_tools/ehdg_plotter.py` & `ehdg_tools-4.2.4/src/ehdg_tools/ehdg_plotter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1326,21 +1326,20 @@
 
 # This function is to draw va testing progress graph from the given config info
 def progress_plot(folder_dir_input, progress_plot_info_input, output_dir_input=None, image_name=None):
     x_label = progress_plot_info_input["x_label"]
     y_label = progress_plot_info_input["y_label"]
     x_data_column_name = progress_plot_info_input["x_data_column_name"]
     y_data_column_name = progress_plot_info_input["y_data_column_name"]
-    okn_matlab_column_name = progress_plot_info_input["okn_matlab_column_name"]
+    okn_column_name = progress_plot_info_input["okn_column_name"]
     phase_column_name = progress_plot_info_input["phase_column_name"]
     final_logmar_column_name = progress_plot_info_input["final_logmar_column_name"]
     graph_line_color = progress_plot_info_input["graph_line_color"]
     graph_line_thickness = progress_plot_info_input["graph_line_thickness"]
     graph_line_style = progress_plot_info_input["graph_line_style"]
-    summary_csv_name = progress_plot_info_input["summary_csv_name"]
     trial_summary_csv_name = progress_plot_info_input["trial_summary_csv_name"]
     output_image_name = progress_plot_info_input["output_image_name"]
     marker_type_equivalent = progress_plot_info_input["marker_type_equivalent"]
     marker_type = progress_plot_info_input["marker_type"]
     marker_size = progress_plot_info_input["marker_size"]
     okn_marker_color = progress_plot_info_input["okn_marker_color"]
     okn_marker_edge_color = progress_plot_info_input["okn_marker_edge_color"]
@@ -1361,46 +1360,44 @@
     legend_background_color = progress_plot_info_input["legend_background_color"]
     legend_edge_color = progress_plot_info_input["legend_edge_color"]
     legend_location = progress_plot_info_input["legend_location"]
     legend_font_size = progress_plot_info_input["legend_font_size"]
     legend_icon_size = progress_plot_info_input["legend_icon_size"]
     line_style_equivalent = progress_plot_info_input["line_style_equivalent"]
 
-    summary_csv_dir = os.path.join(folder_dir_input, summary_csv_name)
-
     trial_data_csv_dir = os.path.join(folder_dir_input, trial_summary_csv_name)
 
     if output_dir_input:
         output_dir = output_dir_input
         if image_name is not None:
             output_image_name = image_name
     else:
         output_dir = folder_dir_input
 
     display_output_dir = os.path.join(output_dir, output_image_name)
 
     try:
-        file_to_open = open(summary_csv_dir)
+        file_to_open = open(trial_data_csv_dir)
         csv_reader = csv.reader(file_to_open)
         header_array = []
         rows = []
         count_one = 0
 
         for row in csv_reader:
             if count_one <= 0:
                 header_array = row
                 count_one += 1
             else:
                 rows.append(row)
 
         x_header_position = get_index(x_data_column_name, header_array)
         y_header_position = get_index(y_data_column_name, header_array)
-        okn_header_position = get_index(okn_matlab_column_name, header_array)
+        okn_header_position = get_index(okn_column_name, header_array)
     except FileNotFoundError:
-        print(f"{summary_csv_dir} could not be found.")
+        print(f"{trial_data_csv_dir} could not be found.")
         rows = []
         x_header_position = None
         y_header_position = None
         okn_header_position = None
 
     # print(x_header_position)
     # print(y_header_position)
@@ -1408,29 +1405,29 @@
     y_array = []
     okn_array = []
     x_index_array = []
 
     if len(rows) > 0:
         for row in rows:
             x_array.append(row[x_header_position])
-            y_array.append(float(row[y_header_position]))
-            okn_array.append(int(float(row[okn_header_position])))
+            y_array.append(disk_to_logmar(str(row[y_header_position])))
+            okn_array.append(str(row[okn_header_position]))
 
         for ind in range(len(x_array)):
             x_index_array.append(str(ind + 1))
 
         # print(x_array)
         # print(y_array)
         # print(okn_array)
         overlay_x_array = []
         overlay_y_array = []
         # final_va_line_level = y_array[-1]
 
         for ind, value in enumerate(okn_array):
-            if value >= 1:
+            if value.lower() == "true" or value.lower() == "1":
                 overlay_x_array.append(x_index_array[ind])
                 overlay_y_array.append(y_array[ind])
 
         bot_limit = min(y_array) - 0.2
         top_limit = max(y_array) + 0.1
 
         plt.plot(x_index_array, y_array, line_style_equivalent[graph_line_style],
@@ -1499,15 +1496,15 @@
         frame.set_alpha(1)
         os.chdir(output_dir)
         plt.savefig(output_image_name)
         # plt.show()
         plt.close()
         print(f"Staircase/progress plot has been saved at:{display_output_dir}")
     else:
-        print(f"There is no data in {summary_csv_dir} or it does not exist.")
+        print(f"There is no data in {trial_summary_csv_name} or it does not exist.")
 
 
 # This function is to produce x and y adjustment limits according the type of adjustment
 # Type comes into the function as int number and is converted into string to be used
 # to retrieve the string type from adjustment dictionary
 def get_adjust_limit(data_dir_input, csv_name, x_header_input, y_header_input, folder_array_input,
                      x_axis_limit_input, y_axis_limit_input, mean_offset_input,
@@ -1696,14 +1693,16 @@
         rows = []
         phase_header_position = None
         final_logmar_header_position = None
 
     va_output = None
 
     if len(rows) > 0:
+        last_row = rows[-1]
+        va_output = float(last_row[final_logmar_header_position])
         for row in rows:
             if row[phase_header_position] == phase_name_input:
                 va_output = float(row[final_logmar_header_position])
     else:
         print(f"There is no data in {csv_dir_input} or it does not exist.")
 
     return va_output
```

### Comparing `ehdg_tools-4.2.3/src/ehdg_tools/ehdg_updater.py` & `ehdg_tools-4.2.4/src/ehdg_tools/ehdg_updater.py`

 * *Files identical despite different names*

### Comparing `ehdg_tools-4.2.3/src/ehdg_tools.egg-info/PKG-INFO` & `ehdg_tools-4.2.4/src/ehdg_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehdg_tools
-Version: 4.2.3
+Version: 4.2.4
 Summary: Python library useful tools for ABI Eye Health Diagnostic Group
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/ZawLinTun16925410/ehdg_tools
 Project-URL: Bug Tracker, https://github.com/ZawLinTun16925410/ehdg_tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

